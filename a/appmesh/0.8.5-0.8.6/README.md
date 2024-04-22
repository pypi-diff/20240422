# Comparing `tmp/appmesh-0.8.5-py3-none-any.whl.zip` & `tmp/appmesh-0.8.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 15369 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-20 02:07 appmesh/__init__.py
--rw-r--r--  2.0 unx    55928 b- defN 24-Apr-20 02:07 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10786 b- defN 24-Apr-20 02:07 appmesh-0.8.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-20 02:07 appmesh-0.8.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-20 02:07 appmesh-0.8.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-Apr-20 02:07 appmesh-0.8.5.dist-info/RECORD
-6 files, 67280 bytes uncompressed, 14547 bytes compressed:  78.4%
+Zip file size: 15674 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-22 04:36 appmesh/__init__.py
+-rw-r--r--  2.0 unx    57114 b- defN 24-Apr-22 04:36 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-Apr-22 04:36 appmesh-0.8.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 04:36 appmesh-0.8.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-22 04:36 appmesh-0.8.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-Apr-22 04:36 appmesh-0.8.6.dist-info/RECORD
+6 files, 68466 bytes uncompressed, 14852 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-0.8.5.dist-info/METADATA
+Filename: appmesh-0.8.6.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-0.8.5.dist-info/WHEEL
+Filename: appmesh-0.8.6.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-0.8.5.dist-info/top_level.txt
+Filename: appmesh-0.8.6.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-0.8.5.dist-info/RECORD
+Filename: appmesh-0.8.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -411,14 +411,79 @@
             if "Access-Token" in resp.json():
                 self.jwt_token = resp.json()["Access-Token"]
         else:
             print(resp.text)
             # resp.raise_for_status()
         return self.jwt_token
 
+    def totp_secret(self) -> str:
+        """Generate TOTP key for current login user and return MFA URI with JSON body
+
+        Returns:
+            str: TOTP secret str
+        """
+        resp = self._request_http(method=AppMeshClient.Method.POST, path="/appmesh/totp/secret")
+        if resp.status_code == HTTPStatus.OK:
+            totp_uri = base64.b64decode(resp.json()["Mfa-Uri"]).decode()
+            return self._parse_totp_uri(totp_uri).get("secret")
+        else:
+            print(resp.text)
+            # resp.raise_for_status()
+        return None
+
+    def totp_setup(self, totp_key: str) -> bool:
+        """Setup 2FA for current login user
+
+        Args:
+            totp_key (str): TOTP key
+
+        Returns:
+            bool: success or failure.
+        """
+        resp = self._request_http(
+            method=AppMeshClient.Method.POST,
+            path=f"/appmesh/totp/setup",
+            header={"Totp": base64.b64encode(totp_key.encode())},
+        )
+        return resp.status_code == HTTPStatus.OK
+
+    def totp_disable(self) -> bool:
+        """Disable 2FA for current user
+
+        Returns:
+            bool: success or failure.
+        """
+        resp = self._request_http(
+            method=AppMeshClient.Method.POST,
+            path=f"/appmesh/totp/disable",
+        )
+        return resp.status_code == HTTPStatus.OK
+
+    @staticmethod
+    def _parse_totp_uri(totp_uri: str) -> dict:
+        """Extract TOTP parameters
+
+        Args:
+            totp_uri (str): TOTP uri
+
+        Returns:
+            dict: eextract parameters
+        """
+        parsed_info = {}
+        parsed_uri = parse.urlparse(totp_uri)
+
+        # Extract label from the path
+        parsed_info["label"] = parsed_uri.path[1:]  # Remove the leading slash
+
+        # Extract parameters from the query string
+        query_params = parse.parse_qs(parsed_uri.query)
+        for key, value in query_params.items():
+            parsed_info[key] = value[0]
+        return parsed_info
+
     ########################################
     # Application view
     ########################################
     def app_view(self, app_name: str) -> App:
         """Get one application information
 
         Args:
@@ -780,41 +845,14 @@
         """
         resp = self._request_http(
             method=AppMeshClient.Method.POST,
             path=f"/appmesh/user/{user_name}/unlock",
         )
         return resp.status_code == HTTPStatus.OK
 
-    def user_2fa_active(self) -> bool:
-        """Active 2FA for current login user and return MFA URI with JSON body
-
-        Returns:
-            bool: success or failure.
-        """
-        resp = self._request_http(
-            method=AppMeshClient.Method.POST,
-            path="/appmesh/user/self/mfa",
-        )
-        return resp.status_code == HTTPStatus.OK
-
-    def user_2fa_deactive(self, user_name: str = "self") -> bool:
-        """DeActive 2FA for a user
-
-        Args:
-            user_name (str, optional): the user name.
-
-        Returns:
-            bool: success or failure.
-        """
-        resp = self._request_http(
-            method=AppMeshClient.Method.DELETE,
-            path=f"/appmesh/user/{user_name}/mfa",
-        )
-        return resp.status_code == HTTPStatus.OK
-
     def users_view(self):
         """Get all users
 
         Returns:
             bool: success or failure.
             dict: all user definition.
         """
```

## Comparing `appmesh-0.8.5.dist-info/METADATA` & `appmesh-0.8.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 0.8.5
+Version: 0.8.6
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 0.8.5 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 0.8.6 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```


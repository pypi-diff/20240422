# Comparing `tmp/gy-erp-sdk-core-0.0.3.tar.gz` & `tmp/gy-erp-sdk-core-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gy-erp-sdk-core-0.0.3.tar", last modified: Mon Aug 23 05:47:57 2021, max compression
+gzip compressed data, was "gy-erp-sdk-core-0.0.4.tar", last modified: Mon Apr 22 02:38:47 2024, max compression
```

## Comparing `gy-erp-sdk-core-0.0.3.tar` & `gy-erp-sdk-core-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 steven     (501) staff       (20)        0 2021-08-23 05:47:57.000000 gy-erp-sdk-core-0.0.3/
--rw-r--r--   0 steven     (501) staff       (20)      840 2021-08-23 05:47:57.000000 gy-erp-sdk-core-0.0.3/PKG-INFO
--rw-r--r--   0 steven     (501) staff       (20)      449 2021-08-20 07:31:48.000000 gy-erp-sdk-core-0.0.3/README.md
-drwxr-xr-x   0 steven     (501) staff       (20)        0 2021-08-23 05:47:57.000000 gy-erp-sdk-core-0.0.3/gy_erp_sdk_core.egg-info/
--rw-r--r--   0 steven     (501) staff       (20)      840 2021-08-23 05:47:57.000000 gy-erp-sdk-core-0.0.3/gy_erp_sdk_core.egg-info/PKG-INFO
--rw-r--r--   0 steven     (501) staff       (20)      364 2021-08-23 05:47:57.000000 gy-erp-sdk-core-0.0.3/gy_erp_sdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 steven     (501) staff       (20)        1 2021-08-23 05:47:57.000000 gy-erp-sdk-core-0.0.3/gy_erp_sdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 steven     (501) staff       (20)       13 2021-08-23 05:47:57.000000 gy-erp-sdk-core-0.0.3/gy_erp_sdk_core.egg-info/top_level.txt
-drwxr-xr-x   0 steven     (501) staff       (20)        0 2021-08-23 05:47:57.000000 gy-erp-sdk-core-0.0.3/gyerpsdkcore/
--rw-r--r--   0 steven     (501) staff       (20)      107 2021-08-23 05:47:29.000000 gy-erp-sdk-core-0.0.3/gyerpsdkcore/__init__.py
-drwxr-xr-x   0 steven     (501) staff       (20)        0 2021-08-23 05:47:57.000000 gy-erp-sdk-core-0.0.3/gyerpsdkcore/api/
--rw-r--r--   0 steven     (501) staff       (20)       80 2021-08-20 02:18:31.000000 gy-erp-sdk-core-0.0.3/gyerpsdkcore/api/__init__.py
--rw-r--r--   0 steven     (501) staff       (20)      751 2021-08-23 02:06:19.000000 gy-erp-sdk-core-0.0.3/gyerpsdkcore/api/base.py
--rw-r--r--   0 steven     (501) staff       (20)      171 2021-07-16 07:36:46.000000 gy-erp-sdk-core-0.0.3/gyerpsdkcore/api/item.py
--rw-r--r--   0 steven     (501) staff       (20)      473 2021-08-20 10:00:32.000000 gy-erp-sdk-core-0.0.3/gyerpsdkcore/api/trade.py
-drwxr-xr-x   0 steven     (501) staff       (20)        0 2021-08-23 05:47:57.000000 gy-erp-sdk-core-0.0.3/gyerpsdkcore/client/
--rw-r--r--   0 steven     (501) staff       (20)      343 2021-08-20 02:27:27.000000 gy-erp-sdk-core-0.0.3/gyerpsdkcore/client/__init__.py
--rw-r--r--   0 steven     (501) staff       (20)     1901 2021-08-23 05:47:14.000000 gy-erp-sdk-core-0.0.3/gyerpsdkcore/client/base.py
--rw-r--r--   0 steven     (501) staff       (20)       38 2021-08-23 05:47:57.000000 gy-erp-sdk-core-0.0.3/setup.cfg
--rw-r--r--   0 steven     (501) staff       (20)      820 2021-08-20 07:34:38.000000 gy-erp-sdk-core-0.0.3/setup.py
+drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:38:47.403409 gy-erp-sdk-core-0.0.4/
+-rw-r--r--   0 zty        (501) staff       (20)      889 2024-04-22 02:38:47.403113 gy-erp-sdk-core-0.0.4/PKG-INFO
+-rw-r--r--   0 zty        (501) staff       (20)      490 2024-04-19 09:51:51.000000 gy-erp-sdk-core-0.0.4/README.md
+drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:38:47.396516 gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/
+-rw-r--r--   0 zty        (501) staff       (20)      889 2024-04-22 02:38:47.000000 gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 zty        (501) staff       (20)      394 2024-04-22 02:38:47.000000 gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 zty        (501) staff       (20)        1 2024-04-22 02:38:47.000000 gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 zty        (501) staff       (20)       13 2024-04-22 02:38:47.000000 gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/top_level.txt
+drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:38:47.396856 gy-erp-sdk-core-0.0.4/gyerpsdkcore/
+-rw-r--r--   0 zty        (501) staff       (20)      107 2024-04-22 02:34:37.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/__init__.py
+drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:38:47.400642 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/
+-rw-r--r--   0 zty        (501) staff       (20)       80 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/__init__.py
+-rw-r--r--   0 zty        (501) staff       (20)      663 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/base.py
+-rw-r--r--   0 zty        (501) staff       (20)      171 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/item.py
+-rw-r--r--   0 zty        (501) staff       (20)      333 2024-04-19 09:51:26.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/new_stock.py
+-rw-r--r--   0 zty        (501) staff       (20)      464 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/trade.py
+drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:38:47.402501 gy-erp-sdk-core-0.0.4/gyerpsdkcore/client/
+-rw-r--r--   0 zty        (501) staff       (20)      343 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/client/__init__.py
+-rw-r--r--   0 zty        (501) staff       (20)     1908 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/client/base.py
+-rw-r--r--   0 zty        (501) staff       (20)       38 2024-04-22 02:38:47.403533 gy-erp-sdk-core-0.0.4/setup.cfg
+-rw-r--r--   0 zty        (501) staff       (20)      820 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gy-erp-sdk-core-0.0.3/PKG-INFO` & `gy-erp-sdk-core-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 1.2
 Name: gy-erp-sdk-core
-Version: 0.0.3
+Version: 0.0.4
 Summary: gy erp api Python sdk.
 Home-page: https://github.com/stevenQiang
 Author: Steven
 Author-email: qianggao7@gmail.com
 License: cc
 Description: # gy-erp-sdk-core
         
         ## Introduction
         针对管易云erp系统，相关接口对接，单独打成一个三方包，方便使用。
         
         ## Method
         - 订单查询（**gy.erp.trade.get**）
         - 订单新增（**gy.erp.trade.add**）
         - 订单退款状态修改（**gy.erp.trade.refund.update**）
+        - 新库存查询 (**gy.erp.new.stock**)
         
         ## Remark
         * 目前根据业务需求，只需要trade和item，所以只加入了这两个，有需求后面在加。
         
         ## Require
         * python version 3.0 and greater
```

### Comparing `gy-erp-sdk-core-0.0.3/gy_erp_sdk_core.egg-info/PKG-INFO` & `gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 1.2
 Name: gy-erp-sdk-core
-Version: 0.0.3
+Version: 0.0.4
 Summary: gy erp api Python sdk.
 Home-page: https://github.com/stevenQiang
 Author: Steven
 Author-email: qianggao7@gmail.com
 License: cc
 Description: # gy-erp-sdk-core
         
         ## Introduction
         针对管易云erp系统，相关接口对接，单独打成一个三方包，方便使用。
         
         ## Method
         - 订单查询（**gy.erp.trade.get**）
         - 订单新增（**gy.erp.trade.add**）
         - 订单退款状态修改（**gy.erp.trade.refund.update**）
+        - 新库存查询 (**gy.erp.new.stock**)
         
         ## Remark
         * 目前根据业务需求，只需要trade和item，所以只加入了这两个，有需求后面在加。
         
         ## Require
         * python version 3.0 and greater
```

### Comparing `gy-erp-sdk-core-0.0.3/gyerpsdkcore/client/base.py` & `gy-erp-sdk-core-0.0.4/gyerpsdkcore/client/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,34 +34,39 @@
         assert self.appKey is not None
         assert self.sessionKey is not None
         assert self.secretKey is not None
 
     def _post(self, **kwargs):
         return self.post(**kwargs)
 
-    def post(self, params):
-        return self._request(http_method='post', params=params)
+    def post(self, **kwargs):
+        return self._request(http_method='post', **kwargs)
 
     def _get(self, **kwargs):
         return self.get(**kwargs)
 
-    def get(self, params):
+    def get(self, **kwargs):
         return self._request(
-            http_method='get',
-            params=params
+            method='get',
+            **kwargs
         )
 
-    def _request(self, http_method, params):
+    def _request(self, http_method, **kwargs):
         res = self._http.request(
             method=http_method,
             url=self.API_BASE_URL,
             headers={'Content-Type': 'application/json'},
-            json=params
+            json=kwargs
         )
-        return res.json()
+        print(res.text)
 
     def encrypt_by_MD5(self, params):
         # json转str，要注意空格，所以不能用str()直接转
-        key = self.secretKey + json.dumps(params, separators=(',',':'), ensure_ascii=False) + self.secretKey
-        signCode = hashlib.md5(key.encode("utf-8")).hexdigest().upper()
-        return signCode
+        key = self.secretKey + json.dumps(params, separators=(',',':')) + self.secretKey
+        input_name = hashlib.md5()
+        input_name.update(key.encode("utf-8"))
+        return (input_name.hexdigest()).upper()
+
+
+
+
```

### Comparing `gy-erp-sdk-core-0.0.3/setup.py` & `gy-erp-sdk-core-0.0.4/setup.py`

 * *Files identical despite different names*


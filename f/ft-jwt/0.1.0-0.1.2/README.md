# Comparing `tmp/ft_jwt-0.1.0.tar.gz` & `tmp/ft_jwt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ft_jwt-0.1.0.tar", last modified: Fri Apr 19 11:40:25 2024, max compression
+gzip compressed data, was "ft_jwt-0.1.2.tar", last modified: Mon Apr 22 08:57:35 2024, max compression
```

## Comparing `ft_jwt-0.1.0.tar` & `ft_jwt-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-19 11:40:25.000000 ft_jwt-0.1.0/
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-19 11:40:24.000000 ft_jwt-0.1.0/ft_jwt/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-15 07:40:53.000000 ft_jwt-0.1.0/ft_jwt/__init__.py
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     3963 2024-04-18 16:42:29.000000 ft_jwt-0.1.0/ft_jwt/ft_jwt.py
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-19 11:40:25.000000 ft_jwt-0.1.0/ft_jwt.egg-info/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-19 11:40:24.000000 ft_jwt-0.1.0/ft_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     2697 2024-04-19 11:40:24.000000 ft_jwt-0.1.0/ft_jwt.egg-info/PKG-INFO
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      174 2024-04-19 11:40:24.000000 ft_jwt-0.1.0/ft_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        7 2024-04-19 11:40:24.000000 ft_jwt-0.1.0/ft_jwt.egg-info/top_level.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     2697 2024-04-19 11:40:25.000000 ft_jwt-0.1.0/PKG-INFO
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1585 2024-04-19 11:40:18.000000 ft_jwt-0.1.0/README.md
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       38 2024-04-19 11:40:25.000000 ft_jwt-0.1.0/setup.cfg
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      724 2024-04-19 11:38:14.000000 ft_jwt-0.1.0/setup.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-22 08:57:35.000000 ft_jwt-0.1.2/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1063 2024-04-15 07:40:53.000000 ft_jwt-0.1.2/LICENSE
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     2193 2024-04-22 08:57:35.000000 ft_jwt-0.1.2/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1626 2024-04-22 08:57:28.000000 ft_jwt-0.1.2/README.md
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-22 08:57:35.000000 ft_jwt-0.1.2/ft_jwt/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-15 07:40:53.000000 ft_jwt-0.1.2/ft_jwt/__init__.py
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     4001 2024-04-22 08:53:54.000000 ft_jwt-0.1.2/ft_jwt/ft_jwt.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-22 08:57:35.000000 ft_jwt-0.1.2/ft_jwt.egg-info/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     2193 2024-04-22 08:57:35.000000 ft_jwt-0.1.2/ft_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      182 2024-04-22 08:57:35.000000 ft_jwt-0.1.2/ft_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-22 08:57:35.000000 ft_jwt-0.1.2/ft_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        7 2024-04-22 08:57:35.000000 ft_jwt-0.1.2/ft_jwt.egg-info/top_level.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       38 2024-04-22 08:57:35.000000 ft_jwt-0.1.2/setup.cfg
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      724 2024-04-22 08:57:22.000000 ft_jwt-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ft_jwt-0.1.0/ft_jwt/ft_jwt.py` & `ft_jwt-0.1.2/ft_jwt/ft_jwt.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import hashlib, base64, hmac, json
 from datetime import datetime, timedelta
 from django.http import JsonResponse
+from django.utils import timezone
 from functools import wraps
 
 class FT_JWT:
 
 	def __init__(self, secret):
 		self.secret = secret
 
@@ -13,15 +14,15 @@
 
 	def createToken(self, sub):
 		"""
 		takes a json object and returns a JWT token
 		- token contains user_id and expiration date (1 day)
 		"""
 		try:
-			current_time = datetime.utcnow() # TODO valentin
+			current_time = timezone.now().replace(tzinfo=None)
 			expire_time = current_time + timedelta(days=1)
 			expire_timestamp = int(expire_time.timestamp())
 
 			header = {
 				'alg': 'HS256',
 				'typ': 'JWT'}
 			payload = {
@@ -55,16 +56,16 @@
 
 			expected_signature = hmac.new(self.secret.encode('utf-8'), f'{encoded_header}.{encoded_payload}'.encode('utf-8'), hashlib.sha256).digest()
 			if not hmac.compare_digest(signature, expected_signature):
 				print ("Signature mismatch")
 				return False, "Signature mismatch"
 
 			if 'exp' in payload:
-				expiration_time = datetime.utcfromtimestamp(payload['exp']) # TODO valentin
-				if expiration_time < datetime.now():
+				expiration_time = datetime.fromtimestamp(payload['exp'])
+				if expiration_time < datetime.now().replace(tzinfo=None):
 					print ("Token expired")
 					return False, "Token expired"
 			else:
 				print ("Expiration time not found in payload")
 				return False, "Expiration time not found in payload"
 			print ("Token is valid")
 			return True, "Token is valid"
```

### Comparing `ft_jwt-0.1.0/ft_jwt.egg-info/PKG-INFO` & `ft_jwt-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,83 @@
 Metadata-Version: 2.1
-Name: ft-jwt
-Version: 0.1.0
+Name: ft_jwt
+Version: 0.1.2
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 Home-page: https://github.com/minthe/ft_transcendence/blob/main/auth/ft_jwt/ft_jwt/ft_jwt.py
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
-License: UNKNOWN
-Description: # JWT Authentication
-        
-        A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
-        
-        ## Changelog
-        
-        ### 0.1.00
-          - does not return the 'user_id' as additional argument anymore.
-          - 'user_id' is now added to the request object.
-          - changed 404 to 401 if token is missing and updated response messages.
-        ### 0.0.20
-          - returns JsonResponse with {'message': "string"} and the status-code
-        
-        ## Features
-        
-        - Generate JWT tokens with customizable expiration times
-        - Validate JWT tokens and verify their integrity using a symmetric secret key and HMAC-SHA256
-        - Extract user information (such as user ID 'sub') from JWT tokens
-        
-        ## Installation
-        
-        You can install the package via pip:
-        
-        ```pip install ft_jwt```
-        
-        ## Usage
-        
-        ```python
-        from ft_jwt.ft_jwt import FT_JWT
-        
-        # Create a JWT instance with your secret key
-        
-        secret_key = 'your_secret_key'
-        ftjwt = FT_JWT(secret_key)
-        
-        # Generate a token for a user
-        
-        sub = '1'
-        token = jwt.createToken(sub)
-        
-        # Validate a token
-        
-        is_valid, message = ftjwt.validateToken(token)
-        if is_valid:
-            print('Token is valid')
-        else:
-            print(f'Token is invalid: {message}')
-        
-        # Get the user ID from a token
-        
-        user_id = ftjwt.getUserId(token)
-        print(f'User ID: {sub}')
-        
-        # Use the decorator to validate against a JWT for a protected route
-        
-        @ftjwt.token_required
-        def protected_route():
-            # This function will be executed only if the token is valid
-            # ...
-        ```
-        
-        # Contributing
-        Contributions are welcome! Please open an issue or submit a pull request.
-        
-        # License
-        This project is licensed under the MIT License.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# JWT Authentication
+
+A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
+
+## Changelog
+
+### 0.1.2
+  - updated timezone awareness
+
+### 0.1.0
+  - does not return the 'user_id' as additional argument anymore.
+  - 'user_id' is now added to the request object.
+  - changed 404 to 401 if token is missing and updated response messages.
+### 0.0.20
+  - returns JsonResponse with {'message': "string"} and the status-code
+
+## Features
+
+- Generate JWT tokens with customizable expiration times
+- Validate JWT tokens and verify their integrity using a symmetric secret key and HMAC-SHA256
+- Extract user information (such as user ID 'sub') from JWT tokens
+
+## Installation
+
+You can install the package via pip:
+
+```pip install ft_jwt```
+
+## Usage
+
+```python
+from ft_jwt.ft_jwt import FT_JWT
+
+# Create a JWT instance with your secret key
+
+secret_key = 'your_secret_key'
+ftjwt = FT_JWT(secret_key)
+
+# Generate a token for a user
+
+sub = '1'
+token = jwt.createToken(sub)
+
+# Validate a token
+
+is_valid, message = ftjwt.validateToken(token)
+if is_valid:
+    print('Token is valid')
+else:
+    print(f'Token is invalid: {message}')
+
+# Get the user ID from a token
+
+user_id = ftjwt.getUserId(token)
+print(f'User ID: {sub}')
+
+# Use the decorator to validate against a JWT for a protected route
+
+@ftjwt.token_required
+def protected_route():
+    # This function will be executed only if the token is valid
+    # ...
+```
+
+# Contributing
+Contributions are welcome! Please open an issue or submit a pull request.
+
+# License
+This project is licensed under the MIT License.
```

### Comparing `ft_jwt-0.1.0/PKG-INFO` & `ft_jwt-0.1.2/ft_jwt.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,83 @@
 Metadata-Version: 2.1
-Name: ft_jwt
-Version: 0.1.0
+Name: ft-jwt
+Version: 0.1.2
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 Home-page: https://github.com/minthe/ft_transcendence/blob/main/auth/ft_jwt/ft_jwt/ft_jwt.py
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
-License: UNKNOWN
-Description: # JWT Authentication
-        
-        A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
-        
-        ## Changelog
-        
-        ### 0.1.00
-          - does not return the 'user_id' as additional argument anymore.
-          - 'user_id' is now added to the request object.
-          - changed 404 to 401 if token is missing and updated response messages.
-        ### 0.0.20
-          - returns JsonResponse with {'message': "string"} and the status-code
-        
-        ## Features
-        
-        - Generate JWT tokens with customizable expiration times
-        - Validate JWT tokens and verify their integrity using a symmetric secret key and HMAC-SHA256
-        - Extract user information (such as user ID 'sub') from JWT tokens
-        
-        ## Installation
-        
-        You can install the package via pip:
-        
-        ```pip install ft_jwt```
-        
-        ## Usage
-        
-        ```python
-        from ft_jwt.ft_jwt import FT_JWT
-        
-        # Create a JWT instance with your secret key
-        
-        secret_key = 'your_secret_key'
-        ftjwt = FT_JWT(secret_key)
-        
-        # Generate a token for a user
-        
-        sub = '1'
-        token = jwt.createToken(sub)
-        
-        # Validate a token
-        
-        is_valid, message = ftjwt.validateToken(token)
-        if is_valid:
-            print('Token is valid')
-        else:
-            print(f'Token is invalid: {message}')
-        
-        # Get the user ID from a token
-        
-        user_id = ftjwt.getUserId(token)
-        print(f'User ID: {sub}')
-        
-        # Use the decorator to validate against a JWT for a protected route
-        
-        @ftjwt.token_required
-        def protected_route():
-            # This function will be executed only if the token is valid
-            # ...
-        ```
-        
-        # Contributing
-        Contributions are welcome! Please open an issue or submit a pull request.
-        
-        # License
-        This project is licensed under the MIT License.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# JWT Authentication
+
+A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
+
+## Changelog
+
+### 0.1.2
+  - updated timezone awareness
+
+### 0.1.0
+  - does not return the 'user_id' as additional argument anymore.
+  - 'user_id' is now added to the request object.
+  - changed 404 to 401 if token is missing and updated response messages.
+### 0.0.20
+  - returns JsonResponse with {'message': "string"} and the status-code
+
+## Features
+
+- Generate JWT tokens with customizable expiration times
+- Validate JWT tokens and verify their integrity using a symmetric secret key and HMAC-SHA256
+- Extract user information (such as user ID 'sub') from JWT tokens
+
+## Installation
+
+You can install the package via pip:
+
+```pip install ft_jwt```
+
+## Usage
+
+```python
+from ft_jwt.ft_jwt import FT_JWT
+
+# Create a JWT instance with your secret key
+
+secret_key = 'your_secret_key'
+ftjwt = FT_JWT(secret_key)
+
+# Generate a token for a user
+
+sub = '1'
+token = jwt.createToken(sub)
+
+# Validate a token
+
+is_valid, message = ftjwt.validateToken(token)
+if is_valid:
+    print('Token is valid')
+else:
+    print(f'Token is invalid: {message}')
+
+# Get the user ID from a token
+
+user_id = ftjwt.getUserId(token)
+print(f'User ID: {sub}')
+
+# Use the decorator to validate against a JWT for a protected route
+
+@ftjwt.token_required
+def protected_route():
+    # This function will be executed only if the token is valid
+    # ...
+```
+
+# Contributing
+Contributions are welcome! Please open an issue or submit a pull request.
+
+# License
+This project is licensed under the MIT License.
```

### Comparing `ft_jwt-0.1.0/README.md` & `ft_jwt-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # JWT Authentication
 
 A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 
 ## Changelog
 
-### 0.1.00
+### 0.1.2
+  - updated timezone awareness
+
+### 0.1.0
   - does not return the 'user_id' as additional argument anymore.
   - 'user_id' is now added to the request object.
   - changed 404 to 401 if token is missing and updated response messages.
 ### 0.0.20
   - returns JsonResponse with {'message': "string"} and the status-code
 
 ## Features
```

### Comparing `ft_jwt-0.1.0/setup.py` & `ft_jwt-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="ft_jwt",
-	version="0.1.0",
+	version="0.1.2",
 	author="vfuhlenb",
 	author_email="minh.tee@gmail.com",
 	description="A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/minthe/ft_transcendence/blob/main/auth/ft_jwt/ft_jwt/ft_jwt.py",
 	packages=setuptools.find_packages(),
```


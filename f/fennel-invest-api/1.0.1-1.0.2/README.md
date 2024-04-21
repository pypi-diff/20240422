# Comparing `tmp/fennel_invest_api-1.0.1.tar.gz` & `tmp/fennel_invest_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fennel_invest_api-1.0.1.tar", last modified: Tue Apr 16 19:56:41 2024, max compression
+gzip compressed data, was "fennel_invest_api-1.0.2.tar", last modified: Sun Apr 21 22:22:06 2024, max compression
```

## Comparing `fennel_invest_api-1.0.1.tar` & `fennel_invest_api-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:56:41.302024 fennel_invest_api-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-16 19:56:41.302024 fennel_invest_api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-16 19:56:37.000000 fennel_invest_api-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:56:41.298024 fennel_invest_api-1.0.1/fennel_invest_api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-16 19:56:37.000000 fennel_invest_api-1.0.1/fennel_invest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-16 19:56:37.000000 fennel_invest_api-1.0.1/fennel_invest_api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-16 19:56:37.000000 fennel_invest_api-1.0.1/fennel_invest_api/fennel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:56:41.302024 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-16 19:56:41.000000 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-16 19:56:41.000000 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:56:41.000000 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 19:56:41.000000 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 19:56:41.000000 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:56:41.302024 fennel_invest_api-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-16 19:56:37.000000 fennel_invest_api-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:22:06.850342 fennel_invest_api-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-21 22:22:06.850342 fennel_invest_api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-21 22:21:59.000000 fennel_invest_api-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:22:06.846342 fennel_invest_api-1.0.2/fennel_invest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 22:21:59.000000 fennel_invest_api-1.0.2/fennel_invest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-21 22:21:59.000000 fennel_invest_api-1.0.2/fennel_invest_api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-21 22:21:59.000000 fennel_invest_api-1.0.2/fennel_invest_api/fennel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:22:06.850342 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-21 22:22:06.000000 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-21 22:22:06.000000 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:22:06.000000 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 22:22:06.000000 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-21 22:22:06.000000 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:22:06.850342 fennel_invest_api-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-21 22:21:59.000000 fennel_invest_api-1.0.2/setup.py
```

### Comparing `fennel_invest_api-1.0.1/PKG-INFO` & `fennel_invest_api-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fennel_invest_api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial Fennel.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/fennel-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: python-dotenv
```

### Comparing `fennel_invest_api-1.0.1/README.md` & `fennel_invest_api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fennel_invest_api-1.0.1/fennel_invest_api/endpoints.py` & `fennel_invest_api-1.0.2/fennel_invest_api/endpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,19 +104,20 @@
                 "timeInForce": "day",
                 "routingOption": "exchange_ats_sdp",
             }
         }
         return json.dumps(self.build_graphql_payload(query, variables))
 
     @staticmethod
-    def build_headers(Bearer, graphql=True):
+    def build_headers(Bearer=None, accounts_host=False):
         headers = {
             "accept": "*/*",
             "accept-encoding": "gzip",
-            "authorization": f"Bearer {Bearer}",
             "content-type": "application/json",
             "host": "fennel-api.prod.fennel.com",
             "user-agent": "Dart/3.3 (dart:io)",
         }
-        if not graphql:
+        if Bearer is not None:
+            headers["authorization"] = f"Bearer {Bearer}"
+        if accounts_host:
             headers["host"] = "accounts.fennel.com"
         return headers
```

### Comparing `fennel_invest_api-1.0.1/fennel_invest_api/fennel.py` & `fennel_invest_api-1.0.2/fennel_invest_api/fennel.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,42 +110,44 @@
         response = self.session.post(url, json=payload)
         if response.status_code != 200:
             raise Exception(f"Failed to login: {response.text}")
         response = response.json()
         self.Bearer = response["access_token"]
         self.Refresh = response["refresh_token"]
         self.ID_Token = response["id_token"]
+        self.refresh_token()
         self._save_credentials()
         return True
 
     def refresh_token(self):
         url = self.endpoints.oauth_url()
+        headers = self.endpoints.build_headers(accounts_host=True)
         payload = {
             "grant_type": "refresh_token",
             "client_id": self.client_id,
             "refresh_token": self.Refresh,
             "scope": "openid profile offline_access email",
         }
-        response = self.session.post(url, json=payload)
+        response = self.session.post(url, json=payload, headers=headers)
         if response.status_code != 200:
             raise Exception(f"Failed to refresh bearer token: {response.text}")
         response = response.json()
         self.Bearer = f"{response['access_token']}"
         self.Refresh = response["refresh_token"]
         self.ID_Token = response["id_token"]
         return response
 
     def _verify_login(self):
         # Test login by getting portfolio summary
         try:
             self.get_portfolio_summary()
             return True
         except Exception:
-            self.refresh_token()
             try:
+                self.refresh_token()
                 self.get_portfolio_summary()
                 return True
             except Exception:
                 return False
 
     @check_login
     def get_portfolio_summary(self):
@@ -154,15 +156,15 @@
         response = self.session.post(
             self.endpoints.graphql, headers=headers, data=query
         )
         if response.status_code != 200:
             raise Exception(
                 f"Portfolio Request failed with status code {response.status_code}: {response.text}"
             )
-        return response.json()
+        return response.json()["data"]["portfolio"]
 
     @check_login
     def get_stock_holdings(self):
         query = self.endpoints.stock_holdings_query()
         headers = self.endpoints.build_headers(self.Bearer)
         response = self.session.post(
             self.endpoints.graphql, headers=headers, data=query
@@ -185,15 +187,15 @@
             raise Exception(
                 f"Market Open Request failed with status code {response.status_code}: {response.text}"
             )
         response = response.json()
         return response["data"]["securityMarketInfo"]["isOpen"]
 
     @check_login
-    def place_order(self, ticker, quantity, side, price="market"):
+    def place_order(self, ticker, quantity, side, price="market", dry_run=False):
         if side.lower() not in ["buy", "sell"]:
             raise Exception("Side must be either 'buy' or 'sell'")
         # Check if market is open
         if not self.is_market_open():
             raise Exception("Market is closed. Cannot place order.")
         # Search for stock "isin"
         query = self.endpoints.stock_search_query(ticker)
@@ -202,14 +204,16 @@
             self.endpoints.graphql, headers=headers, data=query
         )
         if search_response.status_code != 200:
             raise Exception(
                 f"Stock Search Request failed with status code {search_response.status_code}: {search_response.text}"
             )
         search_response = search_response.json()
+        if dry_run:
+            return search_response
         isin = search_response["data"]["searchSearch"]["searchSecurities"][0]["isin"]
         # Place order
         query = self.endpoints.stock_order_query(ticker, quantity, isin, side, price)
         order_response = self.session.post(
             self.endpoints.graphql, headers=headers, data=query
         )
         if order_response.status_code != 200:
```

### Comparing `fennel_invest_api-1.0.1/fennel_invest_api.egg-info/PKG-INFO` & `fennel_invest_api-1.0.2/fennel_invest_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fennel_invest_api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial Fennel.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/fennel-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: python-dotenv
```


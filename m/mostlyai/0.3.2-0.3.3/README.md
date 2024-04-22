# Comparing `tmp/mostlyai-0.3.2.tar.gz` & `tmp/mostlyai-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mostlyai-0.3.2.tar", max compression
+gzip compressed data, was "mostlyai-0.3.3.tar", max compression
```

## Comparing `mostlyai-0.3.2.tar` & `mostlyai-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-12-22 12:47:38.462094 mostlyai-0.3.2/LICENSE
--rw-r--r--   0        0        0     2303 2024-04-02 17:48:15.885881 mostlyai-0.3.2/README.md
--rw-r--r--   0        0        0       26 2024-03-20 14:08:04.920127 mostlyai-0.3.2/mostlyai/__init__.py
--rw-r--r--   0        0        0    13512 2024-04-19 17:00:58.547459 mostlyai-0.3.2/mostlyai/api.py
--rw-r--r--   0        0        0     9150 2024-04-19 16:58:34.132208 mostlyai-0.3.2/mostlyai/base.py
--rw-r--r--   0        0        0     2667 2024-04-19 17:47:47.986738 mostlyai-0.3.2/mostlyai/connectors.py
--rw-r--r--   0        0        0      574 2024-04-19 16:58:25.136734 mostlyai-0.3.2/mostlyai/exceptions.py
--rw-r--r--   0        0        0     3986 2024-04-19 17:47:38.895142 mostlyai-0.3.2/mostlyai/generators.py
--rw-r--r--   0        0        0    38859 2024-04-19 16:58:34.132998 mostlyai-0.3.2/mostlyai/model.py
--rw-r--r--   0        0        0     1694 2024-04-19 17:52:24.624339 mostlyai-0.3.2/mostlyai/shares.py
--rw-r--r--   0        0        0     7008 2024-04-19 17:47:29.352485 mostlyai-0.3.2/mostlyai/synthetic_datasets.py
--rw-r--r--   0        0        0     5217 2024-04-19 16:58:25.140847 mostlyai-0.3.2/mostlyai/utils.py
--rw-r--r--   0        0        0     1264 2024-04-19 17:54:32.905630 mostlyai-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 mostlyai-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-22 12:47:38.462094 mostlyai-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2303 2024-04-02 17:48:15.885881 mostlyai-0.3.3/README.md
+-rw-r--r--   0        0        0       26 2024-03-20 14:08:04.920127 mostlyai-0.3.3/mostlyai/__init__.py
+-rw-r--r--   0        0        0    13512 2024-04-19 17:00:58.547459 mostlyai-0.3.3/mostlyai/api.py
+-rw-r--r--   0        0        0     9150 2024-04-19 16:58:34.132208 mostlyai-0.3.3/mostlyai/base.py
+-rw-r--r--   0        0        0     2859 2024-04-19 16:58:25.136301 mostlyai-0.3.3/mostlyai/connectors.py
+-rw-r--r--   0        0        0      574 2024-04-19 16:58:25.136734 mostlyai-0.3.3/mostlyai/exceptions.py
+-rw-r--r--   0        0        0     4193 2024-04-19 16:58:25.138102 mostlyai-0.3.3/mostlyai/generators.py
+-rw-r--r--   0        0        0    38859 2024-04-19 16:58:34.132998 mostlyai-0.3.3/mostlyai/model.py
+-rw-r--r--   0        0        0     1694 2024-04-22 07:20:07.509641 mostlyai-0.3.3/mostlyai/shares.py
+-rw-r--r--   0        0        0     7215 2024-04-19 16:58:25.140291 mostlyai-0.3.3/mostlyai/synthetic_datasets.py
+-rw-r--r--   0        0        0     5217 2024-04-19 16:58:25.140847 mostlyai-0.3.3/mostlyai/utils.py
+-rw-r--r--   0        0        0     1264 2024-04-22 08:24:08.951204 mostlyai-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 mostlyai-0.3.3/PKG-INFO
```

### Comparing `mostlyai-0.3.2/LICENSE` & `mostlyai-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.2/README.md` & `mostlyai-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.2/mostlyai/api.py` & `mostlyai-0.3.3/mostlyai/api.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.2/mostlyai/base.py` & `mostlyai-0.3.3/mostlyai/base.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.2/mostlyai/connectors.py` & `mostlyai-0.3.3/mostlyai/connectors.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,28 +11,35 @@
     # PUBLIC METHODS #
 
     def list(
         self,
         offset: int = 0,
         limit: int = 50,
         access_type: Optional[str] = None,
+        search_term: Optional[str] = None,
     ) -> Iterator[Connector]:
         """
         List connectors.
 
         Paginate through all connectors that the user has access to.
         Only connectors, that are independent of a table, will be returned.
 
         :param offset: Offset the entities in the response. Optional. Default: 0
         :param limit: Limit the number of entities in the response. Optional. Default: 50
         :param access_type: Filter by access type. Possible values: "SOURCE", "DESTINATION"
+        :param search_term: Filter by string in name. Optional
         :return: Iterator over connectors.
         """
         with Paginator(
-            self, Connector, offset=offset, limit=limit, access_type=access_type
+            self,
+            Connector,
+            offset=offset,
+            limit=limit,
+            access_type=access_type,
+            search_term=search_term,
         ) as paginator:
             for item in paginator:
                 yield item
 
     def get(self, connector_id: str) -> Connector:
         """
         Retrieve a connector.
```

### Comparing `mostlyai-0.3.2/mostlyai/exceptions.py` & `mostlyai-0.3.3/mostlyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.2/mostlyai/generators.py` & `mostlyai-0.3.3/mostlyai/generators.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,35 @@
     # PUBLIC METHODS #
 
     def list(
         self,
         offset: int = 0,
         limit: int = 50,
         status: Optional[Union[str, list[str]]] = None,
+        search_term: Optional[str] = None,
     ) -> Iterator[Generator]:
         """
         List generators.
 
         Paginate through all generators that the user has access to.
 
         :param offset: Offset the entities in the response. Optional. Default: 0
         :param limit: Limit the number of entities in the response. Optional. Default: 50
         :param status: Filter by training status. Optional. Default: None
+        :param search_term: Filter by string in name or description. Optional
         :return: Iterator over generators.
         """
         status = ",".join(status) if isinstance(status, list) else status
         with Paginator(
-            self, Generator, offset=offset, limit=limit, status=status
+            self,
+            Generator,
+            offset=offset,
+            limit=limit,
+            status=status,
+            search_term=search_term,
         ) as paginator:
             for item in paginator:
                 yield item
 
     def get(self, generator_id: str) -> Generator:
         """
         Retrieve generator
```

### Comparing `mostlyai-0.3.2/mostlyai/model.py` & `mostlyai-0.3.3/mostlyai/model.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.2/mostlyai/shares.py` & `mostlyai-0.3.3/mostlyai/shares.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.2/mostlyai/synthetic_datasets.py` & `mostlyai-0.3.3/mostlyai/synthetic_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,35 @@
     # PUBLIC METHODS #
 
     def list(
         self,
         offset: int = 0,
         limit: int = 50,
         status: Optional[Union[str, list[str]]] = None,
+        search_term: Optional[str] = None,
     ) -> Iterator[SyntheticDataset]:
         """
         List synthetic datasets.
 
         Paginate through all synthetic datasets that the user has access to.
 
         :param offset: Offset the entities in the response. Optional. Default: 0
         :param limit: Limit the number of entities in the response. Optional. Default: 50
         :param status: Filter by generation status. Optional. Default: None
+        :param search_term: Filter by string in name or description. Optional
         :return: Iterator over synthetic datasets.
         """
         status = ",".join(status) if isinstance(status, list) else status
         with Paginator(
-            self, SyntheticDataset, offset=offset, limit=limit, status=status
+            self,
+            SyntheticDataset,
+            offset=offset,
+            limit=limit,
+            status=status,
+            search_term=search_term,
         ) as paginator:
             for item in paginator:
                 yield item
 
     def get(self, synthetic_dataset_id: str) -> SyntheticDataset:
         """
         Retrieve synthetic dataset
```

### Comparing `mostlyai-0.3.2/mostlyai/utils.py` & `mostlyai-0.3.3/mostlyai/utils.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.2/pyproject.toml` & `mostlyai-0.3.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mostlyai"
-version = "0.3.2"
+version = "0.3.3"
 description = "The official Python client for the MOSTLY AI platform."
 homepage = "https://app.mostly.ai/"
 authors = ["MOSTLY AI <office@mostly.ai>"]
 license = "Proprietary"
 readme = "README.md"
 packages = [
     { include = "mostlyai" }
```

### Comparing `mostlyai-0.3.2/PKG-INFO` & `mostlyai-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mostlyai
-Version: 0.3.2
+Version: 0.3.3
 Summary: The official Python client for the MOSTLY AI platform.
 Home-page: https://app.mostly.ai/
 License: Proprietary
 Author: MOSTLY AI
 Author-email: office@mostly.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```


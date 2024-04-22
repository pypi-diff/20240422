# Comparing `tmp/runtool-1.0.6.tar.gz` & `tmp/runtool-1.0.7.tar.gz`

## Comparing `runtool-1.0.6.tar` & `runtool-1.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0    45791 2020-02-02 00:00:00.000000 runtool-1.0.6/runtool/__init__.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 runtool-1.0.6/runtool/_additional_cli.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 runtool-1.0.6/runtool/_types.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 runtool-1.0.6/runtool/_version.py
--rw-r--r--   0        0        0    20999 2020-02-02 00:00:00.000000 runtool-1.0.6/runtool/runtool.ini
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 runtool-1.0.6/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 runtool-1.0.6/LICENSE
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 runtool-1.0.6/README.md
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 runtool-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 runtool-1.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0    46956 2020-02-02 00:00:00.000000 runtool-1.0.7/runtool/__init__.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 runtool-1.0.7/runtool/_additional_cli.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 runtool-1.0.7/runtool/_types.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 runtool-1.0.7/runtool/_version.py
+-rw-r--r--   0        0        0    20999 2020-02-02 00:00:00.000000 runtool-1.0.7/runtool/runtool.ini
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 runtool-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 runtool-1.0.7/LICENSE
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 runtool-1.0.7/README.md
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 runtool-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 runtool-1.0.7/PKG-INFO
```

### Comparing `runtool-1.0.6/runtool/__init__.py` & `runtool-1.0.7/runtool/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 from typing import TYPE_CHECKING
 from typing import Union
 from urllib.parse import urljoin
 from urllib.parse import urlparse
 
 
 if TYPE_CHECKING:
+    from requests import PreparedRequest
+    import requests
     from typing import Protocol  # python3.8+
     from typing import Literal
     from typing_extensions import Self
     from typing_extensions import TypeAlias
     from _collections_abc import dict_keys
 
     JSON_TYPE: TypeAlias = Union[str, int, float, bool, None, List[Any], Dict[str, Any]]
@@ -137,40 +139,81 @@
             "python3.12",
             "python3.13",
         )
         if shutil.which(x)
     ) or (sys.executable,)
 
 
+@lru_cache(maxsize=None)
+def domain_env_name(domain: str) -> str:
+    domain = domain.upper()
+    if domain in {"API.GITHUB.COM", "GITHUB.COM"}:
+        domain = f"PUBLIC.{domain}"
+
+    domain = f"TOKEN.{domain}"
+
+    weight = {
+        "GITHUB": 80,
+        "TOKEN": 90,
+    }
+    parsed = domain.rsplit(".", maxsplit=1)[0].upper()
+    tokens = sorted(
+        (x for x in re.split(r"[.-]+", parsed) if x not in {"API", "CLOUD"}),
+        key=lambda x: (weight.get(x, 0), x),
+    )
+    return "_".join(tokens)
+
+
 @lru_cache(maxsize=1)
-def get_request(url: str) -> str:
-    import urllib.request
+def default_session() -> requests.Session:
+    import requests
+    import requests.auth
+
+    class MyAuth(requests.auth.AuthBase):
+        def __call__(self, r: PreparedRequest) -> PreparedRequest:
+            if r.url:
+                from urllib.parse import urlparse
+
+                env_name = domain_env_name(urlparse(r.url).netloc)
+                if env_name in os.environ:
+                    r.headers["Authorization"] = f"token {os.environ[env_name]}"
+            return r
+
+    ret = requests.Session()
+    ret.auth = MyAuth()
+    return ret
+
+
+# def m_requests(url: str, headers: dict[str, str] | None = None) -> _UrlopenRet:
+#     import urllib.request
+
+#     headers = headers or {}
+#     if "github" in url and "GITHUB_TOKEN" in os.environ:
+#         headers["Authorization"] = f'token {os.environ["GITHUB_TOKEN"]}'
 
-    headers = {}
-    if "github" in url and "GITHUB_TOKEN" in os.environ:
-        headers["Authorization"] = f'token {os.environ["GITHUB_TOKEN"]}'
-    req = urllib.request.Request(url, headers=headers)  # noqa: S310
-    with urllib.request.urlopen(req) as f:  # noqa: S310
-        return f.read().decode("utf-8")
+#     req = urllib.request.Request(url, headers=headers or {})
+#     return urllib.request.urlopen(req)
+
+
+@lru_cache(maxsize=1)
+def get_request(url: str) -> str:
+    return default_session().get(url).text
+    # with m_requests(url) as f:
+    #     return f.read().decode("utf-8")
 
 
 @contextmanager
 def download_context(url: str) -> Generator[str, None, None]:
-    import urllib.request
-
     logging.info("Downloading: %s", url)
     derive_name = os.path.basename(url)
     with tempfile.TemporaryDirectory() as tempdir:
         download_path = os.path.join(tempdir, derive_name)
-        headers = {}
-        if "github" in url and "GITHUB_TOKEN" in os.environ:
-            headers["Authorization"] = f'token {os.environ["GITHUB_TOKEN"]}'
-        req = urllib.request.Request(url, headers=headers)  # noqa: S310
-        with open(download_path, "wb") as file, urllib.request.urlopen(req) as f:  # noqa: S310
-            file.write(f.read())
+        with open(download_path, "wb") as file, default_session().get(url, stream=True) as response:
+            for chunk in response.iter_content(chunk_size=4 * 1024):
+                file.write(chunk)
         yield download_path
 
 
 # region core
 
 
 @dataclass
@@ -958,15 +1001,15 @@
 
         with suppress(Exception):
             import warnings
 
             warnings.simplefilter("ignore")
             from importlib.resources import path as importlib_path
 
-            with importlib_path(__package__, config_filename) as ipath:
+            with importlib_path(__package__, config_filename) as ipath:  # pyright: ignore[reportArgumentType]
                 foo.append(ipath.as_posix())
         return list({x: None for x in foo}.keys())
 
     @lru_cache(maxsize=1)  # noqa: B019
     def tools_descriptions(self) -> dict[str, str]:
         return {
             k: v.get("description", "") for k, v in sorted(self.config.items()) if k != "DEFAULT"
```

### Comparing `runtool-1.0.6/runtool/_additional_cli.py` & `runtool-1.0.7/runtool/_additional_cli.py`

 * *Files identical despite different names*

### Comparing `runtool-1.0.6/runtool/_types.py` & `runtool-1.0.7/runtool/_types.py`

 * *Files identical despite different names*

### Comparing `runtool-1.0.6/runtool/runtool.ini` & `runtool-1.0.7/runtool/runtool.ini`

 * *Files identical despite different names*

### Comparing `runtool-1.0.6/.gitignore` & `runtool-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `runtool-1.0.6/LICENSE` & `runtool-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `runtool-1.0.6/README.md` & `runtool-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `runtool-1.0.6/pyproject.toml` & `runtool-1.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,18 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
-dependencies = []
+dependencies = [
+  "requests",
+  "typing_extensions",
+]
 
 [project.scripts]
 runtool = "runtool:main"
 
 [project.urls]
 Documentation = "https://github.com/FlavioAmurrioCS/runtool#readme"
 Issues = "https://github.com/FlavioAmurrioCS/runtool/issues"
```

### Comparing `runtool-1.0.6/PKG-INFO` & `runtool-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: runtool
-Version: 1.0.6
+Version: 1.0.7
 Summary: Install binary from github release.
 Project-URL: Documentation, https://github.com/FlavioAmurrioCS/runtool#readme
 Project-URL: Issues, https://github.com/FlavioAmurrioCS/runtool/issues
 Project-URL: Source, https://github.com/FlavioAmurrioCS/runtool
 Author-email: Flavio Amurrio <25621374+FlavioAmurrioCS@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Requires-Dist: requests
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # runtool
 
 [![PyPI - Version](https://img.shields.io/pypi/v/runtool.svg)](https://pypi.org/project/runtool)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/runtool.svg)](https://pypi.org/project/runtool)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/FlavioAmurrioCS/runtool/main.svg)](https://results.pre-commit.ci/latest/github/FlavioAmurrioCS/runtool/main)
```


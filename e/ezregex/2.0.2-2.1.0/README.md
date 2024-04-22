# Comparing `tmp/ezregex-2.0.2.tar.gz` & `tmp/ezregex-2.1.0.tar.gz`

## Comparing `ezregex-2.0.2.tar` & `ezregex-2.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-2.0.2/.coveragerc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-2.0.2/MANIFEST.in
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ezregex-2.0.2/requirements.txt
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ezregex-2.0.2/setup.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-2.0.2/tox.ini
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-2.0.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 ezregex-2.0.2/.github/workflows/unit-tests.yml
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/EZRegex.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/EZRegex.pyi
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/__init__.py
--rw-r--r--   0        0        0     7510 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/_docs.py
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/api.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/api.pyi
--rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/generate.py
--rw-r--r--   0        0        0    24925 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/invert.py
--rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/invert_old.py
--rw-r--r--   0        0        0   337000 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/assets/common_sorted_words.json
--rw-r--r--   0        0        0  4975177 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/assets/sorted_words.json
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/base/__init__.py
--rw-r--r--   0        0        0    14657 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/base/elements.py
--rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/base/interface.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/javascript/JavaScriptEZRegex.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/javascript/__init__.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/javascript/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/javascript/elements.pyi
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/perl/PerlEZRegex.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/perl/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/perl/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/perl/elements.pyi
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/python/PythonEZRegex.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/python/PythonEZRegex.pyi
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/python/__init__.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/python/elements.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ezregex-2.0.2/ezregex/python/elements.pyi
--rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/test_EZRegex.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/test_api.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/test_generate.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/test_invert.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/test_javascript.py
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/test_operators.py
--rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/test_python.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/test_replacement.py
--rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/testing_color_algorithm.ipynb
--rw-r--r--   0        0        0    13448 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/data/groups.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/data/python_regexs.jsonc
--rw-r--r--   0        0        0    22828 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/data/regexs.jsonc
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 ezregex-2.0.2/tests/data/replacements.jsonc
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 ezregex-2.0.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-2.0.2/LICENSE
--rw-r--r--   0        0        0    55085 2020-02-02 00:00:00.000000 ezregex-2.0.2/README.md
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ezregex-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    56025 2020-02-02 00:00:00.000000 ezregex-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-2.1.0/.coveragerc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-2.1.0/MANIFEST.in
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ezregex-2.1.0/requirements.txt
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ezregex-2.1.0/setup.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-2.1.0/tox.ini
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-2.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 ezregex-2.1.0/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/EZRegex.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/EZRegex.pyi
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/__init__.py
+-rw-r--r--   0        0        0     7510 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/_docs.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/api.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/api.pyi
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/generate.py
+-rw-r--r--   0        0        0    24925 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/invert.py
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/invert_old.py
+-rw-r--r--   0        0        0   337000 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/assets/common_sorted_words.json
+-rw-r--r--   0        0        0  4975177 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/assets/sorted_words.json
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/base/__init__.py
+-rw-r--r--   0        0        0    14657 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/base/elements.py
+-rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/base/interface.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/javascript/JavaScriptEZRegex.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/javascript/__init__.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/javascript/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/javascript/elements.pyi
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/perl/PerlEZRegex.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/perl/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/perl/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/perl/elements.pyi
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/python/PythonEZRegex.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/python/PythonEZRegex.pyi
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/python/__init__.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/python/elements.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ezregex-2.1.0/ezregex/python/elements.pyi
+-rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/test_EZRegex.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/test_api.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/test_generate.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/test_invert.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/test_javascript.py
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/test_operators.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/test_python.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/test_replacement.py
+-rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/testing_color_algorithm.ipynb
+-rw-r--r--   0        0        0    13448 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/data/groups.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/data/python_regexs.jsonc
+-rw-r--r--   0        0        0    22828 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/data/regexs.jsonc
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 ezregex-2.1.0/tests/data/replacements.jsonc
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 ezregex-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-2.1.0/LICENSE
+-rw-r--r--   0        0        0    55085 2020-02-02 00:00:00.000000 ezregex-2.1.0/README.md
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ezregex-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    56025 2020-02-02 00:00:00.000000 ezregex-2.1.0/PKG-INFO
```

### Comparing `ezregex-2.0.2/setup.py` & `ezregex-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/.github/FUNDING.yml` & `ezregex-2.1.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/.github/workflows/unit-tests.yml` & `ezregex-2.1.0/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/EZRegex.py` & `ezregex-2.1.0/ezregex/EZRegex.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/EZRegex.pyi` & `ezregex-2.1.0/ezregex/EZRegex.pyi`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/_docs.py` & `ezregex-2.1.0/ezregex/_docs.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/api.py` & `ezregex-2.1.0/ezregex/api.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/api.pyi` & `ezregex-2.1.0/ezregex/api.pyi`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/generate.py` & `ezregex-2.1.0/ezregex/generate.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/invert.py` & `ezregex-2.1.0/ezregex/invert.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/invert_old.py` & `ezregex-2.1.0/ezregex/invert_old.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/assets/common_sorted_words.json` & `ezregex-2.1.0/ezregex/assets/common_sorted_words.json`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/assets/sorted_words.json` & `ezregex-2.1.0/ezregex/assets/sorted_words.json`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/base/__init__.py` & `ezregex-2.1.0/ezregex/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/base/elements.py` & `ezregex-2.1.0/ezregex/base/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/base/interface.py` & `ezregex-2.1.0/ezregex/base/interface.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/python/PythonEZRegex.py` & `ezregex-2.1.0/ezregex/python/PythonEZRegex.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/python/PythonEZRegex.pyi` & `ezregex-2.1.0/ezregex/python/PythonEZRegex.pyi`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/ezregex/python/elements.py` & `ezregex-2.1.0/ezregex/python/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/test_EZRegex.py` & `ezregex-2.1.0/tests/test_EZRegex.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/test_api.py` & `ezregex-2.1.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/test_generate.py` & `ezregex-2.1.0/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/test_invert.py` & `ezregex-2.1.0/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/test_javascript.py` & `ezregex-2.1.0/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/test_operators.py` & `ezregex-2.1.0/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/test_python.py` & `ezregex-2.1.0/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/test_replacement.py` & `ezregex-2.1.0/tests/test_replacement.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/testing_color_algorithm.ipynb` & `ezregex-2.1.0/tests/testing_color_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/data/groups.py` & `ezregex-2.1.0/tests/data/groups.py`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/data/regexs.jsonc` & `ezregex-2.1.0/tests/data/regexs.jsonc`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/tests/data/replacements.jsonc` & `ezregex-2.1.0/tests/data/replacements.jsonc`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/.gitignore` & `ezregex-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/LICENSE` & `ezregex-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/README.md` & `ezregex-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/pyproject.toml` & `ezregex-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezregex-2.0.2/PKG-INFO` & `ezregex-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ezregex
-Version: 2.0.2
+Version: 2.1.0
 Summary: A readable and intuitive way to generate Regular Expressions
 Project-URL: Documentation, https://github.com/smartycope/ezregex?tab=readme-ov-file#documentation
 Project-URL: Issues, https://github.com/smartycope/ezregex/issues
 Project-URL: Source, https://github.com/smartycope/ezregex
 Project-URL: Official Website, https://ezregex.org
 Author-email: Copeland Carter <smartycope@gmail.com>
 License-Expression: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: ezregex Version: 2.0.2 Summary: A readable and
+Metadata-Version: 2.3 Name: ezregex Version: 2.1.0 Summary: A readable and
 intuitive way to generate Regular Expressions Project-URL: Documentation,
 https://github.com/smartycope/ezregex?tab=readme-ov-file#documentation Project-
 URL: Issues, https://github.com/smartycope/ezregex/issues Project-URL: Source,
 https://github.com/smartycope/ezregex Project-URL: Official Website, https://
 ezregex.org Author-email: Copeland Carter
 gmail.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
```


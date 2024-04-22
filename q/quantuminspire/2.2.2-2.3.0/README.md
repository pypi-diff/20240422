# Comparing `tmp/quantuminspire-2.2.2.tar.gz` & `tmp/quantuminspire-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantuminspire-2.2.2.tar", last modified: Mon Feb 26 08:04:19 2024, max compression
+gzip compressed data, was "quantuminspire-2.3.0.tar", last modified: Mon Apr 22 06:55:31 2024, max compression
```

## Comparing `quantuminspire-2.2.2.tar` & `quantuminspire-2.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 08:04:19.267383 quantuminspire-2.2.2/
--rw-rw-rw-   0        0        0    10354 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/LICENSE.md
--rw-rw-rw-   0        0        0      746 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/NOTICE.md
--rw-rw-rw-   0        0        0    10082 2024-02-26 08:04:19.265383 quantuminspire-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     8476 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-02-26 08:04:19.267383 quantuminspire-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2678 2024-02-26 07:58:38.000000 quantuminspire-2.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-26 08:04:19.220382 quantuminspire-2.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-02-26 08:04:19.238376 quantuminspire-2.2.2/src/quantuminspire/
--rw-rw-rw-   0        0        0       34 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/__init__.py
--rw-rw-rw-   0        0        0    58497 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/api.py
--rw-rw-rw-   0        0        0     8170 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/credentials.py
--rw-rw-rw-   0        0        0     1101 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/exceptions.py
--rw-rw-rw-   0        0        0     3501 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/job.py
-drwxrwxrwx   0        0        0        0 2024-02-26 08:04:19.248376 quantuminspire-2.2.2/src/quantuminspire/projectq/
--rw-rw-rw-   0        0        0        0 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/projectq/__init__.py
--rw-rw-rw-   0        0        0    37411 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/projectq/backend_qx.py
-drwxrwxrwx   0        0        0        0 2024-02-26 08:04:19.261379 quantuminspire-2.2.2/src/quantuminspire/qiskit/
--rw-rw-rw-   0        0        0      116 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/qiskit/__init__.py
--rw-rw-rw-   0        0        0    32915 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/qiskit/backend_qx.py
--rw-rw-rw-   0        0        0    33308 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/qiskit/circuit_parser.py
--rw-rw-rw-   0        0        0    10929 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/qiskit/measurements.py
--rw-rw-rw-   0        0        0     9565 2024-02-26 07:58:38.000000 quantuminspire-2.2.2/src/quantuminspire/qiskit/qi_job.py
--rw-rw-rw-   0        0        0     9215 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/qiskit/qi_result.py
--rw-rw-rw-   0        0        0     8947 2024-02-26 07:41:23.000000 quantuminspire-2.2.2/src/quantuminspire/qiskit/quantum_inspire_provider.py
--rw-rw-rw-   0        0        0       23 2024-02-26 07:58:38.000000 quantuminspire-2.2.2/src/quantuminspire/version.py
-drwxrwxrwx   0        0        0        0 2024-02-26 08:04:19.246377 quantuminspire-2.2.2/src/quantuminspire.egg-info/
--rw-rw-rw-   0        0        0    10082 2024-02-26 08:04:19.000000 quantuminspire-2.2.2/src/quantuminspire.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      803 2024-02-26 08:04:19.000000 quantuminspire-2.2.2/src/quantuminspire.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 08:04:19.000000 quantuminspire-2.2.2/src/quantuminspire.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      284 2024-02-26 08:04:19.000000 quantuminspire-2.2.2/src/quantuminspire.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-02-26 08:04:19.000000 quantuminspire-2.2.2/src/quantuminspire.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 06:55:31.197150 quantuminspire-2.3.0/
+-rw-rw-rw-   0        0        0    10354 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/LICENSE.md
+-rw-rw-rw-   0        0        0      746 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/NOTICE.md
+-rw-rw-rw-   0        0        0    10076 2024-04-22 06:55:31.197150 quantuminspire-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8476 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 06:55:31.197150 quantuminspire-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2672 2024-04-22 06:49:49.000000 quantuminspire-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:55:31.170195 quantuminspire-2.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 06:55:31.182901 quantuminspire-2.3.0/src/quantuminspire/
+-rw-rw-rw-   0        0        0       34 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/__init__.py
+-rw-rw-rw-   0        0        0    58497 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/api.py
+-rw-rw-rw-   0        0        0     8170 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/credentials.py
+-rw-rw-rw-   0        0        0     1101 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/exceptions.py
+-rw-rw-rw-   0        0        0     3501 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/job.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:55:31.187928 quantuminspire-2.3.0/src/quantuminspire/projectq/
+-rw-rw-rw-   0        0        0        0 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/projectq/__init__.py
+-rw-rw-rw-   0        0        0    37411 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/projectq/backend_qx.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:55:31.195637 quantuminspire-2.3.0/src/quantuminspire/qiskit/
+-rw-rw-rw-   0        0        0      116 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/qiskit/__init__.py
+-rw-rw-rw-   0        0        0    32915 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/qiskit/backend_qx.py
+-rw-rw-rw-   0        0        0    33308 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/qiskit/circuit_parser.py
+-rw-rw-rw-   0        0        0    10929 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/qiskit/measurements.py
+-rw-rw-rw-   0        0        0     9565 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/qiskit/qi_job.py
+-rw-rw-rw-   0        0        0     9215 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/qiskit/qi_result.py
+-rw-rw-rw-   0        0        0     8947 2024-04-22 06:40:37.000000 quantuminspire-2.3.0/src/quantuminspire/qiskit/quantum_inspire_provider.py
+-rw-rw-rw-   0        0        0       23 2024-04-22 06:49:49.000000 quantuminspire-2.3.0/src/quantuminspire/version.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:55:31.187416 quantuminspire-2.3.0/src/quantuminspire.egg-info/
+-rw-rw-rw-   0        0        0    10076 2024-04-22 06:55:31.000000 quantuminspire-2.3.0/src/quantuminspire.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2024-04-22 06:55:31.000000 quantuminspire-2.3.0/src/quantuminspire.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 06:55:31.000000 quantuminspire-2.3.0/src/quantuminspire.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      278 2024-04-22 06:55:31.000000 quantuminspire-2.3.0/src/quantuminspire.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-22 06:55:31.000000 quantuminspire-2.3.0/src/quantuminspire.egg-info/top_level.txt
```

### Comparing `quantuminspire-2.2.2/LICENSE.md` & `quantuminspire-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/NOTICE.md` & `quantuminspire-2.3.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/PKG-INFO` & `quantuminspire-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantuminspire
-Version: 2.2.2
+Version: 2.3.0
 Summary: SDK for the Quantum Inspire platform
 Home-page: https://qutech.nl
 Author: QuantumInspire
 Author-email: support@quantum-inspire.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
 Requires-Dist: coreapi>=2.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: jupyter
 Requires-Dist: nbimporter
 Requires-Dist: qilib
 Requires-Dist: setuptools
 Provides-Extra: qiskit
-Requires-Dist: qiskit<1.0,>=0.46; extra == "qiskit"
+Requires-Dist: qiskit>=1.0; extra == "qiskit"
 Requires-Dist: qiskit-aer; extra == "qiskit"
 Provides-Extra: projectq
 Requires-Dist: projectq>=0.8.0; extra == "projectq"
 Provides-Extra: dev
 Requires-Dist: pytest>=3.3.1; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: mypy>=0.670; extra == "dev"
```

### Comparing `quantuminspire-2.2.2/README.md` & `quantuminspire-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/setup.py` & `quantuminspire-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,12 +59,12 @@
           'Programming Language :: Python :: 3.12',
           'License :: OSI Approved :: Apache Software License'],
       license='Apache 2.0',
       packages=['quantuminspire', 'quantuminspire.qiskit', 'quantuminspire.projectq'],
       install_requires=['coverage>=4.5.1', 'matplotlib>=2.1', 'pylatexenc', 'coreapi>=2.3.3', 'numpy>=1.20', 'jupyter',
                         'nbimporter', 'qilib', 'setuptools'],
       extras_require={
-          "qiskit": ["qiskit>=0.46,<1.0", "qiskit-aer"],
+          "qiskit": ["qiskit>=1.0", "qiskit-aer"],
           "projectq": ["projectq>=0.8.0"],
           "dev": ["pytest>=3.3.1", "pylint", "mypy>=0.670"],
           "rtd": ["sphinx", "sphinx_rtd_theme", "nbsphinx", "sphinx-automodapi", "recommonmark"],
       })
```

### Comparing `quantuminspire-2.2.2/src/quantuminspire/api.py` & `quantuminspire-2.3.0/src/quantuminspire/api.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/src/quantuminspire/credentials.py` & `quantuminspire-2.3.0/src/quantuminspire/credentials.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/src/quantuminspire/exceptions.py` & `quantuminspire-2.3.0/src/quantuminspire/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/src/quantuminspire/job.py` & `quantuminspire-2.3.0/src/quantuminspire/job.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/src/quantuminspire/projectq/backend_qx.py` & `quantuminspire-2.3.0/src/quantuminspire/projectq/backend_qx.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/src/quantuminspire/qiskit/backend_qx.py` & `quantuminspire-2.3.0/src/quantuminspire/qiskit/backend_qx.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/src/quantuminspire/qiskit/circuit_parser.py` & `quantuminspire-2.3.0/src/quantuminspire/qiskit/circuit_parser.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/src/quantuminspire/qiskit/measurements.py` & `quantuminspire-2.3.0/src/quantuminspire/qiskit/measurements.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/src/quantuminspire/qiskit/qi_job.py` & `quantuminspire-2.3.0/src/quantuminspire/qiskit/qi_job.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/src/quantuminspire/qiskit/qi_result.py` & `quantuminspire-2.3.0/src/quantuminspire/qiskit/qi_result.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/src/quantuminspire/qiskit/quantum_inspire_provider.py` & `quantuminspire-2.3.0/src/quantuminspire/qiskit/quantum_inspire_provider.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.2.2/src/quantuminspire.egg-info/PKG-INFO` & `quantuminspire-2.3.0/src/quantuminspire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantuminspire
-Version: 2.2.2
+Version: 2.3.0
 Summary: SDK for the Quantum Inspire platform
 Home-page: https://qutech.nl
 Author: QuantumInspire
 Author-email: support@quantum-inspire.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
 Requires-Dist: coreapi>=2.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: jupyter
 Requires-Dist: nbimporter
 Requires-Dist: qilib
 Requires-Dist: setuptools
 Provides-Extra: qiskit
-Requires-Dist: qiskit<1.0,>=0.46; extra == "qiskit"
+Requires-Dist: qiskit>=1.0; extra == "qiskit"
 Requires-Dist: qiskit-aer; extra == "qiskit"
 Provides-Extra: projectq
 Requires-Dist: projectq>=0.8.0; extra == "projectq"
 Provides-Extra: dev
 Requires-Dist: pytest>=3.3.1; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: mypy>=0.670; extra == "dev"
```

### Comparing `quantuminspire-2.2.2/src/quantuminspire.egg-info/SOURCES.txt` & `quantuminspire-2.3.0/src/quantuminspire.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/monit-agd-1.0.tar.gz` & `tmp/monit-agd-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monit-agd-1.0.tar", last modified: Mon Apr 22 01:14:40 2024, max compression
+gzip compressed data, was "monit-agd-1.1.tar", last modified: Mon Apr 22 01:28:05 2024, max compression
```

## Comparing `monit-agd-1.0.tar` & `monit-agd-1.1.tar`

### file list

```diff
@@ -1,19 +1,12 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:14:40.177549 monit-agd-1.0/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.0/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1599 2024-04-22 01:14:40.177549 monit-agd-1.0/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      951 2024-04-22 01:06:10.000000 monit-agd-1.0/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:14:40.174216 monit-agd-1.0/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 monit-agd-1.0/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      344 2024-04-22 01:06:10.000000 monit-agd-1.0/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1465 2024-04-22 01:06:10.000000 monit-agd-1.0/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2345 2024-04-22 01:06:10.000000 monit-agd-1.0/monit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      158 2024-04-22 01:06:10.000000 monit-agd-1.0/monit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2613 2024-04-22 01:06:10.000000 monit-agd-1.0/monit/func.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:14:40.177549 monit-agd-1.0/monit_agd.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1599 2024-04-22 01:14:40.000000 monit-agd-1.0/monit_agd.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      285 2024-04-22 01:14:40.000000 monit-agd-1.0/monit_agd.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-22 01:14:40.000000 monit-agd-1.0/monit_agd.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-22 01:14:40.000000 monit-agd-1.0/monit_agd.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-04-22 01:14:40.000000 monit-agd-1.0/monit_agd.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-22 01:14:40.177549 monit-agd-1.0/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      878 2024-04-22 01:14:16.000000 monit-agd-1.0/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:28:05.191732 monit-agd-1.1/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.1/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1633 2024-04-22 01:28:05.191732 monit-agd-1.1/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      998 2024-04-22 01:18:02.000000 monit-agd-1.1/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:28:05.188399 monit-agd-1.1/monit_agd.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1633 2024-04-22 01:28:05.000000 monit-agd-1.1/monit_agd.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      190 2024-04-22 01:28:05.000000 monit-agd-1.1/monit_agd.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-22 01:28:05.000000 monit-agd-1.1/monit_agd.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-22 01:28:05.000000 monit-agd-1.1/monit_agd.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-22 01:28:05.000000 monit-agd-1.1/monit_agd.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-22 01:28:05.191732 monit-agd-1.1/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-04-22 01:27:53.000000 monit-agd-1.1/setup.py
```

### Comparing `monit-agd-1.0/LICENSE` & `monit-agd-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `monit-agd-1.0/PKG-INFO` & `monit-agd-1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.0
+Version: 1.1
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
-Home-page: https://github.com/Agencia-de-Dados-bsb/monit
+Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,14 +53,15 @@
         # For demonstration purposes, let's raise an exception
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         # Notify the Monitor about the error
         monit.notify(SetupError, e)
+        # monit.notify_and_exit(SetupError, e)
 
     monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `monit-agd-1.0/README.md` & `monit-agd-1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         # For demonstration purposes, let's raise an exception
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         # Notify the Monitor about the error
         monit.notify(SetupError, e)
+        # monit.notify_and_exit(SetupError, e)
 
     monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `monit-agd-1.0/monit_agd.egg-info/PKG-INFO` & `monit-agd-1.1/monit_agd.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.0
+Version: 1.1
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
-Home-page: https://github.com/Agencia-de-Dados-bsb/monit
+Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,14 +53,15 @@
         # For demonstration purposes, let's raise an exception
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         # Notify the Monitor about the error
         monit.notify(SetupError, e)
+        # monit.notify_and_exit(SetupError, e)
 
     monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `monit-agd-1.0/setup.py` & `monit-agd-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='monit-agd',
-    version='1.0',
+    version='1.1',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
-    url='https://github.com/Agencia-de-Dados-bsb/monit',
+    url='https://github.com/arktnld/monit',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'sqlalchemy',
         'pymysql',
         'psutil',
```


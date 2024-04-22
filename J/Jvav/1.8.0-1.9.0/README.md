# Comparing `tmp/Jvav-1.8.0.tar.gz` & `tmp/Jvav-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-lw524crv/Jvav-1.8.0.tar", last modified: Sat Apr 13 04:37:15 2024, max compression
+gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-pwvku5r0/Jvav-1.9.0.tar", last modified: Mon Apr 22 03:23:28 2024, max compression
```

## Comparing `Jvav-1.8.0.tar` & `Jvav-1.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-13 04:37:15.000000 Jvav-1.8.0/
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/
--rw-r--r--   0 zh         (501) staff       (20)     4309 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)      295 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/SOURCES.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/dependency_links.txt
--rw-r--r--   0 zh         (501) staff       (20)       39 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/entry_points.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.8.0/Jvav.egg-info/not-zip-safe
--rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/requires.txt
--rw-r--r--   0 zh         (501) staff       (20)       11 2024-04-13 04:37:15.000000 Jvav-1.8.0/Jvav.egg-info/top_level.txt
--rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.8.0/LICENSE
--rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.8.0/MANIFEST.in
--rw-r--r--   0 zh         (501) staff       (20)     4309 2024-04-13 04:37:15.000000 Jvav-1.8.0/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)     3579 2024-04-13 04:36:21.000000 Jvav-1.8.0/README.md
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-13 04:37:15.000000 Jvav-1.8.0/jvav/
--rw-r--r--   0 zh         (501) staff       (20)      507 2024-04-13 04:36:44.000000 Jvav-1.8.0/jvav/__init__.py
--rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.8.0/jvav/cmd.py
--rw-r--r--   0 zh         (501) staff       (20)    77360 2024-04-13 04:33:40.000000 Jvav-1.8.0/jvav/utils.py
--rw-r--r--   0 zh         (501) staff       (20)      495 2024-02-05 07:01:09.000000 Jvav-1.8.0/requirements.txt
--rw-r--r--   0 zh         (501) staff       (20)       38 2024-04-13 04:37:15.000000 Jvav-1.8.0/setup.cfg
--rw-r--r--   0 zh         (501) staff       (20)     1345 2024-04-13 04:36:33.000000 Jvav-1.8.0/setup.py
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-22 03:23:28.000000 Jvav-1.9.0/
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)      295 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/SOURCES.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/dependency_links.txt
+-rw-r--r--   0 zh         (501) staff       (20)       39 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/entry_points.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.9.0/Jvav.egg-info/not-zip-safe
+-rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/requires.txt
+-rw-r--r--   0 zh         (501) staff       (20)       11 2024-04-22 03:23:28.000000 Jvav-1.9.0/Jvav.egg-info/top_level.txt
+-rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.9.0/LICENSE
+-rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.9.0/MANIFEST.in
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-04-22 03:23:28.000000 Jvav-1.9.0/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-1.9.0/README.md
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-22 03:23:28.000000 Jvav-1.9.0/jvav/
+-rw-r--r--   0 zh         (501) staff       (20)      507 2024-04-22 03:22:48.000000 Jvav-1.9.0/jvav/__init__.py
+-rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.9.0/jvav/cmd.py
+-rw-r--r--   0 zh         (501) staff       (20)    77360 2024-04-13 04:33:40.000000 Jvav-1.9.0/jvav/utils.py
+-rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-22 03:22:14.000000 Jvav-1.9.0/requirements.txt
+-rw-r--r--   0 zh         (501) staff       (20)       38 2024-04-22 03:23:28.000000 Jvav-1.9.0/setup.cfg
+-rw-r--r--   0 zh         (501) staff       (20)     1345 2024-04-22 03:22:55.000000 Jvav-1.9.0/setup.py
```

### Comparing `Jvav-1.8.0/Jvav.egg-info/PKG-INFO` & `Jvav-1.9.0/Jvav.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.8.0
+Version: 1.9.0
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
@@ -95,16 +95,16 @@
 And it is recommended to use python virtual environment to avoid some unnecessary problems.
 
 Here is my developing steps:
 
 ```shell
 git clone https://github.com/akynazh/jvav.git
 cd jvav
-~/.pyenv/versions/3.7.12/bin/python -m venv venv
-source ./venv/bin/activate
+~/.pyenv/versions/3.7.12/bin/python -m venv .venv
+source ./.venv/bin/activate
 pip3 install -r requirements.txt
 ```
 
 And then you can enjoy coding! Remember to write or run test cases in `tests/test.py`.
 Please make sure the test is okay before submitting your code~
 
 ## TODO
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.8.0 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.9.0 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
@@ -30,18 +30,18 @@
 code on DMM -pv2 PV2 Follow a code, get the corresponding preview video of the
 code on Avgle -tp Get the top 25 ranking of DMM actresses -p PROXY, --proxy
 PROXY Followed by a proxy server address (by default reads the value of the
 environment variable http_proxy) ``` ## DEV I use python-3.7.12 for
 development, please use python <= 3.7. And it is recommended to use python
 virtual environment to avoid some unnecessary problems. Here is my developing
 steps: ```shell git clone https://github.com/akynazh/jvav.git cd jvav ~/.pyenv/
-versions/3.7.12/bin/python -m venv venv source ./venv/bin/activate pip3 install
--r requirements.txt ``` And then you can enjoy coding! Remember to write or run
-test cases in `tests/test.py`. Please make sure the test is okay before
-submitting your code~ ## TODO The following are some functions to be
+versions/3.7.12/bin/python -m venv .venv source ./.venv/bin/activate pip3
+install -r requirements.txt ``` And then you can enjoy coding! Remember to
+write or run test cases in `tests/test.py`. Please make sure the test is okay
+before submitting your code~ ## TODO The following are some functions to be
 implemented, and I look forward to your contribution~ - [ ] fix SgpUtil
 (currently not work) - [ ] support RankUtil in CMD - [ ] fix JavLibUtil
 (currently not work because of cloudflare) - [x] cache the successful query
 results locally (Thanks: [@akynazh](https://github.com/akynazh)) - [x] support
 javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake)) - [ ]
 support db.msin.jp - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://
 github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)_ _l_o_g_o_._]Thanks to JetBrains
```

### Comparing `Jvav-1.8.0/LICENSE` & `Jvav-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Jvav-1.8.0/PKG-INFO` & `Jvav-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.8.0
+Version: 1.9.0
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
@@ -95,16 +95,16 @@
 And it is recommended to use python virtual environment to avoid some unnecessary problems.
 
 Here is my developing steps:
 
 ```shell
 git clone https://github.com/akynazh/jvav.git
 cd jvav
-~/.pyenv/versions/3.7.12/bin/python -m venv venv
-source ./venv/bin/activate
+~/.pyenv/versions/3.7.12/bin/python -m venv .venv
+source ./.venv/bin/activate
 pip3 install -r requirements.txt
 ```
 
 And then you can enjoy coding! Remember to write or run test cases in `tests/test.py`.
 Please make sure the test is okay before submitting your code~
 
 ## TODO
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.8.0 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.9.0 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
@@ -30,18 +30,18 @@
 code on DMM -pv2 PV2 Follow a code, get the corresponding preview video of the
 code on Avgle -tp Get the top 25 ranking of DMM actresses -p PROXY, --proxy
 PROXY Followed by a proxy server address (by default reads the value of the
 environment variable http_proxy) ``` ## DEV I use python-3.7.12 for
 development, please use python <= 3.7. And it is recommended to use python
 virtual environment to avoid some unnecessary problems. Here is my developing
 steps: ```shell git clone https://github.com/akynazh/jvav.git cd jvav ~/.pyenv/
-versions/3.7.12/bin/python -m venv venv source ./venv/bin/activate pip3 install
--r requirements.txt ``` And then you can enjoy coding! Remember to write or run
-test cases in `tests/test.py`. Please make sure the test is okay before
-submitting your code~ ## TODO The following are some functions to be
+versions/3.7.12/bin/python -m venv .venv source ./.venv/bin/activate pip3
+install -r requirements.txt ``` And then you can enjoy coding! Remember to
+write or run test cases in `tests/test.py`. Please make sure the test is okay
+before submitting your code~ ## TODO The following are some functions to be
 implemented, and I look forward to your contribution~ - [ ] fix SgpUtil
 (currently not work) - [ ] support RankUtil in CMD - [ ] fix JavLibUtil
 (currently not work because of cloudflare) - [x] cache the successful query
 results locally (Thanks: [@akynazh](https://github.com/akynazh)) - [x] support
 javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake)) - [ ]
 support db.msin.jp - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://
 github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)_ _l_o_g_o_._]Thanks to JetBrains
```

### Comparing `Jvav-1.8.0/README.md` & `Jvav-1.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -75,16 +75,16 @@
 And it is recommended to use python virtual environment to avoid some unnecessary problems.
 
 Here is my developing steps:
 
 ```shell
 git clone https://github.com/akynazh/jvav.git
 cd jvav
-~/.pyenv/versions/3.7.12/bin/python -m venv venv
-source ./venv/bin/activate
+~/.pyenv/versions/3.7.12/bin/python -m venv .venv
+source ./.venv/bin/activate
 pip3 install -r requirements.txt
 ```
 
 And then you can enjoy coding! Remember to write or run test cases in `tests/test.py`.
 Please make sure the test is okay before submitting your code~
 
 ## TODO
```

#### html2text {}

```diff
@@ -20,16 +20,16 @@
 the corresponding preview video of the code on DMM -pv2 PV2 Follow a code, get
 the corresponding preview video of the code on Avgle -tp Get the top 25 ranking
 of DMM actresses -p PROXY, --proxy PROXY Followed by a proxy server address (by
 default reads the value of the environment variable http_proxy) ``` ## DEV I
 use python-3.7.12 for development, please use python <= 3.7. And it is
 recommended to use python virtual environment to avoid some unnecessary
 problems. Here is my developing steps: ```shell git clone https://github.com/
-akynazh/jvav.git cd jvav ~/.pyenv/versions/3.7.12/bin/python -m venv venv
-source ./venv/bin/activate pip3 install -r requirements.txt ``` And then you
+akynazh/jvav.git cd jvav ~/.pyenv/versions/3.7.12/bin/python -m venv .venv
+source ./.venv/bin/activate pip3 install -r requirements.txt ``` And then you
 can enjoy coding! Remember to write or run test cases in `tests/test.py`.
 Please make sure the test is okay before submitting your code~ ## TODO The
 following are some functions to be implemented, and I look forward to your
 contribution~ - [ ] fix SgpUtil(currently not work) - [ ] support RankUtil in
 CMD - [ ] fix JavLibUtil(currently not work because of cloudflare) - [x] cache
 the successful query results locally (Thanks: [@akynazh](https://github.com/
 akynazh)) - [x] support javdb.com (Thanks: [@Steven-Fake](https://github.com/
```

### Comparing `Jvav-1.8.0/jvav/cmd.py` & `Jvav-1.9.0/jvav/cmd.py`

 * *Files identical despite different names*

### Comparing `Jvav-1.8.0/jvav/utils.py` & `Jvav-1.9.0/jvav/utils.py`

 * *Files identical despite different names*

### Comparing `Jvav-1.8.0/setup.py` & `Jvav-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requires = [i.strip() for i in r]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="Jvav",
-    version="1.8.0",
+    version="1.9.0",
     description="Useful tools for Jav.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/akynazh/jvav",
     download_url="https://github.com/akynazh/jvav/releases/latest",
     author="akynazh",
     author_email="akynazh@gmail.com",
```


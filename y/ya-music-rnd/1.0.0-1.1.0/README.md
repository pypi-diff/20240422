# Comparing `tmp/ya-music-rnd-1.0.0.tar.gz` & `tmp/ya_music_rnd-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ya-music-rnd-1.0.0.tar", last modified: Mon Jan 23 01:28:25 2023, max compression
+gzip compressed data, was "ya_music_rnd-1.1.0.tar", last modified: Sun Apr 21 22:06:51 2024, max compression
```

## Comparing `ya-music-rnd-1.0.0.tar` & `ya_music_rnd-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-23 01:28:25.031320 ya-music-rnd-1.0.0/
--rw-rw-rw-   0        0        0     3385 2023-01-22 23:29:24.000000 ya-music-rnd-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       36 2022-06-03 02:09:49.000000 ya-music-rnd-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5139 2023-01-23 01:28:25.031320 ya-music-rnd-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3955 2023-01-23 01:24:33.000000 ya-music-rnd-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-01-23 01:28:25.032318 ya-music-rnd-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1557 2023-01-23 01:27:59.000000 ya-music-rnd-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:28:25.022344 ya-music-rnd-1.0.0/ya_music_rnd/
--rw-rw-rw-   0        0        0     6046 2023-01-20 07:40:31.000000 ya-music-rnd-1.0.0/ya_music_rnd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-23 01:28:25.030322 ya-music-rnd-1.0.0/ya_music_rnd.egg-info/
--rw-rw-rw-   0        0        0     5139 2023-01-23 01:28:24.000000 ya-music-rnd-1.0.0/ya_music_rnd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-01-23 01:28:25.000000 ya-music-rnd-1.0.0/ya_music_rnd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-23 01:28:24.000000 ya-music-rnd-1.0.0/ya_music_rnd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-01-23 01:28:24.000000 ya-music-rnd-1.0.0/ya_music_rnd.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 22:06:51.522766 ya_music_rnd-1.1.0/
+-rw-rw-rw-   0        0        0     3385 2023-01-22 23:29:24.000000 ya_music_rnd-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       36 2022-06-03 02:09:49.000000 ya_music_rnd-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5163 2024-04-21 22:06:51.521769 ya_music_rnd-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3955 2023-01-23 01:24:33.000000 ya_music_rnd-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 22:06:51.522766 ya_music_rnd-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1566 2024-04-19 02:25:20.000000 ya_music_rnd-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:06:51.480808 ya_music_rnd-1.1.0/tests/
+-rw-rw-rw-   0        0        0     8526 2024-04-19 00:59:23.000000 ya_music_rnd-1.1.0/tests/test_1.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:06:51.495384 ya_music_rnd-1.1.0/ya_music_rnd/
+-rw-rw-rw-   0        0        0     7393 2024-04-19 02:24:12.000000 ya_music_rnd-1.1.0/ya_music_rnd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:06:51.520772 ya_music_rnd-1.1.0/ya_music_rnd.egg-info/
+-rw-rw-rw-   0        0        0     5163 2024-04-21 22:06:51.000000 ya_music_rnd-1.1.0/ya_music_rnd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-04-21 22:06:51.000000 ya_music_rnd-1.1.0/ya_music_rnd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 22:06:51.000000 ya_music_rnd-1.1.0/ya_music_rnd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-21 22:06:51.000000 ya_music_rnd-1.1.0/ya_music_rnd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-21 22:06:51.000000 ya_music_rnd-1.1.0/ya_music_rnd.egg-info/top_level.txt
```

### Comparing `ya-music-rnd-1.0.0/LICENSE` & `ya_music_rnd-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ya-music-rnd-1.0.0/PKG-INFO` & `ya_music_rnd-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya-music-rnd
-Version: 1.0.0
+Version: 1.1.0
 Summary: Поиск случайного исполнителя на сайте яндекс музыки
 Home-page: https://github.com/Genzo4/yandex_rnd
 Author: Genzo
 Author-email: genzo@bk.ru
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Genzo4/yandex_rnd/issues
 Keywords: yandex,music,yandex_rnd,ya_music_rnd,ya
@@ -21,14 +21,15 @@
 Classifier: Natural Language :: Russian
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: urllib3
 
 # yandex_rnd
 
 ![PyPI](https://img.shields.io/pypi/v/ya_music_rnd)
 ![PyPI - License](https://img.shields.io/pypi/l/ya_music_rnd)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ya_music_rnd)
```

### Comparing `ya-music-rnd-1.0.0/README.md` & `ya_music_rnd-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ya-music-rnd-1.0.0/setup.py` & `ya_music_rnd-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 top_level_directory = path.abspath(path.dirname(__file__))
 with open(path.join(top_level_directory, 'README.md'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
    name='ya-music-rnd',
-   version='1.0.0',
+   version='1.1.0',
    description='Поиск случайного исполнителя на сайте яндекс музыки',
    long_description=long_description,
    long_description_content_type='text/markdown',
    author='Genzo',
    author_email='genzo@bk.ru',
    url='https://github.com/Genzo4/yandex_rnd',
    project_urls={
@@ -33,10 +33,10 @@
       'Topic :: Scientific/Engineering',
       'Topic :: Software Development',
       'Topic :: Software Development :: Libraries :: Python Modules'
    ],
    keywords=['yandex', 'music', 'yandex_rnd', 'ya_music_rnd', 'ya'],
    license='MIT',
    packages=['ya_music_rnd'],
-   install_requires=[],
+   install_requires=['urllib3'],
    python_requires='>=3.8'
 )
```

### Comparing `ya-music-rnd-1.0.0/ya_music_rnd.egg-info/PKG-INFO` & `ya_music_rnd-1.1.0/ya_music_rnd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya-music-rnd
-Version: 1.0.0
+Version: 1.1.0
 Summary: Поиск случайного исполнителя на сайте яндекс музыки
 Home-page: https://github.com/Genzo4/yandex_rnd
 Author: Genzo
 Author-email: genzo@bk.ru
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Genzo4/yandex_rnd/issues
 Keywords: yandex,music,yandex_rnd,ya_music_rnd,ya
@@ -21,14 +21,15 @@
 Classifier: Natural Language :: Russian
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: urllib3
 
 # yandex_rnd
 
 ![PyPI](https://img.shields.io/pypi/v/ya_music_rnd)
 ![PyPI - License](https://img.shields.io/pypi/l/ya_music_rnd)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ya_music_rnd)
```


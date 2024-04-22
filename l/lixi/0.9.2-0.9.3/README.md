# Comparing `tmp/lixi-0.9.2.tar.gz` & `tmp/lixi-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lixi-0.9.2.tar", last modified: Tue Jun  8 05:51:02 2021, max compression
+gzip compressed data, was "dist/lixi-0.9.3.tar", last modified: Wed Jun  9 06:17:49 2021, max compression
```

## Comparing `lixi-0.9.2.tar` & `lixi-0.9.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-08 05:51:02.000000 lixi-0.9.2/
--rw-rw-rw-   0 root         (0) root         (0)      319 2021-05-31 04:20:16.000000 lixi-0.9.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     5340 2021-05-31 04:20:16.000000 lixi-0.9.2/README.md
--rw-r--r--   0 root         (0) root         (0)     6588 2021-06-08 05:51:02.000000 lixi-0.9.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1739 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     6588 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       60 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi/
--rw-rw-rw-   0 root         (0) root         (0)    94854 2021-05-31 04:20:16.000000 lixi-0.9.2/lixi/_customise_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    13227 2021-05-31 04:20:16.000000 lixi-0.9.2/lixi/_command_line.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2021-05-31 04:20:16.000000 lixi-0.9.2/lixi/_schema_documentation.py
--rw-rw-rw-   0 root         (0) root         (0)    35953 2021-06-08 05:50:14.000000 lixi-0.9.2/lixi/_explode_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2753 2021-05-31 04:20:16.000000 lixi-0.9.2/lixi/_schematron_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    15113 2021-05-31 04:20:16.000000 lixi-0.9.2/lixi/customization.xsd
--rw-rw-rw-   0 root         (0) root         (0)    64839 2021-05-31 04:20:16.000000 lixi-0.9.2/lixi/_LIXI.py
--rw-rw-rw-   0 root         (0) root         (0)    41567 2021-05-31 04:20:16.000000 lixi-0.9.2/lixi/_Message.py
--rw-rw-rw-   0 root         (0) root         (0)    17410 2021-05-31 04:20:16.000000 lixi-0.9.2/lixi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi/documentation/
--rw-r--r--   0 root         (0) root         (0)     5075 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/index.html
--rw-r--r--   0 root         (0) root         (0)       44 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi/documentation/js/
--rw-r--r--   0 root         (0) root         (0)     2640 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/js/theme.js
--rw-r--r--   0 root         (0) root         (0)    42030 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/js/marked.js
--rw-r--r--   0 root         (0) root         (0)   271701 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/js/LIXI_Glossary.js
--rw-r--r--   0 root         (0) root         (0)  6313631 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/js/LIXI-Master-Schema.js
--rw-r--r--   0 root         (0) root         (0)   125720 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/js/GenerateHTML.js
--rw-r--r--   0 root         (0) root         (0)    10111 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/js/vkbeautify.0.99.00.beta.js
--rw-r--r--   0 root         (0) root         (0)    84245 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/js/jquery-2.1.1.min.js
--rw-r--r--   0 root         (0) root         (0)    11084 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/js/modernizr-2.8.3.min.js
--rw-r--r--   0 root         (0) root         (0)      595 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi/documentation/fonts/
--rw-r--r--   0 root         (0) root         (0)    79076 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    43572 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)   197829 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)    37405 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)     1015 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/create_documentation.py
--rw-r--r--   0 root         (0) root         (0)       59 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi/documentation/css/
--rw-r--r--   0 root         (0) root         (0)    88854 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/css/theme.css
--rw-r--r--   0 root         (0) root         (0)     3952 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/css/theme_extra.css
--rw-r--r--   0 root         (0) root         (0)     4761 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/css/extra.css
--rw-r--r--   0 root         (0) root         (0)     1664 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/css/highlight.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi/documentation/img/
--rw-r--r--   0 root         (0) root         (0)      325 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/img/info-icon.png
--rw-r--r--   0 root         (0) root         (0)      622 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/img/info.png
--rw-r--r--   0 root         (0) root         (0)     1205 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/img/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    34661 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/img/wheel.gif
--rw-r--r--   0 root         (0) root         (0)    16453 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/img/clip.png
--rw-r--r--   0 root         (0) root         (0)     4765 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/img/lixi_logo_100.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi/documentation/mkdocs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-08 05:51:02.000000 lixi-0.9.2/lixi/documentation/mkdocs/js/
--rw-r--r--   0 root         (0) root         (0)     8835 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/mkdocs/js/mustache.min.js
--rw-r--r--   0 root         (0) root         (0)     6871 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/mkdocs/js/search.js
--rw-r--r--   0 root         (0) root         (0)    15439 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/mkdocs/js/lunr.min.js
--rw-r--r--   0 root         (0) root         (0)    15611 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/mkdocs/js/text.js
--rw-r--r--   0 root         (0) root         (0)    15292 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/mkdocs/js/require.js
--rw-r--r--   0 root         (0) root         (0)     4031 2021-06-08 05:50:37.000000 lixi-0.9.2/lixi/documentation/search.html
--rw-rw-rw-   0 root         (0) root         (0)     8708 2021-05-31 04:20:16.000000 lixi-0.9.2/lixi/_xslt_transform.py
--rw-rw-rw-   0 root         (0) root         (0)    53924 2021-05-31 04:20:16.000000 lixi-0.9.2/lixi/_jsonschema_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    14381 2021-05-31 04:20:16.000000 lixi-0.9.2/lixi/_path_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    13296 2021-06-08 05:50:14.000000 lixi-0.9.2/lixi/_xml_to_json.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-06-08 05:51:02.000000 lixi-0.9.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1142 2021-05-31 04:20:16.000000 lixi-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-09 06:17:49.000000 lixi-0.9.3/
+-rw-rw-rw-   0 root         (0) root         (0)      319 2021-05-31 04:56:22.000000 lixi-0.9.3/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2021-05-31 04:56:22.000000 lixi-0.9.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     6588 2021-06-09 06:17:49.000000 lixi-0.9.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1739 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     6588 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi/
+-rw-rw-rw-   0 root         (0) root         (0)    94854 2021-05-31 04:56:22.000000 lixi-0.9.3/lixi/_customise_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    13227 2021-05-31 04:56:22.000000 lixi-0.9.3/lixi/_command_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     3887 2021-05-31 04:56:22.000000 lixi-0.9.3/lixi/_schema_documentation.py
+-rw-rw-rw-   0 root         (0) root         (0)    35953 2021-06-08 01:50:16.000000 lixi-0.9.3/lixi/_explode_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2753 2021-05-31 04:56:22.000000 lixi-0.9.3/lixi/_schematron_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15113 2021-05-31 04:56:22.000000 lixi-0.9.3/lixi/customization.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    65667 2021-06-09 06:06:30.000000 lixi-0.9.3/lixi/_LIXI.py
+-rw-rw-rw-   0 root         (0) root         (0)    41567 2021-05-31 04:56:22.000000 lixi-0.9.3/lixi/_Message.py
+-rw-rw-rw-   0 root         (0) root         (0)    17719 2021-06-09 06:06:30.000000 lixi-0.9.3/lixi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi/documentation/
+-rw-r--r--   0 root         (0) root         (0)     5075 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/index.html
+-rw-r--r--   0 root         (0) root         (0)       44 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi/documentation/js/
+-rw-r--r--   0 root         (0) root         (0)     2640 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/js/theme.js
+-rw-r--r--   0 root         (0) root         (0)    42030 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/js/marked.js
+-rw-r--r--   0 root         (0) root         (0)   271701 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/js/LIXI_Glossary.js
+-rw-r--r--   0 root         (0) root         (0)  6313631 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/js/LIXI-Master-Schema.js
+-rw-r--r--   0 root         (0) root         (0)   125720 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/js/GenerateHTML.js
+-rw-r--r--   0 root         (0) root         (0)    10111 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/js/vkbeautify.0.99.00.beta.js
+-rw-r--r--   0 root         (0) root         (0)    84245 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/js/jquery-2.1.1.min.js
+-rw-r--r--   0 root         (0) root         (0)    11084 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/js/modernizr-2.8.3.min.js
+-rw-r--r--   0 root         (0) root         (0)      595 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi/documentation/fonts/
+-rw-r--r--   0 root         (0) root         (0)    79076 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    43572 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)   197829 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)    37405 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)     1015 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/create_documentation.py
+-rw-r--r--   0 root         (0) root         (0)       59 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi/documentation/css/
+-rw-r--r--   0 root         (0) root         (0)    88854 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)     3952 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/css/theme_extra.css
+-rw-r--r--   0 root         (0) root         (0)     4761 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/css/extra.css
+-rw-r--r--   0 root         (0) root         (0)     1664 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/css/highlight.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi/documentation/img/
+-rw-r--r--   0 root         (0) root         (0)      325 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/img/info-icon.png
+-rw-r--r--   0 root         (0) root         (0)      622 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/img/info.png
+-rw-r--r--   0 root         (0) root         (0)     1205 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/img/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    34661 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/img/wheel.gif
+-rw-r--r--   0 root         (0) root         (0)    16453 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/img/clip.png
+-rw-r--r--   0 root         (0) root         (0)     4765 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/img/lixi_logo_100.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi/documentation/mkdocs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-09 06:17:49.000000 lixi-0.9.3/lixi/documentation/mkdocs/js/
+-rw-r--r--   0 root         (0) root         (0)     8835 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/mkdocs/js/mustache.min.js
+-rw-r--r--   0 root         (0) root         (0)     6871 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/mkdocs/js/search.js
+-rw-r--r--   0 root         (0) root         (0)    15439 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/mkdocs/js/lunr.min.js
+-rw-r--r--   0 root         (0) root         (0)    15611 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/mkdocs/js/text.js
+-rw-r--r--   0 root         (0) root         (0)    15292 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/mkdocs/js/require.js
+-rw-r--r--   0 root         (0) root         (0)     4031 2021-06-09 06:17:19.000000 lixi-0.9.3/lixi/documentation/search.html
+-rw-rw-rw-   0 root         (0) root         (0)     8708 2021-05-31 04:56:22.000000 lixi-0.9.3/lixi/_xslt_transform.py
+-rw-rw-rw-   0 root         (0) root         (0)    53924 2021-05-31 04:56:22.000000 lixi-0.9.3/lixi/_jsonschema_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14381 2021-05-31 04:56:22.000000 lixi-0.9.3/lixi/_path_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13296 2021-06-08 01:50:16.000000 lixi-0.9.3/lixi/_xml_to_json.py
+-rw-r--r--   0 root         (0) root         (0)       38 2021-06-09 06:17:49.000000 lixi-0.9.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2021-05-31 04:56:22.000000 lixi-0.9.3/setup.py
```

### Comparing `lixi-0.9.2/README.md` & `lixi-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/PKG-INFO` & `lixi-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lixi
-Version: 0.9.2
+Version: 0.9.3
 Summary: lixi is a python package to manipulate a valid LIXI 2 message and schema.
 Home-page: https://standards.lixi.org.au/lixi-tech/lixi-pypi
 Author: Ammar Khan
 Author-email: lixilab@lixi.org.au
 License: MIT
 Description: LIXI Package Overview
         ====
```

### Comparing `lixi-0.9.2/lixi.egg-info/SOURCES.txt` & `lixi-0.9.3/lixi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi.egg-info/PKG-INFO` & `lixi-0.9.3/lixi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lixi
-Version: 0.9.2
+Version: 0.9.3
 Summary: lixi is a python package to manipulate a valid LIXI 2 message and schema.
 Home-page: https://standards.lixi.org.au/lixi-tech/lixi-pypi
 Author: Ammar Khan
 Author-email: lixilab@lixi.org.au
 License: MIT
 Description: LIXI Package Overview
         ====
```

### Comparing `lixi-0.9.2/lixi/_customise_schema.py` & `lixi-0.9.3/lixi/_customise_schema.py`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/_command_line.py` & `lixi-0.9.3/lixi/_command_line.py`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/_schema_documentation.py` & `lixi-0.9.3/lixi/_schema_documentation.py`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/_explode_schema.py` & `lixi-0.9.3/lixi/_explode_schema.py`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/_schematron_functions.py` & `lixi-0.9.3/lixi/_schematron_functions.py`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/customization.xsd` & `lixi-0.9.3/lixi/customization.xsd`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/_LIXI.py` & `lixi-0.9.3/lixi/_LIXI.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 ns = {
     "xs": "http://www.w3.org/2001/XMLSchema",
     "lx": "lixi.org.au/schema/appinfo_elements",
     "li": "lixi.org.au/schema/appinfo_instructions",
 }
 
 if __name__ == "_LIXI":
-    import _path_functions, _jsonschema_functions, _customise_schema, _xslt_transform, _schema_documentation
+    import _path_functions, _jsonschema_functions, _customise_schema, _xslt_transform, _schema_documentation, _explode_schema
 else:
     from lixi import (
         _path_functions,
         _jsonschema_functions,
         _customise_schema,
         _xslt_transform, 
-        _schema_documentation
+        _schema_documentation,
+        _explode_schema
     )
 
 
 class LIXI(object):
     """Represents a LIXI Instance.
         
     The singleton class exists as a wrapper for all message manipulation functions the library is to provide.
@@ -845,36 +846,42 @@
         self,
         lixi_transaction_type=None,
         lixi_version=None,
         custom_version=None,
         schema_string=None,
         schema_path=None,
         output_path=None,
-        return_annotated = False
+        return_annotated = False,
+        exploded = False        
     ):
         """Fetches a LIXI JSON schema dict object or converts from an LIXI XML schema.
 
         Args:
             lixi_transaction_type (:obj:`str`, optional): The transaction type of the LIXI schema to be fetched. Should be one of 'ACC', 'CAL', 'CDA', 'CNZ', 'DAS', 'LMI', 'SVC', 'VAL'. Defaults to None.
             lixi_version (:obj:`str`, optional): The version of the LIXI schema to be fetched. Should be in the format of '2.6.24'. Defaults to None. Defaults to the latest version if only lixi_transaction_type is provided.
             custom_version (:obj:`str`, optional): The version of the LIXI custom schema to be fetched. Usually a complete file name of the custom schema. Defaults to None.
             schema_string (:obj:`str`, optional): LIXI schema provided as a string. Defaults to None.
             schema_path (:obj:`str`, optional): LIXI schema provided as a path. Defaults to None.
             output_path (:obj:`str`, optional): Path to write the fetched lixi schema to. Defaults to None.
             return_annotated (:obj:`boolean`, optional): Variable to indicated if the returned schema should be annotated or not.
-    
+            exploded (:obj:`boolean`, optional): Variable to indicate if the returned schema should be exploded or not.
+            
+            
         Result:
             A Python dict object of the schema or saved to the output folder specified. 
     
         Raises:
             LIXIInvalidSyntax: Incorrect schema string/file fetched.
             LIXIValidationError: Validation errors in the schema string/file fetched.
             LIXIResouceNotFoundError: File not found or can't be written.
         """
-
+        # Make sure schema is annotated if exploded set to true
+        if exploded==True:
+            return_annotated = True
+            
         # Determine which source is given
         output_schema = None
 
         if (
             lixi_transaction_type == None
             and custom_version == None
             and schema_string == None
@@ -883,17 +890,15 @@
             raise LIXIInvalidSyntax(
                 "Fetch schema failed. Fetch parameters not specified."
             )
 
         # Custom schema is done first to avoid fetching un custom schema based on transaction and version number
         if custom_version != None:
             output_xml_schema = self.__load_schema__(custom_version=custom_version)
-            output_schema = _jsonschema_functions.convert_to_json_schema(
-                output_xml_schema
-            )
+            
 
         # Fetch based on transaction type and version
         elif lixi_version != None or lixi_transaction_type != None:
             if lixi_transaction_type == None:
                 raise LIXIInvalidSyntax(
                     "Fetch schema failed. Transaction type parameter not specified."
                 )
@@ -906,30 +911,35 @@
                     )
                 else:
                     lixi_version = self.get_schema_latest_version(lixi_transaction_type)
 
             output_xml_schema = self.__load_schema__(
                 lixi_transaction_type=lixi_transaction_type, lixi_version=lixi_version, return_annotated=return_annotated
             )
-            output_schema = _jsonschema_functions.convert_to_json_schema(
-                output_xml_schema
-            )
+            
 
         # Fetch based on string or path
         elif schema_string != None or schema_path != None:
 
             if schema_path != None:
                 output_xml_schema = self.__load_schema__(schema_path=schema_path, return_annotated=return_annotated)
             else:
                 output_xml_schema = self.__load_schema__(schema_string=schema_string, return_annotated=return_annotated)
 
-            output_schema = _jsonschema_functions.convert_to_json_schema(
-                output_xml_schema
-            )
-
+            
+            
+        # Explode the schema if flag set to True
+        if exploded==True:
+            output_xml_schema = _explode_schema.main(output_xml_schema)
+            
+        # Convert into JSON
+        output_schema = _jsonschema_functions.convert_to_json_schema(
+            output_xml_schema
+        )        
+            
         # Output the schema to a file or return object
         if output_path == None:
             return _json.dumps(
                         output_schema, sort_keys=True, indent=4, ensure_ascii=False
                     )
         else:
             self.__write__(
@@ -949,36 +959,42 @@
         self,
         lixi_transaction_type=None,
         lixi_version=None,
         custom_version=None,
         schema_string=None,
         schema_path=None,
         output_path=None,
-        return_annotated = False
+        return_annotated = False,
+        exploded = False
     ):
         """Fetches a LIXI XML schema Etree object or converts from an LIXI JSON schema.
 
         Args:
             lixi_transaction_type (:obj:`str`, optional): The transaction type of the LIXI schema to be fetched. Should be one of 'ACC', 'CAL', 'CDA', 'CNZ', 'DAS', 'LMI', 'SVC', 'VAL'. Defaults to None.
             lixi_version (:obj:`str`, optional): The version of the LIXI schema to be fetched. Should be in the format of '2.6.24'. Defaults to None. Defaults to the latest version if only lixi_transaction_type is provided.
             custom_version (:obj:`str`, optional): The version of the LIXI custom schema to be fetched. Usually a complete file name of the custom schema. Defaults to None.
             schema_string (:obj:`str`, optional): LIXI schema provided as a string. Defaults to None.
             schema_path (:obj:`str`, optional): LIXI schema provided as a path. Defaults to None.
             output_path (:obj:`str`, optional): Path to write the fetched lixi schema to. Defaults to None.
             return_annotated (:obj:`boolean`, optional): Variable to indicated if the returned schema should be annotated or not.
-    
+            exploded (:obj:`boolean`, optional): Variable to indicate if the returned schema should be exploded or not.
+            
         Result:
             A Python Etree object of the schema or saved to the output folder specified. 
     
         Raises:
             LIXIInvalidSyntax: Incorrect schema string/file fetched.
             LIXIValidationError: Validation errors in the schema string/file fetched.
             LIXIResouceNotFoundError: File not found or can't be written.
         """
-
+        
+        # Make sure schema is annotated if exploded set to true
+        if exploded==True:
+            return_annotated = True
+            
         # Determine which source is given
         output_schema = None
 
         if (
             lixi_transaction_type == None
             and custom_version == None            
             and schema_string == None
@@ -1015,15 +1031,19 @@
         # Fetch based on string or path
         elif schema_string != None or schema_path != None:
 
             if schema_path != None:
                 output_schema = self.__load_schema__(schema_path=schema_path, return_annotated=return_annotated)
             else:
                 output_schema = self.__load_schema__(schema_string=schema_string, return_annotated=return_annotated)
-
+        
+        # Explode the schema if flag set to True
+        if exploded==True:
+            output_schema = _explode_schema.main(output_schema)
+                
         # Output the schema to a file or return object
         if output_path == None:
             return _etree.tostring(output_schema, pretty_print=True).decode("utf-8")
         else:
             self.__write__(
                 "fetched_xml_schema_output.xsd",
                 output_path,
```

### Comparing `lixi-0.9.2/lixi/_Message.py` & `lixi-0.9.3/lixi/_Message.py`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/__init__.py` & `lixi-0.9.3/lixi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,26 +236,28 @@
 def get_json_schema(
     lixi_transaction_type=None,
     lixi_version=None,
     custom_version=None,
     schema_string=None,
     schema_path=None,
     output_path=None,
-    return_annotated=False
+    return_annotated=False,
+    exploded = False
 ):
     """Fetches a LIXI JSON schema dict object or converts from an LIXI XML schema. 
 
     Args:
         lixi_transaction_type (:obj:`str`, optional): The transaction type of the LIXI schema to be fetched. Should be one of 'ACC', 'CAL', 'CDA', 'CNZ', 'DAS', 'LMI', 'SVC', 'VAL'. Defaults to None. 
         lixi_version (:obj:`str`, optional): The version of the LIXI schema to be fetched. Should be in the format of '2.6.24'. Defaults to None. Defaults to the latest version if only lixi_transaction_type is provided. 
         custom_version (:obj:`str`, optional): The version of the LIXI custom schema to be fetched. Usually a complete file name of the custom schema. Defaults to None. 
         schema_string (:obj:`str`, optional): LIXI schema provided as a string. Defaults to None. 
         schema_path (:obj:`str`, optional): LIXI schema provided as a path. Defaults to None. 
         output_path (:obj:`str`, optional): Path to write the fetched lixi schema to. Defaults to None.
-        return_annotated (:obj:`boolean`, optional): Variable to indicate if the returned schema should be annotated or not. 
+        return_annotated (:obj:`boolean`, optional): Variable to indicate if the returned schema should be annotated or not.
+        exploded (:obj:`boolean`, optional): Variable to indicate if the returned schema should be exploded or not.
 
     Result: 
         A string object of the LIXI JSON schema or saved to the output folder specified.  
 
     Raises:
         LIXIInvalidSyntax: Incorrect schema string/file fetched. 
         LIXIValidationError: Validation errors in the schema string/file fetched. 
@@ -265,37 +267,40 @@
     return _LIXI.getInstance().fetch_json_schema(
         lixi_transaction_type,
         lixi_version,
         custom_version,
         schema_string,
         schema_path,
         output_path,
-        return_annotated
+        return_annotated,
+        exploded
     )
 
 
 def get_xml_schema(
     lixi_transaction_type=None,
     lixi_version=None,
     custom_version=None,
     schema_string=None,
     schema_path=None,
     output_path=None,
-    return_annotated=False
+    return_annotated=False,
+    exploded=False
 ):
     """Fetches a LIXI XML schema Etree object or converts from an LIXI JSON schema.
     
     Args:  
         lixi_transaction_type (:obj:`str`, optional): The transaction type of the LIXI schema to be fetched. Should be one of 'ACC', 'CAL', 'CDA', 'CNZ', 'DAS', 'LMI', 'SVC', 'VAL'. Defaults to None.   
         lixi_version (:obj:`str`, optional): The version of the LIXI schema to be fetched. Should be in the format of '2.6.24'. Defaults to None. Defaults to the latest version if only lixi_transaction_type is provided.   
         custom_version (:obj:`str`, optional): The version of the LIXI custom schema to be fetched. Usually a complete file name of the custom schema. Defaults to None.   
         schema_string (:obj:`str`, optional): LIXI schema provided as a string. Defaults to None.    
         schema_path (:obj:`str`, optional): LIXI schema provided as a path. Defaults to None.    
         output_path (:obj:`str`, optional): Path to write the fetched lixi schema to. Defaults to None.
         return_annotated (:obj:`boolean`, optional): Variable to indicated if the returned schema should be annotated or not.     
+        exploded (:obj:`boolean`, optional): Variable to indicate if the returned schema should be exploded or not.
 
     Result:   
         A string object of the LIXI XML schema or saved to the output folder specified.    
 
     Raises:   
         LIXIInvalidSyntax: Incorrect schema string/file fetched.    
         LIXIValidationError: Validation errors in the schema string/file fetched.    
@@ -305,15 +310,16 @@
     return _LIXI.getInstance().fetch_xml_schema(
         lixi_transaction_type,
         lixi_version,
         custom_version,
         schema_string,
         schema_path,
         output_path,
-        return_annotated
+        return_annotated,
+        exploded
     )
 
 def get_schema_documentation(
     schema_string, 
     output_folder=None, 
     output_name=None,
     glossary_string = None
```

### Comparing `lixi-0.9.2/lixi/documentation/index.html` & `lixi-0.9.3/lixi/documentation/index.html`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/js/theme.js` & `lixi-0.9.3/lixi/documentation/js/theme.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/js/marked.js` & `lixi-0.9.3/lixi/documentation/js/marked.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/js/LIXI_Glossary.js` & `lixi-0.9.3/lixi/documentation/js/LIXI_Glossary.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/js/LIXI-Master-Schema.js` & `lixi-0.9.3/lixi/documentation/js/LIXI-Master-Schema.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/js/GenerateHTML.js` & `lixi-0.9.3/lixi/documentation/js/GenerateHTML.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/js/vkbeautify.0.99.00.beta.js` & `lixi-0.9.3/lixi/documentation/js/vkbeautify.0.99.00.beta.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/js/jquery-2.1.1.min.js` & `lixi-0.9.3/lixi/documentation/js/jquery-2.1.1.min.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/js/modernizr-2.8.3.min.js` & `lixi-0.9.3/lixi/documentation/js/modernizr-2.8.3.min.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/.gitlab-ci.yml` & `lixi-0.9.3/lixi/documentation/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/fonts/fontawesome-webfont.ttf` & `lixi-0.9.3/lixi/documentation/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/fonts/fontawesome-webfont.woff` & `lixi-0.9.3/lixi/documentation/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/fonts/fontawesome-webfont.svg` & `lixi-0.9.3/lixi/documentation/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/fonts/fontawesome-webfont.eot` & `lixi-0.9.3/lixi/documentation/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/create_documentation.py` & `lixi-0.9.3/lixi/documentation/create_documentation.py`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/css/theme.css` & `lixi-0.9.3/lixi/documentation/css/theme.css`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/css/theme_extra.css` & `lixi-0.9.3/lixi/documentation/css/theme_extra.css`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/css/extra.css` & `lixi-0.9.3/lixi/documentation/css/extra.css`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/css/highlight.css` & `lixi-0.9.3/lixi/documentation/css/highlight.css`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/img/info.png` & `lixi-0.9.3/lixi/documentation/img/info.png`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/img/favicon.ico` & `lixi-0.9.3/lixi/documentation/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/img/wheel.gif` & `lixi-0.9.3/lixi/documentation/img/wheel.gif`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/img/clip.png` & `lixi-0.9.3/lixi/documentation/img/clip.png`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/img/lixi_logo_100.png` & `lixi-0.9.3/lixi/documentation/img/lixi_logo_100.png`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/mkdocs/js/mustache.min.js` & `lixi-0.9.3/lixi/documentation/mkdocs/js/mustache.min.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/mkdocs/js/search.js` & `lixi-0.9.3/lixi/documentation/mkdocs/js/search.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/mkdocs/js/lunr.min.js` & `lixi-0.9.3/lixi/documentation/mkdocs/js/lunr.min.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/mkdocs/js/text.js` & `lixi-0.9.3/lixi/documentation/mkdocs/js/text.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/mkdocs/js/require.js` & `lixi-0.9.3/lixi/documentation/mkdocs/js/require.js`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/documentation/search.html` & `lixi-0.9.3/lixi/documentation/search.html`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/_xslt_transform.py` & `lixi-0.9.3/lixi/_xslt_transform.py`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/_jsonschema_functions.py` & `lixi-0.9.3/lixi/_jsonschema_functions.py`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/_path_functions.py` & `lixi-0.9.3/lixi/_path_functions.py`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/lixi/_xml_to_json.py` & `lixi-0.9.3/lixi/_xml_to_json.py`

 * *Files identical despite different names*

### Comparing `lixi-0.9.2/setup.py` & `lixi-0.9.3/setup.py`

 * *Files identical despite different names*


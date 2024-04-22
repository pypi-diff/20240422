# Comparing `tmp/django_log_inspector-0.0.7.tar.gz` & `tmp/django_log_inspector-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_log_inspector-0.0.7.tar", last modified: Mon Apr 22 08:28:02 2024, max compression
+gzip compressed data, was "django_log_inspector-0.0.8.tar", last modified: Mon Apr 22 08:36:11 2024, max compression
```

## Comparing `django_log_inspector-0.0.7.tar` & `django_log_inspector-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.452511 django_log_inspector-0.0.7/
--rw-r--r--   0 peyman627   (501) staff       (20)     1071 2024-01-23 09:55:45.000000 django_log_inspector-0.0.7/LICENSE
--rw-r--r--   0 peyman627   (501) staff       (20)      100 2024-01-23 12:18:13.000000 django_log_inspector-0.0.7/MANIFEST.in
--rw-r--r--   0 peyman627   (501) staff       (20)     4099 2024-04-22 08:28:02.452324 django_log_inspector-0.0.7/PKG-INFO
--rw-r--r--   0 peyman627   (501) staff       (20)     2219 2024-04-22 08:25:21.000000 django_log_inspector-0.0.7/README.md
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.452082 django_log_inspector-0.0.7/django_log_inspector.egg-info/
--rw-r--r--   0 peyman627   (501) staff       (20)     4099 2024-04-22 08:28:02.000000 django_log_inspector-0.0.7/django_log_inspector.egg-info/PKG-INFO
--rw-r--r--   0 peyman627   (501) staff       (20)     1002 2024-04-22 08:28:02.000000 django_log_inspector-0.0.7/django_log_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 peyman627   (501) staff       (20)        1 2024-04-22 08:28:02.000000 django_log_inspector-0.0.7/django_log_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 peyman627   (501) staff       (20)       14 2024-04-22 08:28:02.000000 django_log_inspector-0.0.7/django_log_inspector.egg-info/top_level.txt
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.444662 django_log_inspector-0.0.7/log_inspector/
--rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.7/log_inspector/__init__.py
--rw-r--r--   0 peyman627   (501) staff       (20)       63 2024-01-23 09:38:31.000000 django_log_inspector-0.0.7/log_inspector/admin.py
--rw-r--r--   0 peyman627   (501) staff       (20)      163 2024-01-23 10:07:05.000000 django_log_inspector-0.0.7/log_inspector/apps.py
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.445086 django_log_inspector-0.0.7/log_inspector/migrations/
--rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.7/log_inspector/migrations/__init__.py
--rw-r--r--   0 peyman627   (501) staff       (20)       57 2024-01-23 09:38:31.000000 django_log_inspector-0.0.7/log_inspector/models.py
--rw-r--r--   0 peyman627   (501) staff       (20)      866 2024-04-21 08:26:12.000000 django_log_inspector-0.0.7/log_inspector/settings.py
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.441393 django_log_inspector-0.0.7/log_inspector/static/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.441513 django_log_inspector-0.0.7/log_inspector/static/log_inspector/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.445490 django_log_inspector-0.0.7/log_inspector/static/log_inspector/css/
--rw-r--r--   0 peyman627   (501) staff       (20)     2023 2024-04-16 12:26:40.000000 django_log_inspector-0.0.7/log_inspector/static/log_inspector/css/input.css
--rw-r--r--   0 peyman627   (501) staff       (20)     9954 2024-04-22 08:22:02.000000 django_log_inspector-0.0.7/log_inspector/static/log_inspector/css/output.css
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.446706 django_log_inspector-0.0.7/log_inspector/static/log_inspector/js/
--rw-r--r--   0 peyman627   (501) staff       (20)    43440 2024-01-05 17:19:20.000000 django_log_inspector-0.0.7/log_inspector/static/log_inspector/js/alpinejs.min.js
--rw-r--r--   0 peyman627   (501) staff       (20)    47755 2024-01-05 17:17:16.000000 django_log_inspector-0.0.7/log_inspector/static/log_inspector/js/htmx.min.js
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.441629 django_log_inspector-0.0.7/log_inspector/templates/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.449822 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/
--rw-r--r--   0 peyman627   (501) staff       (20)    10309 2024-04-22 08:21:59.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/home.html
--rw-r--r--   0 peyman627   (501) staff       (20)     1852 2024-04-16 13:11:49.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_entries_data.html
--rw-r--r--   0 peyman627   (501) staff       (20)      686 2024-04-16 10:49:36.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_entries_table.html
--rw-r--r--   0 peyman627   (501) staff       (20)      988 2024-04-16 13:11:49.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_files.html
--rw-r--r--   0 peyman627   (501) staff       (20)     2645 2024-02-05 11:01:20.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/pagination.html
--rw-r--r--   0 peyman627   (501) staff       (20)     1027 2024-04-16 10:25:08.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/start_live.html
--rw-r--r--   0 peyman627   (501) staff       (20)       60 2024-01-23 09:38:31.000000 django_log_inspector-0.0.7/log_inspector/tests.py
--rw-r--r--   0 peyman627   (501) staff       (20)      700 2024-04-15 12:22:26.000000 django_log_inspector-0.0.7/log_inspector/urls.py
--rw-r--r--   0 peyman627   (501) staff       (20)     2660 2024-04-16 12:09:32.000000 django_log_inspector-0.0.7/log_inspector/utils.py
--rw-r--r--   0 peyman627   (501) staff       (20)     3627 2024-04-16 11:12:12.000000 django_log_inspector-0.0.7/log_inspector/views.py
--rw-r--r--   0 peyman627   (501) staff       (20)      779 2024-04-22 08:25:21.000000 django_log_inspector-0.0.7/pyproject.toml
--rw-r--r--   0 peyman627   (501) staff       (20)       38 2024-04-22 08:28:02.452551 django_log_inspector-0.0.7/setup.cfg
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:36:11.239410 django_log_inspector-0.0.8/
+-rw-r--r--   0 peyman627   (501) staff       (20)     1071 2024-01-23 09:55:45.000000 django_log_inspector-0.0.8/LICENSE
+-rw-r--r--   0 peyman627   (501) staff       (20)      100 2024-01-23 12:18:13.000000 django_log_inspector-0.0.8/MANIFEST.in
+-rw-r--r--   0 peyman627   (501) staff       (20)     4198 2024-04-22 08:36:11.239211 django_log_inspector-0.0.8/PKG-INFO
+-rw-r--r--   0 peyman627   (501) staff       (20)     2318 2024-04-22 08:35:12.000000 django_log_inspector-0.0.8/README.md
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:36:11.238974 django_log_inspector-0.0.8/django_log_inspector.egg-info/
+-rw-r--r--   0 peyman627   (501) staff       (20)     4198 2024-04-22 08:36:11.000000 django_log_inspector-0.0.8/django_log_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 peyman627   (501) staff       (20)     1002 2024-04-22 08:36:11.000000 django_log_inspector-0.0.8/django_log_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 peyman627   (501) staff       (20)        1 2024-04-22 08:36:11.000000 django_log_inspector-0.0.8/django_log_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 peyman627   (501) staff       (20)       14 2024-04-22 08:36:11.000000 django_log_inspector-0.0.8/django_log_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:36:11.233992 django_log_inspector-0.0.8/log_inspector/
+-rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.8/log_inspector/__init__.py
+-rw-r--r--   0 peyman627   (501) staff       (20)       63 2024-01-23 09:38:31.000000 django_log_inspector-0.0.8/log_inspector/admin.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      163 2024-01-23 10:07:05.000000 django_log_inspector-0.0.8/log_inspector/apps.py
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:36:11.234210 django_log_inspector-0.0.8/log_inspector/migrations/
+-rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.8/log_inspector/migrations/__init__.py
+-rw-r--r--   0 peyman627   (501) staff       (20)       57 2024-01-23 09:38:31.000000 django_log_inspector-0.0.8/log_inspector/models.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      866 2024-04-21 08:26:12.000000 django_log_inspector-0.0.8/log_inspector/settings.py
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:36:11.230837 django_log_inspector-0.0.8/log_inspector/static/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:36:11.230956 django_log_inspector-0.0.8/log_inspector/static/log_inspector/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:36:11.234612 django_log_inspector-0.0.8/log_inspector/static/log_inspector/css/
+-rw-r--r--   0 peyman627   (501) staff       (20)     2023 2024-04-16 12:26:40.000000 django_log_inspector-0.0.8/log_inspector/static/log_inspector/css/input.css
+-rw-r--r--   0 peyman627   (501) staff       (20)     9954 2024-04-22 08:22:02.000000 django_log_inspector-0.0.8/log_inspector/static/log_inspector/css/output.css
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:36:11.235768 django_log_inspector-0.0.8/log_inspector/static/log_inspector/js/
+-rw-r--r--   0 peyman627   (501) staff       (20)    43440 2024-01-05 17:19:20.000000 django_log_inspector-0.0.8/log_inspector/static/log_inspector/js/alpinejs.min.js
+-rw-r--r--   0 peyman627   (501) staff       (20)    47755 2024-01-05 17:17:16.000000 django_log_inspector-0.0.8/log_inspector/static/log_inspector/js/htmx.min.js
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:36:11.231074 django_log_inspector-0.0.8/log_inspector/templates/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:36:11.238554 django_log_inspector-0.0.8/log_inspector/templates/log_inspector/
+-rw-r--r--   0 peyman627   (501) staff       (20)    10309 2024-04-22 08:21:59.000000 django_log_inspector-0.0.8/log_inspector/templates/log_inspector/home.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     1852 2024-04-16 13:11:49.000000 django_log_inspector-0.0.8/log_inspector/templates/log_inspector/log_entries_data.html
+-rw-r--r--   0 peyman627   (501) staff       (20)      686 2024-04-16 10:49:36.000000 django_log_inspector-0.0.8/log_inspector/templates/log_inspector/log_entries_table.html
+-rw-r--r--   0 peyman627   (501) staff       (20)      988 2024-04-16 13:11:49.000000 django_log_inspector-0.0.8/log_inspector/templates/log_inspector/log_files.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     2645 2024-02-05 11:01:20.000000 django_log_inspector-0.0.8/log_inspector/templates/log_inspector/pagination.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     1027 2024-04-16 10:25:08.000000 django_log_inspector-0.0.8/log_inspector/templates/log_inspector/start_live.html
+-rw-r--r--   0 peyman627   (501) staff       (20)       60 2024-01-23 09:38:31.000000 django_log_inspector-0.0.8/log_inspector/tests.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      700 2024-04-15 12:22:26.000000 django_log_inspector-0.0.8/log_inspector/urls.py
+-rw-r--r--   0 peyman627   (501) staff       (20)     2660 2024-04-16 12:09:32.000000 django_log_inspector-0.0.8/log_inspector/utils.py
+-rw-r--r--   0 peyman627   (501) staff       (20)     3627 2024-04-16 11:12:12.000000 django_log_inspector-0.0.8/log_inspector/views.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      779 2024-04-22 08:35:12.000000 django_log_inspector-0.0.8/pyproject.toml
+-rw-r--r--   0 peyman627   (501) staff       (20)       38 2024-04-22 08:36:11.239451 django_log_inspector-0.0.8/setup.cfg
```

### Comparing `django_log_inspector-0.0.7/LICENSE` & `django_log_inspector-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/PKG-INFO` & `django_log_inspector-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-inspector
-Version: 0.0.7
+Version: 0.0.8
 Summary: Read and Download log files
 Author-email: Peyman Hassani <hassani.peyman627@gmail.com>, Shaghayegh Valadkhani <valadkhani.sh@gmail.com>
 Maintainer-email: Peyman Hassani <hassani.peyman627@gmail.com>, Shaghayegh Valadkhani <valadkhani.sh@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Peyman Hassani
         
@@ -31,15 +31,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Log Inspector
 
 ## _Fast and Live view to your log files_
 
-![version](https://img.shields.io/badge/version-0.0.7-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.8-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
 It delivers a fast and live-view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
@@ -107,7 +107,13 @@
 
 Logs are only accessible to logged-in superusers.
 If your login URL is different from Django's default, specify it in your settings.
 
 ```
 LOGIN_URL = '/my-custom-admin/login/'
 ```
+
+## Static Files
+Deploy static files by running the command
+```
+python manage.py collectstatic
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.7 Summary: Read
+Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.8 Summary: Read
 and Download log files Author-email: Peyman Hassani
 gmail.com>, Shaghayegh Valadkhani
 gmail.com> Maintainer-email: Peyman Hassani
 gmail.com>, Shaghayegh Valadkhani
 gmail.com> License: MIT License Copyright (c) 2024 Peyman Hassani Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
@@ -19,15 +19,15 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/peyzor/
 django-log-inspector Keywords: Django,logging,log viewer,real-time
 monitoring,log analysis,troubleshooting,log management,log files,log
 monitoring,debugging,Python web development,development tool Description-
 Content-Type: text/markdown License-File: LICENSE # Django Log Inspector ##
 _Fast and Live view to your log files_ ![version](https://img.shields.io/badge/
-version-0.0.7-blue.svg) [![Open Source](https://badges.frapsoft.com/os/v1/open-
+version-0.0.8-blue.svg) [![Open Source](https://badges.frapsoft.com/os/v1/open-
 source.svg?v=103)](https://opensource.org/) _[_G_i_t_H_u_b_]Django Log Inspector offers
 real-time monitoring and analysis of log files in Django projects. It delivers
 a fast and live-view of log data, eliminating manual page refreshing. With an
 intuitive interface and live update functionality, it streamlines log file
 management for easier issue tracking and troubleshooting in Django
 applications. Django Log Inspector is available directly from _P_y_P_I: ##
 Installation ``` pip install django-log-inspector ``` Add in INSTALLED_APPS ```
@@ -42,8 +42,9 @@
 total logs per-page LOG_INSPECTOR_MAX_READ_LINES = 1000 # total logs that are
 read LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String regex expression to
 exclude the log ``` Optionally you can set the next variables in order to
 customize ``` LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title" # default: None
 LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" # default: None
 ``` ## Login Logs are only accessible to logged-in superusers. If your login
 URL is different from Django's default, specify it in your settings. ```
-LOGIN_URL = '/my-custom-admin/login/' ```
+LOGIN_URL = '/my-custom-admin/login/' ``` ## Static Files Deploy static files
+by running the command ``` python manage.py collectstatic ```
```

### Comparing `django_log_inspector-0.0.7/README.md` & `django_log_inspector-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Django Log Inspector
 
 ## _Fast and Live view to your log files_
 
-![version](https://img.shields.io/badge/version-0.0.7-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.8-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
 It delivers a fast and live-view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
@@ -73,8 +73,14 @@
 ## Login
 
 Logs are only accessible to logged-in superusers.
 If your login URL is different from Django's default, specify it in your settings.
 
 ```
 LOGIN_URL = '/my-custom-admin/login/'
+```
+
+## Static Files
+Deploy static files by running the command
+```
+python manage.py collectstatic
 ```
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # Django Log Inspector ## _Fast and Live view to your log files_ ![version]
-(https://img.shields.io/badge/version-0.0.7-blue.svg) [![Open Source](https://
+(https://img.shields.io/badge/version-0.0.8-blue.svg) [![Open Source](https://
 badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 _[_G_i_t_H_u_b_]Django Log Inspector offers real-time monitoring and analysis of log
 files in Django projects. It delivers a fast and live-view of log data,
 eliminating manual page refreshing. With an intuitive interface and live update
 functionality, it streamlines log file management for easier issue tracking and
 troubleshooting in Django applications. Django Log Inspector is available
 directly from _P_y_P_I: ## Installation ``` pip install django-log-inspector ```
@@ -19,8 +19,9 @@
 LOG_INSPECTOR_MAX_READ_LINES = 1000 # total logs that are read
 LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String regex expression to exclude
 the log ``` Optionally you can set the next variables in order to customize ```
 LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title" # default: None
 LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" # default: None
 ``` ## Login Logs are only accessible to logged-in superusers. If your login
 URL is different from Django's default, specify it in your settings. ```
-LOGIN_URL = '/my-custom-admin/login/' ```
+LOGIN_URL = '/my-custom-admin/login/' ``` ## Static Files Deploy static files
+by running the command ``` python manage.py collectstatic ```
```

### Comparing `django_log_inspector-0.0.7/django_log_inspector.egg-info/PKG-INFO` & `django_log_inspector-0.0.8/django_log_inspector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-inspector
-Version: 0.0.7
+Version: 0.0.8
 Summary: Read and Download log files
 Author-email: Peyman Hassani <hassani.peyman627@gmail.com>, Shaghayegh Valadkhani <valadkhani.sh@gmail.com>
 Maintainer-email: Peyman Hassani <hassani.peyman627@gmail.com>, Shaghayegh Valadkhani <valadkhani.sh@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Peyman Hassani
         
@@ -31,15 +31,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Log Inspector
 
 ## _Fast and Live view to your log files_
 
-![version](https://img.shields.io/badge/version-0.0.7-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.8-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
 It delivers a fast and live-view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
@@ -107,7 +107,13 @@
 
 Logs are only accessible to logged-in superusers.
 If your login URL is different from Django's default, specify it in your settings.
 
 ```
 LOGIN_URL = '/my-custom-admin/login/'
 ```
+
+## Static Files
+Deploy static files by running the command
+```
+python manage.py collectstatic
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.7 Summary: Read
+Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.8 Summary: Read
 and Download log files Author-email: Peyman Hassani
 gmail.com>, Shaghayegh Valadkhani
 gmail.com> Maintainer-email: Peyman Hassani
 gmail.com>, Shaghayegh Valadkhani
 gmail.com> License: MIT License Copyright (c) 2024 Peyman Hassani Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
@@ -19,15 +19,15 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/peyzor/
 django-log-inspector Keywords: Django,logging,log viewer,real-time
 monitoring,log analysis,troubleshooting,log management,log files,log
 monitoring,debugging,Python web development,development tool Description-
 Content-Type: text/markdown License-File: LICENSE # Django Log Inspector ##
 _Fast and Live view to your log files_ ![version](https://img.shields.io/badge/
-version-0.0.7-blue.svg) [![Open Source](https://badges.frapsoft.com/os/v1/open-
+version-0.0.8-blue.svg) [![Open Source](https://badges.frapsoft.com/os/v1/open-
 source.svg?v=103)](https://opensource.org/) _[_G_i_t_H_u_b_]Django Log Inspector offers
 real-time monitoring and analysis of log files in Django projects. It delivers
 a fast and live-view of log data, eliminating manual page refreshing. With an
 intuitive interface and live update functionality, it streamlines log file
 management for easier issue tracking and troubleshooting in Django
 applications. Django Log Inspector is available directly from _P_y_P_I: ##
 Installation ``` pip install django-log-inspector ``` Add in INSTALLED_APPS ```
@@ -42,8 +42,9 @@
 total logs per-page LOG_INSPECTOR_MAX_READ_LINES = 1000 # total logs that are
 read LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String regex expression to
 exclude the log ``` Optionally you can set the next variables in order to
 customize ``` LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title" # default: None
 LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" # default: None
 ``` ## Login Logs are only accessible to logged-in superusers. If your login
 URL is different from Django's default, specify it in your settings. ```
-LOGIN_URL = '/my-custom-admin/login/' ```
+LOGIN_URL = '/my-custom-admin/login/' ``` ## Static Files Deploy static files
+by running the command ``` python manage.py collectstatic ```
```

### Comparing `django_log_inspector-0.0.7/django_log_inspector.egg-info/SOURCES.txt` & `django_log_inspector-0.0.8/django_log_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/settings.py` & `django_log_inspector-0.0.8/log_inspector/settings.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/static/log_inspector/css/input.css` & `django_log_inspector-0.0.8/log_inspector/static/log_inspector/css/input.css`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/static/log_inspector/css/output.css` & `django_log_inspector-0.0.8/log_inspector/static/log_inspector/css/output.css`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/static/log_inspector/js/alpinejs.min.js` & `django_log_inspector-0.0.8/log_inspector/static/log_inspector/js/alpinejs.min.js`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/static/log_inspector/js/htmx.min.js` & `django_log_inspector-0.0.8/log_inspector/static/log_inspector/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/home.html` & `django_log_inspector-0.0.8/log_inspector/templates/log_inspector/home.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_entries_data.html` & `django_log_inspector-0.0.8/log_inspector/templates/log_inspector/log_entries_data.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_entries_table.html` & `django_log_inspector-0.0.8/log_inspector/templates/log_inspector/log_entries_table.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_files.html` & `django_log_inspector-0.0.8/log_inspector/templates/log_inspector/log_files.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/pagination.html` & `django_log_inspector-0.0.8/log_inspector/templates/log_inspector/pagination.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/start_live.html` & `django_log_inspector-0.0.8/log_inspector/templates/log_inspector/start_live.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/urls.py` & `django_log_inspector-0.0.8/log_inspector/urls.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/utils.py` & `django_log_inspector-0.0.8/log_inspector/utils.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/log_inspector/views.py` & `django_log_inspector-0.0.8/log_inspector/views.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.7/pyproject.toml` & `django_log_inspector-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     { name = "Peyman Hassani", email = "hassani.peyman627@gmail.com" },
     { name = "Shaghayegh Valadkhani", email = "valadkhani.sh@gmail.com" },
 ]
 maintainers = [
     { name = "Peyman Hassani", email = "hassani.peyman627@gmail.com" },
     { name = "Shaghayegh Valadkhani", email = "valadkhani.sh@gmail.com" },
 ]
-version = "0.0.7"
+version = "0.0.8"
 description = "Read and Download log files"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [
     "Django", "logging", "log viewer", "real-time monitoring", "log analysis", "troubleshooting",
     "log management", "log files", "log monitoring", "debugging", "Python web development", "development tool"
 ]
```


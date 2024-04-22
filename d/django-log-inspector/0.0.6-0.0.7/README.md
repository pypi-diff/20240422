# Comparing `tmp/django_log_inspector-0.0.6.tar.gz` & `tmp/django_log_inspector-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_log_inspector-0.0.6.tar", last modified: Sun Apr 21 10:31:17 2024, max compression
+gzip compressed data, was "django_log_inspector-0.0.7.tar", last modified: Mon Apr 22 08:28:02 2024, max compression
```

## Comparing `django_log_inspector-0.0.6.tar` & `django_log_inspector-0.0.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.066179 django_log_inspector-0.0.6/
--rw-r--r--   0 peyman627   (501) staff       (20)     1071 2024-01-23 09:55:45.000000 django_log_inspector-0.0.6/LICENSE
--rw-r--r--   0 peyman627   (501) staff       (20)      100 2024-01-23 12:18:13.000000 django_log_inspector-0.0.6/MANIFEST.in
--rw-r--r--   0 peyman627   (501) staff       (20)     4109 2024-04-21 10:31:17.065987 django_log_inspector-0.0.6/PKG-INFO
--rw-r--r--   0 peyman627   (501) staff       (20)     2229 2024-04-21 10:12:03.000000 django_log_inspector-0.0.6/README.md
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.065629 django_log_inspector-0.0.6/django_log_inspector.egg-info/
--rw-r--r--   0 peyman627   (501) staff       (20)     4109 2024-04-21 10:31:17.000000 django_log_inspector-0.0.6/django_log_inspector.egg-info/PKG-INFO
--rw-r--r--   0 peyman627   (501) staff       (20)     1002 2024-04-21 10:31:17.000000 django_log_inspector-0.0.6/django_log_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 peyman627   (501) staff       (20)        1 2024-04-21 10:31:17.000000 django_log_inspector-0.0.6/django_log_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 peyman627   (501) staff       (20)       14 2024-04-21 10:31:17.000000 django_log_inspector-0.0.6/django_log_inspector.egg-info/top_level.txt
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.059817 django_log_inspector-0.0.6/log_inspector/
--rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.6/log_inspector/__init__.py
--rw-r--r--   0 peyman627   (501) staff       (20)       63 2024-01-23 09:38:31.000000 django_log_inspector-0.0.6/log_inspector/admin.py
--rw-r--r--   0 peyman627   (501) staff       (20)      163 2024-01-23 10:07:05.000000 django_log_inspector-0.0.6/log_inspector/apps.py
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.060217 django_log_inspector-0.0.6/log_inspector/migrations/
--rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.6/log_inspector/migrations/__init__.py
--rw-r--r--   0 peyman627   (501) staff       (20)       57 2024-01-23 09:38:31.000000 django_log_inspector-0.0.6/log_inspector/models.py
--rw-r--r--   0 peyman627   (501) staff       (20)      866 2024-04-21 08:26:12.000000 django_log_inspector-0.0.6/log_inspector/settings.py
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.056187 django_log_inspector-0.0.6/log_inspector/static/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.056360 django_log_inspector-0.0.6/log_inspector/static/log_inspector/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.060623 django_log_inspector-0.0.6/log_inspector/static/log_inspector/css/
--rw-r--r--   0 peyman627   (501) staff       (20)     2023 2024-04-16 12:26:40.000000 django_log_inspector-0.0.6/log_inspector/static/log_inspector/css/input.css
--rw-r--r--   0 peyman627   (501) staff       (20)    10025 2024-04-16 13:11:49.000000 django_log_inspector-0.0.6/log_inspector/static/log_inspector/css/output.css
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.062240 django_log_inspector-0.0.6/log_inspector/static/log_inspector/js/
--rw-r--r--   0 peyman627   (501) staff       (20)    43440 2024-01-05 17:19:20.000000 django_log_inspector-0.0.6/log_inspector/static/log_inspector/js/alpinejs.min.js
--rw-r--r--   0 peyman627   (501) staff       (20)    47755 2024-01-05 17:17:16.000000 django_log_inspector-0.0.6/log_inspector/static/log_inspector/js/htmx.min.js
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.056495 django_log_inspector-0.0.6/log_inspector/templates/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-21 10:31:17.065322 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/
--rw-r--r--   0 peyman627   (501) staff       (20)     9719 2024-04-16 13:11:49.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/home.html
--rw-r--r--   0 peyman627   (501) staff       (20)     1852 2024-04-16 13:11:49.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_entries_data.html
--rw-r--r--   0 peyman627   (501) staff       (20)      686 2024-04-16 10:49:36.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_entries_table.html
--rw-r--r--   0 peyman627   (501) staff       (20)      988 2024-04-16 13:11:49.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_files.html
--rw-r--r--   0 peyman627   (501) staff       (20)     2645 2024-02-05 11:01:20.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/pagination.html
--rw-r--r--   0 peyman627   (501) staff       (20)     1027 2024-04-16 10:25:08.000000 django_log_inspector-0.0.6/log_inspector/templates/log_inspector/start_live.html
--rw-r--r--   0 peyman627   (501) staff       (20)       60 2024-01-23 09:38:31.000000 django_log_inspector-0.0.6/log_inspector/tests.py
--rw-r--r--   0 peyman627   (501) staff       (20)      700 2024-04-15 12:22:26.000000 django_log_inspector-0.0.6/log_inspector/urls.py
--rw-r--r--   0 peyman627   (501) staff       (20)     2660 2024-04-16 12:09:32.000000 django_log_inspector-0.0.6/log_inspector/utils.py
--rw-r--r--   0 peyman627   (501) staff       (20)     3627 2024-04-16 11:12:12.000000 django_log_inspector-0.0.6/log_inspector/views.py
--rw-r--r--   0 peyman627   (501) staff       (20)      779 2024-04-21 10:28:42.000000 django_log_inspector-0.0.6/pyproject.toml
--rw-r--r--   0 peyman627   (501) staff       (20)       38 2024-04-21 10:31:17.066333 django_log_inspector-0.0.6/setup.cfg
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.452511 django_log_inspector-0.0.7/
+-rw-r--r--   0 peyman627   (501) staff       (20)     1071 2024-01-23 09:55:45.000000 django_log_inspector-0.0.7/LICENSE
+-rw-r--r--   0 peyman627   (501) staff       (20)      100 2024-01-23 12:18:13.000000 django_log_inspector-0.0.7/MANIFEST.in
+-rw-r--r--   0 peyman627   (501) staff       (20)     4099 2024-04-22 08:28:02.452324 django_log_inspector-0.0.7/PKG-INFO
+-rw-r--r--   0 peyman627   (501) staff       (20)     2219 2024-04-22 08:25:21.000000 django_log_inspector-0.0.7/README.md
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.452082 django_log_inspector-0.0.7/django_log_inspector.egg-info/
+-rw-r--r--   0 peyman627   (501) staff       (20)     4099 2024-04-22 08:28:02.000000 django_log_inspector-0.0.7/django_log_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 peyman627   (501) staff       (20)     1002 2024-04-22 08:28:02.000000 django_log_inspector-0.0.7/django_log_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 peyman627   (501) staff       (20)        1 2024-04-22 08:28:02.000000 django_log_inspector-0.0.7/django_log_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 peyman627   (501) staff       (20)       14 2024-04-22 08:28:02.000000 django_log_inspector-0.0.7/django_log_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.444662 django_log_inspector-0.0.7/log_inspector/
+-rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.7/log_inspector/__init__.py
+-rw-r--r--   0 peyman627   (501) staff       (20)       63 2024-01-23 09:38:31.000000 django_log_inspector-0.0.7/log_inspector/admin.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      163 2024-01-23 10:07:05.000000 django_log_inspector-0.0.7/log_inspector/apps.py
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.445086 django_log_inspector-0.0.7/log_inspector/migrations/
+-rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.7/log_inspector/migrations/__init__.py
+-rw-r--r--   0 peyman627   (501) staff       (20)       57 2024-01-23 09:38:31.000000 django_log_inspector-0.0.7/log_inspector/models.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      866 2024-04-21 08:26:12.000000 django_log_inspector-0.0.7/log_inspector/settings.py
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.441393 django_log_inspector-0.0.7/log_inspector/static/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.441513 django_log_inspector-0.0.7/log_inspector/static/log_inspector/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.445490 django_log_inspector-0.0.7/log_inspector/static/log_inspector/css/
+-rw-r--r--   0 peyman627   (501) staff       (20)     2023 2024-04-16 12:26:40.000000 django_log_inspector-0.0.7/log_inspector/static/log_inspector/css/input.css
+-rw-r--r--   0 peyman627   (501) staff       (20)     9954 2024-04-22 08:22:02.000000 django_log_inspector-0.0.7/log_inspector/static/log_inspector/css/output.css
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.446706 django_log_inspector-0.0.7/log_inspector/static/log_inspector/js/
+-rw-r--r--   0 peyman627   (501) staff       (20)    43440 2024-01-05 17:19:20.000000 django_log_inspector-0.0.7/log_inspector/static/log_inspector/js/alpinejs.min.js
+-rw-r--r--   0 peyman627   (501) staff       (20)    47755 2024-01-05 17:17:16.000000 django_log_inspector-0.0.7/log_inspector/static/log_inspector/js/htmx.min.js
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.441629 django_log_inspector-0.0.7/log_inspector/templates/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-22 08:28:02.449822 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/
+-rw-r--r--   0 peyman627   (501) staff       (20)    10309 2024-04-22 08:21:59.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/home.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     1852 2024-04-16 13:11:49.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_entries_data.html
+-rw-r--r--   0 peyman627   (501) staff       (20)      686 2024-04-16 10:49:36.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_entries_table.html
+-rw-r--r--   0 peyman627   (501) staff       (20)      988 2024-04-16 13:11:49.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_files.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     2645 2024-02-05 11:01:20.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/pagination.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     1027 2024-04-16 10:25:08.000000 django_log_inspector-0.0.7/log_inspector/templates/log_inspector/start_live.html
+-rw-r--r--   0 peyman627   (501) staff       (20)       60 2024-01-23 09:38:31.000000 django_log_inspector-0.0.7/log_inspector/tests.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      700 2024-04-15 12:22:26.000000 django_log_inspector-0.0.7/log_inspector/urls.py
+-rw-r--r--   0 peyman627   (501) staff       (20)     2660 2024-04-16 12:09:32.000000 django_log_inspector-0.0.7/log_inspector/utils.py
+-rw-r--r--   0 peyman627   (501) staff       (20)     3627 2024-04-16 11:12:12.000000 django_log_inspector-0.0.7/log_inspector/views.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      779 2024-04-22 08:25:21.000000 django_log_inspector-0.0.7/pyproject.toml
+-rw-r--r--   0 peyman627   (501) staff       (20)       38 2024-04-22 08:28:02.452551 django_log_inspector-0.0.7/setup.cfg
```

### Comparing `django_log_inspector-0.0.6/LICENSE` & `django_log_inspector-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/PKG-INFO` & `django_log_inspector-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-inspector
-Version: 0.0.6
+Version: 0.0.7
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
 
-![version](https://img.shields.io/badge/version-0.0.6-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.7-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
 It delivers a fast and live-view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
@@ -87,16 +87,16 @@
 ```
  LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]', '[ERROR]', '[CRITICAL]']
 ```
 
 How logs are displayed
 
 ```
- LOG_INSPECTOR_PAGE_LENGTH = 25             # total log lines per-page
- LOG_INSPECTOR_MAX_READ_LINES = 1000        # total log lines that are read
+ LOG_INSPECTOR_PAGE_LENGTH = 25             # total logs per-page
+ LOG_INSPECTOR_MAX_READ_LINES = 1000        # total logs that are read
  LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None  # String regex expression to exclude the log
 ```
 
 Optionally you can set the next variables in order to customize
 
 ```
 LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title"               # default: None
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.6 Summary: Read
+Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.7 Summary: Read
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
-version-0.0.6-blue.svg) [![Open Source](https://badges.frapsoft.com/os/v1/open-
+version-0.0.7-blue.svg) [![Open Source](https://badges.frapsoft.com/os/v1/open-
 source.svg?v=103)](https://opensource.org/) _[_G_i_t_H_u_b_]Django Log Inspector offers
 real-time monitoring and analysis of log files in Django projects. It delivers
 a fast and live-view of log data, eliminating manual page refreshing. With an
 intuitive interface and live update functionality, it streamlines log file
 management for easier issue tracking and troubleshooting in Django
 applications. Django Log Inspector is available directly from _P_y_P_I: ##
 Installation ``` pip install django-log-inspector ``` Add in INSTALLED_APPS ```
@@ -35,15 +35,15 @@
 ('logs/', include('log_inspector.urls')) ``` ## Settings The directory of log
 files in your project ``` LOG_INSPECTOR_FILES_DIR = 'logs/' ``` A file is
 included if the pattern is matched, or it is specified ``` LOG_INSPECTOR_FILES
 = ['logfile1', 'logfile2', ...] # default: [] LOG_INSPECTOR_FILES_PATTERN =
 '*.log*' ``` You must specify the patterns in which your log files start with
 ``` LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]', '[ERROR]', '
 [CRITICAL]'] ``` How logs are displayed ``` LOG_INSPECTOR_PAGE_LENGTH = 25 #
-total log lines per-page LOG_INSPECTOR_MAX_READ_LINES = 1000 # total log lines
-that are read LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String regex
-expression to exclude the log ``` Optionally you can set the next variables in
-order to customize ``` LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title" #
-default: None LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" #
-default: None ``` ## Login Logs are only accessible to logged-in superusers. If
-your login URL is different from Django's default, specify it in your settings.
-``` LOGIN_URL = '/my-custom-admin/login/' ```
+total logs per-page LOG_INSPECTOR_MAX_READ_LINES = 1000 # total logs that are
+read LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String regex expression to
+exclude the log ``` Optionally you can set the next variables in order to
+customize ``` LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title" # default: None
+LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" # default: None
+``` ## Login Logs are only accessible to logged-in superusers. If your login
+URL is different from Django's default, specify it in your settings. ```
+LOGIN_URL = '/my-custom-admin/login/' ```
```

### Comparing `django_log_inspector-0.0.6/README.md` & `django_log_inspector-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Django Log Inspector
 
 ## _Fast and Live view to your log files_
 
-![version](https://img.shields.io/badge/version-0.0.6-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.7-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
 It delivers a fast and live-view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
@@ -54,16 +54,16 @@
 ```
  LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]', '[ERROR]', '[CRITICAL]']
 ```
 
 How logs are displayed
 
 ```
- LOG_INSPECTOR_PAGE_LENGTH = 25             # total log lines per-page
- LOG_INSPECTOR_MAX_READ_LINES = 1000        # total log lines that are read
+ LOG_INSPECTOR_PAGE_LENGTH = 25             # total logs per-page
+ LOG_INSPECTOR_MAX_READ_LINES = 1000        # total logs that are read
  LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None  # String regex expression to exclude the log
 ```
 
 Optionally you can set the next variables in order to customize
 
 ```
 LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title"               # default: None
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # Django Log Inspector ## _Fast and Live view to your log files_ ![version]
-(https://img.shields.io/badge/version-0.0.6-blue.svg) [![Open Source](https://
+(https://img.shields.io/badge/version-0.0.7-blue.svg) [![Open Source](https://
 badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 _[_G_i_t_H_u_b_]Django Log Inspector offers real-time monitoring and analysis of log
 files in Django projects. It delivers a fast and live-view of log data,
 eliminating manual page refreshing. With an intuitive interface and live update
 functionality, it streamlines log file management for easier issue tracking and
 troubleshooting in Django applications. Django Log Inspector is available
 directly from _P_y_P_I: ## Installation ``` pip install django-log-inspector ```
@@ -11,16 +11,16 @@
 in the URLconf ``` path('logs/', include('log_inspector.urls')) ``` ## Settings
 The directory of log files in your project ``` LOG_INSPECTOR_FILES_DIR = 'logs/
 ' ``` A file is included if the pattern is matched, or it is specified ```
 LOG_INSPECTOR_FILES = ['logfile1', 'logfile2', ...] # default: []
 LOG_INSPECTOR_FILES_PATTERN = '*.log*' ``` You must specify the patterns in
 which your log files start with ``` LOG_INSPECTOR_PATTERNS = ['[INFO]', '
 [DEBUG]', '[WARNING]', '[ERROR]', '[CRITICAL]'] ``` How logs are displayed ```
-LOG_INSPECTOR_PAGE_LENGTH = 25 # total log lines per-page
-LOG_INSPECTOR_MAX_READ_LINES = 1000 # total log lines that are read
+LOG_INSPECTOR_PAGE_LENGTH = 25 # total logs per-page
+LOG_INSPECTOR_MAX_READ_LINES = 1000 # total logs that are read
 LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String regex expression to exclude
 the log ``` Optionally you can set the next variables in order to customize ```
 LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title" # default: None
 LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" # default: None
 ``` ## Login Logs are only accessible to logged-in superusers. If your login
 URL is different from Django's default, specify it in your settings. ```
 LOGIN_URL = '/my-custom-admin/login/' ```
```

### Comparing `django_log_inspector-0.0.6/django_log_inspector.egg-info/PKG-INFO` & `django_log_inspector-0.0.7/django_log_inspector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-inspector
-Version: 0.0.6
+Version: 0.0.7
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
 
-![version](https://img.shields.io/badge/version-0.0.6-blue.svg)
+![version](https://img.shields.io/badge/version-0.0.7-blue.svg)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 <a href="https://github.com/peyzor/django-log-inspector"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
 
 Django Log Inspector offers real-time monitoring and analysis of log files in Django projects.
 It delivers a fast and live-view of log data, eliminating manual page refreshing.
 With an intuitive interface and live update functionality, it streamlines log file management for easier issue tracking
 and troubleshooting in Django applications.
@@ -87,16 +87,16 @@
 ```
  LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]', '[ERROR]', '[CRITICAL]']
 ```
 
 How logs are displayed
 
 ```
- LOG_INSPECTOR_PAGE_LENGTH = 25             # total log lines per-page
- LOG_INSPECTOR_MAX_READ_LINES = 1000        # total log lines that are read
+ LOG_INSPECTOR_PAGE_LENGTH = 25             # total logs per-page
+ LOG_INSPECTOR_MAX_READ_LINES = 1000        # total logs that are read
  LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None  # String regex expression to exclude the log
 ```
 
 Optionally you can set the next variables in order to customize
 
 ```
 LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title"               # default: None
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.6 Summary: Read
+Metadata-Version: 2.1 Name: django-log-inspector Version: 0.0.7 Summary: Read
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
-version-0.0.6-blue.svg) [![Open Source](https://badges.frapsoft.com/os/v1/open-
+version-0.0.7-blue.svg) [![Open Source](https://badges.frapsoft.com/os/v1/open-
 source.svg?v=103)](https://opensource.org/) _[_G_i_t_H_u_b_]Django Log Inspector offers
 real-time monitoring and analysis of log files in Django projects. It delivers
 a fast and live-view of log data, eliminating manual page refreshing. With an
 intuitive interface and live update functionality, it streamlines log file
 management for easier issue tracking and troubleshooting in Django
 applications. Django Log Inspector is available directly from _P_y_P_I: ##
 Installation ``` pip install django-log-inspector ``` Add in INSTALLED_APPS ```
@@ -35,15 +35,15 @@
 ('logs/', include('log_inspector.urls')) ``` ## Settings The directory of log
 files in your project ``` LOG_INSPECTOR_FILES_DIR = 'logs/' ``` A file is
 included if the pattern is matched, or it is specified ``` LOG_INSPECTOR_FILES
 = ['logfile1', 'logfile2', ...] # default: [] LOG_INSPECTOR_FILES_PATTERN =
 '*.log*' ``` You must specify the patterns in which your log files start with
 ``` LOG_INSPECTOR_PATTERNS = ['[INFO]', '[DEBUG]', '[WARNING]', '[ERROR]', '
 [CRITICAL]'] ``` How logs are displayed ``` LOG_INSPECTOR_PAGE_LENGTH = 25 #
-total log lines per-page LOG_INSPECTOR_MAX_READ_LINES = 1000 # total log lines
-that are read LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String regex
-expression to exclude the log ``` Optionally you can set the next variables in
-order to customize ``` LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title" #
-default: None LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" #
-default: None ``` ## Login Logs are only accessible to logged-in superusers. If
-your login URL is different from Django's default, specify it in your settings.
-``` LOGIN_URL = '/my-custom-admin/login/' ```
+total logs per-page LOG_INSPECTOR_MAX_READ_LINES = 1000 # total logs that are
+read LOG_INSPECTOR_EXCLUDE_TEXT_PATTERN = None # String regex expression to
+exclude the log ``` Optionally you can set the next variables in order to
+customize ``` LOG_INSPECTOR_FILE_LIST_TITLE = "Custom title" # default: None
+LOG_INSPECTOR_FILE_LIST_STYLES = "/static/css/my-custom.css" # default: None
+``` ## Login Logs are only accessible to logged-in superusers. If your login
+URL is different from Django's default, specify it in your settings. ```
+LOGIN_URL = '/my-custom-admin/login/' ```
```

### Comparing `django_log_inspector-0.0.6/django_log_inspector.egg-info/SOURCES.txt` & `django_log_inspector-0.0.7/django_log_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/settings.py` & `django_log_inspector-0.0.7/log_inspector/settings.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/static/log_inspector/css/input.css` & `django_log_inspector-0.0.7/log_inspector/static/log_inspector/css/input.css`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/static/log_inspector/css/output.css` & `django_log_inspector-0.0.7/log_inspector/static/log_inspector/css/output.css`

 * *Files 5% similar despite different names*

```diff
@@ -1 +1 @@
-/*! tailwindcss v3.4.3 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}:host,html{-webkit-text-size-adjust:100%;font-feature-settings:normal;-webkit-tap-highlight-color:transparent;font-family:ui-sans-serif,system-ui,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-feature-settings:normal;font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em;font-variation-settings:normal}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{font-feature-settings:inherit;color:inherit;font-family:inherit;font-size:100%;font-variation-settings:inherit;font-weight:inherit;letter-spacing:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}*,::backdrop,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.bottom-3{bottom:.75rem}.right-0{right:0}.right-3{right:.75rem}.top-0{top:0}.z-20{z-index:20}.float-right{float:right}.mx-2{margin-left:.5rem;margin-right:.5rem}.mx-auto{margin-left:auto;margin-right:auto}.mb-6{margin-bottom:1.5rem}.ml-6{margin-left:1.5rem}.mr-8{margin-right:2rem}.mt-1{margin-top:.25rem}.mt-2{margin-top:.5rem}.mt-4{margin-top:1rem}.mt-6{margin-top:1.5rem}.box-border{box-sizing:border-box}.block{display:block}.flex{display:flex}.table{display:table}.h-10{height:2.5rem}.w-10{width:2.5rem}.w-2\/5{width:40%}.w-3\/12{width:25%}.w-9\/12{width:75%}.w-full{width:100%}.min-w-0{min-width:0}.max-w-sm{max-width:24rem}.flex-none{flex:none}.flex-grow{flex-grow:1}.table-fixed{table-layout:fixed}.border-collapse{border-collapse:collapse}.cursor-pointer{cursor:pointer}.items-center{align-items:center}.justify-center{justify-content:center}.overflow-hidden{overflow:hidden}.break-words{overflow-wrap:break-word}.break-all{word-break:break-all}.rounded{border-radius:.25rem}.rounded-md{border-radius:.375rem}.rounded-l{border-bottom-left-radius:.25rem;border-top-left-radius:.25rem}.rounded-r{border-bottom-right-radius:.25rem;border-top-right-radius:.25rem}.border{border-width:1px}.border-2{border-width:2px}.border-gray-300{--tw-border-opacity:1;border-color:rgb(209 213 219/var(--tw-border-opacity))}.border-green-300{--tw-border-opacity:1;border-color:rgb(134 239 172/var(--tw-border-opacity))}.bg-blue-500{--tw-bg-opacity:1;background-color:rgb(59 130 246/var(--tw-bg-opacity))}.bg-green-100{--tw-bg-opacity:1;background-color:rgb(220 252 231/var(--tw-bg-opacity))}.bg-green-500{--tw-bg-opacity:1;background-color:rgb(34 197 94/var(--tw-bg-opacity))}.bg-red-500{--tw-bg-opacity:1;background-color:rgb(239 68 68/var(--tw-bg-opacity))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.p-2{padding:.5rem}.p-3{padding:.75rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.px-4{padding-left:1rem;padding-right:1rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-3{padding-bottom:.75rem;padding-top:.75rem}.pl-1{padding-left:.25rem}.pr-2{padding-right:.5rem}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.font-bold{font-weight:700}.text-black{--tw-text-opacity:1;color:rgb(0 0 0/var(--tw-text-opacity))}.text-green-600{--tw-text-opacity:1;color:rgb(22 163 74/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.shadow-md{--tw-shadow:0 4px 6px -1px #0000001a,0 2px 4px -2px #0000001a;--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color),0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-300{transition-duration:.3s}body{overflow-y:scroll!important}.log-entry-text{white-space:pre-wrap}.lds-roller{display:inline-block;height:80px;position:relative;width:80px}.lds-roller div{animation:lds-roller 1.2s cubic-bezier(.5,0,.5,1) infinite;transform-origin:40px 40px}.lds-roller div:after{background:#fff;border-radius:50%;content:" ";display:block;height:7px;margin:-4px 0 0 -4px;position:absolute;width:7px}.lds-roller div:first-child{animation-delay:-36ms}.lds-roller div:first-child:after{left:63px;top:63px}.lds-roller div:nth-child(2){animation-delay:-72ms}.lds-roller div:nth-child(2):after{left:56px;top:68px}.lds-roller div:nth-child(3){animation-delay:-.108s}.lds-roller div:nth-child(3):after{left:48px;top:71px}.lds-roller div:nth-child(4){animation-delay:-.144s}.lds-roller div:nth-child(4):after{left:40px;top:72px}.lds-roller div:nth-child(5){animation-delay:-.18s}.lds-roller div:nth-child(5):after{left:32px;top:71px}.lds-roller div:nth-child(6){animation-delay:-.216s}.lds-roller div:nth-child(6):after{left:24px;top:68px}.lds-roller div:nth-child(7){animation-delay:-.252s}.lds-roller div:nth-child(7):after{left:17px;top:63px}.lds-roller div:nth-child(8){animation-delay:-.288s}.lds-roller div:nth-child(8):after{left:12px;top:56px}@keyframes lds-roller{0%{transform:rotate(0deg)}to{transform:rotate(1turn)}}.loading-spinner{align-items:center;background-color:#0009;display:flex;height:100vh;justify-content:center;left:0;position:fixed;top:0;width:100vw;z-index:10000}.hover\:bg-gray-100:hover{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.focus\:border-blue-500:focus{--tw-border-opacity:1;border-color:rgb(59 130 246/var(--tw-border-opacity))}.focus\:outline-none:focus{outline:2px solid #0000;outline-offset:2px}.dark\:border-gray-100\/50:is(.dark *){border-color:#f3f4f680}.dark\:border-gray-600:is(.dark *){--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity))}.dark\:border-gray-700:is(.dark *){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}.dark\:border-b-gray-100\/50:is(.dark *){border-bottom-color:#f3f4f680}.dark\:bg-blue-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(29 78 216/var(--tw-bg-opacity))}.dark\:bg-gray-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.dark\:bg-green-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(21 128 61/var(--tw-bg-opacity))}.dark\:bg-red-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(185 28 28/var(--tw-bg-opacity))}.dark\:bg-slate-600:is(.dark *){--tw-bg-opacity:1;background-color:rgb(71 85 105/var(--tw-bg-opacity))}.dark\:bg-slate-700:is(.dark *){--tw-bg-opacity:1;background-color:rgb(51 65 85/var(--tw-bg-opacity))}.dark\:bg-slate-800:is(.dark *){--tw-bg-opacity:1;background-color:rgb(30 41 59/var(--tw-bg-opacity))}.dark\:text-white:is(.dark *){--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.dark\:hover\:bg-gray-500:hover:is(.dark *){--tw-bg-opacity:1;background-color:rgb(107 114 128/var(--tw-bg-opacity))}
+/*! tailwindcss v3.4.1 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}:host,html{-webkit-text-size-adjust:100%;font-feature-settings:normal;-webkit-tap-highlight-color:transparent;font-family:ui-sans-serif,system-ui,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-feature-settings:normal;font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em;font-variation-settings:normal}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{font-feature-settings:inherit;color:inherit;font-family:inherit;font-size:100%;font-variation-settings:inherit;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}*,::backdrop,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.bottom-3{bottom:.75rem}.right-0{right:0}.right-3{right:.75rem}.top-0{top:0}.z-20{z-index:20}.float-right{float:right}.mx-1{margin-left:.25rem;margin-right:.25rem}.mx-auto{margin-left:auto;margin-right:auto}.mb-6{margin-bottom:1.5rem}.ml-6{margin-left:1.5rem}.mr-8{margin-right:2rem}.mt-1{margin-top:.25rem}.mt-2{margin-top:.5rem}.mt-4{margin-top:1rem}.mt-6{margin-top:1.5rem}.box-border{box-sizing:border-box}.block{display:block}.flex{display:flex}.table{display:table}.h-10{height:2.5rem}.w-10{width:2.5rem}.w-2\/5{width:40%}.w-3\/12{width:25%}.w-9\/12{width:75%}.w-full{width:100%}.min-w-0{min-width:0}.max-w-sm{max-width:24rem}.flex-none{flex:none}.flex-grow{flex-grow:1}.table-fixed{table-layout:fixed}.border-collapse{border-collapse:collapse}.cursor-pointer{cursor:pointer}.items-center{align-items:center}.justify-center{justify-content:center}.overflow-hidden{overflow:hidden}.break-words{overflow-wrap:break-word}.break-all{word-break:break-all}.rounded{border-radius:.25rem}.rounded-md{border-radius:.375rem}.rounded-l{border-bottom-left-radius:.25rem;border-top-left-radius:.25rem}.rounded-r{border-bottom-right-radius:.25rem;border-top-right-radius:.25rem}.border{border-width:1px}.border-2{border-width:2px}.border-gray-300{--tw-border-opacity:1;border-color:rgb(209 213 219/var(--tw-border-opacity))}.border-green-300{--tw-border-opacity:1;border-color:rgb(134 239 172/var(--tw-border-opacity))}.bg-blue-500{--tw-bg-opacity:1;background-color:rgb(59 130 246/var(--tw-bg-opacity))}.bg-green-100{--tw-bg-opacity:1;background-color:rgb(220 252 231/var(--tw-bg-opacity))}.bg-green-500{--tw-bg-opacity:1;background-color:rgb(34 197 94/var(--tw-bg-opacity))}.bg-red-500{--tw-bg-opacity:1;background-color:rgb(239 68 68/var(--tw-bg-opacity))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.bg-yellow-500{--tw-bg-opacity:1;background-color:rgb(234 179 8/var(--tw-bg-opacity))}.p-2{padding:.5rem}.p-3{padding:.75rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.px-4{padding-left:1rem;padding-right:1rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-3{padding-bottom:.75rem;padding-top:.75rem}.pl-1{padding-left:.25rem}.pr-2{padding-right:.5rem}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.font-bold{font-weight:700}.text-black{--tw-text-opacity:1;color:rgb(0 0 0/var(--tw-text-opacity))}.text-green-600{--tw-text-opacity:1;color:rgb(22 163 74/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.shadow-md{--tw-shadow:0 4px 6px -1px #0000001a,0 2px 4px -2px #0000001a;--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color),0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-300{transition-duration:.3s}body{overflow-y:scroll!important}.log-entry-text{white-space:pre-wrap}.lds-roller{display:inline-block;height:80px;position:relative;width:80px}.lds-roller div{animation:lds-roller 1.2s cubic-bezier(.5,0,.5,1) infinite;transform-origin:40px 40px}.lds-roller div:after{background:#fff;border-radius:50%;content:" ";display:block;height:7px;margin:-4px 0 0 -4px;position:absolute;width:7px}.lds-roller div:first-child{animation-delay:-36ms}.lds-roller div:first-child:after{left:63px;top:63px}.lds-roller div:nth-child(2){animation-delay:-72ms}.lds-roller div:nth-child(2):after{left:56px;top:68px}.lds-roller div:nth-child(3){animation-delay:-.108s}.lds-roller div:nth-child(3):after{left:48px;top:71px}.lds-roller div:nth-child(4){animation-delay:-.144s}.lds-roller div:nth-child(4):after{left:40px;top:72px}.lds-roller div:nth-child(5){animation-delay:-.18s}.lds-roller div:nth-child(5):after{left:32px;top:71px}.lds-roller div:nth-child(6){animation-delay:-.216s}.lds-roller div:nth-child(6):after{left:24px;top:68px}.lds-roller div:nth-child(7){animation-delay:-.252s}.lds-roller div:nth-child(7):after{left:17px;top:63px}.lds-roller div:nth-child(8){animation-delay:-.288s}.lds-roller div:nth-child(8):after{left:12px;top:56px}@keyframes lds-roller{0%{transform:rotate(0deg)}to{transform:rotate(1turn)}}.loading-spinner{align-items:center;background-color:#0009;display:flex;height:100vh;justify-content:center;left:0;position:fixed;top:0;width:100vw;z-index:10000}.hover\:bg-gray-100:hover{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.focus\:border-blue-500:focus{--tw-border-opacity:1;border-color:rgb(59 130 246/var(--tw-border-opacity))}.focus\:outline-none:focus{outline:2px solid #0000;outline-offset:2px}:is(.dark .dark\:border-gray-100\/50){border-color:#f3f4f680}:is(.dark .dark\:border-gray-600){--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity))}:is(.dark .dark\:border-gray-700){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}:is(.dark .dark\:border-b-gray-100\/50){border-bottom-color:#f3f4f680}:is(.dark .dark\:bg-blue-700){--tw-bg-opacity:1;background-color:rgb(29 78 216/var(--tw-bg-opacity))}:is(.dark .dark\:bg-gray-700){--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}:is(.dark .dark\:bg-green-700){--tw-bg-opacity:1;background-color:rgb(21 128 61/var(--tw-bg-opacity))}:is(.dark .dark\:bg-red-700){--tw-bg-opacity:1;background-color:rgb(185 28 28/var(--tw-bg-opacity))}:is(.dark .dark\:bg-slate-600){--tw-bg-opacity:1;background-color:rgb(71 85 105/var(--tw-bg-opacity))}:is(.dark .dark\:bg-slate-700){--tw-bg-opacity:1;background-color:rgb(51 65 85/var(--tw-bg-opacity))}:is(.dark .dark\:bg-slate-800){--tw-bg-opacity:1;background-color:rgb(30 41 59/var(--tw-bg-opacity))}:is(.dark .dark\:text-white){--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}:is(.dark .dark\:hover\:bg-gray-500:hover){--tw-bg-opacity:1;background-color:rgb(107 114 128/var(--tw-bg-opacity))}
```

### Comparing `django_log_inspector-0.0.6/log_inspector/static/log_inspector/js/alpinejs.min.js` & `django_log_inspector-0.0.7/log_inspector/static/log_inspector/js/alpinejs.min.js`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/static/log_inspector/js/htmx.min.js` & `django_log_inspector-0.0.7/log_inspector/static/log_inspector/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/home.html` & `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/home.html`

 * *Files 2% similar despite different names*

```diff
@@ -73,25 +73,33 @@
                             hx-trigger="click"
                             hx-swap="outerHTML"
                             @click="live = !live"
                             x-show="!live && isFileSelected">
                         {% trans 'Live' %}
                     </button>
                     <button id="stop-button"
-                            class="bg-red-500 text-white px-4 py-2 rounded dark:bg-red-700"
+                            class="bg-red-500 text-white px-4 py-2 mx-1 rounded dark:bg-red-700"
                             hx-target="#log-entries-table"
                             hx-trigger="click"
                             hx-swap="outerHTML"
                             @click="live = !live"
                             x-show="live && isFileSelected">
                         {% trans 'Stop' %}
                     </button>
+                    <button id="refresh-button"
+                            class="bg-green-500 text-white px-4 py-2 mx-1 rounded dark:bg-green-700"
+                            hx-target="#log-entries-table"
+                            hx-trigger="click"
+                            hx-swap="outerHTML"
+                            x-show="!live && isFileSelected">
+                        {% trans 'Refresh' %}
+                    </button>
                     <a id="download-link">
                         <button id="download-button"
-                                class="bg-green-500 text-white px-4 py-2 mx-2 rounded dark:bg-green-700"
+                                class="bg-yellow-500 text-white px-4 py-2 mx-1  rounded"
                                 x-show="isFileSelected">
                             {% trans 'Download' %}
                         </button>
                     </a>
                     <input id="search-box"
                            class="py-2 px-4 mt-1 border-2 border-gray-300 rounded-md focus:outline-none
                             focus:border-blue-500 transition duration-300 box-border h-10 w-2/5 float-right
@@ -203,18 +211,20 @@
         function updateFileName(event) {
             const td = event.target;
             const fileName = td.textContent.trim();
 
             const liveButton = document.getElementById('live-button');
             const stopButton = document.getElementById('stop-button');
             const searchBox = document.getElementById('search-box');
+            const refreshButton = document.getElementById('refresh-button');
             const downloadLink = document.getElementById('download-link');
             const logEntriesTitle = document.getElementById('log-entries-title')
             liveButton.setAttribute('hx-get', `/logs/start-live/${fileName}/`)
             stopButton.setAttribute('hx-get', `/logs/log-entries/${fileName}/`)
+            refreshButton.setAttribute('hx-get', `/logs/log-entries/${fileName}/`)
             searchBox.setAttribute('hx-get', `/logs/log-entries/${fileName}/`)
             downloadLink.setAttribute('href', `/logs/download/${fileName}/`)
             logEntriesTitle.innerText = fileName
 
             htmx.process(document.body)
         }
```

#### html2text {}

```diff
@@ -9,14 +9,14 @@
 {{ block.super }}
 {% if custom_style_file %}
 {% endif %} {% endblock %} {% block extrahead %} {{ block.super }}
 {% endblock %} {% block content %}
 ************ {{%% ttrraannss ''DDjjaannggoo LLoogg IInnssppeeccttoorr'' %%}} ************
 click="live = !live" x-show="!live && isFileSelected"> {% trans 'Live' %}
 click="live = !live" x-show="live && isFileSelected"> {% trans 'Stop' %} {%
-trans 'Download' %}[Unknown INPUT type]
+trans 'Refresh' %} {% trans 'Download' %}[Unknown INPUT type]
 {{%% ttrraannss ''NNoo..'' %%}} {{%% ttrraannss ''LLoogg eennttrriieess'' %%}}
 {% trans 'No entries!' %}
 ********** {{%% ttrraannss ''LLoogg FFiilleess'' %%}} **********
 [Unknown INPUT type]
 {% trans 'No entries!' %}
 {% endblock %}
```

### Comparing `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_entries_data.html` & `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_entries_data.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_entries_table.html` & `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_entries_table.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/log_files.html` & `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/log_files.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/pagination.html` & `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/pagination.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/templates/log_inspector/start_live.html` & `django_log_inspector-0.0.7/log_inspector/templates/log_inspector/start_live.html`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/urls.py` & `django_log_inspector-0.0.7/log_inspector/urls.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/utils.py` & `django_log_inspector-0.0.7/log_inspector/utils.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/log_inspector/views.py` & `django_log_inspector-0.0.7/log_inspector/views.py`

 * *Files identical despite different names*

### Comparing `django_log_inspector-0.0.6/pyproject.toml` & `django_log_inspector-0.0.7/pyproject.toml`

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
-version = "0.0.6"
+version = "0.0.7"
 description = "Read and Download log files"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [
     "Django", "logging", "log viewer", "real-time monitoring", "log analysis", "troubleshooting",
     "log management", "log files", "log monitoring", "debugging", "Python web development", "development tool"
 ]
```


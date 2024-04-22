# Comparing `tmp/django-idp-user-2.5.0.tar.gz` & `tmp/django-idp-user-2.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-idp-user-2.5.0.tar", last modified: Mon Apr 22 07:55:45 2024, max compression
+gzip compressed data, was "django-idp-user-2.5.0.dev0.tar", last modified: Fri Apr 19 16:23:41 2024, max compression
```

## Comparing `django-idp-user-2.5.0.tar` & `django-idp-user-2.5.0.dev0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-22 07:55:45.856467 django-idp-user-2.5.0/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-09-29 13:46:44.000000 django-idp-user-2.5.0/LICENSE
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6474 2024-04-22 07:55:45.852467 django-idp-user-2.5.0/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4094 2023-11-09 15:46:44.000000 django-idp-user-2.5.0/README.md
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-22 07:55:45.844467 django-idp-user-2.5.0/django_idp_user.egg-info/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6474 2024-04-22 07:55:45.000000 django-idp-user-2.5.0/django_idp_user.egg-info/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1478 2024-04-22 07:55:45.000000 django-idp-user-2.5.0/django_idp_user.egg-info/SOURCES.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2024-04-22 07:55:45.000000 django-idp-user-2.5.0/django_idp_user.egg-info/dependency_links.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      441 2024-04-22 07:55:45.000000 django-idp-user-2.5.0/django_idp_user.egg-info/requires.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        9 2024-04-22 07:55:45.000000 django-idp-user-2.5.0/django_idp_user.egg-info/top_level.txt
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-22 07:55:45.848467 django-idp-user-2.5.0/idp_user/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       97 2024-03-20 09:43:22.000000 django-idp-user-2.5.0/idp_user/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2048 2023-09-29 13:46:44.000000 django-idp-user-2.5.0/idp_user/agents.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1018 2023-09-29 13:46:44.000000 django-idp-user-2.5.0/idp_user/apps.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-22 07:55:45.848467 django-idp-user-2.5.0/idp_user/auth/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      306 2024-04-19 16:17:43.000000 django-idp-user-2.5.0/idp_user/auth/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1375 2024-04-22 07:54:54.000000 django-idp-user-2.5.0/idp_user/auth/admin_authentication.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1663 2024-04-19 15:51:09.000000 django-idp-user-2.5.0/idp_user/auth/async_authentication.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2290 2024-04-19 16:17:43.000000 django-idp-user-2.5.0/idp_user/auth/drf_authentication.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      925 2024-04-19 16:17:43.000000 django-idp-user-2.5.0/idp_user/auth/ninja_authentication.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2811 2023-11-09 15:46:44.000000 django-idp-user-2.5.0/idp_user/checks.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-22 07:55:45.848467 django-idp-user-2.5.0/idp_user/management/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/management/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-22 07:55:45.848467 django-idp-user-2.5.0/idp_user/management/commands/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/management/commands/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      803 2023-09-29 13:46:44.000000 django-idp-user-2.5.0/idp_user/management/commands/put_app_entities_records_to_kafka.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-22 07:55:45.852467 django-idp-user-2.5.0/idp_user/migrations/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4340 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/migrations/0001_initial.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6133 2023-09-29 13:46:44.000000 django-idp-user-2.5.0/idp_user/migrations/0001_initial_squashed_0005_alter_userrole_id.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      378 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/migrations/0002_auto_20220120_1617.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      390 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/migrations/0003_auto_20220513_1025.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      579 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/migrations/0004_auto_20220817_1526.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      446 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/migrations/0005_alter_userrole_id.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1270 2024-03-19 08:55:50.000000 django-idp-user-2.5.0/idp_user/migrations/0006_userrole_organization_and_more.py
--rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/migrations/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-22 07:55:45.852467 django-idp-user-2.5.0/idp_user/models/
--rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)       55 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/models/__init__.py
--rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)       89 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/models/user.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)      984 2024-03-19 08:46:17.000000 django-idp-user-2.5.0/idp_user/models/user_role.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1815 2023-09-29 13:46:44.000000 django-idp-user-2.5.0/idp_user/producer.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      834 2024-04-19 15:51:43.000000 django-idp-user-2.5.0/idp_user/schema_extensions.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-22 07:55:45.852467 django-idp-user-2.5.0/idp_user/services/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      139 2023-09-29 13:46:44.000000 django-idp-user-2.5.0/idp_user/services/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    13090 2024-03-19 08:59:11.000000 django-idp-user-2.5.0/idp_user/services/async_user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2581 2023-09-29 13:46:44.000000 django-idp-user-2.5.0/idp_user/services/base_user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16161 2024-04-22 07:29:20.000000 django-idp-user-2.5.0/idp_user/services/user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      836 2023-09-29 13:46:44.000000 django-idp-user-2.5.0/idp_user/settings.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      132 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/signals.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       17 2023-09-29 13:46:44.000000 django-idp-user-2.5.0/idp_user/urls.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-22 07:55:45.852467 django-idp-user-2.5.0/idp_user/utils/
--rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/utils/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      739 2023-09-29 13:46:44.000000 django-idp-user-2.5.0/idp_user/utils/choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      311 2023-06-03 01:21:10.000000 django-idp-user-2.5.0/idp_user/utils/classes.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      165 2024-04-19 14:56:20.000000 django-idp-user-2.5.0/idp_user/utils/exceptions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4226 2024-04-19 16:10:01.000000 django-idp-user-2.5.0/idp_user/utils/functions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2906 2024-03-19 08:59:11.000000 django-idp-user-2.5.0/idp_user/utils/typing.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3831 2024-04-22 07:52:36.000000 django-idp-user-2.5.0/pyproject.toml
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       38 2024-04-22 07:55:45.856467 django-idp-user-2.5.0/setup.cfg
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       69 2023-04-27 07:58:09.000000 django-idp-user-2.5.0/setup.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.689890 django-idp-user-2.5.0.dev0/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/LICENSE
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6479 2024-04-19 16:23:41.689890 django-idp-user-2.5.0.dev0/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4094 2023-11-09 15:46:44.000000 django-idp-user-2.5.0.dev0/README.md
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6479 2024-04-19 16:23:41.000000 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1478 2024-04-19 16:23:41.000000 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/SOURCES.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2024-04-19 16:23:41.000000 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/dependency_links.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      441 2024-04-19 16:23:41.000000 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/requires.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        9 2024-04-19 16:23:41.000000 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/top_level.txt
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       97 2024-03-20 09:43:22.000000 django-idp-user-2.5.0.dev0/idp_user/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2048 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/agents.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1018 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/apps.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/auth/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      306 2024-04-19 16:17:43.000000 django-idp-user-2.5.0.dev0/idp_user/auth/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1439 2024-01-16 11:06:35.000000 django-idp-user-2.5.0.dev0/idp_user/auth/admin_authentication.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1663 2024-04-19 15:51:09.000000 django-idp-user-2.5.0.dev0/idp_user/auth/async_authentication.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2290 2024-04-19 16:17:43.000000 django-idp-user-2.5.0.dev0/idp_user/auth/drf_authentication.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      925 2024-04-19 16:17:43.000000 django-idp-user-2.5.0.dev0/idp_user/auth/ninja_authentication.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2811 2023-11-09 15:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/checks.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/management/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/management/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/management/commands/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/management/commands/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      803 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/management/commands/put_app_entities_records_to_kafka.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/migrations/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4340 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0001_initial.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6133 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0001_initial_squashed_0005_alter_userrole_id.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      378 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0002_auto_20220120_1617.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      390 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0003_auto_20220513_1025.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      579 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0004_auto_20220817_1526.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      446 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0005_alter_userrole_id.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1270 2024-03-19 08:55:50.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0006_userrole_organization_and_more.py
+-rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/models/
+-rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)       55 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/models/__init__.py
+-rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)       89 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/models/user.py
+-rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)      984 2024-03-19 08:46:17.000000 django-idp-user-2.5.0.dev0/idp_user/models/user_role.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1815 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/producer.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      834 2024-04-19 15:51:43.000000 django-idp-user-2.5.0.dev0/idp_user/schema_extensions.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/services/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      139 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/services/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    13090 2024-03-19 08:59:11.000000 django-idp-user-2.5.0.dev0/idp_user/services/async_user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2581 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/services/base_user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16164 2024-03-19 17:13:35.000000 django-idp-user-2.5.0.dev0/idp_user/services/user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      836 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/settings.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      132 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/signals.py
+-rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       17 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/urls.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.689890 django-idp-user-2.5.0.dev0/idp_user/utils/
+-rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/utils/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      739 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/utils/choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      311 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/utils/classes.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      165 2024-04-19 14:56:20.000000 django-idp-user-2.5.0.dev0/idp_user/utils/exceptions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4226 2024-04-19 16:10:01.000000 django-idp-user-2.5.0.dev0/idp_user/utils/functions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2906 2024-03-19 08:59:11.000000 django-idp-user-2.5.0.dev0/idp_user/utils/typing.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3836 2024-04-19 15:58:14.000000 django-idp-user-2.5.0.dev0/pyproject.toml
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       38 2024-04-19 16:23:41.689890 django-idp-user-2.5.0.dev0/setup.cfg
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       69 2023-04-27 07:58:09.000000 django-idp-user-2.5.0.dev0/setup.py
```

### Comparing `django-idp-user-2.5.0/LICENSE` & `django-idp-user-2.5.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/PKG-INFO` & `django-idp-user-2.5.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-idp-user
-Version: 2.5.0
+Version: 2.5.0.dev0
 Summary: A Django app that handles the communication between the IDP and the products for the authorization of users.
 Author: Mahmoud Al-Rawy, Euron Metaliaj, Klajdi Çaushi, Aleksandër Nasto, Andi Çuku, Klement Omeri, Lirim Shala
 Author-email: hello@cardoai.com
 License: Copyright 2023 CardoAI
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django-idp-user-2.5.0/README.md` & `django-idp-user-2.5.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/django_idp_user.egg-info/PKG-INFO` & `django-idp-user-2.5.0.dev0/django_idp_user.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-idp-user
-Version: 2.5.0
+Version: 2.5.0.dev0
 Summary: A Django app that handles the communication between the IDP and the products for the authorization of users.
 Author: Mahmoud Al-Rawy, Euron Metaliaj, Klajdi Çaushi, Aleksandër Nasto, Andi Çuku, Klement Omeri, Lirim Shala
 Author-email: hello@cardoai.com
 License: Copyright 2023 CardoAI
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django-idp-user-2.5.0/django_idp_user.egg-info/SOURCES.txt` & `django-idp-user-2.5.0.dev0/django_idp_user.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/agents.py` & `django-idp-user-2.5.0.dev0/idp_user/agents.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/apps.py` & `django-idp-user-2.5.0.dev0/idp_user/apps.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/auth/admin_authentication.py` & `django-idp-user-2.5.0.dev0/idp_user/auth/admin_authentication.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from typing import Optional
 
+import jwt
 import requests
 from django.conf import settings
 from django.contrib.auth.backends import ModelBackend
-from jwt.exceptions import InvalidTokenError
 
 from idp_user.models.user import User
-from idp_user.utils.functions import get_or_none, get_jwt_payload
+from idp_user.utils.functions import get_or_none
 
 IDP_URL = settings.IDP_USER_APP.get("IDP_URL")
 HTTP_200_OK = 200
 
 
 class IDPAuthBackend(ModelBackend):
     def authenticate(self, request, **kwargs):
         access_token = self._fetch_token(request)
         if not access_token:
             return None
 
         try:
-            jwt_data = get_jwt_payload(access_token)
-        except InvalidTokenError:
+            jwt_data = jwt.decode(
+                access_token,
+                algorithms=["HS256"],
+                options={"verify_signature": False},
+            )
+        except jwt.DecodeError:
             return None
 
         username = jwt_data["username"]
         return get_or_none(User.objects, username=username)
 
     @staticmethod
     def _fetch_token(request) -> Optional[str]:
```

### Comparing `django-idp-user-2.5.0/idp_user/auth/async_authentication.py` & `django-idp-user-2.5.0.dev0/idp_user/auth/async_authentication.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/auth/drf_authentication.py` & `django-idp-user-2.5.0.dev0/idp_user/auth/drf_authentication.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/auth/ninja_authentication.py` & `django-idp-user-2.5.0.dev0/idp_user/auth/ninja_authentication.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/checks.py` & `django-idp-user-2.5.0.dev0/idp_user/checks.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/management/commands/put_app_entities_records_to_kafka.py` & `django-idp-user-2.5.0.dev0/idp_user/management/commands/put_app_entities_records_to_kafka.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/migrations/0001_initial.py` & `django-idp-user-2.5.0.dev0/idp_user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/migrations/0001_initial_squashed_0005_alter_userrole_id.py` & `django-idp-user-2.5.0.dev0/idp_user/migrations/0001_initial_squashed_0005_alter_userrole_id.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/migrations/0004_auto_20220817_1526.py` & `django-idp-user-2.5.0.dev0/idp_user/migrations/0004_auto_20220817_1526.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/migrations/0006_userrole_organization_and_more.py` & `django-idp-user-2.5.0.dev0/idp_user/migrations/0006_userrole_organization_and_more.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/models/user_role.py` & `django-idp-user-2.5.0.dev0/idp_user/models/user_role.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/producer.py` & `django-idp-user-2.5.0.dev0/idp_user/producer.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/schema_extensions.py` & `django-idp-user-2.5.0.dev0/idp_user/schema_extensions.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/services/async_user.py` & `django-idp-user-2.5.0.dev0/idp_user/services/async_user.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/services/base_user.py` & `django-idp-user-2.5.0.dev0/idp_user/services/base_user.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/services/user.py` & `django-idp-user-2.5.0.dev0/idp_user/services/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from collections import defaultdict
 from copy import deepcopy
 from typing import Any, Optional, Union
 
 from django.conf import settings
 from django.core.cache import cache
-from django.core.exceptions import PermissionDenied
 from django.db import models, transaction
 from django.db.models import Q, QuerySet
+from rest_framework.exceptions import PermissionDenied
 from rest_framework.request import Request
 
 from idp_user.models import UserRole
 from idp_user.models.user import User
 from idp_user.services.base_user import BaseUserService
 from idp_user.settings import APP_ENTITIES, APP_IDENTIFIER, IN_DEV, ROLES, TENANTS
 from idp_user.signals import (
```

### Comparing `django-idp-user-2.5.0/idp_user/settings.py` & `django-idp-user-2.5.0.dev0/idp_user/settings.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/utils/choices.py` & `django-idp-user-2.5.0.dev0/idp_user/utils/choices.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/utils/functions.py` & `django-idp-user-2.5.0.dev0/idp_user/utils/functions.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/idp_user/utils/typing.py` & `django-idp-user-2.5.0.dev0/idp_user/utils/typing.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.5.0/pyproject.toml` & `django-idp-user-2.5.0.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-idp-user"
 description = "A Django app that handles the communication between the IDP and the products for the authorization of users."
 requires-python = ">=3.9"
-version = "2.5.0"
+version = "2.5.0.dev0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Intended Audience :: Developers",
```


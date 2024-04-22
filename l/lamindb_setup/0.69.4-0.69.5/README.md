# Comparing `tmp/lamindb_setup-0.69.4.tar.gz` & `tmp/lamindb_setup-0.69.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.69.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.69.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.69.4.tar` & `lamindb_setup-0.69.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     8290 2024-04-16 19:27:14.643060 lamindb_setup-0.69.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.69.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.69.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.69.4/.gitignore
--rw-r--r--   0        0        0     1931 2024-02-29 20:00:56.143838 lamindb_setup-0.69.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.69.4/LICENSE
--rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.69.4/README.md
--rw-r--r--   0        0        0    96713 2024-04-19 17:16:18.465701 lamindb_setup-0.69.4/docs/changelog.md
--rw-r--r--   0        0        0     7378 2024-03-07 18:05:18.839544 lamindb_setup-0.69.4/docs/hub-cloud/01-init-on-prem-instance.ipynb
--rw-r--r--   0        0        0     4054 2024-03-07 18:05:18.839906 lamindb_setup-0.69.4/docs/hub-cloud/02-connect-on-prem-instance.ipynb
--rw-r--r--   0        0        0     5812 2024-03-07 18:05:18.840396 lamindb_setup-0.69.4/docs/hub-cloud/03-set-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-03-07 00:06:34.620916 lamindb_setup-0.69.4/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     3106 2024-04-08 06:13:37.564530 lamindb_setup-0.69.4/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     3383 2024-04-08 09:34:48.611032 lamindb_setup-0.69.4/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     3160 2024-03-07 16:07:21.923709 lamindb_setup-0.69.4/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.621529 lamindb_setup-0.69.4/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-03-07 18:05:18.841099 lamindb_setup-0.69.4/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-03-26 10:01:31.777978 lamindb_setup-0.69.4/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-03-18 14:07:20.594957 lamindb_setup-0.69.4/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2706 2024-03-07 00:06:34.621901 lamindb_setup-0.69.4/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-03-09 06:05:04.471802 lamindb_setup-0.69.4/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-03-07 00:06:34.622152 lamindb_setup-0.69.4/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-03-07 00:06:34.622232 lamindb_setup-0.69.4/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6181 2024-03-22 15:00:34.131177 lamindb_setup-0.69.4/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.622645 lamindb_setup-0.69.4/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.69.4/docs/index.md
--rw-r--r--   0        0        0      486 2024-03-26 10:01:31.778544 lamindb_setup-0.69.4/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.69.4/docs/reference.md
--rw-r--r--   0        0        0     1558 2024-04-19 17:16:06.228783 lamindb_setup-0.69.4/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     1802 2024-03-29 23:29:05.334743 lamindb_setup-0.69.4/lamindb_setup/_add_remote_storage.py
--rw-r--r--   0        0        0      809 2024-02-29 20:00:56.145929 lamindb_setup-0.69.4/lamindb_setup/_cache.py
--rw-r--r--   0        0        0       92 2024-02-29 20:00:56.145990 lamindb_setup-0.69.4/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2543 2024-03-08 11:38:29.530179 lamindb_setup-0.69.4/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1150 2024-03-06 12:44:01.598158 lamindb_setup-0.69.4/lamindb_setup/_close.py
--rw-r--r--   0        0        0    11789 2024-04-19 17:16:01.027505 lamindb_setup-0.69.4/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     3111 2024-03-22 15:00:34.131907 lamindb_setup-0.69.4/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1500 2024-03-06 12:44:01.598969 lamindb_setup-0.69.4/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2084 2024-04-15 04:44:50.596309 lamindb_setup-0.69.4/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1836 2024-04-15 06:35:29.022278 lamindb_setup-0.69.4/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11479 2024-04-08 10:33:42.801066 lamindb_setup-0.69.4/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     8672 2024-04-17 08:15:10.952927 lamindb_setup-0.69.4/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      795 2024-03-08 11:38:29.531409 lamindb_setup-0.69.4/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      642 2024-03-08 11:38:29.531579 lamindb_setup-0.69.4/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     3657 2024-03-29 23:29:05.335131 lamindb_setup-0.69.4/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1548 2024-02-29 20:00:56.147217 lamindb_setup-0.69.4/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      369 2024-04-16 15:26:03.848647 lamindb_setup-0.69.4/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     1762 2024-04-08 09:34:48.611370 lamindb_setup-0.69.4/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2491 2024-03-05 09:37:50.121160 lamindb_setup-0.69.4/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      240 2024-03-05 09:37:50.121230 lamindb_setup-0.69.4/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5520 2024-04-15 15:03:26.266397 lamindb_setup-0.69.4/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    10990 2024-04-15 15:03:26.266901 lamindb_setup-0.69.4/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4505 2024-03-29 23:01:12.640293 lamindb_setup-0.69.4/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1862 2024-03-05 09:37:50.121645 lamindb_setup-0.69.4/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3241 2024-03-14 13:29:19.826564 lamindb_setup-0.69.4/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    11556 2024-04-16 19:47:35.808698 lamindb_setup-0.69.4/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3744 2024-03-14 17:58:31.759147 lamindb_setup-0.69.4/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2563 2024-03-18 14:07:20.595611 lamindb_setup-0.69.4/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    13044 2024-04-16 19:47:35.808927 lamindb_setup-0.69.4/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     1929 2024-03-14 17:58:31.759632 lamindb_setup-0.69.4/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1281 2024-03-07 18:05:18.845546 lamindb_setup-0.69.4/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     2908 2024-03-05 09:37:50.122398 lamindb_setup-0.69.4/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6835 2024-03-26 10:01:31.779365 lamindb_setup-0.69.4/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     3335 2024-04-16 15:26:03.848992 lamindb_setup-0.69.4/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      275 2024-03-08 11:38:29.532093 lamindb_setup-0.69.4/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2011 2024-03-12 21:48:08.236470 lamindb_setup-0.69.4/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      497 2024-04-05 12:59:33.028024 lamindb_setup-0.69.4/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    24039 2024-04-19 11:12:43.243500 lamindb_setup-0.69.4/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     4265 2024-04-08 09:34:48.612298 lamindb_setup-0.69.4/noxfile.py
--rw-r--r--   0        0        0      992 2024-03-26 10:01:31.780237 lamindb_setup-0.69.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-19 17:16:01.027907 lamindb_setup-0.69.4/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      285 2024-03-07 00:06:34.623314 lamindb_setup-0.69.4/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     7021 2024-03-07 01:53:25.975859 lamindb_setup-0.69.4/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      502 2024-03-07 00:06:34.623653 lamindb_setup-0.69.4/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      469 2024-03-07 00:06:34.623714 lamindb_setup-0.69.4/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      338 2024-03-07 18:05:18.846365 lamindb_setup-0.69.4/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0      548 2024-04-08 09:34:48.612599 lamindb_setup-0.69.4/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11318 2024-04-15 15:03:26.267377 lamindb_setup-0.69.4/tests/hub-local/test_all.py
--rw-r--r--   0        0        0      452 2024-03-07 00:06:34.623879 lamindb_setup-0.69.4/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      365 2024-03-07 18:05:18.846587 lamindb_setup-0.69.4/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      158 2024-04-16 15:26:03.849537 lamindb_setup-0.69.4/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1432 2024-04-15 15:03:26.267758 lamindb_setup-0.69.4/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0      595 2024-03-07 00:06:34.624340 lamindb_setup-0.69.4/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1411 2024-03-12 21:17:07.347266 lamindb_setup-0.69.4/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     1985 2024-03-07 18:05:18.846898 lamindb_setup-0.69.4/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      787 2024-03-28 20:35:14.618464 lamindb_setup-0.69.4/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      842 2024-03-26 15:38:38.001397 lamindb_setup-0.69.4/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.69.4/PKG-INFO
+-rw-r--r--   0        0        0     8290 2024-04-16 19:27:14.643060 lamindb_setup-0.69.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.69.5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.69.5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.69.5/.gitignore
+-rw-r--r--   0        0        0     1931 2024-02-29 20:00:56.143838 lamindb_setup-0.69.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.69.5/LICENSE
+-rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.69.5/README.md
+-rw-r--r--   0        0        0    96860 2024-04-22 05:51:48.799859 lamindb_setup-0.69.5/docs/changelog.md
+-rw-r--r--   0        0        0     7378 2024-03-07 18:05:18.839544 lamindb_setup-0.69.5/docs/hub-cloud/01-init-on-prem-instance.ipynb
+-rw-r--r--   0        0        0     4054 2024-03-07 18:05:18.839906 lamindb_setup-0.69.5/docs/hub-cloud/02-connect-on-prem-instance.ipynb
+-rw-r--r--   0        0        0     5812 2024-03-07 18:05:18.840396 lamindb_setup-0.69.5/docs/hub-cloud/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-03-07 00:06:34.620916 lamindb_setup-0.69.5/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3106 2024-04-08 06:13:37.564530 lamindb_setup-0.69.5/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3806 2024-04-21 08:00:19.897288 lamindb_setup-0.69.5/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3160 2024-03-07 16:07:21.923709 lamindb_setup-0.69.5/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 00:06:34.621529 lamindb_setup-0.69.5/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-03-07 18:05:18.841099 lamindb_setup-0.69.5/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-03-26 10:01:31.777978 lamindb_setup-0.69.5/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-03-18 14:07:20.594957 lamindb_setup-0.69.5/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2706 2024-03-07 00:06:34.621901 lamindb_setup-0.69.5/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-03-09 06:05:04.471802 lamindb_setup-0.69.5/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-03-07 00:06:34.622152 lamindb_setup-0.69.5/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-03-07 00:06:34.622232 lamindb_setup-0.69.5/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6181 2024-03-22 15:00:34.131177 lamindb_setup-0.69.5/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 00:06:34.622645 lamindb_setup-0.69.5/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.69.5/docs/index.md
+-rw-r--r--   0        0        0      486 2024-03-26 10:01:31.778544 lamindb_setup-0.69.5/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.69.5/docs/reference.md
+-rw-r--r--   0        0        0     1558 2024-04-22 05:51:36.763309 lamindb_setup-0.69.5/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     1802 2024-03-29 23:29:05.334743 lamindb_setup-0.69.5/lamindb_setup/_add_remote_storage.py
+-rw-r--r--   0        0        0      809 2024-02-29 20:00:56.145929 lamindb_setup-0.69.5/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0       92 2024-02-29 20:00:56.145990 lamindb_setup-0.69.5/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2543 2024-03-08 11:38:29.530179 lamindb_setup-0.69.5/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1150 2024-03-06 12:44:01.598158 lamindb_setup-0.69.5/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    11789 2024-04-19 17:16:01.027505 lamindb_setup-0.69.5/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     3111 2024-03-22 15:00:34.131907 lamindb_setup-0.69.5/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1500 2024-03-06 12:44:01.598969 lamindb_setup-0.69.5/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2084 2024-04-15 04:44:50.596309 lamindb_setup-0.69.5/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1836 2024-04-15 06:35:29.022278 lamindb_setup-0.69.5/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11479 2024-04-08 10:33:42.801066 lamindb_setup-0.69.5/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     8672 2024-04-17 08:15:10.952927 lamindb_setup-0.69.5/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      795 2024-03-08 11:38:29.531409 lamindb_setup-0.69.5/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      642 2024-03-08 11:38:29.531579 lamindb_setup-0.69.5/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     3657 2024-03-29 23:29:05.335131 lamindb_setup-0.69.5/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1548 2024-02-29 20:00:56.147217 lamindb_setup-0.69.5/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      369 2024-04-16 15:26:03.848647 lamindb_setup-0.69.5/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     1762 2024-04-08 09:34:48.611370 lamindb_setup-0.69.5/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2491 2024-03-05 09:37:50.121160 lamindb_setup-0.69.5/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      240 2024-03-05 09:37:50.121230 lamindb_setup-0.69.5/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5520 2024-04-15 15:03:26.266397 lamindb_setup-0.69.5/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    10990 2024-04-15 15:03:26.266901 lamindb_setup-0.69.5/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4505 2024-03-29 23:01:12.640293 lamindb_setup-0.69.5/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1862 2024-03-05 09:37:50.121645 lamindb_setup-0.69.5/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3241 2024-03-14 13:29:19.826564 lamindb_setup-0.69.5/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    11556 2024-04-16 19:47:35.808698 lamindb_setup-0.69.5/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3744 2024-03-14 17:58:31.759147 lamindb_setup-0.69.5/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2563 2024-03-18 14:07:20.595611 lamindb_setup-0.69.5/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    13044 2024-04-16 19:47:35.808927 lamindb_setup-0.69.5/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     1929 2024-03-14 17:58:31.759632 lamindb_setup-0.69.5/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1281 2024-03-07 18:05:18.845546 lamindb_setup-0.69.5/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     2908 2024-03-05 09:37:50.122398 lamindb_setup-0.69.5/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6835 2024-03-26 10:01:31.779365 lamindb_setup-0.69.5/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     3335 2024-04-16 15:26:03.848992 lamindb_setup-0.69.5/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      275 2024-03-08 11:38:29.532093 lamindb_setup-0.69.5/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2011 2024-03-12 21:48:08.236470 lamindb_setup-0.69.5/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      497 2024-04-05 12:59:33.028024 lamindb_setup-0.69.5/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    24510 2024-04-21 08:00:19.898318 lamindb_setup-0.69.5/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     4265 2024-04-08 09:34:48.612298 lamindb_setup-0.69.5/noxfile.py
+-rw-r--r--   0        0        0      992 2024-03-26 10:01:31.780237 lamindb_setup-0.69.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-19 17:16:01.027907 lamindb_setup-0.69.5/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      285 2024-03-07 00:06:34.623314 lamindb_setup-0.69.5/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     7021 2024-03-07 01:53:25.975859 lamindb_setup-0.69.5/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      502 2024-03-07 00:06:34.623653 lamindb_setup-0.69.5/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      469 2024-03-07 00:06:34.623714 lamindb_setup-0.69.5/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      338 2024-03-07 18:05:18.846365 lamindb_setup-0.69.5/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0      548 2024-04-08 09:34:48.612599 lamindb_setup-0.69.5/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11318 2024-04-15 15:03:26.267377 lamindb_setup-0.69.5/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0      452 2024-03-07 00:06:34.623879 lamindb_setup-0.69.5/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      365 2024-03-07 18:05:18.846587 lamindb_setup-0.69.5/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      158 2024-04-16 15:26:03.849537 lamindb_setup-0.69.5/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1432 2024-04-15 15:03:26.267758 lamindb_setup-0.69.5/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0      595 2024-03-07 00:06:34.624340 lamindb_setup-0.69.5/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1411 2024-03-12 21:17:07.347266 lamindb_setup-0.69.5/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     1985 2024-03-07 18:05:18.846898 lamindb_setup-0.69.5/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      787 2024-03-28 20:35:14.618464 lamindb_setup-0.69.5/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      842 2024-03-26 15:38:38.001397 lamindb_setup-0.69.5/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.69.5/PKG-INFO
```

### Comparing `lamindb_setup-0.69.4/.github/workflows/build.yml` & `lamindb_setup-0.69.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/.github/workflows/latest-changes.yml` & `lamindb_setup-0.69.5/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/.gitignore` & `lamindb_setup-0.69.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/.pre-commit-config.yaml` & `lamindb_setup-0.69.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/LICENSE` & `lamindb_setup-0.69.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/changelog.md` & `lamindb_setup-0.69.5/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ Upload dirs inplace | [722](https://github.com/laminlabs/lamindb-setup/pull/722) | [Koncopd](https://github.com/Koncopd) | 2024-04-20 | 0.69.5
 ♻️ Do not always read from local cache | [720](https://github.com/laminlabs/lamindb-setup/pull/720) | [falexwolf](https://github.com/falexwolf) | 2024-04-19 | 0.69.4
 ♻️ Improve suffix handling | [718](https://github.com/laminlabs/lamindb-setup/pull/718) | [falexwolf](https://github.com/falexwolf) | 2024-04-19 | 0.69.3
 ✨ Enable hybrid storage mode | [717](https://github.com/laminlabs/lamindb-setup/pull/717) | [falexwolf](https://github.com/falexwolf) | 2024-04-16 | 0.69.1
 🚸 Better migrations warning | [716](https://github.com/laminlabs/lamindb-setup/pull/716) | [falexwolf](https://github.com/falexwolf) | 2024-04-16 |
 🚸 Refresh token also upon access-aws | [715](https://github.com/laminlabs/lamindb-setup/pull/715) | [falexwolf](https://github.com/falexwolf) | 2024-04-15 |
 🚸 Skip hub request for a purely local instance | [713](https://github.com/laminlabs/lamindb-setup/pull/713) | [falexwolf](https://github.com/falexwolf) | 2024-04-08 | 0.69.0
 🐛 Fix clashes for multi process | [712](https://github.com/laminlabs/lamindb-setup/pull/712) | [falexwolf](https://github.com/falexwolf) | 2024-04-08 |
```

### Comparing `lamindb_setup-0.69.4/docs/hub-cloud/01-init-on-prem-instance.ipynb` & `lamindb_setup-0.69.5/docs/hub-cloud/01-init-on-prem-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-cloud/02-connect-on-prem-instance.ipynb` & `lamindb_setup-0.69.5/docs/hub-cloud/02-connect-on-prem-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-cloud/03-set-storage.ipynb` & `lamindb_setup-0.69.5/docs/hub-cloud/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.69.5/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.69.5/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.69.5/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9897435897435898%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(3, 'assert target_dir.is_dir()\\n'), (4, 'assert "*

 * *            '(target_dir / "test-dir-upload").exists()\\n\'), (5, \'\\n\'), (6, '*

 * *            "'target_dir.rmdir()\\n'), (7, 'assert not target_dir.exists()')], delete: [3]}}, "*

 * *            "insert: [(8, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            "['target_dir.upload_from(test_dir, dir_inplace=True)\\n', '\\n', 'as […]*

```diff
@@ -84,15 +84,31 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "target_dir = root / \"test-dir-upload\"\n",
                 "target_dir.upload_from(test_dir, recursive=True)\n",
                 "\n",
-                "assert target_dir.is_dir()"
+                "assert target_dir.is_dir()\n",
+                "assert (target_dir / \"test-dir-upload\").exists()\n",
+                "\n",
+                "target_dir.rmdir()\n",
+                "assert not target_dir.exists()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "target_dir.upload_from(test_dir, dir_inplace=True)\n",
+                "\n",
+                "assert target_dir.is_dir()\n",
+                "assert not (target_dir / \"test-dir-upload\").exists()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Test that instance can not be deleted from hub:"
```

### Comparing `lamindb_setup-0.69.4/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.69.5/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.69.5/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.69.5/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.69.5/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.69.5/docs/hub-prod/test-empty-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.69.5/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.69.5/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.69.5/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.69.5/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/__init__.py` & `lamindb_setup-0.69.5/lamindb_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.69.4"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.69.5"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._close import close  # noqa
 from ._delete import delete  # noqa
```

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_add_remote_storage.py` & `lamindb_setup-0.69.5/lamindb_setup/_add_remote_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_cache.py` & `lamindb_setup-0.69.5/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_check_setup.py` & `lamindb_setup-0.69.5/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_close.py` & `lamindb_setup-0.69.5/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.69.5/lamindb_setup/_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_delete.py` & `lamindb_setup-0.69.5/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_django.py` & `lamindb_setup-0.69.5/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_exportdb.py` & `lamindb_setup-0.69.5/lamindb_setup/_exportdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_importdb.py` & `lamindb_setup-0.69.5/lamindb_setup/_importdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_init_instance.py` & `lamindb_setup-0.69.5/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_migrate.py` & `lamindb_setup-0.69.5/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_register_instance.py` & `lamindb_setup-0.69.5/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_schema.py` & `lamindb_setup-0.69.5/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_setup_user.py` & `lamindb_setup-0.69.5/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.69.5/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_aws_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_hub_core.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_settings.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_settings_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.69.5/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.69.5/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/django.py` & `lamindb_setup-0.69.5/lamindb_setup/core/django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/hashing.py` & `lamindb_setup-0.69.5/lamindb_setup/core/hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/lamindb_setup/core/upath.py` & `lamindb_setup-0.69.5/lamindb_setup/core/upath.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,55 +161,73 @@
             hooks=dict(print_hook=print_hook), filepath=path_1, action=self.action
         )
 
     def call(self, *args, **kwargs):
         return None
 
 
-def download_to(self, path, print_progress: bool = False, **kwargs):
+def download_to(self, path: UPathStr, print_progress: bool = False, **kwargs):
     """Download to a path."""
     if print_progress:
         # can't do path.is_dir() because path doesn't exist
         # so assume any destination without a suffix is a dir
         # this is temporary until we have a proper progress bar for directories
         if os.path.splitext(path)[-1] not in {"", ".zrad", ".zarr"}:
             cb = ProgressCallback("downloading")
         else:
             # todo: make proper progress bar for directories
             cb = fsspec.callbacks.NoOpCallback()
         kwargs["callback"] = cb
     self.fs.download(str(self), str(path), **kwargs)
 
 
-def upload_from(self, path, print_progress: bool = False, **kwargs):
+def upload_from(
+    self,
+    path: UPathStr,
+    dir_inplace: bool = False,
+    print_progress: bool = False,
+    **kwargs,
+):
     """Upload from a local path."""
+    path_is_dir = os.path.isdir(path)
+    if not path_is_dir:
+        dir_inplace = False
+
     if print_progress:
-        if not os.path.isdir(path):
+        if not path_is_dir:
             cb = ProgressCallback("uploading")
         else:
             # todo: make proper progress bar for directories
             cb = fsspec.callbacks.NoOpCallback()
         kwargs["callback"] = cb
+
+    if dir_inplace:
+        path = Path(path)
+        source = [f for f in path.rglob("*") if f.is_file()]
+        destination = [str(self / f.relative_to(path)) for f in source]
+        source = [str(f) for f in source]  # type: ignore
+    else:
+        source = str(path)  # type: ignore
+        destination = str(self)  # type: ignore
     # this weird thing is to avoid s3fs triggering create_bucket in upload
     # if dirs are present
     # it allows to avoid permission error
-    destination = str(self)
-    if self.protocol != "s3" or os.path.isfile(path):
+    if self.protocol != "s3" or not path_is_dir or dir_inplace:
         cleanup_cache = False
     else:
         bucket = self._url.netloc
         if bucket not in self.fs.dircache:
             self.fs.dircache[bucket] = [{}]
             if not destination.endswith(TRAILING_SEP):  # type: ignore
                 destination += "/"
             cleanup_cache = True
         else:
             cleanup_cache = False
 
-    self.fs.upload(str(path), destination, **kwargs)
+    self.fs.upload(source, destination, **kwargs)
 
     if cleanup_cache:
         # normally this is invalidated after the upload but still better to check
         if bucket in self.fs.dircache:
             del self.fs.dircache[bucket]
```

### Comparing `lamindb_setup-0.69.4/noxfile.py` & `lamindb_setup-0.69.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/pyproject.toml` & `lamindb_setup-0.69.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.69.5/tests/hub-cloud/test_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.69.5/tests/hub-cloud/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/tests/hub-local/conftest.py` & `lamindb_setup-0.69.5/tests/hub-local/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/tests/hub-local/test_all.py` & `lamindb_setup-0.69.5/tests/hub-local/test_all.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.69.5/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/tests/hub-prod/test_upath.py` & `lamindb_setup-0.69.5/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/tests/storage/test_hashing.py` & `lamindb_setup-0.69.5/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/tests/storage/test_storage_access.py` & `lamindb_setup-0.69.5/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/tests/storage/test_storage_basis.py` & `lamindb_setup-0.69.5/tests/storage/test_storage_basis.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/tests/storage/test_storage_stats.py` & `lamindb_setup-0.69.5/tests/storage/test_storage_stats.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.4/PKG-INFO` & `lamindb_setup-0.69.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.69.4
+Version: 0.69.5
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```


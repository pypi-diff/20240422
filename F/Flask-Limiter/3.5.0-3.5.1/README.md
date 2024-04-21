# Comparing `tmp/Flask-Limiter-3.5.0.tar.gz` & `tmp/Flask-Limiter-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Limiter-3.5.0.tar", last modified: Thu Aug 31 00:38:30 2023, max compression
+gzip compressed data, was "Flask-Limiter-3.5.1.tar", last modified: Sun Feb 11 20:56:01 2024, max compression
```

## Comparing `Flask-Limiter-3.5.0.tar` & `Flask-Limiter-3.5.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 00:38:30.983200 Flask-Limiter-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (999)      514 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/CLASSIFIERS
--rw-r--r--   0 runner    (1001) docker     (999)      378 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/CONTRIBUTIONS.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 00:38:30.979200 Flask-Limiter-3.5.0/Flask_Limiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     5983 2023-08-31 00:38:30.000000 Flask-Limiter-3.5.0/Flask_Limiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1707 2023-08-31 00:38:30.000000 Flask-Limiter-3.5.0/Flask_Limiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 00:38:30.000000 Flask-Limiter-3.5.0/Flask_Limiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       54 2023-08-31 00:38:30.000000 Flask-Limiter-3.5.0/Flask_Limiter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 00:38:30.000000 Flask-Limiter-3.5.0/Flask_Limiter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)      153 2023-08-31 00:38:30.000000 Flask-Limiter-3.5.0/Flask_Limiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       14 2023-08-31 00:38:30.000000 Flask-Limiter-3.5.0/Flask_Limiter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)    18261 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1061 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (999)      264 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     5983 2023-08-31 00:38:30.983200 Flask-Limiter-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     4894 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 00:38:30.979200 Flask-Limiter-3.5.0/doc/
--rw-r--r--   0 runner    (1001) docker     (999)     6807 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 00:38:30.979200 Flask-Limiter-3.5.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 00:38:30.979200 Flask-Limiter-3.5.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (999)      493 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/_static/colors.css
--rw-r--r--   0 runner    (1001) docker     (999)     1606 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (999)      439 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/_static/limiter.css
--rw-r--r--   0 runner    (1001) docker     (999)    27408 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/_static/logo-og.png
--rw-r--r--   0 runner    (1001) docker     (999)    47774 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (999)   183556 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (999)    15123 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/_static/tap-icon.ico
--rw-r--r--   0 runner    (1001) docker     (999)    15350 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/_static/tap-icon.png
--rw-r--r--   0 runner    (1001) docker     (999)   161289 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/_static/tap-icon.svg
--rw-r--r--   0 runner    (1001) docker     (999)    20934 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/_static/tap-logo.png
--rw-r--r--   0 runner    (1001) docker     (999)      320 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (999)       31 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2232 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (999)     3078 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (999)    12839 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (999)      634 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/development.rst
--rw-r--r--   0 runner    (1001) docker     (999)    14292 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)      313 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/misc.rst
--rw-r--r--   0 runner    (1001) docker     (999)    19548 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/recipes.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2322 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/strategies.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1456 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/doc/source/theme_config.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 00:38:30.983200 Flask-Limiter-3.5.0/flask_limiter/
--rw-r--r--   0 runner    (1001) docker     (999)      470 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      379 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/_compat.py
--rw-r--r--   0 runner    (1001) docker     (999)      497 2023-08-31 00:38:30.983200 Flask-Limiter-3.5.0/flask_limiter/_version.py
--rw-r--r--   0 runner    (1001) docker     (999)    23563 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/commands.py
--rw-r--r--   0 runner    (1001) docker     (999)     2847 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 00:38:30.983200 Flask-Limiter-3.5.0/flask_limiter/contrib/
--rw-r--r--   0 runner    (1001) docker     (999)       28 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      270 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/contrib/util.py
--rw-r--r--   0 runner    (1001) docker     (999)     1082 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/errors.py
--rw-r--r--   0 runner    (1001) docker     (999)    52178 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/extension.py
--rw-r--r--   0 runner    (1001) docker     (999)    10493 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/manager.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/py.typed
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/typing.py
--rw-r--r--   0 runner    (1001) docker     (999)      960 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/util.py
--rw-r--r--   0 runner    (1001) docker     (999)       47 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/version.py
--rw-r--r--   0 runner    (1001) docker     (999)     5525 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/flask_limiter/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (999)       29 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 00:38:30.983200 Flask-Limiter-3.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (999)       54 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (999)      232 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (999)       72 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (999)      253 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (999)      762 2023-08-31 00:38:30.983200 Flask-Limiter-3.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (999)     1412 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 00:38:30.983200 Flask-Limiter-3.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)    19080 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/tests/test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (999)     4467 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (999)     4360 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (999)     1749 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/tests/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (999)    30256 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (999)    11651 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (999)    29037 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/tests/test_flask_ext.py
--rw-r--r--   0 runner    (1001) docker     (999)     6457 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/tests/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (999)     1629 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (999)     6629 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (999)    81180 2023-08-31 00:38:21.000000 Flask-Limiter-3.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 20:56:01.670295 Flask-Limiter-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/CLASSIFIERS
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/CONTRIBUTIONS.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 20:56:01.670295 Flask-Limiter-3.5.1/Flask_Limiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-02-11 20:56:01.000000 Flask-Limiter-3.5.1/Flask_Limiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-02-11 20:56:01.000000 Flask-Limiter-3.5.1/Flask_Limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 20:56:01.000000 Flask-Limiter-3.5.1/Flask_Limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-11 20:56:01.000000 Flask-Limiter-3.5.1/Flask_Limiter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 20:56:01.000000 Flask-Limiter-3.5.1/Flask_Limiter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-11 20:56:01.000000 Flask-Limiter-3.5.1/Flask_Limiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-11 20:56:01.000000 Flask-Limiter-3.5.1/Flask_Limiter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-02-11 20:56:01.670295 Flask-Limiter-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 20:56:01.662295 Flask-Limiter-3.5.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 20:56:01.666295 Flask-Limiter-3.5.1/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 20:56:01.666295 Flask-Limiter-3.5.1/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/_static/colors.css
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/_static/limiter.css
+-rw-r--r--   0 runner    (1001) docker     (127)    27408 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/_static/logo-og.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47774 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   183556 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/_static/tap-icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/_static/tap-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   161289 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/_static/tap-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    20934 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/_static/tap-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/recipes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/strategies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/doc/source/theme_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 20:56:01.674295 Flask-Limiter-3.5.1/flask_limiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-11 20:56:01.674295 Flask-Limiter-3.5.1/flask_limiter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23575 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 20:56:01.670295 Flask-Limiter-3.5.1/flask_limiter/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/contrib/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52179 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/flask_limiter/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 20:56:01.670295 Flask-Limiter-3.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-02-11 20:56:01.670295 Flask-Limiter-3.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1414 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 20:56:01.670295 Flask-Limiter-3.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19080 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/tests/test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/tests/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30256 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29038 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/tests/test_flask_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/tests/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81180 2024-02-11 20:55:55.000000 Flask-Limiter-3.5.1/versioneer.py
```

### Comparing `Flask-Limiter-3.5.0/CLASSIFIERS` & `Flask-Limiter-3.5.1/CLASSIFIERS`

 * *Files 1% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 Framework :: Flask
 Intended Audience :: Developers
 License :: OSI Approved :: MIT License
 Operating System :: MacOS
 Operating System :: POSIX :: Linux
 Operating System :: OS Independent
 Topic :: Software Development :: Libraries :: Python Modules
-Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.8
 Programming Language :: Python :: 3.9
 Programming Language :: Python :: 3.10
 Programming Language :: Python :: 3.11
+Programming Language :: Python :: 3.12
```

### Comparing `Flask-Limiter-3.5.0/Flask_Limiter.egg-info/PKG-INFO` & `Flask-Limiter-3.5.1/Flask_Limiter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Limiter
-Version: 3.5.0
+Version: 3.5.1
 Summary: Rate limiting for flask applications
 Home-page: https://flask-limiter.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/flask-limiter
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,24 +12,32 @@
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+License-File: LICENSE.txt
+Requires-Dist: limits>=2.8
+Requires-Dist: Flask>=2
+Requires-Dist: ordered-set<5,>4
+Requires-Dist: rich<14,>=12
+Requires-Dist: typing_extensions>=4
 Provides-Extra: redis
+Requires-Dist: limits[redis]; extra == "redis"
 Provides-Extra: memcached
+Requires-Dist: limits[memcached]; extra == "memcached"
 Provides-Extra: mongodb
-License-File: LICENSE.txt
+Requires-Dist: limits[mongodb]; extra == "mongodb"
 
 .. |ci| image:: https://github.com/alisaifee/flask-limiter/workflows/CI/badge.svg?branch=master
    :target: https://github.com/alisaifee/flask-limiter/actions?query=branch%3Amaster+workflow%3ACI
 .. |codecov| image:: https://codecov.io/gh/alisaifee/flask-limiter/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/alisaifee/flask-limiter
 .. |pypi| image:: https://img.shields.io/pypi/v/Flask-Limiter.svg?style=flat-square
    :target: https://pypi.python.org/pypi/Flask-Limiter
@@ -43,35 +51,26 @@
 *************
 
 
 |docs| |ci| |codecov| |pypi| |license|
 
 **Flask-Limiter** adds rate limiting to `Flask <https://flask.palletsprojects.com>`_ applications.
 
-----
-
-Sponsored by `Zuplo <https://zuplo.link/3NuX0co>`_ a fully-managed API Gateway for developers.
-Add `dynamic rate-limiting <https://zuplo.link/flask-dynamic-rate-limit>`_ authentication and more to any API in minutes.
-Learn more at `zuplo.com <https://zuplo.link/3NuX0co>`_
-
-----
-
-
 You can configure rate limits at different levels such as:
 
 - Application wide global limits per user
 - Default limits per route
 - By `Blueprints <https://flask-limiter.readthedocs.io/en/latest/recipes.html#rate-limiting-all-routes-in-a-blueprint>`_
 - By `Class-based views <https://flask-limiter.readthedocs.io/en/latest/recipes.html#using-flask-pluggable-views>`_
 - By `individual routes <https://flask-limiter.readthedocs.io/en/latest/index.html#decorators-to-declare-rate-limits>`_
 
 **Flask-Limiter** can be `configured <https://flask-limiter.readthedocs.io/en/latest/configuration.html>`_ to fit your application in many ways, including:
 
 - Persistance to various commonly used `storage backends <https://flask-limiter.readthedocs.io/en/latest/#configuring-a-storage-backend>`_
-  (such as Redis, Memcached & MongoDB)
+  (such as Redis, Memcached, MongoDB & Etcd)
   via `limits <https://limits.readthedocs.io/en/stable/storage.html>`__
 - Any rate limiting strategy supported by `limits <https://limits.readthedocs.io/en/stable/strategies.html>`__
 
 Follow the quickstart below to get started or `read the documentation <http://flask-limiter.readthedocs.org/en/latest>`_ for more details.
 
 
 Quickstart
@@ -105,14 +104,16 @@
        # storage_uri="redis+cluster://localhost:7000,localhost:7001,localhost:70002",
        # Memcached
        # storage_uri="memcached://localhost:11211",
        # Memcached Cluster
        # storage_uri="memcached://localhost:11211,localhost:11212,localhost:11213",
        # MongoDB
        # storage_uri="mongodb://localhost:27017",
+       # Etcd
+       # storage_uri="etcd://localhost:2379",
        strategy="fixed-window", # or "moving-window"
    )
 
    @app.route("/slow")
    @limiter.limit("1 per day")
    def slow():
        return "24"
```

### Comparing `Flask-Limiter-3.5.0/Flask_Limiter.egg-info/SOURCES.txt` & `Flask-Limiter-3.5.1/Flask_Limiter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/HISTORY.rst` & `Flask-Limiter-3.5.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 .. :changelog:
 
 Changelog
 =========
 
+v3.5.1
+------
+Release Date: 2024-02-11
+
+* Chores
+
+  * Update development dependencies
+  * Use ruff for all linting
+  * Update CI compatibility matrix
+
 v3.5.0
 ------
 Release Date: 2023-08-30
 
 * Feature
 
   * Add `meta_limits` to allow for creating upper limits for
@@ -881,14 +891,15 @@
 
 
 
 
 
 
 
+
```

### Comparing `Flask-Limiter-3.5.0/LICENSE.txt` & `Flask-Limiter-3.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/PKG-INFO` & `Flask-Limiter-3.5.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Limiter
-Version: 3.5.0
+Version: 3.5.1
 Summary: Rate limiting for flask applications
 Home-page: https://flask-limiter.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/flask-limiter
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,24 +12,32 @@
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+License-File: LICENSE.txt
+Requires-Dist: limits>=2.8
+Requires-Dist: Flask>=2
+Requires-Dist: ordered-set<5,>4
+Requires-Dist: rich<14,>=12
+Requires-Dist: typing_extensions>=4
 Provides-Extra: redis
+Requires-Dist: limits[redis]; extra == "redis"
 Provides-Extra: memcached
+Requires-Dist: limits[memcached]; extra == "memcached"
 Provides-Extra: mongodb
-License-File: LICENSE.txt
+Requires-Dist: limits[mongodb]; extra == "mongodb"
 
 .. |ci| image:: https://github.com/alisaifee/flask-limiter/workflows/CI/badge.svg?branch=master
    :target: https://github.com/alisaifee/flask-limiter/actions?query=branch%3Amaster+workflow%3ACI
 .. |codecov| image:: https://codecov.io/gh/alisaifee/flask-limiter/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/alisaifee/flask-limiter
 .. |pypi| image:: https://img.shields.io/pypi/v/Flask-Limiter.svg?style=flat-square
    :target: https://pypi.python.org/pypi/Flask-Limiter
@@ -43,35 +51,26 @@
 *************
 
 
 |docs| |ci| |codecov| |pypi| |license|
 
 **Flask-Limiter** adds rate limiting to `Flask <https://flask.palletsprojects.com>`_ applications.
 
-----
-
-Sponsored by `Zuplo <https://zuplo.link/3NuX0co>`_ a fully-managed API Gateway for developers.
-Add `dynamic rate-limiting <https://zuplo.link/flask-dynamic-rate-limit>`_ authentication and more to any API in minutes.
-Learn more at `zuplo.com <https://zuplo.link/3NuX0co>`_
-
-----
-
-
 You can configure rate limits at different levels such as:
 
 - Application wide global limits per user
 - Default limits per route
 - By `Blueprints <https://flask-limiter.readthedocs.io/en/latest/recipes.html#rate-limiting-all-routes-in-a-blueprint>`_
 - By `Class-based views <https://flask-limiter.readthedocs.io/en/latest/recipes.html#using-flask-pluggable-views>`_
 - By `individual routes <https://flask-limiter.readthedocs.io/en/latest/index.html#decorators-to-declare-rate-limits>`_
 
 **Flask-Limiter** can be `configured <https://flask-limiter.readthedocs.io/en/latest/configuration.html>`_ to fit your application in many ways, including:
 
 - Persistance to various commonly used `storage backends <https://flask-limiter.readthedocs.io/en/latest/#configuring-a-storage-backend>`_
-  (such as Redis, Memcached & MongoDB)
+  (such as Redis, Memcached, MongoDB & Etcd)
   via `limits <https://limits.readthedocs.io/en/stable/storage.html>`__
 - Any rate limiting strategy supported by `limits <https://limits.readthedocs.io/en/stable/strategies.html>`__
 
 Follow the quickstart below to get started or `read the documentation <http://flask-limiter.readthedocs.org/en/latest>`_ for more details.
 
 
 Quickstart
@@ -105,14 +104,16 @@
        # storage_uri="redis+cluster://localhost:7000,localhost:7001,localhost:70002",
        # Memcached
        # storage_uri="memcached://localhost:11211",
        # Memcached Cluster
        # storage_uri="memcached://localhost:11211,localhost:11212,localhost:11213",
        # MongoDB
        # storage_uri="mongodb://localhost:27017",
+       # Etcd
+       # storage_uri="etcd://localhost:2379",
        strategy="fixed-window", # or "moving-window"
    )
 
    @app.route("/slow")
    @limiter.limit("1 per day")
    def slow():
        return "24"
```

### Comparing `Flask-Limiter-3.5.0/README.rst` & `Flask-Limiter-3.5.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -14,35 +14,26 @@
 *************
 
 
 |docs| |ci| |codecov| |pypi| |license|
 
 **Flask-Limiter** adds rate limiting to `Flask <https://flask.palletsprojects.com>`_ applications.
 
-----
-
-Sponsored by `Zuplo <https://zuplo.link/3NuX0co>`_ a fully-managed API Gateway for developers.
-Add `dynamic rate-limiting <https://zuplo.link/flask-dynamic-rate-limit>`_ authentication and more to any API in minutes.
-Learn more at `zuplo.com <https://zuplo.link/3NuX0co>`_
-
-----
-
-
 You can configure rate limits at different levels such as:
 
 - Application wide global limits per user
 - Default limits per route
 - By `Blueprints <https://flask-limiter.readthedocs.io/en/latest/recipes.html#rate-limiting-all-routes-in-a-blueprint>`_
 - By `Class-based views <https://flask-limiter.readthedocs.io/en/latest/recipes.html#using-flask-pluggable-views>`_
 - By `individual routes <https://flask-limiter.readthedocs.io/en/latest/index.html#decorators-to-declare-rate-limits>`_
 
 **Flask-Limiter** can be `configured <https://flask-limiter.readthedocs.io/en/latest/configuration.html>`_ to fit your application in many ways, including:
 
 - Persistance to various commonly used `storage backends <https://flask-limiter.readthedocs.io/en/latest/#configuring-a-storage-backend>`_
-  (such as Redis, Memcached & MongoDB)
+  (such as Redis, Memcached, MongoDB & Etcd)
   via `limits <https://limits.readthedocs.io/en/stable/storage.html>`__
 - Any rate limiting strategy supported by `limits <https://limits.readthedocs.io/en/stable/strategies.html>`__
 
 Follow the quickstart below to get started or `read the documentation <http://flask-limiter.readthedocs.org/en/latest>`_ for more details.
 
 
 Quickstart
@@ -76,14 +67,16 @@
        # storage_uri="redis+cluster://localhost:7000,localhost:7001,localhost:70002",
        # Memcached
        # storage_uri="memcached://localhost:11211",
        # Memcached Cluster
        # storage_uri="memcached://localhost:11211,localhost:11212,localhost:11213",
        # MongoDB
        # storage_uri="mongodb://localhost:27017",
+       # Etcd
+       # storage_uri="etcd://localhost:2379",
        strategy="fixed-window", # or "moving-window"
    )
 
    @app.route("/slow")
    @limiter.limit("1 per day")
    def slow():
        return "24"
```

### Comparing `Flask-Limiter-3.5.0/doc/Makefile` & `Flask-Limiter-3.5.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/_static/logo-og.png` & `Flask-Limiter-3.5.1/doc/source/_static/logo-og.png`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/_static/logo.png` & `Flask-Limiter-3.5.1/doc/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/_static/logo.svg` & `Flask-Limiter-3.5.1/doc/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/_static/tap-icon.ico` & `Flask-Limiter-3.5.1/doc/source/_static/tap-icon.ico`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/_static/tap-icon.png` & `Flask-Limiter-3.5.1/doc/source/_static/tap-icon.png`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/_static/tap-icon.svg` & `Flask-Limiter-3.5.1/doc/source/_static/tap-icon.svg`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/_static/tap-logo.png` & `Flask-Limiter-3.5.1/doc/source/_static/tap-logo.png`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/cli.rst` & `Flask-Limiter-3.5.1/doc/source/cli.rst`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/conf.py` & `Flask-Limiter-3.5.1/doc/source/conf.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import os
 import re
 import sys
 
 sys.path.insert(0, os.path.abspath("../../"))
 sys.path.insert(0, os.path.abspath("./"))
 
-import flask_limiter
-
 from theme_config import *
 
+import flask_limiter
+
 description = "Flask-Limiter adds rate limiting to flask applications."
 copyright = "2023, Ali-Akber Saifee"
 project = "Flask-Limiter"
 
 ahead = 0
 
 if ".post0.dev" in flask_limiter.__version__:
```

### Comparing `Flask-Limiter-3.5.0/doc/source/configuration.rst` & `Flask-Limiter-3.5.1/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/development.rst` & `Flask-Limiter-3.5.1/doc/source/development.rst`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/index.rst` & `Flask-Limiter-3.5.1/doc/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,14 @@
 
 .. image:: _static/logo.png
     :target: /
     :width: 600px
     :align: center
     :class: logo
 
-.. container:: sponsorship
-
-   .. container:: left
-
-      | Sponsored by `Zuplo <https://zuplo.link/3hLbXv5>`_, a fully-managed API gateway for developers.
-      | Add `dynamic rate-limiting <https://zuplo.link/3hxWXAv>`_, authentication and more to any API in minutes.
-
-   .. container:: right
-
-      .. container:: sponsorship-button
-
-         `Try Zuplo <https://zuplo.link/3hLbXv5>`_
-
 =============
 Flask-Limiter
 =============
 
 .. currentmodule:: flask_limiter
 
 .. toctree::
```

### Comparing `Flask-Limiter-3.5.0/doc/source/recipes.rst` & `Flask-Limiter-3.5.1/doc/source/recipes.rst`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/strategies.rst` & `Flask-Limiter-3.5.1/doc/source/strategies.rst`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/doc/source/theme_config.py` & `Flask-Limiter-3.5.1/doc/source/theme_config.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/flask_limiter/commands.py` & `Flask-Limiter-3.5.1/flask_limiter/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,20 +120,22 @@
     for limit in limits[0] + limits[1]:
         if endpoint:
             view_func = app.view_functions.get(endpoint, None)
             source = (
                 "blueprint"
                 if blueprint
                 and limit in limiter.limit_manager.blueprint_limits(app, blueprint)
-                else "route"
-                if limit
-                in limiter.limit_manager.decorated_limits(
-                    get_qualified_name(view_func) if view_func else ""
+                else (
+                    "route"
+                    if limit
+                    in limiter.limit_manager.decorated_limits(
+                        get_qualified_name(view_func) if view_func else ""
+                    )
+                    else "default"
                 )
-                else "default"
             )
         else:
             source = "default"
         if limit.per_method and rule and rule.methods:
             for method in rule.methods:
                 rendered = render_limit(limit, False)
                 entry = f"[{source}]{rendered} [http]({method})[/http][/{source}]"
@@ -194,15 +196,15 @@
 
 @click.group(help="Flask-Limiter maintenance & utility commmands")
 def cli() -> None:
     pass
 
 
 @cli.command(help="View the extension configuration")
-@with_appcontext  # type: ignore
+@with_appcontext
 def config() -> None:
     with current_app.test_request_context():
         console = Console(theme=limiter_theme)
         limiters = list(current_app.extensions.get("limiter", set()))
         limiter = limiters and list(limiters)[0]
         if limiter:
             extension_details = Table(title="Flask-Limiter Config")
@@ -360,15 +362,15 @@
 
 @cli.command(help="Enumerate details about all routes with rate limits")
 @click.option("--endpoint", default=None, help="Endpoint to filter by")
 @click.option("--path", default=None, help="Path to filter by")
 @click.option("--method", default=None, help="HTTP Method to filter by")
 @click.option("--key", default=None, help="Test the limit")
 @click.option("--watch/--no-watch", default=False, help="Create a live dashboard")
-@with_appcontext  # type: ignore
+@with_appcontext
 def limits(
     endpoint: Optional[str] = None,
     path: Optional[str] = None,
     method: str = "GET",
     key: Optional[str] = None,
     watch: bool = False,
 ) -> None:
@@ -482,15 +484,15 @@
 
 @cli.command(help="Clear limits for a specific key")
 @click.option("--endpoint", default=None, help="Endpoint to filter by")
 @click.option("--path", default=None, help="Path to filter by")
 @click.option("--method", default=None, help="HTTP Method to filter by")
 @click.option("--key", default=None, required=True, help="Key to reset the limits for")
 @click.option("-y", is_flag=True, help="Skip prompt for confirmation")
-@with_appcontext  # type: ignore
+@with_appcontext
 def clear(
     key: str,
     endpoint: Optional[str] = None,
     path: Optional[str] = None,
     method: str = "GET",
     y: bool = False,
 ) -> None:
```

### Comparing `Flask-Limiter-3.5.0/flask_limiter/constants.py` & `Flask-Limiter-3.5.1/flask_limiter/constants.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/flask_limiter/errors.py` & `Flask-Limiter-3.5.1/flask_limiter/errors.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/flask_limiter/extension.py` & `Flask-Limiter-3.5.1/flask_limiter/extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Flask-Limiter Extension
 """
+
 from __future__ import annotations
 
 import dataclasses
 import datetime
 import itertools
 import logging
 import time
```

### Comparing `Flask-Limiter-3.5.0/flask_limiter/manager.py` & `Flask-Limiter-3.5.1/flask_limiter/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/flask_limiter/util.py` & `Flask-Limiter-3.5.1/flask_limiter/util.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/flask_limiter/wrappers.py` & `Flask-Limiter-3.5.1/flask_limiter/wrappers.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/setup.cfg` & `Flask-Limiter-3.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/setup.py` & `Flask-Limiter-3.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 
 
 """
 __author__ = "Ali-Akber Saifee"
 __email__ = "ali@indydevs.org"
 __copyright__ = "Copyright 2023, Ali-Akber Saifee"
 
-from setuptools import setup, find_packages
 import os
+
+from setuptools import find_packages, setup
+
 import versioneer
 
 this_dir = os.path.abspath(os.path.dirname(__file__))
 REQUIREMENTS = filter(
     None, open(os.path.join(this_dir, "requirements", "main.txt")).read().splitlines()
 )
 EXTRA_REQUIREMENTS = {
@@ -34,15 +36,15 @@
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     install_requires=list(REQUIREMENTS),
     classifiers=[k for k in open("CLASSIFIERS").read().split("\n") if k],
     description="Rate limiting for flask applications",
     long_description=open("README.rst").read(),
     packages=find_packages(exclude=["tests*"]),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     extras_require=EXTRA_REQUIREMENTS,
     include_package_data=True,
     package_data={
         "flask_limiter": ["py.typed"],
     },
     entry_points={
         'flask.commands': [
```

### Comparing `Flask-Limiter-3.5.0/tests/test_blueprints.py` & `Flask-Limiter-3.5.1/tests/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/tests/test_commands.py` & `Flask-Limiter-3.5.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/tests/test_configuration.py` & `Flask-Limiter-3.5.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/tests/test_context_manager.py` & `Flask-Limiter-3.5.1/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/tests/test_decorators.py` & `Flask-Limiter-3.5.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/tests/test_error_handling.py` & `Flask-Limiter-3.5.1/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/tests/test_flask_ext.py` & `Flask-Limiter-3.5.1/tests/test_flask_ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 
 """
+
 import logging
 import time
 from collections import Counter
 from unittest import mock
 
 import hiro
 from flask import Flask, abort, make_response, request
```

### Comparing `Flask-Limiter-3.5.0/tests/test_regressions.py` & `Flask-Limiter-3.5.1/tests/test_regressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 
 """
+
 import time
 
 import hiro
 from flask import Blueprint
 
 from flask_limiter.constants import ConfigVars
```

### Comparing `Flask-Limiter-3.5.0/tests/test_storage.py` & `Flask-Limiter-3.5.1/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/tests/test_views.py` & `Flask-Limiter-3.5.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.5.0/versioneer.py` & `Flask-Limiter-3.5.1/versioneer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -278,21 +278,21 @@
 # pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
 # pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
 # pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
 # pylint:disable=attribute-defined-outside-init,too-many-arguments
 
 import configparser
 import errno
+import functools
 import json
 import os
 import re
 import subprocess
 import sys
 from typing import Callable, Dict
-import functools
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
```


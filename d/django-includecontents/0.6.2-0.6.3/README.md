# Comparing `tmp/django_includecontents-0.6.2.tar.gz` & `tmp/django_includecontents-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_includecontents-0.6.2.tar", last modified: Sun Apr 21 22:44:34 2024, max compression
+gzip compressed data, was "django_includecontents-0.6.3.tar", last modified: Sun Apr 21 23:01:27 2024, max compression
```

## Comparing `django_includecontents-0.6.2.tar` & `django_includecontents-0.6.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     5368 2024-04-21 20:37:00.117665 django_includecontents-0.6.2/README.md
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.6.2/includecontents/__init__.py
--rw-r--r--   0        0        0     1000 2024-04-19 05:13:37.190112 django_includecontents-0.6.2/includecontents/backend.py
--rw-r--r--   0        0        0     4596 2024-04-19 05:31:33.346108 django_includecontents-0.6.2/includecontents/base.py
--rw-r--r--   0        0        0     1401 2024-04-09 04:42:05.196722 django_includecontents-0.6.2/includecontents/engine.py
--rw-r--r--   0        0        0     1663 2024-04-18 05:37:15.283141 django_includecontents-0.6.2/includecontents/loaders.py
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.6.2/includecontents/templatetags/__init__.py
--rw-r--r--   0        0        0    15820 2024-04-21 22:42:06.493754 django_includecontents-0.6.2/includecontents/templatetags/includecontents.py
--rw-r--r--   0        0        0     1220 2024-04-21 22:44:34.041653 django_includecontents-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      144 2024-04-19 05:31:17.752738 django_includecontents-0.6.2/tests/settings.py
--rw-r--r--   0        0        0      168 2024-04-18 05:37:15.283141 django_includecontents-0.6.2/tests/templates/components/card.html
--rw-r--r--   0        0        0      163 2024-04-21 20:37:00.117665 django_includecontents-0.6.2/tests/templates/components/card_extend.html
--rw-r--r--   0        0        0       42 2024-04-21 22:40:07.372787 django_includecontents-0.6.2/tests/templates/components/empty_props.html
--rw-r--r--   0        0        0       81 2024-04-09 04:52:09.297567 django_includecontents-0.6.2/tests/templates/multiline.html
--rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.6.2/tests/templates/test_component/attrs.html
--rw-r--r--   0        0        0      162 2024-04-18 05:37:15.283141 django_includecontents-0.6.2/tests/templates/test_component/extend_class.html
--rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.6.2/tests/templates/test_component/index.html
--rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.6.2/tests/templates/test_component/missing_attr.html
--rw-r--r--   0        0        0       24 2024-04-09 21:51:57.449090 django_includecontents-0.6.2/tests/templates/test_component/missing_closing_tag.html
--rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.6.2/tests/templates/test_tag/basic.html
--rw-r--r--   0        0        0       54 2024-04-21 20:37:00.117665 django_includecontents-0.6.2/tests/templates/test_tag/inner.html
--rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.6.2/tests/templates/test_tag/with_attr.html
--rw-r--r--   0        0        0     2062 2024-04-21 22:40:28.685646 django_includecontents-0.6.2/tests/test_component.py
--rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.6.2/tests/test_multiline.py
--rw-r--r--   0        0        0      454 2024-04-09 04:52:09.297567 django_includecontents-0.6.2/tests/test_tag.py
--rw-r--r--   0        0        0     6384 1970-01-01 00:00:00.000000 django_includecontents-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     5368 2024-04-21 20:37:00.117665 django_includecontents-0.6.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.6.3/includecontents/__init__.py
+-rw-r--r--   0        0        0     1000 2024-04-19 05:13:37.190112 django_includecontents-0.6.3/includecontents/backend.py
+-rw-r--r--   0        0        0     4596 2024-04-19 05:31:33.346108 django_includecontents-0.6.3/includecontents/base.py
+-rw-r--r--   0        0        0     1401 2024-04-09 04:42:05.196722 django_includecontents-0.6.3/includecontents/engine.py
+-rw-r--r--   0        0        0     1663 2024-04-18 05:37:15.283141 django_includecontents-0.6.3/includecontents/loaders.py
+-rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.6.3/includecontents/templatetags/__init__.py
+-rw-r--r--   0        0        0    15818 2024-04-21 22:54:42.358713 django_includecontents-0.6.3/includecontents/templatetags/includecontents.py
+-rw-r--r--   0        0        0     1220 2024-04-21 23:01:27.692575 django_includecontents-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      144 2024-04-19 05:31:17.752738 django_includecontents-0.6.3/tests/settings.py
+-rw-r--r--   0        0        0      168 2024-04-18 05:37:15.283141 django_includecontents-0.6.3/tests/templates/components/card.html
+-rw-r--r--   0        0        0      163 2024-04-21 20:37:00.117665 django_includecontents-0.6.3/tests/templates/components/card_extend.html
+-rw-r--r--   0        0        0       42 2024-04-21 22:40:07.372787 django_includecontents-0.6.3/tests/templates/components/empty_props.html
+-rw-r--r--   0        0        0       81 2024-04-09 04:52:09.297567 django_includecontents-0.6.3/tests/templates/multiline.html
+-rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.6.3/tests/templates/test_component/attrs.html
+-rw-r--r--   0        0        0      162 2024-04-18 05:37:15.283141 django_includecontents-0.6.3/tests/templates/test_component/extend_class.html
+-rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.6.3/tests/templates/test_component/index.html
+-rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.6.3/tests/templates/test_component/missing_attr.html
+-rw-r--r--   0        0        0       24 2024-04-09 21:51:57.449090 django_includecontents-0.6.3/tests/templates/test_component/missing_closing_tag.html
+-rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.6.3/tests/templates/test_tag/basic.html
+-rw-r--r--   0        0        0       54 2024-04-21 20:37:00.117665 django_includecontents-0.6.3/tests/templates/test_tag/inner.html
+-rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.6.3/tests/templates/test_tag/with_attr.html
+-rw-r--r--   0        0        0     2062 2024-04-21 22:54:55.432044 django_includecontents-0.6.3/tests/test_component.py
+-rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.6.3/tests/test_multiline.py
+-rw-r--r--   0        0        0      454 2024-04-09 04:52:09.297567 django_includecontents-0.6.3/tests/test_tag.py
+-rw-r--r--   0        0        0     6384 1970-01-01 00:00:00.000000 django_includecontents-0.6.3/PKG-INFO
```

### Comparing `django_includecontents-0.6.2/README.md` & `django_includecontents-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.6.2/includecontents/backend.py` & `django_includecontents-0.6.3/includecontents/backend.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.6.2/includecontents/base.py` & `django_includecontents-0.6.3/includecontents/base.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.6.2/includecontents/engine.py` & `django_includecontents-0.6.3/includecontents/engine.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.6.2/includecontents/loaders.py` & `django_includecontents-0.6.3/includecontents/loaders.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.6.2/includecontents/templatetags/includecontents.py` & `django_includecontents-0.6.3/includecontents/templatetags/includecontents.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
 class Attrs(MutableMapping):
     def __init__(self):
         self._attrs: dict[str, Any] = {}
         self._nested_attrs: dict[str, Attrs] = {}
         self._extended: dict[str, dict[str, bool]] = {}
 
     def __getattr__(self, key):
-        if "key" not in self._nested_attrs:
+        if key not in self._nested_attrs:
             raise AttributeError(key)
         return self._nested_attrs[key]
 
     def __getitem__(self, key):
         return self._attrs[key]
 
     def __setitem__(self, key, value):
```

### Comparing `django_includecontents-0.6.2/pyproject.toml` & `django_includecontents-0.6.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-includecontents"
-version = "0.6.2"
+version = "0.6.3"
 description = "Django includecontents component-like tag"
 authors = [
     { name = "Chris Beaven", email = "smileychris@gmail.com" },
 ]
 dependencies = [
     "django",
 ]
```

### Comparing `django_includecontents-0.6.2/tests/test_component.py` & `django_includecontents-0.6.3/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.6.2/PKG-INFO` & `django_includecontents-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-includecontents
-Version: 0.6.2
+Version: 0.6.3
 Summary: Django includecontents component-like tag
 Author-Email: Chris Beaven <smileychris@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```


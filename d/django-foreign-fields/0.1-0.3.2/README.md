# Comparing `tmp/django-foreign-fields-0.1.tar.gz` & `tmp/django_foreign_fields-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-foreign-fields-0.1.tar", last modified: Thu May  3 20:25:43 2018, max compression
+gzip compressed data, was "django_foreign_fields-0.3.2.tar", last modified: Mon Apr 22 02:19:14 2024, max compression
```

## Comparing `django-foreign-fields-0.1.tar` & `django_foreign_fields-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 catena    (1000) catena    (1000)        0 2018-05-03 20:25:43.000000 django-foreign-fields-0.1/
--rw-r--r--   0 catena    (1000) catena    (1000)     1074 2018-05-03 17:02:24.000000 django-foreign-fields-0.1/LICENSE
-drwxrwxr-x   0 catena    (1000) catena    (1000)        0 2018-05-03 20:25:43.000000 django-foreign-fields-0.1/foreign_fields/
--rw-rw-r--   0 catena    (1000) catena    (1000)     1327 2018-05-03 17:48:22.000000 django-foreign-fields-0.1/foreign_fields/test_forms.py
--rw-rw-r--   0 catena    (1000) catena    (1000)     2196 2018-05-01 18:27:33.000000 django-foreign-fields-0.1/foreign_fields/tests.py
--rw-rw-r--   0 catena    (1000) catena    (1000)        0 2018-05-03 17:42:00.000000 django-foreign-fields-0.1/foreign_fields/__init__.py
--rw-rw-r--   0 catena    (1000) catena    (1000)      507 2018-05-02 04:21:13.000000 django-foreign-fields-0.1/foreign_fields/test_models.py
--rw-rw-r--   0 catena    (1000) catena    (1000)     2274 2018-05-02 01:35:44.000000 django-foreign-fields-0.1/foreign_fields/fields.py
-drwxrwxr-x   0 catena    (1000) catena    (1000)        0 2018-05-03 20:25:43.000000 django-foreign-fields-0.1/foreign_fields/migrations/
--rw-rw-r--   0 catena    (1000) catena    (1000)     1379 2018-05-03 17:48:36.000000 django-foreign-fields-0.1/foreign_fields/migrations/0001_initial.py
--rw-rw-r--   0 catena    (1000) catena    (1000)        0 2018-03-20 00:38:08.000000 django-foreign-fields-0.1/foreign_fields/migrations/__init__.py
--rw-rw-r--   0 catena    (1000) catena    (1000)     3771 2018-05-03 15:14:03.000000 django-foreign-fields-0.1/README.rst
--rw-rw-r--   0 catena    (1000) catena    (1000)       59 2018-05-03 16:50:22.000000 django-foreign-fields-0.1/MANIFEST.in
--rw-rw-r--   0 catena    (1000) catena    (1000)       38 2018-05-03 20:25:43.000000 django-foreign-fields-0.1/setup.cfg
--rw-rw-r--   0 catena    (1000) catena    (1000)     5526 2018-05-03 20:25:43.000000 django-foreign-fields-0.1/PKG-INFO
-drwxrwxr-x   0 catena    (1000) catena    (1000)        0 2018-05-03 20:25:43.000000 django-foreign-fields-0.1/django_foreign_fields.egg-info/
--rw-rw-r--   0 catena    (1000) catena    (1000)      434 2018-05-03 20:25:43.000000 django-foreign-fields-0.1/django_foreign_fields.egg-info/SOURCES.txt
--rw-rw-r--   0 catena    (1000) catena    (1000)     5526 2018-05-03 20:25:43.000000 django-foreign-fields-0.1/django_foreign_fields.egg-info/PKG-INFO
--rw-rw-r--   0 catena    (1000) catena    (1000)       15 2018-05-03 20:25:43.000000 django-foreign-fields-0.1/django_foreign_fields.egg-info/top_level.txt
--rw-rw-r--   0 catena    (1000) catena    (1000)        1 2018-05-03 20:25:43.000000 django-foreign-fields-0.1/django_foreign_fields.egg-info/dependency_links.txt
--rw-rw-r--   0 catena    (1000) catena    (1000)     1332 2018-05-03 20:23:03.000000 django-foreign-fields-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:14.387668 django_foreign_fields-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 02:19:10.000000 django_foreign_fields-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-22 02:19:10.000000 django_foreign_fields-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-22 02:19:14.387668 django_foreign_fields-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-22 02:19:10.000000 django_foreign_fields-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:14.387668 django_foreign_fields-0.3.2/django_foreign_fields.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-22 02:19:14.000000 django_foreign_fields-0.3.2/django_foreign_fields.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-22 02:19:14.000000 django_foreign_fields-0.3.2/django_foreign_fields.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 02:19:14.000000 django_foreign_fields-0.3.2/django_foreign_fields.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 02:19:14.000000 django_foreign_fields-0.3.2/django_foreign_fields.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:14.387668 django_foreign_fields-0.3.2/foreign_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:10.000000 django_foreign_fields-0.3.2/foreign_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-22 02:19:10.000000 django_foreign_fields-0.3.2/foreign_fields/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:14.387668 django_foreign_fields-0.3.2/foreign_fields/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-22 02:19:10.000000 django_foreign_fields-0.3.2/foreign_fields/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:10.000000 django_foreign_fields-0.3.2/foreign_fields/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-22 02:19:10.000000 django_foreign_fields-0.3.2/foreign_fields/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-22 02:19:10.000000 django_foreign_fields-0.3.2/foreign_fields/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-22 02:19:10.000000 django_foreign_fields-0.3.2/foreign_fields/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 02:19:14.387668 django_foreign_fields-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-22 02:19:10.000000 django_foreign_fields-0.3.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-foreign-fields-0.1/LICENSE` & `django_foreign_fields-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-foreign-fields-0.1/foreign_fields/test_forms.py` & `django_foreign_fields-0.3.2/foreign_fields/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-foreign-fields-0.1/foreign_fields/tests.py` & `django_foreign_fields-0.3.2/foreign_fields/tests.py`

 * *Files identical despite different names*

### Comparing `django-foreign-fields-0.1/foreign_fields/fields.py` & `django_foreign_fields-0.3.2/foreign_fields/fields.py`

 * *Files identical despite different names*

### Comparing `django-foreign-fields-0.1/foreign_fields/migrations/0001_initial.py` & `django_foreign_fields-0.3.2/foreign_fields/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-foreign-fields-0.1/README.rst` & `django_foreign_fields-0.3.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,103 +1,90 @@
-=====================
-Django Foreign Fields
-=====================
+# Django Foreign Fields
+
+[![PyPI](https://img.shields.io/pypi/v/django-foreign-fields.svg)](https://pypi.python.org/pypi/django-foreign-fields)
+
 Django Foreign Fields is a Django app that offers two new form fields that help handling foreign relationships in a easier way.
 
-Quick start
------------
-.. code:: bash
+## Quick start
+``bash
+pip install django-foreign-fields
+``
 
-   $ pip install django-foreign-fields
+## Usage
 
-Optional
-^^^^^^^^
-If it's desired to test the package fields, it's necessary to install it on the project settings:
+Django-foreign-fields adds two new form fields `ForeignField` and `TextAreaToManyField`.
 
-1. Add "django-foreign-fields" to your INSTALLED_APPS setting like this::
+## Fields
 
-    INSTALLED_APPS = [
-        ...
-        'django-foreign-fields',
-    ]
+Both form fields need two new arguments: `to` and `selector`.
 
-2. Run `python manage.py test django-foreign-fields` to test the foreign fields.
+* `to`: the **target** model of the relationship. Declaring the **target** model as the first parameter will automatically be detected as the **to** argument.
 
-Usage
------
-Django-foreign-fields adds two new form fields ``ForeignField`` and ``TextAreaToManyField``.
+* `selector`: the model field where the given value will be searched on.
 
-Fields
-^^^^^^
-Both form fields need two new arguments: ``to`` and ``selector``.
+### ForeignField
 
-* ``to``: the `target` model of the relationship. Declaring the `target` model as the first parameter will automatically be detected as the `to` argument.
+Receives data and searches for an object in database that has that unique value on the given field. The object is stored as a `ForeignKey`.
 
-* ``selector``: the model field where the given value will be searched on.
+### TextAreaToManyField
 
-ForeignField
-""""""""""""
-Receives data and searches for an object in database that has that unique value on the given field. The object is stored as a ``ForeignKey``.
+Breaks all lines in a `Textarea` and use each one to find objects that correspond to each search. Each search must return a unique object, then, all objects are stored in a `ManyToMany` relationship.
 
-TextAreaToManyField
-"""""""""""""""""""
-Breaks all lines in a ``Textarea`` and use each one to find objects that correspond to each search. Each search must return a unique object, then, all objects are stored in a ``ManyToMany`` relationship.
+## Examples
 
-Examples
-^^^^^^^^
-ForeignField
-""""""""""""
-Given you already have two models, one ``Target`` that holds some information and one ``Referrer`` that will make a foreign relationship to a particular field:
+### ForeignField
 
-.. code:: python
+Given you already have two models, one `Target` that holds some information and one `Referrer` that will make a foreign relationship to a particular field:
 
+```python
    class Target(models.Model):
       name = models.TextField()
 
    class Referrer(models.Model):
       foreign = models.ForeignKey()
+```
 
-It will be needed a new form for the ``Referrer``.
-
-The original form field that holds the foreign key relation on the ``Referrer`` will be substituted for the ``ForeignField``:
+It will be needed a new form for the `Referrer`.
 
-.. code:: python
+The original form field that holds the foreign key relation on the `Referrer` will be substituted for the `ForeignField`:
 
+```python
    import foreign_fields.ForeignField
 
    class ReferrerForm(forms.ModelForm):
       foreign = foreign_fields.ForeignField(to=Target, selector='name')
       
       class Meta:
-           model = Referrer
+         model = Referrer
+```
 
-Now you can use the form on your ``View``. The default widget is ``TextInput``, so when you enter a string in the field and save the form, the ``ForeignField`` will search for a ``Target`` that has the given string in it's ``name`` field that must be unique. If the field is not unique, it will be given a ``ValidationError``.
+Now you can use the form on your `View`. The default widget is `TextInput`, so when you enter a string in the field and save the form, the `ForeignField` will search for a `Target` that has the given string in it's `name` field that must be unique. If the field is not unique, it will be given a `ValidationError`.
 
-It's possible to change the foreign widget into others such as ``NumberInput`` or ``DateInput``.
+It's possible to change the foreign widget into others such as `NumberInput` or `DateInput`.
 
-TextAreaToManyField
-""""""""""""
-Given you already have two models, one ``Target`` that holds some information and one ``Referrer`` that will make a many to many relationship to a particular field:
+###  TextAreaToManyField
 
-.. code:: python
+Given you already have two models, one `Target` that holds some information and one `Referrer` that will make a many to many relationship to a particular field:
 
+```python
    class Target(models.Model):
       name = models.TextField()
 
    class Referrer(models.Model):
       many_to_many = models.ManyToManyField()
+```
 
-It will be needed a new form for the ``Referrer``.
-
-The original form field that holds the many to many relation on the ``Referrer`` will be substituted for the ``TextAreaToManyField``:
+It will be needed a new form for the `Referrer`.
 
-.. code:: python
+The original form field that holds the many to many relation on the `Referrer` will be substituted for the `TextAreaToManyField`:
 
+```python
    import foreign_fields.TextAreaToManyField
 
    class ReferrerForm(forms.ModelForm):
       many_to_many = foreign_fields.TextAreaToManyField(to=Target, selector='name')
       
       class Meta:
            model = Referrer
+```
 
-Now you can use the form on your `View`. The default widget is ``Textarea``, so when you enter a text in the field and save the form, the ``TextAreaToManyField`` will split each line and search for a unique ``Target`` by line that has the given string in it's `name` field. If the field is not unique, it will be given a `ValidationError`.
+Now you can use the form on your `View`. The default widget is `Textarea`, so when you enter a text in the field and save the form, the `TextAreaToManyField` will split each line and search for a unique `Target` by line that has the given string in it's `name` field. If the field is not unique, it will be given a `ValidationError`.
```

### Comparing `django-foreign-fields-0.1/setup.py` & `django_foreign_fields-0.3.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import os
+import subprocess
 from setuptools import find_packages, setup
 
-with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
+def get_latest_tag():
+    ref = os.getenv("GITHUB_REF")
+    if ref:
+        return ref.split("/")[-1]
+    else:
+        return "0.0.0"  # Default version
+
+with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-foreign-fields',
-    version='0.1',
+    version=get_latest_tag(),
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A Django app with new form fields for handling foreign relationships.',
     long_description=README,
+    long_description_content_type='text/markdown',
     url='https://github.com/ThiagoCTN/django-foreign-fields/',
     author='Thiago Nascimento',
     author_email='thiagocampostn@gmail.com',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
@@ -26,12 +35,8 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
-    project_urls={
-    'Source': 'https://github.com/ThiagoCTN/django-foreign-fields/',
-    'Tracker': 'https://github.com/ThiagoCTN/django-foreign-fields/issues',
-},
 )
```


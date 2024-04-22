# Comparing `tmp/design.plone.ioprenoto-1.2.4.tar.gz` & `tmp/design.plone.ioprenoto-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.ioprenoto-1.2.4.tar", last modified: Thu Apr 11 11:01:18 2024, max compression
+gzip compressed data, was "design.plone.ioprenoto-1.2.5.tar", last modified: Mon Apr 22 07:26:32 2024, max compression
```

## Comparing `design.plone.ioprenoto-1.2.4.tar` & `design.plone.ioprenoto-1.2.5.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3755 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/CHANGES.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       58 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/CONTRIBUTORS.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1338 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/DEVELOP.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      662 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/LICENSE.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      136 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/MANIFEST.in
--rw-r--r--   0 mauro     (1000) mauro     (1000)    10313 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4724 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/README.rst
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.673067 design.plone.ioprenoto-1.2.4/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7986 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/docs/conf.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/docs/index.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2600 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.673067 design.plone.ioprenoto-1.2.4/src/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.673067 design.plone.ioprenoto-1.2.4/src/design/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.673067 design.plone.ioprenoto-1.2.4/src/design/plone/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      715 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/adapters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/adapters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1072 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/adapters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3523 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/adapters/stringinterp.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/behaviors/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/behaviors/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1655 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/behaviors/additional_fields.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      913 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/behaviors/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      589 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/behaviors/metadata.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/browser/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/browser/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      628 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/browser/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/browser/overrides/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/browser/overrides/.gitkeep
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/browser/static/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/browser/static/.gitkeep
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1603 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/events/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/events/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      481 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/events/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      136 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/events/on_create.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      284 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1520 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.673067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/en/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1395 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.673067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/it/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1395 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1754 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/update.py
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/update.sh
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/permissions.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.673067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/default/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/default/catalog.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/default/metadata.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/default/registry/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      180 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/default/registry/main.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/default/rolemap.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/default/types/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      373 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/default/types/Prenotazione.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/uninstall/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      280 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      230 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      414 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2439 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2679 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      693 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/vocabularies.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/bookable_list/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      520 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9160 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/booking_schema/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/booking_schema/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      425 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/booking_schema/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      949 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/booking_schema/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/bookings/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      698 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1821 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/bookings/search.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      242 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      794 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/setuphandlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2163 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/robot/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2019 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/robot/test_example.robot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1203 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2837 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_custom_booking_schema.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      866 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_custom_required_fields.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3167 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_prenotazione_add.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4501 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2735 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_servizio.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8101 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2432 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_setup.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4949 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_stringinterp.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3374 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_vocabularies.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/upgrades/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/upgrades/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      373 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/upgrades/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1553 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/upgrades/upgrades.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      483 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/utilities.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/vocabularies/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/vocabularies/__init__py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      252 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/vocabularies/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2207 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/vocabularies/tipologies.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 11:01:18.677067 design.plone.ioprenoto-1.2.4/src/design.plone.ioprenoto.egg-info/
--rw-r--r--   0 mauro     (1000) mauro     (1000)    10313 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design.plone.ioprenoto.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4714 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design.plone.ioprenoto.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design.plone.ioprenoto.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      127 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design.plone.ioprenoto.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       20 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design.plone.ioprenoto.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      297 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design.plone.ioprenoto.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2024-04-11 11:01:18.000000 design.plone.ioprenoto-1.2.4/src/design.plone.ioprenoto.egg-info/top_level.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.571574 design.plone.ioprenoto-1.2.5/
+-rw-r--r--   0 lucabel    (501) staff       (20)     3995 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/CHANGES.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       58 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/CONTRIBUTORS.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)     1338 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/DEVELOP.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)    18092 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/LICENSE.GPL
+-rw-r--r--   0 lucabel    (501) staff       (20)      662 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/LICENSE.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      136 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/MANIFEST.in
+-rw-r--r--   0 lucabel    (501) staff       (20)     9935 2024-04-22 07:26:32.571681 design.plone.ioprenoto-1.2.5/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)     4724 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/README.rst
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.552454 design.plone.ioprenoto-1.2.5/docs/
+-rw-r--r--   0 lucabel    (501) staff       (20)     7986 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/docs/conf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)       89 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/docs/index.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      340 2024-04-22 07:26:32.572130 design.plone.ioprenoto-1.2.5/setup.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2692 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/setup.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.545125 design.plone.ioprenoto-1.2.5/src/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.552692 design.plone.ioprenoto-1.2.5/src/design/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.555278 design.plone.ioprenoto-1.2.5/src/design/plone/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.556974 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/
+-rw-r--r--   0 lucabel    (501) staff       (20)      715 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.557659 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/adapters/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/adapters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1072 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/adapters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3523 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/adapters/stringinterp.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.558502 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/behaviors/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/behaviors/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1655 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/behaviors/additional_fields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      913 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/behaviors/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      589 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/behaviors/metadata.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.558901 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/browser/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/browser/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      628 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/browser/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.559121 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/browser/overrides/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/browser/overrides/.gitkeep
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.559300 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/browser/static/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/browser/static/.gitkeep
+-rw-r--r--   0 lucabel    (501) staff       (20)     1603 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.559908 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/events/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/events/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      481 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/events/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      136 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/events/on_create.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      284 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/interfaces.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.561013 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/
+-rw-r--r--   0 lucabel    (501) staff       (20)      611 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1520 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.546722 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/en/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.561233 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1395 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.546994 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/it/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.561463 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1395 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     1754 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/update.py
+-rwxr-xr-x   0 lucabel    (501) staff       (20)      503 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/update.sh
+-rw-r--r--   0 lucabel    (501) staff       (20)      273 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/permissions.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.547699 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.562349 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/default/
+-rw-r--r--   0 lucabel    (501) staff       (20)      191 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/default/catalog.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      191 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/default/metadata.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.562633 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/default/registry/
+-rw-r--r--   0 lucabel    (501) staff       (20)      180 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/default/registry/main.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      340 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/default/rolemap.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.563074 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/default/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)      373 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/default/types/Prenotazione.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      325 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.563303 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/uninstall/
+-rw-r--r--   0 lucabel    (501) staff       (20)      132 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.563702 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      280 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.564321 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      230 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.565320 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      414 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2439 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2679 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      693 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/vocabularies.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.565544 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.565994 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/bookable_list/
+-rw-r--r--   0 lucabel    (501) staff       (20)      520 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     9205 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.566708 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/booking_schema/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/booking_schema/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      425 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/booking_schema/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      949 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/booking_schema/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.567375 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/bookings/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      698 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1821 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/bookings/search.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      242 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      794 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/setuphandlers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2163 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/testing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.569837 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.570061 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/robot/
+-rw-r--r--   0 lucabel    (501) staff       (20)     2019 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/robot/test_example.robot
+-rw-r--r--   0 lucabel    (501) staff       (20)     1203 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2837 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_custom_booking_schema.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      866 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_custom_required_fields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3167 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_prenotazione_add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4501 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2735 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8101 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2432 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_setup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4949 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_stringinterp.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3374 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_vocabularies.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.570737 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/upgrades/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/upgrades/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      373 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/upgrades/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1553 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/upgrades/upgrades.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      483 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/utilities.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.571391 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/vocabularies/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/vocabularies/__init__py
+-rw-r--r--   0 lucabel    (501) staff       (20)      252 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/vocabularies/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2207 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/vocabularies/tipologies.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 07:26:32.555049 design.plone.ioprenoto-1.2.5/src/design.plone.ioprenoto.egg-info/
+-rw-r--r--   0 lucabel    (501) staff       (20)     9935 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design.plone.ioprenoto.egg-info/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)     4714 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design.plone.ioprenoto.egg-info/SOURCES.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design.plone.ioprenoto.egg-info/dependency_links.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      215 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design.plone.ioprenoto.egg-info/entry_points.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       20 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design.plone.ioprenoto.egg-info/not-zip-safe
+-rw-r--r--   0 lucabel    (501) staff       (20)      297 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design.plone.ioprenoto.egg-info/requires.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        7 2024-04-22 07:26:32.000000 design.plone.ioprenoto-1.2.5/src/design.plone.ioprenoto.egg-info/top_level.txt
```

### Comparing `design.plone.ioprenoto-1.2.4/CHANGES.rst` & `design.plone.ioprenoto-1.2.5/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+1.2.5 (2024-04-22)
+------------------
+
+- Refactor rest service to simplify inheritance
+  [lucabel]
+- Add redturtle.prenotazioni's notify_upcoming_bookings script to console_scripts (allows it to be available in the buildout).
+  [folix-01]
+
 1.2.4 (2024-04-11)
 ------------------
 
 - default b_size for booking types vocabulary serializer to 200
   [mamico]
```

### Comparing `design.plone.ioprenoto-1.2.4/DEVELOP.rst` & `design.plone.ioprenoto-1.2.5/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/LICENSE.GPL` & `design.plone.ioprenoto-1.2.5/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/LICENSE.rst` & `design.plone.ioprenoto-1.2.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/PKG-INFO` & `design.plone.ioprenoto-1.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.ioprenoto
-Version: 1.2.4
+Version: 1.2.5
 Summary: An add-on for Plone
 Home-page: https://github.com/RedTurtle/design.plone.ioprenoto
 Author: RedTurtle
 Author-email: info@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/design.plone.ioprenoto/
 Project-URL: Source, https://github.com/RedTurtle/design.plone.ioprenoto
@@ -19,31 +19,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
+Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
-Requires-Dist: setuptools
-Requires-Dist: z3c.jbot
-Requires-Dist: plone.api>=1.8.4
-Requires-Dist: plone.app.dexterity
-Requires-Dist: redturtle.prenotazioni>=2.2.0
-Requires-Dist: design.plone.policy
-Requires-Dist: plone.restapi>=9.6.0
-Provides-Extra: test
-Requires-Dist: plone.app.testing; extra == "test"
-Requires-Dist: plone.testing>=5.0.0; extra == "test"
-Requires-Dist: plone.app.contenttypes; extra == "test"
-Requires-Dist: plone.app.robotframework[debug]; extra == "test"
-Requires-Dist: collective.MockMailHost; extra == "test"
-Requires-Dist: redturtle.prenotazioni; extra == "test"
-Requires-Dist: design.plone.policy; extra == "test"
 
 
 .. image:: https://img.shields.io/pypi/v/design.plone.ioprenoto.svg
     :target: https://pypi.org/project/design.plone.ioprenoto/
     :alt: Latest Version
 
 .. image:: https://img.shields.io/pypi/pyversions/design.plone.ioprenoto.svg?style=plastic
@@ -217,14 +203,22 @@
 
 - RedTurtle, info@redturtle.it
 
 
 Changelog
 =========
 
+1.2.5 (2024-04-22)
+------------------
+
+- Refactor rest service to simplify inheritance
+  [lucabel]
+- Add redturtle.prenotazioni's notify_upcoming_bookings script to console_scripts (allows it to be available in the buildout).
+  [folix-01]
+
 1.2.4 (2024-04-11)
 ------------------
 
 - default b_size for booking types vocabulary serializer to 200
   [mamico]
```

### Comparing `design.plone.ioprenoto-1.2.4/README.rst` & `design.plone.ioprenoto-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/docs/conf.py` & `design.plone.ioprenoto-1.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/setup.py` & `design.plone.ioprenoto-1.2.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.ioprenoto",
-    version="1.2.4",
+    version="1.2.5",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
@@ -73,9 +73,10 @@
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     [console_scripts]
     update_locale = design.plone.ioprenoto.locales.update:update_locale
+    notify_upcoming_bookings = redturtle.prenotazioni.scripts.notify_upcoming_bookings:main
     """,
 )
```

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/__init__.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/adapters/configure.zcml` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/adapters/stringinterp.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/behaviors/additional_fields.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/behaviors/additional_fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/behaviors/configure.zcml` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/behaviors/metadata.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/behaviors/metadata.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/browser/configure.zcml` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/configure.zcml` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/README.rst` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/locales/update.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/serializers/vocabularies.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/serializers/vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from logging import getLogger
 from plone import api
 from plone.restapi.interfaces import ISerializeToJsonSummary
 from plone.restapi.serializer.converters import json_compatible
 from plone.restapi.services import Service
-from urllib.parse import urlencode
 from urllib.parse import unquote
+from urllib.parse import urlencode
 from zc.relation.interfaces import ICatalog
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.intid.interfaces import IIntIds
 
 import re
 
@@ -100,14 +100,17 @@
         if canale_fisico:
             return [x.to_object.UID() for x in canale_fisico if x.to_object]
         ufficio_responsabile = getattr(service, "ufficio_responsabile", [])
         return [x.to_object.UID() for x in ufficio_responsabile if x.to_object]
 
 
 class BookableUOList(BookableList):
+
+    UO_CONTENT_TYPE = "UnitaOrganizzativa"
+
     def booking_type_check(self, prenotazioni_folder, booking_type):
         if not booking_type:
             return True
         tocheck = [booking_type, unquote(booking_type)]
         # XXX: per qualche problema di doppio encoding arrivano dal frontend delle
         #      stringhe con caratteri in hex, questo codice serve a gestire quelle
         #      casistiche. Una volta fissato sul frontend può essere tolto.
@@ -131,15 +134,15 @@
         """
         Return all UO with at least one back-refence from PrenotazioniFolder
         """
         response = {
             "@id": f"{self.context.absolute_url()}/@bookable-uo-list",
             "items": [],
         }
-        query = dict(portal_type="UnitaOrganizzativa", sort_on="sortable_title")
+        query = dict(portal_type=self.UO_CONTENT_TYPE, sort_on="sortable_title")
         uid = self.request.form.get("uid", "")
         booking_type = self.request.form.get("booking_type", "")
         if uid:
             query["UID"] = self.get_uo_from_service_uid(uid=uid)
 
         uo_list = api.content.find(**query)
         intids = getUtility(IIntIds)
```

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/booking_schema/get.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/booking_schema/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/restapi/services/bookings/search.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/restapi/services/bookings/search.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/setuphandlers.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/testing.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/robot/test_example.robot` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_custom_booking_schema.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_custom_booking_schema.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_custom_required_fields.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_custom_required_fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_prenotazione_add.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_prenotazione_add.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_servizio.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_setup.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_stringinterp.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_stringinterp.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/tests/test_vocabularies.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/upgrades/upgrades.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design/plone/ioprenoto/vocabularies/tipologies.py` & `design.plone.ioprenoto-1.2.5/src/design/plone/ioprenoto/vocabularies/tipologies.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.2.4/src/design.plone.ioprenoto.egg-info/PKG-INFO` & `design.plone.ioprenoto-1.2.5/src/design.plone.ioprenoto.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.ioprenoto
-Version: 1.2.4
+Version: 1.2.5
 Summary: An add-on for Plone
 Home-page: https://github.com/RedTurtle/design.plone.ioprenoto
 Author: RedTurtle
 Author-email: info@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/design.plone.ioprenoto/
 Project-URL: Source, https://github.com/RedTurtle/design.plone.ioprenoto
@@ -19,31 +19,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
+Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
-Requires-Dist: setuptools
-Requires-Dist: z3c.jbot
-Requires-Dist: plone.api>=1.8.4
-Requires-Dist: plone.app.dexterity
-Requires-Dist: redturtle.prenotazioni>=2.2.0
-Requires-Dist: design.plone.policy
-Requires-Dist: plone.restapi>=9.6.0
-Provides-Extra: test
-Requires-Dist: plone.app.testing; extra == "test"
-Requires-Dist: plone.testing>=5.0.0; extra == "test"
-Requires-Dist: plone.app.contenttypes; extra == "test"
-Requires-Dist: plone.app.robotframework[debug]; extra == "test"
-Requires-Dist: collective.MockMailHost; extra == "test"
-Requires-Dist: redturtle.prenotazioni; extra == "test"
-Requires-Dist: design.plone.policy; extra == "test"
 
 
 .. image:: https://img.shields.io/pypi/v/design.plone.ioprenoto.svg
     :target: https://pypi.org/project/design.plone.ioprenoto/
     :alt: Latest Version
 
 .. image:: https://img.shields.io/pypi/pyversions/design.plone.ioprenoto.svg?style=plastic
@@ -217,14 +203,22 @@
 
 - RedTurtle, info@redturtle.it
 
 
 Changelog
 =========
 
+1.2.5 (2024-04-22)
+------------------
+
+- Refactor rest service to simplify inheritance
+  [lucabel]
+- Add redturtle.prenotazioni's notify_upcoming_bookings script to console_scripts (allows it to be available in the buildout).
+  [folix-01]
+
 1.2.4 (2024-04-11)
 ------------------
 
 - default b_size for booking types vocabulary serializer to 200
   [mamico]
```

### Comparing `design.plone.ioprenoto-1.2.4/src/design.plone.ioprenoto.egg-info/SOURCES.txt` & `design.plone.ioprenoto-1.2.5/src/design.plone.ioprenoto.egg-info/SOURCES.txt`

 * *Files identical despite different names*


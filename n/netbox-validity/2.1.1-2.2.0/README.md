# Comparing `tmp/netbox-validity-2.1.1.tar.gz` & `tmp/netbox_validity-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-validity-2.1.1.tar", last modified: Mon Apr  1 20:30:56 2024, max compression
+gzip compressed data, was "netbox_validity-2.2.0.tar", last modified: Sun Apr 21 22:23:58 2024, max compression
```

## Comparing `netbox-validity-2.1.1.tar` & `netbox_validity-2.2.0.tar`

### file list

```diff
@@ -1,191 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.749223 netbox-validity-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-01 20:30:56.749223 netbox-validity-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.745223 netbox-validity-2.1.1/netbox_validity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-01 20:30:56.000000 netbox-validity-2.1.1/netbox_validity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-01 20:30:56.000000 netbox-validity-2.1.1/netbox_validity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:30:56.000000 netbox-validity-2.1.1/netbox_validity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-01 20:30:56.000000 netbox-validity-2.1.1/netbox_validity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 20:30:56.000000 netbox-validity-2.1.1/netbox_validity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.721223 netbox-validity-2.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:30:56.749223 netbox-validity-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.725223 netbox-validity-2.1.1/validity/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.725223 netbox-validity-2.1.1/validity/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.725223 netbox-validity-2.1.1/validity/compliance/
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/dynamic_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.725223 netbox-validity-2.1.1/validity/compliance/eval/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/eval/default_nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/eval/eval_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.729223 netbox-validity-2.1.1/validity/compliance/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/routeros.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/textfsm.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/ttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/custom_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/data_backends.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.729223 netbox-validity-2.1.1/validity/fields/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/fields/encrypted.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.729223 netbox-validity-2.1.1/validity/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/forms/filterset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/forms/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/j2_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.729223 netbox-validity-2.1.1/validity/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0002_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0003_complianceselector_dp_tag_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0004_netbox35_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0005_rename_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0006_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0007_polling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0008_script_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0009_serializer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.733223 netbox-validity-2.1.1/validity/models/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/polling.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/netbox_changes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.733223 netbox-validity-2.1.1/validity/pollers/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/default_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/netconf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.733223 netbox-validity-2.1.1/validity/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.733223 netbox-validity-2.1.1/validity/scripts/install/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/scripts/install/validity_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/scripts/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/scripts/script_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/scripts/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.721223 netbox-validity-2.1.1/validity/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.737223 netbox-validity-2.1.1/validity/static/validity/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/static/validity/connection-type-select.js
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/static/validity/prism-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/static/validity/prism-light.css
--rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/static/validity/prism.js
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/subforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.721223 netbox-validity-2.1.1/validity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.737223 netbox-validity-2.1.1/validity/templates/validity/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/aux_tab_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/command.html
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/compliance_results.html
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/compliancereport.html
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/complianceselector.html
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/compliancetest.html
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/compliancetestresult.html
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/device_state.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.737223 netbox-validity-2.1.1/validity/templates/validity/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/configcontext_format.html
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/datasource_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/parameters.html
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/path_with_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/prism.html
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/report_stats_row.html
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/search_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/yaml_card.html
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/nameset.html
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/poller.html
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/poller_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/report_devices.html
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/serializer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.741223 netbox-validity-2.1.1/validity/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templatetags/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.741223 netbox-validity-2.1.1/validity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.741223 netbox-validity-2.1.1/validity/tests/test_compliance/
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_compliance/test_dynamic_pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_compliance/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_compliance/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_compliance/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_custom_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_data_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.741223 netbox-validity-2.1.1/validity/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_compliancetest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_git_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_vdatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_vdevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_pollers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.745223 netbox-validity-2.1.1/validity/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_scripts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_scripts/test_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_scripts/test_script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.745223 netbox-validity-2.1.1/validity/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_utils/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_utils/test_orm.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.745223 netbox-validity-2.1.1/validity/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/utils/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.745223 netbox-validity-2.1.1/validity/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.789053 netbox_validity-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-04-21 22:23:58.789053 netbox_validity-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.789053 netbox_validity-2.2.0/netbox_validity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-04-21 22:23:58.000000 netbox_validity-2.2.0/netbox_validity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-21 22:23:58.000000 netbox_validity-2.2.0/netbox_validity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:23:58.000000 netbox_validity-2.2.0/netbox_validity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-21 22:23:58.000000 netbox_validity-2.2.0/netbox_validity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 22:23:58.000000 netbox_validity-2.2.0/netbox_validity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.765053 netbox_validity-2.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:23:58.793053 netbox_validity-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.769053 netbox_validity-2.2.0/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.769053 netbox_validity-2.2.0/validity/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.769053 netbox_validity-2.2.0/validity/compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/dynamic_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.769053 netbox_validity-2.2.0/validity/compliance/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/eval/default_nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/eval/eval_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.773053 netbox_validity-2.2.0/validity/compliance/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/routeros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/textfsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/ttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/custom_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/data_backends.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.773053 netbox_validity-2.2.0/validity/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/fields/encrypted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.773053 netbox_validity-2.2.0/validity/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/forms/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/j2_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.773053 netbox_validity-2.2.0/validity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0002_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0003_complianceselector_dp_tag_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0004_netbox35_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0005_rename_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0006_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0007_polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0008_script_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0009_serializer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.777053 netbox_validity-2.2.0/validity/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/netbox_changes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.777053 netbox_validity-2.2.0/validity/pollers/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/default_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/netconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.777053 netbox_validity-2.2.0/validity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.777053 netbox_validity-2.2.0/validity/scripts/install/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/scripts/install/validity_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/scripts/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/scripts/script_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/scripts/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.761053 netbox_validity-2.2.0/validity/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.777053 netbox_validity-2.2.0/validity/static/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/static/validity/connection-type-select.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/static/validity/prism-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/static/validity/prism-light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/static/validity/prism.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/subforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.761053 netbox_validity-2.2.0/validity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.781053 netbox_validity-2.2.0/validity/templates/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/aux_tab_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/command.html
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/compliance_results.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/compliancereport.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/complianceselector.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/compliancetest.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/compliancetestresult.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/device_state.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.781053 netbox_validity-2.2.0/validity/templates/validity/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/configcontext_format.html
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/datasource_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/parameters.html
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/path_with_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/prism.html
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/related_objects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/report_stats_row.html
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/yaml_card.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/nameset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/poller.html
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/poller_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/report_devices.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/serializer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.781053 netbox_validity-2.2.0/validity/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templatetags/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/tests/test_compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_compliance/test_dynamic_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_compliance/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_compliance/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_compliance/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_custom_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_data_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_compliancetest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_git_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_vdatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_vdevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_pollers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_scripts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_scripts/test_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_scripts/test_script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_utils/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_utils/test_orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/utils/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.789053 netbox_validity-2.2.0/validity/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/test_result.py
```

### Comparing `netbox-validity-2.1.1/LICENSE` & `netbox_validity-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/PKG-INFO` & `netbox_validity-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 2.1.1
+Version: 2.2.0
 Summary: NetBox plugin for network devices validation
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,22 +47,23 @@
 Requires-Dist: deepdiff<7,>=6.2.0
 Requires-Dist: django-bootstrap-v5==1.0.*
 Requires-Dist: dulwich
 Requires-Dist: jq<2,>=1.4.0
 Requires-Dist: netmiko<5,>=4.0.0
 Requires-Dist: pydantic<3,>=2.0.0
 Requires-Dist: scrapli_netconf==2024.1.30
-Requires-Dist: simpleeval==0.9.*
+Requires-Dist: simpleeval==0.9.13
 Requires-Dist: textfsm<2,>=1.1.3
 Requires-Dist: ttp==0.9.*
 Requires-Dist: xmltodict<1
 Provides-Extra: dev
 Requires-Dist: debugpy==1.8.1; extra == "dev"
 Requires-Dist: factory_boy==3.3.0; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; extra == "dev"
 Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: pytest-django==4.8.0; extra == "dev"
 Requires-Dist: pytest-subtests==0.12.1; extra == "dev"
 Requires-Dist: ruff==0.3.4; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Provides-Extra: docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 2.1.1 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-validity Version: 2.2.0 Summary: NetBox
 plugin for network devices validation Author-email: Anton Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -25,24 +25,24 @@
 MIT License Classifier: Operating System :: Unix Classifier: Operating System
 :: POSIX :: Linux Classifier: Framework :: Django Classifier: Topic :: System
 :: Networking Classifier: Topic :: Internet Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 deepdiff<7,>=6.2.0 Requires-Dist: django-bootstrap-v5==1.0.* Requires-Dist:
 dulwich Requires-Dist: jq<2,>=1.4.0 Requires-Dist: netmiko<5,>=4.0.0 Requires-
 Dist: pydantic<3,>=2.0.0 Requires-Dist: scrapli_netconf==2024.1.30 Requires-
-Dist: simpleeval==0.9.* Requires-Dist: textfsm<2,>=1.1.3 Requires-Dist:
+Dist: simpleeval==0.9.13 Requires-Dist: textfsm<2,>=1.1.3 Requires-Dist:
 ttp==0.9.* Requires-Dist: xmltodict<1 Provides-Extra: dev Requires-Dist:
 debugpy==1.8.1; extra == "dev" Requires-Dist: factory_boy==3.3.0; extra ==
-"dev" Requires-Dist: ipython; extra == "dev" Requires-Dist: pytest==8.1.1;
-extra == "dev" Requires-Dist: pytest-cov==5.0.0; extra == "dev" Requires-Dist:
-pytest-django==4.8.0; extra == "dev" Requires-Dist: pytest-subtests==0.12.1;
-extra == "dev" Requires-Dist: ruff==0.3.4; extra == "dev" Requires-Dist:
-tomli==2.0.1; extra == "dev" Provides-Extra: docs Requires-Dist: mkdocs==1.4.2;
-extra == "docs" Requires-Dist: mkdocs-include-markdown-plugin==4.0.4; extra ==
-"docs"
+"dev" Requires-Dist: ipython; extra == "dev" Requires-Dist: pre-commit==3.7.0;
+extra == "dev" Requires-Dist: pytest==8.1.1; extra == "dev" Requires-Dist:
+pytest-cov==5.0.0; extra == "dev" Requires-Dist: pytest-django==4.8.0; extra ==
+"dev" Requires-Dist: pytest-subtests==0.12.1; extra == "dev" Requires-Dist:
+ruff==0.3.4; extra == "dev" Requires-Dist: tomli==2.0.1; extra == "dev"
+Provides-Extra: docs Requires-Dist: mkdocs==1.4.2; extra == "docs" Requires-
+Dist: mkdocs-include-markdown-plugin==4.0.4; extra == "docs"
                          _[_C_l_i_c_k_ _t_o_ _v_i_e_w_ _V_a_l_i_d_i_t_y_ _d_o_c_s_]
        ************ VVaalliiddiittyy:: vveennddoorr--aaggnnoossttiicc ccoonnffiigguurraattiioonn ccoommpplliiaannccee ************
                 [CI][Coverage][Python version][NetBox version]
 ## What? Validity is the [NetBox](https://netbox.dev) plugin to write "auto
 tests" for your network devices. You define compliance tests and Validity
 checks device state or configuration against these tests. The two most obvious
 use cases for such a functionality include: * **Configuration compliance**. You
```

### Comparing `netbox-validity-2.1.1/README.md` & `netbox_validity-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/netbox_validity.egg-info/PKG-INFO` & `netbox_validity-2.2.0/netbox_validity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 2.1.1
+Version: 2.2.0
 Summary: NetBox plugin for network devices validation
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,22 +47,23 @@
 Requires-Dist: deepdiff<7,>=6.2.0
 Requires-Dist: django-bootstrap-v5==1.0.*
 Requires-Dist: dulwich
 Requires-Dist: jq<2,>=1.4.0
 Requires-Dist: netmiko<5,>=4.0.0
 Requires-Dist: pydantic<3,>=2.0.0
 Requires-Dist: scrapli_netconf==2024.1.30
-Requires-Dist: simpleeval==0.9.*
+Requires-Dist: simpleeval==0.9.13
 Requires-Dist: textfsm<2,>=1.1.3
 Requires-Dist: ttp==0.9.*
 Requires-Dist: xmltodict<1
 Provides-Extra: dev
 Requires-Dist: debugpy==1.8.1; extra == "dev"
 Requires-Dist: factory_boy==3.3.0; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; extra == "dev"
 Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: pytest-django==4.8.0; extra == "dev"
 Requires-Dist: pytest-subtests==0.12.1; extra == "dev"
 Requires-Dist: ruff==0.3.4; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Provides-Extra: docs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 2.1.1 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-validity Version: 2.2.0 Summary: NetBox
 plugin for network devices validation Author-email: Anton Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -25,24 +25,24 @@
 MIT License Classifier: Operating System :: Unix Classifier: Operating System
 :: POSIX :: Linux Classifier: Framework :: Django Classifier: Topic :: System
 :: Networking Classifier: Topic :: Internet Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 deepdiff<7,>=6.2.0 Requires-Dist: django-bootstrap-v5==1.0.* Requires-Dist:
 dulwich Requires-Dist: jq<2,>=1.4.0 Requires-Dist: netmiko<5,>=4.0.0 Requires-
 Dist: pydantic<3,>=2.0.0 Requires-Dist: scrapli_netconf==2024.1.30 Requires-
-Dist: simpleeval==0.9.* Requires-Dist: textfsm<2,>=1.1.3 Requires-Dist:
+Dist: simpleeval==0.9.13 Requires-Dist: textfsm<2,>=1.1.3 Requires-Dist:
 ttp==0.9.* Requires-Dist: xmltodict<1 Provides-Extra: dev Requires-Dist:
 debugpy==1.8.1; extra == "dev" Requires-Dist: factory_boy==3.3.0; extra ==
-"dev" Requires-Dist: ipython; extra == "dev" Requires-Dist: pytest==8.1.1;
-extra == "dev" Requires-Dist: pytest-cov==5.0.0; extra == "dev" Requires-Dist:
-pytest-django==4.8.0; extra == "dev" Requires-Dist: pytest-subtests==0.12.1;
-extra == "dev" Requires-Dist: ruff==0.3.4; extra == "dev" Requires-Dist:
-tomli==2.0.1; extra == "dev" Provides-Extra: docs Requires-Dist: mkdocs==1.4.2;
-extra == "docs" Requires-Dist: mkdocs-include-markdown-plugin==4.0.4; extra ==
-"docs"
+"dev" Requires-Dist: ipython; extra == "dev" Requires-Dist: pre-commit==3.7.0;
+extra == "dev" Requires-Dist: pytest==8.1.1; extra == "dev" Requires-Dist:
+pytest-cov==5.0.0; extra == "dev" Requires-Dist: pytest-django==4.8.0; extra ==
+"dev" Requires-Dist: pytest-subtests==0.12.1; extra == "dev" Requires-Dist:
+ruff==0.3.4; extra == "dev" Requires-Dist: tomli==2.0.1; extra == "dev"
+Provides-Extra: docs Requires-Dist: mkdocs==1.4.2; extra == "docs" Requires-
+Dist: mkdocs-include-markdown-plugin==4.0.4; extra == "docs"
                          _[_C_l_i_c_k_ _t_o_ _v_i_e_w_ _V_a_l_i_d_i_t_y_ _d_o_c_s_]
        ************ VVaalliiddiittyy:: vveennddoorr--aaggnnoossttiicc ccoonnffiigguurraattiioonn ccoommpplliiaannccee ************
                 [CI][Coverage][Python version][NetBox version]
 ## What? Validity is the [NetBox](https://netbox.dev) plugin to write "auto
 tests" for your network devices. You define compliance tests and Validity
 checks device state or configuration against these tests. The two most obvious
 use cases for such a functionality include: * **Configuration compliance**. You
```

### Comparing `netbox-validity-2.1.1/netbox_validity.egg-info/SOURCES.txt` & `netbox_validity-2.2.0/netbox_validity.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 validity/templates/validity/report_devices.html
 validity/templates/validity/serializer.html
 validity/templates/validity/inc/configcontext_format.html
 validity/templates/validity/inc/datasource_link.html
 validity/templates/validity/inc/parameters.html
 validity/templates/validity/inc/path_with_link.html
 validity/templates/validity/inc/prism.html
+validity/templates/validity/inc/related_objects.html
 validity/templates/validity/inc/report_stats_row.html
 validity/templates/validity/inc/search_form.html
 validity/templates/validity/inc/yaml_card.html
 validity/templatetags/__init__.py
 validity/templatetags/validity.py
 validity/tests/base.py
 validity/tests/conftest.py
@@ -147,14 +148,15 @@
 validity/utils/json.py
 validity/utils/misc.py
 validity/utils/orm.py
 validity/utils/version.py
 validity/views/__init__.py
 validity/views/base.py
 validity/views/command.py
+validity/views/data_source.py
 validity/views/device.py
 validity/views/nameset.py
 validity/views/poller.py
 validity/views/report.py
 validity/views/selector.py
 validity/views/serializer.py
 validity/views/test.py
```

### Comparing `netbox-validity-2.1.1/pyproject.toml` & `netbox_validity-2.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-validity"
-version = "2.1.1"
+version = "2.2.0"
 description = "NetBox plugin for network devices validation"
 authors = [
     {name = "Anton Miasnikov", email = "anton2008m@gmail.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `netbox-validity-2.1.1/validity/__init__.py` & `netbox_validity-2.2.0/validity/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class NetBoxValidityConfig(PluginConfig):
     name = "validity"
     verbose_name = "Validity"
     description = "Write and run auto tests for network devices"
     author = "Anton Miasnikov"
     author_email = "anton2008m@gmail.com"
-    version = "2.1.1"
+    version = "2.2.0"
     base_url = "validity"
     django_apps = ["bootstrap5"]
     min_version = "3.5.0"
 
     # custom field
     netbox_version = NetboxVersion(VERSION)
```

### Comparing `netbox-validity-2.1.1/validity/api/helpers.py` & `netbox_validity-2.2.0/validity/api/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/api/serializers.py` & `netbox_validity-2.2.0/validity/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/api/urls.py` & `netbox_validity-2.2.0/validity/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/api/views.py` & `netbox_validity-2.2.0/validity/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/choices.py` & `netbox_validity-2.2.0/validity/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/compliance/dynamic_pairs.py` & `netbox_validity-2.2.0/validity/compliance/dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/compliance/eval/default_nameset.py` & `netbox_validity-2.2.0/validity/compliance/eval/default_nameset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from builtins import *  # noqa
 
 from validity.models import VDevice
+from validity.utils.orm import model_to_proxy
 from validity.utils.json import jq  # noqa
 
 
 builtins = [
     "abs",
     "all",
     "any",
@@ -53,16 +54,15 @@
 
 __all__ = ["jq", "config", "state"] + builtins
 
 
 def state(device):
     # state() implies presence of "_data_source" and "_poller" global variables
     # which are gonna be set by RunTests script
-    vdevice = VDevice()
-    vdevice.__dict__ = device.__dict__.copy()
+    vdevice = model_to_proxy(device, VDevice)
     vdevice.data_source = _data_source  # noqa
     vdevice._poller = _poller  # noqa
     return vdevice.state
 
 
 def config(device):
     return state(device).config
```

### Comparing `netbox-validity-2.1.1/validity/compliance/eval/eval.py` & `netbox_validity-2.2.0/validity/compliance/eval/eval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 import ast
 import re
 from typing import Literal
 
 import deepdiff
-from simpleeval import EvalWithCompoundTypes
+import simpleeval
 
 from validity.utils.misc import reraise
 from ..exceptions import EvalError
 from . import default_nameset, eval_defaults
 
 
+class DictCompWithElt(ast.DictComp):
+    @property
+    def elt(self):
+        return ast.Tuple(elts=[self.key, self.value])
+
+
+class EvalWithCompoundTypes(simpleeval.EvalWithCompoundTypes):
+    """
+    This class provides support for DictComp and SetComp
+    """
+
+    def __init__(self, operators=None, functions=None, names=None):
+        super().__init__(operators, functions, names)
+        self.nodes |= {ast.DictComp: self._eval_dictcomp, ast.SetComp: lambda node: set(self._eval_comprehension(node))}
+
+    def _eval_dictcomp(self, node):
+        node = DictCompWithElt(**node.__dict__)
+        return dict(self._eval_comprehension(node))
+
+
 class ExplanationalEval(EvalWithCompoundTypes):
     do_not_explain = (ast.Constant, ast.Name, ast.Attribute, ast.Expr)
 
     def __init__(
         self,
         operators=None,
         functions=None,
```

### Comparing `netbox-validity-2.1.1/validity/compliance/eval/eval_defaults.py` & `netbox_validity-2.2.0/validity/compliance/eval/eval_defaults.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/compliance/exceptions.py` & `netbox_validity-2.2.0/validity/compliance/exceptions.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/compliance/serialization/backend.py` & `netbox_validity-2.2.0/validity/compliance/serialization/backend.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/compliance/serialization/routeros.py` & `netbox_validity-2.2.0/validity/compliance/serialization/routeros.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/compliance/serialization/serializable.py` & `netbox_validity-2.2.0/validity/compliance/serialization/serializable.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/compliance/serialization/xml.py` & `netbox_validity-2.2.0/validity/compliance/serialization/xml.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/compliance/state.py` & `netbox_validity-2.2.0/validity/compliance/state.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/custom_validators.py` & `netbox_validity-2.2.0/validity/custom_validators.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/data_backends.py` & `netbox_validity-2.2.0/validity/data_backends.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/fields/encrypted.py` & `netbox_validity-2.2.0/validity/fields/encrypted.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/filtersets.py` & `netbox_validity-2.2.0/validity/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/forms/filterset.py` & `netbox_validity-2.2.0/validity/forms/filterset.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,19 @@
         required=False, placeholder=_("Compliance Passed"), choices=BOOLEAN_WITH_BLANK_CHOICES[1:]
     )
     severity_ge = PlaceholderChoiceField(
         required=False, placeholder=_("Minimum Severity"), choices=SeverityChoices.choices[1:]
     )
 
 
+class DataSourceDevicesFilterForm(Form):
+    q = CharField(label=_("Device Search"), required=False)
+    tenant_id = DynamicModelMultipleChoiceField(label=_("Tenant"), queryset=Tenant.objects.all(), required=False)
+
+
 class TestResultFilterForm(ExcludeMixin, Form):
     latest = PlaceholderChoiceField(required=False, placeholder=_("Latest"), choices=BOOLEAN_WITH_BLANK_CHOICES[1:])
     passed = PlaceholderChoiceField(
         required=False,
         placeholder=_("Passed"),
         choices=BOOLEAN_WITH_BLANK_CHOICES[1:],
     )
```

### Comparing `netbox-validity-2.1.1/validity/forms/general.py` & `netbox_validity-2.2.0/validity/forms/general.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/forms/helpers.py` & `netbox_validity-2.2.0/validity/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/graphql.py` & `netbox_validity-2.2.0/validity/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/managers.py` & `netbox_validity-2.2.0/validity/managers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/migrations/0001_initial.py` & `netbox_validity-2.2.0/validity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/migrations/0002_custom_fields.py` & `netbox_validity-2.2.0/validity/migrations/0002_custom_fields.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/migrations/0005_rename_serializer.py` & `netbox_validity-2.2.0/validity/migrations/0005_rename_serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/migrations/0006_datasources.py` & `netbox_validity-2.2.0/validity/migrations/0006_datasources.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/migrations/0007_polling.py` & `netbox_validity-2.2.0/validity/migrations/0007_polling.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/migrations/0008_script_change.py` & `netbox_validity-2.2.0/validity/migrations/0008_script_change.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/models/base.py` & `netbox_validity-2.2.0/validity/models/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/models/data.py` & `netbox_validity-2.2.0/validity/models/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 class VDataSource(DataSource):
     objects = VDataSourceQS.as_manager()
 
     class Meta:
         proxy = True
 
     @property
+    def bound_devices(self):
+        from validity.models.device import VDevice
+
+        return VDevice.objects.annotate_datasource_id().filter(data_source_id=self.pk)
+
+    @property
     def is_default(self):
         return self.cf.get("default", False)
 
     @property
     def web_url(self) -> str:
         template_text = self.cf.get("web_url") or ""
         template = Environment().from_string(template_text)
```

### Comparing `netbox-validity-2.1.1/validity/models/device.py` & `netbox_validity-2.2.0/validity/models/device.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/models/nameset.py` & `netbox_validity-2.2.0/validity/models/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/models/polling.py` & `netbox_validity-2.2.0/validity/models/polling.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/models/report.py` & `netbox_validity-2.2.0/validity/models/report.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/models/selector.py` & `netbox_validity-2.2.0/validity/models/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/models/serializer.py` & `netbox_validity-2.2.0/validity/models/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/models/test.py` & `netbox_validity-2.2.0/validity/models/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/models/test_result.py` & `netbox_validity-2.2.0/validity/models/test_result.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/navigation.py` & `netbox_validity-2.2.0/validity/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/netbox_changes.py` & `netbox_validity-2.2.0/validity/netbox_changes.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/pollers/base.py` & `netbox_validity-2.2.0/validity/pollers/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/pollers/default_credentials.py` & `netbox_validity-2.2.0/validity/pollers/default_credentials.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/pollers/factory.py` & `netbox_validity-2.2.0/validity/pollers/factory.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/pollers/http.py` & `netbox_validity-2.2.0/validity/pollers/http.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/pollers/result.py` & `netbox_validity-2.2.0/validity/pollers/result.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/scripts/run_tests.py` & `netbox_validity-2.2.0/validity/scripts/run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/scripts/script_data.py` & `netbox_validity-2.2.0/validity/scripts/script_data.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/search.py` & `netbox_validity-2.2.0/validity/search.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/static/validity/connection-type-select.js` & `netbox_validity-2.2.0/validity/static/validity/connection-type-select.js`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/static/validity/prism-dark.css` & `netbox_validity-2.2.0/validity/static/validity/prism-dark.css`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/static/validity/prism-light.css` & `netbox_validity-2.2.0/validity/static/validity/prism-light.css`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/static/validity/prism.js` & `netbox_validity-2.2.0/validity/static/validity/prism.js`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/subforms.py` & `netbox_validity-2.2.0/validity/subforms.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tables.py` & `netbox_validity-2.2.0/validity/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/template_content.py` & `netbox_validity-2.2.0/validity/template_content.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import yaml
 from django.utils.translation import gettext_lazy as _
 from extras.plugins import PluginTemplateExtension
+from tenancy.models import Tenant
 
 from validity.pollers.result import PollingInfo
 
 
-class DataSourceExtension(PluginTemplateExtension):
+class PollingInfoExtension(PluginTemplateExtension):
     model = "core.datasource"
 
     def get_polling_info(self, data_file) -> str:
         if not data_file:
             return _("No polling info yet.")
         polling_info = PollingInfo.model_validate(yaml.safe_load(data_file.data_as_string))
         return yaml.safe_dump(polling_info.model_dump(exclude={"errors"}))
@@ -25,8 +26,25 @@
                 "content": text,
                 "title_link": polling_info_file.get_absolute_url() if polling_info_file else "",
                 "title": _("Polling info"),
             },
         )
 
 
-template_extensions = [DataSourceExtension]
+class DataSourceTenantExtension(PluginTemplateExtension):
+    model = "core.datasource"
+
+    def right_page(self):
+        instance = self.context["object"]
+        tenant_qs = Tenant.objects.restrict(self.context["request"].user, "view").filter(
+            custom_field_data__data_source=instance.pk
+        )
+        if not (qs_count := tenant_qs.count()):
+            return ""
+        related_models = [(qs_count, tenant_qs.model, "cf_data_source")]
+        return self.render(
+            "validity/inc/related_objects.html",
+            extra_context={"related_models": related_models},
+        )
+
+
+template_extensions = [DataSourceTenantExtension, PollingInfoExtension]
```

### Comparing `netbox-validity-2.1.1/validity/templates/validity/aux_tab_table.html` & `netbox_validity-2.2.0/validity/templates/validity/aux_tab_table.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/templates/validity/command.html` & `netbox_validity-2.2.0/validity/templates/validity/command.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/templates/validity/compliancereport.html` & `netbox_validity-2.2.0/validity/templates/validity/compliancereport.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/templates/validity/complianceselector.html` & `netbox_validity-2.2.0/validity/templates/validity/complianceselector.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/templates/validity/compliancetest.html` & `netbox_validity-2.2.0/validity/templates/validity/compliancetest.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/templates/validity/compliancetestresult.html` & `netbox_validity-2.2.0/validity/templates/validity/compliancetestresult.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/templates/validity/device_state.html` & `netbox_validity-2.2.0/validity/templates/validity/device_state.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/templates/validity/inc/parameters.html` & `netbox_validity-2.2.0/validity/templates/validity/inc/parameters.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/templates/validity/nameset.html` & `netbox_validity-2.2.0/validity/templates/validity/nameset.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/templates/validity/poller.html` & `netbox_validity-2.2.0/validity/templates/validity/poller.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/templates/validity/serializer.html` & `netbox_validity-2.2.0/validity/templates/validity/serializer.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/templatetags/validity.py` & `netbox_validity-2.2.0/validity/templatetags/validity.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/base.py` & `netbox_validity-2.2.0/validity/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/conftest.py` & `netbox_validity-2.2.0/validity/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/factories.py` & `netbox_validity-2.2.0/validity/tests/factories.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_api.py` & `netbox_validity-2.2.0/validity/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_choices.py` & `netbox_validity-2.2.0/validity/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_compliance/test_dynamic_pairs.py` & `netbox_validity-2.2.0/validity/tests/test_compliance/test_dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_compliance/test_serialization.py` & `netbox_validity-2.2.0/validity/tests/test_compliance/test_serialization.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_compliance/test_state.py` & `netbox_validity-2.2.0/validity/tests/test_compliance/test_state.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_custom_validators.py` & `netbox_validity-2.2.0/validity/tests/test_custom_validators.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_data_backends.py` & `netbox_validity-2.2.0/validity/tests/test_data_backends.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_fields.py` & `netbox_validity-2.2.0/validity/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_graphql.py` & `netbox_validity-2.2.0/validity/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_managers.py` & `netbox_validity-2.2.0/validity/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_models/test_clean.py` & `netbox_validity-2.2.0/validity/tests/test_models/test_clean.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_models/test_compliancetest.py` & `netbox_validity-2.2.0/validity/tests/test_models/test_compliancetest.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_models/test_git_link.py` & `netbox_validity-2.2.0/validity/tests/test_models/test_git_link.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_models/test_selector.py` & `netbox_validity-2.2.0/validity/tests/test_models/test_selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_models/test_vdatasource.py` & `netbox_validity-2.2.0/validity/tests/test_models/test_vdatasource.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_models/test_vdevice.py` & `netbox_validity-2.2.0/validity/tests/test_models/test_vdevice.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_pollers.py` & `netbox_validity-2.2.0/validity/tests/test_pollers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_scripts/test_run_tests.py` & `netbox_validity-2.2.0/validity/tests/test_scripts/test_run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_scripts/test_script_data.py` & `netbox_validity-2.2.0/validity/tests/test_scripts/test_script_data.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_utils/test_json.py` & `netbox_validity-2.2.0/validity/tests/test_utils/test_json.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_utils/test_misc.py` & `netbox_validity-2.2.0/validity/tests/test_utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_utils/test_orm.py` & `netbox_validity-2.2.0/validity/tests/test_utils/test_orm.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/tests/test_views.py` & `netbox_validity-2.2.0/validity/tests/test_views.py`

 * *Files 12% similar despite different names*

```diff
@@ -181,7 +181,16 @@
     model_class = models.Command
     post_body = {
         "name": "command-1",
         "label": "command_1",
         "type": "CLI",
         "cli_command": "show run",
     }
+
+
+@pytest.mark.django_db
+def test_datasource_devices(admin_client):
+    data_source = DataSourceFactory(custom_field_data={"default": True})
+    DeviceFactory()
+    DeviceFactory()
+    resp = admin_client.get(data_source.get_absolute_url() + "devices/")
+    assert resp.status_code == HTTPStatus.OK
```

### Comparing `netbox-validity-2.1.1/validity/urls.py` & `netbox_validity-2.2.0/validity/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/utils/json.py` & `netbox_validity-2.2.0/validity/utils/json.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/utils/misc.py` & `netbox_validity-2.2.0/validity/utils/misc.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/utils/orm.py` & `netbox_validity-2.2.0/validity/utils/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,7 +181,16 @@
         for item in self._result_cache:
             if isinstance(item, self.model):
                 self.bind_attributes(item)
 
     def set_attribute(self, name, value):
         self._aux_attributes[name] = value
         return self
+
+
+def model_to_proxy(model: Model, proxy_type: type[M]) -> M:
+    """
+    Converts model to its proxy type (e.g. Device to VDevice)
+    """
+    new_model = proxy_type()
+    new_model.__dict__ = model.__dict__.copy()
+    return new_model
```

### Comparing `netbox-validity-2.1.1/validity/utils/version.py` & `netbox_validity-2.2.0/validity/utils/version.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/views/__init__.py` & `netbox_validity-2.2.0/validity/views/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .command import CommandBulkDeleteView, CommandDeleteView, CommandEditView, CommandListView, CommandView
+from .data_source import DataSourceBoundDevicesView
 from .device import DeviceSerializedStateView, TestResultView
 from .nameset import NameSetBulkDeleteView, NameSetDeleteView, NameSetEditView, NameSetListView, NameSetView
 from .poller import PollerBulkDeleteView, PollerDeleteView, PollerEditView, PollerListView, PollerView
 from .report import ComplianceReportListView, ComplianceReportView
 from .selector import (
     ComplianceSelectorBulkDeleteView,
     ComplianceSelectorDeleteView,
```

### Comparing `netbox-validity-2.1.1/validity/views/base.py` & `netbox_validity-2.2.0/validity/views/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/views/command.py` & `netbox_validity-2.2.0/validity/views/command.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/views/device.py` & `netbox_validity-2.2.0/validity/views/device.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/views/nameset.py` & `netbox_validity-2.2.0/validity/views/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/views/poller.py` & `netbox_validity-2.2.0/validity/views/poller.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/views/report.py` & `netbox_validity-2.2.0/validity/views/report.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/views/selector.py` & `netbox_validity-2.2.0/validity/views/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/views/serializer.py` & `netbox_validity-2.2.0/validity/views/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/views/test.py` & `netbox_validity-2.2.0/validity/views/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.1/validity/views/test_result.py` & `netbox_validity-2.2.0/validity/views/test_result.py`

 * *Files identical despite different names*


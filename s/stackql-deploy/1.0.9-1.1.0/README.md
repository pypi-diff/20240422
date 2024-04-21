# Comparing `tmp/stackql_deploy-1.0.9.tar.gz` & `tmp/stackql_deploy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackql_deploy-1.0.9.tar", last modified: Wed Apr 17 01:12:59 2024, max compression
+gzip compressed data, was "stackql_deploy-1.1.0.tar", last modified: Sun Apr 21 22:34:21 2024, max compression
```

## Comparing `stackql_deploy-1.0.9.tar` & `stackql_deploy-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,35 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 01:12:59.084573 stackql_deploy-1.0.9/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.9/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-17 01:12:59.054865 stackql_deploy-1.0.9/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8214 2024-04-16 23:03:24.000000 stackql_deploy-1.0.9/README.rst
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-17 01:12:59.087598 stackql_deploy-1.0.9/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-17 00:53:56.000000 stackql_deploy-1.0.9/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 01:12:56.725468 stackql_deploy-1.0.9/stackql_deploy/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-17 00:53:56.000000 stackql_deploy-1.0.9/stackql_deploy/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5607 2024-04-17 01:12:14.000000 stackql_deploy-1.0.9/stackql_deploy/cli.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 01:12:58.404766 stackql_deploy-1.0.9/stackql_deploy/cmd/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.9/stackql_deploy/cmd/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6291 2024-04-16 23:16:19.000000 stackql_deploy-1.0.9/stackql_deploy/cmd/build.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3433 2024-04-16 23:17:44.000000 stackql_deploy-1.0.9/stackql_deploy/cmd/teardown.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2542 2024-04-16 23:17:44.000000 stackql_deploy-1.0.9/stackql_deploy/cmd/test.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 01:12:58.906858 stackql_deploy-1.0.9/stackql_deploy/lib/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.9/stackql_deploy/lib/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)      333 2024-04-12 03:18:07.000000 stackql_deploy-1.0.9/stackql_deploy/lib/bootstrap.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3647 2024-04-16 02:40:32.000000 stackql_deploy-1.0.9/stackql_deploy/lib/config.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2782 2024-04-16 03:47:18.000000 stackql_deploy-1.0.9/stackql_deploy/lib/templating.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5279 2024-04-16 03:46:51.000000 stackql_deploy-1.0.9/stackql_deploy/lib/utils.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 01:12:59.006557 stackql_deploy-1.0.9/stackql_deploy.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-17 01:12:55.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      576 2024-04-17 01:12:56.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-17 01:12:55.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-17 01:12:55.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/entry_points.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-17 01:12:55.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-17 01:12:55.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/top_level.txt
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-21 22:34:21.234125 stackql_deploy-1.1.0/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.1.0/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    10269 2024-04-21 22:34:21.215709 stackql_deploy-1.1.0/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8359 2024-04-17 09:11:17.000000 stackql_deploy-1.1.0/README.rst
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-21 22:34:21.236202 stackql_deploy-1.1.0/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1657 2024-04-20 03:13:09.000000 stackql_deploy-1.1.0/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-21 22:34:20.203805 stackql_deploy-1.1.0/stackql_deploy/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-20 03:13:09.000000 stackql_deploy-1.1.0/stackql_deploy/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     7906 2024-04-21 21:33:46.000000 stackql_deploy-1.1.0/stackql_deploy/cli.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-21 22:34:20.591357 stackql_deploy-1.1.0/stackql_deploy/cmd/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.1.0/stackql_deploy/cmd/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6258 2024-04-17 22:13:04.000000 stackql_deploy-1.1.0/stackql_deploy/cmd/build.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3433 2024-04-16 23:17:44.000000 stackql_deploy-1.1.0/stackql_deploy/cmd/teardown.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2542 2024-04-16 23:17:44.000000 stackql_deploy-1.1.0/stackql_deploy/cmd/test.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-21 22:34:20.856413 stackql_deploy-1.1.0/stackql_deploy/lib/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.1.0/stackql_deploy/lib/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      192 2024-04-20 03:11:50.000000 stackql_deploy-1.1.0/stackql_deploy/lib/bootstrap.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3498 2024-04-17 22:13:04.000000 stackql_deploy-1.1.0/stackql_deploy/lib/config.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2821 2024-04-17 22:13:04.000000 stackql_deploy-1.1.0/stackql_deploy/lib/templating.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5446 2024-04-17 22:58:56.000000 stackql_deploy-1.1.0/stackql_deploy/lib/utils.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-21 22:34:20.909144 stackql_deploy-1.1.0/stackql_deploy/templates/
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-21 22:34:20.967898 stackql_deploy-1.1.0/stackql_deploy/templates/stackql_docs/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       62 2024-04-17 05:34:52.000000 stackql_deploy-1.1.0/stackql_deploy/templates/stackql_docs/stackql_example_rg.md.template
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      712 2024-04-17 05:34:52.000000 stackql_deploy-1.1.0/stackql_deploy/templates/stackql_manifest.yml.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-21 22:34:21.059492 stackql_deploy-1.1.0/stackql_deploy/templates/stackql_resources/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      892 2024-04-17 05:34:52.000000 stackql_deploy-1.1.0/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-21 22:34:21.129281 stackql_deploy-1.1.0/stackql_deploy/templates/stackql_tests/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      726 2024-04-17 05:34:52.000000 stackql_deploy-1.1.0/stackql_deploy/templates/stackql_tests/stackql_example_rg.iql.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-21 22:34:21.191768 stackql_deploy-1.1.0/stackql_deploy.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    10269 2024-04-21 22:34:19.000000 stackql_deploy-1.1.0/stackql_deploy.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      846 2024-04-21 22:34:19.000000 stackql_deploy-1.1.0/stackql_deploy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-21 22:34:19.000000 stackql_deploy-1.1.0/stackql_deploy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-21 22:34:19.000000 stackql_deploy-1.1.0/stackql_deploy.egg-info/entry_points.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       44 2024-04-21 22:34:19.000000 stackql_deploy-1.1.0/stackql_deploy.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-21 22:34:19.000000 stackql_deploy-1.1.0/stackql_deploy.egg-info/top_level.txt
```

### Comparing `stackql_deploy-1.0.9/LICENSE` & `stackql_deploy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.9/PKG-INFO` & `stackql_deploy-1.1.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,218 +1,197 @@
-Metadata-Version: 2.1
-Name: stackql-deploy
-Version: 1.0.9
-Summary: Model driven resource provisioning and deployment framework using StackQL.
-Home-page: https://github.com/stackql/stackql-deploy
-Author: Jeffrey Aven
-Author-email: javen@stackql.io
-License: MIT
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: python-dotenv
-Requires-Dist: jinja2
-Requires-Dist: pystackql
-
-.. image:: https://stackql.io/img/stackql-logo-bold.png
-    :alt: "stackql logo"
-    :target: https://github.com/stackql/stackql
-    :align: center
-
-==========================================================================
-Model driven resource provisioning and deployment framework using StackQL.
-==========================================================================
-
-.. .. image:: https://readthedocs.org/projects/pystackql/badge/?version=latest
-..    :target: https://pystackql.readthedocs.io/en/latest/
-..    :alt: Documentation Status
-
-.. image:: https://img.shields.io/pypi/v/stackql-deploy
-   :target: https://pypi.org/project/stackql-deploy/
-   :alt: PyPI
-
-==============
-
-**stackql-deploy** is a multi-cloud Infrastructure as Code (IaC) framework using `stackql`_, inspired by dbt (data build tool), which manages data transformation workflows in analytics engineering by treating SQL scripts as models that can be built, tested, and materialized incrementally. You can create a similar framework for infrastructure provisioning with StackQL. The goal is to treat infrastructure-as-code (IaC) queries as models that can be deployed, managed, and interconnected.
-
-This ELT/model-based framework to IaC allows you to provision, test, update and teardown multi-cloud stacks similar to how dbt manages data transformation projects, with the benefits of version control, peer review, and automation. This approach enables you to deploy complex, dependent infrastructure components in a reliable and repeatable manner.
-
-The use of StackQL simplifies the interaction with cloud resources by using SQL-like syntax, making it easier to define and execute complex cloud management operations. Resources are provisioned with ``INSERT`` statements and tests are structured around ``SELECT`` statements.
-
-Features include:
-
-- Dynamic state determination (eliminating the need for state files)
-- Simple flow control with rollback capabilities
-- Single code base for multiple target environments
-- SQL-based definitions for resources and tests
-
-How stackql-deploy Works
-------------------------
-
-**stackql-deploy** orchestrates cloud resource provisioning by parsing SQL-like definitions. It determines the necessity of creating or updating resources based on preflight checks, and ensures the creation and correct desired configuration through post-deployment verifications.
-
-.. image:: https://stackql.io/img/blog/stackql-deploy.png
-    :alt: "stackql-deploy"
-    :target: https://github.com/stackql/stackql
-
-Installing from PyPI
---------------------
-
-To install **stackql-deploy** directly from PyPI, run the following command:
-
-.. code-block:: none
-
-    pip install stackql-deploy
-
-This will install the latest version of **stackql-deploy** and its dependencies from the Python Package Index.
-
-Running stackql-deploy
-----------------------
-
-Once installed, use the `build`, `test`, or `teardown` commands as shown here:
-
-.. code-block:: none
-
-    stackql-deploy build prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000 --dry-run
-    stackql-deploy build prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
-    stackql-deploy test prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
-    stackql-deploy teardown prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
-
-.. note::
-   ``teardown`` deprovisions resources in reverse order to creation
-
-additional options include:
-
-- ``--dry-run``: perform a dry run of the stack operations.
-- ``--on-failure=rollback``: action on failure: rollback, ignore or error.
-- ``--env-file=.env``: specify an environment variable file.
-- ``-e KEY=value```: pass additional environment variables.
-- ``--log-level`` : logging level (DEBUG, INFO, WARNING, ERROR, CRITICAL), defaults to INFO.
-
-use ``stackql-deploy info`` to show information about the package and environment, for example
-
-.. code-block:: none
-
-    $ stackql-deploy info
-    stackql-deploy version: 1.0.0
-    pystackql version     : 3.5.4
-    stackql version       : v0.5.612
-    stackql binary path   : /mnt/c/LocalGitRepos/stackql/stackql-deploy/stackql
-    platform              : Linux x86_64 (Linux-5.15.133.1-microsoft-standard-WSL2-x86_64-with-glibc2.35), Python 3.10.12
-
-Use the ``--help`` option to see more information about the commands and options available:
-
-.. code-block:: none
-
-    stackql-deploy --help
-
-Project Structure
------------------
-
-**stackql-deploy** uses a modular structure where each component of the infrastructure is defined in separate files, allowing for clear separation of concerns and easy management. This example is based on a stack named ``example_stack``, with a resource named ``monitor_resource_group``.
-
-::
-
-    ├── example_stack
-    │   ├── stackql_docs
-    │   │   └── monitor_resource_group.md
-    │   ├── stackql_manifest.yml
-    │   ├── stackql_resources
-    │   │   └── monitor_resource_group.iql
-    │   └── stackql_tests
-    │       └── monitor_resource_group.iql
-
-Manifest File
--------------
-
-- **Manifest File**: The ``stackql_manifest.yml`` is used to define your stack and manage dependencies between infrastructure components. This file defines which resources need to be provisioned before others and parameterizes resources based on environment variables or other configurations.
-
-.. code-block:: yaml
-
-    version: 1
-    name: example_stack
-    description: oss activity monitor stack
-    providers:
-      - azure
-    globals:
-      - name: subscription_id
-        description: azure subscription id
-        value: "{{ vars.AZURE_SUBSCRIPTION_ID }}"
-      - name: location
-        value: eastus
-      - name: resource_group_name_base
-        value: "activity-monitor"
-    resources:
-      - name: monitor_resource_group
-        description: azure resource group for activity monitor
-        props:
-          - name: resource_group_name
-            description: azure resource group name
-            value: "{{ globals.resource_group_name_base }}-{{ globals.stack_env }}"
-            # OR YOU CAN DO...
-            # values:
-            #   prd:
-            #     value: "activity-monitor-prd"
-            #   sit:
-            #     value: "activity-monitor-sit"
-            #   dev:
-            #     value: "activity-monitor-dev"
-
-
-Resource and Test SQL Files
-----------------------------
-
-These files define the SQL-like commands for creating, updating, and testing the deployment of resources.
-
-**Resource SQL (stackql_resources/monitor_resource_group.iql):**
-
-.. code-block:: sql
-
-    /*+ create */
-    INSERT INTO azure.resources.resource_groups(
-      resourceGroupName,
-      subscriptionId,
-      data__location
-    )
-    SELECT
-      '{{ resource_group_name }}',
-      '{{ subscription_id }}',
-      '{{ location }}'
-
-    /*+ update */
-    UPDATE azure.resources.resource_groups
-    SET data__location = '{{ location }}'
-    WHERE resourceGroupName = '{{ resource_group_name }}'
-      AND subscriptionId = '{{ subscription_id }}'
-
-    /*+ delete */
-    DELETE FROM azure.resources.resource_groups
-    WHERE resourceGroupName = '{{ resource_group_name }}' AND subscriptionId = '{{ subscription_id }}'
-
-**Test SQL (stackql_tests/monitor_resource_group.iql):**
-
-.. code-block:: sql
-
-    /*+ preflight */
-    SELECT COUNT(*) as count FROM azure.resources.resource_groups
-    WHERE subscriptionId = '{{ subscription_id }}'
-    AND resourceGroupName = '{{ resource_group_name }}'
-
-    /*+ postdeploy, retries=5, retry_delay=5 */
-    SELECT COUNT(*) as count FROM azure.resources.resource_groups
-    WHERE subscriptionId = '{{ subscription_id }}'
-    AND resourceGroupName = '{{ resource_group_name }}'
-    AND location = '{{ location }}'
-    AND JSON_EXTRACT(properties, '$.provisioningState') = 'Succeeded'
-
-**stackql-deploy** simplifies cloud resource management by treating infrastructure as flexible, dynamically assessed code.
-
-.. _stackql: https://github.com/stackql/stackql
+.. image:: https://stackql.io/img/stackql-logo-bold.png
+    :alt: "stackql logo"
+    :target: https://github.com/stackql/stackql
+    :align: center
+
+==========================================================================
+Model driven resource provisioning and deployment framework using StackQL.
+==========================================================================
+
+.. .. image:: https://readthedocs.org/projects/pystackql/badge/?version=latest
+..    :target: https://pystackql.readthedocs.io/en/latest/
+..    :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/v/stackql-deploy
+   :target: https://pypi.org/project/stackql-deploy/
+   :alt: PyPI
+
+==============
+
+**stackql-deploy** is a multi-cloud Infrastructure as Code (IaC) framework using `stackql`_, inspired by dbt (data build tool), which manages data transformation workflows in analytics engineering by treating SQL scripts as models that can be built, tested, and materialized incrementally. You can create a similar framework for infrastructure provisioning with StackQL. The goal is to treat infrastructure-as-code (IaC) queries as models that can be deployed, managed, and interconnected.
+
+This ELT/model-based framework to IaC allows you to provision, test, update and teardown multi-cloud stacks similar to how dbt manages data transformation projects, with the benefits of version control, peer review, and automation. This approach enables you to deploy complex, dependent infrastructure components in a reliable and repeatable manner.
+
+The use of StackQL simplifies the interaction with cloud resources by using SQL-like syntax, making it easier to define and execute complex cloud management operations. Resources are provisioned with ``INSERT`` statements and tests are structured around ``SELECT`` statements.
+
+Features include:
+
+- Dynamic state determination (eliminating the need for state files)
+- Simple flow control with rollback capabilities
+- Single code base for multiple target environments
+- SQL-based definitions for resources and tests
+
+How stackql-deploy Works
+------------------------
+
+**stackql-deploy** orchestrates cloud resource provisioning by parsing SQL-like definitions. It determines the necessity of creating or updating resources based on preflight checks, and ensures the creation and correct desired configuration through post-deployment verifications.
+
+.. image:: https://stackql.io/img/blog/stackql-deploy.png
+    :alt: "stackql-deploy"
+    :target: https://github.com/stackql/stackql
+
+Installing from PyPI
+--------------------
+
+To install **stackql-deploy** directly from PyPI, run the following command:
+
+.. code-block:: none
+
+    pip install stackql-deploy
+
+This will install the latest version of **stackql-deploy** and its dependencies from the Python Package Index.
+
+Running stackql-deploy
+----------------------
+
+Once installed, use the `build`, `test`, or `teardown` commands as shown here:
+
+.. code-block:: none
+
+    stackql-deploy build prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000 --dry-run
+    stackql-deploy build prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
+    stackql-deploy test prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
+    stackql-deploy teardown prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
+
+.. note::
+   ``teardown`` deprovisions resources in reverse order to creation
+
+additional options include:
+
+- ``--dry-run``: perform a dry run of the stack operations.
+- ``--on-failure=rollback``: action on failure: rollback, ignore or error.
+- ``--env-file=.env``: specify an environment variable file.
+- ``-e KEY=value```: pass additional environment variables.
+- ``--log-level`` : logging level (DEBUG, INFO, WARNING, ERROR, CRITICAL), defaults to INFO.
+
+use ``stackql-deploy info`` to show information about the package and environment, for example
+
+.. code-block:: none
+
+    $ stackql-deploy info
+    stackql-deploy version: 1.0.0
+    pystackql version     : 3.5.4
+    stackql version       : v0.5.612
+    stackql binary path   : /mnt/c/LocalGitRepos/stackql/stackql-deploy/stackql
+    platform              : Linux x86_64 (Linux-5.15.133.1-microsoft-standard-WSL2-x86_64-with-glibc2.35), Python 3.10.12
+
+Use the ``--help`` option to see more information about the commands and options available:
+
+.. code-block:: none
+
+    stackql-deploy --help
+
+Project Structure
+-----------------
+
+**stackql-deploy** uses a modular structure where each component of the infrastructure is defined in separate files, allowing for clear separation of concerns and easy management. This example is based on a stack named ``example_stack``, with a resource named ``monitor_resource_group``.
+
+::
+
+    ├── example_stack
+    │   ├── stackql_docs
+    │   │   └── monitor_resource_group.md
+    │   ├── stackql_manifest.yml
+    │   ├── stackql_resources
+    │   │   └── monitor_resource_group.iql
+    │   └── stackql_tests
+    │       └── monitor_resource_group.iql
+
+.. note::
+   use the ``init`` command to create a new project structure with sample files, for example ``stackql-deploy init example_stack``
+
+Manifest File
+-------------
+
+- **Manifest File**: The ``stackql_manifest.yml`` is used to define your stack and manage dependencies between infrastructure components. This file defines which resources need to be provisioned before others and parameterizes resources based on environment variables or other configurations.
+
+.. code-block:: yaml
+
+    version: 1
+    name: example_stack
+    description: oss activity monitor stack
+    providers:
+      - azure
+    globals:
+      - name: subscription_id
+        description: azure subscription id
+        value: "{{ vars.AZURE_SUBSCRIPTION_ID }}"
+      - name: location
+        value: eastus
+      - name: resource_group_name_base
+        value: "activity-monitor"
+    resources:
+      - name: monitor_resource_group
+        description: azure resource group for activity monitor
+        props:
+          - name: resource_group_name
+            description: azure resource group name
+            value: "{{ globals.resource_group_name_base }}-{{ globals.stack_env }}"
+            # OR YOU CAN DO...
+            # values:
+            #   prd:
+            #     value: "activity-monitor-prd"
+            #   sit:
+            #     value: "activity-monitor-sit"
+            #   dev:
+            #     value: "activity-monitor-dev"
+
+
+Resource and Test SQL Files
+----------------------------
+
+These files define the SQL-like commands for creating, updating, and testing the deployment of resources.
+
+**Resource SQL (stackql_resources/monitor_resource_group.iql):**
+
+.. code-block:: sql
+
+    /*+ create */
+    INSERT INTO azure.resources.resource_groups(
+      resourceGroupName,
+      subscriptionId,
+      data__location
+    )
+    SELECT
+      '{{ resource_group_name }}',
+      '{{ subscription_id }}',
+      '{{ location }}'
+
+    /*+ update */
+    UPDATE azure.resources.resource_groups
+    SET data__location = '{{ location }}'
+    WHERE resourceGroupName = '{{ resource_group_name }}'
+      AND subscriptionId = '{{ subscription_id }}'
+
+    /*+ delete */
+    DELETE FROM azure.resources.resource_groups
+    WHERE resourceGroupName = '{{ resource_group_name }}' AND subscriptionId = '{{ subscription_id }}'
+
+**Test SQL (stackql_tests/monitor_resource_group.iql):**
+
+.. code-block:: sql
+
+    /*+ preflight */
+    SELECT COUNT(*) as count FROM azure.resources.resource_groups
+    WHERE subscriptionId = '{{ subscription_id }}'
+    AND resourceGroupName = '{{ resource_group_name }}'
+
+    /*+ postdeploy, retries=5, retry_delay=5 */
+    SELECT COUNT(*) as count FROM azure.resources.resource_groups
+    WHERE subscriptionId = '{{ subscription_id }}'
+    AND resourceGroupName = '{{ resource_group_name }}'
+    AND location = '{{ location }}'
+    AND JSON_EXTRACT(properties, '$.provisioningState') = 'Succeeded'
+
+**stackql-deploy** simplifies cloud resource management by treating infrastructure as flexible, dynamically assessed code.
+
+.. _stackql: https://github.com/stackql/stackql
```

### Comparing `stackql_deploy-1.0.9/stackql_deploy/cmd/build.py` & `stackql_deploy-1.1.0/stackql_deploy/cmd/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from ..lib.utils import run_test, perform_retries, run_stackql_command
+from ..lib.utils import run_test, perform_retries, run_stackql_command, catch_error_and_exit
 from ..lib.config import setup_environment, load_manifest, get_global_context_and_providers, get_full_context
 from ..lib.templating import get_queries
 
 class StackQLProvisioner:
     
     def __init__(self, stackql, vars, logger, stack_dir, stack_env):
         self.stackql = stackql
@@ -34,15 +34,15 @@
             test_queries, test_query_options = get_queries(self.env, self.stack_dir, 'stackql_tests', resource, full_context, False, self.logger)
 
             create_query = None
             createorupdate_query = None
             update_query = None
 
             if not (('create' in resource_queries or 'createorupdate' in resource_queries) or ('create' in resource_queries and 'update' in resource_queries)):
-                raise ValueError("iql file must include either 'create' or 'createorupdate' anchor, or both 'create' and 'update' anchors.")
+                catch_error_and_exit("iql file must include either 'create' or 'createorupdate' anchor, or both 'create' and 'update' anchors.", self.logger)
 
             if 'create' in resource_queries:
                 create_query = resource_queries['create']
 
             if 'createorupdate' in resource_queries:
                 createorupdate_query = resource_queries['createorupdate']
 
@@ -115,13 +115,11 @@
             else:
                 post_deploy_check_passed = perform_retries(resource, postdeploy_query, postdeploy_retries, postdeploy_retry_delay, self.stackql, self.logger)
                 
             #
             # postdeploy check complete
             #
             if not post_deploy_check_passed:
-                error_message = f"deployment failed for {resource['name']} after post-deploy checks."
-                self.logger.error(error_message)
-                sys.exit(error_message)
+                catch_error_and_exit(f"deployment failed for {resource['name']} after post-deploy checks.", self.logger)
 
             if not dry_run:
                 self.logger.info(f"successfully deployed {resource['name']}")
```

### Comparing `stackql_deploy-1.0.9/stackql_deploy/cmd/teardown.py` & `stackql_deploy-1.1.0/stackql_deploy/cmd/teardown.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.9/stackql_deploy/cmd/test.py` & `stackql_deploy-1.1.0/stackql_deploy/cmd/test.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.9/stackql_deploy/lib/config.py` & `stackql_deploy-1.1.0/stackql_deploy/lib/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os, yaml
-from .utils import pull_providers
+from .utils import pull_providers, catch_error_and_exit
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 
 def render_globals(env, vars, global_vars, stack_env):
     # Render globals with vars and include the stack_env as a special variable
     global_context = {'stack_env': stack_env}
     # Render each global variable defined in the manifest
     for global_var in global_vars:
@@ -24,39 +24,34 @@
             elif 'values' in prop:
                 # Environment-specific values
                 env_value = prop['values'].get(global_context['stack_env'], {}).get('value')
                 if env_value is not None:
                     template = env.from_string(env_value)
                     prop_context[prop['name']] = template.render(globals=global_context)
                 else:
-                    logger.error(f"No value specified for property '{prop['name']}' in stack_env '{global_context['stack_env']}'.")
-                    raise ValueError(f"No value specified for property '{prop['name']}' in stack_env '{global_context['stack_env']}'.")
+                    catch_error_and_exit(f"No value specified for property '{prop['name']}' in stack_env '{global_context['stack_env']}'.", logger)
         except Exception as e:
-            logger.error(f"Failed to render property '{prop['name']}': {e}")
-            raise
+            catch_error_and_exit(f"Failed to render property '{prop['name']}': {e}", logger)
     return prop_context
     
 #
 # exported functions
 #
 
 def load_manifest(stack_dir, logger):
     try:
         # Load and parse the stackql_manifest.yml
         with open(os.path.join(stack_dir, 'stackql_manifest.yml')) as f:
             return yaml.safe_load(f)
     except Exception as e:
-        logger.error("failed to load manifest: " + str(e))
-        raise
+        catch_error_and_exit("failed to load manifest: " + str(e), logger)
 
 def setup_environment(stack_dir, logger):
     if not os.path.exists(stack_dir):
-        errmsg = "stack directory does not exist."
-        logger.error(errmsg)
-        raise FileNotFoundError(errmsg)
+        catch_error_and_exit("stack directory does not exist.", logger)
     env = Environment(
         loader=FileSystemLoader(os.getcwd()),
         autoescape=select_autoescape()
     )
     return env
 
 def get_global_context_and_providers(env, manifest, vars, stack_env, stackql, logger):
@@ -64,20 +59,18 @@
     try:
         global_vars = manifest.get('globals', [])
         global_context = render_globals(env, vars, global_vars, stack_env)
         providers = manifest.get('providers', [])
         pull_providers(providers, stackql, logger)
         return global_context, providers
     except Exception as e:
-        logger.error("Failed to prepare the context: " + str(e))
-        raise
+        catch_error_and_exit("failed to prepare the context: " + str(e), logger)
 
 def get_full_context(env, global_context, resource, logger):
     try:
         resource_props = resource.get('props', {})
         prop_context = render_properties(env, resource_props, global_context, logger)
         full_context = {**global_context, **prop_context}
-        logger.debug(f"Full context: {full_context}")
+        logger.debug(f"full context: {full_context}")
         return full_context
     except Exception as e:
-        logger.error(f"Failed to render properties for {resource.get('name', 'unknown')}: " + str(e))
-        raise
+        catch_error_and_exit(f"failed to render properties for {resource.get('name', 'unknown')}: " + str(e), logger)
```

### Comparing `stackql_deploy-1.0.9/stackql_deploy/lib/templating.py` & `stackql_deploy-1.1.0/stackql_deploy/lib/templating.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-
+from .utils import catch_error_and_exit
 
 def parse_anchor(anchor):
     """Parse anchor to extract key and options."""
     parts = anchor.split(',')
     key = parts[0].strip()
     options = {}
     for part in parts[1:]:
@@ -54,20 +54,18 @@
 #
 
 def get_queries(env, stack_dir, doc_key, resource, full_context, fail_on_error, logger):
     """returns rendered queries and query options for a resource."""
     template_path = os.path.join(stack_dir, doc_key, f"{resource['name']}.iql")
     if not os.path.exists(template_path):
         if fail_on_error:
-            logger.error(f"query file not found: {template_path}")
-            raise
+            catch_error_and_exit(f"query file not found: {template_path}", logger)
         else:
             return {}, {}
     try:
         query_templates, query_options = load_sql_queries(template_path)
         queries = render_queries(env, query_templates, full_context)
         logger.debug(f"rendered queries: {queries}")
         logger.debug(f"query options: {query_options}")
         return queries, query_options
     except Exception as e:
-        logger.error(f"failed to load or render queries for {resource['name']}: " + str(e))
-        raise
+        catch_error_and_exit(f"failed to load or render queries for {resource['name']}: " + str(e), logger)
```

### Comparing `stackql_deploy-1.0.9/stackql_deploy.egg-info/PKG-INFO` & `stackql_deploy-1.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,50 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.9
+Version: 1.1.0
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
-License: MIT
+License: MIT License
+        
+        Copyright (c) 2022 StackQL Studios
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: python-dotenv
 Requires-Dist: jinja2
-Requires-Dist: pystackql
+Requires-Dist: pystackql>=3.6.1
 
 .. image:: https://stackql.io/img/stackql-logo-bold.png
     :alt: "stackql logo"
     :target: https://github.com/stackql/stackql
     :align: center
 
 ==========================================================================
@@ -126,14 +146,17 @@
     │   │   └── monitor_resource_group.md
     │   ├── stackql_manifest.yml
     │   ├── stackql_resources
     │   │   └── monitor_resource_group.iql
     │   └── stackql_tests
     │       └── monitor_resource_group.iql
 
+.. note::
+   use the ``init`` command to create a new project structure with sample files, for example ``stackql-deploy init example_stack``
+
 Manifest File
 -------------
 
 - **Manifest File**: The ``stackql_manifest.yml`` is used to define your stack and manage dependencies between infrastructure components. This file defines which resources need to be provisioned before others and parameterizes resources based on environment variables or other configurations.
 
 .. code-block:: yaml
```


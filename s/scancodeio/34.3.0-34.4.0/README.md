# Comparing `tmp/scancodeio-34.3.0.tar.gz` & `tmp/scancodeio-34.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scancodeio-34.3.0.tar", last modified: Wed Apr 10 16:28:55 2024, max compression
+gzip compressed data, was "scancodeio-34.4.0.tar", last modified: Mon Apr 22 09:30:25 2024, max compression
```

## Comparing `scancodeio-34.3.0.tar` & `scancodeio-34.4.0.tar`

### file list

```diff
@@ -1,552 +1,553 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.889352 scancodeio-34.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.773350 scancodeio-34.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.781350 scancodeio-34.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.github/workflows/ci-docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.github/workflows/publish-docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-10 16:28:50.000000 scancodeio-34.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    54610 2024-04-10 16:28:50.000000 scancodeio-34.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-10 16:28:50.000000 scancodeio-34.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-10 16:28:50.000000 scancodeio-34.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-10 16:28:50.000000 scancodeio-34.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-10 16:28:50.000000 scancodeio-34.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-10 16:28:50.000000 scancodeio-34.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-10 16:28:55.889352 scancodeio-34.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-10 16:28:50.000000 scancodeio-34.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docker-compose-offline.yml
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docker-compose.dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docker.env
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.785350 scancodeio-34.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/application-settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/automation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/built-in-pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/command-line-interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/custom-pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/data-models.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/distros-os-images.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/faq.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.793350 scancodeio-34.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   347827 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/license-clarity-scan-summary.png
--rw-r--r--   0 runner    (1001) docker     (127)   113257 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/output-files-download-results.png
--rw-r--r--   0 runner    (1001) docker     (127)    49405 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/output-files-projects-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    59030 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/output-files-xlsx-packages.png
--rw-r--r--   0 runner    (1001) docker     (127)    56604 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/output-files-xlsx-resources.png
--rw-r--r--   0 runner    (1001) docker     (127)   161773 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-extra-data.png
--rw-r--r--   0 runner    (1001) docker     (127)    45598 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-icon-link.png
--rw-r--r--   0 runner    (1001) docker     (127)    78178 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-packages-link.png
--rw-r--r--   0 runner    (1001) docker     (127)    47458 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-license-policies-results.png
--rw-r--r--   0 runner    (1001) docker     (127)   148235 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-errors-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    71050 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-packages-charts.png
--rw-r--r--   0 runner    (1001) docker     (127)   115814 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-packages-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    86303 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-project-details.png
--rw-r--r--   0 runner    (1001) docker     (127)   152148 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-project-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-project-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    50351 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-projects-list.png
--rw-r--r--   0 runner    (1001) docker     (127)   165263 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-resources-charts.png
--rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-resources-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)   191624 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/tutorial-web-ui-run-log-modal.png
--rw-r--r--   0 runner    (1001) docker     (127)    53788 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-archive-action.png
--rw-r--r--   0 runner    (1001) docker     (127)   127740 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-archive-modal.png
--rw-r--r--   0 runner    (1001) docker     (127)   153488 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-create-project.png
--rw-r--r--   0 runner    (1001) docker     (127)    52651 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-delete-action.png
--rw-r--r--   0 runner    (1001) docker     (127)   108653 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-delete-modal.png
--rw-r--r--   0 runner    (1001) docker     (127)    51714 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-project-details.png
--rw-r--r--   0 runner    (1001) docker     (127)    27257 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-project-list-empty.png
--rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-project-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    52920 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-reset-action.png
--rw-r--r--   0 runner    (1001) docker     (127)    93458 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/images/user-interface-reset-modal.png
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16404 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/output-files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/project-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/rest-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/scanpipe-concepts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/scanpipe-pipes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_api_analyze_package_archive.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_cli_analyze_codebase.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_cli_analyze_docker_image.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_license_policies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_vulnerablecode_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_web_ui_analyze_docker_image.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/tutorial_web_ui_review_scan_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-10 16:28:50.000000 scancodeio-34.3.0/docs/user-interface.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.773350 scancodeio-34.3.0/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.773350 scancodeio-34.3.0/etc/nginx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.793350 scancodeio-34.3.0/etc/nginx/conf.d/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/nginx/conf.d/default.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.793350 scancodeio-34.3.0/etc/nginx/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/nginx/examples/ssl.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.801350 scancodeio-34.3.0/etc/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/bsd-new.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/bsd-simplified.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/isc.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26418 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/lgpl-2.1-plus.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/mit.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/python.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)  5705128 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/virtualenv.pyz
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-10 16:28:50.000000 scancodeio-34.3.0/etc/thirdparty/virtualenv.pyz.ABOUT
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-10 16:28:50.000000 scancodeio-34.3.0/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scan.NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.805350 scancodeio-34.3.0/scancodeio/
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/scan.NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.809350 scancodeio-34.3.0/scancodeio/static/
--rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   422462 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/ace-1.20.0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/ace-1.20.0.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)   368864 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/ace-1.9.5.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/add-inputs.js
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/billboard-3.0.1-datalab.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   465309 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/billboard-3.0.1.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/billboard-3.0.1.pkgd.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bsd-new.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bsd-simplified.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   207302 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bulma-0.9.4.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bulma-toast-2.4.1.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/cc-by-4.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/highlight-10.6.0.css
--rw-r--r--   0 runner    (1001) docker     (127)   133121 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/highlight-10.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/highlight.js-10.6.0.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    15888 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/html5sortable-0.9.17.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    44717 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/htmx-1.9.5.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/htmx-1.9.5.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/mit.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/static/ofl-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scancodeio/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.885352 scancodeio-34.3.0/scancodeio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21925 2024-04-10 16:28:55.000000 scancodeio-34.3.0/scancodeio.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.809350 scancodeio-34.3.0/scanpipe/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.813351 scancodeio-34.3.0/scanpipe/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    25421 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.773350 scancodeio-34.3.0/scanpipe/management/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.813351 scancodeio-34.3.0/scanpipe/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/add-input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/add-pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/archive-project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/create-project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/create-user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/delete-project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/list-project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/purldb-scan-queue-worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/reset-project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/show-pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/management/commands/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.821351 scancodeio-34.3.0/scanpipe/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0002_run_id_and_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0003_remove_run_run_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0004_run_pipeline_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0005_project_input_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0008_package_extra_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0009_discoveredpackage_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0010_codebaseresource_is_key_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0011_codebaseresource_is_media.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0012_run_scancodeio_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0013_project_is_archived.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0014_webhooksubscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0016_discoveredpackage_package_uid.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0018_codebaseresource_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0019_auto_20220804_1836.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0020_alter_codebaseresource_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0021_codebaseresource_package_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0022_create_discovereddependencies_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0023_migrate_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0024_remove_discoveredpackage_dependencies_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0026_run_current_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0028_codebaserelation_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0033_project_notes_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0034_project_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0035_set_projects_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0036_alter_project_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0037_discoveredpackage_vulnerability_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0038_migrate_vulnerability_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0040_discovereddependency_affected_by_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0041_projectmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0042_projecterror_to_projectmessage_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0043_delete_projecterror.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0044_uuidtaggeditem_project_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0045_scan_codebase_packages_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0046_discoveredpackage_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0047_discoveredpackage_scanpipe_di_version_44de05_idx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0048_inputsource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0049_input_sources_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0050_remove_project_input_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0051_rename_pipelines_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0052_run_selected_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0053_restructure_pipelines_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0054_rename_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/0055_discoveredpackage_datafile_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   120580 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.825351 scancodeio-34.3.0/scanpipe/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/collect_source_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/collect_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/deploy_to_develop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/docker_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/find_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/inspect_elf_binaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/inspect_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/load_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/load_sbom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/match_to_matchcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/populate_purldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/resolve_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/root_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/scan_codebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipelines/scan_single_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.829351 scancodeio-34.3.0/scanpipe/pipes/
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/codebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/cyclonedx.py
--rw-r--r--   0 runner    (1001) docker     (127)    60696 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/d2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/elf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     8787 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/js.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/matchcode.py
--rw-r--r--   0 runner    (1001) docker     (127)    30292 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/pathmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/purldb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/rootfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/scancode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.829351 scancodeio-34.3.0/scanpipe/pipes/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    45964 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/schemas/spdx-schema-2.3.json
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/schemas/spdx-schema-2.3.json.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/source_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/spdx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/vulnerablecode.py
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/pipes/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.773350 scancodeio-34.3.0/scanpipe/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.829351 scancodeio-34.3.0/scanpipe/templates/account/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/account/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.829351 scancodeio-34.3.0/scanpipe/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/registration/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.829351 scancodeio-34.3.0/scanpipe/templates/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/rest_framework/api.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.833351 scancodeio-34.3.0/scanpipe/templates/scanpipe/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/app_monitoring.html
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/attribution.html
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dependency_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dependency_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.837351 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/dropdown_hoverable.html
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/filter_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/filter_dropdown_choices_field.html
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/help_dropdown_tooltip.html
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/list_actions_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/project_actions_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/project_download_dropdown.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.841351 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/file_filter.html
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/filter_sort.html
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/filters_breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/form_errors.html
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/list_view_thead.html
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/messages.html
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/navbar_header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination.html
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination_header_relations.html
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_clone_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_downloads.html
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_labels.html
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_list_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_summary_level.html
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/resource_chart_column.html
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/resource_path_links.html
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/run_status_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/search_field.html
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/license_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/license_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/message_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.841351 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_inputs_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_labels_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_pipeline_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/clone_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/edit_input_tag_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal_content.html
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_archive_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_delete_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_inputs_delete_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_reset_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_archive_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_delete_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_reset_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/run_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/run_modal_content.html
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/search_syntax_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/package_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/package_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.845351 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/license_clarity_panel.html
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_codebase.html
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_inputs.html
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_outputs.html
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_pipelines.html
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/resource_license_summary.html
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/resource_status_summary.html
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/scan_summary_panel.html
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/project_charts.html
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/project_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/project_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/project_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/project_settings.html
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/relation_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/resource_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/resource_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.845351 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/field_datafile_resource.html
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/field_default.html
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/field_for_package.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/field_raw.html
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_content_viewer.html
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_default.html
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_detections.html
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_image.html
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_packages.html
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_purldb_content.html
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_purldb_loader.html
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_relations.html
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_resources.html
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tabset.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.849351 scancodeio-34.3.0/scanpipe/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.869351 scancodeio-34.3.0/scanpipe/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    16295 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/alpine_3_15_4.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)   223597 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/archive.zip
--rw-r--r--   0 runner    (1001) docker     (127)    19948 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (127)    21668 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json
--rw-r--r--   0 runner    (1001) docker     (127)    88110 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json
--rw-r--r--   0 runner    (1001) docker     (127)    53875 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json
--rw-r--r--   0 runner    (1001) docker     (127)    90354 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json
--rw-r--r--   0 runner    (1001) docker     (127)    92805 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_tree.json
--rw-r--r--   0 runner    (1001) docker     (127)    91287 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/basic-rootfs.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)    33965 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json
--rw-r--r--   0 runner    (1001) docker     (127)  1447917 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/centos.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)  5427973 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/centos_scan_codebase.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.869351 scancodeio-34.3.0/scanpipe/tests/data/codebase/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/codebase/a.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/codebase/b.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/codebase/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.869351 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/
--rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json
--rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/django-4.0.10-vulnerability.json
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/django-4.0.10_as_cdx.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   105830 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.2.json
--rw-r--r--   0 runner    (1001) docker     (127)   138679 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.3.json
--rw-r--r--   0 runner    (1001) docker     (127)   139669 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.json
--rw-r--r--   0 runner    (1001) docker     (127)   124554 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.xml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/missing_bom_format.json
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/missing_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/nested.cdx.json
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/not_valid.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/
--rw-r--r--   0 runner    (1001) docker     (127)    60018 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/expected.json
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip
--rw-r--r--   0 runner    (1001) docker     (127)    37100 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d/find_java_packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/find_java_packages/Baz.class
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/find_java_packages/Baz.java
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/find_java_packages/Foo.java
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d/jars/
--rw-r--r--   0 runner    (1001) docker     (127)    21813 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip
--rw-r--r--   0 runner    (1001) docker     (127)    37325 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.877351 scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/license_mit.md
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/project.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/project_notice.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/non_whitespace_file.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d/whitespace_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.777350 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/from/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/from/main.js
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/from/unmain.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.873351 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/main.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/unmain.js
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (127)    41154 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/debian.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)    39888 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/debian_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)    57175 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)    24550 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    25250 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)   176998 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)    22298 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json
--rw-r--r--   0 runner    (1001) docker     (127)   148656 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/flume-ng-node-d2d-input.json
--rw-r--r--   0 runner    (1001) docker     (127)   156717 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/flume-ng-node-d2d.json
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/foobar.qcow2.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)    62008 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)  1674309 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.877351 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0.tgz
--rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)    17775 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/javascript_collect_symbols.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.877351 scancodeio-34.3.0/scanpipe/tests/data/jvm/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/jvm/common.java
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/jvm/no-package.java
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.877351 scancodeio-34.3.0/scanpipe/tests/data/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/Django-4.0.8-py3-none-any.whl.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11.pom.xml
--rw-r--r--   0 runner    (1001) docker     (127)    25761 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11_scan_package.json
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/package.expected.json
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/poor_values.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/python-inspector-0.10.0.zip
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/toml.json
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/manifests/toml.spdx.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.777350 scancodeio-34.3.0/scanpipe/tests/data/matchcode/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_check_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_results_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_post_response.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)    32504 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/notice.NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/data/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    24930 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/outputs/expected_attribution.html
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/outputs/render_me.html
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/policies.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/data/scancode/
--rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json
--rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/scancode/package_assembly_codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/scancode/package_assembly_codebase.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/data/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/settings/scancode-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/data/spdx/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/spdx/example-2.3.1.json
--rw-r--r--   0 runner    (1001) docker     (127)    18944 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/data/windows-container-rootfs.tar
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.881352 scancodeio-34.3.0/scanpipe/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/profile_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/raise_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/register_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/steps_as_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipelines/with_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:55.885352 scancodeio-34.3.0/scanpipe/tests/pipes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_codebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_cyclonedx.py
--rw-r--r--   0 runner    (1001) docker     (127)    58850 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_d2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_js.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_matchcode.py
--rw-r--r--   0 runner    (1001) docker     (127)    28436 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_pathmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_pipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_purldb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10331 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_rootfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_scancode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_source_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15580 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_spdx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/pipes/test_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/regen_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44714 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    36535 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)   109259 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    52454 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_scancodeio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    46619 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    72631 2024-04-10 16:28:50.000000 scancodeio-34.3.0/scanpipe/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-10 16:28:55.889352 scancodeio-34.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1297 2024-04-10 16:28:50.000000 scancodeio-34.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.071572 scancodeio-34.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 09:30:21.000000 scancodeio-34.4.0/.VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-22 09:30:21.000000 scancodeio-34.4.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.959572 scancodeio-34.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.967572 scancodeio-34.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-22 09:30:21.000000 scancodeio-34.4.0/.github/workflows/ci-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-22 09:30:21.000000 scancodeio-34.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-22 09:30:21.000000 scancodeio-34.4.0/.github/workflows/publish-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-22 09:30:21.000000 scancodeio-34.4.0/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-22 09:30:21.000000 scancodeio-34.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 09:30:21.000000 scancodeio-34.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    55484 2024-04-22 09:30:21.000000 scancodeio-34.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-22 09:30:21.000000 scancodeio-34.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-22 09:30:21.000000 scancodeio-34.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-22 09:30:21.000000 scancodeio-34.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-22 09:30:21.000000 scancodeio-34.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-22 09:30:21.000000 scancodeio-34.4.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-22 09:30:25.071572 scancodeio-34.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-22 09:30:21.000000 scancodeio-34.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docker-compose-offline.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docker-compose.dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docker-compose.purldb-scan-worker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docker.env
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.971572 scancodeio-34.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/application-settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/automation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/built-in-pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/command-line-interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/custom-pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/data-models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/distros-os-images.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/faq.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.979572 scancodeio-34.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   347827 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/license-clarity-scan-summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)   113257 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/output-files-download-results.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49405 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/output-files-projects-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59030 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/output-files-xlsx-packages.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56604 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/output-files-xlsx-resources.png
+-rw-r--r--   0 runner    (1001) docker     (127)   161773 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-find-vulnerabilities-extra-data.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45598 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-find-vulnerabilities-icon-link.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78178 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-find-vulnerabilities-packages-link.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47458 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-license-policies-results.png
+-rw-r--r--   0 runner    (1001) docker     (127)   148235 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-web-ui-errors-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71050 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-web-ui-packages-charts.png
+-rw-r--r--   0 runner    (1001) docker     (127)   115814 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-web-ui-packages-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86303 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-web-ui-project-details.png
+-rw-r--r--   0 runner    (1001) docker     (127)   152148 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-web-ui-project-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-web-ui-project-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50351 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-web-ui-projects-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165263 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-web-ui-resources-charts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-web-ui-resources-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)   191624 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/tutorial-web-ui-run-log-modal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53788 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/user-interface-archive-action.png
+-rw-r--r--   0 runner    (1001) docker     (127)   127740 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/user-interface-archive-modal.png
+-rw-r--r--   0 runner    (1001) docker     (127)   153488 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/user-interface-create-project.png
+-rw-r--r--   0 runner    (1001) docker     (127)    52651 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/user-interface-delete-action.png
+-rw-r--r--   0 runner    (1001) docker     (127)   108653 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/user-interface-delete-modal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51714 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/user-interface-project-details.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27257 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/user-interface-project-list-empty.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/user-interface-project-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    52920 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/user-interface-reset-action.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93458 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/images/user-interface-reset-modal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16404 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/output-files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/project-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/rest-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/scanpipe-concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/scanpipe-pipes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/tutorial_api_analyze_package_archive.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/tutorial_cli_analyze_codebase.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/tutorial_cli_analyze_docker_image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/tutorial_license_policies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/tutorial_vulnerablecode_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/tutorial_web_ui_analyze_docker_image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/tutorial_web_ui_review_scan_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-22 09:30:21.000000 scancodeio-34.4.0/docs/user-interface.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.959572 scancodeio-34.4.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.959572 scancodeio-34.4.0/etc/nginx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.979572 scancodeio-34.4.0/etc/nginx/conf.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-22 09:30:21.000000 scancodeio-34.4.0/etc/nginx/conf.d/default.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.979572 scancodeio-34.4.0/etc/nginx/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-22 09:30:21.000000 scancodeio-34.4.0/etc/nginx/examples/ssl.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.991572 scancodeio-34.4.0/etc/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-22 09:30:21.000000 scancodeio-34.4.0/etc/thirdparty/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-22 09:30:21.000000 scancodeio-34.4.0/etc/thirdparty/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-22 09:30:21.000000 scancodeio-34.4.0/etc/thirdparty/bsd-simplified.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-22 09:30:21.000000 scancodeio-34.4.0/etc/thirdparty/isc.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26418 2024-04-22 09:30:21.000000 scancodeio-34.4.0/etc/thirdparty/lgpl-2.1-plus.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-22 09:30:21.000000 scancodeio-34.4.0/etc/thirdparty/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-22 09:30:21.000000 scancodeio-34.4.0/etc/thirdparty/python.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)  5705128 2024-04-22 09:30:21.000000 scancodeio-34.4.0/etc/thirdparty/virtualenv.pyz
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-22 09:30:21.000000 scancodeio-34.4.0/etc/thirdparty/virtualenv.pyz.ABOUT
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-22 09:30:21.000000 scancodeio-34.4.0/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scan.NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.991572 scancodeio-34.4.0/scancodeio/
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/scan.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.999572 scancodeio-34.4.0/scancodeio/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   422462 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/ace-1.20.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/ace-1.20.0.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)   368864 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/ace-1.9.5.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/add-inputs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/billboard-3.0.1-datalab.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   465309 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/billboard-3.0.1.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/billboard-3.0.1.pkgd.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/bsd-simplified.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   207302 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/bulma-0.9.4.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/bulma-toast-2.4.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/cc-by-4.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/highlight-10.6.0.css
+-rw-r--r--   0 runner    (1001) docker     (127)   133121 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/highlight-10.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/highlight.js-10.6.0.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    15888 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/html5sortable-0.9.17.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    44717 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/htmx-1.9.5.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/htmx-1.9.5.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/static/ofl-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scancodeio/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.071572 scancodeio-34.4.0/scancodeio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21957 2024-04-22 09:30:24.000000 scancodeio-34.4.0/scancodeio.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.999572 scancodeio-34.4.0/scanpipe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.999572 scancodeio-34.4.0/scanpipe/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25421 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.959572 scancodeio-34.4.0/scanpipe/management/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.003572 scancodeio-34.4.0/scanpipe/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/add-input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/add-pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/archive-project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/create-project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/create-user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/delete-project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/list-project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/purldb-scan-worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/reset-project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/show-pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/management/commands/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.011572 scancodeio-34.4.0/scanpipe/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0002_run_id_and_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0003_remove_run_run_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0004_run_pipeline_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0005_project_input_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0008_package_extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0009_discoveredpackage_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0010_codebaseresource_is_key_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0011_codebaseresource_is_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0012_run_scancodeio_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0013_project_is_archived.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0014_webhooksubscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0016_discoveredpackage_package_uid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0018_codebaseresource_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0019_auto_20220804_1836.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0020_alter_codebaseresource_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0021_codebaseresource_package_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0022_create_discovereddependencies_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0023_migrate_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0024_remove_discoveredpackage_dependencies_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0026_run_current_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0028_codebaserelation_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0033_project_notes_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0034_project_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0035_set_projects_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0036_alter_project_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0037_discoveredpackage_vulnerability_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0038_migrate_vulnerability_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0040_discovereddependency_affected_by_vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0041_projectmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0042_projecterror_to_projectmessage_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0043_delete_projecterror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0044_uuidtaggeditem_project_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0045_scan_codebase_packages_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0046_discoveredpackage_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0047_discoveredpackage_scanpipe_di_version_44de05_idx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0048_inputsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0049_input_sources_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0050_remove_project_input_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0051_rename_pipelines_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0052_run_selected_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0053_restructure_pipelines_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0054_rename_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/0055_discoveredpackage_datafile_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120580 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.015572 scancodeio-34.4.0/scanpipe/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/collect_source_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/collect_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/deploy_to_develop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/docker_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/find_vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/inspect_elf_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/inspect_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/load_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/load_sbom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/match_to_matchcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/populate_purldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/resolve_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/root_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/scan_codebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipelines/scan_single_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.019572 scancodeio-34.4.0/scanpipe/pipes/
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/codebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/cyclonedx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60696 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/d2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8787 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/js.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/matchcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30329 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/pathmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/purldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/scancode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.019572 scancodeio-34.4.0/scanpipe/pipes/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    45964 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/schemas/spdx-schema-2.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/schemas/spdx-schema-2.3.json.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/source_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/spdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/vulnerablecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/pipes/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.963572 scancodeio-34.4.0/scanpipe/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.019572 scancodeio-34.4.0/scanpipe/templates/account/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/account/profile.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.019572 scancodeio-34.4.0/scanpipe/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/registration/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.019572 scancodeio-34.4.0/scanpipe/templates/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/rest_framework/api.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.019572 scancodeio-34.4.0/scanpipe/templates/scanpipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/app_monitoring.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/attribution.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/dependency_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/dependency_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.023572 scancodeio-34.4.0/scanpipe/templates/scanpipe/dropdowns/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/dropdowns/dropdown_hoverable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/dropdowns/filter_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/dropdowns/filter_dropdown_choices_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/dropdowns/help_dropdown_tooltip.html
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/dropdowns/list_actions_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/dropdowns/project_actions_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/dropdowns/project_download_dropdown.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.027572 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/file_filter.html
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/filter_sort.html
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/filters_breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/form_errors.html
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/list_view_thead.html
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/messages.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/navbar_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/pagination_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/pagination_header_relations.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/project_clone_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/project_downloads.html
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/project_labels.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/project_list_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/project_summary_level.html
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/resource_chart_column.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/resource_path_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/run_status_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/search_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/license_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/license_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/message_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.027572 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/add_inputs_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/add_labels_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/add_pipeline_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/clone_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/edit_input_tag_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal_content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/project_archive_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/project_delete_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/project_inputs_delete_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/project_reset_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/projects_archive_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/projects_delete_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/projects_reset_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/run_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/run_modal_content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/search_syntax_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/package_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/package_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.031572 scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/license_clarity_panel.html
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/project_codebase.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/project_inputs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/project_outputs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/project_pipelines.html
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/resource_license_summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/resource_status_summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/scan_summary_panel.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/project_charts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/project_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/project_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/project_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/project_settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/relation_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/resource_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/resource_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.031572 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/field_datafile_resource.html
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/field_default.html
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/field_for_package.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/field_raw.html
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_content_viewer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_default.html
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_detections.html
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_image.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_packages.html
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_purldb_content.html
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_purldb_loader.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_relations.html
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_resources.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tabset.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.035572 scancodeio-34.4.0/scanpipe/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.055572 scancodeio-34.4.0/scanpipe/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    16295 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/alpine_3_15_4.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   223597 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/archive.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    19948 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (127)    21668 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)    88110 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json
+-rw-r--r--   0 runner    (1001) docker     (127)    53875 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90354 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)    92805 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_tree.json
+-rw-r--r--   0 runner    (1001) docker     (127)    91287 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/basic-rootfs.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    33965 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1447917 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/centos.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  5427973 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/centos_scan_codebase.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.055572 scancodeio-34.4.0/scanpipe/tests/data/codebase/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/codebase/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/codebase/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/codebase/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.055572 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/
+-rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/django-4.0.10-vulnerability.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/django-4.0.10_as_cdx.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.055572 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   105830 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   138679 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)   139669 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)   124554 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/missing_bom_format.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/missing_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/nested.cdx.json
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/not_valid.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.055572 scancodeio-34.4.0/scanpipe/tests/data/d2d/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.059572 scancodeio-34.4.0/scanpipe/tests/data/d2d/about_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    60018 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/about_files/expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    37100 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.059572 scancodeio-34.4.0/scanpipe/tests/data/d2d/find_java_packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/find_java_packages/Baz.class
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/find_java_packages/Baz.java
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/find_java_packages/Foo.java
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.059572 scancodeio-34.4.0/scanpipe/tests/data/d2d/jars/
+-rw-r--r--   0 runner    (1001) docker     (127)    21813 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    37325 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.059572 scancodeio-34.4.0/scanpipe/tests/data/d2d/legal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/legal/license_mit.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/legal/project.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/legal/project_notice.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/non_whitespace_file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d/whitespace_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.963572 scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.059572 scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/from/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/from/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/from/unmain.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.059572 scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/to/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/to/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/to/main.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/to/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/to/unmain.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (127)    41154 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/debian.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    39888 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/debian_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)    57175 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/docker-images.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    24550 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25250 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   176998 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)    22298 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json
+-rw-r--r--   0 runner    (1001) docker     (127)   148656 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/flume-ng-node-d2d-input.json
+-rw-r--r--   0 runner    (1001) docker     (127)   156717 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/flume-ng-node-d2d.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/foobar.qcow2.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    62008 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  1674309 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.063572 scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/is-npm-1.0.0.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17775 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/javascript_collect_symbols.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.063572 scancodeio-34.4.0/scanpipe/tests/data/jvm/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/jvm/common.java
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/jvm/no-package.java
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.063572 scancodeio-34.4.0/scanpipe/tests/data/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/manifests/Django-4.0.8-py3-none-any.whl.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11.pom.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25761 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11_scan_package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/manifests/package.expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/manifests/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/manifests/poor_values.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/manifests/python-inspector-0.10.0.zip
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/manifests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/manifests/toml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/manifests/toml.spdx.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:24.963572 scancodeio-34.4.0/scanpipe/tests/data/matchcode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.063572 scancodeio-34.4.0/scanpipe/tests/data/matchcode/match_to_matchcode/
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/matchcode/match_to_matchcode/codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_check_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_results_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_post_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    32504 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/notice.NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.063572 scancodeio-34.4.0/scanpipe/tests/data/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    24930 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/outputs/expected_attribution.html
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/outputs/render_me.html
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/policies.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.063572 scancodeio-34.4.0/scanpipe/tests/data/scancode/
+-rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/scancode/package_assembly_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/scancode/package_assembly_codebase.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.063572 scancodeio-34.4.0/scanpipe/tests/data/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/settings/scancode-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.067572 scancodeio-34.4.0/scanpipe/tests/data/spdx/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/spdx/example-2.3.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18944 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/data/windows-container-rootfs.tar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.067572 scancodeio-34.4.0/scanpipe/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipelines/do_nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipelines/profile_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipelines/raise_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipelines/register_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipelines/steps_as_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipelines/with_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:25.071572 scancodeio-34.4.0/scanpipe/tests/pipes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_codebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_cyclonedx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58850 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_d2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_js.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_matchcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28754 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_pathmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_purldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10331 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_scancode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_source_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15580 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_spdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/pipes/test_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/regen_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45134 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36517 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109259 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52454 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/test_scancodeio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46619 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73008 2024-04-22 09:30:21.000000 scancodeio-34.4.0/scanpipe/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-22 09:30:25.071572 scancodeio-34.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1297 2024-04-22 09:30:21.000000 scancodeio-34.4.0/setup.py
```

### Comparing `scancodeio-34.3.0/.github/workflows/ci.yml` & `scancodeio-34.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/.github/workflows/publish-docker.yml` & `scancodeio-34.4.0/.github/workflows/publish-docker.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/.github/workflows/pypi-release.yml` & `scancodeio-34.4.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/.gitignore` & `scancodeio-34.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/.readthedocs.yaml` & `scancodeio-34.4.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/CHANGELOG.rst` & `scancodeio-34.4.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,34 @@
 Changelog
 =========
 
+v34.4.0 (2024-04-22)
+--------------------
+
+- Upgrade Gunicorn to v22.0.0 security release.
+
+- Display the list of fields available for the advanced search syntax in the modal UI.
+  https://github.com/nexB/scancode.io/issues/1164
+
+- Add support for CycloneDX 1.6 outputs and inputs.
+  Also, the CycloneDX outputs can be downloaded as 1.6, 1.5, and 1.4 spec versions.
+  https://github.com/nexB/scancode.io/pull/1165
+
+- Update matchcode-toolkit to v4.1.0
+
+- Add a new function
+  `scanpipe.pipes.matchcode.fingerprint_codebase_resources()`, which computes
+  approximate file matching fingerprints for text files using the new
+  `get_file_fingerprint_hashes` function from matchcode-toolkit.
+
+- Rename the `purldb-scan-queue-worker` management command to `purldb-scan-worker`.
+
+- Add `docker-compose.purldb-scan-worker.yml` to run ScanCode.io as a PurlDB
+  scan worker service.
+
 v34.3.0 (2024-04-10)
 --------------------
 
 - Associate resolved packages with their source codebase resource.
   https://github.com/nexB/scancode.io/issues/1140
 
 - Add a new `CollectSourceStrings` pipeline (addon) for collecting source string using
```

### Comparing `scancodeio-34.3.0/Dockerfile` & `scancodeio-34.4.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/LICENSE` & `scancodeio-34.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/Makefile` & `scancodeio-34.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/NOTICE` & `scancodeio-34.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/PKG-INFO` & `scancodeio-34.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scancodeio
-Version: 34.3.0
+Version: 34.4.0
 Summary: Automate software composition analysis pipelines
 Home-page: https://github.com/nexB/scancode.io
 Author: nexB Inc.
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: open source,scan,license,package,dependency,copyright,filetype,author,extract,licensing,scancode,scanpipe,docker,rootfs,vm,virtual machine,pipeline,code analysis,container
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,58 +18,58 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 License-File: LICENSE
 License-File: NOTICE
 License-File: scan.NOTICE
 Requires-Dist: importlib-metadata==7.1.0
-Requires-Dist: setuptools==69.2.0
-Requires-Dist: Django==5.0.3
+Requires-Dist: setuptools==69.5.1
+Requires-Dist: Django==5.0.4
 Requires-Dist: django-environ==0.11.2
 Requires-Dist: django-crispy-forms==2.1
 Requires-Dist: crispy-bootstrap3==2024.1
 Requires-Dist: django-filter==24.2
 Requires-Dist: djangorestframework==3.15.1
 Requires-Dist: django-taggit==5.0.1
 Requires-Dist: psycopg[binary]==3.1.18
 Requires-Dist: django-probes==1.7.0
 Requires-Dist: rq==1.16.1
 Requires-Dist: django-rq==2.10.2
 Requires-Dist: redis==5.0.3
-Requires-Dist: gunicorn==21.2.0
+Requires-Dist: gunicorn==22.0.0
 Requires-Dist: container-inspector==32.0.1
 Requires-Dist: scancode-toolkit[packages]==32.1.0
 Requires-Dist: extractcode[full]==31.0.0
 Requires-Dist: commoncode==31.0.3
 Requires-Dist: fetchcode-container==1.2.3.210512; sys_platform == "linux"
 Requires-Dist: python-inspector==0.12.0
 Requires-Dist: elf-inspector==0.0.1
 Requires-Dist: source-inspector==0.3.0
 Requires-Dist: aboutcode-toolkit==10.1.0
 Requires-Dist: XlsxWriter==3.2.0
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: requests==2.31.0
-Requires-Dist: gitpython==3.1.42
+Requires-Dist: gitpython==3.1.43
 Requires-Dist: pyinstrument==4.6.2
-Requires-Dist: cyclonedx-python-lib==6.4.4
+Requires-Dist: cyclonedx-python-lib==7.3.0
 Requires-Dist: jsonschema==4.21.1
 Requires-Dist: fontawesomefree==6.5.1
-Requires-Dist: matchcode-toolkit==4.0.0
+Requires-Dist: matchcode-toolkit==4.1.0
 Requires-Dist: univers==30.11.0
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: bleach==6.1.0
 Provides-Extra: dev
 Requires-Dist: flake8==7.0.0; extra == "dev"
-Requires-Dist: black==24.3.0; extra == "dev"
+Requires-Dist: black==24.4.0; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
 Requires-Dist: doc8==1.1.1; extra == "dev"
 Requires-Dist: pydocstyle==6.3.0; extra == "dev"
 Requires-Dist: bandit==1.7.8; extra == "dev"
 Requires-Dist: django-debug-toolbar==4.3.0; extra == "dev"
-Requires-Dist: Sphinx==7.2.6; extra == "dev"
+Requires-Dist: Sphinx==7.3.7; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==2.0.0; extra == "dev"
 Requires-Dist: sphinx-rtd-dark-mode==1.3.0; extra == "dev"
 Requires-Dist: sphinxcontrib-django==2.5; extra == "dev"
 Requires-Dist: bumpver==2023.1129; extra == "dev"
 Requires-Dist: twine==5.0.0; extra == "dev"
 
 ScanCode.io
```

### Comparing `scancodeio-34.3.0/README.rst` & `scancodeio-34.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docker-compose-offline.yml` & `scancodeio-34.4.0/docker-compose-offline.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-version: "3"
-
 services:
   db:
     image: postgres:13
     env_file:
       - docker.env
     volumes:
       - db_data:/var/lib/postgresql/data/
```

### Comparing `scancodeio-34.3.0/docker-compose.yml` & `scancodeio-34.4.0/docker-compose.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-version: "3"
-
 services:
   db:
     image: postgres:13
     env_file:
       - docker.env
     volumes:
       - db_data:/var/lib/postgresql/data/
```

### Comparing `scancodeio-34.3.0/docs/Makefile` & `scancodeio-34.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/application-settings.rst` & `scancodeio-34.4.0/docs/application-settings.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/automation.rst` & `scancodeio-34.4.0/docs/automation.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/built-in-pipelines.rst` & `scancodeio-34.4.0/docs/built-in-pipelines.rst`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 .. autoclass:: scanpipe.pipelines.docker_windows.DockerWindows()
     :members:
     :member-order: bysource
 
 .. _pipeline_collect_source_strings:
 
 Collect Source Strings (addon)
---------------------------------
+------------------------------
 .. autoclass:: scanpipe.pipelines.collect_source_strings.CollectSourceStrings()
     :members:
     :member-order: bysource
 
 .. _pipeline_collect_symbols:
 
 Collect Codebase Symbols (addon)
```

### Comparing `scancodeio-34.3.0/docs/command-line-interface.rst` & `scancodeio-34.4.0/docs/command-line-interface.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/conf.py` & `scancodeio-34.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/contributing.rst` & `scancodeio-34.4.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/custom-pipelines.rst` & `scancodeio-34.4.0/docs/custom-pipelines.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/data-models.rst` & `scancodeio-34.4.0/docs/data-models.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/distros-os-images.rst` & `scancodeio-34.4.0/docs/distros-os-images.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/faq.rst` & `scancodeio-34.4.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/license-clarity-scan-summary.png` & `scancodeio-34.4.0/docs/images/license-clarity-scan-summary.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/output-files-download-results.png` & `scancodeio-34.4.0/docs/images/output-files-download-results.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/output-files-projects-list.png` & `scancodeio-34.4.0/docs/images/output-files-projects-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/output-files-xlsx-packages.png` & `scancodeio-34.4.0/docs/images/output-files-xlsx-packages.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/output-files-xlsx-resources.png` & `scancodeio-34.4.0/docs/images/output-files-xlsx-resources.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-extra-data.png` & `scancodeio-34.4.0/docs/images/tutorial-find-vulnerabilities-extra-data.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-icon-link.png` & `scancodeio-34.4.0/docs/images/tutorial-find-vulnerabilities-icon-link.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-find-vulnerabilities-packages-link.png` & `scancodeio-34.4.0/docs/images/tutorial-find-vulnerabilities-packages-link.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-license-policies-results.png` & `scancodeio-34.4.0/docs/images/tutorial-license-policies-results.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-web-ui-errors-list.png` & `scancodeio-34.4.0/docs/images/tutorial-web-ui-errors-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-web-ui-packages-charts.png` & `scancodeio-34.4.0/docs/images/tutorial-web-ui-packages-charts.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-web-ui-packages-list.png` & `scancodeio-34.4.0/docs/images/tutorial-web-ui-packages-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-web-ui-project-details.png` & `scancodeio-34.4.0/docs/images/tutorial-web-ui-project-details.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-web-ui-project-form.png` & `scancodeio-34.4.0/docs/images/tutorial-web-ui-project-form.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-web-ui-project-list.png` & `scancodeio-34.4.0/docs/images/tutorial-web-ui-project-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-web-ui-projects-list.png` & `scancodeio-34.4.0/docs/images/tutorial-web-ui-projects-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-web-ui-resources-charts.png` & `scancodeio-34.4.0/docs/images/tutorial-web-ui-resources-charts.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-web-ui-resources-filter.png` & `scancodeio-34.4.0/docs/images/tutorial-web-ui-resources-filter.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/tutorial-web-ui-run-log-modal.png` & `scancodeio-34.4.0/docs/images/tutorial-web-ui-run-log-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/user-interface-archive-action.png` & `scancodeio-34.4.0/docs/images/user-interface-archive-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/user-interface-archive-modal.png` & `scancodeio-34.4.0/docs/images/user-interface-archive-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/user-interface-create-project.png` & `scancodeio-34.4.0/docs/images/user-interface-create-project.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/user-interface-delete-action.png` & `scancodeio-34.4.0/docs/images/user-interface-delete-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/user-interface-delete-modal.png` & `scancodeio-34.4.0/docs/images/user-interface-delete-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/user-interface-project-details.png` & `scancodeio-34.4.0/docs/images/user-interface-project-details.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/user-interface-project-list-empty.png` & `scancodeio-34.4.0/docs/images/user-interface-project-list-empty.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/user-interface-project-list.png` & `scancodeio-34.4.0/docs/images/user-interface-project-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/user-interface-reset-action.png` & `scancodeio-34.4.0/docs/images/user-interface-reset-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/images/user-interface-reset-modal.png` & `scancodeio-34.4.0/docs/images/user-interface-reset-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/index.rst` & `scancodeio-34.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/installation.rst` & `scancodeio-34.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/introduction.rst` & `scancodeio-34.4.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/make.bat` & `scancodeio-34.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/output-files.rst` & `scancodeio-34.4.0/docs/output-files.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/project-configuration.rst` & `scancodeio-34.4.0/docs/project-configuration.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/rest-api.rst` & `scancodeio-34.4.0/docs/rest-api.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/scanpipe-concepts.rst` & `scancodeio-34.4.0/docs/scanpipe-concepts.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/scanpipe-pipes.rst` & `scancodeio-34.4.0/docs/scanpipe-pipes.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/tutorial_api_analyze_package_archive.rst` & `scancodeio-34.4.0/docs/tutorial_api_analyze_package_archive.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/tutorial_cli_analyze_codebase.rst` & `scancodeio-34.4.0/docs/tutorial_cli_analyze_codebase.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/tutorial_cli_analyze_docker_image.rst` & `scancodeio-34.4.0/docs/tutorial_cli_analyze_docker_image.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/tutorial_license_policies.rst` & `scancodeio-34.4.0/docs/tutorial_license_policies.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/tutorial_vulnerablecode_integration.rst` & `scancodeio-34.4.0/docs/tutorial_vulnerablecode_integration.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/tutorial_web_ui_analyze_docker_image.rst` & `scancodeio-34.4.0/docs/tutorial_web_ui_analyze_docker_image.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/tutorial_web_ui_review_scan_results.rst` & `scancodeio-34.4.0/docs/tutorial_web_ui_review_scan_results.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/docs/user-interface.rst` & `scancodeio-34.4.0/docs/user-interface.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/etc/nginx/examples/ssl.conf` & `scancodeio-34.4.0/etc/nginx/examples/ssl.conf`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/etc/thirdparty/apache-2.0.LICENSE` & `scancodeio-34.4.0/etc/thirdparty/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/etc/thirdparty/bsd-new.LICENSE` & `scancodeio-34.4.0/etc/thirdparty/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/etc/thirdparty/bsd-simplified.LICENSE` & `scancodeio-34.4.0/etc/thirdparty/bsd-simplified.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/etc/thirdparty/isc.LICENSE` & `scancodeio-34.4.0/etc/thirdparty/isc.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/etc/thirdparty/lgpl-2.1-plus.LICENSE` & `scancodeio-34.4.0/etc/thirdparty/lgpl-2.1-plus.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/etc/thirdparty/mit.LICENSE` & `scancodeio-34.4.0/etc/thirdparty/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/etc/thirdparty/python.LICENSE` & `scancodeio-34.4.0/etc/thirdparty/python.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/etc/thirdparty/virtualenv.pyz` & `scancodeio-34.4.0/etc/thirdparty/virtualenv.pyz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/etc/thirdparty/virtualenv.pyz.ABOUT` & `scancodeio-34.4.0/etc/thirdparty/virtualenv.pyz.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/__init__.py` & `scancodeio-34.4.0/scancodeio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import sys
 import warnings
 from contextlib import suppress
 from pathlib import Path
 
 import git
 
-VERSION = "34.3.0"
+VERSION = "34.4.0"
 
 PROJECT_DIR = Path(__file__).resolve().parent
 ROOT_DIR = PROJECT_DIR.parent
 SCAN_NOTICE = PROJECT_DIR.joinpath("scan.NOTICE").read_text()
 GITHUB_URL = "https://github.com/nexB/scancode.io"
```

### Comparing `scancodeio-34.3.0/scancodeio/auth.py` & `scancodeio-34.4.0/scancodeio/auth.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/context_processors.py` & `scancodeio-34.4.0/scancodeio/context_processors.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/settings.py` & `scancodeio-34.4.0/scancodeio/settings.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js` & `scancodeio-34.4.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/ace-1.20.0.min.js` & `scancodeio-34.4.0/scancodeio/static/ace-1.20.0.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/ace-1.9.5.min.js` & `scancodeio-34.4.0/scancodeio/static/ace-1.9.5.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/add-inputs.js` & `scancodeio-34.4.0/scancodeio/static/add-inputs.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/billboard-3.0.1-datalab.min.css` & `scancodeio-34.4.0/scancodeio/static/billboard-3.0.1-datalab.min.css`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/billboard-3.0.1.pkgd.min.js` & `scancodeio-34.4.0/scancodeio/static/billboard-3.0.1.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/bsd-new.LICENSE` & `scancodeio-34.4.0/scancodeio/static/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/bsd-simplified.LICENSE` & `scancodeio-34.4.0/scancodeio/static/bsd-simplified.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/bulma-0.9.4.min.css` & `scancodeio-34.4.0/scancodeio/static/bulma-0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT` & `scancodeio-34.4.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/bulma-toast-2.4.1.min.js` & `scancodeio-34.4.0/scancodeio/static/bulma-toast-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT` & `scancodeio-34.4.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/cc-by-4.0.LICENSE` & `scancodeio-34.4.0/scancodeio/static/cc-by-4.0.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/favicon.ico` & `scancodeio-34.4.0/scancodeio/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/highlight-10.6.0.css` & `scancodeio-34.4.0/scancodeio/static/highlight-10.6.0.css`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/highlight-10.6.0.min.js` & `scancodeio-34.4.0/scancodeio/static/highlight-10.6.0.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/html5sortable-0.9.17.min.js` & `scancodeio-34.4.0/scancodeio/static/html5sortable-0.9.17.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT` & `scancodeio-34.4.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/htmx-1.9.5.min.js` & `scancodeio-34.4.0/scancodeio/static/htmx-1.9.5.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/main.js` & `scancodeio-34.4.0/scancodeio/static/main.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/mit.LICENSE` & `scancodeio-34.4.0/scancodeio/static/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/static/ofl-1.1.LICENSE` & `scancodeio-34.4.0/scancodeio/static/ofl-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/urls.py` & `scancodeio-34.4.0/scancodeio/urls.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/worker.py` & `scancodeio-34.4.0/scancodeio/worker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio/wsgi.py` & `scancodeio-34.4.0/scancodeio/wsgi.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scancodeio.egg-info/SOURCES.txt` & `scancodeio-34.4.0/scancodeio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 LICENSE
 MANIFEST.in
 Makefile
 NOTICE
 README.rst
 docker-compose-offline.yml
 docker-compose.dev.yml
+docker-compose.purldb-scan-worker.yml
 docker-compose.yml
 docker.env
 manage.py
 scan.NOTICE
 setup.cfg
 setup.py
 .github/workflows/ci-docker.yml
@@ -141,15 +142,15 @@
 scanpipe/management/commands/archive-project.py
 scanpipe/management/commands/create-project.py
 scanpipe/management/commands/create-user.py
 scanpipe/management/commands/delete-project.py
 scanpipe/management/commands/execute.py
 scanpipe/management/commands/list-project.py
 scanpipe/management/commands/output.py
-scanpipe/management/commands/purldb-scan-queue-worker.py
+scanpipe/management/commands/purldb-scan-worker.py
 scanpipe/management/commands/reset-project.py
 scanpipe/management/commands/show-pipeline.py
 scanpipe/management/commands/status.py
 scanpipe/migrations/0001_initial.py
 scanpipe/migrations/0002_run_id_and_log.py
 scanpipe/migrations/0003_remove_run_run_id.py
 scanpipe/migrations/0004_run_pipeline_name.py
```

### Comparing `scancodeio-34.3.0/scanpipe/__init__.py` & `scancodeio-34.4.0/scanpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/api/__init__.py` & `scancodeio-34.4.0/scanpipe/api/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/api/serializers.py` & `scancodeio-34.4.0/scanpipe/api/serializers.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/api/views.py` & `scancodeio-34.4.0/scanpipe/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,23 +135,27 @@
         return project_results_json_response(self.get_object())
 
     @action(detail=True, name="Results (download)")
     def results_download(self, request, *args, **kwargs):
         """Return the results in the provided `output_format` as an attachment."""
         project = self.get_object()
         format = request.query_params.get("output_format", "json")
+        version = request.query_params.get("version")
+        output_kwargs = {}
 
         if format == "json":
             return project_results_json_response(project, as_attachment=True)
         elif format == "xlsx":
             output_file = output.to_xlsx(project)
         elif format == "spdx":
             output_file = output.to_spdx(project)
         elif format == "cyclonedx":
-            output_file = output.to_cyclonedx(project)
+            if version:
+                output_kwargs["version"] = version
+            output_file = output.to_cyclonedx(project, **output_kwargs)
         elif format == "attribution":
             output_file = output.to_attribution(project)
         else:
             message = {"status": f"Format {format} not supported."}
             return Response(message, status=status.HTTP_400_BAD_REQUEST)
 
         filename = output.safe_filename(f"scancodeio_{project.name}_{output_file.name}")
```

### Comparing `scancodeio-34.3.0/scanpipe/apps.py` & `scancodeio-34.4.0/scanpipe/apps.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/filters.py` & `scancodeio-34.4.0/scanpipe/filters.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/forms.py` & `scancodeio-34.4.0/scanpipe/forms.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/__init__.py` & `scancodeio-34.4.0/scanpipe/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/add-input.py` & `scancodeio-34.4.0/scanpipe/management/commands/add-input.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/add-pipeline.py` & `scancodeio-34.4.0/scanpipe/management/commands/add-pipeline.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/archive-project.py` & `scancodeio-34.4.0/scanpipe/management/commands/archive-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/create-project.py` & `scancodeio-34.4.0/scanpipe/management/commands/create-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/create-user.py` & `scancodeio-34.4.0/scanpipe/management/commands/create-user.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/delete-project.py` & `scancodeio-34.4.0/scanpipe/management/commands/delete-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/execute.py` & `scancodeio-34.4.0/scanpipe/management/commands/execute.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/list-project.py` & `scancodeio-34.4.0/scanpipe/management/commands/list-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/output.py` & `scancodeio-34.4.0/scanpipe/management/commands/output.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/purldb-scan-queue-worker.py` & `scancodeio-34.4.0/scanpipe/management/commands/purldb-scan-worker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/reset-project.py` & `scancodeio-34.4.0/scanpipe/management/commands/reset-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/show-pipeline.py` & `scancodeio-34.4.0/scanpipe/management/commands/show-pipeline.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/management/commands/status.py` & `scancodeio-34.4.0/scanpipe/management/commands/status.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0001_initial.py` & `scancodeio-34.4.0/scanpipe/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0002_run_id_and_log.py` & `scancodeio-34.4.0/scanpipe/migrations/0002_run_id_and_log.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0004_run_pipeline_name.py` & `scancodeio-34.4.0/scanpipe/migrations/0004_run_pipeline_name.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py` & `scancodeio-34.4.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py` & `scancodeio-34.4.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0008_package_extra_data.py` & `scancodeio-34.4.0/scanpipe/migrations/0008_package_extra_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0013_project_is_archived.py` & `scancodeio-34.4.0/scanpipe/migrations/0013_project_is_archived.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0014_webhooksubscription.py` & `scancodeio-34.4.0/scanpipe/migrations/0014_webhooksubscription.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py` & `scancodeio-34.4.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py` & `scancodeio-34.4.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0019_auto_20220804_1836.py` & `scancodeio-34.4.0/scanpipe/migrations/0019_auto_20220804_1836.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0022_create_discovereddependencies_model.py` & `scancodeio-34.4.0/scanpipe/migrations/0022_create_discovereddependencies_model.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0023_migrate_dependencies.py` & `scancodeio-34.4.0/scanpipe/migrations/0023_migrate_dependencies.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py` & `scancodeio-34.4.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py` & `scancodeio-34.4.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0028_codebaserelation_and_more.py` & `scancodeio-34.4.0/scanpipe/migrations/0028_codebaserelation_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py` & `scancodeio-34.4.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py` & `scancodeio-34.4.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py` & `scancodeio-34.4.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py` & `scancodeio-34.4.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0033_project_notes_project_settings.py` & `scancodeio-34.4.0/scanpipe/migrations/0033_project_notes_project_settings.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0035_set_projects_slug.py` & `scancodeio-34.4.0/scanpipe/migrations/0035_set_projects_slug.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0038_migrate_vulnerability_data.py` & `scancodeio-34.4.0/scanpipe/migrations/0038_migrate_vulnerability_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py` & `scancodeio-34.4.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0041_projectmessage.py` & `scancodeio-34.4.0/scanpipe/migrations/0041_projectmessage.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0042_projecterror_to_projectmessage_data.py` & `scancodeio-34.4.0/scanpipe/migrations/0042_projecterror_to_projectmessage_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0044_uuidtaggeditem_project_labels.py` & `scancodeio-34.4.0/scanpipe/migrations/0044_uuidtaggeditem_project_labels.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0045_scan_codebase_packages_data.py` & `scancodeio-34.4.0/scanpipe/migrations/0045_scan_codebase_packages_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0046_discoveredpackage_tag.py` & `scancodeio-34.4.0/scanpipe/migrations/0046_discoveredpackage_tag.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0048_inputsource.py` & `scancodeio-34.4.0/scanpipe/migrations/0048_inputsource.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0049_input_sources_data.py` & `scancodeio-34.4.0/scanpipe/migrations/0049_input_sources_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0051_rename_pipelines_data.py` & `scancodeio-34.4.0/scanpipe/migrations/0051_rename_pipelines_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0052_run_selected_groups.py` & `scancodeio-34.4.0/scanpipe/migrations/0052_run_selected_groups.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0053_restructure_pipelines_data.py` & `scancodeio-34.4.0/scanpipe/migrations/0053_restructure_pipelines_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0054_rename_pipeline.py` & `scancodeio-34.4.0/scanpipe/migrations/0054_rename_pipeline.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/migrations/0055_discoveredpackage_datafile_paths.py` & `scancodeio-34.4.0/scanpipe/migrations/0055_discoveredpackage_datafile_paths.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/models.py` & `scancodeio-34.4.0/scanpipe/models.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/__init__.py` & `scancodeio-34.4.0/scanpipe/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/collect_source_strings.py` & `scancodeio-34.4.0/scanpipe/pipelines/collect_source_strings.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/collect_symbols.py` & `scancodeio-34.4.0/scanpipe/pipelines/collect_symbols.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/deploy_to_develop.py` & `scancodeio-34.4.0/scanpipe/pipelines/deploy_to_develop.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/docker.py` & `scancodeio-34.4.0/scanpipe/pipelines/docker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/docker_windows.py` & `scancodeio-34.4.0/scanpipe/pipelines/docker_windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/find_vulnerabilities.py` & `scancodeio-34.4.0/scanpipe/pipelines/find_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/inspect_elf_binaries.py` & `scancodeio-34.4.0/scanpipe/pipelines/inspect_elf_binaries.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/inspect_packages.py` & `scancodeio-34.4.0/scanpipe/pipelines/inspect_packages.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/load_inventory.py` & `scancodeio-34.4.0/scanpipe/pipelines/load_inventory.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/load_sbom.py` & `scancodeio-34.4.0/scanpipe/pipelines/load_sbom.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/match_to_matchcode.py` & `scancodeio-34.4.0/scanpipe/pipelines/match_to_matchcode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/populate_purldb.py` & `scancodeio-34.4.0/scanpipe/pipelines/populate_purldb.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/resolve_dependencies.py` & `scancodeio-34.4.0/scanpipe/pipelines/resolve_dependencies.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/root_filesystem.py` & `scancodeio-34.4.0/scanpipe/pipelines/root_filesystem.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/scan_codebase.py` & `scancodeio-34.4.0/scanpipe/pipelines/scan_codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipelines/scan_single_package.py` & `scancodeio-34.4.0/scanpipe/pipelines/scan_single_package.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/__init__.py` & `scancodeio-34.4.0/scanpipe/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/codebase.py` & `scancodeio-34.4.0/scanpipe/pipes/codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/compliance.py` & `scancodeio-34.4.0/scanpipe/pipes/compliance.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/cyclonedx.py` & `scancodeio-34.4.0/scanpipe/pipes/cyclonedx.py`

 * *Files 6% similar despite different names*

```diff
@@ -174,14 +174,35 @@
 
 
 def get_components(bom):
     """Return list of components from CycloneDX BOM."""
     return list(bom._get_all_components())
 
 
+def delete_tools(cyclonedx_document_json):
+    """
+    Remove the ``tools`` section, if defined, from the SBOM as it can
+    be in the way of loading a SBOM that is valid regarding the spec, but fails the
+    deserialization.
+
+    The ``metadata.tools`` as an array was deprecated in 1.5 and replaced by an
+    object structure where you can define a list of ``components`` and ``services``.
+
+    The new structure is not yet supported by the cyclonedx-python-lib, neither for
+    serialization (output) nor deserialization (input).
+
+    The tools are not used anyway in the context of loading the SBOM component data as
+    packages.
+    """
+    if "tools" in cyclonedx_document_json.get("metadata", {}):
+        del cyclonedx_document_json["metadata"]["tools"]
+
+    return cyclonedx_document_json
+
+
 def resolve_cyclonedx_packages(input_location):
     """Resolve the packages from the `input_location` CycloneDX document file."""
     input_path = Path(input_location)
     document_data = input_path.read_text()
 
     if str(input_location).endswith(".xml"):
         cyclonedx_document = SafeElementTree.fromstring(document_data)
@@ -190,14 +211,15 @@
     elif str(input_location).endswith(".json"):
         cyclonedx_document = json.loads(document_data)
         if errors := validate_document(cyclonedx_document):
             error_msg = (
                 f'CycloneDX document "{input_path.name}" is not valid:\n{errors}'
             )
             raise ValueError(error_msg)
+        cyclonedx_document = delete_tools(cyclonedx_document)
         cyclonedx_bom = Bom.from_json(data=cyclonedx_document)
 
     else:
         return []
 
     components = get_components(cyclonedx_bom)
     return [cyclonedx_component_to_package_data(component) for component in components]
```

### Comparing `scancodeio-34.3.0/scanpipe/pipes/d2d.py` & `scancodeio-34.4.0/scanpipe/pipes/d2d.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/docker.py` & `scancodeio-34.4.0/scanpipe/pipes/docker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/elf.py` & `scancodeio-34.4.0/scanpipe/pipes/elf.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/fetch.py` & `scancodeio-34.4.0/scanpipe/pipes/fetch.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/flag.py` & `scancodeio-34.4.0/scanpipe/pipes/flag.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/input.py` & `scancodeio-34.4.0/scanpipe/pipes/input.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/js.py` & `scancodeio-34.4.0/scanpipe/pipes/js.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/jvm.py` & `scancodeio-34.4.0/scanpipe/pipes/jvm.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/matchcode.py` & `scancodeio-34.4.0/scanpipe/pipes/matchcode.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,19 +23,23 @@
 import logging
 from collections import defaultdict
 
 from django.conf import settings
 
 import requests
 from matchcode_toolkit.fingerprinting import compute_codebase_directory_fingerprints
+from matchcode_toolkit.fingerprinting import get_file_fingerprint_hashes
+from scancode import Scanner
 
 from scanpipe.pipes import codebase
 from scanpipe.pipes import flag
 from scanpipe.pipes import poll_until_success
 from scanpipe.pipes.output import to_json
+from scanpipe.pipes.scancode import _scan_resource
+from scanpipe.pipes.scancode import scan_resources
 
 
 class MatchCodeIOException(Exception):
     pass
 
 
 label = "MatchCode"
@@ -170,29 +174,86 @@
         fields=["extra_data"],
         batch_size=1000,
     )
 
 
 def fingerprint_codebase_directories(project, to_codebase_only=False):
     """
-    Compute directory fingerprints for the directories of the to/ codebase from
-    `project`.
+    Compute directory fingerprints for the directories from `project`.
 
     These directory fingerprints are used for matching purposes on matchcode.
+
+    If `to_codebase_only` is True, the only directories from the `to/` codebase
+    are computed.
     """
     resources = project.codebaseresources.all()
     if to_codebase_only:
         resources = resources.to_codebase()
     virtual_codebase = codebase.get_basic_virtual_codebase(resources)
     virtual_codebase = compute_codebase_directory_fingerprints(virtual_codebase)
     save_directory_fingerprints(
         project, virtual_codebase, to_codebase_only=to_codebase_only
     )
 
 
+def fingerprint_codebase_resource(location, with_threading=True, **kwargs):
+    """
+    Compute fingerprints for the resource at `location` using the
+    scancode-toolkit direct API.
+
+    Return a dictionary of scan `results` and a list of `errors`.
+    """
+    scanners = [
+        Scanner("fingerprints", get_file_fingerprint_hashes),
+    ]
+    return _scan_resource(location, scanners, with_threading=with_threading)
+
+
+def save_resource_fingerprints(resource, scan_results, scan_errors=None):
+    """
+    Save computed fingerprints from `scan_results` to `resource.extra_data`.
+    Create project errors if any occurred during the scan.
+    """
+    resource.extra_data.update(scan_results)
+    resource.save()
+
+    if scan_errors:
+        resource.add_errors(scan_errors)
+        resource.update(status=flag.SCANNED_WITH_ERROR)
+
+
+def fingerprint_codebase_resources(
+    project, resource_qs=None, progress_logger=None, to_codebase_only=False
+):
+    """
+    Compute fingerprints for the resources from `project`.
+
+    These resource fingerprints are used for matching purposes on matchcode.
+
+    Multiprocessing is enabled by default on this pipe, the number of processes can be
+    controlled through the SCANCODEIO_PROCESSES setting.
+
+    If `to_codebase_only` is True, the only resources from the `to/` codebase
+    are computed.
+    """
+    # Checking for None to make the distinction with an empty resource_qs queryset
+    if resource_qs is None:
+        resource_qs = project.codebaseresources.filter(is_text=True)
+
+    if to_codebase_only:
+        resource_qs = resource_qs.to_codebase()
+
+    scan_resources(
+        resource_qs=resource_qs,
+        scan_func=fingerprint_codebase_resource,
+        save_func=save_resource_fingerprints,
+        progress_logger=progress_logger,
+    )
+
+
 def send_project_json_to_matchcode(
     project, timeout=DEFAULT_TIMEOUT, api_url=MATCHCODEIO_API_URL
 ):
     """
     Given a `project`, create a JSON scan of the `project` CodebaseResources and
     send it to MatchCode.io for matching. Return a tuple containing strings of the url
     to the particular match run and the url to the match results.
```

### Comparing `scancodeio-34.3.0/scanpipe/pipes/output.py` & `scancodeio-34.4.0/scanpipe/pipes/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -708,20 +708,21 @@
     ordered_dict = {
         key: bom_as_dict.get(key) for key in order_from_schema if key in bom_as_dict
     }
 
     return json.dumps(ordered_dict, indent=2)
 
 
-def to_cyclonedx(project, schema_version=SchemaVersion.V1_5):
+def to_cyclonedx(project, version="1.6"):
     """
     Generate output for the provided ``project`` in CycloneDX BOM format.
     The output file is created in the ``project`` "output/" directory.
     Return the path of the generated output file.
     """
+    schema_version = SchemaVersion.from_version(version)
     output_file = project.get_output_file_path("results", "cdx.json")
 
     bom = get_cyclonedx_bom(project)
     json_outputter = make_outputter(bom, OutputFormat.JSON, schema_version)
 
     # Using the internal API in place of the output_as_string() method to avoid
     # a round of deserialization/serialization while fixing the field ordering.
```

### Comparing `scancodeio-34.3.0/scanpipe/pipes/pathmap.py` & `scancodeio-34.4.0/scanpipe/pipes/pathmap.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/purldb.py` & `scancodeio-34.4.0/scanpipe/pipes/purldb.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/resolve.py` & `scancodeio-34.4.0/scanpipe/pipes/resolve.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/rootfs.py` & `scancodeio-34.4.0/scanpipe/pipes/rootfs.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/scancode.py` & `scancodeio-34.4.0/scanpipe/pipes/scancode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/schemas/spdx-schema-2.3.json` & `scancodeio-34.4.0/scanpipe/pipes/schemas/spdx-schema-2.3.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/schemas/spdx-schema-2.3.json.ABOUT` & `scancodeio-34.4.0/scanpipe/pipes/schemas/spdx-schema-2.3.json.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/source_strings.py` & `scancodeio-34.4.0/scanpipe/pipes/source_strings.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/spdx.py` & `scancodeio-34.4.0/scanpipe/pipes/spdx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/symbols.py` & `scancodeio-34.4.0/scanpipe/pipes/symbols.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/vulnerablecode.py` & `scancodeio-34.4.0/scanpipe/pipes/vulnerablecode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/pipes/windows.py` & `scancodeio-34.4.0/scanpipe/pipes/windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tasks.py` & `scancodeio-34.4.0/scanpipe/tasks.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/account/profile.html` & `scancodeio-34.4.0/scanpipe/templates/account/profile.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/registration/login.html` & `scancodeio-34.4.0/scanpipe/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/rest_framework/api.html` & `scancodeio-34.4.0/scanpipe/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/app_monitoring.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/app_monitoring.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/attribution.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/attribution.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/base.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/base.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/dependency_detail.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/dependency_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/dependency_list.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/dependency_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/list_actions_dropdown.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/dropdowns/list_actions_dropdown.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/dropdowns/project_actions_dropdown.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/dropdowns/project_actions_dropdown.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/breadcrumb.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/file_filter.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/file_filter.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/list_view_thead.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/list_view_thead.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/navbar_header.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/navbar_header.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination_header.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/pagination_header.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/pagination_header_relations.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/pagination_header_relations.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_clone_form.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/project_clone_form.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_list_table.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/project_list_table.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/project_summary_level.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/project_summary_level.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/resource_path_links.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/resource_path_links.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/run_status_tag.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/run_status_tag.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/includes/search_field.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/includes/search_field.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/license_detail.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/license_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/license_list.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/license_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/message_list.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/message_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_inputs_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/add_inputs_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_labels_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/add_labels_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/add_pipeline_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/add_pipeline_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/clone_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/clone_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/edit_input_tag_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/edit_input_tag_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal_content.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/pipeline_help_modal_content.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_archive_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/project_archive_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_delete_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/project_delete_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_inputs_delete_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/project_inputs_delete_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/project_reset_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/project_reset_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_archive_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/projects_archive_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_delete_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/projects_delete_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/projects_reset_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/projects_reset_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/run_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/run_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/run_modal_content.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/run_modal_content.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/modals/search_syntax_modal.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/modals/search_syntax_modal.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,70 @@
 <div class="modal" id="search-syntax-modal">
   <div class="modal-background"></div>
   <div class="modal-card">
     <header class="modal-card-head">
-      <p class="modal-card-title">Search syntax</p>
+      <p class="modal-card-title">Search {{ filter.verbose_name_plural }}</p>
       <button class="delete" aria-label="close"></button>
     </header>
-    <section class="modal-card-body px-2">
+    <div class="modal-card-body p-2 pb-4">
       <div class="content">
-        <ul class="mt-0">
-          <li>
-            <strong>Single Term:</strong> Enter a single word to search for exact matches.<br>
-            Example: <code>file.txt</code>
-          </li>
-          <li>
-            <strong>Quoted Phrases:</strong> Use double quotes to search for exact phrases.<br>
-            Example: <code>"name version"</code>
-          </li>
-          <li>
-            <strong>Field Searches:</strong> Specify fields to narrow down your search.<br>
-            Use <code>field_name:</code> followed by your search term.<br>
-            Example: <code>name:file.txt</code></li>
-          <li>
-            <strong>Negation:</strong> Use a hyphen (-) before a field name to exclude results.<br>
-            Example: <code>-name:file.txt</code></li>
-          <li>
-            <strong>Lookup Types:</strong> Use lookup types to perform specific searches.
-            <ul>
-              <li><code>=</code>: Exact match</li>
-              <li><code>^</code>: Starts with</li>
-              <li><code>$</code>: Ends with</li>
-              <li><code>~</code>: Contains</li>
-              <li><code>&gt;</code>: Greater than</li>
-              <li><code>&lt;</code>: Less than</li>
-            </ul>
-            Example: <code>path^:dir1</code>
-          </li>
-          <li>
-            <strong>Multiple queries</strong> are combined with the <code>AND</code> operator.<br>
-            Example: <code>name:file.txt status:scanned</code>
-          </li>
-        </ul>
+        <div class="tabs is-boxed mb-4">
+          <ul class="m-0">
+            <li class="is-active">
+              <a data-target="tab-syntax" >Syntax</a>
+            </li>
+            <li>
+              <a data-target="tab-fields">Fields</a>
+            </li>
+          </ul>
+        </div>
+        <section id="tab-syntax" class="tab-content is-active">
+          <ul class="mt-0">
+            <li>
+              <strong>Single Term:</strong> Enter a single word to search for exact matches.<br>
+              Example: <code>file.txt</code>
+            </li>
+            <li>
+              <strong>Quoted Phrases:</strong> Use double quotes to search for exact phrases.<br>
+              Example: <code>"name version"</code>
+            </li>
+            <li>
+              <strong>Field Searches:</strong> Specify fields to narrow down your search.<br>
+              Use <code>field_name:</code> followed by your search term.<br>
+              Example: <code>name:file.txt</code></li>
+            <li>
+              <strong>Negation:</strong> Use a hyphen (-) before a field name to exclude results.<br>
+              Example: <code>-name:file.txt</code></li>
+            <li>
+              <strong>Lookup Types:</strong> Use lookup types to perform specific searches.
+              <ul>
+                <li><code>=</code>: Exact match</li>
+                <li><code>^</code>: Starts with</li>
+                <li><code>$</code>: Ends with</li>
+                <li><code>~</code>: Contains</li>
+                <li><code>&gt;</code>: Greater than</li>
+                <li><code>&lt;</code>: Less than</li>
+              </ul>
+              Example: <code>path^:dir1</code>
+            </li>
+            <li>
+              <strong>Multiple queries</strong> are combined with the <code>AND</code> operator.<br>
+              Example: <code>name:file.txt status:scanned</code>
+            </li>
+          </ul>
+        </section>
+        <section id="tab-fields" class="tab-content">
+          <ul style="columns: 2;-webkit-columns: 2;-moz-columns: 2;">
+            {% for field_name in searchable_fields %}
+              <li>
+                <code>{{ field_name }}</code>
+              </li>
+            {% endfor %}
+          </ul>
+        </section>
       </div>
-    </section>
+    </div>
     <footer class="modal-card-foot is-flex is-justify-content-space-between">
       <button class="button">Close</button>
     </footer>
   </div>
 </div>
```

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/package_detail.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/package_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/package_list.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/package_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/license_clarity_panel.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/license_clarity_panel.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_codebase.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/project_codebase.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_inputs.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/project_inputs.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_outputs.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/project_outputs.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/project_pipelines.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/project_pipelines.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/resource_license_summary.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/resource_license_summary.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/resource_status_summary.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/resource_status_summary.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/panels/scan_summary_panel.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/panels/scan_summary_panel.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/project_charts.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/project_charts.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/project_detail.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/project_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/project_form.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/project_form.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/project_list.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/project_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/project_settings.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/project_settings.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/relation_list.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/relation_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/resource_detail.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/resource_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/resource_list.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/resource_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_detections.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_detections.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_packages.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_packages.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_purldb_content.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_purldb_content.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_relations.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_relations.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_resources.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_resources.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/templates/scanpipe/tabset/tabset.html` & `scancodeio-34.4.0/scanpipe/templates/scanpipe/tabset/tabset.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/__init__.py` & `scancodeio-34.4.0/scanpipe/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/alpine_3_15_4.tar.gz` & `scancodeio-34.4.0/scanpipe/tests/data/alpine_3_15_4.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json` & `scancodeio-34.4.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/archive.zip` & `scancodeio-34.4.0/scanpipe/tests/data/archive.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl` & `scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json` & `scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json` & `scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json` & `scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json` & `scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json` & `scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_tree.json` & `scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_tree.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json` & `scancodeio-34.4.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/basic-rootfs.tar.gz` & `scancodeio-34.4.0/scanpipe/tests/data/basic-rootfs.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json` & `scancodeio-34.4.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/centos.tar.gz` & `scancodeio-34.4.0/scanpipe/tests/data/centos.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/centos_scan_codebase.json` & `scancodeio-34.4.0/scanpipe/tests/data/centos_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json` & `scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.6.schema.json'", "'specVersion'": "'1.6'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.5.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.6.schema.json",
     "bomFormat": "CycloneDX",
     "components": [
         {
             "bom-ref": "pkg:pypi/asgiref@3.3.0?uuid=90cd6d93-1c46-477a-bd4a-47aa6b3ce773",
             "copyright": "",
             "description": "ASGI specs, helper code, and adapters\nasgiref\n=======\n\n.. image:: https://api.travis-ci.org/django/asgiref.svg\n    :target: https://travis-ci.org/django/asgiref\n\n.. image:: https://img.shields.io/pypi/v/asgiref.svg\n    :target: https://pypi.python.org/pypi/asgiref\n\nASGI is a standard for Python asynchronous web apps and servers to communicate\nwith each other, and positioned as an asynchronous successor to WSGI. You can\nread more at https://asgi.readthedocs.io/en/latest/\n\nThis package includes ASGI base libraries, such as:\n\n* Sync-to-async and async-to-sync function wrappers, ``asgiref.sync``\n* Server base classes, ``asgiref.server``\n* A WSGI-to-ASGI adapter, in ``asgiref.wsgi``\n\n\nFunction wrappers\n-----------------\n\nThese allow you to wrap or decorate async or sync functions to call them from\nthe other style (so you can call async functions from a synchronous thread,\nor vice-versa).\n\nIn particular:\n\n* AsyncToSync lets a synchronous subthread stop and wait while the async\n  function is called on the main thread's event loop, and then control is\n  returned to the thread when the async function is finished.\n\n* SyncToAsync lets async code call a synchronous function, which is run in\n  a threadpool and control returned to the async coroutine when the synchronous\n  function completes.\n\nThe idea is to make it easier to call synchronous APIs from async code and\nasynchronous APIs from synchronous code so it's easier to transition code from\none style to the other. In the case of Channels, we wrap the (synchronous)\nDjango view system with SyncToAsync to allow it to run inside the (asynchronous)\nASGI server.\n\nNote that exactly what threads things run in is very specific, and aimed to\nkeep maximum compatibility with old synchronous code. See\n\"Synchronous code & Threads\" below for a full explanation. By default,\n``sync_to_async`` will run all synchronous code in the program in the same\nthread for safety reasons; you can disable this for more performance with\n``@sync_to_async(thread_sensitive=False)``, but make sure that your code does\nnot rely on anything bound to threads (like database connections) when you do.\n\n\nThreadlocal replacement\n-----------------------\n\nThis is a drop-in replacement for ``threading.local`` that works with both\nthreads and asyncio Tasks. Even better, it will proxy values through from a\ntask-local context to a thread-local context when you use ``sync_to_async``\nto run things in a threadpool, and vice-versa for ``async_to_sync``.\n\nIf you instead want true thread- and task-safety, you can set\n``thread_critical`` on the Local object to ensure this instead.\n\n\nServer base classes\n-------------------\n\nIncludes a ``StatelessServer`` class which provides all the hard work of\nwriting a stateless server (as in, does not handle direct incoming sockets\nbut instead consumes external streams or sockets to work out what is happening).\n\nAn example of such a server would be a chatbot server that connects out to\na central chat server and provides a \"connection scope\" per user chatting to\nit. There's only one actual connection, but the server has to separate things\ninto several scopes for easier writing of the code.\n\nYou can see an example of this being used in `frequensgi <https://github.com/andrewgodwin/frequensgi>`_.\n\n\nWSGI-to-ASGI adapter\n--------------------\n\nAllows you to wrap a WSGI application so it appears as a valid ASGI application.\n\nSimply wrap it around your WSGI application like so::\n\n    asgi_application = WsgiToAsgi(wsgi_application)\n\nThe WSGI application will be run in a synchronous threadpool, and the wrapped\nASGI application will be one that accepts ``http`` class messages.\n\nPlease note that not all extended features of WSGI may be supported (such as\nfile handles for incoming POST bodies).\n\n\nDependencies\n------------\n\n``asgiref`` requires Python 3.5 or higher.\n\n\nContributing\n------------\n\nPlease refer to the\n`main Channels contributing docs <https://github.com/django/channels/blob/master/CONTRIBUTING.rst>`_.\n\n\nTesting\n'''''''\n\nTo run tests, make sure you have installed the ``tests`` extra with the package::\n\n    cd asgiref/\n    pip install -e .[tests]\n    pytest\n\n\nBuilding the documentation\n''''''''''''''''''''''''''\n\nThe documentation uses `Sphinx <http://www.sphinx-doc.org>`_::\n\n    cd asgiref/docs/\n    pip install sphinx\n\nTo build the docs, you can use the default tools::\n\n    sphinx-build -b html . _build/html  # or `make html`, if you've got make set up\n    cd _build/html\n    python -m http.server\n\n...or you can use ``sphinx-autobuild`` to run a server and rebuild/reload\nyour documentation changes automatically::\n\n    pip install sphinx-autobuild\n    sphinx-autobuild . _build/html\n\n\nImplementation Details\n----------------------\n\nSynchronous code & threads\n''''''''''''''''''''''''''\n\nThe ``asgiref.sync`` module provides two wrappers that let you go between\nasynchronous and synchronous code at will, while taking care of the rough edges\nfor you.\n\nUnfortunately, the rough edges are numerous, and the code has to work especially\nhard to keep things in the same thread as much as possible. Notably, the\nrestrictions we are working with are:\n\n* All synchronous code called through ``SyncToAsync`` and marked with\n  ``thread_sensitive`` should run in the same thread as each other (and if the\n  outer layer of the program is synchronous, the main thread)\n\n* If a thread already has a running async loop, ``AsyncToSync`` can't run things\n  on that loop if it's blocked on synchronous code that is above you in the\n  call stack.\n\nThe first compromise you get to might be that ``thread_sensitive`` code should\njust run in the same thread and not spawn in a sub-thread, fulfilling the first\nrestriction, but that immediately runs you into the second restriction.\n\nThe only real solution is to essentially have a variant of ThreadPoolExecutor\nthat executes any ``thread_sensitive`` code on the outermost synchronous\nthread - either the main thread, or a single spawned subthread.\n\nThis means you now have two basic states:\n\n* If the outermost layer of your program is synchronous, then all async code\n  run through ``AsyncToSync`` will run in a per-call event loop in arbitary\n  sub-threads, while all ``thread_sensitive`` code will run in the main thread.\n\n* If the outermost layer of your program is asynchronous, then all async code\n  runs on the main thread's event loop, and all ``thread_sensitive`` synchronous\n  code will run in a single shared sub-thread.\n\nCruicially, this means that in both cases there is a thread which is a shared\nresource that all ``thread_sensitive`` code must run on, and there is a chance\nthat this thread is currently blocked on its own ``AsyncToSync`` call. Thus,\n``AsyncToSync`` needs to act as an executor for thread code while it's blocking.\n\nThe ``CurrentThreadExecutor`` class provides this functionality; rather than\nsimply waiting on a Future, you can call its ``run_until_future`` method and\nit will run submitted code until that Future is done. This means that code\ninside the call can then run code on your thread.\n\n\nMaintenance and Security\n------------------------\n\nTo report security issues, please contact security@djangoproject.com. For GPG\nsignatures and more security process information, see\nhttps://docs.djangoproject.com/en/dev/internals/security/.\n\nTo report bugs or request new features, please open a new GitHub issue.\n\nThis repository is part of the Channels project. For the shepherd and maintenance team, please see the\n`main Channels readme <https://github.com/django/channels/blob/master/README.rst>`_.",
             "externalReferences": [
@@ -118,15 +118,15 @@
             {
                 "name": "ScanCode.io",
                 "version": "0.0.0"
             }
         ]
     },
     "serialNumber": "urn:uuid:b74fe5df-e965-415e-ba65-f38421a0695d",
-    "specVersion": "1.5",
+    "specVersion": "1.6",
     "version": 1,
     "vulnerabilities": [
         {
             "affects": [
                 {
                     "ref": "urn:cdx:pkg:pypi/asgiref@3.3.0?uuid=fb05a7ee-1078-4d60-bf71-2ba031414f1c"
                 }
```

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json` & `scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/django-4.0.10-vulnerability.json` & `scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/django-4.0.10-vulnerability.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/django-4.0.10_as_cdx.json` & `scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/django-4.0.10_as_cdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.2.json` & `scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.2.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.3.json` & `scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.3.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.json` & `scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.xml` & `scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/laravel-7.12.0/bom.1.4.xml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/missing_schema.json` & `scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/missing_schema.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/cyclonedx/nested.cdx.json` & `scancodeio-34.4.0/scanpipe/tests/data/cyclonedx/nested.cdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/expected.json` & `scancodeio-34.4.0/scanpipe/tests/data/d2d/about_files/expected.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip` & `scancodeio-34.4.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip` & `scancodeio-34.4.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip` & `scancodeio-34.4.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip` & `scancodeio-34.4.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/license_mit.md` & `scancodeio-34.4.0/scanpipe/tests/data/d2d/legal/license_mit.md`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/project.LICENSE` & `scancodeio-34.4.0/scanpipe/tests/data/d2d/legal/project.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d/legal/project_notice.txt` & `scancodeio-34.4.0/scanpipe/tests/data/d2d/legal/project_notice.txt`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/from/main.js` & `scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/from/main.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/from/unmain.js` & `scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/from/unmain.js`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/main.js.map` & `scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/to/main.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map` & `scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map` & `scancodeio-34.4.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl` & `scancodeio-34.4.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json` & `scancodeio-34.4.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/debian.tar.gz` & `scancodeio-34.4.0/scanpipe/tests/data/debian.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/debian_scan_codebase.json` & `scancodeio-34.4.0/scanpipe/tests/data/debian_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html` & `scancodeio-34.4.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz` & `scancodeio-34.4.0/scanpipe/tests/data/docker-images.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json` & `scancodeio-34.4.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json` & `scancodeio-34.4.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz` & `scancodeio-34.4.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json` & `scancodeio-34.4.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz` & `scancodeio-34.4.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json` & `scancodeio-34.4.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/flume-ng-node-d2d-input.json` & `scancodeio-34.4.0/scanpipe/tests/data/flume-ng-node-d2d-input.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/flume-ng-node-d2d.json` & `scancodeio-34.4.0/scanpipe/tests/data/flume-ng-node-d2d.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/foobar.qcow2.tar.gz` & `scancodeio-34.4.0/scanpipe/tests/data/foobar.qcow2.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz` & `scancodeio-34.4.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json` & `scancodeio-34.4.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar` & `scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar` & `scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json` & `scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json` & `scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json` & `scancodeio-34.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0.tgz` & `scancodeio-34.4.0/scanpipe/tests/data/is-npm-1.0.0.tgz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json` & `scancodeio-34.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json` & `scancodeio-34.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json` & `scancodeio-34.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/javascript_collect_symbols.json` & `scancodeio-34.4.0/scanpipe/tests/data/javascript_collect_symbols.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/jvm/common.java` & `scancodeio-34.4.0/scanpipe/tests/data/jvm/common.java`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11.pom.xml` & `scancodeio-34.4.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11.pom.xml`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11_scan_package.json` & `scancodeio-34.4.0/scanpipe/tests/data/manifests/openpdf-parent-1.3.11_scan_package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/manifests/package.expected.json` & `scancodeio-34.4.0/scanpipe/tests/data/manifests/package.expected.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/manifests/package.json` & `scancodeio-34.4.0/scanpipe/tests/data/manifests/package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/manifests/python-inspector-0.10.0.zip` & `scancodeio-34.4.0/scanpipe/tests/data/manifests/python-inspector-0.10.0.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/manifests/toml.json` & `scancodeio-34.4.0/scanpipe/tests/data/manifests/toml.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/manifests/toml.spdx.json` & `scancodeio-34.4.0/scanpipe/tests/data/manifests/toml.spdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/codebase.json` & `scancodeio-34.4.0/scanpipe/tests/data/matchcode/match_to_matchcode/codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_check_response.json` & `scancodeio-34.4.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_check_response.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_results_response.json` & `scancodeio-34.4.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_get_results_response.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_post_response.json` & `scancodeio-34.4.0/scanpipe/tests/data/matchcode/match_to_matchcode/request_post_response.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz` & `scancodeio-34.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json` & `scancodeio-34.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json` & `scancodeio-34.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/notice.NOTICE` & `scancodeio-34.4.0/scanpipe/tests/data/notice.NOTICE`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx` & `scancodeio-34.4.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/outputs/expected_attribution.html` & `scancodeio-34.4.0/scanpipe/tests/data/outputs/expected_attribution.html`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json` & `scancodeio-34.4.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/scancode/package_assembly_codebase.json` & `scancodeio-34.4.0/scanpipe/tests/data/scancode/package_assembly_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/spdx/example-2.3.1.json` & `scancodeio-34.4.0/scanpipe/tests/data/spdx/example-2.3.1.json`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/data/windows-container-rootfs.tar` & `scancodeio-34.4.0/scanpipe/tests/data/windows-container-rootfs.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipelines/do_nothing.py` & `scancodeio-34.4.0/scanpipe/tests/pipelines/do_nothing.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipelines/profile_step.py` & `scancodeio-34.4.0/scanpipe/tests/pipelines/profile_step.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipelines/raise_exception.py` & `scancodeio-34.4.0/scanpipe/tests/pipelines/raise_exception.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipelines/register_from_file.py` & `scancodeio-34.4.0/scanpipe/tests/pipelines/register_from_file.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipelines/steps_as_attribute.py` & `scancodeio-34.4.0/scanpipe/tests/pipelines/steps_as_attribute.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipelines/with_groups.py` & `scancodeio-34.4.0/scanpipe/tests/pipelines/with_groups.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_codebase.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_cyclonedx.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_d2d.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_d2d.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_docker.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_docker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_fetch.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_fetch.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_flag.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_flag.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_input.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_input.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_js.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_js.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_jvm.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_jvm.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_matchcode.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_matchcode.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,18 @@
 from pathlib import Path
 from unittest import mock
 
 from django.core.management import call_command
 from django.test import TestCase
 
 from scanpipe.models import AbstractTaskFieldsModel
+from scanpipe.models import CodebaseResource
 from scanpipe.models import Project
 from scanpipe.pipes import matchcode
+from scanpipe.pipes.input import copy_input
 from scanpipe.tests import make_resource_file
 
 
 class MatchCodePipesTest(TestCase):
     data_location = Path(__file__).parent.parent / "data"
 
     def setUp(self):
@@ -307,7 +309,27 @@
             mock_request_get_results_return,
         ]
 
         run_url = "http://192.168.1.12/api/runs/52b2930d-6e85-4b3e-ba3e-17dd9a618650/"
         match_results = matchcode.get_match_results(run_url)
 
         self.assertEqual(mock_request_get_results_return, match_results)
+
+    def test_scanpipe_pipes_matchcode_fingerprint_codebase_resources(self):
+        copy_input(self.data_location / "notice.NOTICE", self.project1.codebase_path)
+        codebase_resource1 = CodebaseResource.objects.create(
+            project=self.project1, path="notice.NOTICE", is_text=True
+        )
+
+        # This resource should not have a fingerprint
+        copy_input(self.data_location / "is-npm-1.0.0.tgz", self.project1.codebase_path)
+        codebase_resource2 = CodebaseResource.objects.create(
+            project=self.project1, path="is-npm-1.0.0.tgz"
+        )
+
+        matchcode.fingerprint_codebase_resources(self.project1)
+        codebase_resource1.refresh_from_db()
+        codebase_resource2.refresh_from_db()
+
+        expected_extra_data = {"halo1": "ef420f7e84c8c74c691315f0a06ac4f0"}
+        self.assertEqual(expected_extra_data, codebase_resource1.extra_data)
+        self.assertFalse(codebase_resource2.extra_data)
```

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_output.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,21 @@
 
         expected_location = self.data_path / "cyclonedx/asgiref-3.3.0.cdx.json"
         if regen:
             expected_location.write_text(results)
 
         self.assertJSONEqual(results, expected_location.read_text())
 
+        output_file = output.to_cyclonedx(project=project, version="1.5")
+        results_json = json.loads(output_file.read_text())
+        self.assertEqual(
+            "http://cyclonedx.org/schema/bom-1.5.schema.json", results_json["$schema"]
+        )
+        self.assertEqual("1.5", results_json["specVersion"])
+
     def test_scanpipe_pipes_outputs_to_spdx(self):
         fixtures = self.data_path / "asgiref-3.3.0_fixtures.json"
         call_command("loaddata", fixtures, **{"verbosity": 0})
         project = Project.objects.get(name="asgiref")
 
         with self.assertNumQueries(8):
             output_file = output.to_spdx(project=project, include_files=True)
```

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_pathmap.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_pathmap.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_pipes.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_pipes.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_purldb.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_purldb.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_resolve.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_resolve.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_rootfs.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_rootfs.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_scancode.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_scancode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_source_strings.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_source_strings.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_spdx.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_spdx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_symbols.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_symbols.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/pipes/test_windows.py` & `scancodeio-34.4.0/scanpipe/tests/pipes/test_windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/regen_test_data.py` & `scancodeio-34.4.0/scanpipe/tests/regen_test_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/test_api.py` & `scancodeio-34.4.0/scanpipe/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,14 +536,26 @@
         self.assertEqual(expected, response["Content-Disposition"])
         self.assertEqual("application/json", response["Content-Type"])
 
         response_value = response.getvalue()
         results = json.loads(response_value)
         self.assertIn("$schema", sorted(results.keys()))
 
+        data = {
+            "output_format": "cyclonedx",
+            "version": "1.5",
+        }
+        response = self.csrf_client.get(url, data=data)
+        response_value = response.getvalue()
+        results = json.loads(response_value)
+        self.assertEqual(
+            "http://cyclonedx.org/schema/bom-1.5.schema.json", results["$schema"]
+        )
+        self.assertEqual("1.5", results["specVersion"])
+
         data = {"output_format": "xlsx"}
         response = self.csrf_client.get(url, data=data)
         expected = [
             "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
             "application/octet-stream",
         ]
         self.assertIn(response["Content-Type"], expected)
```

### Comparing `scancodeio-34.3.0/scanpipe/tests/test_apps.py` & `scancodeio-34.4.0/scanpipe/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/test_auth.py` & `scancodeio-34.4.0/scanpipe/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/test_commands.py` & `scancodeio-34.4.0/scanpipe/tests/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -623,15 +623,15 @@
 
         options = [
             "--max-loops",
             1,
         ]
         out = StringIO()
         with mock.patch("scanpipe.tasks.execute_pipeline_task", task_success):
-            call_command("purldb-scan-queue-worker", *options, stdout=out)
+            call_command("purldb-scan-worker", *options, stdout=out)
 
         out_value = out.getvalue()
         self.assertIn(
             "Project httpsregistrynpmjsorgasdf-asdf-122tgz-97627c6e created", out_value
         )
         self.assertIn("File(s) downloaded to the project inputs directory:", out_value)
         self.assertIn("asdf-1.2.2.tgz", out_value)
@@ -678,15 +678,15 @@
 
         options = [
             "--max-loops",
             1,
         ]
         out = StringIO()
         with mock.patch("scanpipe.tasks.execute_pipeline_task", task_failure):
-            call_command("purldb-scan-queue-worker", *options, stdout=out, stderr=out)
+            call_command("purldb-scan-worker", *options, stdout=out, stderr=out)
 
         out_value = out.getvalue()
         self.assertIn("Exception occured during scan project:", out_value)
         self.assertIn("Error during scan_single_package execution:", out_value)
         self.assertIn("Error log", out_value)
 
         mock_request_post.assert_called_once()
@@ -735,15 +735,15 @@
 
         options = [
             "--max-loops",
             2,
         ]
         out = StringIO()
         with mock.patch("scanpipe.tasks.execute_pipeline_task", task_failure):
-            call_command("purldb-scan-queue-worker", *options, stdout=out, stderr=out)
+            call_command("purldb-scan-worker", *options, stdout=out, stderr=out)
 
         out_value = out.getvalue()
         self.assertIn(
             "Project httpsregistrynpmjsorgasdf-asdf-122tgz-97627c6e created", out_value
         )
         self.assertIn(
             "Project httpsregistrynpmjsorgasdf-asdf-121tgz-0bbdcf88 created", out_value
```

### Comparing `scancodeio-34.3.0/scanpipe/tests/test_filters.py` & `scancodeio-34.4.0/scanpipe/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/test_forms.py` & `scancodeio-34.4.0/scanpipe/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/test_models.py` & `scancodeio-34.4.0/scanpipe/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/test_pipelines.py` & `scancodeio-34.4.0/scanpipe/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/test_scancodeio.py` & `scancodeio-34.4.0/scanpipe/tests/test_scancodeio.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/test_tasks.py` & `scancodeio-34.4.0/scanpipe/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/tests/test_views.py` & `scancodeio-34.4.0/scanpipe/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `scancodeio-34.3.0/scanpipe/urls.py` & `scancodeio-34.4.0/scanpipe/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,19 @@
     ),
     path(
         "pipeline/<str:pipeline_name>/help/",
         views.pipeline_help_view,
         name="pipeline_help",
     ),
     path(
+        "project/<slug:slug>/results/<str:format>/<str:version>/",
+        views.ProjectResultsView.as_view(),
+        name="project_results",
+    ),
+    path(
         "project/<slug:slug>/results/<str:format>/",
         views.ProjectResultsView.as_view(),
         name="project_results",
     ),
     path(
         "project/<slug:slug>/execute_pipelines/",
         views.execute_pipelines_view,
```

### Comparing `scancodeio-34.3.0/scanpipe/views.py` & `scancodeio-34.4.0/scanpipe/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,14 +493,22 @@
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
 
         query_dict = self.request.GET.copy()
         query_dict.pop(PAGE_VAR, None)
         context["url_params_without_page"] = query_dict.urlencode()
 
+        context["searchable_fields"] = sorted(
+            [
+                field.name
+                for field in self.model._meta.get_fields()
+                if not field.is_relation
+            ]
+        )
+
         return context
 
 
 class AccountProfileView(LoginRequiredMixin, generic.TemplateView):
     template_name = "account/profile.html"
 
 
@@ -1277,23 +1285,27 @@
 class ProjectResultsView(ConditionalLoginRequired, generic.DetailView):
     model = Project
 
     def get(self, request, *args, **kwargs):
         self.object = self.get_object()
         project = self.object
         format = self.kwargs["format"]
+        version = self.kwargs.get("version")
+        output_kwargs = {}
 
         if format == "json":
             return project_results_json_response(project, as_attachment=True)
         elif format == "xlsx":
             output_file = output.to_xlsx(project)
         elif format == "spdx":
             output_file = output.to_spdx(project)
         elif format == "cyclonedx":
-            output_file = output.to_cyclonedx(project)
+            if version:
+                output_kwargs["version"] = version
+            output_file = output.to_cyclonedx(project, **output_kwargs)
         elif format == "attribution":
             output_file = output.to_attribution(project)
         else:
             raise Http404("Format not supported.")
 
         filename = output.safe_filename(f"scancodeio_{project.name}_{output_file.name}")
```

### Comparing `scancodeio-34.3.0/setup.cfg` & `scancodeio-34.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scancodeio
-version = 34.3.0
+version = 34.4.0
 license = Apache-2.0
 description = Automate software composition analysis pipelines
 long_description = file:README.rst
 author = nexB Inc.
 author_email = info@aboutcode.org
 url = https://github.com/nexB/scancode.io
 classifiers = 
@@ -46,60 +46,60 @@
 [options]
 python_requires = >=3.10
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
 	importlib-metadata==7.1.0
-	setuptools==69.2.0
-	Django==5.0.3
+	setuptools==69.5.1
+	Django==5.0.4
 	django-environ==0.11.2
 	django-crispy-forms==2.1
 	crispy-bootstrap3==2024.1
 	django-filter==24.2
 	djangorestframework==3.15.1
 	django-taggit==5.0.1
 	psycopg[binary]==3.1.18
 	django-probes==1.7.0
 	rq==1.16.1
 	django-rq==2.10.2
 	redis==5.0.3
-	gunicorn==21.2.0
+	gunicorn==22.0.0
 	container-inspector==32.0.1
 	scancode-toolkit[packages]==32.1.0
 	extractcode[full]==31.0.0
 	commoncode==31.0.3
 	fetchcode-container==1.2.3.210512; sys_platform == "linux"
 	python-inspector==0.12.0
 	elf-inspector==0.0.1
 	source-inspector==0.3.0
 	aboutcode-toolkit==10.1.0
 	XlsxWriter==3.2.0
 	openpyxl==3.1.2
 	requests==2.31.0
-	gitpython==3.1.42
+	gitpython==3.1.43
 	pyinstrument==4.6.2
-	cyclonedx-python-lib==6.4.4
+	cyclonedx-python-lib==7.3.0
 	jsonschema==4.21.1
 	fontawesomefree==6.5.1
-	matchcode-toolkit==4.0.0
+	matchcode-toolkit==4.1.0
 	univers==30.11.0
 	markdown-it-py==3.0.0
 	bleach==6.1.0
 
 [options.extras_require]
 dev = 
 	flake8==7.0.0
-	black==24.3.0
+	black==24.4.0
 	isort==5.13.2
 	doc8==1.1.1
 	pydocstyle==6.3.0
 	bandit==1.7.8
 	django-debug-toolbar==4.3.0
-	Sphinx==7.2.6
+	Sphinx==7.3.7
 	sphinx-rtd-theme==2.0.0
 	sphinx-rtd-dark-mode==1.3.0
 	sphinxcontrib-django==2.5
 	bumpver==2023.1129
 	twine==5.0.0
 
 [options.entry_points]
@@ -137,15 +137,15 @@
 ignore = E203,W503
 
 [pydocstyle]
 ignore = D1,D203,D205,D212,D400,D415
 
 [bumpver]
 version_pattern = "MAJOR.MINOR.PATCH"
-current_version = "34.3.0"
+current_version = "34.4.0"
 
 [bumpver:file_patterns]
 setup.cfg = 
 	version = {version}
 	current_version = "{version}"
 scancodeio/__init__.py = {version}
```

### Comparing `scancodeio-34.3.0/setup.py` & `scancodeio-34.4.0/setup.py`

 * *Files identical despite different names*


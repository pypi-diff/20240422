# Comparing `tmp/cmcrameri-1.8.tar.gz` & `tmp/cmcrameri-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmcrameri-1.8.tar", last modified: Mon Jan 29 14:47:43 2024, max compression
+gzip compressed data, was "cmcrameri-1.9.tar", last modified: Mon Apr 22 08:23:37 2024, max compression
```

## Comparing `cmcrameri-1.8.tar` & `cmcrameri-1.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:47:43.171079 cmcrameri-1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:47:43.159079 cmcrameri-1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:47:43.159079 cmcrameri-1.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-29 14:47:26.000000 cmcrameri-1.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-29 14:47:26.000000 cmcrameri-1.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-01-29 14:47:26.000000 cmcrameri-1.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:47:43.159079 cmcrameri-1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-01-29 14:47:26.000000 cmcrameri-1.8/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-29 14:47:26.000000 cmcrameri-1.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-29 14:47:26.000000 cmcrameri-1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-29 14:47:26.000000 cmcrameri-1.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-01-29 14:47:26.000000 cmcrameri-1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-01-29 14:47:26.000000 cmcrameri-1.8/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-29 14:47:26.000000 cmcrameri-1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-01-29 14:47:43.171079 cmcrameri-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-01-29 14:47:26.000000 cmcrameri-1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:47:43.159079 cmcrameri-1.8/cmcrameri/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-29 14:47:43.000000 cmcrameri-1.8/cmcrameri/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:47:43.171079 cmcrameri-1.8/cmcrameri/cmaps/
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/acton.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/actonS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/bam.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/bamO.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/bamako.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/bamakoS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/batlow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/batlowK.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/batlowKS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/batlowS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/batlowW.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/batlowWS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/berlin.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/bilbao.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/bilbaoS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/broc.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/brocO.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/buda.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/budaS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/bukavu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/cork.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/corkO.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/davos.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/davosS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/devon.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/devonS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/fes.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/glasgow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/glasgowS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/grayC.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/grayCS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/hawaii.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/hawaiiS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/imola.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/imolaS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/lajolla.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/lajollaS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/lapaz.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/lapazS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/lipari.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/lipariS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/lisbon.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/managua.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/navia.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/naviaS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/nuuk.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/nuukS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/oleron.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/oslo.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/osloS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/roma.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/romaO.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/tofino.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/tokyo.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/tokyoS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/turku.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/turkuS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/vanimo.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/vik.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/cmaps/vikO.txt
--rw-r--r--   0 runner    (1001) docker     (127)   147292 2024-01-29 14:47:26.000000 cmcrameri-1.8/cmcrameri/colormaps.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 14:47:43.171079 cmcrameri-1.8/cmcrameri.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-01-29 14:47:43.000000 cmcrameri-1.8/cmcrameri.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-01-29 14:47:26.000000 cmcrameri-1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-29 14:47:26.000000 cmcrameri-1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 14:47:43.171079 cmcrameri-1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:23:37.961825 cmcrameri-1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:23:37.949825 cmcrameri-1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:23:37.949825 cmcrameri-1.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-22 08:23:25.000000 cmcrameri-1.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-22 08:23:25.000000 cmcrameri-1.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-22 08:23:25.000000 cmcrameri-1.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:23:37.949825 cmcrameri-1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-22 08:23:25.000000 cmcrameri-1.9/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-22 08:23:25.000000 cmcrameri-1.9/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-22 08:23:25.000000 cmcrameri-1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-22 08:23:25.000000 cmcrameri-1.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-22 08:23:25.000000 cmcrameri-1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-22 08:23:25.000000 cmcrameri-1.9/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-22 08:23:25.000000 cmcrameri-1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-22 08:23:37.961825 cmcrameri-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-22 08:23:25.000000 cmcrameri-1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:23:37.953825 cmcrameri-1.9/cmcrameri/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 08:23:37.000000 cmcrameri-1.9/cmcrameri/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:23:37.961825 cmcrameri-1.9/cmcrameri/cmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/acton.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/actonS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/bam.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/bamO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/bamako.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/bamakoS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/batlow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/batlowK.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/batlowKS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/batlowS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/batlowW.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/batlowWS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/berlin.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/bilbao.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/bilbaoS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/broc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/brocO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/buda.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/budaS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/bukavu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/cork.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/corkO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/davos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/davosS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/devon.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/devonS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/fes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/glasgow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/glasgowS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/grayC.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/grayCS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/hawaii.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/hawaiiS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/imola.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/imolaS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/lajolla.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/lajollaS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/lapaz.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/lapazS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/lipari.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/lipariS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/lisbon.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/managua.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/navia.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/naviaS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/nuuk.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/nuukS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/oleron.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/oslo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/osloS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/roma.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/romaO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/tofino.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/tokyo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/tokyoS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/turku.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/turkuS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/vanimo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/vik.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/cmaps/vikO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   147292 2024-04-22 08:23:25.000000 cmcrameri-1.9/cmcrameri/colormaps.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:23:37.961825 cmcrameri-1.9/cmcrameri.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-22 08:23:37.000000 cmcrameri-1.9/cmcrameri.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-22 08:23:25.000000 cmcrameri-1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 08:23:25.000000 cmcrameri-1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:23:37.961825 cmcrameri-1.9/setup.cfg
```

### Comparing `cmcrameri-1.8/.github/ISSUE_TEMPLATE/feature_request.md` & `cmcrameri-1.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/.github/workflows/pypi.yml` & `cmcrameri-1.9/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/.github/workflows/tests.yml` & `cmcrameri-1.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/.pre-commit-config.yaml` & `cmcrameri-1.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     - id: check-docstring-first
     - id: check-added-large-files
     - id: requirements-txt-fixer
     - id: file-contents-sorter
       files: requirements-dev.txt
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.1.9
+  rev: v0.3.5
   hooks:
     - id: ruff
 
 - repo: https://github.com/psf/black
-  rev: 23.12.1
+  rev: 24.3.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.9
   hooks:
@@ -34,15 +34,15 @@
   rev: v2.2.6
   hooks:
     - id: codespell
       args:
         - --ignore-words-list=buda
 
 - repo: https://github.com/tox-dev/pyproject-fmt
-  rev: "1.5.3"
+  rev: "1.7.0"
   hooks:
     - id: pyproject-fmt
       additional_dependencies: ["tox>=4.9"]
 
 - repo: https://github.com/aio-libs/sort-all
   rev: "v1.2.0"
   hooks:
```

### Comparing `cmcrameri-1.8/LICENSE.txt` & `cmcrameri-1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/PKG-INFO` & `cmcrameri-1.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmcrameri
-Version: 1.8
+Version: 1.9
 Summary: Perceptually uniform colormaps by Fabio Crameri
 Author-email: Callum Rollo <c.rollo@outlook.com>
 License: MIT License
         
         Colormaps in cmcrameri/cm/cmaps:
         Copyright (c) 2020 Fabio Crameri
         
@@ -25,15 +25,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: documentation, https://callumrollo.github.io/cmcrameri
+Project-URL: documentation, https://github.com/callumrollo/cmcrameri
 Project-URL: homepage, https://pypi.org/project/cmcrameri/
 Project-URL: repository, https://github.com/callumrollo/cmcrameri
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -43,29 +43,25 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: packaging
 
-![Python package](https://github.com/callumrollo/cmcrameri/workflows/Python%20package/badge.svg)
+# cmcrameri
 
-[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)]()
-[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)]()
-[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)]()
-[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)]()
-[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)]()
-[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)]()
-[![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)]()
 
-[![Downloads](https://pepy.tech/badge/cmcrameri)](https://pepy.tech/project/cmcrameri) (PyPI)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 
-[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/cmcrameri.svg)](https://anaconda.org/conda-forge/cmcrameri) (conda-forge)
+![python versions](https://img.shields.io/pypi/pyversions/cmcrameri.svg)
+
+![pypi](https://badge.fury.io/py/cmcrameri.svg) [![Downloads](https://pepy.tech/badge/cmcrameri)](https://pepy.tech/project/cmcrameri)
+
+![anaconda badge](https://anaconda.org/conda-forge/cmcrameri/badges/version.svg) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/cmcrameri.svg)](https://anaconda.org/conda-forge/cmcrameri)
 
-# cmcrameri
 
 This is a Python wrapper around Fabio Crameri's perceptually uniform colormaps.
 
 <https://www.fabiocrameri.ch/colourmaps/>
 
 All credit for creating the colormaps to Fabio.
 Any errors in the Python implementation of colormaps are my own.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cmcrameri-1.8/README.md` & `cmcrameri-1.9/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-![Python package](https://github.com/callumrollo/cmcrameri/workflows/Python%20package/badge.svg)
+# cmcrameri
 
-[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)]()
-[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)]()
-[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)]()
-[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)]()
-[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)]()
-[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)]()
-[![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)]()
 
-[![Downloads](https://pepy.tech/badge/cmcrameri)](https://pepy.tech/project/cmcrameri) (PyPI)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 
-[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/cmcrameri.svg)](https://anaconda.org/conda-forge/cmcrameri) (conda-forge)
+![python versions](https://img.shields.io/pypi/pyversions/cmcrameri.svg)
+
+![pypi](https://badge.fury.io/py/cmcrameri.svg) [![Downloads](https://pepy.tech/badge/cmcrameri)](https://pepy.tech/project/cmcrameri)
+
+![anaconda badge](https://anaconda.org/conda-forge/cmcrameri/badges/version.svg) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/cmcrameri.svg)](https://anaconda.org/conda-forge/cmcrameri)
 
-# cmcrameri
 
 This is a Python wrapper around Fabio Crameri's perceptually uniform colormaps.
 
 <https://www.fabiocrameri.ch/colourmaps/>
 
 All credit for creating the colormaps to Fabio.
 Any errors in the Python implementation of colormaps are my own.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cmcrameri-1.8/cmcrameri/cm.py` & `cmcrameri-1.9/cmcrameri/cm.py`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/acton.txt` & `cmcrameri-1.9/cmcrameri/cmaps/acton.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/actonS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/actonS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/bam.txt` & `cmcrameri-1.9/cmcrameri/cmaps/bam.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/bamO.txt` & `cmcrameri-1.9/cmcrameri/cmaps/bamO.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/bamako.txt` & `cmcrameri-1.9/cmcrameri/cmaps/bamako.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/bamakoS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/bamakoS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/batlow.txt` & `cmcrameri-1.9/cmcrameri/cmaps/batlow.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/batlowK.txt` & `cmcrameri-1.9/cmcrameri/cmaps/batlowK.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/batlowKS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/batlowKS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/batlowS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/batlowS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/batlowW.txt` & `cmcrameri-1.9/cmcrameri/cmaps/batlowW.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/batlowWS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/batlowWS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/berlin.txt` & `cmcrameri-1.9/cmcrameri/cmaps/berlin.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/bilbao.txt` & `cmcrameri-1.9/cmcrameri/cmaps/bilbao.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/bilbaoS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/bilbaoS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/broc.txt` & `cmcrameri-1.9/cmcrameri/cmaps/broc.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/brocO.txt` & `cmcrameri-1.9/cmcrameri/cmaps/brocO.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/buda.txt` & `cmcrameri-1.9/cmcrameri/cmaps/buda.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/budaS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/budaS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/bukavu.txt` & `cmcrameri-1.9/cmcrameri/cmaps/bukavu.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/cork.txt` & `cmcrameri-1.9/cmcrameri/cmaps/cork.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/corkO.txt` & `cmcrameri-1.9/cmcrameri/cmaps/corkO.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/davos.txt` & `cmcrameri-1.9/cmcrameri/cmaps/davos.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/davosS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/davosS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/devon.txt` & `cmcrameri-1.9/cmcrameri/cmaps/devon.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/devonS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/devonS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/fes.txt` & `cmcrameri-1.9/cmcrameri/cmaps/fes.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/glasgow.txt` & `cmcrameri-1.9/cmcrameri/cmaps/glasgow.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/glasgowS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/glasgowS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/grayC.txt` & `cmcrameri-1.9/cmcrameri/cmaps/grayC.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/grayCS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/grayCS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/hawaii.txt` & `cmcrameri-1.9/cmcrameri/cmaps/hawaii.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/hawaiiS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/hawaiiS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/imola.txt` & `cmcrameri-1.9/cmcrameri/cmaps/imola.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/imolaS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/imolaS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/lajolla.txt` & `cmcrameri-1.9/cmcrameri/cmaps/lajolla.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/lajollaS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/lajollaS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/lapaz.txt` & `cmcrameri-1.9/cmcrameri/cmaps/lapaz.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/lapazS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/lapazS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/lipari.txt` & `cmcrameri-1.9/cmcrameri/cmaps/lipari.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/lipariS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/lipariS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/lisbon.txt` & `cmcrameri-1.9/cmcrameri/cmaps/lisbon.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/managua.txt` & `cmcrameri-1.9/cmcrameri/cmaps/managua.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/navia.txt` & `cmcrameri-1.9/cmcrameri/cmaps/navia.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/naviaS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/naviaS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/nuuk.txt` & `cmcrameri-1.9/cmcrameri/cmaps/nuuk.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/nuukS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/nuukS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/oleron.txt` & `cmcrameri-1.9/cmcrameri/cmaps/oleron.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/oslo.txt` & `cmcrameri-1.9/cmcrameri/cmaps/oslo.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/osloS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/osloS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/roma.txt` & `cmcrameri-1.9/cmcrameri/cmaps/roma.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/romaO.txt` & `cmcrameri-1.9/cmcrameri/cmaps/romaO.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/tofino.txt` & `cmcrameri-1.9/cmcrameri/cmaps/tofino.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/tokyo.txt` & `cmcrameri-1.9/cmcrameri/cmaps/tokyo.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/tokyoS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/tokyoS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/turku.txt` & `cmcrameri-1.9/cmcrameri/cmaps/turku.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/turkuS.txt` & `cmcrameri-1.9/cmcrameri/cmaps/turkuS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/vanimo.txt` & `cmcrameri-1.9/cmcrameri/cmaps/vanimo.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/vik.txt` & `cmcrameri-1.9/cmcrameri/cmaps/vik.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/cmaps/vikO.txt` & `cmcrameri-1.9/cmcrameri/cmaps/vikO.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri/colormaps.png` & `cmcrameri-1.9/cmcrameri/colormaps.png`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/cmcrameri.egg-info/SOURCES.txt` & `cmcrameri-1.9/cmcrameri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.8/pyproject.toml` & `cmcrameri-1.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 dependencies = [
   "matplotlib",
   "numpy",
   "packaging",
 ]
 [project.urls]
-documentation = "https://callumrollo.github.io/cmcrameri"
+documentation = "https://github.com/callumrollo/cmcrameri"
 homepage = "https://pypi.org/project/cmcrameri/"
 repository = "https://github.com/callumrollo/cmcrameri"
 
 [tool.setuptools]
 packages = ["cmcrameri"]
 include-package-data = true
```


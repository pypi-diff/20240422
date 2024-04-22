# Comparing `tmp/snk_cli-0.1.4.tar.gz` & `tmp/snk_cli-0.2.0.tar.gz`

## Comparing `snk_cli-0.1.4.tar` & `snk_cli-0.2.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 snk_cli-0.1.4/mkdocs.yml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 snk_cli-0.1.4/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk_cli-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 snk_cli-0.1.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 snk_cli-0.1.4/docs/index.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.1.4/docs/reference/cli.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 snk_cli-0.1.4/docs/reference/config.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.1.4/docs/reference/dynamic_typer.md
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snk_cli-0.1.4/docs/reference/options.md
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 snk_cli-0.1.4/docs/reference/subcommands.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 snk_cli-0.1.4/docs/reference/testing.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 snk_cli-0.1.4/docs/reference/utils.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.1.4/docs/reference/validate.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.1.4/docs/reference/workflow.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/__about__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/__init__.py
--rw-r--r--   0        0        0     8405 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/cli.py
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/dynamic_typer.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/testing.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/utils.py
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/validate.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/workflow.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/config/__init__.py
--rw-r--r--   0        0        0    10313 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/config/config.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/config/utils.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/options/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/options/option.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/options/utils.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/subcommands/__init__.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/subcommands/config.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/subcommands/env.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/subcommands/profile.py
--rw-r--r--   0        0        0    17941 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/subcommands/run.py
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/subcommands/script.py
--rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 snk_cli-0.1.4/src/snk_cli/subcommands/utils.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/test_dynamic_typer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/cov.fasta
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/print_config/Snakefile
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/print_config/cli.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/print_config/config.yaml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/print_config/snk.yaml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/workflow/cli.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/workflow/config.yaml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/workflow/snk.yaml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/workflow/resources/data.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/workflow/things/__about__.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/workflow/workflow/Snakefile
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/workflow/workflow/envs/python.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/workflow/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/workflow/workflow/profiles/slurm/config.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/data/workflow/workflow/scripts/hello.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/test_cli/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/test_cli/test_dynamic_options.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/test_cli/test_run.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/test_cli/test_snk_config.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/test_cli/test_subcommands.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/test_cli/test_validate.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 snk_cli-0.1.4/tests/test_cli/test_workflow_cli.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 snk_cli-0.1.4/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk_cli-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 snk_cli-0.1.4/README.md
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 snk_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 snk_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 snk_cli-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk_cli-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 snk_cli-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/index.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/cli.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/config.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/dynamic_typer.md
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/options.md
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/subcommands.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/testing.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/utils.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/validate.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/workflow.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/__about__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/__init__.py
+-rw-r--r--   0        0        0     8847 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/cli.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/conda.py
+-rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/dynamic_typer.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/testing.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/utils.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/validate.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/workflow.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/config/__init__.py
+-rw-r--r--   0        0        0    10310 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/config/config.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/config/utils.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/options/__init__.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/options/option.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/options/utils.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/__init__.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/config.py
+-rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/env.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/profile.py
+-rw-r--r--   0        0        0    18508 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/run.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/script.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_conda_env.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_dynamic_typer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/cov.fasta
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/print_config/Snakefile
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/print_config/cli.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/print_config/config.yaml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/print_config/snk.yaml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/cli.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/config.yaml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/snk.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/resources/data.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/things/__about__.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/workflow/Snakefile
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/workflow/envs/python.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/workflow/profiles/slurm/config.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/workflow/scripts/hello.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_dynamic_options.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_run.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_snk_config.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_subcommands.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_validate.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_workflow_cli.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 snk_cli-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk_cli-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 snk_cli-0.2.0/README.md
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 snk_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 snk_cli-0.2.0/PKG-INFO
```

### Comparing `snk_cli-0.1.4/mkdocs.yml` & `snk_cli-0.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/.github/workflows/publish.yml` & `snk_cli-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/.github/workflows/tests.yml` & `snk_cli-0.2.0/.github/workflows/tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -27,12 +27,12 @@
           key: ${{ github.ref }}
           path: .cache
       - run: pip install hatch
       - run: sudo apt-get update && sudo apt-get install -y llvm
       - run: sudo apt-get -y install graphviz
       - name: Run tests
         shell: bash
-        run: hatch run cov
+        run: hatch run snakemake:cov
       - name: Upload coverage reports to Codecov
         uses: codecov/codecov-action@v3
```

### Comparing `snk_cli-0.1.4/src/snk_cli/cli.py` & `snk_cli-0.2.0/src/snk_cli/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import platform
 
 import typer
 from pathlib import Path
 from typing import Optional
 import os
 
-
-from snakemake import SNAKEFILE_CHOICES
 from art import text2art
 
 from snk_cli.dynamic_typer import DynamicTyper
 from snk_cli.subcommands import EnvApp, ConfigApp, RunApp, ScriptApp, ProfileApp
 
 from snk_cli.config.config import (
     SnkConfig,
@@ -220,14 +218,25 @@
 
         Raises:
           FileNotFoundError: If the snakefile is not found.
 
         Examples:
           >>> CLI._find_snakefile()
         """
+        SNAKEFILE_CHOICES = list(
+            map(
+                Path,
+                (
+                    "Snakefile",
+                    "snakefile",
+                    "workflow/Snakefile",
+                    "workflow/snakefile",
+                ),
+            )
+        )
         for path in SNAKEFILE_CHOICES:
             if (self.workflow.path / path).exists():
                 return self.workflow.path / path
         raise FileNotFoundError("Snakefile not found!")
 
     def info(self):
         """
@@ -240,10 +249,13 @@
           >>> CLI.info()
         """
         import json
 
         info_dict = {}
         info_dict["name"] = self.workflow.path.name
         info_dict["version"] = self.version
+        info_dict["snakefile"] = str(self.snakefile)
+        info_dict["conda_prefix_dir"] = str(self.conda_prefix_dir)
+        info_dict["singularity_prefix_dir"] = str(self.singularity_prefix_dir)
         info_dict["workflow_dir_path"] = str(self.workflow.path)
         typer.echo(json.dumps(info_dict, indent=2))
```

### Comparing `snk_cli-0.1.4/src/snk_cli/dynamic_typer.py` & `snk_cli-0.2.0/src/snk_cli/dynamic_typer.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,16 +213,16 @@
 
             Notes:
               This function is used in the `add_dynamic_options_to_function` function.
             """
             flat_config = None
 
             if kwargs.get("configfile"):
-                from snakemake import load_configfile
                 from .utils import flatten
+                from snk_cli.config.utils import load_configfile
 
                 snakemake_config = load_configfile(kwargs["configfile"])
                 flat_config = flatten(snakemake_config)
 
             for snk_cli_option in options:
 
                 def add_option_to_args():
```

### Comparing `snk_cli-0.1.4/src/snk_cli/testing.py` & `snk_cli-0.2.0/src/snk_cli/testing.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/src/snk_cli/utils.py` & `snk_cli-0.2.0/src/snk_cli/utils.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/src/snk_cli/validate.py` & `snk_cli-0.2.0/src/snk_cli/validate.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/src/snk_cli/workflow.py` & `snk_cli-0.2.0/src/snk_cli/workflow.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/src/snk_cli/config/config.py` & `snk_cli-0.2.0/src/snk_cli/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from typing import List, Optional
 import snakemake
 from dataclasses import dataclass, field
-from .utils import get_version_from_config
+from .utils import get_version_from_config, load_configfile
 import yaml
 
 
 class SnkConfigError(Exception):
     """
     Base class for all SNK config exceptions.
     """
@@ -93,15 +93,15 @@
             raise MissingSnkConfigError(
                 f"Could not find SNK config file: {snk_config_path}"
             ) from FileNotFoundError
         # raise error if file is empty
         if snk_config_path.stat().st_size == 0:
             raise InvalidSnkConfigError(f"SNK config file is empty: {snk_config_path}") from ValueError
 
-        snk_config_dict = snakemake.load_configfile(snk_config_path)
+        snk_config_dict = load_configfile(snk_config_path)
         snk_config_dict["version"] = get_version_from_config(snk_config_path, snk_config_dict)
         if "annotations" in snk_config_dict:
             # TODO: remove annotations in the future
             snk_config_dict["cli"] = snk_config_dict["annotations"]
             del snk_config_dict["annotations"]
         if "conda_required" in snk_config_dict:
             # TODO: remove conda_required in the future
@@ -253,8 +253,8 @@
     Examples:
       >>> load_workflow_snakemake_config(Path("workflow"))
       {'inputs': {'data': 'data.txt'}, 'outputs': {'results': 'results.txt'}}
     """
     workflow_config_path = get_config_from_workflow_dir(workflow_dir_path)
     if not workflow_config_path or not workflow_config_path.exists():
         return {}
-    return snakemake.load_configfile(workflow_config_path)
+    return load_configfile(workflow_config_path)
```

### Comparing `snk_cli-0.1.4/src/snk_cli/config/utils.py` & `snk_cli-0.2.0/src/snk_cli/config/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from pathlib import Path
-from snakemake import load_configfile
+try:
+    # snakemake < 8.0.0
+    from snakemake import load_configfile
+except ImportError:
+    from snakemake.common.configfile import _load_configfile as load_configfile  # noqa: F401
 
 def get_version_from_config(config_path: Path, config_dict: dict = None) -> str:
     """
     Get the version from the config file or config dictionary.
 
     Args:
       config_path (Path): Path to the config file.
```

### Comparing `snk_cli-0.1.4/src/snk_cli/options/utils.py` & `snk_cli-0.2.0/src/snk_cli/options/utils.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/src/snk_cli/subcommands/config.py` & `snk_cli-0.2.0/src/snk_cli/subcommands/config.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/src/snk_cli/subcommands/env.py` & `snk_cli-0.2.0/src/snk_cli/subcommands/env.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,45 +3,38 @@
 import subprocess
 from pathlib import Path
 import sys
 from typing import List, Optional
 import typer
 
 from snk_cli.dynamic_typer import DynamicTyper
-from .utils import create_snakemake_workflow
+from snk_cli.conda import conda_environment_factory
 from ..workflow import Workflow
 from rich.console import Console
 from rich.syntax import Syntax
 from snakemake.deployment.conda import Conda, Env, CreateCondaEnvironmentException
 from snk_cli.config.config import get_config_from_workflow_dir
 
 from concurrent.futures import ProcessPoolExecutor
 
 def get_num_cores(default=4):
     try:
         return os.cpu_count()
     except:
         return default
 
-def create_conda_environment(args):
-    # unpack args
-    env_path_str, snakefile, snakemake_config, configfiles, conda_prefix_dir_str = args
-    # Reconstruct the snakemake_workflow configuration
+def create_conda_environment_wrapper(args):
+    """
+    This wrapper is designed to be submitted to a ProcessPoolExecutor
+    """
+    env_path_str, conda_prefix_dir_str = args
     conda_prefix_dir = Path(conda_prefix_dir_str).resolve()
-    snakemake_workflow = create_snakemake_workflow(
-        snakefile,
-        config=snakemake_config,
-        configfiles=configfiles,
-        use_conda=True,
-        conda_prefix=conda_prefix_dir,
-    )
     env_path = Path(env_path_str).resolve()
-    env = Env(snakemake_workflow, env_file=env_path)
     try:
-        env.create()
+        conda_environment_factory(env_path, conda_prefix_dir).create()
     except CreateCondaEnvironmentException as e:
         typer.secho(str(e), fg="red", err=True)
         return 1
     return 0
 
 
 class EnvApp(DynamicTyper):
@@ -53,21 +46,14 @@
         snakefile: Path,
     ):
         self.workflow = workflow
         self.conda_prefix_dir = conda_prefix_dir
         self.snakemake_config = snakemake_config
         self.snakefile = snakefile
         self.configfile = get_config_from_workflow_dir(self.workflow.path)
-        self.snakemake_workflow = create_snakemake_workflow(
-            self.snakefile,
-            config=self.snakemake_config,
-            configfiles=[self.configfile] if self.configfile else None,
-            use_conda=True,
-            conda_prefix=self.conda_prefix_dir.resolve(),
-        )
         self.register_command(self.list, help="List the environments in the workflow.")
         self.register_command(self.show, help="Show the contents of an environment.")
         self.register_command(
             self.run, help="Run a command in one of the workflow environments."
         )
         self.register_command(
             self.activate, help="Activate a workflow conda environment."
@@ -82,15 +68,15 @@
         ),
     ):
         from rich.console import Console
         from rich.table import Table
 
         table = Table("Name", "CMD", "Env", show_header=True, show_lines=True)
         for env in self.workflow.environments:
-            conda = Env(self.snakemake_workflow, env_file=env.resolve())
+            conda = conda_environment_factory(env, self.conda_prefix_dir)
             # address relative to cwd
             address = Path(conda.address)
             if address.exists():
                 address = str(address) if verbose else f"[green]{address.name}[/green]"
                 cmd = f"{self.workflow.name} env activate {env.stem}"
             else:
                 address = ""
@@ -133,15 +119,15 @@
         name: str = typer.Argument(..., help="The name of the environment."),
         verbose: bool = typer.Option(
             False, "--verbose", "-v", help="Print the command to run."
         ),
         cmd: List[str] = typer.Argument(..., help="The command to run in environment."),
     ):
         env_path = self._get_conda_env_path(name)
-        env = Env(self.snakemake_workflow, env_file=env_path.resolve())
+        env = conda_environment_factory(env_path, self.conda_prefix_dir)
         env.create()
         cmd = self._shellcmd(env.address, " ".join(cmd))
         if verbose:
             self.log(cmd)
         user_shell = os.environ.get("SHELL", "/bin/bash")
         subprocess.run(cmd, shell=True, env=os.environ.copy(), executable=user_shell)
 
@@ -150,15 +136,15 @@
         name: Optional[str] = typer.Argument(None, help="The name of the environment. If not provided, all environments will be deleted."),
         force: bool = typer.Option(
             False, "--force", "-f", help="Force deletion of the environments."
         ),
     ):
         if name:
             env_path = self._get_conda_env_path(name)
-            env = Env(self.snakemake_workflow, env_file=env_path.resolve())
+            env = conda_environment_factory(env_path, self.conda_prefix_dir)
             path = Path(env.address)
             if not path.exists():
                 self.error(f"Environment {name} not created!")
         else:
             path = self.conda_prefix_dir
         if force or input(f"Delete {path}? [y/N] ").lower() == "y":
             shutil.rmtree(path)
@@ -172,23 +158,20 @@
         if names:
             env_paths = [self._get_conda_env_path(name) for name in names]
         else:
             env_paths = self.workflow.environments
         env_args = [
             (
                 path,
-                self.snakefile,
-                self.snakemake_config,
-                [self.configfile] if self.configfile else None,
                 self.conda_prefix_dir.resolve(),
             )
             for path in env_paths 
         ]
         with ProcessPoolExecutor(max_workers=max_workers) as executor:
-            status_codes = executor.map(create_conda_environment, env_args)
+            status_codes = executor.map(create_conda_environment_wrapper, env_args)
         if any(status_codes):
             self.error("Failed to create all conda environments!")
         if names:
             self.success(f"Created environment{'s' if len(names) > 1 else ''} {' '.join(names)}!")
         else:
             self.success("All conda environments created!")
 
@@ -197,15 +180,15 @@
         name: str = typer.Argument(..., help="The name of the environment."),
         verbose: bool = typer.Option(
             False, "--verbose", "-v", help="Print the activation command."
         ),
     ):
         env_path = self._get_conda_env_path(name)
         self.log(f"Activating {name} environment... (type 'exit' to deactivate)")
-        env = Env(self.snakemake_workflow, env_file=env_path.resolve())
+        env = conda_environment_factory(env_path, self.conda_prefix_dir)
         env.create()
         user_shell = os.environ.get("SHELL", "/bin/bash")
         activate_cmd = self._shellcmd(env.address, user_shell)
         if verbose:
             self.log(activate_cmd)
         subprocess.run(activate_cmd, shell=True, env=os.environ.copy(), executable=user_shell)
         self.log(f"Exiting {name} environment...")
```

### Comparing `snk_cli-0.1.4/src/snk_cli/subcommands/profile.py` & `snk_cli-0.2.0/src/snk_cli/subcommands/profile.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/src/snk_cli/subcommands/run.py` & `snk_cli-0.2.0/src/snk_cli/subcommands/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List, Optional
 from pathlib import Path
 import typer
 from contextlib import contextmanager
 
 from snk_cli.dynamic_typer import DynamicTyper
 from snk_cli.options.option import Option
+from snk_cli.conda import is_snakemake_version_8_or_above
 from ..workflow import Workflow
 from snk_cli.utils import (
     parse_config_args,
     dag_filetype_callback,
     check_command_available
 )
 
@@ -163,15 +164,14 @@
 
         Side Effects:
           Runs the workflow.
 
         Examples:
           >>> RunApp.run(target='my_target', configfile=Path('/path/to/config.yaml'), resource=[Path('/path/to/resource')], verbose=True)
         """
-        import snakemake
         import shutil
         import sys
 
         self.verbose = verbose
         args = []
         if self.snk_config.additional_snakemake_args:
             if verbose:
@@ -270,42 +270,39 @@
             self.snk_config.resources,
             cleanup=not keep_resources,
             symlink_resources=self.snk_config.symlink_resources,
         ):
             if dag:
                 return self._save_dag(snakemake_args=args, filename=dag)
             try:
-                snakemake.parse_config = parse_config_monkeypatch
-                snakemake.main(args)
+                execute_snakemake(args)
             except SystemExit as e:
                 status = int(str(e))
                 if status:
                     sys.exit(status)
         if not keep_snakemake and Path(".snakemake").exists():
             typer.secho("Cleaning up '.snakemake' folder... use --keep-snakemake to keep.", fg=typer.colors.YELLOW, err=True)
             shutil.rmtree(".snakemake")
 
     def _save_dag(self, snakemake_args: List[str], filename: Path):
         from contextlib import redirect_stdout
-        import snakemake
         import subprocess
         import io
 
         snakemake_args.append("--dag")
 
         fileType = filename.suffix.lstrip(".")
 
         # Create a file-like object to redirect the stdout
         snakemake_output = io.StringIO()
         # Use redirect_stdout to redirect stdout to the file-like object
         with redirect_stdout(snakemake_output):
             # Capture the output of snakemake.main(args) using a try-except block
             try:
-                snakemake.parse_config = parse_config_monkeypatch
-                snakemake.main(snakemake_args)
+                execute_snakemake(snakemake_args)
             except SystemExit:  # Catch SystemExit exception to prevent termination
                 pass
         try:
             snakemake_output = snakemake_output.getvalue()
             if "snakemake_dag" not in snakemake_output:
                 self.error("Could not generate dag!", exit=True)
             # discard everything before digraph snakemake_dag
@@ -411,28 +408,51 @@
                         typer.secho(
                             f"Deleting '{copied_resource.name}' resource...",
                             fg=typer.colors.MAGENTA,
                             err=True,
                         )
                     remove_resource(copied_resource)
 
+def execute_snakemake(args):
+    """
+    Execute snakemake with the given arguments.
+
+    Args:
+      args: The arguments to pass to snakemake.
+
+    Side Effects:
+      Executes snakemake with the given arguments.
+    """
+    import snakemake
+    if is_snakemake_version_8_or_above:
+        from snakemake import cli
+        cli.parse_config = parse_config_monkeypatch
+        cli.main(args)
+    else:
+        snakemake.parse_config = parse_config_monkeypatch
+        snakemake.main(args)
 
 def parse_config_monkeypatch(args):
     """
     Monkeypatch the parse_config function from snakemake.
 
     Args:
       args: The arguments to parse.
 
     Returns:
       dict: The parsed config.
     """
     import yaml
-    import snakemake
     import re
+    if is_snakemake_version_8_or_above:
+        from snakemake.cli import parse_key_value_arg, update_config, _bool_parser
+        entries = args
+    else:
+        from snakemake import parse_key_value_arg, update_config, _bool_parser
+        entries = args.config
 
     class NoDatesSafeLoader(yaml.SafeLoader):
         @classmethod
         def remove_implicit_resolver(cls, tag_to_remove):
             """
             Remove implicit resolvers for a particular tag.
 
@@ -461,35 +481,35 @@
 
         Returns:
         The loaded yaml object.
         """
         s = s.replace(": None", ": null")
         return yaml.load(s, Loader=NoDatesSafeLoader)
 
-    parsers = [int, float, snakemake._bool_parser, _yaml_safe_load, str]
+    parsers = [int, float, _bool_parser, _yaml_safe_load, str]
     config = dict()
-    if args.config is not None:
+    if entries is not None:
         valid = re.compile(r"[a-zA-Z_]\w*$")
-        for entry in args.config:
-            key, val = snakemake.parse_key_value_arg(
+        for entry in entries:
+            key, val = parse_key_value_arg(
                 entry,
                 errmsg="Invalid config definition: Config entries have to be defined as name=value pairs.",
             )
             if not valid.match(key):
                 raise ValueError(
                     "Invalid config definition: Config entry must start with a valid identifier."
                 )
             v = None
             if val == "" or val == "None":
-                snakemake.update_config(config, {key: v})
+                update_config(config, {key: v})
                 continue
             for parser in parsers:
                 try:
                     v = parser(val)
                     # avoid accidental interpretation as function
                     if not callable(v):
                         break
                 except:
                     pass
             assert v is not None
-            snakemake.update_config(config, {key: v})
+            update_config(config, {key: v})
     return config
```

### Comparing `snk_cli-0.1.4/src/snk_cli/subcommands/script.py` & `snk_cli-0.2.0/src/snk_cli/subcommands/script.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import subprocess
 from pathlib import Path
 import sys
 from typing import List
 import typer
 
 from ..dynamic_typer import DynamicTyper
-from .utils import create_snakemake_workflow
+from snk_cli.conda import conda_environment_factory
 from ..workflow import Workflow
 from rich.console import Console
 from rich.syntax import Syntax
-from snakemake.deployment.conda import Conda, Env
+from snakemake.deployment.conda import Conda
 from snk_cli.config.config import get_config_from_workflow_dir
 
 
 class ScriptApp(DynamicTyper):
     def __init__(
         self,
         workflow: Workflow,
@@ -112,22 +112,15 @@
         args: List[str] = typer.Argument(None, help="Arguments to pass to the script."),
     ):
         script_path = self._get_script_path(name)
         executor = self._get_executor(script_path.suffix[1:])
         cmd = [executor, f'"{script_path}"'] + args
         if env:
             env_path = self._get_conda_env_path(env)
-            workflow = create_snakemake_workflow(
-                self.snakefile,
-                config=self.snakemake_config,
-                configfiles=[self.configfile] if self.configfile else None,
-                use_conda=True,
-                conda_prefix=self.conda_prefix_dir.resolve(),
-            )
-            env = Env(workflow, env_file=env_path.resolve())
+            env = conda_environment_factory(env_path, self.conda_prefix_dir)
             env.create()
             cmd = self._shellcmd(env.address, " ".join(cmd))
         else:
             cmd = " ".join(cmd)
         user_shell = os.environ.get("SHELL", "/bin/bash")
         subprocess.run(cmd, shell=True, env=os.environ.copy(), executable=user_shell)
```

### Comparing `snk_cli-0.1.4/tests/test_dynamic_typer.py` & `snk_cli-0.2.0/tests/test_dynamic_typer.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/utils.py` & `snk_cli-0.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/data/artic_v4.1.bed` & `snk_cli-0.2.0/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/data/config.yaml` & `snk_cli-0.2.0/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/data/cov.fasta` & `snk_cli-0.2.0/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/data/workflow/snk.yaml` & `snk_cli-0.2.0/tests/data/workflow/snk.yaml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/data/workflow/workflow/Snakefile` & `snk_cli-0.2.0/tests/data/workflow/workflow/Snakefile`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/data/workflow/workflow/envs/python.yml` & `snk_cli-0.2.0/tests/data/workflow/workflow/envs/python.yml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/data/workflow/workflow/profiles/slurm/config.yaml` & `snk_cli-0.2.0/tests/data/workflow/workflow/profiles/slurm/config.yaml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/test_cli/test_dynamic_options.py` & `snk_cli-0.2.0/tests/test_cli/test_dynamic_options.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/test_cli/test_run.py` & `snk_cli-0.2.0/tests/test_cli/test_run.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/test_cli/test_snk_config.py` & `snk_cli-0.2.0/tests/test_cli/test_snk_config.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/test_cli/test_subcommands.py` & `snk_cli-0.2.0/tests/test_cli/test_subcommands.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     (["env", "list"], ["python"], []),
     (["env", "show", "python"], ["python"], []),
     (["env", "create"], ["All conda environments created!"], []),
     (["env", "create", "python"], ["Created environment python!"], []),
     (["env", "run", "python", "which python"], ["bin/python"], []),
     (["env", "activate", "python"], [], ["Activating python environment...", "Exiting python environment..."]),
     (["env", "remove", "-f"], ["Deleted"], []),
+    (["info"], ["name", "version", "snakefile", "conda_prefix_dir", "singularity_prefix_dir", "workflow_dir_path"], []),
 ])
 def test_snk_cli_command(capfd, local_runner, cmd, expected_in_stdout, expected_in_stderr):
     res = local_runner(cmd)
     captured = capfd.readouterr()  # Capture stdout and stderr of subprocess e.g. env and script commands
     assert res.exit_code == 0, res.stderr
     for expected in expected_in_stdout:
         assert expected in res.stdout or expected in captured.out, res.stderr
```

### Comparing `snk_cli-0.1.4/tests/test_cli/test_validate.py` & `snk_cli-0.2.0/tests/test_cli/test_validate.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/tests/test_cli/test_workflow_cli.py` & `snk_cli-0.2.0/tests/test_cli/test_workflow_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from pathlib import Path
 from snk_cli.utils import flatten, convert_key_to_snakemake_format
-import snakemake
 import pytest
 from ..utils import SnkCliRunner
-
+from snk_cli.config.utils import load_configfile
 
 def test_flatten(example_config: Path):
-    config = snakemake.load_configfile(example_config)
+    config = load_configfile(example_config)
     flat_config = flatten(config)
     assert flat_config["diffexp:contrasts:A-vs-B"] == ["A", "B"]
 
 
 @pytest.mark.parametrize(
     "key, value, expected",
     [
```

### Comparing `snk_cli-0.1.4/LICENSE.txt` & `snk_cli-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/README.md` & `snk_cli-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `snk_cli-0.1.4/pyproject.toml` & `snk_cli-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "snakemake>=7,<8",
+  "snakemake>=7",
   "typer[all]~=0.9.0",
   "GitPython~=3.1",
   "pulp<2.8",  # Pin pulp <2.8 for snakemake: https://github.com/snakemake/snakemake/issues/2607
   "art~=5.9",
   "makefun~=1.15",
   "datrie>=0.8.2",
 ]
@@ -39,23 +39,18 @@
 Issues = "https://github.com/unknown/snk-cli/issues"
 Source = "https://github.com/unknown/snk-cli"
 
 [tool.hatch.version]
 path = "src/snk_cli/__about__.py"
 
 
-[[tool.hatch.envs.test.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
-snakemake = ["7.32.4"]
-
-# [[tool.hatch.envs.test.matrix]]
-# python = ["3.11", "3.12"]
-# snakemake = ["8.5.5"]
+[[tool.hatch.envs.snakemake.matrix]]
+snakemake = ["7.32.4", "8.10.8"]
 
-[tool.hatch.envs.test]
+[tool.hatch.snakemake.test]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "snakemake=={matrix:snakemake}"]
 
 [tool.hatch.envs.default]
 dependencies = [
@@ -71,15 +66,15 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
+python = ["3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.types]
 dependencies = [
   "mypy>=1.0.0",
 ]
 [tool.hatch.envs.types.scripts]
 check = "mypy --install-types --non-interactive {args:src/snk_cli tests}"
```

### Comparing `snk_cli-0.1.4/PKG-INFO` & `snk_cli-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snk-cli
-Version: 0.1.4
+Version: 0.2.0
 Project-URL: Documentation, https://github.com/unknown/snk-cli#readme
 Project-URL: Issues, https://github.com/unknown/snk-cli/issues
 Project-URL: Source, https://github.com/unknown/snk-cli
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: art~=5.9
 Requires-Dist: datrie>=0.8.2
 Requires-Dist: gitpython~=3.1
 Requires-Dist: makefun~=1.15
 Requires-Dist: pulp<2.8
-Requires-Dist: snakemake<8,>=7
+Requires-Dist: snakemake>=7
 Requires-Dist: typer[all]~=0.9.0
 Description-Content-Type: text/markdown
 
 # snk-cli
 [![PyPI - Version](https://img.shields.io/pypi/v/snk-cli.svg)](https://pypi.org/project/snk-cli)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/snk-cli.svg)](https://pypi.org/project/snk-cli)
 [![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
```


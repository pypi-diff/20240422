# Comparing `tmp/ropt-0.1.1.tar.gz` & `tmp/ropt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt-0.1.1.tar", last modified: Fri Apr 19 10:51:58 2024, max compression
+gzip compressed data, was "ropt-0.1.2.tar", last modified: Mon Apr 22 06:49:00 2024, max compression
```

## Comparing `ropt-0.1.1.tar` & `ropt-0.1.2.tar`

### file list

```diff
@@ -1,185 +1,184 @@
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.873288 ropt-0.1.1/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.829288 ropt-0.1.1/.github/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.837288 ropt-0.1.1/.github/workflows/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      709 2024-02-02 10:54:40.000000 ropt-0.1.1/.github/workflows/build-docs.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      626 2024-04-19 09:23:16.000000 ropt-0.1.1/.github/workflows/github-pages.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1006 2024-04-19 08:53:50.000000 ropt-0.1.1/.github/workflows/static-checks.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      757 2024-02-02 10:54:40.000000 ropt-0.1.1/.github/workflows/tests.yml
--rwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)       59 2024-04-19 08:53:50.000000 ropt-0.1.1/.gitignore
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      321 2024-04-19 05:26:12.000000 ropt-0.1.1/.readthedocs.yaml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    35149 2024-04-19 05:26:12.000000 ropt-0.1.1/LICENSE
--rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     2536 2024-04-19 10:51:58.873288 ropt-0.1.1/PKG-INFO
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1033 2024-04-19 10:39:15.000000 ropt-0.1.1/README-PyPI.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1268 2024-04-19 08:53:50.000000 ropt-0.1.1/README.md
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.837288 ropt-0.1.1/docs/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3524 2024-04-19 09:05:18.000000 ropt-0.1.1/docs/index.md
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.837288 ropt-0.1.1/docs/javascripts/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      334 2024-02-02 10:54:40.000000 ropt-0.1.1/docs/javascripts/mathjax.js
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.841288 ropt-0.1.1/docs/reference/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      488 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/enopt_config.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      101 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/enums.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      554 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/evaluator.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      101 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/exceptions.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      267 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/function_transforms.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      101 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/optimization.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       35 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/optimization_steps.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      182 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/optimizer_backends.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      330 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/plan_config.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       17 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/plugins.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      533 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/realization_filters.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       16 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/reporting.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1081 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/results.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      195 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/sampler_backends.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       39 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/reference/utilities.md
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.841288 ropt-0.1.1/docs/usage/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3765 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/usage/robust_optimization.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3222 2024-04-19 08:53:50.000000 ropt-0.1.1/docs/usage/running.md
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.841288 ropt-0.1.1/examples/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2821 2024-04-19 08:53:50.000000 ropt-0.1.1/examples/de_linear.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3023 2024-04-19 08:53:50.000000 ropt-0.1.1/examples/de_nonlinear.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3157 2024-04-19 08:53:50.000000 ropt-0.1.1/examples/rosenbrock_deterministic.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4323 2024-04-19 08:53:50.000000 ropt-0.1.1/examples/rosenbrock_ensemble.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.841288 ropt-0.1.1/examples/script_optimizer/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1179 2023-10-10 07:53:14.000000 ropt-0.1.1/examples/script_optimizer/rosenbrock.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2611 2024-04-19 08:53:50.000000 ropt-0.1.1/examples/script_optimizer/run.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2199 2024-04-19 09:42:03.000000 ropt-0.1.1/mkdocs.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2474 2024-04-19 10:39:25.000000 ropt-0.1.1/pyproject.toml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       38 2024-04-19 10:51:58.873288 ropt-0.1.1/setup.cfg
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.829288 ropt-0.1.1/src/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.841288 ropt-0.1.1/src/ropt/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       73 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/__init__.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.845288 ropt-0.1.1/src/ropt/apps/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      143 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/apps/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    17499 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/apps/_script_optimizer.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.845288 ropt-0.1.1/src/ropt/config/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       68 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/__init__.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.849288 ropt-0.1.1/src/ropt/config/enopt/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      993 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      355 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_enopt_base_model.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     9167 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_enopt_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1997 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_function_transform_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6187 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_gradient_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3401 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_linear_constraints_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5071 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_nonlinear_constraints_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4514 2024-04-19 09:03:57.000000 ropt-0.1.1/src/ropt/config/enopt/_objective_functions_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4332 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_optimizer_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2161 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_realization_filter_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3532 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_realizations_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2351 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_sampler_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3890 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_utils.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     8285 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/_variables_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      952 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/enopt/constants.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.849288 ropt-0.1.1/src/ropt/config/plan/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      688 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/plan/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5115 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/plan/_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      574 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/plan/_plan_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      827 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/plan/_step_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5130 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/config/utils.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5477 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/enums.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.853288 ropt-0.1.1/src/ropt/evaluator/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2527 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/evaluator/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     7214 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/evaluator/_concurrent.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    25277 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/evaluator/_ensemble_evaluator.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5969 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/evaluator/_evaluator.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     8928 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/evaluator/_evaluator_results.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2207 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/evaluator/_function.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     8461 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/evaluator/_gradient.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      862 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/evaluator/_utils.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5297 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/evaluator/parsl.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1349 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/events.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      735 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/exceptions.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.853288 ropt-0.1.1/src/ropt/optimization/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      433 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/optimization/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2870 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/optimization/_bases.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4909 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/optimization/_ensemble_optimizer.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      771 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/optimization/_events.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     9297 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/optimization/_optimizer.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6893 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/optimization/_plan.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.853288 ropt-0.1.1/src/ropt/plugins/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1744 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5950 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/_manager.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.853288 ropt-0.1.1/src/ropt/plugins/function_transform/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      210 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/function_transform/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5528 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/function_transform/default.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2600 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/function_transform/protocol.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.857288 ropt-0.1.1/src/ropt/plugins/optimization_steps/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      138 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimization_steps/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2911 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimization_steps/_utils.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1792 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimization_steps/default.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1022 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimization_steps/enopt_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3890 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimization_steps/evaluator.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      748 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimization_steps/label.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4570 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimization_steps/optimizer.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      905 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimization_steps/reset_tracker.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1630 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimization_steps/restart.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2949 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimization_steps/tracker.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1843 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimization_steps/update_config.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.857288 ropt-0.1.1/src/ropt/plugins/optimizer/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1001 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimizer/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4249 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimizer/protocol.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    20113 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimizer/scipy.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     7969 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/optimizer/utils.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.857288 ropt-0.1.1/src/ropt/plugins/realization_filter/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      521 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/realization_filter/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    15031 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/realization_filter/default.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2096 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/realization_filter/protocol.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.857288 ropt-0.1.1/src/ropt/plugins/sampler/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      641 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/sampler/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3555 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/sampler/protocol.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6798 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/plugins/sampler/scipy.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/py.typed
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.861288 ropt-0.1.1/src/ropt/report/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      573 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/report/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     7603 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/report/_data_frame.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5295 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/report/_table.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4065 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/report/_utils.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.865288 ropt-0.1.1/src/ropt/results/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3953 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6147 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_bound_constraints.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5792 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_function_evaluations.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3571 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_function_results.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4229 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_functions.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3377 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_gradient_evaluations.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2879 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_gradient_results.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1969 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_gradients.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2571 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_linear_constraints.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2684 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_maximize.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4262 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_nonlinear_constraints.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3509 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_pandas.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2141 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_realizations.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1235 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_result_field.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     9252 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_results.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3523 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_utils.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4287 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/results/_xarray.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.865288 ropt-0.1.1/src/ropt/utils/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      169 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/utils/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      712 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/utils/_misc.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5351 2024-04-19 08:53:50.000000 ropt-0.1.1/src/ropt/utils/scaling.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      411 2024-04-19 10:51:58.000000 ropt-0.1.1/src/ropt/version.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.869288 ropt-0.1.1/src/ropt.egg-info/
--rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     2536 2024-04-19 10:51:58.000000 ropt-0.1.1/src/ropt.egg-info/PKG-INFO
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5095 2024-04-19 10:51:58.000000 ropt-0.1.1/src/ropt.egg-info/SOURCES.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        1 2024-04-19 10:51:58.000000 ropt-0.1.1/src/ropt.egg-info/dependency_links.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      275 2024-04-19 10:51:58.000000 ropt-0.1.1/src/ropt.egg-info/requires.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        5 2024-04-19 10:51:58.000000 ropt-0.1.1/src/ropt.egg-info/top_level.txt
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 10:51:58.869288 ropt-0.1.1/tests/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2023-10-10 07:53:14.000000 ropt-0.1.1/tests/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4505 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/conftest.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3811 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_concurrent.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    25786 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     9209 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_ensemble_gradient.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1775 2024-02-02 10:54:40.000000 ropt-0.1.1/tests/test_examples.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2185 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_failed_realizations.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4205 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_function_transforms.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5503 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_netcdf.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    42608 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_optimizer.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     7387 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_pandas.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4626 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_parsl.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    27696 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_realization_filters.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6652 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_result_table.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     8616 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_results.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5248 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_results_data_frame.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6602 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_samplers.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    19164 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_scipy_backend.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4474 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_scipy_samplers.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3197 2024-04-19 08:53:50.000000 ropt-0.1.1/tests/test_xarray.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.499660 ropt-0.1.2/
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.455660 ropt-0.1.2/.github/
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.459660 ropt-0.1.2/.github/workflows/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      709 2024-02-02 10:54:40.000000 ropt-0.1.2/.github/workflows/build-docs.yml
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      626 2024-04-19 09:23:16.000000 ropt-0.1.2/.github/workflows/github-pages.yml
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1006 2024-04-19 08:53:50.000000 ropt-0.1.2/.github/workflows/static-checks.yml
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      757 2024-02-02 10:54:40.000000 ropt-0.1.2/.github/workflows/tests.yml
+-rwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)       59 2024-04-19 08:53:50.000000 ropt-0.1.2/.gitignore
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      321 2024-04-19 05:26:12.000000 ropt-0.1.2/.readthedocs.yaml
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    35149 2024-04-19 05:26:12.000000 ropt-0.1.2/LICENSE
+-rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     3159 2024-04-22 06:49:00.499660 ropt-0.1.2/PKG-INFO
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1656 2024-04-22 06:45:56.000000 ropt-0.1.2/README.md
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.459660 ropt-0.1.2/docs/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3524 2024-04-19 09:05:18.000000 ropt-0.1.2/docs/index.md
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.459660 ropt-0.1.2/docs/javascripts/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      334 2024-02-02 10:54:40.000000 ropt-0.1.2/docs/javascripts/mathjax.js
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.463660 ropt-0.1.2/docs/reference/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      488 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/enopt_config.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      101 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/enums.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      554 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/evaluator.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      101 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/exceptions.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      267 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/function_transforms.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      101 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/optimization.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       35 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/optimization_steps.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      182 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/optimizer_backends.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      330 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/plan_config.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       17 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/plugins.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      533 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/realization_filters.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       16 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/reporting.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1081 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/results.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      195 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/sampler_backends.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       39 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/reference/utilities.md
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.463660 ropt-0.1.2/docs/usage/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3765 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/usage/robust_optimization.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3222 2024-04-19 08:53:50.000000 ropt-0.1.2/docs/usage/running.md
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.463660 ropt-0.1.2/examples/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2821 2024-04-19 08:53:50.000000 ropt-0.1.2/examples/de_linear.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3023 2024-04-19 08:53:50.000000 ropt-0.1.2/examples/de_nonlinear.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3157 2024-04-19 08:53:50.000000 ropt-0.1.2/examples/rosenbrock_deterministic.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4323 2024-04-19 08:53:50.000000 ropt-0.1.2/examples/rosenbrock_ensemble.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.463660 ropt-0.1.2/examples/script_optimizer/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1179 2023-10-10 07:53:14.000000 ropt-0.1.2/examples/script_optimizer/rosenbrock.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2611 2024-04-19 08:53:50.000000 ropt-0.1.2/examples/script_optimizer/run.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2199 2024-04-19 09:42:03.000000 ropt-0.1.2/mkdocs.yml
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2469 2024-04-22 06:46:25.000000 ropt-0.1.2/pyproject.toml
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       38 2024-04-22 06:49:00.499660 ropt-0.1.2/setup.cfg
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.455660 ropt-0.1.2/src/
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.467660 ropt-0.1.2/src/ropt/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       73 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/__init__.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.467660 ropt-0.1.2/src/ropt/apps/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      143 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/apps/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    17499 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/apps/_script_optimizer.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.467660 ropt-0.1.2/src/ropt/config/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       68 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/__init__.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.471660 ropt-0.1.2/src/ropt/config/enopt/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      993 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      355 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_enopt_base_model.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     9167 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_enopt_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1997 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_function_transform_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6187 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_gradient_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3401 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_linear_constraints_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5071 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_nonlinear_constraints_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4514 2024-04-19 09:03:57.000000 ropt-0.1.2/src/ropt/config/enopt/_objective_functions_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4332 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_optimizer_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2161 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_realization_filter_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3532 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_realizations_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2351 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_sampler_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3890 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_utils.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     8285 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/_variables_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      952 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/enopt/constants.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.471660 ropt-0.1.2/src/ropt/config/plan/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      688 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/plan/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5115 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/plan/_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      574 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/plan/_plan_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      827 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/plan/_step_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5130 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/config/utils.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5477 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/enums.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.475660 ropt-0.1.2/src/ropt/evaluator/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2527 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/evaluator/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     7214 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/evaluator/_concurrent.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    25277 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/evaluator/_ensemble_evaluator.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5969 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/evaluator/_evaluator.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     8928 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/evaluator/_evaluator_results.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2207 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/evaluator/_function.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     8461 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/evaluator/_gradient.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      862 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/evaluator/_utils.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5297 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/evaluator/parsl.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1349 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/events.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      735 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/exceptions.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.475660 ropt-0.1.2/src/ropt/optimization/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      433 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/optimization/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2870 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/optimization/_bases.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4909 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/optimization/_ensemble_optimizer.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      771 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/optimization/_events.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     9297 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/optimization/_optimizer.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6893 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/optimization/_plan.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.475660 ropt-0.1.2/src/ropt/plugins/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1744 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5950 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/_manager.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.479660 ropt-0.1.2/src/ropt/plugins/function_transform/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      210 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/function_transform/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5528 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/function_transform/default.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2600 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/function_transform/protocol.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.479660 ropt-0.1.2/src/ropt/plugins/optimization_steps/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      138 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimization_steps/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2911 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimization_steps/_utils.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1792 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimization_steps/default.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1022 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimization_steps/enopt_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3890 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimization_steps/evaluator.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      748 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimization_steps/label.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4570 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimization_steps/optimizer.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      905 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimization_steps/reset_tracker.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1630 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimization_steps/restart.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2949 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimization_steps/tracker.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1843 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimization_steps/update_config.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.483660 ropt-0.1.2/src/ropt/plugins/optimizer/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1001 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimizer/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4249 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimizer/protocol.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    20113 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimizer/scipy.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     7969 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/optimizer/utils.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.483660 ropt-0.1.2/src/ropt/plugins/realization_filter/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      521 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/realization_filter/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    15031 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/realization_filter/default.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2096 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/realization_filter/protocol.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.483660 ropt-0.1.2/src/ropt/plugins/sampler/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      641 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/sampler/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3555 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/sampler/protocol.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6798 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/plugins/sampler/scipy.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/py.typed
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.483660 ropt-0.1.2/src/ropt/report/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      573 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/report/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     7603 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/report/_data_frame.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5295 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/report/_table.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4065 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/report/_utils.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.487660 ropt-0.1.2/src/ropt/results/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3953 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6147 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_bound_constraints.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5792 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_function_evaluations.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3571 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_function_results.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4229 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_functions.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3377 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_gradient_evaluations.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2879 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_gradient_results.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1969 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_gradients.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2571 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_linear_constraints.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2684 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_maximize.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4262 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_nonlinear_constraints.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3509 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_pandas.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2141 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_realizations.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1235 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_result_field.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     9252 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_results.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3523 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_utils.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4287 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/results/_xarray.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.491660 ropt-0.1.2/src/ropt/utils/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      169 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/utils/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      712 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/utils/_misc.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5351 2024-04-19 08:53:50.000000 ropt-0.1.2/src/ropt/utils/scaling.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      411 2024-04-22 06:49:00.000000 ropt-0.1.2/src/ropt/version.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.495660 ropt-0.1.2/src/ropt.egg-info/
+-rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     3159 2024-04-22 06:49:00.000000 ropt-0.1.2/src/ropt.egg-info/PKG-INFO
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5080 2024-04-22 06:49:00.000000 ropt-0.1.2/src/ropt.egg-info/SOURCES.txt
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        1 2024-04-22 06:49:00.000000 ropt-0.1.2/src/ropt.egg-info/dependency_links.txt
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      275 2024-04-22 06:49:00.000000 ropt-0.1.2/src/ropt.egg-info/requires.txt
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        5 2024-04-22 06:49:00.000000 ropt-0.1.2/src/ropt.egg-info/top_level.txt
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:49:00.495660 ropt-0.1.2/tests/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2023-10-10 07:53:14.000000 ropt-0.1.2/tests/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4505 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/conftest.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3811 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_concurrent.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    25786 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_config.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     9209 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_ensemble_gradient.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1775 2024-02-02 10:54:40.000000 ropt-0.1.2/tests/test_examples.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2185 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_failed_realizations.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4205 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_function_transforms.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5503 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_netcdf.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    42608 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_optimizer.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     7387 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_pandas.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4626 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_parsl.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    27696 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_realization_filters.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6652 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_result_table.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     8616 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_results.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5248 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_results_data_frame.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     6602 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_samplers.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    19164 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_scipy_backend.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     4474 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_scipy_samplers.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     3197 2024-04-19 08:53:50.000000 ropt-0.1.2/tests/test_xarray.py
```

### Comparing `ropt-0.1.1/.github/workflows/build-docs.yml` & `ropt-0.1.2/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/.github/workflows/github-pages.yml` & `ropt-0.1.2/.github/workflows/github-pages.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/.github/workflows/static-checks.yml` & `ropt-0.1.2/.github/workflows/static-checks.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/.github/workflows/tests.yml` & `ropt-0.1.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/LICENSE` & `ropt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/PKG-INFO` & `ropt-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt
-Version: 0.1.1
+Version: 0.1.2
 Summary: The ropt ensemble optimizer module
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -41,32 +41,60 @@
 # `ropt`
 `ropt` is a Python module for running robust optimization workflows.
 
 `ropt` is developed by the Netherlands Organisation for Applied Scientific
 Research (TNO). All files in this repository are released under the GNU General
 Public License v3.0 (a copy is provided in the LICENSE file).
 
+Detailed documentation and examples can be found in the online manual (on
+[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
+Docs](https://ropt.readthedocs.io/)).
+
 ## Dependencies
 `ropt` has been tested with Python versions 3.8-3.12.
 
 `ropt` requires one or more optimization backends to function. A backend based
-on optimizers included in [SciPy](https://scipy.org/) is installed by default.
+on optimizers included with [SciPy](https://scipy.org/) is installed by default.
 
 ## Installation
+From PyPI:
 ```bash
 pip install ropt
 ```
 
-To enable some options, the following optional-dependencies can be installed:
+The following optional-dependencies can be installed:
 
 - `storage` : Enables `pandas`, `xarrays` and netCDF support.
 - `parsl`   : Enables the parsl-based evaluator functionality.
 
 To install both:
 ```bash
 pip install ropt[storage,parsl]
 ```
 
-## Documentation
-Detailed documentation and examples can be found in the online manual (on
-[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
-Docs](https://ropt.readthedocs.io/)).
+
+## Development
+The `ropt` source distribution can be found on
+[GitHub](https://github.com/tno-ropt/ropt). To install from source, enter the
+`ropt` distribution directory and execute:
+
+```bash
+pip install .
+```
+
+Documentation is written using [`MkDocs`](https://www.mkdocs.org/) and
+[`mkdocstrings`](https://mkdocstrings.github.io/). To view it, install the
+necessary dependencies and start the `MkDocs` built-in server within the `ropt`
+distribution directory:
+
+```bash
+pip install .[docs]
+mkdocs serve
+```
+
+## Running the tests
+To run the test suite, install the necessary dependencies and execute `pytest`:
+
+```bash
+pip install .[test]
+pytest
+```
```

### Comparing `ropt-0.1.1/README-PyPI.md` & `ropt-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,60 @@
 # `ropt`
 `ropt` is a Python module for running robust optimization workflows.
 
 `ropt` is developed by the Netherlands Organisation for Applied Scientific
 Research (TNO). All files in this repository are released under the GNU General
 Public License v3.0 (a copy is provided in the LICENSE file).
 
+Detailed documentation and examples can be found in the online manual (on
+[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
+Docs](https://ropt.readthedocs.io/)).
+
 ## Dependencies
 `ropt` has been tested with Python versions 3.8-3.12.
 
 `ropt` requires one or more optimization backends to function. A backend based
-on optimizers included in [SciPy](https://scipy.org/) is installed by default.
+on optimizers included with [SciPy](https://scipy.org/) is installed by default.
 
 ## Installation
+From PyPI:
 ```bash
 pip install ropt
 ```
 
-To enable some options, the following optional-dependencies can be installed:
+The following optional-dependencies can be installed:
 
 - `storage` : Enables `pandas`, `xarrays` and netCDF support.
 - `parsl`   : Enables the parsl-based evaluator functionality.
 
 To install both:
 ```bash
 pip install ropt[storage,parsl]
 ```
 
-## Documentation
-Detailed documentation and examples can be found in the online manual (on
-[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
-Docs](https://ropt.readthedocs.io/)).
+
+## Development
+The `ropt` source distribution can be found on
+[GitHub](https://github.com/tno-ropt/ropt). To install from source, enter the
+`ropt` distribution directory and execute:
+
+```bash
+pip install .
+```
+
+Documentation is written using [`MkDocs`](https://www.mkdocs.org/) and
+[`mkdocstrings`](https://mkdocstrings.github.io/). To view it, install the
+necessary dependencies and start the `MkDocs` built-in server within the `ropt`
+distribution directory:
+
+```bash
+pip install .[docs]
+mkdocs serve
+```
+
+## Running the tests
+To run the test suite, install the necessary dependencies and execute `pytest`:
+
+```bash
+pip install .[test]
+pytest
+```
```

### Comparing `ropt-0.1.1/docs/index.md` & `ropt-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/docs/reference/evaluator.md` & `ropt-0.1.2/docs/reference/evaluator.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/docs/reference/realization_filters.md` & `ropt-0.1.2/docs/reference/realization_filters.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/docs/reference/results.md` & `ropt-0.1.2/docs/reference/results.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/docs/usage/robust_optimization.md` & `ropt-0.1.2/docs/usage/robust_optimization.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/docs/usage/running.md` & `ropt-0.1.2/docs/usage/running.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/examples/de_linear.py` & `ropt-0.1.2/examples/de_linear.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/examples/de_nonlinear.py` & `ropt-0.1.2/examples/de_nonlinear.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/examples/rosenbrock_deterministic.py` & `ropt-0.1.2/examples/rosenbrock_deterministic.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/examples/rosenbrock_ensemble.py` & `ropt-0.1.2/examples/rosenbrock_ensemble.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/examples/script_optimizer/rosenbrock.py` & `ropt-0.1.2/examples/script_optimizer/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/examples/script_optimizer/run.py` & `ropt-0.1.2/examples/script_optimizer/run.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/mkdocs.yml` & `ropt-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/pyproject.toml` & `ropt-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ropt"
 description = "The ropt ensemble optimizer module"
-readme = "README-PyPI.md"
+readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `ropt-0.1.1/src/ropt/apps/_script_optimizer.py` & `ropt-0.1.2/src/ropt/apps/_script_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/__init__.py` & `ropt-0.1.2/src/ropt/config/enopt/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_enopt_config.py` & `ropt-0.1.2/src/ropt/config/enopt/_enopt_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_function_transform_config.py` & `ropt-0.1.2/src/ropt/config/enopt/_function_transform_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_gradient_config.py` & `ropt-0.1.2/src/ropt/config/enopt/_gradient_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_linear_constraints_config.py` & `ropt-0.1.2/src/ropt/config/enopt/_linear_constraints_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_nonlinear_constraints_config.py` & `ropt-0.1.2/src/ropt/config/enopt/_nonlinear_constraints_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_objective_functions_config.py` & `ropt-0.1.2/src/ropt/config/enopt/_objective_functions_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_optimizer_config.py` & `ropt-0.1.2/src/ropt/config/enopt/_optimizer_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_realization_filter_config.py` & `ropt-0.1.2/src/ropt/config/enopt/_realization_filter_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_realizations_config.py` & `ropt-0.1.2/src/ropt/config/enopt/_realizations_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_sampler_config.py` & `ropt-0.1.2/src/ropt/config/enopt/_sampler_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_utils.py` & `ropt-0.1.2/src/ropt/config/enopt/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/_variables_config.py` & `ropt-0.1.2/src/ropt/config/enopt/_variables_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/enopt/constants.py` & `ropt-0.1.2/src/ropt/config/enopt/constants.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/plan/__init__.py` & `ropt-0.1.2/src/ropt/config/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/plan/_config.py` & `ropt-0.1.2/src/ropt/config/plan/_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/plan/_plan_config.py` & `ropt-0.1.2/src/ropt/config/plan/_plan_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/plan/_step_config.py` & `ropt-0.1.2/src/ropt/config/plan/_step_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/config/utils.py` & `ropt-0.1.2/src/ropt/config/utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/enums.py` & `ropt-0.1.2/src/ropt/enums.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/evaluator/__init__.py` & `ropt-0.1.2/src/ropt/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/evaluator/_concurrent.py` & `ropt-0.1.2/src/ropt/evaluator/_concurrent.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/evaluator/_ensemble_evaluator.py` & `ropt-0.1.2/src/ropt/evaluator/_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/evaluator/_evaluator.py` & `ropt-0.1.2/src/ropt/evaluator/_evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/evaluator/_evaluator_results.py` & `ropt-0.1.2/src/ropt/evaluator/_evaluator_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/evaluator/_function.py` & `ropt-0.1.2/src/ropt/evaluator/_function.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/evaluator/_gradient.py` & `ropt-0.1.2/src/ropt/evaluator/_gradient.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/evaluator/_utils.py` & `ropt-0.1.2/src/ropt/evaluator/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/evaluator/parsl.py` & `ropt-0.1.2/src/ropt/evaluator/parsl.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/events.py` & `ropt-0.1.2/src/ropt/events.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/exceptions.py` & `ropt-0.1.2/src/ropt/exceptions.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/optimization/_bases.py` & `ropt-0.1.2/src/ropt/optimization/_bases.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/optimization/_ensemble_optimizer.py` & `ropt-0.1.2/src/ropt/optimization/_ensemble_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/optimization/_events.py` & `ropt-0.1.2/src/ropt/optimization/_events.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/optimization/_optimizer.py` & `ropt-0.1.2/src/ropt/optimization/_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/optimization/_plan.py` & `ropt-0.1.2/src/ropt/optimization/_plan.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/__init__.py` & `ropt-0.1.2/src/ropt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/_manager.py` & `ropt-0.1.2/src/ropt/plugins/_manager.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/function_transform/default.py` & `ropt-0.1.2/src/ropt/plugins/function_transform/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/function_transform/protocol.py` & `ropt-0.1.2/src/ropt/plugins/function_transform/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimization_steps/_utils.py` & `ropt-0.1.2/src/ropt/plugins/optimization_steps/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimization_steps/default.py` & `ropt-0.1.2/src/ropt/plugins/optimization_steps/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimization_steps/enopt_config.py` & `ropt-0.1.2/src/ropt/plugins/optimization_steps/enopt_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimization_steps/evaluator.py` & `ropt-0.1.2/src/ropt/plugins/optimization_steps/evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimization_steps/label.py` & `ropt-0.1.2/src/ropt/plugins/optimization_steps/label.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimization_steps/optimizer.py` & `ropt-0.1.2/src/ropt/plugins/optimization_steps/optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimization_steps/reset_tracker.py` & `ropt-0.1.2/src/ropt/plugins/optimization_steps/reset_tracker.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimization_steps/restart.py` & `ropt-0.1.2/src/ropt/plugins/optimization_steps/restart.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimization_steps/tracker.py` & `ropt-0.1.2/src/ropt/plugins/optimization_steps/tracker.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimization_steps/update_config.py` & `ropt-0.1.2/src/ropt/plugins/optimization_steps/update_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimizer/__init__.py` & `ropt-0.1.2/src/ropt/plugins/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimizer/protocol.py` & `ropt-0.1.2/src/ropt/plugins/optimizer/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimizer/scipy.py` & `ropt-0.1.2/src/ropt/plugins/optimizer/scipy.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/optimizer/utils.py` & `ropt-0.1.2/src/ropt/plugins/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/realization_filter/__init__.py` & `ropt-0.1.2/src/ropt/plugins/realization_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/realization_filter/default.py` & `ropt-0.1.2/src/ropt/plugins/realization_filter/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/realization_filter/protocol.py` & `ropt-0.1.2/src/ropt/plugins/realization_filter/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/sampler/__init__.py` & `ropt-0.1.2/src/ropt/plugins/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/sampler/protocol.py` & `ropt-0.1.2/src/ropt/plugins/sampler/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/plugins/sampler/scipy.py` & `ropt-0.1.2/src/ropt/plugins/sampler/scipy.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/report/__init__.py` & `ropt-0.1.2/src/ropt/report/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/report/_data_frame.py` & `ropt-0.1.2/src/ropt/report/_data_frame.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/report/_table.py` & `ropt-0.1.2/src/ropt/report/_table.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/report/_utils.py` & `ropt-0.1.2/src/ropt/report/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/__init__.py` & `ropt-0.1.2/src/ropt/results/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_bound_constraints.py` & `ropt-0.1.2/src/ropt/results/_bound_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_function_evaluations.py` & `ropt-0.1.2/src/ropt/results/_function_evaluations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_function_results.py` & `ropt-0.1.2/src/ropt/results/_function_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_functions.py` & `ropt-0.1.2/src/ropt/results/_functions.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_gradient_evaluations.py` & `ropt-0.1.2/src/ropt/results/_gradient_evaluations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_gradient_results.py` & `ropt-0.1.2/src/ropt/results/_gradient_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_gradients.py` & `ropt-0.1.2/src/ropt/results/_gradients.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_linear_constraints.py` & `ropt-0.1.2/src/ropt/results/_linear_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_maximize.py` & `ropt-0.1.2/src/ropt/results/_maximize.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_nonlinear_constraints.py` & `ropt-0.1.2/src/ropt/results/_nonlinear_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_pandas.py` & `ropt-0.1.2/src/ropt/results/_pandas.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_realizations.py` & `ropt-0.1.2/src/ropt/results/_realizations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_result_field.py` & `ropt-0.1.2/src/ropt/results/_result_field.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_results.py` & `ropt-0.1.2/src/ropt/results/_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_utils.py` & `ropt-0.1.2/src/ropt/results/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/results/_xarray.py` & `ropt-0.1.2/src/ropt/results/_xarray.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/utils/_misc.py` & `ropt-0.1.2/src/ropt/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt/utils/scaling.py` & `ropt-0.1.2/src/ropt/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/src/ropt.egg-info/PKG-INFO` & `ropt-0.1.2/src/ropt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt
-Version: 0.1.1
+Version: 0.1.2
 Summary: The ropt ensemble optimizer module
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -41,32 +41,60 @@
 # `ropt`
 `ropt` is a Python module for running robust optimization workflows.
 
 `ropt` is developed by the Netherlands Organisation for Applied Scientific
 Research (TNO). All files in this repository are released under the GNU General
 Public License v3.0 (a copy is provided in the LICENSE file).
 
+Detailed documentation and examples can be found in the online manual (on
+[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
+Docs](https://ropt.readthedocs.io/)).
+
 ## Dependencies
 `ropt` has been tested with Python versions 3.8-3.12.
 
 `ropt` requires one or more optimization backends to function. A backend based
-on optimizers included in [SciPy](https://scipy.org/) is installed by default.
+on optimizers included with [SciPy](https://scipy.org/) is installed by default.
 
 ## Installation
+From PyPI:
 ```bash
 pip install ropt
 ```
 
-To enable some options, the following optional-dependencies can be installed:
+The following optional-dependencies can be installed:
 
 - `storage` : Enables `pandas`, `xarrays` and netCDF support.
 - `parsl`   : Enables the parsl-based evaluator functionality.
 
 To install both:
 ```bash
 pip install ropt[storage,parsl]
 ```
 
-## Documentation
-Detailed documentation and examples can be found in the online manual (on
-[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
-Docs](https://ropt.readthedocs.io/)).
+
+## Development
+The `ropt` source distribution can be found on
+[GitHub](https://github.com/tno-ropt/ropt). To install from source, enter the
+`ropt` distribution directory and execute:
+
+```bash
+pip install .
+```
+
+Documentation is written using [`MkDocs`](https://www.mkdocs.org/) and
+[`mkdocstrings`](https://mkdocstrings.github.io/). To view it, install the
+necessary dependencies and start the `MkDocs` built-in server within the `ropt`
+distribution directory:
+
+```bash
+pip install .[docs]
+mkdocs serve
+```
+
+## Running the tests
+To run the test suite, install the necessary dependencies and execute `pytest`:
+
+```bash
+pip install .[test]
+pytest
+```
```

### Comparing `ropt-0.1.1/src/ropt.egg-info/SOURCES.txt` & `ropt-0.1.2/src/ropt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .gitignore
 .readthedocs.yaml
 LICENSE
-README-PyPI.md
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/build-docs.yml
 .github/workflows/github-pages.yml
 .github/workflows/static-checks.yml
 .github/workflows/tests.yml
```

### Comparing `ropt-0.1.1/tests/conftest.py` & `ropt-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_concurrent.py` & `ropt-0.1.2/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_config.py` & `ropt-0.1.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_ensemble_gradient.py` & `ropt-0.1.2/tests/test_ensemble_gradient.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_examples.py` & `ropt-0.1.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_failed_realizations.py` & `ropt-0.1.2/tests/test_failed_realizations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_function_transforms.py` & `ropt-0.1.2/tests/test_function_transforms.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_netcdf.py` & `ropt-0.1.2/tests/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_optimizer.py` & `ropt-0.1.2/tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_pandas.py` & `ropt-0.1.2/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_parsl.py` & `ropt-0.1.2/tests/test_parsl.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_realization_filters.py` & `ropt-0.1.2/tests/test_realization_filters.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_result_table.py` & `ropt-0.1.2/tests/test_result_table.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_results.py` & `ropt-0.1.2/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_results_data_frame.py` & `ropt-0.1.2/tests/test_results_data_frame.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_samplers.py` & `ropt-0.1.2/tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_scipy_backend.py` & `ropt-0.1.2/tests/test_scipy_backend.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_scipy_samplers.py` & `ropt-0.1.2/tests/test_scipy_samplers.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.1/tests/test_xarray.py` & `ropt-0.1.2/tests/test_xarray.py`

 * *Files identical despite different names*


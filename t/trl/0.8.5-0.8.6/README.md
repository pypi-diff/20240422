# Comparing `tmp/trl-0.8.5.tar.gz` & `tmp/trl-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trl-0.8.5.tar", last modified: Thu Apr 18 11:54:45 2024, max compression
+gzip compressed data, was "trl-0.8.6.tar", last modified: Mon Apr 22 08:56:10 2024, max compression
```

## Comparing `trl-0.8.5.tar` & `trl-0.8.6.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.106394 trl-0.8.5/
--rw-rw-r--   0 younes   (150078) younes   (150078)     2507 2024-04-12 10:22:24.000000 trl-0.8.5/CONTRIBUTING.md
--rw-rw-r--   0 younes   (150078) younes   (150078)    11357 2023-06-01 10:19:35.000000 trl-0.8.5/LICENSE
--rw-rw-r--   0 younes   (150078) younes   (150078)      110 2024-04-12 10:22:24.000000 trl-0.8.5/MANIFEST.in
--rw-rw-r--   0 younes   (150078) younes   (150078)    10388 2024-04-18 11:54:45.106394 trl-0.8.5/PKG-INFO
--rw-rw-r--   0 younes   (150078) younes   (150078)     9273 2024-04-12 10:22:24.000000 trl-0.8.5/README.md
--rw-rw-r--   0 younes   (150078) younes   (150078)      509 2024-04-12 10:22:24.000000 trl-0.8.5/pyproject.toml
--rw-rw-r--   0 younes   (150078) younes   (150078)       73 2024-04-18 11:54:45.106394 trl-0.8.5/setup.cfg
--rw-rw-r--   0 younes   (150078) younes   (150078)     4547 2024-04-18 11:53:34.000000 trl-0.8.5/setup.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.098394 trl-0.8.5/tests/
--rw-rw-r--   0 younes   (150078) younes   (150078)        0 2023-06-01 10:19:35.000000 trl-0.8.5/tests/__init__.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.098394 trl-0.8.5/tests/slow/
--rw-rw-r--   0 younes   (150078) younes   (150078)        0 2024-01-30 06:55:37.000000 trl-0.8.5/tests/slow/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     7757 2024-04-12 10:22:24.000000 trl-0.8.5/tests/slow/test_dpo_slow.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    14741 2024-04-12 10:22:24.000000 trl-0.8.5/tests/slow/test_sft_slow.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1082 2024-01-30 06:55:37.000000 trl-0.8.5/tests/slow/testing_constants.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3158 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_best_of_n_sampler.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1749 2024-04-17 15:11:50.000000 trl-0.8.5/tests/test_cli.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1545 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_core.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6283 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_cpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     5505 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_data_collator_completion_only.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6894 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_dataset_formatting.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4168 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_ddpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    22515 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_dpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)      152 2023-09-22 13:56:18.000000 trl-0.8.5/tests/test_e2e.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    11127 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_environments.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4597 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_iterative_sft_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    14983 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_kto_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    22746 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_modeling_value_head.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     5560 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_no_peft.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6119 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_orpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     9122 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_peft_models.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    49544 2024-04-17 15:11:50.000000 trl-0.8.5/tests/test_ppo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    13419 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_reward_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1640 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_rich_progress_callback.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    43099 2024-04-12 10:22:24.000000 trl-0.8.5/tests/test_sft_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)      799 2023-06-01 10:19:35.000000 trl-0.8.5/tests/testing_constants.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3342 2024-04-12 10:22:24.000000 trl-0.8.5/tests/testing_utils.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.098394 trl-0.8.5/trl/
--rw-rw-r--   0 younes   (150078) younes   (150078)     3931 2024-04-18 11:53:30.000000 trl-0.8.5/trl/__init__.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.102394 trl-0.8.5/trl/commands/
--rw-rw-r--   0 younes   (150078) younes   (150078)     1207 2024-04-12 10:22:24.000000 trl-0.8.5/trl/commands/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     2367 2024-04-12 10:22:24.000000 trl-0.8.5/trl/commands/cli.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    14297 2024-04-18 11:53:05.000000 trl-0.8.5/trl/commands/cli_utils.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.102394 trl-0.8.5/trl/commands/scripts/
--rw-rw-r--   0 younes   (150078) younes   (150078)    13309 2024-04-18 11:53:05.000000 trl-0.8.5/trl/commands/scripts/chat.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.102394 trl-0.8.5/trl/commands/scripts/config/
--rw-rw-r--   0 younes   (150078) younes   (150078)      487 2024-04-12 10:22:24.000000 trl-0.8.5/trl/commands/scripts/config/default_chat_config.yaml
--rw-rw-r--   0 younes   (150078) younes   (150078)     4003 2024-04-12 10:22:24.000000 trl-0.8.5/trl/commands/scripts/cpo.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6500 2024-04-12 10:22:24.000000 trl-0.8.5/trl/commands/scripts/ddpo.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6054 2024-04-12 10:22:24.000000 trl-0.8.5/trl/commands/scripts/dpo.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3729 2024-04-12 10:22:24.000000 trl-0.8.5/trl/commands/scripts/kto.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4057 2024-04-12 10:22:24.000000 trl-0.8.5/trl/commands/scripts/orpo.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     7646 2024-04-12 10:22:24.000000 trl-0.8.5/trl/commands/scripts/ppo.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     5261 2024-04-12 10:22:24.000000 trl-0.8.5/trl/commands/scripts/ppo_multi_adapter.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4596 2024-04-12 10:22:24.000000 trl-0.8.5/trl/commands/scripts/reward_modeling.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4763 2024-04-18 11:53:05.000000 trl-0.8.5/trl/commands/scripts/sft.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     7657 2024-04-17 15:11:50.000000 trl-0.8.5/trl/commands/scripts/vsft_llava.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    12148 2024-04-12 10:22:24.000000 trl-0.8.5/trl/core.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.102394 trl-0.8.5/trl/environment/
--rw-rw-r--   0 younes   (150078) younes   (150078)      390 2024-04-12 10:22:24.000000 trl-0.8.5/trl/environment/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    17569 2024-04-12 10:22:24.000000 trl-0.8.5/trl/environment/base_environment.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.102394 trl-0.8.5/trl/extras/
--rw-rw-r--   0 younes   (150078) younes   (150078)      971 2024-04-12 10:22:24.000000 trl-0.8.5/trl/extras/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     5182 2024-04-12 10:22:24.000000 trl-0.8.5/trl/extras/best_of_n_sampler.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3646 2024-01-30 06:55:37.000000 trl-0.8.5/trl/extras/dataset_formatting.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6079 2024-04-12 10:22:24.000000 trl-0.8.5/trl/import_utils.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.102394 trl-0.8.5/trl/models/
--rw-rw-r--   0 younes   (150078) younes   (150078)     2208 2024-04-12 10:22:24.000000 trl-0.8.5/trl/models/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    28788 2024-04-12 10:22:24.000000 trl-0.8.5/trl/models/modeling_base.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    27695 2024-04-12 10:22:24.000000 trl-0.8.5/trl/models/modeling_sd_base.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    18933 2024-04-12 10:22:24.000000 trl-0.8.5/trl/models/modeling_value_head.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     5874 2024-04-12 10:22:24.000000 trl-0.8.5/trl/models/sd_utils.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6026 2024-04-12 10:22:24.000000 trl-0.8.5/trl/models/utils.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.106394 trl-0.8.5/trl/trainer/
--rw-rw-r--   0 younes   (150078) younes   (150078)     3343 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1772 2023-06-01 10:19:35.000000 trl-0.8.5/trl/trainer/base.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3875 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/cpo_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    44127 2024-04-17 15:11:50.000000 trl-0.8.5/trl/trainer/cpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4891 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/ddpo_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    26796 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/ddpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    62510 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/dpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    16699 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/iterative_sft_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4970 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/kto_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    64532 2024-04-17 15:11:50.000000 trl-0.8.5/trl/trainer/kto_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3297 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/model_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3500 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/orpo_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    45703 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/orpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     8202 2024-01-30 06:55:37.000000 trl-0.8.5/trl/trainer/ppo_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    63096 2024-04-17 15:11:50.000000 trl-0.8.5/trl/trainer/ppo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1623 2024-01-30 06:55:37.000000 trl-0.8.5/trl/trainer/reward_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    14097 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/reward_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    27414 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/sft_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    35309 2024-04-12 10:22:24.000000 trl-0.8.5/trl/trainer/utils.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-18 11:54:45.098394 trl-0.8.5/trl.egg-info/
--rw-r--r--   0 younes   (150078) younes   (150078)    10388 2024-04-18 11:54:45.000000 trl-0.8.5/trl.egg-info/PKG-INFO
--rw-rw-r--   0 younes   (150078) younes   (150078)     2346 2024-04-18 11:54:45.000000 trl-0.8.5/trl.egg-info/SOURCES.txt
--rw-rw-r--   0 younes   (150078) younes   (150078)        1 2024-04-18 11:54:45.000000 trl-0.8.5/trl.egg-info/dependency_links.txt
--rw-rw-r--   0 younes   (150078) younes   (150078)       46 2024-04-18 11:54:45.000000 trl-0.8.5/trl.egg-info/entry_points.txt
--rw-rw-r--   0 younes   (150078) younes   (150078)        1 2023-06-01 10:19:45.000000 trl-0.8.5/trl.egg-info/not-zip-safe
--rw-rw-r--   0 younes   (150078) younes   (150078)      519 2024-04-18 11:54:45.000000 trl-0.8.5/trl.egg-info/requires.txt
--rw-rw-r--   0 younes   (150078) younes   (150078)       10 2024-04-18 11:54:45.000000 trl-0.8.5/trl.egg-info/top_level.txt
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.730500 trl-0.8.6/
+-rw-rw-r--   0 younes   (150078) younes   (150078)     2507 2024-04-12 10:22:24.000000 trl-0.8.6/CONTRIBUTING.md
+-rw-rw-r--   0 younes   (150078) younes   (150078)    11357 2023-06-01 10:19:35.000000 trl-0.8.6/LICENSE
+-rw-rw-r--   0 younes   (150078) younes   (150078)      110 2024-04-12 10:22:24.000000 trl-0.8.6/MANIFEST.in
+-rw-rw-r--   0 younes   (150078) younes   (150078)    10388 2024-04-22 08:56:10.730500 trl-0.8.6/PKG-INFO
+-rw-rw-r--   0 younes   (150078) younes   (150078)     9273 2024-04-12 10:22:24.000000 trl-0.8.6/README.md
+-rw-rw-r--   0 younes   (150078) younes   (150078)      509 2024-04-12 10:22:24.000000 trl-0.8.6/pyproject.toml
+-rw-rw-r--   0 younes   (150078) younes   (150078)       73 2024-04-22 08:56:10.730500 trl-0.8.6/setup.cfg
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4547 2024-04-22 08:50:01.000000 trl-0.8.6/setup.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.722500 trl-0.8.6/tests/
+-rw-rw-r--   0 younes   (150078) younes   (150078)        0 2023-06-01 10:19:35.000000 trl-0.8.6/tests/__init__.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.722500 trl-0.8.6/tests/slow/
+-rw-rw-r--   0 younes   (150078) younes   (150078)        0 2024-01-30 06:55:37.000000 trl-0.8.6/tests/slow/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     7757 2024-04-12 10:22:24.000000 trl-0.8.6/tests/slow/test_dpo_slow.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    14741 2024-04-12 10:22:24.000000 trl-0.8.6/tests/slow/test_sft_slow.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1082 2024-01-30 06:55:37.000000 trl-0.8.6/tests/slow/testing_constants.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3158 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_best_of_n_sampler.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1749 2024-04-17 15:11:50.000000 trl-0.8.6/tests/test_cli.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1545 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_core.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6283 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_cpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     5505 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_data_collator_completion_only.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6894 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_dataset_formatting.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4168 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_ddpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    22515 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_dpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)      152 2023-09-22 13:56:18.000000 trl-0.8.6/tests/test_e2e.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    11127 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_environments.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4597 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_iterative_sft_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    14983 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_kto_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    22746 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_modeling_value_head.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     5560 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_no_peft.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6119 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_orpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     9122 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_peft_models.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    49544 2024-04-17 15:11:50.000000 trl-0.8.6/tests/test_ppo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    13419 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_reward_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1640 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_rich_progress_callback.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    43099 2024-04-12 10:22:24.000000 trl-0.8.6/tests/test_sft_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)      799 2023-06-01 10:19:35.000000 trl-0.8.6/tests/testing_constants.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3342 2024-04-12 10:22:24.000000 trl-0.8.6/tests/testing_utils.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.722500 trl-0.8.6/trl/
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3931 2024-04-22 08:50:04.000000 trl-0.8.6/trl/__init__.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.726500 trl-0.8.6/trl/commands/
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1154 2024-04-18 12:52:30.000000 trl-0.8.6/trl/commands/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     2367 2024-04-12 10:22:24.000000 trl-0.8.6/trl/commands/cli.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    14958 2024-04-22 08:49:39.000000 trl-0.8.6/trl/commands/cli_utils.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.726500 trl-0.8.6/trl/commands/scripts/
+-rw-rw-r--   0 younes   (150078) younes   (150078)    13309 2024-04-18 11:53:05.000000 trl-0.8.6/trl/commands/scripts/chat.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.726500 trl-0.8.6/trl/commands/scripts/config/
+-rw-rw-r--   0 younes   (150078) younes   (150078)      487 2024-04-12 10:22:24.000000 trl-0.8.6/trl/commands/scripts/config/default_chat_config.yaml
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4003 2024-04-12 10:22:24.000000 trl-0.8.6/trl/commands/scripts/cpo.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6500 2024-04-12 10:22:24.000000 trl-0.8.6/trl/commands/scripts/ddpo.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6054 2024-04-12 10:22:24.000000 trl-0.8.6/trl/commands/scripts/dpo.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3729 2024-04-12 10:22:24.000000 trl-0.8.6/trl/commands/scripts/kto.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4057 2024-04-12 10:22:24.000000 trl-0.8.6/trl/commands/scripts/orpo.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     7646 2024-04-12 10:22:24.000000 trl-0.8.6/trl/commands/scripts/ppo.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     5261 2024-04-12 10:22:24.000000 trl-0.8.6/trl/commands/scripts/ppo_multi_adapter.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4596 2024-04-12 10:22:24.000000 trl-0.8.6/trl/commands/scripts/reward_modeling.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4763 2024-04-18 11:53:05.000000 trl-0.8.6/trl/commands/scripts/sft.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     7657 2024-04-17 15:11:50.000000 trl-0.8.6/trl/commands/scripts/vsft_llava.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    12148 2024-04-12 10:22:24.000000 trl-0.8.6/trl/core.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.726500 trl-0.8.6/trl/environment/
+-rw-rw-r--   0 younes   (150078) younes   (150078)      390 2024-04-12 10:22:24.000000 trl-0.8.6/trl/environment/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    17569 2024-04-12 10:22:24.000000 trl-0.8.6/trl/environment/base_environment.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.726500 trl-0.8.6/trl/extras/
+-rw-rw-r--   0 younes   (150078) younes   (150078)      971 2024-04-12 10:22:24.000000 trl-0.8.6/trl/extras/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     5182 2024-04-12 10:22:24.000000 trl-0.8.6/trl/extras/best_of_n_sampler.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3646 2024-01-30 06:55:37.000000 trl-0.8.6/trl/extras/dataset_formatting.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6079 2024-04-12 10:22:24.000000 trl-0.8.6/trl/import_utils.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.726500 trl-0.8.6/trl/models/
+-rw-rw-r--   0 younes   (150078) younes   (150078)     2208 2024-04-12 10:22:24.000000 trl-0.8.6/trl/models/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    28788 2024-04-12 10:22:24.000000 trl-0.8.6/trl/models/modeling_base.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    27695 2024-04-12 10:22:24.000000 trl-0.8.6/trl/models/modeling_sd_base.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    18933 2024-04-12 10:22:24.000000 trl-0.8.6/trl/models/modeling_value_head.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     5874 2024-04-12 10:22:24.000000 trl-0.8.6/trl/models/sd_utils.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6026 2024-04-12 10:22:24.000000 trl-0.8.6/trl/models/utils.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.730500 trl-0.8.6/trl/trainer/
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3343 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1772 2023-06-01 10:19:35.000000 trl-0.8.6/trl/trainer/base.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3875 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/cpo_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    44127 2024-04-17 15:11:50.000000 trl-0.8.6/trl/trainer/cpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4891 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/ddpo_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    26796 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/ddpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    62510 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/dpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    16699 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/iterative_sft_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4970 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/kto_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    64532 2024-04-17 15:11:50.000000 trl-0.8.6/trl/trainer/kto_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3297 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/model_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3500 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/orpo_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    45703 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/orpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     8202 2024-01-30 06:55:37.000000 trl-0.8.6/trl/trainer/ppo_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    63096 2024-04-17 15:11:50.000000 trl-0.8.6/trl/trainer/ppo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1623 2024-01-30 06:55:37.000000 trl-0.8.6/trl/trainer/reward_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    14097 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/reward_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    27414 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/sft_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    35309 2024-04-12 10:22:24.000000 trl-0.8.6/trl/trainer/utils.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-22 08:56:10.726500 trl-0.8.6/trl.egg-info/
+-rw-r--r--   0 younes   (150078) younes   (150078)    10388 2024-04-22 08:56:10.000000 trl-0.8.6/trl.egg-info/PKG-INFO
+-rw-rw-r--   0 younes   (150078) younes   (150078)     2346 2024-04-22 08:56:10.000000 trl-0.8.6/trl.egg-info/SOURCES.txt
+-rw-rw-r--   0 younes   (150078) younes   (150078)        1 2024-04-22 08:56:10.000000 trl-0.8.6/trl.egg-info/dependency_links.txt
+-rw-rw-r--   0 younes   (150078) younes   (150078)       46 2024-04-22 08:56:10.000000 trl-0.8.6/trl.egg-info/entry_points.txt
+-rw-rw-r--   0 younes   (150078) younes   (150078)        1 2023-06-01 10:19:45.000000 trl-0.8.6/trl.egg-info/not-zip-safe
+-rw-rw-r--   0 younes   (150078) younes   (150078)      519 2024-04-22 08:56:10.000000 trl-0.8.6/trl.egg-info/requires.txt
+-rw-rw-r--   0 younes   (150078) younes   (150078)       10 2024-04-22 08:56:10.000000 trl-0.8.6/trl.egg-info/top_level.txt
```

### Comparing `trl-0.8.5/CONTRIBUTING.md` & `trl-0.8.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/LICENSE` & `trl-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/PKG-INFO` & `trl-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trl
-Version: 0.8.5
+Version: 0.8.6
 Summary: Train transformer language models with reinforcement learning.
 Home-page: https://github.com/huggingface/trl
 Author: Leandro von Werra
 Author-email: leandro.vonwerra@gmail.com
 License: Apache 2.0
 Keywords: ppo,transformers,huggingface,gpt2,language modeling,rlhf
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trl Version: 0.8.5 Summary: Train transformer
+Metadata-Version: 2.1 Name: trl Version: 0.8.6 Summary: Train transformer
 language models with reinforcement learning. Home-page: https://github.com/
 huggingface/trl Author: Leandro von Werra Author-email:
 leandro.vonwerra@gmail.com License: Apache 2.0 Keywords:
 ppo,transformers,huggingface,gpt2,language modeling,rlhf Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
```

### Comparing `trl-0.8.5/README.md` & `trl-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/setup.py` & `trl-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
    Then push the change with a message 'set dev version'
 """
 import os
 
 from setuptools import find_packages, setup
 
 
-__version__ = "0.8.5"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+__version__ = "0.8.6"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
 
 REQUIRED_PKGS = [
     "torch>=1.4.0",
     "transformers>=4.31.0",
     "numpy>=1.18.2",
     "accelerate",
     "datasets",
```

### Comparing `trl-0.8.5/tests/slow/test_dpo_slow.py` & `trl-0.8.6/tests/slow/test_dpo_slow.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/slow/test_sft_slow.py` & `trl-0.8.6/tests/slow/test_sft_slow.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/slow/testing_constants.py` & `trl-0.8.6/tests/slow/testing_constants.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_best_of_n_sampler.py` & `trl-0.8.6/tests/test_best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_cli.py` & `trl-0.8.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_core.py` & `trl-0.8.6/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_cpo_trainer.py` & `trl-0.8.6/tests/test_cpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_data_collator_completion_only.py` & `trl-0.8.6/tests/test_data_collator_completion_only.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_dataset_formatting.py` & `trl-0.8.6/tests/test_dataset_formatting.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_ddpo_trainer.py` & `trl-0.8.6/tests/test_ddpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_dpo_trainer.py` & `trl-0.8.6/tests/test_dpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_environments.py` & `trl-0.8.6/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_iterative_sft_trainer.py` & `trl-0.8.6/tests/test_iterative_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_kto_trainer.py` & `trl-0.8.6/tests/test_kto_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_modeling_value_head.py` & `trl-0.8.6/tests/test_modeling_value_head.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_no_peft.py` & `trl-0.8.6/tests/test_no_peft.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_orpo_trainer.py` & `trl-0.8.6/tests/test_orpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_peft_models.py` & `trl-0.8.6/tests/test_peft_models.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_ppo_trainer.py` & `trl-0.8.6/tests/test_ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_reward_trainer.py` & `trl-0.8.6/tests/test_reward_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_rich_progress_callback.py` & `trl-0.8.6/tests/test_rich_progress_callback.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/test_sft_trainer.py` & `trl-0.8.6/tests/test_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/testing_constants.py` & `trl-0.8.6/tests/testing_constants.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/tests/testing_utils.py` & `trl-0.8.6/tests/testing_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/__init__.py` & `trl-0.8.6/trl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa
 
-__version__ = "0.8.5"
+__version__ = "0.8.6"
 
 from typing import TYPE_CHECKING
 from .import_utils import _LazyModule, is_diffusers_available, OptionalDependencyNotAvailable
 
 _import_structure = {
     "core": [
         "set_seed",
```

### Comparing `trl-0.8.5/trl/commands/__init__.py` & `trl-0.8.6/trl/commands/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 # flake8: noqa
 
 from typing import TYPE_CHECKING
 from ..import_utils import _LazyModule, OptionalDependencyNotAvailable
 
 
 _import_structure = {
-    "cli_utils": ["SftArgumentParser", "init_zero_verbose", "DpoScriptArguments", "TrlParser"],
-    "config_parser": ["YamlConfigParser"],
+    "cli_utils": ["SftArgumentParser", "init_zero_verbose", "DpoScriptArguments", "TrlParser", "YamlConfigParser"],
 }
 
 
 if TYPE_CHECKING:
-    from .cli_utils import SftScriptArguments, init_zero_verbose, DpoScriptArguments, TrlParser
-    from .config_parser import YamlConfigParser
+    from .cli_utils import SftScriptArguments, init_zero_verbose, DpoScriptArguments, TrlParser, YamlConfigParser
 else:
     import sys
 
     sys.modules[__name__] = _LazyModule(__name__, globals()["__file__"], _import_structure, module_spec=__spec__)
```

### Comparing `trl-0.8.5/trl/commands/cli.py` & `trl-0.8.6/trl/commands/cli.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/commands/cli_utils.py` & `trl-0.8.6/trl/commands/cli_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,24 +10,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import inspect
+import logging
 import os
 import sys
 from copy import deepcopy
 from dataclasses import asdict, dataclass, field, fields
 from typing import Any, List
 
 import yaml
 from transformers import HfArgumentParser
 
 
+logger = logging.getLogger(__name__)
+
+
 class YamlConfigParser:
     def __init__(self, config_path: str = None, dataclasses: List[Any] = None):
         self.config = None
 
         if config_path is not None:
             with open(config_path) as yaml_file:
                 self.config = yaml.safe_load(yaml_file)
@@ -252,14 +256,16 @@
 
         Args:
             parsers (`List[argparse.ArgumentParser`]):
                 List of parsers.
         """
         super().__init__(parsers)
 
+        self.config_parser = None
+
     def post_process_dataclasses(self, dataclasses):
         # Apply additional post-processing in case some arguments needs a special
         # care
         training_args = trl_args = None
         training_args_index = None
 
         for i, dataclass_obj in enumerate(dataclasses):
@@ -282,36 +288,49 @@
     def parse_args_and_config(self):
         # Hack to force-replace the `output_dir` from the YAML file if one did not passed
         # output_dir in the command line
         if "--config" in sys.argv:
             config_index = sys.argv.index("--config") + 1
             config_path = sys.argv[config_index]
 
-            with open(config_path) as yaml_file:
-                yaml_config = yaml.safe_load(yaml_file)
-
-            output_dir = yaml_config.get("output_dir")
+            self.config_parser = YamlConfigParser(config_path)
+            output_dir = self.config_parser.config.get("output_dir")
 
             if output_dir is not None:
                 if "--output_dir" in sys.argv:
                     output_dir_index = sys.argv.index("--output_dir")
-                    sys.argv.index[output_dir_index + 1] = output_dir
+                    passed_output_dir = sys.argv[output_dir_index + 1]
+                    self.config_parser.config["output_dir"] = passed_output_dir
                 else:
                     sys.argv.extend(["--output_dir", output_dir])
 
         dataclasses = self.parse_args_into_dataclasses(return_remaining_strings=True)
+
+        if len(dataclasses[-1]) > 0:
+            # It is expected that `config` is in that list but not ignored
+            # let's simply remove them
+            list_ignored = dataclasses[-1]
+            if "--config" in list_ignored:
+                config_index = list_ignored.index("--config") + 1
+                config_path = list_ignored[config_index]
+
+                list_ignored.remove(config_path)
+                list_ignored.remove("--config")
+
+            if len(list_ignored) > 0:
+                logger.warning(
+                    f"Detected extra arguments that are going to be ignored: {list_ignored} - make sure to double check what you are doing"
+                )
+
         # Pop the last element which should be the remaining strings
         dataclasses = self.update_dataclasses_with_config(dataclasses[:-1])
         return dataclasses
 
     def update_dataclasses_with_config(self, dataclasses):
-        self.config_parser = None
         for parser_dataclass in dataclasses:
-            if hasattr(parser_dataclass, "config"):
-                if self.config_parser is not None:
-                    raise ValueError("You passed the `config` field twice! Make sure to pass `config` only once.")
+            if hasattr(parser_dataclass, "config") and self.config_parser is None:
                 self.config_parser = YamlConfigParser(parser_dataclass.config)
 
         if self.config_parser is not None:
             dataclasses = self.config_parser.merge_dataclasses(dataclasses)
         dataclasses = self.post_process_dataclasses(dataclasses)
         return dataclasses
```

### Comparing `trl-0.8.5/trl/commands/scripts/chat.py` & `trl-0.8.6/trl/commands/scripts/chat.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/commands/scripts/cpo.py` & `trl-0.8.6/trl/commands/scripts/cpo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/commands/scripts/ddpo.py` & `trl-0.8.6/trl/commands/scripts/ddpo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/commands/scripts/dpo.py` & `trl-0.8.6/trl/commands/scripts/dpo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/commands/scripts/kto.py` & `trl-0.8.6/trl/commands/scripts/kto.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/commands/scripts/orpo.py` & `trl-0.8.6/trl/commands/scripts/orpo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/commands/scripts/ppo.py` & `trl-0.8.6/trl/commands/scripts/ppo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/commands/scripts/ppo_multi_adapter.py` & `trl-0.8.6/trl/commands/scripts/ppo_multi_adapter.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/commands/scripts/reward_modeling.py` & `trl-0.8.6/trl/commands/scripts/reward_modeling.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/commands/scripts/sft.py` & `trl-0.8.6/trl/commands/scripts/sft.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/commands/scripts/vsft_llava.py` & `trl-0.8.6/trl/commands/scripts/vsft_llava.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/core.py` & `trl-0.8.6/trl/core.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/environment/base_environment.py` & `trl-0.8.6/trl/environment/base_environment.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/extras/__init__.py` & `trl-0.8.6/trl/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/extras/best_of_n_sampler.py` & `trl-0.8.6/trl/extras/best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/extras/dataset_formatting.py` & `trl-0.8.6/trl/extras/dataset_formatting.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/import_utils.py` & `trl-0.8.6/trl/import_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/models/__init__.py` & `trl-0.8.6/trl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/models/modeling_base.py` & `trl-0.8.6/trl/models/modeling_base.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/models/modeling_sd_base.py` & `trl-0.8.6/trl/models/modeling_sd_base.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/models/modeling_value_head.py` & `trl-0.8.6/trl/models/modeling_value_head.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/models/sd_utils.py` & `trl-0.8.6/trl/models/sd_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/models/utils.py` & `trl-0.8.6/trl/models/utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/__init__.py` & `trl-0.8.6/trl/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/base.py` & `trl-0.8.6/trl/trainer/base.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/cpo_config.py` & `trl-0.8.6/trl/trainer/cpo_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/cpo_trainer.py` & `trl-0.8.6/trl/trainer/cpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/ddpo_config.py` & `trl-0.8.6/trl/trainer/ddpo_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/ddpo_trainer.py` & `trl-0.8.6/trl/trainer/ddpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/dpo_trainer.py` & `trl-0.8.6/trl/trainer/dpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/iterative_sft_trainer.py` & `trl-0.8.6/trl/trainer/iterative_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/kto_config.py` & `trl-0.8.6/trl/trainer/kto_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/kto_trainer.py` & `trl-0.8.6/trl/trainer/kto_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/model_config.py` & `trl-0.8.6/trl/trainer/model_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/orpo_config.py` & `trl-0.8.6/trl/trainer/orpo_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/orpo_trainer.py` & `trl-0.8.6/trl/trainer/orpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/ppo_config.py` & `trl-0.8.6/trl/trainer/ppo_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/ppo_trainer.py` & `trl-0.8.6/trl/trainer/ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/reward_config.py` & `trl-0.8.6/trl/trainer/reward_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/reward_trainer.py` & `trl-0.8.6/trl/trainer/reward_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/sft_trainer.py` & `trl-0.8.6/trl/trainer/sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl/trainer/utils.py` & `trl-0.8.6/trl/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl.egg-info/PKG-INFO` & `trl-0.8.6/trl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trl
-Version: 0.8.5
+Version: 0.8.6
 Summary: Train transformer language models with reinforcement learning.
 Home-page: https://github.com/huggingface/trl
 Author: Leandro von Werra
 Author-email: leandro.vonwerra@gmail.com
 License: Apache 2.0
 Keywords: ppo,transformers,huggingface,gpt2,language modeling,rlhf
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trl Version: 0.8.5 Summary: Train transformer
+Metadata-Version: 2.1 Name: trl Version: 0.8.6 Summary: Train transformer
 language models with reinforcement learning. Home-page: https://github.com/
 huggingface/trl Author: Leandro von Werra Author-email:
 leandro.vonwerra@gmail.com License: Apache 2.0 Keywords:
 ppo,transformers,huggingface,gpt2,language modeling,rlhf Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
```

### Comparing `trl-0.8.5/trl.egg-info/SOURCES.txt` & `trl-0.8.6/trl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trl-0.8.5/trl.egg-info/requires.txt` & `trl-0.8.6/trl.egg-info/requires.txt`

 * *Files identical despite different names*


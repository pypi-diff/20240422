# Comparing `tmp/stable_baselines3-2.3.0a4.tar.gz` & `tmp/stable_baselines3-2.3.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable_baselines3-2.3.0a4.tar", last modified: Mon Mar 11 12:53:33 2024, max compression
+gzip compressed data, was "stable_baselines3-2.3.0a5.tar", last modified: Sun Mar 31 11:29:09 2024, max compression
```

## Comparing `stable_baselines3-2.3.0a4.tar` & `stable_baselines3-2.3.0a5.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.533395 stable_baselines3-2.3.0a4/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2020-03-18 13:32:59.000000 stable_baselines3-2.3.0a4/LICENSE
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2020-07-16 10:57:35.000000 stable_baselines3-2.3.0a4/NOTICE
--rw-r--r--   0 antonin   (1000) antonin   (1000)     5014 2024-03-11 12:53:33.533395 stable_baselines3-2.3.0a4/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14489 2024-02-13 10:36:31.000000 stable_baselines3-2.3.0a4/README.md
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1662 2024-03-11 09:51:38.000000 stable_baselines3-2.3.0a4/pyproject.toml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2024-03-11 12:53:33.533395 stable_baselines3-2.3.0a4/setup.cfg
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5608 2024-03-11 12:53:17.000000 stable_baselines3-2.3.0a4/setup.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.517395 stable_baselines3-2.3.0a4/stable_baselines3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      939 2024-02-18 14:46:23.000000 stable_baselines3-2.3.0a4/stable_baselines3/__init__.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.517395 stable_baselines3-2.3.0a4/stable_baselines3/a2c/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a4/stable_baselines3/a2c/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9207 2023-12-07 09:45:38.000000 stable_baselines3-2.3.0a4/stable_baselines3/a2c/a2c.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.3.0a4/stable_baselines3/a2c/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.521395 stable_baselines3-2.3.0a4/stable_baselines3/common/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-10-07 09:00:57.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11290 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/atari_wrappers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    37032 2024-03-04 19:02:06.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/base_class.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    34544 2023-11-08 16:24:09.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26933 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    27792 2024-03-04 19:02:06.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    22098 2024-03-04 19:02:06.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/env_checker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7630 2023-10-23 10:24:06.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/env_util.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.521395 stable_baselines3-2.3.0a4/stable_baselines3/common/envs/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      533 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/envs/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9212 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/envs/bit_flipping_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6029 2023-05-08 12:31:56.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/envs/identity_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6499 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/envs/multi_input_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6451 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/evaluation.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    24237 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/logger.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9088 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5541 2023-05-20 08:31:13.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/noise.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26840 2023-12-07 09:45:38.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/off_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13023 2024-03-08 09:43:22.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/on_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    42975 2024-03-11 12:53:17.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8901 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/preprocessing.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4326 2023-03-12 17:58:51.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/results_plotter.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2012 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/running_mean_std.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    21304 2024-03-11 12:53:17.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/save_util.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.521395 stable_baselines3-2.3.0a4/stable_baselines3/common/sb2_compat/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-08-06 19:36:01.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/sb2_compat/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5651 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13722 2023-05-22 09:05:45.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/torch_layers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3189 2024-02-13 10:36:31.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/type_aliases.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20847 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/utils.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.525395 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4382 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    18460 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/base_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6966 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/dummy_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3432 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/patch_gym.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8063 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/stacked_observations.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10514 2023-11-16 16:18:52.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/subproc_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3043 2024-02-13 10:36:31.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/util.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4239 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_check_nan.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1194 2023-05-05 11:41:26.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_extract_dict_obs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2109 2024-02-13 10:36:31.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_frame_stack.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3892 2023-05-05 11:41:26.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13429 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_normalize.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4552 2023-09-03 09:35:50.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_transpose.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3887 2023-09-03 09:35:50.000000 stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_video_recorder.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.525395 stable_baselines3-2.3.0a4/stable_baselines3/ddpg/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      194 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a4/stable_baselines3/ddpg/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5718 2024-01-22 10:13:26.000000 stable_baselines3-2.3.0a4/stable_baselines3/ddpg/ddpg.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      139 2022-03-31 10:10:15.000000 stable_baselines3-2.3.0a4/stable_baselines3/ddpg/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.525395 stable_baselines3-2.3.0a4/stable_baselines3/dqn/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a4/stable_baselines3/dqn/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12859 2024-01-22 10:13:26.000000 stable_baselines3-2.3.0a4/stable_baselines3/dqn/dqn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10689 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/stable_baselines3/dqn/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.525395 stable_baselines3-2.3.0a4/stable_baselines3/her/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      204 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a4/stable_baselines3/her/__init__.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)      649 2020-10-24 10:56:51.000000 stable_baselines3-2.3.0a4/stable_baselines3/her/goal_selection_strategy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    18963 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a4/stable_baselines3/her/her_replay_buffer.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.525395 stable_baselines3-2.3.0a4/stable_baselines3/ppo/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a4/stable_baselines3/ppo/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.3.0a4/stable_baselines3/ppo/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15455 2024-03-11 12:41:13.000000 stable_baselines3-2.3.0a4/stable_baselines3/ppo/ppo.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-07-16 10:57:35.000000 stable_baselines3-2.3.0a4/stable_baselines3/py.typed
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.525395 stable_baselines3-2.3.0a4/stable_baselines3/sac/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a4/stable_baselines3/sac/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20687 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/stable_baselines3/sac/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15940 2023-12-07 09:45:38.000000 stable_baselines3-2.3.0a4/stable_baselines3/sac/sac.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.525395 stable_baselines3-2.3.0a4/stable_baselines3/td3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a4/stable_baselines3/td3/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14486 2023-12-13 10:36:46.000000 stable_baselines3-2.3.0a4/stable_baselines3/td3/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11199 2024-01-22 10:13:26.000000 stable_baselines3-2.3.0a4/stable_baselines3/td3/td3.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2024-03-11 12:53:17.000000 stable_baselines3-2.3.0a4/stable_baselines3/version.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.529395 stable_baselines3-2.3.0a4/stable_baselines3.egg-info/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     5014 2024-03-11 12:53:33.000000 stable_baselines3-2.3.0a4/stable_baselines3.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3614 2024-03-11 12:53:33.000000 stable_baselines3-2.3.0a4/stable_baselines3.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2024-03-11 12:53:33.000000 stable_baselines3-2.3.0a4/stable_baselines3.egg-info/dependency_links.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      498 2024-03-11 12:53:33.000000 stable_baselines3-2.3.0a4/stable_baselines3.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       18 2024-03-11 12:53:33.000000 stable_baselines3-2.3.0a4/stable_baselines3.egg-info/top_level.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-11 12:53:33.529395 stable_baselines3-2.3.0a4/tests/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6515 2023-11-08 16:24:09.000000 stable_baselines3-2.3.0a4/tests/test_buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9523 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/tests/test_callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13692 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a4/tests/test_cnn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2360 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a4/tests/test_custom_policy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1362 2023-05-14 15:40:24.000000 stable_baselines3-2.3.0a4/tests/test_deterministic.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11765 2023-06-22 12:07:17.000000 stable_baselines3-2.3.0a4/tests/test_dict_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9900 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a4/tests/test_distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6309 2023-10-23 10:32:57.000000 stable_baselines3-2.3.0a4/tests/test_env_checker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10404 2024-03-04 19:02:06.000000 stable_baselines3-2.3.0a4/tests/test_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6776 2024-02-04 22:19:06.000000 stable_baselines3-2.3.0a4/tests/test_gae.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    16880 2023-12-07 09:40:18.000000 stable_baselines3-2.3.0a4/tests/test_her.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1989 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a4/tests/test_identity.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15879 2023-10-23 10:34:40.000000 stable_baselines3-2.3.0a4/tests/test_logger.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3957 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a4/tests/test_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4031 2023-10-23 10:34:51.000000 stable_baselines3-2.3.0a4/tests/test_predict.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2429 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a4/tests/test_preprocessing.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7403 2023-11-08 16:24:09.000000 stable_baselines3-2.3.0a4/tests/test_run.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    28910 2023-11-17 22:50:33.000000 stable_baselines3-2.3.0a4/tests/test_save_load.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4271 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a4/tests/test_sde.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5480 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/tests/test_spaces.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2978 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a4/tests/test_tensorboard.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13175 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a4/tests/test_train_eval_mode.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    22783 2023-05-05 11:41:26.000000 stable_baselines3-2.3.0a4/tests/test_utils.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1398 2023-10-23 10:35:07.000000 stable_baselines3-2.3.0a4/tests/test_vec_check_nan.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    21829 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a4/tests/test_vec_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2941 2023-06-07 14:35:29.000000 stable_baselines3-2.3.0a4/tests/test_vec_extract_dict_obs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5276 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a4/tests/test_vec_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17740 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a4/tests/test_vec_normalize.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14821 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a4/tests/test_vec_stacked_obs.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.244469 stable_baselines3-2.3.0a5/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2020-03-18 13:32:59.000000 stable_baselines3-2.3.0a5/LICENSE
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2020-07-16 10:57:35.000000 stable_baselines3-2.3.0a5/NOTICE
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     5014 2024-03-31 11:29:09.240469 stable_baselines3-2.3.0a5/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14489 2024-02-13 10:36:31.000000 stable_baselines3-2.3.0a5/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1662 2024-03-11 09:51:38.000000 stable_baselines3-2.3.0a5/pyproject.toml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2024-03-31 11:29:09.244469 stable_baselines3-2.3.0a5/setup.cfg
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5608 2024-03-11 12:53:17.000000 stable_baselines3-2.3.0a5/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.164468 stable_baselines3-2.3.0a5/stable_baselines3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      939 2024-02-18 14:46:23.000000 stable_baselines3-2.3.0a5/stable_baselines3/__init__.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.168468 stable_baselines3-2.3.0a5/stable_baselines3/a2c/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a5/stable_baselines3/a2c/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9207 2023-12-07 09:45:38.000000 stable_baselines3-2.3.0a5/stable_baselines3/a2c/a2c.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.3.0a5/stable_baselines3/a2c/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.184468 stable_baselines3-2.3.0a5/stable_baselines3/common/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-10-07 09:00:57.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11290 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/atari_wrappers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    37032 2024-03-04 19:02:06.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/base_class.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    34544 2023-11-08 16:24:09.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26933 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    27792 2024-03-04 19:02:06.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    22098 2024-03-04 19:02:06.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/env_checker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7630 2023-10-23 10:24:06.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/env_util.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.188468 stable_baselines3-2.3.0a5/stable_baselines3/common/envs/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      533 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/envs/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9212 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/envs/bit_flipping_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6029 2023-05-08 12:31:56.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/envs/identity_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6499 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/envs/multi_input_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6451 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/evaluation.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    24237 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/logger.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9088 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5541 2023-05-20 08:31:13.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/noise.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26840 2023-12-07 09:45:38.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/off_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13417 2024-03-22 11:17:06.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/on_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    42975 2024-03-11 12:53:17.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8901 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/preprocessing.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4326 2023-03-12 17:58:51.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/results_plotter.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2012 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/running_mean_std.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    21304 2024-03-11 12:53:17.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/save_util.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.192468 stable_baselines3-2.3.0a5/stable_baselines3/common/sb2_compat/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-08-06 19:36:01.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/sb2_compat/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5651 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13722 2023-05-22 09:05:45.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/torch_layers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3189 2024-02-13 10:36:31.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/type_aliases.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20847 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.200468 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4382 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    18460 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/base_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6966 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/dummy_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3432 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/patch_gym.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8063 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/stacked_observations.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10514 2023-11-16 16:18:52.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/subproc_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3043 2024-02-13 10:36:31.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/util.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4239 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_check_nan.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1194 2023-05-05 11:41:26.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_extract_dict_obs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2109 2024-03-20 11:34:49.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_frame_stack.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3892 2023-05-05 11:41:26.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13429 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_normalize.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4552 2023-09-03 09:35:50.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_transpose.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3887 2023-09-03 09:35:50.000000 stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_video_recorder.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.200468 stable_baselines3-2.3.0a5/stable_baselines3/ddpg/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      194 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a5/stable_baselines3/ddpg/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5718 2024-01-22 10:13:26.000000 stable_baselines3-2.3.0a5/stable_baselines3/ddpg/ddpg.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      139 2022-03-31 10:10:15.000000 stable_baselines3-2.3.0a5/stable_baselines3/ddpg/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.200468 stable_baselines3-2.3.0a5/stable_baselines3/dqn/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a5/stable_baselines3/dqn/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12859 2024-01-22 10:13:26.000000 stable_baselines3-2.3.0a5/stable_baselines3/dqn/dqn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10689 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/stable_baselines3/dqn/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.204469 stable_baselines3-2.3.0a5/stable_baselines3/her/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      204 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a5/stable_baselines3/her/__init__.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)      649 2020-10-24 10:56:51.000000 stable_baselines3-2.3.0a5/stable_baselines3/her/goal_selection_strategy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    18963 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a5/stable_baselines3/her/her_replay_buffer.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.204469 stable_baselines3-2.3.0a5/stable_baselines3/ppo/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a5/stable_baselines3/ppo/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.3.0a5/stable_baselines3/ppo/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15455 2024-03-11 12:41:13.000000 stable_baselines3-2.3.0a5/stable_baselines3/ppo/ppo.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-07-16 10:57:35.000000 stable_baselines3-2.3.0a5/stable_baselines3/py.typed
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.204469 stable_baselines3-2.3.0a5/stable_baselines3/sac/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a5/stable_baselines3/sac/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20687 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/stable_baselines3/sac/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15940 2023-12-07 09:45:38.000000 stable_baselines3-2.3.0a5/stable_baselines3/sac/sac.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.204469 stable_baselines3-2.3.0a5/stable_baselines3/td3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a5/stable_baselines3/td3/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14486 2023-12-13 10:36:46.000000 stable_baselines3-2.3.0a5/stable_baselines3/td3/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11199 2024-01-22 10:13:26.000000 stable_baselines3-2.3.0a5/stable_baselines3/td3/td3.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2024-03-22 11:17:06.000000 stable_baselines3-2.3.0a5/stable_baselines3/version.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.228469 stable_baselines3-2.3.0a5/stable_baselines3.egg-info/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     5014 2024-03-31 11:29:09.000000 stable_baselines3-2.3.0a5/stable_baselines3.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3614 2024-03-31 11:29:09.000000 stable_baselines3-2.3.0a5/stable_baselines3.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2024-03-31 11:29:09.000000 stable_baselines3-2.3.0a5/stable_baselines3.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      498 2024-03-31 11:29:09.000000 stable_baselines3-2.3.0a5/stable_baselines3.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       18 2024-03-31 11:29:09.000000 stable_baselines3-2.3.0a5/stable_baselines3.egg-info/top_level.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-03-31 11:29:09.228469 stable_baselines3-2.3.0a5/tests/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6515 2023-11-08 16:24:09.000000 stable_baselines3-2.3.0a5/tests/test_buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9523 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/tests/test_callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13692 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a5/tests/test_cnn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2360 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a5/tests/test_custom_policy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1362 2023-05-14 15:40:24.000000 stable_baselines3-2.3.0a5/tests/test_deterministic.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11765 2023-06-22 12:07:17.000000 stable_baselines3-2.3.0a5/tests/test_dict_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9900 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a5/tests/test_distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6309 2023-10-23 10:32:57.000000 stable_baselines3-2.3.0a5/tests/test_env_checker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10404 2024-03-04 19:02:06.000000 stable_baselines3-2.3.0a5/tests/test_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6776 2024-02-04 22:19:06.000000 stable_baselines3-2.3.0a5/tests/test_gae.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    16880 2023-12-07 09:40:18.000000 stable_baselines3-2.3.0a5/tests/test_her.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1989 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a5/tests/test_identity.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    19287 2024-03-22 11:17:06.000000 stable_baselines3-2.3.0a5/tests/test_logger.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3957 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a5/tests/test_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4031 2023-10-23 10:34:51.000000 stable_baselines3-2.3.0a5/tests/test_predict.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2429 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a5/tests/test_preprocessing.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7403 2023-11-08 16:24:09.000000 stable_baselines3-2.3.0a5/tests/test_run.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    28910 2023-11-17 22:50:33.000000 stable_baselines3-2.3.0a5/tests/test_save_load.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4271 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a5/tests/test_sde.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5480 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/tests/test_spaces.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2978 2023-01-25 14:44:15.000000 stable_baselines3-2.3.0a5/tests/test_tensorboard.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13175 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a5/tests/test_train_eval_mode.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    22783 2023-05-05 11:41:26.000000 stable_baselines3-2.3.0a5/tests/test_utils.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1398 2023-10-23 10:35:07.000000 stable_baselines3-2.3.0a5/tests/test_vec_check_nan.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    21829 2023-11-08 08:47:59.000000 stable_baselines3-2.3.0a5/tests/test_vec_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2941 2023-06-07 14:35:29.000000 stable_baselines3-2.3.0a5/tests/test_vec_extract_dict_obs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5276 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a5/tests/test_vec_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17740 2023-10-23 10:19:05.000000 stable_baselines3-2.3.0a5/tests/test_vec_normalize.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14821 2023-04-14 11:14:22.000000 stable_baselines3-2.3.0a5/tests/test_vec_stacked_obs.py
```

### Comparing `stable_baselines3-2.3.0a4/LICENSE` & `stable_baselines3-2.3.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/NOTICE` & `stable_baselines3-2.3.0a5/NOTICE`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/PKG-INFO` & `stable_baselines3-2.3.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable_baselines3
-Version: 2.3.0a4
+Version: 2.3.0a5
 Summary: Pytorch version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/DLR-RM/stable-baselines3
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/DLR-RM/stable-baselines3
 Project-URL: Documentation, https://stable-baselines3.readthedocs.io/
```

### Comparing `stable_baselines3-2.3.0a4/README.md` & `stable_baselines3-2.3.0a5/README.md`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/pyproject.toml` & `stable_baselines3-2.3.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/setup.py` & `stable_baselines3-2.3.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/__init__.py` & `stable_baselines3-2.3.0a5/stable_baselines3/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/a2c/a2c.py` & `stable_baselines3-2.3.0a5/stable_baselines3/a2c/a2c.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/atari_wrappers.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/atari_wrappers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/base_class.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/base_class.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/buffers.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/buffers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/callbacks.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/callbacks.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/distributions.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/distributions.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/env_checker.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/env_checker.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/env_util.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/env_util.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/envs/__init__.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/envs/bit_flipping_env.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/envs/bit_flipping_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/envs/identity_env.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/envs/identity_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/envs/multi_input_envs.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/envs/multi_input_envs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/evaluation.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/evaluation.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/logger.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/logger.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/monitor.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/noise.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/noise.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/off_policy_algorithm.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/off_policy_algorithm.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/on_policy_algorithm.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/on_policy_algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,15 @@
             learning_rate=learning_rate,
             policy_kwargs=policy_kwargs,
             verbose=verbose,
             device=device,
             use_sde=use_sde,
             sde_sample_freq=sde_sample_freq,
             support_multi_env=True,
+            monitor_wrapper=monitor_wrapper,
             seed=seed,
             stats_window_size=stats_window_size,
             tensorboard_log=tensorboard_log,
             supported_action_spaces=supported_action_spaces,
         )
 
         self.n_steps = n_steps
@@ -196,15 +197,15 @@
             self.num_timesteps += env.num_envs
 
             # Give access to local variables
             callback.update_locals(locals())
             if not callback.on_step():
                 return False
 
-            self._update_info_buffer(infos)
+            self._update_info_buffer(infos, dones)
             n_steps += 1
 
             if isinstance(self.action_space, spaces.Discrete):
                 # Reshape in case of discrete action
                 actions = actions.reshape(-1, 1)
 
             # Handle timeout by bootstraping with value function
@@ -246,14 +247,36 @@
     def train(self) -> None:
         """
         Consume current rollout data and update policy parameters.
         Implemented by individual algorithms.
         """
         raise NotImplementedError
 
+    def _dump_logs(self, iteration: int) -> None:
+        """
+        Write log.
+
+        :param iteration: Current logging iteration
+        """
+        assert self.ep_info_buffer is not None
+        assert self.ep_success_buffer is not None
+
+        time_elapsed = max((time.time_ns() - self.start_time) / 1e9, sys.float_info.epsilon)
+        fps = int((self.num_timesteps - self._num_timesteps_at_start) / time_elapsed)
+        self.logger.record("time/iterations", iteration, exclude="tensorboard")
+        if len(self.ep_info_buffer) > 0 and len(self.ep_info_buffer[0]) > 0:
+            self.logger.record("rollout/ep_rew_mean", safe_mean([ep_info["r"] for ep_info in self.ep_info_buffer]))
+            self.logger.record("rollout/ep_len_mean", safe_mean([ep_info["l"] for ep_info in self.ep_info_buffer]))
+        self.logger.record("time/fps", fps)
+        self.logger.record("time/time_elapsed", int(time_elapsed), exclude="tensorboard")
+        self.logger.record("time/total_timesteps", self.num_timesteps, exclude="tensorboard")
+        if len(self.ep_success_buffer) > 0:
+            self.logger.record("rollout/success_rate", safe_mean(self.ep_success_buffer))
+        self.logger.dump(step=self.num_timesteps)
+
     def learn(
         self: SelfOnPolicyAlgorithm,
         total_timesteps: int,
         callback: MaybeCallback = None,
         log_interval: int = 1,
         tb_log_name: str = "OnPolicyAlgorithm",
         reset_num_timesteps: bool = True,
@@ -281,24 +304,15 @@
 
             iteration += 1
             self._update_current_progress_remaining(self.num_timesteps, total_timesteps)
 
             # Display training infos
             if log_interval is not None and iteration % log_interval == 0:
                 assert self.ep_info_buffer is not None
-                time_elapsed = max((time.time_ns() - self.start_time) / 1e9, sys.float_info.epsilon)
-                fps = int((self.num_timesteps - self._num_timesteps_at_start) / time_elapsed)
-                self.logger.record("time/iterations", iteration, exclude="tensorboard")
-                if len(self.ep_info_buffer) > 0 and len(self.ep_info_buffer[0]) > 0:
-                    self.logger.record("rollout/ep_rew_mean", safe_mean([ep_info["r"] for ep_info in self.ep_info_buffer]))
-                    self.logger.record("rollout/ep_len_mean", safe_mean([ep_info["l"] for ep_info in self.ep_info_buffer]))
-                self.logger.record("time/fps", fps)
-                self.logger.record("time/time_elapsed", int(time_elapsed), exclude="tensorboard")
-                self.logger.record("time/total_timesteps", self.num_timesteps, exclude="tensorboard")
-                self.logger.dump(step=self.num_timesteps)
+                self._dump_logs(iteration)
 
             self.train()
 
         callback.on_training_end()
 
         return self
```

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/policies.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/preprocessing.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/preprocessing.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/results_plotter.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/results_plotter.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/running_mean_std.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/running_mean_std.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/save_util.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/save_util.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/torch_layers.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/torch_layers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/type_aliases.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/type_aliases.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/utils.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/utils.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/__init__.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/base_vec_env.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/base_vec_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/dummy_vec_env.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/dummy_vec_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/patch_gym.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/patch_gym.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/stacked_observations.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/stacked_observations.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/subproc_vec_env.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/subproc_vec_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/util.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/util.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_check_nan.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_check_nan.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_extract_dict_obs.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_extract_dict_obs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_frame_stack.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_frame_stack.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_monitor.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_normalize.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_normalize.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_transpose.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_transpose.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/common/vec_env/vec_video_recorder.py` & `stable_baselines3-2.3.0a5/stable_baselines3/common/vec_env/vec_video_recorder.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/ddpg/ddpg.py` & `stable_baselines3-2.3.0a5/stable_baselines3/ddpg/ddpg.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/dqn/dqn.py` & `stable_baselines3-2.3.0a5/stable_baselines3/dqn/dqn.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/dqn/policies.py` & `stable_baselines3-2.3.0a5/stable_baselines3/dqn/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/her/goal_selection_strategy.py` & `stable_baselines3-2.3.0a5/stable_baselines3/her/goal_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/her/her_replay_buffer.py` & `stable_baselines3-2.3.0a5/stable_baselines3/her/her_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/ppo/ppo.py` & `stable_baselines3-2.3.0a5/stable_baselines3/ppo/ppo.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/sac/policies.py` & `stable_baselines3-2.3.0a5/stable_baselines3/sac/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/sac/sac.py` & `stable_baselines3-2.3.0a5/stable_baselines3/sac/sac.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/td3/policies.py` & `stable_baselines3-2.3.0a5/stable_baselines3/td3/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3/td3/td3.py` & `stable_baselines3-2.3.0a5/stable_baselines3/td3/td3.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3.egg-info/PKG-INFO` & `stable_baselines3-2.3.0a5/stable_baselines3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable_baselines3
-Version: 2.3.0a4
+Version: 2.3.0a5
 Summary: Pytorch version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/DLR-RM/stable-baselines3
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/DLR-RM/stable-baselines3
 Project-URL: Documentation, https://stable-baselines3.readthedocs.io/
```

### Comparing `stable_baselines3-2.3.0a4/stable_baselines3.egg-info/SOURCES.txt` & `stable_baselines3-2.3.0a5/stable_baselines3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_buffers.py` & `stable_baselines3-2.3.0a5/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_callbacks.py` & `stable_baselines3-2.3.0a5/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_cnn.py` & `stable_baselines3-2.3.0a5/tests/test_cnn.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_custom_policy.py` & `stable_baselines3-2.3.0a5/tests/test_custom_policy.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_deterministic.py` & `stable_baselines3-2.3.0a5/tests/test_deterministic.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_dict_env.py` & `stable_baselines3-2.3.0a5/tests/test_dict_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_distributions.py` & `stable_baselines3-2.3.0a5/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_env_checker.py` & `stable_baselines3-2.3.0a5/tests/test_env_checker.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_envs.py` & `stable_baselines3-2.3.0a5/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_gae.py` & `stable_baselines3-2.3.0a5/tests/test_gae.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_her.py` & `stable_baselines3-2.3.0a5/tests/test_her.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_identity.py` & `stable_baselines3-2.3.0a5/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_logger.py` & `stable_baselines3-2.3.0a5/tests/test_logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 import pytest
 import torch as th
 from gymnasium import spaces
 from matplotlib import pyplot as plt
 from pandas.errors import EmptyDataError
 
-from stable_baselines3 import A2C, DQN
+from stable_baselines3 import A2C, DQN, PPO
 from stable_baselines3.common.env_checker import check_env
 from stable_baselines3.common.logger import (
     DEBUG,
     INFO,
     CSVOutputFormat,
     Figure,
     FormatUnsupportedError,
@@ -29,14 +29,15 @@
     TensorBoardOutputFormat,
     Video,
     configure,
     make_output_format,
     read_csv,
     read_json,
 )
+from stable_baselines3.common.monitor import Monitor
 
 KEY_VALUES = {
     "test": 1,
     "b": -3.14,
     "8": 9.9,
     "l": [1, 2],
     "a": np.array([1, 2, 3]),
@@ -470,7 +471,96 @@
 | key1 | value2 |
 | key2 | 43     |
 -----------------
 
 """
 
     assert printed == desired_printed
+
+
+class DummySuccessEnv(gym.Env):
+    """
+    Create a dummy success environment that returns wether True or False for info['is_success']
+    at the end of an episode according to its dummy successes list
+    """
+
+    def __init__(self, dummy_successes, ep_steps):
+        """Init the dummy success env
+
+        :param dummy_successes: list of size (n_logs_iterations, n_episodes_per_log) that specifies
+            the success value of log iteration i at episode j
+        :param ep_steps: number of steps per episode (to activate truncated)
+        """
+        self.n_steps = 0
+        self.log_id = 0
+        self.ep_id = 0
+
+        self.ep_steps = ep_steps
+
+        self.dummy_success = dummy_successes
+        self.num_logs = len(dummy_successes)
+        self.ep_per_log = len(dummy_successes[0])
+        self.steps_per_log = self.ep_per_log * self.ep_steps
+
+        self.action_space = spaces.Discrete(2)
+        self.observation_space = spaces.Discrete(2)
+
+    def reset(self, seed=None, options=None):
+        """
+        Reset the env and advance to the next episode_id to get the next dummy success
+        """
+        self.n_steps = 0
+
+        if self.ep_id == self.ep_per_log:
+            self.ep_id = 0
+            self.log_id = (self.log_id + 1) % self.num_logs
+
+        return self.observation_space.sample(), {}
+
+    def step(self, action):
+        """
+        Step and return a dummy success when an episode is truncated
+        """
+        self.n_steps += 1
+        truncated = self.n_steps >= self.ep_steps
+
+        info = {}
+        if truncated:
+            maybe_success = self.dummy_success[self.log_id][self.ep_id]
+            info["is_success"] = maybe_success
+            self.ep_id += 1
+        return self.observation_space.sample(), 0.0, False, truncated, info
+
+
+def test_rollout_success_rate_on_policy_algorithm(tmp_path):
+    """
+    Test if the rollout/success_rate information is correctly logged with on policy algorithms
+
+    To do so, create a dummy environment that takes as argument dummy successes (i.e when an episode)
+    is going to be successfull or not.
+    """
+
+    STATS_WINDOW_SIZE = 10
+    # Add dummy successes with 0.3, 0.5 and 0.8 success_rate of length STATS_WINDOW_SIZE
+    dummy_successes = [
+        [True] * 3 + [False] * 7,
+        [True] * 5 + [False] * 5,
+        [True] * 8 + [False] * 2,
+    ]
+    ep_steps = 64
+
+    # Monitor the env to track the success info
+    monitor_file = str(tmp_path / "monitor.csv")
+    env = Monitor(DummySuccessEnv(dummy_successes, ep_steps), filename=monitor_file, info_keywords=("is_success",))
+
+    # Equip the model of a custom logger to check the success_rate info
+    model = PPO("MlpPolicy", env=env, stats_window_size=STATS_WINDOW_SIZE, n_steps=env.steps_per_log, verbose=1)
+    logger = InMemoryLogger()
+    model.set_logger(logger)
+
+    # Make the model learn and check that the success rate corresponds to the ratio of dummy successes
+    model.learn(total_timesteps=env.ep_per_log * ep_steps, log_interval=1)
+    assert logger.name_to_value["rollout/success_rate"] == 0.3
+    model.learn(total_timesteps=env.ep_per_log * ep_steps, log_interval=1)
+    assert logger.name_to_value["rollout/success_rate"] == 0.5
+    model.learn(total_timesteps=env.ep_per_log * ep_steps, log_interval=1)
+    assert logger.name_to_value["rollout/success_rate"] == 0.8
```

### Comparing `stable_baselines3-2.3.0a4/tests/test_monitor.py` & `stable_baselines3-2.3.0a5/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_predict.py` & `stable_baselines3-2.3.0a5/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_preprocessing.py` & `stable_baselines3-2.3.0a5/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_run.py` & `stable_baselines3-2.3.0a5/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_save_load.py` & `stable_baselines3-2.3.0a5/tests/test_save_load.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_sde.py` & `stable_baselines3-2.3.0a5/tests/test_sde.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_spaces.py` & `stable_baselines3-2.3.0a5/tests/test_spaces.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_tensorboard.py` & `stable_baselines3-2.3.0a5/tests/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_train_eval_mode.py` & `stable_baselines3-2.3.0a5/tests/test_train_eval_mode.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_utils.py` & `stable_baselines3-2.3.0a5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_vec_check_nan.py` & `stable_baselines3-2.3.0a5/tests/test_vec_check_nan.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_vec_envs.py` & `stable_baselines3-2.3.0a5/tests/test_vec_envs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_vec_extract_dict_obs.py` & `stable_baselines3-2.3.0a5/tests/test_vec_extract_dict_obs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_vec_monitor.py` & `stable_baselines3-2.3.0a5/tests/test_vec_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_vec_normalize.py` & `stable_baselines3-2.3.0a5/tests/test_vec_normalize.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.0a4/tests/test_vec_stacked_obs.py` & `stable_baselines3-2.3.0a5/tests/test_vec_stacked_obs.py`

 * *Files identical despite different names*


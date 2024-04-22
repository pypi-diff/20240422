# Comparing `tmp/sheeprl-0.5.4.tar.gz` & `tmp/sheeprl-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheeprl-0.5.4.tar", last modified: Mon Feb 26 11:20:38 2024, max compression
+gzip compressed data, was "sheeprl-0.5.5.tar", last modified: Mon Apr 22 09:34:12 2024, max compression
```

## Comparing `sheeprl-0.5.4.tar` & `sheeprl-0.5.5.tar`

### file list

```diff
@@ -1,263 +1,268 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.660016 sheeprl-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-02-26 11:20:31.000000 sheeprl-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-26 11:20:31.000000 sheeprl-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-02-26 11:20:38.660016 sheeprl-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23458 2024-02-26 11:20:31.000000 sheeprl-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.620016 sheeprl-0.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-26 11:20:31.000000 sheeprl-0.5.4/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.620016 sheeprl-0.5.4/hydra_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-26 11:20:31.000000 sheeprl-0.5.4/hydra_plugins/sheeprl_search_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-02-26 11:20:31.000000 sheeprl-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 11:20:38.660016 sheeprl-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-26 11:20:31.000000 sheeprl-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.620016 sheeprl-0.5.4/sheeprl/
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.620016 sheeprl-0.5.4/sheeprl/algos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.620016 sheeprl-0.5.4/sheeprl/algos/a2c/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/a2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15271 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/a2c/a2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/a2c/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/a2c/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/a2c/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/a2c/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.624016 sheeprl-0.5.4/sheeprl/algos/dreamer_v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22647 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v1/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    37752 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v1/dreamer_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v1/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v1/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.624016 sheeprl-0.5.4/sheeprl/algos/dreamer_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49305 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v2/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    38886 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v2/dreamer_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v2/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v2/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     7510 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.624016 sheeprl-0.5.4/sheeprl/algos/dreamer_v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53009 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v3/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    35826 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v3/dreamer_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v3/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v3/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/dreamer_v3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.628016 sheeprl-0.5.4/sheeprl/algos/droq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/droq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/droq/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    17688 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/droq/droq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/droq/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/droq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.628016 sheeprl-0.5.4/sheeprl/algos/p2e_dv1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv1/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv1/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    40600 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21582 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.628016 sheeprl-0.5.4/sheeprl/algos/p2e_dv2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv2/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv2/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    47570 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)    23140 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.628016 sheeprl-0.5.4/sheeprl/algos/p2e_dv3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv3/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv3/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    51893 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)    23289 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/p2e_dv3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.632016 sheeprl-0.5.4/sheeprl/algos/ppo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    20232 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo/ppo.py
--rw-r--r--   0 runner    (1001) docker     (127)    29071 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo/ppo_decoupled.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.632016 sheeprl-0.5.4/sheeprl/algos/ppo_recurrent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo_recurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12793 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo_recurrent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo_recurrent/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    23745 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo_recurrent/ppo_recurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/ppo_recurrent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.632016 sheeprl-0.5.4/sheeprl/algos/sac/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac/sac.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac/sac_decoupled.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.636016 sheeprl-0.5.4/sheeprl/algos/sac_ae/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac_ae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20988 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac_ae/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac_ae/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac_ae/sac_ae.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/algos/sac_ae/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/available_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    18170 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.636016 sheeprl-0.5.4/sheeprl/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.640016 sheeprl-0.5.4/sheeprl/configs/algo/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/a2c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/dreamer_v1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/dreamer_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/dreamer_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/dreamer_v3_L.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/dreamer_v3_M.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/dreamer_v3_S.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/dreamer_v3_XL.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/dreamer_v3_XS.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/droq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/p2e_dv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/p2e_dv2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/p2e_dv3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/ppo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/ppo_decoupled.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/ppo_recurrent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/sac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/sac_ae.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/algo/sac_decoupled.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.640016 sheeprl-0.5.4/sheeprl/configs/buffer/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/buffer/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.640016 sheeprl-0.5.4/sheeprl/configs/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/checkpoint/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.640016 sheeprl-0.5.4/sheeprl/configs/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/distribution/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.640016 sheeprl-0.5.4/sheeprl/configs/env/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/atari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/crafter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/diambra.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/dmc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/dummy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/gym.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/minecraft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/minedojo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/minerl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/mujoco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env/super_mario_bros.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/env_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/eval_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.648016 sheeprl-0.5.4/sheeprl/configs/exp/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/a2c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v2_crafter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_100k_boxing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_100k_ms_pacman.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_L_doapp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_XL_crafter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_super_mario_bros.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/droq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv1_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv1_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv2_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv2_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv3_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv3_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/ppo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/ppo_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/ppo_decoupled.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/ppo_recurrent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/ppo_super_mario_bros.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/sac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/sac_ae.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/sac_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/exp/sac_decoupled.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.648016 sheeprl-0.5.4/sheeprl/configs/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/fabric/ddp-cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/fabric/ddp-cuda.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/fabric/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.648016 sheeprl-0.5.4/sheeprl/configs/hydra/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/hydra/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.648016 sheeprl-0.5.4/sheeprl/configs/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/logger/mlflow.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/logger/tensorboard.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.648016 sheeprl-0.5.4/sheeprl/configs/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/metric/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.652016 sheeprl-0.5.4/sheeprl/configs/model_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/a2c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/dreamer_v1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/dreamer_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/dreamer_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/droq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/p2e_dv1_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/ppo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/ppo_recurrent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/sac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager/sac_ae.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/model_manager_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.652016 sheeprl-0.5.4/sheeprl/configs/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/optim/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/optim/rmsprop.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/optim/rmsprop_tf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/configs/optim/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.652016 sheeprl-0.5.4/sheeprl/data/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53725 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/data/buffers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.652016 sheeprl-0.5.4/sheeprl/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/crafter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/diambra.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/dmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/minedojo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/minerl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.652016 sheeprl-0.5.4/sheeprl/envs/minerl_envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/minerl_envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/minerl_envs/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/minerl_envs/navigate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/minerl_envs/obtain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/super_mario_bros.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/envs/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.652016 sheeprl-0.5.4/sheeprl/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20669 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.652016 sheeprl-0.5.4/sheeprl/optim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/optim/rmsprop_tf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.656016 sheeprl-0.5.4/sheeprl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    17999 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-02-26 11:20:31.000000 sheeprl-0.5.4/sheeprl/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 11:20:38.656016 sheeprl-0.5.4/sheeprl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-02-26 11:20:38.000000 sheeprl-0.5.4/sheeprl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-02-26 11:20:38.000000 sheeprl-0.5.4/sheeprl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 11:20:38.000000 sheeprl-0.5.4/sheeprl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-26 11:20:38.000000 sheeprl-0.5.4/sheeprl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-26 11:20:38.000000 sheeprl-0.5.4/sheeprl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-26 11:20:38.000000 sheeprl-0.5.4/sheeprl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.134818 sheeprl-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-22 09:34:07.000000 sheeprl-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-22 09:34:07.000000 sheeprl-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-04-22 09:34:12.134818 sheeprl-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24648 2024-04-22 09:34:07.000000 sheeprl-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.090818 sheeprl-0.5.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-22 09:34:07.000000 sheeprl-0.5.5/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.090818 sheeprl-0.5.5/hydra_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-22 09:34:07.000000 sheeprl-0.5.5/hydra_plugins/sheeprl_search_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-22 09:34:07.000000 sheeprl-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:34:12.134818 sheeprl-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-22 09:34:07.000000 sheeprl-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.094818 sheeprl-0.5.5/sheeprl/
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.094818 sheeprl-0.5.5/sheeprl/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.094818 sheeprl-0.5.5/sheeprl/algos/a2c/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16852 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/a2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/a2c/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.098818 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36796 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/dreamer_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.098818 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50079 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37400 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/dreamer_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.098818 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57479 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35745 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/dreamer_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/dreamer_v3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.098818 sheeprl-0.5.5/sheeprl/algos/droq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/droq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/droq/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/droq/droq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/droq/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/droq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.102818 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39009 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20776 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.102818 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45472 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22095 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.102818 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50554 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22467 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/p2e_dv3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.106818 sheeprl-0.5.5/sheeprl/algos/ppo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20146 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/ppo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29280 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/ppo_decoupled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.106818 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23740 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/ppo_recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.106818 sheeprl-0.5.5/sheeprl/algos/sac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18646 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/sac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25366 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/sac_decoupled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.106818 sheeprl-0.5.5/sheeprl/algos/sac_ae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac_ae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24357 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac_ae/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac_ae/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22314 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac_ae/sac_ae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/algos/sac_ae/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/available_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19690 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.106818 sheeprl-0.5.5/sheeprl/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.110818 sheeprl-0.5.5/sheeprl/configs/algo/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/a2c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3_L.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3_M.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3_S.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3_XL.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v3_XS.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/droq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/ppo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/ppo_decoupled.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/ppo_recurrent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/sac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/sac_ae.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/algo/sac_decoupled.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.110818 sheeprl-0.5.5/sheeprl/configs/buffer/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/buffer/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.110818 sheeprl-0.5.5/sheeprl/configs/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/checkpoint/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.110818 sheeprl-0.5.5/sheeprl/configs/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/distribution/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.114818 sheeprl-0.5.5/sheeprl/configs/env/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/atari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/crafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/diambra.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/dmc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/dummy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/gym.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/minecraft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/minedojo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/minerl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/minerl_obtain_diamond.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/minerl_obtain_iron_pickaxe.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/mujoco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env/super_mario_bros.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/env_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/eval_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.122818 sheeprl-0.5.5/sheeprl/configs/exp/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/a2c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/a2c_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_crafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_100k_boxing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-22 09:34:07.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_100k_ms_pacman.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_L_doapp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_XL_crafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_super_mario_bros.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/droq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv1_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv1_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv2_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv2_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/ppo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/ppo_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/ppo_decoupled.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/ppo_recurrent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/ppo_super_mario_bros.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/sac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/sac_ae.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/sac_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/exp/sac_decoupled.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.122818 sheeprl-0.5.5/sheeprl/configs/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/fabric/ddp-cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/fabric/ddp-cuda.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/fabric/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.122818 sheeprl-0.5.5/sheeprl/configs/hydra/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/hydra/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.122818 sheeprl-0.5.5/sheeprl/configs/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/logger/mlflow.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/logger/tensorboard.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.122818 sheeprl-0.5.5/sheeprl/configs/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/metric/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.126818 sheeprl-0.5.5/sheeprl/configs/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/a2c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/dreamer_v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/dreamer_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/dreamer_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/droq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv1_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/ppo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/ppo_recurrent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/sac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager/sac_ae.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/model_manager_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.126818 sheeprl-0.5.5/sheeprl/configs/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/optim/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/optim/rmsprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/optim/rmsprop_tf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/configs/optim/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.126818 sheeprl-0.5.5/sheeprl/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54229 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/data/buffers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.126818 sheeprl-0.5.5/sheeprl/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/crafter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/diambra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/dmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minedojo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minerl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.126818 sheeprl-0.5.5/sheeprl/envs/minerl_envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minerl_envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minerl_envs/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minerl_envs/navigate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/minerl_envs/obtain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/super_mario_bros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/envs/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.130818 sheeprl-0.5.5/sheeprl/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21610 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.130818 sheeprl-0.5.5/sheeprl/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/optim/rmsprop_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.130818 sheeprl-0.5.5/sheeprl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17999 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-04-22 09:34:08.000000 sheeprl-0.5.5/sheeprl/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:12.130818 sheeprl-0.5.5/sheeprl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 09:34:12.000000 sheeprl-0.5.5/sheeprl.egg-info/top_level.txt
```

### Comparing `sheeprl-0.5.4/LICENSE` & `sheeprl-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/PKG-INFO` & `sheeprl-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheeprl
-Version: 0.5.4
+Version: 0.5.5
 Summary: High-quality, single file and distributed implementation of Deep Reinforcement Learning algorithms with production-friendly features
 Author-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 Maintainer-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -207,33 +207,34 @@
            limitations under the License.
         
 Project-URL: homepage, https://eclecticsheep.ai
 Project-URL: repository, https://github.com/Eclectic-Sheep/sheeprl
 Keywords: reinforcement,machine,learning,distributed,production
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gymnasium==0.29.*
 Requires-Dist: pygame>=2.1.3
 Requires-Dist: moviepy>=1.0.3
 Requires-Dist: tensorboard>=2.10
 Requires-Dist: python-dotenv>=1.0.0
-Requires-Dist: lightning==2.1.*
+Requires-Dist: lightning>=2.0
 Requires-Dist: lightning-utilities<=0.9
 Requires-Dist: hydra-core==1.3.0
 Requires-Dist: torchmetrics
 Requires-Dist: rich==13.5.*
 Requires-Dist: opencv-python==4.8.0.*
 Requires-Dist: torch!=2.2.0,>=2.0
 Provides-Extra: test
 Requires-Dist: pytest==7.3.1; extra == "test"
 Requires-Dist: pytest-timeout==2.1.0; extra == "test"
 Requires-Dist: pytest-coverage; extra == "test"
+Requires-Dist: importlib_resources>=6.2.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: mypy==1.2.0; extra == "dev"
 Requires-Dist: black==23.12.1; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
 Requires-Dist: autoflake==2.2.1; extra == "dev"
 Requires-Dist: ruff==0.1.11; extra == "dev"
@@ -247,24 +248,26 @@
 Provides-Extra: atari
 Requires-Dist: gymnasium[atari]==0.29.*; extra == "atari"
 Requires-Dist: gymnasium[accept-rom-license]==0.29.*; extra == "atari"
 Requires-Dist: gymnasium[other]==0.29.*; extra == "atari"
 Provides-Extra: minedojo
 Requires-Dist: minedojo==0.1; extra == "minedojo"
 Requires-Dist: importlib_resources==5.12.0; extra == "minedojo"
+Requires-Dist: gym==0.21.0; extra == "minedojo"
 Provides-Extra: minerl
 Requires-Dist: setuptools==66.0.0; extra == "minerl"
 Requires-Dist: minerl==0.4.4; extra == "minerl"
+Requires-Dist: gym==0.19.0; extra == "minerl"
 Provides-Extra: diambra
-Requires-Dist: diambra==0.0.16; extra == "diambra"
-Requires-Dist: diambra-arena==2.2.2; extra == "diambra"
+Requires-Dist: diambra==0.0.17; extra == "diambra"
+Requires-Dist: diambra-arena==2.2.6; extra == "diambra"
 Provides-Extra: crafter
-Requires-Dist: crafter==1.8.1; extra == "crafter"
+Requires-Dist: crafter==1.8.3; extra == "crafter"
 Provides-Extra: mlflow
-Requires-Dist: mlflow==2.8.0; extra == "mlflow"
+Requires-Dist: mlflow==2.11.1; extra == "mlflow"
 Provides-Extra: supermario
 Requires-Dist: gym-super-mario-bros==7.4.0; extra == "supermario"
 Requires-Dist: gym<0.26; extra == "supermario"
 
 # ⚡ SheepRL 🐑
 
 <p id="logo" align="center" style="width: 50%; margin: auto;">
```

### Comparing `sheeprl-0.5.4/README.md` & `sheeprl-0.5.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # ⚡ SheepRL 🐑
 
+[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
+
 <p align="center">
   <img src="./assets/images/logo.svg" style="width:40%">
 </p>
 
 <div align="center">
   <table>
     <tr>
@@ -82,70 +87,95 @@
   <table>
     <thead>
       <tr>
         <th colspan="2"></th>
         <th>SheepRL v0.4.0</th>
         <th>SheepRL v0.4.9</th>
         <th>SheepRL v0.5.2<br />(Numpy Buffers)</th>
+        <th>SheepRL v0.5.5<br />(Numpy Buffers)</th>
         <th>StableBaselines3<sup>1</sup></th>
       </tr>
     </thead>
     <tbody>
       <tr>
         <td rowspan="2"><b>PPO</b></td>
         <td><i>1 device</i></td>
         <td>192.31s &plusmn; 1.11</td>
         <td>138.3s &plusmn; 0.16</td>
         <td>80.81s &plusmn; 0.68</td>
+        <td>81.27s &plusmn; 0.47</td>
         <td>77.21s &plusmn; 0.36</td>
       </tr>
       <tr>
         <td><i>2 devices</i></td>
         <td>85.42s &plusmn; 2.27</td>
         <td>59.53s &plusmn; 0.78</td>
         <td>46.09s &plusmn; 0.59</td>
+        <td>36.88s &plusmn; 0.30</td>
+        <td>N.D.</td>
+      </tr>
+      <tr>
+        <td rowspan="2"><b>A2C</b></td>
+        <td><i>1 device</i></td>
+        <td>N.D.</td>
+        <td>N.D.</td>
+        <td>N.D.</td>
+        <td>84.76s &plusmn; 0.37</td>
+        <td>84.22s &plusmn; 0.99</td>
+      </tr>
+      <tr>
+        <td><i>2 devices</i></td>
+        <td>N.D.</td>
+        <td>N.D.</td>
+        <td>N.D.</td>
+        <td>28.95s &plusmn; 0.75</td>
         <td>N.D.</td>
       </tr>
       <tr>
         <td rowspan="2"><b>SAC</b></td>
         <td><i>1 device</i></td>
         <td>421.37s &plusmn; 5.27</td>
         <td>363.74s &plusmn; 3.44</td>
         <td>318.06s &plusmn; 4.46</td>
+        <td>320.21 &plusmn; 6.29</td>
         <td>336.06s &plusmn; 12.26</td>
       </tr>
       <tr>
         <td><i>2 devices</i></td>
         <td>264.29s &plusmn; 1.81</td>
         <td>238.88s &plusmn; 4.97</td>
         <td>210.07s &plusmn; 27</td>
+        <td>225.95 &plusmn; 3.65</td>
         <td>N.D.</td>
       </tr>
       <tr>
         <td><b>Dreamer V1</b></td>
         <td><i>1 device</i></td>
         <td>4201.23s</td>
         <td>N.D.</td>
         <td>2921.38s</td>
+        <td>2207.13s</td>
         <td>N.D.</td>
       </tr>
       <tr>
         <td><b>Dreamer V2</b></td>
         <td><i>1 device</i></td>
         <td>1874.62s</td>
         <td>N.D.</td>
         <td>1148.1s</td>
+        <td>906.42s</td>
         <td>N.D.</td>
       </tr>
       <tr>
         <td><b>Dreamer V3</b></td>
         <td><i>1 device</i></td>
         <td>2022.99s</td>
         <td>N.D.</td>
         <td>1378.01s</td>
+        <td>1589.30s</td>
         <td>N.D.</td>
       </tr>
     </tbody>
   </table>
 </div>
 
 > [!NOTE]
```

#### html2text {}

```diff
@@ -1,8 +1,14 @@
-# â¡ SheepRL ð
+# â¡ SheepRL ð [![Python 3.8](https://img.shields.io/badge/python-3.8-
+blue.svg)](https://www.python.org/downloads/release/python-380/) [![Python 3.9]
+(https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/
+downloads/release/python-390/) [![Python 3.10](https://img.shields.io/badge/
+python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://
+www.python.org/downloads/release/python-3110/)
                           [./assets/images/logo.svg]
 [https://          [https://          [https://github.com/ [https://github.com/
 github.com/        github.com/        Eclectic-Sheep/      Eclectic-Sheep/
 Eclectic-Sheep/    Eclectic-Sheep/    sheeprl/assets/      sheeprl/assets/
 sheeprl/assets/    sheeprl/assets/    18405289/3f38e5eb-   18405289/93749119-
 18405289/6efd09f0- 18405289/dbba57db- aadd-4402-a698-      fe61-44f1-94bb-
 df91-4da0-971d-    6ef5-4db4-9c53-    695d1f99c048]        fdb89c1869b5]
@@ -15,29 +21,33 @@
  o optimizations)1
  Minecraft-Nav(w/  8M           16d 4h        27% >= 70   N.A.         1-V100
  o optimizations)                             14% >= 100
 1. For comparison: 1M in 2d 7h vs 1M in 1d 5h (before and after optimizations
 resp.) 2. Best [leaderboard score in DIAMBRA](https://diambra.ai/leaderboard)
 (11/7/2023) #### Benchmarks The training times of our implementations compared
 to the ones of Stable Baselines3 are shown below:
-                                              SShheeeeppRRLL
-                      SShheeeeppRRLL   SShheeeeppRRLL       vv00..55..22        SSttaabblleeBBaasseelliinneess3311
-                      vv00..44..00    vv00..44..99        ((NNuummppyy
-                                              BBuuffffeerrss))
-            1 device  192.31s ± 138.3s ± 0.16 80.81s ± 0.68 77.21s ± 0.36
- PPPPOO                  1.11
-            2 devices 85.42s ±  59.53s ± 0.78 46.09s ± 0.59 N.D.
-                      2.27
-            1 device  421.37s ± 363.74s ±     318.06s ±     336.06s ± 12.26
- SSAACC                  5.27      3.44          4.46
-            2 devices 264.29s ± 238.88s ±     210.07s ± 27  N.D.
-                      1.81      4.97
- DDrreeaammeerr VV11 1 device  4201.23s  N.D.          2921.38s      N.D.
- DDrreeaammeerr VV22 1 device  1874.62s  N.D.          1148.1s       N.D.
- DDrreeaammeerr VV33 1 device  2022.99s  N.D.          1378.01s      N.D.
+                                          SShheeeeppRRLL   SShheeeeppRRLL
+                      SShheeeeppRRLL   SShheeeeppRRLL   vv00..55..22    vv00..55..55   SSttaabblleeBBaasseelliinneess3311
+                      vv00..44..00    vv00..44..99    ((NNuummppyy    ((NNuummppyy
+                                          BBuuffffeerrss))  BBuuffffeerrss))
+            1 device  192.31s ± 138.3s ±  80.81s ±  81.27s ± 77.21s ± 0.36
+ PPPPOO                  1.11      0.16      0.68      0.47
+            2 devices 85.42s ±  59.53s ±  46.09s ±  36.88s ± N.D.
+                      2.27      0.78      0.59      0.30
+            1 device  N.D.      N.D.      N.D.      84.76s ± 84.22s ± 0.99
+ AA22CC                                                0.37
+            2 devices N.D.      N.D.      N.D.      28.95s ± N.D.
+                                                    0.75
+            1 device  421.37s ± 363.74s ± 318.06s ± 320.21 ± 336.06s ± 12.26
+ SSAACC                  5.27      3.44      4.46      6.29
+            2 devices 264.29s ± 238.88s ± 210.07s ± 225.95 ± N.D.
+                      1.81      4.97      27        3.65
+ DDrreeaammeerr VV11 1 device  4201.23s  N.D.      2921.38s  2207.13s N.D.
+ DDrreeaammeerr VV22 1 device  1874.62s  N.D.      1148.1s   906.42s  N.D.
+ DDrreeaammeerr VV33 1 device  2022.99s  N.D.      1378.01s  1589.30s N.D.
 > [!NOTE] > > All experiments have been run on 4 CPUs in [Lightning Studio]
 (https://lightning.ai/). > All benchmarks, but the Dreamers' ones, have been
 run 5 times and we have taken the mean and the std of the runs. > We have
 disabled the test function, the logging, and the checkpoints. Moreover, the
 models were not registered using MLFlow. > > Dreamers' benchmarks have been run
 1 time with logging and checkpoints, without running the test function. > > 1.
 The StableBaselines3 version is `v2.2.1`, please install the package with `pip
```

### Comparing `sheeprl-0.5.4/docs/README.md` & `sheeprl-0.5.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/hydra_plugins/sheeprl_search_path.py` & `sheeprl-0.5.5/hydra_plugins/sheeprl_search_path.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/pyproject.toml` & `sheeprl-0.5.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -20,23 +20,23 @@
   { name = "Davide Angioni", email = "davide.angioni@orobix.com" },
   { name = "Refik Can Malli", email = "refikcan.malli@orobix.com" },
   { name = "Michele Milesi", email = "michele.milesi@orobix.com" },
 ]
 keywords = ["reinforcement", "machine", "learning", "distributed", "production"]
 license = { file = "LICENSE" }
 readme = { file = "docs/README.md", content-type = "text/markdown" }
-requires-python = ">=3.8,<3.11"
+requires-python = ">=3.8,<3.12"
 classifiers = ["Programming Language :: Python", "Topic :: Scientific/Engineering :: Artificial Intelligence"]
 dependencies = [
   "gymnasium==0.29.*",
   "pygame >=2.1.3",
   "moviepy>=1.0.3",
   "tensorboard>=2.10",
   "python-dotenv>=1.0.0",
-  "lightning==2.1.*",
+  "lightning>=2.0",
   "lightning-utilities<=0.9",
   "hydra-core==1.3.0",
   "torchmetrics",
   "rich==13.5.*",
   "opencv-python==4.8.0.*",
   "torch>=2.0,!=2.2.0"
 ]
@@ -60,15 +60,15 @@
 sheeprl-registration = "sheeprl.cli:registration"
 
 [project.urls]
 homepage = "https://eclecticsheep.ai"
 repository = "https://github.com/Eclectic-Sheep/sheeprl"
 
 [project.optional-dependencies]
-test = ["pytest==7.3.1", "pytest-timeout==2.1.0", "pytest-coverage"]
+test = ["pytest==7.3.1", "pytest-timeout==2.1.0", "pytest-coverage", "importlib_resources>=6.2.0"]
 dev = [
   "pre-commit==3.5.0",
   "mypy==1.2.0",
   "black==23.12.1",
   "isort==5.13.2",
   "autoflake==2.2.1",
   "ruff==0.1.11",
@@ -77,19 +77,19 @@
 dmc = ["dm_control>=1.0.12"]
 box2d = ["gymnasium[box2d]==0.29.*"]
 atari = [
   "gymnasium[atari]==0.29.*",
   "gymnasium[accept-rom-license]==0.29.*",
   "gymnasium[other]==0.29.*",
 ]
-minedojo = ["minedojo==0.1", "importlib_resources==5.12.0"]
-minerl = ["setuptools==66.0.0", "minerl==0.4.4"]
-diambra = ["diambra==0.0.16", "diambra-arena==2.2.2"]
-crafter = ["crafter==1.8.1"]
-mlflow = ["mlflow==2.8.0"]
+minedojo = ["minedojo==0.1", "importlib_resources==5.12.0", "gym==0.21.0"]
+minerl = ["setuptools==66.0.0", "minerl==0.4.4", "gym==0.19.0"]
+diambra = ["diambra==0.0.17", "diambra-arena==2.2.6"]
+crafter = ["crafter==1.8.3"]
+mlflow = ["mlflow==2.11.1"]
 supermario = ["gym-super-mario-bros==7.4.0", "gym<0.26"]
 
 [tool.ruff]
 line-length = 120
 # Enable Pyflakes `E` and `F` codes by default.
 select = [
   "E",
@@ -196,15 +196,15 @@
 # -> Level 4# This one isn't too hard to get passing, but return on investment is lower
 no_implicit_reexport = false
 # This one can be tricky to get passing if you use a lot of untyped libraries
 warn_return_any = false
 
 
 [tool.bumpver]
-current_version = "0.5.4"
+current_version = "0.5.5"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "v{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `sheeprl-0.5.4/setup.py` & `sheeprl-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/__init__.py` & `sheeprl-0.5.5/sheeprl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # fmt: on
 
 # Needed because MineRL 0.4.4 is not compatible with the latest version of numpy
 np.float = np.float32
 np.int = np.int64
 np.bool = bool
 
-__version__ = "0.5.4"
+__version__ = "0.5.5"
 
 
 # Replace `moviepy.decorators.use_clip_fps_by_default` method to work with python 3.8, 3.9, and 3.10
 import moviepy.decorators
 
 
 # Taken from https://github.com/Zulko/moviepy/blob/master/moviepy/decorators.py#L118
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/a2c/a2c.py` & `sheeprl-0.5.5/sheeprl/algos/a2c/a2c.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 import hydra
 import numpy as np
 import torch
 from lightning.fabric import Fabric
 from torch.utils.data import BatchSampler, DistributedSampler, RandomSampler
 from torchmetrics import SumMetric
 
-from sheeprl.algos.a2c.agent import build_agent
+from sheeprl.algos.a2c.agent import A2CAgent, build_agent
 from sheeprl.algos.a2c.loss import policy_loss, value_loss
-from sheeprl.algos.a2c.utils import test
+from sheeprl.algos.a2c.utils import prepare_obs, test
 from sheeprl.data import ReplayBuffer
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
 from sheeprl.utils.utils import gae, save_configs
 
 
 def train(
     fabric: Fabric,
-    agent: torch.nn.Module,
+    agent: A2CAgent,
     optimizer: torch.optim.Optimizer,
     data: Dict[str, torch.Tensor],
     aggregator: MetricAggregator,
     cfg: Dict[str, Any],
 ):
     """Train the agent on the data collected from the environment."""
 
@@ -63,15 +63,17 @@
     for i, batch_idxes in enumerate(sampler):
         batch = {k: v[batch_idxes] for k, v in data.items()}
         obs = {k: v for k, v in batch.items() if k in cfg.algo.mlp_keys.encoder}
 
         # is_accumulating is True for every i except for the last one
         is_accumulating = i < len(sampler) - 1
 
-        with fabric.no_backward_sync(agent, enabled=is_accumulating):
+        with fabric.no_backward_sync(agent.feature_extractor, enabled=is_accumulating), fabric.no_backward_sync(
+            agent.actor, enabled=is_accumulating
+        ), fabric.no_backward_sync(agent.critic, enabled=is_accumulating):
             _, logprobs, values = agent(obs, torch.split(batch["actions"], agent.actions_dim, dim=-1))
 
             # Policy loss
             pg_loss = policy_loss(
                 logprobs,
                 batch["advantages"],
                 cfg.algo.loss_reduction,
@@ -159,15 +161,15 @@
         else (envs.single_action_space.nvec.tolist() if is_multidiscrete else [envs.single_action_space.n])
     )
 
     # Create the agent model: this should be a torch.nn.Module to be accelerated with Fabric
     # Given that the environment has been created with the `make_env` method, the agent
     # forward method must accept as input a dictionary like {"obs1_name": obs1, "obs2_name": obs2, ...}.
     # The agent should be able to process both image and vector-like observations.
-    agent = build_agent(
+    agent, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["agent"] if cfg.checkpoint.resume_from else None,
     )
@@ -220,76 +222,94 @@
     # Get the first environment observation and start the optimization
     step_data = {}
     next_obs = envs.reset(seed=cfg.seed)[0]  # [N_envs, N_obs]
     for k in obs_keys:
         step_data[k] = next_obs[k][np.newaxis]
 
     for update in range(1, num_updates + 1):
-        for _ in range(0, cfg.algo.rollout_steps):
-            policy_step += cfg.env.num_envs * world_size
-
-            # Measure environment interaction time: this considers both the model forward
-            # to get the action given the observation and the time taken into the environment
-            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-                with torch.no_grad():
+        with torch.inference_mode():
+            for _ in range(0, cfg.algo.rollout_steps):
+                policy_step += cfg.env.num_envs * world_size
+
+                # Measure environment interaction time: this considers both the model forward
+                # to get the action given the observation and the time taken into the environment
+                with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                     # Sample an action given the observation received by the environment
                     # This calls the `forward` method of the PyTorch module, escaping from Fabric
                     # because we don't want this to be a synchronization point
-                    torch_obs = {k: torch.as_tensor(next_obs[k], dtype=torch.float32, device=device) for k in obs_keys}
-                    actions, _, values = agent.module(torch_obs)
+                    torch_obs = prepare_obs(fabric, next_obs, num_envs=cfg.env.num_envs)
+                    actions, _, values = player(torch_obs)
                     if is_continuous:
                         real_actions = torch.cat(actions, -1).cpu().numpy()
                     else:
                         real_actions = torch.cat([act.argmax(dim=-1) for act in actions], axis=-1).cpu().numpy()
                     actions = torch.cat(actions, -1).cpu().numpy()
 
-                # Single environment step
-                obs, rewards, done, truncated, info = envs.step(real_actions.reshape(envs.action_space.shape))
-
-            dones = np.logical_or(done, truncated)
-            dones = dones.reshape(cfg.env.num_envs, -1)
-            rewards = rewards.reshape(cfg.env.num_envs, -1)
-
-            # Update the step data
-            step_data["dones"] = dones[np.newaxis]
-            step_data["values"] = values.cpu().numpy()[np.newaxis]
-            step_data["actions"] = actions[np.newaxis]
-            step_data["rewards"] = rewards[np.newaxis]
-            if cfg.buffer.memmap:
-                step_data["returns"] = np.zeros_like(rewards, shape=(1, *rewards.shape))
-                step_data["advantages"] = np.zeros_like(rewards, shape=(1, *rewards.shape))
-
-            # Append data to buffer
-            rb.add(step_data, validate_args=cfg.buffer.validate_args)
-
-            # Update the observation and dones
-            next_obs = {}
-            for k in obs_keys:
-                _obs = obs[k]
-                step_data[k] = _obs[np.newaxis]
-                next_obs[k] = _obs
-
-            if cfg.metric.log_level > 0 and "final_info" in info:
-                for i, agent_ep_info in enumerate(info["final_info"]):
-                    if agent_ep_info is not None:
-                        ep_rew = agent_ep_info["episode"]["r"]
-                        ep_len = agent_ep_info["episode"]["l"]
-                        if aggregator and "Rewards/rew_avg" in aggregator:
-                            aggregator.update("Rewards/rew_avg", ep_rew)
-                        if aggregator and "Game/ep_len_avg" in aggregator:
-                            aggregator.update("Game/ep_len_avg", ep_len)
-                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+                    # Single environment step
+                    obs, rewards, terminated, truncated, info = envs.step(real_actions.reshape(envs.action_space.shape))
+                    truncated_envs = np.nonzero(truncated)[0]
+                    if len(truncated_envs) > 0:
+                        real_next_obs = {
+                            k: torch.empty(
+                                len(truncated_envs),
+                                *observation_space[k].shape,
+                                dtype=torch.float32,
+                                device=device,
+                            )
+                            for k in obs_keys
+                        }
+                        for i, truncated_env in enumerate(truncated_envs):
+                            for k, v in info["final_observation"][truncated_env].items():
+                                torch_v = torch.as_tensor(v, dtype=torch.float32, device=device)
+                                if k in cfg.algo.cnn_keys.encoder:
+                                    torch_v = torch_v.view(-1, *v.shape[-2:])
+                                    torch_v = torch_v / 255.0 - 0.5
+                                real_next_obs[k][i] = torch_v
+                        vals = player.get_values(real_next_obs).cpu().numpy()
+                        rewards[truncated_envs] += cfg.algo.gamma * vals.reshape(rewards[truncated_envs].shape)
+                    dones = np.logical_or(terminated, truncated).reshape(cfg.env.num_envs, -1).astype(np.uint8)
+                    rewards = rewards.reshape(cfg.env.num_envs, -1)
+
+                # Update the step data
+                step_data["dones"] = dones[np.newaxis]
+                step_data["values"] = values.cpu().numpy()[np.newaxis]
+                step_data["actions"] = actions.reshape(1, cfg.env.num_envs, -1)
+                step_data["rewards"] = rewards[np.newaxis]
+                if cfg.buffer.memmap:
+                    step_data["returns"] = np.zeros_like(rewards, shape=(1, *rewards.shape))
+                    step_data["advantages"] = np.zeros_like(rewards, shape=(1, *rewards.shape))
+
+                # Append data to buffer
+                rb.add(step_data, validate_args=cfg.buffer.validate_args)
+
+                # Update the observation and dones
+                next_obs = {}
+                for k in obs_keys:
+                    _obs = obs[k]
+                    step_data[k] = _obs[np.newaxis]
+                    next_obs[k] = _obs
+
+                if cfg.metric.log_level > 0 and "final_info" in info:
+                    for i, agent_ep_info in enumerate(info["final_info"]):
+                        if agent_ep_info is not None:
+                            ep_rew = agent_ep_info["episode"]["r"]
+                            ep_len = agent_ep_info["episode"]["l"]
+                            if aggregator and "Rewards/rew_avg" in aggregator:
+                                aggregator.update("Rewards/rew_avg", ep_rew)
+                            if aggregator and "Game/ep_len_avg" in aggregator:
+                                aggregator.update("Game/ep_len_avg", ep_len)
+                            fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
 
         # Transform the data into PyTorch Tensors
         local_data = rb.to_tensor(dtype=None, device=device, from_numpy=cfg.buffer.from_numpy)
 
         # Estimate returns with GAE (https://arxiv.org/abs/1506.02438)
-        with torch.no_grad():
-            torch_obs = {k: torch.as_tensor(next_obs[k], dtype=torch.float32, device=device) for k in obs_keys}
-            next_values = agent.module.get_value(torch_obs)
+        with torch.inference_mode():
+            torch_obs = prepare_obs(fabric, next_obs, num_envs=cfg.env.num_envs)
+            next_values = player.get_values(torch_obs)
             returns, advantages = gae(
                 local_data["rewards"].to(torch.float64),
                 local_data["values"],
                 local_data["dones"],
                 next_values,
                 cfg.algo.rollout_steps,
                 cfg.algo.gamma,
@@ -334,28 +354,28 @@
             last_log = policy_step
             last_train = train_step
 
         # Checkpoint model
         if (
             (cfg.checkpoint.every > 0 and policy_step - last_checkpoint >= cfg.checkpoint.every)
             or cfg.dry_run
-            or update == num_updates
+            or (update == num_updates and cfg.checkpoint.save_last)
         ):
             last_checkpoint = policy_step
             state = {
                 "agent": agent.state_dict(),
                 "optimizer": optimizer.state_dict(),
                 "update_step": update,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call("on_checkpoint_coupled", fabric=fabric, ckpt_path=ckpt_path, state=state)
 
     envs.close()
-    if fabric.is_global_zero:
-        test(agent.module, fabric, cfg, log_dir)
+    if fabric.is_global_zero and cfg.algo.run_test:
+        test(player, fabric, cfg, log_dir)
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.ppo.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
         models_to_log = {"agent": agent}
         register_model(fabric, log_models, cfg, models_to_log)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/a2c/agent.py` & `sheeprl-0.5.5/sheeprl/algos/a2c/agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+from __future__ import annotations
+
+import copy
 from typing import Any, Dict, List, Optional, Sequence, Tuple
 
 import gymnasium
+import hydra
 import torch
 import torch.nn as nn
 from lightning import Fabric
-from lightning.fabric.wrappers import _FabricModule
 from torch import Tensor
-from torch.distributions import Distribution, Independent, Normal
+from torch.distributions import Distribution, Independent, Normal, OneHotCategorical
 
+from sheeprl.algos.ppo.agent import PPOActor, PPOPlayer
 from sheeprl.models.models import MLP
-from sheeprl.utils.distribution import OneHotCategoricalValidateArgs
+from sheeprl.utils.fabric import get_single_device_fabric
 
 
 class MLPEncoder(nn.Module):
     def __init__(
         self,
         input_dim: int,
         features_dim: int,
@@ -22,15 +26,15 @@
         mlp_layers: int = 2,
         dense_act: nn.Module = nn.ReLU,
         layer_norm: bool = False,
     ) -> None:
         super().__init__()
         self.keys = keys
         self.input_dim = input_dim
-        self.output_dim = features_dim
+        self.output_dim = features_dim if features_dim else dense_units
         self.model = MLP(
             input_dim,
             features_dim,
             [dense_units] * mlp_layers,
             activation=dense_act,
             norm_layer=[nn.LayerNorm for _ in range(mlp_layers)] if layer_norm else None,
             norm_args=[{"normalized_shape": dense_units} for _ in range(mlp_layers)] if layer_norm else None,
@@ -65,135 +69,135 @@
         self.feature_extractor = (
             MLPEncoder(
                 mlp_input_dim,
                 encoder_cfg.mlp_features_dim,
                 mlp_keys,
                 encoder_cfg.dense_units,
                 encoder_cfg.mlp_layers,
-                eval(encoder_cfg.dense_act),
+                hydra.utils.get_class(encoder_cfg.dense_act),
                 encoder_cfg.layer_norm,
             )
             if mlp_keys is not None and len(mlp_keys) > 0
             else None
         )
         features_dim = self.feature_extractor.output_dim
 
         # Critic
         self.critic = MLP(
             input_dims=features_dim,
             output_dim=1,
             hidden_sizes=[critic_cfg.dense_units] * critic_cfg.mlp_layers,
-            activation=eval(critic_cfg.dense_act),
+            activation=hydra.utils.get_class(critic_cfg.dense_act),
             norm_layer=[nn.LayerNorm for _ in range(critic_cfg.mlp_layers)] if critic_cfg.layer_norm else None,
             norm_args=(
                 [{"normalized_shape": critic_cfg.dense_units} for _ in range(critic_cfg.mlp_layers)]
                 if critic_cfg.layer_norm
                 else None
             ),
         )
 
         # Actor
-        self.actor_backbone = MLP(
-            input_dims=features_dim,
-            output_dim=None,
-            hidden_sizes=[actor_cfg.dense_units] * actor_cfg.mlp_layers,
-            activation=eval(actor_cfg.dense_act),
-            flatten_dim=None,
-            norm_layer=[nn.LayerNorm] * actor_cfg.mlp_layers if actor_cfg.layer_norm else None,
-            norm_args=(
-                [{"normalized_shape": actor_cfg.dense_units} for _ in range(actor_cfg.mlp_layers)]
-                if actor_cfg.layer_norm
-                else None
-            ),
+        actor_backbone = (
+            MLP(
+                input_dims=features_dim,
+                output_dim=None,
+                hidden_sizes=[actor_cfg.dense_units] * actor_cfg.mlp_layers,
+                activation=hydra.utils.get_class(actor_cfg.dense_act),
+                flatten_dim=None,
+                norm_layer=[nn.LayerNorm] * actor_cfg.mlp_layers if actor_cfg.layer_norm else None,
+                norm_args=(
+                    [{"normalized_shape": actor_cfg.dense_units} for _ in range(actor_cfg.mlp_layers)]
+                    if actor_cfg.layer_norm
+                    else None
+                ),
+            )
+            if actor_cfg.mlp_layers > 0
+            else nn.Identity()
         )
         if is_continuous:
             # Output is a tuple of two elements: mean and log_std, one for every action
-            self.actor_heads = nn.ModuleList([nn.Linear(actor_cfg.dense_units, sum(actions_dim) * 2)])
+            actor_heads = nn.ModuleList([nn.Linear(actor_cfg.dense_units, sum(actions_dim) * 2)])
         else:
             # Output is a tuple of one element: logits, one for every action
-            self.actor_heads = nn.ModuleList(
-                [nn.Linear(actor_cfg.dense_units, action_dim) for action_dim in actions_dim]
-            )
+            actor_heads = nn.ModuleList([nn.Linear(actor_cfg.dense_units, action_dim) for action_dim in actions_dim])
+        self.actor = PPOActor(actor_backbone, actor_heads, is_continuous=is_continuous)
 
     def forward(
-        self, obs: Dict[str, Tensor], actions: Optional[List[Tensor]] = None
+        self, obs: Dict[str, Tensor], actions: Optional[List[Tensor]] = None, greedy: bool = False
     ) -> Tuple[Sequence[Tensor], Tensor, Tensor]:
         feat = self.feature_extractor(obs)
-        out: Tensor = self.actor_backbone(feat)
-        pre_dist: List[Tensor] = [head(out) for head in self.actor_heads]
+        pre_dist: List[Tensor] = self.actor(feat)
         values = self.critic(feat)
         if self.is_continuous:
             mean, log_std = torch.chunk(pre_dist[0], chunks=2, dim=-1)
             std = log_std.exp()
-            normal = Independent(
-                Normal(mean, std, validate_args=self.distribution_cfg.validate_args),
-                1,
-                validate_args=self.distribution_cfg.validate_args,
-            )
+            normal = Independent(Normal(mean, std), 1)
             if actions is None:
-                actions = normal.sample()
+                actions = normal.mode if greedy else normal.sample()
             else:
                 # always composed by a tuple of one element containing all the
                 # continuous actions
                 actions = actions[0]
             log_prob = normal.log_prob(actions)
             return tuple([actions]), log_prob.unsqueeze(dim=-1), values
         else:
             should_append = False
             actions_logprobs: List[Tensor] = []
             actions_dist: List[Distribution] = []
             if actions is None:
                 should_append = True
                 actions: List[Tensor] = []
             for i, logits in enumerate(pre_dist):
-                actions_dist.append(
-                    OneHotCategoricalValidateArgs(logits=logits, validate_args=self.distribution_cfg.validate_args)
-                )
+                actions_dist.append(OneHotCategorical(logits=logits))
                 if should_append:
-                    actions.append(actions_dist[-1].sample())
+                    actions.append(actions_dist[-1].mode if greedy else actions_dist[-1].sample())
                 actions_logprobs.append(actions_dist[-1].log_prob(actions[i]))
             return tuple(actions), torch.stack(actions_logprobs, dim=-1).sum(dim=-1, keepdim=True), values
 
     def get_value(self, obs: Dict[str, Tensor]) -> Tensor:
         feat = self.feature_extractor(obs)
         return self.critic(feat)
 
-    def get_greedy_actions(self, obs: Dict[str, Tensor]) -> Sequence[Tensor]:
-        feat = self.feature_extractor(obs)
-        out = self.actor_backbone(feat)
-        pre_dist: List[Tensor] = [head(out) for head in self.actor_heads]
-        if self.is_continuous:
-            # Just take the mean of the distribution
-            return [torch.chunk(pre_dist[0], 2, -1)[0]]
-        else:
-            # Take the mode of the distribution
-            return tuple(
-                [
-                    OneHotCategoricalValidateArgs(logits=logits, validate_args=self.distribution_cfg.validate_args).mode
-                    for logits in pre_dist
-                ]
-            )
-
 
 def build_agent(
     fabric: Fabric,
     actions_dim: Sequence[int],
     is_continuous: bool,
     cfg: Dict[str, Any],
     obs_space: gymnasium.spaces.Dict,
     agent_state: Optional[Dict[str, Tensor]] = None,
-) -> _FabricModule:
+) -> Tuple[A2CAgent, PPOPlayer]:
     agent = A2CAgent(
         actions_dim=actions_dim,
         obs_space=obs_space,
         encoder_cfg=cfg.algo.encoder,
         actor_cfg=cfg.algo.actor,
         critic_cfg=cfg.algo.critic,
         mlp_keys=cfg.algo.mlp_keys.encoder,
         distribution_cfg=cfg.distribution,
         is_continuous=is_continuous,
     )
     if agent_state:
         agent.load_state_dict(agent_state)
-    agent = fabric.setup_module(agent)
 
-    return agent
+    # Setup player agent
+    player = PPOPlayer(copy.deepcopy(agent.feature_extractor), copy.deepcopy(agent.actor), copy.deepcopy(agent.critic))
+
+    # Setup training agent
+    agent.feature_extractor = fabric.setup_module(agent.feature_extractor)
+    agent.critic = fabric.setup_module(agent.critic)
+    agent.actor = fabric.setup_module(agent.actor)
+
+    # Setup player agent
+    fabric_player = get_single_device_fabric(fabric)
+    player.feature_extractor = fabric_player.setup_module(player.feature_extractor)
+    player.critic = fabric_player.setup_module(player.critic)
+    player.actor = fabric_player.setup_module(player.actor)
+
+    # Tie weights between the agent and the player
+    for agent_p, player_p in zip(agent.feature_extractor.parameters(), player.feature_extractor.parameters()):
+        player_p.data = agent_p.data
+    for agent_p, player_p in zip(agent.actor.parameters(), player.actor.parameters()):
+        player_p.data = agent_p.data
+    for agent_p, player_p in zip(agent.critic.parameters(), player.critic.parameters()):
+        player_p.data = agent_p.data
+    return agent, player
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/a2c/evaluate.py` & `sheeprl-0.5.5/sheeprl/algos/a2c/evaluate.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,9 +50,10 @@
     is_multidiscrete = isinstance(env.action_space, gym.spaces.MultiDiscrete)
     actions_dim = tuple(
         env.action_space.shape
         if is_continuous
         else (env.action_space.nvec.tolist() if is_multidiscrete else [env.action_space.n])
     )
     # Create the actor and critic models
-    agent = build_agent(fabric, actions_dim, is_continuous, cfg, observation_space, state["agent"])
+    _, agent = build_agent(fabric, actions_dim, is_continuous, cfg, observation_space, state["agent"])
+    del _
     test(agent, fabric, cfg, log_dir)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/a2c/loss.py` & `sheeprl-0.5.5/sheeprl/algos/a2c/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/algos/a2c/utils.py` & `sheeprl-0.5.5/sheeprl/algos/a2c/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,50 @@
+from __future__ import annotations
+
 from typing import Any, Dict
 
+import numpy as np
 import torch
 from lightning import Fabric
+from torch import Tensor
 
-from sheeprl.algos.a2c.agent import A2CAgent
+from sheeprl.algos.ppo.agent import PPOPlayer
 from sheeprl.utils.env import make_env
 
 AGGREGATOR_KEYS = {"Rewards/rew_avg", "Game/ep_len_avg", "Loss/value_loss", "Loss/policy_loss"}
 
 
+def prepare_obs(fabric: Fabric, obs: Dict[str, np.ndarray], *, num_envs: int = 1, **kwargs) -> Dict[str, Tensor]:
+    torch_obs = {k: torch.from_numpy(v.copy()).to(fabric.device).float().reshape(num_envs, -1) for k, v in obs.items()}
+    return torch_obs
+
+
 @torch.no_grad()
-def test(agent: A2CAgent, fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
+def test(agent: PPOPlayer, fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
     env = make_env(cfg, None, 0, log_dir, "test", vector_env_idx=0)()
     agent.eval()
     done = False
     cumulative_rew = 0
-    o = env.reset(seed=cfg.seed)[0]
-    obs = {}
-    for k in o.keys():
-        if k in cfg.algo.mlp_keys.encoder:
-            torch_obs = torch.from_numpy(o[k]).to(fabric.device).unsqueeze(0)
-            torch_obs = torch_obs.float()
-            obs[k] = torch_obs
+    obs = env.reset(seed=cfg.seed)[0]
 
     while not done:
+        # Convert observations to tensors
+        torch_obs = prepare_obs(fabric, obs)
+
         # Act greedly through the environment
-        if agent.is_continuous:
-            actions = torch.cat(agent.get_greedy_actions(obs), dim=-1)
+        actions = agent.get_actions(torch_obs, greedy=True)
+        if agent.actor.is_continuous:
+            actions = torch.cat(actions, dim=-1)
         else:
-            actions = torch.cat([act.argmax(dim=-1) for act in agent.get_greedy_actions(obs)], dim=-1)
+            actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1)
 
         # Single environment step
-        o, reward, done, truncated, _ = env.step(actions.cpu().numpy().reshape(env.action_space.shape))
+        obs, reward, done, truncated, _ = env.step(actions.cpu().numpy().reshape(env.action_space.shape))
         done = done or truncated
         cumulative_rew += reward
-        obs = {}
-        for k in o.keys():
-            if k in cfg.algo.mlp_keys.encoder:
-                torch_obs = torch.from_numpy(o[k]).to(fabric.device).unsqueeze(0)
-                torch_obs = torch_obs.float()
-                obs[k] = torch_obs
 
         if cfg.dry_run:
             done = True
     fabric.print("Test - Reward:", cumulative_rew)
     if cfg.metric.log_level > 0:
         fabric.log_dict({"Test/cumulative_reward": cumulative_rew}, 0)
     env.close()
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v1/agent.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v1/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import copy
 from typing import Any, Dict, Optional, Sequence, Tuple
 
 import gymnasium
 import hydra
 import numpy as np
 import torch
 from lightning.fabric import Fabric
@@ -13,14 +14,15 @@
 
 from sheeprl.algos.dreamer_v1.utils import compute_stochastic_state
 from sheeprl.algos.dreamer_v2.agent import Actor as DV2Actor
 from sheeprl.algos.dreamer_v2.agent import CNNDecoder, CNNEncoder
 from sheeprl.algos.dreamer_v2.agent import MinedojoActor as DV2MinedojoActor
 from sheeprl.algos.dreamer_v2.agent import MLPDecoder, MLPEncoder
 from sheeprl.models.models import MLP, MultiDecoder, MultiEncoder
+from sheeprl.utils.fabric import get_single_device_fabric
 from sheeprl.utils.utils import init_weights
 
 # In order to use the hydra.utils.get_class method, in this way the user can
 # specify in the configs the name of the class without having to know where
 # to go to retrieve the class
 Actor = DV2Actor
 MinedojoActor = DV2MinedojoActor
@@ -145,32 +147,29 @@
             of the distribution of the posterior state.
             posterior (Tensor): the sampled posterior.
         """
         posterior_mean_std, posterior = compute_stochastic_state(
             self.representation_model(torch.cat((recurrent_state, embedded_obs), -1)),
             event_shape=1,
             min_std=self.min_std,
-            validate_args=self.distribution_cfg.validate_args,
         )
         return posterior_mean_std, posterior
 
     def _transition(self, recurrent_out: Tensor) -> Tuple[Tuple[Tensor, Tensor], Tensor]:
         """Predict the prior state (Transition Model).
 
         Args:
             recurrent_out (Tensor): the output of the recurrent model, i.e., the deterministic part of the latent space.
 
         Returns:
             The predicted mean and the standard deviation of the distribution of the prior state (Tensor, Tensor).
             The prior state (Tensor): the sampled prior state predicted by the transition model.
         """
         prior_mean_std = self.transition_model(recurrent_out)
-        return compute_stochastic_state(
-            prior_mean_std, event_shape=1, min_std=self.min_std, validate_args=self.distribution_cfg.validate_args
-        )
+        return compute_stochastic_state(prior_mean_std, event_shape=1, min_std=self.min_std)
 
     def imagination(self, stochastic_state: Tensor, recurrent_state: Tensor, actions: Tensor) -> Tuple[Tensor, Tensor]:
         """One-step imagination of the next latent state.
         It can be used several times to imagine trajectories in the latent space (Transition Model).
 
         Args:
             stochastic_state (Tensor): the stochastic space (can be either the posterior or the prior).
@@ -217,52 +216,50 @@
         self.continue_model = continue_model
 
 
 class PlayerDV1(nn.Module):
     """The model of the DreamerV1 player.
 
     Args:
-        encoder (nn.Module): the encoder.
-        recurrent_model (nn.Module): the recurrent model.
-        representation_model (nn.Module): the representation model.
-        actor (nn.Module): the actor.
+        encoder (nn.Module| _FabricModule): the encoder.
+        recurrent_model (nn.Module| _FabricModule): the recurrent model.
+        representation_model (nn.Module| _FabricModule): the representation model.
+        actor (nn.Module| _FabricModule): the actor.
         actions_dim (Sequence[int]): the dimension of each action.
         num_envs (int): the number of environments.
         stochastic_size (int): the size of the stochastic state.
         recurrent_state_size (int): the size of the recurrent state.
-        device (torch.device): the device to work on.
+        device (str | torch.device): the device where the model is stored.
         actor_type (str, optional): which actor the player is using ('task' or 'exploration').
             Default to None.
     """
 
     def __init__(
         self,
-        encoder: nn.Module,
-        recurrent_model: nn.Module,
-        representation_model: nn.Module,
-        actor: nn.Module,
+        encoder: MultiEncoder | _FabricModule,
+        recurrent_model: RecurrentModel | _FabricModule,
+        representation_model: MLP | _FabricModule,
+        actor: Actor | _FabricModule,
         actions_dim: Sequence[int],
         num_envs: int,
         stochastic_size: int,
         recurrent_state_size: int,
-        device: torch.device,
+        device: str | torch.device,
         actor_type: str | None = None,
     ) -> None:
         super().__init__()
         self.encoder = encoder
         self.recurrent_model = recurrent_model
         self.representation_model = representation_model
         self.actor = actor
-        self.device = device
         self.actions_dim = actions_dim
+        self.num_envs = num_envs
         self.stochastic_size = stochastic_size
         self.recurrent_state_size = recurrent_state_size
-        self.num_envs = num_envs
-        self.validate_args = self.actor.distribution_cfg.validate_args
-        self.init_states()
+        self.device = device
         self.actor_type = actor_type
 
     def init_states(self, reset_envs: Optional[Sequence[int]] = None) -> None:
         """Initialize the states and the actions for the ended environments.
 
         Args:
             reset_envs (Optional[Sequence[int]], optional): which environments' states to reset.
@@ -274,70 +271,75 @@
             self.recurrent_state = torch.zeros(1, self.num_envs, self.recurrent_state_size, device=self.device)
             self.stochastic_state = torch.zeros(1, self.num_envs, self.stochastic_size, device=self.device)
         else:
             self.actions[:, reset_envs] = torch.zeros_like(self.actions[:, reset_envs])
             self.recurrent_state[:, reset_envs] = torch.zeros_like(self.recurrent_state[:, reset_envs])
             self.stochastic_state[:, reset_envs] = torch.zeros_like(self.stochastic_state[:, reset_envs])
 
-    def get_exploration_action(self, obs: Tensor, mask: Optional[Dict[str, Tensor]] = None) -> Sequence[Tensor]:
+    def get_exploration_actions(
+        self, obs: Tensor, greedy: bool = False, mask: Optional[Dict[str, Tensor]] = None, step: int = 0
+    ) -> Sequence[Tensor]:
         """Return the actions with a certain amount of noise for exploration.
 
         Args:
             obs (Tensor): the current observations.
+            greedy (bool): whether or not to sample the actions.
+                Default to False.
             mask (Dict[str, Tensor], optional): the action mask (whether or not each action can be executed).
                 Defaults to None.
+            step (int): the step of the training, used for the exploration amount.
+                Default to 0.
 
         Returns:
             The actions the agent has to perform (Sequence[Tensor]).
         """
-        actions = self.get_greedy_action(obs, mask=mask)
+        actions = self.get_actions(obs, greedy=greedy, mask=mask)
         expl_actions = None
-        if self.actor.expl_amount > 0:
-            expl_actions = self.actor.add_exploration_noise(actions, mask=mask)
+        if self.actor._expl_amount > 0:
+            expl_actions = self.actor.add_exploration_noise(actions, step=step, mask=mask)
             self.actions = torch.cat(expl_actions, dim=-1)
         return expl_actions or actions
 
-    def get_greedy_action(
-        self, obs: Tensor, is_training: bool = True, mask: Optional[Dict[str, Tensor]] = None
+    def get_actions(
+        self, obs: Tensor, greedy: bool = False, mask: Optional[Dict[str, Tensor]] = None
     ) -> Sequence[Tensor]:
         """Return the greedy actions.
 
         Args:
             obs (Tensor): the current observations.
-            is_training (bool): whether it is training.
-                Default to True.
+            greedy (bool): whether or not to sample the actions.
+                Default to False.
             mask (Dict[str, Tensor], optional): the action mask (whether or not each action can be executed).
                 Defaults to None.
 
         Returns:
             The actions the agent has to perform (Sequence[Tensor]).
         """
         embedded_obs = self.encoder(obs)
         _, self.recurrent_state = self.recurrent_model(
             torch.cat((self.stochastic_state, self.actions), -1), self.recurrent_state
         )
         _, self.stochastic_state = compute_stochastic_state(
             self.representation_model(torch.cat((self.recurrent_state, embedded_obs), -1)),
-            validate_args=self.validate_args,
         )
-        actions, _ = self.actor(torch.cat((self.stochastic_state, self.recurrent_state), -1), is_training, mask)
+        actions, _ = self.actor(torch.cat((self.stochastic_state, self.recurrent_state), -1), greedy, mask)
         self.actions = torch.cat(actions, -1)
         return actions
 
 
 def build_agent(
     fabric: Fabric,
     actions_dim: Sequence[int],
     is_continuous: bool,
     cfg: Dict[str, Any],
     obs_space: gymnasium.spaces.Dict,
     world_model_state: Optional[Dict[str, Tensor]] = None,
     actor_state: Optional[Dict[str, Tensor]] = None,
     critic_state: Optional[Dict[str, Tensor]] = None,
-) -> Tuple[WorldModel, _FabricModule, _FabricModule]:
+) -> Tuple[WorldModel, _FabricModule, _FabricModule, PlayerDV1]:
     """Build the models and wrap them with Fabric.
 
     Args:
         fabric (Fabric): the fabric object.
         actions_dim (Sequence[int]): the dimension of the actions.
         is_continuous (bool): whether or not the actions are continuous.
         cfg (DictConfig): the hyper-parameters of DreamerV1.
@@ -350,14 +352,15 @@
             Default to None.
 
     Returns:
         The world model (WorldModel): composed by the encoder, rssm, observation and
         reward models and the continue model.
         The actor (_FabricModule).
         The critic (_FabricModule).
+        The player (PlayerDV1).
     """
     world_model_cfg = cfg.algo.world_model
     actor_cfg = cfg.algo.actor
     critic_cfg = cfg.algo.critic
 
     # Sizes
     latent_state_size = world_model_cfg.stochastic_size + world_model_cfg.recurrent_model.recurrent_state_size
@@ -366,51 +369,51 @@
     cnn_encoder = (
         CNNEncoder(
             keys=cfg.algo.cnn_keys.encoder,
             input_channels=[int(np.prod(obs_space[k].shape[:-2])) for k in cfg.algo.cnn_keys.encoder],
             image_size=obs_space[cfg.algo.cnn_keys.encoder[0]].shape[-2:],
             channels_multiplier=world_model_cfg.encoder.cnn_channels_multiplier,
             layer_norm=False,
-            activation=eval(world_model_cfg.encoder.cnn_act),
+            activation=hydra.utils.get_class(world_model_cfg.encoder.cnn_act),
         )
         if cfg.algo.cnn_keys.encoder is not None and len(cfg.algo.cnn_keys.encoder) > 0
         else None
     )
     mlp_encoder = (
         MLPEncoder(
             keys=cfg.algo.mlp_keys.encoder,
             input_dims=[obs_space[k].shape[0] for k in cfg.algo.mlp_keys.encoder],
             mlp_layers=world_model_cfg.encoder.mlp_layers,
             dense_units=world_model_cfg.encoder.dense_units,
-            activation=eval(world_model_cfg.encoder.dense_act),
+            activation=hydra.utils.get_class(world_model_cfg.encoder.dense_act),
             layer_norm=False,
         )
         if cfg.algo.mlp_keys.encoder is not None and len(cfg.algo.mlp_keys.encoder) > 0
         else None
     )
     encoder = MultiEncoder(cnn_encoder, mlp_encoder)
     recurrent_model = RecurrentModel(
         input_size=sum(actions_dim) + world_model_cfg.stochastic_size,
         recurrent_state_size=world_model_cfg.recurrent_model.recurrent_state_size,
-        activation=eval(world_model_cfg.recurrent_model.dense_act),
+        activation=hydra.utils.get_class(world_model_cfg.recurrent_model.dense_act),
     )
     representation_model = MLP(
         input_dims=(
             world_model_cfg.recurrent_model.recurrent_state_size + encoder.cnn_output_dim + encoder.mlp_output_dim
         ),
         output_dim=world_model_cfg.stochastic_size * 2,
         hidden_sizes=[world_model_cfg.representation_model.hidden_size],
-        activation=eval(world_model_cfg.representation_model.dense_act),
+        activation=hydra.utils.get_class(world_model_cfg.representation_model.dense_act),
         flatten_dim=None,
     )
     transition_model = MLP(
         input_dims=world_model_cfg.recurrent_model.recurrent_state_size,
         output_dim=world_model_cfg.stochastic_size * 2,
         hidden_sizes=[world_model_cfg.transition_model.hidden_size],
-        activation=eval(world_model_cfg.transition_model.dense_act),
+        activation=hydra.utils.get_class(world_model_cfg.transition_model.dense_act),
         flatten_dim=None,
     )
     rssm = RSSM(
         recurrent_model=recurrent_model.apply(init_weights),
         representation_model=representation_model.apply(init_weights),
         transition_model=transition_model.apply(init_weights),
         distribution_cfg=cfg.distribution,
@@ -420,47 +423,47 @@
         CNNDecoder(
             keys=cfg.algo.cnn_keys.decoder,
             output_channels=[int(np.prod(obs_space[k].shape[:-2])) for k in cfg.algo.cnn_keys.decoder],
             channels_multiplier=world_model_cfg.observation_model.cnn_channels_multiplier,
             latent_state_size=latent_state_size,
             cnn_encoder_output_dim=cnn_encoder.output_dim,
             image_size=obs_space[cfg.algo.cnn_keys.decoder[0]].shape[-2:],
-            activation=eval(world_model_cfg.observation_model.cnn_act),
+            activation=hydra.utils.get_class(world_model_cfg.observation_model.cnn_act),
             layer_norm=False,
         )
         if cfg.algo.cnn_keys.decoder is not None and len(cfg.algo.cnn_keys.decoder) > 0
         else None
     )
     mlp_decoder = (
         MLPDecoder(
             keys=cfg.algo.mlp_keys.decoder,
             output_dims=[obs_space[k].shape[0] for k in cfg.algo.mlp_keys.decoder],
             latent_state_size=latent_state_size,
             mlp_layers=world_model_cfg.observation_model.mlp_layers,
             dense_units=world_model_cfg.observation_model.dense_units,
-            activation=eval(world_model_cfg.observation_model.dense_act),
+            activation=hydra.utils.get_class(world_model_cfg.observation_model.dense_act),
             layer_norm=False,
         )
         if cfg.algo.mlp_keys.decoder is not None and len(cfg.algo.mlp_keys.decoder) > 0
         else None
     )
     observation_model = MultiDecoder(cnn_decoder, mlp_decoder)
     reward_model = MLP(
         input_dims=latent_state_size,
         output_dim=1,
         hidden_sizes=[world_model_cfg.reward_model.dense_units] * world_model_cfg.reward_model.mlp_layers,
-        activation=eval(world_model_cfg.reward_model.dense_act),
+        activation=hydra.utils.get_class(world_model_cfg.reward_model.dense_act),
         flatten_dim=None,
     )
     if world_model_cfg.use_continues:
         continue_model = MLP(
             input_dims=latent_state_size,
             output_dim=1,
             hidden_sizes=[world_model_cfg.discount_model.dense_units] * world_model_cfg.discount_model.mlp_layers,
-            activation=eval(world_model_cfg.discount_model.dense_act),
+            activation=hydra.utils.get_class(world_model_cfg.discount_model.dense_act),
             flatten_dim=None,
         )
     world_model = WorldModel(
         encoder.apply(init_weights),
         rssm,
         observation_model.apply(init_weights),
         reward_model.apply(init_weights),
@@ -471,42 +474,74 @@
         latent_state_size=latent_state_size,
         actions_dim=actions_dim,
         is_continuous=is_continuous,
         init_std=actor_cfg.init_std,
         min_std=actor_cfg.min_std,
         mlp_layers=actor_cfg.mlp_layers,
         dense_units=actor_cfg.dense_units,
-        activation=eval(actor_cfg.dense_act),
+        activation=hydra.utils.get_class(actor_cfg.dense_act),
         distribution_cfg=cfg.distribution,
         layer_norm=False,
+        expl_amount=actor_cfg.expl_amount,
+        expl_decay=actor_cfg.expl_decay,
+        expl_min=actor_cfg.expl_min,
     )
     critic = MLP(
         input_dims=latent_state_size,
         output_dim=1,
         hidden_sizes=[critic_cfg.dense_units] * critic_cfg.mlp_layers,
-        activation=eval(critic_cfg.dense_act),
+        activation=hydra.utils.get_class(critic_cfg.dense_act),
         flatten_dim=None,
     )
     actor.apply(init_weights)
     critic.apply(init_weights)
 
     # Load models from checkpoint
     if world_model_state:
         world_model.load_state_dict(world_model_state)
     if actor_state:
         actor.load_state_dict(actor_state)
     if critic_state:
         critic.load_state_dict(critic_state)
 
+    # Create the player agent
+    fabric_player = get_single_device_fabric(fabric)
+    player = PlayerDV1(
+        copy.deepcopy(world_model.encoder),
+        copy.deepcopy(world_model.rssm.recurrent_model),
+        copy.deepcopy(world_model.rssm.representation_model),
+        copy.deepcopy(actor),
+        actions_dim,
+        cfg.env.num_envs,
+        cfg.algo.world_model.stochastic_size,
+        cfg.algo.world_model.recurrent_model.recurrent_state_size,
+        fabric_player.device,
+    )
+
     # Setup models with Fabric
     world_model.encoder = fabric.setup_module(world_model.encoder)
     world_model.observation_model = fabric.setup_module(world_model.observation_model)
     world_model.reward_model = fabric.setup_module(world_model.reward_model)
     world_model.rssm.recurrent_model = fabric.setup_module(world_model.rssm.recurrent_model)
     world_model.rssm.representation_model = fabric.setup_module(world_model.rssm.representation_model)
     world_model.rssm.transition_model = fabric.setup_module(world_model.rssm.transition_model)
     if world_model.continue_model:
         world_model.continue_model = fabric.setup_module(world_model.continue_model)
     actor = fabric.setup_module(actor)
     critic = fabric.setup_module(critic)
 
-    return world_model, actor, critic
+    # Setup the player agent with a single-device Fabric
+    player.encoder = fabric_player.setup_module(player.encoder)
+    player.recurrent_model = fabric_player.setup_module(player.recurrent_model)
+    player.representation_model = fabric_player.setup_module(player.representation_model)
+    player.actor = fabric_player.setup_module(player.actor)
+
+    # Tie weights between the agent and the player
+    for agent_p, p in zip(world_model.encoder.parameters(), player.encoder.parameters()):
+        p.data = agent_p.data
+    for agent_p, p in zip(world_model.rssm.recurrent_model.parameters(), player.recurrent_model.parameters()):
+        p.data = agent_p.data
+    for agent_p, p in zip(world_model.rssm.representation_model.parameters(), player.representation_model.parameters()):
+        p.data = agent_p.data
+    for agent_p, p in zip(actor.parameters(), player.actor.parameters()):
+        p.data = agent_p.data
+    return world_model, actor, critic, player
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v1/dreamer_v1.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v1/dreamer_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 from lightning.fabric import Fabric
 from lightning.fabric.wrappers import _FabricModule, _FabricOptimizer
 from torch import Tensor
 from torch.distributions import Bernoulli, Independent, Normal
 from torch.distributions.utils import logits_to_probs
 from torchmetrics import SumMetric
 
-from sheeprl.algos.dreamer_v1.agent import PlayerDV1, WorldModel, build_agent
+from sheeprl.algos.dreamer_v1.agent import WorldModel, build_agent
 from sheeprl.algos.dreamer_v1.loss import actor_loss, critic_loss, reconstruction_loss
 from sheeprl.algos.dreamer_v1.utils import compute_lambda_values
-from sheeprl.algos.dreamer_v2.utils import test
+from sheeprl.algos.dreamer_v2.utils import prepare_obs, test
 from sheeprl.data.buffers import EnvIndependentReplayBuffer, SequentialReplayBuffer
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import polynomial_decay, save_configs
+from sheeprl.utils.utils import Ratio, save_configs
 
 # Decomment the following two lines if you cannot start an experiment with DMC environments
 # os.environ["PYOPENGL_PLATFORM"] = ""
 # os.environ["MUJOCO_GL"] = "osmesa"
 
 
 def train(
@@ -97,15 +97,14 @@
         critic_optimizer (_FabricOptimizer): the critic optimizer.
         data (Dict[str, Tensor]): the batch of data to use for training.
         aggregator (MetricAggregator, optional): the aggregator to print the metrics.
         cfg (DictConfig): the configs.
     """
     batch_size = cfg.algo.per_rank_batch_size
     sequence_length = cfg.algo.per_rank_sequence_length
-    validate_args = cfg.distribution.validate_args
     recurrent_state_size = cfg.algo.world_model.recurrent_model.recurrent_state_size
     stochastic_size = cfg.algo.world_model.stochastic_size
     device = fabric.device
     batch_obs = {k: data[k] / 255 - 0.5 for k in cfg.algo.cnn_keys.encoder}
     batch_obs.update({k: data[k] for k in cfg.algo.mlp_keys.encoder})
 
     # Dynamic Learning
@@ -162,80 +161,60 @@
 
     # compute predictions for the observations
     decoded_information: Dict[str, torch.Tensor] = world_model.observation_model(latent_states)
     # compute the distribution of the reconstructed observations
     # it is necessary an Independent distribution because
     # it is necessary to create (batch_size * sequence_length) independent distributions,
     # each producing a sample of size observations.shape
-    qo = {
-        k: Independent(
-            Normal(rec_obs, 1, validate_args=validate_args),
-            len(rec_obs.shape[2:]),
-            validate_args=validate_args,
-        )
-        for k, rec_obs in decoded_information.items()
-    }
+    qo = {k: Independent(Normal(rec_obs, 1), len(rec_obs.shape[2:])) for k, rec_obs in decoded_information.items()}
 
     # compute predictions for the rewards
     # it is necessary an Independent distribution because
     # it is necessary to create (batch_size * sequence_length) independent distributions,
     # each producing a sample of size equal to the number of rewards
-    qr = Independent(
-        Normal(world_model.reward_model(latent_states), 1, validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
+    qr = Independent(Normal(world_model.reward_model(latent_states), 1), 1)
 
     # compute predictions for terminal steps, if required
     if cfg.algo.world_model.use_continues and world_model.continue_model:
-        qc = Independent(
-            Bernoulli(logits=world_model.continue_model(latent_states), validate_args=validate_args),
-            1,
-            validate_args=validate_args,
-        )
-        continue_targets = (1 - data["dones"]) * cfg.algo.gamma
+        qc = Independent(Bernoulli(logits=world_model.continue_model(latent_states)), 1)
+        continues_targets = (1 - data["terminated"]) * cfg.algo.gamma
     else:
-        qc = continue_targets = None
+        qc = continues_targets = None
 
     # compute the distributions of the states (posteriors and priors)
     # it is necessary an Independent distribution because
     # it is necessary to create (batch_size * sequence_length) independent distributions,
     # each producing a sample of size equal to the stochastic size
-    posteriors_dist = Independent(
-        Normal(posteriors_mean, posteriors_std, validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
-    priors_dist = Independent(
-        Normal(priors_mean, priors_std, validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
+    posteriors_dist = Independent(Normal(posteriors_mean, posteriors_std), 1)
+    priors_dist = Independent(Normal(priors_mean, priors_std), 1)
 
     # world model optimization step
     world_optimizer.zero_grad(set_to_none=True)
     # compute the overall loss of the world model
     rec_loss, kl, state_loss, reward_loss, observation_loss, continue_loss = reconstruction_loss(
         qo,
         batch_obs,
         qr,
         data["rewards"],
         posteriors_dist,
         priors_dist,
         cfg.algo.world_model.kl_free_nats,
         cfg.algo.world_model.kl_regularizer,
         qc,
-        continue_targets,
+        continues_targets,
         cfg.algo.world_model.continue_scale_factor,
     )
     fabric.backward(rec_loss)
     world_model_grads = None
     if cfg.algo.world_model.clip_gradients is not None and cfg.algo.world_model.clip_gradients > 0:
         world_model_grads = fabric.clip_gradients(
-            module=world_model, optimizer=world_optimizer, max_norm=cfg.algo.world_model.clip_gradients
+            module=world_model,
+            optimizer=world_optimizer,
+            max_norm=cfg.algo.world_model.clip_gradients,
+            error_if_nonfinite=False,
         )
     world_optimizer.step()
 
     # Behaviour Learning
     # Unflatten first 2 dimensions of recurrent and posterior states in order
     # to have all the states on the first dimension.
     # The 1 in the second dimension is needed for the recurrent model in the imagination step,
@@ -333,40 +312,42 @@
     actor_optimizer.zero_grad(set_to_none=True)
     # compute the policy loss
     policy_loss = actor_loss(discount * lambda_values)
     fabric.backward(policy_loss)
     actor_grads = None
     if cfg.algo.actor.clip_gradients is not None and cfg.algo.actor.clip_gradients > 0:
         actor_grads = fabric.clip_gradients(
-            module=actor, optimizer=actor_optimizer, max_norm=cfg.algo.actor.clip_gradients
+            module=actor,
+            optimizer=actor_optimizer,
+            max_norm=cfg.algo.actor.clip_gradients,
+            error_if_nonfinite=False,
         )
     actor_optimizer.step()
 
     # Predict the values distribution only for the first H (horizon) imagined states
     # (to match the dimension with the lambda values),
     # it removes the last imagined state in the trajectory
     # because it is used only for computing correclty the lambda values
-    qv = Independent(
-        Normal(critic(imagined_trajectories.detach())[:-1], 1, validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
+    qv = Independent(Normal(critic(imagined_trajectories.detach())[:-1], 1), 1)
 
     # critic optimization step
     critic_optimizer.zero_grad(set_to_none=True)
     # compute the value loss
     # the discount has shape (horizon, seuqence_length * batch_size, 1), so,
     # it is necessary to remove the last dimension to properly match the shapes
     # for the log prob
     value_loss = critic_loss(qv, lambda_values.detach(), discount[..., 0])
     fabric.backward(value_loss)
     critic_grads = None
     if cfg.algo.critic.clip_gradients is not None and cfg.algo.critic.clip_gradients > 0:
         critic_grads = fabric.clip_gradients(
-            module=critic, optimizer=critic_optimizer, max_norm=cfg.algo.critic.clip_gradients
+            module=critic,
+            optimizer=critic_optimizer,
+            max_norm=cfg.algo.critic.clip_gradients,
+            error_if_nonfinite=False,
         )
     critic_optimizer.step()
 
     # Log metrics
     if aggregator and not aggregator.disabled:
         aggregator.update("Loss/world_model_loss", rec_loss.detach())
         aggregator.update("Loss/observation_loss", observation_loss.detach())
@@ -392,16 +373,14 @@
 
 
 @register_algorithm()
 def main(fabric: Fabric, cfg: Dict[str, Any]):
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     # These arguments cannot be changed
     cfg.env.screen_size = 64
     cfg.env.frame_stack = 1
@@ -459,35 +438,24 @@
     if cfg.metric.log_level > 0:
         fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
         fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
         fabric.print("Decoder CNN keys:", cfg.algo.cnn_keys.decoder)
         fabric.print("Decoder MLP keys:", cfg.algo.mlp_keys.decoder)
     obs_keys = cfg.algo.cnn_keys.encoder + cfg.algo.mlp_keys.encoder
 
-    world_model, actor, critic = build_agent(
+    world_model, actor, critic, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["world_model"] if cfg.checkpoint.resume_from else None,
         state["actor"] if cfg.checkpoint.resume_from else None,
         state["critic"] if cfg.checkpoint.resume_from else None,
     )
-    player = PlayerDV1(
-        world_model.encoder.module,
-        world_model.rssm.recurrent_model.module,
-        world_model.rssm.representation_model.module,
-        actor.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-    )
 
     # Optimizers
     world_optimizer = hydra.utils.instantiate(
         cfg.algo.world_model.optimizer, params=world_model.parameters(), _convert_="all"
     )
     actor_optimizer = hydra.utils.instantiate(cfg.algo.actor.optimizer, params=actor.parameters(), _convert_="all")
     critic_optimizer = hydra.utils.instantiate(cfg.algo.critic.optimizer, params=critic.parameters(), _convert_="all")
@@ -536,30 +504,26 @@
         if cfg.checkpoint.resume_from
         else 1
     )
     policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
     policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    updates_before_training = cfg.algo.train_every // policy_steps_per_update if not cfg.dry_run else 0
     num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
     learning_starts = (cfg.algo.learning_starts // policy_steps_per_update) if not cfg.dry_run else 0
-    expl_decay_steps = state["expl_decay_steps"] if cfg.checkpoint.resume_from else 0
-    max_step_expl_decay = cfg.algo.actor.max_step_expl_decay // (cfg.algo.per_rank_gradient_steps * world_size)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        actor.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
         if not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -575,161 +539,158 @@
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         if k in cfg.algo.cnn_keys.encoder:
             obs[k] = obs[k].reshape(cfg.env.num_envs, -1, *obs[k].shape[-2:])
         step_data[k] = obs[k][np.newaxis]
-    step_data["dones"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
 
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * world_size
 
-        # Measure environment interaction time: this considers both the model forward
-        # to get the action given the observation and the time taken into the environment
-        with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            # Sample an action given the observation received by the environment
-            if (
-                update <= learning_starts
-                and cfg.checkpoint.resume_from is None
-                and "minedojo" not in cfg.env.wrapper._target_.lower()
-            ):
-                real_actions = actions = np.array(envs.action_space.sample())
-                if not is_continuous:
-                    actions = np.concatenate(
-                        [
-                            F.one_hot(torch.as_tensor(act), act_dim).numpy()
-                            for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
-                        ],
-                        axis=-1,
-                    )
-            else:
-                with torch.no_grad():
-                    normalized_obs = {}
-                    for k in obs_keys:
-                        torch_obs = torch.as_tensor(obs[k][np.newaxis], dtype=torch.float32, device=device)
-                        if k in cfg.algo.cnn_keys.encoder:
-                            torch_obs = torch_obs / 255 - 0.5
-                        normalized_obs[k] = torch_obs
-                    mask = {k: v for k, v in normalized_obs.items() if k.startswith("mask")}
+        with torch.inference_mode():
+            # Measure environment interaction time: this considers both the model forward
+            # to get the action given the observation and the time taken into the environment
+            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
+                # Sample an action given the observation received by the environment
+                if (
+                    update <= learning_starts
+                    and cfg.checkpoint.resume_from is None
+                    and "minedojo" not in cfg.env.wrapper._target_.lower()
+                ):
+                    real_actions = actions = np.array(envs.action_space.sample())
+                    if not is_continuous:
+                        actions = np.concatenate(
+                            [
+                                F.one_hot(torch.as_tensor(act), act_dim).numpy()
+                                for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
+                            ],
+                            axis=-1,
+                        )
+                else:
+                    torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                    mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
-                    real_actions = actions = player.get_exploration_action(normalized_obs, mask)
+                    real_actions = actions = player.get_exploration_actions(torch_obs, mask=mask, step=policy_step)
                     actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                     if is_continuous:
                         real_actions = torch.cat(real_actions, -1).cpu().numpy()
                     else:
                         real_actions = (
                             torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
-            next_obs, rewards, dones, truncated, infos = envs.step(real_actions.reshape(envs.action_space.shape))
-            dones = np.logical_or(dones, truncated).astype(np.uint8)
+                next_obs, rewards, terminated, truncated, infos = envs.step(
+                    real_actions.reshape(envs.action_space.shape)
+                )
+                dones = np.logical_or(terminated, truncated).astype(np.uint8)
 
-        if cfg.metric.log_level > 0 and "final_info" in infos:
-            for i, agent_ep_info in enumerate(infos["final_info"]):
-                if agent_ep_info is not None:
-                    ep_rew = agent_ep_info["episode"]["r"]
-                    ep_len = agent_ep_info["episode"]["l"]
-                    if aggregator and not aggregator.disabled:
-                        aggregator.update("Rewards/rew_avg", ep_rew)
-                        aggregator.update("Game/ep_len_avg", ep_len)
-                    fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
-
-        # Save the real next observation
-        real_next_obs = copy.deepcopy(next_obs)
-        if "final_observation" in infos:
-            for idx, final_obs in enumerate(infos["final_observation"]):
-                if final_obs is not None:
-                    for k, v in final_obs.items():
-                        real_next_obs[k][idx] = v
-
-        for k in obs_keys:
-            if k in cfg.algo.cnn_keys.encoder:
-                next_obs[k] = next_obs[k].reshape(cfg.env.num_envs, -1, *next_obs[k].shape[-2:])
-                real_next_obs[k] = real_next_obs[k].reshape(cfg.env.num_envs, -1, *real_next_obs[k].shape[-2:])
-            step_data[k] = real_next_obs[k][np.newaxis]
-
-        # next_obs becomes the new obs
-        obs = next_obs
-
-        step_data["dones"] = dones[np.newaxis]
-        step_data["actions"] = actions[np.newaxis]
-        step_data["rewards"] = clip_rewards_fn(rewards)[np.newaxis]
-        rb.add(step_data, validate_args=cfg.buffer.validate_args)
-
-        # Reset and save the observation coming from the automatic reset
-        dones_idxes = dones.nonzero()[0].tolist()
-        reset_envs = len(dones_idxes)
-        if reset_envs > 0:
-            reset_data = {}
-            for k in obs_keys:
-                reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
-            reset_data["dones"] = np.zeros((1, reset_envs, 1))
-            reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
-            reset_data["rewards"] = np.zeros((1, reset_envs, 1))
-            rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
-            # Reset dones so that `is_first` is updated
-            for d in dones_idxes:
-                step_data["dones"][0, d] = np.zeros_like(step_data["dones"][0, d])
-            # Reset internal agent states
-            player.init_states(reset_envs=dones_idxes)
+            if cfg.metric.log_level > 0 and "final_info" in infos:
+                for i, agent_ep_info in enumerate(infos["final_info"]):
+                    if agent_ep_info is not None:
+                        ep_rew = agent_ep_info["episode"]["r"]
+                        ep_len = agent_ep_info["episode"]["l"]
+                        if aggregator and not aggregator.disabled:
+                            aggregator.update("Rewards/rew_avg", ep_rew)
+                            aggregator.update("Game/ep_len_avg", ep_len)
+                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+
+            # Save the real next observation
+            real_next_obs = copy.deepcopy(next_obs)
+            if "final_observation" in infos:
+                for idx, final_obs in enumerate(infos["final_observation"]):
+                    if final_obs is not None:
+                        for k, v in final_obs.items():
+                            real_next_obs[k][idx] = v
 
-        updates_before_training -= 1
+            for k in obs_keys:
+                if k in cfg.algo.cnn_keys.encoder:
+                    next_obs[k] = next_obs[k].reshape(cfg.env.num_envs, -1, *next_obs[k].shape[-2:])
+                    real_next_obs[k] = real_next_obs[k].reshape(cfg.env.num_envs, -1, *real_next_obs[k].shape[-2:])
+                step_data[k] = real_next_obs[k][np.newaxis]
+
+            # next_obs becomes the new obs
+            obs = next_obs
+
+            step_data["terminated"] = terminated[np.newaxis]
+            step_data["truncated"] = truncated[np.newaxis]
+            step_data["actions"] = actions[np.newaxis]
+            step_data["rewards"] = clip_rewards_fn(rewards)[np.newaxis]
+            rb.add(step_data, validate_args=cfg.buffer.validate_args)
+
+            # Reset and save the observation coming from the automatic reset
+            dones_idxes = dones.nonzero()[0].tolist()
+            reset_envs = len(dones_idxes)
+            if reset_envs > 0:
+                reset_data = {}
+                for k in obs_keys:
+                    reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
+                reset_data["terminated"] = np.zeros((1, reset_envs, 1))
+                reset_data["truncated"] = np.zeros((1, reset_envs, 1))
+                reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
+                reset_data["rewards"] = np.zeros((1, reset_envs, 1))
+                rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
+                for d in dones_idxes:
+                    step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
+                    step_data["truncated"][0, d] = np.zeros_like(step_data["truncated"][0, d])
+                # Reset internal agent states
+                player.init_states(reset_envs=dones_idxes)
 
         # Train the agent
-        if update > learning_starts and updates_before_training <= 0:
-            # Start training
-            with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
-                for i in range(cfg.algo.per_rank_gradient_steps):
+        if update >= learning_starts:
+            per_rank_gradient_steps = ratio(policy_step / world_size)
+            if per_rank_gradient_steps > 0:
+                with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
                     sample = rb.sample_tensors(
                         batch_size=cfg.algo.per_rank_batch_size,
                         sequence_length=cfg.algo.per_rank_sequence_length,
-                        n_samples=1,
+                        n_samples=per_rank_gradient_steps,
                         dtype=None,
                         device=device,
                         from_numpy=cfg.buffer.from_numpy,
                     )  # [N_samples, Seq_len, Batch_size, ...]
-                    batch = {k: v[0].float() for k, v in sample.items()}
-                    train(
-                        fabric,
-                        world_model,
-                        actor,
-                        critic,
-                        world_optimizer,
-                        actor_optimizer,
-                        critic_optimizer,
-                        batch,
-                        aggregator,
-                        cfg,
-                    )
-                train_step += world_size
-            updates_before_training = cfg.algo.train_every // policy_steps_per_update
-            if cfg.algo.actor.expl_decay:
-                expl_decay_steps += 1
-                actor.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
-                )
-            if aggregator:
-                aggregator.update("Params/exploration_amount", actor.expl_amount)
+                    for i in range(per_rank_gradient_steps):
+                        batch = {k: v[i].float() for k, v in sample.items()}
+                        train(
+                            fabric,
+                            world_model,
+                            actor,
+                            critic,
+                            world_optimizer,
+                            actor_optimizer,
+                            critic_optimizer,
+                            batch,
+                            aggregator,
+                            cfg,
+                        )
+                        cumulative_per_rank_gradient_steps += 1
+                    train_step += world_size
+                if aggregator:
+                    aggregator.update("Params/exploration_amount", actor._get_expl_amount(policy_step))
 
         # Log metrics
         if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -756,15 +717,15 @@
             state = {
                 "world_model": world_model.state_dict(),
                 "actor": actor.state_dict(),
                 "critic": critic.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "critic_optimizer": critic_optimizer.state_dict(),
-                "expl_decay_steps": expl_decay_steps,
+                "ratio": ratio.state_dict(),
                 "update": update * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v1/evaluate.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v1/evaluate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Any, Dict
 
 import gymnasium as gym
 from lightning import Fabric
 
-from sheeprl.algos.dreamer_v1.agent import PlayerDV1, build_agent
+from sheeprl.algos.dreamer_v1.agent import build_agent
 from sheeprl.algos.dreamer_v2.utils import test
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.registry import register_evaluation
 
 
 @register_evaluation(algorithms="dreamer_v1")
@@ -40,29 +40,18 @@
 
     is_continuous = isinstance(action_space, gym.spaces.Box)
     is_multidiscrete = isinstance(action_space, gym.spaces.MultiDiscrete)
     actions_dim = tuple(
         action_space.shape if is_continuous else (action_space.nvec.tolist() if is_multidiscrete else [action_space.n])
     )
     # Create the actor and critic models
-    world_model, actor, _ = build_agent(
+    _, _, _, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["world_model"],
         state["actor"],
     )
-    player = PlayerDV1(
-        world_model.encoder.module,
-        world_model.rssm.recurrent_model.module,
-        world_model.rssm.representation_model.module,
-        actor.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-    )
-
-    test(player, fabric, cfg, log_dir, sample_actions=False)
+    del _
+    test(player, fabric, cfg, log_dir, greedy=True)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v1/loss.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v1/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v1/utils.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v1/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     "Loss/observation_loss",
     "Loss/reward_loss",
     "Loss/state_loss",
     "Loss/continue_loss",
     "State/post_entropy",
     "State/prior_entropy",
     "State/kl",
-    "Params/exploration_amount",
     "Grads/world_model",
     "Grads/actor",
     "Grads/critic",
+    "Params/exploration_amount",
 }
 MODELS_TO_REGISTER = {"world_model", "actor", "critic"}
 
 
 def compute_lambda_values(
     rewards: Tensor,
     values: Tensor,
@@ -74,15 +74,15 @@
         delta = rewards[step] + next_values * done_mask[step]
         last_lambda_values = delta + lmbda * done_mask[step] * last_lambda_values
         lambda_targets.append(last_lambda_values)
     return torch.stack(list(reversed(lambda_targets)), dim=0)
 
 
 def compute_stochastic_state(
-    state_information: Tensor, event_shape: int = 1, min_std: float = 0.1, validate_args: bool = False
+    state_information: Tensor, event_shape: int = 1, min_std: float = 0.1
 ) -> Tuple[Tuple[Tensor, Tensor], Tensor]:
     """
     Compute the stochastic state from the information of the distribution of the stochastic state.
 
     Args:
         state_information (Tensor): information about the distribution of the stochastic state,
             it is the output of either the representation model or the transition model.
@@ -93,20 +93,20 @@
 
     Returns:
         The mean and the standard deviation of the distribution of the stochastic state.
         The sampled stochastic state.
     """
     mean, std = torch.chunk(state_information, 2, -1)
     std = F.softplus(std) + min_std
-    state_distribution: Distribution = Normal(mean, std, validate_args=validate_args)
+    state_distribution: Distribution = Normal(mean, std)
     if event_shape:
         # it is necessary an Independent distribution because
         # it is necessary to create (batch_size * sequence_length) independent distributions,
         # each producing a sample of size equal to the stochastic size
-        state_distribution = Independent(state_distribution, event_shape, validate_args=validate_args)
+        state_distribution = Independent(state_distribution, event_shape)
     stochastic_state = state_distribution.rsample()
     return (mean, std), stochastic_state
 
 
 def log_models(
     cfg: Dict[str, Any],
     models_to_log: Dict[str, torch.nn.Module | _FabricModule],
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v2/agent.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v2/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,29 @@
 import hydra
 import numpy as np
 import torch
 import torch.nn.functional as F
 from lightning.fabric import Fabric
 from lightning.fabric.wrappers import _FabricModule
 from torch import Tensor, nn
-from torch.distributions import Distribution, Independent, Normal, TanhTransform, TransformedDistribution
+from torch.distributions import (
+    Distribution,
+    Independent,
+    Normal,
+    OneHotCategorical,
+    OneHotCategoricalStraightThrough,
+    TanhTransform,
+    TransformedDistribution,
+)
 
 from sheeprl.algos.dreamer_v2.utils import compute_stochastic_state, init_weights
-from sheeprl.models.models import CNN, MLP, DeCNN, LayerNormGRUCell, MultiDecoder, MultiEncoder
-from sheeprl.utils.distribution import (
-    OneHotCategoricalStraightThroughValidateArgs,
-    OneHotCategoricalValidateArgs,
-    TruncatedNormal,
-)
-from sheeprl.utils.model import LayerNormChannelLast, ModuleType, cnn_forward
+from sheeprl.models.models import CNN, MLP, DeCNN, LayerNormChannelLast, LayerNormGRUCell, MultiDecoder, MultiEncoder
+from sheeprl.utils.distribution import TruncatedNormal
+from sheeprl.utils.fabric import get_single_device_fabric
+from sheeprl.utils.model import ModuleType, cnn_forward
 
 
 class CNNEncoder(nn.Module):
     """The Dreamer-V2 image encoder. This is composed of 4 `nn.Conv2d` with
     kernel_size=3, stride=2 and padding=1. No bias is used if a `nn.LayerNorm`
     is used after the convolution. This 4-stages model assumes that the image
     is a 64x64. If more than one image is to be encoded, then those will
@@ -57,17 +62,17 @@
         self.model = nn.Sequential(
             CNN(
                 input_channels=sum(input_channels),
                 hidden_channels=(torch.tensor([1, 2, 4, 8]) * channels_multiplier).tolist(),
                 layer_args={"kernel_size": 4, "stride": 2},
                 activation=activation,
                 norm_layer=[LayerNormChannelLast for _ in range(4)] if layer_norm else None,
-                norm_args=[{"normalized_shape": (2**i) * channels_multiplier} for i in range(4)]
-                if layer_norm
-                else None,
+                norm_args=(
+                    [{"normalized_shape": (2**i) * channels_multiplier} for i in range(4)] if layer_norm else None
+                ),
             ),
             nn.Flatten(-3, -1),
         )
         with torch.no_grad():
             self.output_dim = self.model(torch.zeros(1, *self.input_dim)).shape[-1]
 
     def forward(self, obs: Dict[str, Tensor]) -> Tensor:
@@ -113,15 +118,15 @@
             activation=activation,
             norm_layer=[nn.LayerNorm for _ in range(mlp_layers)] if layer_norm else None,
             norm_args=[{"normalized_shape": dense_units} for _ in range(mlp_layers)] if layer_norm else None,
         )
         self.output_dim = dense_units
 
     def forward(self, obs: Dict[str, Tensor]) -> Tensor:
-        x = torch.cat([obs[k] for k in self.keys], -1).type(torch.float32)
+        x = torch.cat([obs[k] for k in self.keys], -1)
         return self.model(x)
 
 
 class CNNDecoder(nn.Module):
     """The almost-exact inverse of the `CNNEncoder` class, where in 4 stages it reconstructs
     the observation image to 64x64. If multiple images are to be reconstructed,
     then it will create a dictionary with an entry for every reconstructed image.
@@ -168,20 +173,20 @@
                     {"kernel_size": 5, "stride": 2},
                     {"kernel_size": 5, "stride": 2},
                     {"kernel_size": 6, "stride": 2},
                     {"kernel_size": 6, "stride": 2},
                 ],
                 activation=[activation, activation, activation, None],
                 norm_layer=[LayerNormChannelLast for _ in range(3)] + [None] if layer_norm else None,
-                norm_args=[
-                    {"normalized_shape": (2 ** (4 - i - 2)) * channels_multiplier} for i in range(self.output_dim[0])
-                ]
-                + [None]
-                if layer_norm
-                else None,
+                norm_args=(
+                    [{"normalized_shape": (2 ** (4 - i - 2)) * channels_multiplier} for i in range(self.output_dim[0])]
+                    + [None]
+                    if layer_norm
+                    else None
+                ),
             ),
         )
 
     def forward(self, latent_states: Tensor) -> Dict[str, Tensor]:
         reconstructed_obs = {}
         x = cnn_forward(self.model, latent_states, (latent_states.shape[-1],), self.output_dim)
         reconstructed_obs.update(
@@ -269,15 +274,17 @@
             input_dims=input_size,
             output_dim=None,
             hidden_sizes=[dense_units],
             activation=activation,
             norm_layer=[nn.LayerNorm] if layer_norm else None,
             norm_args=[{"normalized_shape": dense_units}] if layer_norm else None,
         )
-        self.rnn = LayerNormGRUCell(dense_units, recurrent_state_size, bias=True, batch_first=False, layer_norm=True)
+        self.rnn = LayerNormGRUCell(
+            dense_units, recurrent_state_size, bias=True, batch_first=False, layer_norm_cls=nn.LayerNorm
+        )
 
     def forward(self, input: Tensor, recurrent_state: Tensor) -> Tensor:
         """
         Compute the next recurrent state from the latent state (stochastic and recurrent states) and the actions.
 
         Args:
             input (Tensor): the input tensor composed by the stochastic state and the actions concatenated together.
@@ -369,31 +376,27 @@
             embedded_obs (Tensor): the embedded real observations provided by the environment.
 
         Returns:
             logits (Tensor): the logits of the distribution of the posterior state.
             posterior (Tensor): the sampled posterior stochastic state.
         """
         logits = self.representation_model(torch.cat((recurrent_state, embedded_obs), -1))
-        return logits, compute_stochastic_state(
-            logits, discrete=self.discrete, validate_args=self.distribution_cfg.validate_args
-        )
+        return logits, compute_stochastic_state(logits, discrete=self.discrete)
 
     def _transition(self, recurrent_out: Tensor) -> Tuple[Tensor, Tensor]:
         """
         Args:
             recurrent_out (Tensor): the output of the recurrent model, i.e., the deterministic part of the latent space.
 
         Returns:
             logits (Tensor): the logits of the distribution of the prior state.
             prior (Tensor): the sampled prior stochastic state.
         """
         logits = self.transition_model(recurrent_out)
-        return logits, compute_stochastic_state(
-            logits, discrete=self.discrete, validate_args=self.distribution_cfg.validate_args
-        )
+        return logits, compute_stochastic_state(logits, discrete=self.discrete)
 
     def imagination(self, prior: Tensor, recurrent_state: Tensor, actions: Tensor) -> Tuple[Tensor, Tensor]:
         """
         One-step imagination of the next latent state.
         It can be used several times to imagine trajectories in the latent space (Transition Model).
 
         Args:
@@ -430,14 +433,18 @@
             Default to nn.ELU.
         mlp_layers (int): the number of linear layers.
             Default to 4.
         layer_norm (bool): whether or not to use the layer norm.
             Default to False.
         expl_amount (float): the exploration amount to use during training.
             Default to 0.0.
+        expl_decay (float): the exploration decay to use during training.
+            Default to 0.0.
+        expl_min (float): the exploration amount minimum to use during training.
+            Default to 0.0.
     """
 
     def __init__(
         self,
         latent_state_size: int,
         actions_dim: Sequence[int],
         is_continuous: bool,
@@ -445,14 +452,16 @@
         init_std: float = 0.0,
         min_std: float = 0.1,
         dense_units: int = 400,
         activation: nn.Module = nn.ELU,
         mlp_layers: int = 4,
         layer_norm: bool = False,
         expl_amount: float = 0.0,
+        expl_decay: float = 0.0,
+        expl_min: float = 0.0,
     ) -> None:
         super().__init__()
         self.distribution_cfg = distribution_cfg
         self.distribution = distribution_cfg.get("type", "auto").lower()
         if self.distribution not in ("auto", "normal", "tanh_normal", "discrete", "trunc_normal"):
             raise ValueError(
                 "The distribution must be on of: `auto`, `discrete`, `normal`, `tanh_normal` and `trunc_normal`. "
@@ -480,104 +489,91 @@
             self.mlp_heads = nn.ModuleList([nn.Linear(dense_units, action_dim) for action_dim in actions_dim])
         self.actions_dim = actions_dim
         self.is_continuous = is_continuous
         self.init_std = torch.tensor(init_std)
         self.min_std = min_std
         self.distribution_cfg = distribution_cfg
         self._expl_amount = expl_amount
+        self._expl_decay = expl_decay
+        self._expl_min = expl_min
 
-    @property
-    def expl_amount(self) -> float:
-        return self._expl_amount
-
-    @expl_amount.setter
-    def expl_amount(self, amount: float):
-        self._expl_amount = amount
+    def _get_expl_amount(self, step: int) -> Tensor:
+        amount = self._expl_amount
+        if self._expl_decay:
+            amount *= 0.5 ** float(step) / self._expl_decay
+        return max(amount, self._expl_min)
 
     def forward(
-        self, state: Tensor, is_training: bool = True, mask: Optional[Dict[str, Tensor]] = None
+        self, state: Tensor, greedy: bool = False, mask: Optional[Dict[str, Tensor]] = None
     ) -> Tuple[Sequence[Tensor], Sequence[Distribution]]:
         """
         Call the forward method of the actor model and reorganizes the result with shape (batch_size, *, num_actions),
         where * means any number of dimensions including None.
 
         Args:
             state (Tensor): the current state of shape (batch_size, *, stochastic_size + recurrent_state_size).
-            is_training (bool): whether it is in the training phase.
-                Default to True.
+            greedy (bool): whether or not to sample the actions.
+                Default to False.
             mask (Dict[str, Tensor], optional): the action mask (which actions can be selected).
                 Default to None.
 
         Returns:
             The tensor of the actions taken by the agent with shape (batch_size, *, num_actions).
             The distribution of the actions
         """
         out: Tensor = self.model(state)
         pre_dist: List[Tensor] = [head(out) for head in self.mlp_heads]
         if self.is_continuous:
             mean, std = torch.chunk(pre_dist[0], 2, -1)
             if self.distribution == "tanh_normal":
                 mean = 5 * torch.tanh(mean / 5)
                 std = F.softplus(std + self.init_std) + self.min_std
-                actions_dist = Normal(mean, std, validate_args=self.distribution_cfg.validate_args)
-                actions_dist = Independent(
-                    TransformedDistribution(
-                        actions_dist, TanhTransform(), validate_args=self.distribution_cfg.validate_args
-                    ),
-                    1,
-                    validate_args=self.distribution_cfg.validate_args,
-                )
+                actions_dist = Normal(mean, std)
+                actions_dist = Independent(TransformedDistribution(actions_dist, TanhTransform()), 1)
             elif self.distribution == "normal":
-                actions_dist = Normal(mean, std, validate_args=self.distribution_cfg.validate_args)
-                actions_dist = Independent(actions_dist, 1, validate_args=self.distribution_cfg.validate_args)
+                actions_dist = Normal(mean, std)
+                actions_dist = Independent(actions_dist, 1)
             elif self.distribution == "trunc_normal":
                 std = 2 * torch.sigmoid((std + self.init_std) / 2) + self.min_std
-                dist = TruncatedNormal(torch.tanh(mean), std, -1, 1, validate_args=self.distribution_cfg.validate_args)
-                actions_dist = Independent(dist, 1, validate_args=self.distribution_cfg.validate_args)
-            if is_training:
+                dist = TruncatedNormal(torch.tanh(mean), std, -1, 1)
+                actions_dist = Independent(dist, 1)
+            if not greedy:
                 actions = actions_dist.rsample()
             else:
                 sample = actions_dist.sample((100,))
                 log_prob = actions_dist.log_prob(sample)
                 actions = sample[log_prob.argmax(0)].view(1, 1, -1)
             actions = [actions]
             actions_dist = [actions_dist]
         else:
             actions_dist: List[Distribution] = []
             actions: List[Tensor] = []
             for logits in pre_dist:
-                actions_dist.append(
-                    OneHotCategoricalStraightThroughValidateArgs(
-                        logits=logits, validate_args=self.distribution_cfg.validate_args
-                    )
-                )
-                if is_training:
+                actions_dist.append(OneHotCategoricalStraightThrough(logits=logits))
+                if not greedy:
                     actions.append(actions_dist[-1].rsample())
                 else:
                     actions.append(actions_dist[-1].mode)
         return tuple(actions), tuple(actions_dist)
 
     def add_exploration_noise(
-        self, actions: Sequence[Tensor], mask: Optional[Dict[str, Tensor]] = None
+        self, actions: Sequence[Tensor], step: int = 0, mask: Optional[Dict[str, Tensor]] = None
     ) -> Sequence[Tensor]:
+        expl_amount = self._get_expl_amount(step)
         if self.is_continuous:
             actions = torch.cat(actions, -1)
-            if self._expl_amount > 0.0:
-                actions = torch.clip(Normal(actions, self._expl_amount).sample(), -1, 1)
+            if expl_amount > 0.0:
+                actions = torch.clip(Normal(actions, expl_amount).sample(), -1, 1)
             expl_actions = [actions]
         else:
             expl_actions = []
             for act in actions:
-                sample = (
-                    OneHotCategoricalValidateArgs(logits=torch.zeros_like(act), validate_args=False)
-                    .sample()
-                    .to(act.device)
-                )
+                sample = OneHotCategorical(logits=torch.zeros_like(act)).sample().to(act.device)
                 expl_actions.append(
-                    torch.where(torch.rand(act.shape[:1], device=act.device) < self._expl_amount, sample, act)
+                    torch.where(torch.rand(act.shape[:1], device=act.device) < expl_amount, sample, act)
                 )
         return tuple(expl_actions)
 
 
 class MinedojoActor(Actor):
     def __init__(
         self,
@@ -588,40 +584,44 @@
         init_std: float = 0,
         min_std: float = 0.1,
         dense_units: int = 400,
         activation: nn.Module = nn.ELU,
         mlp_layers: int = 4,
         layer_norm: bool = False,
         expl_amount: float = 0.0,
+        expl_decay: float = 0.0,
+        expl_min: float = 0.0,
     ) -> None:
         super().__init__(
             latent_state_size=latent_state_size,
             actions_dim=actions_dim,
             is_continuous=is_continuous,
             distribution_cfg=distribution_cfg,
             init_std=init_std,
             min_std=min_std,
             dense_units=dense_units,
             activation=activation,
             mlp_layers=mlp_layers,
             layer_norm=layer_norm,
             expl_amount=expl_amount,
+            expl_decay=expl_decay,
+            expl_min=expl_min,
         )
 
     def forward(
-        self, state: Tensor, is_training: bool = True, mask: Optional[Dict[str, Tensor]] = None
+        self, state: Tensor, greedy: bool = False, mask: Optional[Dict[str, Tensor]] = None
     ) -> Tuple[Sequence[Tensor], Sequence[Distribution]]:
         """
         Call the forward method of the actor model and reorganizes the result with shape (batch_size, *, num_actions),
         where * means any number of dimensions including None.
 
         Args:
             state (Tensor): the current state of shape (batch_size, *, stochastic_size + recurrent_state_size).
-            is_training (bool): whether it is in the training phase.
-                Default to True.
+            greedy (bool): whether or not to sample the actions.
+                Default to False.
             mask (Dict[str, Tensor], optional): the action mask (which actions can be selected).
                 Default to None.
 
         Returns:
             The tensor of the actions taken by the agent with shape (batch_size, *, num_actions).
             The distribution of the actions
         """
@@ -647,29 +647,25 @@
                     for t in range(functional_action.shape[0]):
                         for b in range(functional_action.shape[1]):
                             sampled_action = functional_action[t, b].item()
                             if sampled_action in (16, 17):  # Equip/Place action
                                 logits[t, b][torch.logical_not(mask["mask_equip_place"][t, b])] = -torch.inf
                             elif sampled_action == 18:  # Destroy action
                                 logits[t, b][torch.logical_not(mask["mask_destroy"][t, b])] = -torch.inf
-            actions_dist.append(
-                OneHotCategoricalStraightThroughValidateArgs(
-                    logits=logits, validate_args=self.distribution_cfg.validate_args
-                )
-            )
-            if is_training:
+            actions_dist.append(OneHotCategoricalStraightThrough(logits=logits))
+            if not greedy:
                 actions.append(actions_dist[-1].rsample())
             else:
                 actions.append(actions_dist[-1].mode)
             if functional_action is None:
                 functional_action = actions[0].argmax(dim=-1)  # [T, B]
         return tuple(actions), tuple(actions_dist)
 
     def add_exploration_noise(
-        self, actions: Sequence[Tensor], mask: Optional[Dict[str, Tensor]] = None
+        self, actions: Sequence[Tensor], step: int = 0, mask: Optional[Dict[str, Tensor]] = None
     ) -> Sequence[Tensor]:
         expl_actions = []
         functional_action = actions[0].argmax(dim=-1)
         for i, act in enumerate(actions):
             logits = torch.zeros_like(act)
             # Exploratory action must respect the constraints of the environment
             if mask is not None:
@@ -688,18 +684,16 @@
                     for t in range(functional_action.shape[0]):
                         for b in range(functional_action.shape[1]):
                             sampled_action = functional_action[t, b].item()
                             if sampled_action in {16, 17}:  # Equip/Place action
                                 logits[t, b][torch.logical_not(mask["mask_equip_place"][t, b])] = -torch.inf
                             elif sampled_action == 18:  # Destroy action
                                 logits[t, b][torch.logical_not(mask["mask_destroy"][t, b])] = -torch.inf
-            sample = (
-                OneHotCategoricalValidateArgs(logits=torch.zeros_like(act), validate_args=False).sample().to(act.device)
-            )
-            expl_amount = self.expl_amount
+            sample = OneHotCategorical(logits=torch.zeros_like(act)).sample().to(act.device)
+            expl_amount = self._get_expl_amount(step)
             # If the action[0] was changed, and now it is critical, then we force to change also the other 2 actions
             # to satisfy the constraints of the environment
             if (
                 i in {1, 2}
                 and actions[0].argmax() != expl_actions[0].argmax()
                 and expl_actions[0].argmax().item() in {15, 16, 17, 18}
             ):
@@ -739,56 +733,55 @@
 
 
 class PlayerDV2(nn.Module):
     """
     The model of the Dreamer_v2 player.
 
     Args:
-        encoder (nn.Module): the encoder.
-        recurrent_model (nn.Module): the recurrent model.
-        representation_model (nn.Module): the representation model.
-        actor (nn.Module): the actor.
+        encoder (nn.Module | _FabricModule): the encoder.
+        recurrent_model (nn.Module | _FabricModule): the recurrent model.
+        representation_model (nn.Module | _FabricModule): the representation model.
+        actor (nn.Module | _FabricModule): the actor.
         actions_dim (Sequence[int]): the dimension of the actions.
         num_envs (int): the number of environments.
         stochastic_size (int): the size of the stochastic state.
         recurrent_state_size (int): the size of the recurrent state.
-        device (torch.device): the device to work on.
+        device (str | torch.device): the device where the model is stored.
         discrete_size (int): the dimension of a single Categorical variable in the
             stochastic state (prior or posterior).
             Defaults to 32.
         actor_type (str, optional): which actor the player is using ('task' or 'exploration').
             Default to None.
     """
 
     def __init__(
         self,
-        encoder: nn.Module,
-        recurrent_model: nn.Module,
-        representation_model: nn.Module,
-        actor: nn.Module,
+        encoder: nn.Module | _FabricModule,
+        recurrent_model: nn.Module | _FabricModule,
+        representation_model: nn.Module | _FabricModule,
+        actor: nn.Module | _FabricModule,
         actions_dim: Sequence[int],
         num_envs: int,
         stochastic_size: int,
         recurrent_state_size: int,
-        device: torch.device,
+        device: str | torch.device,
         discrete_size: int = 32,
         actor_type: str | None = None,
     ) -> None:
         super().__init__()
         self.encoder = encoder
         self.recurrent_model = recurrent_model
         self.representation_model = representation_model
         self.actor = actor
-        self.device = device
         self.actions_dim = actions_dim
+        self.num_envs = num_envs
         self.stochastic_size = stochastic_size
-        self.discrete_size = discrete_size
         self.recurrent_state_size = recurrent_state_size
-        self.num_envs = num_envs
-        self.validate_args = self.actor.distribution_cfg.validate_args
+        self.device = device
+        self.discrete_size = discrete_size
         self.actor_type = actor_type
 
     def init_states(self, reset_envs: Optional[Sequence[int]] = None) -> None:
         """Initialize the states and the actions for the ended environments.
 
         Args:
             reset_envs (Optional[Sequence[int]], optional): which environments' states to reset.
@@ -802,80 +795,58 @@
                 1, self.num_envs, self.stochastic_size * self.discrete_size, device=self.device
             )
         else:
             self.actions[:, reset_envs] = torch.zeros_like(self.actions[:, reset_envs])
             self.recurrent_state[:, reset_envs] = torch.zeros_like(self.recurrent_state[:, reset_envs])
             self.stochastic_state[:, reset_envs] = torch.zeros_like(self.stochastic_state[:, reset_envs])
 
-    def get_exploration_action(self, obs: Dict[str, Tensor], mask: Optional[Dict[str, Tensor]] = None) -> Tensor:
-        """
-        Return the actions with a certain amount of noise for exploration.
-
-        Args:
-            obs (Dict[str, Tensor]): the current observations.
-            is_continuous (bool): whether or not the actions are continuous.
-            mask (Dict[str, Tensor], optional): the action mask (which actions can be selected).
-                Default to None.
-
-        Returns:
-            The actions the agent has to perform.
-        """
-        actions = self.get_greedy_action(obs, mask=mask)
-        expl_actions = None
-        if self.actor.expl_amount > 0:
-            expl_actions = self.actor.add_exploration_noise(actions, mask=mask)
-            self.actions = torch.cat(expl_actions, dim=-1)
-        return expl_actions or actions
-
-    def get_greedy_action(
+    def get_actions(
         self,
         obs: Dict[str, Tensor],
-        is_training: bool = True,
+        greedy: bool = False,
         mask: Optional[Dict[str, Tensor]] = None,
     ) -> Sequence[Tensor]:
         """
         Return the greedy actions.
 
         Args:
             obs (Dict[str, Tensor]): the current observations.
-            is_training (bool): whether it is training.
-                Default to True.
+            greedy (bool): whether or not to sample the actions.
+                Default to False.
             mask (Dict[str, Tensor], optional): the action mask (which actions can be selected).
                 Default to None.
 
         Returns:
             The actions the agent has to perform.
         """
         embedded_obs = self.encoder(obs)
         self.recurrent_state = self.recurrent_model(
             torch.cat((self.stochastic_state, self.actions), -1), self.recurrent_state
         )
         posterior_logits = self.representation_model(torch.cat((self.recurrent_state, embedded_obs), -1))
-        stochastic_state = compute_stochastic_state(
-            posterior_logits, discrete=self.discrete_size, validate_args=self.validate_args
-        )
+        stochastic_state = compute_stochastic_state(posterior_logits, discrete=self.discrete_size)
         self.stochastic_state = stochastic_state.view(
             *stochastic_state.shape[:-2], self.stochastic_size * self.discrete_size
         )
-        actions, _ = self.actor(torch.cat((self.stochastic_state, self.recurrent_state), -1), is_training, mask)
+        actions, _ = self.actor(torch.cat((self.stochastic_state, self.recurrent_state), -1), greedy, mask)
         self.actions = torch.cat(actions, -1)
         return actions
 
 
 def build_agent(
     fabric: Fabric,
     actions_dim: Sequence[int],
     is_continuous: bool,
     cfg: Dict[str, Any],
     obs_space: gymnasium.spaces.Dict,
     world_model_state: Optional[Dict[str, Tensor]] = None,
     actor_state: Optional[Dict[str, Tensor]] = None,
     critic_state: Optional[Dict[str, Tensor]] = None,
     target_critic_state: Optional[Dict[str, Tensor]] = None,
-) -> Tuple[WorldModel, _FabricModule, _FabricModule, nn.Module]:
+) -> Tuple[WorldModel, _FabricModule, _FabricModule, _FabricModule, PlayerDV2]:
     """Build the models and wrap them with Fabric.
 
     Args:
         fabric (Fabric): the fabric object.
         actions_dim (Sequence[int]): the dimension of the actions.
         is_continuous (bool): whether or not the actions are continuous.
         cfg (DictConfig): the configs.
@@ -890,15 +861,15 @@
             Default to None.
 
     Returns:
         The world model (WorldModel): composed by the encoder, rssm, observation and
         reward models and the continue model.
         The actor (_FabricModule).
         The critic (_FabricModule).
-        The target critic (nn.Module).
+        The target critic (_FabricModule).
     """
     world_model_cfg = cfg.algo.world_model
     actor_cfg = cfg.algo.actor
     critic_cfg = cfg.algo.critic
 
     # Sizes
     stochastic_size = world_model_cfg.stochastic_size * world_model_cfg.discrete_size
@@ -908,26 +879,26 @@
     cnn_encoder = (
         CNNEncoder(
             keys=cfg.algo.cnn_keys.encoder,
             input_channels=[int(np.prod(obs_space[k].shape[:-2])) for k in cfg.algo.cnn_keys.encoder],
             image_size=obs_space[cfg.algo.cnn_keys.encoder[0]].shape[-2:],
             channels_multiplier=world_model_cfg.encoder.cnn_channels_multiplier,
             layer_norm=world_model_cfg.encoder.layer_norm,
-            activation=eval(world_model_cfg.encoder.cnn_act),
+            activation=hydra.utils.get_class(world_model_cfg.encoder.cnn_act),
         )
         if cfg.algo.cnn_keys.encoder is not None and len(cfg.algo.cnn_keys.encoder) > 0
         else None
     )
     mlp_encoder = (
         MLPEncoder(
             keys=cfg.algo.mlp_keys.encoder,
             input_dims=[obs_space[k].shape[0] for k in cfg.algo.mlp_keys.encoder],
             mlp_layers=world_model_cfg.encoder.mlp_layers,
             dense_units=world_model_cfg.encoder.dense_units,
-            activation=eval(world_model_cfg.encoder.dense_act),
+            activation=hydra.utils.get_class(world_model_cfg.encoder.dense_act),
             layer_norm=world_model_cfg.encoder.layer_norm,
         )
         if cfg.algo.mlp_keys.encoder is not None and len(cfg.algo.mlp_keys.encoder) > 0
         else None
     )
     encoder = MultiEncoder(cnn_encoder, mlp_encoder)
     recurrent_model = RecurrentModel(
@@ -936,31 +907,35 @@
     )
     representation_model = MLP(
         input_dims=(
             world_model_cfg.recurrent_model.recurrent_state_size + encoder.cnn_output_dim + encoder.mlp_output_dim
         ),
         output_dim=stochastic_size,
         hidden_sizes=[world_model_cfg.representation_model.hidden_size],
-        activation=eval(world_model_cfg.representation_model.dense_act),
+        activation=hydra.utils.get_class(world_model_cfg.representation_model.dense_act),
         flatten_dim=None,
         norm_layer=[nn.LayerNorm] if world_model_cfg.representation_model.layer_norm else None,
-        norm_args=[{"normalized_shape": world_model_cfg.representation_model.hidden_size}]
-        if world_model_cfg.representation_model.layer_norm
-        else None,
+        norm_args=(
+            [{"normalized_shape": world_model_cfg.representation_model.hidden_size}]
+            if world_model_cfg.representation_model.layer_norm
+            else None
+        ),
     )
     transition_model = MLP(
         input_dims=world_model_cfg.recurrent_model.recurrent_state_size,
         output_dim=stochastic_size,
         hidden_sizes=[world_model_cfg.transition_model.hidden_size],
-        activation=eval(world_model_cfg.transition_model.dense_act),
+        activation=hydra.utils.get_class(world_model_cfg.transition_model.dense_act),
         flatten_dim=None,
         norm_layer=[nn.LayerNorm] if world_model_cfg.transition_model.layer_norm else None,
-        norm_args=[{"normalized_shape": world_model_cfg.transition_model.hidden_size}]
-        if world_model_cfg.transition_model.layer_norm
-        else None,
+        norm_args=(
+            [{"normalized_shape": world_model_cfg.transition_model.hidden_size}]
+            if world_model_cfg.transition_model.layer_norm
+            else None
+        ),
     )
     rssm = RSSM(
         recurrent_model=recurrent_model.apply(init_weights),
         representation_model=representation_model.apply(init_weights),
         transition_model=transition_model.apply(init_weights),
         distribution_cfg=cfg.distribution,
         discrete=world_model_cfg.discrete_size,
@@ -969,66 +944,74 @@
         CNNDecoder(
             keys=cfg.algo.cnn_keys.decoder,
             output_channels=[int(np.prod(obs_space[k].shape[:-2])) for k in cfg.algo.cnn_keys.decoder],
             channels_multiplier=world_model_cfg.observation_model.cnn_channels_multiplier,
             latent_state_size=latent_state_size,
             cnn_encoder_output_dim=cnn_encoder.output_dim,
             image_size=obs_space[cfg.algo.cnn_keys.decoder[0]].shape[-2:],
-            activation=eval(world_model_cfg.observation_model.cnn_act),
+            activation=hydra.utils.get_class(world_model_cfg.observation_model.cnn_act),
             layer_norm=world_model_cfg.observation_model.layer_norm,
         )
         if cfg.algo.cnn_keys.decoder is not None and len(cfg.algo.cnn_keys.decoder) > 0
         else None
     )
     mlp_decoder = (
         MLPDecoder(
             keys=cfg.algo.mlp_keys.decoder,
             output_dims=[obs_space[k].shape[0] for k in cfg.algo.mlp_keys.decoder],
             latent_state_size=latent_state_size,
             mlp_layers=world_model_cfg.observation_model.mlp_layers,
             dense_units=world_model_cfg.observation_model.dense_units,
-            activation=eval(world_model_cfg.observation_model.dense_act),
+            activation=hydra.utils.get_class(world_model_cfg.observation_model.dense_act),
             layer_norm=world_model_cfg.observation_model.layer_norm,
         )
         if cfg.algo.mlp_keys.decoder is not None and len(cfg.algo.mlp_keys.decoder) > 0
         else None
     )
     observation_model = MultiDecoder(cnn_decoder, mlp_decoder)
     reward_model = MLP(
         input_dims=latent_state_size,
         output_dim=1,
         hidden_sizes=[world_model_cfg.reward_model.dense_units] * world_model_cfg.reward_model.mlp_layers,
-        activation=eval(world_model_cfg.reward_model.dense_act),
+        activation=hydra.utils.get_class(world_model_cfg.reward_model.dense_act),
         flatten_dim=None,
-        norm_layer=[nn.LayerNorm for _ in range(world_model_cfg.reward_model.mlp_layers)]
-        if world_model_cfg.reward_model.layer_norm
-        else None,
-        norm_args=[
-            {"normalized_shape": world_model_cfg.reward_model.dense_units}
-            for _ in range(world_model_cfg.reward_model.mlp_layers)
-        ]
-        if world_model_cfg.reward_model.layer_norm
-        else None,
+        norm_layer=(
+            [nn.LayerNorm for _ in range(world_model_cfg.reward_model.mlp_layers)]
+            if world_model_cfg.reward_model.layer_norm
+            else None
+        ),
+        norm_args=(
+            [
+                {"normalized_shape": world_model_cfg.reward_model.dense_units}
+                for _ in range(world_model_cfg.reward_model.mlp_layers)
+            ]
+            if world_model_cfg.reward_model.layer_norm
+            else None
+        ),
     )
     if world_model_cfg.use_continues:
         continue_model = MLP(
             input_dims=latent_state_size,
             output_dim=1,
             hidden_sizes=[world_model_cfg.discount_model.dense_units] * world_model_cfg.discount_model.mlp_layers,
-            activation=eval(world_model_cfg.discount_model.dense_act),
+            activation=hydra.utils.get_class(world_model_cfg.discount_model.dense_act),
             flatten_dim=None,
-            norm_layer=[nn.LayerNorm for _ in range(world_model_cfg.discount_model.mlp_layers)]
-            if world_model_cfg.discount_model.layer_norm
-            else None,
-            norm_args=[
-                {"normalized_shape": world_model_cfg.discount_model.dense_units}
-                for _ in range(world_model_cfg.discount_model.mlp_layers)
-            ]
-            if world_model_cfg.discount_model.layer_norm
-            else None,
+            norm_layer=(
+                [nn.LayerNorm for _ in range(world_model_cfg.discount_model.mlp_layers)]
+                if world_model_cfg.discount_model.layer_norm
+                else None
+            ),
+            norm_args=(
+                [
+                    {"normalized_shape": world_model_cfg.discount_model.dense_units}
+                    for _ in range(world_model_cfg.discount_model.mlp_layers)
+                ]
+                if world_model_cfg.discount_model.layer_norm
+                else None
+            ),
         )
     world_model = WorldModel(
         encoder.apply(init_weights),
         rssm,
         observation_model.apply(init_weights),
         reward_model.apply(init_weights),
         continue_model.apply(init_weights) if world_model_cfg.use_continues else None,
@@ -1038,49 +1021,84 @@
         latent_state_size=latent_state_size,
         actions_dim=actions_dim,
         is_continuous=is_continuous,
         init_std=actor_cfg.init_std,
         min_std=actor_cfg.min_std,
         mlp_layers=actor_cfg.mlp_layers,
         dense_units=actor_cfg.dense_units,
-        activation=eval(actor_cfg.dense_act),
+        activation=hydra.utils.get_class(actor_cfg.dense_act),
         distribution_cfg=cfg.distribution,
         layer_norm=actor_cfg.layer_norm,
     )
     critic = MLP(
         input_dims=latent_state_size,
         output_dim=1,
         hidden_sizes=[critic_cfg.dense_units] * critic_cfg.mlp_layers,
-        activation=eval(critic_cfg.dense_act),
+        activation=hydra.utils.get_class(critic_cfg.dense_act),
         flatten_dim=None,
         norm_layer=[nn.LayerNorm for _ in range(critic_cfg.mlp_layers)] if critic_cfg.layer_norm else None,
-        norm_args=[{"normalized_shape": critic_cfg.dense_units} for _ in range(critic_cfg.mlp_layers)]
-        if critic_cfg.layer_norm
-        else None,
+        norm_args=(
+            [{"normalized_shape": critic_cfg.dense_units} for _ in range(critic_cfg.mlp_layers)]
+            if critic_cfg.layer_norm
+            else None
+        ),
     )
     actor.apply(init_weights)
     critic.apply(init_weights)
 
     # Load models from checkpoint
     if world_model_state:
         world_model.load_state_dict(world_model_state)
     if actor_state:
         actor.load_state_dict(actor_state)
     if critic_state:
         critic.load_state_dict(critic_state)
 
+    # Create the player agent
+    fabric_player = get_single_device_fabric(fabric)
+    player = PlayerDV2(
+        copy.deepcopy(world_model.encoder),
+        copy.deepcopy(world_model.rssm.recurrent_model),
+        copy.deepcopy(world_model.rssm.representation_model),
+        copy.deepcopy(actor),
+        actions_dim,
+        cfg.env.num_envs,
+        cfg.algo.world_model.stochastic_size,
+        cfg.algo.world_model.recurrent_model.recurrent_state_size,
+        fabric_player.device,
+        discrete_size=cfg.algo.world_model.discrete_size,
+    )
+
     # Setup models with Fabric
     world_model.encoder = fabric.setup_module(world_model.encoder)
     world_model.observation_model = fabric.setup_module(world_model.observation_model)
     world_model.reward_model = fabric.setup_module(world_model.reward_model)
     world_model.rssm.recurrent_model = fabric.setup_module(world_model.rssm.recurrent_model)
     world_model.rssm.representation_model = fabric.setup_module(world_model.rssm.representation_model)
     world_model.rssm.transition_model = fabric.setup_module(world_model.rssm.transition_model)
     if world_model.continue_model:
         world_model.continue_model = fabric.setup_module(world_model.continue_model)
     actor = fabric.setup_module(actor)
     critic = fabric.setup_module(critic)
+
+    # Setup target critic with a SingleDeviceStrategy
     target_critic = copy.deepcopy(critic.module)
     if target_critic_state:
         target_critic.load_state_dict(target_critic_state)
+    target_critic = fabric_player.setup_module(target_critic)
 
-    return world_model, actor, critic, target_critic
+    # Setup the player agent with a single-device Fabric
+    player.encoder = fabric_player.setup_module(player.encoder)
+    player.recurrent_model = fabric_player.setup_module(player.recurrent_model)
+    player.representation_model = fabric_player.setup_module(player.representation_model)
+    player.actor = fabric_player.setup_module(player.actor)
+
+    # Tie weights between the agent and the player
+    for agent_p, p in zip(world_model.encoder.parameters(), player.encoder.parameters()):
+        p.data = agent_p.data
+    for agent_p, p in zip(world_model.rssm.recurrent_model.parameters(), player.recurrent_model.parameters()):
+        p.data = agent_p.data
+    for agent_p, p in zip(world_model.rssm.representation_model.parameters(), player.representation_model.parameters()):
+        p.data = agent_p.data
+    for agent_p, p in zip(actor.parameters(), player.actor.parameters()):
+        p.data = agent_p.data
+    return world_model, actor, critic, target_critic, player
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v2/dreamer_v2.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v2/dreamer_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Dreamer-V2 implementation from [https://arxiv.org/abs/2010.02193](https://arxiv.org/abs/2010.02193).
 Adapted from the original implementation from https://github.com/danijar/dreamerv2
 """
+
 from __future__ import annotations
 
 import copy
 import os
 import warnings
 from typing import Any, Dict, Sequence
 
@@ -12,30 +13,29 @@
 import hydra
 import numpy as np
 import torch
 import torch.nn.functional as F
 from lightning.fabric import Fabric
 from lightning.fabric.wrappers import _FabricModule
 from torch import Tensor
-from torch.distributions import Bernoulli, Distribution, Independent, Normal
+from torch.distributions import Bernoulli, Distribution, Independent, Normal, OneHotCategorical
 from torch.distributions.utils import logits_to_probs
 from torch.optim import Optimizer
 from torchmetrics import SumMetric
 
-from sheeprl.algos.dreamer_v2.agent import PlayerDV2, WorldModel, build_agent
+from sheeprl.algos.dreamer_v2.agent import WorldModel, build_agent
 from sheeprl.algos.dreamer_v2.loss import reconstruction_loss
-from sheeprl.algos.dreamer_v2.utils import compute_lambda_values, test
+from sheeprl.algos.dreamer_v2.utils import compute_lambda_values, prepare_obs, test
 from sheeprl.data.buffers import EnvIndependentReplayBuffer, EpisodeBuffer, SequentialReplayBuffer
-from sheeprl.utils.distribution import OneHotCategoricalValidateArgs
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import polynomial_decay, save_configs
+from sheeprl.utils.utils import Ratio, save_configs
 
 # Decomment the following two lines if you cannot start an experiment with DMC environments
 # os.environ["PYOPENGL_PLATFORM"] = ""
 # os.environ["MUJOCO_GL"] = "osmesa"
 
 
 def train(
@@ -109,15 +109,14 @@
     # Observations:  o0       o1       o2      o3
     # Rewards:       0        r1       r2      r3
     # Dones:         0        d1       d2      d3
     # Is-first       1        i1       i2      i3
 
     batch_size = cfg.algo.per_rank_batch_size
     sequence_length = cfg.algo.per_rank_sequence_length
-    validate_args = cfg.distribution.validate_args
     recurrent_state_size = cfg.algo.world_model.recurrent_model.recurrent_state_size
     stochastic_size = cfg.algo.world_model.stochastic_size
     discrete_size = cfg.algo.world_model.discrete_size
     device = fabric.device
     batch_obs = {k: data[k] / 255 - 0.5 for k in cfg.algo.cnn_keys.encoder}
     batch_obs.update({k: data[k] for k in cfg.algo.mlp_keys.encoder})
 
@@ -157,40 +156,25 @@
     # Latent_states has dimension (sequence_length, batch_size, recurrent_state_size + stochastic_size * discrete_size)
     latent_states = torch.cat((posteriors.view(*posteriors.shape[:-2], -1), recurrent_states), -1)
 
     # Compute predictions for the observations
     decoded_information: Dict[str, torch.Tensor] = world_model.observation_model(latent_states)
 
     # Compute the distribution over the reconstructed observations
-    po = {
-        k: Independent(
-            Normal(rec_obs, 1, validate_args=validate_args),
-            len(rec_obs.shape[2:]),
-            validate_args=validate_args,
-        )
-        for k, rec_obs in decoded_information.items()
-    }
+    po = {k: Independent(Normal(rec_obs, 1), len(rec_obs.shape[2:])) for k, rec_obs in decoded_information.items()}
 
     # Compute the distribution over the rewards
-    pr = Independent(
-        Normal(world_model.reward_model(latent_states), 1, validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
+    pr = Independent(Normal(world_model.reward_model(latent_states), 1), 1)
 
     # Compute the distribution over the terminal steps, if required
     if cfg.algo.world_model.use_continues and world_model.continue_model:
-        pc = Independent(
-            Bernoulli(logits=world_model.continue_model(latent_states), validate_args=validate_args),
-            1,
-            validate_args=validate_args,
-        )
-        continue_targets = (1 - data["dones"]) * cfg.algo.gamma
+        pc = Independent(Bernoulli(logits=world_model.continue_model(latent_states)), 1)
+        continues_targets = (1 - data["terminated"]) * cfg.algo.gamma
     else:
-        pc = continue_targets = None
+        pc = continues_targets = None
 
     # Reshape posterior and prior logits to shape [T, B, 32, 32]
     priors_logits = priors_logits.view(*priors_logits.shape[:-1], stochastic_size, discrete_size)
     posteriors_logits = posteriors_logits.view(*posteriors_logits.shape[:-1], stochastic_size, discrete_size)
 
     # World model optimization step
     world_optimizer.zero_grad(set_to_none=True)
@@ -202,17 +186,16 @@
         priors_logits,
         posteriors_logits,
         cfg.algo.world_model.kl_balancing_alpha,
         cfg.algo.world_model.kl_free_nats,
         cfg.algo.world_model.kl_free_avg,
         cfg.algo.world_model.kl_regularizer,
         pc,
-        continue_targets,
+        continues_targets,
         cfg.algo.world_model.discount_scale_factor,
-        validate_args=validate_args,
     )
     fabric.backward(rec_loss)
     world_model_grads = None
     if cfg.algo.world_model.clip_gradients is not None and cfg.algo.world_model.clip_gradients > 0:
         world_model_grads = fabric.clip_gradients(
             module=world_model,
             optimizer=world_optimizer,
@@ -277,16 +260,16 @@
         imagined_trajectories[i] = imagined_latent_state
 
     # Predict values and rewards
     predicted_target_values = target_critic(imagined_trajectories)
     predicted_rewards = world_model.reward_model(imagined_trajectories)
     if cfg.algo.world_model.use_continues and world_model.continue_model:
         continues = logits_to_probs(world_model.continue_model(imagined_trajectories), is_binary=True)
-        true_done = (1 - data["dones"]).reshape(1, -1, 1) * cfg.algo.gamma
-        continues = torch.cat((true_done, continues[1:]))
+        true_continue = (1 - data["terminated"]).reshape(1, -1, 1) * cfg.algo.gamma
+        continues = torch.cat((true_continue, continues[1:]))
     else:
         continues = torch.ones_like(predicted_rewards.detach()) * cfg.algo.gamma
 
     # Compute the lambda_values, by passing as last value the value of the last imagined state
     # (horizon, batch_size * sequence_length, 1)
     lambda_values = compute_lambda_values(
         predicted_rewards[:-1],
@@ -348,19 +331,15 @@
             module=actor, optimizer=actor_optimizer, max_norm=cfg.algo.actor.clip_gradients, error_if_nonfinite=False
         )
     actor_optimizer.step()
 
     # Predict the values distribution only for the first H (horizon)
     # imagined states (to match the dimension with the lambda values),
     # It removes the last imagined state in the trajectory because it is used for bootstrapping
-    qv = Independent(
-        Normal(critic(imagined_trajectories.detach()[:-1]), 1, validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
+    qv = Independent(Normal(critic(imagined_trajectories.detach()[:-1]), 1), 1)
 
     # Critic optimization step. Eq. 5 from the paper.
     critic_optimizer.zero_grad(set_to_none=True)
     value_loss = -torch.mean(discount[:-1, ..., 0] * qv.log_prob(lambda_values.detach()))
     fabric.backward(value_loss)
     critic_grads = None
     if cfg.algo.critic.clip_gradients is not None and cfg.algo.critic.clip_gradients > 0:
@@ -375,33 +354,19 @@
         aggregator.update("Loss/observation_loss", observation_loss.detach())
         aggregator.update("Loss/reward_loss", reward_loss.detach())
         aggregator.update("Loss/state_loss", state_loss.detach())
         aggregator.update("Loss/continue_loss", continue_loss.detach())
         aggregator.update("State/kl", kl.mean().detach())
         aggregator.update(
             "State/post_entropy",
-            Independent(
-                OneHotCategoricalValidateArgs(logits=posteriors_logits.detach(), validate_args=validate_args),
-                1,
-                validate_args=validate_args,
-            )
-            .entropy()
-            .mean()
-            .detach(),
+            Independent(OneHotCategorical(logits=posteriors_logits.detach()), 1).entropy().mean().detach(),
         )
         aggregator.update(
             "State/prior_entropy",
-            Independent(
-                OneHotCategoricalValidateArgs(logits=priors_logits.detach(), validate_args=validate_args),
-                1,
-                validate_args=validate_args,
-            )
-            .entropy()
-            .mean()
-            .detach(),
+            Independent(OneHotCategorical(logits=priors_logits.detach()), 1).entropy().mean().detach(),
         )
         aggregator.update("Loss/policy_loss", policy_loss.detach())
         aggregator.update("Loss/value_loss", value_loss.detach())
         if world_model_grads:
             aggregator.update("Grads/world_model", world_model_grads.mean().detach())
         if actor_grads:
             aggregator.update("Grads/actor", actor_grads.mean().detach())
@@ -415,16 +380,14 @@
 
 
 @register_algorithm()
 def main(fabric: Fabric, cfg: Dict[str, Any]):
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     # These arguments cannot be changed
     cfg.env.screen_size = 64
     cfg.env.frame_stack = 1
@@ -483,37 +446,25 @@
     if cfg.metric.log_level > 0:
         fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
         fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
         fabric.print("Decoder CNN keys:", cfg.algo.cnn_keys.decoder)
         fabric.print("Decoder MLP keys:", cfg.algo.mlp_keys.decoder)
     obs_keys = cfg.algo.cnn_keys.encoder + cfg.algo.mlp_keys.encoder
 
-    world_model, actor, critic, target_critic = build_agent(
+    world_model, actor, critic, target_critic, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["world_model"] if cfg.checkpoint.resume_from else None,
         state["actor"] if cfg.checkpoint.resume_from else None,
         state["critic"] if cfg.checkpoint.resume_from else None,
         state["target_critic"] if cfg.checkpoint.resume_from else None,
     )
-    player = PlayerDV2(
-        world_model.encoder.module,
-        world_model.rssm.recurrent_model.module,
-        world_model.rssm.representation_model.module,
-        actor.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        discrete_size=cfg.algo.world_model.discrete_size,
-    )
 
     # Optimizers
     world_optimizer = hydra.utils.instantiate(
         cfg.algo.world_model.optimizer, params=world_model.parameters(), _convert_="all"
     )
     actor_optimizer = hydra.utils.instantiate(cfg.algo.actor.optimizer, params=actor.parameters(), _convert_="all")
     critic_optimizer = hydra.utils.instantiate(cfg.algo.critic.optimizer, params=critic.parameters(), _convert_="all")
@@ -576,30 +527,26 @@
         if cfg.checkpoint.resume_from
         else 1
     )
     policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
     policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    updates_before_training = cfg.algo.train_every // policy_steps_per_update if not cfg.dry_run else 0
     num_updates = cfg.algo.total_steps // policy_steps_per_update if not cfg.dry_run else 1
     learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
-    expl_decay_steps = state["expl_decay_steps"] if cfg.checkpoint.resume_from else 0
-    max_step_expl_decay = cfg.algo.actor.max_step_expl_decay // (cfg.algo.per_rank_gradient_steps * world_size)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        actor.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
         if not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -613,175 +560,171 @@
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
-    step_data["dones"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     if cfg.dry_run:
-        step_data["dones"] = step_data["dones"] + 1
+        step_data["truncated"] = step_data["truncated"] + 1
+        step_data["terminated"] = step_data["terminated"] + 1
     step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
-    step_data["is_first"] = np.ones_like(step_data["dones"])
+    step_data["is_first"] = np.ones_like(step_data["terminated"])
     rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
 
-    per_rank_gradient_steps = 0
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * world_size
 
-        # Measure environment interaction time: this considers both the model forward
-        # to get the action given the observation and the time taken into the environment
-        with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            # Sample an action given the observation received by the environment
-            if (
-                update <= learning_starts
-                and cfg.checkpoint.resume_from is None
-                and "minedojo" not in cfg.env.wrapper._target_.lower()
-            ):
-                real_actions = actions = np.array(envs.action_space.sample())
-                if not is_continuous:
-                    actions = np.concatenate(
-                        [
-                            F.one_hot(torch.as_tensor(act), act_dim).numpy()
-                            for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
-                        ],
-                        axis=-1,
-                    )
-            else:
-                with torch.no_grad():
-                    normalized_obs = {}
-                    for k in obs_keys:
-                        torch_obs = torch.as_tensor(obs[k][np.newaxis], dtype=torch.float32, device=device)
-                        if k in cfg.algo.cnn_keys.encoder:
-                            torch_obs = torch_obs / 255 - 0.5
-                        normalized_obs[k] = torch_obs
-                    mask = {k: v for k, v in normalized_obs.items() if k.startswith("mask")}
+        with torch.inference_mode():
+            # Measure environment interaction time: this considers both the model forward
+            # to get the action given the observation and the time taken into the environment
+            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
+                # Sample an action given the observation received by the environment
+                if (
+                    update <= learning_starts
+                    and cfg.checkpoint.resume_from is None
+                    and "minedojo" not in cfg.env.wrapper._target_.lower()
+                ):
+                    real_actions = actions = np.array(envs.action_space.sample())
+                    if not is_continuous:
+                        actions = np.concatenate(
+                            [
+                                F.one_hot(torch.as_tensor(act), act_dim).numpy()
+                                for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
+                            ],
+                            axis=-1,
+                        )
+                else:
+                    torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                    mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
-                    real_actions = actions = player.get_exploration_action(normalized_obs, mask)
+                    real_actions = actions = player.get_actions(torch_obs, mask=mask)
                     actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                     if is_continuous:
                         real_actions = torch.cat(real_actions, -1).cpu().numpy()
                     else:
                         real_actions = (
                             torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
 
-            step_data["is_first"] = copy.deepcopy(step_data["dones"])
-            next_obs, rewards, dones, truncated, infos = envs.step(real_actions.reshape(envs.action_space.shape))
-            dones = np.logical_or(dones, truncated).astype(np.uint8)
-            if cfg.dry_run and buffer_type == "episode":
-                dones = np.ones_like(dones)
-
-        if cfg.metric.log_level > 0 and "final_info" in infos:
-            for i, agent_ep_info in enumerate(infos["final_info"]):
-                if agent_ep_info is not None:
-                    ep_rew = agent_ep_info["episode"]["r"]
-                    ep_len = agent_ep_info["episode"]["l"]
-                    if aggregator and not aggregator.disabled:
-                        aggregator.update("Rewards/rew_avg", ep_rew)
-                        aggregator.update("Game/ep_len_avg", ep_len)
-                    fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
-
-        # Save the real next observation
-        real_next_obs = copy.deepcopy(next_obs)
-        if "final_observation" in infos:
-            for idx, final_obs in enumerate(infos["final_observation"]):
-                if final_obs is not None:
-                    for k, v in final_obs.items():
-                        real_next_obs[k][idx] = v
-
-        for k in obs_keys:  # [N_envs, N_obs]
-            step_data[k] = real_next_obs[k][np.newaxis]
-
-        # Next_obs becomes the new obs
-        obs = next_obs
-
-        step_data["dones"] = dones.reshape((1, cfg.env.num_envs, -1))
-        step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
-        step_data["rewards"] = clip_rewards_fn(rewards).reshape((1, cfg.env.num_envs, -1))
-        rb.add(step_data, validate_args=cfg.buffer.validate_args)
-
-        # Reset and save the observation coming from the automatic reset
-        dones_idxes = dones.nonzero()[0].tolist()
-        reset_envs = len(dones_idxes)
-        if reset_envs > 0:
-            reset_data = {}
-            for k in obs_keys:
-                reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
-            reset_data["dones"] = np.zeros((1, reset_envs, 1))
-            reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
-            reset_data["rewards"] = np.zeros((1, reset_envs, 1))
-            reset_data["is_first"] = np.ones_like(reset_data["dones"])
-            rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
-            # Reset dones so that `is_first` is updated
-            for d in dones_idxes:
-                step_data["dones"][0, d] = np.zeros_like(step_data["dones"][0, d])
-            # Reset internal agent states
-            player.init_states(dones_idxes)
-
-        updates_before_training -= 1
+                step_data["is_first"] = copy.deepcopy(np.logical_or(step_data["terminated"], step_data["truncated"]))
+                next_obs, rewards, terminated, truncated, infos = envs.step(
+                    real_actions.reshape(envs.action_space.shape)
+                )
+                dones = np.logical_or(terminated, truncated).astype(np.uint8)
+                if cfg.dry_run and buffer_type == "episode":
+                    dones = np.ones_like(dones)
+
+            if cfg.metric.log_level > 0 and "final_info" in infos:
+                for i, agent_ep_info in enumerate(infos["final_info"]):
+                    if agent_ep_info is not None:
+                        ep_rew = agent_ep_info["episode"]["r"]
+                        ep_len = agent_ep_info["episode"]["l"]
+                        if aggregator and not aggregator.disabled:
+                            aggregator.update("Rewards/rew_avg", ep_rew)
+                            aggregator.update("Game/ep_len_avg", ep_len)
+                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+
+            # Save the real next observation
+            real_next_obs = copy.deepcopy(next_obs)
+            if "final_observation" in infos:
+                for idx, final_obs in enumerate(infos["final_observation"]):
+                    if final_obs is not None:
+                        for k, v in final_obs.items():
+                            real_next_obs[k][idx] = v
+
+            for k in obs_keys:  # [N_envs, N_obs]
+                step_data[k] = real_next_obs[k][np.newaxis]
+
+            # Next_obs becomes the new obs
+            obs = next_obs
+
+            step_data["terminated"] = terminated.reshape((1, cfg.env.num_envs, -1))
+            step_data["truncated"] = truncated.reshape((1, cfg.env.num_envs, -1))
+            step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
+            step_data["rewards"] = clip_rewards_fn(rewards).reshape((1, cfg.env.num_envs, -1))
+            rb.add(step_data, validate_args=cfg.buffer.validate_args)
+
+            # Reset and save the observation coming from the automatic reset
+            dones_idxes = dones.nonzero()[0].tolist()
+            reset_envs = len(dones_idxes)
+            if reset_envs > 0:
+                reset_data = {}
+                for k in obs_keys:
+                    reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
+                reset_data["terminated"] = np.zeros((1, reset_envs, 1))
+                reset_data["truncated"] = np.zeros((1, reset_envs, 1))
+                reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
+                reset_data["rewards"] = np.zeros((1, reset_envs, 1))
+                reset_data["is_first"] = np.ones_like(reset_data["terminated"])
+                rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
+                # Reset dones so that `is_first` is updated
+                for d in dones_idxes:
+                    step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
+                    step_data["truncated"][0, d] = np.zeros_like(step_data["truncated"][0, d])
+                # Reset internal agent states
+                player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts and updates_before_training <= 0:
-            n_samples = (
-                cfg.algo.per_rank_pretrain_steps if update == learning_starts else cfg.algo.per_rank_gradient_steps
-            )
-            local_data = rb.sample_tensors(
-                batch_size=cfg.algo.per_rank_batch_size,
-                sequence_length=cfg.algo.per_rank_sequence_length,
-                n_samples=n_samples,
-                dtype=None,
-                device=fabric.device,
-                from_numpy=cfg.buffer.from_numpy,
-            )
-            with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
-                for i in range(next(iter(local_data.values())).shape[0]):
-                    if per_rank_gradient_steps % cfg.algo.critic.target_network_update_freq == 0:
-                        for cp, tcp in zip(critic.module.parameters(), target_critic.parameters()):
-                            tcp.data.copy_(cp.data)
-                    batch = {k: v[i].float() for k, v in local_data.items()}
-                    train(
-                        fabric,
-                        world_model,
-                        actor,
-                        critic,
-                        target_critic,
-                        world_optimizer,
-                        actor_optimizer,
-                        critic_optimizer,
-                        batch,
-                        aggregator,
-                        cfg,
-                        actions_dim,
-                    )
-                    per_rank_gradient_steps += 1
-                train_step += world_size
-            updates_before_training = cfg.algo.train_every // policy_steps_per_update
-            if cfg.algo.actor.expl_decay:
-                expl_decay_steps += 1
-                actor.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
+        if update >= learning_starts:
+            per_rank_gradient_steps = ratio(policy_step / world_size)
+            if per_rank_gradient_steps > 0:
+                local_data = rb.sample_tensors(
+                    batch_size=cfg.algo.per_rank_batch_size,
+                    sequence_length=cfg.algo.per_rank_sequence_length,
+                    n_samples=per_rank_gradient_steps,
+                    dtype=None,
+                    device=fabric.device,
+                    from_numpy=cfg.buffer.from_numpy,
                 )
-            if aggregator and not aggregator.disabled:
-                aggregator.update("Params/exploration_amount", actor.expl_amount)
+                with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
+                    for i in range(per_rank_gradient_steps):
+                        if (
+                            cumulative_per_rank_gradient_steps % cfg.algo.critic.per_rank_target_network_update_freq
+                            == 0
+                        ):
+                            for cp, tcp in zip(critic.module.parameters(), target_critic.module.parameters()):
+                                tcp.data.copy_(cp.data)
+                        batch = {k: v[i].float() for k, v in local_data.items()}
+                        train(
+                            fabric,
+                            world_model,
+                            actor,
+                            critic,
+                            target_critic,
+                            world_optimizer,
+                            actor_optimizer,
+                            critic_optimizer,
+                            batch,
+                            aggregator,
+                            cfg,
+                            actions_dim,
+                        )
+                        cumulative_per_rank_gradient_steps += 1
+                    train_step += world_size
 
         # Log metrics
         if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -809,15 +752,15 @@
                 "world_model": world_model.state_dict(),
                 "actor": actor.state_dict(),
                 "critic": critic.state_dict(),
                 "target_critic": target_critic.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "critic_optimizer": critic_optimizer.state_dict(),
-                "expl_decay_steps": expl_decay_steps,
+                "ratio": ratio.state_dict(),
                 "update": update * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v2/evaluate.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v3/evaluate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from typing import Any, Dict
 
 import gymnasium as gym
 from lightning import Fabric
 
-from sheeprl.algos.dreamer_v2.agent import PlayerDV2, build_agent
-from sheeprl.algos.dreamer_v2.utils import test
+from sheeprl.algos.dreamer_v3.agent import build_agent
+from sheeprl.algos.dreamer_v3.utils import test
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.registry import register_evaluation
 
 
-@register_evaluation(algorithms="dreamer_v2")
+@register_evaluation(algorithms="dreamer_v3")
 def evaluate(fabric: Fabric, cfg: Dict[str, Any], state: Dict[str, Any]):
     logger = get_logger(fabric, cfg)
     if logger and fabric.is_global_zero:
         fabric._loggers = [logger]
         fabric.logger.log_hyperparams(cfg)
     log_dir = get_log_dir(fabric, cfg.root_dir, cfg.run_name)
     fabric.print(f"Log dir: {log_dir}")
@@ -40,30 +40,18 @@
 
     is_continuous = isinstance(action_space, gym.spaces.Box)
     is_multidiscrete = isinstance(action_space, gym.spaces.MultiDiscrete)
     actions_dim = tuple(
         action_space.shape if is_continuous else (action_space.nvec.tolist() if is_multidiscrete else [action_space.n])
     )
     # Create the actor and critic models
-    world_model, actor, _, _ = build_agent(
+    _, _, _, _, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["world_model"],
         state["actor"],
     )
-    player = PlayerDV2(
-        world_model.encoder.module,
-        world_model.rssm.recurrent_model.module,
-        world_model.rssm.representation_model.module,
-        actor.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        discrete_size=cfg.algo.world_model.discrete_size,
-    )
-
-    test(player, fabric, cfg, log_dir, sample_actions=False)
+    del _
+    test(player, fabric, cfg, log_dir, greedy=False)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v2/loss.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v3/loss.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,88 @@
 from typing import Dict, Optional, Tuple
 
 import torch
 from torch import Tensor
-from torch.distributions import Distribution, Independent
+from torch.distributions import Distribution, Independent, OneHotCategoricalStraightThrough
 from torch.distributions.kl import kl_divergence
 
-from sheeprl.utils.distribution import OneHotCategoricalStraightThroughValidateArgs
-
 
 def reconstruction_loss(
     po: Dict[str, Distribution],
-    observations: Dict[str, Tensor],
+    observations: Tensor,
     pr: Distribution,
     rewards: Tensor,
     priors_logits: Tensor,
     posteriors_logits: Tensor,
-    kl_balancing_alpha: float = 0.8,
-    kl_free_nats: float = 0.0,
-    kl_free_avg: bool = True,
+    kl_dynamic: float = 0.5,
+    kl_representation: float = 0.1,
+    kl_free_nats: float = 1.0,
     kl_regularizer: float = 1.0,
     pc: Optional[Distribution] = None,
     continue_targets: Optional[Tensor] = None,
-    discount_scale_factor: float = 1.0,
-    validate_args: bool = False,
+    continue_scale_factor: float = 1.0,
 ) -> Tuple[Tensor, Tensor, Tensor, Tensor, Tensor, Tensor]:
     """
-    Compute the reconstruction loss as described in Eq. 2 in
-    [https://arxiv.org/abs/2010.02193](https://arxiv.org/abs/2010.02193).
+    Compute the reconstruction loss as described in Eq. 5 in
+    [https://arxiv.org/abs/2301.04104](https://arxiv.org/abs/2301.04104).
 
     Args:
         po (Dict[str, Distribution]): the distribution returned by the observation_model (decoder).
-        observations (Dict[str, Tensor]): the observations provided by the environment.
+        observations (Tensor): the observations provided by the environment.
         pr (Distribution): the reward distribution returned by the reward_model.
         rewards (Tensor): the rewards obtained by the agent during the "Environment interaction" phase.
         priors_logits (Tensor): the logits of the prior.
         posteriors_logits (Tensor): the logits of the posterior.
-        kl_balancing_alpha (float): the kl-balancing alpha value.
-            Defaults to 0.8.
+        kl_dynamic (float): the kl-balancing dynamic loss regularizer.
+            Defaults to 0.5.
+        kl_balancing_alpha (float): the kl-balancing representation loss regularizer.
+            Defaults to 0.1.
         kl_free_nats (float): lower bound of the KL divergence.
-            Default to 0.0.
+            Default to 1.0.
         kl_regularizer (float): scale factor of the KL divergence.
             Default to 1.0.
-        pc (Distribution, optional): the predicted Bernoulli distribution of the terminal steps.
+        pc (Bernoulli, optional): the predicted Bernoulli distribution of the terminal steps.
             0s for the entries that are relative to a terminal step, 1s otherwise.
             Default to None.
         continue_targets (Tensor, optional): the targets for the discount predictor. Those are normally computed
             as `(1 - data["dones"]) * args.gamma`.
             Default to None.
-        discount_scale_factor (float): the scale factor for the continue loss.
-            Default to 1.0.
-        validate_args (bool): Whether or not to validate distributions arguments.
-            Default to False.
+        continue_scale_factor (float): the scale factor for the continue loss.
+            Default to 10.
 
     Returns:
         observation_loss (Tensor): the value of the observation loss.
-        kl divergence (Tensor): the KL between posterior and prior state.
+        KL divergence (Tensor): the KL divergence between the posterior and the prior.
         reward_loss (Tensor): the value of the reward loss.
         state_loss (Tensor): the value of the state loss.
         continue_loss (Tensor): the value of the continue loss (0 if it is not computed).
         reconstruction_loss (Tensor): the value of the overall reconstruction loss.
     """
-    observation_loss = -sum([po[k].log_prob(observations[k]).mean() for k in po.keys()])
-    reward_loss = -pr.log_prob(rewards).mean()
+    rewards.device
+    observation_loss = -sum([po[k].log_prob(observations[k]) for k in po.keys()])
+    reward_loss = -pr.log_prob(rewards)
     # KL balancing
-    lhs = kl = kl_divergence(
-        Independent(
-            OneHotCategoricalStraightThroughValidateArgs(
-                logits=posteriors_logits.detach(), validate_args=validate_args
-            ),
-            1,
-            validate_args=validate_args,
-        ),
-        Independent(
-            OneHotCategoricalStraightThroughValidateArgs(logits=priors_logits, validate_args=validate_args),
-            1,
-            validate_args=validate_args,
-        ),
+    dyn_loss = kl = kl_divergence(
+        Independent(OneHotCategoricalStraightThrough(logits=posteriors_logits.detach()), 1),
+        Independent(OneHotCategoricalStraightThrough(logits=priors_logits), 1),
     )
-    rhs = kl_divergence(
-        Independent(
-            OneHotCategoricalStraightThroughValidateArgs(logits=posteriors_logits, validate_args=validate_args),
-            1,
-            validate_args=validate_args,
-        ),
-        Independent(
-            OneHotCategoricalStraightThroughValidateArgs(logits=priors_logits.detach(), validate_args=validate_args),
-            1,
-            validate_args=validate_args,
-        ),
+    free_nats = torch.full_like(dyn_loss, kl_free_nats)
+    dyn_loss = kl_dynamic * torch.maximum(dyn_loss, free_nats)
+    repr_loss = kl_divergence(
+        Independent(OneHotCategoricalStraightThrough(logits=posteriors_logits), 1),
+        Independent(OneHotCategoricalStraightThrough(logits=priors_logits.detach()), 1),
     )
-    if kl_free_avg:
-        lhs = lhs.mean()
-        rhs = rhs.mean()
-        free_nats = torch.full_like(lhs, kl_free_nats)
-        loss_lhs = torch.maximum(lhs, free_nats)
-        loss_rhs = torch.maximum(rhs, free_nats)
-    else:
-        free_nats = torch.full_like(lhs, kl_free_nats)
-        loss_lhs = torch.maximum(lhs, kl_free_nats).mean()
-        loss_rhs = torch.maximum(rhs, kl_free_nats).mean()
-    kl_loss = kl_balancing_alpha * loss_lhs + (1 - kl_balancing_alpha) * loss_rhs
+    repr_loss = kl_representation * torch.maximum(repr_loss, free_nats)
+    kl_loss = dyn_loss + repr_loss
     if pc is not None and continue_targets is not None:
-        continue_loss = discount_scale_factor * -pc.log_prob(continue_targets).mean()
+        continue_loss = continue_scale_factor * -pc.log_prob(continue_targets)
     else:
         continue_loss = torch.zeros_like(reward_loss)
-    reconstruction_loss = kl_regularizer * kl_loss + observation_loss + reward_loss + continue_loss
-    return reconstruction_loss, kl, kl_loss, reward_loss, observation_loss, continue_loss
+    reconstruction_loss = (kl_regularizer * kl_loss + observation_loss + reward_loss + continue_loss).mean()
+    return (
+        reconstruction_loss,
+        kl.mean(),
+        kl_loss.mean(),
+        reward_loss.mean(),
+        observation_loss.mean(),
+        continue_loss.mean(),
+    )
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v2/utils.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v2/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence
 
 import gymnasium as gym
+import numpy as np
 import torch
 import torch.nn as nn
 from lightning import Fabric
 from torch import Tensor
-from torch.distributions import Independent
+from torch.distributions import Independent, OneHotCategoricalStraightThrough
 
-from sheeprl.utils.distribution import OneHotCategoricalStraightThroughValidateArgs
 from sheeprl.utils.env import make_env
 from sheeprl.utils.imports import _IS_MLFLOW_AVAILABLE
 from sheeprl.utils.utils import unwrap_fabric
 
 if TYPE_CHECKING:
     from mlflow.models.model import ModelInfo
 
@@ -30,40 +30,37 @@
     "Loss/observation_loss",
     "Loss/reward_loss",
     "Loss/state_loss",
     "Loss/continue_loss",
     "State/post_entropy",
     "State/prior_entropy",
     "State/kl",
-    "Params/exploration_amount",
     "Grads/world_model",
     "Grads/actor",
     "Grads/critic",
 }
 MODELS_TO_REGISTER = {"world_model", "actor", "critic", "target_critic"}
 
 
-def compute_stochastic_state(logits: Tensor, discrete: int = 32, sample=True, validate_args=False) -> Tensor:
+def compute_stochastic_state(logits: Tensor, discrete: int = 32, sample=True) -> Tensor:
     """
     Compute the stochastic state from the logits computed by the transition or representaiton model.
 
     Args:
         logits (Tensor): logits from either the representation model or the transition model.
         discrete (int, optional): the size of the Categorical variables.
             Defaults to 32.
         sample (bool): whether or not to sample the stochastic state.
             Default to True.
-        validate_args: whether or not to validate distribution arguments.
-            Default to False.
 
     Returns:
         The sampled stochastic state.
     """
     logits = logits.view(*logits.shape[:-1], -1, discrete)
-    dist = Independent(OneHotCategoricalStraightThroughValidateArgs(logits=logits, validate_args=validate_args), 1)
+    dist = Independent(OneHotCategoricalStraightThrough(logits=logits), 1)
     stochastic_state = dist.rsample() if sample else dist.mode
     return stochastic_state
 
 
 def init_weights(m: nn.Module, mode: str = "normal"):
     """
     Initialize the parameters of the m module acording to the Xavier
@@ -101,64 +98,68 @@
     lv = []
     for i in reversed(range(horizon)):
         agg = inputs[i] + continues[i] * lmbda * agg
         lv.append(agg)
     return torch.cat(list(reversed(lv)), dim=0)
 
 
+def prepare_obs(
+    fabric: Fabric, obs: Dict[str, np.ndarray], *, cnn_keys: Sequence[str] = [], num_envs: int = 1, **kwargs
+) -> Dict[str, Tensor]:
+    torch_obs = {}
+    for k, v in obs.items():
+        torch_obs[k] = torch.from_numpy(v.copy()).to(fabric.device).float()
+        if k in cnn_keys:
+            torch_obs[k] = torch_obs[k].view(1, num_envs, -1, *v.shape[-2:]) / 255 - 0.5
+        else:
+            torch_obs[k] = torch_obs[k].view(1, num_envs, -1)
+
+    return torch_obs
+
+
 @torch.no_grad()
 def test(
-    player: Union["PlayerDV2", "PlayerDV1"],
+    player: "PlayerDV2" | "PlayerDV1",
     fabric: Fabric,
     cfg: Dict[str, Any],
     log_dir: str,
     test_name: str = "",
-    sample_actions: bool = False,
+    greedy: bool = True,
 ):
     """Test the model on the environment with the frozen model.
 
     Args:
         player (PlayerDV2 | PlayerDV1): the agent which contains all the models needed to play.
         fabric (Fabric): the fabric instance.
         cfg (Dict[str, Any]): the hyper-parameters.
         log_dir (str): the logging directory.
         test_name (str): the name of the test.
             Default to "".
-        sample_actoins (bool): whether or not to sample actions.
-            Default to False.
+        greedy (bool): whether or not to sample actions.
+            Default to True.
     """
     env: gym.Env = make_env(cfg, cfg.seed, 0, log_dir, "test" + (f"_{test_name}" if test_name != "" else ""))()
     done = False
     cumulative_rew = 0
-    device = fabric.device
-    next_obs = env.reset(seed=cfg.seed)[0]
-    for k in next_obs.keys():
-        next_obs[k] = torch.from_numpy(next_obs[k]).view(1, *next_obs[k].shape).float()
+    obs = env.reset(seed=cfg.seed)[0]
     player.num_envs = 1
     player.init_states()
     while not done:
         # Act greedly through the environment
-        preprocessed_obs = {}
-        for k, v in next_obs.items():
-            if k in cfg.algo.cnn_keys.encoder:
-                preprocessed_obs[k] = v[None, ...].to(device) / 255 - 0.5
-            elif k in cfg.algo.mlp_keys.encoder:
-                preprocessed_obs[k] = v[None, ...].to(device)
-        real_actions = player.get_greedy_action(
-            preprocessed_obs, sample_actions, {k: v for k, v in preprocessed_obs.items() if k.startswith("mask")}
+        torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder)
+        real_actions = player.get_actions(
+            torch_obs, greedy, {k: v for k, v in torch_obs.items() if k.startswith("mask")}
         )
         if player.actor.is_continuous:
             real_actions = torch.cat(real_actions, -1).cpu().numpy()
         else:
             real_actions = torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
 
         # Single environment step
-        next_obs, reward, done, truncated, _ = env.step(real_actions.reshape(env.action_space.shape))
-        for k in next_obs.keys():
-            next_obs[k] = torch.from_numpy(next_obs[k]).view(1, *next_obs[k].shape).float()
+        obs, reward, done, truncated, _ = env.step(real_actions.reshape(env.action_space.shape))
         done = done or truncated or cfg.dry_run
         cumulative_rew += reward
     fabric.print("Test - Reward:", cumulative_rew)
     if cfg.metric.log_level > 0 and len(fabric.loggers) > 0:
         fabric.logger.log_metrics({"Test/cumulative_reward": cumulative_rew}, 0)
     env.close()
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v3/agent.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v3/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 from __future__ import annotations
 
 import copy
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple
 
 import gymnasium
 import hydra
 import numpy as np
 import torch
 import torch.nn.functional as F
 from lightning.fabric import Fabric
 from lightning.fabric.wrappers import _FabricModule
-from torch import Tensor, device, nn
-from torch.distributions import Distribution, Independent, Normal, TanhTransform, TransformedDistribution
+from torch import Tensor, nn
+from torch.distributions import (
+    Distribution,
+    Independent,
+    Normal,
+    OneHotCategoricalStraightThrough,
+    TanhTransform,
+    TransformedDistribution,
+)
 from torch.distributions.utils import probs_to_logits
 
 from sheeprl.algos.dreamer_v2.agent import WorldModel
 from sheeprl.algos.dreamer_v2.utils import compute_stochastic_state
 from sheeprl.algos.dreamer_v3.utils import init_weights, uniform_init_weights
-from sheeprl.models.models import CNN, MLP, DeCNN, LayerNormGRUCell, MultiDecoder, MultiEncoder
-from sheeprl.utils.distribution import (
-    OneHotCategoricalStraightThroughValidateArgs,
-    OneHotCategoricalValidateArgs,
-    TruncatedNormal,
+from sheeprl.models.models import (
+    CNN,
+    MLP,
+    DeCNN,
+    LayerNorm,
+    LayerNormChannelLast,
+    LayerNormGRUCell,
+    MultiDecoder,
+    MultiEncoder,
 )
-from sheeprl.utils.model import LayerNormChannelLast, ModuleType, cnn_forward
+from sheeprl.utils.fabric import get_single_device_fabric
+from sheeprl.utils.model import ModuleType, cnn_forward
 from sheeprl.utils.utils import symlog
 
 
 class CNNEncoder(nn.Module):
     """The Dreamer-V3 image encoder. This is composed of 4 `nn.Conv2d` with
     kernel_size=3, stride=2 and padding=1. No bias is used if a `nn.LayerNorm`
     is used after the convolution. This 4-stages model assumes that the image
@@ -36,47 +48,48 @@
 
     Args:
         keys (Sequence[str]): the keys representing the image observations to encode.
         input_channels (Sequence[int]): the input channels, one for each image observation to encode.
         image_size (Tuple[int, int]): the image size as (Height,Width).
         channels_multiplier (int): the multiplier for the output channels. Given the 4 stages, the 4 output channels
             will be [1, 2, 4, 8] * `channels_multiplier`.
-        layer_norm (bool, optional): whether to apply the layer normalization.
-            Defaults to True.
+        layer_norm_cls (Callable[..., nn.Module]): the layer norm to apply after the input projection.
+            Defaults to LayerNormChannelLast.
+        layer_norm_kw (Dict[str, Any]): the kwargs of the layer norm.
+            Default to {"eps": 1e-3}.
         activation (ModuleType, optional): the activation function.
             Defaults to nn.SiLU.
         stages (int, optional): how many stages for the CNN.
     """
 
     def __init__(
         self,
         keys: Sequence[str],
         input_channels: Sequence[int],
         image_size: Tuple[int, int],
         channels_multiplier: int,
-        layer_norm: bool = True,
+        layer_norm_cls: Callable[..., nn.Module] = LayerNormChannelLast,
+        layer_norm_kw: Dict[str, Any] = {"eps": 1e-3},
         activation: ModuleType = nn.SiLU,
         stages: int = 4,
     ) -> None:
         super().__init__()
         self.keys = keys
         self.input_dim = (sum(input_channels), *image_size)
         self.model = nn.Sequential(
             CNN(
                 input_channels=self.input_dim[0],
                 hidden_channels=(torch.tensor([2**i for i in range(stages)]) * channels_multiplier).tolist(),
                 cnn_layer=nn.Conv2d,
-                layer_args={"kernel_size": 4, "stride": 2, "padding": 1, "bias": not layer_norm},
+                layer_args={"kernel_size": 4, "stride": 2, "padding": 1, "bias": layer_norm_cls == nn.Identity},
                 activation=activation,
-                norm_layer=[LayerNormChannelLast for _ in range(stages)] if layer_norm else None,
-                norm_args=(
-                    [{"normalized_shape": (2**i) * channels_multiplier, "eps": 1e-3} for i in range(stages)]
-                    if layer_norm
-                    else None
-                ),
+                norm_layer=[layer_norm_cls] * stages,
+                norm_args=[
+                    {**layer_norm_kw, "normalized_shape": (2**i) * channels_multiplier} for i in range(stages)
+                ],
             ),
             nn.Flatten(-3, -1),
         )
         with torch.no_grad():
             self.output_dim = self.model(torch.zeros(1, *self.input_dim)).shape[-1]
 
     def forward(self, obs: Dict[str, Tensor]) -> Tensor:
@@ -93,45 +106,46 @@
     Args:
         keys (Sequence[str]): the keys representing the vector observations to encode.
         input_dims (Sequence[int]): the dimensions of every vector to encode.
         mlp_layers (int, optional): how many mlp layers.
             Defaults to 4.
         dense_units (int, optional): the dimension of every mlp.
             Defaults to 512.
-        layer_norm (bool, optional): whether to apply the layer normalization.
-            Defaults to True.
+        layer_norm_cls (Callable[..., nn.Module]): the layer norm to apply after the input projection.
+            Defaults to LayerNorm.
+        layer_norm_kw (Dict[str, Any]): the kwargs of the layer norm.
+            Default to {"eps": 1e-3}.
         activation (ModuleType, optional): the activation function after every layer.
             Defaults to nn.SiLU.
         symlog_inputs (bool, optional): whether to squash the input with the symlog function.
             Defaults to True.
     """
 
     def __init__(
         self,
         keys: Sequence[str],
         input_dims: Sequence[int],
         mlp_layers: int = 4,
         dense_units: int = 512,
-        layer_norm: bool = True,
+        layer_norm_cls: Callable[..., nn.Module] = LayerNorm,
+        layer_norm_kw: Dict[str, Any] = {"eps": 1e-3},
         activation: ModuleType = nn.SiLU,
         symlog_inputs: bool = True,
     ) -> None:
         super().__init__()
         self.keys = keys
         self.input_dim = sum(input_dims)
         self.model = MLP(
             self.input_dim,
             None,
             [dense_units] * mlp_layers,
             activation=activation,
-            layer_args={"bias": not layer_norm},
-            norm_layer=[nn.LayerNorm for _ in range(mlp_layers)] if layer_norm else None,
-            norm_args=(
-                [{"normalized_shape": dense_units, "eps": 1e-3} for _ in range(mlp_layers)] if layer_norm else None
-            ),
+            layer_args={"bias": layer_norm_cls == nn.Identity},
+            norm_layer=layer_norm_cls,
+            norm_args={**layer_norm_kw, "normalized_shape": dense_units},
         )
         self.output_dim = dense_units
         self.symlog_inputs = symlog_inputs
 
     def forward(self, obs: Dict[str, Tensor]) -> Tensor:
         x = torch.cat([symlog(obs[k]) if self.symlog_inputs else obs[k] for k in self.keys], -1)
         return self.model(x)
@@ -152,29 +166,32 @@
             a `nn.Linear` layer is used to project the latent state to a feature vector
             of dimension [8 * `channels_multiplier`, 4, 4].
         cnn_encoder_output_dim (int): the output of the image encoder. It should be equal to
             8 * `channels_multiplier` * 4 * 4.
         image_size (Tuple[int, int]): the final image size.
         activation (nn.Module, optional): the activation function.
             Defaults to nn.SiLU.
-        layer_norm (bool, optional): whether to apply the layer normalization.
-            Defaults to True.
+        layer_norm_cls (Callable[..., nn.Module]): the layer norm to apply after the input projection.
+            Defaults to LayerNormChannelLast.
+        layer_norm_kw (Dict[str, Any]): the kwargs of the layer norm.
+            Default to {"eps": 1e-3}.
         stages (int): how many stages in the CNN decoder.
     """
 
     def __init__(
         self,
         keys: Sequence[str],
         output_channels: Sequence[int],
         channels_multiplier: int,
         latent_state_size: int,
         cnn_encoder_output_dim: int,
         image_size: Tuple[int, int],
         activation: nn.Module = nn.SiLU,
-        layer_norm: bool = True,
+        layer_norm_cls: Callable[..., nn.Module] = LayerNormChannelLast,
+        layer_norm_kw: Dict[str, Any] = {"eps": 1e-3},
         stages: int = 4,
     ) -> None:
         super().__init__()
         self.keys = keys
         self.output_channels = output_channels
         self.cnn_encoder_output_dim = cnn_encoder_output_dim
         self.image_size = image_size
@@ -186,28 +203,25 @@
                 input_channels=(2 ** (stages - 1)) * channels_multiplier,
                 hidden_channels=(
                     torch.tensor([2**i for i in reversed(range(stages - 1))]) * channels_multiplier
                 ).tolist()
                 + [self.output_dim[0]],
                 cnn_layer=nn.ConvTranspose2d,
                 layer_args=[
-                    {"kernel_size": 4, "stride": 2, "padding": 1, "bias": not layer_norm} for _ in range(stages - 1)
+                    {"kernel_size": 4, "stride": 2, "padding": 1, "bias": layer_norm_cls == nn.Identity}
+                    for _ in range(stages - 1)
                 ]
                 + [{"kernel_size": 4, "stride": 2, "padding": 1}],
                 activation=[activation for _ in range(stages - 1)] + [None],
-                norm_layer=[LayerNormChannelLast for _ in range(stages - 1)] + [None] if layer_norm else None,
-                norm_args=(
-                    [
-                        {"normalized_shape": (2 ** (stages - i - 2)) * channels_multiplier, "eps": 1e-3}
-                        for i in range(stages - 1)
-                    ]
-                    + [None]
-                    if layer_norm
-                    else None
-                ),
+                norm_layer=[layer_norm_cls for _ in range(stages - 1)] + [None],
+                norm_args=[
+                    {**layer_norm_kw, "normalized_shape": (2 ** (stages - i - 2)) * channels_multiplier}
+                    for i in range(stages - 1)
+                ]
+                + [None],
             ),
         )
 
     def forward(self, latent_states: Tensor) -> Dict[str, Tensor]:
         cnn_out = cnn_forward(self.model, latent_states, (latent_states.shape[-1],), self.output_dim)
         return {k: rec_obs for k, rec_obs in zip(self.keys, torch.split(cnn_out, self.output_channels, -3))}
 
@@ -222,43 +236,44 @@
         keys (Sequence[str]): the keys representing the vector observations to decode.
         output_dims (Sequence[int]): the dimensions of every vector to decode.
         latent_state_size (int): the dimension of the latent state.
         mlp_layers (int, optional): how many mlp layers.
             Defaults to 4.
         dense_units (int, optional): the dimension of every mlp.
             Defaults to 512.
-        layer_norm (bool, optional): whether to apply the layer normalization.
-            Defaults to True.
+        layer_norm_cls (Callable[..., nn.Module]): the layer norm to apply after the input projection.
+            Defaults to LayerNorm.
+        layer_norm_kw (Dict[str, Any]): the kwargs of the layer norm.
+            Default to {"eps": 1e-3}.
         activation (ModuleType, optional): the activation function after every layer.
             Defaults to nn.SiLU.
     """
 
     def __init__(
         self,
         keys: Sequence[str],
         output_dims: Sequence[str],
         latent_state_size: int,
         mlp_layers: int = 4,
         dense_units: int = 512,
         activation: ModuleType = nn.SiLU,
-        layer_norm: bool = True,
+        layer_norm_cls: Callable[..., nn.Module] = LayerNorm,
+        layer_norm_kw: Dict[str, Any] = {"eps": 1e-3},
     ) -> None:
         super().__init__()
         self.output_dims = output_dims
         self.keys = keys
         self.model = MLP(
             latent_state_size,
             None,
             [dense_units] * mlp_layers,
             activation=activation,
-            layer_args={"bias": not layer_norm},
-            norm_layer=[nn.LayerNorm for _ in range(mlp_layers)] if layer_norm else None,
-            norm_args=(
-                [{"normalized_shape": dense_units, "eps": 1e-3} for _ in range(mlp_layers)] if layer_norm else None
-            ),
+            layer_args={"bias": layer_norm_cls == nn.Identity},
+            norm_layer=layer_norm_cls,
+            norm_args={**layer_norm_kw, "normalized_shape": dense_units},
         )
         self.heads = nn.ModuleList([nn.Linear(dense_units, mlp_dim) for mlp_dim in self.output_dims])
 
     def forward(self, latent_states: Tensor) -> Dict[str, Tensor]:
         x = self.model(latent_states)
         return {k: h(x) for k, h in zip(self.keys, self.heads)}
 
@@ -271,37 +286,48 @@
 
     Args:
         input_size (int): the input size of the model.
         dense_units (int): the number of dense units.
         recurrent_state_size (int): the size of the recurrent state.
         activation_fn (nn.Module): the activation function.
             Default to SiLU.
-        layer_norm (bool): whether to use the LayerNorm inside the GRU.
-            Defaults to True.
+        layer_norm_cls (Callable[..., nn.Module]): the layer norm to apply after the input projection.
+            Defaults to LayerNorm.
+        layer_norm_kw (Dict[str, Any]): the kwargs of the layer norm.
+            Default to {"eps": 1e-3}.
     """
 
     def __init__(
         self,
         input_size: int,
         recurrent_state_size: int,
         dense_units: int,
         activation_fn: nn.Module = nn.SiLU,
-        layer_norm: bool = True,
+        layer_norm_cls: Callable[..., nn.Module] = LayerNorm,
+        layer_norm_kw: Dict[str, Any] = {"eps": 1e-3},
     ) -> None:
         super().__init__()
         self.mlp = MLP(
             input_dims=input_size,
             output_dim=None,
             hidden_sizes=[dense_units],
             activation=activation_fn,
-            layer_args={"bias": not layer_norm},
-            norm_layer=[nn.LayerNorm] if layer_norm else None,
-            norm_args=[{"normalized_shape": dense_units, "eps": 1e-3}] if layer_norm else None,
+            layer_args={"bias": layer_norm_cls == nn.Identity},
+            norm_layer=[layer_norm_cls],
+            norm_args=[{**layer_norm_kw, "normalized_shape": dense_units}],
         )
-        self.rnn = LayerNormGRUCell(dense_units, recurrent_state_size, bias=False, batch_first=False, layer_norm=True)
+        self.rnn = LayerNormGRUCell(
+            dense_units,
+            recurrent_state_size,
+            bias=False,
+            batch_first=False,
+            layer_norm_cls=layer_norm_cls,
+            layer_norm_kw=layer_norm_kw,
+        )
+        self.recurrent_state_size = recurrent_state_size
 
     def forward(self, input: Tensor, recurrent_state: Tensor) -> Tensor:
         """
         Compute the next recurrent state from the latent state (stochastic and recurrent states) and the actions.
 
         Args:
             input (Tensor): the input tensor composed by the stochastic state and the actions concatenated together.
@@ -334,28 +360,42 @@
             distribution over states, i.e. given some logits `l` and probabilities `p = softmax(l)`,
             then `p = (1 - self.unimix) * p + self.unimix * unif`, where `unif = `1 / self.discrete`.
             Defaults to 0.01.
     """
 
     def __init__(
         self,
-        recurrent_model: nn.Module,
-        representation_model: nn.Module,
-        transition_model: nn.Module,
+        recurrent_model: RecurrentModel | _FabricModule,
+        representation_model: nn.Module | _FabricModule,
+        transition_model: nn.Module | _FabricModule,
         distribution_cfg: Dict[str, Any],
         discrete: int = 32,
         unimix: float = 0.01,
+        learnable_initial_recurrent_state: bool = True,
     ) -> None:
         super().__init__()
         self.recurrent_model = recurrent_model
         self.representation_model = representation_model
         self.transition_model = transition_model
+        self.distribution_cfg = distribution_cfg
         self.discrete = discrete
         self.unimix = unimix
-        self.distribution_cfg = distribution_cfg
+        if learnable_initial_recurrent_state:
+            self.initial_recurrent_state = nn.Parameter(
+                torch.zeros(recurrent_model.recurrent_state_size, dtype=torch.float32)
+            )
+        else:
+            self.register_buffer(
+                "initial_recurrent_state", torch.zeros(recurrent_model.recurrent_state_size, dtype=torch.float32)
+            )
+
+    def get_initial_states(self, batch_shape: Sequence[int] | torch.Size) -> Tuple[Tensor, Tensor]:
+        initial_recurrent_state = torch.tanh(self.initial_recurrent_state).expand(*batch_shape, -1)
+        initial_posterior = self._transition(initial_recurrent_state, sample_state=False)[1]
+        return initial_recurrent_state, initial_posterior
 
     def dynamic(
         self, posterior: Tensor, recurrent_state: Tensor, action: Tensor, embedded_obs: Tensor, is_first: Tensor
     ) -> Tuple[Tensor, Tensor, Tensor, Tensor, Tensor]:
         """
         Perform one step of the dynamic learning:
             Recurrent model: compute the recurrent state from the previous latent space, the action taken by the agent,
@@ -379,19 +419,20 @@
             The posterior stochastic state (Tensor): computed by the representation model
             The prior stochastic state (Tensor): computed by the transition model
             The logits of the posterior state (Tensor): computed by the transition model from the recurrent state.
             The logits of the prior state (Tensor): computed by the transition model from the recurrent state.
             from the recurrent state and the embbedded observation.
         """
         action = (1 - is_first) * action
-        recurrent_state = (1 - is_first) * recurrent_state + is_first * torch.tanh(torch.zeros_like(recurrent_state))
+
+        initial_recurrent_state, initial_posterior = self.get_initial_states(recurrent_state.shape[:2])
+        recurrent_state = (1 - is_first) * recurrent_state + is_first * initial_recurrent_state
         posterior = posterior.view(*posterior.shape[:-2], -1)
-        posterior = (1 - is_first) * posterior + is_first * self._transition(recurrent_state, sample_state=False)[
-            1
-        ].view_as(posterior)
+        posterior = (1 - is_first) * posterior + is_first * initial_posterior.view_as(posterior)
+
         recurrent_state = self.recurrent_model(torch.cat((posterior, action), -1), recurrent_state)
         prior_logits, prior = self._transition(recurrent_state)
         posterior_logits, posterior = self._representation(recurrent_state, embedded_obs)
         return recurrent_state, posterior, prior, posterior_logits, prior_logits
 
     def _uniform_mix(self, logits: Tensor) -> Tensor:
         dim = logits.dim()
@@ -417,34 +458,30 @@
 
         Returns:
             logits (Tensor): the logits of the distribution of the posterior state.
             posterior (Tensor): the sampled posterior stochastic state.
         """
         logits: Tensor = self.representation_model(torch.cat((recurrent_state, embedded_obs), -1))
         logits = self._uniform_mix(logits)
-        return logits, compute_stochastic_state(
-            logits, discrete=self.discrete, validate_args=self.distribution_cfg.validate_args
-        )
+        return logits, compute_stochastic_state(logits, discrete=self.discrete)
 
     def _transition(self, recurrent_out: Tensor, sample_state=True) -> Tuple[Tensor, Tensor]:
         """
         Args:
             recurrent_out (Tensor): the output of the recurrent model, i.e., the deterministic part of the latent space.
             sampler_state (bool): whether or not to sample the stochastic state.
                 Default to True
 
         Returns:
             logits (Tensor): the logits of the distribution of the prior state.
             prior (Tensor): the sampled prior stochastic state.
         """
         logits: Tensor = self.transition_model(recurrent_out)
         logits = self._uniform_mix(logits)
-        return logits, compute_stochastic_state(
-            logits, discrete=self.discrete, sample=sample_state, validate_args=self.distribution_cfg.validate_args
-        )
+        return logits, compute_stochastic_state(logits, discrete=self.discrete, sample=sample_state)
 
     def imagination(self, prior: Tensor, recurrent_state: Tensor, actions: Tensor) -> Tuple[Tensor, Tensor]:
         """
         One-step imagination of the next latent state.
         It can be used several times to imagine trajectories in the latent space (Transition Model).
 
         Args:
@@ -457,363 +494,407 @@
             The recurrent state (Tensor).
         """
         recurrent_state = self.recurrent_model(torch.cat((prior, actions), -1), recurrent_state)
         _, imagined_prior = self._transition(recurrent_state)
         return imagined_prior, recurrent_state
 
 
+class DecoupledRSSM(RSSM):
+    """RSSM model for the model-base Dreamer agent.
+
+    Args:
+        recurrent_model (nn.Module): the recurrent model of the RSSM model described in
+            [https://arxiv.org/abs/1811.04551](https://arxiv.org/abs/1811.04551).
+        representation_model (nn.Module): the representation model composed by a
+            multi-layer perceptron to compute the stochastic part of the latent state.
+            For more information see [https://arxiv.org/abs/2010.02193](https://arxiv.org/abs/2010.02193).
+        transition_model (nn.Module): the transition model described in
+            [https://arxiv.org/abs/2010.02193](https://arxiv.org/abs/2010.02193).
+            The model is composed by a multi-layer perceptron to predict the stochastic part of the latent state.
+        distribution_cfg (Dict[str, Any]): the configs of the distributions.
+        discrete (int, optional): the size of the Categorical variables.
+            Defaults to 32.
+        unimix: (float, optional): the percentage of uniform distribution to inject into the categorical
+            distribution over states, i.e. given some logits `l` and probabilities `p = softmax(l)`,
+            then `p = (1 - self.unimix) * p + self.unimix * unif`, where `unif = `1 / self.discrete`.
+            Defaults to 0.01.
+    """
+
+    def __init__(
+        self,
+        recurrent_model: nn.Module | _FabricModule,
+        representation_model: nn.Module | _FabricModule,
+        transition_model: nn.Module | _FabricModule,
+        distribution_cfg: Dict[str, Any],
+        discrete: int = 32,
+        unimix: float = 0.01,
+        learnable_initial_recurrent_state: bool = True,
+    ) -> None:
+        super().__init__(
+            recurrent_model,
+            representation_model,
+            transition_model,
+            distribution_cfg,
+            discrete,
+            unimix,
+            learnable_initial_recurrent_state,
+        )
+
+    def dynamic(
+        self, posterior: Tensor, recurrent_state: Tensor, action: Tensor, is_first: Tensor
+    ) -> Tuple[Tensor, Tensor, Tensor, Tensor, Tensor]:
+        """
+        Perform one step of the dynamic learning:
+            Recurrent model: compute the recurrent state from the previous latent space, the action taken by the agent,
+                i.e., it computes the deterministic state (or ht).
+            Transition model: predict the prior from the recurrent output.
+            Representation model: compute the posterior from the recurrent state and from
+                the embedded observations provided by the environment.
+        For more information see [https://arxiv.org/abs/1811.04551](https://arxiv.org/abs/1811.04551)
+        and [https://arxiv.org/abs/2010.02193](https://arxiv.org/abs/2010.02193).
+
+        Args:
+            posterior (Tensor): the stochastic state computed by the representation model (posterior). It is expected
+                to be of dimension `[stoch_size, self.discrete]`, which by default is `[32, 32]`.
+            recurrent_state (Tensor): a tuple representing the recurrent state of the recurrent model.
+            action (Tensor): the action taken by the agent.
+            embedded_obs (Tensor): the embedded observations provided by the environment.
+            is_first (Tensor): if this is the first step in the episode.
+
+        Returns:
+            The recurrent state (Tensor): the recurrent state of the recurrent model.
+            The posterior stochastic state (Tensor): computed by the representation model
+            The prior stochastic state (Tensor): computed by the transition model
+            The logits of the posterior state (Tensor): computed by the transition model from the recurrent state.
+            The logits of the prior state (Tensor): computed by the transition model from the recurrent state.
+            from the recurrent state and the embbedded observation.
+        """
+        action = (1 - is_first) * action
+
+        initial_recurrent_state, initial_posterior = self.get_initial_states(recurrent_state.shape[:2])
+        recurrent_state = (1 - is_first) * recurrent_state + is_first * initial_recurrent_state
+        posterior = posterior.view(*posterior.shape[:-2], -1)
+        posterior = (1 - is_first) * posterior + is_first * initial_posterior.view_as(posterior)
+
+        recurrent_state = self.recurrent_model(torch.cat((posterior, action), -1), recurrent_state)
+        prior_logits, prior = self._transition(recurrent_state)
+        return recurrent_state, prior, prior_logits
+
+    def _representation(self, embedded_obs: Tensor) -> Tuple[Tensor, Tensor]:
+        """
+        Args:
+            embedded_obs (Tensor): the embedded real observations provided by the environment.
+
+        Returns:
+            logits (Tensor): the logits of the distribution of the posterior state.
+            posterior (Tensor): the sampled posterior stochastic state.
+        """
+        logits: Tensor = self.representation_model(embedded_obs)
+        logits = self._uniform_mix(logits)
+        return logits, compute_stochastic_state(logits, discrete=self.discrete)
+
+
 class PlayerDV3(nn.Module):
     """
     The model of the Dreamer_v3 player.
 
     Args:
-        encoder (_FabricModule): the encoder.
-        recurrent_model (_FabricModule): the recurrent model.
-        representation_model (_FabricModule): the representation model.
+        encoder (MultiEncoder): the encoder.
+        rssm (RSSM | DecoupledRSSM): the RSSM model.
         actor (_FabricModule): the actor.
         actions_dim (Sequence[int]): the dimension of the actions.
         num_envs (int): the number of environments.
         stochastic_size (int): the size of the stochastic state.
         recurrent_state_size (int): the size of the recurrent state.
-        device (torch.device): the device to work on.
         transition_model (_FabricModule): the transition model.
         discrete_size (int): the dimension of a single Categorical variable in the
             stochastic state (prior or posterior).
             Defaults to 32.
         actor_type (str, optional): which actor the player is using ('task' or 'exploration').
             Default to None.
+        decoupled_rssm (bool, optional): whether to use the DecoupledRSSM model.
     """
 
     def __init__(
         self,
-        encoder: _FabricModule,
-        rssm: RSSM,
-        actor: _FabricModule,
+        encoder: MultiEncoder | _FabricModule,
+        rssm: RSSM | DecoupledRSSM,
+        actor: Actor | MinedojoActor | _FabricModule,
         actions_dim: Sequence[int],
         num_envs: int,
         stochastic_size: int,
         recurrent_state_size: int,
-        device: device = "cpu",
+        device: str | torch.device,
         discrete_size: int = 32,
         actor_type: str | None = None,
     ) -> None:
         super().__init__()
         self.encoder = encoder
-        self.rssm = RSSM(
-            recurrent_model=rssm.recurrent_model.module,
-            representation_model=rssm.representation_model.module,
-            transition_model=rssm.transition_model.module,
-            distribution_cfg=actor.distribution_cfg,
-            discrete=rssm.discrete,
-            unimix=rssm.unimix,
-        )
+        self.rssm = rssm
         self.actor = actor
-        self.device = device
         self.actions_dim = actions_dim
+        self.num_envs = num_envs
         self.stochastic_size = stochastic_size
-        self.discrete_size = discrete_size
         self.recurrent_state_size = recurrent_state_size
-        self.num_envs = num_envs
-        self.validate_args = self.actor.distribution_cfg.validate_args
+        self.device = device
+        self.discrete_size = discrete_size
         self.actor_type = actor_type
+        self.decoupled_rssm = isinstance(rssm, DecoupledRSSM)
 
     @torch.no_grad()
     def init_states(self, reset_envs: Optional[Sequence[int]] = None) -> None:
         """Initialize the states and the actions for the ended environments.
 
         Args:
             reset_envs (Optional[Sequence[int]], optional): which environments' states to reset.
                 If None, then all environments' states are reset.
                 Defaults to None.
         """
         if reset_envs is None or len(reset_envs) == 0:
             self.actions = torch.zeros(1, self.num_envs, np.sum(self.actions_dim), device=self.device)
-            self.recurrent_state = torch.tanh(
-                torch.zeros(1, self.num_envs, self.recurrent_state_size, device=self.device)
-            )
-            self.stochastic_state = self.rssm._transition(self.recurrent_state, sample_state=False)[1].reshape(
-                1, self.num_envs, -1
-            )
+            self.recurrent_state, stochastic_state = self.rssm.get_initial_states((1, self.num_envs))
+            self.stochastic_state = stochastic_state.reshape(1, self.num_envs, -1)
         else:
             self.actions[:, reset_envs] = torch.zeros_like(self.actions[:, reset_envs])
-            self.recurrent_state[:, reset_envs] = torch.tanh(torch.zeros_like(self.recurrent_state[:, reset_envs]))
-            self.stochastic_state[:, reset_envs] = self.rssm._transition(
-                self.recurrent_state[:, reset_envs], sample_state=False
-            )[1].reshape(1, len(reset_envs), -1)
-
-    def get_exploration_action(self, obs: Dict[str, Tensor], mask: Optional[Dict[str, Tensor]] = None) -> Tensor:
-        """
-        Return the actions with a certain amount of noise for exploration.
-
-        Args:
-            obs (Dict[str, Tensor]): the current observations.
-            mask (Dict[str, Tensor], optional): the mask of the actions.
-                Default to None.
-
-        Returns:
-            The actions the agent has to perform.
-        """
-        actions = self.get_greedy_action(obs, mask=mask)
-        expl_actions = None
-        if self.actor.expl_amount > 0:
-            expl_actions = self.actor.add_exploration_noise(actions, mask=mask)
-            self.actions = torch.cat(expl_actions, dim=-1)
-        return expl_actions or actions
+            self.recurrent_state[:, reset_envs], stochastic_state = self.rssm.get_initial_states((1, len(reset_envs)))
+            self.stochastic_state[:, reset_envs] = stochastic_state.reshape(1, len(reset_envs), -1)
 
-    def get_greedy_action(
+    def get_actions(
         self,
         obs: Dict[str, Tensor],
-        is_training: bool = True,
+        greedy: bool = False,
         mask: Optional[Dict[str, Tensor]] = None,
     ) -> Sequence[Tensor]:
         """
         Return the greedy actions.
 
         Args:
             obs (Dict[str, Tensor]): the current observations.
-            is_training (bool): whether it is training.
-                Default to True.
+            greedy (bool): whether or not to sample the actions.
+                Default to False.
 
         Returns:
             The actions the agent has to perform.
         """
         embedded_obs = self.encoder(obs)
         self.recurrent_state = self.rssm.recurrent_model(
             torch.cat((self.stochastic_state, self.actions), -1), self.recurrent_state
         )
-        _, self.stochastic_state = self.rssm._representation(self.recurrent_state, embedded_obs)
+        if self.decoupled_rssm:
+            _, self.stochastic_state = self.rssm._representation(embedded_obs)
+        else:
+            _, self.stochastic_state = self.rssm._representation(self.recurrent_state, embedded_obs)
         self.stochastic_state = self.stochastic_state.view(
             *self.stochastic_state.shape[:-2], self.stochastic_size * self.discrete_size
         )
-        actions, _ = self.actor(torch.cat((self.stochastic_state, self.recurrent_state), -1), is_training, mask)
+        actions, _ = self.actor(torch.cat((self.stochastic_state, self.recurrent_state), -1), greedy, mask)
         self.actions = torch.cat(actions, -1)
         return actions
 
 
 class Actor(nn.Module):
     """
     The wrapper class of the Dreamer_v2 Actor model.
 
     Args:
         latent_state_size (int): the dimension of the latent state (stochastic size + recurrent_state_size).
         actions_dim (Sequence[int]): the dimension in output of the actor.
             The number of actions if continuous, the dimension of the action if discrete.
         is_continuous (bool): whether or not the actions are continuous.
         distribution_cfg (Dict[str, Any]): The configs of the distributions.
-        init_std (float): the amount to sum to the input of the softplus function for the standard deviation.
+        init_std (float): the amount to sum to the standard deviation.
             Default to 0.0.
         min_std (float): the minimum standard deviation for the actions.
-            Default to 0.1.
+            Default to 1.0.
+        max_std (float): the maximum standard deviation for the actions.
+            Default to 1.0.
         dense_units (int): the dimension of the hidden dense layers.
             Default to 1024.
         activation (int): the activation function to apply after the dense layers.
             Default to nn.SiLU.
         mlp_layers (int): the number of dense layers.
             Default to 5.
-        layer_norm (bool, optional): whether to apply the layer normalization.
-            Defaults to True.
+        layer_norm_cls (Callable[..., nn.Module]): the layer norm to apply after the input projection.
+            Defaults to LayerNorm.
+        layer_norm_kw (Dict[str, Any]): the kwargs of the layer norm.
+            Default to {"eps": 1e-3}.
         unimix: (float, optional): the percentage of uniform distribution to inject into the categorical
             distribution over actions, i.e. given some logits `l` and probabilities `p = softmax(l)`,
             then `p = (1 - self.unimix) * p + self.unimix * unif`,
             where `unif = `1 / self.discrete`.
             Defaults to 0.01.
-        expl_amount (float): the exploration amount to use during training.
-            Default to 0.0.
+        action_clip (float): the action clip parameter.
+            Default to 1.0.
     """
 
     def __init__(
         self,
         latent_state_size: int,
         actions_dim: Sequence[int],
         is_continuous: bool,
         distribution_cfg: Dict[str, Any],
         init_std: float = 0.0,
-        min_std: float = 0.1,
+        min_std: float = 1.0,
+        max_std: float = 1.0,
         dense_units: int = 1024,
         activation: nn.Module = nn.SiLU,
         mlp_layers: int = 5,
-        layer_norm: bool = True,
+        layer_norm_cls: Callable[..., nn.Module] = LayerNorm,
+        layer_norm_kw: Dict[str, Any] = {"eps": 1e-3},
         unimix: float = 0.01,
-        expl_amount: float = 0.0,
+        action_clip: float = 1.0,
     ) -> None:
         super().__init__()
         self.distribution_cfg = distribution_cfg
         self.distribution = distribution_cfg.get("type", "auto").lower()
-        if self.distribution not in ("auto", "normal", "tanh_normal", "discrete", "trunc_normal"):
+        if self.distribution not in ("auto", "normal", "tanh_normal", "discrete", "scaled_normal"):
             raise ValueError(
-                "The distribution must be on of: `auto`, `discrete`, `normal`, `tanh_normal` and `trunc_normal`. "
+                "The distribution must be on of: `auto`, `discrete`, `normal`, `tanh_normal` and `scaled_normal`. "
                 f"Found: {self.distribution}"
             )
         if self.distribution == "discrete" and is_continuous:
             raise ValueError("You have choose a discrete distribution but `is_continuous` is true")
         if self.distribution == "auto":
             if is_continuous:
-                self.distribution = "trunc_normal"
+                self.distribution = "scaled_normal"
             else:
                 self.distribution = "discrete"
         self.model = MLP(
             input_dims=latent_state_size,
             output_dim=None,
             hidden_sizes=[dense_units] * mlp_layers,
             activation=activation,
             flatten_dim=None,
-            layer_args={"bias": not layer_norm},
-            norm_layer=[nn.LayerNorm for _ in range(mlp_layers)] if layer_norm else None,
-            norm_args=(
-                [{"normalized_shape": dense_units, "eps": 1e-3} for _ in range(mlp_layers)] if layer_norm else None
-            ),
+            layer_args={"bias": layer_norm_cls == nn.Identity},
+            norm_layer=layer_norm_cls,
+            norm_args={**layer_norm_kw, "normalized_shape": dense_units},
         )
         if is_continuous:
             self.mlp_heads = nn.ModuleList([nn.Linear(dense_units, np.sum(actions_dim) * 2)])
         else:
             self.mlp_heads = nn.ModuleList([nn.Linear(dense_units, action_dim) for action_dim in actions_dim])
         self.actions_dim = actions_dim
         self.is_continuous = is_continuous
-        self.init_std = torch.tensor(init_std)
+        self.init_std = init_std
         self.min_std = min_std
+        self.max_std = max_std
         self._unimix = unimix
-        self._expl_amount = expl_amount
-
-    @property
-    def expl_amount(self) -> float:
-        return self._expl_amount
-
-    @expl_amount.setter
-    def expl_amount(self, amount: float):
-        self._expl_amount = amount
+        self._action_clip = action_clip
 
     def forward(
-        self, state: Tensor, is_training: bool = True, mask: Optional[Dict[str, Tensor]] = None
+        self, state: Tensor, greedy: bool = False, mask: Optional[Dict[str, Tensor]] = None
     ) -> Tuple[Sequence[Tensor], Sequence[Distribution]]:
         """
         Call the forward method of the actor model and reorganizes the result with shape (batch_size, *, num_actions),
         where * means any number of dimensions including None.
 
         Args:
             state (Tensor): the current state of shape (batch_size, *, stochastic_size + recurrent_state_size).
+            greedy (bool): whether or not to sample the actions.
+                Default to False.
+            mask (Dict[str, Tensor], optional): the mask to use on the actions.
+                Default to None.
 
         Returns:
             The tensor of the actions taken by the agent with shape (batch_size, *, num_actions).
             The distribution of the actions
         """
         out: Tensor = self.model(state)
         pre_dist: List[Tensor] = [head(out) for head in self.mlp_heads]
         if self.is_continuous:
             mean, std = torch.chunk(pre_dist[0], 2, -1)
             if self.distribution == "tanh_normal":
                 mean = 5 * torch.tanh(mean / 5)
                 std = F.softplus(std + self.init_std) + self.min_std
                 actions_dist = Normal(mean, std)
-                actions_dist = Independent(
-                    TransformedDistribution(
-                        actions_dist, TanhTransform(), validate_args=self.distribution_cfg.validate_args
-                    ),
-                    1,
-                    validate_args=self.distribution_cfg.validate_args,
-                )
+                actions_dist = Independent(TransformedDistribution(actions_dist, TanhTransform()), 1)
             elif self.distribution == "normal":
-                actions_dist = Normal(mean, std, validate_args=self.distribution_cfg.validate_args)
-                actions_dist = Independent(actions_dist, 1, validate_args=self.distribution_cfg.validate_args)
-            elif self.distribution == "trunc_normal":
-                std = 2 * torch.sigmoid((std + self.init_std) / 2) + self.min_std
-                dist = TruncatedNormal(torch.tanh(mean), std, -1, 1, validate_args=self.distribution_cfg.validate_args)
-                actions_dist = Independent(dist, 1, validate_args=self.distribution_cfg.validate_args)
-            if is_training:
+                actions_dist = Normal(mean, std)
+                actions_dist = Independent(actions_dist, 1)
+            elif self.distribution == "scaled_normal":
+                std = (self.max_std - self.min_std) * torch.sigmoid(std + self.init_std) + self.min_std
+                dist = Normal(torch.tanh(mean), std)
+                actions_dist = Independent(dist, 1)
+            if not greedy:
                 actions = actions_dist.rsample()
             else:
                 sample = actions_dist.sample((100,))
                 log_prob = actions_dist.log_prob(sample)
                 actions = sample[log_prob.argmax(0)].view(1, 1, -1)
+            if self._action_clip > 0.0:
+                action_clip = torch.full_like(actions, self._action_clip)
+                actions = actions * (action_clip / torch.maximum(action_clip, torch.abs(actions))).detach()
             actions = [actions]
             actions_dist = [actions_dist]
         else:
             actions_dist: List[Distribution] = []
             actions: List[Tensor] = []
             for logits in pre_dist:
-                actions_dist.append(
-                    OneHotCategoricalStraightThroughValidateArgs(
-                        logits=self._uniform_mix(logits), validate_args=self.distribution_cfg.validate_args
-                    )
-                )
-                if is_training:
+                actions_dist.append(OneHotCategoricalStraightThrough(logits=self._uniform_mix(logits)))
+                if not greedy:
                     actions.append(actions_dist[-1].rsample())
                 else:
                     actions.append(actions_dist[-1].mode)
         return tuple(actions), tuple(actions_dist)
 
     def _uniform_mix(self, logits: Tensor) -> Tensor:
         if self._unimix > 0.0:
             probs = logits.softmax(dim=-1)
             uniform = torch.ones_like(probs) / probs.shape[-1]
             probs = (1 - self._unimix) * probs + self._unimix * uniform
             logits = probs_to_logits(probs)
         return logits
 
-    def add_exploration_noise(
-        self, actions: Sequence[Tensor], mask: Optional[Dict[str, Tensor]] = None
-    ) -> Sequence[Tensor]:
-        if self.is_continuous:
-            actions = torch.cat(actions, -1)
-            if self._expl_amount > 0.0:
-                actions = torch.clip(Normal(actions, self._expl_amount).sample(), -1, 1)
-            expl_actions = [actions]
-        else:
-            expl_actions = []
-            for act in actions:
-                sample = (
-                    OneHotCategoricalValidateArgs(logits=torch.zeros_like(act), validate_args=False)
-                    .sample()
-                    .to(act.device)
-                )
-                expl_actions.append(
-                    torch.where(torch.rand(act.shape[:1], device=act.device) < self._expl_amount, sample, act)
-                )
-        return tuple(expl_actions)
-
 
 class MinedojoActor(Actor):
     def __init__(
         self,
         latent_state_size: int,
         actions_dim: Sequence[int],
         is_continuous: bool,
         distribution_cfg: Dict[str, Any],
         init_std: float = 0,
         min_std: float = 0.1,
         dense_units: int = 1024,
         activation: nn.Module = nn.SiLU,
         mlp_layers: int = 5,
-        layer_norm: bool = True,
+        layer_norm_cls: Callable[..., nn.Module] = LayerNorm,
+        layer_norm_kw: Dict[str, Any] = {"eps": 1e-3},
         unimix: float = 0.01,
-        expl_amount: float = 0.0,
+        action_clip: float = 1.0,
     ) -> None:
         super().__init__(
             latent_state_size=latent_state_size,
             actions_dim=actions_dim,
             is_continuous=is_continuous,
             distribution_cfg=distribution_cfg,
             init_std=init_std,
             min_std=min_std,
             dense_units=dense_units,
             activation=activation,
             mlp_layers=mlp_layers,
-            layer_norm=layer_norm,
+            layer_norm_cls=layer_norm_cls,
+            layer_norm_kw=layer_norm_kw,
             unimix=unimix,
-            expl_amount=expl_amount,
+            action_clip=action_clip,
         )
 
     def forward(
-        self, state: Tensor, is_training: bool = True, mask: Optional[Dict[str, Tensor]] = None
+        self, state: Tensor, greedy: bool = True, mask: Optional[Dict[str, Tensor]] = None
     ) -> Tuple[Sequence[Tensor], Sequence[Distribution]]:
         """
         Call the forward method of the actor model and reorganizes the result with shape (batch_size, *, num_actions),
         where * means any number of dimensions including None.
 
         Args:
             state (Tensor): the current state of shape (batch_size, *, stochastic_size + recurrent_state_size).
+            greedy (bool): whether or not to sample the actions.
+                Default to True.
+            mask (Dict[str, Tensor], optional): the mask to apply to the actions.
+                Default to None.
 
         Returns:
             The tensor of the actions taken by the agent with shape (batch_size, *, num_actions).
             The distribution of the actions
         """
         out: Tensor = self.model(state)
         actions_logits: List[Tensor] = [self._uniform_mix(head(out)) for head in self.mlp_heads]
@@ -837,84 +918,35 @@
                     for t in range(functional_action.shape[0]):
                         for b in range(functional_action.shape[1]):
                             sampled_action = functional_action[t, b].item()
                             if sampled_action in (16, 17):  # Equip/Place action
                                 logits[t, b][torch.logical_not(mask["mask_equip_place"][t, b])] = -torch.inf
                             elif sampled_action == 18:  # Destroy action
                                 logits[t, b][torch.logical_not(mask["mask_destroy"][t, b])] = -torch.inf
-            actions_dist.append(
-                OneHotCategoricalStraightThroughValidateArgs(
-                    logits=logits, validate_args=self.distribution_cfg.validate_args
-                )
-            )
-            if is_training:
+            actions_dist.append(OneHotCategoricalStraightThrough(logits=logits))
+            if not greedy:
                 actions.append(actions_dist[-1].rsample())
             else:
                 actions.append(actions_dist[-1].mode)
             if functional_action is None:
                 functional_action = actions[0].argmax(dim=-1)  # [T, B]
         return tuple(actions), tuple(actions_dist)
 
-    def add_exploration_noise(
-        self, actions: Sequence[Tensor], mask: Optional[Dict[str, Tensor]] = None
-    ) -> Sequence[Tensor]:
-        expl_actions = []
-        functional_action = actions[0].argmax(dim=-1)
-        for i, act in enumerate(actions):
-            logits = torch.zeros_like(act)
-            # Exploratory action must respect the constraints of the environment
-            if mask is not None:
-                if i == 0:
-                    logits[torch.logical_not(mask["mask_action_type"].expand_as(logits))] = -torch.inf
-                elif i == 1:
-                    mask["mask_craft_smelt"] = mask["mask_craft_smelt"].expand_as(logits)
-                    for t in range(functional_action.shape[0]):
-                        for b in range(functional_action.shape[1]):
-                            sampled_action = functional_action[t, b].item()
-                            if sampled_action == 15:  # Craft action
-                                logits[t, b][torch.logical_not(mask["mask_craft_smelt"][t, b])] = -torch.inf
-                elif i == 2:
-                    mask["mask_destroy"][t, b] = mask["mask_destroy"].expand_as(logits)
-                    mask["mask_equip_place"] = mask["mask_equip_place"].expand_as(logits)
-                    for t in range(functional_action.shape[0]):
-                        for b in range(functional_action.shape[1]):
-                            sampled_action = functional_action[t, b].item()
-                            if sampled_action in {16, 17}:  # Equip/Place action
-                                logits[t, b][torch.logical_not(mask["mask_equip_place"][t, b])] = -torch.inf
-                            elif sampled_action == 18:  # Destroy action
-                                logits[t, b][torch.logical_not(mask["mask_destroy"][t, b])] = -torch.inf
-            sample = (
-                OneHotCategoricalValidateArgs(logits=torch.zeros_like(act), validate_args=False).sample().to(act.device)
-            )
-            expl_amount = self.expl_amount
-            # If the action[0] was changed, and now it is critical, then we force to change also the other 2 actions
-            # to satisfy the constraints of the environment
-            if (
-                i in {1, 2}
-                and actions[0].argmax() != expl_actions[0].argmax()
-                and expl_actions[0].argmax().item() in {15, 16, 17, 18}
-            ):
-                expl_amount = 2
-            expl_actions.append(torch.where(torch.rand(act.shape[:1], device=self.device) < expl_amount, sample, act))
-            if mask is not None and i == 0:
-                functional_action = expl_actions[0].argmax(dim=-1)
-        return tuple(expl_actions)
-
 
 def build_agent(
     fabric: Fabric,
     actions_dim: Sequence[int],
     is_continuous: bool,
     cfg: Dict[str, Any],
     obs_space: gymnasium.spaces.Dict,
     world_model_state: Optional[Dict[str, Tensor]] = None,
     actor_state: Optional[Dict[str, Tensor]] = None,
     critic_state: Optional[Dict[str, Tensor]] = None,
     target_critic_state: Optional[Dict[str, Tensor]] = None,
-) -> Tuple[WorldModel, _FabricModule, _FabricModule, torch.nn.Module]:
+) -> Tuple[WorldModel, _FabricModule, _FabricModule, _FabricModule, PlayerDV3]:
     """Build the models and wrap them with Fabric.
 
     Args:
         fabric (Fabric): the fabric object.
         actions_dim (Sequence[int]): the dimension of the actions.
         is_continuous (bool): whether or not the actions are continuous.
         cfg (DictConfig): the configs of DreamerV3.
@@ -948,179 +980,193 @@
     cnn_stages = int(np.log2(cfg.env.screen_size) - np.log2(4))
     cnn_encoder = (
         CNNEncoder(
             keys=cfg.algo.cnn_keys.encoder,
             input_channels=[int(np.prod(obs_space[k].shape[:-2])) for k in cfg.algo.cnn_keys.encoder],
             image_size=obs_space[cfg.algo.cnn_keys.encoder[0]].shape[-2:],
             channels_multiplier=world_model_cfg.encoder.cnn_channels_multiplier,
-            layer_norm=world_model_cfg.encoder.layer_norm,
-            activation=eval(world_model_cfg.encoder.cnn_act),
+            layer_norm_cls=hydra.utils.get_class(world_model_cfg.encoder.cnn_layer_norm.cls),
+            layer_norm_kw=world_model_cfg.encoder.cnn_layer_norm.kw,
+            activation=hydra.utils.get_class(world_model_cfg.encoder.cnn_act),
             stages=cnn_stages,
         )
         if cfg.algo.cnn_keys.encoder is not None and len(cfg.algo.cnn_keys.encoder) > 0
         else None
     )
     mlp_encoder = (
         MLPEncoder(
             keys=cfg.algo.mlp_keys.encoder,
             input_dims=[obs_space[k].shape[0] for k in cfg.algo.mlp_keys.encoder],
             mlp_layers=world_model_cfg.encoder.mlp_layers,
             dense_units=world_model_cfg.encoder.dense_units,
-            activation=eval(world_model_cfg.encoder.dense_act),
-            layer_norm=world_model_cfg.encoder.layer_norm,
+            activation=hydra.utils.get_class(world_model_cfg.encoder.dense_act),
+            layer_norm_cls=hydra.utils.get_class(world_model_cfg.encoder.mlp_layer_norm.cls),
+            layer_norm_kw=world_model_cfg.encoder.mlp_layer_norm.kw,
         )
         if cfg.algo.mlp_keys.encoder is not None and len(cfg.algo.mlp_keys.encoder) > 0
         else None
     )
     encoder = MultiEncoder(cnn_encoder, mlp_encoder)
+
     recurrent_model = RecurrentModel(
-        **world_model_cfg.recurrent_model,
         input_size=int(sum(actions_dim) + stochastic_size),
+        recurrent_state_size=world_model_cfg.recurrent_model.recurrent_state_size,
+        dense_units=world_model_cfg.recurrent_model.dense_units,
+        layer_norm_cls=hydra.utils.get_class(world_model_cfg.recurrent_model.layer_norm.cls),
+        layer_norm_kw=world_model_cfg.recurrent_model.layer_norm.kw,
     )
+    represention_model_input_size = encoder.output_dim
+    if not cfg.algo.world_model.decoupled_rssm:
+        represention_model_input_size += recurrent_state_size
+    representation_ln_cls = hydra.utils.get_class(world_model_cfg.representation_model.layer_norm.cls)
     representation_model = MLP(
-        input_dims=recurrent_state_size + encoder.cnn_output_dim + encoder.mlp_output_dim,
+        input_dims=represention_model_input_size,
         output_dim=stochastic_size,
         hidden_sizes=[world_model_cfg.representation_model.hidden_size],
-        activation=eval(world_model_cfg.representation_model.dense_act),
-        layer_args={"bias": not world_model_cfg.representation_model.layer_norm},
+        activation=hydra.utils.get_class(world_model_cfg.representation_model.dense_act),
+        layer_args={"bias": representation_ln_cls == nn.Identity},
         flatten_dim=None,
-        norm_layer=[nn.LayerNorm] if world_model_cfg.representation_model.layer_norm else None,
-        norm_args=(
-            [{"normalized_shape": world_model_cfg.representation_model.hidden_size}]
-            if world_model_cfg.representation_model.layer_norm
-            else None
-        ),
+        norm_layer=[representation_ln_cls],
+        norm_args=[
+            {
+                **world_model_cfg.representation_model.layer_norm.kw,
+                "normalized_shape": world_model_cfg.representation_model.hidden_size,
+            }
+        ],
     )
+    transition_ln_cls = hydra.utils.get_class(world_model_cfg.transition_model.layer_norm.cls)
     transition_model = MLP(
         input_dims=recurrent_state_size,
         output_dim=stochastic_size,
         hidden_sizes=[world_model_cfg.transition_model.hidden_size],
-        activation=eval(world_model_cfg.transition_model.dense_act),
-        layer_args={"bias": not world_model_cfg.transition_model.layer_norm},
+        activation=hydra.utils.get_class(world_model_cfg.transition_model.dense_act),
+        layer_args={"bias": transition_ln_cls == nn.Identity},
         flatten_dim=None,
-        norm_layer=[nn.LayerNorm] if world_model_cfg.transition_model.layer_norm else None,
-        norm_args=(
-            [{"normalized_shape": world_model_cfg.transition_model.hidden_size}]
-            if world_model_cfg.transition_model.layer_norm
-            else None
-        ),
+        norm_layer=[transition_ln_cls],
+        norm_args=[
+            {
+                **world_model_cfg.transition_model.layer_norm.kw,
+                "normalized_shape": world_model_cfg.transition_model.hidden_size,
+            }
+        ],
     )
-    rssm = RSSM(
+
+    if cfg.algo.world_model.decoupled_rssm:
+        rssm_cls = DecoupledRSSM
+    else:
+        rssm_cls = RSSM
+    rssm = rssm_cls(
         recurrent_model=recurrent_model.apply(init_weights),
         representation_model=representation_model.apply(init_weights),
         transition_model=transition_model.apply(init_weights),
         distribution_cfg=cfg.distribution,
         discrete=world_model_cfg.discrete_size,
         unimix=cfg.algo.unimix,
-    )
+        learnable_initial_recurrent_state=cfg.algo.world_model.learnable_initial_recurrent_state,
+    ).to(fabric.device)
+
     cnn_decoder = (
         CNNDecoder(
             keys=cfg.algo.cnn_keys.decoder,
             output_channels=[int(np.prod(obs_space[k].shape[:-2])) for k in cfg.algo.cnn_keys.decoder],
             channels_multiplier=world_model_cfg.observation_model.cnn_channels_multiplier,
             latent_state_size=latent_state_size,
             cnn_encoder_output_dim=cnn_encoder.output_dim,
             image_size=obs_space[cfg.algo.cnn_keys.decoder[0]].shape[-2:],
-            activation=eval(world_model_cfg.observation_model.cnn_act),
-            layer_norm=world_model_cfg.observation_model.layer_norm,
+            activation=hydra.utils.get_class(world_model_cfg.observation_model.cnn_act),
+            layer_norm_cls=hydra.utils.get_class(world_model_cfg.observation_model.cnn_layer_norm.cls),
+            layer_norm_kw=world_model_cfg.observation_model.mlp_layer_norm.kw,
             stages=cnn_stages,
         )
         if cfg.algo.cnn_keys.decoder is not None and len(cfg.algo.cnn_keys.decoder) > 0
         else None
     )
     mlp_decoder = (
         MLPDecoder(
             keys=cfg.algo.mlp_keys.decoder,
             output_dims=[obs_space[k].shape[0] for k in cfg.algo.mlp_keys.decoder],
             latent_state_size=latent_state_size,
             mlp_layers=world_model_cfg.observation_model.mlp_layers,
             dense_units=world_model_cfg.observation_model.dense_units,
-            activation=eval(world_model_cfg.observation_model.dense_act),
-            layer_norm=world_model_cfg.observation_model.layer_norm,
+            activation=hydra.utils.get_class(world_model_cfg.observation_model.dense_act),
+            layer_norm_cls=hydra.utils.get_class(world_model_cfg.observation_model.mlp_layer_norm.cls),
+            layer_norm_kw=world_model_cfg.observation_model.mlp_layer_norm.kw,
         )
         if cfg.algo.mlp_keys.decoder is not None and len(cfg.algo.mlp_keys.decoder) > 0
         else None
     )
     observation_model = MultiDecoder(cnn_decoder, mlp_decoder)
+
+    reward_ln_cls = hydra.utils.get_class(world_model_cfg.reward_model.layer_norm.cls)
     reward_model = MLP(
         input_dims=latent_state_size,
         output_dim=world_model_cfg.reward_model.bins,
         hidden_sizes=[world_model_cfg.reward_model.dense_units] * world_model_cfg.reward_model.mlp_layers,
-        activation=eval(world_model_cfg.reward_model.dense_act),
-        layer_args={"bias": not world_model_cfg.reward_model.layer_norm},
+        activation=hydra.utils.get_class(world_model_cfg.reward_model.dense_act),
+        layer_args={"bias": reward_ln_cls == nn.Identity},
         flatten_dim=None,
-        norm_layer=(
-            [nn.LayerNorm for _ in range(world_model_cfg.reward_model.mlp_layers)]
-            if world_model_cfg.reward_model.layer_norm
-            else None
-        ),
-        norm_args=(
-            [
-                {"normalized_shape": world_model_cfg.reward_model.dense_units}
-                for _ in range(world_model_cfg.reward_model.mlp_layers)
-            ]
-            if world_model_cfg.reward_model.layer_norm
-            else None
-        ),
+        norm_layer=reward_ln_cls,
+        norm_args={
+            **world_model_cfg.reward_model.layer_norm.kw,
+            "normalized_shape": world_model_cfg.reward_model.dense_units,
+        },
     )
+
+    discount_ln_cls = hydra.utils.get_class(world_model_cfg.discount_model.layer_norm.cls)
     continue_model = MLP(
         input_dims=latent_state_size,
         output_dim=1,
         hidden_sizes=[world_model_cfg.discount_model.dense_units] * world_model_cfg.discount_model.mlp_layers,
-        activation=eval(world_model_cfg.discount_model.dense_act),
-        layer_args={"bias": not world_model_cfg.discount_model.layer_norm},
+        activation=hydra.utils.get_class(world_model_cfg.discount_model.dense_act),
+        layer_args={"bias": discount_ln_cls == nn.Identity},
         flatten_dim=None,
-        norm_layer=(
-            [nn.LayerNorm for _ in range(world_model_cfg.discount_model.mlp_layers)]
-            if world_model_cfg.discount_model.layer_norm
-            else None
-        ),
-        norm_args=(
-            [
-                {"normalized_shape": world_model_cfg.discount_model.dense_units}
-                for _ in range(world_model_cfg.discount_model.mlp_layers)
-            ]
-            if world_model_cfg.discount_model.layer_norm
-            else None
-        ),
+        norm_layer=discount_ln_cls,
+        norm_args={
+            **world_model_cfg.discount_model.layer_norm.kw,
+            "normalized_shape": world_model_cfg.discount_model.dense_units,
+        },
     )
     world_model = WorldModel(
         encoder.apply(init_weights),
         rssm,
         observation_model.apply(init_weights),
         reward_model.apply(init_weights),
         continue_model.apply(init_weights),
     )
+
     actor_cls = hydra.utils.get_class(cfg.algo.actor.cls)
-    actor: nn.Module = actor_cls(
+    actor: Actor | MinedojoActor = actor_cls(
         latent_state_size=latent_state_size,
         actions_dim=actions_dim,
         is_continuous=is_continuous,
         init_std=actor_cfg.init_std,
         min_std=actor_cfg.min_std,
         dense_units=actor_cfg.dense_units,
-        activation=eval(actor_cfg.dense_act),
+        activation=hydra.utils.get_class(actor_cfg.dense_act),
         mlp_layers=actor_cfg.mlp_layers,
         distribution_cfg=cfg.distribution,
-        layer_norm=actor_cfg.layer_norm,
+        layer_norm_cls=hydra.utils.get_class(actor_cfg.layer_norm.cls),
+        layer_norm_kw=actor_cfg.layer_norm.kw,
         unimix=cfg.algo.unimix,
+        action_clip=actor_cfg.action_clip,
     )
+
+    critic_ln_cls = hydra.utils.get_class(critic_cfg.layer_norm.cls)
     critic = MLP(
         input_dims=latent_state_size,
         output_dim=critic_cfg.bins,
         hidden_sizes=[critic_cfg.dense_units] * critic_cfg.mlp_layers,
-        activation=eval(critic_cfg.dense_act),
-        layer_args={"bias": not critic_cfg.layer_norm},
+        activation=hydra.utils.get_class(critic_cfg.dense_act),
+        layer_args={"bias": critic_ln_cls == nn.Identity},
         flatten_dim=None,
-        norm_layer=[nn.LayerNorm for _ in range(critic_cfg.mlp_layers)] if critic_cfg.layer_norm else None,
-        norm_args=(
-            [{"normalized_shape": critic_cfg.dense_units} for _ in range(critic_cfg.mlp_layers)]
-            if critic_cfg.layer_norm
-            else None
-        ),
+        norm_layer=critic_ln_cls,
+        norm_args={
+            **critic_cfg.layer_norm.kw,
+            "normalized_shape": critic_cfg.dense_units,
+        },
     )
     actor.apply(init_weights)
     critic.apply(init_weights)
 
     if cfg.algo.hafner_initialization:
         actor.mlp_heads.apply(uniform_init_weights(1.0))
         critic.model[-1].apply(uniform_init_weights(0.0))
@@ -1137,23 +1183,54 @@
     if world_model_state:
         world_model.load_state_dict(world_model_state)
     if actor_state:
         actor.load_state_dict(actor_state)
     if critic_state:
         critic.load_state_dict(critic_state)
 
+    # Create the player agent
+    fabric_player = get_single_device_fabric(fabric)
+    player = PlayerDV3(
+        copy.deepcopy(world_model.encoder),
+        copy.deepcopy(world_model.rssm),
+        copy.deepcopy(actor),
+        actions_dim,
+        cfg.env.num_envs,
+        cfg.algo.world_model.stochastic_size,
+        cfg.algo.world_model.recurrent_model.recurrent_state_size,
+        fabric_player.device,
+        discrete_size=cfg.algo.world_model.discrete_size,
+    )
+
     # Setup models with Fabric
     world_model.encoder = fabric.setup_module(world_model.encoder)
     world_model.observation_model = fabric.setup_module(world_model.observation_model)
     world_model.reward_model = fabric.setup_module(world_model.reward_model)
     world_model.rssm.recurrent_model = fabric.setup_module(world_model.rssm.recurrent_model)
     world_model.rssm.representation_model = fabric.setup_module(world_model.rssm.representation_model)
     world_model.rssm.transition_model = fabric.setup_module(world_model.rssm.transition_model)
     if world_model.continue_model:
         world_model.continue_model = fabric.setup_module(world_model.continue_model)
     actor = fabric.setup_module(actor)
     critic = fabric.setup_module(critic)
+
+    # Setup target critic with a SingleDeviceStrategy
     target_critic = copy.deepcopy(critic.module)
     if target_critic_state:
         target_critic.load_state_dict(target_critic_state)
+    target_critic = fabric_player.setup_module(target_critic)
 
-    return world_model, actor, critic, target_critic
+    # Setup the player agent with a single-device Fabric
+    player.encoder = fabric_player.setup_module(player.encoder)
+    player.rssm.recurrent_model = fabric_player.setup_module(player.rssm.recurrent_model)
+    player.rssm.transition_model = fabric_player.setup_module(player.rssm.transition_model)
+    player.rssm.representation_model = fabric_player.setup_module(player.rssm.representation_model)
+    player.actor = fabric_player.setup_module(player.actor)
+
+    # Tie weights between the agent and the player
+    for agent_p, p in zip(world_model.encoder.parameters(), player.encoder.parameters()):
+        p.data = agent_p.data
+    for agent_p, p in zip(world_model.rssm.parameters(), player.rssm.parameters()):
+        p.data = agent_p.data
+    for agent_p, p in zip(actor.parameters(), player.actor.parameters()):
+        p.data = agent_p.data
+    return world_model, actor, critic, target_critic, player
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v3/dreamer_v3.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v3/dreamer_v3.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,36 +14,35 @@
 import hydra
 import numpy as np
 import torch
 import torch.nn.functional as F
 from lightning.fabric import Fabric
 from lightning.fabric.wrappers import _FabricModule
 from torch import Tensor
-from torch.distributions import Distribution, Independent
+from torch.distributions import Distribution, Independent, OneHotCategorical
 from torch.optim import Optimizer
 from torchmetrics import SumMetric
 
-from sheeprl.algos.dreamer_v3.agent import PlayerDV3, WorldModel, build_agent
+from sheeprl.algos.dreamer_v3.agent import WorldModel, build_agent
 from sheeprl.algos.dreamer_v3.loss import reconstruction_loss
-from sheeprl.algos.dreamer_v3.utils import Moments, compute_lambda_values, test
+from sheeprl.algos.dreamer_v3.utils import Moments, compute_lambda_values, prepare_obs, test
 from sheeprl.data.buffers import EnvIndependentReplayBuffer, SequentialReplayBuffer
 from sheeprl.envs.wrappers import RestartOnException
 from sheeprl.utils.distribution import (
     BernoulliSafeMode,
     MSEDistribution,
-    OneHotCategoricalValidateArgs,
     SymlogDistribution,
     TwoHotEncodingDistribution,
 )
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import polynomial_decay, save_configs
+from sheeprl.utils.utils import Ratio, save_configs
 
 # Decomment the following two lines if you cannot start an experiment with DMC environments
 # os.environ["PYOPENGL_PLATFORM"] = ""
 # os.environ["MUJOCO_GL"] = "osmesa"
 
 
 def train(
@@ -88,15 +87,14 @@
     # Observations:  o0       o1       o2       o3
     # Rewards:       0        r1       r2       r3
     # Dones:         0        d1       d2       d3
     # Is-first       1        i1       i2       i3
 
     batch_size = cfg.algo.per_rank_batch_size
     sequence_length = cfg.algo.per_rank_sequence_length
-    validate_args = cfg.distribution.validate_args
     recurrent_state_size = cfg.algo.world_model.recurrent_model.recurrent_state_size
     stochastic_size = cfg.algo.world_model.stochastic_size
     discrete_size = cfg.algo.world_model.discrete_size
     device = fabric.device
     batch_obs = {k: data[k] / 255.0 - 0.5 for k in cfg.algo.cnn_keys.encoder}
     batch_obs.update({k: data[k] for k in cfg.algo.mlp_keys.encoder})
     data["is_first"][0, :] = torch.ones_like(data["is_first"][0, :])
@@ -104,31 +102,51 @@
     # Given how the environment interaction works, we remove the last actions
     # and add the first one as the zero action
     batch_actions = torch.cat((torch.zeros_like(data["actions"][:1]), data["actions"][:-1]), dim=0)
 
     # Dynamic Learning
     stoch_state_size = stochastic_size * discrete_size
     recurrent_state = torch.zeros(1, batch_size, recurrent_state_size, device=device)
-    posterior = torch.zeros(1, batch_size, stochastic_size, discrete_size, device=device)
     recurrent_states = torch.empty(sequence_length, batch_size, recurrent_state_size, device=device)
     priors_logits = torch.empty(sequence_length, batch_size, stoch_state_size, device=device)
-    posteriors = torch.empty(sequence_length, batch_size, stochastic_size, discrete_size, device=device)
-    posteriors_logits = torch.empty(sequence_length, batch_size, stoch_state_size, device=device)
 
     # Embed observations from the environment
     embedded_obs = world_model.encoder(batch_obs)
 
-    for i in range(0, sequence_length):
-        recurrent_state, posterior, _, posterior_logits, prior_logits = world_model.rssm.dynamic(
-            posterior, recurrent_state, batch_actions[i : i + 1], embedded_obs[i : i + 1], data["is_first"][i : i + 1]
-        )
-        recurrent_states[i] = recurrent_state
-        priors_logits[i] = prior_logits
-        posteriors[i] = posterior
-        posteriors_logits[i] = posterior_logits
+    if cfg.algo.world_model.decoupled_rssm:
+        posteriors_logits, posteriors = world_model.rssm._representation(embedded_obs)
+        for i in range(0, sequence_length):
+            if i == 0:
+                posterior = torch.zeros_like(posteriors[:1])
+            else:
+                posterior = posteriors[i - 1 : i]
+            recurrent_state, posterior_logits, prior_logits = world_model.rssm.dynamic(
+                posterior,
+                recurrent_state,
+                batch_actions[i : i + 1],
+                data["is_first"][i : i + 1],
+            )
+            recurrent_states[i] = recurrent_state
+            priors_logits[i] = prior_logits
+    else:
+        posterior = torch.zeros(1, batch_size, stochastic_size, discrete_size, device=device)
+        posteriors = torch.empty(sequence_length, batch_size, stochastic_size, discrete_size, device=device)
+        posteriors_logits = torch.empty(sequence_length, batch_size, stoch_state_size, device=device)
+        for i in range(0, sequence_length):
+            recurrent_state, posterior, _, posterior_logits, prior_logits = world_model.rssm.dynamic(
+                posterior,
+                recurrent_state,
+                batch_actions[i : i + 1],
+                embedded_obs[i : i + 1],
+                data["is_first"][i : i + 1],
+            )
+            recurrent_states[i] = recurrent_state
+            priors_logits[i] = prior_logits
+            posteriors[i] = posterior
+            posteriors_logits[i] = posterior_logits
     latent_states = torch.cat((posteriors.view(*posteriors.shape[:-2], -1), recurrent_states), -1)
 
     # Compute predictions for the observations
     reconstructed_obs: Dict[str, torch.Tensor] = world_model.observation_model(latent_states)
 
     # Compute the distribution over the reconstructed observations
     po = {
@@ -142,20 +160,16 @@
         }
     )
 
     # Compute the distribution over the rewards
     pr = TwoHotEncodingDistribution(world_model.reward_model(latent_states), dims=1)
 
     # Compute the distribution over the terminal steps, if required
-    pc = Independent(
-        BernoulliSafeMode(logits=world_model.continue_model(latent_states), validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
-    continue_targets = 1 - data["dones"]
+    pc = Independent(BernoulliSafeMode(logits=world_model.continue_model(latent_states)), 1)
+    continues_targets = 1 - data["terminated"]
 
     # Reshape posterior and prior logits to shape [B, T, 32, 32]
     priors_logits = priors_logits.view(*priors_logits.shape[:-1], stochastic_size, discrete_size)
     posteriors_logits = posteriors_logits.view(*posteriors_logits.shape[:-1], stochastic_size, discrete_size)
 
     # World model optimization step. Eq. 4 in the paper
     world_optimizer.zero_grad(set_to_none=True)
@@ -167,17 +181,16 @@
         priors_logits,
         posteriors_logits,
         cfg.algo.world_model.kl_dynamic,
         cfg.algo.world_model.kl_representation,
         cfg.algo.world_model.kl_free_nats,
         cfg.algo.world_model.kl_regularizer,
         pc,
-        continue_targets,
+        continues_targets,
         cfg.algo.world_model.continue_scale_factor,
-        validate_args=validate_args,
     )
     fabric.backward(rec_loss)
     world_model_grads = None
     if cfg.algo.world_model.clip_gradients is not None and cfg.algo.world_model.clip_gradients > 0:
         world_model_grads = fabric.clip_gradients(
             module=world_model,
             optimizer=world_optimizer,
@@ -226,21 +239,17 @@
         imagined_trajectories[i] = imagined_latent_state
         actions = torch.cat(actor(imagined_latent_state.detach())[0], dim=-1)
         imagined_actions[i] = actions
 
     # Predict values, rewards and continues
     predicted_values = TwoHotEncodingDistribution(critic(imagined_trajectories), dims=1).mean
     predicted_rewards = TwoHotEncodingDistribution(world_model.reward_model(imagined_trajectories), dims=1).mean
-    continues = Independent(
-        BernoulliSafeMode(logits=world_model.continue_model(imagined_trajectories), validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    ).mode
-    true_done = (1 - data["dones"]).flatten().reshape(1, -1, 1)
-    continues = torch.cat((true_done, continues[1:]))
+    continues = Independent(BernoulliSafeMode(logits=world_model.continue_model(imagined_trajectories)), 1).mode
+    true_continue = (1 - data["terminated"]).flatten().reshape(1, -1, 1)
+    continues = torch.cat((true_continue, continues[1:]))
 
     # Estimate lambda-values
     lambda_values = compute_lambda_values(
         predicted_rewards[1:],
         predicted_values[1:],
         continues[1:] * cfg.algo.gamma,
         lmbda=cfg.algo.lmbda,
@@ -320,33 +329,19 @@
         aggregator.update("Loss/observation_loss", observation_loss.detach())
         aggregator.update("Loss/reward_loss", reward_loss.detach())
         aggregator.update("Loss/state_loss", state_loss.detach())
         aggregator.update("Loss/continue_loss", continue_loss.detach())
         aggregator.update("State/kl", kl.mean().detach())
         aggregator.update(
             "State/post_entropy",
-            Independent(
-                OneHotCategoricalValidateArgs(logits=posteriors_logits.detach(), validate_args=validate_args),
-                1,
-                validate_args=validate_args,
-            )
-            .entropy()
-            .mean()
-            .detach(),
+            Independent(OneHotCategorical(logits=posteriors_logits.detach()), 1).entropy().mean().detach(),
         )
         aggregator.update(
             "State/prior_entropy",
-            Independent(
-                OneHotCategoricalValidateArgs(logits=priors_logits.detach(), validate_args=validate_args),
-                1,
-                validate_args=validate_args,
-            )
-            .entropy()
-            .mean()
-            .detach(),
+            Independent(OneHotCategorical(logits=priors_logits.detach()), 1).entropy().mean().detach(),
         )
         aggregator.update("Loss/policy_loss", policy_loss.detach())
         aggregator.update("Loss/value_loss", value_loss.detach())
         if world_model_grads:
             aggregator.update("Grads/world_model", world_model_grads.mean().detach())
         if actor_grads:
             aggregator.update("Grads/actor", actor_grads.mean().detach())
@@ -360,16 +355,14 @@
 
 
 @register_algorithm()
 def main(fabric: Fabric, cfg: Dict[str, Any]):
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     # These arguments cannot be changed
     cfg.env.frame_stack = -1
     if 2 ** int(np.log2(cfg.env.screen_size)) != cfg.env.screen_size:
@@ -432,36 +425,25 @@
     if cfg.metric.log_level > 0:
         fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
         fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
         fabric.print("Decoder CNN keys:", cfg.algo.cnn_keys.decoder)
         fabric.print("Decoder MLP keys:", cfg.algo.mlp_keys.decoder)
     obs_keys = cfg.algo.cnn_keys.encoder + cfg.algo.mlp_keys.encoder
 
-    world_model, actor, critic, target_critic = build_agent(
+    world_model, actor, critic, target_critic, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["world_model"] if cfg.checkpoint.resume_from else None,
         state["actor"] if cfg.checkpoint.resume_from else None,
         state["critic"] if cfg.checkpoint.resume_from else None,
         state["target_critic"] if cfg.checkpoint.resume_from else None,
     )
-    player = PlayerDV3(
-        world_model.encoder.module,
-        world_model.rssm,
-        actor.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        discrete_size=cfg.algo.world_model.discrete_size,
-    )
 
     # Optimizers
     world_optimizer = hydra.utils.instantiate(
         cfg.algo.world_model.optimizer, params=world_model.parameters(), _convert_="all"
     )
     actor_optimizer = hydra.utils.instantiate(cfg.algo.actor.optimizer, params=actor.parameters(), _convert_="all")
     critic_optimizer = hydra.utils.instantiate(cfg.algo.critic.optimizer, params=critic.parameters(), _convert_="all")
@@ -501,15 +483,14 @@
     if cfg.checkpoint.resume_from and cfg.buffer.checkpoint:
         if isinstance(state["rb"], list) and fabric.world_size == len(state["rb"]):
             rb = state["rb"][fabric.global_rank]
         elif isinstance(state["rb"], EnvIndependentReplayBuffer):
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {fabric.world_size} processes are instantiated")
-    expl_decay_steps = state["expl_decay_steps"] if cfg.checkpoint.resume_from else 0
 
     # Global variables
     train_step = 0
     last_train = 0
     start_step = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
@@ -518,29 +499,26 @@
         if cfg.checkpoint.resume_from
         else 1
     )
     policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
     policy_steps_per_update = int(cfg.env.num_envs * fabric.world_size)
-    updates_before_training = cfg.algo.train_every // policy_steps_per_update
     num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
     learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
-    max_step_expl_decay = cfg.algo.actor.max_step_expl_decay // (cfg.algo.per_rank_gradient_steps * fabric.world_size)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // fabric.world_size
-        actor.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
         if not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -554,182 +532,184 @@
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
-    step_data["dones"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
-    step_data["is_first"] = np.ones_like(step_data["dones"])
+    step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["is_first"] = np.ones_like(step_data["terminated"])
     player.init_states()
 
-    per_rank_gradient_steps = 0
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * world_size
 
-        # Measure environment interaction time: this considers both the model forward
-        # to get the action given the observation and the time taken into the environment
-        with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            # Sample an action given the observation received by the environment
-            if (
-                update <= learning_starts
-                and cfg.checkpoint.resume_from is None
-                and "minedojo" not in cfg.env.wrapper._target_.lower()
-            ):
-                real_actions = actions = np.array(envs.action_space.sample())
-                if not is_continuous:
-                    actions = np.concatenate(
-                        [
-                            F.one_hot(torch.as_tensor(act), act_dim).numpy()
-                            for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
-                        ],
-                        axis=-1,
-                    )
-            else:
-                with torch.no_grad():
-                    preprocessed_obs = {}
-                    for k, v in obs.items():
-                        preprocessed_obs[k] = torch.as_tensor(v[np.newaxis], dtype=torch.float32, device=device)
-                        if k in cfg.algo.cnn_keys.encoder:
-                            preprocessed_obs[k] = preprocessed_obs[k] / 255.0 - 0.5
-                    mask = {k: v for k, v in preprocessed_obs.items() if k.startswith("mask")}
+        with torch.inference_mode():
+            # Measure environment interaction time: this considers both the model forward
+            # to get the action given the observation and the time taken into the environment
+            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
+                # Sample an action given the observation received by the environment
+                if (
+                    update <= learning_starts
+                    and cfg.checkpoint.resume_from is None
+                    and "minedojo" not in cfg.env.wrapper._target_.lower()
+                ):
+                    real_actions = actions = np.array(envs.action_space.sample())
+                    if not is_continuous:
+                        actions = np.concatenate(
+                            [
+                                F.one_hot(torch.as_tensor(act), act_dim).numpy()
+                                for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
+                            ],
+                            axis=-1,
+                        )
+                else:
+                    torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                    mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
-                    real_actions = actions = player.get_exploration_action(preprocessed_obs, mask)
+                    real_actions = actions = player.get_actions(torch_obs, mask=mask)
                     actions = torch.cat(actions, -1).cpu().numpy()
                     if is_continuous:
                         real_actions = torch.cat(real_actions, dim=-1).cpu().numpy()
                     else:
                         real_actions = (
                             torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
 
-            step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
-            rb.add(step_data, validate_args=cfg.buffer.validate_args)
+                step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
+                rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
-            next_obs, rewards, dones, truncated, infos = envs.step(real_actions.reshape(envs.action_space.shape))
-            dones = np.logical_or(dones, truncated).astype(np.uint8)
+                next_obs, rewards, terminated, truncated, infos = envs.step(
+                    real_actions.reshape(envs.action_space.shape)
+                )
+                dones = np.logical_or(terminated, truncated).astype(np.uint8)
 
-        step_data["is_first"] = np.zeros_like(step_data["dones"])
-        if "restart_on_exception" in infos:
-            for i, agent_roe in enumerate(infos["restart_on_exception"]):
-                if agent_roe and not dones[i]:
-                    last_inserted_idx = (rb.buffer[i]._pos - 1) % rb.buffer[i].buffer_size
-                    rb.buffer[i]["dones"][last_inserted_idx] = np.ones_like(rb.buffer[i]["dones"][last_inserted_idx])
-                    rb.buffer[i]["is_first"][last_inserted_idx] = np.zeros_like(
-                        rb.buffer[i]["is_first"][last_inserted_idx]
-                    )
-                    step_data["is_first"][i] = np.ones_like(step_data["is_first"][i])
+            step_data["is_first"] = np.zeros_like(step_data["terminated"])
+            if "restart_on_exception" in infos:
+                for i, agent_roe in enumerate(infos["restart_on_exception"]):
+                    if agent_roe and not dones[i]:
+                        last_inserted_idx = (rb.buffer[i]._pos - 1) % rb.buffer[i].buffer_size
+                        rb.buffer[i]["terminated"][last_inserted_idx] = np.zeros_like(
+                            rb.buffer[i]["terminated"][last_inserted_idx]
+                        )
+                        rb.buffer[i]["truncated"][last_inserted_idx] = np.ones_like(
+                            rb.buffer[i]["truncated"][last_inserted_idx]
+                        )
+                        rb.buffer[i]["is_first"][last_inserted_idx] = np.zeros_like(
+                            rb.buffer[i]["is_first"][last_inserted_idx]
+                        )
+                        step_data["is_first"][i] = np.ones_like(step_data["is_first"][i])
+
+            if cfg.metric.log_level > 0 and "final_info" in infos:
+                for i, agent_ep_info in enumerate(infos["final_info"]):
+                    if agent_ep_info is not None:
+                        ep_rew = agent_ep_info["episode"]["r"]
+                        ep_len = agent_ep_info["episode"]["l"]
+                        if aggregator and not aggregator.disabled:
+                            aggregator.update("Rewards/rew_avg", ep_rew)
+                            aggregator.update("Game/ep_len_avg", ep_len)
+                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+
+            # Save the real next observation
+            real_next_obs = copy.deepcopy(next_obs)
+            if "final_observation" in infos:
+                for idx, final_obs in enumerate(infos["final_observation"]):
+                    if final_obs is not None:
+                        for k, v in final_obs.items():
+                            real_next_obs[k][idx] = v
 
-        if cfg.metric.log_level > 0 and "final_info" in infos:
-            for i, agent_ep_info in enumerate(infos["final_info"]):
-                if agent_ep_info is not None:
-                    ep_rew = agent_ep_info["episode"]["r"]
-                    ep_len = agent_ep_info["episode"]["l"]
-                    if aggregator and not aggregator.disabled:
-                        aggregator.update("Rewards/rew_avg", ep_rew)
-                        aggregator.update("Game/ep_len_avg", ep_len)
-                    fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
-
-        # Save the real next observation
-        real_next_obs = copy.deepcopy(next_obs)
-        if "final_observation" in infos:
-            for idx, final_obs in enumerate(infos["final_observation"]):
-                if final_obs is not None:
-                    for k, v in final_obs.items():
-                        real_next_obs[k][idx] = v
-
-        for k in obs_keys:
-            step_data[k] = next_obs[k][np.newaxis]
-
-        # next_obs becomes the new obs
-        obs = next_obs
-
-        rewards = rewards.reshape((1, cfg.env.num_envs, -1))
-        step_data["dones"] = dones.reshape((1, cfg.env.num_envs, -1))
-        step_data["rewards"] = clip_rewards_fn(rewards)
-
-        dones_idxes = dones.nonzero()[0].tolist()
-        reset_envs = len(dones_idxes)
-        if reset_envs > 0:
-            reset_data = {}
             for k in obs_keys:
-                reset_data[k] = (real_next_obs[k][dones_idxes])[np.newaxis]
-            reset_data["dones"] = np.ones((1, reset_envs, 1))
-            reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
-            reset_data["rewards"] = step_data["rewards"][:, dones_idxes]
-            reset_data["is_first"] = np.zeros_like(reset_data["dones"])
-            rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
-
-            # Reset already inserted step data
-            step_data["rewards"][:, dones_idxes] = np.zeros_like(reset_data["rewards"])
-            step_data["dones"][:, dones_idxes] = np.zeros_like(step_data["dones"][:, dones_idxes])
-            step_data["is_first"][:, dones_idxes] = np.ones_like(step_data["is_first"][:, dones_idxes])
-            player.init_states(dones_idxes)
+                step_data[k] = next_obs[k][np.newaxis]
+
+            # next_obs becomes the new obs
+            obs = next_obs
 
-        updates_before_training -= 1
+            rewards = rewards.reshape((1, cfg.env.num_envs, -1))
+            step_data["terminated"] = terminated.reshape((1, cfg.env.num_envs, -1))
+            step_data["truncated"] = truncated.reshape((1, cfg.env.num_envs, -1))
+            step_data["rewards"] = clip_rewards_fn(rewards)
+
+            dones_idxes = dones.nonzero()[0].tolist()
+            reset_envs = len(dones_idxes)
+            if reset_envs > 0:
+                reset_data = {}
+                for k in obs_keys:
+                    reset_data[k] = (real_next_obs[k][dones_idxes])[np.newaxis]
+                reset_data["terminated"] = step_data["terminated"][:, dones_idxes]
+                reset_data["truncated"] = step_data["truncated"][:, dones_idxes]
+                reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
+                reset_data["rewards"] = step_data["rewards"][:, dones_idxes]
+                reset_data["is_first"] = np.zeros_like(reset_data["terminated"])
+                rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
+
+                # Reset already inserted step data
+                step_data["rewards"][:, dones_idxes] = np.zeros_like(reset_data["rewards"])
+                step_data["terminated"][:, dones_idxes] = np.zeros_like(step_data["terminated"][:, dones_idxes])
+                step_data["truncated"][:, dones_idxes] = np.zeros_like(step_data["truncated"][:, dones_idxes])
+                step_data["is_first"][:, dones_idxes] = np.ones_like(step_data["is_first"][:, dones_idxes])
+                player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts and updates_before_training <= 0:
-            local_data = rb.sample_tensors(
-                cfg.algo.per_rank_batch_size,
-                sequence_length=cfg.algo.per_rank_sequence_length,
-                n_samples=(
-                    cfg.algo.per_rank_pretrain_steps if update == learning_starts else cfg.algo.per_rank_gradient_steps
-                ),
-                dtype=None,
-                device=fabric.device,
-                from_numpy=cfg.buffer.from_numpy,
-            )
-            with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
-                for i in range(next(iter(local_data.values())).shape[0]):
-                    if per_rank_gradient_steps % cfg.algo.critic.target_network_update_freq == 0:
-                        tau = 1 if per_rank_gradient_steps == 0 else cfg.algo.critic.tau
-                        for cp, tcp in zip(critic.module.parameters(), target_critic.parameters()):
-                            tcp.data.copy_(tau * cp.data + (1 - tau) * tcp.data)
-                    batch = {k: v[i].float() for k, v in local_data.items()}
-                    train(
-                        fabric,
-                        world_model,
-                        actor,
-                        critic,
-                        target_critic,
-                        world_optimizer,
-                        actor_optimizer,
-                        critic_optimizer,
-                        batch,
-                        aggregator,
-                        cfg,
-                        is_continuous,
-                        actions_dim,
-                        moments,
-                    )
-                    per_rank_gradient_steps += 1
-                train_step += world_size
-            updates_before_training = cfg.algo.train_every // policy_steps_per_update
-            if cfg.algo.actor.expl_decay:
-                expl_decay_steps += 1
-                actor.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
+        if update >= learning_starts:
+            per_rank_gradient_steps = ratio(policy_step / world_size)
+            if per_rank_gradient_steps > 0:
+                local_data = rb.sample_tensors(
+                    cfg.algo.per_rank_batch_size,
+                    sequence_length=cfg.algo.per_rank_sequence_length,
+                    n_samples=per_rank_gradient_steps,
+                    dtype=None,
+                    device=fabric.device,
+                    from_numpy=cfg.buffer.from_numpy,
                 )
-            if aggregator and not aggregator.disabled:
-                aggregator.update("Params/exploration_amount", actor.expl_amount)
+                with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
+                    for i in range(per_rank_gradient_steps):
+                        if (
+                            cumulative_per_rank_gradient_steps % cfg.algo.critic.per_rank_target_network_update_freq
+                            == 0
+                        ):
+                            tau = 1 if cumulative_per_rank_gradient_steps == 0 else cfg.algo.critic.tau
+                            for cp, tcp in zip(critic.module.parameters(), target_critic.parameters()):
+                                tcp.data.copy_(tau * cp.data + (1 - tau) * tcp.data)
+                        batch = {k: v[i].float() for k, v in local_data.items()}
+                        train(
+                            fabric,
+                            world_model,
+                            actor,
+                            critic,
+                            target_critic,
+                            world_optimizer,
+                            actor_optimizer,
+                            critic_optimizer,
+                            batch,
+                            aggregator,
+                            cfg,
+                            is_continuous,
+                            actions_dim,
+                            moments,
+                        )
+                        cumulative_per_rank_gradient_steps += 1
+                    train_step += world_size
 
         # Log metrics
         if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -757,16 +737,16 @@
                 "world_model": world_model.state_dict(),
                 "actor": actor.state_dict(),
                 "critic": critic.state_dict(),
                 "target_critic": target_critic.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "critic_optimizer": critic_optimizer.state_dict(),
-                "expl_decay_steps": expl_decay_steps,
                 "moments": moments.state_dict(),
+                "ratio": ratio.state_dict(),
                 "update": update * fabric.world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * fabric.world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
@@ -775,15 +755,15 @@
                 ckpt_path=ckpt_path,
                 state=state,
                 replay_buffer=rb if cfg.buffer.checkpoint else None,
             )
 
     envs.close()
     if fabric.is_global_zero and cfg.algo.run_test:
-        test(player, fabric, cfg, log_dir, sample_actions=True)
+        test(player, fabric, cfg, log_dir, greedy=False)
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.dreamer_v1.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
         models_to_log = {
             "world_model": world_model,
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v3/evaluate.py` & `sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/evaluate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from typing import Any, Dict
 
 import gymnasium as gym
 from lightning import Fabric
 
-from sheeprl.algos.dreamer_v3.agent import PlayerDV3, build_agent
-from sheeprl.algos.dreamer_v3.utils import test
+from sheeprl.algos.ppo_recurrent.agent import build_agent
+from sheeprl.algos.ppo_recurrent.utils import test
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.registry import register_evaluation
 
 
-@register_evaluation(algorithms="dreamer_v3")
+@register_evaluation(algorithms="ppo_recurrent")
 def evaluate(fabric: Fabric, cfg: Dict[str, Any], state: Dict[str, Any]):
     logger = get_logger(fabric, cfg)
     if logger and fabric.is_global_zero:
         fabric._loggers = [logger]
         fabric.logger.log_hyperparams(cfg)
     log_dir = get_log_dir(fabric, cfg.root_dir, cfg.run_name)
     fabric.print(f"Log dir: {log_dir}")
@@ -26,43 +26,29 @@
         cfg.seed,
         0,
         log_dir,
         "test",
         vector_env_idx=0,
     )()
     observation_space = env.observation_space
-    action_space = env.action_space
 
     if not isinstance(observation_space, gym.spaces.Dict):
         raise RuntimeError(f"Unexpected observation type, should be of type Dict, got: {observation_space}")
-
+    if cfg.algo.cnn_keys.encoder + cfg.algo.mlp_keys.encoder == []:
+        raise RuntimeError(
+            "You should specify at least one CNN keys or MLP keys from the cli: "
+            "`cnn_keys.encoder=[rgb]` or `mlp_keys.encoder=[state]`"
+        )
     fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
     fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
 
-    is_continuous = isinstance(action_space, gym.spaces.Box)
-    is_multidiscrete = isinstance(action_space, gym.spaces.MultiDiscrete)
+    is_continuous = isinstance(env.action_space, gym.spaces.Box)
+    is_multidiscrete = isinstance(env.action_space, gym.spaces.MultiDiscrete)
     actions_dim = tuple(
-        action_space.shape if is_continuous else (action_space.nvec.tolist() if is_multidiscrete else [action_space.n])
+        env.action_space.shape
+        if is_continuous
+        else (env.action_space.nvec.tolist() if is_multidiscrete else [env.action_space.n])
     )
     # Create the actor and critic models
-    world_model, actor, _, _ = build_agent(
-        fabric,
-        actions_dim,
-        is_continuous,
-        cfg,
-        observation_space,
-        state["world_model"],
-        state["actor"],
-    )
-    player = PlayerDV3(
-        world_model.encoder.module,
-        world_model.rssm,
-        actor.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        discrete_size=cfg.algo.world_model.discrete_size,
-    )
-
-    test(player, fabric, cfg, log_dir, sample_actions=True)
+    _, agent = build_agent(fabric, actions_dim, is_continuous, cfg, observation_space, state["agent"])
+    del _
+    test(agent, fabric, cfg, log_dir)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/dreamer_v3/utils.py` & `sheeprl-0.5.5/sheeprl/algos/dreamer_v3/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     "Loss/observation_loss",
     "Loss/reward_loss",
     "Loss/state_loss",
     "Loss/continue_loss",
     "State/kl",
     "State/post_entropy",
     "State/prior_entropy",
-    "Params/exploration_amount",
     "Grads/world_model",
     "Grads/actor",
     "Grads/critic",
 }
 MODELS_TO_REGISTER = {"world_model", "actor", "critic", "target_critic", "moments"}
 
 
@@ -51,15 +50,15 @@
         self._max = torch.tensor(max_)
         self._percentile_low = percentile_low
         self._percentile_high = percentile_high
         self.register_buffer("low", torch.zeros((), dtype=torch.float32))
         self.register_buffer("high", torch.zeros((), dtype=torch.float32))
 
     def forward(self, x: Tensor, fabric: Fabric) -> Any:
-        gathered_x = fabric.all_gather(x).detach()
+        gathered_x = fabric.all_gather(x).float().detach()
         low = torch.quantile(gathered_x, self._percentile_low)
         high = torch.quantile(gathered_x, self._percentile_high)
         self.low = self._decay * self.low + (1 - self._decay) * low
         self.high = self._decay * self.high + (1 - self._decay) * high
         invscale = torch.max(1 / self._max, self.high - self.low)
         return self.low.detach(), invscale.detach()
 
@@ -74,64 +73,68 @@
     interm = rewards + continues * values * (1 - lmbda)
     for t in reversed(range(len(continues))):
         vals.append(interm[t] + continues[t] * lmbda * vals[-1])
     ret = torch.cat(list(reversed(vals))[:-1])
     return ret
 
 
+def prepare_obs(
+    fabric: Fabric, obs: Dict[str, np.ndarray], *, cnn_keys: Sequence[str] = [], num_envs: int = 1, **kwargs
+) -> Dict[str, Tensor]:
+    torch_obs = {}
+    for k, v in obs.items():
+        torch_obs[k] = torch.from_numpy(v.copy()).to(fabric.device).float()
+        if k in cnn_keys:
+            torch_obs[k] = torch_obs[k].view(1, num_envs, -1, *v.shape[-2:]) / 255 - 0.5
+        else:
+            torch_obs[k] = torch_obs[k].view(1, num_envs, -1)
+
+    return torch_obs
+
+
 @torch.no_grad()
 def test(
     player: "PlayerDV3",
     fabric: Fabric,
     cfg: Dict[str, Any],
     log_dir: str,
     test_name: str = "",
-    sample_actions: bool = False,
+    greedy: bool = True,
 ):
     """Test the model on the environment with the frozen model.
 
     Args:
         player (PlayerDV3): the agent which contains all the models needed to play.
         fabric (Fabric): the fabric instance.
         cfg (DictConfig): the hyper-parameters.
         log_dir (str): the logging directory.
         test_name (str): the name of the test.
             Default to "".
-        sample_actions (bool): whether or not to sample the actions.
-            Default to False.
+        greedy (bool): whether or not to sample the actions.
+            Default to True.
     """
     env: gym.Env = make_env(cfg, cfg.seed, 0, log_dir, "test" + (f"_{test_name}" if test_name != "" else ""))()
     done = False
     cumulative_rew = 0
-    device = fabric.device
-    next_obs = env.reset(seed=cfg.seed)[0]
-    for k in next_obs.keys():
-        next_obs[k] = torch.from_numpy(next_obs[k]).view(1, *next_obs[k].shape).float()
+    obs = env.reset(seed=cfg.seed)[0]
     player.num_envs = 1
     player.init_states()
     while not done:
         # Act greedly through the environment
-        preprocessed_obs = {}
-        for k, v in next_obs.items():
-            if k in cfg.algo.cnn_keys.encoder:
-                preprocessed_obs[k] = v[None, ...].to(device) / 255 - 0.5
-            elif k in cfg.algo.mlp_keys.encoder:
-                preprocessed_obs[k] = v[None, ...].to(device)
-        real_actions = player.get_greedy_action(
-            preprocessed_obs, sample_actions, {k: v for k, v in preprocessed_obs.items() if k.startswith("mask")}
+        torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder)
+        real_actions = player.get_actions(
+            torch_obs, greedy, {k: v for k, v in torch_obs.items() if k.startswith("mask")}
         )
         if player.actor.is_continuous:
             real_actions = torch.cat(real_actions, -1).cpu().numpy()
         else:
             real_actions = torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
 
         # Single environment step
-        next_obs, reward, done, truncated, _ = env.step(real_actions.reshape(env.action_space.shape))
-        for k in next_obs.keys():
-            next_obs[k] = torch.from_numpy(next_obs[k]).view(1, *next_obs[k].shape).float()
+        obs, reward, done, truncated, _ = env.step(real_actions.reshape(env.action_space.shape))
         done = done or truncated or cfg.dry_run
         cumulative_rew += reward
     fabric.print("Test - Reward:", cumulative_rew)
     if cfg.metric.log_level > 0 and len(fabric.loggers) > 0:
         fabric.logger.log_metrics({"Test/cumulative_reward": cumulative_rew}, 0)
     env.close()
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/droq/agent.py` & `sheeprl-0.5.5/sheeprl/algos/droq/agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 import gymnasium
 import torch
 import torch.nn as nn
 from lightning import Fabric
 from lightning.fabric.wrappers import _FabricModule
 from torch import Tensor
 
-from sheeprl.algos.sac.agent import SACActor
+from sheeprl.algos.sac.agent import SACActor, SACPlayer
 from sheeprl.models.models import MLP
+from sheeprl.utils.fabric import get_single_device_fabric
 
 LOG_STD_MAX = 2
 LOG_STD_MIN = -5
 
 
 class DROQCritic(nn.Module):
     def __init__(self, observation_dim: int, hidden_size: int = 256, num_critics: int = 1, dropout: float = 0.0):
@@ -150,14 +151,19 @@
         self._actor = actor
         return
 
     @property
     def qfs_target(self) -> nn.ModuleList:
         return self._qfs_target
 
+    @qfs_target.setter
+    def qfs_target(self, qfs_target: nn.ModuleList) -> None:
+        self._qfs_target = qfs_target
+        return
+
     @property
     def alpha(self) -> float:
         return self._log_alpha.exp().item()
 
     @property
     def target_entropy(self) -> Tensor:
         return self._target_entropy
@@ -205,15 +211,15 @@
 
 def build_agent(
     fabric: Fabric,
     cfg: Dict[str, Any],
     obs_space: gymnasium.spaces.Dict,
     action_space: gymnasium.spaces.Box,
     agent_state: Optional[Dict[str, Tensor]] = None,
-) -> DROQAgent:
+) -> Tuple[DROQAgent, SACPlayer]:
     act_dim = prod(action_space.shape)
     obs_dim = sum([prod(obs_space[k].shape) for k in cfg.algo.mlp_keys.encoder])
     actor = SACActor(
         observation_dim=obs_dim,
         action_dim=act_dim,
         distribution_cfg=cfg.distribution,
         hidden_size=cfg.algo.actor.hidden_size,
@@ -227,15 +233,46 @@
             num_critics=1,
             dropout=cfg.algo.critic.dropout,
         )
         for _ in range(cfg.algo.critic.n)
     ]
     target_entropy = -act_dim
     agent = DROQAgent(
-        actor, critics, target_entropy, alpha=cfg.algo.alpha.alpha, tau=cfg.algo.tau, device=fabric.device
+        actor,
+        critics,
+        target_entropy,
+        alpha=cfg.algo.alpha.alpha,
+        tau=cfg.algo.tau,
+        device=fabric.device,
     )
     if agent_state:
         agent.load_state_dict(agent_state)
+
+    # Setup player agent
+    player = SACPlayer(
+        copy.deepcopy(agent.actor.model),
+        copy.deepcopy(agent.actor.fc_mean),
+        copy.deepcopy(agent.actor.fc_logstd),
+        action_low=action_space.low,
+        action_high=action_space.high,
+    )
+
+    # Setup training agent
     agent.actor = fabric.setup_module(agent.actor)
     agent.critics = [fabric.setup_module(critic) for critic in agent.critics]
 
-    return agent
+    # Wrap the target q-functions with a single-device fabric. This let the target q-functions
+    # to be on the same device as the agent and to run with the same precision
+    fabric_player = get_single_device_fabric(fabric)
+    agent.qfs_target = nn.ModuleList([fabric_player.setup_module(target) for target in agent.qfs_target])
+
+    # Setup player agent
+    player.model = fabric_player.setup_module(player.model)
+    player.fc_mean = fabric_player.setup_module(player.fc_mean)
+    player.fc_logstd = fabric_player.setup_module(player.fc_logstd)
+    player.action_scale = player.action_scale.to(fabric_player.device)
+    player.action_bias = player.action_bias.to(fabric_player.device)
+
+    # Tie weights between the agent and the player
+    for agent_p, player_p in zip(agent.actor.parameters(), player.parameters()):
+        player_p.data = agent_p.data
+    return agent, player
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/droq/droq.py` & `sheeprl-0.5.5/sheeprl/algos/droq/droq.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,44 +14,49 @@
 from torch.optim import Optimizer
 from torch.utils.data.distributed import DistributedSampler
 from torch.utils.data.sampler import BatchSampler
 from torchmetrics import SumMetric
 
 from sheeprl.algos.droq.agent import DROQAgent, build_agent
 from sheeprl.algos.sac.loss import entropy_loss, policy_loss
-from sheeprl.algos.sac.sac import test
+from sheeprl.algos.sac.utils import prepare_obs, test
 from sheeprl.data.buffers import ReplayBuffer
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import save_configs
+from sheeprl.utils.utils import Ratio, save_configs
 
 
 def train(
     fabric: Fabric,
     agent: DROQAgent,
     actor_optimizer: Optimizer,
     qf_optimizer: Optimizer,
     alpha_optimizer: Optimizer,
     rb: ReplayBuffer,
     aggregator: MetricAggregator | None,
     cfg: Dict[str, Any],
+    per_rank_gradient_steps: int,
 ):
     # Sample a minibatch in a distributed way: Line 5 - Algorithm 2
     # We sample one time to reduce the communications between processes
     sample = rb.sample_tensors(
-        cfg.algo.per_rank_gradient_steps * cfg.algo.per_rank_batch_size,
+        per_rank_gradient_steps * cfg.algo.per_rank_batch_size,
         sample_next_obs=cfg.buffer.sample_next_obs,
         from_numpy=cfg.buffer.from_numpy,
     )
-    critic_data = fabric.all_gather(sample)
-    flatten_dim = 3 if fabric.world_size > 1 else 2
-    critic_data = {k: v.view(-1, *v.shape[flatten_dim:]) for k, v in critic_data.items()}
+    critic_data: Dict[str, torch.Tensor] = fabric.all_gather(sample)  # [World, G*B]
+    for k, v in critic_data.items():
+        critic_data[k] = v.float()  # [G*B*World]
+        if fabric.world_size > 1:
+            critic_data[k] = critic_data[k].flatten(start_dim=0, end_dim=2)
+        else:
+            critic_data[k] = critic_data[k].flatten(start_dim=0, end_dim=1)
     critic_idxes = range(len(critic_data[next(iter(critic_data.keys()))]))
     if fabric.world_size > 1:
         dist_sampler: DistributedSampler = DistributedSampler(
             critic_idxes,
             num_replicas=fabric.world_size,
             rank=fabric.global_rank,
             shuffle=True,
@@ -63,15 +68,20 @@
         )
     else:
         critic_sampler = BatchSampler(sampler=critic_idxes, batch_size=cfg.algo.per_rank_batch_size, drop_last=False)
 
     # Sample a different minibatch in a distributed way to update actor and alpha parameter
     sample = rb.sample_tensors(cfg.algo.per_rank_batch_size, from_numpy=cfg.buffer.from_numpy)
     actor_data = fabric.all_gather(sample)
-    actor_data = {k: v.view(-1, *v.shape[flatten_dim:]) for k, v in actor_data.items()}
+    for k, v in actor_data.items():
+        actor_data[k] = v.float()  # [G*B*World]
+        if fabric.world_size > 1:
+            actor_data[k] = actor_data[k].flatten(start_dim=0, end_dim=2)
+        else:
+            actor_data[k] = actor_data[k].flatten(start_dim=0, end_dim=1)
     if fabric.world_size > 1:
         actor_sampler: DistributedSampler = DistributedSampler(
             range(len(actor_data[next(iter(actor_data.keys()))])),
             num_replicas=fabric.world_size,
             rank=fabric.global_rank,
             shuffle=True,
             seed=cfg.seed,
@@ -82,15 +92,15 @@
     with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
         # Update the soft-critic
         for batch_idxes in critic_sampler:
             critic_batch_data = {k: critic_data[k][batch_idxes] for k in critic_data.keys()}
             next_target_qf_value = agent.get_next_target_q_values(
                 critic_batch_data["next_observations"],
                 critic_batch_data["rewards"],
-                critic_batch_data["dones"],
+                critic_batch_data["terminated"],
                 cfg.algo.gamma,
             )
             for qf_value_idx in range(agent.num_critics):
                 # Line 8 - Algorithm 2
                 qf_loss = F.mse_loss(
                     agent.get_ith_q_value(
                         critic_batch_data["observations"], critic_batch_data["actions"], qf_value_idx
@@ -136,16 +146,14 @@
             "in order to play correctly the game. "
             "As an alternative you can use one of the Dreamers' agents."
         )
 
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     # Resume from checkpoint
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     if len(cfg.algo.cnn_keys.encoder) > 0:
         warnings.warn("DroQ algorithm cannot allow to use images as observations, the CNN keys will be ignored")
@@ -189,15 +197,15 @@
                 "Only environments with vector-only observations are supported by the DroQ agent. "
                 f"Provided environment: {cfg.env.id}"
             )
     if cfg.metric.log_level > 0:
         fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
 
     # Define the agent and the optimizer and setup them with Fabric
-    agent = build_agent(
+    agent, player = build_agent(
         fabric, cfg, observation_space, action_space, state["agent"] if cfg.checkpoint.resume_from else None
     )
 
     # Optimizers
     qf_optimizer = hydra.utils.instantiate(cfg.algo.critic.optimizer, params=agent.qfs.parameters(), _convert_="all")
     actor_optimizer = hydra.utils.instantiate(
         cfg.algo.actor.optimizer, params=agent.actor.parameters(), _convert_="all"
@@ -254,14 +262,19 @@
     num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
     learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // fabric.world_size
         if not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -272,29 +285,33 @@
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the checkpoint will be saved at the nearest greater multiple of the "
             "policy_steps_per_update value."
         )
 
     step_data = {}
     # Get the first environment observation and start the optimization
-    o = envs.reset(seed=cfg.seed)[0]
-    obs = np.concatenate([o[k] for k in cfg.algo.mlp_keys.encoder], axis=-1).astype(np.float32)
+    obs = envs.reset(seed=cfg.seed)[0]
 
+    per_rank_gradient_steps = 0
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * fabric.world_size
 
         # Measure environment interaction time: this considers both the model forward
         # to get the action given the observation and the time taken into the environment
         with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            with torch.no_grad():
-                # Sample an action given the observation received by the environment
-                actions, _ = agent.actor.module(torch.from_numpy(obs).to(device))
-                actions = actions.cpu().numpy()
-            next_obs, rewards, dones, truncated, infos = envs.step(actions.reshape(envs.action_space.shape))
-            dones = np.logical_or(dones, truncated)
+            if update <= learning_starts:
+                actions = envs.action_space.sample()
+            else:
+                with torch.inference_mode():
+                    # Sample an action given the observation received by the environment
+                    torch_obs = prepare_obs(fabric, obs, num_envs=cfg.env.num_envs)
+                    actions = player(torch_obs)
+                    actions = actions.cpu().numpy()
+            next_obs, rewards, terminated, truncated, infos = envs.step(actions.reshape(envs.action_space.shape))
 
         if cfg.metric.log_level > 0 and "final_info" in infos:
             for i, agent_ep_info in enumerate(infos["final_info"]):
                 if agent_ep_info is not None:
                     ep_rew = agent_ep_info["episode"]["r"]
                     ep_len = agent_ep_info["episode"]["l"]
                     if aggregator and not aggregator.disabled:
@@ -305,44 +322,63 @@
         # Save the real next observation
         real_next_obs = copy.deepcopy(next_obs)
         if "final_observation" in infos:
             for idx, final_obs in enumerate(infos["final_observation"]):
                 if final_obs is not None:
                     for k, v in final_obs.items():
                         real_next_obs[k][idx] = v
-
-        next_obs = np.concatenate([next_obs[k] for k in cfg.algo.mlp_keys.encoder], axis=-1).astype(np.float32)
         real_next_obs = np.concatenate([real_next_obs[k] for k in cfg.algo.mlp_keys.encoder], axis=-1).astype(
             np.float32
         )
 
-        step_data["observations"] = obs[np.newaxis]
+        step_data["observations"] = np.concatenate([obs[k] for k in cfg.algo.mlp_keys.encoder], axis=-1).astype(
+            np.float32
+        )[np.newaxis]
         if not cfg.buffer.sample_next_obs:
             step_data["next_observations"] = real_next_obs[np.newaxis]
         step_data["actions"] = actions.reshape(1, cfg.env.num_envs, -1)
-        step_data["dones"] = dones.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
+        step_data["terminated"] = terminated.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
+        step_data["truncated"] = truncated.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
         step_data["rewards"] = rewards.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
         rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
         # next_obs becomes the new obs
         obs = next_obs
 
         # Train the agent
-        if update > learning_starts:
-            train(fabric, agent, actor_optimizer, qf_optimizer, alpha_optimizer, rb, aggregator, cfg)
-            train_step += world_size
+        if update >= learning_starts:
+            per_rank_gradient_steps = ratio(policy_step / world_size)
+            if per_rank_gradient_steps > 0:
+                train(
+                    fabric,
+                    agent,
+                    actor_optimizer,
+                    qf_optimizer,
+                    alpha_optimizer,
+                    rb,
+                    aggregator,
+                    cfg,
+                    per_rank_gradient_steps,
+                )
+                train_step += world_size
+                cumulative_per_rank_gradient_steps += per_rank_gradient_steps
 
         # Log metrics
         if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -367,14 +403,15 @@
         ):
             last_checkpoint = policy_step
             state = {
                 "agent": agent.state_dict(),
                 "qf_optimizer": qf_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "alpha_optimizer": alpha_optimizer.state_dict(),
+                "ratio": ratio.state_dict(),
                 "update": update * fabric.world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * fabric.world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call(
@@ -383,15 +420,15 @@
                 ckpt_path=ckpt_path,
                 state=state,
                 replay_buffer=rb if cfg.buffer.checkpoint else None,
             )
 
     envs.close()
     if fabric.is_global_zero and cfg.algo.run_test:
-        test(agent.actor.module, fabric, cfg, log_dir)
+        test(player, fabric, cfg, log_dir)
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.sac.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
         models_to_log = {"agent": agent}
         register_model(fabric, log_models, cfg, models_to_log)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/droq/evaluate.py` & `sheeprl-0.5.5/sheeprl/algos/droq/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,9 +42,10 @@
             raise ValueError(
                 "Only environments with vector-only observations are supported by the DroQ agent. "
                 f"Provided environment: {cfg.env.id}"
             )
     if cfg.metric.log_level > 0:
         fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
 
-    agent = build_agent(fabric, cfg, observation_space, action_space, state["agent"])
-    test(agent.actor, fabric, cfg, log_dir)
+    _, agent = build_agent(fabric, cfg, observation_space, action_space, state["agent"])
+    del _
+    test(agent, fabric, cfg, log_dir)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/droq/utils.py` & `sheeprl-0.5.5/sheeprl/algos/droq/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv1/agent.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv1/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 import hydra
 import torch
 from lightning.fabric import Fabric
 from lightning.fabric.wrappers import _FabricModule
 from lightning.pytorch.utilities.seed import isolate_rng
 from torch import nn
 
-from sheeprl.algos.dreamer_v1.agent import WorldModel
+from sheeprl.algos.dreamer_v1.agent import PlayerDV1, WorldModel
 from sheeprl.algos.dreamer_v1.agent import build_agent as dv1_build_agent
 from sheeprl.algos.dreamer_v2.agent import Actor as DV2Actor
 from sheeprl.algos.dreamer_v2.agent import MinedojoActor as DV2MinedojoActor
 from sheeprl.models.models import MLP
-from sheeprl.utils.utils import init_weights
+from sheeprl.utils.fabric import get_single_device_fabric
+from sheeprl.utils.utils import init_weights, unwrap_fabric
 
 # In order to use the hydra.utils.get_class method, in this way the user can
 # specify in the configs the name of the class without having to know where
 # to go to retrieve the class
 Actor = DV2Actor
 MinedojoActor = DV2MinedojoActor
 
@@ -30,15 +31,15 @@
     obs_space: gymnasium.spaces.Dict,
     world_model_state: Optional[Dict[str, torch.Tensor]] = None,
     ensembles_state: Optional[Dict[str, torch.Tensor]] = None,
     actor_task_state: Optional[Dict[str, torch.Tensor]] = None,
     critic_task_state: Optional[Dict[str, torch.Tensor]] = None,
     actor_exploration_state: Optional[Dict[str, torch.Tensor]] = None,
     critic_exploration_state: Optional[Dict[str, torch.Tensor]] = None,
-) -> Tuple[WorldModel, _FabricModule, _FabricModule, _FabricModule, _FabricModule, _FabricModule]:
+) -> Tuple[WorldModel, nn.ModuleList, _FabricModule, _FabricModule, _FabricModule, _FabricModule, PlayerDV1]:
     """Build the models and wrap them with Fabric.
 
     Args:
         fabric (Fabric): the fabric object.
         actions_dim (Sequence[int]): the dimension of the actions.
         is_continuous (bool): whether or not the actions are continuous.
         cfg (DictConfig): the hyper-parameters of DreamerV1.
@@ -60,51 +61,56 @@
         The world model (WorldModel): composed by the encoder, rssm, observation and
             reward models and the continue model.
         The ensembles (_FabricModule): for estimating the intrinsic reward.
         The actor_task (_FabricModule): for learning the task.
         The critic_task (_FabricModule): for predicting the values of the task.
         The actor_exploration (_FabricModule): for exploring the environment.
         The critic_exploration (_FabricModule): for predicting the values of the exploration.
+        The player (PlayerDV1): the player object.
     """
     world_model_cfg = cfg.algo.world_model
     actor_cfg = cfg.algo.actor
     critic_cfg = cfg.algo.critic
 
     # Sizes
     latent_state_size = world_model_cfg.stochastic_size + world_model_cfg.recurrent_model.recurrent_state_size
 
     # Create exploration models
-    world_model, actor_exploration, critic_exploration = dv1_build_agent(
+    world_model, actor_exploration, critic_exploration, player = dv1_build_agent(
         fabric,
         actions_dim=actions_dim,
         is_continuous=is_continuous,
         cfg=cfg,
         obs_space=obs_space,
         world_model_state=world_model_state,
         actor_state=actor_exploration_state,
         critic_state=critic_exploration_state,
     )
+    player.actor_type = cfg.algo.player.actor_type
     actor_cls = hydra.utils.get_class(cfg.algo.actor.cls)
     actor_task: Union[Actor, MinedojoActor] = actor_cls(
         latent_state_size=latent_state_size,
         actions_dim=actions_dim,
         is_continuous=is_continuous,
         init_std=actor_cfg.init_std,
         min_std=actor_cfg.min_std,
         mlp_layers=actor_cfg.mlp_layers,
         dense_units=actor_cfg.dense_units,
-        activation=eval(actor_cfg.dense_act),
+        activation=hydra.utils.get_class(actor_cfg.dense_act),
         distribution_cfg=cfg.distribution,
         layer_norm=False,
+        expl_amount=actor_cfg.expl_amount,
+        expl_decay=actor_cfg.expl_decay,
+        expl_min=actor_cfg.expl_min,
     )
     critic_task = MLP(
         input_dims=latent_state_size,
         output_dim=1,
         hidden_sizes=[critic_cfg.dense_units] * critic_cfg.mlp_layers,
-        activation=eval(critic_cfg.dense_act),
+        activation=hydra.utils.get_class(critic_cfg.dense_act),
         flatten_dim=None,
     )
     actor_task.apply(init_weights)
     critic_task.apply(init_weights)
 
     # Load task models from checkpoint
     if actor_task_state:
@@ -125,17 +131,25 @@
                     input_dims=(
                         int(sum(actions_dim))
                         + cfg.algo.world_model.recurrent_model.recurrent_state_size
                         + cfg.algo.world_model.stochastic_size
                     ),
                     output_dim=world_model.encoder.cnn_output_dim + world_model.encoder.mlp_output_dim,
                     hidden_sizes=[cfg.algo.ensembles.dense_units] * cfg.algo.ensembles.mlp_layers,
-                    activation=eval(cfg.algo.ensembles.dense_act),
+                    activation=hydra.utils.get_class(cfg.algo.ensembles.dense_act),
                 ).apply(init_weights)
             )
     ensembles = nn.ModuleList(ens_list)
     if ensembles_state:
         ensembles.load_state_dict(ensembles_state)
     for i in range(len(ensembles)):
         ensembles[i] = fabric.setup_module(ensembles[i])
 
-    return world_model, ensembles, actor_task, critic_task, actor_exploration, critic_exploration
+    # Setup player agent
+    if cfg.algo.player.actor_type != "exploration":
+        fabric_player = get_single_device_fabric(fabric)
+        player_actor = unwrap_fabric(actor_task)
+        player.actor = fabric_player.setup_module(player_actor)
+        for agent_p, p in zip(actor_task.parameters(), player.actor.parameters()):
+            p.data = agent_p.data
+
+    return world_model, ensembles, actor_task, critic_task, actor_exploration, critic_exploration, player
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv1/evaluate.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv1/evaluate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Dict
 
 import gymnasium as gym
 from lightning import Fabric
 
-from sheeprl.algos.dreamer_v1.agent import PlayerDV1
 from sheeprl.algos.dreamer_v2.utils import test
 from sheeprl.algos.p2e_dv1.agent import build_agent
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.registry import register_evaluation
 
 
@@ -41,29 +40,19 @@
 
     is_continuous = isinstance(action_space, gym.spaces.Box)
     is_multidiscrete = isinstance(action_space, gym.spaces.MultiDiscrete)
     actions_dim = tuple(
         action_space.shape if is_continuous else (action_space.nvec.tolist() if is_multidiscrete else [action_space.n])
     )
     # Create the actor and critic models
-    world_model, _, actor_task, _, _, _ = build_agent(
+    cfg.algo.player.actor_type = "task"
+    _, _, _, _, _, _, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
-        state["world_model"],
-        state["actor_task"],
+        world_model_state=state["world_model"],
+        actor_task_state=state["actor_task"],
     )
-    player = PlayerDV1(
-        world_model.encoder.module,
-        world_model.rssm.recurrent_model.module,
-        world_model.rssm.representation_model.module,
-        actor_task.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-    )
-
-    test(player, fabric, cfg, log_dir, sample_actions=False)
+    del _
+    test(player, fabric, cfg, log_dir, greedy=True)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 from lightning.fabric import Fabric
 from lightning.fabric.wrappers import _FabricModule, _FabricOptimizer
 from torch import Tensor
 from torch.distributions import Bernoulli, Independent, Normal
 from torch.distributions.utils import logits_to_probs
 from torchmetrics import SumMetric
 
-from sheeprl.algos.dreamer_v1.agent import PlayerDV1, WorldModel
+from sheeprl.algos.dreamer_v1.agent import WorldModel
 from sheeprl.algos.dreamer_v1.loss import actor_loss, critic_loss, reconstruction_loss
 from sheeprl.algos.dreamer_v1.utils import compute_lambda_values
-from sheeprl.algos.dreamer_v2.utils import test
+from sheeprl.algos.dreamer_v2.utils import prepare_obs, test
 from sheeprl.algos.p2e_dv1.agent import build_agent
 from sheeprl.data.buffers import EnvIndependentReplayBuffer, SequentialReplayBuffer
 from sheeprl.utils.env import make_env
+from sheeprl.utils.fabric import get_single_device_fabric
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import polynomial_decay, save_configs
+from sheeprl.utils.utils import Ratio, save_configs, unwrap_fabric
 
 # Decomment the following line if you are using MineDojo on an headless machine
 # os.environ["MINEDOJO_HEADLESS"] = "1"
 
 
 def train(
     fabric: Fabric,
@@ -93,15 +94,14 @@
         actor_exploration (_FabricModule): the actor for exploration.
         critic_exploration (_FabricModule): the critic for exploration.
         actor_exploration_optimizer (_FabricOptimizer): the optimizer of the actor for exploration.
         critic_exploration_optimizer (_FabricOptimizer): the optimizer of the critic for exploration.
     """
     batch_size = cfg.algo.per_rank_batch_size
     sequence_length = cfg.algo.per_rank_sequence_length
-    validate_args = cfg.distribution.validate_args
     recurrent_state_size = cfg.algo.world_model.recurrent_model.recurrent_state_size
     stochastic_size = cfg.algo.world_model.stochastic_size
     device = fabric.device
     batch_obs = {k: data[k] / 255 - 0.5 for k in cfg.algo.cnn_keys.encoder}
     batch_obs.update({k: data[k] for k in cfg.algo.mlp_keys.encoder})
 
     # Dynamic Learning
@@ -126,53 +126,36 @@
         posteriors_std[i] = posterior_mean_std[1]
         priors_mean[i] = prior_mean_std[0]
         priors_std[i] = prior_mean_std[1]
         priors[i] = prior
     latent_states = torch.cat((posteriors, recurrent_states), -1)
 
     decoded_information: Dict[str, torch.Tensor] = world_model.observation_model(latent_states)
-    qo = {
-        k: Independent(
-            Normal(rec_obs, 1, validate_args=validate_args), len(rec_obs.shape[2:]), validate_args=validate_args
-        )
-        for k, rec_obs in decoded_information.items()
-    }
-    qr = Independent(
-        Normal(world_model.reward_model(latent_states.detach()), 1, validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
+    qo = {k: Independent(Normal(rec_obs, 1), len(rec_obs.shape[2:])) for k, rec_obs in decoded_information.items()}
+    qr = Independent(Normal(world_model.reward_model(latent_states.detach()), 1), 1)
     if cfg.algo.world_model.use_continues and world_model.continue_model:
-        qc = Independent(
-            Bernoulli(logits=world_model.continue_model(latent_states.detach()), validate_args=validate_args),
-            1,
-            validate_args=validate_args,
-        )
-        continue_targets = (1 - data["dones"]) * cfg.algo.gamma
+        qc = Independent(Bernoulli(logits=world_model.continue_model(latent_states.detach())), 1)
+        continues_targets = (1 - data["terminated"]) * cfg.algo.gamma
     else:
-        qc = continue_targets = None
-    posteriors_dist = Independent(
-        Normal(posteriors_mean, posteriors_std, validate_args=validate_args), 1, validate_args=validate_args
-    )
-    priors_dist = Independent(
-        Normal(priors_mean, priors_std, validate_args=validate_args), 1, validate_args=validate_args
-    )
+        qc = continues_targets = None
+    posteriors_dist = Independent(Normal(posteriors_mean, posteriors_std), 1)
+    priors_dist = Independent(Normal(priors_mean, priors_std), 1)
 
     world_optimizer.zero_grad(set_to_none=True)
     rec_loss, kl, state_loss, reward_loss, observation_loss, continue_loss = reconstruction_loss(
         qo,
         batch_obs,
         qr,
         data["rewards"],
         posteriors_dist,
         priors_dist,
         cfg.algo.world_model.kl_free_nats,
         cfg.algo.world_model.kl_regularizer,
         qc,
-        continue_targets,
+        continues_targets,
         cfg.algo.world_model.continue_scale_factor,
     )
     fabric.backward(rec_loss)
     world_grad = None
     if cfg.algo.world_model.clip_gradients is not None and cfg.algo.world_model.clip_gradients > 0:
         world_grad = fabric.clip_gradients(
             module=world_model,
@@ -183,17 +166,15 @@
     world_optimizer.step()
 
     # Ensemble Learning
     loss = 0.0
     ensemble_optimizer.zero_grad(set_to_none=True)
     for ens in ensembles:
         out = ens(torch.cat((posteriors.detach(), recurrent_states.detach(), data["actions"].detach()), -1))[:-1]
-        next_obs_embedding_dist = Independent(
-            Normal(out, 1, validate_args=validate_args), 1, validate_args=validate_args
-        )
+        next_obs_embedding_dist = Independent(Normal(out, 1), 1)
         loss -= next_obs_embedding_dist.log_prob(embedded_obs.detach()[1:]).mean()
     loss.backward()
     ensemble_grad = None
     if cfg.algo.ensembles.clip_gradients is not None and cfg.algo.ensembles.clip_gradients > 0:
         ensemble_grad = fabric.clip_gradients(
             module=ens,
             optimizer=ensemble_optimizer,
@@ -263,19 +244,15 @@
             module=actor_exploration,
             optimizer=actor_exploration_optimizer,
             max_norm=cfg.algo.actor.clip_gradients,
             error_if_nonfinite=False,
         )
     actor_exploration_optimizer.step()
 
-    qv = Independent(
-        Normal(critic_exploration(imagined_trajectories.detach())[:-1], 1, validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
+    qv = Independent(Normal(critic_exploration(imagined_trajectories.detach())[:-1], 1), 1)
     critic_exploration_optimizer.zero_grad(set_to_none=True)
     value_loss_exploration = critic_loss(qv, lambda_values_exploration.detach(), discount[..., 0])
     fabric.backward(value_loss_exploration)
     critic_exploration_grad = None
     if cfg.algo.critic.clip_gradients is not None and cfg.algo.critic.clip_gradients > 0:
         critic_exploration_grad = fabric.clip_gradients(
             module=critic_exploration,
@@ -329,19 +306,15 @@
             module=actor_task,
             optimizer=actor_task_optimizer,
             max_norm=cfg.algo.actor.clip_gradients,
             error_if_nonfinite=False,
         )
     actor_task_optimizer.step()
 
-    qv = Independent(
-        Normal(critic_task(imagined_trajectories.detach())[:-1], 1, validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
+    qv = Independent(Normal(critic_task(imagined_trajectories.detach())[:-1], 1), 1)
     critic_task_optimizer.zero_grad(set_to_none=True)
     value_loss_task = critic_loss(qv, lambda_values_task.detach(), discount[..., 0])
     fabric.backward(value_loss_task)
     critic_task_grad = None
     if cfg.algo.critic.clip_gradients is not None and cfg.algo.critic.clip_gradients > 0:
         critic_task_grad = fabric.clip_gradients(
             module=critic_task,
@@ -390,16 +363,14 @@
 
 
 @register_algorithm()
 def main(fabric: Fabric, cfg: Dict[str, Any]):
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     # These arguments cannot be changed
     cfg.env.screen_size = 64
     cfg.env.frame_stack = 1
@@ -458,41 +429,28 @@
     if cfg.metric.log_level > 0:
         fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
         fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
         fabric.print("Decoder CNN keys:", cfg.algo.cnn_keys.decoder)
         fabric.print("Decoder MLP keys:", cfg.algo.mlp_keys.decoder)
     obs_keys = cfg.algo.cnn_keys.encoder + cfg.algo.mlp_keys.encoder
 
-    world_model, ensembles, actor_task, critic_task, actor_exploration, critic_exploration = build_agent(
+    world_model, ensembles, actor_task, critic_task, actor_exploration, critic_exploration, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["world_model"] if cfg.checkpoint.resume_from else None,
         state["ensembles"] if cfg.checkpoint.resume_from else None,
         state["actor_task"] if cfg.checkpoint.resume_from else None,
         state["critic_task"] if cfg.checkpoint.resume_from else None,
         state["actor_exploration"] if cfg.checkpoint.resume_from else None,
         state["critic_exploration"] if cfg.checkpoint.resume_from else None,
     )
 
-    player = PlayerDV1(
-        world_model.encoder.module,
-        world_model.rssm.recurrent_model.module,
-        world_model.rssm.representation_model.module,
-        actor_exploration.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        actor_type=cfg.algo.player.actor_type,
-    )
-
     # Optimizers
     world_optimizer = hydra.utils.instantiate(
         cfg.algo.world_model.optimizer, params=world_model.parameters(), _convert_="all"
     )
     actor_task_optimizer = hydra.utils.instantiate(
         cfg.algo.actor.optimizer, params=actor_task.parameters(), _convert_="all"
     )
@@ -554,15 +512,14 @@
         if isinstance(state["rb"], list) and world_size == len(state["rb"]):
             rb = state["rb"][fabric.global_rank]
         elif isinstance(state["rb"], EnvIndependentReplayBuffer):
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
     step_data = {}
-    expl_decay_steps = state["expl_decay_steps"] if cfg.checkpoint.resume_from else 0
 
     # Global variables
     train_step = 0
     last_train = 0
     start_step = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
@@ -571,35 +528,26 @@
         if cfg.checkpoint.resume_from
         else 1
     )
     policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
     policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    updates_before_training = cfg.algo.train_every // policy_steps_per_update if not cfg.dry_run else 0
     num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
     learning_starts = (cfg.algo.learning_starts // policy_steps_per_update) if not cfg.dry_run else 0
-    max_step_expl_decay = cfg.algo.actor.max_step_expl_decay // (cfg.algo.per_rank_gradient_steps * world_size)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        actor_task.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
-        actor_exploration.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
         if not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -615,174 +563,168 @@
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         if k in cfg.algo.cnn_keys.encoder:
             obs[k] = obs[k].reshape(cfg.env.num_envs, -1, *obs[k].shape[-2:])
         step_data[k] = obs[k][np.newaxis]
-    step_data["dones"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
 
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * world_size
 
-        # Measure environment interaction time: this considers both the model forward
-        # to get the action given the observation and the time taken into the environment
-        with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            # Sample an action given the observation received by the environment
-            if (
-                update <= learning_starts
-                and cfg.checkpoint.resume_from is None
-                and "minedojo" not in cfg.env.wrapper._target_.lower()
-            ):
-                real_actions = actions = np.array(envs.action_space.sample())
-                if not is_continuous:
-                    actions = np.concatenate(
-                        [
-                            F.one_hot(torch.as_tensor(act), act_dim).numpy()
-                            for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
-                        ],
-                        axis=-1,
-                    )
-            else:
-                with torch.no_grad():
-                    normalized_obs = {}
-                    for k in obs_keys:
-                        torch_obs = torch.as_tensor(obs[k][np.newaxis], dtype=torch.float32, device=device)
-                        if k in cfg.algo.cnn_keys.encoder:
-                            torch_obs = torch_obs / 255 - 0.5
-                        normalized_obs[k] = torch_obs
-                    mask = {k: v for k, v in normalized_obs.items() if k.startswith("mask")}
+        with torch.inference_mode():
+            # Measure environment interaction time: this considers both the model forward
+            # to get the action given the observation and the time taken into the environment
+            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
+                # Sample an action given the observation received by the environment
+                if (
+                    update <= learning_starts
+                    and cfg.checkpoint.resume_from is None
+                    and "minedojo" not in cfg.env.wrapper._target_.lower()
+                ):
+                    real_actions = actions = np.array(envs.action_space.sample())
+                    if not is_continuous:
+                        actions = np.concatenate(
+                            [
+                                F.one_hot(torch.as_tensor(act), act_dim).numpy()
+                                for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
+                            ],
+                            axis=-1,
+                        )
+                else:
+                    torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                    mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
-                    real_actions = actions = player.get_exploration_action(normalized_obs, mask)
+                    real_actions = actions = player.get_exploration_actions(torch_obs, mask=mask, step=policy_step)
                     actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                     if is_continuous:
                         real_actions = torch.cat(real_actions, -1).cpu().numpy()
                     else:
                         real_actions = (
                             torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
-            next_obs, rewards, dones, truncated, infos = envs.step(real_actions.reshape(envs.action_space.shape))
-            dones = np.logical_or(dones, truncated).astype(np.uint8)
+                next_obs, rewards, terminated, truncated, infos = envs.step(
+                    real_actions.reshape(envs.action_space.shape)
+                )
+                dones = np.logical_or(terminated, truncated).astype(np.uint8)
 
-        if cfg.metric.log_level > 0 and "final_info" in infos:
-            for i, agent_ep_info in enumerate(infos["final_info"]):
-                if agent_ep_info is not None:
-                    ep_rew = agent_ep_info["episode"]["r"]
-                    ep_len = agent_ep_info["episode"]["l"]
-                    if aggregator and not aggregator.disabled:
-                        aggregator.update("Rewards/rew_avg", ep_rew)
-                        aggregator.update("Game/ep_len_avg", ep_len)
-                    fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
-
-        # Save the real next observation
-        real_next_obs = copy.deepcopy(next_obs)
-        if "final_observation" in infos:
-            for idx, final_obs in enumerate(infos["final_observation"]):
-                if final_obs is not None:
-                    for k, v in final_obs.items():
-                        real_next_obs[k][idx] = v
-
-        for k in obs_keys:
-            if k in cfg.algo.cnn_keys.encoder:
-                next_obs[k] = next_obs[k].reshape(cfg.env.num_envs, -1, *next_obs[k].shape[-2:])
-                real_next_obs[k] = real_next_obs[k].reshape(cfg.env.num_envs, -1, *real_next_obs[k].shape[-2:])
-            step_data[k] = real_next_obs[k][np.newaxis]
-
-        # next_obs becomes the new obs
-        obs = next_obs
-
-        step_data["dones"] = dones[np.newaxis]
-        step_data["actions"] = actions[np.newaxis]
-        step_data["rewards"] = clip_rewards_fn(rewards)[np.newaxis]
-        rb.add(step_data, validate_args=cfg.buffer.validate_args)
-
-        # Reset and save the observation coming from the automatic reset
-        dones_idxes = dones.nonzero()[0].tolist()
-        reset_envs = len(dones_idxes)
-        if reset_envs > 0:
-            reset_data = {}
-            for k in obs_keys:
-                reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
-            reset_data["dones"] = np.zeros((1, reset_envs, 1))
-            reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
-            reset_data["rewards"] = np.zeros((1, reset_envs, 1))
-            rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
-            # Reset dones so that `is_first` is updated
-            for d in dones_idxes:
-                step_data["dones"][0, d] = np.zeros_like(step_data["dones"][0, d])
-            # Reset internal agent states
-            player.init_states(reset_envs=dones_idxes)
+            if cfg.metric.log_level > 0 and "final_info" in infos:
+                for i, agent_ep_info in enumerate(infos["final_info"]):
+                    if agent_ep_info is not None:
+                        ep_rew = agent_ep_info["episode"]["r"]
+                        ep_len = agent_ep_info["episode"]["l"]
+                        if aggregator and not aggregator.disabled:
+                            aggregator.update("Rewards/rew_avg", ep_rew)
+                            aggregator.update("Game/ep_len_avg", ep_len)
+                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+
+            # Save the real next observation
+            real_next_obs = copy.deepcopy(next_obs)
+            if "final_observation" in infos:
+                for idx, final_obs in enumerate(infos["final_observation"]):
+                    if final_obs is not None:
+                        for k, v in final_obs.items():
+                            real_next_obs[k][idx] = v
 
-        updates_before_training -= 1
+            for k in obs_keys:
+                if k in cfg.algo.cnn_keys.encoder:
+                    next_obs[k] = next_obs[k].reshape(cfg.env.num_envs, -1, *next_obs[k].shape[-2:])
+                    real_next_obs[k] = real_next_obs[k].reshape(cfg.env.num_envs, -1, *real_next_obs[k].shape[-2:])
+                step_data[k] = real_next_obs[k][np.newaxis]
+
+            # next_obs becomes the new obs
+            obs = next_obs
+
+            step_data["terminated"] = terminated[np.newaxis]
+            step_data["truncated"] = truncated[np.newaxis]
+            step_data["actions"] = actions[np.newaxis]
+            step_data["rewards"] = clip_rewards_fn(rewards)[np.newaxis]
+            rb.add(step_data, validate_args=cfg.buffer.validate_args)
+
+            # Reset and save the observation coming from the automatic reset
+            dones_idxes = dones.nonzero()[0].tolist()
+            reset_envs = len(dones_idxes)
+            if reset_envs > 0:
+                reset_data = {}
+                for k in obs_keys:
+                    reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
+                reset_data["terminated"] = np.zeros((1, reset_envs, 1))
+                reset_data["truncated"] = np.zeros((1, reset_envs, 1))
+                reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
+                reset_data["rewards"] = np.zeros((1, reset_envs, 1))
+                rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
+                for d in dones_idxes:
+                    step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
+                    step_data["truncated"][0, d] = np.zeros_like(step_data["truncated"][0, d])
+                # Reset internal agent states
+                player.init_states(reset_envs=dones_idxes)
 
         # Train the agent
-        if update >= learning_starts and updates_before_training <= 0:
-            # Start training
-            with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
-                for i in range(cfg.algo.per_rank_gradient_steps):
+        if update >= learning_starts:
+            per_rank_gradient_steps = ratio(policy_step / world_size)
+            if per_rank_gradient_steps > 0:
+                with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
                     sample = rb.sample_tensors(
                         batch_size=cfg.algo.per_rank_batch_size,
                         sequence_length=cfg.algo.per_rank_sequence_length,
-                        n_samples=1,
+                        n_samples=per_rank_gradient_steps,
                         dtype=None,
                         device=device,
                         from_numpy=cfg.buffer.from_numpy,
                     )  # [N_samples, Seq_len, Batch_size, ...]
-                    batch = {k: v[0].float() for k, v in sample.items()}
-                    train(
-                        fabric,
-                        world_model,
-                        actor_task,
-                        critic_task,
-                        world_optimizer,
-                        actor_task_optimizer,
-                        critic_task_optimizer,
-                        batch,
-                        aggregator,
-                        cfg,
-                        ensembles=ensembles,
-                        ensemble_optimizer=ensemble_optimizer,
-                        actor_exploration=actor_exploration,
-                        critic_exploration=critic_exploration,
-                        actor_exploration_optimizer=actor_exploration_optimizer,
-                        critic_exploration_optimizer=critic_exploration_optimizer,
+                    for i in range(per_rank_gradient_steps):
+                        batch = {k: v[i].float() for k, v in sample.items()}
+                        train(
+                            fabric,
+                            world_model,
+                            actor_task,
+                            critic_task,
+                            world_optimizer,
+                            actor_task_optimizer,
+                            critic_task_optimizer,
+                            batch,
+                            aggregator,
+                            cfg,
+                            ensembles=ensembles,
+                            ensemble_optimizer=ensemble_optimizer,
+                            actor_exploration=actor_exploration,
+                            critic_exploration=critic_exploration,
+                            actor_exploration_optimizer=actor_exploration_optimizer,
+                            critic_exploration_optimizer=critic_exploration_optimizer,
+                        )
+                        cumulative_per_rank_gradient_steps += 1
+                    train_step += world_size
+
+                if aggregator and not aggregator.disabled:
+                    aggregator.update("Params/exploration_amount_task", actor_task._get_expl_amount(policy_step))
+                    aggregator.update(
+                        "Params/exploration_amount_exploration", actor_exploration._get_expl_amount(policy_step)
                     )
-                train_step += world_size
-            updates_before_training = cfg.algo.train_every // policy_steps_per_update
-            if cfg.algo.actor.expl_decay:
-                expl_decay_steps += 1
-                actor_task.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
-                )
-                actor_exploration.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
-                )
-            if aggregator and not aggregator.disabled:
-                aggregator.update("Params/exploration_amount_task", actor_task.expl_amount)
-                aggregator.update("Params/exploration_amount_exploration", actor_exploration.expl_amount)
 
         # Log metrics
         if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -811,15 +753,15 @@
                 "actor_task": actor_task.state_dict(),
                 "critic_task": critic_task.state_dict(),
                 "ensembles": ensembles.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
                 "ensemble_optimizer": ensemble_optimizer.state_dict(),
-                "expl_decay_steps": expl_decay_steps,
+                "ratio": ratio.state_dict(),
                 "update": update * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "critic_exploration": critic_exploration.state_dict(),
                 "actor_exploration_optimizer": actor_exploration_optimizer.state_dict(),
                 "critic_exploration_optimizer": critic_exploration_optimizer.state_dict(),
                 "last_log": last_log,
@@ -833,16 +775,17 @@
                 state=state,
                 replay_buffer=rb if cfg.buffer.checkpoint else None,
             )
 
     envs.close()
     # task test zero-shot
     if fabric.is_global_zero and cfg.algo.run_test:
-        player.actor = actor_task.module
         player.actor_type = "task"
+        fabric_player = get_single_device_fabric(fabric)
+        player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
         test(player, fabric, cfg, log_dir, "zero-shot")
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.dreamer_v1.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
         models_to_log = {
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,37 +9,38 @@
 import gymnasium as gym
 import hydra
 import numpy as np
 import torch
 from lightning.fabric import Fabric
 from torchmetrics import SumMetric
 
-from sheeprl.algos.dreamer_v1.agent import PlayerDV1
 from sheeprl.algos.dreamer_v1.dreamer_v1 import train
-from sheeprl.algos.dreamer_v2.utils import test
+from sheeprl.algos.dreamer_v2.utils import prepare_obs, test
 from sheeprl.algos.p2e_dv1.agent import build_agent
 from sheeprl.data.buffers import EnvIndependentReplayBuffer, SequentialReplayBuffer
 from sheeprl.utils.env import make_env
+from sheeprl.utils.fabric import get_single_device_fabric
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import polynomial_decay, save_configs
+from sheeprl.utils.utils import Ratio, save_configs, unwrap_fabric
 
 # Decomment the following line if you are using MineDojo on an headless machine
 # os.environ["MINEDOJO_HEADLESS"] = "1"
 
 
 @register_algorithm()
 def main(fabric: Fabric, cfg: Dict[str, Any], exploration_cfg: Dict[str, Any]):
+    # Single-device fabric object
+    fabric_player = get_single_device_fabric(fabric)
+
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     ckpt_path = pathlib.Path(cfg.checkpoint.exploration_ckpt_path)
     resume_from_checkpoint = cfg.checkpoint.resume_from is not None
     # Finetuning that was interrupted for some reason
     if resume_from_checkpoint:
         state = fabric.load(pathlib.Path(cfg.checkpoint.resume_from))
     else:
@@ -127,40 +128,27 @@
     if cfg.metric.log_level > 0:
         fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
         fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
         fabric.print("Decoder CNN keys:", cfg.algo.cnn_keys.decoder)
         fabric.print("Decoder MLP keys:", cfg.algo.mlp_keys.decoder)
     obs_keys = cfg.algo.cnn_keys.encoder + cfg.algo.mlp_keys.encoder
 
-    world_model, _, actor_task, critic_task, actor_exploration, _ = build_agent(
+    world_model, _, actor_task, critic_task, actor_exploration, _, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["world_model"],
         None,
         state["actor_task"],
         state["critic_task"],
         state["actor_exploration"],
     )
 
-    player = PlayerDV1(
-        world_model.encoder.module,
-        world_model.rssm.recurrent_model.module,
-        world_model.rssm.representation_model.module,
-        actor_exploration.module if cfg.algo.player.actor_type == "exploration" else actor_task.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        actor_type=cfg.algo.player.actor_type,
-    )
-
     # Optimizers
     world_optimizer = hydra.utils.instantiate(
         cfg.algo.world_model.optimizer, params=world_model.parameters(), _convert_="all"
     )
     actor_task_optimizer = hydra.utils.instantiate(
         cfg.algo.actor.optimizer, params=actor_task.parameters(), _convert_="all"
     )
@@ -195,15 +183,14 @@
     if resume_from_checkpoint or (cfg.buffer.load_from_exploration and exploration_cfg.buffer.checkpoint):
         if isinstance(state["rb"], list) and world_size == len(state["rb"]):
             rb = state["rb"][fabric.global_rank]
         elif isinstance(state["rb"], EnvIndependentReplayBuffer):
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
-    expl_decay_steps = state["expl_decay_steps"] if resume_from_checkpoint else 0
 
     # Global variables
     train_step = 0
     last_train = 0
     start_step = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
@@ -212,35 +199,26 @@
         if resume_from_checkpoint
         else 1
     )
     policy_step = state["update"] * cfg.env.num_envs if resume_from_checkpoint else 0
     last_log = state["last_log"] if resume_from_checkpoint else 0
     last_checkpoint = state["last_checkpoint"] if resume_from_checkpoint else 0
     policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    updates_before_training = cfg.algo.train_every // policy_steps_per_update if not cfg.dry_run else 0
     num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
     learning_starts = (cfg.algo.learning_starts // policy_steps_per_update) if not cfg.dry_run else 0
-    max_step_expl_decay = cfg.algo.actor.max_step_expl_decay // (cfg.algo.per_rank_gradient_steps * world_size)
     if resume_from_checkpoint:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        actor_task.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
-        actor_exploration.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
         if resume_from_checkpoint and not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -256,155 +234,150 @@
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         if k in cfg.algo.cnn_keys.encoder:
             obs[k] = obs[k].reshape(cfg.env.num_envs, -1, *obs[k].shape[-2:])
         step_data[k] = obs[k][np.newaxis]
-    step_data["dones"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
     rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
-    player.init_states()
 
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * world_size
 
-        # Measure environment interaction time: this considers both the model forward
-        # to get the action given the observation and the time taken into the environment
-        with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            with torch.no_grad():
-                normalized_obs = {}
-                for k in obs_keys:
-                    torch_obs = torch.as_tensor(obs[k][np.newaxis], dtype=torch.float32, device=device)
-                    if k in cfg.algo.cnn_keys.encoder:
-                        torch_obs = torch_obs / 255 - 0.5
-                    normalized_obs[k] = torch_obs
-                mask = {k: v for k, v in normalized_obs.items() if k.startswith("mask")}
+        with torch.inference_mode():
+            # Measure environment interaction time: this considers both the model forward
+            # to get the action given the observation and the time taken into the environment
+            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
+                torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                 if len(mask) == 0:
                     mask = None
-                real_actions = actions = player.get_exploration_action(normalized_obs, mask)
+                real_actions = actions = player.get_exploration_actions(torch_obs, mask=mask, step=policy_step)
                 actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                 if is_continuous:
                     real_actions = torch.cat(real_actions, -1).cpu().numpy()
                 else:
                     real_actions = (
                         torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                     )
-            next_obs, rewards, dones, truncated, infos = envs.step(real_actions.reshape(envs.action_space.shape))
-            dones = np.logical_or(dones, truncated).astype(np.uint8)
+                next_obs, rewards, terminated, truncated, infos = envs.step(
+                    real_actions.reshape(envs.action_space.shape)
+                )
+                dones = np.logical_or(terminated, truncated).astype(np.uint8)
 
-        if cfg.metric.log_level > 0 and "final_info" in infos:
-            for i, agent_ep_info in enumerate(infos["final_info"]):
-                if agent_ep_info is not None:
-                    ep_rew = agent_ep_info["episode"]["r"]
-                    ep_len = agent_ep_info["episode"]["l"]
-                    if aggregator and not aggregator.disabled:
-                        aggregator.update("Rewards/rew_avg", ep_rew)
-                        aggregator.update("Game/ep_len_avg", ep_len)
-                    fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
-
-        # Save the real next observation
-        real_next_obs = copy.deepcopy(next_obs)
-        if "final_observation" in infos:
-            for idx, final_obs in enumerate(infos["final_observation"]):
-                if final_obs is not None:
-                    for k, v in final_obs.items():
-                        real_next_obs[k][idx] = v
-
-        for k in obs_keys:
-            if k in cfg.algo.cnn_keys.encoder:
-                next_obs[k] = next_obs[k].reshape(cfg.env.num_envs, -1, *next_obs[k].shape[-2:])
-                real_next_obs[k] = real_next_obs[k].reshape(cfg.env.num_envs, -1, *real_next_obs[k].shape[-2:])
-            step_data[k] = real_next_obs[k][np.newaxis]
-
-        # next_obs becomes the new obs
-        obs = next_obs
-
-        step_data["dones"] = dones[np.newaxis]
-        step_data["actions"] = actions[np.newaxis]
-        step_data["rewards"] = clip_rewards_fn(rewards)[np.newaxis]
-        rb.add(step_data, validate_args=cfg.buffer.validate_args)
-
-        # Reset and save the observation coming from the automatic reset
-        dones_idxes = dones.nonzero()[0].tolist()
-        reset_envs = len(dones_idxes)
-        if reset_envs > 0:
-            reset_data = {}
-            for k in obs_keys:
-                reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
-            reset_data["dones"] = np.zeros((1, reset_envs, 1))
-            reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
-            reset_data["rewards"] = np.zeros((1, reset_envs, 1))
-            rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
-            # Reset dones so that `is_first` is updated
-            for d in dones_idxes:
-                step_data["dones"][0, d] = np.zeros_like(step_data["dones"][0, d])
-            # Reset internal agent states
-            player.init_states(reset_envs=dones_idxes)
+            if cfg.metric.log_level > 0 and "final_info" in infos:
+                for i, agent_ep_info in enumerate(infos["final_info"]):
+                    if agent_ep_info is not None:
+                        ep_rew = agent_ep_info["episode"]["r"]
+                        ep_len = agent_ep_info["episode"]["l"]
+                        if aggregator and not aggregator.disabled:
+                            aggregator.update("Rewards/rew_avg", ep_rew)
+                            aggregator.update("Game/ep_len_avg", ep_len)
+                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+
+            # Save the real next observation
+            real_next_obs = copy.deepcopy(next_obs)
+            if "final_observation" in infos:
+                for idx, final_obs in enumerate(infos["final_observation"]):
+                    if final_obs is not None:
+                        for k, v in final_obs.items():
+                            real_next_obs[k][idx] = v
 
-        updates_before_training -= 1
+            for k in obs_keys:
+                if k in cfg.algo.cnn_keys.encoder:
+                    next_obs[k] = next_obs[k].reshape(cfg.env.num_envs, -1, *next_obs[k].shape[-2:])
+                    real_next_obs[k] = real_next_obs[k].reshape(cfg.env.num_envs, -1, *real_next_obs[k].shape[-2:])
+                step_data[k] = real_next_obs[k][np.newaxis]
+
+            # next_obs becomes the new obs
+            obs = next_obs
+
+            step_data["terminated"] = terminated[np.newaxis]
+            step_data["truncated"] = truncated[np.newaxis]
+            step_data["actions"] = actions[np.newaxis]
+            step_data["rewards"] = clip_rewards_fn(rewards)[np.newaxis]
+            rb.add(step_data, validate_args=cfg.buffer.validate_args)
+
+            # Reset and save the observation coming from the automatic reset
+            dones_idxes = dones.nonzero()[0].tolist()
+            reset_envs = len(dones_idxes)
+            if reset_envs > 0:
+                reset_data = {}
+                for k in obs_keys:
+                    reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
+                reset_data["terminated"] = np.zeros((1, reset_envs, 1))
+                reset_data["truncated"] = np.zeros((1, reset_envs, 1))
+                reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
+                reset_data["rewards"] = np.zeros((1, reset_envs, 1))
+                rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
+                for d in dones_idxes:
+                    step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
+                    step_data["truncated"][0, d] = np.zeros_like(step_data["truncated"][0, d])
+                # Reset internal agent states
+                player.init_states(reset_envs=dones_idxes)
 
         # Train the agent
-        if update >= learning_starts and updates_before_training <= 0:
-            if player.actor_type == "exploration":
-                player.actor = actor_task.module
-                player.actor_type = "task"
-            with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
-                for i in range(cfg.algo.per_rank_gradient_steps):
+        if update >= learning_starts:
+            per_rank_gradient_steps = ratio(policy_step / world_size)
+            if per_rank_gradient_steps > 0:
+                if player.actor_type != "task":
+                    player.actor_type = "task"
+                    player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
+                    for agent_p, p in zip(actor_task.parameters(), player.actor.parameters()):
+                        p.data = agent_p.data
+                with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
                     sample = rb.sample_tensors(
                         batch_size=cfg.algo.per_rank_batch_size,
                         sequence_length=cfg.algo.per_rank_sequence_length,
-                        n_samples=1,
+                        n_samples=per_rank_gradient_steps,
                         dtype=None,
                         device=device,
                         from_numpy=cfg.buffer.from_numpy,
                     )  # [N_samples, Seq_len, Batch_size, ...]
-                    batch = {k: v[0].float() for k, v in sample.items()}
-                    train(
-                        fabric,
-                        world_model,
-                        actor_task,
-                        critic_task,
-                        world_optimizer,
-                        actor_task_optimizer,
-                        critic_task_optimizer,
-                        batch,
-                        aggregator,
-                        cfg,
+                    for i in range(per_rank_gradient_steps):
+                        batch = {k: v[i].float() for k, v in sample.items()}
+                        train(
+                            fabric,
+                            world_model,
+                            actor_task,
+                            critic_task,
+                            world_optimizer,
+                            actor_task_optimizer,
+                            critic_task_optimizer,
+                            batch,
+                            aggregator,
+                            cfg,
+                        )
+                        cumulative_per_rank_gradient_steps += 1
+                    train_step += world_size
+                if aggregator and not aggregator.disabled:
+                    aggregator.update("Params/exploration_amount_task", actor_task._get_expl_amount(policy_step))
+                    aggregator.update(
+                        "Params/exploration_amount_exploration", actor_exploration._get_expl_amount(policy_step)
                     )
-                train_step += world_size
-            updates_before_training = cfg.algo.train_every // policy_steps_per_update
-            if cfg.algo.actor.expl_decay:
-                expl_decay_steps += 1
-                actor_task.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
-                )
-                actor_exploration.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
-                )
-            if aggregator and not aggregator.disabled:
-                aggregator.update("Params/exploration_amount_task", actor_task.expl_amount)
-                aggregator.update("Params/exploration_amount_exploration", actor_exploration.expl_amount)
 
         # Log metrics
         if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -431,15 +404,15 @@
             state = {
                 "world_model": world_model.state_dict(),
                 "actor_task": actor_task.state_dict(),
                 "critic_task": critic_task.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
-                "expl_decay_steps": expl_decay_steps,
+                "ratio": ratio.state_dict(),
                 "update": update * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
@@ -450,16 +423,16 @@
                 state=state,
                 replay_buffer=rb if cfg.buffer.checkpoint else None,
             )
 
     envs.close()
     # task test few-shot
     if fabric.is_global_zero and cfg.algo.run_test:
-        player.actor = actor_task.module
         player.actor_type = "task"
+        player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
         test(player, fabric, cfg, log_dir, "few-shot")
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.dreamer_v1.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
         models_to_log = {"world_model": world_model, "actor_task": actor_task, "critic_task": critic_task}
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv1/utils.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv1/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv2/agent.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv2/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 from lightning.fabric import Fabric
 from lightning.fabric.wrappers import _FabricModule
 from lightning.pytorch.utilities.seed import isolate_rng
 from torch import nn
 
 from sheeprl.algos.dreamer_v2.agent import Actor as DV2Actor
 from sheeprl.algos.dreamer_v2.agent import MinedojoActor as DV2MinedojoActor
-from sheeprl.algos.dreamer_v2.agent import WorldModel
+from sheeprl.algos.dreamer_v2.agent import PlayerDV2, WorldModel
 from sheeprl.algos.dreamer_v2.agent import build_agent as dv2_build_agent
 from sheeprl.models.models import MLP
-from sheeprl.utils.utils import init_weights
+from sheeprl.utils.fabric import get_single_device_fabric
+from sheeprl.utils.utils import init_weights, unwrap_fabric
 
 # In order to use the hydra.utils.get_class method, in this way the user can
 # specify in the configs the name of the class without having to know where
 # to go to retrieve the class
 Actor = DV2Actor
 MinedojoActor = DV2MinedojoActor
 
@@ -33,15 +34,25 @@
     ensembles_state: Optional[Dict[str, torch.Tensor]] = None,
     actor_task_state: Optional[Dict[str, torch.Tensor]] = None,
     critic_task_state: Optional[Dict[str, torch.Tensor]] = None,
     target_critic_task_state: Optional[Dict[str, torch.Tensor]] = None,
     actor_exploration_state: Optional[Dict[str, torch.Tensor]] = None,
     critic_exploration_state: Optional[Dict[str, torch.Tensor]] = None,
     target_critic_exploration_state: Optional[Dict[str, torch.Tensor]] = None,
-) -> Tuple[WorldModel, _FabricModule, _FabricModule, _FabricModule, nn.Module, _FabricModule, _FabricModule, nn.Module]:
+) -> Tuple[
+    WorldModel,
+    nn.ModuleList,
+    _FabricModule,
+    _FabricModule,
+    _FabricModule,
+    _FabricModule,
+    _FabricModule,
+    _FabricModule,
+    PlayerDV2,
+]:
     """Build the models and wrap them with Fabric.
 
     Args:
         fabric (Fabric): the fabric object.
         action_dim (int): the dimension of the actions.
         is_continuous (bool): whether or not the actions are continuous.
         cfg (DictConfig): the configs of P2E_DV2.
@@ -79,15 +90,15 @@
     critic_cfg = cfg.algo.critic
 
     # Sizes
     stochastic_size = world_model_cfg.stochastic_size * world_model_cfg.discrete_size
     latent_state_size = stochastic_size + world_model_cfg.recurrent_model.recurrent_state_size
 
     # Create exploration models
-    world_model, actor_exploration, critic_exploration, target_critic_exploration = dv2_build_agent(
+    world_model, actor_exploration, critic_exploration, target_critic_exploration, player = dv2_build_agent(
         fabric,
         actions_dim=actions_dim,
         is_continuous=is_continuous,
         cfg=cfg,
         obs_space=obs_space,
         world_model_state=world_model_state,
         actor_state=actor_exploration_state,
@@ -101,28 +112,30 @@
         latent_state_size=latent_state_size,
         actions_dim=actions_dim,
         is_continuous=is_continuous,
         init_std=actor_cfg.init_std,
         min_std=actor_cfg.min_std,
         mlp_layers=actor_cfg.mlp_layers,
         dense_units=actor_cfg.dense_units,
-        activation=eval(actor_cfg.dense_act),
+        activation=hydra.utils.get_class(actor_cfg.dense_act),
         distribution_cfg=cfg.distribution,
         layer_norm=actor_cfg.layer_norm,
     )
     critic_task = MLP(
         input_dims=latent_state_size,
         output_dim=1,
         hidden_sizes=[critic_cfg.dense_units] * critic_cfg.mlp_layers,
-        activation=eval(critic_cfg.dense_act),
+        activation=hydra.utils.get_class(critic_cfg.dense_act),
         flatten_dim=None,
         norm_layer=[nn.LayerNorm for _ in range(critic_cfg.mlp_layers)] if critic_cfg.layer_norm else None,
-        norm_args=[{"normalized_shape": critic_cfg.dense_units} for _ in range(critic_cfg.mlp_layers)]
-        if critic_cfg.layer_norm
-        else None,
+        norm_args=(
+            [{"normalized_shape": critic_cfg.dense_units} for _ in range(critic_cfg.mlp_layers)]
+            if critic_cfg.layer_norm
+            else None
+        ),
     )
     actor_task.apply(init_weights)
     critic_task.apply(init_weights)
 
     # Load task models from checkpoint
     if actor_task_state:
         actor_task.load_state_dict(actor_task_state)
@@ -131,14 +144,16 @@
 
     # Setup task models with Fabric
     actor_task = fabric.setup_module(actor_task)
     critic_task = fabric.setup_module(critic_task)
     target_critic_task = copy.deepcopy(critic_task.module)
     if target_critic_task_state:
         target_critic_task.load_state_dict(target_critic_task_state)
+    single_device_fabric = get_single_device_fabric(fabric)
+    target_critic_task = single_device_fabric.setup_module(target_critic_task)
 
     # initialize the ensembles with different seeds to be sure they have different weights
     ens_list = []
     with isolate_rng():
         for i in range(cfg.algo.ensembles.n):
             fabric.seed_everything(cfg.seed + i)
             ens_list.append(
@@ -146,15 +161,15 @@
                     input_dims=int(
                         sum(actions_dim)
                         + cfg.algo.world_model.recurrent_model.recurrent_state_size
                         + cfg.algo.world_model.stochastic_size * cfg.algo.world_model.discrete_size
                     ),
                     output_dim=cfg.algo.world_model.stochastic_size * cfg.algo.world_model.discrete_size,
                     hidden_sizes=[cfg.algo.ensembles.dense_units] * cfg.algo.ensembles.mlp_layers,
-                    activation=eval(cfg.algo.ensembles.dense_act),
+                    activation=hydra.utils.get_class(cfg.algo.ensembles.dense_act),
                     flatten_dim=None,
                     norm_layer=(
                         [nn.LayerNorm for _ in range(cfg.algo.ensembles.mlp_layers)]
                         if cfg.algo.ensembles.layer_norm
                         else None
                     ),
                     norm_args=(
@@ -169,17 +184,26 @@
             )
     ensembles = nn.ModuleList(ens_list)
     if ensembles_state:
         ensembles.load_state_dict(ensembles_state)
     for i in range(len(ensembles)):
         ensembles[i] = fabric.setup_module(ensembles[i])
 
+    # Setup player agent
+    if cfg.algo.player.actor_type != "exploration":
+        fabric_player = get_single_device_fabric(fabric)
+        player_actor = unwrap_fabric(actor_task)
+        player.actor = fabric_player.setup_module(player_actor)
+        for agent_p, p in zip(actor_task.parameters(), player.actor.parameters()):
+            p.data = agent_p.data
+
     return (
         world_model,
         ensembles,
         actor_task,
         critic_task,
         target_critic_task,
         actor_exploration,
         critic_exploration,
         target_critic_exploration,
+        player,
     )
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv2/evaluate.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv2/evaluate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Dict
 
 import gymnasium as gym
 from lightning import Fabric
 
-from sheeprl.algos.dreamer_v2.agent import PlayerDV2
 from sheeprl.algos.dreamer_v2.utils import test
 from sheeprl.algos.p2e_dv2.agent import build_agent
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.registry import register_evaluation
 
 
@@ -41,31 +40,19 @@
 
     is_continuous = isinstance(action_space, gym.spaces.Box)
     is_multidiscrete = isinstance(action_space, gym.spaces.MultiDiscrete)
     actions_dim = tuple(
         action_space.shape if is_continuous else (action_space.nvec.tolist() if is_multidiscrete else [action_space.n])
     )
     # Create the actor and critic models
-    world_model, _, actor_task, _, _, _, _, _ = build_agent(
+    cfg.algo.player.actor_type = "task"
+    _, _, _, _, _, _, _, _, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
-        state["world_model"],
-        None,
-        state["actor_task"],
+        world_model_state=state["world_model"],
+        actor_task_state=state["actor_task"],
     )
-    player = PlayerDV2(
-        world_model.encoder.module,
-        world_model.rssm.recurrent_model.module,
-        world_model.rssm.representation_model.module,
-        actor_task.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        discrete_size=cfg.algo.world_model.discrete_size,
-    )
-
-    test(player, fabric, cfg, log_dir, sample_actions=False)
+    del _
+    test(player, fabric, cfg, log_dir, greedy=True)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 import hydra
 import numpy as np
 import torch
 import torch.nn.functional as F
 from lightning.fabric import Fabric
 from lightning.fabric.wrappers import _FabricModule, _FabricOptimizer
 from torch import Tensor, nn
-from torch.distributions import Bernoulli, Distribution, Independent, Normal
+from torch.distributions import Bernoulli, Distribution, Independent, Normal, OneHotCategorical
 from torch.distributions.utils import logits_to_probs
 from torchmetrics import SumMetric
 
-from sheeprl.algos.dreamer_v2.agent import PlayerDV2, WorldModel
+from sheeprl.algos.dreamer_v2.agent import WorldModel
 from sheeprl.algos.dreamer_v2.loss import reconstruction_loss
-from sheeprl.algos.dreamer_v2.utils import compute_lambda_values, test
+from sheeprl.algos.dreamer_v2.utils import compute_lambda_values, prepare_obs, test
 from sheeprl.algos.p2e_dv2.agent import build_agent
 from sheeprl.data.buffers import EnvIndependentReplayBuffer, EpisodeBuffer, SequentialReplayBuffer
-from sheeprl.utils.distribution import OneHotCategoricalValidateArgs
 from sheeprl.utils.env import make_env
+from sheeprl.utils.fabric import get_single_device_fabric
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import polynomial_decay, save_configs
+from sheeprl.utils.utils import Ratio, save_configs, unwrap_fabric
 
 # Decomment the following line if you are using MineDojo on an headless machine
 # os.environ["MINEDOJO_HEADLESS"] = "1"
 
 
 def train(
     fabric: Fabric,
@@ -98,19 +98,17 @@
         actor_exploration (_FabricModule): the actor for exploration.
         critic_exploration (_FabricModule): the critic for exploration.
         target_critic_exploration (nn.Module): the target critic for exploration.
         actor_exploration_optimizer (_FabricOptimizer): the optimizer of the actor for exploration.
         critic_exploration_optimizer (_FabricOptimizer): the optimizer of the critic for exploration.
         is_continuous (bool): whether or not are continuous actions.
         actions_dim (Sequence[int]): the actions dimension.
-        is_exploring (bool): whether the agent is exploring.
     """
     batch_size = cfg.algo.per_rank_batch_size
     sequence_length = cfg.algo.per_rank_sequence_length
-    validate_args = cfg.distribution.validate_args
     recurrent_state_size = cfg.algo.world_model.recurrent_model.recurrent_state_size
     stochastic_size = cfg.algo.world_model.stochastic_size
     discrete_size = cfg.algo.world_model.discrete_size
     device = fabric.device
     data = {k: data[k] for k in data.keys()}
     batch_obs = {k: data[k] / 255 - 0.5 for k in cfg.algo.cnn_keys.encoder}
     batch_obs.update({k: data[k] for k in cfg.algo.mlp_keys.encoder})
@@ -142,38 +140,25 @@
     # latent_states has dimension (sequence_length, batch_size, recurrent_state_size + stochastic_size * discrete_size)
     latent_states = torch.cat((posteriors.view(*posteriors.shape[:-2], -1), recurrent_states), -1)
 
     # compute predictions for the observations
     decoded_information: Dict[str, torch.Tensor] = world_model.observation_model(latent_states)
 
     # compute the distribution over the reconstructed observations
-    po = {
-        k: Independent(
-            Normal(rec_obs, 1, validate_args=validate_args), len(rec_obs.shape[2:]), validate_args=validate_args
-        )
-        for k, rec_obs in decoded_information.items()
-    }
+    po = {k: Independent(Normal(rec_obs, 1), len(rec_obs.shape[2:])) for k, rec_obs in decoded_information.items()}
 
     # compute the distribution over the rewards
-    pr = Independent(
-        Normal(world_model.reward_model(latent_states.detach()), 1, validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
+    pr = Independent(Normal(world_model.reward_model(latent_states.detach()), 1), 1)
 
     # compute the distribution over the terminal steps, if required
     if cfg.algo.world_model.use_continues and world_model.continue_model:
-        pc = Independent(
-            Bernoulli(logits=world_model.continue_model(latent_states.detach()), validate_args=validate_args),
-            1,
-            validate_args=validate_args,
-        )
-        continue_targets = (1 - data["dones"]) * cfg.algo.gamma
+        pc = Independent(Bernoulli(logits=world_model.continue_model(latent_states.detach())), 1)
+        continues_targets = (1 - data["terminated"]) * cfg.algo.gamma
     else:
-        pc = continue_targets = None
+        pc = continues_targets = None
 
     # Reshape posterior and prior logits to shape [B, T, 32, 32]
     priors_logits = priors_logits.view(*priors_logits.shape[:-1], stochastic_size, discrete_size)
     posteriors_logits = posteriors_logits.view(*posteriors_logits.shape[:-1], stochastic_size, discrete_size)
 
     # world model optimization step
     world_optimizer.zero_grad(set_to_none=True)
@@ -185,17 +170,16 @@
         priors_logits,
         posteriors_logits,
         cfg.algo.world_model.kl_balancing_alpha,
         cfg.algo.world_model.kl_free_nats,
         cfg.algo.world_model.kl_free_avg,
         cfg.algo.world_model.kl_regularizer,
         pc,
-        continue_targets,
+        continues_targets,
         cfg.algo.world_model.discount_scale_factor,
-        validate_args=validate_args,
     )
     fabric.backward(rec_loss)
     world_grad = None
     if cfg.algo.world_model.clip_gradients is not None and cfg.algo.world_model.clip_gradients > 0:
         world_grad = fabric.clip_gradients(
             module=world_model,
             optimizer=world_optimizer,
@@ -214,17 +198,15 @@
                     posteriors.view(*posteriors.shape[:-2], -1).detach(),
                     recurrent_states.detach(),
                     data["actions"].detach(),
                 ),
                 -1,
             )
         )[:-1]
-        next_obs_embedding_dist = Independent(
-            Normal(out, 1, validate_args=validate_args), 1, validate_args=validate_args
-        )
+        next_obs_embedding_dist = Independent(Normal(out, 1), 1)
         loss -= next_obs_embedding_dist.log_prob(posteriors.view(sequence_length, batch_size, -1).detach()[1:]).mean()
     loss.backward()
     ensemble_grad = None
     if cfg.algo.ensembles.clip_gradients is not None and cfg.algo.ensembles.clip_gradients > 0:
         ensemble_grad = fabric.clip_gradients(
             module=ens,
             optimizer=ensemble_optimizer,
@@ -274,16 +256,16 @@
         next_obs_embedding[i] = ens(torch.cat((imagined_trajectories.detach(), imagined_actions.detach()), -1))
 
     # next_obs_embedding -> N_ensemble x Horizon x Batch_size*Seq_len x Obs_embedding_size
     intrinsic_reward = next_obs_embedding.var(0).mean(-1, keepdim=True) * cfg.algo.intrinsic_reward_multiplier
 
     if cfg.algo.world_model.use_continues and world_model.continue_model:
         continues = logits_to_probs(logits=world_model.continue_model(imagined_trajectories), is_binary=True)
-        true_done = (1 - data["dones"]).flatten().reshape(1, -1, 1) * cfg.algo.gamma
-        continues = torch.cat((true_done, continues[1:]))
+        true_continue = (1 - data["terminated"]).flatten().reshape(1, -1, 1) * cfg.algo.gamma
+        continues = torch.cat((true_continue, continues[1:]))
     else:
         continues = torch.ones_like(intrinsic_reward.detach()) * cfg.algo.gamma
 
     lambda_values_exploration = compute_lambda_values(
         intrinsic_reward[:-1],
         predicted_target_values_exploration[:-1],
         continues[:-1],
@@ -324,19 +306,15 @@
             module=actor_exploration,
             optimizer=actor_exploration_optimizer,
             max_norm=cfg.algo.actor.clip_gradients,
             error_if_nonfinite=False,
         )
     actor_exploration_optimizer.step()
 
-    qv = Independent(
-        Normal(critic_exploration(imagined_trajectories.detach())[:-1], 1, validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
+    qv = Independent(Normal(critic_exploration(imagined_trajectories.detach())[:-1], 1), 1)
     critic_exploration_optimizer.zero_grad(set_to_none=True)
     value_loss_exploration = -torch.mean(discount[:-1, ..., 0] * qv.log_prob(lambda_values_exploration.detach()))
     fabric.backward(value_loss_exploration)
     critic_exploration_grad = None
     if cfg.algo.critic.clip_gradients is not None and cfg.algo.critic.clip_gradients > 0:
         critic_exploration_grad = fabric.clip_gradients(
             module=critic_exploration,
@@ -377,16 +355,16 @@
         imagined_latent_state = torch.cat((imagined_prior, recurrent_state), -1)
         imagined_trajectories[i] = imagined_latent_state
 
     predicted_target_values_task = target_critic_task(imagined_trajectories)
     predicted_rewards = world_model.reward_model(imagined_trajectories)
     if cfg.algo.world_model.use_continues and world_model.continue_model:
         continues = logits_to_probs(logits=world_model.continue_model(imagined_trajectories), is_binary=True)
-        true_done = (1 - data["dones"]).reshape(1, -1, 1) * cfg.algo.gamma
-        continues = torch.cat((true_done, continues[1:]))
+        true_continue = (1 - data["terminated"]).reshape(1, -1, 1) * cfg.algo.gamma
+        continues = torch.cat((true_continue, continues[1:]))
     else:
         continues = torch.ones_like(predicted_rewards.detach()) * cfg.algo.gamma
 
     lambda_values_task = compute_lambda_values(
         predicted_rewards[:-1],
         predicted_target_values_task[:-1],
         continues[:-1],
@@ -428,17 +406,16 @@
             optimizer=actor_task_optimizer,
             max_norm=cfg.algo.actor.clip_gradients,
             error_if_nonfinite=False,
         )
     actor_task_optimizer.step()
 
     qv = Independent(
-        Normal(critic_task(imagined_trajectories.detach())[:-1], 1, validate_args=validate_args),
+        Normal(critic_task(imagined_trajectories.detach())[:-1], 1),
         1,
-        validate_args=validate_args,
     )
     critic_task_optimizer.zero_grad(set_to_none=True)
     value_loss_task = -torch.mean(discount[:-1, ..., 0] * qv.log_prob(lambda_values_task.detach()))
     fabric.backward(value_loss_task)
     critic_task_grad = None
     if cfg.algo.critic.clip_gradients is not None and cfg.algo.critic.clip_gradients > 0:
         critic_task_grad = fabric.clip_gradients(
@@ -453,33 +430,19 @@
         aggregator.update("Loss/observation_loss", observation_loss.detach())
         aggregator.update("Loss/reward_loss", reward_loss.detach())
         aggregator.update("Loss/state_loss", state_loss.detach())
         aggregator.update("Loss/continue_loss", continue_loss.detach())
         aggregator.update("State/kl", kl.mean().detach())
         aggregator.update(
             "State/post_entropy",
-            Independent(
-                OneHotCategoricalValidateArgs(logits=posteriors_logits.detach(), validate_args=validate_args),
-                1,
-                validate_args=validate_args,
-            )
-            .entropy()
-            .mean()
-            .detach(),
+            Independent(OneHotCategorical(logits=posteriors_logits.detach()), 1).entropy().mean().detach(),
         )
         aggregator.update(
             "State/prior_entropy",
-            Independent(
-                OneHotCategoricalValidateArgs(logits=priors_logits.detach(), validate_args=validate_args),
-                1,
-                validate_args=validate_args,
-            )
-            .entropy()
-            .mean()
-            .detach(),
+            Independent(OneHotCategorical(logits=priors_logits.detach()), 1).entropy().mean().detach(),
         )
         aggregator.update("Loss/ensemble_loss", loss.detach().cpu())
         aggregator.update("Rewards/intrinsic", intrinsic_reward.detach().cpu().mean())
         aggregator.update(
             "Values_exploration/predicted_values", predicted_target_values_exploration.detach().cpu().mean()
         )
         aggregator.update("Values_exploration/lambda_values", lambda_values_exploration.detach().cpu().mean())
@@ -510,16 +473,14 @@
 
 
 @register_algorithm()
 def main(fabric: Fabric, cfg: Dict[str, Any]):
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     # These arguments cannot be changed
     cfg.env.screen_size = 64
     cfg.env.frame_stack = 1
@@ -588,14 +549,15 @@
         ensembles,
         actor_task,
         critic_task,
         target_critic_task,
         actor_exploration,
         critic_exploration,
         target_critic_exploration,
+        player,
     ) = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["world_model"] if cfg.checkpoint.resume_from else None,
@@ -604,28 +566,14 @@
         state["critic_task"] if cfg.checkpoint.resume_from else None,
         state["target_critic_task"] if cfg.checkpoint.resume_from else None,
         state["actor_exploration"] if cfg.checkpoint.resume_from else None,
         state["critic_exploration"] if cfg.checkpoint.resume_from else None,
         state["target_critic_exploration"] if cfg.checkpoint.resume_from else None,
     )
 
-    player = PlayerDV2(
-        world_model.encoder.module,
-        world_model.rssm.recurrent_model.module,
-        world_model.rssm.representation_model.module,
-        actor_exploration.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        discrete_size=cfg.algo.world_model.discrete_size,
-        actor_type=cfg.algo.player.actor_type,
-    )
-
     # Optimizers
     world_optimizer = hydra.utils.instantiate(
         cfg.algo.world_model.optimizer, params=world_model.parameters(), _convert_="all"
     )
     actor_exploration_optimizer = hydra.utils.instantiate(
         cfg.algo.actor.optimizer, params=actor_exploration.parameters(), _convert_="all"
     )
@@ -699,15 +647,14 @@
     if cfg.checkpoint.resume_from and cfg.buffer.checkpoint:
         if isinstance(state["rb"], list) and world_size == len(state["rb"]):
             rb = state["rb"][fabric.global_rank]
         elif isinstance(state["rb"], (EnvIndependentReplayBuffer, EpisodeBuffer)):
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
-    expl_decay_steps = state["expl_decay_steps"] if cfg.checkpoint.resume_from else 0
 
     # Global variables
     train_step = 0
     last_train = 0
     start_step = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
@@ -716,35 +663,26 @@
         if cfg.checkpoint.resume_from
         else 1
     )
     policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
     policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    updates_before_training = cfg.algo.train_every // policy_steps_per_update if not cfg.dry_run else 0
     num_updates = cfg.algo.total_steps // policy_steps_per_update if not cfg.dry_run else 1
     learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
-    max_step_expl_decay = cfg.algo.actor.max_step_expl_decay // (cfg.algo.per_rank_gradient_steps * world_size)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        actor_task.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
-        actor_exploration.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
         if not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -758,194 +696,184 @@
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
-    step_data["dones"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     if cfg.dry_run:
-        step_data["dones"] = step_data["dones"] + 1
+        step_data["terminated"] = step_data["terminated"] + 1
+        step_data["truncated"] = step_data["truncated"] + 1
     step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
-    step_data["is_first"] = np.ones_like(step_data["dones"])
+    step_data["is_first"] = np.ones_like(step_data["terminated"])
     rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
 
-    per_rank_gradient_steps = 0
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * world_size
 
-        # Measure environment interaction time: this considers both the model forward
-        # to get the action given the observation and the time taken into the environment
-        with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            # Sample an action given the observation received by the environment
-            if (
-                update <= learning_starts
-                and cfg.checkpoint.resume_from is None
-                and "minedojo" not in cfg.env.wrapper._target_.lower()
-            ):
-                real_actions = actions = np.array(envs.action_space.sample())
-                if not is_continuous:
-                    actions = np.concatenate(
-                        [
-                            F.one_hot(torch.as_tensor(act), act_dim).numpy()
-                            for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
-                        ],
-                        axis=-1,
-                    )
-            else:
-                with torch.no_grad():
-                    normalized_obs = {}
-                    for k in obs_keys:
-                        torch_obs = torch.as_tensor(obs[k][np.newaxis], dtype=torch.float32, device=device)
-                        if k in cfg.algo.cnn_keys.encoder:
-                            torch_obs = torch_obs / 255 - 0.5
-                        normalized_obs[k] = torch_obs
-                    mask = {k: v for k, v in normalized_obs.items() if k.startswith("mask")}
+        with torch.inference_mode():
+            # Measure environment interaction time: this considers both the model forward
+            # to get the action given the observation and the time taken into the environment
+            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
+                # Sample an action given the observation received by the environment
+                if (
+                    update <= learning_starts
+                    and cfg.checkpoint.resume_from is None
+                    and "minedojo" not in cfg.env.wrapper._target_.lower()
+                ):
+                    real_actions = actions = np.array(envs.action_space.sample())
+                    if not is_continuous:
+                        actions = np.concatenate(
+                            [
+                                F.one_hot(torch.as_tensor(act), act_dim).numpy()
+                                for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
+                            ],
+                            axis=-1,
+                        )
+                else:
+                    torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                    mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
-                    real_actions = actions = player.get_exploration_action(normalized_obs, mask)
+                    real_actions = actions = player.get_actions(torch_obs, mask=mask)
                     actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                     if is_continuous:
                         real_actions = torch.cat(real_actions, -1).cpu().numpy()
                     else:
                         real_actions = (
                             torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
 
-            step_data["is_first"] = copy.deepcopy(step_data["dones"])
-            next_obs, rewards, dones, truncated, infos = envs.step(real_actions.reshape(envs.action_space.shape))
-            dones = np.logical_or(dones, truncated).astype(np.uint8)
-            if cfg.dry_run and buffer_type == "episode":
-                dones = np.ones_like(dones)
-
-        if cfg.metric.log_level > 0 and "final_info" in infos:
-            for i, agent_ep_info in enumerate(infos["final_info"]):
-                if agent_ep_info is not None:
-                    ep_rew = agent_ep_info["episode"]["r"]
-                    ep_len = agent_ep_info["episode"]["l"]
-                    if aggregator and not aggregator.disabled:
-                        aggregator.update("Rewards/rew_avg", ep_rew)
-                        aggregator.update("Game/ep_len_avg", ep_len)
-                    fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
-
-        # Save the real next observation
-        real_next_obs = copy.deepcopy(next_obs)
-        if "final_observation" in infos:
-            for idx, final_obs in enumerate(infos["final_observation"]):
-                if final_obs is not None:
-                    for k, v in final_obs.items():
-                        real_next_obs[k][idx] = v
-
-        for k in obs_keys:  # [N_envs, N_obs]
-            step_data[k] = real_next_obs[k][np.newaxis]
-
-        # Next_obs becomes the new obs
-        obs = next_obs
-
-        step_data["dones"] = dones.reshape((1, cfg.env.num_envs, -1))
-        step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
-        step_data["rewards"] = clip_rewards_fn(rewards).reshape((1, cfg.env.num_envs, -1))
-        rb.add(step_data, validate_args=cfg.buffer.validate_args)
-
-        # Reset and save the observation coming from the automatic reset
-        dones_idxes = dones.nonzero()[0].tolist()
-        reset_envs = len(dones_idxes)
-        if reset_envs > 0:
-            reset_data = {}
-            for k in obs_keys:
-                reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
-            reset_data["dones"] = np.zeros((1, reset_envs, 1))
-            reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
-            reset_data["rewards"] = np.zeros((1, reset_envs, 1))
-            reset_data["is_first"] = np.ones_like(reset_data["dones"])
-            rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
-            # Reset dones so that `is_first` is updated
-            for d in dones_idxes:
-                step_data["dones"][0, d] = np.zeros_like(step_data["dones"][0, d])
-            # Reset internal agent states
-            player.init_states(dones_idxes)
-
-        updates_before_training -= 1
+                step_data["is_first"] = copy.deepcopy(np.logical_or(step_data["terminated"], step_data["truncated"]))
+                next_obs, rewards, terminated, truncated, infos = envs.step(
+                    real_actions.reshape(envs.action_space.shape)
+                )
+                dones = np.logical_or(terminated, truncated).astype(np.uint8)
+                if cfg.dry_run and buffer_type == "episode":
+                    dones = np.ones_like(dones)
+
+            if cfg.metric.log_level > 0 and "final_info" in infos:
+                for i, agent_ep_info in enumerate(infos["final_info"]):
+                    if agent_ep_info is not None:
+                        ep_rew = agent_ep_info["episode"]["r"]
+                        ep_len = agent_ep_info["episode"]["l"]
+                        if aggregator and not aggregator.disabled:
+                            aggregator.update("Rewards/rew_avg", ep_rew)
+                            aggregator.update("Game/ep_len_avg", ep_len)
+                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+
+            # Save the real next observation
+            real_next_obs = copy.deepcopy(next_obs)
+            if "final_observation" in infos:
+                for idx, final_obs in enumerate(infos["final_observation"]):
+                    if final_obs is not None:
+                        for k, v in final_obs.items():
+                            real_next_obs[k][idx] = v
+
+            for k in obs_keys:  # [N_envs, N_obs]
+                step_data[k] = real_next_obs[k][np.newaxis]
+
+            # Next_obs becomes the new obs
+            obs = next_obs
+
+            step_data["terminated"] = terminated.reshape((1, cfg.env.num_envs, -1))
+            step_data["truncated"] = truncated.reshape((1, cfg.env.num_envs, -1))
+            step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
+            step_data["rewards"] = clip_rewards_fn(rewards).reshape((1, cfg.env.num_envs, -1))
+            rb.add(step_data, validate_args=cfg.buffer.validate_args)
+
+            # Reset and save the observation coming from the automatic reset
+            dones_idxes = dones.nonzero()[0].tolist()
+            reset_envs = len(dones_idxes)
+            if reset_envs > 0:
+                reset_data = {}
+                for k in obs_keys:
+                    reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
+                reset_data["terminated"] = np.zeros((1, reset_envs, 1))
+                reset_data["truncated"] = np.zeros((1, reset_envs, 1))
+                reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
+                reset_data["rewards"] = np.zeros((1, reset_envs, 1))
+                reset_data["is_first"] = np.ones_like(reset_data["terminated"])
+                rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
+                # Reset dones so that `is_first` is updated
+                for d in dones_idxes:
+                    step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
+                    step_data["truncated"][0, d] = np.zeros_like(step_data["truncated"][0, d])
+                # Reset internal agent states
+                player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts and updates_before_training <= 0:
-            n_samples = (
-                cfg.algo.per_rank_pretrain_steps if update == learning_starts else cfg.algo.per_rank_gradient_steps
-            )
-            local_data = rb.sample_tensors(
-                batch_size=cfg.algo.per_rank_batch_size,
-                sequence_length=cfg.algo.per_rank_sequence_length,
-                n_samples=n_samples,
-                dtype=None,
-                device=fabric.device,
-                from_numpy=cfg.buffer.from_numpy,
-            )
-            # Start training
-            with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
-                for i in range(next(iter(local_data.values())).shape[0]):
-                    if per_rank_gradient_steps % cfg.algo.critic.target_network_update_freq == 0:
-                        for cp, tcp in zip(critic_task.module.parameters(), target_critic_task.parameters()):
-                            tcp.data.copy_(cp.data)
-                        for cp, tcp in zip(
-                            critic_exploration.module.parameters(), target_critic_exploration.parameters()
-                        ):
-                            tcp.data.copy_(cp.data)
-                    batch = {k: v[i].float() for k, v in local_data.items()}
-                    train(
-                        fabric,
-                        world_model,
-                        actor_task,
-                        critic_task,
-                        target_critic_task,
-                        world_optimizer,
-                        actor_task_optimizer,
-                        critic_task_optimizer,
-                        batch,
-                        aggregator,
-                        cfg,
-                        ensembles=ensembles,
-                        ensemble_optimizer=ensemble_optimizer,
-                        actor_exploration=actor_exploration,
-                        critic_exploration=critic_exploration,
-                        target_critic_exploration=target_critic_exploration,
-                        actor_exploration_optimizer=actor_exploration_optimizer,
-                        critic_exploration_optimizer=critic_exploration_optimizer,
-                        is_continuous=is_continuous,
-                        actions_dim=actions_dim,
-                    )
-                train_step += world_size
-            updates_before_training = cfg.algo.train_every // policy_steps_per_update
-            if cfg.algo.actor.expl_decay:
-                expl_decay_steps += 1
-                actor_task.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
-                )
-                actor_exploration.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
+        if update >= learning_starts:
+            per_rank_gradient_steps = ratio(policy_step / world_size)
+            if per_rank_gradient_steps > 0:
+                local_data = rb.sample_tensors(
+                    batch_size=cfg.algo.per_rank_batch_size,
+                    sequence_length=cfg.algo.per_rank_sequence_length,
+                    n_samples=per_rank_gradient_steps,
+                    dtype=None,
+                    device=fabric.device,
+                    from_numpy=cfg.buffer.from_numpy,
                 )
-            if aggregator and not aggregator.disabled:
-                aggregator.update("Params/exploration_amount_task", actor_task.expl_amount)
-                aggregator.update("Params/exploration_amount_exploration", actor_exploration.expl_amount)
+                # Start training
+                with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
+                    for i in range(per_rank_gradient_steps):
+                        if (
+                            cumulative_per_rank_gradient_steps % cfg.algo.critic.per_rank_target_network_update_freq
+                            == 0
+                        ):
+                            for cp, tcp in zip(critic_task.module.parameters(), target_critic_task.parameters()):
+                                tcp.data.copy_(cp.data)
+                            for cp, tcp in zip(
+                                critic_exploration.module.parameters(), target_critic_exploration.parameters()
+                            ):
+                                tcp.data.copy_(cp.data)
+                        batch = {k: v[i].float() for k, v in local_data.items()}
+                        train(
+                            fabric,
+                            world_model,
+                            actor_task,
+                            critic_task,
+                            target_critic_task,
+                            world_optimizer,
+                            actor_task_optimizer,
+                            critic_task_optimizer,
+                            batch,
+                            aggregator,
+                            cfg,
+                            ensembles=ensembles,
+                            ensemble_optimizer=ensemble_optimizer,
+                            actor_exploration=actor_exploration,
+                            critic_exploration=critic_exploration,
+                            target_critic_exploration=target_critic_exploration,
+                            actor_exploration_optimizer=actor_exploration_optimizer,
+                            critic_exploration_optimizer=critic_exploration_optimizer,
+                            is_continuous=is_continuous,
+                            actions_dim=actions_dim,
+                        )
+                        cumulative_per_rank_gradient_steps += 1
+                    train_step += world_size
 
         # Log metrics
         if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -975,15 +903,15 @@
                 "critic_task": critic_task.state_dict(),
                 "target_critic_task": target_critic_task.state_dict(),
                 "ensembles": ensembles.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
                 "ensemble_optimizer": ensemble_optimizer.state_dict(),
-                "expl_decay_steps": expl_decay_steps,
+                "ratio": ratio.state_dict(),
                 "update": update * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "critic_exploration": critic_exploration.state_dict(),
                 "target_critic_exploration": target_critic_exploration.state_dict(),
                 "actor_exploration_optimizer": actor_exploration_optimizer.state_dict(),
                 "critic_exploration_optimizer": critic_exploration_optimizer.state_dict(),
@@ -998,16 +926,17 @@
                 state=state,
                 replay_buffer=rb if cfg.buffer.checkpoint else None,
             )
 
     envs.close()
     # task test zero-shot
     if fabric.is_global_zero and cfg.algo.run_test:
-        player.actor = actor_task.module
         player.actor_type = "task"
+        fabric_player = get_single_device_fabric(fabric)
+        player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
         test(player, fabric, cfg, log_dir, "zero-shot")
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.dreamer_v1.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
         models_to_log = {
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,41 @@
-from __future__ import annotations
-
 import copy
 import os
 import pathlib
 import warnings
 from typing import Any, Dict
 
 import gymnasium as gym
 import hydra
 import numpy as np
 import torch
 from lightning.fabric import Fabric
 from torchmetrics import SumMetric
 
-from sheeprl.algos.dreamer_v2.agent import PlayerDV2
-from sheeprl.algos.dreamer_v2.dreamer_v2 import train
-from sheeprl.algos.dreamer_v2.utils import test
-from sheeprl.algos.p2e_dv2.agent import build_agent
-from sheeprl.data.buffers import EnvIndependentReplayBuffer, EpisodeBuffer, SequentialReplayBuffer
+from sheeprl.algos.dreamer_v3.dreamer_v3 import train
+from sheeprl.algos.dreamer_v3.utils import Moments, prepare_obs, test
+from sheeprl.algos.p2e_dv3.agent import build_agent
+from sheeprl.data.buffers import EnvIndependentReplayBuffer, SequentialReplayBuffer
 from sheeprl.utils.env import make_env
+from sheeprl.utils.fabric import get_single_device_fabric
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import polynomial_decay, save_configs
-
-# Decomment the following line if you are using MineDojo on an headless machine
-# os.environ["MINEDOJO_HEADLESS"] = "1"
+from sheeprl.utils.utils import Ratio, save_configs, unwrap_fabric
 
 
 @register_algorithm()
 def main(fabric: Fabric, cfg: Dict[str, Any], exploration_cfg: Dict[str, Any]):
+    # Single-device fabric object
+    fabric_player = get_single_device_fabric(fabric)
+
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     ckpt_path = pathlib.Path(cfg.checkpoint.exploration_ckpt_path)
     resume_from_checkpoint = cfg.checkpoint.resume_from is not None
 
     # Finetuning that was interrupted for some reason
     if resume_from_checkpoint:
         state = fabric.load(pathlib.Path(cfg.checkpoint.resume_from))
@@ -69,15 +65,14 @@
     if cfg.buffer.load_from_exploration and exploration_cfg.buffer.checkpoint:
         cfg.env.num_envs = exploration_cfg.env.num_envs
     # There must be the same cnn and mlp keys during exploration and finetuning
     cfg.algo.cnn_keys = exploration_cfg.algo.cnn_keys
     cfg.algo.mlp_keys = exploration_cfg.algo.mlp_keys
 
     # These arguments cannot be changed
-    cfg.env.screen_size = 64
     cfg.env.frame_stack = 1
 
     # Create Logger. This will create the logger only on the
     # rank-0 process
     logger = get_logger(fabric, cfg)
     if logger and fabric.is_global_zero:
         fabric._loggers = [logger]
@@ -130,42 +125,28 @@
     if cfg.metric.log_level > 0:
         fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
         fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
         fabric.print("Decoder CNN keys:", cfg.algo.cnn_keys.decoder)
         fabric.print("Decoder MLP keys:", cfg.algo.mlp_keys.decoder)
     obs_keys = cfg.algo.cnn_keys.encoder + cfg.algo.mlp_keys.encoder
 
-    world_model, _, actor_task, critic_task, target_critic_task, actor_exploration, _, _ = build_agent(
+    (world_model, _, actor_task, critic_task, target_critic_task, actor_exploration, _, player) = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["world_model"],
         None,
         state["actor_task"],
         state["critic_task"],
         state["target_critic_task"],
         state["actor_exploration"],
     )
 
-    player = PlayerDV2(
-        world_model.encoder.module,
-        world_model.rssm.recurrent_model.module,
-        world_model.rssm.representation_model.module,
-        actor_exploration.module if cfg.algo.player.actor_type == "exploration" else actor_task.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        discrete_size=cfg.algo.world_model.discrete_size,
-        actor_type=cfg.algo.player.actor_type,
-    )
-
     # Optimizers
     world_optimizer = hydra.utils.instantiate(
         cfg.algo.world_model.optimizer, params=world_model.parameters(), _convert_="all"
     )
     actor_task_optimizer = hydra.utils.instantiate(
         cfg.algo.actor.optimizer, params=actor_task.parameters(), _convert_="all"
     )
@@ -175,91 +156,74 @@
     world_optimizer.load_state_dict(state["world_optimizer"])
     actor_task_optimizer.load_state_dict(state["actor_task_optimizer"])
     critic_task_optimizer.load_state_dict(state["critic_task_optimizer"])
     world_optimizer, actor_task_optimizer, critic_task_optimizer = fabric.setup_optimizers(
         world_optimizer, actor_task_optimizer, critic_task_optimizer
     )
 
+    moments_task = Moments(
+        cfg.algo.actor.moments.decay,
+        cfg.algo.actor.moments.max,
+        cfg.algo.actor.moments.percentile.low,
+        cfg.algo.actor.moments.percentile.high,
+    )
+    moments_task.load_state_dict(state["moments_task"])
+
     if fabric.is_global_zero:
         save_configs(cfg, log_dir)
 
     # Metrics
     aggregator = None
     if not MetricAggregator.disabled:
         aggregator: MetricAggregator = hydra.utils.instantiate(cfg.metric.aggregator, _convert_="all").to(device)
 
     # Local data
     buffer_size = cfg.buffer.size // int(cfg.env.num_envs * world_size) if not cfg.dry_run else 4
-    buffer_type = cfg.buffer.type.lower()
-    if buffer_type == "sequential":
-        rb = EnvIndependentReplayBuffer(
-            buffer_size,
-            n_envs=cfg.env.num_envs,
-            obs_keys=obs_keys,
-            memmap=cfg.buffer.memmap,
-            memmap_dir=os.path.join(log_dir, "memmap_buffer", f"rank_{fabric.global_rank}"),
-            buffer_cls=SequentialReplayBuffer,
-        )
-    elif buffer_type == "episode":
-        rb = EpisodeBuffer(
-            buffer_size,
-            minimum_episode_length=1 if cfg.dry_run else cfg.algo.per_rank_sequence_length,
-            n_envs=cfg.env.num_envs,
-            obs_keys=obs_keys,
-            prioritize_ends=cfg.buffer.prioritize_ends,
-            memmap=cfg.buffer.memmap,
-            memmap_dir=os.path.join(log_dir, "memmap_buffer", f"rank_{fabric.global_rank}"),
-        )
-    else:
-        raise ValueError(f"Unrecognized buffer type: must be one of `sequential` or `episode`, received: {buffer_type}")
+    rb = EnvIndependentReplayBuffer(
+        buffer_size,
+        n_envs=cfg.env.num_envs,
+        memmap=cfg.buffer.memmap,
+        memmap_dir=os.path.join(log_dir, "memmap_buffer", f"rank_{fabric.global_rank}"),
+        buffer_cls=SequentialReplayBuffer,
+    )
     if resume_from_checkpoint or (cfg.buffer.load_from_exploration and exploration_cfg.buffer.checkpoint):
         if isinstance(state["rb"], list) and world_size == len(state["rb"]):
             rb = state["rb"][fabric.global_rank]
-        elif isinstance(state["rb"], (EnvIndependentReplayBuffer, EpisodeBuffer)):
+        elif isinstance(state["rb"], EnvIndependentReplayBuffer):
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
-    expl_decay_steps = state["expl_decay_steps"] if resume_from_checkpoint else 0
 
     # Global variables
     train_step = 0
     last_train = 0
     start_step = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // world_size) + 1
+        (state["update"] // fabric.world_size) + 1
         if resume_from_checkpoint
         else 1
     )
     policy_step = state["update"] * cfg.env.num_envs if resume_from_checkpoint else 0
     last_log = state["last_log"] if resume_from_checkpoint else 0
     last_checkpoint = state["last_checkpoint"] if resume_from_checkpoint else 0
-    policy_steps_per_update = int(cfg.env.num_envs * world_size)
-    updates_before_training = cfg.algo.train_every // policy_steps_per_update if not cfg.dry_run else 0
-    num_updates = cfg.algo.total_steps // policy_steps_per_update if not cfg.dry_run else 1
+    policy_steps_per_update = int(cfg.env.num_envs * fabric.world_size)
+    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
     learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
-    max_step_expl_decay = cfg.algo.actor.max_step_expl_decay // (cfg.algo.per_rank_gradient_steps * world_size)
     if resume_from_checkpoint:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        actor_task.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
-        actor_exploration.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
         if not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -273,169 +237,174 @@
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
-    step_data["dones"] = np.zeros((1, cfg.env.num_envs, 1))
-    if cfg.dry_run:
-        step_data["dones"] = step_data["dones"] + 1
-    step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
+    step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
-    step_data["is_first"] = np.ones_like(step_data["dones"])
-    rb.add(step_data, validate_args=cfg.buffer.validate_args)
+    step_data["is_first"] = np.ones_like(step_data["terminated"])
     player.init_states()
 
-    per_rank_gradient_steps = 0
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * world_size
 
-        # Measure environment interaction time: this considers both the model forward
-        # to get the action given the observation and the time taken into the environment
-        with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            with torch.no_grad():
-                normalized_obs = {}
-                for k in obs_keys:
-                    torch_obs = torch.as_tensor(obs[k][np.newaxis], dtype=torch.float32, device=device)
-                    if k in cfg.algo.cnn_keys.encoder:
-                        torch_obs = torch_obs / 255 - 0.5
-                    normalized_obs[k] = torch_obs
-                mask = {k: v for k, v in normalized_obs.items() if k.startswith("mask")}
+        with torch.inference_mode():
+            # Measure environment interaction time: this considers both the model forward
+            # to get the action given the observation and the time taken into the environment
+            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
+                torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                 if len(mask) == 0:
                     mask = None
-                real_actions = actions = player.get_exploration_action(normalized_obs, mask)
-                actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
+                real_actions = actions = player.get_actions(torch_obs, mask=mask)
+                actions = torch.cat(actions, -1).cpu().numpy()
                 if is_continuous:
-                    real_actions = torch.cat(real_actions, -1).cpu().numpy()
+                    real_actions = torch.cat(real_actions, dim=-1).cpu().numpy()
                 else:
                     real_actions = (
                         torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                     )
 
-            step_data["is_first"] = copy.deepcopy(step_data["dones"])
-            next_obs, rewards, dones, truncated, infos = envs.step(real_actions.reshape(envs.action_space.shape))
-            dones = np.logical_or(dones, truncated).astype(np.uint8)
-            if cfg.dry_run and buffer_type == "episode":
-                dones = np.ones_like(dones)
-
-        if cfg.metric.log_level > 0 and "final_info" in infos:
-            for i, agent_ep_info in enumerate(infos["final_info"]):
-                if agent_ep_info is not None:
-                    ep_rew = agent_ep_info["episode"]["r"]
-                    ep_len = agent_ep_info["episode"]["l"]
-                    if aggregator and not aggregator.disabled:
-                        aggregator.update("Rewards/rew_avg", ep_rew)
-                        aggregator.update("Game/ep_len_avg", ep_len)
-                    fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
-
-        # Save the real next observation
-        real_next_obs = copy.deepcopy(next_obs)
-        if "final_observation" in infos:
-            for idx, final_obs in enumerate(infos["final_observation"]):
-                if final_obs is not None:
-                    for k, v in final_obs.items():
-                        real_next_obs[k][idx] = v
-
-        for k in obs_keys:  # [N_envs, N_obs]
-            step_data[k] = real_next_obs[k][np.newaxis]
-
-        # Next_obs becomes the new obs
-        obs = next_obs
-
-        step_data["dones"] = dones.reshape((1, cfg.env.num_envs, -1))
-        step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
-        step_data["rewards"] = clip_rewards_fn(rewards).reshape((1, cfg.env.num_envs, -1))
-        rb.add(step_data, validate_args=cfg.buffer.validate_args)
-
-        # Reset and save the observation coming from the automatic reset
-        dones_idxes = dones.nonzero()[0].tolist()
-        reset_envs = len(dones_idxes)
-        if reset_envs > 0:
-            reset_data = {}
+                step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
+                rb.add(step_data, validate_args=cfg.buffer.validate_args)
+
+                next_obs, rewards, terminated, truncated, infos = envs.step(
+                    real_actions.reshape(envs.action_space.shape)
+                )
+                dones = np.logical_or(terminated, truncated).astype(np.uint8)
+
+            step_data["is_first"] = np.zeros_like(step_data["terminated"])
+            if "restart_on_exception" in infos:
+                for i, agent_roe in enumerate(infos["restart_on_exception"]):
+                    if agent_roe and not dones[i]:
+                        last_inserted_idx = (rb.buffer[i]._pos - 1) % rb.buffer[i].buffer_size
+                        rb.buffer[i]["terminated"][last_inserted_idx] = np.zeros_like(
+                            rb.buffer[i]["terminated"][last_inserted_idx]
+                        )
+                        rb.buffer[i]["truncated"][last_inserted_idx] = np.ones_like(
+                            rb.buffer[i]["truncated"][last_inserted_idx]
+                        )
+                        rb.buffer[i]["is_first"][last_inserted_idx] = np.zeros_like(
+                            rb.buffer[i]["is_first"][last_inserted_idx]
+                        )
+                        step_data["is_first"][i] = np.ones_like(step_data["is_first"][i])
+
+            if cfg.metric.log_level > 0 and "final_info" in infos:
+                for i, agent_ep_info in enumerate(infos["final_info"]):
+                    if agent_ep_info is not None:
+                        ep_rew = agent_ep_info["episode"]["r"]
+                        ep_len = agent_ep_info["episode"]["l"]
+                        if aggregator and not aggregator.disabled:
+                            aggregator.update("Rewards/rew_avg", ep_rew)
+                            aggregator.update("Game/ep_len_avg", ep_len)
+                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+
+            # Save the real next observation
+            real_next_obs = copy.deepcopy(next_obs)
+            if "final_observation" in infos:
+                for idx, final_obs in enumerate(infos["final_observation"]):
+                    if final_obs is not None:
+                        for k, v in final_obs.items():
+                            real_next_obs[k][idx] = v
+
             for k in obs_keys:
-                reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
-            reset_data["dones"] = np.zeros((1, reset_envs, 1))
-            reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
-            reset_data["rewards"] = np.zeros((1, reset_envs, 1))
-            reset_data["is_first"] = np.ones_like(reset_data["dones"])
-            rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
-            # Reset dones so that `is_first` is updated
-            for d in dones_idxes:
-                step_data["dones"][0, d] = np.zeros_like(step_data["dones"][0, d])
-            # Reset internal agent states
-            player.init_states(dones_idxes)
+                step_data[k] = next_obs[k][np.newaxis]
+
+            # next_obs becomes the new obs
+            obs = next_obs
 
-        updates_before_training -= 1
+            rewards = rewards.reshape((1, cfg.env.num_envs, -1))
+            step_data["terminated"] = terminated.reshape((1, cfg.env.num_envs, -1))
+            step_data["truncated"] = truncated.reshape((1, cfg.env.num_envs, -1))
+            step_data["rewards"] = clip_rewards_fn(rewards)
+
+            dones_idxes = dones.nonzero()[0].tolist()
+            reset_envs = len(dones_idxes)
+            if reset_envs > 0:
+                reset_data = {}
+                for k in obs_keys:
+                    reset_data[k] = (real_next_obs[k][dones_idxes])[np.newaxis]
+                reset_data["terminated"] = step_data["terminated"][:, dones_idxes]
+                reset_data["truncated"] = step_data["truncated"][:, dones_idxes]
+                reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
+                reset_data["rewards"] = step_data["rewards"][:, dones_idxes]
+                reset_data["is_first"] = np.zeros_like(reset_data["terminated"])
+                rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
+
+                # Reset already inserted step data
+                step_data["rewards"][:, dones_idxes] = np.zeros_like(reset_data["rewards"])
+                step_data["terminated"][:, dones_idxes] = np.zeros_like(step_data["terminated"][:, dones_idxes])
+                step_data["truncated"][:, dones_idxes] = np.zeros_like(step_data["truncated"][:, dones_idxes])
+                step_data["is_first"][:, dones_idxes] = np.ones_like(step_data["is_first"][:, dones_idxes])
+                player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts and updates_before_training <= 0:
-            if player.actor_type == "exploration":
-                player.actor = actor_task.module
-                player.actor_type = "task"
-            n_samples = (
-                cfg.algo.per_rank_pretrain_steps if update == learning_starts else cfg.algo.per_rank_gradient_steps
-            )
-            local_data = rb.sample_tensors(
-                batch_size=cfg.algo.per_rank_batch_size,
-                sequence_length=cfg.algo.per_rank_sequence_length,
-                n_samples=n_samples,
-                dtype=None,
-                device=fabric.device,
-                from_numpy=cfg.buffer.from_numpy,
-            )
-            # Start training
-            with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
-                for i in range(next(iter(local_data.values())).shape[0]):
-                    if per_rank_gradient_steps % cfg.algo.critic.target_network_update_freq == 0:
-                        for cp, tcp in zip(critic_task.module.parameters(), target_critic_task.parameters()):
-                            tcp.data.copy_(cp.data)
-                    batch = {k: v[i].float() for k, v in local_data.items()}
-                    train(
-                        fabric,
-                        world_model,
-                        actor_task,
-                        critic_task,
-                        target_critic_task,
-                        world_optimizer,
-                        actor_task_optimizer,
-                        critic_task_optimizer,
-                        batch,
-                        aggregator,
-                        cfg,
-                        actions_dim=actions_dim,
-                    )
-                train_step += world_size
-            updates_before_training = cfg.algo.train_every // policy_steps_per_update
-            if cfg.algo.actor.expl_decay:
-                expl_decay_steps += 1
-                actor_task.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
+        if update >= learning_starts:
+            per_rank_gradient_steps = ratio(policy_step / world_size)
+            if per_rank_gradient_steps > 0:
+                if player.actor_type != "task":
+                    player.actor_type = "task"
+                    player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
+                    for agent_p, p in zip(actor_task.parameters(), player.actor.parameters()):
+                        p.data = agent_p.data
+                local_data = rb.sample_tensors(
+                    cfg.algo.per_rank_batch_size,
+                    sequence_length=cfg.algo.per_rank_sequence_length,
+                    n_samples=per_rank_gradient_steps,
+                    dtype=None,
+                    device=fabric.device,
+                    from_numpy=cfg.buffer.from_numpy,
                 )
-                actor_exploration.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
-                )
-            if aggregator and not aggregator.disabled:
-                aggregator.update("Params/exploration_amount_task", actor_task.expl_amount)
-                aggregator.update("Params/exploration_amount_exploration", actor_exploration.expl_amount)
+                # Start training
+                with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
+                    for i in range(per_rank_gradient_steps):
+                        if (
+                            cumulative_per_rank_gradient_steps % cfg.algo.critic.per_rank_target_network_update_freq
+                            == 0
+                        ):
+                            tau = 1 if cumulative_per_rank_gradient_steps == 0 else cfg.algo.critic.tau
+                            for cp, tcp in zip(critic_task.module.parameters(), target_critic_task.parameters()):
+                                tcp.data.copy_(tau * cp.data + (1 - tau) * tcp.data)
+                        batch = {k: v[i].float() for k, v in local_data.items()}
+                        train(
+                            fabric,
+                            world_model,
+                            actor_task,
+                            critic_task,
+                            target_critic_task,
+                            world_optimizer,
+                            actor_task_optimizer,
+                            critic_task_optimizer,
+                            batch,
+                            aggregator,
+                            cfg,
+                            is_continuous=is_continuous,
+                            actions_dim=actions_dim,
+                            moments=moments_task,
+                        )
+                        cumulative_per_rank_gradient_steps += 1
+                    train_step += world_size
 
         # Log metrics
         if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -463,36 +432,44 @@
                 "world_model": world_model.state_dict(),
                 "actor_task": actor_task.state_dict(),
                 "critic_task": critic_task.state_dict(),
                 "target_critic_task": target_critic_task.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
-                "expl_decay_steps": expl_decay_steps,
+                "ratio": ratio.state_dict(),
                 "update": update * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
+                "moments_task": moments_task.state_dict(),
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
                 "on_checkpoint_coupled",
                 fabric=fabric,
                 ckpt_path=ckpt_path,
                 state=state,
                 replay_buffer=rb if cfg.buffer.checkpoint else None,
             )
 
     envs.close()
+
     # task test few-shot
     if fabric.is_global_zero and cfg.algo.run_test:
-        player.actor = actor_task.module
         player.actor_type = "task"
-        test(player, fabric, cfg, log_dir, "few-shot")
+        player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
+        test(player, fabric, cfg, log_dir, "few-shot", greedy=False)
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.dreamer_v1.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
-        models_to_log = {"world_model": world_model, "actor_task": actor_task, "critic_task": critic_task}
+        models_to_log = {
+            "world_model": world_model,
+            "actor_task": actor_task,
+            "critic_task": critic_task,
+            "target_critic_task": target_critic_task,
+            "moments_task": moments_task,
+        }
         register_model(fabric, log_models, cfg, models_to_log)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv2/utils.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv2/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,14 @@
     "Loss/reward_loss",
     "Loss/state_loss",
     "Loss/continue_loss",
     "Loss/ensemble_loss",
     "State/kl",
     "State/post_entropy",
     "State/prior_entropy",
-    "Params/exploration_amount_task",
-    "Params/exploration_amount_exploration",
     "Rewards/intrinsic",
     "Values_exploration/predicted_values",
     "Values_exploration/lambda_values",
     "Grads/world_model",
     "Grads/actor_task",
     "Grads/critic_task",
     "Grads/actor_exploration",
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv3/agent.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv3/agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from lightning.fabric import Fabric
 from lightning.fabric.wrappers import _FabricModule
 from lightning.pytorch.utilities.seed import isolate_rng
 from torch import nn
 
 from sheeprl.algos.dreamer_v3.agent import Actor as DV3Actor
 from sheeprl.algos.dreamer_v3.agent import MinedojoActor as DV3MinedojoActor
-from sheeprl.algos.dreamer_v3.agent import WorldModel
+from sheeprl.algos.dreamer_v3.agent import PlayerDV3, WorldModel
 from sheeprl.algos.dreamer_v3.agent import build_agent as dv3_build_agent
 from sheeprl.algos.dreamer_v3.utils import init_weights, uniform_init_weights
 from sheeprl.models.models import MLP
+from sheeprl.utils.fabric import get_single_device_fabric
+from sheeprl.utils.utils import unwrap_fabric
 
 # In order to use the hydra.utils.get_class method, in this way the user can
 # specify in the configs the name of the class without having to know where
 # to go to retrieve the class
 Actor = DV3Actor
 MinedojoActor = DV3MinedojoActor
 
@@ -31,15 +33,17 @@
     world_model_state: Optional[Dict[str, torch.Tensor]] = None,
     ensembles_state: Optional[Dict[str, torch.Tensor]] = None,
     actor_task_state: Optional[Dict[str, torch.Tensor]] = None,
     critic_task_state: Optional[Dict[str, torch.Tensor]] = None,
     target_critic_task_state: Optional[Dict[str, torch.Tensor]] = None,
     actor_exploration_state: Optional[Dict[str, torch.Tensor]] = None,
     critics_exploration_state: Optional[Dict[str, Dict[str, Any]]] = None,
-) -> Tuple[WorldModel, _FabricModule, _FabricModule, _FabricModule, nn.Module, _FabricModule, Dict[str, Any]]:
+) -> Tuple[
+    WorldModel, nn.ModuleList, _FabricModule, _FabricModule, _FabricModule, _FabricModule, Dict[str, Any], PlayerDV3
+]:
     """Build the models and wrap them with Fabric.
 
     Args:
         fabric (Fabric): the fabric object.
         action_dim (int): the dimension of the actions.
         is_continuous (bool): whether or not the actions are continuous.
         cfg (Dict[str, Any]): the configs of P2E_DV3.
@@ -77,15 +81,15 @@
     critic_cfg = cfg.algo.critic
 
     # Sizes
     stochastic_size = world_model_cfg.stochastic_size * world_model_cfg.discrete_size
     latent_state_size = stochastic_size + world_model_cfg.recurrent_model.recurrent_state_size
 
     # Create task models
-    world_model, actor_task, critic_task, target_critic_task = dv3_build_agent(
+    world_model, actor_task, critic_task, target_critic_task, player = dv3_build_agent(
         fabric,
         actions_dim=actions_dim,
         is_continuous=is_continuous,
         cfg=cfg,
         obs_space=obs_space,
         world_model_state=world_model_state,
         actor_state=actor_task_state,
@@ -98,52 +102,59 @@
     actor_exploration: Union[Actor, MinedojoActor] = actor_cls(
         latent_state_size=latent_state_size,
         actions_dim=actions_dim,
         is_continuous=is_continuous,
         init_std=actor_cfg.init_std,
         min_std=actor_cfg.min_std,
         dense_units=actor_cfg.dense_units,
-        activation=eval(actor_cfg.dense_act),
+        activation=hydra.utils.get_class(actor_cfg.dense_act),
         mlp_layers=actor_cfg.mlp_layers,
         distribution_cfg=cfg.distribution,
-        layer_norm=actor_cfg.layer_norm,
+        layer_norm_cls=hydra.utils.get_class(actor_cfg.layer_norm.cls),
+        layer_norm_kw=actor_cfg.layer_norm.kw,
         unimix=cfg.algo.unimix,
     )
 
+    single_device_fabric = get_single_device_fabric(fabric)
     critics_exploration = {}
     intrinsic_critics = 0
+    critic_ln_cls = hydra.utils.get_class(critic_cfg.layer_norm.cls)
     for k, v in cfg.algo.critics_exploration.items():
         if v.weight > 0:
             if v.reward_type == "intrinsic":
                 intrinsic_critics += 1
             critics_exploration[k] = {
                 "weight": v.weight,
                 "reward_type": v.reward_type,
                 "module": MLP(
                     input_dims=latent_state_size,
                     output_dim=critic_cfg.bins,
                     hidden_sizes=[critic_cfg.dense_units] * critic_cfg.mlp_layers,
-                    activation=eval(critic_cfg.dense_act),
+                    activation=hydra.utils.get_class(critic_cfg.dense_act),
                     flatten_dim=None,
-                    layer_args={"bias": not critic_cfg.layer_norm},
-                    norm_layer=[nn.LayerNorm for _ in range(critic_cfg.mlp_layers)] if critic_cfg.layer_norm else None,
-                    norm_args=[{"normalized_shape": critic_cfg.dense_units} for _ in range(critic_cfg.mlp_layers)]
-                    if critic_cfg.layer_norm
-                    else None,
+                    layer_args={"bias": critic_ln_cls == nn.Identity},
+                    norm_layer=critic_ln_cls,
+                    norm_args={
+                        **critic_cfg.layer_norm.kw,
+                        "normalized_shape": critic_cfg.dense_units,
+                    },
                 ),
             }
             critics_exploration[k]["module"].apply(init_weights)
             if cfg.algo.hafner_initialization:
                 critics_exploration[k]["module"].model[-1].apply(uniform_init_weights(0.0))
             if critics_exploration_state:
                 critics_exploration[k]["module"].load_state_dict(critics_exploration_state[k]["module"])
             critics_exploration[k]["module"] = fabric.setup_module(critics_exploration[k]["module"])
             critics_exploration[k]["target_module"] = copy.deepcopy(critics_exploration[k]["module"].module)
             if critics_exploration_state:
                 critics_exploration[k]["target_module"].load_state_dict(critics_exploration_state[k]["target_module"])
+            critics_exploration[k]["target_module"] = single_device_fabric.setup_module(
+                critics_exploration[k]["target_module"]
+            )
 
     if intrinsic_critics == 0:
         raise RuntimeError("You must specify at least one intrinsic critic (`reward_type='intrinsic'`)")
 
     actor_exploration.apply(init_weights)
     if cfg.algo.hafner_initialization:
         actor_exploration.mlp_heads.apply(uniform_init_weights(1.0))
@@ -159,47 +170,54 @@
     target_critic_task.requires_grad_(False)
     for c in critics_exploration.values():
         c["target_module"].requires_grad_(False)
 
     # initialize the ensembles with different seeds to be sure they have different weights
     ens_list = []
     cfg_ensembles = cfg.algo.ensembles
+    ensembles_ln_cls = hydra.utils.get_class(cfg_ensembles.layer_norm.cls)
     with isolate_rng():
         for i in range(cfg_ensembles.n):
             fabric.seed_everything(cfg.seed + i)
             ens_list.append(
                 MLP(
                     input_dims=int(
                         sum(actions_dim)
                         + cfg.algo.world_model.recurrent_model.recurrent_state_size
                         + cfg.algo.world_model.stochastic_size * cfg.algo.world_model.discrete_size
                     ),
                     output_dim=cfg.algo.world_model.stochastic_size * cfg.algo.world_model.discrete_size,
                     hidden_sizes=[cfg_ensembles.dense_units] * cfg_ensembles.mlp_layers,
-                    activation=eval(cfg_ensembles.dense_act),
+                    activation=hydra.utils.get_class(cfg_ensembles.dense_act),
                     flatten_dim=None,
-                    layer_args={"bias": not cfg.algo.ensembles.layer_norm},
-                    norm_layer=(
-                        [nn.LayerNorm for _ in range(cfg_ensembles.mlp_layers)] if cfg_ensembles.layer_norm else None
-                    ),
-                    norm_args=(
-                        [{"normalized_shape": cfg_ensembles.dense_units} for _ in range(cfg_ensembles.mlp_layers)]
-                        if cfg_ensembles.layer_norm
-                        else None
-                    ),
+                    layer_args={"bias": ensembles_ln_cls == nn.Identity},
+                    norm_layer=ensembles_ln_cls,
+                    norm_args={
+                        **cfg_ensembles.layer_norm.kw,
+                        "normalized_shape": cfg_ensembles.dense_units,
+                    },
                 ).apply(init_weights)
             )
     ensembles = nn.ModuleList(ens_list)
     if ensembles_state:
         ensembles.load_state_dict(ensembles_state)
     for i in range(len(ensembles)):
         ensembles[i] = fabric.setup_module(ensembles[i])
 
+    # Setup player agent
+    if cfg.algo.player.actor_type == "exploration":
+        fabric_player = get_single_device_fabric(fabric)
+        player_actor = unwrap_fabric(actor_exploration)
+        player.actor = fabric_player.setup_module(player_actor)
+        for agent_p, p in zip(actor_exploration.parameters(), player.actor.parameters()):
+            p.data = agent_p.data
+
     return (
         world_model,
         ensembles,
         actor_task,
         critic_task,
         target_critic_task,
         actor_exploration,
         critics_exploration,
+        player,
     )
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv3/evaluate.py` & `sheeprl-0.5.5/sheeprl/algos/sac/evaluate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
 from typing import Any, Dict
 
 import gymnasium as gym
 from lightning import Fabric
 
-from sheeprl.algos.dreamer_v3.agent import PlayerDV3
-from sheeprl.algos.dreamer_v3.utils import test
-from sheeprl.algos.p2e_dv3.agent import build_agent
+from sheeprl.algos.sac.agent import build_agent
+from sheeprl.algos.sac.utils import test
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.registry import register_evaluation
 
 
-@register_evaluation(algorithms=["p2e_dv3_exploration", "p2e_dv3_finetuning"])
+@register_evaluation(algorithms=["sac", "sac_decoupled"])
 def evaluate(fabric: Fabric, cfg: Dict[str, Any], state: Dict[str, Any]):
     logger = get_logger(fabric, cfg)
     if logger and fabric.is_global_zero:
         fabric._loggers = [logger]
         fabric.logger.log_hyperparams(cfg)
     log_dir = get_log_dir(fabric, cfg.root_dir, cfg.run_name)
     fabric.print(f"Log dir: {log_dir}")
@@ -26,47 +25,26 @@
         cfg,
         cfg.seed,
         0,
         log_dir,
         "test",
         vector_env_idx=0,
     )()
-    observation_space = env.observation_space
     action_space = env.action_space
-
+    observation_space = env.observation_space
+    if not isinstance(action_space, gym.spaces.Box):
+        raise ValueError("Only continuous action space is supported for the SAC agent")
     if not isinstance(observation_space, gym.spaces.Dict):
         raise RuntimeError(f"Unexpected observation type, should be of type Dict, got: {observation_space}")
-
-    fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
+    if len(cfg.algo.mlp_keys.encoder) == 0:
+        raise RuntimeError("You should specify at least one MLP key for the encoder: `mlp_keys.encoder=[state]`")
+    for k in cfg.algo.mlp_keys.encoder:
+        if len(observation_space[k].shape) > 1:
+            raise ValueError(
+                "Only environments with vector-only observations are supported by the SAC agent. "
+                f"Provided environment: {cfg.env.id}"
+            )
     fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
 
-    is_continuous = isinstance(action_space, gym.spaces.Box)
-    is_multidiscrete = isinstance(action_space, gym.spaces.MultiDiscrete)
-    actions_dim = tuple(
-        action_space.shape if is_continuous else (action_space.nvec.tolist() if is_multidiscrete else [action_space.n])
-    )
-    # Create the actor and critic models
-    world_model, _, actor, _, _, _, _ = build_agent(
-        fabric,
-        actions_dim,
-        is_continuous,
-        cfg,
-        observation_space,
-        state["world_model"],
-        None,
-        state["actor_task"],
-    )
-    player = PlayerDV3(
-        world_model.encoder.module,
-        world_model.rssm,
-        actor.module,
-        actions_dim,
-        cfg.algo.player.expl_amount,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        discrete_size=cfg.algo.world_model.discrete_size,
-        actor_type="task",
-    )
-
-    test(player, fabric, cfg, log_dir, sample_actions=True)
+    _, agent = build_agent(fabric, cfg, observation_space, action_space, state["agent"])
+    del _
+    test(agent, fabric, cfg, log_dir)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 import numpy as np
 import torch
 import torch.nn.functional as F
 from lightning.fabric import Fabric
 from lightning.fabric.wrappers import _FabricModule, _FabricOptimizer
 from omegaconf import DictConfig
 from torch import Tensor, nn
-from torch.distributions import Distribution, Independent
+from torch.distributions import Distribution, Independent, OneHotCategorical
 from torchmetrics import SumMetric
 
-from sheeprl.algos.dreamer_v3.agent import PlayerDV3, WorldModel
+from sheeprl.algos.dreamer_v3.agent import WorldModel
 from sheeprl.algos.dreamer_v3.loss import reconstruction_loss
-from sheeprl.algos.dreamer_v3.utils import Moments, compute_lambda_values, test
+from sheeprl.algos.dreamer_v3.utils import Moments, compute_lambda_values, prepare_obs, test
 from sheeprl.algos.p2e_dv3.agent import build_agent
 from sheeprl.data.buffers import EnvIndependentReplayBuffer, SequentialReplayBuffer
 from sheeprl.utils.distribution import (
     BernoulliSafeMode,
     MSEDistribution,
-    OneHotCategoricalValidateArgs,
     SymlogDistribution,
     TwoHotEncodingDistribution,
 )
 from sheeprl.utils.env import make_env
+from sheeprl.utils.fabric import get_single_device_fabric
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import polynomial_decay, save_configs
+from sheeprl.utils.utils import Ratio, save_configs, unwrap_fabric
 
 # Decomment the following line if you are using MineDojo on an headless machine
 # os.environ["MINEDOJO_HEADLESS"] = "1"
 
 
 def train(
     fabric: Fabric,
@@ -103,15 +103,14 @@
         critics_exploration (Dict[str, Dict[str, Any]]): the critic for exploration.
         actor_exploration_optimizer (_FabricOptimizer): the optimizer of the actor for exploration.
         is_continuous (bool): whether or not are continuous actions.
         actions_dim (Sequence[int]): the actions dimension.
     """
     batch_size = cfg.algo.per_rank_batch_size
     sequence_length = cfg.algo.per_rank_sequence_length
-    validate_args = cfg.distribution.validate_args
     recurrent_state_size = cfg.algo.world_model.recurrent_model.recurrent_state_size
     stochastic_size = cfg.algo.world_model.stochastic_size
     discrete_size = cfg.algo.world_model.discrete_size
     device = fabric.device
     data = {k: data[k] for k in data.keys()}
     batch_obs = {k: data[k] / 255.0 - 0.5 for k in cfg.algo.cnn_keys.encoder}
     batch_obs.update({k: data[k] for k in cfg.algo.mlp_keys.encoder})
@@ -157,20 +156,16 @@
             for k in cfg.algo.mlp_keys.decoder
         }
     )
     # Compute the distribution over the rewards
     pr = TwoHotEncodingDistribution(world_model.reward_model(latent_states.detach()), dims=1)
 
     # Compute the distribution over the terminal steps, if required
-    pc = Independent(
-        BernoulliSafeMode(logits=world_model.continue_model(latent_states.detach()), validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    )
-    continue_targets = 1 - data["dones"]
+    pc = Independent(BernoulliSafeMode(logits=world_model.continue_model(latent_states.detach())), 1)
+    continues_targets = 1 - data["terminated"]
 
     # Reshape posterior and prior logits to shape [B, T, 32, 32]
     priors_logits = priors_logits.view(*priors_logits.shape[:-1], stochastic_size, discrete_size)
     posteriors_logits = posteriors_logits.view(*posteriors_logits.shape[:-1], stochastic_size, discrete_size)
 
     # world model optimization step
     world_optimizer.zero_grad(set_to_none=True)
@@ -182,15 +177,15 @@
         priors_logits,
         posteriors_logits,
         cfg.algo.world_model.kl_dynamic,
         cfg.algo.world_model.kl_representation,
         cfg.algo.world_model.kl_free_nats,
         cfg.algo.world_model.kl_regularizer,
         pc,
-        continue_targets,
+        continues_targets,
         cfg.algo.world_model.continue_scale_factor,
     )
     fabric.backward(rec_loss)
     world_model_grads = None
     if cfg.algo.world_model.clip_gradients is not None and cfg.algo.world_model.clip_gradients > 0:
         world_model_grads = fabric.clip_gradients(
             module=world_model,
@@ -264,21 +259,17 @@
         imagined_actions[i] = actions
 
     advantages = []
     weights_sum = sum([c["weight"] for c in critics_exploration.values()])
     for k, critic in critics_exploration.items():
         # Predict values and continues
         predicted_values = TwoHotEncodingDistribution(critic["module"](imagined_trajectories), dims=1).mean
-        continues = Independent(
-            BernoulliSafeMode(logits=world_model.continue_model(imagined_trajectories), validate_args=validate_args),
-            1,
-            validate_args=validate_args,
-        ).mode
-        true_done = (1 - data["dones"]).flatten().reshape(1, -1, 1)
-        continues = torch.cat((true_done, continues[1:]))
+        continues = Independent(BernoulliSafeMode(logits=world_model.continue_model(imagined_trajectories)), 1).mode
+        true_continue = (1 - data["terminated"]).flatten().reshape(1, -1, 1)
+        continues = torch.cat((true_continue, continues[1:]))
 
         if critic["reward_type"] == "intrinsic":
             # Predict intrinsic reward
             next_state_embedding = torch.empty(
                 len(ensembles),
                 cfg.algo.horizon + 1,
                 batch_size * sequence_length,
@@ -408,21 +399,17 @@
         imagined_trajectories[i] = imagined_latent_state
         actions = torch.cat(actor_task(imagined_latent_state.detach())[0], dim=-1)
         imagined_actions[i] = actions
 
     # Predict values, rewards and continues
     predicted_values = TwoHotEncodingDistribution(critic_task(imagined_trajectories), dims=1).mean
     predicted_rewards = TwoHotEncodingDistribution(world_model.reward_model(imagined_trajectories), dims=1).mean
-    continues = Independent(
-        BernoulliSafeMode(logits=world_model.continue_model(imagined_trajectories), validate_args=validate_args),
-        1,
-        validate_args=validate_args,
-    ).mode
-    true_done = (1 - data["dones"]).flatten().reshape(1, -1, 1)
-    continues = torch.cat((true_done, continues[1:]))
+    continues = Independent(BernoulliSafeMode(logits=world_model.continue_model(imagined_trajectories)), 1).mode
+    true_continue = (1 - data["terminated"]).flatten().reshape(1, -1, 1)
+    continues = torch.cat((true_continue, continues[1:]))
 
     lambda_values = compute_lambda_values(
         predicted_rewards[1:],
         predicted_values[1:],
         continues[1:] * cfg.algo.gamma,
         lmbda=cfg.algo.lmbda,
     )
@@ -496,33 +483,19 @@
         aggregator.update("Loss/observation_loss", observation_loss.detach())
         aggregator.update("Loss/reward_loss", reward_loss.detach())
         aggregator.update("Loss/state_loss", state_loss.detach())
         aggregator.update("Loss/continue_loss", continue_loss.detach())
         aggregator.update("State/kl", kl.mean().detach())
         aggregator.update(
             "State/post_entropy",
-            Independent(
-                OneHotCategoricalValidateArgs(logits=posteriors_logits.detach(), validate_args=validate_args),
-                1,
-                validate_args=validate_args,
-            )
-            .entropy()
-            .mean()
-            .detach(),
+            Independent(OneHotCategorical(logits=posteriors_logits.detach()), 1).entropy().mean().detach(),
         )
         aggregator.update(
             "State/prior_entropy",
-            Independent(
-                OneHotCategoricalValidateArgs(logits=priors_logits.detach(), validate_args=validate_args),
-                1,
-                validate_args=validate_args,
-            )
-            .entropy()
-            .mean()
-            .detach(),
+            Independent(OneHotCategorical(logits=priors_logits.detach()), 1).entropy().mean().detach(),
         )
         aggregator.update("Loss/ensemble_loss", loss.detach().cpu())
         aggregator.update("Loss/policy_loss_exploration", policy_loss_exploration.detach())
         aggregator.update("Loss/policy_loss_task", policy_loss_task.detach())
         aggregator.update("Loss/value_loss_task", value_loss_task.detach())
         if world_model_grads:
             aggregator.update("Grads/world_model", world_model_grads.mean().detach())
@@ -546,16 +519,14 @@
 
 
 @register_algorithm()
 def main(fabric: Fabric, cfg: Dict[str, Any]):
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     # These arguments cannot be changed
     cfg.env.frame_stack = 1
     cfg.algo.player.actor_type = "exploration"
@@ -622,14 +593,15 @@
         world_model,
         ensembles,
         actor_task,
         critic_task,
         target_critic_task,
         actor_exploration,
         critics_exploration,
+        player,
     ) = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["world_model"] if cfg.checkpoint.resume_from else None,
@@ -637,27 +609,14 @@
         state["actor_task"] if cfg.checkpoint.resume_from else None,
         state["critic_task"] if cfg.checkpoint.resume_from else None,
         state["target_critic_task"] if cfg.checkpoint.resume_from else None,
         state["actor_exploration"] if cfg.checkpoint.resume_from else None,
         state["critics_exploration"] if cfg.checkpoint.resume_from else None,
     )
 
-    player = PlayerDV3(
-        world_model.encoder.module,
-        world_model.rssm,
-        actor_exploration.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        discrete_size=cfg.algo.world_model.discrete_size,
-        actor_type=cfg.algo.player.actor_type,
-    )
-
     # Optimizers
     world_optimizer = hydra.utils.instantiate(
         cfg.algo.world_model.optimizer, params=world_model.parameters(), _convert_="all"
     )
     actor_exploration_optimizer = hydra.utils.instantiate(
         cfg.algo.actor.optimizer, params=actor_exploration.parameters(), _convert_="all"
     )
@@ -765,15 +724,14 @@
     if cfg.checkpoint.resume_from and cfg.buffer.checkpoint:
         if isinstance(state["rb"], list) and world_size == len(state["rb"]):
             rb = state["rb"][fabric.global_rank]
         elif isinstance(state["rb"], EnvIndependentReplayBuffer):
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
-    expl_decay_steps = state["expl_decay_steps"] if cfg.checkpoint.resume_from else 0
 
     # Global variables
     train_step = 0
     last_train = 0
     start_step = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
@@ -782,35 +740,26 @@
         if cfg.checkpoint.resume_from
         else 1
     )
     policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
     policy_steps_per_update = int(cfg.env.num_envs * fabric.world_size)
-    updates_before_training = cfg.algo.train_every // policy_steps_per_update
     num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
     learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
-    max_step_expl_decay = cfg.algo.actor.max_step_expl_decay // (cfg.algo.per_rank_gradient_steps * fabric.world_size)
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        actor_task.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
-        actor_exploration.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
         if not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -824,201 +773,197 @@
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
-    step_data["dones"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
-    step_data["is_first"] = np.ones_like(step_data["dones"])
+    step_data["is_first"] = np.ones_like(step_data["terminated"])
     player.init_states()
 
-    per_rank_gradient_steps = 0
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * world_size
 
-        # Measure environment interaction time: this considers both the model forward
-        # to get the action given the observation and the time taken into the environment
-        with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            # Sample an action given the observation received by the environment
-            if (
-                update <= learning_starts
-                and cfg.checkpoint.resume_from is None
-                and "minedojo" not in cfg.algo.actor.cls.lower()
-            ):
-                real_actions = actions = np.array(envs.action_space.sample())
-                if not is_continuous:
-                    actions = np.concatenate(
-                        [
-                            F.one_hot(torch.as_tensor(act), act_dim).numpy()
-                            for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
-                        ],
-                        axis=-1,
-                    )
-            else:
-                with torch.no_grad():
-                    preprocessed_obs = {}
-                    for k, v in obs.items():
-                        preprocessed_obs[k] = torch.as_tensor(v[np.newaxis], dtype=torch.float32, device=device)
-                        if k in cfg.algo.cnn_keys.encoder:
-                            preprocessed_obs[k] = preprocessed_obs[k] / 255.0 - 0.5
-                    mask = {k: v for k, v in preprocessed_obs.items() if k.startswith("mask")}
+        with torch.inference_mode():
+            # Measure environment interaction time: this considers both the model forward
+            # to get the action given the observation and the time taken into the environment
+            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
+                # Sample an action given the observation received by the environment
+                if (
+                    update <= learning_starts
+                    and cfg.checkpoint.resume_from is None
+                    and "minedojo" not in cfg.algo.actor.cls.lower()
+                ):
+                    real_actions = actions = np.array(envs.action_space.sample())
+                    if not is_continuous:
+                        actions = np.concatenate(
+                            [
+                                F.one_hot(torch.as_tensor(act), act_dim).numpy()
+                                for act, act_dim in zip(actions.reshape(len(actions_dim), -1), actions_dim)
+                            ],
+                            axis=-1,
+                        )
+                else:
+                    torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                    mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                     if len(mask) == 0:
                         mask = None
-                    real_actions = actions = player.get_exploration_action(preprocessed_obs, mask)
+                    real_actions = actions = player.get_actions(torch_obs, mask=mask)
                     actions = torch.cat(actions, -1).cpu().numpy()
                     if is_continuous:
                         real_actions = torch.cat(real_actions, dim=-1).cpu().numpy()
                     else:
                         real_actions = (
                             torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                         )
 
-            step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
-            rb.add(step_data, validate_args=cfg.buffer.validate_args)
+                step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
+                rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
-            next_obs, rewards, dones, truncated, infos = envs.step(real_actions.reshape(envs.action_space.shape))
-            dones = np.logical_or(dones, truncated).astype(np.uint8)
+                next_obs, rewards, terminated, truncated, infos = envs.step(
+                    real_actions.reshape(envs.action_space.shape)
+                )
+                dones = np.logical_or(terminated, truncated).astype(np.uint8)
 
-        step_data["is_first"] = np.zeros_like(step_data["dones"])
-        if "restart_on_exception" in infos:
-            for i, agent_roe in enumerate(infos["restart_on_exception"]):
-                if agent_roe and not dones[i]:
-                    last_inserted_idx = (rb.buffer[i]._pos - 1) % rb.buffer[i].buffer_size
-                    rb.buffer[i]["dones"][last_inserted_idx] = np.ones_like(rb.buffer[i]["dones"][last_inserted_idx])
-                    rb.buffer[i]["is_first"][last_inserted_idx] = np.zeros_like(
-                        rb.buffer[i]["is_first"][last_inserted_idx]
-                    )
-                    step_data["is_first"][i] = np.ones_like(step_data["is_first"][i])
+            step_data["is_first"] = np.zeros_like(step_data["terminated"])
+            if "restart_on_exception" in infos:
+                for i, agent_roe in enumerate(infos["restart_on_exception"]):
+                    if agent_roe and not dones[i]:
+                        last_inserted_idx = (rb.buffer[i]._pos - 1) % rb.buffer[i].buffer_size
+                        rb.buffer[i]["terminated"][last_inserted_idx] = np.zeros_like(
+                            rb.buffer[i]["terminated"][last_inserted_idx]
+                        )
+                        rb.buffer[i]["truncated"][last_inserted_idx] = np.ones_like(
+                            rb.buffer[i]["truncated"][last_inserted_idx]
+                        )
+                        rb.buffer[i]["is_first"][last_inserted_idx] = np.zeros_like(
+                            rb.buffer[i]["is_first"][last_inserted_idx]
+                        )
+                        step_data["is_first"][i] = np.ones_like(step_data["is_first"][i])
+
+            if cfg.metric.log_level > 0 and "final_info" in infos:
+                for i, agent_ep_info in enumerate(infos["final_info"]):
+                    if agent_ep_info is not None:
+                        ep_rew = agent_ep_info["episode"]["r"]
+                        ep_len = agent_ep_info["episode"]["l"]
+                        if aggregator and not aggregator.disabled:
+                            aggregator.update("Rewards/rew_avg", ep_rew)
+                            aggregator.update("Game/ep_len_avg", ep_len)
+                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+
+            # Save the real next observation
+            real_next_obs = copy.deepcopy(next_obs)
+            if "final_observation" in infos:
+                for idx, final_obs in enumerate(infos["final_observation"]):
+                    if final_obs is not None:
+                        for k, v in final_obs.items():
+                            real_next_obs[k][idx] = v
 
-        if cfg.metric.log_level > 0 and "final_info" in infos:
-            for i, agent_ep_info in enumerate(infos["final_info"]):
-                if agent_ep_info is not None:
-                    ep_rew = agent_ep_info["episode"]["r"]
-                    ep_len = agent_ep_info["episode"]["l"]
-                    if aggregator and not aggregator.disabled:
-                        aggregator.update("Rewards/rew_avg", ep_rew)
-                        aggregator.update("Game/ep_len_avg", ep_len)
-                    fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
-
-        # Save the real next observation
-        real_next_obs = copy.deepcopy(next_obs)
-        if "final_observation" in infos:
-            for idx, final_obs in enumerate(infos["final_observation"]):
-                if final_obs is not None:
-                    for k, v in final_obs.items():
-                        real_next_obs[k][idx] = v
-
-        for k in obs_keys:
-            step_data[k] = next_obs[k][np.newaxis]
-
-        # next_obs becomes the new obs
-        obs = next_obs
-
-        rewards = rewards.reshape((1, cfg.env.num_envs, -1))
-        step_data["dones"] = dones.reshape((1, cfg.env.num_envs, -1))
-        step_data["rewards"] = clip_rewards_fn(rewards)
-
-        dones_idxes = dones.nonzero()[0].tolist()
-        reset_envs = len(dones_idxes)
-        if reset_envs > 0:
-            reset_data = {}
             for k in obs_keys:
-                reset_data[k] = (real_next_obs[k][dones_idxes])[np.newaxis]
-            reset_data["dones"] = np.ones((1, reset_envs, 1))
-            reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
-            reset_data["rewards"] = step_data["rewards"][:, dones_idxes]
-            reset_data["is_first"] = np.zeros_like(reset_data["dones"])
-            rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
-
-            # Reset already inserted step data
-            step_data["rewards"][:, dones_idxes] = np.zeros_like(reset_data["rewards"])
-            step_data["dones"][:, dones_idxes] = np.zeros_like(step_data["dones"][:, dones_idxes])
-            step_data["is_first"][:, dones_idxes] = np.ones_like(step_data["is_first"][:, dones_idxes])
-            player.init_states(dones_idxes)
+                step_data[k] = next_obs[k][np.newaxis]
+
+            # next_obs becomes the new obs
+            obs = next_obs
 
-        updates_before_training -= 1
+            rewards = rewards.reshape((1, cfg.env.num_envs, -1))
+            step_data["terminated"] = terminated.reshape((1, cfg.env.num_envs, -1))
+            step_data["truncated"] = truncated.reshape((1, cfg.env.num_envs, -1))
+            step_data["rewards"] = clip_rewards_fn(rewards)
+
+            dones_idxes = dones.nonzero()[0].tolist()
+            reset_envs = len(dones_idxes)
+            if reset_envs > 0:
+                reset_data = {}
+                for k in obs_keys:
+                    reset_data[k] = (real_next_obs[k][dones_idxes])[np.newaxis]
+                reset_data["terminated"] = step_data["terminated"][:, dones_idxes]
+                reset_data["truncated"] = step_data["truncated"][:, dones_idxes]
+                reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
+                reset_data["rewards"] = step_data["rewards"][:, dones_idxes]
+                reset_data["is_first"] = np.zeros_like(reset_data["terminated"])
+                rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
+
+                # Reset already inserted step data
+                step_data["rewards"][:, dones_idxes] = np.zeros_like(reset_data["rewards"])
+                step_data["terminated"][:, dones_idxes] = np.zeros_like(step_data["terminated"][:, dones_idxes])
+                step_data["truncated"][:, dones_idxes] = np.zeros_like(step_data["truncated"][:, dones_idxes])
+                step_data["is_first"][:, dones_idxes] = np.ones_like(step_data["is_first"][:, dones_idxes])
+                player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts and updates_before_training <= 0:
-            local_data = rb.sample_tensors(
-                cfg.algo.per_rank_batch_size,
-                sequence_length=cfg.algo.per_rank_sequence_length,
-                n_samples=(
-                    cfg.algo.per_rank_pretrain_steps if update == learning_starts else cfg.algo.per_rank_gradient_steps
-                ),
-                dtype=None,
-                device=fabric.device,
-                from_numpy=cfg.buffer.from_numpy,
-            )
-            # Start training
-            with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
-                for i in range(next(iter(local_data.values())).shape[0]):
-                    if per_rank_gradient_steps % cfg.algo.critic.target_network_update_freq == 0:
-                        tau = 1 if per_rank_gradient_steps == 0 else cfg.algo.critic.tau
-                        for cp, tcp in zip(critic_task.module.parameters(), target_critic_task.parameters()):
-                            tcp.data.copy_(tau * cp.data + (1 - tau) * tcp.data)
-                        for k in critics_exploration.keys():
-                            for cp, tcp in zip(
-                                critics_exploration[k]["module"].module.parameters(),
-                                critics_exploration[k]["target_module"].parameters(),
-                            ):
-                                tcp.data.copy_(tau * cp.data + (1 - tau) * tcp.data)
-                    batch = {k: v[i].float() for k, v in local_data.items()}
-                    train(
-                        fabric,
-                        world_model,
-                        actor_task,
-                        critic_task,
-                        target_critic_task,
-                        world_optimizer,
-                        actor_task_optimizer,
-                        critic_task_optimizer,
-                        batch,
-                        aggregator,
-                        cfg,
-                        ensembles=ensembles,
-                        ensemble_optimizer=ensemble_optimizer,
-                        actor_exploration=actor_exploration,
-                        critics_exploration=critics_exploration,
-                        actor_exploration_optimizer=actor_exploration_optimizer,
-                        is_continuous=is_continuous,
-                        actions_dim=actions_dim,
-                        moments_exploration=moments_exploration,
-                        moments_task=moments_task,
-                    )
-                train_step += world_size
-            updates_before_training = cfg.algo.train_every // policy_steps_per_update
-            if cfg.algo.actor.expl_decay:
-                expl_decay_steps += 1
-                actor_task.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
-                )
-                actor_exploration.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
+        if update >= learning_starts:
+            per_rank_gradient_steps = ratio(policy_step / world_size)
+            if per_rank_gradient_steps > 0:
+                local_data = rb.sample_tensors(
+                    cfg.algo.per_rank_batch_size,
+                    sequence_length=cfg.algo.per_rank_sequence_length,
+                    n_samples=per_rank_gradient_steps,
+                    dtype=None,
+                    device=fabric.device,
+                    from_numpy=cfg.buffer.from_numpy,
                 )
-            if aggregator and not aggregator.disabled:
-                aggregator.update("Params/exploration_amount_task", actor_task.expl_amount)
-                aggregator.update("Params/exploration_amount_exploration", actor_exploration.expl_amount)
+                # Start training
+                with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
+                    for i in range(per_rank_gradient_steps):
+                        if (
+                            cumulative_per_rank_gradient_steps % cfg.algo.critic.per_rank_target_network_update_freq
+                            == 0
+                        ):
+                            tau = 1 if cumulative_per_rank_gradient_steps == 0 else cfg.algo.critic.tau
+                            for cp, tcp in zip(critic_task.module.parameters(), target_critic_task.parameters()):
+                                tcp.data.copy_(tau * cp.data + (1 - tau) * tcp.data)
+                            for k in critics_exploration.keys():
+                                for cp, tcp in zip(
+                                    critics_exploration[k]["module"].module.parameters(),
+                                    critics_exploration[k]["target_module"].parameters(),
+                                ):
+                                    tcp.data.copy_(tau * cp.data + (1 - tau) * tcp.data)
+                        batch = {k: v[i].float() for k, v in local_data.items()}
+                        train(
+                            fabric,
+                            world_model,
+                            actor_task,
+                            critic_task,
+                            target_critic_task,
+                            world_optimizer,
+                            actor_task_optimizer,
+                            critic_task_optimizer,
+                            batch,
+                            aggregator,
+                            cfg,
+                            ensembles=ensembles,
+                            ensemble_optimizer=ensemble_optimizer,
+                            actor_exploration=actor_exploration,
+                            critics_exploration=critics_exploration,
+                            actor_exploration_optimizer=actor_exploration_optimizer,
+                            is_continuous=is_continuous,
+                            actions_dim=actions_dim,
+                            moments_exploration=moments_exploration,
+                            moments_task=moments_task,
+                        )
+                        cumulative_per_rank_gradient_steps += 1
+                    train_step += world_size
 
         # Log metrics
         if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -1056,15 +1001,15 @@
                 "critic_task": critic_task.state_dict(),
                 "target_critic_task": target_critic_task.state_dict(),
                 "ensembles": ensembles.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
                 "ensemble_optimizer": ensemble_optimizer.state_dict(),
-                "expl_decay_steps": expl_decay_steps,
+                "ratio": ratio.state_dict(),
                 "update": update * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "actor_exploration_optimizer": actor_exploration_optimizer.state_dict(),
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
                 "moments_task": moments_task.state_dict(),
@@ -1078,17 +1023,18 @@
                 state=state,
                 replay_buffer=rb if cfg.buffer.checkpoint else None,
             )
 
     envs.close()
     # task test zero-shot
     if fabric.is_global_zero and cfg.algo.run_test:
-        player.actor = actor_task.module
         player.actor_type = "task"
-        test(player, fabric, cfg, log_dir, "zero-shot")
+        fabric_player = get_single_device_fabric(fabric)
+        player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
+        test(player, fabric, cfg, log_dir, "zero-shot", greedy=False)
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.dreamer_v1.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
         models_to_log = {
             "world_model": world_model,
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,46 @@
+from __future__ import annotations
+
 import copy
 import os
 import pathlib
 import warnings
 from typing import Any, Dict
 
 import gymnasium as gym
 import hydra
 import numpy as np
 import torch
 from lightning.fabric import Fabric
 from torchmetrics import SumMetric
 
-from sheeprl.algos.dreamer_v3.agent import PlayerDV3
-from sheeprl.algos.dreamer_v3.dreamer_v3 import train
-from sheeprl.algos.dreamer_v3.utils import Moments, test
-from sheeprl.algos.p2e_dv3.agent import build_agent
-from sheeprl.data.buffers import EnvIndependentReplayBuffer, SequentialReplayBuffer
+from sheeprl.algos.dreamer_v2.dreamer_v2 import train
+from sheeprl.algos.dreamer_v2.utils import prepare_obs, test
+from sheeprl.algos.p2e_dv2.agent import build_agent
+from sheeprl.data.buffers import EnvIndependentReplayBuffer, EpisodeBuffer, SequentialReplayBuffer
 from sheeprl.utils.env import make_env
+from sheeprl.utils.fabric import get_single_device_fabric
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import polynomial_decay, save_configs
+from sheeprl.utils.utils import Ratio, save_configs, unwrap_fabric
+
+# Decomment the following line if you are using MineDojo on an headless machine
+# os.environ["MINEDOJO_HEADLESS"] = "1"
 
 
 @register_algorithm()
 def main(fabric: Fabric, cfg: Dict[str, Any], exploration_cfg: Dict[str, Any]):
+    # Single-device fabric object
+    fabric_player = get_single_device_fabric(fabric)
+
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     ckpt_path = pathlib.Path(cfg.checkpoint.exploration_ckpt_path)
     resume_from_checkpoint = cfg.checkpoint.resume_from is not None
 
     # Finetuning that was interrupted for some reason
     if resume_from_checkpoint:
         state = fabric.load(pathlib.Path(cfg.checkpoint.resume_from))
@@ -64,14 +70,15 @@
     if cfg.buffer.load_from_exploration and exploration_cfg.buffer.checkpoint:
         cfg.env.num_envs = exploration_cfg.env.num_envs
     # There must be the same cnn and mlp keys during exploration and finetuning
     cfg.algo.cnn_keys = exploration_cfg.algo.cnn_keys
     cfg.algo.mlp_keys = exploration_cfg.algo.mlp_keys
 
     # These arguments cannot be changed
+    cfg.env.screen_size = 64
     cfg.env.frame_stack = 1
 
     # Create Logger. This will create the logger only on the
     # rank-0 process
     logger = get_logger(fabric, cfg)
     if logger and fabric.is_global_zero:
         fabric._loggers = [logger]
@@ -124,50 +131,28 @@
     if cfg.metric.log_level > 0:
         fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
         fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
         fabric.print("Decoder CNN keys:", cfg.algo.cnn_keys.decoder)
         fabric.print("Decoder MLP keys:", cfg.algo.mlp_keys.decoder)
     obs_keys = cfg.algo.cnn_keys.encoder + cfg.algo.mlp_keys.encoder
 
-    (
-        world_model,
-        _,
-        actor_task,
-        critic_task,
-        target_critic_task,
-        actor_exploration,
-        _,
-    ) = build_agent(
+    world_model, _, actor_task, critic_task, target_critic_task, actor_exploration, _, _, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["world_model"],
         None,
         state["actor_task"],
         state["critic_task"],
         state["target_critic_task"],
         state["actor_exploration"],
     )
 
-    # initialize the ensembles with different seeds to be sure they have different weights
-    player = PlayerDV3(
-        world_model.encoder.module,
-        world_model.rssm,
-        actor_exploration.module if cfg.algo.player.actor_type == "exploration" else actor_task.module,
-        actions_dim,
-        cfg.env.num_envs,
-        cfg.algo.world_model.stochastic_size,
-        cfg.algo.world_model.recurrent_model.recurrent_state_size,
-        fabric.device,
-        discrete_size=cfg.algo.world_model.discrete_size,
-        actor_type=cfg.algo.player.actor_type,
-    )
-
     # Optimizers
     world_optimizer = hydra.utils.instantiate(
         cfg.algo.world_model.optimizer, params=world_model.parameters(), _convert_="all"
     )
     actor_task_optimizer = hydra.utils.instantiate(
         cfg.algo.actor.optimizer, params=actor_task.parameters(), _convert_="all"
     )
@@ -177,84 +162,81 @@
     world_optimizer.load_state_dict(state["world_optimizer"])
     actor_task_optimizer.load_state_dict(state["actor_task_optimizer"])
     critic_task_optimizer.load_state_dict(state["critic_task_optimizer"])
     world_optimizer, actor_task_optimizer, critic_task_optimizer = fabric.setup_optimizers(
         world_optimizer, actor_task_optimizer, critic_task_optimizer
     )
 
-    moments_task = Moments(
-        cfg.algo.actor.moments.decay,
-        cfg.algo.actor.moments.max,
-        cfg.algo.actor.moments.percentile.low,
-        cfg.algo.actor.moments.percentile.high,
-    )
-    moments_task.load_state_dict(state["moments_task"])
-
     if fabric.is_global_zero:
         save_configs(cfg, log_dir)
 
     # Metrics
     aggregator = None
     if not MetricAggregator.disabled:
         aggregator: MetricAggregator = hydra.utils.instantiate(cfg.metric.aggregator, _convert_="all").to(device)
 
     # Local data
     buffer_size = cfg.buffer.size // int(cfg.env.num_envs * world_size) if not cfg.dry_run else 4
-    rb = EnvIndependentReplayBuffer(
-        buffer_size,
-        n_envs=cfg.env.num_envs,
-        memmap=cfg.buffer.memmap,
-        memmap_dir=os.path.join(log_dir, "memmap_buffer", f"rank_{fabric.global_rank}"),
-        buffer_cls=SequentialReplayBuffer,
-    )
+    buffer_type = cfg.buffer.type.lower()
+    if buffer_type == "sequential":
+        rb = EnvIndependentReplayBuffer(
+            buffer_size,
+            n_envs=cfg.env.num_envs,
+            obs_keys=obs_keys,
+            memmap=cfg.buffer.memmap,
+            memmap_dir=os.path.join(log_dir, "memmap_buffer", f"rank_{fabric.global_rank}"),
+            buffer_cls=SequentialReplayBuffer,
+        )
+    elif buffer_type == "episode":
+        rb = EpisodeBuffer(
+            buffer_size,
+            minimum_episode_length=1 if cfg.dry_run else cfg.algo.per_rank_sequence_length,
+            n_envs=cfg.env.num_envs,
+            obs_keys=obs_keys,
+            prioritize_ends=cfg.buffer.prioritize_ends,
+            memmap=cfg.buffer.memmap,
+            memmap_dir=os.path.join(log_dir, "memmap_buffer", f"rank_{fabric.global_rank}"),
+        )
+    else:
+        raise ValueError(f"Unrecognized buffer type: must be one of `sequential` or `episode`, received: {buffer_type}")
     if resume_from_checkpoint or (cfg.buffer.load_from_exploration and exploration_cfg.buffer.checkpoint):
         if isinstance(state["rb"], list) and world_size == len(state["rb"]):
             rb = state["rb"][fabric.global_rank]
-        elif isinstance(state["rb"], EnvIndependentReplayBuffer):
+        elif isinstance(state["rb"], (EnvIndependentReplayBuffer, EpisodeBuffer)):
             rb = state["rb"]
         else:
             raise RuntimeError(f"Given {len(state['rb'])}, but {world_size} processes are instantiated")
-    expl_decay_steps = state["expl_decay_steps"] if resume_from_checkpoint else 0
 
     # Global variables
     train_step = 0
     last_train = 0
     start_step = (
         # + 1 because the checkpoint is at the end of the update step
         # (when resuming from a checkpoint, the update at the checkpoint
         # is ended and you have to start with the next one)
-        (state["update"] // fabric.world_size) + 1
+        (state["update"] // world_size) + 1
         if resume_from_checkpoint
         else 1
     )
     policy_step = state["update"] * cfg.env.num_envs if resume_from_checkpoint else 0
     last_log = state["last_log"] if resume_from_checkpoint else 0
     last_checkpoint = state["last_checkpoint"] if resume_from_checkpoint else 0
-    policy_steps_per_update = int(cfg.env.num_envs * fabric.world_size)
-    updates_before_training = cfg.algo.train_every // policy_steps_per_update
-    num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
+    policy_steps_per_update = int(cfg.env.num_envs * world_size)
+    num_updates = cfg.algo.total_steps // policy_steps_per_update if not cfg.dry_run else 1
     learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
-    max_step_expl_decay = cfg.algo.actor.max_step_expl_decay // (cfg.algo.per_rank_gradient_steps * fabric.world_size)
     if resume_from_checkpoint:
         cfg.algo.per_rank_batch_size = state["batch_size"] // world_size
-        actor_task.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
-        actor_exploration.expl_amount = polynomial_decay(
-            expl_decay_steps,
-            initial=cfg.algo.actor.expl_amount,
-            final=cfg.algo.actor.expl_min,
-            max_decay_steps=max_step_expl_decay,
-        )
         if not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -268,176 +250,161 @@
         )
 
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]
     for k in obs_keys:
         step_data[k] = obs[k][np.newaxis]
-    step_data["dones"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["terminated"] = np.zeros((1, cfg.env.num_envs, 1))
+    step_data["truncated"] = np.zeros((1, cfg.env.num_envs, 1))
+    if cfg.dry_run:
+        step_data["terminated"] = step_data["terminated"] + 1
+        step_data["truncated"] = step_data["truncated"] + 1
+    step_data["actions"] = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     step_data["rewards"] = np.zeros((1, cfg.env.num_envs, 1))
-    step_data["is_first"] = np.ones_like(step_data["dones"])
+    step_data["is_first"] = np.ones_like(step_data["terminated"])
+    rb.add(step_data, validate_args=cfg.buffer.validate_args)
     player.init_states()
 
-    per_rank_gradient_steps = 0
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * world_size
 
-        # Measure environment interaction time: this considers both the model forward
-        # to get the action given the observation and the time taken into the environment
-        with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            with torch.no_grad():
-                preprocessed_obs = {}
-                for k, v in obs.items():
-                    preprocessed_obs[k] = torch.as_tensor(v[np.newaxis], dtype=torch.float32, device=device)
-                    if k in cfg.algo.cnn_keys.encoder:
-                        preprocessed_obs[k] = preprocessed_obs[k] / 255.0 - 0.5
-                mask = {k: v for k, v in preprocessed_obs.items() if k.startswith("mask")}
+        with torch.inference_mode():
+            # Measure environment interaction time: this considers both the model forward
+            # to get the action given the observation and the time taken into the environment
+            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
+                torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                mask = {k: v for k, v in torch_obs.items() if k.startswith("mask")}
                 if len(mask) == 0:
                     mask = None
-                real_actions = actions = player.get_exploration_action(preprocessed_obs, mask)
-                actions = torch.cat(actions, -1).cpu().numpy()
+                real_actions = actions = player.get_actions(torch_obs, mask=mask)
+                actions = torch.cat(actions, -1).view(cfg.env.num_envs, -1).cpu().numpy()
                 if is_continuous:
-                    real_actions = torch.cat(real_actions, dim=-1).cpu().numpy()
+                    real_actions = torch.cat(real_actions, -1).cpu().numpy()
                 else:
                     real_actions = (
                         torch.cat([real_act.argmax(dim=-1) for real_act in real_actions], dim=-1).cpu().numpy()
                     )
 
-            step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
-            rb.add(step_data, validate_args=cfg.buffer.validate_args)
+                step_data["is_first"] = copy.deepcopy(np.logical_or(step_data["terminated"], step_data["truncated"]))
+                next_obs, rewards, terminated, truncated, infos = envs.step(
+                    real_actions.reshape(envs.action_space.shape)
+                )
+                dones = np.logical_or(terminated, truncated).astype(np.uint8)
+                if cfg.dry_run and buffer_type == "episode":
+                    dones = np.ones_like(dones)
+
+            if cfg.metric.log_level > 0 and "final_info" in infos:
+                for i, agent_ep_info in enumerate(infos["final_info"]):
+                    if agent_ep_info is not None:
+                        ep_rew = agent_ep_info["episode"]["r"]
+                        ep_len = agent_ep_info["episode"]["l"]
+                        if aggregator and not aggregator.disabled:
+                            aggregator.update("Rewards/rew_avg", ep_rew)
+                            aggregator.update("Game/ep_len_avg", ep_len)
+                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+
+            # Save the real next observation
+            real_next_obs = copy.deepcopy(next_obs)
+            if "final_observation" in infos:
+                for idx, final_obs in enumerate(infos["final_observation"]):
+                    if final_obs is not None:
+                        for k, v in final_obs.items():
+                            real_next_obs[k][idx] = v
 
-            next_obs, rewards, dones, truncated, infos = envs.step(real_actions.reshape(envs.action_space.shape))
-            dones = np.logical_or(dones, truncated).astype(np.uint8)
+            for k in obs_keys:  # [N_envs, N_obs]
+                step_data[k] = real_next_obs[k][np.newaxis]
 
-        step_data["is_first"] = np.zeros_like(step_data["dones"])
-        if "restart_on_exception" in infos:
-            for i, agent_roe in enumerate(infos["restart_on_exception"]):
-                if agent_roe and not dones[i]:
-                    last_inserted_idx = (rb.buffer[i]._pos - 1) % rb.buffer[i].buffer_size
-                    rb.buffer[i]["dones"][last_inserted_idx] = np.ones_like(rb.buffer[i]["dones"][last_inserted_idx])
-                    rb.buffer[i]["is_first"][last_inserted_idx] = np.zeros_like(
-                        rb.buffer[i]["is_first"][last_inserted_idx]
-                    )
-                    step_data["is_first"][i] = np.ones_like(step_data["is_first"][i])
+            # Next_obs becomes the new obs
+            obs = next_obs
 
-        if cfg.metric.log_level > 0 and "final_info" in infos:
-            for i, agent_ep_info in enumerate(infos["final_info"]):
-                if agent_ep_info is not None:
-                    ep_rew = agent_ep_info["episode"]["r"]
-                    ep_len = agent_ep_info["episode"]["l"]
-                    if aggregator and not aggregator.disabled:
-                        aggregator.update("Rewards/rew_avg", ep_rew)
-                        aggregator.update("Game/ep_len_avg", ep_len)
-                    fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
-
-        # Save the real next observation
-        real_next_obs = copy.deepcopy(next_obs)
-        if "final_observation" in infos:
-            for idx, final_obs in enumerate(infos["final_observation"]):
-                if final_obs is not None:
-                    for k, v in final_obs.items():
-                        real_next_obs[k][idx] = v
-
-        for k in obs_keys:
-            step_data[k] = next_obs[k][np.newaxis]
-
-        # next_obs becomes the new obs
-        obs = next_obs
-
-        rewards = rewards.reshape((1, cfg.env.num_envs, -1))
-        step_data["dones"] = dones.reshape((1, cfg.env.num_envs, -1))
-        step_data["rewards"] = clip_rewards_fn(rewards)
-
-        dones_idxes = dones.nonzero()[0].tolist()
-        reset_envs = len(dones_idxes)
-        if reset_envs > 0:
-            reset_data = {}
-            for k in obs_keys:
-                reset_data[k] = (real_next_obs[k][dones_idxes])[np.newaxis]
-            reset_data["dones"] = np.ones((1, reset_envs, 1))
-            reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
-            reset_data["rewards"] = step_data["rewards"][:, dones_idxes]
-            reset_data["is_first"] = np.zeros_like(reset_data["dones"])
-            rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
-
-            # Reset already inserted step data
-            step_data["rewards"][:, dones_idxes] = np.zeros_like(reset_data["rewards"])
-            step_data["dones"][:, dones_idxes] = np.zeros_like(step_data["dones"][:, dones_idxes])
-            step_data["is_first"][:, dones_idxes] = np.ones_like(step_data["is_first"][:, dones_idxes])
-            player.init_states(dones_idxes)
+            step_data["terminated"] = terminated.reshape((1, cfg.env.num_envs, -1))
+            step_data["terminated"] = terminated.reshape((1, cfg.env.num_envs, -1))
+            step_data["actions"] = actions.reshape((1, cfg.env.num_envs, -1))
+            step_data["rewards"] = clip_rewards_fn(rewards).reshape((1, cfg.env.num_envs, -1))
+            rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
-        updates_before_training -= 1
+            # Reset and save the observation coming from the automatic reset
+            dones_idxes = dones.nonzero()[0].tolist()
+            reset_envs = len(dones_idxes)
+            if reset_envs > 0:
+                reset_data = {}
+                for k in obs_keys:
+                    reset_data[k] = (next_obs[k][dones_idxes])[np.newaxis]
+                reset_data["terminated"] = np.zeros((1, reset_envs, 1))
+                reset_data["truncated"] = np.zeros((1, reset_envs, 1))
+                reset_data["actions"] = np.zeros((1, reset_envs, np.sum(actions_dim)))
+                reset_data["rewards"] = np.zeros((1, reset_envs, 1))
+                reset_data["is_first"] = np.ones_like(reset_data["terminated"])
+                rb.add(reset_data, dones_idxes, validate_args=cfg.buffer.validate_args)
+                # Reset dones so that `is_first` is updated
+                for d in dones_idxes:
+                    step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
+                    step_data["terminated"][0, d] = np.zeros_like(step_data["terminated"][0, d])
+                # Reset internal agent states
+                player.init_states(dones_idxes)
 
         # Train the agent
-        if update >= learning_starts and updates_before_training <= 0:
-            if player.actor_type == "exploration":
-                player.actor = actor_task.module
-                player.actor_type = "task"
-            local_data = rb.sample_tensors(
-                cfg.algo.per_rank_batch_size,
-                sequence_length=cfg.algo.per_rank_sequence_length,
-                n_samples=(
-                    cfg.algo.per_rank_pretrain_steps if update == learning_starts else cfg.algo.per_rank_gradient_steps
-                ),
-                dtype=None,
-                device=fabric.device,
-                from_numpy=cfg.buffer.from_numpy,
-            )
-            # Start training
-            with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
-                for i in range(next(iter(local_data.values())).shape[0]):
-                    tau = 1 if per_rank_gradient_steps == 0 else cfg.algo.critic.tau
-                    if per_rank_gradient_steps % cfg.algo.critic.target_network_update_freq == 0:
-                        for cp, tcp in zip(critic_task.module.parameters(), target_critic_task.parameters()):
-                            tcp.data.copy_(tau * cp.data + (1 - tau) * tcp.data)
-                    batch = {k: v[i].float() for k, v in local_data.items()}
-                    train(
-                        fabric,
-                        world_model,
-                        actor_task,
-                        critic_task,
-                        target_critic_task,
-                        world_optimizer,
-                        actor_task_optimizer,
-                        critic_task_optimizer,
-                        batch,
-                        aggregator,
-                        cfg,
-                        is_continuous=is_continuous,
-                        actions_dim=actions_dim,
-                        moments=moments_task,
-                    )
-                train_step += world_size
-            updates_before_training = cfg.algo.train_every // policy_steps_per_update
-            if cfg.algo.actor.expl_decay:
-                expl_decay_steps += 1
-                actor_task.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
-                )
-                actor_exploration.expl_amount = polynomial_decay(
-                    expl_decay_steps,
-                    initial=cfg.algo.actor.expl_amount,
-                    final=cfg.algo.actor.expl_min,
-                    max_decay_steps=max_step_expl_decay,
+        if update >= learning_starts:
+            per_rank_gradient_steps = ratio(policy_step / world_size)
+            if per_rank_gradient_steps > 0:
+                if player.actor_type != "task":
+                    player.actor_type = "task"
+                    player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
+                    for agent_p, p in zip(actor_task.parameters(), player.actor.parameters()):
+                        p.data = agent_p.data
+                local_data = rb.sample_tensors(
+                    batch_size=cfg.algo.per_rank_batch_size,
+                    sequence_length=cfg.algo.per_rank_sequence_length,
+                    n_samples=per_rank_gradient_steps,
+                    dtype=None,
+                    device=fabric.device,
+                    from_numpy=cfg.buffer.from_numpy,
                 )
-            if aggregator and not aggregator.disabled:
-                aggregator.update("Params/exploration_amount_task", actor_task.expl_amount)
-                aggregator.update("Params/exploration_amount_exploration", actor_exploration.expl_amount)
+                # Start training
+                with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
+                    for i in range(per_rank_gradient_steps):
+                        if (
+                            cumulative_per_rank_gradient_steps % cfg.algo.critic.per_rank_target_network_update_freq
+                            == 0
+                        ):
+                            for cp, tcp in zip(critic_task.module.parameters(), target_critic_task.parameters()):
+                                tcp.data.copy_(cp.data)
+                        batch = {k: v[i].float() for k, v in local_data.items()}
+                        train(
+                            fabric,
+                            world_model,
+                            actor_task,
+                            critic_task,
+                            target_critic_task,
+                            world_optimizer,
+                            actor_task_optimizer,
+                            critic_task_optimizer,
+                            batch,
+                            aggregator,
+                            cfg,
+                            actions_dim=actions_dim,
+                        )
+                        cumulative_per_rank_gradient_steps += 1
+                    train_step += world_size
 
         # Log metrics
         if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -465,43 +432,36 @@
                 "world_model": world_model.state_dict(),
                 "actor_task": actor_task.state_dict(),
                 "critic_task": critic_task.state_dict(),
                 "target_critic_task": target_critic_task.state_dict(),
                 "world_optimizer": world_optimizer.state_dict(),
                 "actor_task_optimizer": actor_task_optimizer.state_dict(),
                 "critic_task_optimizer": critic_task_optimizer.state_dict(),
-                "expl_decay_steps": expl_decay_steps,
+                "ratio": ratio.state_dict(),
                 "update": update * world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * world_size,
                 "actor_exploration": actor_exploration.state_dict(),
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
-                "moments_task": moments_task.state_dict(),
             }
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
                 "on_checkpoint_coupled",
                 fabric=fabric,
                 ckpt_path=ckpt_path,
                 state=state,
                 replay_buffer=rb if cfg.buffer.checkpoint else None,
             )
 
     envs.close()
     # task test few-shot
     if fabric.is_global_zero and cfg.algo.run_test:
-        player.actor = actor_task.module
         player.actor_type = "task"
+        player.actor = fabric_player.setup_module(unwrap_fabric(actor_task))
         test(player, fabric, cfg, log_dir, "few-shot")
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.dreamer_v1.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
-        models_to_log = {
-            "world_model": world_model,
-            "actor_task": actor_task,
-            "critic_task": critic_task,
-            "target_critic_task": target_critic_task,
-            "moments_task": moments_task,
-        }
+        models_to_log = {"world_model": world_model, "actor_task": actor_task, "critic_task": critic_task}
         register_model(fabric, log_models, cfg, models_to_log)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/p2e_dv3/utils.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv3/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,14 @@
     "Loss/policy_loss_exploration",
     "Loss/observation_loss",
     "Loss/reward_loss",
     "Loss/state_loss",
     "Loss/continue_loss",
     "Loss/ensemble_loss",
     "State/kl",
-    "Params/exploration_amount_task",
-    "Params/exploration_amount_exploration",
     "State/post_entropy",
     "State/prior_entropy",
     "Grads/world_model",
     "Grads/actor_task",
     "Grads/critic_task",
     "Grads/actor_exploration",
     "Grads/ensemble",
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/ppo/agent.py` & `sheeprl-0.5.5/sheeprl/algos/ppo/agent.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
+import copy
 from math import prod
 from typing import Any, Dict, List, Optional, Sequence, Tuple
 
 import gymnasium
+import hydra
 import torch
 import torch.nn as nn
 from lightning import Fabric
-from lightning.fabric.wrappers import _FabricModule
 from torch import Tensor
-from torch.distributions import Distribution, Independent, Normal
+from torch.distributions import Distribution, Independent, Normal, OneHotCategorical
 
 from sheeprl.models.models import MLP, MultiEncoder, NatureCNN
-from sheeprl.utils.distribution import OneHotCategoricalValidateArgs
+from sheeprl.utils.fabric import get_single_device_fabric
 
 
 class CNNEncoder(nn.Module):
     def __init__(
         self,
         in_channels: int,
         features_dim: int,
@@ -59,14 +60,26 @@
         )
 
     def forward(self, obs: Dict[str, Tensor]) -> Tensor:
         x = torch.cat([obs[k] for k in self.keys], dim=-1)
         return self.model(x)
 
 
+class PPOActor(nn.Module):
+    def __init__(self, actor_backbone: torch.nn.Module, actor_heads: torch.nn.ModuleList, is_continuous: bool) -> None:
+        super().__init__()
+        self.actor_backbone = actor_backbone
+        self.actor_heads = actor_heads
+        self.is_continuous = is_continuous
+
+    def forward(self, x: Tensor) -> List[Tensor]:
+        x = self.actor_backbone(x)
+        return [head(x) for head in self.actor_heads]
+
+
 class PPOAgent(nn.Module):
     def __init__(
         self,
         actions_dim: Sequence[int],
         obs_space: gymnasium.spaces.Dict,
         encoder_cfg: Dict[str, Any],
         actor_cfg: Dict[str, Any],
@@ -74,14 +87,15 @@
         cnn_keys: Sequence[str],
         mlp_keys: Sequence[str],
         screen_size: int,
         distribution_cfg: Dict[str, Any],
         is_continuous: bool = False,
     ):
         super().__init__()
+        self.is_continuous = is_continuous
         self.distribution_cfg = distribution_cfg
         self.actions_dim = actions_dim
         in_channels = sum([prod(obs_space[k].shape[:-2]) for k in cnn_keys])
         mlp_input_dim = sum([obs_space[k].shape[0] for k in mlp_keys])
         cnn_encoder = (
             CNNEncoder(in_channels, encoder_cfg.cnn_features_dim, screen_size, cnn_keys)
             if cnn_keys is not None and len(cnn_keys) > 0
@@ -90,74 +104,67 @@
         mlp_encoder = (
             MLPEncoder(
                 mlp_input_dim,
                 encoder_cfg.mlp_features_dim,
                 mlp_keys,
                 encoder_cfg.dense_units,
                 encoder_cfg.mlp_layers,
-                eval(encoder_cfg.dense_act),
+                hydra.utils.get_class(encoder_cfg.dense_act),
                 encoder_cfg.layer_norm,
             )
             if mlp_keys is not None and len(mlp_keys) > 0
             else None
         )
         self.feature_extractor = MultiEncoder(cnn_encoder, mlp_encoder)
-        self.is_continuous = is_continuous
         features_dim = self.feature_extractor.output_dim
         self.critic = MLP(
             input_dims=features_dim,
             output_dim=1,
             hidden_sizes=[critic_cfg.dense_units] * critic_cfg.mlp_layers,
-            activation=eval(critic_cfg.dense_act),
+            activation=hydra.utils.get_class(critic_cfg.dense_act),
             norm_layer=[nn.LayerNorm for _ in range(critic_cfg.mlp_layers)] if critic_cfg.layer_norm else None,
             norm_args=(
                 [{"normalized_shape": critic_cfg.dense_units} for _ in range(critic_cfg.mlp_layers)]
                 if critic_cfg.layer_norm
                 else None
             ),
         )
-        self.actor_backbone = (
+        actor_backbone = (
             MLP(
                 input_dims=features_dim,
                 output_dim=None,
                 hidden_sizes=[actor_cfg.dense_units] * actor_cfg.mlp_layers,
-                activation=eval(actor_cfg.dense_act),
+                activation=hydra.utils.get_class(actor_cfg.dense_act),
                 flatten_dim=None,
                 norm_layer=[nn.LayerNorm] * actor_cfg.mlp_layers if actor_cfg.layer_norm else None,
                 norm_args=(
                     [{"normalized_shape": actor_cfg.dense_units} for _ in range(actor_cfg.mlp_layers)]
                     if actor_cfg.layer_norm
                     else None
                 ),
             )
             if actor_cfg.mlp_layers > 0
             else nn.Identity()
         )
         if is_continuous:
-            self.actor_heads = nn.ModuleList([nn.Linear(actor_cfg.dense_units, sum(actions_dim) * 2)])
+            actor_heads = nn.ModuleList([nn.Linear(actor_cfg.dense_units, sum(actions_dim) * 2)])
         else:
-            self.actor_heads = nn.ModuleList(
-                [nn.Linear(actor_cfg.dense_units, action_dim) for action_dim in actions_dim]
-            )
+            actor_heads = nn.ModuleList([nn.Linear(actor_cfg.dense_units, action_dim) for action_dim in actions_dim])
+        self.actor = PPOActor(actor_backbone, actor_heads, is_continuous)
 
     def forward(
         self, obs: Dict[str, Tensor], actions: Optional[List[Tensor]] = None
     ) -> Tuple[Sequence[Tensor], Tensor, Tensor, Tensor]:
         feat = self.feature_extractor(obs)
-        out: Tensor = self.actor_backbone(feat)
-        pre_dist: List[Tensor] = [head(out) for head in self.actor_heads]
+        actor_out: List[Tensor] = self.actor(feat)
         values = self.critic(feat)
         if self.is_continuous:
-            mean, log_std = torch.chunk(pre_dist[0], chunks=2, dim=-1)
+            mean, log_std = torch.chunk(actor_out[0], chunks=2, dim=-1)
             std = log_std.exp()
-            normal = Independent(
-                Normal(mean, std, validate_args=self.distribution_cfg.validate_args),
-                1,
-                validate_args=self.distribution_cfg.validate_args,
-            )
+            normal = Independent(Normal(mean, std), 1)
             if actions is None:
                 actions = normal.sample()
             else:
                 # always composed by a tuple of one element containing all the
                 # continuous actions
                 actions = actions[0]
             log_prob = normal.log_prob(actions)
@@ -166,66 +173,126 @@
             should_append = False
             actions_logprobs: List[Tensor] = []
             actions_entropies: List[Tensor] = []
             actions_dist: List[Distribution] = []
             if actions is None:
                 should_append = True
                 actions: List[Tensor] = []
-            for i, logits in enumerate(pre_dist):
-                actions_dist.append(
-                    OneHotCategoricalValidateArgs(logits=logits, validate_args=self.distribution_cfg.validate_args)
-                )
+            for i, logits in enumerate(actor_out):
+                actions_dist.append(OneHotCategorical(logits=logits))
                 actions_entropies.append(actions_dist[-1].entropy())
                 if should_append:
                     actions.append(actions_dist[-1].sample())
                 actions_logprobs.append(actions_dist[-1].log_prob(actions[i]))
             return (
                 tuple(actions),
                 torch.stack(actions_logprobs, dim=-1).sum(dim=-1, keepdim=True),
                 torch.stack(actions_entropies, dim=-1).sum(dim=-1, keepdim=True),
                 values,
             )
 
-    def get_value(self, obs: Dict[str, Tensor]) -> Tensor:
+
+class PPOPlayer(nn.Module):
+    def __init__(self, feature_extractor: MultiEncoder, actor: PPOActor, critic: nn.Module) -> None:
+        super().__init__()
+        self.feature_extractor = feature_extractor
+        self.critic = critic
+        self.actor = actor
+
+    def forward(self, obs: Dict[str, Tensor]) -> Tuple[Sequence[Tensor], Tensor, Tensor]:
+        feat = self.feature_extractor(obs)
+        values = self.critic(feat)
+        actor_out: List[Tensor] = self.actor(feat)
+        if self.actor.is_continuous:
+            mean, log_std = torch.chunk(actor_out[0], chunks=2, dim=-1)
+            std = log_std.exp()
+            normal = Independent(Normal(mean, std), 1)
+            actions = normal.sample()
+            log_prob = normal.log_prob(actions)
+            return tuple([actions]), log_prob.unsqueeze(dim=-1), values
+        else:
+            actions_dist: List[Distribution] = []
+            actions_logprobs: List[Tensor] = []
+            actions: List[Tensor] = []
+            for i, logits in enumerate(actor_out):
+                actions_dist.append(OneHotCategorical(logits=logits))
+                actions.append(actions_dist[-1].sample())
+                actions_logprobs.append(actions_dist[-1].log_prob(actions[i]))
+            return (
+                tuple(actions),
+                torch.stack(actions_logprobs, dim=-1).sum(dim=-1, keepdim=True),
+                values,
+            )
+
+    def get_values(self, obs: Dict[str, Tensor]) -> Tensor:
         feat = self.feature_extractor(obs)
         return self.critic(feat)
 
-    def get_greedy_actions(self, obs: Dict[str, Tensor]) -> Sequence[Tensor]:
+    def get_actions(self, obs: Dict[str, Tensor], greedy: bool = False) -> Sequence[Tensor]:
         feat = self.feature_extractor(obs)
-        out = self.actor_backbone(feat)
-        pre_dist: List[Tensor] = [head(out) for head in self.actor_heads]
-        if self.is_continuous:
-            return [torch.chunk(pre_dist[0], 2, -1)[0]]
+        actor_out: List[Tensor] = self.actor(feat)
+        if self.actor.is_continuous:
+            mean, log_std = torch.chunk(actor_out[0], chunks=2, dim=-1)
+            if greedy:
+                actions = mean
+            else:
+                std = log_std.exp()
+                normal = Independent(Normal(mean, std), 1)
+                actions = normal.sample()
+            return tuple([actions])
         else:
-            return tuple(
-                [
-                    OneHotCategoricalValidateArgs(logits=logits, validate_args=self.distribution_cfg.validate_args).mode
-                    for logits in pre_dist
-                ]
-            )
+            actions: List[Tensor] = []
+            actions_dist: List[Distribution] = []
+            for logits in actor_out:
+                actions_dist.append(OneHotCategorical(logits=logits))
+                if greedy:
+                    actions.append(actions_dist[-1].mode)
+                else:
+                    actions.append(actions_dist[-1].sample())
+            return tuple(actions)
 
 
 def build_agent(
     fabric: Fabric,
     actions_dim: Sequence[int],
     is_continuous: bool,
     cfg: Dict[str, Any],
     obs_space: gymnasium.spaces.Dict,
     agent_state: Optional[Dict[str, Tensor]] = None,
-) -> _FabricModule:
+) -> Tuple[PPOAgent, PPOPlayer]:
     agent = PPOAgent(
         actions_dim=actions_dim,
         obs_space=obs_space,
         encoder_cfg=cfg.algo.encoder,
         actor_cfg=cfg.algo.actor,
         critic_cfg=cfg.algo.critic,
         cnn_keys=cfg.algo.cnn_keys.encoder,
         mlp_keys=cfg.algo.mlp_keys.encoder,
         screen_size=cfg.env.screen_size,
         distribution_cfg=cfg.distribution,
         is_continuous=is_continuous,
     )
     if agent_state:
         agent.load_state_dict(agent_state)
-    agent = fabric.setup_module(agent)
 
-    return agent
+    # Setup player agent
+    player = PPOPlayer(copy.deepcopy(agent.feature_extractor), copy.deepcopy(agent.actor), copy.deepcopy(agent.critic))
+
+    # Setup training agent
+    agent.feature_extractor = fabric.setup_module(agent.feature_extractor)
+    agent.critic = fabric.setup_module(agent.critic)
+    agent.actor = fabric.setup_module(agent.actor)
+
+    # Setup player agent
+    fabric_player = get_single_device_fabric(fabric)
+    player.feature_extractor = fabric_player.setup_module(player.feature_extractor)
+    player.critic = fabric_player.setup_module(player.critic)
+    player.actor = fabric_player.setup_module(player.actor)
+
+    # Tie weights between the agent and the player
+    for agent_p, player_p in zip(agent.feature_extractor.parameters(), player.feature_extractor.parameters()):
+        player_p.data = agent_p.data
+    for agent_p, player_p in zip(agent.actor.parameters(), player.actor.parameters()):
+        player_p.data = agent_p.data
+    for agent_p, player_p in zip(agent.critic.parameters(), player.critic.parameters()):
+        player_p.data = agent_p.data
+    return agent, player
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/ppo/evaluate.py` & `sheeprl-0.5.5/sheeprl/algos/ppo/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     is_multidiscrete = isinstance(env.action_space, gym.spaces.MultiDiscrete)
     actions_dim = tuple(
         env.action_space.shape
         if is_continuous
         else (env.action_space.nvec.tolist() if is_multidiscrete else [env.action_space.n])
     )
     # Create the actor and critic models
-    agent = build_agent(fabric, actions_dim, is_continuous, cfg, observation_space, state["agent"])
+    _, agent = build_agent(fabric, actions_dim, is_continuous, cfg, observation_space, state["agent"])
+    del _
     test(agent, fabric, cfg, log_dir)
 
 
 # This is just for showcase
 @register_evaluation(algorithms="ppo_decoupled")
 def evaluate_ppo_decoupled(fabric: Fabric, cfg: Dict[str, Any], state: Dict[str, Any]):
     evaluate_ppo(fabric, cfg, state)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/ppo/loss.py` & `sheeprl-0.5.5/sheeprl/algos/ppo/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/algos/ppo/ppo.py` & `sheeprl-0.5.5/sheeprl/algos/ppo/ppo.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from lightning.fabric.wrappers import _FabricModule
 from torch import nn
 from torch.utils.data import BatchSampler, DistributedSampler, RandomSampler
 from torchmetrics import SumMetric
 
 from sheeprl.algos.ppo.agent import build_agent
 from sheeprl.algos.ppo.loss import entropy_loss, policy_loss, value_loss
-from sheeprl.algos.ppo.utils import normalize_obs, test
+from sheeprl.algos.ppo.utils import normalize_obs, prepare_obs, test
 from sheeprl.data.buffers import ReplayBuffer
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
 from sheeprl.utils.utils import gae, normalize_tensor, polynomial_decay, save_configs
@@ -115,16 +115,14 @@
     initial_ent_coef = copy.deepcopy(cfg.algo.ent_coef)
     initial_clip_coef = copy.deepcopy(cfg.algo.clip_coef)
 
     # Initialize Fabric
     rank = fabric.global_rank
     world_size = fabric.world_size
     device = fabric.device
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     # Resume from checkpoint
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     # Create Logger. This will create the logger only on the
     # rank-0 process
@@ -168,15 +166,15 @@
     is_multidiscrete = isinstance(envs.single_action_space, gym.spaces.MultiDiscrete)
     actions_dim = tuple(
         envs.single_action_space.shape
         if is_continuous
         else (envs.single_action_space.nvec.tolist() if is_multidiscrete else [envs.single_action_space.n])
     )
     # Create the actor and critic models
-    agent = build_agent(
+    agent, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["agent"] if cfg.checkpoint.resume_from else None,
     )
@@ -261,100 +259,97 @@
     next_obs = envs.reset(seed=cfg.seed)[0]  # [N_envs, N_obs]
     for k in obs_keys:
         if k in cfg.algo.cnn_keys.encoder:
             next_obs[k] = next_obs[k].reshape(cfg.env.num_envs, -1, *next_obs[k].shape[-2:])
         step_data[k] = next_obs[k][np.newaxis]
 
     for update in range(start_step, num_updates + 1):
-        for _ in range(0, cfg.algo.rollout_steps):
-            policy_step += cfg.env.num_envs * world_size
-
-            # Measure environment interaction time: this considers both the model forward
-            # to get the action given the observation and the time taken into the environment
-            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-                with torch.no_grad():
+        with torch.inference_mode():
+            for _ in range(0, cfg.algo.rollout_steps):
+                policy_step += cfg.env.num_envs * world_size
+
+                # Measure environment interaction time: this considers both the model forward
+                # to get the action given the observation and the time taken into the environment
+                with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                     # Sample an action given the observation received by the environment
-                    normalized_obs = normalize_obs(next_obs, cfg.algo.cnn_keys.encoder, obs_keys)
-                    torch_obs = {
-                        k: torch.as_tensor(normalized_obs[k], dtype=torch.float32, device=device) for k in obs_keys
-                    }
-                    actions, logprobs, _, values = agent.module(torch_obs)
+                    torch_obs = prepare_obs(
+                        fabric, next_obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs
+                    )
+                    actions, logprobs, values = player(torch_obs)
                     if is_continuous:
                         real_actions = torch.cat(actions, -1).cpu().numpy()
                     else:
                         real_actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1).cpu().numpy()
                     actions = torch.cat(actions, -1).cpu().numpy()
 
-                # Single environment step
-                obs, rewards, dones, truncated, info = envs.step(real_actions.reshape(envs.action_space.shape))
-                truncated_envs = np.nonzero(truncated)[0]
-                if len(truncated_envs) > 0:
-                    real_next_obs = {
-                        k: torch.empty(
-                            len(truncated_envs),
-                            *observation_space[k].shape,
-                            dtype=torch.float32,
-                            device=device,
-                        )
-                        for k in obs_keys
-                    }
-                    for i, truncated_env in enumerate(truncated_envs):
-                        for k, v in info["final_observation"][truncated_env].items():
-                            torch_v = torch.as_tensor(v, dtype=torch.float32, device=device)
-                            if k in cfg.algo.cnn_keys.encoder:
-                                torch_v = torch_v.view(-1, *v.shape[-2:])
-                                torch_v = torch_v / 255.0 - 0.5
-                            real_next_obs[k][i] = torch_v
-                    with torch.no_grad():
-                        vals = agent.module.get_value(real_next_obs).cpu().numpy()
-                        rewards[truncated_envs] += vals.reshape(rewards[truncated_envs].shape)
-                dones = np.logical_or(dones, truncated).reshape(cfg.env.num_envs, -1).astype(np.uint8)
-                rewards = rewards.reshape(cfg.env.num_envs, -1)
-
-            # Update the step data
-            step_data["dones"] = dones[np.newaxis]
-            step_data["values"] = values.cpu().numpy()[np.newaxis]
-            step_data["actions"] = actions[np.newaxis]
-            step_data["logprobs"] = logprobs.cpu().numpy()[np.newaxis]
-            step_data["rewards"] = rewards[np.newaxis]
-            if cfg.buffer.memmap:
-                step_data["returns"] = np.zeros_like(rewards, shape=(1, *rewards.shape))
-                step_data["advantages"] = np.zeros_like(rewards, shape=(1, *rewards.shape))
-
-            # Append data to buffer
-            rb.add(step_data, validate_args=cfg.buffer.validate_args)
-
-            # Update the observation and dones
-            next_obs = {}
-            for k in obs_keys:
-                _obs = obs[k]
-                if k in cfg.algo.cnn_keys.encoder:
-                    _obs = _obs.reshape(cfg.env.num_envs, -1, *_obs.shape[-2:])
-                step_data[k] = _obs[np.newaxis]
-                next_obs[k] = _obs
-
-            if cfg.metric.log_level > 0 and "final_info" in info:
-                for i, agent_ep_info in enumerate(info["final_info"]):
-                    if agent_ep_info is not None:
-                        ep_rew = agent_ep_info["episode"]["r"]
-                        ep_len = agent_ep_info["episode"]["l"]
-                        if aggregator and "Rewards/rew_avg" in aggregator:
-                            aggregator.update("Rewards/rew_avg", ep_rew)
-                        if aggregator and "Game/ep_len_avg" in aggregator:
-                            aggregator.update("Game/ep_len_avg", ep_len)
-                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+                    # Single environment step
+                    obs, rewards, terminated, truncated, info = envs.step(real_actions.reshape(envs.action_space.shape))
+                    truncated_envs = np.nonzero(truncated)[0]
+                    if len(truncated_envs) > 0:
+                        real_next_obs = {
+                            k: torch.empty(
+                                len(truncated_envs),
+                                *observation_space[k].shape,
+                                dtype=torch.float32,
+                                device=device,
+                            )
+                            for k in obs_keys
+                        }
+                        for i, truncated_env in enumerate(truncated_envs):
+                            for k, v in info["final_observation"][truncated_env].items():
+                                torch_v = torch.as_tensor(v, dtype=torch.float32, device=device)
+                                if k in cfg.algo.cnn_keys.encoder:
+                                    torch_v = torch_v.view(-1, *v.shape[-2:])
+                                    torch_v = torch_v / 255.0 - 0.5
+                                real_next_obs[k][i] = torch_v
+                        vals = player.get_values(real_next_obs).cpu().numpy()
+                        rewards[truncated_envs] += cfg.algo.gamma * vals.reshape(rewards[truncated_envs].shape)
+                    dones = np.logical_or(terminated, truncated).reshape(cfg.env.num_envs, -1).astype(np.uint8)
+                    rewards = rewards.reshape(cfg.env.num_envs, -1)
+
+                # Update the step data
+                step_data["dones"] = dones[np.newaxis]
+                step_data["values"] = values.cpu().numpy()[np.newaxis]
+                step_data["actions"] = actions[np.newaxis]
+                step_data["logprobs"] = logprobs.cpu().numpy()[np.newaxis]
+                step_data["rewards"] = rewards[np.newaxis]
+                if cfg.buffer.memmap:
+                    step_data["returns"] = np.zeros_like(rewards, shape=(1, *rewards.shape))
+                    step_data["advantages"] = np.zeros_like(rewards, shape=(1, *rewards.shape))
+
+                # Append data to buffer
+                rb.add(step_data, validate_args=cfg.buffer.validate_args)
+
+                # Update the observation and dones
+                next_obs = {}
+                for k in obs_keys:
+                    _obs = obs[k]
+                    if k in cfg.algo.cnn_keys.encoder:
+                        _obs = _obs.reshape(cfg.env.num_envs, -1, *_obs.shape[-2:])
+                    step_data[k] = _obs[np.newaxis]
+                    next_obs[k] = _obs
+
+                if cfg.metric.log_level > 0 and "final_info" in info:
+                    for i, agent_ep_info in enumerate(info["final_info"]):
+                        if agent_ep_info is not None:
+                            ep_rew = agent_ep_info["episode"]["r"]
+                            ep_len = agent_ep_info["episode"]["l"]
+                            if aggregator and "Rewards/rew_avg" in aggregator:
+                                aggregator.update("Rewards/rew_avg", ep_rew)
+                            if aggregator and "Game/ep_len_avg" in aggregator:
+                                aggregator.update("Game/ep_len_avg", ep_len)
+                            fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
 
         # Transform the data into PyTorch Tensors
         local_data = rb.to_tensor(dtype=None, device=device, from_numpy=cfg.buffer.from_numpy)
 
         # Estimate returns with GAE (https://arxiv.org/abs/1506.02438)
-        with torch.no_grad():
-            normalized_obs = normalize_obs(next_obs, cfg.algo.cnn_keys.encoder, obs_keys)
-            torch_obs = {k: torch.as_tensor(normalized_obs[k], dtype=torch.float32, device=device) for k in obs_keys}
-            next_values = agent.module.get_value(torch_obs)
+        with torch.inference_mode():
+            torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+            next_values = player.get_values(torch_obs)
             returns, advantages = gae(
                 local_data["rewards"].to(torch.float64),
                 local_data["values"],
                 local_data["dones"],
                 next_values,
                 cfg.algo.rollout_steps,
                 cfg.algo.gamma,
@@ -443,15 +438,15 @@
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call("on_checkpoint_coupled", fabric=fabric, ckpt_path=ckpt_path, state=state)
 
     envs.close()
     if fabric.is_global_zero and cfg.algo.run_test:
-        test(agent.module, fabric, cfg, log_dir)
+        test(player, fabric, cfg, log_dir)
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.ppo.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
         models_to_log = {"agent": agent}
         register_model(fabric, log_models, cfg, models_to_log)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/ppo/ppo_decoupled.py` & `sheeprl-0.5.5/sheeprl/algos/ppo/ppo_decoupled.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,39 +12,42 @@
 from lightning.fabric.plugins.collectives import TorchCollective
 from lightning.fabric.plugins.collectives.collective import CollectibleGroup
 from lightning.fabric.strategies import DDPStrategy
 from torch.distributed.algorithms.join import Join
 from torch.utils.data import BatchSampler, RandomSampler
 from torchmetrics import SumMetric
 
-from sheeprl.algos.ppo.agent import PPOAgent
+from sheeprl.algos.ppo.agent import build_agent
 from sheeprl.algos.ppo.loss import entropy_loss, policy_loss, value_loss
-from sheeprl.algos.ppo.utils import normalize_obs, test
+from sheeprl.algos.ppo.utils import normalize_obs, prepare_obs, test
 from sheeprl.data.buffers import ReplayBuffer
 from sheeprl.utils.env import make_env
+from sheeprl.utils.fabric import get_single_device_fabric
 from sheeprl.utils.logger import get_log_dir
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
 from sheeprl.utils.utils import gae, normalize_tensor, polynomial_decay, save_configs
 
 
-@torch.no_grad()
+@torch.inference_mode()
 def player(
-    fabric: Fabric, cfg: Dict[str, Any], world_collective: TorchCollective, player_trainer_collective: TorchCollective
+    fabric: Fabric,
+    world_collective: TorchCollective,
+    player_trainer_collective: TorchCollective,
+    cfg: Dict[str, Any],
 ):
-    # Initialize the fabric object
-    log_dir = get_log_dir(fabric, cfg.root_dir, cfg.run_name, False)
-    device = fabric.device
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
+    # Initialize Fabric player-only
+    fabric_player = get_single_device_fabric(fabric)
+    log_dir = get_log_dir(fabric_player, cfg.root_dir, cfg.run_name, False)
+    device = fabric_player.device
 
     # Resume from checkpoint
     if cfg.checkpoint.resume_from:
-        state = fabric.load(cfg.checkpoint.resume_from)
+        state = fabric_player.load(cfg.checkpoint.resume_from)
 
     # Environment setup
     vectorized_env = gym.vector.SyncVectorEnv if cfg.env.sync_env else gym.vector.AsyncVectorEnv
     envs = vectorized_env(
         [
             make_env(
                 cfg,
@@ -88,15 +91,23 @@
         "critic_cfg": cfg.algo.critic,
         "cnn_keys": cfg.algo.cnn_keys.encoder,
         "mlp_keys": cfg.algo.mlp_keys.encoder,
         "screen_size": cfg.env.screen_size,
         "distribution_cfg": cfg.distribution,
         "is_continuous": is_continuous,
     }
-    agent = PPOAgent(**agent_args).to(device)
+    _, agent = build_agent(
+        fabric_player,
+        actions_dim=actions_dim,
+        is_continuous=is_continuous,
+        cfg=cfg,
+        obs_space=observation_space,
+        agent_state=state["agent"] if cfg.checkpoint.resume_from else None,
+    )
+    del _
 
     if fabric.is_global_zero:
         save_configs(cfg, log_dir)
     # Send (possibly updated, by the make_env method for example) cfg to the trainers
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // (world_collective.world_size - 1)
     cfg.checkpoint.log_dir = log_dir
@@ -188,29 +199,25 @@
     for _ in range(start_step, num_updates + 1):
         for _ in range(0, cfg.algo.rollout_steps):
             policy_step += cfg.env.num_envs
 
             # Measure environment interaction time: this considers both the model forward
             # to get the action given the observation and the time taken into the environment
             with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-                with torch.no_grad():
-                    # Sample an action given the observation received by the environment
-                    normalized_obs = normalize_obs(next_obs, cfg.algo.cnn_keys.encoder, obs_keys)
-                    torch_obs = {
-                        k: torch.as_tensor(normalized_obs[k], dtype=torch.float32, device=device) for k in obs_keys
-                    }
-                    actions, logprobs, _, values = agent(torch_obs)
-                    if is_continuous:
-                        real_actions = torch.cat(actions, -1).cpu().numpy()
-                    else:
-                        real_actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1).cpu().numpy()
-                    actions = torch.cat(actions, -1).cpu().numpy()
+                # Sample an action given the observation received by the environment
+                torch_obs = prepare_obs(fabric, next_obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                actions, logprobs, values = agent(torch_obs)
+                if is_continuous:
+                    real_actions = torch.cat(actions, -1).cpu().numpy()
+                else:
+                    real_actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1).cpu().numpy()
+                actions = torch.cat(actions, -1).cpu().numpy()
 
                 # Single environment step
-                obs, rewards, dones, truncated, info = envs.step(real_actions.reshape(envs.action_space.shape))
+                obs, rewards, terminated, truncated, info = envs.step(real_actions.reshape(envs.action_space.shape))
                 truncated_envs = np.nonzero(truncated)[0]
                 if len(truncated_envs) > 0:
                     real_next_obs = {
                         k: torch.empty(
                             len(truncated_envs),
                             *observation_space[k].shape,
                             dtype=torch.float32,
@@ -221,24 +228,23 @@
                     for i, truncated_env in enumerate(truncated_envs):
                         for k, v in info["final_observation"][truncated_env].items():
                             torch_v = torch.as_tensor(v, dtype=torch.float32, device=device)
                             if k in cfg.algo.cnn_keys.encoder:
                                 torch_v = torch_v.view(-1, *v.shape[-2:])
                                 torch_v = torch_v / 255.0 - 0.5
                             real_next_obs[k][i] = torch_v
-                    with torch.no_grad():
-                        vals = agent.get_value(real_next_obs).cpu().numpy()
-                        rewards[truncated_envs] += vals.reshape(rewards[truncated_envs].shape)
-                dones = np.logical_or(dones, truncated).reshape(cfg.env.num_envs, -1).astype(np.uint8)
+                    vals = agent.get_values(real_next_obs).cpu().numpy()
+                    rewards[truncated_envs] += cfg.algo.gamma * vals.reshape(rewards[truncated_envs].shape)
+                dones = np.logical_or(terminated, truncated).reshape(cfg.env.num_envs, -1).astype(np.uint8)
                 rewards = rewards.reshape(cfg.env.num_envs, -1)
 
             # Update the step data
             step_data["dones"] = dones[np.newaxis]
             step_data["values"] = values.cpu().numpy()[np.newaxis]
-            step_data["actions"] = actions[np.newaxis]
+            step_data["actions"] = actions.reshape(1, cfg.env.num_envs, -1)
             step_data["logprobs"] = logprobs.cpu().numpy()[np.newaxis]
             step_data["rewards"] = rewards[np.newaxis]
             if cfg.buffer.memmap:
                 step_data["returns"] = np.zeros_like(rewards, shape=(1, *rewards.shape))
                 step_data["advantages"] = np.zeros_like(rewards, shape=(1, *rewards.shape))
 
             # Append data to buffer
@@ -263,17 +269,16 @@
                             aggregator.update("Game/ep_len_avg", ep_len)
                         fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
 
         # Transform the data into PyTorch Tensors
         local_data = rb.to_tensor(dtype=None, device=device, from_numpy=cfg.buffer.from_numpy)
 
         # Estimate returns with GAE (https://arxiv.org/abs/1506.02438)
-        normalized_obs = normalize_obs(next_obs, cfg.algo.cnn_keys.encoder, obs_keys)
-        torch_obs = {k: torch.as_tensor(normalized_obs[k], dtype=torch.float32, device=device) for k in obs_keys}
-        next_values = agent.get_value(torch_obs)
+        torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+        next_values = agent.get_values(torch_obs)
         returns, advantages = gae(
             local_data["rewards"].to(torch.float64),
             local_data["values"],
             local_data["dones"],
             next_values,
             cfg.algo.rollout_steps,
             cfg.algo.gamma,
@@ -373,16 +378,14 @@
     cfg.fabric.pop("loggers", None)
     cfg.fabric.pop("strategy", None)
     fabric: Fabric = hydra.utils.instantiate(
         cfg.fabric, strategy=DDPStrategy(process_group=optimization_pg), _convert_="all"
     )
     fabric.launch()
     device = fabric.device
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     # Resume from checkpoint
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     # Receive (possibly updated, by the make_env method for example) cfg from the player
     data = [None]
@@ -390,24 +393,31 @@
     cfg: Dict[str, Any] = data[0]
 
     # Environment setup
     agent_args = [None]
     world_collective.broadcast_object_list(agent_args, src=0)
 
     # Define the agent and the optimizer
-    agent = PPOAgent(**agent_args[0])
+    agent, _ = build_agent(
+        fabric,
+        actions_dim=agent_args[0]["actions_dim"],
+        is_continuous=agent_args[0]["is_continuous"],
+        cfg=cfg,
+        obs_space=agent_args[0]["obs_space"],
+        agent_state=state["agent"] if cfg.checkpoint.resume_from else None,
+    )
+    del _
     optimizer = hydra.utils.instantiate(cfg.algo.optimizer, params=agent.parameters(), _convert_="all")
 
     # Load the state from the checkpoint
     if cfg.checkpoint.resume_from:
         agent.load_state_dict(state["agent"])
         optimizer.load_state_dict(state["optimizer"])
 
     # Setup agent and optimizer with Fabric
-    agent = fabric.setup_module(agent)
     optimizer = fabric.setup_optimizers(optimizer)
 
     # Send weights to rank-0, a.k.a. the player
     if global_rank == 1:
         player_trainer_collective.broadcast(
             torch.nn.utils.convert_parameters.parameters_to_vector(agent.parameters()),
             src=1,
@@ -480,15 +490,17 @@
 
         # Start training
         with timer(
             "Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute, process_group=optimization_pg
         ):
             # The Join context is needed because there can be the possibility
             # that some ranks receive less data
-            with Join([agent._forward_module]):
+            with Join(
+                [agent.feature_extractor._forward_module, agent.actor._forward_module, agent.critic._forward_module]
+            ):
                 for _ in range(cfg.algo.update_epochs):
                     for batch_idxes in sampler:
                         batch = {k: data[k][batch_idxes] for k in data.keys()}
                         normalized_obs = normalize_obs(
                             batch, cfg.algo.cnn_keys.encoder, cfg.algo.mlp_keys.encoder + cfg.algo.cnn_keys.encoder
                         )
                         _, logprobs, entropy, new_values = agent(
@@ -648,10 +660,10 @@
     # Create a new group, without assigning it to the collective: in this way the trainers can
     # still communicate with the player through the global group, but they can optimize the agent
     # between themselves
     optimization_pg = world_collective.new_group(
         ranks=list(range(1, world_collective.world_size)), timeout=timedelta(days=1)
     )
     if global_rank == 0:
-        player(fabric, cfg, world_collective, player_trainer_collective)
+        player(fabric, world_collective, player_trainer_collective, cfg)
     else:
         trainer(world_collective, player_trainer_collective, optimization_pg, cfg)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/ppo/utils.py` & `sheeprl-0.5.5/sheeprl/algos/ppo/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,63 +6,61 @@
 import gymnasium as gym
 import numpy as np
 import torch
 from lightning import Fabric
 from lightning.fabric.wrappers import _FabricModule
 from torch import Tensor
 
-from sheeprl.algos.ppo.agent import PPOAgent, build_agent
+from sheeprl.algos.ppo.agent import PPOPlayer, build_agent
 from sheeprl.utils.env import make_env
 from sheeprl.utils.imports import _IS_MLFLOW_AVAILABLE
 from sheeprl.utils.utils import unwrap_fabric
 
 if TYPE_CHECKING:
     from mlflow.models.model import ModelInfo
 
 AGGREGATOR_KEYS = {"Rewards/rew_avg", "Game/ep_len_avg", "Loss/value_loss", "Loss/policy_loss", "Loss/entropy_loss"}
 MODELS_TO_REGISTER = {"agent"}
 
 
+def prepare_obs(
+    fabric: Fabric, obs: Dict[str, np.ndarray], *, cnn_keys: Sequence[str] = [], num_envs: int = 1, **kwargs
+) -> Dict[str, Tensor]:
+    torch_obs = {}
+    for k in obs.keys():
+        torch_obs[k] = torch.from_numpy(obs[k].copy()).to(fabric.device).float()
+        if k in cnn_keys:
+            torch_obs[k] = torch_obs[k].reshape(num_envs, -1, *torch_obs[k].shape[-2:])
+        else:
+            torch_obs[k] = torch_obs[k].reshape(num_envs, -1)
+    return normalize_obs(torch_obs, cnn_keys, obs.keys())
+
+
 @torch.no_grad()
-def test(agent: PPOAgent, fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
+def test(agent: PPOPlayer, fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
     env = make_env(cfg, None, 0, log_dir, "test", vector_env_idx=0)()
     agent.eval()
     done = False
     cumulative_rew = 0
-    o = env.reset(seed=cfg.seed)[0]
-    obs = {}
-    for k in o.keys():
-        if k in cfg.algo.mlp_keys.encoder + cfg.algo.cnn_keys.encoder:
-            torch_obs = torch.from_numpy(o[k]).to(fabric.device).unsqueeze(0)
-            if k in cfg.algo.cnn_keys.encoder:
-                torch_obs = torch_obs.reshape(1, -1, *torch_obs.shape[-2:]) / 255 - 0.5
-            if k in cfg.algo.mlp_keys.encoder:
-                torch_obs = torch_obs.float()
-            obs[k] = torch_obs
+    obs = env.reset(seed=cfg.seed)[0]
 
     while not done:
+        torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder)
+
         # Act greedly through the environment
-        if agent.is_continuous:
-            actions = torch.cat(agent.get_greedy_actions(obs), dim=-1)
+        actions = agent.get_actions(torch_obs, greedy=True)
+        if agent.actor.is_continuous:
+            actions = torch.cat(actions, dim=-1)
         else:
-            actions = torch.cat([act.argmax(dim=-1) for act in agent.get_greedy_actions(obs)], dim=-1)
+            actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1)
 
         # Single environment step
-        o, reward, done, truncated, _ = env.step(actions.cpu().numpy().reshape(env.action_space.shape))
+        obs, reward, done, truncated, _ = env.step(actions.cpu().numpy().reshape(env.action_space.shape))
         done = done or truncated
         cumulative_rew += reward
-        obs = {}
-        for k in o.keys():
-            if k in cfg.algo.mlp_keys.encoder + cfg.algo.cnn_keys.encoder:
-                torch_obs = torch.from_numpy(o[k]).to(fabric.device).unsqueeze(0)
-                if k in cfg.algo.cnn_keys.encoder:
-                    torch_obs = torch_obs.reshape(1, -1, *torch_obs.shape[-2:]) / 255 - 0.5
-                if k in cfg.algo.mlp_keys.encoder:
-                    torch_obs = torch_obs.float()
-                obs[k] = torch_obs
 
         if cfg.dry_run:
             done = True
     fabric.print("Test - Reward:", cumulative_rew)
     if cfg.metric.log_level > 0:
         fabric.log_dict({"Test/cumulative_reward": cumulative_rew}, 0)
     env.close()
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/ppo_recurrent/agent.py` & `sheeprl-0.5.5/sheeprl/algos/sac/agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,319 +1,371 @@
+import copy
 from math import prod
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, Optional, Sequence, SupportsFloat, Tuple, Union
 
 import gymnasium
 import torch
 import torch.nn as nn
 from lightning import Fabric
+from lightning.fabric.wrappers import _FabricModule
+from numpy.typing import NDArray
 from torch import Tensor
-from torch.distributions import Independent, Normal
 
-from sheeprl.algos.ppo.agent import CNNEncoder, MLPEncoder
-from sheeprl.models.models import MLP, MultiEncoder
-from sheeprl.utils.distribution import OneHotCategoricalValidateArgs
+from sheeprl.models.models import MLP
+from sheeprl.utils.fabric import get_single_device_fabric
 
+LOG_STD_MAX = 2
+LOG_STD_MIN = -5
 
-class RecurrentModel(nn.Module):
-    def __init__(
-        self, input_size: int, lstm_hidden_size: int, pre_rnn_mlp_cfg: Dict[str, Any], post_rnn_mlp_cfg: Dict[str, Any]
-    ) -> None:
+
+class SACCritic(nn.Module):
+    def __init__(self, observation_dim: int, hidden_size: int = 256, num_critics: int = 1):
+        """The SAC critic. The architecture is the one specified in https://arxiv.org/abs/1812.05905
+
+        Args:
+            observation_dim (int): the input dimensions. Can be either an integer
+                or a sequence of integers.
+            hidden_size (int): the hidden sizes for both of the two-layer MLP.
+                Defaults to 256.
+            num_critics (int, optional): the number of critic values to output.
+                This is useful if one wants to have a single shared backbone that outputs
+                `num_critics` critic values.
+                Defaults to 1.
+        """
         super().__init__()
-        if pre_rnn_mlp_cfg.apply:
-            self._pre_mlp = MLP(
-                input_dims=input_size,
-                output_dim=None,
-                hidden_sizes=[pre_rnn_mlp_cfg.dense_units],
-                activation=eval(pre_rnn_mlp_cfg.activation),
-                layer_args={"bias": pre_rnn_mlp_cfg.bias},
-                norm_layer=[nn.LayerNorm] if pre_rnn_mlp_cfg.layer_norm else None,
-                norm_args=[{"normalized_shape": pre_rnn_mlp_cfg.dense_units, "eps": 1e-3}]
-                if pre_rnn_mlp_cfg.layer_norm
-                else None,
-            )
-        else:
-            self._pre_mlp = nn.Identity()
-        self._lstm = nn.LSTM(
-            input_size=pre_rnn_mlp_cfg.dense_units if pre_rnn_mlp_cfg.apply else input_size,
-            hidden_size=lstm_hidden_size,
-            batch_first=False,
+        self.model = MLP(
+            input_dims=observation_dim,
+            output_dim=num_critics,
+            hidden_sizes=(hidden_size, hidden_size),
+            activation=nn.ReLU,
+            flatten_dim=None,
         )
-        if post_rnn_mlp_cfg.apply:
-            self._post_mlp = MLP(
-                input_dims=lstm_hidden_size,
-                output_dim=None,
-                hidden_sizes=[post_rnn_mlp_cfg.dense_units],
-                activation=eval(post_rnn_mlp_cfg.activation),
-                layer_args={"bias": post_rnn_mlp_cfg.bias},
-                norm_layer=[nn.LayerNorm] if post_rnn_mlp_cfg.layer_norm else None,
-                norm_args=[{"normalized_shape": post_rnn_mlp_cfg.dense_units, "eps": 1e-3}]
-                if post_rnn_mlp_cfg.layer_norm
-                else None,
-            )
-            self._output_dim = post_rnn_mlp_cfg.dense_units
-        else:
-            self._post_mlp = nn.Identity()
-            self._output_dim = lstm_hidden_size
 
-    @property
-    def output_dim(self) -> int:
-        return self._output_dim
+    def forward(self, obs: Tensor, action: Tensor) -> Tensor:
+        """Return the Q-value conditioned on the observation and the action
 
-    def forward(
-        self, input: Tensor, states: Tuple[Tensor, Tensor], mask: Optional[Tensor] = None
-    ) -> Tuple[Tensor, Tuple[Tensor, Tensor]]:
-        x = self._pre_mlp(input)
-        self._lstm.flatten_parameters()
-        if mask is not None:
-            # To avoid: RuntimeError: 'lengths' argument should be a 1D CPU int64 tensor, but got 1D cuda:0 Long tensor
-            lengths = mask.sum(dim=0).view(-1).cpu()
-            x = torch.nn.utils.rnn.pack_padded_sequence(x, lengths=lengths, batch_first=False, enforce_sorted=False)
-        out, states = self._lstm(x, states)
-        if mask is not None:
-            out, _ = torch.nn.utils.rnn.pad_packed_sequence(out, batch_first=False, total_length=mask.shape[0])
-        shape = out.shape
-        return self._post_mlp(out.view(-1, *shape[2:])).view(shape), states
+        Args:
+            obs (Tensor): input observation
+            action (Tensor): input action
 
+        Returns:
+            q-value
+        """
+        x = torch.cat([obs, action], -1)
+        return self.model(x)
 
-class RecurrentPPOAgent(nn.Module):
+
+class SACActor(nn.Module):
     def __init__(
         self,
-        actions_dim: Sequence[int],
-        obs_space: gymnasium.spaces.Dict,
-        encoder_cfg: Dict[str, Any],
-        rnn_cfg: Dict[str, Any],
-        actor_cfg: Dict[str, Any],
-        critic_cfg: Dict[str, Any],
-        cnn_keys: Sequence[str],
-        mlp_keys: Sequence[str],
-        is_continuous: bool,
+        observation_dim: int,
+        action_dim: int,
         distribution_cfg: Dict[str, Any],
-        num_envs: int = 1,
-        screen_size: int = 64,
-        device: Union[torch.device, str] = "cpu",
+        hidden_size: int = 256,
+        action_low: Union[SupportsFloat, NDArray] = -1.0,
+        action_high: Union[SupportsFloat, NDArray] = 1.0,
     ):
+        """The SAC critic. The architecture is the one specified in https://arxiv.org/abs/1812.05905
+
+        Args:
+            observation_dim (int): the input dimensions. Can be either an integer
+                or a sequence of integers.
+            action_dim (int): the action dimension.
+            distribution_cfg (Dict[str, Any]): the configs of the distributions.
+            hidden_size (int): the hidden sizes for both of the two-layer MLP.
+                Defaults to 256.
+            action_low (Union[SupportsFloat, NDArray], optional): the action lower bound.
+                Defaults to -1.0.
+            action_high (Union[SupportsFloat, NDArray], optional): the action higher bound.
+                Defaults to 1.0.
+        """
         super().__init__()
-        self.num_envs = num_envs
-        self.actions_dim = actions_dim
         self.distribution_cfg = distribution_cfg
-        self.rnn_hidden_size = rnn_cfg.lstm.hidden_size
-        self.device = torch.device(device) if isinstance(device, str) else device
 
-        # Encoder
-        in_channels = sum([prod(obs_space[k].shape[:-2]) for k in cnn_keys])
-        mlp_input_dim = sum([obs_space[k].shape[0] for k in mlp_keys])
-        cnn_encoder = (
-            CNNEncoder(in_channels, encoder_cfg.cnn_features_dim, screen_size, cnn_keys)
-            if cnn_keys is not None and len(cnn_keys) > 0
-            else None
-        )
-        mlp_encoder = (
-            MLPEncoder(
-                mlp_input_dim,
-                encoder_cfg.mlp_features_dim,
-                mlp_keys,
-                encoder_cfg.dense_units,
-                encoder_cfg.mlp_layers,
-                eval(encoder_cfg.dense_act),
-                encoder_cfg.layer_norm,
-            )
-            if mlp_keys is not None and len(mlp_keys) > 0
-            else None
-        )
-        self.feature_extractor = MultiEncoder(cnn_encoder, mlp_encoder)
-        self.is_continuous = is_continuous
-        features_dim = self.feature_extractor.output_dim
-
-        # Recurrent model
-        self.rnn = RecurrentModel(
-            input_size=int(features_dim + sum(actions_dim)),
-            lstm_hidden_size=rnn_cfg.lstm.hidden_size,
-            pre_rnn_mlp_cfg=rnn_cfg.pre_rnn_mlp,
-            post_rnn_mlp_cfg=rnn_cfg.post_rnn_mlp,
-        )
+        self.model = MLP(input_dims=observation_dim, hidden_sizes=(hidden_size, hidden_size), flatten_dim=None)
+        self.fc_mean = nn.Linear(self.model.output_dim, action_dim)
+        self.fc_logstd = nn.Linear(self.model.output_dim, action_dim)
+
+        # Action rescaling buffers
+        self.register_buffer("action_scale", torch.tensor((action_high - action_low) / 2.0, dtype=torch.float32))
+        self.register_buffer("action_bias", torch.tensor((action_high + action_low) / 2.0, dtype=torch.float32))
+
+    def forward(self, obs: Tensor) -> Tuple[Tensor, Tensor]:
+        """Given an observation, it returns a tanh-squashed
+        sampled action (correctly rescaled to the environment action bounds) and its
+        log-prob (as defined in Eq. 26 of https://arxiv.org/abs/1812.05905)
 
-        # Critic
-        self.critic = MLP(
-            input_dims=self.rnn_hidden_size,
-            output_dim=1,
-            hidden_sizes=[critic_cfg.dense_units] * critic_cfg.mlp_layers,
-            activation=eval(critic_cfg.dense_act),
-            norm_layer=[nn.LayerNorm for _ in range(critic_cfg.mlp_layers)] if critic_cfg.layer_norm else None,
-            norm_args=(
-                [{"normalized_shape": critic_cfg.dense_units} for _ in range(critic_cfg.mlp_layers)]
-                if critic_cfg.layer_norm
-                else None
-            ),
-        )
+        Args:
+            obs (Tensor): the observation tensor
 
-        # Actor
-        self.actor_backbone = MLP(
-            input_dims=self.rnn_hidden_size,
-            output_dim=None,
-            hidden_sizes=[actor_cfg.dense_units] * actor_cfg.mlp_layers,
-            activation=eval(actor_cfg.dense_act),
-            flatten_dim=None,
-            norm_layer=[nn.LayerNorm] * actor_cfg.mlp_layers if actor_cfg.layer_norm else None,
-            norm_args=(
-                [{"normalized_shape": actor_cfg.dense_units} for _ in range(actor_cfg.mlp_layers)]
-                if actor_cfg.layer_norm
-                else None
-            ),
-        )
-        if is_continuous:
-            self.actor_heads = nn.ModuleList([nn.Linear(actor_cfg.dense_units, int(sum(actions_dim)) * 2)])
-        else:
-            self.actor_heads = nn.ModuleList(
-                [nn.Linear(actor_cfg.dense_units, action_dim) for action_dim in actions_dim]
-            )
+        Returns:
+            tanh-squashed action, rescaled to the environment action bounds
+            action log-prob
+        """
+        x = self.model(obs)
+        mean = self.fc_mean(x)
+        log_std = self.fc_logstd(x)
+        std = torch.clamp(log_std, LOG_STD_MIN, LOG_STD_MAX).exp()
+        return self._get_actions_and_log_probs(mean, std)
+
+    def _get_actions_and_log_probs(self, mean: Tensor, std: Tensor) -> Tuple[Tensor, Tensor]:
+        """Given the mean and the std of a Normal distribution, it returns a tanh-squashed
+        sampled action (correctly rescaled to the environment action bounds) and its
+        log-prob (as defined in Eq. 26 of https://arxiv.org/abs/1812.05905)
 
-        # Initial recurrent states for both the actor and critic rnn
-        self._initial_states: Tensor = self.reset_hidden_states()
+        Args:
+            mean (Tensor): the mean of the distribution
+            std (Tensor): the standard deviation of the distribution
 
-    @property
-    def initial_states(self) -> Tuple[Tensor, Tensor]:
-        return self._initial_states
+        Returns:
+            tanh-squashed action, rescaled to the environment action bounds
+            action log-prob
+        """
+        normal = torch.distributions.Normal(mean, std)
+
+        # Reparameterization trick (mean + std * N(0,1))
+        x_t = normal.rsample()
+
+        # Squash sample
+        y_t = torch.tanh(x_t)
+
+        # Action sampled from a Tanh transformed Gaussian distribution
+        action = y_t * self.action_scale + self.action_bias
+
+        # Change of variable for probability distributions
+        # Eq. 26 of https://arxiv.org/abs/1812.05905
+        log_prob = normal.log_prob(x_t)
+        log_prob -= torch.log(self.action_scale * (1 - y_t.pow(2)) + 1e-6)
+
+        # Log-prob of independent actions is the sum of the log-probs
+        log_prob = log_prob.sum(-1, keepdim=True)
+
+        return action, log_prob
 
-    @initial_states.setter
-    def initial_states(self, value: Tuple[Tensor, Tensor]) -> None:
-        self._initial_states = value
-
-    def reset_hidden_states(self) -> Tuple[Tensor, Tensor]:
-        states = (
-            torch.zeros(1, self.num_envs, self.rnn_hidden_size, device=self.device),
-            torch.zeros(1, self.num_envs, self.rnn_hidden_size, device=self.device),
-        )
-        return states
 
-    def get_greedy_actions(
+class SACAgent(nn.Module):
+    def __init__(
         self,
-        obs: Dict[str, Tensor],
-        prev_states: Tuple[Tensor, Tensor],
-        prev_actions: Tensor,
-        mask: Optional[Tensor] = None,
-    ) -> Tuple[Tuple[Tensor, ...], Tuple[Tensor, Tensor]]:
-        embedded_obs = self.feature_extractor(obs)
-        out, states = self.rnn(torch.cat((embedded_obs, prev_actions), dim=-1), prev_states, mask)
-        pre_dist = self.get_pre_dist(out)
-        actions = []
-        if self.is_continuous:
-            dist = Independent(
-                Normal(*pre_dist, validate_args=self.distribution_cfg.validate_args),
-                1,
-                validate_args=self.distribution_cfg.validate_args,
-            )
-            actions.append(dist.mode)
-        else:
-            for logits in pre_dist:
-                dist = OneHotCategoricalValidateArgs(logits=logits, validate_args=self.distribution_cfg.validate_args)
-                actions.append(dist.mode)
-        return tuple(actions), states
-
-    def get_sampled_actions(
-        self, pre_dist: Tuple[Tensor, ...], actions: Optional[List[Tensor]] = None
-    ) -> Tuple[Tuple[Tensor, ...], Tensor, Tensor]:
-        logprobs = []
-        entropies = []
-        sampled_actions = []
-        if self.is_continuous:
-            dist = Independent(
-                Normal(*pre_dist, validate_args=self.distribution_cfg.validate_args),
-                1,
-                validate_args=self.distribution_cfg.validate_args,
-            )
-            if actions is None:
-                actions = dist.sample()
+        actor: Union[SACActor, _FabricModule],
+        critics: Sequence[Union[SACCritic, _FabricModule]],
+        target_entropy: float,
+        alpha: float = 1.0,
+        tau: float = 0.005,
+        device: torch.device = torch.device("cpu"),
+    ) -> None:
+        super().__init__()
+
+        # Actor and critics
+        self._num_critics = len(critics)
+        self.actor = actor
+        self.critics = critics
+
+        # Automatic entropy tuning
+        self._target_entropy = torch.tensor(target_entropy, device=device)
+        self._log_alpha = torch.nn.Parameter(torch.log(torch.tensor([alpha], device=device)), requires_grad=True)
+
+        # EMA tau
+        self._tau = tau
+
+    def __setattr__(self, name: str, value: Union[Tensor, nn.Module]) -> None:
+        # Taken from https://github.com/pytorch/pytorch/pull/92044
+        # Check if a property setter exists. If it does, use it.
+        class_attr = getattr(self.__class__, name, None)
+        if isinstance(class_attr, property) and class_attr.fset is not None:
+            return class_attr.fset(self, value)
+        super().__setattr__(name, value)
+
+    @property
+    def critics(self) -> nn.ModuleList:
+        return self.qfs
+
+    @critics.setter
+    def critics(self, critics: Sequence[Union[SACCritic, _FabricModule]]) -> None:
+        self._qfs = nn.ModuleList(critics)
+
+        # Create target critic unwrapping the DDP module from the critics to prevent
+        # `RuntimeError: DDP Pickling/Unpickling are only supported when using DDP with the default process group.
+        # That is, when you have called init_process_group and have not passed process_group
+        # argument to DDP constructor`.
+        # This happens when we're using the decoupled version of SAC for example
+        qfs_unwrapped_modules = []
+        for critic in critics:
+            if hasattr(critic, "module"):
+                critic_module = critic.module
             else:
-                # always composed by a tuple of one element containing all the
-                # continuous actions
-                actions = actions[0]
-            sampled_actions.append(actions)
-            entropies.append(dist.entropy())
-            logprobs.append(dist.log_prob(actions))
-        else:
-            for i, logits in enumerate(pre_dist):
-                dist = OneHotCategoricalValidateArgs(logits=logits, validate_args=self.distribution_cfg.validate_args)
-                if actions is None:
-                    sampled_actions.append(dist.sample())
-                else:
-                    sampled_actions.append(actions[i])
-                entropies.append(dist.entropy())
-                logprobs.append(dist.log_prob(sampled_actions[-1]))
-        return (
-            tuple(sampled_actions),
-            torch.stack(logprobs, dim=-1).sum(dim=-1, keepdim=True),
-            torch.stack(entropies, dim=-1).sum(dim=-1, keepdim=True),
-        )
+                critic_module = critic
+            qfs_unwrapped_modules.append(critic_module)
+        self._qfs_unwrapped = nn.ModuleList(qfs_unwrapped_modules)
+        self._qfs_target = copy.deepcopy(self._qfs_unwrapped)
+        for p in self._qfs_target.parameters():
+            p.requires_grad = False
+        return
 
-    def get_pre_dist(self, input: Tensor) -> Union[Tuple[Tensor, ...], Tuple[Tensor, Tensor]]:
-        features = self.actor_backbone(input)
-        pre_dist: List[Tensor] = [head(features) for head in self.actor_heads]
-        if self.is_continuous:
-            mean, log_std = torch.chunk(pre_dist[0], chunks=2, dim=-1)
-            std = log_std.exp()
-            return (mean, std)
-        else:
-            return tuple(pre_dist)
+    @property
+    def num_critics(self) -> int:
+        return self._num_critics
+
+    @property
+    def qfs(self) -> nn.ModuleList:
+        return self._qfs
+
+    @property
+    def qfs_unwrapped(self) -> nn.ModuleList:
+        return self._qfs_unwrapped
+
+    @property
+    def actor(self) -> Union[SACActor, _FabricModule]:
+        return self._actor
+
+    @actor.setter
+    def actor(self, actor: Union[SACActor, _FabricModule]) -> None:
+        self._actor = actor
+        return
 
-    def get_values(self, input: Tensor) -> Tensor:
-        return self.critic(input)
+    @property
+    def qfs_target(self) -> nn.ModuleList:
+        return self._qfs_target
+
+    @qfs_target.setter
+    def qfs_target(self, qfs_target: nn.ModuleList) -> None:
+        self._qfs_target = qfs_target
+        return
+
+    @property
+    def alpha(self) -> float:
+        return self._log_alpha.exp().item()
+
+    @property
+    def target_entropy(self) -> Tensor:
+        return self._target_entropy
+
+    @property
+    def log_alpha(self) -> Tensor:
+        return self._log_alpha
+
+    def get_actions_and_log_probs(self, obs: Tensor) -> Tuple[Tensor, Tensor]:
+        return self.actor(obs)
+
+    def get_q_values(self, obs: Tensor, action: Tensor) -> Tensor:
+        return torch.cat([self.qfs[i](obs, action) for i in range(len(self.qfs))], dim=-1)
 
-    def forward(
+    @torch.no_grad()
+    def get_target_q_values(self, obs: Tensor, action: Tensor) -> Tensor:
+        return torch.cat([self.qfs_target[i](obs, action) for i in range(len(self.qfs))], dim=-1)
+
+    @torch.no_grad()
+    def get_next_target_q_values(self, next_obs: Tensor, rewards: Tensor, dones: Tensor, gamma: float):
+        # Get q-values for the next observations and actions, estimated by the target q-functions
+        next_state_actions, next_state_log_pi = self.get_actions_and_log_probs(next_obs)
+        qf_next_target = self.get_target_q_values(next_obs, next_state_actions)
+        min_qf_next_target = torch.min(qf_next_target, dim=-1, keepdim=True)[0] - self.alpha * next_state_log_pi
+        next_qf_value = rewards + (1 - dones) * gamma * min_qf_next_target
+        return next_qf_value
+
+    @torch.no_grad()
+    def qfs_target_ema(self) -> None:
+        for param, target_param in zip(self.qfs_unwrapped.parameters(), self.qfs_target.parameters()):
+            target_param.data.copy_(self._tau * param.data + (1 - self._tau) * target_param.data)
+
+
+class SACPlayer(nn.Module):
+    def __init__(
         self,
-        obs: Dict[str, Tensor],
-        prev_actions: Tensor,
-        prev_states: Tuple[Tensor, Tensor],
-        actions: Optional[List[Tensor]] = None,
-        mask: Optional[Tensor] = None,
-    ) -> Tuple[Tuple[Tensor, ...], Tensor, Tensor, Tensor, Tuple[Tensor, Tensor]]:
-        """Compute actor logits and critic values.
+        feature_extractor: nn.Module,
+        fc_mean: nn.Module,
+        fc_logstd: nn.Module,
+        action_low: Union[SupportsFloat, NDArray] = -1.0,
+        action_high: Union[SupportsFloat, NDArray] = 1.0,
+    ):
+        super().__init__()
+        self.model = feature_extractor
+        self.fc_mean = fc_mean
+        self.fc_logstd = fc_logstd
+
+        # Action rescaling buffers
+        self.register_buffer("action_scale", torch.tensor((action_high - action_low) / 2.0, dtype=torch.float32))
+        self.register_buffer("action_bias", torch.tensor((action_high + action_low) / 2.0, dtype=torch.float32))
+
+    def forward(self, obs: Tensor, greedy: bool = False) -> Tensor:
+        """Given an observation, it returns a tanh-squashed
+        sampled action (correctly rescaled to the environment action bounds) and its
+        log-prob (as defined in Eq. 26 of https://arxiv.org/abs/1812.05905)
 
         Args:
-            obs (Tensor): observations collected (possibly padded with zeros).
-            prev_actions (Tensor): the previous actions.
-            prev_states (Tuple[Tensor, Tensor]): the previous state of the LSTM.
-            actions (List[Tensor], optional): the actions from the replay buffer.
-            mask (Tensor, optional): the mask of the padded sequences.
+            obs (Tensor): the observation tensor
 
         Returns:
-            actions (Tuple[Tensor, ...]): the sampled actions
-            logprobs (Tensor): the log probabilities of the actions w.r.t. their distributions.
-            entropies (Tensor): the entropies of the actions distributions.
-            values (Tensor): the state values.
-            states (Tuple[Tensor, Tensor]): the new recurrent states (hx, cx).
+            tanh-squashed action, rescaled to the environment action bounds
+            action log-prob
         """
-        embedded_obs = self.feature_extractor(obs)
-        out, states = self.rnn(torch.cat((embedded_obs, prev_actions), dim=-1), prev_states, mask)
-        values = self.get_values(out)
-        pre_dist = self.get_pre_dist(out)
-        actions, logprobs, entropies = self.get_sampled_actions(pre_dist, actions)
-        return actions, logprobs, entropies, values, states
+        x = self.model(obs)
+        mean = self.fc_mean(x)
+        if greedy:
+            return torch.tanh(mean) * self.action_scale + self.action_bias
+        else:
+            log_std = self.fc_logstd(x)
+            std = torch.clamp(log_std, LOG_STD_MIN, LOG_STD_MAX).exp()
+            normal = torch.distributions.Normal(mean, std)
+            x_t = normal.rsample()
+            y_t = torch.tanh(x_t)
+            actions = y_t * self.action_scale + self.action_bias
+            return actions
+
+    def get_actions(self, obs: Tensor, greedy: bool = False) -> Tensor:
+        return self(obs, greedy=greedy)
 
 
 def build_agent(
     fabric: Fabric,
-    actions_dim: Sequence[int],
-    is_continuous: bool,
     cfg: Dict[str, Any],
     obs_space: gymnasium.spaces.Dict,
+    action_space: gymnasium.spaces.Box,
     agent_state: Optional[Dict[str, Tensor]] = None,
-) -> RecurrentPPOAgent:
-    agent = RecurrentPPOAgent(
-        actions_dim=actions_dim,
-        obs_space=obs_space,
-        encoder_cfg=cfg.algo.encoder,
-        rnn_cfg=cfg.algo.rnn,
-        actor_cfg=cfg.algo.actor,
-        critic_cfg=cfg.algo.critic,
-        cnn_keys=cfg.algo.cnn_keys.encoder,
-        mlp_keys=cfg.algo.mlp_keys.encoder,
-        is_continuous=is_continuous,
+) -> Tuple[SACAgent, SACPlayer]:
+    act_dim = prod(action_space.shape)
+    obs_dim = sum([prod(obs_space[k].shape) for k in cfg.algo.mlp_keys.encoder])
+    actor = SACActor(
+        observation_dim=obs_dim,
+        action_dim=act_dim,
         distribution_cfg=cfg.distribution,
-        num_envs=cfg.env.num_envs,
-        screen_size=cfg.env.screen_size,
-        device=fabric.device,
+        hidden_size=cfg.algo.actor.hidden_size,
+        action_low=action_space.low,
+        action_high=action_space.high,
     )
+    critics = [
+        SACCritic(observation_dim=obs_dim + act_dim, hidden_size=cfg.algo.critic.hidden_size, num_critics=1)
+        for _ in range(cfg.algo.critic.n)
+    ]
+    target_entropy = -act_dim
+    agent = SACAgent(actor, critics, target_entropy, alpha=cfg.algo.alpha.alpha, tau=cfg.algo.tau, device=fabric.device)
     if agent_state:
         agent.load_state_dict(agent_state)
-    agent = fabric.setup_module(agent)
 
-    return agent
+    # Setup player agent
+    player = SACPlayer(
+        copy.deepcopy(agent.actor.model),
+        copy.deepcopy(agent.actor.fc_mean),
+        copy.deepcopy(agent.actor.fc_logstd),
+        action_low=action_space.low,
+        action_high=action_space.high,
+    )
+
+    # Setup training agent
+    agent.actor = fabric.setup_module(agent.actor)
+    agent.critics = [fabric.setup_module(critic) for critic in agent.critics]
+
+    # Wrap the target q-functions with a single-device fabric. This let the target q-functions
+    # to be on the same device as the agent and to run with the same precision
+    fabric_player = get_single_device_fabric(fabric)
+    agent.qfs_target = nn.ModuleList([fabric_player.setup_module(target) for target in agent.qfs_target])
+
+    # Setup player agent
+    player.model = fabric_player.setup_module(player.model)
+    player.fc_mean = fabric_player.setup_module(player.fc_mean)
+    player.fc_logstd = fabric_player.setup_module(player.fc_logstd)
+    player.action_scale = player.action_scale.to(fabric_player.device)
+    player.action_bias = player.action_bias.to(fabric_player.device)
+
+    # Tie weights between the agent and the player
+    for agent_p, player_p in zip(agent.actor.parameters(), player.parameters()):
+        player_p.data = agent_p.data
+    return agent, player
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/ppo_recurrent/evaluate.py` & `sheeprl-0.5.5/sheeprl/algos/p2e_dv3/evaluate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from typing import Any, Dict
 
 import gymnasium as gym
 from lightning import Fabric
 
-from sheeprl.algos.ppo_recurrent.agent import build_agent
-from sheeprl.algos.ppo_recurrent.utils import test
+from sheeprl.algos.dreamer_v3.utils import test
+from sheeprl.algos.p2e_dv3.agent import build_agent
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.registry import register_evaluation
 
 
-@register_evaluation(algorithms="ppo_recurrent")
+@register_evaluation(algorithms=["p2e_dv3_exploration", "p2e_dv3_finetuning"])
 def evaluate(fabric: Fabric, cfg: Dict[str, Any], state: Dict[str, Any]):
     logger = get_logger(fabric, cfg)
     if logger and fabric.is_global_zero:
         fabric._loggers = [logger]
         fabric.logger.log_hyperparams(cfg)
     log_dir = get_log_dir(fabric, cfg.root_dir, cfg.run_name)
     fabric.print(f"Log dir: {log_dir}")
@@ -26,28 +26,33 @@
         cfg.seed,
         0,
         log_dir,
         "test",
         vector_env_idx=0,
     )()
     observation_space = env.observation_space
+    action_space = env.action_space
 
     if not isinstance(observation_space, gym.spaces.Dict):
         raise RuntimeError(f"Unexpected observation type, should be of type Dict, got: {observation_space}")
-    if cfg.algo.cnn_keys.encoder + cfg.algo.mlp_keys.encoder == []:
-        raise RuntimeError(
-            "You should specify at least one CNN keys or MLP keys from the cli: "
-            "`cnn_keys.encoder=[rgb]` or `mlp_keys.encoder=[state]`"
-        )
+
     fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
     fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
 
-    is_continuous = isinstance(env.action_space, gym.spaces.Box)
-    is_multidiscrete = isinstance(env.action_space, gym.spaces.MultiDiscrete)
+    is_continuous = isinstance(action_space, gym.spaces.Box)
+    is_multidiscrete = isinstance(action_space, gym.spaces.MultiDiscrete)
     actions_dim = tuple(
-        env.action_space.shape
-        if is_continuous
-        else (env.action_space.nvec.tolist() if is_multidiscrete else [env.action_space.n])
+        action_space.shape if is_continuous else (action_space.nvec.tolist() if is_multidiscrete else [action_space.n])
     )
     # Create the actor and critic models
-    agent = build_agent(fabric, actions_dim, is_continuous, cfg, observation_space, state["agent"])
-    test(agent, fabric, cfg, log_dir)
+    cfg.algo.player.actor_type == "task"
+    _, _, _, _, _, _, _, player = build_agent(
+        fabric,
+        actions_dim,
+        is_continuous,
+        cfg,
+        observation_space,
+        world_model_state=state["world_model"],
+        actor_task_state=state["actor_task"],
+    )
+    del _
+    test(player, fabric, cfg, log_dir, greedy=False)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/ppo_recurrent/ppo_recurrent.py` & `sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/ppo_recurrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 from lightning.fabric import Fabric
 from torch import Tensor
 from torch.distributed.algorithms.join import Join
 from torch.utils.data.sampler import BatchSampler, RandomSampler
 from torchmetrics import SumMetric
 
 from sheeprl.algos.ppo.loss import entropy_loss, policy_loss, value_loss
-from sheeprl.algos.ppo.utils import normalize_obs
 from sheeprl.algos.ppo_recurrent.agent import RecurrentPPOAgent, build_agent
-from sheeprl.algos.ppo_recurrent.utils import test
+from sheeprl.algos.ppo_recurrent.utils import prepare_obs, test
 from sheeprl.data.buffers import ReplayBuffer
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
 from sheeprl.utils.utils import gae, normalize_tensor, polynomial_decay, save_configs
@@ -39,15 +38,26 @@
 ):
     num_sequences = data[next(iter(data.keys()))].shape[1]
     if cfg.algo.per_rank_num_batches > 0:
         batch_size = num_sequences // cfg.algo.per_rank_num_batches
         batch_size = batch_size if batch_size > 0 else num_sequences
     else:
         batch_size = 1
-    with Join([agent._forward_module]) if fabric.world_size > 1 else nullcontext():
+    with (
+        Join(
+            [
+                agent.feature_extractor._forward_module,
+                agent.rnn._forward_module,
+                agent.actor._forward_module,
+                agent.critic._forward_module,
+            ]
+        )
+        if fabric.world_size > 1
+        else nullcontext()
+    ):
         for _ in range(cfg.algo.update_epochs):
             sampler = BatchSampler(
                 RandomSampler(range(num_sequences)),
                 batch_size=batch_size,
                 drop_last=False,
             )  # Random sampling sequences
             for idxes in sampler:
@@ -123,16 +133,14 @@
         warnings.warn(
             "The script has been called with `buffer.share_data=True`: with recurrent PPO only gradients are shared"
         )
 
     rank = fabric.global_rank
     world_size = fabric.world_size
     device = fabric.device
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     # Resume from checkpoint
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     # Create Logger. This will create the logger only on the
     # rank-0 process
@@ -177,15 +185,15 @@
     actions_dim = tuple(
         envs.single_action_space.shape
         if is_continuous
         else (envs.single_action_space.nvec.tolist() if is_multidiscrete else [envs.single_action_space.n])
     )
 
     # Define the agent and the optimizer
-    agent = build_agent(
+    agent, player = build_agent(
         fabric,
         actions_dim,
         is_continuous,
         cfg,
         observation_space,
         state["agent"] if cfg.checkpoint.resume_from else None,
     )
@@ -273,119 +281,116 @@
 
     # Get the resetted recurrent states from the agent
     prev_states = agent.initial_states
     prev_actions = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     torch_prev_actions = torch.zeros(1, cfg.env.num_envs, sum(actions_dim), device=device, dtype=torch.float32)
 
     for update in range(start_step, num_updates + 1):
-        for _ in range(0, cfg.algo.rollout_steps):
-            policy_step += cfg.env.num_envs * world_size
-
-            # Measure environment interaction time: this considers both the model forward
-            # to get the action given the observation and the time taken into the environment
-            with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-                with torch.no_grad():
+        with torch.inference_mode():
+            for _ in range(0, cfg.algo.rollout_steps):
+                policy_step += cfg.env.num_envs * world_size
+
+                # Measure environment interaction time: this considers both the model forward
+                # to get the action given the observation and the time taken into the environment
+                with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                     # Sample an action given the observation received by the environment
                     # [Seq_len, Batch_size, D] --> [1, num_envs, D]
-                    normalized_obs = normalize_obs(obs, cfg.algo.cnn_keys.encoder, obs_keys)
-                    torch_obs = {k: torch.as_tensor(v, device=device).float() for k, v in normalized_obs.items()}
-                    actions, logprobs, _, values, states = agent.module(
+                    torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                    actions, logprobs, values, states = player(
                         torch_obs, prev_actions=torch_prev_actions, prev_states=prev_states
                     )
                     if is_continuous:
                         real_actions = torch.cat(actions, -1).cpu().numpy()
                     else:
                         real_actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1).cpu().numpy()
                     torch_actions = torch.cat(actions, dim=-1)
                     actions = torch_actions.cpu().numpy()
 
-                # Single environment step
-                next_obs, rewards, dones, truncated, info = envs.step(real_actions.reshape(envs.action_space.shape))
-                truncated_envs = np.nonzero(truncated)[0]
-                if len(truncated_envs) > 0:
-                    real_next_obs = {
-                        k: torch.empty(
-                            1,
-                            len(truncated_envs),
-                            *observation_space[k].shape,
-                            dtype=torch.float32,
-                            device=device,
-                        )
-                        for k in obs_keys
-                    }  # [Seq_len, Batch_size, D] --> [1, num_truncated_envs, D]
-                    for i, truncated_env in enumerate(truncated_envs):
-                        for k, v in info["final_observation"][truncated_env].items():
-                            torch_v = torch.as_tensor(v, dtype=torch.float32, device=device)
-                            if k in cfg.algo.cnn_keys.encoder:
-                                torch_v = torch_v.view(1, 1, -1, *torch_v.shape[-2:]) / 255.0 - 0.5
-                            real_next_obs[k][0, i] = torch_v
-                    with torch.no_grad():
-                        feat = agent.module.feature_extractor(real_next_obs)
-                        rnn_out, _ = agent.module.rnn(
-                            torch.cat((feat, torch_actions[:, truncated_envs, :]), dim=-1),
+                    # Single environment step
+                    next_obs, rewards, terminated, truncated, info = envs.step(
+                        real_actions.reshape(envs.action_space.shape)
+                    )
+                    truncated_envs = np.nonzero(truncated)[0]
+                    if len(truncated_envs) > 0:
+                        real_next_obs = {
+                            k: torch.empty(
+                                1,
+                                len(truncated_envs),
+                                *observation_space[k].shape,
+                                dtype=torch.float32,
+                                device=device,
+                            )
+                            for k in obs_keys
+                        }  # [Seq_len, Batch_size, D] --> [1, num_truncated_envs, D]
+                        for i, truncated_env in enumerate(truncated_envs):
+                            for k, v in info["final_observation"][truncated_env].items():
+                                torch_v = torch.as_tensor(v, dtype=torch.float32, device=device)
+                                if k in cfg.algo.cnn_keys.encoder:
+                                    torch_v = torch_v.view(1, 1, -1, *torch_v.shape[-2:]) / 255.0 - 0.5
+                                real_next_obs[k][0, i] = torch_v
+                        vals, _ = player.get_values(
+                            real_next_obs,
+                            torch_actions[:, truncated_envs, :],
                             tuple(s[:, truncated_envs, ...] for s in states),
                         )
-                        vals = agent.module.get_values(rnn_out).view(rewards[truncated_envs].shape).cpu().numpy()
-                        rewards[truncated_envs] += vals.reshape(rewards[truncated_envs].shape)
-                dones = np.logical_or(dones, truncated).reshape(1, cfg.env.num_envs, -1).astype(np.float32)
-                rewards = rewards.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
-
-            step_data["dones"] = dones.reshape(1, cfg.env.num_envs, -1)
-            step_data["values"] = values.cpu().numpy().reshape(1, cfg.env.num_envs, -1)
-            step_data["actions"] = actions.reshape(1, cfg.env.num_envs, -1)
-            step_data["rewards"] = rewards.reshape(1, cfg.env.num_envs, -1)
-            step_data["logprobs"] = logprobs.cpu().numpy()
-            step_data["prev_hx"] = prev_states[0].cpu().numpy().reshape(1, cfg.env.num_envs, -1)
-            step_data["prev_cx"] = prev_states[1].cpu().numpy().reshape(1, cfg.env.num_envs, -1)
-            step_data["prev_actions"] = prev_actions.reshape(1, cfg.env.num_envs, -1)
-            if cfg.buffer.memmap:
-                step_data["returns"] = np.zeros_like(rewards)
-                step_data["advantages"] = np.zeros_like(rewards)
-
-            # Append data to buffer
-            rb.add(step_data, validate_args=cfg.buffer.validate_args)
-
-            # Update actions
-            prev_actions = (1 - dones) * actions
-            torch_prev_actions = torch.from_numpy(prev_actions).to(device).float()
-
-            # Update the observation
-            obs = next_obs
-            for k in obs_keys:
-                obs[k] = obs[k][np.newaxis]
-                if k in cfg.algo.cnn_keys.encoder:
-                    obs[k] = obs[k].reshape(1, cfg.env.num_envs, -1, *obs[k].shape[-2:])
-                step_data[k] = obs[k]
-
-            # Reset the states if the episode is done
-            if cfg.algo.reset_recurrent_state_on_done:
-                prev_states = tuple([(1 - torch.as_tensor(dones, device=device)) * s for s in states])
-            else:
-                prev_states = states
-
-            if cfg.metric.log_level > 0 and "final_info" in info:
-                for i, agent_ep_info in enumerate(info["final_info"]):
-                    if agent_ep_info is not None:
-                        ep_rew = agent_ep_info["episode"]["r"]
-                        ep_len = agent_ep_info["episode"]["l"]
-                        if aggregator and not aggregator.disabled:
-                            aggregator.update("Rewards/rew_avg", ep_rew)
-                            aggregator.update("Game/ep_len_avg", ep_len)
-                        fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
+                        vals = vals.view(rewards[truncated_envs].shape).cpu().numpy()
+                        rewards[truncated_envs] += cfg.algo.gamma * vals.reshape(rewards[truncated_envs].shape)
+                    dones = np.logical_or(terminated, truncated).reshape(1, cfg.env.num_envs, -1).astype(np.float32)
+                    rewards = rewards.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
+
+                step_data["dones"] = dones.reshape(1, cfg.env.num_envs, -1)
+                step_data["values"] = values.cpu().numpy().reshape(1, cfg.env.num_envs, -1)
+                step_data["actions"] = actions.reshape(1, cfg.env.num_envs, -1)
+                step_data["rewards"] = rewards.reshape(1, cfg.env.num_envs, -1)
+                step_data["logprobs"] = logprobs.cpu().numpy()
+                step_data["prev_hx"] = prev_states[0].cpu().numpy().reshape(1, cfg.env.num_envs, -1)
+                step_data["prev_cx"] = prev_states[1].cpu().numpy().reshape(1, cfg.env.num_envs, -1)
+                step_data["prev_actions"] = prev_actions.reshape(1, cfg.env.num_envs, -1)
+                if cfg.buffer.memmap:
+                    step_data["returns"] = np.zeros_like(rewards)
+                    step_data["advantages"] = np.zeros_like(rewards)
+
+                # Append data to buffer
+                rb.add(step_data, validate_args=cfg.buffer.validate_args)
+
+                # Update actions
+                prev_actions = (1 - dones) * actions
+                torch_prev_actions = torch.from_numpy(prev_actions).to(device).float()
+
+                # Update the observation
+                obs = next_obs
+                for k in obs_keys:
+                    obs[k] = obs[k][np.newaxis]
+                    if k in cfg.algo.cnn_keys.encoder:
+                        obs[k] = obs[k].reshape(1, cfg.env.num_envs, -1, *obs[k].shape[-2:])
+                    step_data[k] = obs[k]
+
+                # Reset the states if the episode is done
+                if cfg.algo.reset_recurrent_state_on_done:
+                    prev_states = tuple([(1 - torch.as_tensor(dones, device=device)) * s for s in states])
+                else:
+                    prev_states = states
+
+                if cfg.metric.log_level > 0 and "final_info" in info:
+                    for i, agent_ep_info in enumerate(info["final_info"]):
+                        if agent_ep_info is not None:
+                            ep_rew = agent_ep_info["episode"]["r"]
+                            ep_len = agent_ep_info["episode"]["l"]
+                            if aggregator and not aggregator.disabled:
+                                aggregator.update("Rewards/rew_avg", ep_rew)
+                                aggregator.update("Game/ep_len_avg", ep_len)
+                            fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
 
         # Transform the data into PyTorch Tensors
         local_data = rb.to_tensor(dtype=None, device=device, from_numpy=cfg.buffer.from_numpy)
 
         # Estimate returns with GAE (https://arxiv.org/abs/1506.02438)
-        with torch.no_grad():
-            normalized_obs = normalize_obs(obs, cfg.algo.cnn_keys.encoder, obs_keys)
-            torch_obs = {k: torch.as_tensor(v, device=device).float() for k, v in normalized_obs.items()}
-            feat = agent.module.feature_extractor(torch_obs)
-            rnn_out, _ = agent.module.rnn(torch.cat((feat, torch_actions), dim=-1), states)
-            next_values = agent.module.get_values(rnn_out)
+        with torch.inference_mode():
+            torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+            next_values, _ = player.get_values(torch_obs, torch_actions, states)
             returns, advantages = gae(
                 local_data["rewards"].to(torch.float64),
                 local_data["values"],
                 local_data["dones"],
                 next_values,
                 cfg.algo.rollout_steps,
                 cfg.algo.gamma,
@@ -423,15 +428,14 @@
             sequences = {k: [] for k in episodes[0].keys()}
             for ep in episodes:
                 for k in sequences.keys():
                     seq = torch.split(ep[k], sl)
                     sequences[k].extend(seq)
                 # Regardless of the key, the shapes are the same
                 lengths.extend([s.shape[0] for s in seq])
-
         else:
             sequences = episodes
 
         padded_sequences = {
             k: torch.nn.utils.rnn.pad_sequence(v, batch_first=False, padding_value=0) for k, v in sequences.items()
         }
         max_len = max(lengths)
@@ -507,14 +511,14 @@
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call("on_checkpoint_coupled", fabric=fabric, ckpt_path=ckpt_path, state=ckpt_state)
 
     envs.close()
     if fabric.is_global_zero and cfg.algo.run_test:
-        test(agent.module, fabric, cfg, log_dir)
+        test(player, fabric, cfg, log_dir)
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.ppo.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
         register_model(fabric, log_models, cfg, models_to_log)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/ppo_recurrent/utils.py` & `sheeprl-0.5.5/sheeprl/algos/ppo_recurrent/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Dict, Sequence
 
 import gymnasium as gym
+import numpy as np
 import torch
 from lightning import Fabric
+from torch import Tensor
 
 from sheeprl.algos.ppo.utils import AGGREGATOR_KEYS as ppo_aggregator_keys
 from sheeprl.algos.ppo.utils import MODELS_TO_REGISTER as ppo_models_to_register
-from sheeprl.algos.ppo_recurrent.agent import RecurrentPPOAgent, build_agent
+from sheeprl.algos.ppo.utils import normalize_obs
+from sheeprl.algos.ppo_recurrent.agent import RecurrentPPOPlayer, build_agent
 from sheeprl.utils.env import make_env
 from sheeprl.utils.imports import _IS_MLFLOW_AVAILABLE
 from sheeprl.utils.utils import unwrap_fabric
 
 if TYPE_CHECKING:
     from mlflow.models.model import ModelInfo
 
 
 AGGREGATOR_KEYS = ppo_aggregator_keys
 MODELS_TO_REGISTER = ppo_models_to_register
 
 
+def prepare_obs(
+    fabric: Fabric, obs: Dict[str, np.ndarray], *, cnn_keys: Sequence[str] = [], num_envs: int = 1, **kwargs
+) -> Dict[str, Tensor]:
+    torch_obs = {}
+    with fabric.device:
+        for k, v in obs.items():
+            torch_obs[k] = torch.as_tensor(v.copy(), dtype=torch.float32, device=fabric.device)
+            if k in cnn_keys:
+                torch_obs[k] = torch_obs[k].view(1, num_envs, -1, *v.shape[-2:])
+            else:
+                torch_obs[k] = torch_obs[k].view(1, num_envs, -1)
+    return normalize_obs(torch_obs, cnn_keys, torch_obs.keys())
+
+
 @torch.no_grad()
-def test(agent: "RecurrentPPOAgent", fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
+def test(agent: "RecurrentPPOPlayer", fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
     env = make_env(cfg, None, 0, log_dir, "test", vector_env_idx=0)()
     agent.eval()
     done = False
     cumulative_rew = 0
     agent.num_envs = 1
+    obs = env.reset(seed=cfg.seed)[0]
     with fabric.device:
-        o = env.reset(seed=cfg.seed)[0]
-        next_obs = {
-            k: torch.as_tensor(o[k], dtype=torch.float32, device=fabric.device).view(1, 1, -1, *o[k].shape[-2:]) / 255
-            for k in cfg.algo.cnn_keys.encoder
-        }
-        next_obs.update(
-            {
-                k: torch.as_tensor(o[k], dtype=torch.float32, device=fabric.device).view(1, 1, -1)
-                for k in cfg.algo.mlp_keys.encoder
-            }
-        )
         state = (
             torch.zeros(1, 1, agent.rnn_hidden_size, device=fabric.device),
             torch.zeros(1, 1, agent.rnn_hidden_size, device=fabric.device),
         )
         actions = torch.zeros(1, 1, sum(agent.actions_dim), device=fabric.device)
     while not done:
+        torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder)
         # Act greedly through the environment
-        actions, state = agent.get_greedy_actions(next_obs, state, actions)
-        if agent.is_continuous:
+        actions, state = agent.get_actions(torch_obs, actions, state, greedy=True)
+        if agent.actor.is_continuous:
             real_actions = torch.cat(actions, -1)
             actions = torch.cat(actions, dim=-1).view(1, 1, -1)
         else:
             real_actions = torch.cat([act.argmax(dim=-1) for act in actions], dim=-1)
             actions = torch.cat([act for act in actions], dim=-1).view(1, 1, -1)
 
         # Single environment step
-        o, reward, done, truncated, info = env.step(real_actions.cpu().numpy().reshape(env.action_space.shape))
+        obs, reward, done, truncated, info = env.step(real_actions.cpu().numpy().reshape(env.action_space.shape))
         done = done or truncated
         cumulative_rew += reward
-        with fabric.device:
-            next_obs = {
-                k: torch.as_tensor(o[k], dtype=torch.float32).view(1, 1, -1, *o[k].shape[-2:]) / 255
-                for k in cfg.algo.cnn_keys.encoder
-            }
-            next_obs.update(
-                {k: torch.as_tensor(o[k], dtype=torch.float32).view(1, 1, -1) for k in cfg.algo.mlp_keys.encoder}
-            )
 
         if cfg.dry_run:
             done = True
     fabric.print("Test - Reward:", cumulative_rew)
     if cfg.metric.log_level > 0:
         fabric.log_dict({"Test/cumulative_reward": cumulative_rew}, 0)
     env.close()
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/sac/loss.py` & `sheeprl-0.5.5/sheeprl/algos/sac/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/algos/sac/sac.py` & `sheeprl-0.5.5/sheeprl/algos/sac/sac.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from torch.optim import Optimizer
 from torch.utils.data.distributed import DistributedSampler
 from torch.utils.data.sampler import BatchSampler
 from torchmetrics import SumMetric
 
 from sheeprl.algos.sac.agent import SACAgent, build_agent
 from sheeprl.algos.sac.loss import critic_loss, entropy_loss, policy_loss
-from sheeprl.algos.sac.utils import test
+from sheeprl.algos.sac.utils import prepare_obs, test
 from sheeprl.data.buffers import ReplayBuffer
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import save_configs
+from sheeprl.utils.utils import Ratio, save_configs
 
 
 def train(
     fabric: Fabric,
     agent: SACAgent,
     actor_optimizer: Optimizer,
     qf_optimizer: Optimizer,
@@ -40,15 +40,15 @@
     update: int,
     cfg: Dict[str, Any],
     policy_steps_per_update: int,
     group: Optional[CollectibleGroup] = None,
 ):
     # Update the soft-critic
     next_target_qf_value = agent.get_next_target_q_values(
-        data["next_observations"], data["rewards"], data["dones"], cfg.algo.gamma
+        data["next_observations"], data["rewards"], data["terminated"], cfg.algo.gamma
     )
     qf_values = agent.get_q_values(data["observations"], data["actions"])
     qf_loss = critic_loss(qf_values, next_target_qf_value, agent.num_critics)
     qf_optimizer.zero_grad(set_to_none=True)
     fabric.backward(qf_loss)
     qf_optimizer.step()
 
@@ -87,16 +87,14 @@
             "in order to play correctly the game. "
             "As an alternative you can use one of the Dreamers' agents."
         )
 
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     # Resume from checkpoint
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     if len(cfg.algo.cnn_keys.encoder) > 0:
         warnings.warn("SAC algorithm cannot allow to use images as observations, the CNN keys will be ignored")
@@ -141,24 +139,34 @@
                 f"The observation with key '{k}' has shape {observation_space[k].shape}. "
                 f"Provided environment: {cfg.env.id}"
             )
     if cfg.metric.log_level > 0:
         fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
 
     # Define the agent and the optimizer and setup sthem with Fabric
-    agent = build_agent(
+    agent, player = build_agent(
         fabric, cfg, observation_space, action_space, state["agent"] if cfg.checkpoint.resume_from else None
     )
 
     # Optimizers
-    qf_optimizer = hydra.utils.instantiate(cfg.algo.critic.optimizer, params=agent.qfs.parameters(), _convert_="all")
+    qf_optimizer = hydra.utils.instantiate(
+        cfg.algo.critic.optimizer,
+        params=agent.qfs.parameters(),
+        _convert_="all",
+    )
     actor_optimizer = hydra.utils.instantiate(
-        cfg.algo.actor.optimizer, params=agent.actor.parameters(), _convert_="all"
+        cfg.algo.actor.optimizer,
+        params=agent.actor.parameters(),
+        _convert_="all",
+    )
+    alpha_optimizer = hydra.utils.instantiate(
+        cfg.algo.alpha.optimizer,
+        params=[agent.log_alpha],
+        _convert_="all",
     )
-    alpha_optimizer = hydra.utils.instantiate(cfg.algo.alpha.optimizer, params=[agent.log_alpha], _convert_="all")
     if cfg.checkpoint.resume_from:
         qf_optimizer.load_state_dict(state["qf_optimizer"])
         actor_optimizer.load_state_dict(state["actor_optimizer"])
         alpha_optimizer.load_state_dict(state["alpha_optimizer"])
     qf_optimizer, actor_optimizer, alpha_optimizer = fabric.setup_optimizers(
         qf_optimizer, actor_optimizer, alpha_optimizer
     )
@@ -206,14 +214,19 @@
     num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
     learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // fabric.world_size
         if not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -225,33 +238,32 @@
             "the checkpoint will be saved at the nearest greater multiple of the "
             "policy_steps_per_update value."
         )
 
     step_data = {}
     # Get the first environment observation and start the optimization
     obs = envs.reset(seed=cfg.seed)[0]
-    obs = np.concatenate([obs[k] for k in cfg.algo.mlp_keys.encoder], axis=-1)
 
+    per_rank_gradient_steps = 0
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * world_size
 
         # Measure environment interaction time: this considers both the model forward
         # to get the action given the observation and the time taken into the environment
         with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
             if update <= learning_starts:
                 actions = envs.action_space.sample()
             else:
                 # Sample an action given the observation received by the environment
-                with torch.no_grad():
-                    torch_obs = torch.as_tensor(obs, dtype=torch.float32, device=device)
-                    actions, _ = agent.actor.module(torch_obs)
+                with torch.inference_mode():
+                    torch_obs = prepare_obs(fabric, obs, num_envs=cfg.env.num_envs)
+                    actions = player(torch_obs)
                     actions = actions.cpu().numpy()
-            next_obs, rewards, dones, truncated, infos = envs.step(actions)
-            next_obs = np.concatenate([next_obs[k] for k in cfg.algo.mlp_keys.encoder], axis=-1)
-            dones = np.logical_or(dones, truncated).reshape(cfg.env.num_envs, -1).astype(np.uint8)
+            next_obs, rewards, terminated, truncated, infos = envs.step(actions.reshape(envs.action_space.shape))
             rewards = rewards.reshape(cfg.env.num_envs, -1)
 
         if cfg.metric.log_level > 0 and "final_info" in infos:
             for i, agent_ep_info in enumerate(infos["final_info"]):
                 if agent_ep_info is not None:
                     ep_rew = agent_ep_info["episode"]["r"]
                     ep_len = agent_ep_info["episode"]["l"]
@@ -261,92 +273,101 @@
                     fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
 
         # Save the real next observation
         real_next_obs = copy.deepcopy(next_obs)
         if "final_observation" in infos:
             for idx, final_obs in enumerate(infos["final_observation"]):
                 if final_obs is not None:
-                    real_next_obs[idx] = np.concatenate(
-                        [v for k, v in final_obs.items() if k in cfg.algo.mlp_keys.encoder], axis=-1
-                    )
+                    for k, v in final_obs.items():
+                        real_next_obs[k][idx] = v
+        real_next_obs = np.concatenate([real_next_obs[k] for k in cfg.algo.mlp_keys.encoder], axis=-1).astype(
+            np.float32
+        )
 
-        step_data["dones"] = dones[np.newaxis]
-        step_data["actions"] = actions[np.newaxis]
-        step_data["observations"] = obs[np.newaxis]
+        step_data["terminated"] = terminated.reshape(1, cfg.env.num_envs, -1).astype(np.uint8)
+        step_data["truncated"] = truncated.reshape(1, cfg.env.num_envs, -1).astype(np.uint8)
+        step_data["actions"] = actions.reshape(1, cfg.env.num_envs, -1)
+        step_data["observations"] = np.concatenate([obs[k] for k in cfg.algo.mlp_keys.encoder], axis=-1)[np.newaxis]
         if not cfg.buffer.sample_next_obs:
             step_data["next_observations"] = real_next_obs[np.newaxis]
         step_data["rewards"] = rewards[np.newaxis]
         rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
         # next_obs becomes the new obs
         obs = next_obs
 
         # Train the agent
         if update >= learning_starts:
-            training_steps = learning_starts if update == learning_starts else 1
-
-            # We sample one time to reduce the communications between processes
-            sample = rb.sample_tensors(
-                batch_size=training_steps * cfg.algo.per_rank_gradient_steps * cfg.algo.per_rank_batch_size,
-                sample_next_obs=cfg.buffer.sample_next_obs,
-                dtype=None,
-                device=device,
-                from_numpy=cfg.buffer.from_numpy,
-            )  # [G*B]
-            gathered_data: Dict[str, torch.Tensor] = fabric.all_gather(sample)  # [World, G*B]
-            for k, v in gathered_data.items():
-                gathered_data[k] = v.float()  # [G*B*World]
-                if fabric.world_size > 1:
-                    gathered_data[k] = gathered_data[k].flatten(start_dim=0, end_dim=2)
+            per_rank_gradient_steps = ratio(policy_step / world_size) if not cfg.run_benchmarks else 1
+            if per_rank_gradient_steps > 0:
+                # We sample one time to reduce the communications between processes
+                sample = rb.sample_tensors(
+                    batch_size=per_rank_gradient_steps * cfg.algo.per_rank_batch_size,
+                    sample_next_obs=cfg.buffer.sample_next_obs,
+                    dtype=None,
+                    device=device,
+                    from_numpy=cfg.buffer.from_numpy,
+                )  # [G*B]
+                gathered_data: Dict[str, torch.Tensor] = fabric.all_gather(sample)  # [World, G*B]
+                for k, v in gathered_data.items():
+                    gathered_data[k] = v.float()  # [G*B*World]
+                    if fabric.world_size > 1:
+                        gathered_data[k] = gathered_data[k].flatten(start_dim=0, end_dim=2)
+                    else:
+                        gathered_data[k] = gathered_data[k].flatten(start_dim=0, end_dim=1)
+                idxes_to_sample = list(range(next(iter(gathered_data.values())).shape[0]))
+                if world_size > 1:
+                    dist_sampler: DistributedSampler = DistributedSampler(
+                        idxes_to_sample,
+                        num_replicas=world_size,
+                        rank=fabric.global_rank,
+                        shuffle=True,
+                        seed=cfg.seed,
+                        drop_last=False,
+                    )
+                    sampler: BatchSampler = BatchSampler(
+                        sampler=dist_sampler, batch_size=cfg.algo.per_rank_batch_size, drop_last=False
+                    )
                 else:
-                    gathered_data[k] = gathered_data[k].flatten(start_dim=0, end_dim=1)
-            idxes_to_sample = list(range(next(iter(gathered_data.values())).shape[0]))
-            if world_size > 1:
-                dist_sampler: DistributedSampler = DistributedSampler(
-                    idxes_to_sample,
-                    num_replicas=world_size,
-                    rank=fabric.global_rank,
-                    shuffle=True,
-                    seed=cfg.seed,
-                    drop_last=False,
-                )
-                sampler: BatchSampler = BatchSampler(
-                    sampler=dist_sampler, batch_size=cfg.algo.per_rank_batch_size, drop_last=False
-                )
-            else:
-                sampler = BatchSampler(
-                    sampler=idxes_to_sample, batch_size=cfg.algo.per_rank_batch_size, drop_last=False
-                )
-
-            # Start training
-            with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
-                for batch_idxes in sampler:
-                    batch = {k: v[batch_idxes] for k, v in gathered_data.items()}
-                    train(
-                        fabric,
-                        agent,
-                        actor_optimizer,
-                        qf_optimizer,
-                        alpha_optimizer,
-                        batch,
-                        aggregator,
-                        update,
-                        cfg,
-                        policy_steps_per_update,
+                    sampler = BatchSampler(
+                        sampler=idxes_to_sample, batch_size=cfg.algo.per_rank_batch_size, drop_last=False
                     )
-                train_step += world_size
+
+                # Start training
+                with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
+                    for batch_idxes in sampler:
+                        batch = {k: v[batch_idxes] for k, v in gathered_data.items()}
+                        train(
+                            fabric,
+                            agent,
+                            actor_optimizer,
+                            qf_optimizer,
+                            alpha_optimizer,
+                            batch,
+                            aggregator,
+                            update,
+                            cfg,
+                            policy_steps_per_update,
+                        )
+                        cumulative_per_rank_gradient_steps += 1
+                    train_step += world_size
 
         # Log metrics
         if cfg.metric.log_level > 0 and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -371,14 +392,15 @@
         ):
             last_checkpoint = policy_step
             state = {
                 "agent": agent.state_dict(),
                 "qf_optimizer": qf_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "alpha_optimizer": alpha_optimizer.state_dict(),
+                "ratio": ratio.state_dict(),
                 "update": update * fabric.world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * fabric.world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call(
@@ -387,15 +409,15 @@
                 ckpt_path=ckpt_path,
                 state=state,
                 replay_buffer=rb if cfg.buffer.checkpoint else None,
             )
 
     envs.close()
     if fabric.is_global_zero and cfg.algo.run_test:
-        test(agent.actor.module, fabric, cfg, log_dir)
+        test(player, fabric, cfg, log_dir)
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.sac.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
         models_to_log = {"agent": agent}
         register_model(fabric, log_models, cfg, models_to_log)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/sac/sac_decoupled.py` & `sheeprl-0.5.5/sheeprl/algos/sac/sac_decoupled.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,39 +12,40 @@
 from lightning.fabric import Fabric
 from lightning.fabric.plugins.collectives import TorchCollective
 from lightning.fabric.plugins.collectives.collective import CollectibleGroup
 from lightning.fabric.strategies import DDPStrategy
 from torch.utils.data.sampler import BatchSampler
 from torchmetrics import SumMetric
 
-from sheeprl.algos.sac.agent import SACActor, SACAgent, SACCritic, build_agent
+from sheeprl.algos.sac.agent import SACAgent, SACCritic, build_agent
 from sheeprl.algos.sac.sac import train
-from sheeprl.algos.sac.utils import test
+from sheeprl.algos.sac.utils import prepare_obs, test
 from sheeprl.data.buffers import ReplayBuffer
 from sheeprl.utils.env import make_env
+from sheeprl.utils.fabric import get_single_device_fabric
 from sheeprl.utils.logger import get_log_dir
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import save_configs
+from sheeprl.utils.utils import Ratio, save_configs
 
 
-@torch.no_grad()
+@torch.inference_mode()
 def player(
-    fabric: Fabric, cfg: Dict[str, Any], world_collective: TorchCollective, player_trainer_collective: TorchCollective
+    fabric: Fabric, world_collective: TorchCollective, player_trainer_collective: TorchCollective, cfg: Dict[str, Any]
 ):
-    log_dir = get_log_dir(fabric, cfg.root_dir, cfg.run_name, False)
+    # Initialize Fabric player-only
+    fabric_player = get_single_device_fabric(fabric)
+    log_dir = get_log_dir(fabric_player, cfg.root_dir, cfg.run_name, False)
+    device = fabric_player.device
     rank = fabric.global_rank
-    device = fabric.device
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     # Resume from checkpoint
     if cfg.checkpoint.resume_from:
-        state = fabric.load(cfg.checkpoint.resume_from)
+        state = fabric_player.load(cfg.checkpoint.resume_from)
 
     if len(cfg.algo.cnn_keys.encoder) > 0:
         warnings.warn("SAC algorithm cannot allow to use images as observations, the CNN keys will be ignored")
         cfg.algo.cnn_keys.encoder = []
 
     # Environment setup
     vectorized_env = gym.vector.SyncVectorEnv if cfg.env.sync_env else gym.vector.AsyncVectorEnv
@@ -86,22 +87,21 @@
         cfg.algo.per_rank_batch_size = state["batch_size"] // fabric.world_size
     cfg.checkpoint.log_dir = log_dir
     world_collective.broadcast_object_list([cfg], src=0)
 
     # Define the agent and the optimizer and setup them with Fabric
     act_dim = prod(action_space.shape)
     obs_dim = sum([prod(observation_space[k].shape) for k in cfg.algo.mlp_keys.encoder])
-    actor = SACActor(
-        observation_dim=obs_dim,
-        action_dim=act_dim,
-        distribution_cfg=cfg.distribution,
-        hidden_size=cfg.algo.actor.hidden_size,
-        action_low=action_space.low,
-        action_high=action_space.high,
-    ).to(device)
+    _, actor = build_agent(
+        fabric_player,
+        cfg,
+        observation_space,
+        action_space,
+        state["agent"] if cfg.checkpoint.resume_from else None,
+    )
     flattened_parameters = torch.empty_like(
         torch.nn.utils.convert_parameters.parameters_to_vector(actor.parameters()), device=device
     )
 
     # Receive the first weights from the rank-1, a.k.a. the first of the trainers
     # In this way we are sure that before the first iteration everyone starts with the same parameters
     player_trainer_collective.broadcast(flattened_parameters, src=1)
@@ -144,14 +144,19 @@
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
     policy_steps_per_update = int(cfg.env.num_envs)
     num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
     learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
     if cfg.checkpoint.resume_from and not cfg.buffer.checkpoint:
         learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -163,33 +168,31 @@
             "the checkpoint will be saved at the nearest greater multiple of the "
             "policy_steps_per_update value."
         )
 
     step_data = {}
     # Get the first environment observation and start the optimization
     obs = envs.reset(seed=cfg.seed)[0]
-    obs = np.concatenate([obs[k] for k in cfg.algo.mlp_keys.encoder], axis=-1)
 
+    per_rank_gradient_steps = 0
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs
 
         # Measure environment interaction time: this considers both the model forward
         # to get the action given the observation and the time taken into the environment
         with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
             if update <= learning_starts:
                 actions = envs.action_space.sample()
             else:
                 # Sample an action given the observation received by the environment
-                with torch.no_grad():
-                    torch_obs = torch.as_tensor(obs, dtype=torch.float32, device=device)
-                    actions, _ = actor(torch_obs)
-                    actions = actions.cpu().numpy()
-            next_obs, rewards, dones, truncated, infos = envs.step(actions)
-            next_obs = np.concatenate([next_obs[k] for k in cfg.algo.mlp_keys.encoder], axis=-1)
-            dones = np.logical_or(dones, truncated).reshape(cfg.env.num_envs, -1).astype(np.uint8)
+                torch_obs = prepare_obs(fabric, obs, num_envs=cfg.env.num_envs)
+                actions = actor(torch_obs)
+                actions = actions.cpu().numpy()
+            next_obs, rewards, terminated, truncated, infos = envs.step(actions)
             rewards = rewards.reshape(cfg.env.num_envs, -1)
 
         if cfg.metric.log_level > 0 and "final_info" in infos:
             for i, agent_ep_info in enumerate(infos["final_info"]):
                 if agent_ep_info is not None:
                     ep_rew = agent_ep_info["episode"]["r"]
                     ep_len = agent_ep_info["episode"]["l"]
@@ -199,80 +202,89 @@
                     fabric.print(f"Rank-0: policy_step={policy_step}, reward_env_{i}={ep_rew[-1]}")
 
         # Save the real next observation
         real_next_obs = copy.deepcopy(next_obs)
         if "final_observation" in infos:
             for idx, final_obs in enumerate(infos["final_observation"]):
                 if final_obs is not None:
-                    real_next_obs[idx] = np.concatenate(
-                        [v for k, v in final_obs.items() if k in cfg.algo.mlp_keys.encoder], axis=-1
-                    )
+                    for k, v in final_obs.items():
+                        real_next_obs[k][idx] = v
+        real_next_obs = np.concatenate([real_next_obs[k] for k in cfg.algo.mlp_keys.encoder], axis=-1).astype(
+            np.float32
+        )
 
-        step_data["dones"] = dones[np.newaxis]
-        step_data["actions"] = actions[np.newaxis]
-        step_data["observations"] = obs[np.newaxis]
+        step_data["terminated"] = terminated.reshape(1, cfg.env.num_envs, -1).astype(np.uint8)
+        step_data["truncated"] = truncated.reshape(1, cfg.env.num_envs, -1).astype(np.uint8)
+        step_data["actions"] = actions.reshape(1, cfg.env.num_envs, -1)
+        step_data["observations"] = np.concatenate([obs[k] for k in cfg.algo.mlp_keys.encoder], axis=-1)[np.newaxis]
         if not cfg.buffer.sample_next_obs:
             step_data["next_observations"] = real_next_obs[np.newaxis]
         step_data["rewards"] = rewards[np.newaxis]
         rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
         # next_obs becomes the new obs
         obs = next_obs
 
         # Send data to the training agents
         if update >= learning_starts:
-            # Send local info to the trainers
-            if not first_info_sent:
-                world_collective.broadcast_object_list(
-                    [{"update": update, "last_log": last_log, "last_checkpoint": last_checkpoint}], src=0
-                )
-                first_info_sent = True
+            per_rank_gradient_steps = ratio(policy_step / (fabric.world_size - 1))
+            cumulative_per_rank_gradient_steps += per_rank_gradient_steps
+            if per_rank_gradient_steps > 0:
+                # Send local info to the trainers
+                if not first_info_sent:
+                    world_collective.broadcast_object_list(
+                        [{"update": update, "last_log": last_log, "last_checkpoint": last_checkpoint}], src=0
+                    )
+                    first_info_sent = True
 
-            # Sample data to be sent to the trainers
-            training_steps = learning_starts if update == learning_starts else 1
-            sample = rb.sample_tensors(
-                batch_size=training_steps
-                * cfg.algo.per_rank_gradient_steps
-                * cfg.algo.per_rank_batch_size
-                * (fabric.world_size - 1),
-                sample_next_obs=cfg.buffer.sample_next_obs,
-                dtype=None,
-                device=device,
-                from_numpy=cfg.buffer.from_numpy,
-            )
-            # chunks = {k1: [k1_chunk_1, k1_chunk_2, ...], k2: [k2_chunk_1, k2_chunk_2, ...]}
-            chunks = {
-                k: v.float().split(training_steps * cfg.algo.per_rank_gradient_steps * cfg.algo.per_rank_batch_size)
-                for k, v in sample.items()
-            }
-            # chunks = [{k1: k1_chunk_1, k2: k2_chunk_1}, {k1: k1_chunk_2, k2: k2_chunk_2}, ...]
-            chunks = [{k: v[i] for k, v in chunks.items()} for i in range(len(chunks[next(iter(chunks.keys()))]))]
-            world_collective.scatter_object_list([None], [None] + chunks, src=0)
-
-            # Wait the trainers to finish
-            player_trainer_collective.broadcast(flattened_parameters, src=1)
-
-            # Convert back the parameters
-            torch.nn.utils.convert_parameters.vector_to_parameters(flattened_parameters, actor.parameters())
-
-            # Logs trainers-only metrics
-            if cfg.metric.log_level > 0 and policy_step - last_log >= cfg.metric.log_every:
-                # Gather metrics from the trainers
-                metrics = [None]
-                player_trainer_collective.broadcast_object_list(metrics, src=1)
+                # Sample data to be sent to the trainers
+                sample = rb.sample_tensors(
+                    batch_size=per_rank_gradient_steps * cfg.algo.per_rank_batch_size * (fabric.world_size - 1),
+                    sample_next_obs=cfg.buffer.sample_next_obs,
+                    dtype=None,
+                    device=device,
+                    from_numpy=cfg.buffer.from_numpy,
+                )
+                # chunks = {k1: [k1_chunk_1, k1_chunk_2, ...], k2: [k2_chunk_1, k2_chunk_2, ...]}
+                chunks = {
+                    k: v.float().split(per_rank_gradient_steps * cfg.algo.per_rank_batch_size)
+                    for k, v in sample.items()
+                }
+                # chunks = [{k1: k1_chunk_1, k2: k2_chunk_1}, {k1: k1_chunk_2, k2: k2_chunk_2}, ...]
+                chunks = [{k: v[i] for k, v in chunks.items()} for i in range(len(chunks[next(iter(chunks.keys()))]))]
+                world_collective.scatter_object_list([None], [None] + chunks, src=0)
+
+                # Wait the trainers to finish
+                player_trainer_collective.broadcast(flattened_parameters, src=1)
+
+                # Convert back the parameters
+                torch.nn.utils.convert_parameters.vector_to_parameters(flattened_parameters, actor.parameters())
+
+                # Logs trainers-only metrics
+                if cfg.metric.log_level > 0 and policy_step - last_log >= cfg.metric.log_every:
+                    # Gather metrics from the trainers
+                    metrics = [None]
+                    player_trainer_collective.broadcast_object_list(metrics, src=1)
 
-                # Log metrics
-                fabric.log_dict(metrics[0], policy_step)
+                    # Log metrics
+                    fabric.log_dict(metrics[0], policy_step)
 
         # Logs player-only metrics
         if cfg.metric.log_level > 0 and policy_step - last_log >= cfg.metric.log_every:
             if aggregator and not aggregator.disabled:
                 fabric.log_dict(aggregator.compute(), policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio",
+                cumulative_per_rank_gradient_steps * (fabric.world_size - 1) / policy_step,
+                policy_step,
+            )
+
             # Sync timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 fabric.log(
                     "Time/sps_env_interaction",
                     ((policy_step - last_log) * cfg.env.action_repeat) / timer_metrics["Time/env_interaction_time"],
                     policy_step,
@@ -292,27 +304,29 @@
             ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
             fabric.call(
                 "on_checkpoint_player",
                 fabric=fabric,
                 player_trainer_collective=player_trainer_collective,
                 ckpt_path=ckpt_path,
                 replay_buffer=rb if cfg.buffer.checkpoint else None,
+                ratio_state_dict=ratio.state_dict(),
             )
 
     world_collective.scatter_object_list([None], [None] + [-1] * (world_collective.world_size - 1), src=0)
 
     # Last Checkpoint
     if cfg.checkpoint.save_last:
         ckpt_path = log_dir + f"/checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt"
         fabric.call(
             "on_checkpoint_player",
             fabric=fabric,
             player_trainer_collective=player_trainer_collective,
             ckpt_path=ckpt_path,
             replay_buffer=rb if cfg.buffer.checkpoint else None,
+            ratio_state_dict=ratio.state_dict(),
         )
 
     envs.close()
     if fabric.is_global_zero and cfg.algo.run_test:
         test(actor, fabric, cfg, log_dir)
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
@@ -348,16 +362,14 @@
     cfg.fabric.pop("loggers", None)
     cfg.fabric.pop("strategy", None)
     fabric: Fabric = hydra.utils.instantiate(
         cfg.fabric, strategy=DDPStrategy(process_group=optimization_pg), _convert_="all"
     )
     fabric.launch()
     device = fabric.device
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     # Resume from checkpoint
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     # Receive (possibly updated, by the make_env method for example) cfg from the player
     data = [None]
@@ -366,15 +378,15 @@
 
     # Environment setup
     vectorized_env = gym.vector.SyncVectorEnv if cfg.env.sync_env else gym.vector.AsyncVectorEnv
     envs = vectorized_env([make_env(cfg, 0, 0, None)])
     assert isinstance(envs.single_action_space, gym.spaces.Box), "only continuous action space is supported"
 
     # Define the agent and the optimizer and setup them with Fabric
-    agent = build_agent(
+    agent, _ = build_agent(
         fabric,
         cfg,
         envs.single_observation_space,
         envs.single_action_space,
         state["agent"] if cfg.checkpoint.resume_from else None,
     )
 
@@ -399,15 +411,15 @@
         )
 
     # Metrics
     aggregator = None
     if not MetricAggregator.disabled:
         aggregator: MetricAggregator = hydra.utils.instantiate(cfg.metric.aggregator, _convert_="all").to(device)
 
-    # Receive data from player reagrding the:
+    # Receive data from player regarding the:
     # * update
     # * last_log
     # * last_checkpoint
     data = [None]
     world_collective.broadcast_object_list(data, src=0)
     update = data[0]["update"]
     last_log = data[0]["last_log"]
@@ -562,10 +574,10 @@
     # Create a new group, without assigning it to the collective: in this way the trainers can
     # still communicate with the player through the global group, but they can optimize the agent
     # between themselves
     optimization_pg = world_collective.new_group(
         ranks=list(range(1, world_collective.world_size)), timeout=timedelta(days=1)
     )
     if global_rank == 0:
-        player(fabric, cfg, world_collective, player_trainer_collective)
+        player(fabric, world_collective, player_trainer_collective, cfg)
     else:
         trainer(world_collective, player_trainer_collective, optimization_pg, cfg)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/sac/utils.py` & `sheeprl-0.5.5/sheeprl/algos/sac/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 import warnings
 from typing import TYPE_CHECKING, Any, Dict, Sequence
 
 import gymnasium as gym
+import numpy as np
 import torch
 from lightning import Fabric
 from lightning.fabric.wrappers import _FabricModule
+from torch import Tensor
 
-from sheeprl.algos.sac.agent import SACActor, build_agent
+from sheeprl.algos.sac.agent import SACPlayer, build_agent
 from sheeprl.utils.env import make_env
 from sheeprl.utils.imports import _IS_MLFLOW_AVAILABLE
 from sheeprl.utils.utils import unwrap_fabric
 
 if TYPE_CHECKING:
     from mlflow.models.model import ModelInfo
 
@@ -22,39 +24,36 @@
     "Loss/value_loss",
     "Loss/policy_loss",
     "Loss/alpha_loss",
 }
 MODELS_TO_REGISTER = {"agent"}
 
 
+def prepare_obs(fabric: Fabric, obs: Dict[str, np.ndarray], *, num_envs: int = 1, **kwargs) -> Tensor:
+    with fabric.device:
+        torch_obs = torch.cat([torch.as_tensor(obs[k].copy(), dtype=torch.float32) for k in obs.keys()], dim=-1)
+    return torch_obs.reshape(num_envs, -1)
+
+
 @torch.no_grad()
-def test(actor: SACActor, fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
+def test(actor: SACPlayer, fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
     env = make_env(cfg, None, 0, log_dir, "test", vector_env_idx=0)()
     actor.eval()
     done = False
     cumulative_rew = 0
-    with fabric.device:
-        o = env.reset(seed=cfg.seed)[0]
-        next_obs = torch.cat(
-            [torch.as_tensor(o[k], dtype=torch.float32) for k in cfg.algo.mlp_keys.encoder], dim=-1
-        ).unsqueeze(
-            0
-        )  # [N_envs, N_obs]
+    obs = env.reset(seed=cfg.seed)[0]
     while not done:
         # Act greedly through the environment
-        action = actor.get_greedy_actions(next_obs)
+        torch_obs = prepare_obs(fabric, obs)
+        action = actor.get_actions(torch_obs, greedy=True)
 
         # Single environment step
-        next_obs, reward, done, truncated, info = env.step(action.cpu().numpy().reshape(env.action_space.shape))
+        obs, reward, done, truncated, info = env.step(action.cpu().numpy().reshape(env.action_space.shape))
         done = done or truncated
         cumulative_rew += reward
-        with fabric.device:
-            next_obs = torch.cat(
-                [torch.as_tensor(next_obs[k], dtype=torch.float32) for k in cfg.algo.mlp_keys.encoder], dim=-1
-            )
 
         if cfg.dry_run:
             done = True
     fabric.print("Test - Reward:", cumulative_rew)
     if cfg.metric.log_level > 0:
         fabric.logger.log_metrics({"Test/cumulative_reward": cumulative_rew}, 0)
     env.close()
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/sac_ae/agent.py` & `sheeprl-0.5.5/sheeprl/algos/sac_ae/agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+from __future__ import annotations
+
 import copy
 from math import prod
 from typing import Any, Dict, List, Optional, Sequence, SupportsFloat, Tuple, Union
 
 import gymnasium
+import hydra
 import numpy as np
 import torch
 import torch.nn as nn
 from lightning import Fabric
 from lightning.fabric.wrappers import _FabricModule
 from numpy.typing import NDArray
 from torch import Size, Tensor
 
 from sheeprl.algos.sac_ae.utils import weight_init
 from sheeprl.models.models import CNN, MLP, DeCNN, MultiDecoder, MultiEncoder
+from sheeprl.utils.fabric import get_single_device_fabric
 from sheeprl.utils.model import cnn_forward
 
 LOG_STD_MAX = 2
 LOG_STD_MIN = -10
 
 
 class CNNEncoder(CNN):
@@ -67,14 +71,17 @@
         self.input_dim = in_channels
 
     @property
     def conv_output_shape(self) -> Size:
         return self._conv_output_shape
 
     def forward(self, obs: Dict[str, Tensor], *, detach_encoder_features: bool = False, **kwargs) -> Tensor:
+        dtypes = [obs[k].dtype for k in self.keys]
+        if dtypes.count(dtypes[0]) != len(dtypes):
+            raise ValueError("All the tensors must have the same dtype: {}".format(dtypes))
         x = torch.cat([obs[k] for k in self.keys], dim=-3)
         x = cnn_forward(self.model, x, x.shape[-3:], (-1,))
         if detach_encoder_features:
             x = x.detach()
         x = self.fc(x)
         return x
 
@@ -98,15 +105,18 @@
             norm_layer=nn.LayerNorm if layer_norm else None,
             norm_args=[{"normalized_shape": dense_units}] * mlp_layers if layer_norm else None,
         )
         self.output_dim = dense_units
         self.input_dim = input_dim
 
     def forward(self, obs: Dict[str, Tensor], *args, detach_encoder_features: bool = False, **kwargs) -> Tensor:
-        x = torch.cat([obs[k] for k in self.keys], dim=-1).type(torch.float32)
+        dtypes = [obs[k].dtype for k in self.keys]
+        if dtypes.count(dtypes[0]) != len(dtypes):
+            raise ValueError("All the tensors must have the same dtype: {}".format(dtypes))
+        x = torch.cat([obs[k] for k in self.keys], dim=-1)
         x = self.model(x)
         if detach_encoder_features:
             x = x.detach()
         return x
 
 
 class MLPDecoder(nn.Module):
@@ -269,28 +279,28 @@
         mean = self.fc_mean(x)
         log_std = self.fc_logstd(x)
         # log_std = torch.clamp(log_std, LOG_STD_MIN, LOG_STD_MAX)
         log_std = torch.tanh(log_std)
         log_std = LOG_STD_MIN + 0.5 * (LOG_STD_MAX - LOG_STD_MIN) * (log_std + 1)
         return self.get_actions_and_log_probs(mean, log_std.exp())
 
-    def get_actions_and_log_probs(self, mean: Tensor, std: Tensor):
+    def get_actions_and_log_probs(self, mean: Tensor, std: Tensor) -> Tuple[Tensor, Tensor]:
         """Given the mean and the std of a Normal distribution, it returns a tanh-squashed
         sampled action (correctly rescaled to the environment action bounds) and its
         log-prob (as defined in Eq. 26 of https://arxiv.org/abs/1812.05905)
 
         Args:
             mean (Tensor): the mean of the distribution
             std (Tensor): the standard deviation of the distribution
 
         Returns:
             tanh-squashed action, rescaled to the environment action bounds
             action log-prob
         """
-        normal = torch.distributions.Normal(mean, std, validate_args=self.distribution_cfg.validate_args)
+        normal = torch.distributions.Normal(mean, std)
 
         # Reparameterization trick (mean + std * N(0,1))
         x_t = normal.rsample()
 
         # Squash sample
         y_t = torch.tanh(x_t)
 
@@ -303,29 +313,14 @@
         log_prob -= torch.log(self.action_scale * (1 - y_t.pow(2)) + 1e-6)
 
         # Log-prob of independent actions is the sum of the log-probs
         log_prob = log_prob.sum(-1, keepdim=True)
 
         return action, log_prob
 
-    def get_greedy_actions(self, obs: Tensor) -> Tensor:
-        """Get the action given the input observation greedily
-
-        Args:
-            obs (Tensor): input observation
-
-        Returns:
-            action
-        """
-        features = self.encoder(obs)
-        x = self.model(features)
-        mean = self.fc_mean(x)
-        mean = torch.tanh(mean) * self.action_scale + self.action_bias
-        return mean
-
 
 class SACAEAgent(nn.Module):
     def __init__(
         self,
         actor: Union[SACAEContinuousActor, _FabricModule],
         critic: Union[SACAECritic, _FabricModule],
         target_entropy: float,
@@ -402,14 +397,19 @@
         self._actor = actor
         return
 
     @property
     def critic_target(self) -> SACAECritic:
         return self._critic_target
 
+    @critic_target.setter
+    def critic_target(self, critic_target: SACAECritic | _FabricModule) -> None:
+        self._critic_target = critic_target
+        return
+
     @property
     def alpha(self) -> float:
         return self._log_alpha.exp().item()
 
     @property
     def target_entropy(self) -> Tensor:
         return self._target_entropy
@@ -417,17 +417,14 @@
     @property
     def log_alpha(self) -> Tensor:
         return self._log_alpha
 
     def get_actions_and_log_probs(self, obs: Tensor, detach_encoder_features: bool = False) -> Tuple[Tensor, Tensor]:
         return self.actor(obs, detach_encoder_features)
 
-    def get_greedy_actions(self, obs: Tensor) -> Tensor:
-        return self.actor.get_greedy_actions(obs)
-
     def get_q_values(self, obs: Tensor, action: Tensor, detach_encoder_features: bool = False) -> Tensor:
         return self.critic(obs, action, detach_encoder_features)
 
     @torch.no_grad()
     def get_target_q_values(self, obs: Tensor, action: Tensor) -> Tensor:
         return self.critic_target(obs, action)
 
@@ -449,23 +446,75 @@
     def critic_encoder_target_ema(self) -> None:
         for param, target_param in zip(
             self.critic_unwrapped.encoder.parameters(), self.critic_target.encoder.parameters()
         ):
             target_param.data.copy_(self._encoder_tau * param.data + (1 - self._encoder_tau) * target_param.data)
 
 
+class SACAEPlayer(nn.Module):
+    def __init__(
+        self,
+        feature_extractor: MultiEncoder,
+        fc: nn.Module,
+        fc_mean: nn.Module,
+        fc_logstd: nn.Module,
+        action_low: Union[SupportsFloat, NDArray] = -1.0,
+        action_high: Union[SupportsFloat, NDArray] = 1.0,
+    ):
+        super().__init__()
+        self.encoder = feature_extractor
+        self.model = fc
+        self.fc_mean = fc_mean
+        self.fc_logstd = fc_logstd
+
+        # Action rescaling buffers
+        self.register_buffer("action_scale", torch.tensor((action_high - action_low) / 2.0, dtype=torch.float32))
+        self.register_buffer("action_bias", torch.tensor((action_high + action_low) / 2.0, dtype=torch.float32))
+
+    def forward(self, obs: Tensor, greedy: bool = False) -> Tensor:
+        """Given an observation, it returns a tanh-squashed
+        sampled action (correctly rescaled to the environment action bounds) and its
+        log-prob (as defined in Eq. 26 of https://arxiv.org/abs/1812.05905)
+
+        Args:
+            obs (Tensor): the observation tensor
+
+        Returns:
+            tanh-squashed action, rescaled to the environment action bounds
+            action log-prob
+        """
+        features = self.encoder(obs, detach_encoder_features=False)
+        x = self.model(features)
+        mean = self.fc_mean(x)
+        if greedy:
+            return torch.tanh(mean) * self.action_scale + self.action_bias
+        else:
+            log_std = self.fc_logstd(x)
+            # log_std = torch.clamp(log_std, LOG_STD_MIN, LOG_STD_MAX)
+            log_std = torch.tanh(log_std)
+            log_std = LOG_STD_MIN + 0.5 * (LOG_STD_MAX - LOG_STD_MIN) * (log_std + 1)
+            normal = torch.distributions.Normal(mean, log_std.exp())
+            x_t = normal.rsample()
+            y_t = torch.tanh(x_t)
+            actions = y_t * self.action_scale + self.action_bias
+            return actions
+
+    def get_actions(self, obs: Tensor, greedy: bool = False) -> Tensor:
+        return self(obs, greedy)
+
+
 def build_agent(
     fabric: Fabric,
     cfg: Dict[str, Any],
     obs_space: gymnasium.spaces.Dict,
     action_space: gymnasium.spaces.Box,
     agent_state: Optional[Dict[str, Tensor]] = None,
     encoder_state: Optional[Dict[str, Tensor]] = None,
     decoder_sate: Optional[Dict[str, Tensor]] = None,
-) -> Tuple[SACAEAgent, _FabricModule, _FabricModule]:
+) -> Tuple[SACAEAgent, _FabricModule, _FabricModule, SACAEPlayer]:
     act_dim = prod(action_space.shape)
     target_entropy = -act_dim
 
     # Define the encoder and decoder and setup them with fabric.
     # Then we will set the critic encoder and actor decoder as the unwrapped encoder module:
     # we do not need it wrapped with the strategy inside actor and critic
     cnn_channels = [prod(obs_space[k].shape[:-2]) for k in cfg.algo.cnn_keys.encoder]
@@ -483,15 +532,15 @@
     )
     mlp_encoder = (
         MLPEncoder(
             sum(mlp_dims),
             cfg.algo.mlp_keys.encoder,
             cfg.algo.encoder.dense_units,
             cfg.algo.encoder.mlp_layers,
-            eval(cfg.algo.encoder.dense_act),
+            hydra.utils.get_class(cfg.algo.encoder.dense_act),
             cfg.algo.encoder.layer_norm,
         )
         if cfg.algo.mlp_keys.encoder is not None and len(cfg.algo.mlp_keys.encoder) > 0
         else None
     )
     encoder = MultiEncoder(cnn_encoder, mlp_encoder)
     cnn_decoder = (
@@ -509,15 +558,15 @@
     mlp_decoder = (
         MLPDecoder(
             encoder.output_dim,
             mlp_dims,
             cfg.algo.mlp_keys.decoder,
             cfg.algo.decoder.dense_units,
             cfg.algo.decoder.mlp_layers,
-            eval(cfg.algo.decoder.dense_act),
+            hydra.utils.get_class(cfg.algo.decoder.dense_act),
             cfg.algo.decoder.layer_norm,
         )
         if cfg.algo.mlp_keys.decoder is not None and len(cfg.algo.mlp_keys.decoder) > 0
         else None
     )
     decoder = MultiDecoder(cnn_decoder, mlp_decoder)
     if encoder_state:
@@ -553,13 +602,39 @@
         encoder_tau=cfg.algo.encoder.tau,
         device=fabric.device,
     )
 
     if agent_state:
         agent.load_state_dict(agent_state)
 
+    # Setup player agent
+    player = SACAEPlayer(
+        copy.deepcopy(agent.actor.encoder),
+        copy.deepcopy(agent.actor.model),
+        copy.deepcopy(agent.actor.fc_mean),
+        copy.deepcopy(agent.actor.fc_logstd),
+        action_low=action_space.low,
+        action_high=action_space.high,
+    )
+
     encoder = fabric.setup_module(encoder)
     decoder = fabric.setup_module(decoder)
     agent.actor = fabric.setup_module(agent.actor)
     agent.critic = fabric.setup_module(agent.critic)
 
-    return agent, encoder, decoder
+    # Wrap the target critic with a single-device fabric. This lets the target critic
+    # to be on the same device as the agent and to run with the same precision
+    fabric_player = get_single_device_fabric(fabric)
+    agent.critic_target = fabric_player.setup_module(agent.critic_target)
+
+    # Setup player agent
+    player.encoder = fabric_player.setup_module(player.encoder)
+    player.model = fabric_player.setup_module(player.model)
+    player.fc_mean = fabric_player.setup_module(player.fc_mean)
+    player.fc_logstd = fabric_player.setup_module(player.fc_logstd)
+    player.action_scale = player.action_scale.to(fabric_player.device)
+    player.action_bias = player.action_bias.to(fabric_player.device)
+
+    # Tie weights between the agent and the player
+    for agent_p, player_p in zip(agent.actor.parameters(), player.parameters()):
+        player_p.data = agent_p.data
+    return agent, encoder, decoder, player
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/sac_ae/evaluate.py` & `sheeprl-0.5.5/sheeprl/algos/sac_ae/evaluate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Any, Dict
 
 import gymnasium as gym
 from lightning import Fabric
 
-from sheeprl.algos.sac_ae.agent import SACAEAgent, build_agent
+from sheeprl.algos.sac_ae.agent import build_agent
 from sheeprl.algos.sac_ae.utils import test
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.registry import register_evaluation
 
 
 @register_evaluation(algorithms="sac_ae")
@@ -34,12 +34,11 @@
     action_space = env.action_space
     if not isinstance(observation_space, gym.spaces.Dict):
         raise RuntimeError(f"Unexpected observation type, should be of type Dict, got: {observation_space}")
 
     fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
     fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
 
-    agent: SACAEAgent
-    agent, _, _ = build_agent(
+    _, _, _, agent = build_agent(
         fabric, cfg, observation_space, action_space, state["agent"], state["encoder"], state["decoder"]
     )
-    test(agent.actor, fabric, cfg, log_dir)
+    test(agent, fabric, cfg, log_dir)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/sac_ae/sac_ae.py` & `sheeprl-0.5.5/sheeprl/algos/sac_ae/sac_ae.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import copy
 import os
-import time
 import warnings
 from typing import Any, Dict, Optional, Union
 
 import gymnasium as gym
 import hydra
 import numpy as np
 import torch
@@ -18,74 +17,70 @@
 from torch.optim import Optimizer
 from torch.utils.data.distributed import DistributedSampler
 from torch.utils.data.sampler import BatchSampler
 from torchmetrics import SumMetric
 
 from sheeprl.algos.sac.loss import critic_loss, entropy_loss, policy_loss
 from sheeprl.algos.sac_ae.agent import SACAEAgent, build_agent
-from sheeprl.algos.sac_ae.utils import preprocess_obs, test
+from sheeprl.algos.sac_ae.utils import prepare_obs, preprocess_obs, test
 from sheeprl.data.buffers import ReplayBuffer
 from sheeprl.models.models import MultiDecoder, MultiEncoder
 from sheeprl.utils.env import make_env
 from sheeprl.utils.logger import get_log_dir, get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import register_algorithm
 from sheeprl.utils.timer import timer
-from sheeprl.utils.utils import save_configs
+from sheeprl.utils.utils import Ratio, save_configs
 
 
 def train(
     fabric: Fabric,
     agent: SACAEAgent,
     encoder: Union[MultiEncoder, _FabricModule],
     decoder: Union[MultiDecoder, _FabricModule],
     actor_optimizer: Optimizer,
     qf_optimizer: Optimizer,
     alpha_optimizer: Optimizer,
     encoder_optimizer: Optimizer,
     decoder_optimizer: Optimizer,
     data: Dict[str, Tensor],
     aggregator: MetricAggregator | None,
-    update: int,
+    cumulative_per_rank_gradient_steps: int,
     cfg: Dict[str, Any],
-    policy_steps_per_update: int,
     group: Optional[CollectibleGroup] = None,
 ):
-    critic_target_network_frequency = cfg.algo.critic.target_network_frequency // policy_steps_per_update + 1
-    actor_network_frequency = cfg.algo.actor.network_frequency // policy_steps_per_update + 1
-    decoder_update_freq = cfg.algo.decoder.update_freq // policy_steps_per_update + 1
-    normalized_obs = {}
     normalized_next_obs = {}
+    normalized_obs = {}
     for k in cfg.algo.cnn_keys.encoder + cfg.algo.mlp_keys.encoder:
         if k in cfg.algo.cnn_keys.encoder:
             normalized_obs[k] = data[k] / 255.0
             normalized_next_obs[k] = data[f"next_{k}"] / 255.0
         else:
             normalized_obs[k] = data[k]
             normalized_next_obs[k] = data[f"next_{k}"]
 
     # Update the soft-critic
     next_target_qf_value = agent.get_next_target_q_values(
-        normalized_next_obs, data["rewards"], data["dones"], cfg.algo.gamma
+        normalized_next_obs, data["rewards"], data["terminated"], cfg.algo.gamma
     )
     qf_values = agent.get_q_values(normalized_obs, data["actions"])
     qf_loss = critic_loss(qf_values, next_target_qf_value, agent.num_critics)
     qf_optimizer.zero_grad(set_to_none=True)
     fabric.backward(qf_loss)
     qf_optimizer.step()
     if aggregator and not aggregator.disabled:
         aggregator.update("Loss/value_loss", qf_loss)
 
     # Update the target networks with EMA
-    if update % critic_target_network_frequency == 0:
+    if cumulative_per_rank_gradient_steps % cfg.algo.critic.per_rank_target_network_update_freq == 0:
         agent.critic_target_ema()
         agent.critic_encoder_target_ema()
 
     # Update the actor
-    if update % actor_network_frequency == 0:
+    if cumulative_per_rank_gradient_steps % cfg.algo.actor.per_rank_update_freq == 0:
         actions, logprobs = agent.get_actions_and_log_probs(normalized_obs, detach_encoder_features=True)
         qf_values = agent.get_q_values(normalized_obs, actions, detach_encoder_features=True)
         min_qf_values = torch.min(qf_values, dim=-1, keepdim=True)[0]
         actor_loss = policy_loss(agent.alpha, logprobs, min_qf_values)
         actor_optimizer.zero_grad(set_to_none=True)
         fabric.backward(actor_loss)
         actor_optimizer.step()
@@ -98,15 +93,15 @@
         alpha_optimizer.step()
 
         if aggregator and not aggregator.disabled:
             aggregator.update("Loss/policy_loss", actor_loss)
             aggregator.update("Loss/alpha_loss", alpha_loss)
 
     # Update the decoder
-    if update % decoder_update_freq == 0:
+    if cumulative_per_rank_gradient_steps % cfg.algo.decoder.per_rank_update_freq == 0:
         hidden = encoder(normalized_obs)
         reconstruction = decoder(hidden)
         reconstruction_loss = 0
         for k in cfg.algo.cnn_keys.decoder + cfg.algo.mlp_keys.decoder:
             target = preprocess_obs(data[k], bits=5) if k in cfg.algo.cnn_keys.decoder else data[k]
             reconstruction_loss += (
                 F.mse_loss(target, reconstruction[k])  # Reconstruction
@@ -130,16 +125,14 @@
             "in order to play correctly the game. "
             "As an alternative you can use one of the Dreamers' agents."
         )
 
     device = fabric.device
     rank = fabric.global_rank
     world_size = fabric.world_size
-    fabric.seed_everything(cfg.seed)
-    torch.backends.cudnn.deterministic = cfg.torch_deterministic
 
     # Resume from checkpoint
     if cfg.checkpoint.resume_from:
         state = fabric.load(cfg.checkpoint.resume_from)
 
     # These arguments cannot be changed
     cfg.env.screen_size = 64
@@ -196,35 +189,49 @@
         fabric.print("Encoder CNN keys:", cfg.algo.cnn_keys.encoder)
         fabric.print("Encoder MLP keys:", cfg.algo.mlp_keys.encoder)
         fabric.print("Decoder CNN keys:", cfg.algo.cnn_keys.decoder)
         fabric.print("Decoder MLP keys:", cfg.algo.mlp_keys.decoder)
     obs_keys = cfg.algo.cnn_keys.encoder + cfg.algo.mlp_keys.encoder
 
     # Define the agent and the optimizer and setup them with Fabric
-    agent, encoder, decoder = build_agent(
+    agent, encoder, decoder, player = build_agent(
         fabric,
         cfg,
         observation_space,
         envs.single_action_space,
         state["agent"] if cfg.checkpoint.resume_from else None,
         state["encoder"] if cfg.checkpoint.resume_from else None,
         state["decoder"] if cfg.checkpoint.resume_from else None,
     )
 
     # Optimizers
-    qf_optimizer = hydra.utils.instantiate(cfg.algo.critic.optimizer, params=agent.critic.parameters(), _convert_="all")
+    qf_optimizer = hydra.utils.instantiate(
+        cfg.algo.critic.optimizer,
+        params=agent.critic.parameters(),
+        _convert_="all",
+    )
     actor_optimizer = hydra.utils.instantiate(
-        cfg.algo.actor.optimizer, params=agent.actor.parameters(), _convert_="all"
+        cfg.algo.actor.optimizer,
+        params=agent.actor.parameters(),
+        _convert_="all",
+    )
+    alpha_optimizer = hydra.utils.instantiate(
+        cfg.algo.alpha.optimizer,
+        params=[agent.log_alpha],
+        _convert_="all",
     )
-    alpha_optimizer = hydra.utils.instantiate(cfg.algo.alpha.optimizer, params=[agent.log_alpha], _convert_="all")
     encoder_optimizer = hydra.utils.instantiate(
-        cfg.algo.encoder.optimizer, params=encoder.parameters(), _convert_="all"
+        cfg.algo.encoder.optimizer,
+        params=encoder.parameters(),
+        _convert_="all",
     )
     decoder_optimizer = hydra.utils.instantiate(
-        cfg.algo.decoder.optimizer, params=decoder.parameters(), _convert_="all"
+        cfg.algo.decoder.optimizer,
+        params=decoder.parameters(),
+        _convert_="all",
     )
 
     if cfg.checkpoint.resume_from:
         qf_optimizer.load_state_dict(state["qf_optimizer"])
         actor_optimizer.load_state_dict(state["actor_optimizer"])
         alpha_optimizer.load_state_dict(state["alpha_optimizer"])
         encoder_optimizer.load_state_dict(state["encoder_optimizer"])
@@ -270,23 +277,27 @@
         (state["update"] // fabric.world_size) + 1
         if cfg.checkpoint.resume_from
         else 1
     )
     policy_step = state["update"] * cfg.env.num_envs if cfg.checkpoint.resume_from else 0
     last_log = state["last_log"] if cfg.checkpoint.resume_from else 0
     last_checkpoint = state["last_checkpoint"] if cfg.checkpoint.resume_from else 0
-    time.time()
     policy_steps_per_update = int(cfg.env.num_envs * fabric.world_size)
     num_updates = int(cfg.algo.total_steps // policy_steps_per_update) if not cfg.dry_run else 1
     learning_starts = cfg.algo.learning_starts // policy_steps_per_update if not cfg.dry_run else 0
     if cfg.checkpoint.resume_from:
         cfg.algo.per_rank_batch_size = state["batch_size"] // fabric.world_size
         if not cfg.buffer.checkpoint:
             learning_starts += start_step
 
+    # Create Ratio class
+    ratio = Ratio(cfg.algo.replay_ratio, pretrain_steps=cfg.algo.per_rank_pretrain_steps)
+    if cfg.checkpoint.resume_from:
+        ratio.load_state_dict(state["ratio"])
+
     # Warning for log and checkpoint every
     if cfg.metric.log_level > 0 and cfg.metric.log_every % policy_steps_per_update != 0:
         warnings.warn(
             f"The metric.log_every parameter ({cfg.metric.log_every}) is not a multiple of the "
             f"policy_steps_per_update value ({policy_steps_per_update}), so "
             "the metrics will be logged at the nearest greater multiple of the "
             "policy_steps_per_update value."
@@ -302,30 +313,29 @@
     # Get the first environment observation and start the optimization
     step_data = {}
     obs = envs.reset(seed=cfg.seed)[0]  # [N_envs, N_obs]
     for k in obs_keys:
         if k in cfg.algo.cnn_keys.encoder:
             obs[k] = obs[k].reshape(cfg.env.num_envs, -1, *obs[k].shape[-2:])
 
+    per_rank_gradient_steps = 0
+    cumulative_per_rank_gradient_steps = 0
     for update in range(start_step, num_updates + 1):
         policy_step += cfg.env.num_envs * fabric.world_size
 
         # Measure environment interaction time: this considers both the model forward
         # to get the action given the observation and the time taken into the environment
         with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
-            if update < learning_starts:
+            if update <= learning_starts:
                 actions = envs.action_space.sample()
             else:
-                with torch.no_grad():
-                    normalized_obs = {k: v / 255 if k in cfg.algo.cnn_keys.encoder else v for k, v in obs.items()}
-                    torch_obs = {k: torch.from_numpy(v).to(device).float() for k, v in normalized_obs.items()}
-                    actions, _ = agent.actor.module(torch_obs)
-                    actions = actions.cpu().numpy()
-            next_obs, rewards, dones, truncated, infos = envs.step(actions.reshape(envs.action_space.shape))
-            dones = np.logical_or(dones, truncated)
+                with torch.inference_mode():
+                    torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
+                    actions = player(torch_obs).cpu().numpy()
+            next_obs, rewards, terminated, truncated, infos = envs.step(actions.reshape(envs.action_space.shape))
 
         if cfg.metric.log_level > 0 and "final_info" in infos:
             for i, agent_ep_info in enumerate(infos["final_info"]):
                 if agent_ep_info is not None:
                     ep_rew = agent_ep_info["episode"]["r"]
                     ep_len = agent_ep_info["episode"]["l"]
                     if aggregator and not aggregator.disabled:
@@ -349,82 +359,88 @@
             if not cfg.buffer.sample_next_obs:
                 step_data[f"next_{k}"] = real_next_obs[k][np.newaxis]
                 if k in cfg.algo.cnn_keys.encoder:
                     step_data[f"next_{k}"] = step_data[f"next_{k}"].reshape(
                         1, cfg.env.num_envs, -1, *step_data[f"next_{k}"].shape[-2:]
                     )
 
-        step_data["dones"] = dones.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
+        step_data["terminated"] = terminated.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
+        step_data["truncated"] = truncated.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
         step_data["actions"] = actions.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
         step_data["rewards"] = rewards.reshape(1, cfg.env.num_envs, -1).astype(np.float32)
         rb.add(step_data, validate_args=cfg.buffer.validate_args)
 
         # next_obs becomes the new obs
         obs = next_obs
 
         # Train the agent
-        if update >= learning_starts - 1:
-            training_steps = learning_starts if update == learning_starts - 1 else 1
-
-            # We sample one time to reduce the communications between processes
-            sample = rb.sample_tensors(
-                training_steps * cfg.algo.per_rank_gradient_steps * cfg.algo.per_rank_batch_size,
-                sample_next_obs=cfg.buffer.sample_next_obs,
-                from_numpy=cfg.buffer.from_numpy,
-            )  # [G*B, 1]
-            gathered_data = fabric.all_gather(sample)  # [G*B, World, 1]
-            flatten_dim = 3 if fabric.world_size > 1 else 2
-            gathered_data = {k: v.view(-1, *v.shape[flatten_dim:]) for k, v in gathered_data.items()}  # [G*B*World]
-            len_data = len(gathered_data[next(iter(gathered_data.keys()))])
-            if fabric.world_size > 1:
-                dist_sampler: DistributedSampler = DistributedSampler(
-                    range(len_data),
-                    num_replicas=fabric.world_size,
-                    rank=fabric.global_rank,
-                    shuffle=True,
-                    seed=cfg.seed,
-                    drop_last=False,
-                )
-                sampler: BatchSampler = BatchSampler(
-                    sampler=dist_sampler, batch_size=cfg.algo.per_rank_batch_size, drop_last=False
-                )
-            else:
-                sampler = BatchSampler(
-                    sampler=range(len_data), batch_size=cfg.algo.per_rank_batch_size, drop_last=False
-                )
-
-            # Start training
-            with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
-                for batch_idxes in sampler:
-                    train(
-                        fabric,
-                        agent,
-                        encoder,
-                        decoder,
-                        actor_optimizer,
-                        qf_optimizer,
-                        alpha_optimizer,
-                        encoder_optimizer,
-                        decoder_optimizer,
-                        {k: v[batch_idxes] for k, v in gathered_data.items()},
-                        aggregator,
-                        update,
-                        cfg,
-                        policy_steps_per_update,
+        if update >= learning_starts:
+            per_rank_gradient_steps = ratio(policy_step / world_size)
+            if per_rank_gradient_steps > 0:
+                # We sample one time to reduce the communications between processes
+                sample = rb.sample_tensors(
+                    per_rank_gradient_steps * cfg.algo.per_rank_batch_size,
+                    sample_next_obs=cfg.buffer.sample_next_obs,
+                    from_numpy=cfg.buffer.from_numpy,
+                )  # [1, G*B]
+                gathered_data: Dict[str, torch.Tensor] = fabric.all_gather(sample)  # [World, 1, G*B]
+                for k, v in gathered_data.items():
+                    gathered_data[k] = v.flatten(start_dim=0, end_dim=2).float()  # [G*B*World]
+                len_data = len(gathered_data[next(iter(gathered_data.keys()))])
+                if fabric.world_size > 1:
+                    dist_sampler: DistributedSampler = DistributedSampler(
+                        range(len_data),
+                        num_replicas=fabric.world_size,
+                        rank=fabric.global_rank,
+                        shuffle=True,
+                        seed=cfg.seed,
+                        drop_last=False,
+                    )
+                    sampler: BatchSampler = BatchSampler(
+                        sampler=dist_sampler, batch_size=cfg.algo.per_rank_batch_size, drop_last=False
+                    )
+                else:
+                    sampler = BatchSampler(
+                        sampler=range(len_data), batch_size=cfg.algo.per_rank_batch_size, drop_last=False
                     )
-                train_step += world_size
+
+                # Start training
+                with timer("Time/train_time", SumMetric, sync_on_compute=cfg.metric.sync_on_compute):
+                    for batch_idxes in sampler:
+                        train(
+                            fabric,
+                            agent,
+                            encoder,
+                            decoder,
+                            actor_optimizer,
+                            qf_optimizer,
+                            alpha_optimizer,
+                            encoder_optimizer,
+                            decoder_optimizer,
+                            {k: v[batch_idxes] for k, v in gathered_data.items()},
+                            aggregator,
+                            cumulative_per_rank_gradient_steps,
+                            cfg,
+                        )
+                        cumulative_per_rank_gradient_steps += 1
+                    train_step += world_size
 
         # Log metrics
         if cfg.metric.log_level and (policy_step - last_log >= cfg.metric.log_every or update == num_updates):
             # Sync distributed metrics
             if aggregator and not aggregator.disabled:
                 metrics_dict = aggregator.compute()
                 fabric.log_dict(metrics_dict, policy_step)
                 aggregator.reset()
 
+            # Log replay ratio
+            fabric.log(
+                "Params/replay_ratio", cumulative_per_rank_gradient_steps * world_size / policy_step, policy_step
+            )
+
             # Sync distributed timers
             if not timer.disabled:
                 timer_metrics = timer.compute()
                 if "Time/train_time" in timer_metrics:
                     fabric.log(
                         "Time/sps_train",
                         (train_step - last_train) / timer_metrics["Time/train_time"],
@@ -453,14 +469,15 @@
                 "encoder": encoder.state_dict(),
                 "decoder": decoder.state_dict(),
                 "qf_optimizer": qf_optimizer.state_dict(),
                 "actor_optimizer": actor_optimizer.state_dict(),
                 "alpha_optimizer": alpha_optimizer.state_dict(),
                 "encoder_optimizer": encoder_optimizer.state_dict(),
                 "decoder_optimizer": decoder_optimizer.state_dict(),
+                "ratio": ratio.state_dict(),
                 "update": update * fabric.world_size,
                 "batch_size": cfg.algo.per_rank_batch_size * fabric.world_size,
                 "last_log": last_log,
                 "last_checkpoint": last_checkpoint,
             }
             ckpt_path = os.path.join(log_dir, f"checkpoint/ckpt_{policy_step}_{fabric.global_rank}.ckpt")
             fabric.call(
@@ -469,15 +486,15 @@
                 ckpt_path=ckpt_path,
                 state=state,
                 replay_buffer=rb if cfg.buffer.checkpoint else None,
             )
 
     envs.close()
     if fabric.is_global_zero and cfg.algo.run_test:
-        test(agent.actor.module, fabric, cfg, log_dir)
+        test(player, fabric, cfg, log_dir)
 
     if not cfg.model_manager.disabled and fabric.is_global_zero:
         from sheeprl.algos.sac_ae.utils import log_models
         from sheeprl.utils.mlflow import register_model
 
         models_to_log = {"agent": agent, "encoder": encoder, "decoder": decoder}
         register_model(fabric, log_models, cfg, models_to_log)
```

### Comparing `sheeprl-0.5.4/sheeprl/algos/sac_ae/utils.py` & `sheeprl-0.5.5/sheeprl/algos/sac_ae/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,66 @@
 from __future__ import annotations
 
 import warnings
 from typing import TYPE_CHECKING, Any, Dict, Sequence
 
 import gymnasium as gym
+import numpy as np
 import torch
 import torch.nn as nn
 from lightning import Fabric
 from lightning.fabric.wrappers import _FabricModule
 from torch import Tensor
 
 from sheeprl.algos.sac.utils import AGGREGATOR_KEYS
 from sheeprl.utils.env import make_env
 from sheeprl.utils.imports import _IS_MLFLOW_AVAILABLE
 from sheeprl.utils.utils import unwrap_fabric
 
 if TYPE_CHECKING:
     from mlflow.models.model import ModelInfo
 
-    from sheeprl.algos.sac_ae.agent import SACAEContinuousActor
+    from sheeprl.algos.sac_ae.agent import SACAEPlayer
 
 AGGREGATOR_KEYS = AGGREGATOR_KEYS.union({"Loss/reconstruction_loss"})
 MODELS_TO_REGISTER = {"agent", "encoder", "decoder"}
 
 
+def prepare_obs(
+    fabric: Fabric, obs: Dict[str, np.ndarray], *, cnn_keys: Sequence[str] = [], num_envs: int = 1, **kwargs
+) -> Dict[str, Tensor]:
+    torch_obs = {}
+    for k in obs.keys():
+        torch_obs[k] = torch.from_numpy(obs[k].copy()).to(fabric.device).float()
+        if k in cnn_keys:
+            torch_obs[k] = torch_obs[k].reshape(num_envs, -1, *torch_obs[k].shape[-2:]) / 255
+        else:
+            torch_obs[k] = torch_obs[k].reshape(num_envs, -1)
+
+    return torch_obs
+
+
 @torch.no_grad()
-def test(actor: "SACAEContinuousActor", fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
+def test(actor: "SACAEPlayer", fabric: Fabric, cfg: Dict[str, Any], log_dir: str):
     env = make_env(cfg, cfg.seed, 0, log_dir, "test", vector_env_idx=0)()
-    cnn_keys = actor.encoder.cnn_keys
-    mlp_keys = actor.encoder.mlp_keys
     actor.eval()
     done = False
     cumulative_rew = 0
-    next_obs = {}
-    o = env.reset(seed=cfg.seed)[0]  # [N_envs, N_obs]
-    for k in o.keys():
-        if k in mlp_keys + cnn_keys:
-            torch_obs = torch.from_numpy(o[k]).to(fabric.device).unsqueeze(0)
-            if k in cnn_keys:
-                torch_obs = torch_obs.reshape(1, -1, *torch_obs.shape[-2:]) / 255
-            if k in mlp_keys:
-                torch_obs = torch_obs.float()
-            next_obs[k] = torch_obs
+    obs = env.reset(seed=cfg.seed)[0]  # [N_envs, N_obs]
 
     while not done:
+        torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder)
         # Act greedly through the environment
-        action = actor.get_greedy_actions(next_obs)
+        action = actor.get_actions(torch_obs, greedy=True)
 
         # Single environment step
-        o, reward, done, truncated, _ = env.step(action.cpu().numpy().reshape(env.action_space.shape))
+        obs, reward, done, truncated, _ = env.step(action.cpu().numpy().reshape(env.action_space.shape))
         done = done or truncated
         cumulative_rew += reward
 
-        next_obs = {}
-        for k in o.keys():
-            if k in mlp_keys + cnn_keys:
-                torch_obs = torch.from_numpy(o[k]).to(fabric.device).unsqueeze(0)
-                if k in cnn_keys:
-                    torch_obs = torch_obs.reshape(1, -1, *torch_obs.shape[-2:]) / 255
-                if k in mlp_keys:
-                    torch_obs = torch_obs.float()
-                next_obs[k] = torch_obs
-
         if cfg.dry_run:
             done = True
     fabric.print("Test - Reward:", cumulative_rew)
     if cfg.metric.log_level > 0:
         fabric.log_dict({"Test/cumulative_reward": cumulative_rew}, 0)
     env.close()
```

### Comparing `sheeprl-0.5.4/sheeprl/available_agents.py` & `sheeprl-0.5.5/sheeprl/available_agents.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/cli.py` & `sheeprl-0.5.5/sheeprl/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, Dict
 
 import hydra
 import torch
 from lightning import Fabric
 from lightning.fabric.strategies import STRATEGY_REGISTRY, DDPStrategy, SingleDeviceStrategy, Strategy
 from omegaconf import DictConfig, OmegaConf, open_dict
+from torch.distributions import Distribution
 
 from sheeprl.utils.imports import _IS_MLFLOW_AVAILABLE
 from sheeprl.utils.logger import get_logger
 from sheeprl.utils.metric import MetricAggregator
 from sheeprl.utils.registry import algorithm_registry, evaluation_registry
 from sheeprl.utils.timer import timer
 from sheeprl.utils.utils import dotdict, print_config
@@ -54,14 +55,17 @@
         cfg (Dict[str, Any]): the loaded configuration.
     """
 
     # Torch settings
     os.environ["OMP_NUM_THREADS"] = str(cfg.num_threads)
     torch.set_float32_matmul_precision(cfg.float32_matmul_precision)
 
+    # Set the distribution validate_args once here
+    Distribution.set_default_validate_args(cfg.distribution.validate_args)
+
     # Given the algorithm's name, retrieve the module where
     # 'cfg.algo.name'.py is contained; from there retrieve the
     # 'register_algorithm'-decorated entrypoint;
     # the entrypoint will be launched by Fabric with 'fabric.launch(entrypoint)'
     module = None
     decoupled = False
     entrypoint = None
@@ -162,29 +166,49 @@
             )
         else:
             predefined_models_keys = utils.MODELS_TO_REGISTER
         keys_to_remove = set(cfg.model_manager.models.keys()) - predefined_models_keys
         for k in keys_to_remove:
             cfg.model_manager.models.pop(k, None)
         cfg.model_manager.disabled == cfg.model_manager.disabled or len(cfg.model_manager.models) == 0
-    fabric.launch(command, cfg, **kwargs)
+
+    # This function is used to make the algorithm reproducible.
+    # It can be an overkill since Fabric already captures everything we're setting here
+    # when multiprocessing is used with a `spawn` method (default with DDP strategy).
+    # https://github.com/Lightning-AI/pytorch-lightning/blob/f23b3b1e7fdab1d325f79f69a28706d33144f27e/src/lightning/fabric/strategies/launchers/multiprocessing.py#L112
+    def reproducible(func):
+        def wrapper(fabric: Fabric, cfg: Dict[str, Any], *args, **kwargs):
+            if cfg.cublas_workspace_config is not None:
+                os.environ["CUBLAS_WORKSPACE_CONFIG"] = cfg.cublas_workspace_config
+            fabric.seed_everything(cfg.seed)
+            torch.backends.cudnn.benchmark = cfg.torch_backends_cudnn_benchmark
+            torch.backends.cudnn.deterministic = cfg.torch_backends_cudnn_deterministic
+            torch.use_deterministic_algorithms(cfg.torch_use_deterministic_algorithms)
+            return func(fabric, cfg, *args, **kwargs)
+
+        return wrapper
+
+    fabric.launch(reproducible(command), cfg, **kwargs)
 
 
 def eval_algorithm(cfg: DictConfig):
     """Run the algorithm specified in the configuration.
 
     Args:
         cfg (DictConfig): the loaded configuration.
     """
     cfg = dotdict(OmegaConf.to_container(cfg, resolve=True, throw_on_missing=True))
 
     # Torch settings
     os.environ["OMP_NUM_THREADS"] = str(cfg.num_threads)
     torch.set_float32_matmul_precision(cfg.float32_matmul_precision)
 
+    # Set the distribution validate_args once here
+    Distribution.set_default_validate_args(cfg.distribution.validate_args)
+
     # TODO: change the number of devices when FSDP will be supported
     accelerator = cfg.fabric.get("accelerator", "auto")
     fabric: Fabric = hydra.utils.instantiate(
         cfg.fabric, accelerator=accelerator, devices=1, num_nodes=1, _convert_="all"
     )
 
     # Seed everything
@@ -219,30 +243,37 @@
         raise RuntimeError(
             f"Given the module and algorithm named `{module}` and `{algo_name}` respectively, "
             "no evaluation file has been found to be imported."
         )
     task = importlib.import_module(f"{module}.{evaluation_file}")
     command = task.__dict__[entrypoint]
     if getattr(cfg, "disable_grads", True):
-        command = torch.no_grad(command)
+
+        def no_grad(func):
+            def wrapper(*args, **kwargs):
+                with torch.no_grad():
+                    return func(*args, **kwargs)
+
+            return wrapper
+
+        command = no_grad(command)
     fabric.launch(command, cfg, state)
 
 
 def check_configs(cfg: Dict[str, Any]):
     """Check the validity of the configuration.
 
     Args:
         cfg (Dict[str, Any]): the loaded configuration to check.
     """
     if cfg.float32_matmul_precision not in {"medium", "high", "highest"}:
         raise ValueError(
             f"Invalid value '{cfg.float32_matmul_precision}' for the 'float32_matmul_precision' parameter. "
             "It must be one of 'medium', 'high' or 'highest'."
         )
-
     decoupled = False
     algo_name = cfg.algo.name
     for _, _algos in algorithm_registry.items():
         for _algo in _algos:
             if algo_name == _algo["name"]:
                 decoupled = _algo["decoupled"]
                 break
@@ -302,15 +333,14 @@
 
 def check_configs_evaluation(cfg: DictConfig):
     if cfg.float32_matmul_precision not in {"medium", "high", "highest"}:
         raise ValueError(
             f"Invalid value '{cfg.float32_matmul_precision}' for the 'float32_matmul_precision' parameter. "
             "It must be one of 'medium', 'high' or 'highest'."
         )
-
     if cfg.checkpoint_path is None:
         raise ValueError("You must specify the evaluation checkpoint path")
 
 
 @hydra.main(version_base="1.3", config_path="configs", config_name="config")
 def run(cfg: DictConfig):
     """SheepRL zero-code command line utility."""
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/algo/a2c.yaml` & `sheeprl-0.5.5/sheeprl/configs/algo/a2c.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/algo/dreamer_v1.yaml` & `sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v1.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 gamma: 0.99
 lmbda: 0.95
 horizon: 15
 name: dreamer_v1
 
 # Training recipe
-train_every: 1000
+replay_ratio: 0.1
 learning_starts: 5000
-per_rank_gradient_steps: 100
+per_rank_pretrain_steps: 0
 per_rank_sequence_length: ???
 
 # Encoder and decoder keys
 cnn_keys:
   decoder: ${algo.cnn_keys.encoder}
 mlp_keys:
   decoder: ${algo.mlp_keys.encoder}
@@ -96,16 +96,15 @@
   init_std: 5.0
   dense_act: ${algo.dense_act}
   mlp_layers: ${algo.mlp_layers}
   dense_units: ${algo.dense_units}
   clip_gradients: 100.0
   expl_amount: 0.3
   expl_min: 0.0
-  expl_decay: False
-  max_step_expl_decay: 200000
+  expl_decay: 0.0
 
   # Actor optimizer
   optimizer:
     lr: 8e-5
     eps: 1e-5
     weight_decay: 0
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/algo/dreamer_v2.yaml` & `sheeprl-0.5.5/sheeprl/configs/algo/dreamer_v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 
 name: dreamer_v2
 gamma: 0.99
 lmbda: 0.95
 horizon: 15
 
 # Training recipe
-train_every: 5
+replay_ratio: 0.2
 learning_starts: 1000
-per_rank_gradient_steps: 1
 per_rank_pretrain_steps: 100
 per_rank_sequence_length: ???
 
 # Encoder and decoder keys
 cnn_keys:
   decoder: ${algo.cnn_keys.encoder}
 mlp_keys:
@@ -107,32 +106,28 @@
   init_std: 0.0
   objective_mix: 1.0
   dense_act: ${algo.dense_act}
   mlp_layers: ${algo.mlp_layers}
   layer_norm: ${algo.layer_norm}
   dense_units: ${algo.dense_units}
   clip_gradients: 100.0
-  expl_amount: 0.0
-  expl_min: 0.0
-  expl_decay: False
-  max_step_expl_decay: 0
 
   # Actor optimizer
   optimizer:
     lr: 8e-5
     eps: 1e-5
     weight_decay: 1e-6
 
 # Critic
 critic:
   dense_act: ${algo.dense_act}
   mlp_layers: ${algo.mlp_layers}
   layer_norm: ${algo.layer_norm}
   dense_units: ${algo.dense_units}
-  target_network_update_freq: 100
+  per_rank_target_network_update_freq: 100
   clip_gradients: 100.0
 
   # Critic optimizer
   optimizer:
     lr: 8e-5
     eps: 1e-5
     weight_decay: 1e-6
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/algo/p2e_dv1.yaml` & `sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv1.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/algo/p2e_dv2.yaml` & `sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv2.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/algo/p2e_dv3.yaml` & `sheeprl-0.5.5/sheeprl/configs/algo/p2e_dv3.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,13 +18,13 @@
     reward_type: task
 
 ensembles:
   n: 8 # the number of the ensembles
   dense_act: ${algo.dense_act}
   mlp_layers: ${algo.mlp_layers}
   dense_units: ${algo.dense_units}
-  layer_norm: ${algo.layer_norm}
+  layer_norm: ${algo.mlp_layer_norm}
   clip_gradients: 100
   optimizer:
     lr: 1e-4
     eps: 1e-5
     weight_decay: 0
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/algo/ppo.yaml` & `sheeprl-0.5.5/sheeprl/configs/algo/ppo.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/algo/ppo_recurrent.yaml` & `sheeprl-0.5.5/sheeprl/configs/algo/ppo_recurrent.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -3,42 +3,42 @@
   - _self_
 
 # Algo related parameters
 name: ppo_recurrent
 vf_coef: 0.2
 clip_coef: 0.2
 ent_coef: 0.001
-clip_vloss: True
+clip_vloss: False
 anneal_lr: False
 max_grad_norm: 0.5
-anneal_ent_coef: True
-normalize_advantages: True
+anneal_ent_coef: False
+normalize_advantages: False
 reset_recurrent_state_on_done: True
 per_rank_sequence_length: ???
 
 # Model related parameters
 mlp_layers: 1
 layer_norm: True
-dense_units: 256
+dense_units: 64
 dense_act: torch.nn.ReLU
 rnn:
   lstm:
-    hidden_size: 128
+    hidden_size: 64
   pre_rnn_mlp:
     bias: True
     apply: False
     activation: ${algo.dense_act}
     layer_norm: ${algo.layer_norm}
     dense_units: ${algo.encoder.dense_units}
   post_rnn_mlp:
     bias: True
     apply: False
     activation: ${algo.dense_act}
     layer_norm: ${algo.layer_norm}
     dense_units: ${algo.rnn.lstm.hidden_size}
 encoder:
-  dense_units: 128
+  dense_units: 64
 
 # Optimizer related parameters
 optimizer:
   lr: 3e-4
   _target_: torch.optim.AdamW
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/algo/sac.yaml` & `sheeprl-0.5.5/sheeprl/configs/algo/sac.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 name: sac
 tau: 0.005
 gamma: 0.99
 hidden_size: 256
 
 # Training recipe
+replay_ratio: 1.0
 learning_starts: 100
-per_rank_gradient_steps: 1
+per_rank_pretrain_steps: 0
 
 # Model related parameters
 # Actor
 actor:
   hidden_size: ${algo.hidden_size}
   optimizer:
     lr: 3e-4
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/algo/sac_ae.yaml` & `sheeprl-0.5.5/sheeprl/configs/algo/sac_ae.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,17 @@
   - /optim@encoder.optimizer: adam
   - /optim@decoder.optimizer: adam
   - _self_
 
 name: sac_ae
 
 # Training recipe
+replay_ratio: 1.0
 learning_starts: 1000
+per_rank_pretrain_steps: 0
 
 # Model related parameters
 cnn_channels_multiplier: 16
 dense_units: 64
 mlp_layers: 2
 dense_act: torch.nn.ReLU
 layer_norm: False
@@ -34,35 +36,35 @@
   optimizer:
     lr: 1e-3
     eps: 1e-08
 
 # Decoder
 decoder:
   l2_lambda: 1e-6
-  update_freq: 1
+  per_rank_update_freq: 1
   cnn_channels_multiplier: ${algo.cnn_channels_multiplier}
   dense_units: ${algo.dense_units}
   mlp_layers: ${algo.mlp_layers}
   dense_act: ${algo.dense_act}
   layer_norm: ${algo.layer_norm}
   optimizer:
     lr: 1e-3
     weight_decay: 1e-7
     eps: 1e-08
 
 # Override from `sac` config
 tau: 0.01
 hidden_size: 1024
 actor:
-  network_frequency: 2
+  per_rank_update_freq: 2
   optimizer:
     lr: 1e-3
     eps: 1e-08
 critic:
-  target_network_frequency: 2
+  per_rank_target_network_update_freq: 2
   optimizer:
     lr: 1e-3
     eps: 1e-08
 alpha:
   alpha: 0.1
   optimizer:
     lr: 1e-4
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/env/atari.yaml` & `sheeprl-0.5.5/sheeprl/configs/env/atari.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/env/diambra.yaml` & `sheeprl-0.5.5/sheeprl/configs/env/diambra.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 sync_env: False
 action_repeat: 1
 
 # Wrapper to be instantiated
 wrapper:
   _target_: sheeprl.envs.diambra.DiambraWrapper
   id: ${env.id}
-  action_space: diambra.arena.SpaceTypes.DISCRETE # or diambra.arena.SpaceTypes.MULTI_DISCRETE
+  action_space: DISCRETE # or MULTI_DISCRETE
   screen_size: ${env.screen_size}
   grayscale: ${env.grayscale}
   repeat_action: ${env.action_repeat}
   rank: null
   log_level: 0
   increase_performance: True
   diambra_settings:
-    role: diambra.arena.Roles.P1 # or diambra.arena.Roles.P2 or null
+    role: P1 # or P2 or null
     step_ratio: 6
     difficulty: 4
     continue_game: 0.0
     show_final: False
     outfits: 4
     splash_screen: False
   diambra_wrappers:
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/env/minerl.yaml` & `sheeprl-0.5.5/sheeprl/configs/env/minerl.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 defaults:
   - minecraft
   - _self_
 
 # Override from `minecraft` config
 id: custom_navigate
 action_repeat: 1
+max_episode_steps: 12000
+reward_as_observation: True
+num_envs: 4
 
 # Wrapper to be instantiated
 wrapper:
   _target_: sheeprl.envs.minerl.MineRLWrapper
   id: ${env.id}
   height: ${env.screen_size}
   width: ${env.screen_size}
   pitch_limits:
     - ${env.min_pitch}
     - ${env.max_pitch}
   seed: null
   break_speed_multiplier: ${env.break_speed_multiplier}
-  multihot_inventory: True
+  multihot_inventory: False
   sticky_attack: ${env.sticky_attack}
   sticky_jump: ${env.sticky_jump}
   dense: True
   extreme: False
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/a2c.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/a2c.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v1.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v1.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # @package _global_
 
 defaults:
   - dreamer_v1
   - override /env: atari
   - _self_
 
-# Experiment
-seed: 5
-
 # Environment
 env:
   num_envs: 1
   max_episode_steps: 27000
   id: MsPacmanNoFrameskip-v4
 
 # Checkpoint
@@ -22,18 +19,19 @@
 buffer:
   size: 16384
   checkpoint: True
 
 # Algorithm
 algo:
   learning_starts: 1024
-  train_every: 16
+  replay_ratio: 0.0625
+  
   dense_units: 8
   mlp_layers: 1
-  per_rank_gradient_steps: 1
+  
   world_model:
     stochastic_size: 4
     encoder:
       cnn_channels_multiplier: 2
     recurrent_model:
       recurrent_state_size: 8
     transition_model:
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v2.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # @package _global_
 
 defaults:
-  - override /algo: dreamer_v2
+  - override /algo: dreamer_v3_S
   - override /env: atari
-  - override /model_manager: dreamer_v2
+  - override /model_manager: dreamer_v3
   - _self_
 
 # Algorithm
 algo:
+  replay_ratio: 1
   total_steps: 5000000
   per_rank_batch_size: 16
-  per_rank_sequence_length: 50
+  per_rank_sequence_length: 64
   cnn_keys:
     encoder: [rgb]
     decoder: [rgb]
 
 # Checkpoint
 checkpoint:
   every: 100000
 
 # Buffer
 buffer:
-  size: 5000000
-  type: sequential
+  size: 1000000
   checkpoint: False
-  prioritize_ends: False
 
 # Distribution
 distribution:
   type: "auto"
 
 metric:
   aggregator:
@@ -50,24 +49,21 @@
         sync_on_compute: ${metric.sync_on_compute}
       Loss/state_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Loss/continue_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      State/post_entropy:
-        _target_: torchmetrics.MeanMetric
-        sync_on_compute: ${metric.sync_on_compute}
-      State/prior_entropy:
+      State/kl:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      State/kl:
+      State/post_entropy:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      Params/exploration_amount:
+      State/prior_entropy:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Grads/world_model:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Grads/actor:
         _target_: torchmetrics.MeanMetric
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # @package _global_
 
 defaults:
   - dreamer_v2
   - override /env: atari
   - _self_
 
-# Experiment
-seed: 5
-
 # Environment
 env:
   num_envs: 1
   max_episode_steps: 27000
   id: MsPacmanNoFrameskip-v4
 
 # Checkpoint
@@ -22,18 +19,19 @@
 buffer:
   size: 16384
   checkpoint: True
 
 # Algorithm
 algo:
   learning_starts: 1024
-  per_rank_pretrain_steps: 1
-  train_every: 16
+  per_rank_pretrain_steps: 0
+  replay_ratio: 0.0625
+  
   dense_units: 8
-  mlp_layers: 
+  mlp_layers: 1
   world_model:
     discrete_size: 4
     stochastic_size: 4
     encoder:
       cnn_channels_multiplier: 2
     recurrent_model:
       recurrent_state_size: 8
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v2_crafter.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_crafter.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
   encoder:
     - reward
   decoder: []
 
 # Algorithm
 algo:
   gamma: 0.999
-  train_every: 5
   layer_norm: True
   learning_starts: 10000
   per_rank_pretrain_steps: 1
   world_model:
     kl_free_nats: 0.0
     use_continues: True
     recurrent_model:
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -22,20 +22,20 @@
   type: episode
   checkpoint: True
   prioritize_ends: True
 
 # Algorithm
 algo:
   gamma: 0.995
-  train_every: 16
+  replay_ratio: 0.0625
   total_steps: 200000000
   learning_starts: 200000
   per_rank_batch_size: 32
   per_rank_pretrain_steps: 1
-  per_rank_gradient_steps: 1
+  
   world_model:
     use_continues: True
     kl_free_nats: 0.0
     kl_regularizer: 0.1
     discount_scale_factor: 0.5
     optimizer:
       lr: 0.0002
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v2.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # @package _global_
 
 defaults:
-  - override /algo: dreamer_v3_S
+  - override /algo: dreamer_v2
   - override /env: atari
-  - override /model_manager: dreamer_v3
+  - override /model_manager: dreamer_v2
   - _self_
 
 # Algorithm
 algo:
   total_steps: 5000000
   per_rank_batch_size: 16
-  per_rank_sequence_length: 64
+  per_rank_sequence_length: 50
   cnn_keys:
     encoder: [rgb]
     decoder: [rgb]
 
 # Checkpoint
 checkpoint:
   every: 100000
 
 # Buffer
 buffer:
-  size: 1000000
+  size: 5000000
+  type: sequential
   checkpoint: False
+  prioritize_ends: False
 
 # Distribution
 distribution:
   type: "auto"
 
 metric:
   aggregator:
@@ -48,24 +50,21 @@
         sync_on_compute: ${metric.sync_on_compute}
       Loss/state_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Loss/continue_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      State/kl:
-        _target_: torchmetrics.MeanMetric
-        sync_on_compute: ${metric.sync_on_compute}
       State/post_entropy:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       State/prior_entropy:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      Params/exploration_amount:
+      State/kl:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Grads/world_model:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Grads/actor:
         _target_: torchmetrics.MeanMetric
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   checkpoint: True
 
 # Algorithm
 algo:
   total_steps: 10000000
   per_rank_batch_size: 8
   learning_starts: 65536
-  train_every: 8
+  replay_ratio: 0.125
   cnn_keys:
     encoder:
       - frame
   mlp_keys:
     encoder:
       - own_character
       - own_health
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # Buffer
 buffer:
   checkpoint: True
 
 # Algorithm
 algo:
-  train_every: 16
+  replay_ratio: 0.015625
   learning_starts: 65536
   cnn_keys:
     encoder:
       - rgb
   mlp_keys:
     encoder:
       - life_stats
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # @package _global_
 
 defaults:
   - dreamer_v3
   - override /env: atari
   - _self_
 
-# Experiment
-seed: 5
-
 # Environment
 env:
   num_envs: 1
   max_episode_steps: 27000
   id: MsPacmanNoFrameskip-v4
 
 # Checkpoint
@@ -22,15 +19,15 @@
 buffer:
   size: 16384
   checkpoint: True
 
 # Algorithm
 algo:
   learning_starts: 1024
-  train_every: 16
+  replay_ratio: 0.0625
   dense_units: 8
   mlp_layers: 1
   world_model:
     discrete_size: 4
     stochastic_size: 4
     encoder:
       cnn_channels_multiplier: 2
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -8,37 +8,39 @@
 
 # Experiment
 seed: 5
 
 # Environment
 env:
   num_envs: 4
+  action_repeat: 2
   max_episode_steps: -1
-  id: walker_walk
   wrapper:
+    domain_name: cartpole
+    task_name: swingup_sparse
     from_vectors: False
     from_pixels: True
 
 # Checkpoint
 checkpoint:
   every: 10000
 
 # Buffer
 buffer:
-  size: 100000
+  size: 500_000
   checkpoint: True
   memmap: True
 
 # Algorithm
 algo:
-  total_steps: 1000000
+  total_steps: 500_000
   cnn_keys:
     encoder:
       - rgb
   mlp_keys:
     encoder: []
-  learning_starts: 1024
-  train_every: 2
+  learning_starts: 1300
+  
 
 # Metric
 metric:
   log_every: 5000
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv1_exploration.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv1_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv1_finetuning.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv1_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv2_exploration.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv2_exploration.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -47,20 +47,14 @@
         sync_on_compute: ${metric.sync_on_compute}
       State/post_entropy: 
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       State/prior_entropy: 
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      Params/exploration_amount_task: 
-        _target_: torchmetrics.MeanMetric
-        sync_on_compute: ${metric.sync_on_compute}
-      Params/exploration_amount_exploration: 
-        _target_: torchmetrics.MeanMetric
-        sync_on_compute: ${metric.sync_on_compute}
       Rewards/intrinsic: 
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Values_exploration/predicted_values: 
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Values_exploration/lambda_values:
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv2_finetuning.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_finetuning.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # @package _global_
 
 defaults:
-  - dreamer_v2
-  - override /algo: p2e_dv2
-  - override /model_manager: p2e_dv2_finetuning
+  - dreamer_v3
+  - override /algo: p2e_dv3
+  - override /model_manager: p2e_dv3_finetuning
   - _self_
 
 algo:
-  name: p2e_dv2_finetuning
-  learning_starts: 10000
+  name: p2e_dv3_finetuning
+  learning_starts: 16384
   total_steps: 1000000
   player:
     actor_type: exploration
 
 buffer:
   load_from_exploration: False
 
@@ -21,45 +21,39 @@
 
 metric:
   aggregator:
     metrics:
       Loss/world_model_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      Loss/value_loss:
+      Loss/policy_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      Loss/policy_loss:
+      Loss/value_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Loss/observation_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Loss/reward_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Loss/state_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Loss/continue_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      State/post_entropy:
-        _target_: torchmetrics.MeanMetric
-        sync_on_compute: ${metric.sync_on_compute}
-      State/prior_entropy:
-        _target_: torchmetrics.MeanMetric
-        sync_on_compute: ${metric.sync_on_compute}
       State/kl:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      Params/exploration_amount_task:
+      State/post_entropy:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      Params/exploration_amount_exploration:
+      State/prior_entropy:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Grads/world_model:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Grads/actor:
         _target_: torchmetrics.MeanMetric
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Buffer
 buffer:
   checkpoint: True
 
 # Algorithm
 algo:
   learning_starts: 131072
-  train_every: 1
+  
   dense_units: 768
   mlp_layers: 4
   world_model:
     encoder:
       cnn_channels_multiplier: 48
     recurrent_model:
       recurrent_state_size: 1024
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv3_exploration.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_exploration.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -44,20 +44,14 @@
         sync_on_compute: ${metric.sync_on_compute}
       Loss/ensemble_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       State/kl:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      Params/exploration_amount_task:
-        _target_: torchmetrics.MeanMetric
-        sync_on_compute: ${metric.sync_on_compute}
-      Params/exploration_amount_exploration:
-        _target_: torchmetrics.MeanMetric
-        sync_on_compute: ${metric.sync_on_compute}
       State/post_entropy:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       State/prior_entropy:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Grads/world_model:
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv3_finetuning.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv2_finetuning.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # @package _global_
 
 defaults:
-  - dreamer_v3
-  - override /algo: p2e_dv3
-  - override /model_manager: p2e_dv3_finetuning
+  - dreamer_v2
+  - override /algo: p2e_dv2
+  - override /model_manager: p2e_dv2_finetuning
   - _self_
 
 algo:
-  name: p2e_dv3_finetuning
-  learning_starts: 65536
+  name: p2e_dv2_finetuning
+  learning_starts: 10000
   total_steps: 1000000
   player:
     actor_type: exploration
 
 buffer:
   load_from_exploration: False
 
@@ -21,47 +21,41 @@
 
 metric:
   aggregator:
     metrics:
       Loss/world_model_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      Loss/policy_loss:
+      Loss/value_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      Loss/value_loss:
+      Loss/policy_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Loss/observation_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Loss/reward_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Loss/state_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Loss/continue_loss:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
-      State/kl:
-        _target_: torchmetrics.MeanMetric
-        sync_on_compute: ${metric.sync_on_compute}
-      Params/exploration_amount_task:
-        _target_: torchmetrics.MeanMetric
-        sync_on_compute: ${metric.sync_on_compute}
-      Params/exploration_amount_exploration:
-        _target_: torchmetrics.MeanMetric
-        sync_on_compute: ${metric.sync_on_compute}
       State/post_entropy:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       State/prior_entropy:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
+      State/kl:
+        _target_: torchmetrics.MeanMetric
+        sync_on_compute: ${metric.sync_on_compute}
       Grads/world_model:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Grads/actor:
         _target_: torchmetrics.MeanMetric
         sync_on_compute: ${metric.sync_on_compute}
       Grads/critic:
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   num_envs: 16
   grayscale: True
   frame_stack: 1
   screen_size: 64
   reward_as_observation: True
   wrapper:
     diambra_settings:
-      role: diambra.arena.Roles.P1
+      role: P1
       characters: Lei-Fang
       difficulty: 4
       outfits: 1
     diambra_wrappers:
       no_attack_buttons_combinations: False
 
 # Checkpoint
@@ -33,15 +33,15 @@
 # Buffer
 buffer:
   checkpoint: True
 
 # Algorithm
 algo:
   learning_starts: 65536
-  train_every: 1
+  
   dense_units: 768
   mlp_layers: 4
   world_model:
     encoder:
       cnn_channels_multiplier: 48
     recurrent_model:
       recurrent_state_size: 1024
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/ppo.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/ppo.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/ppo_benchmarks.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/ppo_benchmarks.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,28 @@
   capture_video: False
   num_envs: 1
   sync_env: True
 
 # Algorithm
 algo:
   name: ppo
+  vf_coef: 0.5
+  clip_vloss: False
+  max_grad_norm: 0.5
   rollout_steps: 128
   normalize_advantages: True
-  max_grad_norm: 0.5
   encoder:
     mlp_features_dim: null
   actor:
     mlp_layers: 0
   critic:
     mlp_layers: 0
   optimizer:
-    lr: 1e-3
+    lr: 3e-4
+    eps: 1e-5
   per_rank_batch_size: 64
   # # If you want to run this benchmark with older versions,
   # you need to comment the test function in the `./sheeprl/algos/ppo/ppo.py` file.
   run_test: False
   # If you want to run this benchmark with older versions,
   # you need to move the `total_steps` and the `mlp_keys` config from `algo` to the root.
   total_steps: 65536
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/ppo_super_mario_bros.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/ppo_super_mario_bros.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/sac.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/sac.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/exp/sac_benchmarks.yaml` & `sheeprl-0.5.5/sheeprl/configs/exp/sac_benchmarks.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 # @package _global_
 
 defaults:
+  - default
   - override /algo: sac
   - override /env: gym
   - _self_
 
+run_benchmarks: True
+
 # Environment
 env:
   id: LunarLanderContinuous-v2
   capture_video: False
-  num_envs: 8
+  num_envs: 4
 
 # Algorithm
 algo:
   name: sac
   learning_starts: 100
-  per_rank_gradient_steps: 1
-  per_rank_batch_size: 512
+  
+  per_rank_batch_size: 256
   # # If you want to run this benchmark with older versions,
   # you need to comment the test function in the `./sheeprl/algos/ppo/ppo.py` file.
   run_test: False
   # If you want to run this benchmark with older versions,
   # you need to move the `total_steps` and the `mlp_keys` config from `algo` to the root.
   total_steps: 65536
+  optimier:
+    lr: 3e-4
+    eps: 1e-5
   mlp_keys: 
     encoder: [state]
 
 # Buffer
 buffer:
   checkpoint: True
   sample_next_obs: False
   memmap: False
   size: 65537
 
 fabric:
-  devices: 2
+  devices: 1
   accelerator: cpu
 
 checkpoint:
   every: 70000
   save_last: False
 
 metric:
```

### Comparing `sheeprl-0.5.4/sheeprl/configs/metric/default.yaml` & `sheeprl-0.5.5/sheeprl/configs/metric/default.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/model_manager/dreamer_v2.yaml` & `sheeprl-0.5.5/sheeprl/configs/model_manager/dreamer_v2.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/model_manager/dreamer_v3.yaml` & `sheeprl-0.5.5/sheeprl/configs/model_manager/dreamer_v3.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml` & `sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml` & `sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml` & `sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml` & `sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml` & `sheeprl-0.5.5/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/data/buffers.py` & `sheeprl-0.5.5/sheeprl/data/buffers.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,18 @@
                 with the 'torch.as_tensor' function. Defaults to False.
             kwargs: additional keyword arguments to be passed to the 'self.sample' method.
 
         Returns:
             Dict[str, Tensor]: the sampled dictionary, containing the sampled array,
             one for every key, with a shape of [n_samples, batch_size, ...]
         """
-        samples = self.sample(batch_size=batch_size, sample_next_obs=sample_next_obs, clone=clone, **kwargs)
+        n_samples = kwargs.pop("n_samples", 1)
+        samples = self.sample(
+            batch_size=batch_size, sample_next_obs=sample_next_obs, clone=clone, n_samples=n_samples, **kwargs
+        )
         return {
             k: get_tensor(v, dtype=dtype, clone=clone, device=device, from_numpy=from_numpy) for k, v in samples.items()
         }
 
     def __getitem__(self, key: str) -> np.ndarray | np.memmap | MemmapArray:
         if not isinstance(key, str):
             raise TypeError("'key' must be a string")
@@ -916,29 +919,31 @@
                             "Every array in `data` must be congruent in the first 2 dimensions: "
                             f"found key `{last_key}` with shape `{last_batch_shape}` "
                             f"and `{current_key}` with shape `{current_batch_shape}`"
                         )
                     last_key = current_key
                     last_batch_shape = current_batch_shape
 
-            if "dones" not in data:
-                raise RuntimeError(f"The episode must contain the `dones` key, got: {data.keys()}")
+            if "terminated" not in data and "truncated" not in data:
+                raise RuntimeError(
+                    f"The episode must contain the `terminated` and the `truncated` keys, got: {data.keys()}"
+                )
 
             if env_idxes is not None and (np.array(env_idxes) >= self._n_envs).any():
                 raise ValueError(
                     f"The indices of the environment must be integers in [0, {self._n_envs}), given {env_idxes}"
                 )
 
         # For each environment
         if env_idxes is None:
             env_idxes = range(self._n_envs)
         for i, env in enumerate(env_idxes):
             # Take the data from a single environment
             env_data = {k: v[:, i] for k, v in data.items()}
-            done = env_data["dones"]
+            done = np.logical_or(env_data["terminated"], env_data["truncated"])
             # Take episode ends
             episode_ends = done.nonzero()[0].tolist()
             # If there is not any done, then add the data to the respective open episode
             if len(episode_ends) == 0:
                 self._open_episodes[env].append(env_data)
             else:
                 # In case there is at leas one done, then split the environment data into episodes
@@ -947,37 +952,41 @@
                 # For each episode in the received data
                 for ep_end_idx in episode_ends:
                     stop = ep_end_idx
                     # Take the episode from the data
                     episode = {k: env_data[k][start : stop + 1] for k in env_data.keys()}
                     # If the episode length is greater than zero, then add it to the open episode
                     # of the corresponding environment.
-                    if len(episode["dones"]) > 0:
+                    if len(np.logical_or(episode["terminated"], episode["truncated"])) > 0:
                         self._open_episodes[env].append(episode)
                     start = stop + 1
                     # If the open episode is not empty and the last element is a done, then save the episode
                     # in the buffer and clear the open episode
-                    if len(self._open_episodes[env]) > 0 and self._open_episodes[env][-1]["dones"][-1] == 1:
+                    should_save = len(self._open_episodes[env]) > 0 and np.logical_or(
+                        self._open_episodes[env][-1]["terminated"][-1], self._open_episodes[env][-1]["truncated"][-1]
+                    )
+                    if should_save:
                         self._save_episode(self._open_episodes[env])
                         self._open_episodes[env] = []
 
     def _save_episode(self, episode_chunks: Sequence[Dict[str, np.ndarray | MemmapArray]]) -> None:
         if len(episode_chunks) == 0:
             raise RuntimeError("Invalid episode, an empty sequence is given. You must pass a non-empty sequence.")
         # Concatenate all the chunks of the episode
         episode = {k: [] for k in episode_chunks[0].keys()}
         for chunk in episode_chunks:
             for k in chunk.keys():
                 episode[k].append(chunk[k])
         episode = {k: np.concatenate(v, axis=0) for k, v in episode.items()}
 
         # Control the validity of the episode
-        ep_len = episode["dones"].shape[0]
-        if len(episode["dones"].nonzero()[0]) != 1 or episode["dones"][-1] != 1:
-            raise RuntimeError(f"The episode must contain exactly one done, got: {len(np.nonzero(episode['dones']))}")
+        ends = np.logical_or(episode["terminated"], episode["truncated"])
+        ep_len = ends.shape[0]
+        if len(ends.nonzero()[0]) != 1 or ends[-1] != 1:
+            raise RuntimeError(f"The episode must contain exactly one done, got: {len(np.nonzero(ends))}")
         if ep_len < self._minimum_episode_length:
             raise RuntimeError(
                 f"Episode too short (at least {self._minimum_episode_length} steps), got: {ep_len} steps"
             )
         if ep_len > self._buffer_size:
             raise RuntimeError(f"Episode too long (at most {self._buffer_size} steps), got: {ep_len} steps")
 
@@ -1069,15 +1078,15 @@
             np.intp
         )
         samples_per_eps = {k: [] for k in valid_episodes[0].keys()}
         if sample_next_obs:
             samples_per_eps.update({f"next_{k}": [] for k in self._obs_keys})
         for i, n in enumerate(nsample_per_eps):
             if n > 0:
-                ep_len = valid_episodes[i]["dones"].shape[0]
+                ep_len = np.logical_or(valid_episodes[i]["terminated"], valid_episodes[i]["truncated"]).shape[0]
                 if sample_next_obs:
                     ep_len -= 1
                 # Define the maximum index that can be sampled in the episodes
                 upper = ep_len - sequence_length + 1
                 # If you want to prioritize ends, then all the indices of the episode
                 # can be sampled as starting index
                 if self._prioritize_ends:
```

### Comparing `sheeprl-0.5.4/sheeprl/envs/crafter.py` & `sheeprl-0.5.5/sheeprl/envs/crafter.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         return self._render_mode
 
     def _convert_obs(self, obs: np.ndarray) -> Dict[str, np.ndarray]:
         return {"rgb": obs}
 
     def step(self, action: Any) -> Tuple[Any, SupportsFloat, bool, bool, Dict[str, Any]]:
         obs, reward, done, info = self.env.step(action)
-        return self._convert_obs(obs), reward, done, False, info
+        return self._convert_obs(obs), reward, done and info["discount"] == 0, done and info["discount"] != 0, info
 
     def reset(
         self, *, seed: Optional[int] = None, options: Optional[Dict[str, Any]] = None
     ) -> Tuple[Any, Dict[str, Any]]:
         self.env._seed = seed
         obs = self.env.reset()
         return self._convert_obs(obs), {}
```

### Comparing `sheeprl-0.5.4/sheeprl/envs/diambra.py` & `sheeprl-0.5.5/sheeprl/envs/diambra.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from gymnasium.core import RenderFrame
 
 
 class DiambraWrapper(gym.Wrapper):
     def __init__(
         self,
         id: str,
-        action_space: str = "diambra.arena.SpaceTypes.DISCRETE",
+        action_space: str = "DISCRETE",
         screen_size: Union[int, Tuple[int, int]] = 64,
         grayscale: bool = False,
         repeat_action: int = 1,
         rank: int = 0,
         diambra_settings: Dict[str, Any] = {},
         diambra_wrappers: Dict[str, Any] = {},
         render_mode: str = "rgb_array",
@@ -39,24 +39,31 @@
 
         if diambra_settings.pop("frame_shape", None) is not None:
             warnings.warn("The DIAMBRA frame_shape setting is disabled")
         if diambra_settings.pop("n_players", None) is not None:
             warnings.warn("The DIAMBRA n_players setting is disabled")
 
         role = diambra_settings.pop("role", None)
-        self._action_type = "discrete" if "diambra.arena.SpaceTypes.DISCRETE" == action_space else "multi-discrete"
+        if action_space not in {"DISCRETE", "MULTI_DISCRETE"}:
+            raise ValueError(
+                "The valid values for the `action_space` attribute are "
+                f"'DISCRETE' or 'MULTI_DISCRETE', got {action_space}"
+            )
+        if role is not None and role not in {"P1", "P2"}:
+            raise ValueError(f"The valid values for the `role` attribute are 'P1' or 'P2' or None, got {role}")
+        self._action_type = action_space.lower()
         settings = EnvironmentSettings(
-            **diambra_settings,
             **{
+                **diambra_settings,
                 "game_id": id,
-                "action_space": eval(action_space),
+                "action_space": getattr(diambra.arena.SpaceTypes, action_space, diambra.arena.SpaceTypes.DISCRETE),
                 "n_players": 1,
-                "role": eval(role) if role is not None else None,
+                "role": getattr(diambra.arena.Roles, role, diambra.arena.Roles.P1) if role is not None else None,
                 "render_mode": render_mode,
-            },
+            }
         )
         if repeat_action > 1:
             if "step_ratio" not in settings or settings["step_ratio"] > 1:
                 warnings.warn(
                     f"step_ratio parameter modified to 1 because the sticky action is active ({repeat_action})"
                 )
             settings["step_ratio"] = 1
@@ -65,19 +72,19 @@
         if diambra_wrappers.pop("stack_frames", None) is not None:
             warnings.warn("The DIAMBRA stack_frames wrapper is disabled")
         if diambra_wrappers.pop("dilation", None) is not None:
             warnings.warn("The DIAMBRA dilation wrapper is disabled")
         if diambra_wrappers.pop("flatten", None) is not None:
             warnings.warn("The DIAMBRA flatten wrapper is disabled")
         wrappers = WrappersSettings(
-            **diambra_wrappers,
             **{
+                **diambra_wrappers,
                 "flatten": True,
                 "repeat_action": repeat_action,
-            },
+            }
         )
         if increase_performance:
             settings.frame_shape = screen_size + (int(grayscale),)
         else:
             wrappers.frame_shape = screen_size + (int(grayscale),)
         env = diambra.arena.make(id, settings, wrappers, rank=rank, render_mode=render_mode, log_level=log_level)
         super().__init__(env)
@@ -119,17 +126,17 @@
             for k, v in obs.items()
         }
 
     def step(self, action: Any) -> Tuple[Any, SupportsFloat, bool, bool, Dict[str, Any]]:
         if self._action_type == "discrete" and isinstance(action, np.ndarray):
             action = action.squeeze()
             action = action.item()
-        obs, reward, done, truncated, infos = self.env.step(action)
+        obs, reward, terminated, truncated, infos = self.env.step(action)
         infos["env_domain"] = "DIAMBRA"
-        return self._convert_obs(obs), reward, done or infos.get("env_done", False), truncated, infos
+        return self._convert_obs(obs), reward, terminated or infos.get("env_done", False), truncated, infos
 
     def render(self, mode: str = "rgb_array", **kwargs) -> Optional[Union[RenderFrame, List[RenderFrame]]]:
         return self.env.render()
 
     def reset(
         self, *, seed: Optional[int] = None, options: Optional[Dict[str, Any]] = None
     ) -> Tuple[Any, Dict[str, Any]]:
```

### Comparing `sheeprl-0.5.4/sheeprl/envs/dmc.py` & `sheeprl-0.5.5/sheeprl/envs/dmc.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         obs_pieces.append(flat)
     return np.concatenate(obs_pieces, axis=0)
 
 
 class DMCWrapper(gym.Wrapper):
     def __init__(
         self,
-        id: str,
+        domain_name: str,
+        task_name: str,
         from_pixels: bool = False,
         from_vectors: bool = True,
         height: int = 84,
         width: int = 84,
         camera_id: int = 0,
         task_kwargs: Optional[Dict[Any, Any]] = None,
         environment_kwargs: Optional[Dict[Any, Any]] = None,
@@ -70,15 +71,16 @@
         image and vector observation respectively
         * If only `from_vectors` is True, then the observation will be a single numpy array
         containing the concatenation of all the vector observations defined by the task
         * If only `from_pixels` is True, then the observation will be the image rendered
         by the camera specified through the `camera_id` parameter
 
         Args:
-            id (str): the task id, e.g. 'walker_walk'. The id must be 'underscore' separated.
+            domain_name (str): the domain of the environment, e.g., "walker".
+            task_name (str): the task of the environment, e.g., "walk".
             from_pixels (bool, optional): whether to return the image observation.
                 If both 'from_pixels' and 'from_vectors' are True, then the observation space
                 will be a `gymnasium.spaces.Dict` with two keys: 'rgb' and 'state' for the
                 image and vector observation respectively.
                 Defaults to False.
             from_vectors (bool, optional): whether to return the vector observation. This will
                 be a flattened observation made up by the concatenation of the multiple
@@ -108,15 +110,14 @@
         """
         if not (from_vectors or from_pixels):
             raise ValueError(
                 "'from_vectors' and 'from_pixels' must not be both False: "
                 f"got {from_vectors} and {from_pixels} respectively."
             )
 
-        domain_name, task_name = id.split("_")
         self._from_pixels = from_pixels
         self._from_vectors = from_vectors
         self._height = height
         self._width = width
         self._camera_id = camera_id
         self._channels_first = channels_first
 
@@ -215,21 +216,22 @@
 
     def step(
         self, action: Any
     ) -> Tuple[Union[Dict[str, np.ndarray], np.ndarray], SupportsFloat, bool, bool, Dict[str, Any]]:
         action = self._convert_action(action)
         time_step = self.env.step(action)
         reward = time_step.reward or 0.0
-        done = time_step.last()
         obs = self._get_obs(time_step)
         self.current_state = _flatten_obs(time_step.observation)
         extra = {}
         extra["discount"] = time_step.discount
         extra["internal_state"] = self.env.physics.get_state().copy()
-        return obs, reward, done, False, extra
+        truncated = time_step.last() and time_step.discount == 1
+        terminated = False if time_step.first() else time_step.last() and time_step.discount == 0
+        return obs, reward, terminated, truncated, extra
 
     def reset(
         self, seed: Optional[int] = None, options: Optional[Dict[str, Any]] = None
     ) -> Tuple[Union[Dict[str, np.ndarray], np.ndarray], Dict[str, Any]]:
         if not isinstance(seed, np.random.RandomState):
             seed = np.random.RandomState(seed)
         self.env.task._random = seed
```

### Comparing `sheeprl-0.5.4/sheeprl/envs/minedojo.py` & `sheeprl-0.5.5/sheeprl/envs/minedojo.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,29 +65,28 @@
     ):
         self._height = height
         self._width = width
         self._pitch_limits = pitch_limits
         self._pos = kwargs.get("start_position", None)
         self._break_speed_multiplier = kwargs.get("break_speed_multiplier", 100)
         self._start_pos = copy.deepcopy(self._pos)
-        self._sticky_attack = sticky_attack
+        self._sticky_attack = 0 if self._break_speed_multiplier > 1 else sticky_attack
         self._sticky_jump = sticky_jump
         self._sticky_attack_counter = 0
         self._sticky_jump_counter = 0
 
         if self._pos is not None and not (self._pitch_limits[0] <= self._pos["pitch"] <= self._pitch_limits[1]):
             raise ValueError(
                 f"The initial position must respect the pitch limits {self._pitch_limits}, given {self._pos['pitch']}"
             )
 
         env: ARNNWrapper = minedojo.make(
             task_id=id,
             image_size=(height, width),
             world_seed=seed,
-            generate_world_type="default",
             fast_reset=True,
             **kwargs,
         )
         super().__init__(env)
         self._inventory = {}
         self._inventory_names = None
         self._inventory_max = np.zeros(N_ALL_ITEMS)
@@ -241,32 +240,37 @@
         a = action
         action = self._convert_action(action)
         next_pitch = self._pos["pitch"] + (action[3] - 12) * 15
         if not (self._pitch_limits[0] <= next_pitch <= self._pitch_limits[1]):
             action[3] = 12
 
         obs, reward, done, info = self.env.step(action)
+        is_timelimit = info.get("TimeLimit.truncated", False)
+        terminated = done and not is_timelimit
+        truncated = done and is_timelimit
         self._pos = {
             "x": float(obs["location_stats"]["pos"][0]),
             "y": float(obs["location_stats"]["pos"][1]),
             "z": float(obs["location_stats"]["pos"][2]),
             "pitch": float(obs["location_stats"]["pitch"].item()),
             "yaw": float(obs["location_stats"]["yaw"].item()),
         }
-        info = {
-            "life_stats": {
-                "life": float(obs["life_stats"]["life"].item()),
-                "oxygen": float(obs["life_stats"]["oxygen"].item()),
-                "food": float(obs["life_stats"]["food"].item()),
-            },
-            "location_stats": copy.deepcopy(self._pos),
-            "action": a.tolist(),
-            "biomeid": float(obs["location_stats"]["biome_id"].item()),
-        }
-        return self._convert_obs(obs), reward, done, False, info
+        info.update(
+            {
+                "life_stats": {
+                    "life": float(obs["life_stats"]["life"].item()),
+                    "oxygen": float(obs["life_stats"]["oxygen"].item()),
+                    "food": float(obs["life_stats"]["food"].item()),
+                },
+                "location_stats": copy.deepcopy(self._pos),
+                "action": a.tolist(),
+                "biomeid": float(obs["location_stats"]["biome_id"].item()),
+            }
+        )
+        return self._convert_obs(obs), reward, terminated, truncated, info
 
     def reset(
         self, seed: Optional[int] = None, options: Optional[Dict[str, Any]] = None
     ) -> Tuple[np.ndarray, Dict[str, Any]]:
         obs = self.env.reset()
         self._pos = {
             "x": float(obs["location_stats"]["pos"][0]),
```

### Comparing `sheeprl-0.5.4/sheeprl/envs/minerl.py` & `sheeprl-0.5.5/sheeprl/envs/minerl.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         break_speed_multiplier: Optional[int] = 100,
         multihot_inventory: bool = True,
         **kwargs: Optional[Dict[Any, Any]],
     ):
         self._height = height
         self._width = width
         self._pitch_limits = pitch_limits
-        self._sticky_attack = sticky_attack
+        self._sticky_attack = 0 if break_speed_multiplier > 1 else sticky_attack
         self._sticky_jump = sticky_jump
         self._sticky_attack_counter = 0
         self._sticky_jump_counter = 0
         self._break_speed_multiplier = break_speed_multiplier
         self._multihot_inventory = multihot_inventory
         if "navigate" not in id.lower():
             kwargs.pop("extreme", None)
@@ -299,15 +299,14 @@
             next_pitch = self._pos["pitch"]
 
         obs, reward, done, info = self.env.step(converted_actions)
         self._pos = {
             "pitch": next_pitch,
             "yaw": next_yaw,
         }
-        info = {}
         return self._convert_obs(obs), reward, done, False, info
 
     def reset(
         self, seed: Optional[int] = None, options: Optional[Dict[str, Any]] = None
     ) -> Tuple[np.ndarray, Dict[str, Any]]:
         obs = self.env.reset()
         self._max_inventory = np.zeros(self.inventory_size)
```

### Comparing `sheeprl-0.5.4/sheeprl/envs/minerl_envs/backend.py` & `sheeprl-0.5.5/sheeprl/envs/minerl_envs/backend.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/envs/minerl_envs/navigate.py` & `sheeprl-0.5.5/sheeprl/envs/minerl_envs/navigate.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 if not _IS_MINERL_0_4_4_AVAILABLE:
     raise ModuleNotFoundError(_IS_MINERL_0_4_4_AVAILABLE)
 
 from typing import List
 
 import minerl.herobraine.hero.handlers as handlers
 from minerl.herobraine.hero.handler import Handler
-from minerl.herobraine.hero.mc import MS_PER_STEP
 
 from sheeprl.envs.minerl_envs.backend import CustomSimpleEmbodimentEnvSpec
 
 NAVIGATE_STEPS = 6000
 
 
 class CustomNavigate(CustomSimpleEmbodimentEnvSpec):
     def __init__(self, dense, extreme, *args, **kwargs):
         suffix = "Extreme" if extreme else ""
         suffix += "Dense" if dense else ""
         name = "CustomMineRLNavigate{}-v0".format(suffix)
         self.dense, self.extreme = dense, extreme
-        super().__init__(name, *args, max_episode_steps=6000, **kwargs)
+
+        # The time limit is handled outside because MineRL does not provide a way
+        # to distinguish between terminated and truncated
+        kwargs.pop("max_episode_steps", None)
+        super().__init__(name, *args, max_episode_steps=None, **kwargs)
 
     def is_from_folder(self, folder: str) -> bool:
         return folder == "navigateextreme" if self.extreme else folder == "navigate"
 
     def create_observables(self) -> List[Handler]:
         return super().create_observables() + [
             handlers.CompassObservation(angle=True, distance=False),
@@ -56,15 +59,15 @@
     def create_server_world_generators(self) -> List[Handler]:
         if self.extreme:
             return [handlers.BiomeGenerator(biome=3, force_reset=True)]
         else:
             return [handlers.DefaultWorldGenerator(force_reset=True)]
 
     def create_server_quit_producers(self) -> List[Handler]:
-        return [handlers.ServerQuitFromTimeUp(NAVIGATE_STEPS * MS_PER_STEP), handlers.ServerQuitWhenAnyAgentFinishes()]
+        return [handlers.ServerQuitWhenAnyAgentFinishes()]
 
     def create_server_decorators(self) -> List[Handler]:
         return [
             handlers.NavigationDecorator(
                 max_randomized_radius=64,
                 min_randomized_radius=64,
                 block="diamond_block",
```

### Comparing `sheeprl-0.5.4/sheeprl/envs/minerl_envs/obtain.py` & `sheeprl-0.5.5/sheeprl/envs/minerl_envs/obtain.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 if not _IS_MINERL_0_4_4_AVAILABLE:
     raise ModuleNotFoundError(_IS_MINERL_0_4_4_AVAILABLE)
 
 from typing import Dict, List, Union
 
 from minerl.herobraine.hero import handlers
 from minerl.herobraine.hero.handler import Handler
-from minerl.herobraine.hero.mc import MS_PER_STEP
 
 from sheeprl.envs.minerl_envs.backend import CustomSimpleEmbodimentEnvSpec
 
 none = "none"
 other = "other"
 
 
@@ -24,15 +23,15 @@
 class CustomObtain(CustomSimpleEmbodimentEnvSpec):
     def __init__(
         self,
         target_item,
         dense,
         reward_schedule: List[Dict[str, Union[str, int, float]]],
         *args,
-        max_episode_steps=6000,
+        max_episode_steps=None,
         **kwargs,
     ):
         # 6000 for obtain iron  (5 mins)
         # 18000 for obtain diamond (15 mins)
         self.target_item = target_item
         self.dense = dense
         suffix = snake_to_camel(self.target_item)
@@ -134,18 +133,15 @@
     def create_agent_handlers(self) -> List[Handler]:
         return [handlers.AgentQuitFromPossessingItem([dict(type="diamond", amount=1)])]
 
     def create_server_world_generators(self) -> List[Handler]:
         return [handlers.DefaultWorldGenerator(force_reset=True)]
 
     def create_server_quit_producers(self) -> List[Handler]:
-        return [
-            handlers.ServerQuitFromTimeUp(time_limit_ms=self.max_episode_steps * MS_PER_STEP),
-            handlers.ServerQuitWhenAnyAgentFinishes(),
-        ]
+        return [handlers.ServerQuitWhenAnyAgentFinishes()]
 
     def create_server_decorators(self) -> List[Handler]:
         return []
 
     def create_server_initial_conditions(self) -> List[Handler]:
         return [
             handlers.TimeInitialCondition(
@@ -171,14 +167,17 @@
         reward_values = [s["reward"] for s in self.reward_schedule]
 
         return len(rewards.intersection(reward_values)) >= len(reward_values) - max_missing
 
 
 class CustomObtainDiamond(CustomObtain):
     def __init__(self, dense, *args, **kwargs):
+        # The time limit is handled outside because MineRL does not provide a way
+        # to distinguish between terminated and truncated
+        kwargs.pop("max_episode_steps", None)
         super(CustomObtainDiamond, self).__init__(
             *args,
             target_item="diamond",
             dense=dense,
             reward_schedule=[
                 dict(type="log", amount=1, reward=1),
                 dict(type="planks", amount=1, reward=2),
@@ -189,15 +188,15 @@
                 dict(type="furnace", amount=1, reward=32),
                 dict(type="stone_pickaxe", amount=1, reward=32),
                 dict(type="iron_ore", amount=1, reward=64),
                 dict(type="iron_ingot", amount=1, reward=128),
                 dict(type="iron_pickaxe", amount=1, reward=256),
                 dict(type="diamond", amount=1, reward=1024),
             ],
-            max_episode_steps=18000,
+            max_episode_steps=None,
             **kwargs,
         )
 
     def is_from_folder(self, folder: str) -> bool:
         return folder == "o_dia"
 
     def get_docstring(self):
@@ -247,14 +246,17 @@
 
 \n"""
         )
 
 
 class CustomObtainIronPickaxe(CustomObtain):
     def __init__(self, dense, *args, **kwargs):
+        # The time limit is handled outside because MineRL does not provide a way
+        # to distinguish between terminated and truncated
+        kwargs.pop("max_episode_steps", None)
         super(CustomObtainIronPickaxe, self).__init__(
             *args,
             target_item="iron_pickaxe",
             dense=dense,
             reward_schedule=[
                 dict(type="log", amount=1, reward=1),
                 dict(type="planks", amount=1, reward=2),
@@ -264,14 +266,15 @@
                 dict(type="cobblestone", amount=1, reward=16),
                 dict(type="furnace", amount=1, reward=32),
                 dict(type="stone_pickaxe", amount=1, reward=32),
                 dict(type="iron_ore", amount=1, reward=64),
                 dict(type="iron_ingot", amount=1, reward=128),
                 dict(type="iron_pickaxe", amount=1, reward=256),
             ],
+            max_episode_steps=None,
             **kwargs,
         )
 
     def create_agent_handlers(self):
         return [handlers.AgentQuitFromCraftingItem([dict(type="iron_pickaxe", amount=1)])]
 
     def is_from_folder(self, folder: str) -> bool:
```

### Comparing `sheeprl-0.5.4/sheeprl/envs/super_mario_bros.py` & `sheeprl-0.5.5/sheeprl/envs/super_mario_bros.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         self._render_mode = render_mode
 
     def step(self, action: np.ndarray | int) -> Tuple[Any, SupportsFloat, bool, bool, Dict[str, Any]]:
         if isinstance(action, np.ndarray):
             action = action.squeeze().item()
         obs, reward, done, info = self.env.step(action)
         converted_obs = {"rgb": obs.copy()}
-        return converted_obs, reward, done, False, info
+        is_timelimit = info.get("time", False)
+        return converted_obs, reward, done and not is_timelimit, done and is_timelimit, info
 
     def render(self) -> RenderFrame | list[RenderFrame] | None:
         rendered_frame: np.ndarray | None = self.env.render(mode=self.render_mode)
         if self.render_mode == "rgb_array" and rendered_frame is not None:
             return rendered_frame.copy()
         return
```

### Comparing `sheeprl-0.5.4/sheeprl/envs/wrappers.py` & `sheeprl-0.5.5/sheeprl/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/models/models.py` & `sheeprl-0.5.5/sheeprl/models/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Adapted from: https://github.com/thu-ml/tianshou/blob/master/tianshou/utils/net/common.py
 """
+
 import warnings
 from math import prod
-from typing import Dict, Optional, Sequence, Union, no_type_check
+from typing import Any, Callable, Dict, Optional, Sequence, Union, no_type_check
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn
 
 from sheeprl.utils.model import ArgsType, ModuleType, cnn_forward, create_layers, miniblock
 
@@ -337,31 +338,38 @@
     Args:
         input_size (int): the input size.
         hidden_size (int): the hidden state size
         bias (bool, optional): whether to apply a bias to the input projection.
             Defaults to True.
         batch_first (bool, optional): whether the first dimension represent the batch dimension or not.
             Defaults to False.
-        layer_norm (bool, optional): whether to apply a LayerNorm after the input projection.
-            Defaults to False.
+        layer_norm_cls (Callable[..., nn.Module]): the layer norm to apply after the input projection.
+            Defaults to nn.Identiy.
+        layer_norm_kw (Dict[str, Any]): the kwargs of the layer norm.
+            Default to {}.
     """
 
     def __init__(
-        self, input_size: int, hidden_size: int, bias: bool = True, batch_first: bool = False, layer_norm: bool = False
+        self,
+        input_size: int,
+        hidden_size: int,
+        bias: bool = True,
+        batch_first: bool = False,
+        layer_norm_cls: Callable[..., nn.Module] = nn.Identity,
+        layer_norm_kw: Dict[str, Any] = {},
     ) -> None:
         super().__init__()
         self.input_size = input_size
         self.hidden_size = hidden_size
         self.bias = bias
         self.batch_first = batch_first
         self.linear = nn.Linear(input_size + hidden_size, 3 * hidden_size, bias=self.bias)
-        if layer_norm:
-            self.layer_norm = torch.nn.LayerNorm(3 * hidden_size)
-        else:
-            self.layer_norm = nn.Identity()
+        # Avoid multiple values for the `normalized_shape` argument
+        layer_norm_kw.pop("normalized_shape", None)
+        self.layer_norm = layer_norm_cls(3 * hidden_size, **layer_norm_kw)
 
     def forward(self, input: Tensor, hx: Optional[Tensor] = None) -> Tensor:
         is_3d = input.dim() == 3
         if is_3d:
             if input.shape[int(self.batch_first)] == 1:
                 input = input.squeeze(int(self.batch_first))
             else:
@@ -490,7 +498,28 @@
     def forward(self, x: Tensor) -> Dict[str, Tensor]:
         reconstructed_obs = {}
         if self.cnn_decoder is not None:
             reconstructed_obs.update(self.cnn_decoder(x))
         if self.mlp_decoder is not None:
             reconstructed_obs.update(self.mlp_decoder(x))
         return reconstructed_obs
+
+
+class LayerNormChannelLast(nn.LayerNorm):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    def forward(self, x: Tensor) -> Tensor:
+        if x.dim() != 4:
+            raise ValueError(f"Input tensor must be 4D (NCHW), received {len(x.shape)}D instead: {x.shape}")
+        input_dtype = x.dtype
+        x = x.permute(0, 2, 3, 1)
+        x = super().forward(x)
+        x = x.permute(0, 3, 1, 2)
+        return x.to(input_dtype)
+
+
+class LayerNorm(nn.LayerNorm):
+    def forward(self, x: Tensor) -> Tensor:
+        input_dtype = x.dtype
+        out = super().forward(x)
+        return out.to(input_dtype)
```

### Comparing `sheeprl-0.5.4/sheeprl/optim/rmsprop_tf.py` & `sheeprl-0.5.5/sheeprl/optim/rmsprop_tf.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/utils/callback.py` & `sheeprl-0.5.5/sheeprl/utils/callback.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,21 +57,24 @@
 
     def on_checkpoint_player(
         self,
         fabric: Fabric,
         player_trainer_collective: TorchCollective,
         ckpt_path: str,
         replay_buffer: Optional["ReplayBuffer"] = None,
+        ratio_state_dict: Dict[str, Any] | None = None,
     ):
         state = [None]
         player_trainer_collective.broadcast_object_list(state, src=1)
         state = state[0]
         if replay_buffer is not None:
             rb_state = self._ckpt_rb(replay_buffer)
             state["rb"] = replay_buffer
+        if ratio_state_dict is not None:
+            state["ratio"] = ratio_state_dict
         fabric.save(ckpt_path, state)
         if replay_buffer is not None:
             self._experiment_consistent_rb(replay_buffer, rb_state)
         if fabric.is_global_zero and self.keep_last:
             self._delete_old_checkpoints(pathlib.Path(ckpt_path).parent)
 
     def on_checkpoint_trainer(
@@ -98,22 +101,22 @@
             rb (ReplayBuffer | EnvIndependentReplayBuffer | EpisodeBuffer): the buffer.
 
         Returns:
             The original state of the buffer.
         """
         if isinstance(rb, ReplayBuffer):
             # clone the true done
-            state = rb["dones"][(rb._pos - 1) % rb.buffer_size, :].copy()
+            state = rb["truncated"][(rb._pos - 1) % rb.buffer_size, :].copy()
             # substitute the last done with all True values (all the environment are truncated)
-            rb["dones"][(rb._pos - 1) % rb.buffer_size, :] = True
+            rb["truncated"][(rb._pos - 1) % rb.buffer_size, :] = 1
         elif isinstance(rb, EnvIndependentReplayBuffer):
             state = []
             for b in rb.buffer:
-                state.append(b["dones"][(b._pos - 1) % b.buffer_size, :].copy())
-                b["dones"][(b._pos - 1) % b.buffer_size, :] = True
+                state.append(b["truncated"][(b._pos - 1) % b.buffer_size, :].copy())
+                b["truncated"][(b._pos - 1) % b.buffer_size, :] = 1
         elif isinstance(rb, EpisodeBuffer):
             # remove open episodes from the buffer because the state of the environment is not saved
             state = rb._open_episodes
             rb._open_episodes = [[] for _ in range(rb.n_envs)]
         return state
 
     def _experiment_consistent_rb(
@@ -126,18 +129,18 @@
 
         Args:
             rb (ReplayBuffer | EnvIndependentReplayBuffer | EpisodeBuffer): the buffer.
             state (Tensor | Sequence[Tensor] | Sequence[Sequence[Tensor]]): the original state of the buffer.
         """
         if isinstance(rb, ReplayBuffer):
             # reinsert the true dones in the buffer
-            rb["dones"][(rb._pos - 1) % rb.buffer_size, :] = state
+            rb["truncated"][(rb._pos - 1) % rb.buffer_size, :] = state
         elif isinstance(rb, EnvIndependentReplayBuffer):
             for i, b in enumerate(rb.buffer):
-                b["dones"][(b._pos - 1) % b.buffer_size, :] = state[i]
+                b["truncated"][(b._pos - 1) % b.buffer_size, :] = state[i]
         elif isinstance(rb, EpisodeBuffer):
             # reinsert the open episodes to continue the training
             rb._open_episodes = state
 
     def _delete_old_checkpoints(self, ckpt_folder: pathlib.Path):
         ckpts = list(sorted(ckpt_folder.glob("*.ckpt"), key=os.path.getmtime))
         if len(ckpts) > self.keep_last:
```

### Comparing `sheeprl-0.5.4/sheeprl/utils/distribution.py` & `sheeprl-0.5.5/sheeprl/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/utils/env.py` & `sheeprl-0.5.5/sheeprl/utils/env.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/utils/imports.py` & `sheeprl-0.5.5/sheeprl/utils/imports.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/utils/logger.py` & `sheeprl-0.5.5/sheeprl/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/utils/memmap.py` & `sheeprl-0.5.5/sheeprl/utils/memmap.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/utils/metric.py` & `sheeprl-0.5.5/sheeprl/utils/metric.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/utils/mlflow.py` & `sheeprl-0.5.5/sheeprl/utils/mlflow.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/utils/model.py` & `sheeprl-0.5.5/sheeprl/utils/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Adapted from: https://github.com/thu-ml/tianshou/blob/master/tianshou/utils/net/common.py
 """
+
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import torch
 from torch import Tensor, nn
 
 ModuleType = Optional[Type[nn.Module]]
 ArgType = Union[Tuple[Any, ...], Dict[Any, Any], None]
@@ -216,20 +217,7 @@
         >>> cnn_forward(decoder, input, (230,), (3, 64, 64)).shape
         torch.Size([10, 20, 3, 64, 64])
     """
     batch_shapes = input.shape[: -len(input_dim)]
     flatten_input = input.reshape(-1, *input_dim)
     model_out = model(flatten_input)
     return model_out.reshape(*batch_shapes, *output_dim)
-
-
-class LayerNormChannelLast(nn.LayerNorm):
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-    def forward(self, x: Tensor) -> Tensor:
-        if x.dim() != 4:
-            raise ValueError(f"Input tensor must be 4D (NCHW), received {len(x.shape)}D instead: {x.shape}")
-        x = x.permute(0, 2, 3, 1)
-        x = super().forward(x)
-        x = x.permute(0, 3, 1, 2)
-        return x
```

### Comparing `sheeprl-0.5.4/sheeprl/utils/registry.py` & `sheeprl-0.5.5/sheeprl/utils/registry.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl/utils/timer.py` & `sheeprl-0.5.5/sheeprl/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.4/sheeprl.egg-info/PKG-INFO` & `sheeprl-0.5.5/sheeprl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheeprl
-Version: 0.5.4
+Version: 0.5.5
 Summary: High-quality, single file and distributed implementation of Deep Reinforcement Learning algorithms with production-friendly features
 Author-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 Maintainer-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -207,33 +207,34 @@
            limitations under the License.
         
 Project-URL: homepage, https://eclecticsheep.ai
 Project-URL: repository, https://github.com/Eclectic-Sheep/sheeprl
 Keywords: reinforcement,machine,learning,distributed,production
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gymnasium==0.29.*
 Requires-Dist: pygame>=2.1.3
 Requires-Dist: moviepy>=1.0.3
 Requires-Dist: tensorboard>=2.10
 Requires-Dist: python-dotenv>=1.0.0
-Requires-Dist: lightning==2.1.*
+Requires-Dist: lightning>=2.0
 Requires-Dist: lightning-utilities<=0.9
 Requires-Dist: hydra-core==1.3.0
 Requires-Dist: torchmetrics
 Requires-Dist: rich==13.5.*
 Requires-Dist: opencv-python==4.8.0.*
 Requires-Dist: torch!=2.2.0,>=2.0
 Provides-Extra: test
 Requires-Dist: pytest==7.3.1; extra == "test"
 Requires-Dist: pytest-timeout==2.1.0; extra == "test"
 Requires-Dist: pytest-coverage; extra == "test"
+Requires-Dist: importlib_resources>=6.2.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: mypy==1.2.0; extra == "dev"
 Requires-Dist: black==23.12.1; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
 Requires-Dist: autoflake==2.2.1; extra == "dev"
 Requires-Dist: ruff==0.1.11; extra == "dev"
@@ -247,24 +248,26 @@
 Provides-Extra: atari
 Requires-Dist: gymnasium[atari]==0.29.*; extra == "atari"
 Requires-Dist: gymnasium[accept-rom-license]==0.29.*; extra == "atari"
 Requires-Dist: gymnasium[other]==0.29.*; extra == "atari"
 Provides-Extra: minedojo
 Requires-Dist: minedojo==0.1; extra == "minedojo"
 Requires-Dist: importlib_resources==5.12.0; extra == "minedojo"
+Requires-Dist: gym==0.21.0; extra == "minedojo"
 Provides-Extra: minerl
 Requires-Dist: setuptools==66.0.0; extra == "minerl"
 Requires-Dist: minerl==0.4.4; extra == "minerl"
+Requires-Dist: gym==0.19.0; extra == "minerl"
 Provides-Extra: diambra
-Requires-Dist: diambra==0.0.16; extra == "diambra"
-Requires-Dist: diambra-arena==2.2.2; extra == "diambra"
+Requires-Dist: diambra==0.0.17; extra == "diambra"
+Requires-Dist: diambra-arena==2.2.6; extra == "diambra"
 Provides-Extra: crafter
-Requires-Dist: crafter==1.8.1; extra == "crafter"
+Requires-Dist: crafter==1.8.3; extra == "crafter"
 Provides-Extra: mlflow
-Requires-Dist: mlflow==2.8.0; extra == "mlflow"
+Requires-Dist: mlflow==2.11.1; extra == "mlflow"
 Provides-Extra: supermario
 Requires-Dist: gym-super-mario-bros==7.4.0; extra == "supermario"
 Requires-Dist: gym<0.26; extra == "supermario"
 
 # ⚡ SheepRL 🐑
 
 <p id="logo" align="center" style="width: 50%; margin: auto;">
```

### Comparing `sheeprl-0.5.4/sheeprl.egg-info/SOURCES.txt` & `sheeprl-0.5.5/sheeprl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -121,17 +121,20 @@
 sheeprl/configs/env/diambra.yaml
 sheeprl/configs/env/dmc.yaml
 sheeprl/configs/env/dummy.yaml
 sheeprl/configs/env/gym.yaml
 sheeprl/configs/env/minecraft.yaml
 sheeprl/configs/env/minedojo.yaml
 sheeprl/configs/env/minerl.yaml
+sheeprl/configs/env/minerl_obtain_diamond.yaml
+sheeprl/configs/env/minerl_obtain_iron_pickaxe.yaml
 sheeprl/configs/env/mujoco.yaml
 sheeprl/configs/env/super_mario_bros.yaml
 sheeprl/configs/exp/a2c.yaml
+sheeprl/configs/exp/a2c_benchmarks.yaml
 sheeprl/configs/exp/default.yaml
 sheeprl/configs/exp/dreamer_v1.yaml
 sheeprl/configs/exp/dreamer_v1_benchmarks.yaml
 sheeprl/configs/exp/dreamer_v2.yaml
 sheeprl/configs/exp/dreamer_v2_benchmarks.yaml
 sheeprl/configs/exp/dreamer_v2_crafter.yaml
 sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml
@@ -139,14 +142,15 @@
 sheeprl/configs/exp/dreamer_v3_100k_boxing.yaml
 sheeprl/configs/exp/dreamer_v3_100k_ms_pacman.yaml
 sheeprl/configs/exp/dreamer_v3_L_doapp.yaml
 sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml
 sheeprl/configs/exp/dreamer_v3_L_navigate.yaml
 sheeprl/configs/exp/dreamer_v3_XL_crafter.yaml
 sheeprl/configs/exp/dreamer_v3_benchmarks.yaml
+sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml
 sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml
 sheeprl/configs/exp/dreamer_v3_super_mario_bros.yaml
 sheeprl/configs/exp/droq.yaml
 sheeprl/configs/exp/p2e_dv1_exploration.yaml
 sheeprl/configs/exp/p2e_dv1_finetuning.yaml
 sheeprl/configs/exp/p2e_dv2_exploration.yaml
 sheeprl/configs/exp/p2e_dv2_finetuning.yaml
@@ -209,14 +213,15 @@
 sheeprl/models/models.py
 sheeprl/optim/__init__.py
 sheeprl/optim/rmsprop_tf.py
 sheeprl/utils/__init__.py
 sheeprl/utils/callback.py
 sheeprl/utils/distribution.py
 sheeprl/utils/env.py
+sheeprl/utils/fabric.py
 sheeprl/utils/imports.py
 sheeprl/utils/logger.py
 sheeprl/utils/memmap.py
 sheeprl/utils/metric.py
 sheeprl/utils/mlflow.py
 sheeprl/utils/model.py
 sheeprl/utils/registry.py
```

### Comparing `sheeprl-0.5.4/sheeprl.egg-info/requires.txt` & `sheeprl-0.5.5/sheeprl.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 gymnasium==0.29.*
 pygame>=2.1.3
 moviepy>=1.0.3
 tensorboard>=2.10
 python-dotenv>=1.0.0
-lightning==2.1.*
+lightning>=2.0
 lightning-utilities<=0.9
 hydra-core==1.3.0
 torchmetrics
 rich==13.5.*
 opencv-python==4.8.0.*
 torch!=2.2.0,>=2.0
 
@@ -16,47 +16,50 @@
 gymnasium[accept-rom-license]==0.29.*
 gymnasium[other]==0.29.*
 
 [box2d]
 gymnasium[box2d]==0.29.*
 
 [crafter]
-crafter==1.8.1
+crafter==1.8.3
 
 [dev]
 pre-commit==3.5.0
 mypy==1.2.0
 black==23.12.1
 isort==5.13.2
 autoflake==2.2.1
 ruff==0.1.11
 
 [diambra]
-diambra==0.0.16
-diambra-arena==2.2.2
+diambra==0.0.17
+diambra-arena==2.2.6
 
 [dmc]
 dm_control>=1.0.12
 
 [minedojo]
 minedojo==0.1
 importlib_resources==5.12.0
+gym==0.21.0
 
 [minerl]
 setuptools==66.0.0
 minerl==0.4.4
+gym==0.19.0
 
 [mlflow]
-mlflow==2.8.0
+mlflow==2.11.1
 
 [mujoco]
 mujoco>=2.3.3
 gymnasium[mujoco]==0.29.*
 
 [supermario]
 gym-super-mario-bros==7.4.0
 gym<0.26
 
 [test]
 pytest==7.3.1
 pytest-timeout==2.1.0
 pytest-coverage
+importlib_resources>=6.2.0
```


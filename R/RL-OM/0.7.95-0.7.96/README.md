# Comparing `tmp/RL_OM-0.7.95.tar.gz` & `tmp/RL_OM-0.7.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.7.95.tar", last modified: Wed Apr 10 17:31:13 2024, max compression
+gzip compressed data, was "RL_OM-0.7.96.tar", last modified: Fri May  3 07:14:45 2024, max compression
```

## Comparing `RL_OM-0.7.95.tar` & `RL_OM-0.7.96.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.379601 RL_OM-0.7.95/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.7.95/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.7.95/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-04-10 17:31:13.379463 RL_OM-0.7.95/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.7.95/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.370307 RL_OM-0.7.95/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)     1284 2024-03-23 05:21:04.000000 RL_OM-0.7.95/RL_OM/MLtools.py
--rw-r--r--   0 magnus     (501) staff       (20)       23 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)   231218 2024-03-21 02:54:55.000000 RL_OM-0.7.95/RL_OM/_modidx 2.py
--rw-r--r--   0 magnus     (501) staff       (20)   240779 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.371518 RL_OM-0.7.95/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.373358 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     1707 2023-12-01 14:08:43.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/PPO_SB3.py
--rw-r--r--   0 magnus     (501) staff       (20)      468 2023-12-01 14:08:43.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/PPO_TEMP.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6605 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/cbs.py
--rw-r--r--   0 magnus     (501) staff       (20)     6389 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/eoq.py
--rw-r--r--   0 magnus     (501) staff       (20)     8752 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/mp_agents_ERM.py
--rw-r--r--   0 magnus     (501) staff       (20)     2355 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/nv_agents.py
--rw-r--r--   0 magnus     (501) staff       (20)    60659 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/nv_agents_ERM.py
--rw-r--r--   0 magnus     (501) staff       (20)     9918 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/nv_agents_SAA.py
--rw-r--r--   0 magnus     (501) staff       (20)     9350 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py
--rw-r--r--   0 magnus     (501) staff       (20)    23263 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/qr.py
--rw-r--r--   0 magnus     (501) staff       (20)    14565 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/saa.py
--rw-r--r--   0 magnus     (501) staff       (20)    13815 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/benchmark_agents/ss.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.373881 RL_OM-0.7.95/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6890 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1369 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     9657 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.374277 RL_OM-0.7.95/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1162 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/processors/eoq_preprocessors.py
--rw-r--r--   0 magnus     (501) staff       (20)     6401 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.375115 RL_OM-0.7.95/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.375988 RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14243 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13708 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19176 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19614 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19118 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.377810 RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     3234 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)    12009 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py
--rw-r--r--   0 magnus     (501) staff       (20)     4995 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)     5053 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)     5269 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    16656 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)     5082 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
--rw-r--r--   0 magnus     (501) staff       (20)     4875 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.7.95/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.378519 RL_OM-0.7.95/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    16847 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)     6137 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/environments/data_generators.py
--rw-r--r--   0 magnus     (501) staff       (20)     2575 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/environments/feature_converters.py
--rw-r--r--   0 magnus     (501) staff       (20)    43500 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.378811 RL_OM-0.7.95/RL_OM/experiment_functions/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/experiment_functions/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    32862 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/experiment_functions/run_experiment.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.379242 RL_OM-0.7.95/RL_OM/utils/
--rw-r--r--   0 magnus     (501) staff       (20)     1259 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/utils/MLtools.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/utils/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    10828 2024-04-10 17:30:32.000000 RL_OM-0.7.95/RL_OM/utils/utils.py
--rw-r--r--   0 magnus     (501) staff       (20)    10817 2024-03-23 04:58:03.000000 RL_OM-0.7.95/RL_OM/utils.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 17:31:13.371352 RL_OM-0.7.95/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-04-10 17:31:13.000000 RL_OM-0.7.95/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     2613 2024-04-10 17:31:13.000000 RL_OM-0.7.95/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2024-04-10 17:31:13.000000 RL_OM-0.7.95/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2024-04-10 17:31:13.000000 RL_OM-0.7.95/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.7.95/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2024-04-10 17:31:13.000000 RL_OM-0.7.95/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2024-04-10 17:31:13.000000 RL_OM-0.7.95/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      990 2024-04-10 17:31:09.000000 RL_OM-0.7.95/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2024-04-10 17:31:13.379644 RL_OM-0.7.95/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.7.95/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.500750 RL_OM-0.7.96/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.7.96/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.7.96/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-05-03 07:14:45.500608 RL_OM-0.7.96/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.7.96/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.481552 RL_OM-0.7.96/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)     1284 2024-03-23 05:21:04.000000 RL_OM-0.7.96/RL_OM/MLtools.py
+-rw-r--r--   0 magnus     (501) staff       (20)       23 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   231218 2024-03-21 02:54:55.000000 RL_OM-0.7.96/RL_OM/_modidx 2.py
+-rw-r--r--   0 magnus     (501) staff       (20)   241126 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.483206 RL_OM-0.7.96/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.488612 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     1707 2023-12-01 14:08:43.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/PPO_SB3.py
+-rw-r--r--   0 magnus     (501) staff       (20)      468 2023-12-01 14:08:43.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/PPO_TEMP.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6605 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/cbs.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6389 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/eoq.py
+-rw-r--r--   0 magnus     (501) staff       (20)     8752 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/mp_agents_ERM.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2355 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/nv_agents.py
+-rw-r--r--   0 magnus     (501) staff       (20)    60657 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/nv_agents_ERM.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9918 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/nv_agents_SAA.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9350 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py
+-rw-r--r--   0 magnus     (501) staff       (20)    23263 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/qr.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14565 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/saa.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13815 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/benchmark_agents/ss.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.490416 RL_OM-0.7.96/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6890 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1369 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9657 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.491224 RL_OM-0.7.96/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1162 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6523 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.492942 RL_OM-0.7.96/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.494238 RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.497784 RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     3234 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)    12009 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4995 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5053 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5269 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16656 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5082 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4875 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.7.96/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.499022 RL_OM-0.7.96/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    20455 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6137 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2575 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    44045 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.499410 RL_OM-0.7.96/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    32862 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/experiment_functions/run_experiment.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.500144 RL_OM-0.7.96/RL_OM/utils/
+-rw-r--r--   0 magnus     (501) staff       (20)     1259 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/utils/MLtools.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 06:06:15.000000 RL_OM-0.7.96/RL_OM/utils/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10828 2024-05-03 06:06:14.000000 RL_OM-0.7.96/RL_OM/utils/utils.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10817 2024-03-23 04:58:03.000000 RL_OM-0.7.96/RL_OM/utils.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 07:14:45.483059 RL_OM-0.7.96/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-05-03 07:14:45.000000 RL_OM-0.7.96/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     2613 2024-05-03 07:14:45.000000 RL_OM-0.7.96/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2024-05-03 07:14:45.000000 RL_OM-0.7.96/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2024-05-03 07:14:45.000000 RL_OM-0.7.96/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.7.96/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2024-05-03 07:14:45.000000 RL_OM-0.7.96/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2024-05-03 07:14:45.000000 RL_OM-0.7.96/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      990 2024-05-03 07:14:17.000000 RL_OM-0.7.96/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2024-05-03 07:14:45.500796 RL_OM-0.7.96/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.7.96/setup.py
```

### Comparing `RL_OM-0.7.95/LICENSE` & `RL_OM-0.7.96/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/PKG-INFO` & `RL_OM-0.7.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.7.95
+Version: 0.7.96
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.7.95/RL_OM/MLtools.py` & `RL_OM-0.7.96/RL_OM/MLtools.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/_modidx 2.py` & `RL_OM-0.7.96/RL_OM/_modidx 2.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/_modidx.py` & `RL_OM-0.7.96/RL_OM/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1172,15 +1172,17 @@
                                                             'RL_OM.agents.rl_agents.sac_hybrid_separate.SAC_hybrid_separate._post_load': ( 'agents/rl_agents/sac_hybrid_separate.html#sac_hybrid_separate._post_load',
                                                                                                                                            'RL_OM/agents/rl_agents/sac_hybrid_separate.py'),
                                                             'RL_OM.agents.rl_agents.sac_hybrid_separate.SAC_hybrid_separate._update_alpha': ( 'agents/rl_agents/sac_hybrid_separate.html#sac_hybrid_separate._update_alpha',
                                                                                                                                               'RL_OM/agents/rl_agents/sac_hybrid_separate.py'),
                                                             'RL_OM.agents.rl_agents.sac_hybrid_separate.SAC_hybrid_separate.fit': ( 'agents/rl_agents/sac_hybrid_separate.html#sac_hybrid_separate.fit',
                                                                                                                                     'RL_OM/agents/rl_agents/sac_hybrid_separate.py')},
             'RL_OM.core': {'RL_OM.core.foo': ('core.html#foo', 'RL_OM/core.py')},
-            'RL_OM.environments.calculation_functions': { 'RL_OM.environments.calculation_functions.eoq_qr_calculations_qr_action': ( 'environments/calculation_functions.html#eoq_qr_calculations_qr_action',
+            'RL_OM.environments.calculation_functions': { 'RL_OM.environments.calculation_functions.ds_calculations': ( 'environments/calculation_functions.html#ds_calculations',
+                                                                                                                        'RL_OM/environments/calculation_functions.py'),
+                                                          'RL_OM.environments.calculation_functions.eoq_qr_calculations_qr_action': ( 'environments/calculation_functions.html#eoq_qr_calculations_qr_action',
                                                                                                                                       'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.eoq_qr_calculations_single_action': ( 'environments/calculation_functions.html#eoq_qr_calculations_single_action',
                                                                                                                                           'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.get_fixed_ordering_cost': ( 'environments/calculation_functions.html#get_fixed_ordering_cost',
                                                                                                                                 'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.get_orders_arriving_stochastic': ( 'environments/calculation_functions.html#get_orders_arriving_stochastic',
                                                                                                                                        'RL_OM/environments/calculation_functions.py'),
```

### Comparing `RL_OM-0.7.95/RL_OM/agents/benchmark_agents/PPO_SB3.py` & `RL_OM-0.7.96/RL_OM/agents/benchmark_agents/PPO_SB3.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/benchmark_agents/cbs.py` & `RL_OM-0.7.96/RL_OM/agents/benchmark_agents/cbs.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.7.96/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/benchmark_agents/mp_agents_ERM.py` & `RL_OM-0.7.96/RL_OM/agents/benchmark_agents/mp_agents_ERM.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/benchmark_agents/nv_agents.py` & `RL_OM-0.7.96/RL_OM/agents/benchmark_agents/nv_agents.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/benchmark_agents/nv_agents_ERM.py` & `RL_OM-0.7.96/RL_OM/agents/benchmark_agents/nv_agents_ERM.py`

 * *Files 0% similar despite different names*

```diff
@@ -844,15 +844,15 @@
                 # Update cache
                 k = torch.cat([self.kv_cache[0], k], dim=1)[:, 1:]
                 v = torch.cat([self.kv_cache[1], v], dim=1)[:, 1:]
                 self.kv_cache = k, v
             else:
                 # Build cache
                 self.kv_cache = k, v
-
+        
         k = k.view(B, -1, self.n_head, self.n_embd_per_head).transpose(
             1, 2
         )  # (B, nh, T, hs)
         q = q.view(B, -1, self.n_head, self.n_embd_per_head).transpose(
             1, 2
         )  # (B, nh, T, hs)
         v = v.view(B, -1, self.n_head, self.n_embd_per_head).transpose(
@@ -1033,15 +1033,14 @@
         self.y_cache = False  # used at time of inference when kv cached is used
         
         if relu_output:
             self.final_activation = nn.ReLU()  # output is non-negative
         else:
             self.final_activation = nn.Identity()
 
-
         def _init_weights(self, module: nn.Module) -> None:
             if isinstance(module, nn.Linear):
                 torch.nn.init.normal_(
                     module.weight, mean=0.0, std=0.02 / math.sqrt(2 * self.n_layer)
                 )
             elif isinstance(module, nn.Embedding):
                 torch.nn.init.normal_(
@@ -1110,15 +1109,14 @@
             x
         )  # (bsz, context_length+(pred_len-1), n_embd_per_head*n_head)
         if use_kv_cache:
             self.y_cache = True
 
         raw_output = x
         
-        
         output = self.param_proj(
             x
         )  # (bsz, context_length+(pred_len-1)) ; (bsz, context_length+(pred_len-1))
 
         output_after_projection = output
         
         output = self.final_activation(output)
```

### Comparing `RL_OM-0.7.95/RL_OM/agents/benchmark_agents/nv_agents_SAA.py` & `RL_OM-0.7.96/RL_OM/agents/benchmark_agents/nv_agents_SAA.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py` & `RL_OM-0.7.96/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/benchmark_agents/qr.py` & `RL_OM-0.7.96/RL_OM/agents/benchmark_agents/qr.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/benchmark_agents/saa.py` & `RL_OM-0.7.96/RL_OM/agents/benchmark_agents/saa.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/benchmark_agents/ss.py` & `RL_OM-0.7.96/RL_OM/agents/benchmark_agents/ss.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/networks/actors.py` & `RL_OM-0.7.96/RL_OM/agents/networks/actors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/networks/base.py` & `RL_OM-0.7.96/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/networks/critics.py` & `RL_OM-0.7.96/RL_OM/agents/networks/critics.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/processors/eoq_preprocessors.py` & `RL_OM-0.7.96/RL_OM/agents/processors/eoq_preprocessors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/processors/processors.py` & `RL_OM-0.7.96/RL_OM/agents/processors/processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,18 @@
     """
     
 
     def __init__(self, increment):
         self.increment = increment
     
     def __call__(self, input):
-        return np.round(input / self.increment) * self.increment
+        # print("input for rounding: ", input)
+        output = np.round(input / self.increment) * self.increment
+        # print("output after rounding: ", output)
+        return output
 
 # %% ../../../nbs/agents/processors/01_processors.ipynb 7
 class ClipNegative():
     """
     This class implements a processor that clips the input to zero if it is
     negative.
```

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/sac_discrete.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.7.96/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/environments/calculation_functions.py` & `RL_OM-0.7.96/RL_OM/environments/calculation_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/environments/10_calculation_functions.ipynb.
 
 # %% auto 0
 __all__ = ['normalize_reward_FC', 'normalize_reward_NV', 'get_orders_arriving_stochastic', 'eoq_qr_calculations_single_action',
-           'eoq_qr_calculations_qr_action', 'mpfc_calculations_ss_action', 'nv_calculations', 'get_fixed_ordering_cost']
+           'ds_calculations', 'eoq_qr_calculations_qr_action', 'mpfc_calculations_ss_action', 'nv_calculations',
+           'get_fixed_ordering_cost']
 
 # %% ../../nbs/environments/10_calculation_functions.ipynb 4
 # General libraries:
 import numpy as np
 import time
 
 # %% ../../nbs/environments/10_calculation_functions.ipynb 8
@@ -220,14 +221,115 @@
     )
 
     self.period += 1
 
     return reward_norm, info
 
 # %% ../../nbs/environments/10_calculation_functions.ipynb 12
+def ds_calculations(self, action):
+
+    # time.sleep(5)
+    # print("raw actions:", action)
+
+    #! Only works for single-product environments.
+    if len(action.shape) == 1:
+        q = action[0]
+        q_expedited = action[1]
+    else:
+        q = action[0][0]
+        q_expedited = action[0][1]
+
+    # print("q:", q)
+    # print("q_expedited:", q_expedited)
+
+    variable_cost_normal_step = self.variable_ordering_cost * q
+    variable_cost_expedited_step = self.variable_ordering_cost_expedited * q_expedited
+    variable_cost_step = variable_cost_normal_step + variable_cost_expedited_step
+    # print("variable_cost_step:", variable_cost_step)
+
+    # print("pipeline before update:", self.order_pipeline)
+
+    if self.use_order_pipeline:
+        if self.lead_time_stochastic:
+
+            raise NotImplementedError("Stochastic lead times not implemented for DS")
+
+        else:
+            orders_arriving = self.order_pipeline[:,-1].copy()
+            # print("orders_arriving: ", orders_arriving)
+
+            self.order_pipeline[:, 1:] = self.order_pipeline[:, :-1]
+            product_indices = np.arange(self.num_products)
+            insert_indices = -self.lead_time
+            self.order_pipeline[product_indices, insert_indices] = q
+            self.order_pipeline[:,-1] += q_expedited
+
+    else:
+        orders_arriving = order
+    
+    # print("pipeline after update:", self.order_pipeline)
+
+    # print("orders_arriving:", orders_arriving)
+    # print("new pipeline:", self.order_pipeline)
+
+    self.inventory += orders_arriving # first, the order will be added to inventory (meaning lead-time is 0)
+
+    # print("inventory after order:", self.inventory)
+
+    self.inventory = np.maximum(self.inventory, 0) # inventory cannot be negative
+
+    self.inventory = np.minimum(self.inventory, self.inventory_cap) # inventory cannot be higher than inventory_cap
+
+    # print("demand:", self.demand[self.period, :])
+
+    self.inventory -= self.demand[self.period, :] # Then demand is subtracted from inventory
+
+    outages = np.where(self.inventory < 0, np.abs(self.inventory), 0)
+    penalty_cost_step = self.underage_cost * outages.sum()
+
+    self.inventory = np.maximum(self.inventory, 0) # inventory cannot be negative
+    holding_cost_step = self.holding_cost * self.inventory
+
+    total_cost_step = variable_cost_step + penalty_cost_step + holding_cost_step
+    reward = - total_cost_step.sum() # maximize negative cost (sum over all products)
+
+    # print(f"fixed_ordering_cost_step: {fixed_ordering_cost_step}")
+    # print(f"penalty_cost_step: {penalty_cost_step}")
+    # print(f"holding_cost_step: {holding_cost_step}")
+
+
+    # print(f"fixed_ordering_cost_step: {fixed_ordering_cost_step}")
+    # print(f"penalty_cost_step: {penalty_cost_step}")
+    # print(f"holding_cost_step: {holding_cost_step}")
+    # print(f"total_cost_step: {total_cost_step}")
+
+    reward_norm = normalize_reward_FC(self, reward)
+
+    # print("new inventory:", self.inventory)
+
+    # # print(f"reward_norm: {reward_norm}")
+    # if self.normalize_reward:
+    # time.sleep(2)
+
+    info = dict(
+            inventory = self.inventory,
+            demand = self.demand[self.period, :],
+            action = action,
+            order = action,
+            penalty = penalty_cost_step,
+            holding = holding_cost_step,
+            variable_ordering_standard = variable_cost_normal_step,
+            variable_ordering_expedited = variable_cost_expedited_step
+    )
+
+    self.period += 1
+
+    return reward_norm, info
+
+# %% ../../nbs/environments/10_calculation_functions.ipynb 13
 def eoq_qr_calculations_qr_action(self, action):
 
     # TODO Think about naming of the function
     
     # print("inventory: ", self.inventory)
     # print("pipeline: ", self.order_pipeline)
     # print("action: ", action.shape)
@@ -323,15 +425,15 @@
             fixed_ordering = fixed_ordering_cost_step,
     )
 
     self.period += 1
 
     return reward_norm, info
 
-# %% ../../nbs/environments/10_calculation_functions.ipynb 13
+# %% ../../nbs/environments/10_calculation_functions.ipynb 14
 def mpfc_calculations_ss_action(self, action):
 
     # TODO Think about naming of the function
 
     if len(action.shape) == 1:
         s = action[0]
         S = action[1]
@@ -397,15 +499,15 @@
             fixed_ordering = fixed_ordering_cost_step,
     )
 
     self.period += 1
 
     return reward_norm, info
 
-# %% ../../nbs/environments/10_calculation_functions.ipynb 14
+# %% ../../nbs/environments/10_calculation_functions.ipynb 15
 def nv_calculations(self, action):
     
     if self.full_demand:
         demand = self.demand[self.period+self.full_additional_context, :]
     else:
         demand = self.demand[self.period, :]
 
@@ -444,15 +546,15 @@
         cost = cost
     )
 
     self.period += 1
 
     return reward_norm, info
 
-# %% ../../nbs/environments/10_calculation_functions.ipynb 16
+# %% ../../nbs/environments/10_calculation_functions.ipynb 17
 def get_fixed_ordering_cost(self, action, positive_only = True):
     """ 
     Returns the fixed ordering cost for the period.
 
     Parameters
     ----------
     action : array
```

### Comparing `RL_OM-0.7.95/RL_OM/environments/data_generators.py` & `RL_OM-0.7.96/RL_OM/environments/data_generators.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/environments/feature_converters.py` & `RL_OM-0.7.96/RL_OM/environments/feature_converters.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.7.96/RL_OM/environments/multi_period_inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
                 ### cost related to overage and underate
                 overage_cost = np.array([0]), 
                 underage_cost = np.array([0]), #! check if there can be a case where this is different from penalty cost
 
                 ### cost related to ordering
                 fixed_ordering_cost = np.array([0]), 
                 variable_ordering_cost = np.array([0]), 
+                variable_ordering_cost_expedited = None,
 
                 ### demand parameters
                 max_demand_backlog = np.array([0]), 
 
                 ### inventory parameters
                 inventory_allowed = True,
                 start_inventory = np.array([0]), 
@@ -48,14 +49,17 @@
                 holding_cost = None, 
 
                 ### ordering parameters
                 lead_time = np.array([0]), 
                 lead_time_stochastic = None, # other values: "gamma", "normal", "normal_percentage"
                 lead_time_variance = np.array([0]), # not implemented, only relevant for stochastic lead times with variance as factor, currently only gamma distribution is implemented
                 max_lead_time = None, # factor dependent on mean demand
+                
+                lead_time_expedited = None,  # only implemented fixed expedited lead time 
+
                 actions_per_product = 1,
                 order_limit_low = None, 
                 order_limit_high = None, 
 
                 ### other parameters
                 horizon = 365, # lenght of each episode in simulation
                 gamma = 1, # discount factor
@@ -140,21 +144,21 @@
 
         # print("overage_cost:", self.overage_cost)
         # print("underage_cost:", self.underage_cost)
 
 
         self.fixed_ordering_cost = self.convert_to_numpy_array(fixed_ordering_cost, expand = True)
         self.variable_ordering_cost = self.convert_to_numpy_array(variable_ordering_cost, expand = True)
+        self.variable_ordering_cost_expedited = self.convert_to_numpy_array(variable_ordering_cost_expedited, expand = True)
 
         self.max_demand_backlog = self.convert_to_numpy_array(max_demand_backlog, expand = True)
 
         # print("max_demand_backlog:", self.max_demand_backlog)
         # print("variable_ordering_cost:", self.variable_ordering_cost)
         # print("fixed_ordering_cost:", self.fixed_ordering_cost)
-        
 
         self.inventory_allowed = inventory_allowed
 
         if not self.inventory_allowed:
             assert np.all(start_inventory == 0), "If inventory is not allowed, start_inventory must be 0"
         self.start_inventory = self.convert_to_numpy_array(start_inventory, expand = True)
         # print("setting inventory cap")
@@ -197,25 +201,31 @@
 
         else:
             if lead_time_stochastic == "gamma":
                 if np.any(lead_time_variance == 1):
                     raise ValueError("Variance of lead time must be greater than 1 for gamma distribution, otherwise it is deterministically 1")
             self.max_lead_time = int(np.ceil(max_lead_time * np.max(self.lead_time))) # max lead time is factor of mean
             self.max_observation_lead_time = self.lag_window # the agnet can look back according to the lag window
+        
+        self.lead_time_expedited = self.convert_to_numpy_array(lead_time_expedited, expand = True)
 
         if order_limit_low is None:
             self.order_limit_low = np.zeros(self.num_products)
             self.order_limit_high = np.ones(self.num_products)
         
         self.order_limit_low = self.convert_to_numpy_array(order_limit_low, expand = True)
         self.order_limit_high = self.convert_to_numpy_array(order_limit_high, expand = True)
 
         # print("order_limit_low:", self.order_limit_low.shape)
         # print("order_limit_high:", self.order_limit_high.shape)
 
+        if self.lead_time_expedited is not None:
+            print("Using Dual Sourcing problem")
+            actions_per_product = actions_per_product*2
+
         order_limit_low = np.repeat(self.order_limit_low, actions_per_product)
         order_limit_high = np.repeat(self.order_limit_high, actions_per_product)
 
         self.action_space = Box(order_limit_low, order_limit_high, shape=(self.num_products*actions_per_product,))
         # print("action space:", self.action_space.shape)
```

### Comparing `RL_OM-0.7.95/RL_OM/experiment_functions/run_experiment.py` & `RL_OM-0.7.96/RL_OM/experiment_functions/run_experiment.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/utils/MLtools.py` & `RL_OM-0.7.96/RL_OM/utils/MLtools.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/utils/utils.py` & `RL_OM-0.7.96/RL_OM/utils/utils.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM/utils.py` & `RL_OM-0.7.96/RL_OM/utils.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.7.96/RL_OM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.7.95
+Version: 0.7.96
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.7.95/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.7.96/RL_OM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.95/settings.ini` & `RL_OM-0.7.96/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.7.95
+version = 0.7.96
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.7.95/setup.py` & `RL_OM-0.7.96/setup.py`

 * *Files identical despite different names*


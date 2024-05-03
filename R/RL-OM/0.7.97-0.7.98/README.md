# Comparing `tmp/RL_OM-0.7.97.tar.gz` & `tmp/RL_OM-0.7.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.7.97.tar", last modified: Fri May  3 09:56:27 2024, max compression
+gzip compressed data, was "RL_OM-0.7.98.tar", last modified: Fri May  3 10:31:57 2024, max compression
```

## Comparing `RL_OM-0.7.97.tar` & `RL_OM-0.7.98.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.833790 RL_OM-0.7.97/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.7.97/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.7.97/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-05-03 09:56:27.833634 RL_OM-0.7.97/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.7.97/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.823108 RL_OM-0.7.97/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)     1284 2024-03-23 05:21:04.000000 RL_OM-0.7.97/RL_OM/MLtools.py
--rw-r--r--   0 magnus     (501) staff       (20)       23 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)   231218 2024-03-21 02:54:55.000000 RL_OM-0.7.97/RL_OM/_modidx 2.py
--rw-r--r--   0 magnus     (501) staff       (20)   248795 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.824332 RL_OM-0.7.97/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.826963 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     1707 2023-12-01 14:08:43.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/PPO_SB3.py
--rw-r--r--   0 magnus     (501) staff       (20)      468 2023-12-01 14:08:43.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/PPO_TEMP.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6605 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/cbs.py
--rw-r--r--   0 magnus     (501) staff       (20)    16468 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/dual_sourcing.py
--rw-r--r--   0 magnus     (501) staff       (20)     6389 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/eoq.py
--rw-r--r--   0 magnus     (501) staff       (20)     8752 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/mp_agents_ERM.py
--rw-r--r--   0 magnus     (501) staff       (20)     2355 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/nv_agents.py
--rw-r--r--   0 magnus     (501) staff       (20)    60657 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/nv_agents_ERM.py
--rw-r--r--   0 magnus     (501) staff       (20)     9918 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/nv_agents_SAA.py
--rw-r--r--   0 magnus     (501) staff       (20)     9350 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py
--rw-r--r--   0 magnus     (501) staff       (20)    23263 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/qr.py
--rw-r--r--   0 magnus     (501) staff       (20)    14565 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/saa.py
--rw-r--r--   0 magnus     (501) staff       (20)    13815 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/benchmark_agents/ss.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.827629 RL_OM-0.7.97/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6890 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1369 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     9657 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.828096 RL_OM-0.7.97/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1383 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/processors/eoq_preprocessors.py
--rw-r--r--   0 magnus     (501) staff       (20)     6523 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.828983 RL_OM-0.7.97/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.830087 RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14243 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13708 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19176 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19614 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19118 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.831797 RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     3234 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)    12009 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py
--rw-r--r--   0 magnus     (501) staff       (20)     4995 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)     5053 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)     5269 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    16656 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)     5082 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
--rw-r--r--   0 magnus     (501) staff       (20)     4875 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.7.97/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.832619 RL_OM-0.7.97/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    20455 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)     6137 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/environments/data_generators.py
--rw-r--r--   0 magnus     (501) staff       (20)     2575 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/environments/feature_converters.py
--rw-r--r--   0 magnus     (501) staff       (20)    44045 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.832921 RL_OM-0.7.97/RL_OM/experiment_functions/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/experiment_functions/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    32862 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/experiment_functions/run_experiment.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.833418 RL_OM-0.7.97/RL_OM/utils/
--rw-r--r--   0 magnus     (501) staff       (20)     1259 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/utils/MLtools.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/utils/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    10828 2024-05-03 09:50:20.000000 RL_OM-0.7.97/RL_OM/utils/utils.py
--rw-r--r--   0 magnus     (501) staff       (20)    10817 2024-03-23 04:58:03.000000 RL_OM-0.7.97/RL_OM/utils.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 09:56:27.824151 RL_OM-0.7.97/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-05-03 09:56:27.000000 RL_OM-0.7.97/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     2660 2024-05-03 09:56:27.000000 RL_OM-0.7.97/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2024-05-03 09:56:27.000000 RL_OM-0.7.97/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2024-05-03 09:56:27.000000 RL_OM-0.7.97/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.7.97/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2024-05-03 09:56:27.000000 RL_OM-0.7.97/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2024-05-03 09:56:27.000000 RL_OM-0.7.97/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      990 2024-05-03 09:52:45.000000 RL_OM-0.7.97/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2024-05-03 09:56:27.833845 RL_OM-0.7.97/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.7.97/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.897328 RL_OM-0.7.98/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.7.98/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.7.98/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-05-03 10:31:57.897173 RL_OM-0.7.98/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.7.98/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.886308 RL_OM-0.7.98/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)     1284 2024-03-23 05:21:04.000000 RL_OM-0.7.98/RL_OM/MLtools.py
+-rw-r--r--   0 magnus     (501) staff       (20)       23 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   231218 2024-03-21 02:54:55.000000 RL_OM-0.7.98/RL_OM/_modidx 2.py
+-rw-r--r--   0 magnus     (501) staff       (20)   248795 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.887885 RL_OM-0.7.98/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.890346 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     1707 2023-12-01 14:08:43.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/PPO_SB3.py
+-rw-r--r--   0 magnus     (501) staff       (20)      468 2023-12-01 14:08:43.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/PPO_TEMP.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6605 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/cbs.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16873 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/dual_sourcing.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6389 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/eoq.py
+-rw-r--r--   0 magnus     (501) staff       (20)     8752 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/mp_agents_ERM.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2355 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/nv_agents.py
+-rw-r--r--   0 magnus     (501) staff       (20)    60657 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/nv_agents_ERM.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9918 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/nv_agents_SAA.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9350 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py
+-rw-r--r--   0 magnus     (501) staff       (20)    23263 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/qr.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14565 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/saa.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13815 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/benchmark_agents/ss.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.890905 RL_OM-0.7.98/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6890 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1369 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9657 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.891319 RL_OM-0.7.98/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1383 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6523 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.892399 RL_OM-0.7.98/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.893435 RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.895002 RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     3234 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)    12009 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4995 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5053 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5269 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16656 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5082 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4875 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.7.98/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.896104 RL_OM-0.7.98/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    20455 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6137 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2575 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    44045 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.896437 RL_OM-0.7.98/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    32862 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/experiment_functions/run_experiment.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.896917 RL_OM-0.7.98/RL_OM/utils/
+-rw-r--r--   0 magnus     (501) staff       (20)     1259 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/utils/MLtools.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/utils/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10828 2024-05-03 10:31:50.000000 RL_OM-0.7.98/RL_OM/utils/utils.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10817 2024-03-23 04:58:03.000000 RL_OM-0.7.98/RL_OM/utils.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-05-03 10:31:57.887737 RL_OM-0.7.98/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-05-03 10:31:57.000000 RL_OM-0.7.98/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     2660 2024-05-03 10:31:57.000000 RL_OM-0.7.98/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2024-05-03 10:31:57.000000 RL_OM-0.7.98/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2024-05-03 10:31:57.000000 RL_OM-0.7.98/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.7.98/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2024-05-03 10:31:57.000000 RL_OM-0.7.98/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2024-05-03 10:31:57.000000 RL_OM-0.7.98/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      990 2024-05-03 10:31:14.000000 RL_OM-0.7.98/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2024-05-03 10:31:57.897380 RL_OM-0.7.98/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.7.98/setup.py
```

### Comparing `RL_OM-0.7.97/LICENSE` & `RL_OM-0.7.98/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/PKG-INFO` & `RL_OM-0.7.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.7.97
+Version: 0.7.98
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.7.97/RL_OM/MLtools.py` & `RL_OM-0.7.98/RL_OM/MLtools.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/_modidx 2.py` & `RL_OM-0.7.98/RL_OM/_modidx 2.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/_modidx.py` & `RL_OM-0.7.98/RL_OM/_modidx.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/PPO_SB3.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/PPO_SB3.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/cbs.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/cbs.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/dual_sourcing.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/dual_sourcing.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             algorithm = algorithm,
             #search_space = search_space
         )
 
         self.precision=precision
 
         if agent_name is None:
-            self.name = 'Single_Index_Agent'
+            self.name = 'Dual_Index_Agent'
         else:
             self.name = agent_name
         
         self.train_directly=True
         self.train_mode = "direct"
 
         super().__init__(mdp_info, policy)
@@ -351,25 +351,28 @@
             numpy.ndarray: The action to be taken, indicating the quantity to order for each product.
 
         """
 
         for preprocessor in self.preprocessors:
             input = preprocessor(input)
 
+        # print("input")
         total_inventory_position = np.sum(input)
+        # print(total_inventory_position)
         if total_inventory_position < self.S_e:
             q_e = self.S_e - total_inventory_position
             q = self.S-self.S_e
         elif total_inventory_position < self.S:
             q_e=0
             q = self.S - total_inventory_position 
         else:
             q_e=0
             q = 0 
 
+        # print("q", q, "q_e", q_e)
         action = np.array([q, q_e])
 
         for postprocessor in self.postprocessors:
             action = postprocessor(action)
 
         return action
     
@@ -427,15 +430,15 @@
                  unit_size = 0.01,
                  preprocessors = None,
                  postprocessors = None,
                  num_iterations_per_parameter = 12,
                  algorithm = "brute_0_1", # "brute_0_1": brute force for demand between 0 and 1 and unit-size <1, "brute_0_1": brute force for demand large 1 and unit size 1
                  ):
         
-        super.__init__(l, l_e, mdp, unit_size, preprocessors, postprocessors, num_iterations_per_parameter, algorithm)
+        super().__init__(l, l_e, mdp, unit_size, preprocessors, postprocessors, num_iterations_per_parameter, algorithm)
     
     def draw_action(self, input):
 
         """
         Generate an action based on the current state.
 
         # TODO adjust description
@@ -449,27 +452,32 @@
             numpy.ndarray: The action to be taken, indicating the quantity to order for each product.
 
         """
 
         for preprocessor in self.preprocessors:
             input = preprocessor(input)
 
-        time.sleep(5)
-        print(input)
+        # print(input)
 
         total_inventory_position = np.sum(input)
-        if total_inventory_position < self.S_e:
-            q_e = self.S_e - total_inventory_position
-            q = self.S-self.S_e
+        expedited_inventory_position = input[0]+np.sum(input[-self.l_e]) # first position is inventory, rest is pipeline vector
+        # print(input[0])
+        # print(input[-self.l_e])
+        # print("total:", expedited_inventory_position)
+
+        if expedited_inventory_position < self.S_e:
+            q_e = self.S_e - expedited_inventory_position
+            q = np.maximum(self.S-total_inventory_position-q_e,0)
         elif total_inventory_position < self.S:
             q_e=0
             q = self.S - total_inventory_position 
         else:
             q_e=0
-            q = 0 
+            q = 0
+        # print("q", q, "q_e", q_e)
 
         action = np.array([q, q_e])
 
         for postprocessor in self.postprocessors:
             action = postprocessor(action)
 
         return action
```

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/mp_agents_ERM.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/mp_agents_ERM.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/nv_agents.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/nv_agents.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/nv_agents_ERM.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/nv_agents_ERM.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/nv_agents_SAA.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/nv_agents_SAA.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/qr.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/qr.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/saa.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/saa.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/benchmark_agents/ss.py` & `RL_OM-0.7.98/RL_OM/agents/benchmark_agents/ss.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/networks/actors.py` & `RL_OM-0.7.98/RL_OM/agents/networks/actors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/networks/base.py` & `RL_OM-0.7.98/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/networks/critics.py` & `RL_OM-0.7.98/RL_OM/agents/networks/critics.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/processors/eoq_preprocessors.py` & `RL_OM-0.7.98/RL_OM/agents/processors/eoq_preprocessors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/processors/processors.py` & `RL_OM-0.7.98/RL_OM/agents/processors/processors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/sac_discrete.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.7.98/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/environments/calculation_functions.py` & `RL_OM-0.7.98/RL_OM/environments/calculation_functions.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/environments/data_generators.py` & `RL_OM-0.7.98/RL_OM/environments/data_generators.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/environments/feature_converters.py` & `RL_OM-0.7.98/RL_OM/environments/feature_converters.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.7.98/RL_OM/environments/multi_period_inventory.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/experiment_functions/run_experiment.py` & `RL_OM-0.7.98/RL_OM/experiment_functions/run_experiment.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/utils/MLtools.py` & `RL_OM-0.7.98/RL_OM/utils/MLtools.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/utils/utils.py` & `RL_OM-0.7.98/RL_OM/utils/utils.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM/utils.py` & `RL_OM-0.7.98/RL_OM/utils.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.7.98/RL_OM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.7.97
+Version: 0.7.98
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.7.97/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.7.98/RL_OM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.97/settings.ini` & `RL_OM-0.7.98/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.7.97
+version = 0.7.98
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.7.97/setup.py` & `RL_OM-0.7.98/setup.py`

 * *Files identical despite different names*


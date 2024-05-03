# Comparing `tmp/utilsrl-0.6.8.tar.gz` & `tmp/utilsrl-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilsrl-0.6.8.tar", last modified: Sun Apr 21 11:55:55 2024, max compression
+gzip compressed data, was "utilsrl-0.6.9.tar", last modified: Fri May  3 17:20:21 2024, max compression
```

## Comparing `utilsrl-0.6.8.tar` & `utilsrl-0.6.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.484351 utilsrl-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 11:55:52.000000 utilsrl-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-21 11:55:55.484351 utilsrl-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-21 11:55:52.000000 utilsrl-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.476351 utilsrl-0.6.8/UtilsRL/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.476351 utilsrl-0.6.8/UtilsRL/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/data_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/data_structure/data_structure.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.480351 utilsrl-0.6.8/UtilsRL/env/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.480351 utilsrl-0.6.8/UtilsRL/env/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/env/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/env/wrapper/atari_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/env/wrapper/base_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/env/wrapper/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/env/wrapper/dmc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/env/wrapper/mujoco_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.480351 utilsrl-0.6.8/UtilsRL/exp/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/exp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/exp/_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/exp/_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/exp/argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.480351 utilsrl-0.6.8/UtilsRL/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/logger/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/logger/composite_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/logger/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/logger/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/logger/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.480351 utilsrl-0.6.8/UtilsRL/math/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/math/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.480351 utilsrl-0.6.8/UtilsRL/misc/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/misc/chore.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/misc/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/misc/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.484351 utilsrl-0.6.8/UtilsRL/net/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/net/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/net/cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/net/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/net/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/net/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.484351 utilsrl-0.6.8/UtilsRL/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/plot/tb_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.484351 utilsrl-0.6.8/UtilsRL/rl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/rl/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.484351 utilsrl-0.6.8/UtilsRL/rl/buffer/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/rl/buffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/rl/buffer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/rl/buffer/prioritized_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/rl/buffer/transition_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/rl/critic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12534 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/rl/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/rl/video_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.484351 utilsrl-0.6.8/UtilsRL/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-21 11:55:52.000000 utilsrl-0.6.8/UtilsRL/third_party/tqdm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:55:55.484351 utilsrl-0.6.8/UtilsRL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-21 11:55:55.000000 utilsrl-0.6.8/UtilsRL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-21 11:55:55.000000 utilsrl-0.6.8/UtilsRL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:55:55.000000 utilsrl-0.6.8/UtilsRL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-21 11:55:55.000000 utilsrl-0.6.8/UtilsRL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 11:55:55.000000 utilsrl-0.6.8/UtilsRL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 11:55:52.000000 utilsrl-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:55:55.484351 utilsrl-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-21 11:55:52.000000 utilsrl-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.302117 utilsrl-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 17:20:17.000000 utilsrl-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-03 17:20:21.302117 utilsrl-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-03 17:20:17.000000 utilsrl-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.294118 utilsrl-0.6.9/UtilsRL/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.294118 utilsrl-0.6.9/UtilsRL/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/data_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/data_structure/data_structure.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.294118 utilsrl-0.6.9/UtilsRL/env/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.298117 utilsrl-0.6.9/UtilsRL/env/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/env/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/env/wrapper/atari_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/env/wrapper/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/env/wrapper/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/env/wrapper/dmc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/env/wrapper/mujoco_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.298117 utilsrl-0.6.9/UtilsRL/exp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/exp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/exp/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/exp/_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/exp/argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.298117 utilsrl-0.6.9/UtilsRL/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/logger/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/logger/composite_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/logger/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/logger/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/logger/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.298117 utilsrl-0.6.9/UtilsRL/math/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/math/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.298117 utilsrl-0.6.9/UtilsRL/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/misc/chore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/misc/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/misc/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.298117 utilsrl-0.6.9/UtilsRL/net/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/net/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/net/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/net/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/net/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/net/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.298117 utilsrl-0.6.9/UtilsRL/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/plot/tb_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.302117 utilsrl-0.6.9/UtilsRL/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/rl/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.302117 utilsrl-0.6.9/UtilsRL/rl/buffer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/rl/buffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/rl/buffer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/rl/buffer/prioritized_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/rl/buffer/transition_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/rl/critic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12534 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/rl/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/rl/video_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.302117 utilsrl-0.6.9/UtilsRL/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-05-03 17:20:17.000000 utilsrl-0.6.9/UtilsRL/third_party/tqdm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:20:21.302117 utilsrl-0.6.9/UtilsRL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-03 17:20:21.000000 utilsrl-0.6.9/UtilsRL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-03 17:20:21.000000 utilsrl-0.6.9/UtilsRL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:20:21.000000 utilsrl-0.6.9/UtilsRL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-03 17:20:21.000000 utilsrl-0.6.9/UtilsRL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 17:20:21.000000 utilsrl-0.6.9/UtilsRL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 17:20:17.000000 utilsrl-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:20:21.302117 utilsrl-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-03 17:20:17.000000 utilsrl-0.6.9/setup.py
```

### Comparing `utilsrl-0.6.8/LICENSE` & `utilsrl-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/PKG-INFO` & `utilsrl-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UtilsRL
-Version: 0.6.8
+Version: 0.6.9
 Summary: A python module desgined for RL logging, monitoring and experiments managing. 
 Home-page: https://github.com/typoverflow/UtilsRL
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `utilsrl-0.6.8/README.md` & `utilsrl-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/data_structure/data_structure.cc` & `utilsrl-0.6.9/UtilsRL/data_structure/data_structure.cc`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/env/__init__.py` & `utilsrl-0.6.9/UtilsRL/env/__init__.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/env/wrapper/atari_wrapper.py` & `utilsrl-0.6.9/UtilsRL/env/wrapper/atari_wrapper.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/env/wrapper/base_wrapper.py` & `utilsrl-0.6.9/UtilsRL/env/wrapper/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/env/wrapper/compat.py` & `utilsrl-0.6.9/UtilsRL/env/wrapper/compat.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/env/wrapper/dmc_wrapper.py` & `utilsrl-0.6.9/UtilsRL/env/wrapper/dmc_wrapper.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/env/wrapper/mujoco_wrapper.py` & `utilsrl-0.6.9/UtilsRL/env/wrapper/mujoco_wrapper.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/exp/__init__.py` & `utilsrl-0.6.9/UtilsRL/exp/__init__.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/exp/_device.py` & `utilsrl-0.6.9/UtilsRL/exp/_device.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/exp/argparse.py` & `utilsrl-0.6.9/UtilsRL/exp/argparse.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/logger/__init__.py` & `utilsrl-0.6.9/UtilsRL/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/logger/base_logger.py` & `utilsrl-0.6.9/UtilsRL/logger/base_logger.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/logger/composite_logger.py` & `utilsrl-0.6.9/UtilsRL/logger/composite_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,20 +44,20 @@
         *args, **kwargs
     ):
         super().__init__(log_dir, name, unique_name, backup_stdout, activate, level)
         if not self.activate:
             return
         # create loggers
         default_config = {
-            "log_dir": log_dir, 
-            "name": name, 
-            "unique_name": unique_name, 
+            "log_dir": self.log_dir, 
+            # "name": name, 
+            "unique_name": self.unique_name, 
             "backup_stdout": False,
-            "activate": activate, 
-            "level": level
+            "activate": self.activate, 
+            "level": self.level
         }
         self.loggers = dict()
         self.logger_config = dict()
         self.logger_cls = set()
         for logger_cls in logger_config:
             config = default_config.copy()
             config.update(logger_config[logger_cls])
@@ -67,22 +67,14 @@
             if config.get("activate", True) == False:
                 continue
             self.loggers[logger_cls] = self.logger_registry[logger_cls](
                 **config
             )
             self.logger_cls.add(logger_cls)
         
-    # def __getattr__(self, __name: str):
-    #     # if the method does not exist for CompositeLogger
-    #     for _logger_cls, _logger in self.loggers.items():
-    #         if hasattr(_logger, __name):
-    #             return _logger.__getattribute__(__name)
-    #     else:
-    #         raise AttributeError(f"CompositeLogger, as well as its components {self.logger_cls}, does not have attribute {str(__name)}.")
-
     def _try_call_by_group(self, func: str, group: list, *args, **kwargs):
         if self.can_log():
             return {
                 _logger_cls: getattr(self.loggers[_logger_cls], func)(*args, **kwargs)\
                     for _logger_cls in group if _logger_cls in self.logger_cls
             }
```

### Comparing `utilsrl-0.6.8/UtilsRL/logger/csv_logger.py` & `utilsrl-0.6.9/UtilsRL/logger/csv_logger.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/logger/tensorboard_logger.py` & `utilsrl-0.6.9/UtilsRL/logger/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/logger/wandb_logger.py` & `utilsrl-0.6.9/UtilsRL/logger/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/math/distributions.py` & `utilsrl-0.6.9/UtilsRL/math/distributions.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/misc/chore.py` & `utilsrl-0.6.9/UtilsRL/misc/chore.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/misc/decorator.py` & `utilsrl-0.6.9/UtilsRL/misc/decorator.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/misc/namespace.py` & `utilsrl-0.6.9/UtilsRL/misc/namespace.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/net/basic.py` & `utilsrl-0.6.9/UtilsRL/net/basic.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/net/cnn.py` & `utilsrl-0.6.9/UtilsRL/net/cnn.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/net/mlp.py` & `utilsrl-0.6.9/UtilsRL/net/mlp.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/net/rnn.py` & `utilsrl-0.6.9/UtilsRL/net/rnn.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/plot/tb_parser.py` & `utilsrl-0.6.9/UtilsRL/plot/tb_parser.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/rl/actor.py` & `utilsrl-0.6.9/UtilsRL/rl/actor.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/rl/buffer/__init__.py` & `utilsrl-0.6.9/UtilsRL/rl/buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/rl/buffer/base.py` & `utilsrl-0.6.9/UtilsRL/rl/buffer/base.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/rl/buffer/prioritized_replay.py` & `utilsrl-0.6.9/UtilsRL/rl/buffer/prioritized_replay.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/rl/buffer/transition_replay.py` & `utilsrl-0.6.9/UtilsRL/rl/buffer/transition_replay.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/rl/critic.py` & `utilsrl-0.6.9/UtilsRL/rl/critic.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/rl/normalizer.py` & `utilsrl-0.6.9/UtilsRL/rl/normalizer.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/rl/video_recorder.py` & `utilsrl-0.6.9/UtilsRL/rl/video_recorder.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL/third_party/tqdm.py` & `utilsrl-0.6.9/UtilsRL/third_party/tqdm.py`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/UtilsRL.egg-info/PKG-INFO` & `utilsrl-0.6.9/UtilsRL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UtilsRL
-Version: 0.6.8
+Version: 0.6.9
 Summary: A python module desgined for RL logging, monitoring and experiments managing. 
 Home-page: https://github.com/typoverflow/UtilsRL
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `utilsrl-0.6.8/UtilsRL.egg-info/SOURCES.txt` & `utilsrl-0.6.9/UtilsRL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `utilsrl-0.6.8/setup.py` & `utilsrl-0.6.9/setup.py`

 * *Files identical despite different names*


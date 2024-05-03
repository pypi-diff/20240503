# Comparing `tmp/momaland-0.0.2.tar.gz` & `tmp/momaland-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momaland-0.0.2.tar", last modified: Wed Dec 20 09:26:14 2023, max compression
+gzip compressed data, was "momaland-0.1.0.tar", last modified: Fri May  3 17:02:59 2024, max compression
```

## Comparing `momaland-0.0.2.tar` & `momaland-0.1.0.tar`

### file list

```diff
@@ -1,74 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.239762 momaland-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-20 09:26:01.000000 momaland-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2023-12-20 09:26:14.239762 momaland-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2023-12-20 09:26:01.000000 momaland-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.231762 momaland-0.0.2/momaland/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.231762 momaland-0.0.2/momaland/envs/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.231762 momaland-0.0.2/momaland/envs/beach_domain/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/beach_domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/beach_domain/beach_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/beach_domain/mobeach_v0.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.235762 momaland-0.0.2/momaland/envs/congestion_game/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/congestion_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17931 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/congestion_game/congestion_game.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/congestion_game/mocongestion_v0.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.235762 momaland-0.0.2/momaland/envs/congestion_game/networks/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/congestion_game/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7665 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/congestion_game/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.235762 momaland-0.0.2/momaland/envs/crazyrl/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.235762 momaland-0.0.2/momaland/envs/crazyrl/catch/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/catch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/catch/catch.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/catch/catch_v0.py
--rw-r--r--   0 runner    (1001) docker     (127)    13886 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/crazyRL_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.235762 momaland-0.0.2/momaland/envs/crazyrl/escort/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/escort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/escort/escort.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/escort/escort_v0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/gl_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.235762 momaland-0.0.2/momaland/envs/crazyrl/surround/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/surround/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/surround/surround.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/crazyrl/surround/surround_v0.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.235762 momaland-0.0.2/momaland/envs/item_gathering/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/item_gathering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/item_gathering/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18563 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/item_gathering/item_gathering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/item_gathering/map_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/item_gathering/moitemgathering_v0.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.239762 momaland-0.0.2/momaland/envs/multiwalker/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/multiwalker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/multiwalker/momultiwalker_v0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/multiwalker/multiwalker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/multiwalker/multiwalker_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.239762 momaland-0.0.2/momaland/envs/pistonball/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/pistonball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/pistonball/mopistonball_v0.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/envs/pistonball/pistonball.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.239762 momaland-0.0.2/momaland/test/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17700 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/test/api_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/test/wrapper_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.239762 momaland-0.0.2/momaland/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/utils/aec_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/utils/all_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/utils/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/utils/generate_gif_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/utils/parallel_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-12-20 09:26:01.000000 momaland-0.0.2/momaland/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.239762 momaland-0.0.2/momaland.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2023-12-20 09:26:14.000000 momaland-0.0.2/momaland.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2023-12-20 09:26:14.000000 momaland-0.0.2/momaland.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 09:26:14.000000 momaland-0.0.2/momaland.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-20 09:26:14.000000 momaland-0.0.2/momaland.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-20 09:26:14.000000 momaland-0.0.2/momaland.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2023-12-20 09:26:01.000000 momaland-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 09:26:14.239762 momaland-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      844 2023-12-20 09:26:01.000000 momaland-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:14.239762 momaland-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2023-12-20 09:26:01.000000 momaland-0.0.2/tests/test_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.957113 momaland-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-03 17:02:51.000000 momaland-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-05-03 17:02:59.957113 momaland-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-05-03 17:02:51.000000 momaland-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.941113 momaland-0.1.0/momaland/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.941113 momaland-0.1.0/momaland/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.941113 momaland-0.1.0/momaland/envs/beach/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/beach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15522 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/beach/beach.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/beach/mobeach_v0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.941113 momaland-0.1.0/momaland/envs/breakthrough/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/breakthrough/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/breakthrough/breakthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/breakthrough/breakthrough_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/breakthrough/mobreakthrough_v0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.941113 momaland-0.1.0/momaland/envs/congestion/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/congestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/congestion/congestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/congestion/mocongestion_v0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.941113 momaland-0.1.0/momaland/envs/congestion/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/congestion/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/congestion/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.941113 momaland-0.1.0/momaland/envs/connect4/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/connect4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18730 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/connect4/connect4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/connect4/connect4_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/connect4/moconnect4_v0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.945113 momaland-0.1.0/momaland/envs/crazyrl/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.945113 momaland-0.1.0/momaland/envs/crazyrl/catch/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/catch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/catch/catch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/catch/catch_v0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/crazyRL_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.945113 momaland-0.1.0/momaland/envs/crazyrl/escort/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/escort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/escort/escort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/escort/escort_v0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/gl_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.945113 momaland-0.1.0/momaland/envs/crazyrl/surround/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/surround/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/surround/surround.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/crazyrl/surround/surround_v0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.945113 momaland-0.1.0/momaland/envs/gem_mining/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/gem_mining/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/gem_mining/gem_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/gem_mining/mogem_mining_v0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.945113 momaland-0.1.0/momaland/envs/ingenious/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/ingenious/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/ingenious/ingenious.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17871 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/ingenious/ingenious_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16070 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/ingenious/ingenious_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/ingenious/ingenious_seedtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/ingenious/moingenious_v0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.945113 momaland-0.1.0/momaland/envs/item_gathering/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/item_gathering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/item_gathering/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19125 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/item_gathering/item_gathering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/item_gathering/map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/item_gathering/moitem_gathering_v0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.949113 momaland-0.1.0/momaland/envs/multiwalker_stability/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/multiwalker_stability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/multiwalker_stability/momultiwalker_stability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/multiwalker_stability/momultiwalker_stability_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/multiwalker_stability/momultiwalker_stability_v0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.949113 momaland-0.1.0/momaland/envs/pistonball/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/pistonball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/pistonball/mopistonball_v0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/pistonball/pistonball.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.949113 momaland-0.1.0/momaland/envs/samegame/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/samegame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/samegame/mosame_game_v0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23689 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/samegame/same_game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/envs/samegame/samegame_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.949113 momaland-0.1.0/momaland/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.949113 momaland-0.1.0/momaland/learning/cooperative_momappo/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/cooperative_momappo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26043 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/cooperative_momappo/continuous_momappo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/cooperative_momappo/discrete_momappo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/cooperative_momappo/exec_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/cooperative_momappo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.949113 momaland-0.1.0/momaland/learning/iql/
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/iql/iql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/iql/pf_bpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/iql/plot_exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/iql/plot_pf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/iql/tabular_bpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/iql/train_iql_bpd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.953113 momaland-0.1.0/momaland/learning/morl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/morl/random_centralised_agent_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/morl/sa_env_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/morl/train_bpd_GPILS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/morl/train_bpd_PCN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/morl/train_ig_GPILS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/morl/train_ig_PCN.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/u_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/learning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.953113 momaland-0.1.0/momaland/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17700 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/test/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/test/wrapper_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.953113 momaland-0.1.0/momaland/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/utils/aec_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/utils/all_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/utils/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/utils/generate_gif_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-03 17:02:51.000000 momaland-0.1.0/momaland/utils/parallel_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.953113 momaland-0.1.0/momaland.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-05-03 17:02:59.000000 momaland-0.1.0/momaland.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-03 17:02:59.000000 momaland-0.1.0/momaland.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:02:59.000000 momaland-0.1.0/momaland.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-03 17:02:59.000000 momaland-0.1.0/momaland.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 17:02:59.000000 momaland-0.1.0/momaland.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-03 17:02:51.000000 momaland-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:02:59.957113 momaland-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-03 17:02:51.000000 momaland-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:02:59.953113 momaland-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-03 17:02:51.000000 momaland-0.1.0/tests/test_envs.py
```

### Comparing `momaland-0.0.2/LICENSE` & `momaland-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `momaland-0.0.2/momaland/envs/beach_domain/beach_domain.py` & `momaland-0.1.0/momaland/envs/beach/beach.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """Beach problem domain.
 
 From Mannion, P., Devlin, S., Duggan, J., and Howley, E. (2018). Reward shaping for knowledge-based multi-objective multi-agent reinforcement learning.
 """
 
 import functools
 import random
-
-# from gymnasium.utils import EzPickle
 from typing_extensions import override
 
 import numpy as np
 from gymnasium.logger import warn
 from gymnasium.spaces import Box, Discrete
+from gymnasium.utils import EzPickle
 from pettingzoo.utils import wrappers
 
 from momaland.utils.conversions import mo_parallel_to_aec
 from momaland.utils.env import MOParallelEnv
 
 
 LEFT = -1
 RIGHT = 1
 STAY = 0
-MOVES = ["LEFT", "RIGHT", "STAY"]
+MOVES = [LEFT, STAY, RIGHT]
 NUM_OBJECTIVES = 2
 
 
 def parallel_env(**kwargs):
     """Parallel env factory function for the beach problem domain."""
     return raw_env(**kwargs)
 
@@ -48,35 +47,71 @@
 
 
 def raw_env(**kwargs):
     """Env factory function for the beach problem domain."""
     return MOBeachDomain(**kwargs)
 
 
-class MOBeachDomain(MOParallelEnv):
-    """Environment for MO Beach problem domain.
+class MOBeachDomain(MOParallelEnv, EzPickle):
+    """A `Parallel` 2-objective environment of the Beach problem domain.
 
-    The init method takes in environment arguments and should define the following attributes:
-    - possible_agents
-    - action_spaces
-    - observation_spaces
-    These attributes should not be changed after initialization.
+    ## Observation Space
+    The observation space is a continuous box with the length `5` containing:
+     - agent type
+     - section id (where the agent is)
+     - section capacity
+     - section consumption
+     - percentage of agents of the agent's type in the section
+
+    Example:
+    `[a_type, section_id, section_capacity, section_consumption, %_of_a_of_current_type]`
+
+    ## Action Space
+    The action space is a Discrete space [0, 1, 2], corresponding to moving left, moving right, staying in place.
+
+    ## Reward Space
+    The reward space is a 2D vector containing rewards for two different schemes ('local' or 'global') for:
+    - the occupation level
+    - the mixture level
+    If the scheme is 'local', the reward is given for the currently occupied section.
+    If the scheme is 'global', the reward is summed over all sections.
+
+    ## Starting State
+    The initial position is a uniform random distribution of agents over the sections. This can be changed via the
+    'position_distribution' argument. The agent types are also randomly distributed according to the
+    'type_distribution' argument. The default is a uniform distribution over all types.
+
+    ## Episode Termination
+    The episode is terminated if num_timesteps is reached. The default value is 100.
+    Agents only receive the reward after the last timestep.
+
+    ## Episode Truncation
+    The problem is not truncated. It has a maximum number of timesteps.
+
+    ## Arguments
+    - 'num_timesteps (int)': number of timesteps in the domain. Default: 1
+    - 'num_agents (int)': number of agents in the domain. Default: 100
+    - 'reward_scheme (str)': the reward scheme to use ('local', or 'global'). Default: local
+    - 'sections (int)': number of beach sections in the domain. Default: 6
+    - 'capacity (int)': capacity of each beach section. Default: 7
+    - 'type_distribution (tuple)': the distribution of agent types in the domain. Default: 2 types equally distributed (0.3, 0.7).
+    - 'position_distribution (tuple)': the initial distribution of agents in the domain. Default: uniform over all sections (None).
+    - 'render_mode (str)': render mode. Default: None
     """
 
-    metadata = {"render_modes": ["human"], "name": "mobeach_v0"}
+    metadata = {"render_modes": ["human"], "name": "mobeach_v0", "central_observation": True}
 
-    # TODO does this environment require max_cycle?
     def __init__(
         self,
-        num_timesteps=10,
+        num_timesteps=1,
         num_agents=100,
         reward_scheme="local",
         sections=6,
-        capacity=10,
-        type_distribution=(0.5, 0.5),
+        capacity=7,
+        type_distribution=(0.3, 0.7),
         position_distribution=None,
         render_mode=None,
     ):
         """Initializes the beach domain.
 
         Args:
             sections: number of beach sections in the domain
@@ -84,14 +119,25 @@
             num_agents: number of agents in the domain
             type_distribution: the distribution of agent types in the domain. Default: 2 types equally distributed.
             position_distribution: the initial distribution of agents in the domain. Default: uniform over all sections.
             num_timesteps: number of timesteps in the domain
             render_mode: render mode
             reward_scheme: the reward scheme to use ('local', or 'global'). Default: local
         """
+        EzPickle.__init__(
+            self,
+            num_timesteps,
+            num_agents,
+            reward_scheme,
+            sections,
+            capacity,
+            type_distribution,
+            position_distribution,
+            render_mode,
+        )
         self.reward_scheme = reward_scheme
         self.sections = sections
         # TODO Extend to distinct capacities per section?
         self.resource_capacities = [capacity for _ in range(sections)]
         self.num_timesteps = num_timesteps
         self.episode_num = 0
         self.type_distribution = type_distribution
@@ -102,15 +148,15 @@
                 len(position_distribution) == self.sections
             ), "number of sections should be equal to the length of the provided position_distribution:"
             self.position_distribution = position_distribution
 
         self.render_mode = render_mode
         self.possible_agents = ["agent_" + str(r) for r in range(num_agents)]
         self.agents = self.possible_agents[:]
-        self.types, self.state = self._init_state()
+        self._types, self._state = self._init_state()
         self.terminations = {agent: False for agent in self.agents}
         self.truncations = {agent: False for agent in self.agents}
 
         self.action_spaces = dict(zip(self.agents, [Discrete(len(MOVES))] * num_agents))
         self.observation_spaces = dict(
             zip(
                 self.agents,
@@ -124,14 +170,23 @@
                         dtype=np.float32,
                     )
                 ]
                 * num_agents,
             )
         )
 
+        self.central_observation_space = Box(
+            low=0,
+            high=self.num_agents,
+            # Observation form:
+            # agents * [agent type, section id, section capacity, section consumption, % of agents of current type]
+            shape=(self.num_agents * 5,),
+            dtype=np.float32,
+        )
+
         # maximum capacity reward can be calculated  by calling the _global_capacity_reward()
         optimal_consumption = [capacity for _ in range(sections)]
         optimal_consumption[-1] = max(self.num_agents - ((sections - 1) * capacity), 0)
         max_r = _global_capacity_reward(self.resource_capacities, optimal_consumption)
         self.reward_spaces = dict(zip(self.agents, [Box(low=0, high=max_r, shape=(NUM_OBJECTIVES,))] * num_agents))
 
     # this cache ensures that same space object is returned for the same agent
@@ -148,14 +203,18 @@
         return self.action_spaces[agent]
 
     @override
     def reward_space(self, agent):
         """Returns the reward space for the given agent."""
         return self.reward_spaces[agent]
 
+    def get_central_observation_space(self):
+        """Returns the central observation space."""
+        return self.central_observation_space
+
     @override
     def render(self):
         """Renders the environment.
 
         In human mode, it can print to terminal, open
         up a graphical window, or open up some other display that a human can see and understand.
         """
@@ -174,15 +233,15 @@
 
         Returns the observations for each agent
         """
         if seed is not None:
             np.random.seed(seed)
             random.seed(seed)
         self.agents = self.possible_agents[:]
-        self.types, self.state = self._init_state()
+        self._types, self._state = self._init_state()
         self.terminations = {agent: False for agent in self.agents}
         self.truncations = {agent: False for agent in self.agents}
         section_consumptions, section_agent_types = self._get_stats()
         observations = {
             agent: self._get_obs(i, section_consumptions, section_agent_types) for i, agent in enumerate(self.agents)
         }
         self.episode_num = 0
@@ -222,15 +281,15 @@
         if not actions:
             self.agents = []
             return {}, {}, {}, {}, {}
 
         # Apply actions and update system state
         for i, agent in enumerate(self.agents):
             act = actions[agent]
-            self.state[i] = min(self.sections - 1, max(self.state[i] + act, 0))
+            self._state[i] = min(self.sections - 1, max(self._state[i] + MOVES[act], 0))
 
         section_consumptions, section_agent_types = self._get_stats()
 
         self.episode_num += 1
 
         env_termination = self.episode_num >= self.num_timesteps
         self.terminations = {agent: env_termination for agent in self.agents}
@@ -251,44 +310,66 @@
         # Obs: agent type, section id, section capacity, section consumption, % of agents of current type
         observations = {agent: None for agent in self.agents}
         # Note that agents only receive the reward after the last timestep
         rewards = {self.agents[i]: np.array([0, 0], dtype=np.float32) for i in range(self.num_agents)}
 
         for i, agent in enumerate(self.agents):
             observations[agent] = self._get_obs(i, section_consumptions, section_agent_types)
-            rewards[agent] = reward_per_section[self.state[i]]
+            rewards[agent] = reward_per_section[self._state[i]]
 
         # typically there won't be any information in the infos, but there must
         # still be an entry for each agent
         infos = {agent: {} for agent in self.agents}
 
         if env_termination:
             self.agents = []
 
         if self.render_mode == "human":
             self.render()
 
         return observations, rewards, self.truncations, self.terminations, infos
 
+    @override
+    def state(self) -> np.ndarray:
+        """Returns the global observation of the beach.
+
+        Returns: a 1D Numpy array with the following items in order:
+        [agentX_section, agentX_type, ...,
+        capacity, sectionY_consumption, sectionY_%_of_agents_of_current_type, ...]
+        """
+        # return np.array(self._types + self._state, dtype=np.int32)
+        section_consumptions, section_agent_types = self._get_stats()
+        global_obs = [self._get_obs(i, section_consumptions, section_agent_types) for i in range(len(self.agents))]
+        global_obs = np.array(global_obs, dtype=np.float32).flatten()
+        assert len(global_obs) == len(self.agents) * 5
+
+        return np.array(global_obs, dtype=np.float32).flatten()
+
     def _get_obs(self, i, section_consumptions, section_agent_types):
-        total_same_type = section_agent_types[self.state[i]][self.types[i]]
-        t = total_same_type / section_consumptions[self.state[i]]
+        total_same_type = section_agent_types[self._state[i]][self._types[i]]
+        t = total_same_type / section_consumptions[self._state[i]]
         obs = np.array(
-            [self.types[i], self.state[i], self.resource_capacities[self.state[i]], section_consumptions[self.state[i]], t],
+            [
+                self._types[i],
+                self._state[i],
+                self.resource_capacities[self._state[i]],
+                section_consumptions[self._state[i]],
+                t,
+            ],
             dtype=np.float32,
         )
         return obs
 
     def _get_stats(self):
         section_consumptions = np.zeros(self.sections)
         section_agent_types = np.zeros((self.sections, len(self.type_distribution)))
 
         for i in range(len(self.agents)):
-            section_consumptions[self.state[i]] += 1
-            section_agent_types[self.state[i]][self.types[i]] += 1
+            section_consumptions[self._state[i]] += 1
+            section_agent_types[self._state[i]][self._types[i]] += 1
         return section_consumptions, section_agent_types
 
 
 def _global_capacity_reward(capacities, consumptions):
     global_capacity_r = 0
     for i in range(len(capacities)):
         global_capacity_r += _local_capacity_reward(capacities[i], consumptions[i])
```

### Comparing `momaland-0.0.2/momaland/envs/congestion_game/congestion_game.py` & `momaland-0.1.0/momaland/envs/congestion/congestion.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from collections import defaultdict
 from typing_extensions import override
 
 import networkx as nx
 import numpy as np
 from gymnasium.logger import warn
 from gymnasium.spaces import Box, Discrete
+from gymnasium.utils import EzPickle
 from pettingzoo.utils import wrappers
 from sympy import diff, lambdify, sympify
 
 from momaland.utils.conversions import mo_parallel_to_aec
 from momaland.utils.env import MOParallelEnv
 
 
@@ -42,25 +43,55 @@
     # this wrapper helps error handling for discrete action spaces
     env = wrappers.AssertOutOfBoundsWrapper(env)
     return env
 
 
 def raw_env(**kwargs):
     """Env factory function for the congestion game."""
-    return MOCongestionGame(**kwargs)
+    return MOCongestion(**kwargs)
 
 
-class MOCongestionGame(MOParallelEnv):
-    """Environment for MO Congestion Game problem.
+class MOCongestion(MOParallelEnv, EzPickle):
+    """A `Parallel` environment where drivers learn to travel from a source to a destination while avoiding congestion.
 
-    The init method takes in environment arguments and should define the following attributes:
-    - possible_agents
-    - action_spaces
-    - observation_spaces
-    These attributes should not be changed after initialization.
+    Multi-objective version of Braess' Paradox where drivers have two objectives: travel time and monetary cost.
+    The environment is a road network and the agents are the drivers that needs to travel from an origin to a destination point.
+
+    ## Observation Space
+    This environment is stateless, so the observation space is a constant 0. (Discrete with shape (1,)).
+
+    ## Action Space
+    The action space is a discrete space representing the possible routes that the agent can take.
+    The number of routes is different for each agent, as it depends on the number of possible routes for the OD pair of the agent.
+    Selecting an action corresponds to choosing a route.
+
+    ## Reward Space
+    The reward space is a 2D vector containing rewards for:
+    - Minimizing travel time (latency).
+    - Minimizing monetary cost.
+
+    ## Starting State
+    The environment is stateless, so there is no starting state.
+
+    ## Episode Termination
+    The environment is stateless, so there are no episodes. Each "episode" is therefore terminated after each timestep.
+
+    ## Episode Truncation
+    Episodes are not truncated as there are terminated after each timestep.
+
+    ## Arguments
+    - `render_mode (str, optional)`: The mode to display the rendering of the environment. Can be human or None.
+    - `problem_name (str, optional)`: The name of the road network that will be used.
+    - `num_agents (int, optional)`: The number of drivers in the network.
+    - `toll_mode (str, optional)`: The tolling mode that is used, tolls are either placed randomly "random" or using marginal cost tolling "mct".
+    - `random_toll_percentage (float, optional)`: In the case of random tolling the percentage of roads that will be taxed.
+    - `num_timesteps (int, optional)`: The number of timesteps (stateless, therefore always 1 timestep).
+
+    ## Credits
+    The code was adapted from [codebase of "Toll-Based Learning for Minimising Congestion under Heterogeneous Preferences"](https://github.com/goramos/marl-route-choice).
     """
 
     def __init__(
         self,
         problem_name="Braess_1_4200_10_c1",
         num_agents=4200,
         toll_mode="mct",
@@ -74,14 +105,23 @@
             problem_name: the name of the network that will be used
             num_agents: number of agents in the network
             toll_mode: the tolling mode that is used, tolls are either placed randomly "random" or using marginal cost tolling "mct"
             random_toll_percentage: in the case of random tolling the percentage of roads that will be taxed
             num_timesteps: number of timesteps (stateless, therefore always 1 timestep)
             render_mode: render mode
         """
+        EzPickle.__init__(
+            self,
+            problem_name,
+            num_agents,
+            toll_mode,
+            random_toll_percentage,
+            num_timesteps,
+            render_mode,
+        )
         # Read in the problem from the corresponding .json file in the networks directory
         self.graph, self.od, self.routes, self._max_route_length = self._read_problem(problem_name)
         # Keep track of the current flow on each link the network
         self.flows = {f"{edge[0]}-{edge[1]}": 0 for edge in self.graph.edges}
 
         # Episodes/Timesteps
         self.num_timesteps = num_timesteps
@@ -100,19 +140,16 @@
         # action space can be different for agents when there are multiple OD pairs with different numbers of routes
         self.action_spaces = dict(zip(self.agents, route_choices_per_agent))
         # stateless setting, agents receive a constant '0' as an observation in each timestep
         self.observation_spaces = dict(
             zip(
                 self.agents,
                 [
-                    Box(
-                        low=0,
-                        high=self.num_agents,
-                        shape=(1,),
-                        dtype=np.float32,
+                    Discrete(
+                        1,
                     )
                 ]
                 * num_agents,
             )
         )
         # keep track of the maximum link latency and cost to scale the rewards returned to the agents
         self._max_link_latency = None
@@ -166,15 +203,15 @@
             np.random.seed(seed)
             random.seed(seed)
         self.agents = self.possible_agents[:]
         self.terminations = {agent: False for agent in self.agents}
         self.truncations = {agent: False for agent in self.agents}
         # Reset the flows of each arc
         self.flows = {f"{edge[0]}-{edge[1]}": 0 for edge in self.graph.edges}
-        observations = {agent: np.array([0], dtype=np.float32) for agent in self.agents}
+        observations = {agent: 0 for agent in self.agents}
         self.episode_num = 0
 
         infos = {agent: {} for agent in self.agents}
         return observations, infos
 
     def _init_state(self):
         """Initializes the state of the environment. This is called by reset()."""
@@ -216,15 +253,15 @@
             agent_routes.append(agent_route)
         # add the flow of all routes to the links of each route:
         for route in agents_on_routes:
             self._add_flow_to_route(route, agents_on_routes[route])
 
         # - Observations -#
         # return constant observations '0' as this is a stateless setting
-        observations = {agent: np.array([0], dtype=np.float32) for agent in self.agents}
+        observations = {agent: 0 for agent in self.agents}
 
         # - Rewards -#
         # compute latency and cost of each route
         latency_routes, cost_routes = self._compute_latency_and_cost(agents_on_routes)
 
         rewards = dict()
         for i in range(len(self.agents)):
```

### Comparing `momaland-0.0.2/momaland/envs/congestion_game/networks/utils.py` & `momaland-0.1.0/momaland/envs/congestion/networks/utils.py`

 * *Files identical despite different names*

### Comparing `momaland-0.0.2/momaland/envs/crazyrl/crazyRL_base.py` & `momaland-0.1.0/momaland/envs/crazyrl/crazyRL_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,53 +3,16 @@
 from typing import Optional
 from typing_extensions import override
 
 import numpy as np
 import numpy.typing as npt
 import pygame
 from gymnasium import spaces
-from OpenGL.GL import (
-    GL_AMBIENT,
-    GL_AMBIENT_AND_DIFFUSE,
-    GL_BLEND,
-    GL_COLOR_BUFFER_BIT,
-    GL_COLOR_MATERIAL,
-    GL_DEPTH_BUFFER_BIT,
-    GL_DEPTH_TEST,
-    GL_DIFFUSE,
-    GL_FRONT_AND_BACK,
-    GL_LIGHT0,
-    GL_LIGHTING,
-    GL_MODELVIEW,
-    GL_MODELVIEW_MATRIX,
-    GL_ONE_MINUS_SRC_ALPHA,
-    GL_POSITION,
-    GL_PROJECTION,
-    GL_SMOOTH,
-    GL_SRC_ALPHA,
-    glBlendFunc,
-    glClear,
-    glColor4f,
-    glColorMaterial,
-    glEnable,
-    glGetFloatv,
-    glLight,
-    glLightfv,
-    glLineWidth,
-    glLoadIdentity,
-    glMatrixMode,
-    glMultMatrixf,
-    glPopMatrix,
-    glPushMatrix,
-    glShadeModel,
-)
-from OpenGL.raw.GLU import gluLookAt, gluPerspective
 from pygame import DOUBLEBUF, OPENGL
 
-from momaland.envs.crazyrl.gl_utils import axes, field, point, target_point
 from momaland.utils.env import MOParallelEnv
 
 
 def _distance_to_target(agent_location: npt.NDArray[np.float32], target_location: npt.NDArray[np.float32]) -> float:
     return np.linalg.norm(agent_location - target_location)
 
 
@@ -309,14 +272,52 @@
         infos = self._compute_info()
 
         return observations, rewards, terminations, truncations, infos
 
     @override
     def render(self):
         """Renders the current frame of the environment. Only works in human rendering mode."""
+        from OpenGL.GL import (
+            GL_AMBIENT,
+            GL_AMBIENT_AND_DIFFUSE,
+            GL_BLEND,
+            GL_COLOR_BUFFER_BIT,
+            GL_COLOR_MATERIAL,
+            GL_DEPTH_BUFFER_BIT,
+            GL_DEPTH_TEST,
+            GL_DIFFUSE,
+            GL_FRONT_AND_BACK,
+            GL_LIGHT0,
+            GL_LIGHTING,
+            GL_MODELVIEW,
+            GL_MODELVIEW_MATRIX,
+            GL_ONE_MINUS_SRC_ALPHA,
+            GL_POSITION,
+            GL_PROJECTION,
+            GL_SMOOTH,
+            GL_SRC_ALPHA,
+            glBlendFunc,
+            glClear,
+            glColor4f,
+            glColorMaterial,
+            glEnable,
+            glGetFloatv,
+            glLight,
+            glLightfv,
+            glLineWidth,
+            glLoadIdentity,
+            glMatrixMode,
+            glMultMatrixf,
+            glPopMatrix,
+            glPushMatrix,
+            glShadeModel,
+        )
+        from OpenGL.raw.GLU import gluLookAt, gluPerspective
+
+        from momaland.envs.crazyrl.gl_utils import axes, field, point, target_point
 
         def init_window():
             """Initializes the PyGame window."""
             pygame.init()
             pygame.display.init()
             pygame.display.set_caption("Crazy RL")
```

### Comparing `momaland-0.0.2/momaland/envs/crazyrl/escort/escort.py` & `momaland-0.1.0/momaland/envs/crazyrl/escort/escort.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Escort environment for Crazyflie 2. Each agent is supposed to learn to surround a common target point moving to one point to another."""
 
 from typing_extensions import override
 
 import numpy as np
+from gymnasium.utils import EzPickle
 from pettingzoo.utils.wrappers import AssertOutOfBoundsWrapper
 
 from momaland.envs.crazyrl.crazyRL_base import FPS, CrazyRLBaseParallelEnv
 from momaland.utils.conversions import mo_parallel_to_aec
 
 
 def env(*args, **kwargs):
@@ -37,43 +38,88 @@
     return env
 
 
 def raw_env(*args, **kwargs):
     """Returns the environment in `Parallel` format.
 
     Args:
-        **kwargs: keyword args to forward to create the `MOMultiwalker` environment.
+        **kwargs: keyword args to forward to create the `CrazyRLEscort` environment.
 
     Returns:
         A raw env.
     """
     return Escort(*args, **kwargs)
 
 
-class Escort(CrazyRLBaseParallelEnv):
-    """A Parallel Environment where drone learn how to surround a moving target, going straight to one point to another."""
+class Escort(CrazyRLBaseParallelEnv, EzPickle):
+    """A `Parallel` environment where drones learn how to escort a moving target.
+
+    ## Observation Space
+    The observation space is a continuous box with the length `(num_drones + 1) * 3` where each 3 values represent the XYZ coordinates of the drones in this order:
+    - the agent.
+    - the target.
+    - the other agents.
+
+    Example:
+    `[x_0, y_0, z_0, x_targ, y_targ, z_targ, x_1, y_1, z_1, ..., x_n, y_n, z_n]`
+
+    ## Action Space
+    The action space is a 3D speed vector representing the direction in which the agent should move.
+
+    ## Reward Space
+    The reward space is a 2D vector containing rewards for:
+    - Minimizing distance towards the target
+    - Maximizing average distance towards other agents (avoiding collision).
+
+    ## Starting State
+    Where `size = 3`, the initial starting positions of the agents are `[0, 0, 1], [1, 1, 1], [0, 1, 1], [2, 2, 1]` while the target position is `[1, 1, 2.5]`
+
+    ## Episode Termination
+    The episode is terminated if one of the following conditions are met:
+    - 2 agents collide.
+    - An agent and the target collide.
+    - An agent collides with the ground.
+
+    ## Episode Truncation
+    The episode is truncated when an agent reaches 200 steps.
+
+    ## Arguments
+    - `render_mode (str, optional)`: The mode to display the rendering of the environment. Can be human or None.
+    - `size (int, optional)`: Size of the area sides
+    - `num_drones (int, optional)`: Amount of drones
+    - `init_flying_pos (nparray[float], optional)`: 2d array containing the coordinates of the agents is a (3)-shaped array containing the initial XYZ position of the drones.
+    - `init_target_location (nparray[float], optional)`: A (3)-shaped array for the XYZ position of the target.
+    - `target_speed (float, optional)`: Distance traveled by the target at each timestep
+    - `final_target_location (nparray[float], optional)`: Array of the final position of the moving target
+    - `num_intermediate_points (int, optional)`: Number of intermediate points in the target trajectory
+
+    ## Credits
+    The code was adapted from [Felten's source](https://github.com/ffelten/CrazyRL).
+    """
 
     metadata = {"render_modes": ["human"], "name": "escort_v0", "is_parallelizable": True, "render_fps": FPS}
 
     def __init__(self, *args, num_intermediate_points: int = 50, final_target_location=np.array([-2, -2, 3]), **kwargs):
         """Escort environment in CrazyRL.
 
         Args:
             render_mode (str, optional): The mode to display the rendering of the environment. Can be human or None.
             size (int, optional): Size of the area sides
-            num_drones: amount of drones
-            init_flying_pos: 2d array containing the coordinates of the agents
+            num_drones (int, optional): amount of drones
+            init_flying_pos (nparray[float], optional): 2d array containing the coordinates of the agents
                 is a (3)-shaped array containing the initial XYZ position of the drones.
-            init_target_location: A (3)-shaped array for the XYZ position of the target.
-            final_target_location: Array of the final position of the moving target
-            num_intermediate_points: Number of intermediate points in the target trajectory
+            init_target_location (nparray[float], optional): A (3)-shaped array for the XYZ position of the target.
+            final_target_location (nparray[float], optional): Array of the final position of the moving target
+            num_intermediate_points (int, optional): Number of intermediate points in the target trajectory
         """
-        self.final_target_location = final_target_location
-
+        EzPickle.__init__(
+            self, *args, num_intermediate_points=num_intermediate_points, final_target_location=final_target_location, **kwargs
+        )
         super().__init__(*args, **kwargs)
+        self.final_target_location = final_target_location
 
         # There are two more ref points than intermediate points, one for the initial and final target locations
         self.num_ref_points = num_intermediate_points + 2
         # Ref is a 2d arrays for the target
         # it contains the reference points (xyz) for the target at each timestep
         self.ref: np.ndarray = np.array([self.init_target_location])
```

### Comparing `momaland-0.0.2/momaland/envs/crazyrl/gl_utils.py` & `momaland-0.1.0/momaland/envs/crazyrl/gl_utils.py`

 * *Files identical despite different names*

### Comparing `momaland-0.0.2/momaland/envs/item_gathering/__init__.py` & `momaland-0.1.0/momaland/envs/item_gathering/__init__.py`

 * *Files identical despite different names*

### Comparing `momaland-0.0.2/momaland/envs/item_gathering/asset_utils.py` & `momaland-0.1.0/momaland/envs/item_gathering/asset_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """disgracefully stolen.
 
 https://stackoverflow.com/questions/73956440/python-to-change-image-into-a-color-that-is-not-one-of-the-images-dominant-colo
 """
 
 import os
+import shutil
 
 import numpy as np
 from PIL import Image
 
 
 def get_colored(asset: str, count: int):
     """Generating random colored visual assets for dynamic environment variables.
@@ -16,39 +17,30 @@
         asset: `str` value. Either "item" or "agent".
         count: `int` value. The amount of total agents/items in the environment.
 
     Returns:
         numpy.ndarray with RGB values for the new colored assets.
     """
     assert asset == "item" or asset == "agent", "You must specify an asset to get colored versions of."
-
     path = os.path.dirname(os.path.realpath(__file__))
     seed = 1 if asset == "item" else 2
     rng = np.random.default_rng(seed)  # local seed
     im = Image.open(f"{path}/assets/{asset}.png").convert("RGBA")
     alpha = im.getchannel("A")
     im = im.convert("RGB")
 
     for i in range(count - 1):  # subtracting the default asset
         rgb = rng.random((3, 3))
         matrix = (rgb[0, 0], rgb[1, 0], rgb[2, 0], 0, rgb[0, 1], rgb[1, 1], rgb[2, 1], 0, rgb[0, 2], rgb[1, 2], rgb[2, 2], 0)
 
         # Apply above transform, reinsert alpha and save
         colored_im = im.convert("RGB", matrix)
         colored_im.putalpha(alpha)
+        if not os.path.isdir(f"{path}/assets/colored/"):
+            os.mkdir(f"{path}/assets/colored/")
         colored_im.save(f"{path}/assets/colored/{asset}{i}.png")
 
 
-def del_colored(asset: str, count: int):
-    """Deleting the previously random colored visual assets.
-
-    Args:
-        asset: `str` value. Either "item" or "agent".
-        count: `int` value. The amount of total agents/items in the environment.
-
-    """
-    assert asset == "item" or asset == "agent", "You must specify an asset to delete colored versions of."
-
+def del_colored():
+    """Deleting the previously random colored visual assets."""
     path = os.path.dirname(os.path.realpath(__file__))
-
-    for i in range(count - 1):  # subtracting the default asset
-        os.remove(f"{path}/assets/colored/{asset}{i}.png")
+    shutil.rmtree(f"{path}/assets/colored/")  # deletes the leaf directory and its content
```

### Comparing `momaland-0.0.2/momaland/envs/item_gathering/item_gathering.py` & `momaland-0.1.0/momaland/envs/item_gathering/item_gathering.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,32 +10,30 @@
      2 for the other agents) or items (3, 4, etc., depending on the number of items).
     - The number of agents and items is configurable, by providing an initial map.
     - If no initial map is provided, the environment uses a default map
 
 Central observation:
     - If the central_observation flag is set to True, then the environment implements:
         - a central observation space: self.central_observation_space
-        - a central observation function: self.central_observation()
+        - a central observation function: self.state()
 """
 
-import functools
 import random
 from copy import deepcopy
 from os import path
-
-# from gymnasium.utils import EzPickle
 from typing_extensions import override
 
 import numpy as np
 import pygame
 from gymnasium.logger import warn
 from gymnasium.spaces import Box, Discrete, Tuple
+from gymnasium.utils import EzPickle
 from pettingzoo.utils import wrappers
 
-from momaland.envs.item_gathering.asset_utils import del_colored, get_colored
+from momaland.envs.item_gathering.asset_utils import get_colored
 from momaland.envs.item_gathering.map_utils import DEFAULT_MAP, randomise_map
 from momaland.utils.conversions import mo_parallel_to_aec
 from momaland.utils.env import MOParallelEnv
 
 
 ACTIONS = {
     0: np.array([0, 0], dtype=np.int32),  # stay
@@ -56,42 +54,67 @@
 
     Args:
         **kwargs: keyword args to forward to the parallel_env function
 
     Returns:
         A fully wrapped env
     """
-    env = parallel_env(**kwargs)
+    env = raw_env(**kwargs)
     env = mo_parallel_to_aec(env)
 
     # this wrapper helps error handling for discrete action spaces
     env = wrappers.AssertOutOfBoundsWrapper(env)
     return env
 
 
 def raw_env(**kwargs):
     """Env factory function for the item gathering problem."""
     return MOItemGathering(**kwargs)
 
 
-class MOItemGathering(MOParallelEnv):
-    """Environment for the Item Gathering domain.
+class MOItemGathering(MOParallelEnv, EzPickle):
+    """A `Parallel` multi-objective environment of the Item Gathering problem.
 
-    The init method takes in environment arguments and should define the following attributes:
-    - possible_agents
-    - action_spaces
-    - observation_spaces
-    These attributes should not be changed after initialization.
+    ## Observation Space
+    The observation space is a tuple containing the agent id (a negative integer) and the 2D map observation, where
+    0 is an empty cell, negative integers represent agent IDs, and positive integers represent items
+
+    ## Action Space
+    The action space is a Discrete space, where:
+    -   0: stay
+    -   1: up
+    -   2: down
+    -   3: left
+    -   4: right
+
+    ## Reward Space
+    The reward space is a vector containing rewards for each type of items available in the environment
+
+    ## Starting State
+    The initial position of the agent is determined by the 1 entries of the initial map.
+
+    ## Episode Termination
+    The episode is terminated if all the items have been gathered.
+
+    ## Episode Truncation
+    The episode termination occurs if the maximum number of timesteps is reached.
+
+    ## Arguments
+    - 'num_timesteps': number of timesteps to run the environment for. Default: 10
+    - 'initial_map': map of the environment. Default: 8x8 grid, 2 agents, 3 objectives (Källström and Heintz, 2019)
+    - 'randomise': whether to randomise the map, at each episode. Default: False
+    - 'render_mode': render mode for the environment. Default: None
     """
 
     metadata = {
         "render_modes": ["human", "rgb_array"],
-        "name": "moitemgathering_v0",
-        "render_fps": 50,
+        "name": "moitem_gathering_v0",
+        "is_parallelizable": True,
         "central_observation": True,
+        "render_fps": 30,
     }
 
     def __init__(
         self,
         num_timesteps=10,
         initial_map=DEFAULT_MAP,
         randomise=False,
@@ -101,25 +124,26 @@
 
         Args:
             num_timesteps: number of timesteps to run the environment for
             initial_map: map of the environment
             randomise: whether to randomise the map, at each episode
             render_mode: render mode for the environment
         """
+        EzPickle.__init__(
+            self,
+            num_timesteps,
+            initial_map,
+            randomise,
+            render_mode,
+        )
         self.num_timesteps = num_timesteps
         self.current_timestep = 0
         self.render_mode = render_mode
         self.randomise = randomise
 
-        """
-        # check is the initial map has any entries equal to 2
-        assert (
-            len(np.argwhere(initial_map == 2).flatten()) == 0
-        ), "Initial map cannot contain any 2s. That values is reserved for other agents, in the observation space."
-        """
         # check if the initial map has any entries equal to 1
         assert len(np.argwhere(initial_map == 1).flatten()) > 0, "The initial map does not contain any agents (1s)."
         self.initial_map = initial_map
 
         # self.env_map is the working copy used in each episode. self.initial_map should not be modified.
         self.agent_positions, self.env_map = self._init_map_and_positions(deepcopy(self.initial_map))
 
@@ -142,15 +166,15 @@
 
         assert len(item_counts) > 0, "There are no resources in the map."
 
         self.action_spaces = dict(zip(self.agents, [Discrete(len(ACTIONS))] * len(self.agent_positions)))
 
         # observations are a tuple of agent id (in the map) and the map observation
         # the map observation is a 2D array of integers, where each integer represents either agents or items.
-        # 0 for empty, 1 for the current agent, 2 for other agents, 3 for objective 1, 4 for objective 2, ...
+        # 0 for empty, negative integers for agents, positive integers for items
         self.observation_spaces = dict(
             zip(
                 self.agents,
                 [
                     Tuple(
                         (
                             Discrete(len(self.possible_agents), start=-(len(self.possible_agents))),
@@ -166,15 +190,15 @@
                 * len(self.agent_positions),
             )
         )
 
         self.central_observation_space = Box(
             low=-(len(self.possible_agents)),
             high=self.num_objectives,
-            shape=self.env_map.shape,
+            shape=self.env_map.flatten().shape,
             dtype=np.int64,
         )
 
         self.reward_spaces = dict(
             zip(self.agents, [Box(low=0, high=max(item_counts), shape=(self.num_objectives,))] * len(self.agent_positions))
         )
 
@@ -187,32 +211,28 @@
         )
         self.clock = None
         self.agent_imgs = []
         self.item_imgs = []
         self.map_bg_imgs = []
         self.window = None
 
-    # this cache ensures that same space object is returned for the same agent
-    # allows action space seeding to work as expected
-    @functools.lru_cache(maxsize=None)
     @override
     def observation_space(self, agent):
         # gymnasium spaces are defined and documented here: https://gymnasiuspspom.farama.org/api/spaces/
         return self.observation_spaces[agent]
 
-    @functools.lru_cache(maxsize=None)
     @override
     def action_space(self, agent):
         return self.action_spaces[agent]
 
     @override
     def reward_space(self, agent):
         return self.reward_spaces[agent]
 
-    def central_observation_space(self):
+    def get_central_observation_space(self):
         """Returns the central observation space."""
         return self.central_observation_space
 
     @override
     def render(self):
         if self.render_mode is None:
             warn("You are calling render method without specifying any render mode.")
@@ -280,18 +300,18 @@
             pygame.display.update()
             self.clock.tick(self.metadata["render_fps"])
         elif self.render_mode == "rgb_array":  # rgb_array
             return np.transpose(np.array(pygame.surfarray.pixels3d(self.window)), axes=(1, 0, 2))
 
     @override
     def close(self):
-        if self.render_mode is not None:
-            del_colored("item", len(self.item_dict))
-            del_colored("agent", len(self.possible_agents))
         pass
+        # This breaks the pickle tests
+        # if self.render_mode is not None:
+        #     del_colored()
 
     @override
     def reset(self, seed=None, options=None):
         if seed is not None:
             np.random.seed(seed)
             random.seed(seed)
         self.agents = self.possible_agents[:]
@@ -302,15 +322,15 @@
         if self.randomise:
             self.env_map = randomise_map(deepcopy(self.initial_map))
         else:
             self.env_map = deepcopy(self.initial_map)
 
         self.agent_positions, self.env_map = self._init_map_and_positions(self.env_map)
 
-        map_obs = self.central_observation()
+        map_obs = self.state()
         # observations are a tuple of agent id (in the map) and the map observation
         observations = {agent: (-(i + 1), map_obs) for i, agent in enumerate(self.agents)}
         self.time_num = 0
 
         infos = {agent: {} for agent in self.agents}
         return observations, infos
 
@@ -349,56 +369,57 @@
                 new_positions[i] = new_position
 
         # Check for collisions, resolve here only the collision, have final new position list at end
         collisions = []
         # initial collision check, verify all agent pairs
         new_positions, collisions = self._verify_collisions(collisions, new_positions)
 
-        max_collisions = self.num_agents * 10
+        max_collisions = self.num_agents * 50
         while len(collisions) > 0 and max_collisions > 0:
             new_positions, collisions = self._verify_collisions(collisions, new_positions)
             max_collisions -= 1
         assert collisions == [], "Collision resolution failed"
 
         # update the agent positions now that all collisions are resolved
         self.agent_positions = deepcopy(new_positions)
 
         # initialise rewards and observations
         rewards = {agent: np.array(np.zeros(self.num_objectives)) for agent in self.agents}
 
         # update all reward vectors with collected items (if any), delete items from the map
         for i in range(len(self.agent_positions)):
             value_in_cell = self.env_map[self.agent_positions[i][0], self.agent_positions[i][1]]
-            if value_in_cell > len(self.possible_agents):
+            if value_in_cell > 0:
                 rewards[self.agents[i]][self.item_dict[value_in_cell]] += 1
                 self.env_map[self.agent_positions[i][0], self.agent_positions[i][1]] = 0
 
-        map_obs = self.central_observation()
+        map_obs = self.state()
         observations = {agent: (-(i + 1), map_obs) for i, agent in enumerate(self.agents)}
 
         # typically there won't be any information in the infos, but there must
         # still be an entry for each agent
         infos = {agent: {} for agent in self.agents}
 
-        # environment termination, after all timesteps are exhausted or all items or gathered
+        # termination occurs when all items or gathered
+        # truncation occurs if all timesteps are exhausted
         self.time_num += 1
         env_termination = bool(np.sum(self.env_map) == 0)
         env_truncation = bool(self.time_num >= self.num_timesteps)
         self.terminations = {agent: env_termination for agent in self.agents}
         self.truncations = {agent: env_truncation for agent in self.agents}
         if env_termination or env_truncation:
             self.agents = []
 
         if self.render_mode == "human":
             self.render()
 
         return observations, rewards, self.truncations, self.terminations, infos
 
-    def central_observation(self):
-        """Function to create the observation passed to each agent at the end of a timestep.
+    def state(self):
+        """Returns the global observation of the map passed to each agent at the end of a timestep.
 
         Returns: a 2D Numpy array with the following items encoded:
         - 0 is empty space
         - -1, -2, -3 ... denote the positions of the agents with the specified -(agent_id+1)
         - 1, 2, 3 ... denote the locations of items representing different objectives
         """
         map_obs = deepcopy(self.env_map)
```

### Comparing `momaland-0.0.2/momaland/envs/item_gathering/map_utils.py` & `momaland-0.1.0/momaland/envs/item_gathering/map_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,43 +13,49 @@
         [0, 0, 3, 3, 0, 5, 0, 0],
         [0, 0, 0, 0, 0, 0, 0, 0],
         [1, 0, 0, 0, 0, 0, 0, 0],
     ]
 )
 
 
-def randomise_map(env_map):
+def randomise_map(env_map, seed=None):
     """Randomize the interior of the map (only the item positions).
 
     Args:
         env_map (np.ndarray): The map to randomize.
+        seed (int, optional): The seed to use for the randomization. Defaults to None.
 
     Returns:
         np.ndarray: The randomized map.
     """
+    if seed is not None:
+        np.random.seed(seed)
     interior_map = env_map[2:-2, 2:-2]
     # shuffle row-wise
     interior_map = np.random.permutation(interior_map)
     # shuffle column-wise
     interior_map = np.random.permutation(interior_map.transpose()).transpose()
     env_map[2:-2, 2:-2] = interior_map
     return env_map
 
 
-def generate_map(rows=8, columns=8, item_distribution=(3, 3, 2), num_agents=2):
+def generate_map(rows=8, columns=8, item_distribution=(3, 3, 2), num_agents=2, seed=None):
     """Generate a map for the Item Gathering environment, according to the original paper.
 
     Items are only generated in the interior of the map, i.e., not in the 2 outermost layers of the map.
 
     Args:
         rows (int, optional): The number of rows in the map. Defaults to 8.
         columns (int, optional): The number of columns in the map. Defaults to 8.
         item_distribution (tuple, optional): The number of items of each type to place in the map. Defaults to (3, 3, 2).
         num_agents (int, optional): The number of agents to place in the map. Defaults to 2.
+        seed (int, optional): The seed to use for the randomization. Defaults to None.
     """
+    if seed is not None:
+        np.random.seed(seed)
     map = np.zeros((rows, columns), dtype=int)
     interior_map = map[2:-2, 2:-2]
     item_index_start = 2
     for item in item_distribution:
         for i in range(item):
             empty_locations = np.argwhere(interior_map == 0)
             assert empty_locations.shape[0] > 0, "Not enough empty locations to place items"
```

### Comparing `momaland-0.0.2/momaland/envs/multiwalker/multiwalker_base.py` & `momaland-0.1.0/momaland/envs/multiwalker_stability/momultiwalker_stability_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     BipedalWalker as pz_bipedalwalker,
 )
 from pettingzoo.sisl.multiwalker.multiwalker_base import (
     MultiWalkerEnv as pz_multiwalker_base,
 )
 
 
-class MOBipedalWalker(pz_bipedalwalker):
+class MOBipedalWalkerStability(pz_bipedalwalker):
     """Walker Object with the physics implemented."""
 
     @override
     def __init__(
         self,
         world,
         forward_reward,
@@ -50,31 +50,28 @@
         self.fall_reward = fall_reward
         self.terminate_reward = terminate_reward
         self.terrain_length = terrain_length
         self.terrain_step = terrain_step
 
     @property
     def reward_space(self):
-        """Reward space shape = 3 element 1D array, each element representing 1 objective.
+        """Reward space shape = 2 element 1D array, each element representing 1 objective.
 
-        1. package moving forward.
-        2. no walkers falling.
-        3. package not falling.
+        1. package moving forward + no walkers falling + package not falling
+        2. package not tipping  + no walkers falling + package not falling
         """
         return spaces.Box(
-            low=np.array(
-                [-(self.terrain_step * self.forward_reward), self.fall_reward + self.terminate_reward, self.terminate_reward]
-            ),
-            high=np.array([self.terrain_step * self.forward_reward, 0, 0]),
-            shape=(3,),
+            low=np.array([-210, -0.01567]),
+            high=np.array([-210 + 0.46, 0]),
+            shape=(2,),
             dtype=np.float32,
         )
 
 
-class MOMultiWalkerEnv(pz_multiwalker_base):
+class MOMultiWalkerStabilityEnv(pz_multiwalker_base):
     """Multiwalker problem domain environment engine.
 
     Deals with the simulation of the environment.
     """
 
     @override
     def __init__(
@@ -103,39 +100,44 @@
             terminate_on_fall=terminate_on_fall,
             remove_on_fall=remove_on_fall,
             terrain_length=terrain_length,
             max_cycles=max_cycles,
             render_mode=render_mode,
         )
         self.setup()
-        self.last_rewards = [np.zeros(shape=(3,), dtype=np.float32) for _ in range(self.n_walkers)]
+        self.last_rewards = [np.zeros(shape=(2,), dtype=np.float32) for _ in range(self.n_walkers)]
 
     @override
     def setup(self):
         """Continuation of the `__init__`."""
         super().setup()
         init_y = TERRAIN_HEIGHT + 2 * LEG_H
         self.walkers = [
-            MOBipedalWalker(
+            MOBipedalWalkerStability(
                 self.world,
                 self.forward_reward,
                 self.fall_reward,
                 self.terminate_reward,
                 init_x=sx,
                 init_y=init_y,
                 seed=self.seed_val,
             )
             for sx in self.start_x
         ]
         self.reward_space = [agent.reward_space for agent in self.walkers]
 
     @override
+    def _generate_package(self):
+        super()._generate_package()
+        self.previous_pkg_angle = self.package.angle  # to init this value
+
+    @override
     def reset(self):
         obs = super().reset()
-        self.last_rewards = [np.zeros(shape=(3,), dtype=np.float32) for _ in range(self.n_walkers)]
+        self.last_rewards = [np.zeros(shape=(2,), dtype=np.float32) for _ in range(self.n_walkers)]
         return obs
 
     @override
     def step(self, action, agent_id, is_last):
         # action is array of size 4
         action = action.reshape(4)
         assert self.walkers[agent_id].hull is not None, agent_id
@@ -153,20 +155,20 @@
         if self.render_mode == "human":
             self.render()
 
     @override
     def scroll_subroutine(self):
         """This is the step engine of the environment.
 
-        Here we have vectorized the reward math from the PettingZoo env to be multi-objective.
+        Here we have vectorized the reward by adding the stability objective to each agent's reward.
         """
         xpos = np.zeros(self.n_walkers)
         obs = []
         done = False
-        rewards = np.array([np.zeros(shape=(3,), dtype=np.float32) for _ in range(self.n_walkers)])
+        rewards = np.array([np.zeros(shape=(2,), dtype=np.float32) for _ in range(self.n_walkers)])
 
         for i in range(self.n_walkers):
             if self.walkers[i].hull is None:
                 obs.append(np.zeros_like(self.observation_space[i].low))
                 continue
             pos = self.walkers[i].hull.position
             x, y = pos.x, pos.y
@@ -187,35 +189,39 @@
             xd = (self.package.position.x - x) / self.package_length
             yd = (self.package.position.y - y) / self.package_length
             neighbor_obs.append(self.np_random.normal(xd, self.position_noise))
             neighbor_obs.append(self.np_random.normal(yd, self.position_noise))
             neighbor_obs.append(self.np_random.normal(self.package.angle, self.angle_noise))
             obs.append(np.array(walker_obs + neighbor_obs))
 
-        # Below this point is the MO reward computation. Above this point is the original PZ code.
-        package_shaping = self.forward_reward * self.package.position.x
+            shaping = -5.0 * abs(walker_obs[0])
+            rewards[i, 0] = shaping - self.prev_shaping[i]
+            self.prev_shaping[i] = shaping
+
+        package_shaping = self.forward_reward * 130 * self.package.position.x / SCALE
         rewards[:, 0] = package_shaping - self.prev_package_shaping  # obj1: move forward
         self.prev_package_shaping = package_shaping
 
+        # obj 2: package stability
+        pkg_angle_delta = abs(self.previous_pkg_angle - self.package.angle)
+        rewards[:, 1] = -pkg_angle_delta
+        self.previous_pkg_angle = self.package.angle
+
         self.scroll = xpos.mean() - VIEWPORT_W / SCALE / 5 - (self.n_walkers - 1) * WALKER_SEPERATION * TERRAIN_STEP
 
+        # fall
         done = [False] * self.n_walkers
         for i, (fallen, walker) in enumerate(zip(self.fallen_walkers, self.walkers)):
-            if fallen:  # obj2: agent does not fall
-                rewards[i, 1] = self.fall_reward  # not all, only the one that fell
+            if fallen:
+                rewards[i, :] += self.fall_reward
                 if self.remove_on_fall:
                     walker._destroy()
-                if self.terminate_on_fall:
-                    rewards[:, 1] += self.terminate_reward
+                if not self.terminate_on_fall:
+                    rewards[i, :] += self.terminate_reward
                 done[i] = True
-
-        if self.terminate_on_fall and np.sum(self.fallen_walkers) > 0:  # terminate_on_fall global termination
-            done = [True] * self.n_walkers
-
-        if self.game_over or self.package.position.x < 0:  # obj3: package doesn't fall
+        if (self.terminate_on_fall and np.sum(self.fallen_walkers) > 0) or self.game_over or self.package.position.x < 0:
+            rewards[:, :] += self.terminate_reward
             done = [True] * self.n_walkers
-            rewards[:, 2] = self.terminate_reward
-
         elif self.package.position.x > (self.terrain_length - TERRAIN_GRASS) * TERRAIN_STEP:
             done = [True] * self.n_walkers
 
         return rewards, done, obs
```

### Comparing `momaland-0.0.2/momaland/test/api_test.py` & `momaland-0.1.0/momaland/test/api_test.py`

 * *Files identical despite different names*

### Comparing `momaland-0.0.2/momaland/test/wrapper_test.py` & `momaland-0.1.0/momaland/test/wrapper_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -83,14 +83,30 @@
     observations, infos = env.reset(seed=42)
     while env.agents:
         actions = {agent: env.action_space(agent).sample() for agent in env.agents}
         observations, rewards, terminations, truncations, infos = env.step(actions)
     env.close()
 
 
+def parallel_centralized_agent_test(env_module):
+    """Soft test unit. No assertions.
+
+    This test unit is used to check if the API breaks when the central agent wrapper is applied.
+    """
+    env = env_module.parallel_env()
+    env = ParallelWrappers.CentraliseAgent(env)
+    observation, info = env.reset(seed=42)
+    done = False
+    while done:
+        actions = {agent: env.action_space[agent].sample() for agent in env.agents}
+        observation, reward, truncation, termination, info = env.step(actions)
+        done = truncation or termination
+    env.close()
+
+
 def aec_test(env_module):
     """Testing for the following wrappers for AEC:
     - Normalization
     - Linear Scalarization
     """
     aec_normalization_test(env_module)
     aec_linearization_test(env_module)
@@ -103,11 +119,18 @@
     - Linear Scalarization
     """
     parallel_normalization_test(env_module)
     parallel_linearization_test(env_module)
     print("Passed Parallel wrapper test")
 
 
+def central_agent_test(env_module):
+    """Testing for the CentralisedAgent wrapper for Parallel."""
+    parallel_centralized_agent_test(env_module)
+    print("Passed Centralized Agent Parallel wrapper test")
+
+
 def wrapper_test(env_module):
     """Wrapper testing for AEC and Parallel environments."""
     aec_test(env_module)
     parallel_test(env_module)
+    central_agent_test(env_module)
```

### Comparing `momaland-0.0.2/momaland/utils/aec_wrappers.py` & `momaland-0.1.0/momaland/utils/aec_wrappers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,57 @@
 """Various wrappers for AEC MO environments."""
+from typing import Optional
 
 import numpy as np
 from gymnasium.wrappers.normalize import RunningMeanStd
 from pettingzoo.utils.wrappers.base import BaseWrapper
 
 
+class RecordEpisodeStatistics(BaseWrapper):
+    """This wrapper will record episode statistics and print them at the end of each episode."""
+
+    def __init__(self, env):
+        """This wrapper will record episode statistics and print them at the end of each episode.
+
+        Args:
+            env (env): The environment to apply the wrapper
+        """
+        BaseWrapper.__init__(self, env)
+        self.episode_rewards = {agent: 0 for agent in self.possible_agents}
+        self.episode_lengths = {agent: 0 for agent in self.possible_agents}
+
+    def last(self, observe: bool = True):
+        """Receives the latest observation from the environment, recording episode statistics."""
+        obs, rews, terminated, truncated, infos = super().last(observe=observe)
+        for agent in self.env.possible_agents:
+            self.episode_rewards[agent] += rews
+            self.episode_lengths[agent] += 1
+        if terminated or truncated:
+            infos["episode"] = {
+                "r": self.episode_rewards,
+                "l": self.episode_lengths,
+            }
+        return obs, rews, terminated, truncated, infos
+
+    def reset(self, seed: Optional[int] = None, options: Optional[dict] = None):
+        """Resets the environment and the episode statistics."""
+        super().reset(seed, options)
+        for agent in self.env.possible_agents:
+            self.episode_rewards[agent] = 0
+            self.episode_lengths[agent] = 0
+
+
 class LinearizeReward(BaseWrapper):
     """Convert MO reward vector into scalar SO reward value.
 
     `weights` represents the weights of each objective in the reward vector space for each agent.
 
     Example:
-    >>> weights = {"agent_0": np.array([0.1, 0.9]), "agent_1": np.array([0.2, 0.8]}
-    >>> env = LinearizeReward(env, weights)
+        >>> weights = {"agent_0": np.array([0.1, 0.9]), "agent_1": np.array([0.2, 0.8]}
+        ... env = LinearizeReward(env, weights)
     """
 
     def __init__(self, env, weights: dict):
         """Reward linearization class initializer.
 
         Args:
             env: base env to add the wrapper on.
@@ -39,17 +74,17 @@
     The exponential moving average will have variance :math:`(1 - \gamma)^2`.
 
     Note:
         The scaling depends on past trajectories and rewards will not be scaled correctly if the wrapper was newly
         instantiated or the policy was changed recently.
 
     Example:
-    >>> for agent in env.possible_agents:
-    >>>     for idx in range(env.reward_space(agent).shape[0]):
-    >>>         env = AECWrappers.NormalizeReward(env, agent, idx)
+        >>> for agent in env.possible_agents:
+        ...     for idx in range(env.reward_space(agent).shape[0]):
+        ...         env = AECWrappers.NormalizeReward(env, agent, idx)
     """
 
     def __init__(
         self,
         env,
         agent,
         idx,
```

### Comparing `momaland-0.0.2/momaland/utils/all_modules.py` & `momaland-0.1.0/momaland/utils/all_modules.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 """Environment registry.
 
 Used for:
 - testing
 - rendering GIF images
 """
 
-from momaland.envs.beach_domain import mobeach_v0
-from momaland.envs.congestion_game import mocongestion_v0
+from momaland.envs.beach import mobeach_v0
+from momaland.envs.breakthrough import mobreakthrough_v0
+from momaland.envs.congestion import mocongestion_v0
+from momaland.envs.connect4 import moconnect4_v0
 from momaland.envs.crazyrl.catch import catch_v0
 from momaland.envs.crazyrl.escort import escort_v0
 from momaland.envs.crazyrl.surround import surround_v0
-from momaland.envs.item_gathering import moitemgathering_v0
-from momaland.envs.multiwalker import momultiwalker_v0
+from momaland.envs.gem_mining import mogem_mining_v0
+from momaland.envs.ingenious import moingenious_v0
+from momaland.envs.item_gathering import moitem_gathering_v0
+from momaland.envs.multiwalker_stability import momultiwalker_stability_v0
 from momaland.envs.pistonball import mopistonball_v0
+from momaland.envs.samegame import mosame_game_v0
 
 
 all_environments = {
     "mobeach_v0": mobeach_v0,
-    "momultiwalker_v0": momultiwalker_v0,
+    "momultiwalker_stability_v0": momultiwalker_stability_v0,
     "catch_v0": catch_v0,
     "surround_v0": surround_v0,
     "escort_v0": escort_v0,
-    "moitemgathering_v0": moitemgathering_v0,
+    "moitem_gathering_v0": moitem_gathering_v0,
+    "moingenious_v0": moingenious_v0,
     "mopistonball_v0": mopistonball_v0,
     "mocongestion_v0": mocongestion_v0,
+    "moconnect4_v0": moconnect4_v0,
+    "mobreakthrough_v0": mobreakthrough_v0,
+    "mosame_game_v0": mosame_game_v0,
+    "mogem_mining_v0": mogem_mining_v0,
 }
```

### Comparing `momaland-0.0.2/momaland/utils/conversions.py` & `momaland-0.1.0/momaland/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `momaland-0.0.2/momaland/utils/env.py` & `momaland-0.1.0/momaland/utils/env.py`

 * *Files identical despite different names*

### Comparing `momaland-0.0.2/momaland/utils/generate_gif_image.py` & `momaland-0.1.0/momaland/utils/generate_gif_image.py`

 * *Files identical despite different names*

### Comparing `momaland-0.0.2/setup.py` & `momaland-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `momaland-0.0.2/tests/test_envs.py` & `momaland-0.1.0/tests/test_envs.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 
 @pytest.mark.parametrize(("name", "env_module"), list(all_environments.items()))
 def test_module(name, env_module):
     _env = env_module.env(render_mode=None)
     assert str(_env) == os.path.basename(name)
     api_test(_env)
-    parallel_api_test(env_module.parallel_env())
+    if _env.metadata["is_parallelizable"]:
+        parallel_api_test(env_module.parallel_env())
     # wrapper_test(env_module): TODO: There are some problems with the NormalizeReward wrapper.
     seed_test(env_module.env, 50)
 
     # TODO render_test(env_module.env)
     # TODO max_cycles_test(env_module)
 
     recreated_env = pickle.loads(pickle.dumps(_env))
```


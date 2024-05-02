# Comparing `tmp/reponews-0.4.0.tar.gz` & `tmp/reponews-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reponews-0.4.0.tar", last modified: Tue Oct 31 16:49:12 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `reponews-0.4.0.tar` & `reponews-0.5.0.tar`

### file list

```diff
@@ -1,83 +1,65 @@
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-31 16:49:12.052916 reponews-0.4.0/
--rw-r--r--   0 jwodder    (501) staff       (20)     1099 2023-10-31 16:49:05.000000 reponews-0.4.0/CHANGELOG.md
--rw-r--r--   0 jwodder    (501) staff       (20)     1095 2023-10-31 16:49:05.000000 reponews-0.4.0/LICENSE
--rw-r--r--   0 jwodder    (501) staff       (20)      126 2021-11-13 01:54:07.000000 reponews-0.4.0/MANIFEST.in
--rw-r--r--   0 jwodder    (501) staff       (20)    18451 2023-10-31 16:49:12.052615 reponews-0.4.0/PKG-INFO
--rw-r--r--   0 jwodder    (501) staff       (20)    16689 2023-10-31 16:47:20.000000 reponews-0.4.0/README.rst
--rw-r--r--   0 jwodder    (501) staff       (20)       91 2022-07-07 12:48:58.000000 reponews-0.4.0/pyproject.toml
--rw-r--r--   0 jwodder    (501) staff       (20)     2252 2023-10-31 16:49:12.054051 reponews-0.4.0/setup.cfg
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-31 16:49:11.990488 reponews-0.4.0/src/
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-31 16:49:11.999570 reponews-0.4.0/src/reponews/
--rw-r--r--   0 jwodder    (501) staff       (20)     1018 2023-10-31 16:49:05.000000 reponews-0.4.0/src/reponews/__init__.py
--rw-r--r--   0 jwodder    (501) staff       (20)     3823 2023-10-30 21:44:12.000000 reponews-0.4.0/src/reponews/__main__.py
--rw-r--r--   0 jwodder    (501) staff       (20)     5496 2023-10-31 16:47:20.000000 reponews-0.4.0/src/reponews/client.py
--rw-r--r--   0 jwodder    (501) staff       (20)     9463 2023-10-31 16:47:20.000000 reponews-0.4.0/src/reponews/config.py
--rw-r--r--   0 jwodder    (501) staff       (20)     8395 2023-10-31 16:47:20.000000 reponews-0.4.0/src/reponews/core.py
--rw-r--r--   0 jwodder    (501) staff       (20)        0 2021-11-13 01:54:07.000000 reponews-0.4.0/src/reponews/py.typed
--rw-r--r--   0 jwodder    (501) staff       (20)     4849 2023-02-20 03:04:49.000000 reponews-0.4.0/src/reponews/qlobjs.py
--rw-r--r--   0 jwodder    (501) staff       (20)     6840 2023-10-31 16:47:20.000000 reponews-0.4.0/src/reponews/qmanager.py
--rw-r--r--   0 jwodder    (501) staff       (20)    10308 2023-10-31 16:47:20.000000 reponews-0.4.0/src/reponews/types.py
--rw-r--r--   0 jwodder    (501) staff       (20)     1077 2023-10-31 16:47:20.000000 reponews-0.4.0/src/reponews/util.py
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-31 16:49:12.003255 reponews-0.4.0/src/reponews.egg-info/
--rw-r--r--   0 jwodder    (501) staff       (20)    18451 2023-10-31 16:49:11.000000 reponews-0.4.0/src/reponews.egg-info/PKG-INFO
--rw-r--r--   0 jwodder    (501) staff       (20)     2138 2023-10-31 16:49:11.000000 reponews-0.4.0/src/reponews.egg-info/SOURCES.txt
--rw-r--r--   0 jwodder    (501) staff       (20)        1 2023-10-31 16:49:11.000000 reponews-0.4.0/src/reponews.egg-info/dependency_links.txt
--rw-r--r--   0 jwodder    (501) staff       (20)       52 2023-10-31 16:49:11.000000 reponews-0.4.0/src/reponews.egg-info/entry_points.txt
--rw-r--r--   0 jwodder    (501) staff       (20)      258 2023-10-31 16:49:11.000000 reponews-0.4.0/src/reponews.egg-info/requires.txt
--rw-r--r--   0 jwodder    (501) staff       (20)        9 2023-10-31 16:49:11.000000 reponews-0.4.0/src/reponews.egg-info/top_level.txt
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-31 16:49:12.008822 reponews-0.4.0/test/
--rw-r--r--   0 jwodder    (501) staff       (20)      645 2021-11-29 16:59:39.000000 reponews-0.4.0/test/conftest.py
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-31 16:49:11.991340 reponews-0.4.0/test/data/
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-31 16:49:12.018311 reponews-0.4.0/test/data/bad-config/
--rw-r--r--   0 jwodder    (501) staff       (20)       28 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/bad-config/bad-address01.toml
--rw-r--r--   0 jwodder    (501) staff       (20)       38 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/bad-config/bad-address02.toml
--rw-r--r--   0 jwodder    (501) staff       (20)       57 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/bad-config/bad-address03.toml
--rw-r--r--   0 jwodder    (501) staff       (20)       60 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/bad-config/bad-address04.toml
--rw-r--r--   0 jwodder    (501) staff       (20)       38 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/bad-config/bad-include.toml
--rw-r--r--   0 jwodder    (501) staff       (20)       47 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/bad-config/bad-pref-spec01.toml
--rw-r--r--   0 jwodder    (501) staff       (20)       51 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/bad-config/bad-pref-spec02.toml
--rw-r--r--   0 jwodder    (501) staff       (20)       51 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/bad-config/bad-pref-spec03.toml
--rw-r--r--   0 jwodder    (501) staff       (20)       24 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/bad-config/unknown-key.toml
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-31 16:49:12.029949 reponews-0.4.0/test/data/config/
--rw-r--r--   0 jwodder    (501) staff       (20)      973 2021-11-26 19:40:15.000000 reponews-0.4.0/test/data/config/empty.json
--rw-r--r--   0 jwodder    (501) staff       (20)        0 2021-11-19 14:51:48.000000 reponews-0.4.0/test/data/config/empty.toml
--rw-r--r--   0 jwodder    (501) staff       (20)     1285 2021-11-26 19:40:15.000000 reponews-0.4.0/test/data/config/full.json
--rw-r--r--   0 jwodder    (501) staff       (20)      464 2021-11-19 14:51:48.000000 reponews-0.4.0/test/data/config/full.toml
--rw-r--r--   0 jwodder    (501) staff       (20)     1040 2021-11-26 19:40:15.000000 reponews-0.4.0/test/data/config/minimal.json
--rw-r--r--   0 jwodder    (501) staff       (20)       69 2021-11-13 01:54:07.000000 reponews-0.4.0/test/data/config/minimal.toml
--rw-r--r--   0 jwodder    (501) staff       (20)     1015 2021-11-26 19:40:15.000000 reponews-0.4.0/test/data/config/relpaths.json
--rw-r--r--   0 jwodder    (501) staff       (20)       76 2021-11-19 14:51:48.000000 reponews-0.4.0/test/data/config/relpaths.toml
--rw-r--r--   0 jwodder    (501) staff       (20)     1753 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/config/repo-activity01.json
--rw-r--r--   0 jwodder    (501) staff       (20)      212 2021-11-26 19:40:15.000000 reponews-0.4.0/test/data/config/repo-activity01.toml
--rw-r--r--   0 jwodder    (501) staff       (20)     1756 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/config/repo-activity02.json
--rw-r--r--   0 jwodder    (501) staff       (20)      321 2021-11-26 19:40:15.000000 reponews-0.4.0/test/data/config/repo-activity02.toml
--rw-r--r--   0 jwodder    (501) staff       (20)     1037 2021-11-26 19:40:15.000000 reponews-0.4.0/test/data/config/yestags.json
--rw-r--r--   0 jwodder    (501) staff       (20)      118 2021-11-19 14:51:48.000000 reponews-0.4.0/test/data/config/yestags.toml
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-31 16:49:12.042058 reponews-0.4.0/test/data/inclusions/
--rw-r--r--   0 jwodder    (501) staff       (20)      143 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/empty.json
--rw-r--r--   0 jwodder    (501) staff       (20)        0 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/empty.toml
--rw-r--r--   0 jwodder    (501) staff       (20)      261 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/include01.json
--rw-r--r--   0 jwodder    (501) staff       (20)       64 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/include01.toml
--rw-r--r--   0 jwodder    (501) staff       (20)      237 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/include02.json
--rw-r--r--   0 jwodder    (501) staff       (20)       80 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/include02.toml
--rw-r--r--   0 jwodder    (501) staff       (20)      350 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/include03.json
--rw-r--r--   0 jwodder    (501) staff       (20)      112 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/include03.toml
--rw-r--r--   0 jwodder    (501) staff       (20)      350 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/repo-activity01.json
--rw-r--r--   0 jwodder    (501) staff       (20)      222 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/repo-activity01.toml
--rw-r--r--   0 jwodder    (501) staff       (20)      339 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/repo-activity02.json
--rw-r--r--   0 jwodder    (501) staff       (20)      254 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/repo-activity02.toml
--rw-r--r--   0 jwodder    (501) staff       (20)      228 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/repo-activity03.json
--rw-r--r--   0 jwodder    (501) staff       (20)       99 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/inclusions/repo-activity03.toml
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-31 16:49:12.047279 reponews-0.4.0/test/data/mock/
--rw-r--r--   0 jwodder    (501) staff       (20)     1223 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/mock/body.txt
--rw-r--r--   0 jwodder    (501) staff       (20)     1893 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/mock/dump-repos.txt
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-31 16:49:12.051514 reponews-0.4.0/test/data/mock/home/
--rw-r--r--   0 jwodder    (501) staff       (20)      598 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/mock/home/config.toml
--rw-r--r--   0 jwodder    (501) staff       (20)     5499 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/mock/home/state.json
--rw-r--r--   0 jwodder    (501) staff       (20)     5517 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/mock/new-state.json
--rw-r--r--   0 jwodder    (501) staff       (20)    21119 2021-11-29 16:59:39.000000 reponews-0.4.0/test/data/mock/session-data.json
--rw-r--r--   0 jwodder    (501) staff       (20)    13600 2023-10-31 16:47:20.000000 reponews-0.4.0/test/test_config.py
--rw-r--r--   0 jwodder    (501) staff       (20)     9150 2023-10-31 16:47:20.000000 reponews-0.4.0/test/test_main.py
--rw-r--r--   0 jwodder    (501) staff       (20)    82580 2023-10-30 21:40:54.000000 reponews-0.4.0/test/test_qmanager.py
--rw-r--r--   0 jwodder    (501) staff       (20)    15337 2021-11-29 16:59:39.000000 reponews-0.4.0/test/test_types.py
--rw-r--r--   0 jwodder    (501) staff       (20)     1531 2023-10-31 16:47:20.000000 reponews-0.4.0/tox.ini
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 reponews-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 reponews-0.5.0/tox.ini
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 reponews-0.5.0/src/reponews/__init__.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 reponews-0.5.0/src/reponews/__main__.py
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 reponews-0.5.0/src/reponews/client.py
+-rw-r--r--   0        0        0     9589 2020-02-02 00:00:00.000000 reponews-0.5.0/src/reponews/config.py
+-rw-r--r--   0        0        0     9020 2020-02-02 00:00:00.000000 reponews-0.5.0/src/reponews/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reponews-0.5.0/src/reponews/py.typed
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 reponews-0.5.0/src/reponews/qlobjs.py
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 reponews-0.5.0/src/reponews/qmanager.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 reponews-0.5.0/src/reponews/types.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 reponews-0.5.0/src/reponews/util.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 reponews-0.5.0/test/conftest.py
+-rw-r--r--   0        0        0    14799 2020-02-02 00:00:00.000000 reponews-0.5.0/test/test_config.py
+-rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 reponews-0.5.0/test/test_main.py
+-rw-r--r--   0        0        0    82580 2020-02-02 00:00:00.000000 reponews-0.5.0/test/test_qmanager.py
+-rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 reponews-0.5.0/test/test_types.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/bad-config/bad-address01.toml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/bad-config/bad-address02.toml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/bad-config/bad-address03.toml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/bad-config/bad-address04.toml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/bad-config/bad-include.toml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/bad-config/bad-pref-spec01.toml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/bad-config/bad-pref-spec02.toml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/bad-config/bad-pref-spec03.toml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/bad-config/unknown-key.toml
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/empty.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/empty.toml
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/full.json
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/full.toml
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/minimal.json
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/minimal.toml
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/relpaths.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/relpaths.toml
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/repo-activity01.json
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/repo-activity01.toml
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/repo-activity02.json
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/repo-activity02.toml
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/yestags.json
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/config/yestags.toml
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/empty.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/empty.toml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/include01.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/include01.toml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/include02.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/include02.toml
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/include03.json
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/include03.toml
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/repo-activity01.json
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/repo-activity01.toml
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/repo-activity02.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/repo-activity02.toml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/repo-activity03.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/inclusions/repo-activity03.toml
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/mock/body.txt
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/mock/dump-repos.txt
+-rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/mock/new-state.json
+-rw-r--r--   0        0        0    21121 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/mock/session-data.json
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/mock/home/config.toml
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 reponews-0.5.0/test/data/mock/home/state.json
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 reponews-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 reponews-0.5.0/LICENSE
+-rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 reponews-0.5.0/README.rst
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 reponews-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    19193 2020-02-02 00:00:00.000000 reponews-0.5.0/PKG-INFO
```

### Comparing `reponews-0.4.0/CHANGELOG.md` & `reponews-0.5.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v0.5.0 (2024-05-02)
+-------------------
+- Support platformdirs v4.0
+- Migrated from setuptools to hatch
+- Support configuring whether to report prereleases and/or draft releases
+
 v0.4.0 (2023-10-31)
 -------------------
 - Support python-dotenv v1.0
 - Use [`ghtoken`](https://github.com/jwodder/ghtoken) for looking up GitHub
   tokens
 - Ensure that the state file is always read & written using UTF-8 encoding
 - Always read the auth-token-file using UTF-8 encoding
```

### Comparing `reponews-0.4.0/LICENSE` & `reponews-0.5.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021-2023 John Thorvald Wodder II
+Copyright (c) 2021-2024 John Thorvald Wodder II
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `reponews-0.4.0/PKG-INFO` & `reponews-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: reponews
-Version: 0.4.0
+Version: 0.5.0
 Summary: Send e-mails about new events on your GitHub repositories
-Home-page: https://github.com/jwodder/reponews
-Author: John Thorvald Wodder II
-Author-email: reponews@varonathe.org
-License: MIT
 Project-URL: Source Code, https://github.com/jwodder/reponews
 Project-URL: Bug Tracker, https://github.com/jwodder/reponews/issues
+Author-email: John Thorvald Wodder II <reponews@varonathe.org>
+License-Expression: MIT
+License-File: LICENSE
 Keywords: GitHub,GitHub activity,GitHub issues,e-mail,notifications,pull requests
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: click>=8.0
 Requires-Dist: click-loglevel~=0.5
+Requires-Dist: click>=8.0
 Requires-Dist: eletter~=0.2
 Requires-Dist: ghrepo~=0.1
 Requires-Dist: ghtoken~=0.1
 Requires-Dist: mailbits~=0.2
 Requires-Dist: outgoing~=0.6
-Requires-Dist: platformdirs~=3.0
+Requires-Dist: platformdirs<5.0,>=3.0
 Requires-Dist: pydantic~=2.0
 Requires-Dist: python-dotenv<2.0,>=0.11
 Requires-Dist: requests~=2.20
-Requires-Dist: tomli<3.0,>=1.2; python_version < "3.11"
-Requires-Dist: typing_extensions; python_version < "3.9"
+Requires-Dist: tomli<3.0,>=1.2; python_version < '3.11'
+Requires-Dist: typing-extensions; python_version < '3.9'
+Description-Content-Type: text/x-rst
 
-.. image:: http://www.repostatus.org/badges/latest/active.svg
-    :target: http://www.repostatus.org/#active
+|repostatus| |ci-status| |coverage| |pyversions| |license|
+
+.. |repostatus| image:: https://www.repostatus.org/badges/latest/active.svg
+    :target: https://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
 
-.. image:: https://github.com/jwodder/reponews/workflows/Test/badge.svg?branch=master
-    :target: https://github.com/jwodder/reponews/actions?workflow=Test
+.. |ci-status| image:: https://github.com/jwodder/reponews/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/jwodder/reponews/actions/workflows/test.yml
     :alt: CI Status
 
-.. image:: https://codecov.io/gh/jwodder/reponews/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/jwodder/reponews/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/jwodder/reponews
 
-.. image:: https://img.shields.io/pypi/pyversions/reponews.svg
+.. |pyversions| image:: https://img.shields.io/pypi/pyversions/reponews.svg
     :target: https://pypi.org/project/reponews/
 
-.. image:: https://img.shields.io/github/license/jwodder/reponews.svg
+.. |license| image:: https://img.shields.io/github/license/jwodder/reponews.svg
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 `GitHub <https://github.com/jwodder/reponews>`_
 | `PyPI <https://pypi.org/project/reponews/>`_
 | `Issues <https://github.com/jwodder/reponews/issues>`_
 | `Changelog <https://github.com/jwodder/reponews/blob/master/CHANGELOG.md>`_
@@ -303,14 +303,27 @@
         Whether to report new `discussions`_ in tracked repositories; defaults
         to true
 
     ``releases`` : boolean
         Whether to report new releases in tracked repositories; defaults to
         true
 
+    ``prereleases`` : boolean
+        Whether to report new prereleases in tracked repositories; defaults to
+        true.  This setting only has an effect when ``releases`` is true.
+
+     ``drafts`` : boolean
+        Whether to report new draft releases in tracked repositories; defaults
+        to true.  This setting only has an effect when ``releases`` is true.
+
+        Note that, if ``reponews`` sees a release while it's in a draft state
+        (even if the draft is not reported), and then, on a later run, the
+        release has been published, the release will not be reported on the
+        later run, regardless of the value of ``drafts``.
+
     ``tags`` : boolean
         Whether to report new tags in tracked repositories; defaults to true
 
     ``released-tags`` : boolean
         This setting controls how to handle tags that are also made into
         releases when both tags and releases are being tracked.  If true, such
         tags are reported separately from the releases.  If false (the
```

### Comparing `reponews-0.4.0/README.rst` & `reponews-0.5.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-.. image:: http://www.repostatus.org/badges/latest/active.svg
-    :target: http://www.repostatus.org/#active
+|repostatus| |ci-status| |coverage| |pyversions| |license|
+
+.. |repostatus| image:: https://www.repostatus.org/badges/latest/active.svg
+    :target: https://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
 
-.. image:: https://github.com/jwodder/reponews/workflows/Test/badge.svg?branch=master
-    :target: https://github.com/jwodder/reponews/actions?workflow=Test
+.. |ci-status| image:: https://github.com/jwodder/reponews/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/jwodder/reponews/actions/workflows/test.yml
     :alt: CI Status
 
-.. image:: https://codecov.io/gh/jwodder/reponews/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/jwodder/reponews/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/jwodder/reponews
 
-.. image:: https://img.shields.io/pypi/pyversions/reponews.svg
+.. |pyversions| image:: https://img.shields.io/pypi/pyversions/reponews.svg
     :target: https://pypi.org/project/reponews/
 
-.. image:: https://img.shields.io/github/license/jwodder/reponews.svg
+.. |license| image:: https://img.shields.io/github/license/jwodder/reponews.svg
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 `GitHub <https://github.com/jwodder/reponews>`_
 | `PyPI <https://pypi.org/project/reponews/>`_
 | `Issues <https://github.com/jwodder/reponews/issues>`_
 | `Changelog <https://github.com/jwodder/reponews/blob/master/CHANGELOG.md>`_
@@ -260,14 +262,27 @@
         Whether to report new `discussions`_ in tracked repositories; defaults
         to true
 
     ``releases`` : boolean
         Whether to report new releases in tracked repositories; defaults to
         true
 
+    ``prereleases`` : boolean
+        Whether to report new prereleases in tracked repositories; defaults to
+        true.  This setting only has an effect when ``releases`` is true.
+
+     ``drafts`` : boolean
+        Whether to report new draft releases in tracked repositories; defaults
+        to true.  This setting only has an effect when ``releases`` is true.
+
+        Note that, if ``reponews`` sees a release while it's in a draft state
+        (even if the draft is not reported), and then, on a later run, the
+        release has been published, the release will not be reported on the
+        later run, regardless of the value of ``drafts``.
+
     ``tags`` : boolean
         Whether to report new tags in tracked repositories; defaults to true
 
     ``released-tags`` : boolean
         This setting controls how to handle tags that are also made into
         releases when both tags and releases are being tracked.  If true, such
         tags are reported separately from the releases.  If false (the
```

### Comparing `reponews-0.4.0/src/reponews/__init__.py` & `reponews-0.5.0/src/reponews/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 another job scheduler (sold separately), point it at a compatible e-mail
 sending service (also sold separately), and you'll get periodic e-mails listing
 new events.
 
 Visit <https://github.com/jwodder/reponews> for more information.
 """
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __author__ = "John Thorvald Wodder II"
 __author_email__ = "reponews@varonathe.org"
 __license__ = "MIT"
 __url__ = "https://github.com/jwodder/reponews"
```

### Comparing `reponews-0.4.0/src/reponews/__main__.py` & `reponews-0.5.0/src/reponews/__main__.py`

 * *Files identical despite different names*

### Comparing `reponews-0.4.0/src/reponews/client.py` & `reponews-0.5.0/src/reponews/client.py`

 * *Files identical despite different names*

### Comparing `reponews-0.4.0/src/reponews/config.py` & `reponews-0.5.0/src/reponews/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,26 +89,30 @@
 
 
 class PartialActivityPrefs(BaseConfig):
     issues: Optional[bool] = None
     pull_requests: Optional[bool] = None
     discussions: Optional[bool] = None
     releases: Optional[bool] = None
+    prereleases: Optional[bool] = None
+    drafts: Optional[bool] = None
     tags: Optional[bool] = None
     released_tags: Optional[bool] = None
     stars: Optional[bool] = None
     forks: Optional[bool] = None
     my_activity: Optional[bool] = None
 
 
 class ActivityPrefs(PartialActivityPrefs):
     issues: bool = True
     pull_requests: bool = True
     discussions: bool = True
     releases: bool = True
+    prereleases: bool = True
+    drafts: bool = True
     tags: bool = True
     released_tags: bool = False
     stars: bool = True
     forks: bool = True
     my_activity: bool = False
 
     def get_activity_types(self) -> list[ActivityType]:
```

### Comparing `reponews-0.4.0/src/reponews/core.py` & `reponews-0.5.0/src/reponews/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from types import TracebackType
 from typing import Dict
 from eletter import compose
 from pydantic import BaseModel, Field, TypeAdapter
 from . import client
 from .config import Configuration
 from .types import (
-    ActivityType,
     CursorDict,
     Event,
     NewReleaseEvent,
     NewTagEvent,
     RepoActivity,
     RepoRenamedEvent,
     Repository,
@@ -142,19 +141,28 @@
                 events2 = []
                 for ev in new_events:
                     if ev.is_mine:
                         log.info("<%s> was created by current user; not reporting", ev)
                     else:
                         events2.append(ev)
                 new_events = events2
-            if (
-                ActivityType.RELEASE in types
-                and ActivityType.TAG in types
-                and not activity.released_tags
-            ):
+            if activity.releases and (not activity.prereleases or not activity.drafts):
+                events2 = []
+                for ev in new_events:
+                    if isinstance(ev, NewReleaseEvent):
+                        if not activity.prereleases and ev.isPrerelease:
+                            log.info("<%s> is prerelease; not reporting", ev)
+                        elif not activity.drafts and ev.isDraft:
+                            log.info("<%s> is draft release; not reporting", ev)
+                        else:
+                            events2.append(ev)
+                    else:
+                        events2.append(ev)
+                new_events = events2
+            if activity.releases and activity.tags and not activity.released_tags:
                 events2 = []
                 release_tags = set()
                 tag_events: list[NewTagEvent] = []
                 for ev in new_events:
                     if isinstance(ev, NewTagEvent):
                         tag_events.append(ev)
                     else:
@@ -216,17 +224,19 @@
     def compose_email(self, events: list[Event]) -> EmailMessage:
         if self.config.recipient is None:
             raise UserError(
                 "reponews.recipient must be set when constructing an e-mail"
             )
         return compose(
             subject=self.config.subject,
-            from_=self.config.sender.as_py_address()
-            if self.config.sender is not None
-            else None,
+            from_=(
+                self.config.sender.as_py_address()
+                if self.config.sender is not None
+                else None
+            ),
             to=[self.config.recipient.as_py_address()],
             text=self.compose_email_body(events),
             headers={"User-Agent": MAIL_USER_AGENT},
         )
 
     def save_state(self) -> None:
         log.info("Saving state ...")
```

### Comparing `reponews-0.4.0/src/reponews/qlobjs.py` & `reponews-0.5.0/src/reponews/qlobjs.py`

 * *Files identical despite different names*

### Comparing `reponews-0.4.0/src/reponews/qmanager.py` & `reponews-0.5.0/src/reponews/qmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 
 
 @dataclass
 class QueryManager(Generic[T]):
     has_next_page: bool = field(init=False, default=True)
 
     @abstractmethod
-    def make_query(self) -> tuple[str, dict[str, Any]]:
-        ...
+    def make_query(self) -> tuple[str, dict[str, Any]]: ...
 
     @abstractmethod
-    def parse_response(self, data: Any) -> list[T]:
-        ...
+    def parse_response(self, data: Any) -> list[T]: ...
 
 
 @dataclass
 class ReposQuery(QueryManager[Repository]):
     PATH: ClassVar[tuple[str, ...]]
     cursor: str | None = field(init=False, default=None)
```

### Comparing `reponews-0.4.0/src/reponews/types.py` & `reponews-0.5.0/src/reponews/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,31 +75,28 @@
 
 class Event(BaseModel):
     event_type: str
     timestamp: datetime  # Used for sorting
     repo: Repository
 
     @abstractmethod
-    def render(self) -> str:
-        ...
+    def render(self) -> str: ...
 
 
 class RepoActivity(Event):
     CONNECTION: ClassVar[Object]
     LAST_CONNECTION: ClassVar[Object]
 
     @classmethod
     @abstractmethod
-    def from_node(cls, repo: Repository, node: dict[str, Any]) -> Self:
-        ...
+    def from_node(cls, repo: Repository, node: dict[str, Any]) -> Self: ...
 
     @property
     @abstractmethod
-    def is_mine(self) -> bool:
-        ...
+    def is_mine(self) -> bool: ...
 
 
 class NewIssueoidEvent(RepoActivity):
     number: int
     title: str
     author: User
     url: str
```

### Comparing `reponews-0.4.0/src/reponews/util.py` & `reponews-0.5.0/src/reponews/util.py`

 * *Files identical despite different names*

### Comparing `reponews-0.4.0/test/conftest.py` & `reponews-0.5.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `reponews-0.4.0/test/data/config/empty.json` & `reponews-0.5.0/test/data/config/yestags.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.929098679098679%*

 * *Differences: {"'activity'": "{'releases': True, 'tags': True, 'released_tags': True, 'affiliated': "*

 * *               "{'prereleases': None, 'drafts': None}, 'prereleases': None, 'drafts': None}",*

 * * "'recipient'": "{replace: OrderedDict([('name', 'Myself'), ('address', 'me@here.there')])}"}*

```diff
@@ -1,35 +1,42 @@
 {
     "activity": {
         "affiliated": {
             "discussions": null,
+            "drafts": null,
             "forks": null,
             "issues": null,
             "my_activity": null,
+            "prereleases": null,
             "pull_requests": null,
             "released_tags": null,
             "releases": null,
             "stars": null,
             "tags": null
         },
         "discussions": null,
+        "drafts": null,
         "forks": null,
         "issues": null,
         "my_activity": null,
+        "prereleases": null,
         "pull_requests": null,
-        "released_tags": null,
-        "releases": null,
+        "released_tags": true,
+        "releases": true,
         "repo": {},
         "stars": null,
-        "tags": null
+        "tags": true
     },
     "api_url": "https://api.github.com/graphql",
     "auth_token": null,
     "auth_token_file": null,
-    "recipient": null,
+    "recipient": {
+        "address": "me@here.there",
+        "name": "Myself"
+    },
     "repos": {
         "affiliations": [
             "OWNER",
             "ORGANIZATION_MEMBER",
             "COLLABORATOR"
         ],
         "exclude": [],
```

### Comparing `reponews-0.4.0/test/data/config/full.json` & `reponews-0.5.0/test/data/config/full.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910644910644911%*

 * *Differences: {"'activity'": "{'affiliated': {'prereleases': None, 'drafts': None}, 'prereleases': None, "*

 * *               "'drafts': False}"}*

```diff
@@ -1,24 +1,28 @@
 {
     "activity": {
         "affiliated": {
             "discussions": null,
+            "drafts": null,
             "forks": null,
             "issues": null,
             "my_activity": null,
+            "prereleases": null,
             "pull_requests": null,
             "released_tags": null,
             "releases": null,
             "stars": null,
             "tags": null
         },
         "discussions": true,
+        "drafts": false,
         "forks": null,
         "issues": false,
         "my_activity": true,
+        "prereleases": null,
         "pull_requests": false,
         "released_tags": null,
         "releases": null,
         "repo": {},
         "stars": null,
         "tags": null
     },
```

### Comparing `reponews-0.4.0/test/data/config/minimal.json` & `reponews-0.5.0/test/data/config/minimal.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910644910644911%*

 * *Differences: {"'activity'": "{'affiliated': {'prereleases': None, 'drafts': None}, 'prereleases': None, "*

 * *               "'drafts': None}"}*

```diff
@@ -1,24 +1,28 @@
 {
     "activity": {
         "affiliated": {
             "discussions": null,
+            "drafts": null,
             "forks": null,
             "issues": null,
             "my_activity": null,
+            "prereleases": null,
             "pull_requests": null,
             "released_tags": null,
             "releases": null,
             "stars": null,
             "tags": null
         },
         "discussions": null,
+        "drafts": null,
         "forks": null,
         "issues": null,
         "my_activity": null,
+        "prereleases": null,
         "pull_requests": null,
         "released_tags": null,
         "releases": null,
         "repo": {},
         "stars": null,
         "tags": null
     },
```

### Comparing `reponews-0.4.0/test/data/config/relpaths.json` & `reponews-0.5.0/test/data/config/empty.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.87995337995338%*

 * *Differences: {"'activity'": "{'affiliated': {'prereleases': None, 'drafts': None}, 'prereleases': None, "*

 * *               "'drafts': None}",*

 * * "'auth_token_file'": 'None',*

 * * "'state_file'": 'None'}*

```diff
@@ -1,41 +1,45 @@
 {
     "activity": {
         "affiliated": {
             "discussions": null,
+            "drafts": null,
             "forks": null,
             "issues": null,
             "my_activity": null,
+            "prereleases": null,
             "pull_requests": null,
             "released_tags": null,
             "releases": null,
             "stars": null,
             "tags": null
         },
         "discussions": null,
+        "drafts": null,
         "forks": null,
         "issues": null,
         "my_activity": null,
+        "prereleases": null,
         "pull_requests": null,
         "released_tags": null,
         "releases": null,
         "repo": {},
         "stars": null,
         "tags": null
     },
     "api_url": "https://api.github.com/graphql",
     "auth_token": null,
-    "auth_token_file": "{config}/token.txt",
+    "auth_token_file": null,
     "recipient": null,
     "repos": {
         "affiliations": [
             "OWNER",
             "ORGANIZATION_MEMBER",
             "COLLABORATOR"
         ],
         "exclude": [],
         "include": []
     },
     "sender": null,
-    "state_file": "{config}/state/reponews.json",
+    "state_file": null,
     "subject": "[reponews] New activity on your GitHub repositories"
 }
```

### Comparing `reponews-0.4.0/test/data/config/repo-activity01.json` & `reponews-0.5.0/test/data/config/repo-activity02.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821977790727792%*

 * *Differences: {"'activity'": "{'issues': False, 'discussions': False, 'stars': False, 'forks': False, "*

 * *               "'affiliated': {'issues': True, 'prereleases': None, 'drafts': None}, 'repo': "*

 * *               "{'owner/*': {'stars': True, 'prereleases': None, 'drafts': None}, 'owner/repo': "*

 * *               "{'forks': True, 'prereleases': None, 'drafts': None}}, 'prereleases': None, "*

 * *               "'drafts': None}"}*

```diff
@@ -1,54 +1,62 @@
 {
     "activity": {
         "affiliated": {
             "discussions": null,
+            "drafts": null,
             "forks": null,
-            "issues": false,
+            "issues": true,
             "my_activity": null,
+            "prereleases": null,
             "pull_requests": false,
             "released_tags": null,
             "releases": null,
             "stars": null,
             "tags": null
         },
-        "discussions": null,
-        "forks": null,
-        "issues": null,
+        "discussions": false,
+        "drafts": null,
+        "forks": false,
+        "issues": false,
         "my_activity": null,
+        "prereleases": null,
         "pull_requests": null,
         "released_tags": null,
         "releases": null,
         "repo": {
             "owner/*": {
                 "discussions": null,
+                "drafts": null,
                 "forks": null,
                 "include": true,
                 "issues": null,
                 "my_activity": true,
+                "prereleases": null,
                 "pull_requests": null,
                 "released_tags": null,
                 "releases": null,
-                "stars": null,
+                "stars": true,
                 "tags": false
             },
             "owner/repo": {
                 "discussions": null,
-                "forks": null,
+                "drafts": null,
+                "forks": true,
                 "include": true,
                 "issues": null,
                 "my_activity": false,
+                "prereleases": null,
                 "pull_requests": null,
                 "released_tags": null,
                 "releases": false,
                 "stars": null,
                 "tags": null
             }
         },
-        "stars": null,
+        "stars": false,
         "tags": null
     },
     "api_url": "https://api.github.com/graphql",
     "auth_token": null,
     "auth_token_file": null,
     "recipient": null,
     "repos": {
```

### Comparing `reponews-0.4.0/test/data/config/repo-activity02.json` & `reponews-0.5.0/test/data/config/repo-activity01.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821977790727792%*

 * *Differences: {"'activity'": "{'issues': None, 'discussions': None, 'stars': None, 'forks': None, 'affiliated': "*

 * *               "{'issues': False, 'prereleases': None, 'drafts': None}, 'repo': {'owner/*': "*

 * *               "{'stars': None, 'prereleases': None, 'drafts': None}, 'owner/repo': {'forks': "*

 * *               "None, 'prereleases': None, 'drafts': None}}, 'prereleases': None, 'drafts': None}"}*

```diff
@@ -1,54 +1,62 @@
 {
     "activity": {
         "affiliated": {
             "discussions": null,
+            "drafts": null,
             "forks": null,
-            "issues": true,
+            "issues": false,
             "my_activity": null,
+            "prereleases": null,
             "pull_requests": false,
             "released_tags": null,
             "releases": null,
             "stars": null,
             "tags": null
         },
-        "discussions": false,
-        "forks": false,
-        "issues": false,
+        "discussions": null,
+        "drafts": null,
+        "forks": null,
+        "issues": null,
         "my_activity": null,
+        "prereleases": null,
         "pull_requests": null,
         "released_tags": null,
         "releases": null,
         "repo": {
             "owner/*": {
                 "discussions": null,
+                "drafts": null,
                 "forks": null,
                 "include": true,
                 "issues": null,
                 "my_activity": true,
+                "prereleases": null,
                 "pull_requests": null,
                 "released_tags": null,
                 "releases": null,
-                "stars": true,
+                "stars": null,
                 "tags": false
             },
             "owner/repo": {
                 "discussions": null,
-                "forks": true,
+                "drafts": null,
+                "forks": null,
                 "include": true,
                 "issues": null,
                 "my_activity": false,
+                "prereleases": null,
                 "pull_requests": null,
                 "released_tags": null,
                 "releases": false,
                 "stars": null,
                 "tags": null
             }
         },
-        "stars": false,
+        "stars": null,
         "tags": null
     },
     "api_url": "https://api.github.com/graphql",
     "auth_token": null,
     "auth_token_file": null,
     "recipient": null,
     "repos": {
```

### Comparing `reponews-0.4.0/test/data/config/yestags.json` & `reponews-0.5.0/test/data/config/relpaths.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.817987567987568%*

 * *Differences: {"'activity'": "{'releases': None, 'tags': None, 'released_tags': None, 'affiliated': "*

 * *               "{'prereleases': None, 'drafts': None}, 'prereleases': None, 'drafts': None}",*

 * * "'auth_token_file'": "'{config}/token.txt'",*

 * * "'recipient'": 'None',*

 * * "'state_file'": "'{config}/state/reponews.json'"}*

```diff
@@ -1,44 +1,45 @@
 {
     "activity": {
         "affiliated": {
             "discussions": null,
+            "drafts": null,
             "forks": null,
             "issues": null,
             "my_activity": null,
+            "prereleases": null,
             "pull_requests": null,
             "released_tags": null,
             "releases": null,
             "stars": null,
             "tags": null
         },
         "discussions": null,
+        "drafts": null,
         "forks": null,
         "issues": null,
         "my_activity": null,
+        "prereleases": null,
         "pull_requests": null,
-        "released_tags": true,
-        "releases": true,
+        "released_tags": null,
+        "releases": null,
         "repo": {},
         "stars": null,
-        "tags": true
+        "tags": null
     },
     "api_url": "https://api.github.com/graphql",
     "auth_token": null,
-    "auth_token_file": null,
-    "recipient": {
-        "address": "me@here.there",
-        "name": "Myself"
-    },
+    "auth_token_file": "{config}/token.txt",
+    "recipient": null,
     "repos": {
         "affiliations": [
             "OWNER",
             "ORGANIZATION_MEMBER",
             "COLLABORATOR"
         ],
         "exclude": [],
         "include": []
     },
     "sender": null,
-    "state_file": null,
+    "state_file": "{config}/state/reponews.json",
     "subject": "[reponews] New activity on your GitHub repositories"
 }
```

### Comparing `reponews-0.4.0/test/data/mock/body.txt` & `reponews-0.5.0/test/data/mock/body.txt`

 * *Files identical despite different names*

### Comparing `reponews-0.4.0/test/data/mock/dump-repos.txt` & `reponews-0.5.0/test/data/mock/dump-repos.txt`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9025974025974026%*

 * *Differences: {"'luser/my-repo'": "{'drafts': True, 'prereleases': True}",*

 * * "'org/big-project'": "{'issues': False, 'releases': True, 'drafts': False, 'prereleases': False}",*

 * * "'org/workspace'": "{'drafts': False, 'prereleases': True}",*

 * * "'theteam/new-project'": "{'drafts': True, 'prereleases': True}",*

 * * "'viewer/new-repo'": "{'drafts': True, 'prereleases': True}",*

 * * "'viewer/project'": "{'drafts': True, 'prereleases': True}",*

 * * "'viewer/repo'": "{'drafts': True, 'prereleases': True}"}*

```diff
@@ -1,79 +1,93 @@
 {
     "luser/my-repo": {
         "discussions": true,
+        "drafts": true,
         "forks": true,
         "issues": true,
         "my_activity": false,
+        "prereleases": true,
         "pull_requests": true,
         "released_tags": true,
         "releases": true,
         "stars": true,
         "tags": true
     },
     "org/big-project": {
         "discussions": true,
+        "drafts": false,
         "forks": true,
-        "issues": true,
+        "issues": false,
         "my_activity": true,
+        "prereleases": false,
         "pull_requests": true,
         "released_tags": false,
-        "releases": false,
+        "releases": true,
         "stars": true,
         "tags": true
     },
     "org/workspace": {
         "discussions": true,
+        "drafts": false,
         "forks": true,
         "issues": true,
         "my_activity": true,
+        "prereleases": true,
         "pull_requests": true,
         "released_tags": false,
         "releases": true,
         "stars": true,
         "tags": true
     },
     "theteam/new-project": {
         "discussions": true,
+        "drafts": true,
         "forks": true,
         "issues": true,
         "my_activity": false,
+        "prereleases": true,
         "pull_requests": true,
         "released_tags": false,
         "releases": true,
         "stars": true,
         "tags": true
     },
     "viewer/new-repo": {
         "discussions": true,
+        "drafts": true,
         "forks": true,
         "issues": true,
         "my_activity": false,
+        "prereleases": true,
         "pull_requests": true,
         "released_tags": false,
         "releases": true,
         "stars": true,
         "tags": true
     },
     "viewer/project": {
         "discussions": true,
+        "drafts": true,
         "forks": true,
         "issues": true,
         "my_activity": false,
+        "prereleases": true,
         "pull_requests": true,
         "released_tags": false,
         "releases": true,
         "stars": true,
         "tags": true
     },
     "viewer/repo": {
         "discussions": true,
+        "drafts": true,
         "forks": true,
         "issues": true,
         "my_activity": false,
+        "prereleases": true,
         "pull_requests": true,
         "released_tags": false,
         "releases": true,
         "stars": true,
         "tags": true
     }
 }
```

### Comparing `reponews-0.4.0/test/data/mock/home/config.toml` & `reponews-0.5.0/test/data/mock/home/config.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 subject = "Your Repo News is here!"
 auth-token = "1234567890"
 api-url = "https://test.nil/api"
 state-file = "state.json"
 
 [reponews.activity.repo."org/*"]
 my-activity = true
+drafts = false
+prereleases = true
 
 [reponews.activity.repo."org/big-project"]
-releases = false
+issues = false
+prereleases = false
 
 [reponews.activity.repo."luser/my-repo"]
 released-tags = true
 
 [reponews.repos]
 affiliations = ["OWNER", "COLLABORATOR"]
 include = [
```

### Comparing `reponews-0.4.0/test/data/mock/home/state.json` & `reponews-0.5.0/test/data/mock/home/state.json`

 * *Files identical despite different names*

### Comparing `reponews-0.4.0/test/data/mock/new-state.json` & `reponews-0.5.0/test/data/mock/new-state.json`

 * *Files identical despite different names*

### Comparing `reponews-0.4.0/test/data/mock/session-data.json` & `reponews-0.5.0/test/data/mock/session-data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996811224489797%*

 * *Differences: {"'activity'": "{'org/big-project': {'activity_types': {insert: [(2, 'release')], delete: [0]}}}"}*

```diff
@@ -85,17 +85,17 @@
                     "timestamp": "2021-11-29T14:45:21+00:00",
                     "url": "https://github.com/luser/my-repo/releases/tag/2.0.1"
                 }
             ]
         },
         "org/big-project": {
             "activity_types": [
-                "issue",
                 "pr",
                 "discussion",
+                "release",
                 "tag",
                 "star",
                 "fork"
             ],
             "cursors_in": {
                 "discussion": "discussions:org/big-project:01",
                 "fork": "forks:org/big-project:01",
```

### Comparing `reponews-0.4.0/test/test_config.py` & `reponews-0.5.0/test/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,14 +87,16 @@
             mkrepo("owner", "repo"),
             True,
             ActivityPrefs(
                 issues=True,
                 pull_requests=True,
                 discussions=True,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=True,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=False,
             ),
         ),
@@ -103,14 +105,16 @@
             mkrepo("owner", "repo"),
             False,
             ActivityPrefs(
                 issues=True,
                 pull_requests=True,
                 discussions=True,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=True,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=False,
             ),
         ),
@@ -119,14 +123,16 @@
             mkrepo("owner", "repo"),
             True,
             ActivityPrefs(
                 issues=False,
                 pull_requests=False,
                 discussions=True,
                 releases=True,
+                prereleases=True,
+                drafts=False,
                 tags=True,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=True,
             ),
         ),
@@ -135,14 +141,16 @@
             mkrepo("owner", "repo"),
             False,
             ActivityPrefs(
                 issues=False,
                 pull_requests=False,
                 discussions=True,
                 releases=True,
+                prereleases=True,
+                drafts=False,
                 tags=True,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=True,
             ),
         ),
@@ -151,14 +159,16 @@
             mkrepo("luser", "repo"),
             True,
             ActivityPrefs(
                 issues=False,
                 pull_requests=False,
                 discussions=True,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=True,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=False,
             ),
         ),
@@ -167,14 +177,16 @@
             mkrepo("luser", "repo"),
             False,
             ActivityPrefs(
                 issues=True,
                 pull_requests=True,
                 discussions=True,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=True,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=False,
             ),
         ),
@@ -183,14 +195,16 @@
             mkrepo("owner", "project"),
             False,
             ActivityPrefs(
                 issues=True,
                 pull_requests=True,
                 discussions=True,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=False,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=True,
             ),
         ),
@@ -199,14 +213,16 @@
             mkrepo("owner", "repo"),
             False,
             ActivityPrefs(
                 issues=True,
                 pull_requests=True,
                 discussions=True,
                 releases=False,
+                prereleases=True,
+                drafts=True,
                 tags=False,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=False,
             ),
         ),
@@ -215,14 +231,16 @@
             mkrepo("owner", "repo"),
             True,
             ActivityPrefs(
                 issues=False,
                 pull_requests=False,
                 discussions=True,
                 releases=False,
+                prereleases=True,
+                drafts=True,
                 tags=False,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=False,
             ),
         ),
@@ -231,14 +249,16 @@
             mkrepo("luser", "repo"),
             True,
             ActivityPrefs(
                 issues=True,
                 pull_requests=False,
                 discussions=False,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=True,
                 released_tags=False,
                 stars=False,
                 forks=False,
                 my_activity=False,
             ),
         ),
@@ -247,14 +267,16 @@
             mkrepo("luser", "repo"),
             False,
             ActivityPrefs(
                 issues=False,
                 pull_requests=True,
                 discussions=False,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=True,
                 released_tags=False,
                 stars=False,
                 forks=False,
                 my_activity=False,
             ),
         ),
@@ -263,14 +285,16 @@
             mkrepo("owner", "project"),
             False,
             ActivityPrefs(
                 issues=False,
                 pull_requests=True,
                 discussions=False,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=False,
                 released_tags=False,
                 stars=True,
                 forks=False,
                 my_activity=True,
             ),
         ),
@@ -279,14 +303,16 @@
             mkrepo("owner", "repo"),
             False,
             ActivityPrefs(
                 issues=False,
                 pull_requests=True,
                 discussions=False,
                 releases=False,
+                prereleases=True,
+                drafts=True,
                 tags=False,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=False,
             ),
         ),
@@ -295,14 +321,16 @@
             mkrepo("owner", "repo"),
             True,
             ActivityPrefs(
                 issues=True,
                 pull_requests=False,
                 discussions=False,
                 releases=False,
+                prereleases=True,
+                drafts=True,
                 tags=False,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=False,
             ),
         ),
@@ -311,14 +339,16 @@
             mkrepo("owner", "repo"),
             True,
             ActivityPrefs(
                 issues=True,
                 pull_requests=True,
                 discussions=True,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=True,
                 released_tags=True,
                 stars=True,
                 forks=True,
                 my_activity=False,
             ),
         ),
@@ -327,14 +357,16 @@
             mkrepo("owner", "repo"),
             False,
             ActivityPrefs(
                 issues=True,
                 pull_requests=True,
                 discussions=True,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=True,
                 released_tags=True,
                 stars=True,
                 forks=True,
                 my_activity=False,
             ),
         ),
@@ -352,14 +384,16 @@
     [
         (
             ActivityPrefs(
                 issues=True,
                 pull_requests=True,
                 discussions=True,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=True,
                 released_tags=False,
                 stars=True,
                 forks=True,
                 my_activity=False,
             ),
             [
@@ -374,28 +408,32 @@
         ),
         (
             ActivityPrefs(
                 issues=False,
                 pull_requests=False,
                 discussions=False,
                 releases=False,
+                prereleases=True,
+                drafts=True,
                 tags=False,
                 released_tags=True,
                 stars=False,
                 forks=False,
                 my_activity=True,
             ),
             [],
         ),
         (
             ActivityPrefs(
                 issues=True,
                 pull_requests=True,
                 discussions=True,
                 releases=True,
+                prereleases=True,
+                drafts=True,
                 tags=False,
                 released_tags=True,
                 stars=False,
                 forks=False,
                 my_activity=True,
             ),
             [
```

### Comparing `reponews-0.4.0/test/test_main.py` & `reponews-0.5.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `reponews-0.4.0/test/test_qmanager.py` & `reponews-0.5.0/test/test_qmanager.py`

 * *Files identical despite different names*

### Comparing `reponews-0.4.0/test/test_types.py` & `reponews-0.5.0/test/test_types.py`

 * *Files identical despite different names*

### Comparing `reponews-0.4.0/tox.ini` & `reponews-0.5.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     mypy src test
 
 [pytest]
 addopts = --cov=reponews --no-cov-on-fail
 filterwarnings =
     error
     # <https://github.com/urllib3/urllib3/issues/3020>
-    ignore:urllib3 v2.0 only supports OpenSSL
+    ignore:urllib3 v2(.0)? only supports OpenSSL
     # Warning emitted due to mocking a BaseModel:
     ignore:The `__fields__` attribute is deprecated:pydantic.warnings.PydanticDeprecatedSince20
 norecursedirs = test/data
 
 [coverage:run]
 branch = True
 parallel = True
@@ -55,21 +55,20 @@
 exclude_lines =
     pragma: no cover
     if TYPE_CHECKING:
     \.\.\.
 
 [flake8]
 doctests = True
-exclude = .*/,build/,dist/,test/data,venv/
-hang-closing = False
+extend-exclude = build/,dist/,test/data,venv/
 max-doc-length = 100
 max-line-length = 80
 unused-arguments-ignore-stub-functions = True
-select = A,B,B902,B950,C,E,E242,F,U100,W
-ignore = B005,E203,E262,E266,E501,W503
+extend-select = B901,B902,B950
+ignore = A003,A005,B005,E203,E262,E266,E501,E704,U101,W503
 
 [isort]
 atomic = True
 force_sort_within_sections = True
 honor_noqa = True
 lines_between_sections = 0
 profile = black
```


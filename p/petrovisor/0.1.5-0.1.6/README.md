# Comparing `tmp/petrovisor-0.1.5.tar.gz` & `tmp/petrovisor-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petrovisor-0.1.5.tar", last modified: Sun Apr 28 11:45:29 2024, max compression
+gzip compressed data, was "petrovisor-0.1.6.tar", last modified: Fri May  3 11:39:05 2024, max compression
```

## Comparing `petrovisor-0.1.5.tar` & `petrovisor-0.1.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:29.004218 petrovisor-0.1.5/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-04-28 11:45:24.000000 petrovisor-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-28 11:45:29.004218 petrovisor-0.1.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3311 2024-04-28 11:45:24.000000 petrovisor-0.1.5/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-04-28 11:45:24.000000 petrovisor-0.1.5/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      919 2024-04-28 11:45:29.004218 petrovisor-0.1.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-04-28 11:45:24.000000 petrovisor-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:28.992218 petrovisor-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:28.992218 petrovisor-0.1.5/src/petrovisor/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:28.996218 petrovisor-0.1.5/src/petrovisor/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18461 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:28.996218 petrovisor-0.1.5/src/petrovisor/api/enums/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/enums/data_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/enums/increments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/enums/internal_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/enums/items.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/enums/ml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:29.000218 petrovisor-0.1.5/src/petrovisor/api/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29822 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/data_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)    48466 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17056 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/pivot_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/psharp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/reference_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)    60533 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/methods/workspace_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:29.000218 petrovisor-0.1.5/src/petrovisor/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/models/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/models/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/models/entity_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/models/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/models/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/models/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/models/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:29.000218 petrovisor-0.1.5/src/petrovisor/api/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/protocols/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:29.000218 petrovisor-0.1.5/src/petrovisor/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/utils/datastructs.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12256 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/utils/login.py
--rw-r--r--   0 runner    (1001) docker     (127)    16700 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/utils/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/api/utils/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:29.004218 petrovisor-0.1.5/src/petrovisor/models/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/models/contexts_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2705 2024-04-28 11:45:24.000000 petrovisor-0.1.5/src/petrovisor/petrovisor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:29.004218 petrovisor-0.1.5/src/petrovisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-28 11:45:28.000000 petrovisor-0.1.5/src/petrovisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-28 11:45:28.000000 petrovisor-0.1.5/src/petrovisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 11:45:28.000000 petrovisor-0.1.5/src/petrovisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 11:45:28.000000 petrovisor-0.1.5/src/petrovisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 11:45:28.000000 petrovisor-0.1.5/src/petrovisor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:45:29.004218 petrovisor-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-28 11:45:24.000000 petrovisor-0.1.5/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-28 11:45:24.000000 petrovisor-0.1.5/tests/test_entities_and_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-28 11:45:24.000000 petrovisor-0.1.5/tests/test_reference_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-04-28 11:45:24.000000 petrovisor-0.1.5/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-28 11:45:24.000000 petrovisor-0.1.5/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.696401 petrovisor-0.1.6/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-05-03 11:39:01.000000 petrovisor-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-03 11:39:05.696401 petrovisor-0.1.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3311 2024-05-03 11:39:01.000000 petrovisor-0.1.6/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-05-03 11:39:01.000000 petrovisor-0.1.6/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      919 2024-05-03 11:39:05.696401 petrovisor-0.1.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-05-03 11:39:01.000000 petrovisor-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.684401 petrovisor-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.688401 petrovisor-0.1.6/src/petrovisor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.688401 petrovisor-0.1.6/src/petrovisor/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18461 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.688401 petrovisor-0.1.6/src/petrovisor/api/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/enums/data_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/enums/increments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/enums/internal_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/enums/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/enums/ml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.692401 petrovisor-0.1.6/src/petrovisor/api/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29822 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/data_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48466 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17056 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/pivot_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/psharp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/reference_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61878 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/methods/workspace_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.692401 petrovisor-0.1.6/src/petrovisor/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/models/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/models/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/models/entity_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/models/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/models/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/models/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/models/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.692401 petrovisor-0.1.6/src/petrovisor/api/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/protocols/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.696401 petrovisor-0.1.6/src/petrovisor/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/utils/datastructs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12256 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/utils/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/api/utils/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.696401 petrovisor-0.1.6/src/petrovisor/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/models/contexts_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2705 2024-05-03 11:39:01.000000 petrovisor-0.1.6/src/petrovisor/petrovisor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.696401 petrovisor-0.1.6/src/petrovisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-03 11:39:05.000000 petrovisor-0.1.6/src/petrovisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-03 11:39:05.000000 petrovisor-0.1.6/src/petrovisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:39:05.000000 petrovisor-0.1.6/src/petrovisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 11:39:05.000000 petrovisor-0.1.6/src/petrovisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 11:39:05.000000 petrovisor-0.1.6/src/petrovisor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:39:05.696401 petrovisor-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-03 11:39:01.000000 petrovisor-0.1.6/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-03 11:39:01.000000 petrovisor-0.1.6/tests/test_entities_and_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-03 11:39:01.000000 petrovisor-0.1.6/tests/test_reference_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-05-03 11:39:01.000000 petrovisor-0.1.6/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-03 11:39:01.000000 petrovisor-0.1.6/tests/test_units.py
```

### Comparing `petrovisor-0.1.5/LICENSE` & `petrovisor-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/PKG-INFO` & `petrovisor-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petrovisor
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python API for PetroVisor platform.
 Home-page: https://github.com/Datagration/petrovisor-python-api
 Author: Datagration Solutions Inc.
 Author-email: "Datagration Solutions Inc." <developers@datagration.com>
 License: MIT License
         
         Copyright (c) 2021 Datagration Solutions Inc.
```

### Comparing `petrovisor-0.1.5/README.md` & `petrovisor-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/pyproject.toml` & `petrovisor-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/setup.cfg` & `petrovisor-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/__init__.py` & `petrovisor-0.1.6/src/petrovisor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 # api
 from petrovisor.petrovisor import PetroVisor
 
 # data types
 from petrovisor.api.enums.items import ItemType
 from petrovisor.api.enums.internal_dtypes import (
```

### Comparing `petrovisor-0.1.5/src/petrovisor/api/base.py` & `petrovisor-0.1.6/src/petrovisor/api/base.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/enums/data_grids.py` & `petrovisor-0.1.6/src/petrovisor/api/enums/data_grids.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/enums/increments.py` & `petrovisor-0.1.6/src/petrovisor/api/enums/increments.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/enums/internal_dtypes.py` & `petrovisor-0.1.6/src/petrovisor/api/enums/internal_dtypes.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/enums/items.py` & `petrovisor-0.1.6/src/petrovisor/api/enums/items.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/enums/ml.py` & `petrovisor-0.1.6/src/petrovisor/api/enums/ml.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/contexts.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/contexts.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/data_grids.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/data_grids.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/dataframes.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/dataframes.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/entities.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/entities.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/files.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/files.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/items.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/items.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/logs.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/logs.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/ml.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/ml.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/pivot_tables.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/pivot_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import (
     Any,
     Optional,
     Union,
     Dict,
 )
 import warnings
-import time
 
 from petrovisor.api.utils.helper import ApiHelper
 from petrovisor.api.utils.requests import ApiRequests
 from petrovisor.api.enums.items import ItemType
 from petrovisor.api.protocols.protocols import (
     SupportsRequests,
     SupportsItemRequests,
```

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/psharp.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/psharp.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/reference_tables.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/reference_tables.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/signals.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -787,15 +787,15 @@
             if depth_step is not None:
                 data_rqst["DepthStep"] = depth_step
 
             table_data = self.post("Filters/Data", data=data_rqst) or {}
             data_time_num = table_data.get("DataNumeric", [])
             data_time_str = table_data.get("DataString", [])
             data_depth_num = table_data.get("DataDepth", [])
-            data_depth_str = table_data.get("DataStringDepth", [])
+            data_depth_str = table_data.get("DataDepthString", [])
 
             if data_time_num and data_time_str:
                 data_time = [*data_time_num, *data_time_str]
             elif data_time_num:
                 data_time = data_time_num
             elif data_time_str:
                 data_time = data_time_str
@@ -816,44 +816,60 @@
                 df_normalized = pd.json_normalize(
                     data_time,
                     meta=["EntityName", "ResultName", "UnitName"],
                     record_path=["Data"],
                 )
 
                 # generate PivotTable
-                df = df_normalized.pivot(
-                    index=["EntityName", "Date"], columns="ResultName", values="Value"
-                )
-                df.columns.name = None
-                df = df.rename(columns=signals_with_units_map)
-                df = df.reset_index()
-                df = df.rename(columns={"EntityName": "Entity"})
-                df["Date"] = pd.to_datetime(df["Date"])
-                if has_time_signals:
-                    df_time = df
+                if "Date" not in df_normalized.columns:
+                    warnings.warn(
+                        "PetroVisor::load_signals_data():: Couldn't retrieve any 'time' data.",
+                        RuntimeWarning,
+                    )
                 else:
-                    df_static = df.drop(columns=["Date"])
+                    df = df_normalized.pivot(
+                        index=["EntityName", "Date"],
+                        columns="ResultName",
+                        values="Value",
+                    )
+                    df.columns.name = None
+                    df = df.rename(columns=signals_with_units_map)
+                    df = df.reset_index()
+                    df = df.rename(columns={"EntityName": "Entity"})
+                    df["Date"] = pd.to_datetime(df["Date"])
+                    if has_time_signals:
+                        df_time = df
+                    else:
+                        df_static = df.drop(columns=["Date"])
 
             if data_depth:
                 # create DataFrame by normalizing json
                 df_normalized = pd.json_normalize(
                     data_depth,
                     meta=["EntityName", "ResultName", "UnitName"],
                     record_path=["Data"],
                 )
 
                 # generate PivotTable
-                df = df_normalized.pivot(
-                    index=["EntityName", "Depth"], columns="ResultName", values="Value"
-                )
-                df.columns.name = None
-                df = df.rename(columns=signals_with_units_map)
-                df = df.reset_index()
-                df = df.rename(columns={"EntityName": "Entity"})
-                df_depth = df
+                if "Depth" not in df_normalized.columns:
+                    warnings.warn(
+                        "PetroVisor::load_signals_data():: Couldn't retrieve any 'depth' data.",
+                        RuntimeWarning,
+                    )
+                else:
+                    df = df_normalized.pivot(
+                        index=["EntityName", "Depth"],
+                        columns="ResultName",
+                        values="Value",
+                    )
+                    df.columns.name = None
+                    df = df.rename(columns=signals_with_units_map)
+                    df = df.reset_index()
+                    df = df.rename(columns={"EntityName": "Entity"})
+                    df_depth = df
         else:
             for data_type, data_type_signals in signal_types.items():
                 if data_type == "static":
                     num_signal_type = "Static"
                     str_signal_type = "String"
                 elif data_type == "time":
                     num_signal_type = "TimeDependent"
@@ -992,26 +1008,32 @@
                 elif data_str:
                     data = data_str
                 else:
                     data = []
 
                 if not data:
                     warnings.warn(
-                        f"PetroVisor::load_signals_data():: Couldn't retrieve any {data_type} data.",
+                        f"PetroVisor::load_signals_data():: Couldn't retrieve any '{data_type}' data.",
                         RuntimeWarning,
                     )
                     continue
 
                 if data_type == "time":
                     # create DataFrame by normalizing json
                     df_normalized = pd.json_normalize(
                         data, meta=["Entity", "Signal", "Unit"], record_path=["Data"]
                     )
 
                     # generate PivotTable
+                    if "Date" not in df_normalized.columns:
+                        warnings.warn(
+                            f"PetroVisor::load_signals_data():: Couldn't retrieve any '{data_type}' data.",
+                            RuntimeWarning,
+                        )
+                        continue
                     df = df_normalized.pivot(
                         index=["Entity", "Date"], columns="Signal", values="Value"
                     )
                     df.columns.name = None
                     df = df.rename(columns=signals_with_units_map)
                     df = df.reset_index()
                     df["Date"] = pd.to_datetime(df["Date"])
@@ -1019,14 +1041,20 @@
                 elif data_type == "depth":
                     # create DataFrame by normalizing json
                     df_normalized = pd.json_normalize(
                         data, meta=["Entity", "Signal", "Unit"], record_path=["Data"]
                     )
 
                     # generate PivotTable
+                    if "Depth" not in df_normalized.columns:
+                        warnings.warn(
+                            f"PetroVisor::load_signals_data():: Couldn't retrieve any '{data_type}' data.",
+                            RuntimeWarning,
+                        )
+                        continue
                     df = df_normalized.pivot(
                         index=["Entity", "Depth"], columns="Signal", values="Value"
                     )
                     df.columns.name = None
                     df = df.rename(columns=signals_with_units_map)
                     df = df.reset_index()
                     df_depth = df
```

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/units.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/units.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/workflows.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/workflows.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/methods/workspace_values.py` & `petrovisor-0.1.6/src/petrovisor/api/methods/workspace_values.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/models/context.py` & `petrovisor-0.1.6/src/petrovisor/api/models/context.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/models/scope.py` & `petrovisor-0.1.6/src/petrovisor/api/models/scope.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/models/signal.py` & `petrovisor-0.1.6/src/petrovisor/api/models/signal.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/models/unit.py` & `petrovisor-0.1.6/src/petrovisor/api/models/unit.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/protocols/protocols.py` & `petrovisor-0.1.6/src/petrovisor/api/protocols/protocols.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/utils/datastructs.py` & `petrovisor-0.1.6/src/petrovisor/api/utils/datastructs.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/utils/helper.py` & `petrovisor-0.1.6/src/petrovisor/api/utils/helper.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/utils/login.py` & `petrovisor-0.1.6/src/petrovisor/api/utils/login.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/api/utils/requests.py` & `petrovisor-0.1.6/src/petrovisor/api/utils/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,19 +314,18 @@
         # method name
         method_name = method.upper().strip()
 
         # convert data to json string
         if data and not isinstance(data, str):
             data = json.dumps(data)
 
-        # request secs
+        # request specs
         timeout = None  # no timeout
-        max_retries = (
-            1  # increased to 3 times in case of 400 Bad Request or 4004 Not Found
-        )
+        max_retries_top = 5
+        max_retries = 1  # increased to max_retries_top times in case of 400 Bad Request or 404 Not Found
         waiting_time = 5  # in seconds
 
         # get response
         response = None
         attempt = 0
         while attempt < max_retries:
             attempt += 1
@@ -422,15 +421,15 @@
                 ):
                     return response
 
                 if response.status_code in {
                     requests.codes.bad_request,
                     requests.codes.not_found,
                 }:
-                    max_retries = 3
+                    max_retries = max_retries_top
 
                 # retry request
                 if attempt < max_retries:
                     time.sleep(waiting_time)
                     response = None
                     continue
```

### Comparing `petrovisor-0.1.5/src/petrovisor/api/utils/validators.py` & `petrovisor-0.1.6/src/petrovisor/api/utils/validators.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor/models/contexts_manager.py` & `petrovisor-0.1.6/src/petrovisor/models/contexts_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.api = api
 
         # get EntitySet
         if entity_set:
             if isinstance(entity_set, str) and api.item_exists(
                 ItemType.EntitySet, entity_set
             ):
-                entity_set = api.get_entity(entity_set)
+                entity_set = api.get_entity_set(entity_set)
             entity_set = api.create_entity_set(entity_set)
 
         # get Scope
         if scope:
             if isinstance(scope, str) and api.item_exists(ItemType.Scope, scope):
                 scope = api.get_scope(scope)
             scope = api.create_scope(scope)
```

### Comparing `petrovisor-0.1.5/src/petrovisor/petrovisor.py` & `petrovisor-0.1.6/src/petrovisor/petrovisor.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/src/petrovisor.egg-info/PKG-INFO` & `petrovisor-0.1.6/src/petrovisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petrovisor
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python API for PetroVisor platform.
 Home-page: https://github.com/Datagration/petrovisor-python-api
 Author: Datagration Solutions Inc.
 Author-email: "Datagration Solutions Inc." <developers@datagration.com>
 License: MIT License
         
         Copyright (c) 2021 Datagration Solutions Inc.
```

### Comparing `petrovisor-0.1.5/src/petrovisor.egg-info/SOURCES.txt` & `petrovisor-0.1.6/src/petrovisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/tests/test_entities_and_signals.py` & `petrovisor-0.1.6/tests/test_entities_and_signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
             "Name": entity_name,
             "EntityTypeName": "Well",
             "Alias": "",
             "IsOpportunity": False,
         },
     )
     # rename entity
-    new_entity_name = entity_name.replace("_entity", "_renamed entity")
-    # pv_api.rename_entity(old_name=entity_name, new_name=new_entity_name)
+    # new_entity_name = entity_name.replace("_entity", "_renamed entity")
+    # api.rename_entity(old_name=entity_name, new_name=new_entity_name)
     # delete entity
-    # pv_api.delete_entity(new_entity_name)
+    # api.delete_entity(new_entity_name)
     # add signal
     signal_name = "Time Signal"
     signal_unit = " "
     max_length = 29
     short_signal_name = (
         signal_name[:max_length] if len(signal_name) > max_length else signal_name
     )
```

### Comparing `petrovisor-0.1.5/tests/test_reference_tables.py` & `petrovisor-0.1.6/tests/test_reference_tables.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.5/tests/test_signals.py` & `petrovisor-0.1.6/tests/test_signals.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import pandas as pd
-from datetime import datetime
 from petrovisor import (
     Signal,
     Entity,
     EntitySet,
     Hierarchy,
     Scope,
     Context,
@@ -18,15 +17,15 @@
 
 def test_signals(api: PetroVisor):
     stat_num_signal = "static numeric signal"
     stat_str_signal = "static string signal"
     time_num_signal = "time numeric signal"
     time_str_signal = "time string signal"
     depth_num_signal = "depth numeric signal"
-    depth_str_signal = "depth string signal"
+    # depth_str_signal = "depth string signal"
     signals = [
         Signal(
             type=SignalType.Static.name,
             name=stat_num_signal,
             unit=" ",
             unit_measurement="Dimensionless",
         ),
@@ -50,27 +49,35 @@
         ),
         Signal(
             type=SignalType.DepthDependent.name,
             name=depth_num_signal,
             unit=" ",
             unit_measurement="Dimensionless",
         ),
-        Signal(
-            type=SignalType.StringDepthDependent.name,
-            name=depth_str_signal,
-            unit=" ",
-            unit_measurement="Dimensionless",
-        ),
+        # Signal(
+        #     type=SignalType.StringDepthDependent.name,
+        #     name=depth_str_signal,
+        #     unit=" ",
+        #     unit_measurement="Dimensionless",
+        # ),
     ]
 
     # create signals
     for signal in signals:
         if not api.item_exists(ItemType.Signal, signal.name):
             api.add_signal(signal)
 
+    # wait until all signals created
+    all_signals_exist = False
+    while not all_signals_exist:
+        all_signals_exist = True
+        for signal in signals:
+            if not api.item_exists(ItemType.Signal, signal.name):
+                all_signals_exist = False
+
     # entities
     entities = [
         Entity(name="Well 001", type="Well"),
         Entity(name="Well 002", type="Well"),
         Entity(name="Well 003", type="Well"),
         Entity(name="Well 004", type="Well"),
         Entity(name="Well 005", type="Well"),
@@ -79,51 +86,53 @@
 
     # create entities
     for entity in entities:
         if not api.item_exists(ItemType.Entity, entity.name):
             api.add_entity(entity)
 
     # create entity set
-    entity_set = EntitySet(name="Field 1 Wells",
-                           entities=entities)
+    entity_set = EntitySet(name="Field 1 Wells", entities=entities)
 
     # create hierarchy
     relationship = {
         "Well 001": "Field 1",
         "Well 002": "Field 1",
         "Well 003": "Field 1",
         "Well 004": "Field 1",
         "Well 005": "Field 1",
     }
-    hierarchy = Hierarchy(name="Field 1 Wells",
-                          relationship=relationship,
-                          )
+    hierarchy = Hierarchy(
+        name="Field 1 Wells",
+        relationship=relationship,
+    )
 
     # create scope
     time_start = "2021-01-01T00:00:00"
     time_end = "2022-01-01T00:00:00"
     time_step = TimeIncrement.Daily.name
     depth_start = 0
     depth_end = 10
     depth_step = DepthIncrement.Meter.name
-    scope = Scope(name="Field 1 Wells Scope",
-                  time_start=time_start,
-                  time_end=time_end,
-                  time_step=time_step,
-                  depth_start=depth_start,
-                  depth_end=depth_end,
-                  depth_step=depth_step,
-                  )
+    scope = Scope(
+        name="Field 1 Wells Scope",
+        time_start=time_start,
+        time_end=time_end,
+        time_step=time_step,
+        depth_start=depth_start,
+        depth_end=depth_end,
+        depth_step=depth_step,
+    )
 
     # create context
-    context = Context(name="Context",
-                      scope=scope,
-                      entity_set=entity_set,
-                      hierarchy=hierarchy,
-                      )
+    context = Context(
+        name="Context",
+        scope=scope,
+        entity_set=entity_set,
+        hierarchy=hierarchy,
+    )
 
     # data preparation
     entity_col = "Entity"
     time_col = "Date"
     depth_col = "Depth [m]"
     letters = list(map(chr, range(97, 123)))
     num_wells = 5
@@ -134,85 +143,110 @@
     # static data
     data_stat = []
     for i in range(0, num_wells):
         well_idx = i + 1
         entities = [f"Well 00{well_idx}"]
         num_vals = [i]
         str_vals = [letters[i]]
-        data_stat.append(pd.DataFrame({
-            entity_col: entities,
-            stat_num_signal: num_vals,
-            stat_str_signal: str_vals,
-        }))
+        data_stat.append(
+            pd.DataFrame(
+                {
+                    entity_col: entities,
+                    stat_num_signal: num_vals,
+                    stat_str_signal: str_vals,
+                }
+            )
+        )
     df_stat = pd.concat(data_stat, ignore_index=True)
 
     # save static data
     api.save_table_data(df_stat)
 
     # time data
     data_time = []
     for i in range(0, num_wells):
         well_idx = i + 1
         entities = np.repeat(f"Well 00{well_idx}", time_steps)
         dates = pd.date_range(time_start, periods=time_steps, freq="d").to_list()
         num_vals = np.random.uniform(1, 4, time_steps)
         str_vals = np.random.choice(letters, time_steps)
-        data_time.append(pd.DataFrame({
-            entity_col: entities,
-            time_col: dates,
-            time_num_signal: num_vals,
-            time_str_signal: str_vals,
-        }))
+        data_time.append(
+            pd.DataFrame(
+                {
+                    entity_col: entities,
+                    time_col: dates,
+                    time_num_signal: num_vals,
+                    time_str_signal: str_vals,
+                }
+            )
+        )
     df_time = pd.concat(data_time, ignore_index=True)
 
     # save time data
     api.save_table_data(df_time)
 
     # depth data
     data_depth = []
-    for i in range(0,num_wells):
+    for i in range(0, num_wells):
         well_idx = i + 1
-        entities = np.repeat(f"Well 00{well_idx}",depth_steps)
-        depths = np.arange(0,depth_steps).tolist()
-        num_vals = np.sin(np.linspace(0,1,depth_steps))*100
+        entities = np.repeat(f"Well 00{well_idx}", depth_steps)
+        depths = np.arange(0, depth_steps).tolist()
+        num_vals = np.sin(np.linspace(0, 1, depth_steps)) * 100
         str_vals = np.random.choice(letters, depth_steps)
-        data_depth.append(pd.DataFrame({
-            entity_col: entities,
-            depth_col: depths,
-            depth_num_signal: num_vals,
-            depth_str_signal: str_vals,
-        }))
+        data_depth.append(
+            pd.DataFrame(
+                {
+                    entity_col: entities,
+                    depth_col: depths,
+                    depth_num_signal: num_vals,
+                    # depth_str_signal: str_vals,
+                }
+            )
+        )
     df_depth = pd.concat(data_depth, ignore_index=True)
 
     # save depth data
     api.save_table_data(df_depth)
 
     # load static signals
-    df_loaded = api.load_signals_data([stat_num_signal,
-                                       stat_str_signal,
-                                       ],
-                                      context=context)
+    df_loaded = api.load_signals_data(
+        [
+            stat_num_signal,
+            stat_str_signal,
+        ],
+        context=context,
+    )
     assert df_loaded.shape[0] >= num_wells + 1
 
     # load time signals
-    df_loaded = api.load_signals_data([time_num_signal,
-                                       time_str_signal],
-                                      context=context)
+    df_loaded = api.load_signals_data(
+        [time_num_signal, time_str_signal], context=context
+    )
     assert df_loaded.shape[0] >= num_wells * time_steps
 
     # load depth signals
-    df_loaded = api.load_signals_data([depth_num_signal,
-                                       depth_str_signal,
-                                      ],
-                                      context=context)
+    df_loaded = api.load_signals_data(
+        [
+            depth_num_signal,
+            # depth_str_signal,
+        ],
+        context=context,
+    )
     assert df_loaded.shape[0] >= num_wells * depth_steps
 
     # load static, time and depth signals
-    df_loaded = api.load_signals_data([stat_num_signal,
-                                       stat_str_signal,
-                                       time_num_signal,
-                                       time_str_signal,
-                                       depth_num_signal,
-                                       depth_str_signal,
-                                       ],
-                                      context=context)
+    df_loaded = api.load_signals_data(
+        [
+            stat_num_signal,
+            stat_str_signal,
+            time_num_signal,
+            time_str_signal,
+            depth_num_signal,
+            # depth_str_signal,
+        ],
+        context=context,
+    )
     assert df_loaded.shape[0] >= num_wells * time_steps * depth_steps
+
+    # delete signals
+    # for s in signals:
+    #     api.delete_signal(s)
```


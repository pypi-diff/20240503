# Comparing `tmp/dbt-synapse-1.8.0rc2.tar.gz` & `tmp/dbt_synapse-1.8.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-synapse-1.8.0rc2.tar", last modified: Mon Apr  8 19:48:06 2024, max compression
+gzip compressed data, was "dbt_synapse-1.8.0rc3.tar", last modified: Fri May  3 14:53:41 2024, max compression
```

## Comparing `dbt-synapse-1.8.0rc2.tar` & `dbt_synapse-1.8.0rc3.tar`

### file list

```diff
@@ -1,59 +1,64 @@
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.714302 dbt-synapse-1.8.0rc2/
--rw-r--r--   0 dataders   (502) staff       (20)     1087 2022-01-19 01:45:31.000000 dbt-synapse-1.8.0rc2/LICENSE
--rw-r--r--   0 dataders   (502) staff       (20)       47 2022-06-03 22:08:34.000000 dbt-synapse-1.8.0rc2/MANIFEST.in
--rw-r--r--   0 dataders   (502) staff       (20)     3574 2024-04-08 19:48:06.713995 dbt-synapse-1.8.0rc2/PKG-INFO
--rw-r--r--   0 dataders   (502) staff       (20)     2748 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/README.md
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.702317 dbt-synapse-1.8.0rc2/dbt/
--rw-r--r--   0 dataders   (502) staff       (20)       65 2022-01-19 01:45:31.000000 dbt-synapse-1.8.0rc2/dbt/__init__.py
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.702667 dbt-synapse-1.8.0rc2/dbt/adapters/
--rw-r--r--   0 dataders   (502) staff       (20)       65 2022-01-19 01:45:31.000000 dbt-synapse-1.8.0rc2/dbt/adapters/__init__.py
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.704379 dbt-synapse-1.8.0rc2/dbt/adapters/synapse/
--rw-r--r--   0 dataders   (502) staff       (20)      649 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/dbt/adapters/synapse/__init__.py
--rw-r--r--   0 dataders   (502) staff       (20)       21 2024-04-08 19:42:25.000000 dbt-synapse-1.8.0rc2/dbt/adapters/synapse/__version__.py
--rw-r--r--   0 dataders   (502) staff       (20)     3661 2024-04-08 19:37:58.000000 dbt-synapse-1.8.0rc2/dbt/adapters/synapse/synapse_adapter.py
--rw-r--r--   0 dataders   (502) staff       (20)      394 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/dbt/adapters/synapse/synapse_column.py
--rw-r--r--   0 dataders   (502) staff       (20)      153 2024-04-08 19:37:58.000000 dbt-synapse-1.8.0rc2/dbt/adapters/synapse/synapse_connection_manager.py
--rw-r--r--   0 dataders   (502) staff       (20)      202 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/dbt/adapters/synapse/synapse_credentials.py
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.704770 dbt-synapse-1.8.0rc2/dbt/include/
--rw-r--r--   0 dataders   (502) staff       (20)       65 2022-01-19 01:45:31.000000 dbt-synapse-1.8.0rc2/dbt/include/__init__.py
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.705194 dbt-synapse-1.8.0rc2/dbt/include/synapse/
--rw-r--r--   0 dataders   (502) staff       (20)       52 2022-01-19 01:45:31.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/__init__.py
--rw-r--r--   0 dataders   (502) staff       (20)       75 2022-06-03 22:08:34.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/dbt_project.yml
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.701265 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.708263 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/
--rw-r--r--   0 dataders   (502) staff       (20)     4776 2024-04-01 15:46:25.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/catalog.sql
--rw-r--r--   0 dataders   (502) staff       (20)     1896 2022-06-03 22:08:34.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/columns.sql
--rw-r--r--   0 dataders   (502) staff       (20)     6773 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/indexes.sql
--rw-r--r--   0 dataders   (502) staff       (20)      915 2022-12-02 19:06:04.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/metadata.sql
--rw-r--r--   0 dataders   (502) staff       (20)      302 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/persist_docs.sql
--rw-r--r--   0 dataders   (502) staff       (20)     2172 2024-04-01 15:46:25.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/relation.sql
--rw-r--r--   0 dataders   (502) staff       (20)     2325 2024-04-01 15:46:25.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/replace.sql
--rw-r--r--   0 dataders   (502) staff       (20)     1471 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/schema.sql
--rw-r--r--   0 dataders   (502) staff       (20)      661 2024-04-08 19:30:18.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/show.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.701192 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.701029 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.708929 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/materialized_view/
--rw-r--r--   0 dataders   (502) staff       (20)     1043 2024-04-01 15:46:25.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/materialized_view/create_materialized_view_as.sql
--rw-r--r--   0 dataders   (502) staff       (20)     5041 2024-04-01 15:46:25.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/materialized_view/materialized_view.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.709501 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/table/
--rw-r--r--   0 dataders   (502) staff       (20)     1715 2024-04-01 15:46:25.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 dataders   (502) staff       (20)      790 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/table/create_table_constraints.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.709805 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/view/
--rw-r--r--   0 dataders   (502) staff       (20)      439 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/view/create_view_as.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.710740 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/seeds/
--rw-r--r--   0 dataders   (502) staff       (20)     3205 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 dataders   (502) staff       (20)      200 2022-06-03 22:08:34.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/seeds/str_replace.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.711007 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/snapshots/
--rw-r--r--   0 dataders   (502) staff       (20)     1776 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/snapshots/snapshot.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.711923 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/utils/
--rw-r--r--   0 dataders   (502) staff       (20)     1911 2024-04-01 15:46:25.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/utils/date_spine.sql
--rw-r--r--   0 dataders   (502) staff       (20)     1456 2024-04-01 15:46:25.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/utils/generate_series.sql
--rw-r--r--   0 dataders   (502) staff       (20)      712 2024-03-14 16:14:27.000000 dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/utils/split_part.sql
-drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-04-08 19:48:06.713636 dbt-synapse-1.8.0rc2/dbt_synapse.egg-info/
--rw-r--r--   0 dataders   (502) staff       (20)     3574 2024-04-08 19:48:06.000000 dbt-synapse-1.8.0rc2/dbt_synapse.egg-info/PKG-INFO
--rw-r--r--   0 dataders   (502) staff       (20)     1797 2024-04-08 19:48:06.000000 dbt-synapse-1.8.0rc2/dbt_synapse.egg-info/SOURCES.txt
--rw-r--r--   0 dataders   (502) staff       (20)        1 2024-04-08 19:48:06.000000 dbt-synapse-1.8.0rc2/dbt_synapse.egg-info/dependency_links.txt
--rw-r--r--   0 dataders   (502) staff       (20)       21 2024-04-08 19:48:06.000000 dbt-synapse-1.8.0rc2/dbt_synapse.egg-info/requires.txt
--rw-r--r--   0 dataders   (502) staff       (20)        4 2024-04-08 19:48:06.000000 dbt-synapse-1.8.0rc2/dbt_synapse.egg-info/top_level.txt
--rw-r--r--   0 dataders   (502) staff       (20)       38 2024-04-08 19:48:06.714610 dbt-synapse-1.8.0rc2/setup.cfg
--rw-r--r--   0 dataders   (502) staff       (20)     2886 2024-04-08 19:37:58.000000 dbt-synapse-1.8.0rc2/setup.py
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.699549 dbt_synapse-1.8.0rc3/
+-rw-r--r--   0 dataders   (502) staff       (20)     1087 2022-01-19 01:45:31.000000 dbt_synapse-1.8.0rc3/LICENSE
+-rw-r--r--   0 dataders   (502) staff       (20)       47 2022-06-03 22:08:34.000000 dbt_synapse-1.8.0rc3/MANIFEST.in
+-rw-r--r--   0 dataders   (502) staff       (20)     3571 2024-05-03 14:53:41.699249 dbt_synapse-1.8.0rc3/PKG-INFO
+-rw-r--r--   0 dataders   (502) staff       (20)     2748 2024-03-14 16:14:27.000000 dbt_synapse-1.8.0rc3/README.md
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.687780 dbt_synapse-1.8.0rc3/dbt/
+-rw-r--r--   0 dataders   (502) staff       (20)       65 2022-01-19 01:45:31.000000 dbt_synapse-1.8.0rc3/dbt/__init__.py
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.688098 dbt_synapse-1.8.0rc3/dbt/adapters/
+-rw-r--r--   0 dataders   (502) staff       (20)       65 2022-01-19 01:45:31.000000 dbt_synapse-1.8.0rc3/dbt/adapters/__init__.py
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.690707 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/
+-rw-r--r--   0 dataders   (502) staff       (20)      649 2024-03-14 16:14:27.000000 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/__init__.py
+-rw-r--r--   0 dataders   (502) staff       (20)       21 2024-05-03 14:49:24.000000 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/__version__.py
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.691780 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/relation_configs/
+-rw-r--r--   0 dataders   (502) staff       (20)      138 2024-05-03 14:46:08.000000 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/relation_configs/__init__.py
+-rw-r--r--   0 dataders   (502) staff       (20)     2297 2024-05-03 14:46:08.000000 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/relation_configs/base.py
+-rw-r--r--   0 dataders   (502) staff       (20)      517 2024-05-03 14:46:08.000000 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/relation_configs/policies.py
+-rw-r--r--   0 dataders   (502) staff       (20)     3758 2024-05-03 14:46:08.000000 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/synapse_adapter.py
+-rw-r--r--   0 dataders   (502) staff       (20)      394 2024-03-14 16:14:27.000000 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/synapse_column.py
+-rw-r--r--   0 dataders   (502) staff       (20)      153 2024-04-29 18:28:35.000000 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/synapse_connection_manager.py
+-rw-r--r--   0 dataders   (502) staff       (20)      202 2024-03-14 16:14:27.000000 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/synapse_credentials.py
+-rw-r--r--   0 dataders   (502) staff       (20)      733 2024-05-03 14:46:08.000000 dbt_synapse-1.8.0rc3/dbt/adapters/synapse/synapse_relation.py
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.691949 dbt_synapse-1.8.0rc3/dbt/include/
+-rw-r--r--   0 dataders   (502) staff       (20)       65 2022-01-19 01:45:31.000000 dbt_synapse-1.8.0rc3/dbt/include/__init__.py
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.692296 dbt_synapse-1.8.0rc3/dbt/include/synapse/
+-rw-r--r--   0 dataders   (502) staff       (20)       52 2022-01-19 01:45:31.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/__init__.py
+-rw-r--r--   0 dataders   (502) staff       (20)       75 2022-06-03 22:08:34.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/dbt_project.yml
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.686705 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.694650 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/
+-rw-r--r--   0 dataders   (502) staff       (20)     4776 2024-04-01 15:46:25.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/catalog.sql
+-rw-r--r--   0 dataders   (502) staff       (20)     1896 2022-06-03 22:08:34.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/columns.sql
+-rw-r--r--   0 dataders   (502) staff       (20)     6773 2024-03-14 16:14:27.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/indexes.sql
+-rw-r--r--   0 dataders   (502) staff       (20)     1607 2024-05-03 14:46:08.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/metadata.sql
+-rw-r--r--   0 dataders   (502) staff       (20)      302 2024-03-14 16:14:27.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/persist_docs.sql
+-rw-r--r--   0 dataders   (502) staff       (20)     1980 2024-05-03 14:46:08.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/relation.sql
+-rw-r--r--   0 dataders   (502) staff       (20)     2325 2024-04-01 15:46:25.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/replace.sql
+-rw-r--r--   0 dataders   (502) staff       (20)     1471 2024-03-14 16:14:27.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/schema.sql
+-rw-r--r--   0 dataders   (502) staff       (20)      377 2024-04-15 19:58:56.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/show.sql
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.686633 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.686492 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.695062 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/materialized_view/
+-rw-r--r--   0 dataders   (502) staff       (20)      926 2024-05-03 14:46:08.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/materialized_view/create_materialized_view_as.sql
+-rw-r--r--   0 dataders   (502) staff       (20)     5041 2024-04-01 15:46:25.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/materialized_view/materialized_view.sql
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.695588 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/table/
+-rw-r--r--   0 dataders   (502) staff       (20)     1715 2024-04-01 15:46:25.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 dataders   (502) staff       (20)      766 2024-05-03 14:46:08.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/table/create_table_constraints.sql
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.695757 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/view/
+-rw-r--r--   0 dataders   (502) staff       (20)      415 2024-05-03 14:46:08.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/view/create_view_as.sql
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.696307 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/seeds/
+-rw-r--r--   0 dataders   (502) staff       (20)     3205 2024-03-14 16:14:27.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 dataders   (502) staff       (20)      200 2022-06-03 22:08:34.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/seeds/str_replace.sql
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.696569 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/snapshots/
+-rw-r--r--   0 dataders   (502) staff       (20)     1776 2024-03-14 16:14:27.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/snapshots/snapshot.sql
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.697386 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/utils/
+-rw-r--r--   0 dataders   (502) staff       (20)     1911 2024-04-01 15:46:25.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/utils/date_spine.sql
+-rw-r--r--   0 dataders   (502) staff       (20)     1456 2024-04-01 15:46:25.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/utils/generate_series.sql
+-rw-r--r--   0 dataders   (502) staff       (20)      712 2024-03-14 16:14:27.000000 dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/utils/split_part.sql
+drwxr-xr-x   0 dataders   (502) staff       (20)        0 2024-05-03 14:53:41.698873 dbt_synapse-1.8.0rc3/dbt_synapse.egg-info/
+-rw-r--r--   0 dataders   (502) staff       (20)     3571 2024-05-03 14:53:41.000000 dbt_synapse-1.8.0rc3/dbt_synapse.egg-info/PKG-INFO
+-rw-r--r--   0 dataders   (502) staff       (20)     1984 2024-05-03 14:53:41.000000 dbt_synapse-1.8.0rc3/dbt_synapse.egg-info/SOURCES.txt
+-rw-r--r--   0 dataders   (502) staff       (20)        1 2024-05-03 14:53:41.000000 dbt_synapse-1.8.0rc3/dbt_synapse.egg-info/dependency_links.txt
+-rw-r--r--   0 dataders   (502) staff       (20)       18 2024-05-03 14:53:41.000000 dbt_synapse-1.8.0rc3/dbt_synapse.egg-info/requires.txt
+-rw-r--r--   0 dataders   (502) staff       (20)        4 2024-05-03 14:53:41.000000 dbt_synapse-1.8.0rc3/dbt_synapse.egg-info/top_level.txt
+-rw-r--r--   0 dataders   (502) staff       (20)       38 2024-05-03 14:53:41.699597 dbt_synapse-1.8.0rc3/setup.cfg
+-rw-r--r--   0 dataders   (502) staff       (20)     2883 2024-05-03 14:46:08.000000 dbt_synapse-1.8.0rc3/setup.py
```

### Comparing `dbt-synapse-1.8.0rc2/LICENSE` & `dbt_synapse-1.8.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/PKG-INFO` & `dbt_synapse-1.8.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-synapse
-Version: 1.8.0rc2
+Version: 1.8.0rc3
 Summary: An Azure Synapse adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-synapse
 Author: Pradeep Srikakolapu, Nandan Hegde, Chaerin Lee, Alieu Sanneh, Anders Swanson, Sam Debruyn
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -12,15 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-fabric~=1.8.0rc2
+Requires-Dist: dbt-fabric==1.8.2
 
 # dbt-synapse
 
 [dbt](https://www.getdbt.com) adapter for Azure Synapse Dedicated SQL Pool (Azure Synapse Data Warehouse).
 
 The adapter supports dbt-core 0.18 or newer and follows the same versioning scheme.
 E.g. version 1.1.x of the adapter will be compatible with dbt-core 1.1.x.
```

### Comparing `dbt-synapse-1.8.0rc2/README.md` & `dbt_synapse-1.8.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/adapters/synapse/__init__.py` & `dbt_synapse-1.8.0rc3/dbt/adapters/synapse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/adapters/synapse/synapse_adapter.py` & `dbt_synapse-1.8.0rc3/dbt/adapters/synapse/synapse_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 from dbt.adapters.fabric import FabricAdapter
 from dbt.adapters.sql.impl import CREATE_SCHEMA_MACRO_NAME
 from dbt_common.contracts.constraints import ColumnLevelConstraint, ConstraintType
 from dbt_common.events.functions import fire_event
 
 from dbt.adapters.synapse.synapse_column import SynapseColumn
 from dbt.adapters.synapse.synapse_connection_manager import SynapseConnectionManager
+from dbt.adapters.synapse.synapse_relation import SynapseRelation
 
 
 class SynapseAdapter(FabricAdapter):
     ConnectionManager = SynapseConnectionManager
     Column = SynapseColumn
+    Relation = SynapseRelation
 
     def create_schema(self, relation: BaseRelation) -> None:
         relation = relation.without_identifier()
         fire_event(SchemaCreation(relation=_make_ref_key_dict(relation)))
         macro_name = CREATE_SCHEMA_MACRO_NAME
         kwargs = {
             "relation": relation,
```

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/catalog.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/columns.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/indexes.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/metadata.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/metadata.sql`

 * *Files 25% similar despite different names*

```diff
@@ -19,7 +19,25 @@
 
     from INFORMATION_SCHEMA.TABLES
     where table_schema like '{{ schema_relation.schema }}'
       and table_catalog like '{{ schema_relation.database }}'
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
+
+{% macro synapse__get_relation_without_caching(schema_relation) -%}
+  {% call statement('list_relations_without_caching', fetch_result=True) -%}
+    select
+      table_catalog as [database],
+      table_name as [name],
+      table_schema as [schema],
+      case when table_type = 'BASE TABLE' then 'table'
+           when table_type = 'VIEW' then 'view'
+           else table_type
+      end as table_type
+
+    from INFORMATION_SCHEMA.TABLES {{ information_schema_hints() }}
+    where table_schema like '{{ schema_relation.schema }}'
+    and table_name like '{{ schema_relation.identifier }}'
+  {% endcall %}
+  {{ return(load_result('list_relations_without_caching').table) }}
+{% endmacro %}
```

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/relation.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/relation.sql`

 * *Files 18% similar despite different names*

```diff
@@ -8,22 +8,22 @@
   {% if relation is not none %}
   {% if relation.type == 'view' or relation.type == 'materialized_view' -%}
     {% set object_id_type = 'V' %}
   {% elif relation.type == 'table'%}
     {% set object_id_type = 'U' %}
   {%- else -%} invalid target name
   {% endif %}
-    if object_id ('{{ relation.include(database=False) }}','{{ object_id_type }}') is not null
+    if object_id ('{{ relation }}','{{ object_id_type }}') is not null
     {% if relation.type == 'view' or relation.type == 'materialized_view' -%}
       begin
-      drop view {{ relation.include(database=False) }}
+      drop view {{ relation }}
       end
     {% elif relation.type == 'table' %}
       begin
-      drop {{ relation.type }} {{ relation.include(database=False) }}
+      drop {{ relation.type }} {{ relation }}
       end
     {% endif %}
   {% else %}
     -- no object to drop
     select 1 as nothing
   {% endif %}
 {% endmacro %}
@@ -35,25 +35,25 @@
   {% call statement('rename_relation') %}
     {{ synapse__rename_relation_script(from_relation, to_relation) }}
   {%- endcall %}
 {% endmacro %}
 
 {% macro synapse__rename_relation_script(from_relation, to_relation) -%}
   -- drop all object types with to_relation.identifier name, to avoid error "new name already in use...duplicate...not permitted"
-  if object_id ('{{ to_relation.include(database=False) }}','V') is not null
+  if object_id ('{{ to_relation }}','V') is not null
     begin
-    drop view {{ to_relation.include(database=False) }}
+    drop view {{ to_relation }}
     end
 
-  if object_id ('{{ to_relation.include(database=False) }}','U') is not null
+  if object_id ('{{ to_relation }}','U') is not null
     begin
-    drop table {{ to_relation.include(database=False) }}
+    drop table {{ to_relation }}
     end
 
-  rename object {{ from_relation.include(database=False) }} to {{ to_relation.identifier }}
+  rename object {{ from_relation }} to {{ to_relation.identifier }}
 {% endmacro %}
 
 {% macro synapse__truncate_relation(relation) %}
     {% call statement('truncate_relation') -%}
       truncate table {{ relation }}
     {%- endcall %}
 {% endmacro %}
```

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/replace.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/adapters/schema.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/materialized_view/create_materialized_view_as.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/materialized_view/create_materialized_view_as.sql`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-{% macro ref(model_name) %}
-
-    {% do return(builtins.ref(model_name).include(database=false)) %}
-
-{% endmacro %}
-
-
 {% macro synapse__get_replace_materialized_view_as_sql(relation, sql, existing_relation, backup_relation, intermediate_relation) %}
     {# Synapse does not have ALTER...RENAME function, so use synapse__rename_relation_script #}
 
     {%- set dist = config.get('dist', default="ROUND_ROBIN") -%}
     EXEC('
     CREATE materialized view [{{intermediate_relation.schema}}].[{{intermediate_relation.identifier}}]
     WITH ( DISTRIBUTION = {{dist}} )
```

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/materialized_view/materialized_view.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/materialized_view/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/table/create_table_as.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/models/table/create_table_constraints.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/models/table/create_table_constraints.sql`

 * *Files 11% similar despite different names*

```diff
@@ -8,10 +8,10 @@
     )
 {% endmacro %}
 
 {% macro synapse__build_model_constraints(relation) %}
   {# loop through user_provided_columns to create DDL with data types and constraints #}
     {%- set raw_model_constraints = adapter.render_raw_model_constraints(raw_constraints=model['constraints']) -%}
     {% for c in raw_model_constraints -%}
-        alter table {{ relation.include(database=False) }} {{c}};
+        alter table {{ relation }} {{c}};
     {% endfor -%}
 {% endmacro %}
```

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/seeds/helpers.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/materializations/snapshots/snapshot.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/utils/date_spine.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/utils/date_spine.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/utils/generate_series.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/utils/generate_series.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt/include/synapse/macros/utils/split_part.sql` & `dbt_synapse-1.8.0rc3/dbt/include/synapse/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-synapse-1.8.0rc2/dbt_synapse.egg-info/PKG-INFO` & `dbt_synapse-1.8.0rc3/dbt_synapse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-synapse
-Version: 1.8.0rc2
+Version: 1.8.0rc3
 Summary: An Azure Synapse adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-synapse
 Author: Pradeep Srikakolapu, Nandan Hegde, Chaerin Lee, Alieu Sanneh, Anders Swanson, Sam Debruyn
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -12,15 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-fabric~=1.8.0rc2
+Requires-Dist: dbt-fabric==1.8.2
 
 # dbt-synapse
 
 [dbt](https://www.getdbt.com) adapter for Azure Synapse Dedicated SQL Pool (Azure Synapse Data Warehouse).
 
 The adapter supports dbt-core 0.18 or newer and follows the same versioning scheme.
 E.g. version 1.1.x of the adapter will be compatible with dbt-core 1.1.x.
```

### Comparing `dbt-synapse-1.8.0rc2/dbt_synapse.egg-info/SOURCES.txt` & `dbt_synapse-1.8.0rc3/dbt_synapse.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 dbt/adapters/__init__.py
 dbt/adapters/synapse/__init__.py
 dbt/adapters/synapse/__version__.py
 dbt/adapters/synapse/synapse_adapter.py
 dbt/adapters/synapse/synapse_column.py
 dbt/adapters/synapse/synapse_connection_manager.py
 dbt/adapters/synapse/synapse_credentials.py
+dbt/adapters/synapse/synapse_relation.py
+dbt/adapters/synapse/relation_configs/__init__.py
+dbt/adapters/synapse/relation_configs/base.py
+dbt/adapters/synapse/relation_configs/policies.py
 dbt/include/__init__.py
 dbt/include/synapse/__init__.py
 dbt/include/synapse/dbt_project.yml
 dbt/include/synapse/macros/adapters/catalog.sql
 dbt/include/synapse/macros/adapters/columns.sql
 dbt/include/synapse/macros/adapters/indexes.sql
 dbt/include/synapse/macros/adapters/metadata.sql
```

### Comparing `dbt-synapse-1.8.0rc2/setup.py` & `dbt_synapse-1.8.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Nandan Hegde",
     "Chaerin Lee",
     "Alieu Sanneh",
     "Anders Swanson",
     "Sam Debruyn",
 ]
 dbt_version = "1.8"
-dbt_fabric_requirement = "dbt-fabric~=1.8.0rc2"
+dbt_fabric_requirement = "dbt-fabric==1.8.2"
 description = """An Azure Synapse adapter plugin for dbt"""
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
```


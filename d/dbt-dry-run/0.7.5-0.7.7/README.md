# Comparing `tmp/dbt_dry_run-0.7.5.tar.gz` & `tmp/dbt_dry_run-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_dry_run-0.7.5.tar", max compression
+gzip compressed data, was "dbt_dry_run-0.7.7.tar", max compression
```

## Comparing `dbt_dry_run-0.7.5.tar` & `dbt_dry_run-0.7.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    11356 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/LICENSE
--rw-r--r--   0        0        0    12787 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/README.md
--rw-r--r--   0        0        0        0 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/__init__.py
--rw-r--r--   0        0        0      110 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/__main__.py
--rw-r--r--   0        0        0        0 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/adapter/__init__.py
--rw-r--r--   0        0        0     2144 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/adapter/service.py
--rw-r--r--   0        0        0      122 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/adapter/utils.py
--rw-r--r--   0        0        0     4409 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/cli.py
--rw-r--r--   0        0        0     4153 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/columns_metadata.py
--rw-r--r--   0        0        0     1327 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/exception.py
--rw-r--r--   0        0        0     4212 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/execution.py
--rw-r--r--   0        0        0      715 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/flags.py
--rw-r--r--   0        0        0        0 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/linting/__init__.py
--rw-r--r--   0        0        0     1783 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/linting/column_linting.py
--rw-r--r--   0        0        0     4967 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/literals.py
--rw-r--r--   0        0        0      264 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/models/__init__.py
--rw-r--r--   0        0        0     4567 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/models/manifest.py
--rw-r--r--   0        0        0     2491 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/models/profile.py
--rw-r--r--   0        0        0      692 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/models/report.py
--rw-r--r--   0        0        0     2176 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/models/table.py
--rw-r--r--   0        0        0     1686 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/node_dispatch.py
--rw-r--r--   0        0        0     1343 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/node_runner/__init__.py
--rw-r--r--   0        0        0     7350 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/node_runner/incremental_runner.py
--rw-r--r--   0        0        0      728 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/node_runner/node_test_runner.py
--rw-r--r--   0        0        0     1808 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/node_runner/seed_runner.py
--rw-r--r--   0        0        0     3826 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/node_runner/snapshot_runner.py
--rw-r--r--   0        0        0     1704 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/node_runner/source_runner.py
--rw-r--r--   0        0        0      973 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/node_runner/table_runner.py
--rw-r--r--   0        0        0     1099 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/node_runner/view_runner.py
--rw-r--r--   0        0        0     4679 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/result_reporter.py
--rw-r--r--   0        0        0     2468 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/results.py
--rw-r--r--   0        0        0     4899 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/scheduler.py
--rw-r--r--   0        0        0      955 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/sql_runner/__init__.py
--rw-r--r--   0        0        0     3435 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/sql_runner/big_query_sql_runner.py
--rw-r--r--   0        0        0        0 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/__init__.py
--rw-r--r--   0        0        0      231 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/conftest.py
--rw-r--r--   0        0        0        0 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/linting/__init__.py
--rw-r--r--   0        0        0     1846 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/linting/test_column_linting.py
--rw-r--r--   0        0        0     1691 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/models/test_manifest.py
--rw-r--r--   0        0        0     2761 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/models/test_profile.py
--rw-r--r--   0        0        0        0 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/__init__.py
--rw-r--r--   0        0        0    19093 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_incremental_runner.py
--rw-r--r--   0        0        0     1633 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_node_runner.py
--rw-r--r--   0        0        0     3406 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_seed_runner.py
--rw-r--r--   0        0        0     9693 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_snapshot_runner.py
--rw-r--r--   0        0        0     1238 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_source_runner.py
--rw-r--r--   0        0        0     4400 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_table_runner.py
--rw-r--r--   0        0        0     2938 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_test_runner.py
--rw-r--r--   0        0        0     5364 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_view_runner.py
--rw-r--r--   0        0        0        0 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/sql_runner/__init__.py
--rw-r--r--   0        0        0     4436 2024-01-10 13:54:13.600319 dbt_dry_run-0.7.5/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py
--rw-r--r--   0        0        0     5503 2024-01-10 13:54:13.604319 dbt_dry_run-0.7.5/dbt_dry_run/test/test_columns_metadata.py
--rw-r--r--   0        0        0     2678 2024-01-10 13:54:13.604319 dbt_dry_run-0.7.5/dbt_dry_run/test/test_execution.py
--rw-r--r--   0        0        0     8855 2024-01-10 13:54:13.604319 dbt_dry_run-0.7.5/dbt_dry_run/test/test_literals.py
--rw-r--r--   0        0        0     2337 2024-01-10 13:54:13.604319 dbt_dry_run-0.7.5/dbt_dry_run/test/test_result_reporter.py
--rw-r--r--   0        0        0     3831 2024-01-10 13:54:13.604319 dbt_dry_run-0.7.5/dbt_dry_run/test/test_scheduler.py
--rw-r--r--   0        0        0     2631 2024-01-10 13:54:13.604319 dbt_dry_run-0.7.5/dbt_dry_run/test/utils.py
--rw-r--r--   0        0        0      167 2024-01-10 13:54:13.604319 dbt_dry_run-0.7.5/dbt_dry_run/version.py
--rw-r--r--   0        0        0     2133 2024-01-10 13:54:13.608319 dbt_dry_run-0.7.5/pyproject.toml
--rw-r--r--   0        0        0    13733 1970-01-01 00:00:00.000000 dbt_dry_run-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/LICENSE
+-rw-r--r--   0        0        0    12787 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/__init__.py
+-rw-r--r--   0        0        0      110 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/adapter/__init__.py
+-rw-r--r--   0        0        0     2144 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/adapter/service.py
+-rw-r--r--   0        0        0      122 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/adapter/utils.py
+-rw-r--r--   0        0        0     4409 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/cli.py
+-rw-r--r--   0        0        0     4153 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/columns_metadata.py
+-rw-r--r--   0        0        0     1327 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/exception.py
+-rw-r--r--   0        0        0     4212 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/execution.py
+-rw-r--r--   0        0        0      715 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/flags.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/linting/__init__.py
+-rw-r--r--   0        0        0     1783 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/linting/column_linting.py
+-rw-r--r--   0        0        0     4967 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/literals.py
+-rw-r--r--   0        0        0      264 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/models/__init__.py
+-rw-r--r--   0        0        0     4567 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/models/manifest.py
+-rw-r--r--   0        0        0     2491 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/models/profile.py
+-rw-r--r--   0        0        0      733 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/models/report.py
+-rw-r--r--   0        0        0     2176 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/models/table.py
+-rw-r--r--   0        0        0     1686 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_dispatch.py
+-rw-r--r--   0        0        0     1494 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/__init__.py
+-rw-r--r--   0        0        0     7654 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/incremental_runner.py
+-rw-r--r--   0        0        0      860 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/node_test_runner.py
+-rw-r--r--   0        0        0     1927 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/seed_runner.py
+-rw-r--r--   0        0        0     4089 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/snapshot_runner.py
+-rw-r--r--   0        0        0     1798 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/source_runner.py
+-rw-r--r--   0        0        0     1066 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/table_runner.py
+-rw-r--r--   0        0        0     1192 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/node_runner/view_runner.py
+-rw-r--r--   0        0        0     4747 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/result_reporter.py
+-rw-r--r--   0        0        0     2670 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/results.py
+-rw-r--r--   0        0        0     4899 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/scheduler.py
+-rw-r--r--   0        0        0      970 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/sql_runner/__init__.py
+-rw-r--r--   0        0        0     3578 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/sql_runner/big_query_sql_runner.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/test/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/test/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/test/linting/__init__.py
+-rw-r--r--   0        0        0     1846 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/test/linting/test_column_linting.py
+-rw-r--r--   0        0        0     1691 2024-05-03 13:02:59.722599 dbt_dry_run-0.7.7/dbt_dry_run/test/models/test_manifest.py
+-rw-r--r--   0        0        0     2761 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/models/test_profile.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/__init__.py
+-rw-r--r--   0        0        0    19372 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_incremental_runner.py
+-rw-r--r--   0        0        0     1633 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_node_runner.py
+-rw-r--r--   0        0        0     3406 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_seed_runner.py
+-rw-r--r--   0        0        0     9714 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_snapshot_runner.py
+-rw-r--r--   0        0        0     1238 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_source_runner.py
+-rw-r--r--   0        0        0     4896 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_table_runner.py
+-rw-r--r--   0        0        0     2941 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_test_runner.py
+-rw-r--r--   0        0        0     5886 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_view_runner.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/sql_runner/__init__.py
+-rw-r--r--   0        0        0     4439 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py
+-rw-r--r--   0        0        0     5503 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/test_columns_metadata.py
+-rw-r--r--   0        0        0     2678 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/test_execution.py
+-rw-r--r--   0        0        0     8855 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/test_literals.py
+-rw-r--r--   0        0        0     2442 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/test_result_reporter.py
+-rw-r--r--   0        0        0     3831 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/test_scheduler.py
+-rw-r--r--   0        0        0     2631 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/test/utils.py
+-rw-r--r--   0        0        0      167 2024-05-03 13:02:59.726600 dbt_dry_run-0.7.7/dbt_dry_run/version.py
+-rw-r--r--   0        0        0     2171 2024-05-03 13:02:59.734599 dbt_dry_run-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0    13728 1970-01-01 00:00:00.000000 dbt_dry_run-0.7.7/PKG-INFO
```

### Comparing `dbt_dry_run-0.7.5/LICENSE` & `dbt_dry_run-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/README.md` & `dbt_dry_run-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/adapter/service.py` & `dbt_dry_run-0.7.7/dbt_dry_run/adapter/service.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/cli.py` & `dbt_dry_run-0.7.7/dbt_dry_run/cli.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/columns_metadata.py` & `dbt_dry_run-0.7.7/dbt_dry_run/columns_metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/exception.py` & `dbt_dry_run-0.7.7/dbt_dry_run/exception.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/execution.py` & `dbt_dry_run-0.7.7/dbt_dry_run/execution.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/flags.py` & `dbt_dry_run-0.7.7/dbt_dry_run/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/linting/column_linting.py` & `dbt_dry_run-0.7.7/dbt_dry_run/linting/column_linting.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/literals.py` & `dbt_dry_run-0.7.7/dbt_dry_run/literals.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/models/manifest.py` & `dbt_dry_run-0.7.7/dbt_dry_run/models/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/models/profile.py` & `dbt_dry_run-0.7.7/dbt_dry_run/models/profile.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/models/report.py` & `dbt_dry_run-0.7.7/dbt_dry_run/models/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 class ReportNode(BaseModel):
     unique_id: str
     success: bool
     status: DryRunStatus
     error_message: Optional[str]
     table: Optional[Table]
+    total_bytes_processed: Optional[int]
     linting_status: LintingStatus
     linting_errors: List[ReportLintingError]
 
 
 class Report(BaseModel):
     success: bool
     execution_time: float
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/models/table.py` & `dbt_dry_run-0.7.7/dbt_dry_run/models/table.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/node_dispatch.py` & `dbt_dry_run-0.7.7/dbt_dry_run/node_dispatch.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/node_runner/__init__.py` & `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,17 +26,22 @@
         node_compiled = node.compiled
         if not node_compiled:
             if not flags.SKIP_NOT_COMPILED:
                 return DryRunResult(
                     node=node,
                     table=None,
                     status=DryRunStatus.FAILURE,
+                    total_bytes_processed=0,
                     exception=NotCompiledException(
                         f"Node {node.unique_id} was not compiled"
                     ),
                 )
             else:
                 return DryRunResult(
-                    node, table=None, status=DryRunStatus.SKIPPED, exception=None
+                    node,
+                    table=None,
+                    status=DryRunStatus.SKIPPED,
+                    total_bytes_processed=0,
+                    exception=None,
                 )
         else:
             return None
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/node_runner/incremental_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/incremental_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,26 +59,31 @@
     )
     target_table_field_names = set([field.name for field in target_table.fields])
     added_fields = predicted_table_field_names.difference(target_table_field_names)
     removed_fields = target_table_field_names.difference(predicted_table_field_names)
     schema_changed = added_fields or removed_fields
     table: Optional[Table] = target_table
     status = dry_run_result.status
+    total_bytes_processed = dry_run_result.total_bytes_processed
     exception = dry_run_result.exception
     if schema_changed:
         table = None
         status = DryRunStatus.FAILURE
         msg = (
             f"Incremental model has changed schemas. "
             f"Fields added: {added_fields}, "
             f"Fields removed: {removed_fields}"
         )
         exception = SchemaChangeException(msg)
     return DryRunResult(
-        node=dry_run_result.node, table=table, status=status, exception=exception
+        node=dry_run_result.node,
+        table=table,
+        status=status,
+        total_bytes_processed=total_bytes_processed,
+        exception=exception,
     )
 
 
 ON_SCHEMA_CHANGE_TABLE_HANDLER: Dict[
     OnSchemaChange, Callable[[DryRunResult, Table], DryRunResult]
 ] = {
     OnSchemaChange.IGNORE: ignore_handler,
@@ -139,19 +144,21 @@
         common_field_names = get_common_field_names(initial_result.table, target_table)
         if not common_field_names:
             return initial_result
         sql_statement_with_merge = get_merge_sql(
             node, common_field_names, sql_statement
         )
         sql_statement = self._modify_sql(node, sql_statement_with_merge)
-        status, model_schema, exception = self._sql_runner.query(sql_statement)
+        status, model_schema, total_bytes_processed, exception = self._sql_runner.query(
+            sql_statement
+        )
         if status == DryRunStatus.SUCCESS:
             return initial_result
         else:
-            return DryRunResult(node, None, status, exception)
+            return DryRunResult(node, None, status, total_bytes_processed, exception)
 
     def _modify_sql(self, node: Node, sql_statement: str) -> str:
         if node.config.sql_header:
             sql_statement = f"{node.config.sql_header}\n{sql_statement}"
 
         if node.config.partition_by and "_dbt_max_partition" in node.compiled_code:
             dbt_max_partition_declaration = (
@@ -168,19 +175,23 @@
             return node.config.full_refresh
         return flags.FULL_REFRESH
 
     def run(self, node: Node) -> DryRunResult:
         try:
             sql_with_literals = insert_dependant_sql_literals(node, self._results)
         except UpstreamFailedException as e:
-            return DryRunResult(node, None, DryRunStatus.FAILURE, e)
+            return DryRunResult(node, None, DryRunStatus.FAILURE, 0, e)
         run_sql = self._modify_sql(node, sql_with_literals)
-        status, model_schema, exception = self._sql_runner.query(run_sql)
+        status, model_schema, total_bytes_processed, exception = self._sql_runner.query(
+            run_sql
+        )
 
-        result = DryRunResult(node, model_schema, status, exception)
+        result = DryRunResult(
+            node, model_schema, status, total_bytes_processed, exception
+        )
 
         full_refresh = self._get_full_refresh_config(node)
 
         if result.status == DryRunStatus.SUCCESS and not full_refresh:
             target_table = self._sql_runner.get_node_schema(node)
             if target_table:
                 on_schema_change = node.config.on_schema_change or OnSchemaChange.IGNORE
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/node_runner/node_test_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/node_test_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,13 +6,20 @@
 
 
 class NodeTestRunner(NodeRunner):
     def run(self, node: Node) -> DryRunResult:
         try:
             run_sql = insert_dependant_sql_literals(node, self._results)
         except UpstreamFailedException as e:
-            return DryRunResult(node, None, DryRunStatus.FAILURE, e)
+            return DryRunResult(node, None, DryRunStatus.FAILURE, 0, e)
 
-        status, predicted_table, exception = self._sql_runner.query(run_sql)
+        (
+            status,
+            predicted_table,
+            total_bytes_processed,
+            exception,
+        ) = self._sql_runner.query(run_sql)
 
-        result = DryRunResult(node, predicted_table, status, exception)
+        result = DryRunResult(
+            node, predicted_table, status, total_bytes_processed, exception
+        )
         return result
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/node_runner/seed_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/seed_runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,21 +27,26 @@
             if new_type is None:
                 msg = f"Unknown Big Query schema for seed '{node.unique_id}' Column '{column.name}'"
                 exception = UnknownSchemaException(msg)
                 return DryRunResult(
                     node=node,
                     table=None,
                     status=DryRunStatus.FAILURE,
+                    total_bytes_processed=0,
                     exception=exception,
                 )
             new_field = TableField(
                 name=column.name, type=BigQueryFieldType[new_type.upper()]
             )
             fields.append(new_field)
 
         schema = Table(fields=fields)
         return DryRunResult(
-            node=node, table=schema, status=DryRunStatus.SUCCESS, exception=None
+            node=node,
+            table=schema,
+            status=DryRunStatus.SUCCESS,
+            total_bytes_processed=0,
+            exception=None,
         )
 
     def validate_node(self, node: Node) -> Optional[DryRunResult]:
         return None
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/node_runner/snapshot_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/snapshot_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,47 +52,57 @@
             exception = SnapshotConfigException(
                 f"Missing `unique_key` column '{node.config.unique_key}'"
             )
             return DryRunResult(
                 node=result.node,
                 table=result.table,
                 status=DryRunStatus.FAILURE,
+                total_bytes_processed=0,
                 exception=exception,
             )
         if node.config.strategy == "timestamp":
             if node.config.updated_at not in result.table.field_names:
                 exception = SnapshotConfigException(
                     f"Missing `updated_at` column '{node.config.updated_at}'"
                 )
                 return DryRunResult(
                     node=result.node,
                     table=result.table,
                     status=DryRunStatus.FAILURE,
+                    total_bytes_processed=0,
                     exception=exception,
                 )
         elif node.config.strategy == "check":
             if _check_cols_missing(node, result.table):
                 exception = SnapshotConfigException(
                     f"Missing `check_cols` '{node.config.check_cols}'"
                 )
                 return DryRunResult(
                     node=result.node,
                     table=result.table,
                     status=DryRunStatus.FAILURE,
+                    total_bytes_processed=0,
                     exception=exception,
                 )
         else:
             raise ValueError(f"Unknown snapshot strategy: '{node.config.strategy}'")
         return result
 
     def run(self, node: Node) -> DryRunResult:
         try:
             run_sql = insert_dependant_sql_literals(node, self._results)
         except UpstreamFailedException as e:
-            return DryRunResult(node, None, DryRunStatus.FAILURE, e)
+            return DryRunResult(node, None, DryRunStatus.FAILURE, 0, e)
 
-        status, predicted_table, exception = self._sql_runner.query(run_sql)
-        result = DryRunResult(node, predicted_table, status, exception)
+        (
+            status,
+            predicted_table,
+            total_bytes_processed,
+            exception,
+        ) = self._sql_runner.query(run_sql)
+        result = DryRunResult(
+            node, predicted_table, status, total_bytes_processed, exception
+        )
         if result.status == DryRunStatus.SUCCESS and result.table:
             result.table.fields = [*result.table.fields, *DBT_SNAPSHOT_FIELDS]
             result = self._validate_snapshot_config(node, result)
         return result
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/node_runner/source_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/source_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from dbt_dry_run.results import DryRunResult, DryRunStatus
 
 
 class SourceRunner(NodeRunner):
     def run(self, node: Node) -> DryRunResult:
         exception: Optional[Exception] = None
         predicted_table: Optional[Table] = None
+        total_bytes_processed: Optional[int] = 0
         status = DryRunStatus.SUCCESS
         if node.is_external_source():
             external_config = cast(ExternalConfig, node.external)
             try:
                 # Use columns schema if dry_run_columns is not specified
                 columns_to_map = (
                     external_config.dry_run_columns_map
@@ -33,11 +34,13 @@
         else:
             if not self._sql_runner.node_exists(node):
                 status = DryRunStatus.FAILURE
                 exception = SourceMissingException(
                     f"Could not find source in target environment for node '{node.unique_id}'"
                 )
 
-        return DryRunResult(node, predicted_table, status, exception)
+        return DryRunResult(
+            node, predicted_table, status, total_bytes_processed, exception
+        )
 
     def validate_node(self, node: Node) -> Optional[DryRunResult]:
         return None
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/node_runner/table_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/table_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,18 @@
             sql_statement = f"{node.config.sql_header}\n{sql_statement}"
         return sql_statement
 
     def run(self, node: Node) -> DryRunResult:
         try:
             run_sql = insert_dependant_sql_literals(node, self._results)
         except UpstreamFailedException as e:
-            return DryRunResult(node, None, DryRunStatus.FAILURE, e)
+            return DryRunResult(node, None, DryRunStatus.FAILURE, 0, e)
 
         run_sql = self._modify_sql(node, run_sql)
-        status, model_schema, exception = self._sql_runner.query(run_sql)
+        status, model_schema, total_bytes_processed, exception = self._sql_runner.query(
+            run_sql
+        )
 
-        result = DryRunResult(node, model_schema, status, exception)
+        result = DryRunResult(
+            node, model_schema, status, total_bytes_processed, exception
+        )
         return result
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/node_runner/view_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/node_runner/view_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,18 @@
             sql_statement = f"{node.config.sql_header}\n{sql_statement}"
         return sql_statement
 
     def run(self, node: Node) -> DryRunResult:
         try:
             run_sql = insert_dependant_sql_literals(node, self._results)
         except UpstreamFailedException as e:
-            return DryRunResult(node, None, DryRunStatus.FAILURE, e)
+            return DryRunResult(node, None, DryRunStatus.FAILURE, 0, e)
 
         run_sql = self._modify_sql(node, run_sql)
-        status, model_schema, exception = self._sql_runner.query(run_sql)
+        status, model_schema, total_bytes_processed, exception = self._sql_runner.query(
+            run_sql
+        )
 
-        result = DryRunResult(node, model_schema, status, exception)
+        result = DryRunResult(
+            node, model_schema, status, total_bytes_processed, exception
+        )
         return result
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/result_reporter.py` & `dbt_dry_run-0.7.7/dbt_dry_run/result_reporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,15 @@
             )
             new_node = ReportNode(
                 unique_id=result.node.unique_id,
                 success=result.status == DryRunStatus.SUCCESS,
                 status=result.status,
                 error_message=exception_type,
                 table=result.table,
+                total_bytes_processed=result.total_bytes_processed,
                 linting_status=result.linting_status,
                 linting_errors=_map_column_errors(result.linting_errors),
             )
             report_nodes.append(new_node)
 
             node_count += 1
             if not new_node.success or new_node.linting_status == LintingStatus.FAILURE:
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/results.py` & `dbt_dry_run-0.7.7/dbt_dry_run/results.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,32 +27,38 @@
 
 
 @dataclass(frozen=True)
 class DryRunResult:
     node: Node
     table: Optional[Table]
     status: DryRunStatus
+    total_bytes_processed: Optional[int]
     exception: Optional[Exception]
     linting_status: LintingStatus = LintingStatus.SKIPPED
     linting_errors: List[LintingError] = field(default_factory=lambda: [])
 
     def replace_table(self, table: Table) -> "DryRunResult":
         return DryRunResult(
-            node=self.node, table=table, status=self.status, exception=self.exception
+            node=self.node,
+            table=table,
+            status=self.status,
+            total_bytes_processed=self.total_bytes_processed,
+            exception=self.exception,
         )
 
     def with_linting_errors(self, linting_errors: List[LintingError]) -> "DryRunResult":
         if linting_errors:
             linting_status = LintingStatus.FAILURE
         else:
             linting_status = LintingStatus.SUCCESS
         return DryRunResult(
             node=self.node,
             table=self.table,
             status=self.status,
+            total_bytes_processed=self.total_bytes_processed,
             exception=self.exception,
             linting_errors=linting_errors,
             linting_status=linting_status,
         )
 
 
 class Results:
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/scheduler.py` & `dbt_dry_run-0.7.7/dbt_dry_run/scheduler.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/sql_runner/__init__.py` & `dbt_dry_run-0.7.7/dbt_dry_run/sql_runner/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,14 @@
     @abstractmethod
     def get_node_schema(self, node: Node) -> Optional[Table]:
         ...
 
     @abstractmethod
     def query(
         self, sql: str
-    ) -> Tuple[DryRunStatus, Optional[Table], Optional[Exception]]:
+    ) -> Tuple[DryRunStatus, Optional[Table], Optional[int], Optional[Exception]]:
         ...
 
     def convert_agate_type(
         self, agate_table: agate.Table, col_idx: int
     ) -> Optional[str]:
         return self._project.adapter.convert_agate_type(agate_table, col_idx)
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/sql_runner/big_query_sql_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/sql_runner/big_query_sql_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,28 +54,30 @@
     @retry(
         retry=retry_if_exception_type(BadRequest),
         stop=stop_after_attempt(MAX_ATTEMPT_NUMBER),
         wait=wait_exponential(multiplier=0.5, min=0.5, max=10),
     )
     def query(
         self, sql: str
-    ) -> Tuple[DryRunStatus, Optional[Table], Optional[Exception]]:
+    ) -> Tuple[DryRunStatus, Optional[Table], Optional[int], Optional[Exception]]:
         exception = None
         table = None
+        total_bytes_processed = None
         client = self.get_client()
         try:
             query_job = client.query(sql, job_config=self.JOB_CONFIG)
             table = self.get_schema_from_schema_fields(query_job.schema or [])
+            total_bytes_processed = query_job.total_bytes_processed
             status = DryRunStatus.SUCCESS
         except (Forbidden, BadRequest, NotFound) as e:
             status = DryRunStatus.FAILURE
             if QUERY_TIMED_OUT in str(e):
                 raise
             exception = e
-        return status, table, exception
+        return status, table, total_bytes_processed, exception
 
     @staticmethod
     def get_schema_from_schema_fields(schema_fields: List[SchemaField]) -> Table:
         def _map_schema_fields_to_table_field(schema_field: SchemaField) -> TableField:
             try:
                 parsed_fields = (
                     BigQuerySQLRunner.get_schema_from_schema_fields(
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/linting/test_column_linting.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/linting/test_column_linting.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/models/test_manifest.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/models/test_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/models/test_profile.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/models/test_profile.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_incremental_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_incremental_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         TableField(
             name="a",
             type=BigQueryFieldType.STRING,
         )
     ]
 )
 
+A_TOTAL_BYTES_PROCESSED = 1000
+
 A_NODE = SimpleNode(
     unique_id="node1", depends_on=[], resource_type=ManifestScheduler.MODEL
 ).to_node()
 
 
 def get_mock_sql_runner_with_all_string_columns(
     model_names: List[str], target_names: Optional[List[str]]
@@ -54,25 +56,30 @@
     return get_mock_sql_runner_with(model_schema, target_schema)
 
 
 def get_mock_sql_runner_with(
     model_schema: Table, target_schema: Optional[Table]
 ) -> MagicMock:
     mock_sql_runner = MagicMock()
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, model_schema, None)
+    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, model_schema, 0, None)
     mock_sql_runner.get_node_schema.return_value = target_schema
     return mock_sql_runner
 
 
 def test_partitioned_incremental_model_declares_dbt_max_partition_variable() -> None:
     dbt_max_partition_declaration = (
         "declare _dbt_max_partition timestamp default CURRENT_TIMESTAMP();"
     )
     mock_sql_runner = MagicMock()
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, A_SIMPLE_TABLE, None)
+    mock_sql_runner.query.return_value = (
+        DryRunStatus.SUCCESS,
+        A_SIMPLE_TABLE,
+        A_TOTAL_BYTES_PROCESSED,
+        None,
+    )
 
     node = SimpleNode(
         unique_id="node1",
         depends_on=[],
         resource_type=ManifestScheduler.MODEL,
         table_config=NodeConfig(
             materialized="incremental",
@@ -459,15 +466,20 @@
     mock_sql_runner.get_node_schema.assert_called_with(
         node_with_full_refresh_set_to_false
     )
 
 
 def test_model_with_sql_header_executes_header_first() -> None:
     mock_sql_runner = MagicMock()
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, A_SIMPLE_TABLE, None)
+    mock_sql_runner.query.return_value = (
+        DryRunStatus.SUCCESS,
+        A_SIMPLE_TABLE,
+        A_TOTAL_BYTES_PROCESSED,
+        None,
+    )
 
     pre_header_value = "DECLARE x INT64;"
 
     node = SimpleNode(
         unique_id="node1", depends_on=[], resource_type=ManifestScheduler.MODEL
     ).to_node()
     node.depends_on.deep_nodes = []
@@ -488,15 +500,19 @@
         fields=[
             TableField(name="col_1", type=BigQueryFieldType.STRING),
             TableField(name="col_2", type=BigQueryFieldType.STRING),
             TableField(name="col_3", type=BigQueryFieldType.STRING),
         ]
     )
     dry_run_result = DryRunResult(
-        node=A_NODE, status=DryRunStatus.SUCCESS, table=model_table, exception=None
+        node=A_NODE,
+        status=DryRunStatus.SUCCESS,
+        table=model_table,
+        total_bytes_processed=0,
+        exception=None,
     )
     target_table = Table(
         fields=[
             TableField(name="col_2", type=BigQueryFieldType.STRING),
             TableField(name="col_1", type=BigQueryFieldType.STRING),
         ]
     )
@@ -518,15 +534,19 @@
         fields=[
             TableField(name="col_3", type=BigQueryFieldType.STRING),
             TableField(name="col_2", type=BigQueryFieldType.STRING),
             TableField(name="col_4", type=BigQueryFieldType.STRING),
         ]
     )
     dry_run_result = DryRunResult(
-        node=A_NODE, status=DryRunStatus.SUCCESS, table=model_table, exception=None
+        node=A_NODE,
+        status=DryRunStatus.SUCCESS,
+        table=model_table,
+        total_bytes_processed=0,
+        exception=None,
     )
     target_table = Table(
         fields=[
             TableField(name="col_1", type=BigQueryFieldType.STRING),
             TableField(name="col_2", type=BigQueryFieldType.STRING),
             TableField(name="col_3", type=BigQueryFieldType.STRING),
         ]
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_node_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_node_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_seed_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_seed_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_snapshot_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_snapshot_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         fields=[
             TableField(
                 name="a",
                 type=BigQueryFieldType.STRING,
             )
         ]
     )
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, None)
+    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, 0, None)
 
     node = SimpleNode(
         unique_id="node1",
         depends_on=[],
         resource_type=ManifestScheduler.SNAPSHOT,
         table_config=NodeConfig(
             unique_key="a", strategy="check", check_cols="all", materialized="snapshot"
@@ -72,15 +72,15 @@
         fields=[
             TableField(
                 name="a",
                 type=BigQueryFieldType.STRING,
             )
         ]
     )
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, None)
+    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, 0, None)
 
     node = SimpleNode(
         unique_id="node1",
         depends_on=[],
         resource_type=ManifestScheduler.SNAPSHOT,
         table_config=NodeConfig(
             unique_key="a_missing_column",
@@ -110,15 +110,15 @@
             ),
             TableField(
                 name="b",
                 type=BigQueryFieldType.STRING,
             ),
         ]
     )
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, None)
+    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, 0, None)
 
     node = SimpleNode(
         unique_id="node1",
         depends_on=[],
         resource_type=ManifestScheduler.SNAPSHOT,
         table_config=NodeConfig(
             unique_key="a",
@@ -148,15 +148,15 @@
         fields=[
             TableField(
                 name="a",
                 type=BigQueryFieldType.STRING,
             )
         ]
     )
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, None)
+    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, 0, None)
 
     node = SimpleNode(
         unique_id="node1",
         depends_on=[],
         resource_type=ManifestScheduler.SNAPSHOT,
         table_config=NodeConfig(
             unique_key="a",
@@ -183,15 +183,15 @@
             TableField(
                 name="a",
                 type=BigQueryFieldType.STRING,
             ),
             TableField(name="last_updated_col", type=BigQueryFieldType.TIMESTAMP),
         ]
     )
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, None)
+    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, 0, None)
 
     node = SimpleNode(
         unique_id="node1",
         depends_on=[],
         resource_type=ManifestScheduler.SNAPSHOT,
         table_config=NodeConfig(
             unique_key="a",
@@ -218,15 +218,15 @@
             TableField(
                 name="a",
                 type=BigQueryFieldType.STRING,
             ),
             TableField(name="last_updated_col", type=BigQueryFieldType.TIMESTAMP),
         ]
     )
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, None)
+    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, 0, None)
 
     node = SimpleNode(
         unique_id="node1",
         depends_on=[],
         resource_type=ManifestScheduler.SNAPSHOT,
         table_config=NodeConfig(
             unique_key="a",
@@ -257,15 +257,15 @@
             TableField(
                 name="a",
                 type=BigQueryFieldType.STRING,
             ),
             TableField(name="last_updated_col", type=BigQueryFieldType.TIMESTAMP),
         ]
     )
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, None)
+    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, 0, None)
 
     node = SimpleNode(
         unique_id="node1",
         depends_on=[],
         resource_type=ManifestScheduler.SNAPSHOT,
         table_config=NodeConfig(
             unique_key=["a", "b"],
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_source_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_source_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_table_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_table_runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,26 +15,33 @@
         TableField(
             name="a",
             type=BigQueryFieldType.STRING,
         )
     ]
 )
 
+A_TOTAL_BYTES_PROCESSED = 1000
+
 
 def test_model_with_no_dependencies_runs_sql() -> None:
     mock_sql_runner = MagicMock()
     expected_table = Table(
         fields=[
             TableField(
                 name="a",
                 type=BigQueryFieldType.STRING,
             )
         ]
     )
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, None)
+    mock_sql_runner.query.return_value = (
+        DryRunStatus.SUCCESS,
+        expected_table,
+        A_TOTAL_BYTES_PROCESSED,
+        None,
+    )
 
     node = SimpleNode(
         unique_id="node1", depends_on=[], resource_type=ManifestScheduler.SEED
     ).to_node()
     node.depends_on.deep_nodes = []
 
     results = Results()
@@ -42,19 +49,25 @@
     model_runner = TableRunner(mock_sql_runner, results)
 
     result = model_runner.run(node)
     mock_sql_runner.query.assert_called_with(node.compiled_code)
     assert result.status == DryRunStatus.SUCCESS
     assert result.table
     assert result.table.fields[0].name == expected_table.fields[0].name
+    assert result.total_bytes_processed == A_TOTAL_BYTES_PROCESSED
 
 
 def test_model_with_failed_dependency_raises_upstream_failed_exception() -> None:
     mock_sql_runner = MagicMock()
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, A_SIMPLE_TABLE, None)
+    mock_sql_runner.query.return_value = (
+        DryRunStatus.SUCCESS,
+        A_SIMPLE_TABLE,
+        A_TOTAL_BYTES_PROCESSED,
+        None,
+    )
 
     upstream_simple_node = SimpleNode(unique_id="upstream", depends_on=[])
     upstream_node = upstream_simple_node.to_node()
     upstream_node.depends_on.deep_nodes = []
 
     node = SimpleNode(
         unique_id="node1",
@@ -66,27 +79,34 @@
     results = Results()
     results.add_result(
         "upstream",
         DryRunResult(
             node=upstream_node,
             status=DryRunStatus.FAILURE,
             table=None,
+            total_bytes_processed=0,
             exception=Exception("BOOM"),
         ),
     )
 
     model_runner = TableRunner(mock_sql_runner, results)
     result = model_runner.run(node)
     assert result.status == DryRunStatus.FAILURE
+    assert result.total_bytes_processed == 0
     assert isinstance(result.exception, UpstreamFailedException)
 
 
 def test_model_with_dependency_inserts_sql_literal() -> None:
     mock_sql_runner = MagicMock()
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, A_SIMPLE_TABLE, None)
+    mock_sql_runner.query.return_value = (
+        DryRunStatus.SUCCESS,
+        A_SIMPLE_TABLE,
+        A_TOTAL_BYTES_PROCESSED,
+        None,
+    )
 
     upstream_simple_node = SimpleNode(unique_id="upstream", depends_on=[])
     upstream_node = upstream_simple_node.to_node()
     upstream_node.depends_on.deep_nodes = []
 
     compiled_code = f"""SELECT * FROM {upstream_node.to_table_ref_literal()}"""
 
@@ -101,29 +121,35 @@
     results = Results()
     results.add_result(
         "upstream",
         DryRunResult(
             node=upstream_node,
             status=DryRunStatus.SUCCESS,
             table=A_SIMPLE_TABLE,
+            total_bytes_processed=A_TOTAL_BYTES_PROCESSED,
             exception=Exception("BOOM"),
         ),
     )
 
     model_runner = TableRunner(mock_sql_runner, results)
     result = model_runner.run(node)
 
     executed_sql = get_executed_sql(mock_sql_runner)
     assert result.status == DryRunStatus.SUCCESS
     assert executed_sql == "SELECT * FROM (SELECT 'foo' as `a`)"
 
 
 def test_model_with_sql_header_executes_header_first() -> None:
     mock_sql_runner = MagicMock()
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, A_SIMPLE_TABLE, None)
+    mock_sql_runner.query.return_value = (
+        DryRunStatus.SUCCESS,
+        A_SIMPLE_TABLE,
+        A_TOTAL_BYTES_PROCESSED,
+        None,
+    )
 
     pre_header_value = "DECLARE x INT64;"
 
     node = SimpleNode(
         unique_id="node1", depends_on=[], resource_type=ManifestScheduler.MODEL
     ).to_node()
     node.depends_on.deep_nodes = []
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_test_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_test_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         fields=[
             TableField(
                 name="a",
                 type=BigQueryFieldType.STRING,
             )
         ]
     )
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, None)
+    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, 0, None)
 
     test_node = SimpleNode(
         unique_id="test1", depends_on=[], resource_type=ManifestScheduler.TEST
     ).to_node()
     test_node.depends_on.deep_nodes = []
 
     results = Results()
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/node_runner/test_view_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/node_runner/test_view_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         TableField(
             name="a",
             type=BigQueryFieldType.STRING,
         )
     ]
 )
 
+A_TOTAL_BYTES_PROCESSED = 1000
+
 
 def sql_with_view_creation(node: Node, sql_statement: str) -> str:
     return f"CREATE OR REPLACE VIEW `{node.database}`.`{node.db_schema}`.`{node.alias}` AS (\n{sql_statement}\n)"
 
 
 def test_model_with_no_dependencies_runs_sql() -> None:
     mock_sql_runner = MagicMock()
@@ -32,15 +34,15 @@
         fields=[
             TableField(
                 name="a",
                 type=BigQueryFieldType.STRING,
             )
         ]
     )
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, None)
+    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, expected_table, 0, None)
 
     node = SimpleNode(
         unique_id="node1", depends_on=[], resource_type=ManifestScheduler.SEED
     ).to_node()
     node.depends_on.deep_nodes = []
 
     results = Results()
@@ -48,21 +50,27 @@
     model_runner = ViewRunner(mock_sql_runner, results)
 
     result = model_runner.run(node)
     mock_sql_runner.query.assert_called_with(
         sql_with_view_creation(node, node.compiled_code)
     )
     assert result.status == DryRunStatus.SUCCESS
+    assert result.total_bytes_processed == 0
     assert result.table
     assert result.table.fields[0].name == expected_table.fields[0].name
 
 
 def test_model_as_view_runs_create_view() -> None:
     mock_sql_runner = MagicMock()
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, A_SIMPLE_TABLE, None)
+    mock_sql_runner.query.return_value = (
+        DryRunStatus.SUCCESS,
+        A_SIMPLE_TABLE,
+        A_TOTAL_BYTES_PROCESSED,
+        None,
+    )
 
     node = SimpleNode(
         unique_id="node1", depends_on=[], resource_type=ManifestScheduler.MODEL
     ).to_node()
     node.depends_on.deep_nodes = []
     node.config.materialized = "view"
 
@@ -74,15 +82,20 @@
     executed_sql = get_executed_sql(mock_sql_runner)
     assert executed_sql.startswith(VIEW_CREATION_SQL)
     assert node.compiled_code in executed_sql
 
 
 def test_model_with_failed_dependency_raises_upstream_failed_exception() -> None:
     mock_sql_runner = MagicMock()
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, A_SIMPLE_TABLE, None)
+    mock_sql_runner.query.return_value = (
+        DryRunStatus.SUCCESS,
+        A_SIMPLE_TABLE,
+        A_TOTAL_BYTES_PROCESSED,
+        None,
+    )
 
     upstream_simple_node = SimpleNode(unique_id="upstream", depends_on=[])
     upstream_node = upstream_simple_node.to_node()
     upstream_node.depends_on.deep_nodes = []
 
     node = SimpleNode(
         unique_id="node1",
@@ -94,27 +107,34 @@
     results = Results()
     results.add_result(
         "upstream",
         DryRunResult(
             node=upstream_node,
             status=DryRunStatus.FAILURE,
             table=None,
+            total_bytes_processed=0,
             exception=Exception("BOOM"),
         ),
     )
 
     model_runner = ViewRunner(mock_sql_runner, results)
     result = model_runner.run(node)
     assert result.status == DryRunStatus.FAILURE
+    assert result.total_bytes_processed == 0
     assert isinstance(result.exception, UpstreamFailedException)
 
 
 def test_model_with_dependency_inserts_sql_literal() -> None:
     mock_sql_runner = MagicMock()
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, A_SIMPLE_TABLE, None)
+    mock_sql_runner.query.return_value = (
+        DryRunStatus.SUCCESS,
+        A_SIMPLE_TABLE,
+        A_TOTAL_BYTES_PROCESSED,
+        None,
+    )
 
     upstream_simple_node = SimpleNode(unique_id="upstream", depends_on=[])
     upstream_node = upstream_simple_node.to_node()
     upstream_node.depends_on.deep_nodes = []
 
     compiled_code = f"""SELECT * FROM {upstream_node.to_table_ref_literal()}"""
 
@@ -129,31 +149,38 @@
     results = Results()
     results.add_result(
         "upstream",
         DryRunResult(
             node=upstream_node,
             status=DryRunStatus.SUCCESS,
             table=A_SIMPLE_TABLE,
+            total_bytes_processed=0,
             exception=Exception("BOOM"),
         ),
     )
 
     model_runner = ViewRunner(mock_sql_runner, results)
     result = model_runner.run(node)
 
     executed_sql = get_executed_sql(mock_sql_runner)
     assert result.status == DryRunStatus.SUCCESS
+    assert result.total_bytes_processed == A_TOTAL_BYTES_PROCESSED
     assert executed_sql == sql_with_view_creation(
         node, "SELECT * FROM (SELECT 'foo' as `a`)"
     )
 
 
 def test_model_with_sql_header_executes_header_first() -> None:
     mock_sql_runner = MagicMock()
-    mock_sql_runner.query.return_value = (DryRunStatus.SUCCESS, A_SIMPLE_TABLE, None)
+    mock_sql_runner.query.return_value = (
+        DryRunStatus.SUCCESS,
+        A_SIMPLE_TABLE,
+        A_TOTAL_BYTES_PROCESSED,
+        None,
+    )
 
     pre_header_value = "DECLARE x INT64;"
 
     node = SimpleNode(
         unique_id="node1",
         depends_on=[],
         resource_type=ManifestScheduler.MODEL,
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 def test_error_query_does_not_retry() -> None:
     mock_project = MockProject()
     raised_exception = BadRequest(message="FOO")
     mock_project.mock_client.query.side_effect = raised_exception
     sql_runner = BigQuerySQLRunner(cast(ProjectService, mock_project))
 
     expected_sql = "SELECT * FROM foo"
-    status, _, exc = sql_runner.query(expected_sql)
+    status, _, _, exc = sql_runner.query(expected_sql)
 
     assert status == DryRunStatus.FAILURE
     assert exc is raised_exception
 
     mock_project.assert_query_called_with_sql(expected_sql)
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/test_columns_metadata.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/test_columns_metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/test_execution.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/test_literals.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/test_literals.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/test_result_reporter.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/test_result_reporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,35 +17,38 @@
 @pytest.fixture()
 def successful_result() -> DryRunResult:
     return DryRunResult(
         node=SimpleNode(unique_id="A", depends_on=[]).to_node(),
         table=Table(fields=[]),
         status=DryRunStatus.SUCCESS,
         exception=None,
+        total_bytes_processed=1000,
         linting_status=LintingStatus.SKIPPED,
     )
 
 
 @pytest.fixture()
 def failed_result() -> DryRunResult:
     return DryRunResult(
         node=SimpleNode(unique_id="B", depends_on=[]).to_node(),
         table=Table(fields=[]),
         status=DryRunStatus.FAILURE,
+        total_bytes_processed=0,
         exception=Exception("Oh no!"),
         linting_status=LintingStatus.SKIPPED,
     )
 
 
 @pytest.fixture()
 def failed_linting_result() -> DryRunResult:
     return DryRunResult(
         node=SimpleNode(unique_id="B", depends_on=[]).to_node(),
         table=Table(fields=[]),
         status=DryRunStatus.SUCCESS,
+        total_bytes_processed=1000,
         exception=None,
         linting_status=LintingStatus.FAILURE,
         linting_errors=[
             LintingError(rule="TEST_LINTING_RULE", message="Linting wrong")
         ],
     )
```

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/test_scheduler.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/dbt_dry_run/test/utils.py` & `dbt_dry_run-0.7.7/dbt_dry_run/test/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.7.5/pyproject.toml` & `dbt_dry_run-0.7.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 [tool.poetry]
 name = "dbt-dry-run"
-version = "0.7.5"
+version = "0.7.7"
 description = "Dry run dbt projects"
 authors = ["Connor Charles <connor.charles@autotrader.co.uk>",
            "Phil hope <philip.hope@autotrader.co.uk>",
            "Angelos Georgiadis <angelos.georgiadis@autotrader.co.uk>",
            "Richard Wilmer <richard.wilmer@autotrader.co.uk>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/autotraderuk/dbt-dry-run"
 
 [tool.poetry.scripts]
 dbt-dry-run = "dbt_dry_run.__main__:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-agate = "^1.6"
+agate = ">=1.7.0,<1.10"
 google-cloud-bigquery = "^3"
 pydantic = "^1.9.0"
 tenacity = "^8.2"
-networkx = "^2.6"
+networkx = ">=2.3,<4.0"
 pyyaml = "~6"
-typer = "^0.6.1"
+typer = "~0"
 
 [tool.poetry.dev-dependencies]
 black = "^22"
 isort = "^5.10.1"
 pytest = "^7.2.0"
 mypy = "^0.931"
 types-PyYAML = "^6.0.4"
 pytest-cov = "^4.0.0"
 twine = "^3.8.0"
 types-setuptools = "^57.4.9"
 pytest-mock = "^3.7.0"
-dbt-bigquery = "^1.6.0"
+dbt-bigquery = "~1.7.0"
 
 [build-system]
 requires = ["poetry-core>=1.5.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = "dbt_dry_run/test"
 filterwarnings = [
     "error",
     "ignore:Deprecated call to",
     "ignore:pkg_resources is deprecated as an API",
     "ignore:invalid escape sequence",
     "ignore:unclosed",
     "ignore:'cgi' is deprecated and slated for removal",
-    "ignore:Your application has authenticated using end user credentials"
+    "ignore:Your application has authenticated using end user credentials",
+    "ignore::UserWarning"
 ]
 pythonpath = [
   "."
 ]
 
 [tool.coverage.run]
 source = ["dbt_dry_run"]
```

### Comparing `dbt_dry_run-0.7.5/PKG-INFO` & `dbt_dry_run-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: dbt-dry-run
-Version: 0.7.5
+Version: 0.7.7
 Summary: Dry run dbt projects
 Home-page: https://github.com/autotraderuk/dbt-dry-run
 License: Apache-2.0
 Author: Connor Charles
 Author-email: connor.charles@autotrader.co.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: agate (>=1.6,<2.0)
+Requires-Dist: agate (>=1.7.0,<1.10)
 Requires-Dist: google-cloud-bigquery (>=3,<4)
-Requires-Dist: networkx (>=2.6,<3.0)
+Requires-Dist: networkx (>=2.3,<4.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: pyyaml (>=6,<7)
 Requires-Dist: tenacity (>=8.2,<9.0)
-Requires-Dist: typer (>=0.6.1,<0.7.0)
+Requires-Dist: typer (>=0,<1)
 Project-URL: Repository, https://github.com/autotraderuk/dbt-dry-run
 Description-Content-Type: text/markdown
 
 # dbt-dry-run
 
 [dbt][dbt-home] is a tool that helps manage data transformations using templated SQL queries. These SQL queries are
 executed against a target data warehouse. It doesn't check the validity of SQL queries before it executes your project.
```


# Comparing `tmp/bmsdna_sql_utils-0.12.6.tar.gz` & `tmp/bmsdna_sql_utils-0.12.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_sql_utils-0.12.6.tar", max compression
+gzip compressed data, was "bmsdna_sql_utils-0.12.7.tar", max compression
```

## Comparing `bmsdna_sql_utils-0.12.6.tar` & `bmsdna_sql_utils-0.12.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      255 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/README.md
--rw-r--r--   0        0        0        0 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/__init__.py
--rw-r--r--   0        0        0      382 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/__init__.py
--rw-r--r--   0        0        0     3133 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/async_db_helper.py
--rw-r--r--   0        0        0     1169 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/case_preserving_set.py
--rw-r--r--   0        0        0     3529 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_helper.py
--rw-r--r--   0        0        0        0 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/__init__.py
--rw-r--r--   0        0        0     2373 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/db_logging.py
--rw-r--r--   0        0        0     5388 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/delta_polars_source.py
--rw-r--r--   0        0        0     6066 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/delta_source.py
--rw-r--r--   0        0        0    25911 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/fill_table.py
--rw-r--r--   0        0        0     2116 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/json_insert.py
--rw-r--r--   0        0        0     5178 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/lake_source.py
--rw-r--r--   0        0        0     1754 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/meta_sql_store.py
--rw-r--r--   0        0        0     1481 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/odbc_insert.py
--rw-r--r--   0        0        0     1856 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/source.py
--rw-r--r--   0        0        0     5679 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/source_spark.py
--rw-r--r--   0        0        0      739 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/sql_utils.py
--rw-r--r--   0        0        0    17094 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/sqlschema.py
--rw-r--r--   0        0        0     1132 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/dbapi.py
--rw-r--r--   0        0        0     1332 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/integrity_check.py
--rw-r--r--   0        0        0      199 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/lake/__init__.py
--rw-r--r--   0        0        0     2423 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/lake/lake_meta.py
--rw-r--r--   0        0        0      996 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/lake/type_fromarrow.py
--rw-r--r--   0        0        0      884 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/lake/types.py
--rw-r--r--   0        0        0     5671 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/metadata/__init__.py
--rw-r--r--   0        0        0     4009 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/query.py
--rw-r--r--   0        0        0     2759 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/query_generation.py
--rw-r--r--   0        0        0     2619 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/result.py
--rw-r--r--   0        0        0     4026 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/server_info.py
--rw-r--r--   0        0        0     1078 2024-05-01 12:12:37.585126 bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/sql_gen.py
--rw-r--r--   0        0        0     1870 2024-05-01 12:12:37.589126 bmsdna_sql_utils-0.12.6/pyproject.toml
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.12.6/PKG-INFO
+-rw-r--r--   0        0        0      255 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/__init__.py
+-rw-r--r--   0        0        0      382 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/__init__.py
+-rw-r--r--   0        0        0     3133 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/async_db_helper.py
+-rw-r--r--   0        0        0     1169 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/case_preserving_set.py
+-rw-r--r--   0        0        0     3529 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_helper.py
+-rw-r--r--   0        0        0        0 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/__init__.py
+-rw-r--r--   0        0        0     2373 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/db_logging.py
+-rw-r--r--   0        0        0     5388 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/delta_polars_source.py
+-rw-r--r--   0        0        0     6066 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/delta_source.py
+-rw-r--r--   0        0        0    25911 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/fill_table.py
+-rw-r--r--   0        0        0     2116 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/json_insert.py
+-rw-r--r--   0        0        0     5178 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/lake_source.py
+-rw-r--r--   0        0        0     1754 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/meta_sql_store.py
+-rw-r--r--   0        0        0     1481 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/odbc_insert.py
+-rw-r--r--   0        0        0     1856 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/source.py
+-rw-r--r--   0        0        0     6001 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/source_spark.py
+-rw-r--r--   0        0        0      739 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/sql_utils.py
+-rw-r--r--   0        0        0    17094 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/sqlschema.py
+-rw-r--r--   0        0        0     1132 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/dbapi.py
+-rw-r--r--   0        0        0     1332 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/integrity_check.py
+-rw-r--r--   0        0        0      199 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/lake/__init__.py
+-rw-r--r--   0        0        0     2423 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/lake/lake_meta.py
+-rw-r--r--   0        0        0      996 2024-05-03 08:35:59.625210 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/lake/type_fromarrow.py
+-rw-r--r--   0        0        0      884 2024-05-03 08:35:59.629211 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/lake/types.py
+-rw-r--r--   0        0        0     5671 2024-05-03 08:35:59.629211 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/metadata/__init__.py
+-rw-r--r--   0        0        0     4009 2024-05-03 08:35:59.629211 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/query.py
+-rw-r--r--   0        0        0     2759 2024-05-03 08:35:59.629211 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/query_generation.py
+-rw-r--r--   0        0        0     2619 2024-05-03 08:35:59.629211 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/result.py
+-rw-r--r--   0        0        0     4026 2024-05-03 08:35:59.629211 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/server_info.py
+-rw-r--r--   0        0        0     1078 2024-05-03 08:35:59.629211 bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/sql_gen.py
+-rw-r--r--   0        0        0     1870 2024-05-03 08:35:59.629211 bmsdna_sql_utils-0.12.7/pyproject.toml
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.12.7/PKG-INFO
```

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/async_db_helper.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/async_db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/case_preserving_set.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/case_preserving_set.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_helper.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/db_logging.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/db_logging.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/delta_polars_source.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/delta_polars_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/delta_source.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/delta_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/fill_table.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/fill_table.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/json_insert.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/json_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/lake_source.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/lake_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/meta_sql_store.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/meta_sql_store.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/odbc_insert.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/odbc_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/source.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/source_spark.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/source_spark.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,23 @@
 
 class SourceSpark(ImportSource):
     def __init__(
         self,
         df: "DataFrame",
         use_json_insert=False,
         change_date: datetime | None = None,
+        partition_columns: list[str] | None = None,
     ) -> None:
         super().__init__()
 
         self._schema: list[SQLField] | None = None
         self.use_json_insert = use_json_insert
         self.df = df
         self.change_date = change_date
+        self.partition_columns = partition_columns
 
     async def write_to_sql_server(
         self,
         target_table: str | tuple[str, str],
         connection_string: str | dict,
         partition_filters: dict | None,
         select: list[str] | None,
@@ -84,17 +86,23 @@
             record_batch_reader = pa.RecordBatchReader.from_batches(tbl.schema, tbl.to_batches())
             res = await insert_record_batch_to_sql(connection_string_sql, table_str, record_batch_reader, select)
             col_names = [f["name"] for f in res["fields"]]
         return WriteInfo(column_names=col_names, table_name=target_table)
 
     def get_partition_values(self) -> list[dict]:
         col_names = [f.column_name for f in self.get_schema()]
-        if "_partition" in col_names:
+        if "_partition" in col_names and self.partition_columns is None:
+            self.partition_columns = ["_partition"]
+        if self.partition_columns:
             return [
-                r.asDict(True) for r in self.df.selectExpr("_partition").orderBy("_partition").distinct().collect()
+                r.asDict(True)
+                for r in self.df.selectExpr(*self.partition_columns)
+                .orderBy(*self.partition_columns)
+                .distinct()
+                .collect()
             ]
         return []
 
     def get_schema(self) -> list[SQLField]:
         fields = self.df.schema.fields
 
         def sqlglot_type(dtype):
```

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/sql_utils.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/sql_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/db_io/sqlschema.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/db_io/sqlschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/dbapi.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/dbapi.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/integrity_check.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/integrity_check.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/lake/lake_meta.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/lake/lake_meta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/lake/type_fromarrow.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/lake/type_fromarrow.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/lake/types.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/lake/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/metadata/__init__.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/query.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/query.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/query_generation.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/query_generation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/result.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/result.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/server_info.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/server_info.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/bmsdna/sql_utils/sql_gen.py` & `bmsdna_sql_utils-0.12.7/bmsdna/sql_utils/sql_gen.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.6/pyproject.toml` & `bmsdna_sql_utils-0.12.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "bmsdna-sql-utils"
-version = "0.12.6"
+version = "0.12.7"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 readme = "README.md"
 packages = [{ include = "bmsdna" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyodbc = { version = "^5.0.1", optional = true }
 aioodbc = { version = "^0.5.0", optional = true }
 python-tds = { version = "^1.13.0", optional = true }
 pydantic = { version = "^2.3.0", optional = true }
 aiohttp = "^3.8.5"
 requests = ">=2.28.0"
 duckdb = { version = "^0.10.1", optional = true }
-lakeapi2sql = { version = ">=0.8.4", optional = true }
+lakeapi2sql = { version = ">=0.9.1", optional = true }
 deltalake = { version = ">=0.16.4", optional = true }
 python-dateutil = { version = "^2.8.2", python = "<3.11" }
 arrow-odbc = { version = "^5.0.0", optional = true }
 deltalake2db = ">=0.3.0"
 polars = {extras = ["chrono-tz"], version = ">=0.20.21", optional = true }
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `bmsdna_sql_utils-0.12.6/PKG-INFO` & `bmsdna_sql_utils-0.12.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-sql-utils
-Version: 0.12.6
+Version: 0.12.7
 Summary: 
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,15 +15,15 @@
 Provides-Extra: polars
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: aioodbc (>=0.5.0,<0.6.0)
 Requires-Dist: arrow-odbc (>=5.0.0,<6.0.0) ; extra == "db2delta"
 Requires-Dist: deltalake (>=0.16.4) ; extra == "delta" or extra == "db2delta"
 Requires-Dist: deltalake2db (>=0.3.0)
 Requires-Dist: duckdb (>=0.10.1,<0.11.0) ; extra == "delta" or extra == "db2delta"
-Requires-Dist: lakeapi2sql (>=0.8.4) ; extra == "db-io"
+Requires-Dist: lakeapi2sql (>=0.9.1) ; extra == "db-io"
 Requires-Dist: polars[chrono-tz] (>=0.20.21) ; extra == "polars"
 Requires-Dist: pydantic (>=2.3.0,<3.0.0)
 Requires-Dist: pyodbc (>=5.0.1,<6.0.0) ; extra == "db-io"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) ; python_version < "3.11"
 Requires-Dist: python-tds (>=1.13.0,<2.0.0)
 Requires-Dist: requests (>=2.28.0)
 Description-Content-Type: text/markdown
```


# Comparing `tmp/jenfi_pipeline_data_app-0.4.2.tar.gz` & `tmp/jenfi_pipeline_data_app-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenfi_pipeline_data_app-0.4.2.tar", max compression
+gzip compressed data, was "jenfi_pipeline_data_app-0.4.3.tar", max compression
```

## Comparing `jenfi_pipeline_data_app-0.4.2.tar` & `jenfi_pipeline_data_app-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      510 2023-01-16 03:30:30.019998 jenfi_pipeline_data_app-0.4.2/README.md
--rw-r--r--   0        0        0     1313 2023-01-16 02:40:26.715779 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/API.md
--rw-r--r--   0        0        0     1526 2023-05-30 09:11:12.212975 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/__init__.py
--rw-r--r--   0        0        0      354 2023-05-30 09:11:12.213698 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/_pdoc.py
--rw-r--r--   0        0        0     2367 2024-05-02 16:14:34.857722 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app.py
--rw-r--r--   0        0        0      345 2023-05-30 09:11:12.214511 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_constants.py
--rw-r--r--   0        0        0     1107 2024-02-22 07:39:24.264183 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_db_handler.py
--rw-r--r--   0        0        0     1066 2023-01-16 02:40:26.716191 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_exit_program.py
--rw-r--r--   0        0        0     1074 2023-05-30 09:11:12.215285 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_models_s3.py
--rw-r--r--   0        0        0     1323 2023-05-30 09:11:12.216581 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_parameters.py
--rw-r--r--   0        0        0     1282 2023-05-30 09:11:12.216967 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_query.py
--rw-r--r--   0        0        0     2896 2023-05-30 09:11:12.217328 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_result.py
--rw-r--r--   0        0        0      569 2023-05-30 09:11:12.217681 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_test_funcs.py
--rw-r--r--   0        0        0     1419 2024-02-22 07:14:05.283471 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/config/db.py
--rw-r--r--   0        0        0      395 2023-05-30 09:11:12.218386 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/config/s3.py
--rw-r--r--   0        0        0       43 2023-05-30 09:11:12.218741 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/db_cache/__init__.py
--rw-r--r--   0        0        0     3838 2023-05-30 09:11:12.219328 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/db_cache/cacher.py
--rw-r--r--   0        0        0     2051 2024-05-03 07:52:46.652243 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/db_cache/db_cache.py
--rw-r--r--   0        0        0     2050 2023-05-30 09:11:12.220034 jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/db_models.py
--rw-r--r--   0        0        0      982 2024-05-03 07:54:03.961750 jenfi_pipeline_data_app-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 jenfi_pipeline_data_app-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      510 2023-01-16 03:30:30.019998 jenfi_pipeline_data_app-0.4.3/README.md
+-rw-r--r--   0        0        0     1313 2023-01-16 02:40:26.715779 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/API.md
+-rw-r--r--   0        0        0     1526 2023-05-30 09:11:12.212975 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/__init__.py
+-rw-r--r--   0        0        0      354 2023-05-30 09:11:12.213698 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/_pdoc.py
+-rw-r--r--   0        0        0     2367 2024-05-02 16:14:34.857722 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app.py
+-rw-r--r--   0        0        0      345 2023-05-30 09:11:12.214511 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_constants.py
+-rw-r--r--   0        0        0     1107 2024-02-22 07:39:24.264183 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_db_handler.py
+-rw-r--r--   0        0        0     1066 2023-01-16 02:40:26.716191 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_exit_program.py
+-rw-r--r--   0        0        0     1074 2023-05-30 09:11:12.215285 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_models_s3.py
+-rw-r--r--   0        0        0     1323 2023-05-30 09:11:12.216581 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_parameters.py
+-rw-r--r--   0        0        0     1282 2023-05-30 09:11:12.216967 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_query.py
+-rw-r--r--   0        0        0     2896 2023-05-30 09:11:12.217328 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_result.py
+-rw-r--r--   0        0        0      569 2023-05-30 09:11:12.217681 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_test_funcs.py
+-rw-r--r--   0        0        0     1419 2024-02-22 07:14:05.283471 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/config/db.py
+-rw-r--r--   0        0        0      395 2023-05-30 09:11:12.218386 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/config/s3.py
+-rw-r--r--   0        0        0       43 2023-05-30 09:11:12.218741 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/db_cache/__init__.py
+-rw-r--r--   0        0        0     3838 2023-05-30 09:11:12.219328 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/db_cache/cacher.py
+-rw-r--r--   0        0        0     1973 2024-05-03 11:14:13.782052 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/db_cache/db_cache.py
+-rw-r--r--   0        0        0     3726 2024-05-03 11:16:31.474624 jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/db_models.py
+-rw-r--r--   0        0        0      982 2024-05-03 11:15:05.316368 jenfi_pipeline_data_app-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 jenfi_pipeline_data_app-0.4.3/PKG-INFO
```

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/API.md` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/API.md`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/__init__.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/__init__.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_db_handler.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_db_handler.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_exit_program.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_exit_program.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_models_s3.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_models_s3.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_parameters.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_parameters.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_query.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_query.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_result.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_result.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/app_funcs/_test_funcs.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/app_funcs/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/config/db.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/config/db.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/db_cache/cacher.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/db_cache/cacher.py`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/db_cache/db_cache.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/db_cache/db_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,19 +30,16 @@
         return self._with_cacher(self._df_query, query_str, rebuild_cache)
 
     def _df_query(self, query_str: str) -> pd.DataFrame:
         # For pandas 2.2.0
         # https://stackoverflow.com/a/77949093
 
         # Debugging
-        print("Querying DB")
-        print()
         print(query_str)
         print(self.db_engine)
-        print("End Querying DB")
         with self.db_engine.connect() as conn:
             return pd.read_sql(query_str, conn.connection)
 
     def query_one(self, query_str: str, rebuild_cache: bool):
         return self._with_cacher(self._query_one, query_str, rebuild_cache)
 
     def _query_one(self, query_str: str):
```

### Comparing `jenfi_pipeline_data_app-0.4.2/jenfi_pipeline_data_app/db_models.py` & `jenfi_pipeline_data_app-0.4.3/jenfi_pipeline_data_app/db_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import os
 
 from sqlalchemy import JSON, Column, DateTime, Integer, MetaData, Table
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.ext.mutable import MutableDict
 
 
 # This shouldn't be a function, but I can't figure out how to pass a db_engine before the class creation on import.
@@ -32,15 +33,43 @@
                 .with_for_update(of=StateMachineRun, nowait=False)
                 .get(state_machine_run_id)
             )
             sm_run.result[logical_step_name] = results
 
             return app.db.commit()
 
-    return StateMachineRun
+    class NellieStateMachineRun(Base):
+        __table__ = Table(
+            "pipeline_statemachinerun",
+            metadata,
+            Column("id", Integer, primary_key=True),
+            Column("result", MutableDict.as_mutable(JSON)),
+            Column("created", DateTime, default=datetime.datetime.now),
+            Column("modified", DateTime, default=datetime.datetime.now),
+            autoload=True,
+        )
+
+        def result_to_db(self, logical_step_name, state_machine_run_id, results):
+            sm_run = (
+                app.db.query(NellieStateMachineRun)
+                .populate_existing()
+                .with_for_update(of=NellieStateMachineRun, nowait=False)
+                .get(state_machine_run_id)
+            )
+            sm_run.result[logical_step_name] = results
+
+            return app.db.commit()
+
+    STATE_MACHINE_RUN_MODEL_MAP = {
+        "NelliePipelineProd": NellieStateMachineRun,
+        "NelliePipelineStage": NellieStateMachineRun,
+    }
+    app_name = os.getenv("CORE_APP_NAME", None)
+
+    return STATE_MACHINE_RUN_MODEL_MAP.get(app_name, StateMachineRun)
 
 
 def state_machine_model(app):
     Base = declarative_base()
     metadata = MetaData(bind=app.db_engine)
 
     class StateMachine(Base):
@@ -49,8 +78,24 @@
             metadata,
             Column("id", Integer, primary_key=True),
             Column("created_at", DateTime, default=datetime.datetime.now),
             Column("updated_at", DateTime, default=datetime.datetime.now),
             autoload=True,
         )
 
-    return StateMachine
+    class NellieStateMachine(Base):
+        __table__ = Table(
+            "pipeline_statemachine",
+            metadata,
+            Column("id", Integer, primary_key=True),
+            Column("created", DateTime, default=datetime.datetime.now),
+            Column("modified", DateTime, default=datetime.datetime.now),
+            autoload=True,
+        )
+
+    STATE_MACHINE_MODEL_MAP = {
+        "NelliePipelineProd": NellieStateMachine,
+        "NelliePipelineStage": NellieStateMachine,
+    }
+    app_name = os.getenv("CORE_APP_NAME", None)
+
+    return STATE_MACHINE_MODEL_MAP.get(app_name, StateMachine)
```

### Comparing `jenfi_pipeline_data_app-0.4.2/pyproject.toml` & `jenfi_pipeline_data_app-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jenfi-pipeline-data-app"
-version = "0.4.2"
+version = "0.4.3"
 description = ""
 readme = "README.md"
 authors = ["Justin Louie <224840+nitsujri@users.noreply.github.com>"]
 
 [tool.poetry.dependencies]
 python = "~3.10"
 SQLAlchemy = "^1.4.40"
```

### Comparing `jenfi_pipeline_data_app-0.4.2/PKG-INFO` & `jenfi_pipeline_data_app-0.4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jenfi-pipeline-data-app
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Author: Justin Louie
 Author-email: 224840+nitsujri@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: SQLAlchemy (>=1.4.40,<2.0.0)
```


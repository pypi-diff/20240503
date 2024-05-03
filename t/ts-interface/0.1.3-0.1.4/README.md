# Comparing `tmp/ts_interface-0.1.3.tar.gz` & `tmp/ts_interface-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts_interface-0.1.3.tar", max compression
+gzip compressed data, was "ts_interface-0.1.4.tar", max compression
```

## Comparing `ts_interface-0.1.3.tar` & `ts_interface-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2024-05-01 09:19:49.827766 ts_interface-0.1.3/LICENSE
--rw-r--r--   0        0        0       38 2024-05-01 09:19:49.827766 ts_interface-0.1.3/README.md
--rw-r--r--   0        0        0      325 2024-05-03 07:01:03.100175 ts_interface-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      392 2024-05-02 08:06:57.221335 ts_interface-0.1.3/tsinterface/io/bbox_io.py
--rw-r--r--   0        0        0      565 2024-05-02 08:06:57.229334 ts_interface-0.1.3/tsinterface/io/detection_io.py
--rw-r--r--   0        0        0      396 2024-05-02 08:06:57.233334 ts_interface-0.1.3/tsinterface/io/distribution_io.py
--rw-r--r--   0        0        0     1427 2024-05-02 08:06:57.225335 ts_interface-0.1.3/tsinterface/io/info_dto.py
--rw-r--r--   0        0        0       93 2024-05-02 08:03:36.270009 ts_interface-0.1.3/tsinterface/io/io.py
--rw-r--r--   0        0        0      400 2024-05-02 08:06:57.237334 ts_interface-0.1.3/tsinterface/io/label_io.py
--rw-r--r--   0        0        0      355 2024-05-02 07:08:15.057595 ts_interface-0.1.3/tsinterface/schema/load_output_schema.json
--rw-r--r--   0        0        0      305 2024-05-01 12:27:25.558900 ts_interface-0.1.3/tsinterface/schema/process_input_schema.json
--rw-r--r--   0        0        0     3307 2024-05-01 12:25:43.821850 ts_interface-0.1.3/tsinterface/schema/process_output_schema.json
--rw-r--r--   0        0        0      381 2024-05-02 11:44:12.415036 ts_interface-0.1.3/tsinterface/schema/validation_output_schema.json
--rw-r--r--   0        0        0     1312 2024-05-03 07:00:58.023675 ts_interface-0.1.3/tsinterface/ts_interface.py
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 ts_interface-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-01 09:19:49.827766 ts_interface-0.1.4/LICENSE
+-rw-r--r--   0        0        0       38 2024-05-01 09:19:49.827766 ts_interface-0.1.4/README.md
+-rw-r--r--   0        0        0      325 2024-05-03 07:07:04.689402 ts_interface-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      392 2024-05-02 08:06:57.221335 ts_interface-0.1.4/tsinterface/io/bbox_io.py
+-rw-r--r--   0        0        0      565 2024-05-02 08:06:57.229334 ts_interface-0.1.4/tsinterface/io/detection_io.py
+-rw-r--r--   0        0        0      396 2024-05-02 08:06:57.233334 ts_interface-0.1.4/tsinterface/io/distribution_io.py
+-rw-r--r--   0        0        0     1427 2024-05-02 08:06:57.225335 ts_interface-0.1.4/tsinterface/io/info_dto.py
+-rw-r--r--   0        0        0       93 2024-05-02 08:03:36.270009 ts_interface-0.1.4/tsinterface/io/io.py
+-rw-r--r--   0        0        0      400 2024-05-02 08:06:57.237334 ts_interface-0.1.4/tsinterface/io/label_io.py
+-rw-r--r--   0        0        0      355 2024-05-02 07:08:15.057595 ts_interface-0.1.4/tsinterface/schema/load_output_schema.json
+-rw-r--r--   0        0        0      305 2024-05-01 12:27:25.558900 ts_interface-0.1.4/tsinterface/schema/process_input_schema.json
+-rw-r--r--   0        0        0     3307 2024-05-01 12:25:43.821850 ts_interface-0.1.4/tsinterface/schema/process_output_schema.json
+-rw-r--r--   0        0        0      381 2024-05-02 11:44:12.415036 ts_interface-0.1.4/tsinterface/schema/validation_output_schema.json
+-rw-r--r--   0        0        0      833 2024-05-03 07:07:03.113051 ts_interface-0.1.4/tsinterface/ts_interface.py
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 ts_interface-0.1.4/PKG-INFO
```

### Comparing `ts_interface-0.1.3/LICENSE` & `ts_interface-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ts_interface-0.1.3/tsinterface/io/detection_io.py` & `ts_interface-0.1.4/tsinterface/io/detection_io.py`

 * *Files identical despite different names*

### Comparing `ts_interface-0.1.3/tsinterface/io/info_dto.py` & `ts_interface-0.1.4/tsinterface/io/info_dto.py`

 * *Files identical despite different names*

### Comparing `ts_interface-0.1.3/tsinterface/schema/process_output_schema.json` & `ts_interface-0.1.4/tsinterface/schema/process_output_schema.json`

 * *Files identical despite different names*

### Comparing `ts_interface-0.1.3/tsinterface/ts_interface.py` & `ts_interface-0.1.4/tsinterface/ts_interface.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,31 +20,15 @@
 
     @staticmethod
     @abc.abstractmethod
     def validate() -> str:
         pass
 
     @staticmethod
-    def get_validation_output_schema():
-        return TsInterface._get_schema('validation_output_schema')
-
-    @staticmethod
-    def get_load_output_schema():
-        return TsInterface._get_schema('load_output_schema')
-
-    @staticmethod
-    def get_process_input_schema():
-        return TsInterface._get_schema('process_input_schema')
-
-    @staticmethod
-    def get_process_output_schema():
-        return TsInterface._get_schema('process_output_schema')
-
-    @staticmethod
-    def _get_schema(name: str):
+    def get_schema(name: str):
         with open(os.path.join(BASE_DIR, 'schema', name + '.json')) as schema:
             schema = json.load(schema)
         return schema
 
     @staticmethod
     def get_schemas():
         schema_dir = os.path.join(BASE_DIR, 'schema')
```

### Comparing `ts_interface-0.1.3/PKG-INFO` & `ts_interface-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-interface
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: ph
 Author-email: ph@tordenskjold.space
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


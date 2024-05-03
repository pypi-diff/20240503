# Comparing `tmp/ts_interface-0.1.1.tar.gz` & `tmp/ts_interface-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts_interface-0.1.1.tar", max compression
+gzip compressed data, was "ts_interface-0.1.2.tar", max compression
```

## Comparing `ts_interface-0.1.1.tar` & `ts_interface-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2024-05-01 09:19:49.827766 ts_interface-0.1.1/LICENSE
--rw-r--r--   0        0        0       38 2024-05-01 09:19:49.827766 ts_interface-0.1.1/README.md
--rw-r--r--   0        0        0      325 2024-05-02 09:47:02.072053 ts_interface-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      392 2024-05-02 08:06:57.221335 ts_interface-0.1.1/tsinterface/io/bbox_io.py
--rw-r--r--   0        0        0      565 2024-05-02 08:06:57.229334 ts_interface-0.1.1/tsinterface/io/detection_io.py
--rw-r--r--   0        0        0      396 2024-05-02 08:06:57.233334 ts_interface-0.1.1/tsinterface/io/distribution_io.py
--rw-r--r--   0        0        0     1427 2024-05-02 08:06:57.225335 ts_interface-0.1.1/tsinterface/io/info_dto.py
--rw-r--r--   0        0        0       93 2024-05-02 08:03:36.270009 ts_interface-0.1.1/tsinterface/io/io.py
--rw-r--r--   0        0        0      400 2024-05-02 08:06:57.237334 ts_interface-0.1.1/tsinterface/io/label_io.py
--rw-r--r--   0        0        0      305 2024-05-01 12:27:25.558900 ts_interface-0.1.1/tsinterface/schema/input_schema.json
--rw-r--r--   0        0        0      355 2024-05-02 07:08:15.057595 ts_interface-0.1.1/tsinterface/schema/load_schema.json
--rw-r--r--   0        0        0     3307 2024-05-01 12:25:43.821850 ts_interface-0.1.1/tsinterface/schema/output_schema.json
--rw-r--r--   0        0        0      365 2024-05-02 06:54:15.554393 ts_interface-0.1.1/tsinterface/schema/validate_schema.json
--rw-r--r--   0        0        0      434 2024-05-02 08:28:40.739206 ts_interface-0.1.1/tsinterface/ts_interface.py
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 ts_interface-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-01 09:19:49.827766 ts_interface-0.1.2/LICENSE
+-rw-r--r--   0        0        0       38 2024-05-01 09:19:49.827766 ts_interface-0.1.2/README.md
+-rw-r--r--   0        0        0      325 2024-05-02 12:28:27.540073 ts_interface-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      392 2024-05-02 08:06:57.221335 ts_interface-0.1.2/tsinterface/io/bbox_io.py
+-rw-r--r--   0        0        0      565 2024-05-02 08:06:57.229334 ts_interface-0.1.2/tsinterface/io/detection_io.py
+-rw-r--r--   0        0        0      396 2024-05-02 08:06:57.233334 ts_interface-0.1.2/tsinterface/io/distribution_io.py
+-rw-r--r--   0        0        0     1427 2024-05-02 08:06:57.225335 ts_interface-0.1.2/tsinterface/io/info_dto.py
+-rw-r--r--   0        0        0       93 2024-05-02 08:03:36.270009 ts_interface-0.1.2/tsinterface/io/io.py
+-rw-r--r--   0        0        0      400 2024-05-02 08:06:57.237334 ts_interface-0.1.2/tsinterface/io/label_io.py
+-rw-r--r--   0        0        0      355 2024-05-02 07:08:15.057595 ts_interface-0.1.2/tsinterface/schema/load_output_schema.json
+-rw-r--r--   0        0        0      305 2024-05-01 12:27:25.558900 ts_interface-0.1.2/tsinterface/schema/process_input_schema.json
+-rw-r--r--   0        0        0     3307 2024-05-01 12:25:43.821850 ts_interface-0.1.2/tsinterface/schema/process_output_schema.json
+-rw-r--r--   0        0        0      381 2024-05-02 11:44:12.415036 ts_interface-0.1.2/tsinterface/schema/validation_output_schema.json
+-rw-r--r--   0        0        0     1139 2024-05-02 11:57:49.677299 ts_interface-0.1.2/tsinterface/ts_interface.py
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 ts_interface-0.1.2/PKG-INFO
```

### Comparing `ts_interface-0.1.1/LICENSE` & `ts_interface-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ts_interface-0.1.1/tsinterface/io/detection_io.py` & `ts_interface-0.1.2/tsinterface/io/detection_io.py`

 * *Files identical despite different names*

### Comparing `ts_interface-0.1.1/tsinterface/io/info_dto.py` & `ts_interface-0.1.2/tsinterface/io/info_dto.py`

 * *Files identical despite different names*

### Comparing `ts_interface-0.1.1/tsinterface/schema/output_schema.json` & `ts_interface-0.1.2/tsinterface/schema/process_output_schema.json`

 * *Files identical despite different names*

### Comparing `ts_interface-0.1.1/PKG-INFO` & `ts_interface-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-interface
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: ph
 Author-email: ph@tordenskjold.space
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


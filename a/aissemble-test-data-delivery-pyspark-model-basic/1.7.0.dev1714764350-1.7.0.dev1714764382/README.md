# Comparing `tmp/aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350.tar.gz` & `tmp/aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350.tar", max compression
+gzip compressed data, was "aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382.tar", max compression
```

## Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350.tar` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     9580 2024-05-03 19:25:27.961318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/LICENSE
--rw-r--r--   0        0        0     1827 2024-05-03 19:25:50.532307 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/pyproject.toml
--rw-r--r--   0        0        0      208 2024-05-03 19:25:27.945318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:25:27.904318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/__init__.py.tmp
--rw-r--r--   0        0        0     1007 2024-05-03 19:25:27.945318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py
--rw-r--r--   0        0        0      799 2024-05-03 19:25:27.904318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py.tmp
--rw-r--r--   0        0        0      818 2024-05-03 19:25:27.943318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py
--rw-r--r--   0        0        0      610 2024-05-03 19:25:27.890318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py.tmp
--rw-r--r--   0        0        0      208 2024-05-03 19:25:27.934318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:25:27.884318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/__init__.py.tmp
--rw-r--r--   0        0        0     3938 2024-05-03 19:25:27.933318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py
--rw-r--r--   0        0        0     3730 2024-05-03 19:25:27.883318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py.tmp
--rw-r--r--   0        0        0      670 2024-05-03 19:25:27.936318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py
--rw-r--r--   0        0        0      462 2024-05-03 19:25:27.904318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py.tmp
--rw-r--r--   0        0        0     1902 2024-05-03 19:25:27.939318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py
--rw-r--r--   0        0        0     1694 2024-05-03 19:25:27.907318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py.tmp
--rw-r--r--   0        0        0     1865 2024-05-03 19:25:27.941318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py
--rw-r--r--   0        0        0     1657 2024-05-03 19:25:27.914318 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py.tmp
--rw-r--r--   0        0        0      602 2024-05-03 19:16:24.523693 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/resources/pipelines/PysparkDataDeliveryBasic.json
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-03 19:25:58.856022 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/LICENSE
+-rw-r--r--   0        0        0     1827 2024-05-03 19:26:23.205381 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/pyproject.toml
+-rw-r--r--   0        0        0      208 2024-05-03 19:25:58.846022 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:25:58.796023 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/__init__.py.tmp
+-rw-r--r--   0        0        0     1007 2024-05-03 19:25:58.836022 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py
+-rw-r--r--   0        0        0      799 2024-05-03 19:25:58.796023 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py.tmp
+-rw-r--r--   0        0        0      818 2024-05-03 19:25:58.836022 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py
+-rw-r--r--   0        0        0      610 2024-05-03 19:25:58.776024 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-03 19:25:58.826022 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:25:58.776024 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/__init__.py.tmp
+-rw-r--r--   0        0        0     3938 2024-05-03 19:25:58.826022 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py
+-rw-r--r--   0        0        0     3730 2024-05-03 19:25:58.776024 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py.tmp
+-rw-r--r--   0        0        0      670 2024-05-03 19:25:58.836022 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py
+-rw-r--r--   0        0        0      462 2024-05-03 19:25:58.796023 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py.tmp
+-rw-r--r--   0        0        0     1902 2024-05-03 19:25:58.836022 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py
+-rw-r--r--   0        0        0     1694 2024-05-03 19:25:58.796023 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py.tmp
+-rw-r--r--   0        0        0     1865 2024-05-03 19:25:58.836022 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py
+-rw-r--r--   0        0        0     1657 2024-05-03 19:25:58.806023 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py.tmp
+-rw-r--r--   0        0        0      602 2024-05-03 19:16:24.721112 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/resources/pipelines/PysparkDataDeliveryBasic.json
+-rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/PKG-INFO
```

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/LICENSE` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/pyproject.toml` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # GENERATED STUB - PLEASE ***DO*** MODIFY
 
 [tool.poetry]
 name = "aissemble-test-data-delivery-pyspark-model-basic"
-version = "1.7.0.dev1714764350"
+version = "1.7.0.dev1714764382"
 description = "Pyspark test module"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 
 # Ensure that generated code is included in package archives
 include = ["src/aissemble_test_data_delivery_pyspark_model_basic/generated/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py.tmp` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/src/aissemble_test_data_delivery_pyspark_model_basic/resources/pipelines/PysparkDataDeliveryBasic.json` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/src/aissemble_test_data_delivery_pyspark_model_basic/resources/pipelines/PysparkDataDeliveryBasic.json`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764350/PKG-INFO` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1714764382/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-test-data-delivery-pyspark-model-basic
-Version: 1.7.0.dev1714764350
+Version: 1.7.0.dev1714764382
 Summary: Pyspark test module
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aissemble-extensions-data-delivery-spark-py (==1.7.0.*)
```


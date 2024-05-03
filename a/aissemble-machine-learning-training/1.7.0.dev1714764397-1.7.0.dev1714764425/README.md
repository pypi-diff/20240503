# Comparing `tmp/aissemble_machine_learning_training-1.7.0.dev1714764397.tar.gz` & `tmp/aissemble_machine_learning_training-1.7.0.dev1714764425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_machine_learning_training-1.7.0.dev1714764397.tar", max compression
+gzip compressed data, was "aissemble_machine_learning_training-1.7.0.dev1714764425.tar", max compression
```

## Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397.tar` & `aissemble_machine_learning_training-1.7.0.dev1714764425.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     9580 2024-05-03 19:26:04.483297 aissemble_machine_learning_training-1.7.0.dev1714764397/LICENSE
--rw-r--r--   0        0        0     1725 2024-05-03 19:26:37.844282 aissemble_machine_learning_training-1.7.0.dev1714764397/pyproject.toml
--rw-r--r--   0        0        0      224 2024-05-03 19:26:04.460297 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:04.394298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/__init__.py.tmp
--rw-r--r--   0        0        0    16690 2024-05-03 19:26:04.465298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py
--rw-r--r--   0        0        0    16465 2024-05-03 19:26:04.408298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py.tmp
--rw-r--r--   0        0        0     4725 2024-05-03 19:26:04.444298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py
--rw-r--r--   0        0        0     4501 2024-05-03 19:26:04.387297 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py.tmp
--rw-r--r--   0        0        0      224 2024-05-03 19:26:04.445298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:04.394298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/__init__.py.tmp
--rw-r--r--   0        0        0     1900 2024-05-03 19:26:04.460297 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py
--rw-r--r--   0        0        0     1676 2024-05-03 19:26:04.421298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py.tmp
--rw-r--r--   0        0        0     1956 2024-05-03 19:26:04.451298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py
--rw-r--r--   0        0        0     1732 2024-05-03 19:26:04.400297 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py.tmp
--rw-r--r--   0        0        0     1641 2024-05-03 19:26:04.453297 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py
--rw-r--r--   0        0        0     1417 2024-05-03 19:26:04.402298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py.tmp
--rw-r--r--   0        0        0     1984 2024-05-03 19:26:04.449298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py
--rw-r--r--   0        0        0     1760 2024-05-03 19:26:04.398298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py.tmp
--rw-r--r--   0        0        0     2002 2024-05-03 19:26:04.447298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py
--rw-r--r--   0        0        0     1778 2024-05-03 19:26:04.397297 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py.tmp
--rw-r--r--   0        0        0     4836 2024-05-03 19:26:04.458298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py
--rw-r--r--   0        0        0     4612 2024-05-03 19:26:04.418298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py.tmp
--rw-r--r--   0        0        0     4294 2024-05-03 19:26:04.455298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py
--rw-r--r--   0        0        0     4070 2024-05-03 19:26:04.415298 aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py.tmp
--rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 aissemble_machine_learning_training-1.7.0.dev1714764397/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-03 19:26:38.264963 aissemble_machine_learning_training-1.7.0.dev1714764425/LICENSE
+-rw-r--r--   0        0        0     1725 2024-05-03 19:27:05.914225 aissemble_machine_learning_training-1.7.0.dev1714764425/pyproject.toml
+-rw-r--r--   0        0        0      224 2024-05-03 19:26:38.244964 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:38.164966 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/__init__.py.tmp
+-rw-r--r--   0        0        0    16690 2024-05-03 19:26:38.254963 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py
+-rw-r--r--   0        0        0    16465 2024-05-03 19:26:38.184965 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py.tmp
+-rw-r--r--   0        0        0     4725 2024-05-03 19:26:38.224964 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py
+-rw-r--r--   0        0        0     4501 2024-05-03 19:26:38.154966 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py.tmp
+-rw-r--r--   0        0        0      224 2024-05-03 19:26:38.224964 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:38.164966 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/__init__.py.tmp
+-rw-r--r--   0        0        0     1900 2024-05-03 19:26:38.244964 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py
+-rw-r--r--   0        0        0     1676 2024-05-03 19:26:38.194965 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py.tmp
+-rw-r--r--   0        0        0     1956 2024-05-03 19:26:38.234964 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py
+-rw-r--r--   0        0        0     1732 2024-05-03 19:26:38.174965 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py.tmp
+-rw-r--r--   0        0        0     1641 2024-05-03 19:26:38.234964 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py
+-rw-r--r--   0        0        0     1417 2024-05-03 19:26:38.174965 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py.tmp
+-rw-r--r--   0        0        0     1984 2024-05-03 19:26:38.234964 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py
+-rw-r--r--   0        0        0     1760 2024-05-03 19:26:38.174965 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py.tmp
+-rw-r--r--   0        0        0     2002 2024-05-03 19:26:38.224964 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py
+-rw-r--r--   0        0        0     1778 2024-05-03 19:26:38.174965 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py.tmp
+-rw-r--r--   0        0        0     4836 2024-05-03 19:26:38.244964 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py
+-rw-r--r--   0        0        0     4612 2024-05-03 19:26:38.194965 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py.tmp
+-rw-r--r--   0        0        0     4294 2024-05-03 19:26:38.234964 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py
+-rw-r--r--   0        0        0     4070 2024-05-03 19:26:38.194965 aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py.tmp
+-rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 aissemble_machine_learning_training-1.7.0.dev1714764425/PKG-INFO
```

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/LICENSE` & `aissemble_machine_learning_training-1.7.0.dev1714764425/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/pyproject.toml` & `aissemble_machine_learning_training-1.7.0.dev1714764425/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GENERATED STUB - PLEASE ***DO*** MODIFY
 # Originally generated from templates/general-mlflow/pyproject.toml.vm.
 
 [tool.poetry]
 name = "aissemble-machine-learning-training"
-version = "1.7.0.dev1714764397"
+version = "1.7.0.dev1714764425"
 description = "Description of package"
 authors = ["Your Name <you@example.com>"]
 
 # Ensure that generated code is included in package archives
 include = ["src/aissemble_machine_learning_training/generated/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1714764425/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1714764397/PKG-INFO` & `aissemble_machine_learning_training-1.7.0.dev1714764425/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-machine-learning-training
-Version: 1.7.0.dev1714764397
+Version: 1.7.0.dev1714764425
 Summary: Description of package
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aissemble-foundation-core-python (==1.7.0.*)
```


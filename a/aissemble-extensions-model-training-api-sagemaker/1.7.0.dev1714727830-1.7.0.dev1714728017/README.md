# Comparing `tmp/aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830.tar.gz` & `tmp/aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830.tar", max compression
+gzip compressed data, was "aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017.tar", max compression
```

## Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830.tar` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9580 2024-05-03 09:16:31.006674 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830/LICENSE
--rw-r--r--   0        0        0        0 2024-05-03 08:12:09.201240 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830/README.md
--rw-r--r--   0        0        0      791 2024-05-03 09:17:11.035622 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830/pyproject.toml
--rw-r--r--   0        0        0     8837 2024-05-03 08:12:09.202240 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830/src/model_training_api_sagemaker/model_training_api_sagemaker.py
--rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-03 09:19:34.930888 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-03 08:12:09.081403 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017/README.md
+-rw-r--r--   0        0        0      791 2024-05-03 09:20:18.069712 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017/pyproject.toml
+-rw-r--r--   0        0        0     8837 2024-05-03 08:12:09.081403 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017/src/model_training_api_sagemaker/model_training_api_sagemaker.py
+-rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017/PKG-INFO
```

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830/LICENSE` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830/pyproject.toml` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-extensions-model-training-api-sagemaker"
-version = "1.7.0.dev1714727830"
+version = "1.7.0.dev1714728017"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "model_training_api_sagemaker", from = "src"},
 ]
```

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830/src/model_training_api_sagemaker/model_training_api_sagemaker.py` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017/src/model_training_api_sagemaker/model_training_api_sagemaker.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714727830/PKG-INFO` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714728017/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-extensions-model-training-api-sagemaker
-Version: 1.7.0.dev1714727830
+Version: 1.7.0.dev1714728017
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: fastapi (>=0.95.0)
 Requires-Dist: krausening (>=19)
```


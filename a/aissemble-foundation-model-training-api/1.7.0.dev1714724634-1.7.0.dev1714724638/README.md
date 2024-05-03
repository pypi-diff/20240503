# Comparing `tmp/aissemble_foundation_model_training_api-1.7.0.dev1714724634.tar.gz` & `tmp/aissemble_foundation_model_training_api-1.7.0.dev1714724638.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_model_training_api-1.7.0.dev1714724634.tar", max compression
+gzip compressed data, was "aissemble_foundation_model_training_api-1.7.0.dev1714724638.tar", max compression
```

## Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714724634.tar` & `aissemble_foundation_model_training_api-1.7.0.dev1714724638.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     9580 2024-05-03 08:23:38.263434 aissemble_foundation_model_training_api-1.7.0.dev1714724634/LICENSE
--rw-r--r--   0        0        0      318 2024-05-03 08:12:09.245240 aissemble_foundation_model_training_api-1.7.0.dev1714724634/LICENSE.txt
--rw-r--r--   0        0        0     1796 2024-05-03 08:12:09.245240 aissemble_foundation_model_training_api-1.7.0.dev1714724634/README.md
--rw-r--r--   0        0        0      859 2024-05-03 08:23:54.652415 aissemble_foundation_model_training_api-1.7.0.dev1714724634/pyproject.toml
--rw-r--r--   0        0        0     6779 2024-05-03 08:12:09.245240 aissemble_foundation_model_training_api-1.7.0.dev1714724634/src/model_training_api/model_training_api.py
--rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 aissemble_foundation_model_training_api-1.7.0.dev1714724634/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-03 08:23:41.422565 aissemble_foundation_model_training_api-1.7.0.dev1714724638/LICENSE
+-rw-r--r--   0        0        0      318 2024-05-03 08:12:09.121402 aissemble_foundation_model_training_api-1.7.0.dev1714724638/LICENSE.txt
+-rw-r--r--   0        0        0     1796 2024-05-03 08:12:09.131402 aissemble_foundation_model_training_api-1.7.0.dev1714724638/README.md
+-rw-r--r--   0        0        0      859 2024-05-03 08:23:59.192077 aissemble_foundation_model_training_api-1.7.0.dev1714724638/pyproject.toml
+-rw-r--r--   0        0        0     6779 2024-05-03 08:12:09.131402 aissemble_foundation_model_training_api-1.7.0.dev1714724638/src/model_training_api/model_training_api.py
+-rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 aissemble_foundation_model_training_api-1.7.0.dev1714724638/PKG-INFO
```

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714724634/LICENSE` & `aissemble_foundation_model_training_api-1.7.0.dev1714724638/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714724634/README.md` & `aissemble_foundation_model_training_api-1.7.0.dev1714724638/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714724634/pyproject.toml` & `aissemble_foundation_model_training_api-1.7.0.dev1714724638/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-model-training-api"
-version = "1.7.0.dev1714724634"
+version = "1.7.0.dev1714724638"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "model_training_api", from = "src"},
 ]
```

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714724634/src/model_training_api/model_training_api.py` & `aissemble_foundation_model_training_api-1.7.0.dev1714724638/src/model_training_api/model_training_api.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714724634/PKG-INFO` & `aissemble_foundation_model_training_api-1.7.0.dev1714724638/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-model-training-api
-Version: 1.7.0.dev1714724634
+Version: 1.7.0.dev1714724638
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: aissemble-foundation-messaging-python (==1.7.0.*)
 Requires-Dist: fastapi (>=0.95.0)
```


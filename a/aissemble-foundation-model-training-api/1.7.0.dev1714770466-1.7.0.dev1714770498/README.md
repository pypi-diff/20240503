# Comparing `tmp/aissemble_foundation_model_training_api-1.7.0.dev1714770466.tar.gz` & `tmp/aissemble_foundation_model_training_api-1.7.0.dev1714770498.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_model_training_api-1.7.0.dev1714770466.tar", max compression
+gzip compressed data, was "aissemble_foundation_model_training_api-1.7.0.dev1714770498.tar", max compression
```

## Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714770466.tar` & `aissemble_foundation_model_training_api-1.7.0.dev1714770498.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     9580 2024-05-03 21:07:15.169565 aissemble_foundation_model_training_api-1.7.0.dev1714770466/LICENSE
--rw-r--r--   0        0        0      318 2024-05-03 20:58:59.567138 aissemble_foundation_model_training_api-1.7.0.dev1714770466/LICENSE.txt
--rw-r--r--   0        0        0     1796 2024-05-03 20:58:59.567138 aissemble_foundation_model_training_api-1.7.0.dev1714770466/README.md
--rw-r--r--   0        0        0      859 2024-05-03 21:07:47.076526 aissemble_foundation_model_training_api-1.7.0.dev1714770466/pyproject.toml
--rw-r--r--   0        0        0     6779 2024-05-03 20:58:59.567138 aissemble_foundation_model_training_api-1.7.0.dev1714770466/src/model_training_api/model_training_api.py
--rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 aissemble_foundation_model_training_api-1.7.0.dev1714770466/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-03 21:08:00.764396 aissemble_foundation_model_training_api-1.7.0.dev1714770498/LICENSE
+-rw-r--r--   0        0        0      318 2024-05-03 20:59:00.598691 aissemble_foundation_model_training_api-1.7.0.dev1714770498/LICENSE.txt
+-rw-r--r--   0        0        0     1796 2024-05-03 20:59:00.598691 aissemble_foundation_model_training_api-1.7.0.dev1714770498/README.md
+-rw-r--r--   0        0        0      859 2024-05-03 21:08:18.523926 aissemble_foundation_model_training_api-1.7.0.dev1714770498/pyproject.toml
+-rw-r--r--   0        0        0     6779 2024-05-03 20:59:00.598691 aissemble_foundation_model_training_api-1.7.0.dev1714770498/src/model_training_api/model_training_api.py
+-rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 aissemble_foundation_model_training_api-1.7.0.dev1714770498/PKG-INFO
```

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714770466/LICENSE` & `aissemble_foundation_model_training_api-1.7.0.dev1714770498/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714770466/README.md` & `aissemble_foundation_model_training_api-1.7.0.dev1714770498/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714770466/pyproject.toml` & `aissemble_foundation_model_training_api-1.7.0.dev1714770498/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-model-training-api"
-version = "1.7.0.dev1714770466"
+version = "1.7.0.dev1714770498"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "model_training_api", from = "src"},
 ]
```

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714770466/src/model_training_api/model_training_api.py` & `aissemble_foundation_model_training_api-1.7.0.dev1714770498/src/model_training_api/model_training_api.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714770466/PKG-INFO` & `aissemble_foundation_model_training_api-1.7.0.dev1714770498/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-model-training-api
-Version: 1.7.0.dev1714770466
+Version: 1.7.0.dev1714770498
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: aissemble-foundation-messaging-python (==1.7.0.*)
 Requires-Dist: fastapi (>=0.95.0)
```


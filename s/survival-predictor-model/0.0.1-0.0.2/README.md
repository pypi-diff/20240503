# Comparing `tmp/survival_predictor_model-0.0.1.tar.gz` & `tmp/survival_predictor_model-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shashankagarwal/Documents/Restart/study_plan/udemy_ML_deployment/mlops-template/model_package/dist/.tmp-rvp0zsbe/surviva", last modified: Thu May  2 14:08:05 2024, max compression
+gzip compressed data, was "/Users/shashankagarwal/Documents/Restart/study_plan/udemy_ML_deployment/mlops-template/model_package/dist/.tmp-_rx1sw2j/surviva", last modified: Fri May  3 11:53:36 2024, max compression
```

## Comparing `survival_predictor_model-0.0.1.tar` & `survival_predictor_model-0.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-02 14:08:05.879087 survival_predictor_model-0.0.1/
--rw-r--r--   0 shashankagarwal   (501) staff       (20)    11357 2024-05-02 13:07:22.000000 survival_predictor_model-0.0.1/LICENSE
--rw-r--r--   0 shashankagarwal   (501) staff       (20)      392 2024-05-02 13:07:22.000000 survival_predictor_model-0.0.1/MANIFEST.in
--rw-r--r--   0 shashankagarwal   (501) staff       (20)     1185 2024-05-02 14:08:05.878529 survival_predictor_model-0.0.1/PKG-INFO
-drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-02 14:08:05.869183 survival_predictor_model-0.0.1/model/
--rw-r--r--   0 shashankagarwal   (501) staff       (20)        6 2024-04-29 13:09:13.000000 survival_predictor_model-0.0.1/model/VERSION
--rw-r--r--   0 shashankagarwal   (501) staff       (20)      847 2024-04-30 11:27:48.000000 survival_predictor_model-0.0.1/model/__init__.py
-drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-02 14:08:05.870116 survival_predictor_model-0.0.1/model/config/
--rw-r--r--   0 shashankagarwal   (501) staff       (20)        0 2024-04-29 12:57:48.000000 survival_predictor_model-0.0.1/model/config/__init__.py
--rw-r--r--   0 shashankagarwal   (501) staff       (20)     2099 2024-05-01 13:17:22.000000 survival_predictor_model-0.0.1/model/config/core.py
--rw-r--r--   0 shashankagarwal   (501) staff       (20)      656 2024-05-01 17:26:34.000000 survival_predictor_model-0.0.1/model/config.yml
-drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-02 14:08:05.871693 survival_predictor_model-0.0.1/model/datasets/
--rw-r--r--   0 shashankagarwal   (501) staff       (20)        0 2024-04-29 12:55:54.000000 survival_predictor_model-0.0.1/model/datasets/__init__.py
--rw-r--r--   0 shashankagarwal   (501) staff       (20)    23135 2024-04-30 12:05:27.000000 survival_predictor_model-0.0.1/model/datasets/test.csv
--rw-r--r--   0 shashankagarwal   (501) staff       (20)    94633 2024-04-30 12:05:27.000000 survival_predictor_model-0.0.1/model/datasets/train.csv
--rw-r--r--   0 shashankagarwal   (501) staff       (20)     1867 2024-05-01 17:24:03.000000 survival_predictor_model-0.0.1/model/pipeline.py
--rw-r--r--   0 shashankagarwal   (501) staff       (20)     1069 2024-05-01 17:34:54.000000 survival_predictor_model-0.0.1/model/predict.py
-drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-02 14:08:05.874017 survival_predictor_model-0.0.1/model/processing/
--rw-r--r--   0 shashankagarwal   (501) staff       (20)        0 2024-04-29 12:56:54.000000 survival_predictor_model-0.0.1/model/processing/__init__.py
--rw-r--r--   0 shashankagarwal   (501) staff       (20)     2686 2024-05-01 13:51:59.000000 survival_predictor_model-0.0.1/model/processing/data_manager.py
--rw-r--r--   0 shashankagarwal   (501) staff       (20)      659 2024-04-30 12:42:43.000000 survival_predictor_model-0.0.1/model/processing/features.py
--rw-r--r--   0 shashankagarwal   (501) staff       (20)     1829 2024-05-01 17:11:57.000000 survival_predictor_model-0.0.1/model/processing/validation.py
--rw-r--r--   0 shashankagarwal   (501) staff       (20)      967 2024-05-01 13:18:58.000000 survival_predictor_model-0.0.1/model/train_pipeline.py
-drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-02 14:08:05.874369 survival_predictor_model-0.0.1/model/trained_models/
--rw-r--r--   0 shashankagarwal   (501) staff       (20)     4846 2024-05-02 13:36:56.000000 survival_predictor_model-0.0.1/model/trained_models/model_output_v0.0.1.pkl
--rw-r--r--   0 shashankagarwal   (501) staff       (20)     1914 2024-05-02 13:07:22.000000 survival_predictor_model-0.0.1/pyproject.toml
-drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-02 14:08:05.865338 survival_predictor_model-0.0.1/requirements/
--rw-r--r--   0 shashankagarwal   (501) staff       (20)      578 2024-05-02 13:33:01.000000 survival_predictor_model-0.0.1/requirements/requirements.txt
--rw-r--r--   0 shashankagarwal   (501) staff       (20)       65 2024-05-02 13:32:56.000000 survival_predictor_model-0.0.1/requirements/test_requirements.txt
--rw-r--r--   0 shashankagarwal   (501) staff       (20)       38 2024-05-02 14:08:05.879217 survival_predictor_model-0.0.1/setup.cfg
--rw-r--r--   0 shashankagarwal   (501) staff       (20)     2233 2024-05-02 14:07:40.000000 survival_predictor_model-0.0.1/setup.py
-drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-02 14:08:05.877805 survival_predictor_model-0.0.1/survival_predictor_model.egg-info/
--rw-r--r--   0 shashankagarwal   (501) staff       (20)     1185 2024-05-02 14:08:05.000000 survival_predictor_model-0.0.1/survival_predictor_model.egg-info/PKG-INFO
--rw-r--r--   0 shashankagarwal   (501) staff       (20)      796 2024-05-02 14:08:05.000000 survival_predictor_model-0.0.1/survival_predictor_model.egg-info/SOURCES.txt
--rw-r--r--   0 shashankagarwal   (501) staff       (20)        1 2024-05-02 14:08:05.000000 survival_predictor_model-0.0.1/survival_predictor_model.egg-info/dependency_links.txt
--rw-r--r--   0 shashankagarwal   (501) staff       (20)      188 2024-05-02 14:08:05.000000 survival_predictor_model-0.0.1/survival_predictor_model.egg-info/requires.txt
--rw-r--r--   0 shashankagarwal   (501) staff       (20)        6 2024-05-02 14:08:05.000000 survival_predictor_model-0.0.1/survival_predictor_model.egg-info/top_level.txt
-drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-02 14:08:05.877241 survival_predictor_model-0.0.1/tests/
--rw-r--r--   0 shashankagarwal   (501) staff       (20)      473 2024-05-02 13:36:00.000000 survival_predictor_model-0.0.1/tests/test_features.py
--rw-r--r--   0 shashankagarwal   (501) staff       (20)      619 2024-05-02 13:36:06.000000 survival_predictor_model-0.0.1/tests/test_prediction.py
+drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-03 11:53:36.121119 survival_predictor_model-0.0.2/
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)    11357 2024-05-02 13:07:22.000000 survival_predictor_model-0.0.2/LICENSE
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)      392 2024-05-02 13:07:22.000000 survival_predictor_model-0.0.2/MANIFEST.in
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)     1185 2024-05-03 11:53:36.120464 survival_predictor_model-0.0.2/PKG-INFO
+drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-03 11:53:36.106809 survival_predictor_model-0.0.2/model/
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)        6 2024-05-03 11:53:30.000000 survival_predictor_model-0.0.2/model/VERSION
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)      847 2024-04-30 11:27:48.000000 survival_predictor_model-0.0.2/model/__init__.py
+drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-03 11:53:36.107709 survival_predictor_model-0.0.2/model/config/
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)        0 2024-04-29 12:57:48.000000 survival_predictor_model-0.0.2/model/config/__init__.py
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)     2099 2024-05-01 13:17:22.000000 survival_predictor_model-0.0.2/model/config/core.py
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)      656 2024-05-01 17:26:34.000000 survival_predictor_model-0.0.2/model/config.yml
+drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-03 11:53:36.110590 survival_predictor_model-0.0.2/model/datasets/
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)        0 2024-04-29 12:55:54.000000 survival_predictor_model-0.0.2/model/datasets/__init__.py
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)    23135 2024-04-30 12:05:27.000000 survival_predictor_model-0.0.2/model/datasets/test.csv
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)    94633 2024-04-30 12:05:27.000000 survival_predictor_model-0.0.2/model/datasets/train.csv
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)     1867 2024-05-01 17:24:03.000000 survival_predictor_model-0.0.2/model/pipeline.py
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)     1069 2024-05-01 17:34:54.000000 survival_predictor_model-0.0.2/model/predict.py
+drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-03 11:53:36.114161 survival_predictor_model-0.0.2/model/processing/
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)        0 2024-04-29 12:56:54.000000 survival_predictor_model-0.0.2/model/processing/__init__.py
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)     2686 2024-05-01 13:51:59.000000 survival_predictor_model-0.0.2/model/processing/data_manager.py
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)      659 2024-04-30 12:42:43.000000 survival_predictor_model-0.0.2/model/processing/features.py
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)     1829 2024-05-03 11:46:59.000000 survival_predictor_model-0.0.2/model/processing/validation.py
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)      967 2024-05-01 13:18:58.000000 survival_predictor_model-0.0.2/model/train_pipeline.py
+drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-03 11:53:36.114785 survival_predictor_model-0.0.2/model/trained_models/
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)     4846 2024-05-03 11:49:55.000000 survival_predictor_model-0.0.2/model/trained_models/model_output_v0.0.1.pkl
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)     1914 2024-05-02 13:07:22.000000 survival_predictor_model-0.0.2/pyproject.toml
+drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-03 11:53:36.103057 survival_predictor_model-0.0.2/requirements/
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)      578 2024-05-02 13:33:01.000000 survival_predictor_model-0.0.2/requirements/requirements.txt
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)       65 2024-05-02 13:32:56.000000 survival_predictor_model-0.0.2/requirements/test_requirements.txt
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)       38 2024-05-03 11:53:36.121250 survival_predictor_model-0.0.2/setup.cfg
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)     2233 2024-05-02 14:07:40.000000 survival_predictor_model-0.0.2/setup.py
+drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-03 11:53:36.119747 survival_predictor_model-0.0.2/survival_predictor_model.egg-info/
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)     1185 2024-05-03 11:53:36.000000 survival_predictor_model-0.0.2/survival_predictor_model.egg-info/PKG-INFO
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)      796 2024-05-03 11:53:36.000000 survival_predictor_model-0.0.2/survival_predictor_model.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)        1 2024-05-03 11:53:36.000000 survival_predictor_model-0.0.2/survival_predictor_model.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)      188 2024-05-03 11:53:36.000000 survival_predictor_model-0.0.2/survival_predictor_model.egg-info/requires.txt
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)        6 2024-05-03 11:53:36.000000 survival_predictor_model-0.0.2/survival_predictor_model.egg-info/top_level.txt
+drwxr-xr-x   0 shashankagarwal   (501) staff       (20)        0 2024-05-03 11:53:36.119118 survival_predictor_model-0.0.2/tests/
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)      473 2024-05-02 13:36:00.000000 survival_predictor_model-0.0.2/tests/test_features.py
+-rw-r--r--   0 shashankagarwal   (501) staff       (20)      619 2024-05-02 13:36:06.000000 survival_predictor_model-0.0.2/tests/test_prediction.py
```

### Comparing `survival_predictor_model-0.0.1/LICENSE` & `survival_predictor_model-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/PKG-INFO` & `survival_predictor_model-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survival-predictor-model
-Version: 0.0.1
+Version: 0.0.2
 Summary: A template for deploying ML model using MLOps.
 Home-page: https://github.com/shashankag14/mlops-template
 Author: Shashank Agarwal
 Author-email: shashankag14@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `survival_predictor_model-0.0.1/model/__init__.py` & `survival_predictor_model-0.0.2/model/__init__.py`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/model/config/core.py` & `survival_predictor_model-0.0.2/model/config/core.py`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/model/config.yml` & `survival_predictor_model-0.0.2/model/config.yml`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/model/datasets/test.csv` & `survival_predictor_model-0.0.2/model/datasets/test.csv`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/model/datasets/train.csv` & `survival_predictor_model-0.0.2/model/datasets/train.csv`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/model/pipeline.py` & `survival_predictor_model-0.0.2/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/model/predict.py` & `survival_predictor_model-0.0.2/model/predict.py`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/model/processing/data_manager.py` & `survival_predictor_model-0.0.2/model/processing/data_manager.py`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/model/processing/features.py` & `survival_predictor_model-0.0.2/model/processing/features.py`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/model/processing/validation.py` & `survival_predictor_model-0.0.2/model/processing/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,19 +43,19 @@
     except ValidationError as error:
         errors = error.json()
 
     return validated_data, errors
 
 
 class TitanicInputSchema(BaseModel):
-    Sex: Optional[str]
-    Age: Optional[float]
-    Sibsp: Optional[int]
-    Parch: Optional[int]
-    Fare: Optional[float]
-    Cabin: Optional[str]
-    Embarked: Optional[str]
-    Title: Optional[str]
+    sex: Optional[str]
+    age: Optional[float]
+    sibsp: Optional[int]
+    parch: Optional[int]
+    fare: Optional[float]
+    cabin: Optional[str]
+    embarked: Optional[str]
+    title: Optional[str]
 
 
 class TitanicDataInputs(BaseModel):
     inputs: List[TitanicInputSchema]
```

### Comparing `survival_predictor_model-0.0.1/model/train_pipeline.py` & `survival_predictor_model-0.0.2/model/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/model/trained_models/model_output_v0.0.1.pkl` & `survival_predictor_model-0.0.2/model/trained_models/model_output_v0.0.1.pkl`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/pyproject.toml` & `survival_predictor_model-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/requirements/requirements.txt` & `survival_predictor_model-0.0.2/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/setup.py` & `survival_predictor_model-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/survival_predictor_model.egg-info/PKG-INFO` & `survival_predictor_model-0.0.2/survival_predictor_model.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survival-predictor-model
-Version: 0.0.1
+Version: 0.0.2
 Summary: A template for deploying ML model using MLOps.
 Home-page: https://github.com/shashankag14/mlops-template
 Author: Shashank Agarwal
 Author-email: shashankag14@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `survival_predictor_model-0.0.1/survival_predictor_model.egg-info/SOURCES.txt` & `survival_predictor_model-0.0.2/survival_predictor_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `survival_predictor_model-0.0.1/tests/test_prediction.py` & `survival_predictor_model-0.0.2/tests/test_prediction.py`

 * *Files identical despite different names*


# Comparing `tmp/responsibleai_vision-0.3.7.tar.gz` & `tmp/responsibleai_vision-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_vision-0.3.7.tar", last modified: Thu Apr 11 20:22:11 2024, max compression
+gzip compressed data, was "responsibleai_vision-0.3.8.tar", last modified: Fri May  3 20:49:25 2024, max compression
```

## Comparing `responsibleai_vision-0.3.7.tar` & `responsibleai_vision-0.3.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.993970 responsibleai_vision-0.3.7/responsibleai_vision/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/responsibleai_vision/common/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/common/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/responsibleai_vision/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/managers/error_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    29096 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/managers/explainer_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/responsibleai_vision/rai_vision_insights/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/rai_vision_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49549 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/responsibleai_vision/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/utils/feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/utils/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-11 20:22:10.000000 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 20:22:10.000000 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:22:10.000000 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-11 20:22:10.000000 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 20:22:10.000000 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/tests/test_feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/tests/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/tests/test_rai_vision_automl_images_insights.py
--rw-r--r--   0 runner    (1001) docker     (127)    16408 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/tests/test_rai_vision_insights.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/tests/test_rai_vision_insights_save_and_load_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:49:25.338601 responsibleai_vision-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-03 20:49:25.338601 responsibleai_vision-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:49:25.334601 responsibleai_vision-0.3.8/responsibleai_vision/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:49:25.334601 responsibleai_vision-0.3.8/responsibleai_vision/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/common/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:49:25.334601 responsibleai_vision-0.3.8/responsibleai_vision/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15244 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/managers/error_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29096 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/managers/explainer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:49:25.338601 responsibleai_vision-0.3.8/responsibleai_vision/rai_vision_insights/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/rai_vision_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49659 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:49:25.338601 responsibleai_vision-0.3.8/responsibleai_vision/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/utils/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/utils/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/responsibleai_vision/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:49:25.338601 responsibleai_vision-0.3.8/responsibleai_vision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-03 20:49:25.000000 responsibleai_vision-0.3.8/responsibleai_vision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 20:49:25.000000 responsibleai_vision-0.3.8/responsibleai_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:49:25.000000 responsibleai_vision-0.3.8/responsibleai_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-03 20:49:25.000000 responsibleai_vision-0.3.8/responsibleai_vision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 20:49:25.000000 responsibleai_vision-0.3.8/responsibleai_vision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:49:25.338601 responsibleai_vision-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:49:25.338601 responsibleai_vision-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/tests/test_feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/tests/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/tests/test_rai_vision_automl_images_insights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16408 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/tests/test_rai_vision_insights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-05-03 20:45:33.000000 responsibleai_vision-0.3.8/tests/test_rai_vision_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_vision-0.3.7/PKG-INFO` & `responsibleai_vision-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_vision
-Version: 0.3.7
+Version: 0.3.8
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 Requires-Dist: numpy>=1.17.2
 Requires-Dist: pandas<2.0.0,>=0.25.1
 Requires-Dist: Pillow>=10.0.0; python_version > "3.7"
 Requires-Dist: Pillow<10.0.0; python_version <= "3.7"
 Requires-Dist: scikit-learn>=0.22.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: semver~=2.13.0
-Requires-Dist: responsibleai>=0.34.1
+Requires-Dist: responsibleai>=0.35.0
 Requires-Dist: torchmetrics[detection]
 Requires-Dist: vision_explanation_methods
 
 # Responsible AI Vision SDK for Python
 
 ### This package has been tested with Python 3.7, 3.8 and 3.9
```

### Comparing `responsibleai_vision-0.3.7/README.md` & `responsibleai_vision-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/responsibleai_vision/common/constants.py` & `responsibleai_vision-0.3.8/responsibleai_vision/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/responsibleai_vision/managers/error_analysis_manager.py` & `responsibleai_vision-0.3.8/responsibleai_vision/managers/error_analysis_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,21 +312,29 @@
         else:
             dropped_cols = [target_column]
         dataset = rai_insights._ext_test_df.drop(columns=dropped_cols)
         inst.__dict__['_dataset'] = dataset
         feature_names = list(dataset.columns)
         inst.__dict__['_feature_names'] = feature_names
         task_type = rai_insights.task_type
-        wrapped_model = wrap_model(rai_insights.model, dataset,
-                                   task_type,
-                                   classes=rai_insights._classes,
-                                   device=rai_insights.device)
+        classes = rai_insights._classes
+        device = rai_insights.device
+
+        test = rai_insights.test
+        image_mode = rai_insights.image_mode
+        transformations = rai_insights._transformations
+        sample = test.iloc[0:2]
+        sample = get_images(sample, image_mode, transformations)
+        wrapped_model = wrap_model(
+            rai_insights.model, sample, task_type, classes=classes,
+            device=device)
+
         inst.__dict__['_task_type'] = task_type
-        index_classes = rai_insights._classes
-        index_dataset = rai_insights.test
+        index_classes = classes
+        index_dataset = test
         if isinstance(target_column, list):
             # create copy of dataset as we will make modifications to it
             index_dataset = index_dataset.copy()
             index_classes = target_column
             labels = _concat_labels_column(index_dataset, target_column,
                                            index_classes)
             index_dataset.drop(columns=target_column, inplace=True)
```

### Comparing `responsibleai_vision-0.3.7/responsibleai_vision/managers/explainer_manager.py` & `responsibleai_vision-0.3.8/responsibleai_vision/managers/explainer_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/responsibleai_vision/rai_vision_insights/rai_vision_insights.py` & `responsibleai_vision-0.3.8/responsibleai_vision/rai_vision_insights/rai_vision_insights.py`

 * *Files 1% similar despite different names*

```diff
@@ -1091,15 +1091,17 @@
             ManagerNames.EXPLAINER: ExplainerManager,
             ManagerNames.ERROR_ANALYSIS: ErrorAnalysisManager,
         }
 
         # load current state
         RAIBaseInsights._load(
             path, inst, manager_map, RAIVisionInsights._load_metadata)
-        inst._wrapped_model = wrap_model(inst.model, inst.test, inst.task_type,
+        sample = inst.test.iloc[0:2]
+        sample = get_images(sample, inst.image_mode, inst._transformations)
+        inst._wrapped_model = wrap_model(inst.model, sample, inst.task_type,
                                          classes=inst._classes,
                                          device=inst.device)
         inst.automl_image_model = is_automl_image_model(inst._wrapped_model)
         inst.predict_output = None
         return inst
 
     def compute_object_detection_metrics(
```

### Comparing `responsibleai_vision-0.3.7/responsibleai_vision/utils/feature_extractors.py` & `responsibleai_vision-0.3.8/responsibleai_vision/utils/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/responsibleai_vision/utils/image_reader.py` & `responsibleai_vision-0.3.8/responsibleai_vision/utils/image_reader.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/responsibleai_vision/utils/image_utils.py` & `responsibleai_vision-0.3.8/responsibleai_vision/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/responsibleai_vision.egg-info/PKG-INFO` & `responsibleai_vision-0.3.8/responsibleai_vision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_vision
-Version: 0.3.7
+Version: 0.3.8
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 Requires-Dist: numpy>=1.17.2
 Requires-Dist: pandas<2.0.0,>=0.25.1
 Requires-Dist: Pillow>=10.0.0; python_version > "3.7"
 Requires-Dist: Pillow<10.0.0; python_version <= "3.7"
 Requires-Dist: scikit-learn>=0.22.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: semver~=2.13.0
-Requires-Dist: responsibleai>=0.34.1
+Requires-Dist: responsibleai>=0.35.0
 Requires-Dist: torchmetrics[detection]
 Requires-Dist: vision_explanation_methods
 
 # Responsible AI Vision SDK for Python
 
 ### This package has been tested with Python 3.7, 3.8 and 3.9
```

### Comparing `responsibleai_vision-0.3.7/responsibleai_vision.egg-info/SOURCES.txt` & `responsibleai_vision-0.3.8/responsibleai_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/setup.py` & `responsibleai_vision-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/tests/test_feature_extractors.py` & `responsibleai_vision-0.3.8/tests/test_feature_extractors.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/tests/test_image_utils.py` & `responsibleai_vision-0.3.8/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/tests/test_rai_vision_automl_images_insights.py` & `responsibleai_vision-0.3.8/tests/test_rai_vision_automl_images_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/tests/test_rai_vision_insights.py` & `responsibleai_vision-0.3.8/tests/test_rai_vision_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.7/tests/test_rai_vision_insights_save_and_load_scenarios.py` & `responsibleai_vision-0.3.8/tests/test_rai_vision_insights_save_and_load_scenarios.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 
 import numpy as np
 import PIL
 import pytest
 from common_vision_utils import (DummyFlowersPipelineSerializer,
                                  ImageClassificationPipelineSerializer,
                                  ObjectDetectionPipelineSerializer,
+                                 TorchvisionDummyPipelineSerializer,
                                  create_dummy_model,
                                  create_image_classification_pipeline,
+                                 create_raw_torchvision_classification_model,
                                  load_flowers_dataset,
                                  load_fridge_object_detection_dataset,
                                  load_imagenet_dataset, load_imagenet_labels,
                                  retrieve_fridge_object_detection_model)
 from rai_vision_insights_validator import run_and_validate_serialization
 
 from responsibleai_vision import ModelTask, RAIVisionInsights
@@ -45,14 +47,30 @@
         test = data[:3]
         label = ImageColumns.LABEL
         serializer = ImageClassificationPipelineSerializer()
 
         run_and_validate_serialization(
             pred, test, task_type, class_names, label, serializer)
 
+    def test_rai_insights_pytorch_empty_save_load_save(self):
+        data = load_flowers_dataset(upscale=False)
+        data = data[0:1]
+        # stack two of the same image since we need same
+        # image sizes for pytorch model
+        data = data.append(data).reset_index(drop=True)
+        pred = create_raw_torchvision_classification_model()
+        test = data
+        class_names = data[ImageColumns.LABEL.value].unique()
+        task_type = ModelTask.IMAGE_CLASSIFICATION
+        label = ImageColumns.LABEL
+        serializer = TorchvisionDummyPipelineSerializer()
+
+        run_and_validate_serialization(
+            pred, test, task_type, class_names, label, serializer)
+
     @pytest.mark.skip("Insufficient memory on test machines to load images")
     def test_rai_insights_large_images_save_load_save(self):
         PIL.Image.MAX_IMAGE_PIXELS = None
         data = load_flowers_dataset(upscale=True)
         model = create_dummy_model(data)
         test = data
         class_names = data[ImageColumns.LABEL.value].unique()
```


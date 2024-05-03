# Comparing `tmp/detectools-0.1.4.tar.gz` & `tmp/detectools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detectools-0.1.4.tar", last modified: Mon Apr 29 14:54:36 2024, max compression
+gzip compressed data, was "detectools-0.1.5.tar", last modified: Fri May  3 10:11:05 2024, max compression
```

## Comparing `detectools-0.1.4.tar` & `detectools-0.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 14:54:36.236121 detectools-0.1.4/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1087 2024-03-21 13:04:40.000000 detectools-0.1.4/LICENSE.txt
--rw-r--r--   0 lucas     (1002) lucas     (1002)     3107 2024-04-29 14:54:36.236121 detectools-0.1.4/PKG-INFO
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1637 2024-03-21 11:28:28.000000 detectools-0.1.4/README.md
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      599 2024-04-17 13:45:59.000000 detectools-0.1.4/README_deployment.md
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1442 2024-04-23 09:24:44.000000 detectools-0.1.4/pyproject.toml
--rw-rw-r--   0 lucas     (1002) lucas     (1002)       38 2024-04-29 14:54:36.236121 detectools-0.1.4/setup.cfg
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      145 2024-03-21 13:29:41.000000 detectools-0.1.4/setup.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 14:54:36.232121 detectools-0.1.4/src/
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 14:54:36.232121 detectools-0.1.4/src/detectools/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2051 2024-04-29 14:52:45.000000 detectools-0.1.4/src/detectools/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2417 2024-04-17 12:26:22.000000 detectools-0.1.4/src/detectools/augmentation.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    10779 2024-04-18 14:52:14.000000 detectools-0.1.4/src/detectools/dataset.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 14:54:36.232121 detectools-0.1.4/src/detectools/formats/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     3989 2024-03-21 11:28:28.000000 detectools-0.1.4/src/detectools/formats/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    13188 2024-04-29 08:39:42.000000 detectools-0.1.4/src/detectools/formats/base.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     7175 2024-04-23 07:27:53.000000 detectools-0.1.4/src/detectools/formats/detection_format.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     7057 2024-04-23 08:35:56.000000 detectools-0.1.4/src/detectools/formats/mask.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     9748 2024-04-23 07:27:33.000000 detectools-0.1.4/src/detectools/formats/segmentation_format.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     6555 2024-04-22 14:49:17.000000 detectools-0.1.4/src/detectools/inference.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2209 2024-04-15 10:47:30.000000 detectools-0.1.4/src/detectools/metrics.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 14:54:36.232121 detectools-0.1.4/src/detectools/models/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      330 2024-04-15 10:47:30.000000 detectools-0.1.4/src/detectools/models/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2641 2024-04-15 10:47:30.000000 detectools-0.1.4/src/detectools/models/base.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    11002 2024-04-17 09:16:04.000000 detectools-0.1.4/src/detectools/models/mask2former.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    10950 2024-04-15 10:47:30.000000 detectools-0.1.4/src/detectools/models/yolo.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    16594 2024-04-16 14:42:36.000000 detectools-0.1.4/src/detectools/models/yolov8_seg.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     8112 2024-04-16 07:53:15.000000 detectools-0.1.4/src/detectools/trainer.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 14:54:36.236121 detectools-0.1.4/src/detectools/utils/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)        0 2024-03-21 13:12:26.000000 detectools-0.1.4/src/detectools/utils/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     3401 2024-04-16 11:03:27.000000 detectools-0.1.4/src/detectools/utils/data_management.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     6207 2024-04-15 10:47:30.000000 detectools-0.1.4/src/detectools/utils/inference.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2775 2024-04-15 10:47:30.000000 detectools-0.1.4/src/detectools/utils/mask_utils.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    16319 2024-04-29 14:48:36.000000 detectools-0.1.4/src/detectools/utils/metrics.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1202 2024-03-21 11:28:28.000000 detectools-0.1.4/src/detectools/utils/trainer.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     4708 2024-04-29 09:26:52.000000 detectools-0.1.4/src/detectools/utils/visualisation.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 14:54:36.236121 detectools-0.1.4/src/detectools.egg-info/
--rw-r--r--   0 lucas     (1002) lucas     (1002)     3107 2024-04-29 14:54:36.000000 detectools-0.1.4/src/detectools.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1016 2024-04-29 14:54:36.000000 detectools-0.1.4/src/detectools.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1002) lucas     (1002)        1 2024-04-29 14:54:36.000000 detectools-0.1.4/src/detectools.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      218 2024-04-29 14:54:36.000000 detectools-0.1.4/src/detectools.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1002) lucas     (1002)       11 2024-04-29 14:54:36.000000 detectools-0.1.4/src/detectools.egg-info/top_level.txt
+drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.733847 detectools-0.1.5/
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1087 2024-05-03 10:08:37.000000 detectools-0.1.5/LICENSE.txt
+-rw-r--r--   0 jbernigauds  (1000) jbernigauds  (1000)     3107 2024-05-03 10:11:05.733847 detectools-0.1.5/PKG-INFO
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1637 2024-05-03 10:08:37.000000 detectools-0.1.5/README.md
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      599 2024-05-03 10:08:37.000000 detectools-0.1.5/README_deployment.md
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1442 2024-05-03 10:08:37.000000 detectools-0.1.5/pyproject.toml
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)       38 2024-05-03 10:11:05.733847 detectools-0.1.5/setup.cfg
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      145 2024-05-03 10:08:37.000000 detectools-0.1.5/setup.py
+drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.709847 detectools-0.1.5/src/
+drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.717847 detectools-0.1.5/src/detectools/
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2051 2024-05-03 10:10:21.000000 detectools-0.1.5/src/detectools/__init__.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2417 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/augmentation.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    10779 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/dataset.py
+drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.725847 detectools-0.1.5/src/detectools/formats/
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     3989 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/formats/__init__.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    13188 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/formats/base.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     7175 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/formats/detection_format.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     7057 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/formats/mask.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     9748 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/formats/segmentation_format.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     6555 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/inference.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2209 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/metrics.py
+drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.725847 detectools-0.1.5/src/detectools/models/
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      330 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/models/__init__.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2641 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/models/base.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    11002 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/models/mask2former.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    10950 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/models/yolo.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    16751 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/models/yolov8_seg.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     8112 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/trainer.py
+drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.729847 detectools-0.1.5/src/detectools/utils/
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/__init__.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     3401 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/data_management.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     6207 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/inference.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     2775 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/mask_utils.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)    16319 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/metrics.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1202 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/trainer.py
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     4708 2024-05-03 10:08:37.000000 detectools-0.1.5/src/detectools/utils/visualisation.py
+drwxrwxr-x   0 jbernigauds  (1000) jbernigauds  (1000)        0 2024-05-03 10:11:05.729847 detectools-0.1.5/src/detectools.egg-info/
+-rw-r--r--   0 jbernigauds  (1000) jbernigauds  (1000)     3107 2024-05-03 10:11:05.000000 detectools-0.1.5/src/detectools.egg-info/PKG-INFO
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)     1016 2024-05-03 10:11:05.000000 detectools-0.1.5/src/detectools.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)        1 2024-05-03 10:11:05.000000 detectools-0.1.5/src/detectools.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)      218 2024-05-03 10:11:05.000000 detectools-0.1.5/src/detectools.egg-info/requires.txt
+-rw-rw-r--   0 jbernigauds  (1000) jbernigauds  (1000)       11 2024-05-03 10:11:05.000000 detectools-0.1.5/src/detectools.egg-info/top_level.txt
```

### Comparing `detectools-0.1.4/LICENSE.txt` & `detectools-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/PKG-INFO` & `detectools-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detectools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Overlay of PyTorch to generalize trainning and inference processes for detection & instance segmentation tasks.
 Author-email: Lucas Bernigaud Samatan <lucas.bernigaud-samatan@inrae.fr>, Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 Maintainer-email: Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 License: The MIT License (MIT)
         
         Copyright (c) <year> <copyright holders>
```

### Comparing `detectools-0.1.4/README.md` & `detectools-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/README_deployment.md` & `detectools-0.1.5/README_deployment.md`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/pyproject.toml` & `detectools-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/__init__.py` & `detectools-0.1.5/src/detectools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Torch prebuild functions to train, evaluate and use models in production."""
 import json
 import os
 import sys
 from pathlib import Path
 from typing import Any, Dict, Literal, Union
 
-__version__ = "0.1.4" # change detectools version here
+__version__ = "0.1.5" # change detectools version here
 
 IMAGE_FOLDER = "images"
 ANNOTATION_FILE = "coco_annotations.json"
 
 COLORS = [
     (0, 102, 204),
     (51, 255, 51),
```

### Comparing `detectools-0.1.4/src/detectools/augmentation.py` & `detectools-0.1.5/src/detectools/augmentation.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/dataset.py` & `detectools-0.1.5/src/detectools/dataset.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/formats/__init__.py` & `detectools-0.1.5/src/detectools/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/formats/base.py` & `detectools-0.1.5/src/detectools/formats/base.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/formats/detection_format.py` & `detectools-0.1.5/src/detectools/formats/detection_format.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/formats/mask.py` & `detectools-0.1.5/src/detectools/formats/mask.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/formats/segmentation_format.py` & `detectools-0.1.5/src/detectools/formats/segmentation_format.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/inference.py` & `detectools-0.1.5/src/detectools/inference.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/metrics.py` & `detectools-0.1.5/src/detectools/metrics.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/models/base.py` & `detectools-0.1.5/src/detectools/models/base.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/models/mask2former.py` & `detectools-0.1.5/src/detectools/models/mask2former.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/models/yolo.py` & `detectools-0.1.5/src/detectools/models/yolo.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/models/yolov8_seg.py` & `detectools-0.1.5/src/detectools/models/yolov8_seg.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,17 @@
         else:
             raw_outputs = self(prepared_images)
         # compute loss
         loss_dict = self.compute_loss(raw_outputs, prepared_targets)
         # return predictions if needed
         if predict:
             predictions = self.build_results(raw_outputs)
+            left, top, _, _ = self.yolo_pad_requirements(images)
+            h, w = images.shape[-2:]
+            predictions.apply("crop", top, left, h, w)
             return loss_dict, predictions
         else:
             return loss_dict
 
     def get_predictions(self, images: Tensor) -> BatchedFormats:
         """Prepare images, Apply model forward pass and build results.
```

### Comparing `detectools-0.1.4/src/detectools/trainer.py` & `detectools-0.1.5/src/detectools/trainer.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/utils/data_management.py` & `detectools-0.1.5/src/detectools/utils/data_management.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/utils/inference.py` & `detectools-0.1.5/src/detectools/utils/inference.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/utils/mask_utils.py` & `detectools-0.1.5/src/detectools/utils/mask_utils.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/utils/metrics.py` & `detectools-0.1.5/src/detectools/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/utils/trainer.py` & `detectools-0.1.5/src/detectools/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools/utils/visualisation.py` & `detectools-0.1.5/src/detectools/utils/visualisation.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.4/src/detectools.egg-info/PKG-INFO` & `detectools-0.1.5/src/detectools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detectools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Overlay of PyTorch to generalize trainning and inference processes for detection & instance segmentation tasks.
 Author-email: Lucas Bernigaud Samatan <lucas.bernigaud-samatan@inrae.fr>, Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 Maintainer-email: Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 License: The MIT License (MIT)
         
         Copyright (c) <year> <copyright holders>
```

### Comparing `detectools-0.1.4/src/detectools.egg-info/SOURCES.txt` & `detectools-0.1.5/src/detectools.egg-info/SOURCES.txt`

 * *Files identical despite different names*


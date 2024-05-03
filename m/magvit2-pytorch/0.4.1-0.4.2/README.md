# Comparing `tmp/magvit2_pytorch-0.4.1.tar.gz` & `tmp/magvit2_pytorch-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magvit2_pytorch-0.4.1.tar", last modified: Wed May  1 23:11:17 2024, max compression
+gzip compressed data, was "magvit2_pytorch-0.4.2.tar", last modified: Fri May  3 17:30:40 2024, max compression
```

## Comparing `magvit2_pytorch-0.4.1.tar` & `magvit2_pytorch-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:11:17.407495 magvit2_pytorch-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-01 23:11:17.407495 magvit2_pytorch-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:11:17.403495 magvit2_pytorch-0.4.1/magvit2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    56410 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/magvit2_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:11:17.407495 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-01 23:11:17.000000 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-01 23:11:17.000000 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:11:17.000000 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 23:11:17.000000 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 23:11:17.000000 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 23:11:17.407495 magvit2_pytorch-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:30:40.842503 magvit2_pytorch-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-03 17:30:40.842503 magvit2_pytorch-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:30:40.842503 magvit2_pytorch-0.4.2/magvit2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56410 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/magvit2_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/magvit2_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:30:40.842503 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-03 17:30:40.000000 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-03 17:30:40.000000 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:30:40.000000 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-03 17:30:40.000000 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 17:30:40.000000 magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:30:40.842503 magvit2_pytorch-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-03 17:30:36.000000 magvit2_pytorch-0.4.2/setup.py
```

### Comparing `magvit2_pytorch-0.4.1/LICENSE` & `magvit2_pytorch-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.1/PKG-INFO` & `magvit2_pytorch-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magvit2-pytorch
-Version: 0.4.1
+Version: 0.4.2
 Summary: MagViT2 - Pytorch
 Home-page: https://github.com/lucidrains/magvit2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,attention mechanisms,generative video model
 Classifier: Development Status :: 4 - Beta
@@ -21,12 +21,12 @@
 Requires-Dist: pytorch-warmup
 Requires-Dist: gateloop-transformer>=0.2.2
 Requires-Dist: kornia
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 Requires-Dist: pytorch-custom-utils>=0.0.9
 Requires-Dist: numpy
-Requires-Dist: vector-quantize-pytorch>=1.11.8
+Requires-Dist: vector-quantize-pytorch>=1.14.10
 Requires-Dist: taylor-series-linear-attention>=0.1.5
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: x-transformers
```

### Comparing `magvit2_pytorch-0.4.1/README.md` & `magvit2_pytorch-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.1/magvit2_pytorch/attend.py` & `magvit2_pytorch-0.4.2/magvit2_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.1/magvit2_pytorch/data.py` & `magvit2_pytorch-0.4.2/magvit2_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.1/magvit2_pytorch/magvit2_pytorch.py` & `magvit2_pytorch-0.4.2/magvit2_pytorch/magvit2_pytorch.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.1/magvit2_pytorch/optimizer.py` & `magvit2_pytorch-0.4.2/magvit2_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.1/magvit2_pytorch/trainer.py` & `magvit2_pytorch-0.4.2/magvit2_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/PKG-INFO` & `magvit2_pytorch-0.4.2/magvit2_pytorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magvit2-pytorch
-Version: 0.4.1
+Version: 0.4.2
 Summary: MagViT2 - Pytorch
 Home-page: https://github.com/lucidrains/magvit2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,attention mechanisms,generative video model
 Classifier: Development Status :: 4 - Beta
@@ -21,12 +21,12 @@
 Requires-Dist: pytorch-warmup
 Requires-Dist: gateloop-transformer>=0.2.2
 Requires-Dist: kornia
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 Requires-Dist: pytorch-custom-utils>=0.0.9
 Requires-Dist: numpy
-Requires-Dist: vector-quantize-pytorch>=1.11.8
+Requires-Dist: vector-quantize-pytorch>=1.14.10
 Requires-Dist: taylor-series-linear-attention>=0.1.5
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: x-transformers
```

### Comparing `magvit2_pytorch-0.4.1/setup.py` & `magvit2_pytorch-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     'pytorch-warmup',
     'gateloop-transformer>=0.2.2',
     'kornia',
     'opencv-python',
     'pillow',
     'pytorch-custom-utils>=0.0.9',
     'numpy',
-    'vector-quantize-pytorch>=1.11.8',
+    'vector-quantize-pytorch>=1.14.10',
     'taylor-series-linear-attention>=0.1.5',
     'torch',
     'torchvision',
     'x-transformers'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
```


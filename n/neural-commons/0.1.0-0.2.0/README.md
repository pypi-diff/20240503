# Comparing `tmp/neural-commons-0.1.0.tar.gz` & `tmp/neural-commons-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-commons-0.1.0.tar", last modified: Sun Apr 28 17:26:52 2024, max compression
+gzip compressed data, was "neural-commons-0.2.0.tar", last modified: Fri May  3 17:47:18 2024, max compression
```

## Comparing `neural-commons-0.1.0.tar` & `neural-commons-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.785545 neural-commons-0.1.0/
--rw-rw-rw-   0        0        0      745 2024-04-28 17:26:52.785545 neural-commons-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-28 15:46:56.000000 neural-commons-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.752250 neural-commons-0.1.0/neural_commons/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.754289 neural-commons-0.1.0/neural_commons/cf_nn/
--rw-rw-rw-   0        0        0     3238 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/cf_nn/CFConv2d.py
--rw-rw-rw-   0        0        0     1511 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/cf_nn/CFLinear.py
--rw-rw-rw-   0        0        0      305 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/cf_nn/CFModule.py
--rw-rw-rw-   0        0        0     8322 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/cf_nn/CFTrainer.py
--rw-rw-rw-   0        0        0      898 2024-04-28 16:00:09.000000 neural-commons-0.1.0/neural_commons/cf_nn/LRFunctions.py
--rw-rw-rw-   0        0        0      168 2024-04-28 16:58:17.000000 neural-commons-0.1.0/neural_commons/cf_nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.754289 neural-commons-0.1.0/neural_commons/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/helpers/__init__.py
--rw-rw-rw-   0        0        0     4887 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.785545 neural-commons-0.1.0/neural_commons/modules/
--rw-rw-rw-   0        0        0      699 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/AdaptiveSimpleNorm.py
--rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.1.0/neural_commons/modules/ConvMixer2d.py
--rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/GTanh.py
--rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/GaELU.py
--rw-rw-rw-   0        0        0     1266 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/InputEncoder.py
--rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/LogShape.py
--rw-rw-rw-   0        0        0     2188 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/NeuralLayer.py
--rw-rw-rw-   0        0        0      842 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/NeuralLayer2d.py
--rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/ParametricReLU.py
--rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.1.0/neural_commons/modules/Permute.py
--rw-rw-rw-   0        0        0      472 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/Quadratic.py
--rw-rw-rw-   0        0        0      235 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/RMSELoss.py
--rw-rw-rw-   0        0        0      470 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/RndNonLinearFunction.py
--rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/RndProjection.py
--rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.1.0/neural_commons/modules/SMoE.py
--rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/SMoEMixIn.py
--rw-rw-rw-   0        0        0      548 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.785545 neural-commons-0.1.0/neural_commons/opt/
--rw-rw-rw-   0        0        0     1909 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/opt/CosineScheduleOptimizer.py
--rw-rw-rw-   0        0        0     1428 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/opt/CosineScheduler.py
--rw-rw-rw-   0        0        0     2066 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/opt/TBCosineScheduleOptimizer.py
--rw-rw-rw-   0        0        0      174 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/opt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.754289 neural-commons-0.1.0/neural_commons.egg-info/
--rw-rw-rw-   0        0        0      745 2024-04-28 17:26:52.000000 neural-commons-0.1.0/neural_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1307 2024-04-28 17:26:52.000000 neural-commons-0.1.0/neural_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 17:26:52.000000 neural-commons-0.1.0/neural_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-28 17:26:52.000000 neural-commons-0.1.0/neural_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-28 17:26:52.000000 neural-commons-0.1.0/neural_commons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 17:26:52.785545 neural-commons-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      969 2024-04-28 15:00:31.000000 neural-commons-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.525122 neural-commons-0.2.0/
+-rw-rw-rw-   0        0        0      745 2024-05-03 17:47:18.525122 neural-commons-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-28 15:46:56.000000 neural-commons-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.462621 neural-commons-0.2.0/neural_commons/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.478246 neural-commons-0.2.0/neural_commons/cf_nn/
+-rw-rw-rw-   0        0        0     3238 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/cf_nn/CFConv2d.py
+-rw-rw-rw-   0        0        0     1511 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/cf_nn/CFLinear.py
+-rw-rw-rw-   0        0        0      778 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/CFModule.py
+-rw-rw-rw-   0        0        0    11347 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/CFTrainer.py
+-rw-rw-rw-   0        0        0      361 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/LRStrategy.py
+-rw-rw-rw-   0        0        0      166 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.478246 neural-commons-0.2.0/neural_commons/cf_nn/lrs/
+-rw-rw-rw-   0        0        0      998 2024-05-03 13:07:40.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/CrossEntropyLossLRS.py
+-rw-rw-rw-   0        0        0      989 2024-05-03 13:07:40.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/MSELossLRS.py
+-rw-rw-rw-   0        0        0     1472 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/SlideLRS.py
+-rw-rw-rw-   0        0        0      120 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.478246 neural-commons-0.2.0/neural_commons/cf_nn/lrs/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/tests/__init__.py
+-rw-rw-rw-   0        0        0     1260 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/tests/test_slide_lrs.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.493872 neural-commons-0.2.0/neural_commons/cf_nn/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/tests/__init__.py
+-rw-rw-rw-   0        0        0     6253 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/tests/test_cf_conv2d.py
+-rw-rw-rw-   0        0        0     3186 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/tests/test_cf_linear.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.493872 neural-commons-0.2.0/neural_commons/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/helpers/__init__.py
+-rw-rw-rw-   0        0        0     4887 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.525122 neural-commons-0.2.0/neural_commons/modules/
+-rw-rw-rw-   0        0        0      699 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/AdaptiveSimpleNorm.py
+-rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.2.0/neural_commons/modules/ConvMixer2d.py
+-rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/GTanh.py
+-rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/GaELU.py
+-rw-rw-rw-   0        0        0     1266 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/InputEncoder.py
+-rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/LogShape.py
+-rw-rw-rw-   0        0        0      203 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/modules/MAELoss.py
+-rw-rw-rw-   0        0        0     2188 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/NeuralLayer.py
+-rw-rw-rw-   0        0        0      842 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/NeuralLayer2d.py
+-rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/ParametricReLU.py
+-rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.2.0/neural_commons/modules/Permute.py
+-rw-rw-rw-   0        0        0      472 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/Quadratic.py
+-rw-rw-rw-   0        0        0      235 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/RMSELoss.py
+-rw-rw-rw-   0        0        0      470 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/RndNonLinearFunction.py
+-rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/RndProjection.py
+-rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.2.0/neural_commons/modules/SMoE.py
+-rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/SMoEMixIn.py
+-rw-rw-rw-   0        0        0      578 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.525122 neural-commons-0.2.0/neural_commons/opt/
+-rw-rw-rw-   0        0        0     1909 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/opt/CosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0     1428 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/opt/CosineScheduler.py
+-rw-rw-rw-   0        0        0     2066 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/opt/TBCosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0      174 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/opt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.462621 neural-commons-0.2.0/neural_commons.egg-info/
+-rw-rw-rw-   0        0        0      745 2024-05-03 17:47:18.000000 neural-commons-0.2.0/neural_commons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1722 2024-05-03 17:47:18.000000 neural-commons-0.2.0/neural_commons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 17:47:18.000000 neural-commons-0.2.0/neural_commons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-03 17:47:18.000000 neural-commons-0.2.0/neural_commons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-03 17:47:18.000000 neural-commons-0.2.0/neural_commons.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 17:47:18.525122 neural-commons-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      969 2024-05-03 17:46:06.000000 neural-commons-0.2.0/setup.py
```

### Comparing `neural-commons-0.1.0/PKG-INFO` & `neural-commons-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-commons
-Version: 0.1.0
+Version: 0.2.0
 Summary: A neural network utility library for PyTorch.
 Author: Jose Solorzano
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.23
```

### Comparing `neural-commons-0.1.0/neural_commons/cf_nn/CFConv2d.py` & `neural-commons-0.2.0/neural_commons/cf_nn/CFConv2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/cf_nn/CFLinear.py` & `neural-commons-0.2.0/neural_commons/cf_nn/CFLinear.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/helpers/torch_helper.py` & `neural-commons-0.2.0/neural_commons/helpers/torch_helper.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/modules/AdaptiveSimpleNorm.py` & `neural-commons-0.2.0/neural_commons/modules/AdaptiveSimpleNorm.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/modules/ConvMixer2d.py` & `neural-commons-0.2.0/neural_commons/modules/ConvMixer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/modules/InputEncoder.py` & `neural-commons-0.2.0/neural_commons/modules/InputEncoder.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/modules/NeuralLayer.py` & `neural-commons-0.2.0/neural_commons/modules/NeuralLayer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/modules/NeuralLayer2d.py` & `neural-commons-0.2.0/neural_commons/modules/NeuralLayer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/modules/RndProjection.py` & `neural-commons-0.2.0/neural_commons/modules/RndProjection.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/modules/SMoE.py` & `neural-commons-0.2.0/neural_commons/modules/SMoE.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/modules/SMoEMixIn.py` & `neural-commons-0.2.0/neural_commons/modules/SMoEMixIn.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/modules/__init__.py` & `neural-commons-0.2.0/neural_commons/modules/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .RMSELoss import RMSELoss
+from .MAELoss import MAELoss
 from .GaELU import GaELU
 from .GTanh import GTanh
 from .ParametricReLU import ParametricReLU
 from .Quadratic import Quadratic
 from .Permute import Permute
 from .AdaptiveSimpleNorm import AdaptiveSimpleNorm
 from .NeuralLayer import NeuralLayer
```

### Comparing `neural-commons-0.1.0/neural_commons/opt/CosineScheduleOptimizer.py` & `neural-commons-0.2.0/neural_commons/opt/CosineScheduleOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/opt/CosineScheduler.py` & `neural-commons-0.2.0/neural_commons/opt/CosineScheduler.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons/opt/TBCosineScheduleOptimizer.py` & `neural-commons-0.2.0/neural_commons/opt/TBCosineScheduleOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.1.0/neural_commons.egg-info/PKG-INFO` & `neural-commons-0.2.0/neural_commons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-commons
-Version: 0.1.0
+Version: 0.2.0
 Summary: A neural network utility library for PyTorch.
 Author: Jose Solorzano
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.23
```

### Comparing `neural-commons-0.1.0/neural_commons.egg-info/SOURCES.txt` & `neural-commons-0.2.0/neural_commons.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -6,24 +6,34 @@
 neural_commons.egg-info/dependency_links.txt
 neural_commons.egg-info/requires.txt
 neural_commons.egg-info/top_level.txt
 neural_commons/cf_nn/CFConv2d.py
 neural_commons/cf_nn/CFLinear.py
 neural_commons/cf_nn/CFModule.py
 neural_commons/cf_nn/CFTrainer.py
-neural_commons/cf_nn/LRFunctions.py
+neural_commons/cf_nn/LRStrategy.py
 neural_commons/cf_nn/__init__.py
+neural_commons/cf_nn/lrs/CrossEntropyLossLRS.py
+neural_commons/cf_nn/lrs/MSELossLRS.py
+neural_commons/cf_nn/lrs/SlideLRS.py
+neural_commons/cf_nn/lrs/__init__.py
+neural_commons/cf_nn/lrs/tests/__init__.py
+neural_commons/cf_nn/lrs/tests/test_slide_lrs.py
+neural_commons/cf_nn/tests/__init__.py
+neural_commons/cf_nn/tests/test_cf_conv2d.py
+neural_commons/cf_nn/tests/test_cf_linear.py
 neural_commons/helpers/__init__.py
 neural_commons/helpers/torch_helper.py
 neural_commons/modules/AdaptiveSimpleNorm.py
 neural_commons/modules/ConvMixer2d.py
 neural_commons/modules/GTanh.py
 neural_commons/modules/GaELU.py
 neural_commons/modules/InputEncoder.py
 neural_commons/modules/LogShape.py
+neural_commons/modules/MAELoss.py
 neural_commons/modules/NeuralLayer.py
 neural_commons/modules/NeuralLayer2d.py
 neural_commons/modules/ParametricReLU.py
 neural_commons/modules/Permute.py
 neural_commons/modules/Quadratic.py
 neural_commons/modules/RMSELoss.py
 neural_commons/modules/RndNonLinearFunction.py
```

### Comparing `neural-commons-0.1.0/setup.py` & `neural-commons-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 
 from setuptools import setup, find_packages
 
 # Define project metadata
 NAME = 'neural-commons'
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 DESCRIPTION = 'A neural network utility library for PyTorch.'
 AUTHOR = 'Jose Solorzano'
 
 REQUIRES = [
     'numpy>=1.23',
     'tqdm>=4.0.0',
     'torch>=2.1.0',
```


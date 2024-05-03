# Comparing `tmp/pepperpepper-0.0.6.7.tar.gz` & `tmp/pepperpepper-0.0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.6.7.tar", last modified: Fri May  3 07:59:04 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.6.8.tar", last modified: Fri May  3 08:07:13 2024, max compression
```

## Comparing `pepperpepper-0.0.6.7.tar` & `pepperpepper-0.0.6.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.578035 pepperpepper-0.0.6.7/
--rw-rw-rw-   0        0        0      433 2024-05-03 07:59:04.578035 pepperpepper-0.0.6.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.478664 pepperpepper-0.0.6.7/PepperPepper/
--rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.7/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.535559 pepperpepper-0.0.6.7/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.7/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.7/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.7/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.541930 pepperpepper-0.0.6.7/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.7/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.7/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.7/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.551991 pepperpepper-0.0.6.7/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.7/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.7/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.7/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.7/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.7/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.557927 pepperpepper-0.0.6.7/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.7/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.7/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.7/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.7/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.561771 pepperpepper-0.0.6.7/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.7/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.7/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.7/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.565240 pepperpepper-0.0.6.7/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.7/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.7/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.570591 pepperpepper-0.0.6.7/PepperPepper/models/
--rw-rw-rw-   0        0        0     1192 2024-05-03 07:57:17.000000 pepperpepper-0.0.6.7/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    25734 2024-05-03 07:56:28.000000 pepperpepper-0.0.6.7/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.7/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.7/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.7/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.575897 pepperpepper-0.0.6.7/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.7/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.7/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.7/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.575897 pepperpepper-0.0.6.7/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-03 07:59:04.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-05-03 07:59:04.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 07:59:04.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-03 07:59:04.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-03 07:59:04.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-03 07:59:04.578035 pepperpepper-0.0.6.7/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-03 07:57:30.000000 pepperpepper-0.0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.305228 pepperpepper-0.0.6.8/
+-rw-rw-rw-   0        0        0      433 2024-05-03 08:07:13.305228 pepperpepper-0.0.6.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.242176 pepperpepper-0.0.6.8/PepperPepper/
+-rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.8/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.273874 pepperpepper-0.0.6.8/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.8/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.8/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.8/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.273874 pepperpepper-0.0.6.8/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.8/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.8/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.8/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.273874 pepperpepper-0.0.6.8/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.8/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.8/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.8/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.8/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.8/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.291214 pepperpepper-0.0.6.8/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.8/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.8/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.8/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.8/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.291214 pepperpepper-0.0.6.8/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.8/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.8/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.8/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.291214 pepperpepper-0.0.6.8/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.8/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.8/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.291214 pepperpepper-0.0.6.8/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1192 2024-05-03 07:57:17.000000 pepperpepper-0.0.6.8/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    25740 2024-05-03 08:06:15.000000 pepperpepper-0.0.6.8/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.8/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.8/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.8/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.305228 pepperpepper-0.0.6.8/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.8/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.8/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.8/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.305228 pepperpepper-0.0.6.8/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-03 08:07:13.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-05-03 08:07:13.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 08:07:13.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-03 08:07:13.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-03 08:07:13.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-03 08:07:13.305228 pepperpepper-0.0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-03 08:06:28.000000 pepperpepper-0.0.6.8/setup.py
```

### Comparing `pepperpepper-0.0.6.7/PepperPepper/__init__.py` & `pepperpepper-0.0.6.8/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.6.8/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.6.8/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper/core/__init__.py` & `pepperpepper-0.0.6.8/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper/core/utils.py` & `pepperpepper-0.0.6.8/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.6.8/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.6.8/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.6.8/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.6.8/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.6.8/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper/models/__init__.py` & `pepperpepper-0.0.6.8/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper/models/cnn.py` & `pepperpepper-0.0.6.8/PepperPepper/models/cnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -622,15 +622,15 @@
 
     def forward(self, x):
         x = self.features(x)
         x = self.classifier(x)
         return x
 
     # resnet块
-    def _resnet_block(in_channels, out_channels, num_residual, fist_block=False):
+    def _resnet_block(self, in_channels, out_channels, num_residual, fist_block=False):
         blk = []
         for i in range(num_residual):
             if i==0 and not fist_block:
                 blk.append(ResidualBlock(in_channels, out_channels, strides=2))
             else:
                 blk.append(ResidualBlock(out_channels, out_channels))
         return blk
```

### Comparing `pepperpepper-0.0.6.7/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.6.8/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.6.8/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.7/setup.py` & `pepperpepper-0.0.6.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.6.7",
+    version="0.0.6.8",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```


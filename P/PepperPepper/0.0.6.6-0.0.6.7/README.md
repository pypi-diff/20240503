# Comparing `tmp/pepperpepper-0.0.6.6.tar.gz` & `tmp/pepperpepper-0.0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.6.6.tar", last modified: Fri May  3 06:42:19 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.6.7.tar", last modified: Fri May  3 07:59:04 2024, max compression
```

## Comparing `pepperpepper-0.0.6.6.tar` & `pepperpepper-0.0.6.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.429593 pepperpepper-0.0.6.6/
--rw-rw-rw-   0        0        0      433 2024-05-03 06:42:19.429593 pepperpepper-0.0.6.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.335367 pepperpepper-0.0.6.6/PepperPepper/
--rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.6/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.367930 pepperpepper-0.0.6.6/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.6/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.6/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.6/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.382826 pepperpepper-0.0.6.6/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.6/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.6/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.6/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.397950 pepperpepper-0.0.6.6/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.6/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.6/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.6/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.6/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.6/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.404958 pepperpepper-0.0.6.6/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.6/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.6/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.6/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.6/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.413966 pepperpepper-0.0.6.6/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.6/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.6/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.6/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.413966 pepperpepper-0.0.6.6/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.6/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.6/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.413966 pepperpepper-0.0.6.6/PepperPepper/models/
--rw-rw-rw-   0        0        0     1153 2024-05-03 06:41:21.000000 pepperpepper-0.0.6.6/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    23427 2024-05-03 06:40:08.000000 pepperpepper-0.0.6.6/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.6/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.6/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.6/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.413966 pepperpepper-0.0.6.6/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.6/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.6/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.6/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.429593 pepperpepper-0.0.6.6/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-03 06:42:19.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-05-03 06:42:19.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 06:42:19.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-03 06:42:19.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-03 06:42:19.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-03 06:42:19.429593 pepperpepper-0.0.6.6/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-03 06:41:50.000000 pepperpepper-0.0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.578035 pepperpepper-0.0.6.7/
+-rw-rw-rw-   0        0        0      433 2024-05-03 07:59:04.578035 pepperpepper-0.0.6.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.478664 pepperpepper-0.0.6.7/PepperPepper/
+-rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.7/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.535559 pepperpepper-0.0.6.7/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.7/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.7/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.7/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.541930 pepperpepper-0.0.6.7/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.7/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.7/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.7/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.551991 pepperpepper-0.0.6.7/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.7/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.7/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.7/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.7/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.7/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.557927 pepperpepper-0.0.6.7/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.7/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.7/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.7/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.7/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.561771 pepperpepper-0.0.6.7/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.7/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.7/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.7/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.565240 pepperpepper-0.0.6.7/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.7/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.7/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.570591 pepperpepper-0.0.6.7/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1192 2024-05-03 07:57:17.000000 pepperpepper-0.0.6.7/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    25734 2024-05-03 07:56:28.000000 pepperpepper-0.0.6.7/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.7/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.7/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.7/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.575897 pepperpepper-0.0.6.7/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.7/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.7/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.7/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:59:04.575897 pepperpepper-0.0.6.7/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-03 07:59:04.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-05-03 07:59:04.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 07:59:04.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-03 07:59:04.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-03 07:59:04.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.7/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-03 07:59:04.578035 pepperpepper-0.0.6.7/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-03 07:57:30.000000 pepperpepper-0.0.6.7/setup.py
```

### Comparing `pepperpepper-0.0.6.6/PepperPepper/__init__.py` & `pepperpepper-0.0.6.7/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.6.7/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.6.7/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/PepperPepper/core/__init__.py` & `pepperpepper-0.0.6.7/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/PepperPepper/core/utils.py` & `pepperpepper-0.0.6.7/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.6.7/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.6.7/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.6.7/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.6.7/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.6.7/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/PepperPepper/models/__init__.py` & `pepperpepper-0.0.6.7/PepperPepper/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .cnn import VGG16
 from .cnn import MLPConv
 from .cnn import NiNBlock
 from .cnn import NiN
 from .cnn import InceptionBlockV1
 from .cnn import GoogLeNet
 from .cnn import ResidualBlock
+from .cnn import ResNet
 
 
 
 #from .rnn import RNNModel
 #from .transformer import TransformerModel
 #from .custom_model import CustomModel
 
@@ -34,9 +35,10 @@
    'VGGBlock',
    'VGG16',
    'MLPConv',
    'NiNBlock',
    'NiN',
    'InceptionBlockV1',
    'GoogLeNet',
-   'ResidualBlock'
+   'ResidualBlock',
+   'ResNet'
 ]
```

### Comparing `pepperpepper-0.0.6.6/PepperPepper/models/cnn.py` & `pepperpepper-0.0.6.7/PepperPepper/models/cnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -574,10 +574,65 @@
 
         # 主路径输出
         shortcut = self.shortcut(x)
 
         # 将残差路径和主路径的输出相加，并经过ReLU激活函数
         out = shortcut + residual
         out = torch.nn.functional.relu(out)
+        return out
+
+
+
+
+
+"""
+10.ResNet的复现
+简介：ResNet最突出的特点是采用了残差学习（residual learning）的思想。这种思想通过引入残差块（Residual Block），跳过网络的某些层或部分，直接将输入传到后面的层中。残差块的设计使得模型可以学习到残差，即剩余的映射，而不仅仅是对输入的变换。通过引入残差连接，ResNet使得信息可以更容易地在网络中传播，即使网络非常深，梯度也可以通过残差连接直接传递到较浅层，从而避免了梯度消失的问题。
+
+"""
+class ResNet(torch.nn.Module):
+    def __init__(self, in_channels=3, num_classes=1000):
+        super(ResNet,self).__init__()
+
+        # 第一个模块：7x7的卷积层+3x3的最大汇聚层
+        self.block1 = torch.nn.Sequential(
+            torch.nn.Conv2d(in_channels, 64, kernel_size=7, stride=2, padding=3),
+            torch.nn.BatchNorm2d(64),
+            torch.nn.ReLU(),
+            torch.nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
+        )
+
+        # 第二个模块~第五个模块都是有两个残差块组成
+        self.block2 = torch.nn.Sequential(*self._resnet_block(64,64,2,True))
+        self.block3 = torch.nn.Sequential(*self._resnet_block(64,128,2))
+        self.block4 = torch.nn.Sequential(*self._resnet_block(128,256,2))
+        self.block5 = torch.nn.Sequential(*self._resnet_block(256,512,2))
+
+        #  特征提取
+        self.features = torch.nn.Sequential(
+            self.block1,self.block2,self.block3,self.block4,self.block5,
+            torch.nn.AdaptiveAvgPool2d((1, 1)),
+        )
+
+        # 分类器
+        self.classifier = torch.nn.Sequential(
+            torch.nn.Flatten(),
+            torch.nn.Linear(512,num_classes)
+        )
+
+
+    def forward(self, x):
+        x = self.features(x)
+        x = self.classifier(x)
+        return x
+
+    # resnet块
+    def _resnet_block(in_channels, out_channels, num_residual, fist_block=False):
+        blk = []
+        for i in range(num_residual):
+            if i==0 and not fist_block:
+                blk.append(ResidualBlock(in_channels, out_channels, strides=2))
+            else:
+                blk.append(ResidualBlock(out_channels, out_channels))
+        return blk
 
 
-        return out
```

### Comparing `pepperpepper-0.0.6.6/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.6.7/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.6.7/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.6/setup.py` & `pepperpepper-0.0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.6.6",
+    version="0.0.6.7",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```


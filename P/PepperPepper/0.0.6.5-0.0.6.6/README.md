# Comparing `tmp/pepperpepper-0.0.6.5.tar.gz` & `tmp/pepperpepper-0.0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.6.5.tar", last modified: Fri May  3 03:58:50 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.6.6.tar", last modified: Fri May  3 06:42:19 2024, max compression
```

## Comparing `pepperpepper-0.0.6.5.tar` & `pepperpepper-0.0.6.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:50.594563 pepperpepper-0.0.6.5/
--rw-rw-rw-   0        0        0      433 2024-05-03 03:58:50.594563 pepperpepper-0.0.6.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:50.528268 pepperpepper-0.0.6.5/PepperPepper/
--rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.5/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:50.565589 pepperpepper-0.0.6.5/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.5/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.5/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.5/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:50.565589 pepperpepper-0.0.6.5/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.5/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.5/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.5/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:50.576496 pepperpepper-0.0.6.5/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.5/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.5/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.5/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.5/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.5/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:50.576496 pepperpepper-0.0.6.5/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.5/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.5/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.5/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.5/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:50.584503 pepperpepper-0.0.6.5/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.5/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.5/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.5/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:50.584503 pepperpepper-0.0.6.5/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.5/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.5/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:50.594563 pepperpepper-0.0.6.5/PepperPepper/models/
--rw-rw-rw-   0        0        0     1100 2024-05-02 09:25:35.000000 pepperpepper-0.0.6.5/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    21481 2024-05-03 03:58:06.000000 pepperpepper-0.0.6.5/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.5/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.5/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.5/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:50.594563 pepperpepper-0.0.6.5/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.5/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.5/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.5/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:58:50.594563 pepperpepper-0.0.6.5/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-03 03:58:50.000000 pepperpepper-0.0.6.5/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-05-03 03:58:50.000000 pepperpepper-0.0.6.5/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 03:58:50.000000 pepperpepper-0.0.6.5/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-03 03:58:50.000000 pepperpepper-0.0.6.5/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-03 03:58:50.000000 pepperpepper-0.0.6.5/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.5/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-03 03:58:50.594563 pepperpepper-0.0.6.5/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-03 03:58:17.000000 pepperpepper-0.0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.429593 pepperpepper-0.0.6.6/
+-rw-rw-rw-   0        0        0      433 2024-05-03 06:42:19.429593 pepperpepper-0.0.6.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.335367 pepperpepper-0.0.6.6/PepperPepper/
+-rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.6/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.367930 pepperpepper-0.0.6.6/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.6/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.6/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.6/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.382826 pepperpepper-0.0.6.6/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.6/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.6/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.6/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.397950 pepperpepper-0.0.6.6/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.6/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.6/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.6/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.6/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.6/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.404958 pepperpepper-0.0.6.6/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.6/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.6/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.6/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.6/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.413966 pepperpepper-0.0.6.6/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.6/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.6/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.6/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.413966 pepperpepper-0.0.6.6/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.6/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.6/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.413966 pepperpepper-0.0.6.6/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1153 2024-05-03 06:41:21.000000 pepperpepper-0.0.6.6/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    23427 2024-05-03 06:40:08.000000 pepperpepper-0.0.6.6/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.6/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.6/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.6/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.413966 pepperpepper-0.0.6.6/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.6/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.6/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.6/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:42:19.429593 pepperpepper-0.0.6.6/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-03 06:42:19.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-05-03 06:42:19.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 06:42:19.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-03 06:42:19.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-03 06:42:19.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.6/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-03 06:42:19.429593 pepperpepper-0.0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-03 06:41:50.000000 pepperpepper-0.0.6.6/setup.py
```

### Comparing `pepperpepper-0.0.6.5/PepperPepper/__init__.py` & `pepperpepper-0.0.6.6/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.6.6/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.6.6/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/PepperPepper/core/__init__.py` & `pepperpepper-0.0.6.6/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/PepperPepper/core/utils.py` & `pepperpepper-0.0.6.6/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.6.6/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.6.6/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.6.6/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.6.6/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.6.6/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/PepperPepper/models/__init__.py` & `pepperpepper-0.0.6.6/PepperPepper/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .cnn import VGGBlock
 from .cnn import VGG16
 from .cnn import MLPConv
 from .cnn import NiNBlock
 from .cnn import NiN
 from .cnn import InceptionBlockV1
 from .cnn import GoogLeNet
+from .cnn import ResidualBlock
 
 
 
 #from .rnn import RNNModel
 #from .transformer import TransformerModel
 #from .custom_model import CustomModel
 
@@ -32,9 +33,10 @@
    'AlexNet',
    'VGGBlock',
    'VGG16',
    'MLPConv',
    'NiNBlock',
    'NiN',
    'InceptionBlockV1',
-   'GoogLeNet'
+   'GoogLeNet',
+   'ResidualBlock'
 ]
```

### Comparing `pepperpepper-0.0.6.5/PepperPepper/models/cnn.py` & `pepperpepper-0.0.6.6/PepperPepper/models/cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,29 +47,28 @@
     def forward(self, x):
         x = self.features(x)
         #x = x.view(x.size(0), -1)  # 确保这里的展平操作是正确的
         x = self.classifier(x)
         return x
 
 
+
     def initialize_weights(self):
         for m in self.modules():
             if isinstance(m, torch.nn.Conv2d):
                 torch.nn.init.xavier_uniform_(m.weight)
                 if m.bias is not None:
                     torch.nn.init.zeros_(m.bias)
             elif isinstance(m, torch.nn.Linear):
                 torch.nn.init.xavier_uniform_(m.weight)
                 if m.bias is not None:
                     torch.nn.init.zeros_(m.bias)
 
 
 
-
-
 """
 2.AlexNet
 abstract:
         AlexNet 是 2012 年 ImageNet 竞赛的冠军模型，由 Alex Krizhevsky、Ilya Sutskever 和 Geoffrey Hinton 提出。
 
 struct:
         模型首先包含了一个特征提取部分 self.features，该部分由几个卷积层、ReLU 激活函数和最大池化层组成。然后，通过一个自适应平均池化层 self.avgpool 将特征图的大小减小到 6x6。最后，通过三个全连接层 self.classifier 进行分类。
@@ -527,7 +526,58 @@
 
         # 展平特征图，准备进行全连接层
         x = self.classifier(x)
 
         # 输出分类结果
         return x
 
+
+
+
+
+
+
+
+"""
+10.ResidualBlock的复现
+简介：残差块允许网络学习残差映射，这有助于解决深度网络中的梯度消失和表示瓶颈问题。
+参数:  
+    - in_channels: 输入的通道数  
+    - out_channels: 输出的通道数  
+    - stride: 卷积的步长，默认为1  
+"""
+class ResidualBlock(torch.nn.Module):
+    def __init__(self, in_channels, out_channels, strides=1):
+        super(ResidualBlock, self).__init__()
+
+        # 当输入输出通道数不同或者步长不为1时，需要使用一个1x1的卷积进行降维和步长调整
+        # 这样可以确保主路径（shortcut）和残差路径（residual path）的输出形状一致
+        self.shortcut = torch.nn.Sequential()
+        if strides != 1 or in_channels != out_channels:
+            self.shortcut = torch.nn.Sequential(
+                torch.nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=strides),
+            )
+
+        # 残差路径包含两个3x3的卷积层，每个卷积层后都跟着一个批量归一化层和一个ReLU激活函数
+        self.residual = torch.nn.Sequential(
+            torch.nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=strides, padding=1),
+            torch.nn.BatchNorm2d(out_channels),
+            torch.nn.ReLU(inplace=True),
+            torch.nn.Conv2d(out_channels, out_channels, kernel_size=3, padding=1),
+            torch.nn.BatchNorm2d(out_channels)
+        )
+
+        # 最后一个ReLU激活函数在残差块外部，以确保仅在残差路径有贡献时才进行非线性变换
+
+    def forward(self, x):
+        # 残差路径的输出
+        residual = self.residual(x)
+
+        # 主路径输出
+        shortcut = self.shortcut(x)
+
+        # 将残差路径和主路径的输出相加，并经过ReLU激活函数
+        out = shortcut + residual
+        out = torch.nn.functional.relu(out)
+
+
+        return out
```

### Comparing `pepperpepper-0.0.6.5/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.6.6/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.6.6/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.5/setup.py` & `pepperpepper-0.0.6.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.6.5",
+    version="0.0.6.6",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```


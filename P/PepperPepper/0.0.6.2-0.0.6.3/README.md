# Comparing `tmp/pepperpepper-0.0.6.2.tar.gz` & `tmp/pepperpepper-0.0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.6.2.tar", last modified: Thu May  2 15:26:07 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.6.3.tar", last modified: Thu May  2 15:54:48 2024, max compression
```

## Comparing `pepperpepper-0.0.6.2.tar` & `pepperpepper-0.0.6.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.940295 pepperpepper-0.0.6.2/
--rw-rw-rw-   0        0        0      433 2024-05-02 15:26:07.936291 pepperpepper-0.0.6.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.846907 pepperpepper-0.0.6.2/PepperPepper/
--rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.2/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.895025 pepperpepper-0.0.6.2/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.2/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.2/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.2/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.899562 pepperpepper-0.0.6.2/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.2/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.2/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.2/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.910310 pepperpepper-0.0.6.2/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.2/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.2/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.2/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.2/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.2/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.917204 pepperpepper-0.0.6.2/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.2/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.2/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.2/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.2/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.921018 pepperpepper-0.0.6.2/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.2/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.2/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.2/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.925122 pepperpepper-0.0.6.2/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.2/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.2/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.931121 pepperpepper-0.0.6.2/PepperPepper/models/
--rw-rw-rw-   0        0        0     1100 2024-05-02 09:25:35.000000 pepperpepper-0.0.6.2/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    21299 2024-05-02 15:24:02.000000 pepperpepper-0.0.6.2/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.2/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.2/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.2/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.934338 pepperpepper-0.0.6.2/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.2/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.2/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.2/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.935291 pepperpepper-0.0.6.2/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-02 15:26:07.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-05-02 15:26:07.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 15:26:07.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-02 15:26:07.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-02 15:26:07.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-02 15:26:07.940295 pepperpepper-0.0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      569 2024-05-02 15:26:04.000000 pepperpepper-0.0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.550886 pepperpepper-0.0.6.3/
+-rw-rw-rw-   0        0        0      433 2024-05-02 15:54:48.547881 pepperpepper-0.0.6.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.483288 pepperpepper-0.0.6.3/PepperPepper/
+-rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.3/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.513610 pepperpepper-0.0.6.3/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.3/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.3/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.3/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.518243 pepperpepper-0.0.6.3/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.3/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.3/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.3/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.524242 pepperpepper-0.0.6.3/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.3/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.3/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.3/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.3/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.3/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.528603 pepperpepper-0.0.6.3/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.3/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.3/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.3/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.3/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.531608 pepperpepper-0.0.6.3/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.3/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.3/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.3/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.534777 pepperpepper-0.0.6.3/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.3/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.3/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.543429 pepperpepper-0.0.6.3/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1100 2024-05-02 09:25:35.000000 pepperpepper-0.0.6.3/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    21449 2024-05-02 15:49:08.000000 pepperpepper-0.0.6.3/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.3/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.3/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.3/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.545895 pepperpepper-0.0.6.3/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.3/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.3/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.3/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.546906 pepperpepper-0.0.6.3/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-02 15:54:48.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-05-02 15:54:48.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 15:54:48.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-02 15:54:48.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-02 15:54:48.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-02 15:54:48.550886 pepperpepper-0.0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-02 15:54:38.000000 pepperpepper-0.0.6.3/setup.py
```

### Comparing `pepperpepper-0.0.6.2/PepperPepper/__init__.py` & `pepperpepper-0.0.6.3/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.6.3/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.6.3/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper/core/__init__.py` & `pepperpepper-0.0.6.3/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper/core/utils.py` & `pepperpepper-0.0.6.3/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.6.3/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.6.3/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.6.3/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.6.3/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.6.3/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper/models/__init__.py` & `pepperpepper-0.0.6.3/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper/models/cnn.py` & `pepperpepper-0.0.6.3/PepperPepper/models/cnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,23 @@
         LeNet5是一个经典的卷积神经网络，由多个卷积层、池化层和全连接层组成。它通过卷积操作提取图像中的局部特征，利用池化层进行特征下采样，并通过全连接层进行分类。LeNet最初用于手写数字识别任务，并展现出了良好的性能。其结构简洁明了，为后续更复杂的神经网络结构提供了基础，对深度学习领域的发展产生了重要影响。
 
 struct:
         卷积编码器：由两个卷积层组成;
         全连接层密集块：由三个全连接层组成。
 
 input: 
-        28*28的单通道（黑白）图像通过LeNet,1×28×28。
+        28*28的单通道（黑白）图像通过LeNet,in_channels×28×28。
     
 output: 
         最后一层输出为10的Linear层，分别代表十种数字的类别数。
 """
 class LeNet5(torch.nn.Module):
-    def __init__(self, num_classes=10):
+    def __init__(self,in_channels=3 ,num_classes=10):
         super(LeNet5, self).__init__()
-        self.conv1 = torch.nn.Conv2d(1, 6, 5,padding=2)  # 输入通道数为1，输出通道数为6，卷积核大小为5
+        self.conv1 = torch.nn.Conv2d(in_channels, 6, 5,padding=2)  # 输入通道数为1，输出通道数为6，卷积核大小为5
         self.conv2 = torch.nn.Conv2d(6, 16, 5)  # 输入通道数为6，输出通道数为16，卷积核大小为5
         self.fc1 = torch.nn.Linear(16 * 5 * 5, 120)  # 输入特征数为16*5*5，输出特征数为120
         self.fc2 = torch.nn.Linear(120, 84)  # 输入特征数为120，输出特征数为84
         self.fc3 = torch.nn.Linear(84, num_classes)  # 输入特征数为84，输出特征数为类别数
 
     def forward(self, x):
         # 添加ReLU激活函数和最大池化层
@@ -64,29 +64,29 @@
 abstract:
         AlexNet 是 2012 年 ImageNet 竞赛的冠军模型，由 Alex Krizhevsky、Ilya Sutskever 和 Geoffrey Hinton 提出。
 
 struct:
         模型首先包含了一个特征提取部分 self.features，该部分由几个卷积层、ReLU 激活函数和最大池化层组成。然后，通过一个自适应平均池化层 self.avgpool 将特征图的大小减小到 6x6。最后，通过三个全连接层 self.classifier 进行分类。
 
 input: 
-        输入图像的大小是 3x224x224（AlexNet 的原始输入大小）。
+        输入图像的大小是 in_channelsx224x224（AlexNet 的原始输入大小）。
 
 output: 
         num_classes 参数用于指定分类的类别数，你可以根据你的任务需求进行修改。
 """
 # 定义AlexNet模型类，继承自nn.Module
 class AlexNet(torch.nn.Module):
     # 初始化函数，用于设置网络层
-    def __init__(self, num_classes=1000):
+    def __init__(self, in_channels=3, num_classes=1000):
         super(AlexNet,self).__init__()  # 调用父类nn.Module的初始化函数
 
         # 定义特征提取部分
         self.features = torch.nn.Sequential(
             # 第一个卷积层，输入通道3（RGB），输出通道64，卷积核大小11x11，步长4，填充2
-            torch.nn.Conv2d(3, 64, kernel_size=11, stride=4, padding=2),
+            torch.nn.Conv2d(in_channels, 64, kernel_size=11, stride=4, padding=2),
             # ReLU激活函数，inplace=True表示直接修改原变量，节省内存
             torch.nn.ReLU(inplace=True),
             # 最大池化层，池化核大小3x3，步长2
             torch.nn.MaxPool2d(kernel_size=3, stride=2),
 
             # 第二个卷积层，输入通道64，输出通道192，卷积核大小5x5，填充2
             torch.nn.Conv2d(64, 192, kernel_size=5, padding=2),
@@ -197,26 +197,26 @@
 
 
 
 
 
 #4.定义VGG16模型
 class VGG16(torch.nn.Module):
-    def __init__(self, num_classes=1000):
+    def __init__(self, in_channels=3, num_classes=1000):
         """
         VGG16模型
 
         参数:
             num_classes (int, 可选): 分类的数量。默认为1000
         """
         super(VGG16, self).__init__()
 
         # 定义特征提取部分
         self.features = torch.nn.Sequential(
-            VGGBlock(3, 64, 2, pool=True),  # block1: 64 channels, 2 conv layers, maxpool
+            VGGBlock(in_channels, 64, 2, pool=True),  # block1: 64 channels, 2 conv layers, maxpool
             VGGBlock(64, 128, 2, pool=True),  # block2: 128 channels, 2 conv layers, maxpool
             VGGBlock(128, 256, 3, pool=True),  # block3: 256 channels, 3 conv layers, maxpool
             VGGBlock(256, 512, 3, pool=True),  # block4: 512 channels, 3 conv layers, maxpool
             VGGBlock(512, 512, 3, pool=True)  # block5: 512 channels, 3 conv layers, maxpool
         )
 
         # 定义分类器部分（全连接层）
@@ -308,15 +308,15 @@
 
 
 #6.NiN块
 class NiNBlock(torch.nn.Module):
     """
     NiN块，包含一个标准的卷积层和一个MLPConv层
     """
-    def __init__(self, in_channels, num_channels, kernel_size=3, stride=1, padding=1):
+    def __init__(self, in_channels, num_channels , kernel_size=3, stride=1, padding=1):
         super(NiNBlock, self).__init__()
         # 标准的卷积层
         self.conv = torch.nn.Conv2d(in_channels, num_channels, kernel_size=kernel_size, stride=stride, padding=padding, bias=True)
         # MLPConv层
         self.mlpconv = MLPConv(num_channels, num_channels // 2, num_channels)
 
 
@@ -336,19 +336,19 @@
 #7.Network in Network模型
 class NiN(torch.nn.Module):
     """
     Network in Network模型
     输入图片大小为224x224
     """
 
-    def __init__(self, num_classes=10):
+    def __init__(self, in_channels=3, num_classes=10):
         super(NiN, self).__init__()
         # 初始卷积层
         self.features = torch.nn.Sequential(
-            NiNBlock(3, 96, kernel_size=11, stride=4, padding=0),  # 使用较大的卷积核和步长来减少空间维度
+            NiNBlock(in_channels, 96, kernel_size=11, stride=4, padding=0),  # 使用较大的卷积核和步长来减少空间维度
             torch.nn.MaxPool2d(kernel_size=3, stride=2),  # 最大池化层
             NiNBlock(96, 256, kernel_size=5, stride=1, padding=2),
             torch.nn.MaxPool2d(kernel_size=3, stride=2),
             NiNBlock(256, 384, kernel_size=3, stride=1, padding=1),
             torch.nn.MaxPool2d(kernel_size=3, stride=2),
             torch.nn.Dropout(p=0.5),  # 引入Dropout层防止过拟合
             NiNBlock(384, num_classes, kernel_size=3, stride=1, padding=1),
@@ -437,31 +437,35 @@
 
 
 
 
 
 
 
+
+
+
+
 #9.GoogLeNet的复现
 """
 简介：GoogLeNet的设计特点在于既有深度，又在横向上拥有“宽度”，并采用了一种名为Inception的核心子网络结构。这个网络名字中的“GoogLeNet”是对LeNet的致敬，LeNet是早期由Yann LeCun设计的卷积神经网络。
 基本结构：
     Inception模块：这是GoogLeNet的核心子网络结构。Inception模块的基本组成结构有四个：1x1卷积、3x3卷积、5x5卷积和3x3最大池化。这四个操作并行进行以提取特征，然后将这四个操作的输出进行通道维度的拼接。这种设计使得网络能够捕捉不同尺度的特征。
     1x1卷积：在Inception模块中，1x1卷积起到了两个主要作用。首先，它可以在相同尺寸的感受野中叠加更多的卷积，从而提取到更丰富的特征。其次，它还可以用于降维，降低计算复杂度。当某个卷积层输入的特征数较多时，对输入先进行降维，减少特征数后再做卷积，可以显著减少计算量。
     辅助分类器：GoogLeNet在网络的不同深度处添加了两个辅助分类器。这些辅助分类器在训练过程中与主分类器一同进行优化，有助于提升整个网络的训练效果。
     全局平均池化：与传统的全连接层相比，全局平均池化能够减少网络参数，降低过拟合风险，并且具有更强的鲁棒性。
 """
 class GoogLeNet(torch.nn.Module):
-    def __init__(self,num_classes=1000):
+    def __init__(self, in_channels=3, num_classes=1000):
         super(GoogLeNet,self).__init__()
 
 
         # 第一个模块:使用64个通道、7x7卷积层。
         self.block1 = torch.nn.Sequential(
-            torch.nn.Conv2d(3, 64, kernel_size=7, stride=2, padding=3),
+            torch.nn.Conv2d(in_channels, 64, kernel_size=7, stride=2, padding=3),
             torch.nn.ReLU(),
             torch.nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
         )
 
 
         # 第二个模块:第一层卷积层是64个通道、1x1卷积层；第二个卷积层使用将通道数增加3x的3x3卷积层。
         self.block2 = torch.nn.Sequential(
@@ -516,9 +520,7 @@
 
         # 展平特征图，准备进行全连接层
         x = self.classifier(x)
 
         # 输出分类结果
         return x
 
-
-
```

### Comparing `pepperpepper-0.0.6.2/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.6.3/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.6.3/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.2/setup.py` & `pepperpepper-0.0.6.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,21 +10,20 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.6.2",
+    version="0.0.6.3",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
     install_requires=requirements,
 )
 
 
 
-
```


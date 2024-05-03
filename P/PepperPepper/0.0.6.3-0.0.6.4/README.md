# Comparing `tmp/pepperpepper-0.0.6.3.tar.gz` & `tmp/pepperpepper-0.0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.6.3.tar", last modified: Thu May  2 15:54:48 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.6.4.tar", last modified: Fri May  3 03:31:53 2024, max compression
```

## Comparing `pepperpepper-0.0.6.3.tar` & `pepperpepper-0.0.6.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.550886 pepperpepper-0.0.6.3/
--rw-rw-rw-   0        0        0      433 2024-05-02 15:54:48.547881 pepperpepper-0.0.6.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.483288 pepperpepper-0.0.6.3/PepperPepper/
--rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.3/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.513610 pepperpepper-0.0.6.3/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.3/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.3/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.3/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.518243 pepperpepper-0.0.6.3/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.3/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.3/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.3/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.524242 pepperpepper-0.0.6.3/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.3/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.3/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.3/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.3/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.3/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.528603 pepperpepper-0.0.6.3/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.3/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.3/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.3/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.3/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.531608 pepperpepper-0.0.6.3/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.3/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.3/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.3/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.534777 pepperpepper-0.0.6.3/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.3/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.3/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.543429 pepperpepper-0.0.6.3/PepperPepper/models/
--rw-rw-rw-   0        0        0     1100 2024-05-02 09:25:35.000000 pepperpepper-0.0.6.3/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    21449 2024-05-02 15:49:08.000000 pepperpepper-0.0.6.3/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.3/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.3/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.3/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.545895 pepperpepper-0.0.6.3/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.3/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.3/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.3/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:54:48.546906 pepperpepper-0.0.6.3/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-02 15:54:48.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-05-02 15:54:48.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 15:54:48.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-02 15:54:48.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-02 15:54:48.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.3/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-02 15:54:48.550886 pepperpepper-0.0.6.3/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-02 15:54:38.000000 pepperpepper-0.0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:31:53.010547 pepperpepper-0.0.6.4/
+-rw-rw-rw-   0        0        0      433 2024-05-03 03:31:53.010547 pepperpepper-0.0.6.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 03:31:52.866598 pepperpepper-0.0.6.4/PepperPepper/
+-rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.4/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:31:52.920420 pepperpepper-0.0.6.4/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.4/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.4/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.4/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:31:52.932474 pepperpepper-0.0.6.4/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.4/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.4/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.4/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:31:52.950154 pepperpepper-0.0.6.4/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.4/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.4/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.4/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.4/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.4/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:31:52.963317 pepperpepper-0.0.6.4/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.4/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.4/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.4/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.4/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:31:52.970583 pepperpepper-0.0.6.4/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.4/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.4/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.4/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:31:52.980570 pepperpepper-0.0.6.4/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.4/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.4/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:31:52.994984 pepperpepper-0.0.6.4/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1100 2024-05-02 09:25:35.000000 pepperpepper-0.0.6.4/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    21384 2024-05-03 03:30:05.000000 pepperpepper-0.0.6.4/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.4/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.4/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.4/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:31:53.005533 pepperpepper-0.0.6.4/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.4/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.4/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.4/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:31:53.009040 pepperpepper-0.0.6.4/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-03 03:31:52.000000 pepperpepper-0.0.6.4/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-05-03 03:31:52.000000 pepperpepper-0.0.6.4/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 03:31:52.000000 pepperpepper-0.0.6.4/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-03 03:31:52.000000 pepperpepper-0.0.6.4/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-03 03:31:52.000000 pepperpepper-0.0.6.4/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.4/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-03 03:31:53.010547 pepperpepper-0.0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-03 03:31:17.000000 pepperpepper-0.0.6.4/setup.py
```

### Comparing `pepperpepper-0.0.6.3/PepperPepper/__init__.py` & `pepperpepper-0.0.6.4/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.6.4/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.6.4/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper/core/__init__.py` & `pepperpepper-0.0.6.4/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper/core/utils.py` & `pepperpepper-0.0.6.4/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.6.4/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.6.4/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.6.4/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.6.4/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.6.4/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper/models/__init__.py` & `pepperpepper-0.0.6.4/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper/models/cnn.py` & `pepperpepper-0.0.6.4/PepperPepper/models/cnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,41 +10,47 @@
 
 struct:
         卷积编码器：由两个卷积层组成;
         全连接层密集块：由三个全连接层组成。
 
 input: 
         28*28的单通道（黑白）图像通过LeNet,in_channels×28×28。
-    
+
 output: 
         最后一层输出为10的Linear层，分别代表十种数字的类别数。
+
 """
 class LeNet5(torch.nn.Module):
     def __init__(self,in_channels=3 ,num_classes=10):
         super(LeNet5, self).__init__()
-        self.conv1 = torch.nn.Conv2d(in_channels, 6, 5,padding=2)  # 输入通道数为1，输出通道数为6，卷积核大小为5
-        self.conv2 = torch.nn.Conv2d(6, 16, 5)  # 输入通道数为6，输出通道数为16，卷积核大小为5
-        self.fc1 = torch.nn.Linear(16 * 5 * 5, 120)  # 输入特征数为16*5*5，输出特征数为120
-        self.fc2 = torch.nn.Linear(120, 84)  # 输入特征数为120，输出特征数为84
-        self.fc3 = torch.nn.Linear(84, num_classes)  # 输入特征数为84，输出特征数为类别数
+        self.features = torch.nn.Sequential(
+            torch.nn.Conv2d(in_channels, 6, 5), # 输入通道数为in_channels，输出通道数为6，卷积核大小为5
+            torch.nn.BatchNorm2d(6),
+            torch.nn.Sigmoid(),
+            torch.nn.AvgPool2d(kernel_size=2, stride=2), # 池化窗口2x2，步长2
+            torch.nn.Conv2d(6, 16, 5), # 输入通道6，输出通道16，卷积核5x5
+            torch.nn.BatchNorm2d(16),
+            torch.nn.Sigmoid(),
+            torch.nn.AvgPool2d(kernel_size=2, stride=2), # 池化窗口2x2，步长2
+        )
+
+        self.classifier = torch.nn.Sequential(
+            torch.nn.Flatten(),
+            torch.nn.Linear(256, 120),
+            torch.nn.BatchNorm1d(120),
+            torch.nn.Sigmoid(),
+            torch.nn.Linear(120, 84),
+            torch.nn.BatchNorm1d(84),
+            torch.nn.Sigmoid(),
+            torch.nn.Linear(84, num_classes)
+        )
 
     def forward(self, x):
-        # 添加ReLU激活函数和最大池化层
-        x = torch.nn.functional.sigmoid(self.conv1(x))
-        x = torch.nn.functional.max_pool2d(x, kernel_size=2,stride=2)
-        x = torch.nn.functional.sigmoid(self.conv2(x))
-        x = torch.nn.functional.max_pool2d(x, kernel_size=2,stride=2)
-
-        # 将卷积层的输出展平
-        x = x.view(x.size(0), -1)
-
-        x = torch.nn.functional.sigmoid(self.fc1(x))
-        x = torch.nn.functional.sigmoid(self.fc2(x))
-        x = self.fc3(x)
-
+        x = self.features(x)
+        x = self.classifier(x)
         return x
 
 
     def initialize_weights(self):
         for m in self.modules():
             if isinstance(m, torch.nn.Conv2d):
                 torch.nn.init.xavier_uniform_(m.weight)
```

### Comparing `pepperpepper-0.0.6.3/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.6.4/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.6.4/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.3/setup.py` & `pepperpepper-0.0.6.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.6.3",
+    version="0.0.6.4",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```


# Comparing `tmp/keras-vision-0.3.tar.gz` & `tmp/keras-vision-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-vision-0.3.tar", last modified: Fri Apr 19 21:11:04 2024, max compression
+gzip compressed data, was "keras-vision-0.4.tar", last modified: Fri May  3 19:10:00 2024, max compression
```

## Comparing `keras-vision-0.3.tar` & `keras-vision-0.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 21:11:04.203968 keras-vision-0.3/
--rw-rw-rw-   0        0        0     1142 2024-04-19 21:11:04.202961 keras-vision-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 21:11:04.184420 keras-vision-0.3/keras_vision/
-drwxrwxrwx   0        0        0        0 2024-04-19 21:11:04.201441 keras-vision-0.3/keras_vision/MobileViT_v1/
--rw-rw-rw-   0        0        0     7166 2024-04-18 19:33:34.000000 keras-vision-0.3/keras_vision/MobileViT_v1/BaseLayers.py
--rw-rw-rw-   0        0        0      500 2024-04-18 05:20:36.000000 keras-vision-0.3/keras_vision/MobileViT_v1/__init__.py
--rw-rw-rw-   0        0        0     2428 2024-04-17 12:26:24.000000 keras-vision-0.3/keras_vision/MobileViT_v1/configs.py
--rw-rw-rw-   0        0        0     8676 2024-04-18 19:30:16.000000 keras-vision-0.3/keras_vision/MobileViT_v1/minimal_example.py
--rw-rw-rw-   0        0        0     7039 2024-04-19 07:49:27.000000 keras-vision-0.3/keras_vision/MobileViT_v1/mobile_vit_v1.py
--rw-rw-rw-   0        0        0     8904 2024-04-18 05:47:49.000000 keras-vision-0.3/keras_vision/MobileViT_v1/mobile_vit_v1_block.py
--rw-rw-rw-   0        0        0     4861 2024-04-17 11:31:19.000000 keras-vision-0.3/keras_vision/MobileViT_v1/multihead_self_attention_2D.py
--rw-rw-rw-   0        0        0      523 2024-04-17 10:55:18.000000 keras-vision-0.3/keras_vision/MobileViT_v1/utils.py
--rw-rw-rw-   0        0        0       39 2024-04-17 11:28:04.000000 keras-vision-0.3/keras_vision/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 21:11:04.191466 keras-vision-0.3/keras_vision.egg-info/
--rw-rw-rw-   0        0        0     1142 2024-04-19 21:11:04.000000 keras-vision-0.3/keras_vision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2024-04-19 21:11:04.000000 keras-vision-0.3/keras_vision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 21:11:04.000000 keras-vision-0.3/keras_vision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-19 21:11:04.000000 keras-vision-0.3/keras_vision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-19 21:11:04.000000 keras-vision-0.3/keras_vision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 21:11:04.203968 keras-vision-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1823 2024-04-19 21:11:01.000000 keras-vision-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:10:00.813512 keras-vision-0.4/
+-rw-rw-rw-   0        0        0     1142 2024-05-03 19:10:00.811506 keras-vision-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 19:10:00.794632 keras-vision-0.4/keras_vision/
+drwxrwxrwx   0        0        0        0 2024-05-03 19:10:00.810491 keras-vision-0.4/keras_vision/MobileViT_v1/
+-rw-rw-rw-   0        0        0      501 2024-05-03 18:35:52.000000 keras-vision-0.4/keras_vision/MobileViT_v1/__init__.py
+-rw-rw-rw-   0        0        0     4516 2024-05-03 18:38:00.000000 keras-vision-0.4/keras_vision/MobileViT_v1/base_layers.py
+-rw-rw-rw-   0        0        0     2428 2024-05-03 18:38:07.000000 keras-vision-0.4/keras_vision/MobileViT_v1/configs.py
+-rw-rw-rw-   0        0        0     6761 2024-05-03 18:40:51.000000 keras-vision-0.4/keras_vision/MobileViT_v1/mobile_vit_v1.py
+-rw-rw-rw-   0        0        0    16065 2024-05-03 18:38:33.000000 keras-vision-0.4/keras_vision/MobileViT_v1/mobile_vit_v1_block.py
+-rw-rw-rw-   0        0        0     2529 2024-05-03 18:37:13.000000 keras-vision-0.4/keras_vision/MobileViT_v1/multihead_self_attention_2D.py
+-rw-rw-rw-   0        0        0      523 2024-04-17 10:55:18.000000 keras-vision-0.4/keras_vision/MobileViT_v1/utils.py
+-rw-rw-rw-   0        0        0       39 2024-04-17 11:28:04.000000 keras-vision-0.4/keras_vision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:10:00.801633 keras-vision-0.4/keras_vision.egg-info/
+-rw-rw-rw-   0        0        0     1142 2024-05-03 19:10:00.000000 keras-vision-0.4/keras_vision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-03 19:10:00.000000 keras-vision-0.4/keras_vision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 19:10:00.000000 keras-vision-0.4/keras_vision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 19:10:00.000000 keras-vision-0.4/keras_vision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-03 19:10:00.000000 keras-vision-0.4/keras_vision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 19:10:00.813512 keras-vision-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1823 2024-05-03 19:09:15.000000 keras-vision-0.4/setup.py
```

### Comparing `keras-vision-0.3/PKG-INFO` & `keras-vision-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-vision
-Version: 0.3
+Version: 0.4
 Summary: Building Vision models in Keras3 for framework agnostic training and inference.
 Home-page: https://github.com/veb-101/keras-vision
 Author: Vaibhav Singh
 Author-email: vaibhav.singh.3001@gmail.com
 License: Apache 2.0
 Keywords: keras3 tensorflow Jax PyTorch Vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `keras-vision-0.3/keras_vision/MobileViT_v1/configs.py` & `keras-vision-0.4/keras_vision/MobileViT_v1/configs.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.3/keras_vision/MobileViT_v1/mobile_vit_v1.py` & `keras-vision-0.4/keras_vision/MobileViT_v1/mobile_vit_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-# import os
-
-# # This guide can only be run with the jax backend.
-# os.environ["KERAS_BACKEND"] = "jax"
-
 from typing import Optional
 
 import keras.ops as kops
 from keras import Model, Input
 from keras.layers import GlobalAveragePooling2D, Dropout, Dense
 
 from .configs import get_mobile_vit_v1_configs
-from .BaseLayers import ConvLayer, InvertedResidualBlock
+from .base_layers import ConvLayer, InvertedResidualBlock
 from .mobile_vit_v1_block import MobileViT_v1_Block
 
 
 def MobileViT_v1(
     configs,
+    dropout: float = 0.1,
     linear_drop: float = 0.0,
-    attention_drop: float = 0.2,
+    attention_drop: float = 0.0,
     num_classes: int = 1000,
     input_shape: tuple[int, int, int] = (256, 256, 3),
     model_name: str = f"MobileViT_v1-S",
 ):
     """
     Arguments
     --------
@@ -46,70 +42,62 @@
     out = ConvLayer(
         num_filters=configs.block_1_1_dims,
         kernel_size=3,
         strides=2,
         name="block-1-Conv",
     )(input_layer)
 
-    out_1_2 = InvertedResidualBlock(
+    out = InvertedResidualBlock(
         in_channels=configs.block_1_1_dims,
         out_channels=configs.block_1_2_dims,
         depthwise_stride=1,
         expansion_factor=configs.depthwise_expansion_factor,
         name="block-1-IR2",
     )(out)
 
-    if kops.shape(out)[-1] == kops.shape(out_1_2)[-1]:
-        out = out + out_1_2
-    else:
-        out = out_1_2
-
     # Block 2
     out = InvertedResidualBlock(
         in_channels=configs.block_1_2_dims,
         out_channels=configs.block_2_1_dims,
         depthwise_stride=2,
         expansion_factor=configs.depthwise_expansion_factor,
         name="block-2-IR1",
     )(out)
 
-    out_b2_2 = InvertedResidualBlock(
+    out = InvertedResidualBlock(
         in_channels=configs.block_2_1_dims,
         out_channels=configs.block_2_2_dims,
         depthwise_stride=1,
         expansion_factor=configs.depthwise_expansion_factor,
         name="block-2-IR2",
     )(out)
 
-    out = out + out_b2_2
-
-    out_b2_3 = InvertedResidualBlock(
+    out = InvertedResidualBlock(
         in_channels=configs.block_2_2_dims,
         out_channels=configs.block_2_3_dims,
         depthwise_stride=1,
         expansion_factor=configs.depthwise_expansion_factor,
         name="block-2-IR3",
     )(out)
 
-    out = out + out_b2_3
-
     # Block 3
     out = InvertedResidualBlock(
         in_channels=configs.block_2_2_dims,
         out_channels=configs.block_3_1_dims,
         depthwise_stride=2,
         expansion_factor=configs.depthwise_expansion_factor,
         name="block-3-IR1",
     )(out)
 
     out = MobileViT_v1_Block(
         out_filters=configs.block_3_2_dims,
         embedding_dim=configs.tf_block_3_dims,
         transformer_repeats=configs.tf_block_3_repeats,
         name="MobileViTBlock-1",
+        dropout=dropout,
         attention_drop=attention_drop,
         linear_drop=linear_drop,
     )(out)
 
     # Block 4
     out = InvertedResidualBlock(
         in_channels=configs.block_3_2_dims,
@@ -120,14 +108,15 @@
     )(out)
 
     out = MobileViT_v1_Block(
         out_filters=configs.block_4_2_dims,
         embedding_dim=configs.tf_block_4_dims,
         transformer_repeats=configs.tf_block_4_repeats,
         name="MobileViTBlock-2",
+        dropout=dropout,
         attention_drop=attention_drop,
         linear_drop=linear_drop,
     )(out)
 
     # Block 5
     out = InvertedResidualBlock(
         in_channels=configs.block_4_2_dims,
@@ -138,57 +127,54 @@
     )(out)
 
     out = MobileViT_v1_Block(
         out_filters=configs.block_5_2_dims,
         embedding_dim=configs.tf_block_5_dims,
         transformer_repeats=configs.tf_block_5_repeats,
         name="MobileViTBlock-3",
+        dropout=dropout,
         attention_drop=attention_drop,
         linear_drop=linear_drop,
     )(out)
 
     out = ConvLayer(num_filters=configs.final_conv_dims, kernel_size=1, strides=1)(out)
 
     # Output layer
     out = GlobalAveragePooling2D()(out)
 
     if linear_drop > 0.0:
-        out = Dropout(rate=linear_drop)(out)
+        out = Dropout(rate=dropout)(out)
 
     out = Dense(units=num_classes)(out)
 
     model = Model(inputs=input_layer, outputs=out, name=model_name)
 
     return model
 
 
 def build_MobileViT_v1(
-    model_type: str = "XXs",
+    model_type: str = "S",
     num_classes: int = 1000,
     input_shape: tuple = (256, 256, 3),
     updates: Optional[dict] = None,
     **kwargs,
 ):
     """
     Create MobileViT-v1 Classification models
 
     Arguments
     --------
         model_type: (str)   MobileViT version to create. Options: S, XS, XSS
-
         num_classes: (int)   Number of output classes
-
         input_shape: (tuple) Input shape -> H, W, C
         updates: (dict) a key-value pair indicating the changes to be made to the base model.
 
     Additional arguments:
     ---------------------
-
         linear_drop: (float) Dropout rate for Dense layers
-
         attention_drop: (float) Dropout rate for the attention matrix
 
     """
     model_type = model_type.upper()
 
     if model_type not in ("S", "XS", "XXS"):
         raise ValueError("Bad Input. 'model_type' should one of ['S', 'XS', 'XXS']")
@@ -198,45 +184,42 @@
     model = MobileViT_v1(
         configs=updated_configs,
         num_classes=num_classes,
         input_shape=input_shape,
         model_name=f"MobileViT_v1-{model_type}",
         **kwargs,
     )
-
-    # Print model summary
-    model.summary()
+    # model.summary()
 
     return model
 
 
 if __name__ == "__main__":
     model = build_MobileViT_v1(
         model_type="S",  # "XS", "XXS"
         input_shape=(256, 256, 3),  # (None, None, 3)
         num_classes=1000,
         linear_drop=0.0,
         attention_drop=0.0,
     )
 
-    # _ = model(kops.random.uniform((1, 256, 256, 3)), training=False)
+    print(f"{model.name} num. parametes: {model.count_params()}")
     # model.summary(positions=[0.33, 0.64, 0.75, 1.0])
     # model.save(f"{model.name}", include_optimizer=False)
-    print(f"{model.name} num. parametes: {model.count_params()}")
 
-    # Refer to BaseConfigs class to see all customizable modules available.
-    updates = {
-        "block_3_1_dims": 256,
-        "block_3_2_dims": 384,
-        "tf_block_3_dims": 164,
-        "tf_block_3_repeats": 3,
-    }
+    # # Refer to BaseConfigs class to see all customizable modules available.
+    # updates = {
+    #     "block_3_1_dims": 256,
+    #     "block_3_2_dims": 384,
+    #     "tf_block_3_dims": 164,
+    #     "tf_block_3_repeats": 3,
+    # }
+
+    # model = build_MobileViT_v1(
+    #     model_type="XXS",
+    #     updates=updates,
+    #     linear_drop=0.0,
+    #     attention_drop=0.0,
+    # )
 
-    model = build_MobileViT_v1(
-        model_type="XXS",
-        updates=updates,
-        linear_drop=0.0,
-        attention_drop=0.0,
-    )
-
-    # model.summary(positions=[0.33, 0.64, 0.75, 1.0])
-    print(f"{model.name} num. parametes: {model.count_params()}")
+    # # model.summary(positions=[0.33, 0.64, 0.75, 1.0])
+    # print(f"{model.name} num. parametes: {model.count_params()}")
```

### Comparing `keras-vision-0.3/keras_vision/MobileViT_v1/utils.py` & `keras-vision-0.4/keras_vision/MobileViT_v1/utils.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.3/keras_vision.egg-info/PKG-INFO` & `keras-vision-0.4/keras_vision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-vision
-Version: 0.3
+Version: 0.4
 Summary: Building Vision models in Keras3 for framework agnostic training and inference.
 Home-page: https://github.com/veb-101/keras-vision
 Author: Vaibhav Singh
 Author-email: vaibhav.singh.3001@gmail.com
 License: Apache 2.0
 Keywords: keras3 tensorflow Jax PyTorch Vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `keras-vision-0.3/keras_vision.egg-info/SOURCES.txt` & `keras-vision-0.4/keras_vision.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 setup.py
 keras_vision/__init__.py
 keras_vision.egg-info/PKG-INFO
 keras_vision.egg-info/SOURCES.txt
 keras_vision.egg-info/dependency_links.txt
 keras_vision.egg-info/requires.txt
 keras_vision.egg-info/top_level.txt
-keras_vision/MobileViT_v1/BaseLayers.py
 keras_vision/MobileViT_v1/__init__.py
+keras_vision/MobileViT_v1/base_layers.py
 keras_vision/MobileViT_v1/configs.py
-keras_vision/MobileViT_v1/minimal_example.py
 keras_vision/MobileViT_v1/mobile_vit_v1.py
 keras_vision/MobileViT_v1/mobile_vit_v1_block.py
 keras_vision/MobileViT_v1/multihead_self_attention_2D.py
 keras_vision/MobileViT_v1/utils.py
```

### Comparing `keras-vision-0.3/setup.py` & `keras-vision-0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
-__version__ = "0.3"
+__version__ = "0.4"
 DESCRIPTION = "Building Vision models in Keras3 for framework agnostic training and inference."
 
 # Setting up
 setup(
     name="keras-vision",
     version=__version__,
     author="Vaibhav Singh",
```


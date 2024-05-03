# Comparing `tmp/mlx_vlm-0.0.3.tar.gz` & `tmp/mlx_vlm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_vlm-0.0.3.tar", last modified: Tue Apr 23 14:10:54 2024, max compression
+gzip compressed data, was "mlx_vlm-0.0.4.tar", last modified: Fri May  3 20:54:34 2024, max compression
```

## Comparing `mlx_vlm-0.0.3.tar` & `mlx_vlm-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.566111 mlx_vlm-0.0.3/mlx_vlm/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/mlx_vlm/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/mlx_vlm/models/llava/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/llava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/llava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/llava/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/llava/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/nanoLlava.py
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/sample_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10109 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/tokenizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/mlx_vlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 14:10:54.000000 mlx_vlm-0.0.3/mlx_vlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 14:10:54.000000 mlx_vlm-0.0.3/mlx_vlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:10:54.000000 mlx_vlm-0.0.3/mlx_vlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 14:10:54.000000 mlx_vlm-0.0.3/mlx_vlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 14:10:54.000000 mlx_vlm-0.0.3/mlx_vlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.427915 mlx_vlm-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-03 20:54:34.427915 mlx_vlm-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.423915 mlx_vlm-0.0.4/mlx_vlm/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.423915 mlx_vlm-0.0.4/mlx_vlm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.423915 mlx_vlm-0.0.4/mlx_vlm/models/idefics2/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/idefics2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/idefics2/idefics2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/idefics2/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/idefics2/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.423915 mlx_vlm-0.0.4/mlx_vlm/models/llava/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/llava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/llava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/llava/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/llava/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.423915 mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/nanoLlava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/prompt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/sample_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.427915 mlx_vlm-0.0.4/mlx_vlm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/tokenizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25427 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/mlx_vlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:34.427915 mlx_vlm-0.0.4/mlx_vlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-03 20:54:34.000000 mlx_vlm-0.0.4/mlx_vlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-03 20:54:34.000000 mlx_vlm-0.0.4/mlx_vlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:54:34.000000 mlx_vlm-0.0.4/mlx_vlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 20:54:34.000000 mlx_vlm-0.0.4/mlx_vlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 20:54:34.000000 mlx_vlm-0.0.4/mlx_vlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:54:34.427915 mlx_vlm-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 20:54:29.000000 mlx_vlm-0.0.4/setup.py
```

### Comparing `mlx_vlm-0.0.3/LICENSE` & `mlx_vlm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.3/PKG-INFO` & `mlx_vlm-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-vlm
-Version: 0.0.3
+Version: 0.0.4
 Summary: Vision LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/Blaizzy/mlx-vlm
 Author: Prince Canuma
 Author-email: prince.gdt@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm/convert.py` & `mlx_vlm-0.0.4/mlx_vlm/convert.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,8 +55,8 @@
 def main():
     parser = configure_parser()
     args = parser.parse_args()
     convert(**vars(args))
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm/generate.py` & `mlx_vlm-0.0.4/mlx_vlm/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import argparse
 import codecs
 
 import mlx.core as mx
-from .utils import load, load_config, load_image_processor, generate, get_model_path
 
+from .prompt_utils import get_message_json
+from .utils import generate, get_model_path, load, load_config, load_image_processor
 
 MODEL_TYPE = ""
+
+
 def parse_arguments():
     parser = argparse.ArgumentParser(
         description="Generate text from an image using a model."
     )
     parser.add_argument(
         "--model",
         type=str,
@@ -33,61 +36,72 @@
         type=int,
         default=100,
         help="Maximum number of tokens to generate.",
     )
     parser.add_argument(
         "--temp", type=float, default=0.3, help="Temperature for sampling."
     )
+    parser.add_argument(
+        "--verbose",
+        type=bool,
+        help="Detailed output.",
+        default=True,
+    )
     return parser.parse_args()
 
 
 def get_model_and_processors(model_path):
     model_path = get_model_path(model_path)
-    model, processor = load(model_path, {"trust_remote_code": True})
     config = load_config(model_path)
-    image_processor = load_image_processor(config)
-    return model, processor, image_processor
+    model, processor = load(model_path, {"trust_remote_code": True})
+    image_processor = load_image_processor(model_path)
+    return model, processor, image_processor, config
 
 
 def sample(logits, temperature=0.0):
     if temperature == 0:
         return mx.argmax(logits, axis=-1)
     else:
         return mx.random.categorical(logits * (1 / temperature))
 
 
-
 def main():
     args = parse_arguments()
-    model, processor, image_processor = get_model_and_processors(args.model)
+    model, processor, image_processor, config = get_model_and_processors(args.model)
 
     prompt = codecs.decode(args.prompt, "unicode_escape")
 
     if "chat_template" in processor.__dict__.keys():
         prompt = processor.apply_chat_template(
-            [{"role": "user", "content": f"<image>\n{prompt}"}],
+            [get_message_json(config["model_type"], prompt)],
             tokenize=False,
             add_generation_prompt=True,
         )
+
     elif "tokenizer" in processor.__dict__.keys():
         prompt = processor.tokenizer.apply_chat_template(
-            [{"role": "user", "content": f"<image>\n{prompt}"}],
+            [get_message_json(config["model_type"], prompt)],
             tokenize=False,
             add_generation_prompt=True,
         )
+
     else:
-        ValueError("Error: processor does not have 'chat_template' or 'tokenizer' attribute.")
+        ValueError(
+            "Error: processor does not have 'chat_template' or 'tokenizer' attribute."
+        )
 
-    generate(
+    output = generate(
         model,
         processor,
         args.image,
         prompt,
         image_processor,
         args.temp,
         args.max_tokens,
-        True
+        args.verbose,
     )
+    if not args.verbose:
+        print(output)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm/models/base.py` & `mlx_vlm-0.0.4/mlx_vlm/models/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-
 from abc import ABC, abstractmethod
 from typing import Dict
 
 from transformers.image_processing_utils import get_size_dict
-from transformers.image_utils import (ChannelDimension, PILImageResampling )
+from transformers.image_utils import ChannelDimension, PILImageResampling
 
 
 class BaseImageProcessor(ABC):
-    def __init__(self,
-                 image_mean=(0.5, 0.5, 0.5),
-                 image_std=(0.5, 0.5, 0.5),
-                 size=(384, 384),
-                 crop_size: Dict[str, int] = None,
-                 resample=PILImageResampling.BICUBIC,
-                 rescale_factor=1 / 255,
-                 data_format=ChannelDimension.FIRST):
-        crop_size = crop_size if crop_size is not None else {"height": 384, "width": 384}
-        crop_size = get_size_dict(crop_size, default_to_square=True, param_name="crop_size")
+    def __init__(
+        self,
+        image_mean=(0.5, 0.5, 0.5),
+        image_std=(0.5, 0.5, 0.5),
+        size=(384, 384),
+        crop_size: Dict[str, int] = None,
+        resample=PILImageResampling.BICUBIC,
+        rescale_factor=1 / 255,
+        data_format=ChannelDimension.FIRST,
+    ):
+        crop_size = (
+            crop_size if crop_size is not None else {"height": 384, "width": 384}
+        )
+        crop_size = get_size_dict(
+            crop_size, default_to_square=True, param_name="crop_size"
+        )
 
         self.image_mean = image_mean
         self.image_std = image_std
         self.size = size
         self.resample = resample
         self.rescale_factor = rescale_factor
         self.data_format = data_format
         self.crop_size = crop_size
 
     @abstractmethod
     def preprocess(self, images):
         pass
-
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm/models/llava/language.py` & `mlx_vlm-0.0.4/mlx_vlm/models/llava/language.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import inspect
 from dataclasses import dataclass
 from typing import Dict, Optional, Tuple, Union
 
 import mlx.core as mx
 import mlx.nn as nn
 
@@ -205,7 +204,11 @@
 
     @staticmethod
     def sanitize(weights):
         # Remove unused precomputed rotary freqs
         return {
             k: v for k, v in weights.items() if "self_attn.rotary_emb.inv_freq" not in k
         }
+
+    @property
+    def layers(self):
+        return self.model.layers
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm/models/llava/llava.py` & `mlx_vlm-0.0.4/mlx_vlm/models/llava/llava.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-
-
 import glob
 import inspect
 import json
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
 
 import mlx.core as mx
 import mlx.nn as nn
 import numpy as np
 from huggingface_hub import snapshot_download
+
 from .language import LanguageModel, TextConfig
 from .vision import VisionConfig, VisionModel
 
 
 @dataclass
 class ModelConfig:
     text_config: TextConfig
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm/models/llava/vision.py` & `mlx_vlm-0.0.4/mlx_vlm/models/llava/vision.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 import inspect
 import math
 from dataclasses import dataclass
 from typing import Optional
 
 import mlx.core as mx
 import mlx.nn as nn
@@ -29,14 +27,15 @@
             **{
                 k: v
                 for k, v in params.items()
                 if k in inspect.signature(cls).parameters
             }
         )
 
+
 def check_array_shape(arr):
     shape = arr.shape
 
     # Check if the shape has 4 dimensions
     if len(shape) != 4:
         return False
 
@@ -44,14 +43,15 @@
 
     # Check if out_channels is the largest, and kH and KW are the same
     if (out_channels >= kH) and (out_channels >= KW) and (kH == KW):
         return True
     else:
         return False
 
+
 class Attention(nn.Module):
     def __init__(
         self,
         dims: int,
         num_heads: int,
         query_input_dims: Optional[int] = None,
         key_input_dims: Optional[int] = None,
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/language.py` & `mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from dataclasses import dataclass
 from typing import Dict, Optional, Tuple, Union
 
 import mlx.core as mx
 import mlx.nn as nn
 
 
-
 @dataclass
 class TextConfig:
     model_type: str
     hidden_size: int
     num_hidden_layers: int
     intermediate_size: int
     num_attention_heads: int
@@ -158,33 +157,31 @@
 
     def __call__(
         self,
         inputs: mx.array,
         cache=None,
         inputs_embeds=None,
     ):
-       # for passing merged input embeddings
+        # for passing merged input embeddings
         if inputs_embeds is None:
             h = self.embed_tokens(inputs)
         else:
             h = inputs_embeds
 
-
         mask = None
         if h.shape[1] > 1:
             mask = nn.MultiHeadAttention.create_additive_causal_mask(h.shape[1])
             mask = mask.astype(h.dtype)
 
         if cache is None:
             cache = [None] * len(self.layers)
 
         for e, layer in enumerate(self.layers):
             h, cache[e] = layer(h, mask, cache[e])
 
-
         return self.lm_head(self.norm(h)), cache
 
 
 class LanguageModel(nn.Module):
     def __init__(self, args: TextConfig):
         super().__init__()
         self.args = args
@@ -197,16 +194,21 @@
         cache=None,
         inputs_embeds=None,
     ):
         out, cache = self.model(inputs, cache, inputs_embeds=inputs_embeds)
         return out, cache
 
     def sanitize(self, weights):
-        if self.args.tie_word_embeddings and "language_model.model.lm_head.weight" not in weights:
-            weights["language_model.model.lm_head.weight"] = weights["language_model.model.embed_tokens.weight"]
+        if (
+            self.args.tie_word_embeddings
+            and "language_model.model.lm_head.weight" not in weights
+        ):
+            weights["language_model.model.lm_head.weight"] = weights[
+                "language_model.model.embed_tokens.weight"
+            ]
 
         return {
             k: v for k, v in weights.items() if "self_attn.rotary_emb.inv_freq" not in k
         }
 
     @property
     def layers(self):
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/nanoLlava.py` & `mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/nanoLlava.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-
-import re
 import glob
 import inspect
 import json
+import re
 from dataclasses import dataclass
+from functools import partial, reduce
 from pathlib import Path
-from typing import Optional
+from typing import Dict, Optional
 
 import mlx.core as mx
 import mlx.nn as nn
 import numpy as np
 from huggingface_hub import snapshot_download
+from PIL import Image
 from transformers import AutoConfig
+from transformers.image_transforms import (
+    convert_to_rgb,
+    normalize,
+    rescale,
+    resize,
+    to_channel_dimension_format,
+)
+from transformers.image_utils import to_numpy_array
+
+from ..base import BaseImageProcessor
 from .language import LanguageModel, TextConfig
 from .vision import VisionConfig, VisionModel
-from ..base import BaseImageProcessor
-
 
-from typing import Optional, Dict
-from dataclasses import dataclass
-from functools import partial, reduce
-from PIL import Image
-from transformers.image_transforms import (convert_to_rgb, normalize, rescale, resize, to_channel_dimension_format, )
-from transformers.image_utils import ( to_numpy_array, )
 
 @dataclass
 class ModelConfig:
     text_config: TextConfig
     vision_config: VisionConfig
     model_type: str
     auto_map: dict
     hidden_size: int
     mm_hidden_size: int
-    mm_hidden_size: int
     mm_vision_tower: str
     mm_projector_type: str = "mlp2x_gelu"
     ignore_index: int = -100
     image_token_index: int = -200
     vocab_size: int = 151936
 
-
     @classmethod
     def from_dict(cls, params):
         return cls(
             **{
                 k: v
                 for k, v in params.items()
                 if k in inspect.signature(cls).parameters
@@ -57,24 +58,39 @@
             images = [images]
         else:
             assert isinstance(images, list)
 
         transforms = [
             convert_to_rgb,
             to_numpy_array,
-            partial(resize, size=self.size, resample=self.resample, data_format=self.data_format),
+            partial(
+                resize,
+                size=self.size,
+                resample=self.resample,
+                data_format=self.data_format,
+            ),
             partial(rescale, scale=self.rescale_factor, data_format=self.data_format),
-            partial(normalize, mean=self.image_mean, std=self.image_std, data_format=self.data_format),
-            partial(to_channel_dimension_format, channel_dim=self.data_format, input_channel_dim=self.data_format),
+            partial(
+                normalize,
+                mean=self.image_mean,
+                std=self.image_std,
+                data_format=self.data_format,
+            ),
+            partial(
+                to_channel_dimension_format,
+                channel_dim=self.data_format,
+                input_channel_dim=self.data_format,
+            ),
         ]
 
         images = reduce(lambda x, f: [*map(f, x)], transforms, images)
 
         return images
 
+
 class LlavaMultiModalProjector(nn.Module):
     def __init__(self, config: ModelConfig):
         super().__init__()
         self.linear_1 = nn.Linear(
             config.vision_config.hidden_size, config.text_config.hidden_size, bias=True
         )
         self.gelu = nn.GELU()
@@ -84,24 +100,26 @@
 
     def __call__(self, x: mx.array) -> mx.array:
         x = self.linear_1(x)
         x = self.gelu(x)
         x = self.linear_2(x)
         return x
 
+
 class SigLipVisionTower(nn.Module):
     def __init__(self, config: VisionConfig):
         super().__init__()
         self.vision_tower = VisionModel(config)
 
     def __call__(
         self, x: mx.array, output_hidden_states: Optional[bool] = None
     ) -> mx.array:
         return self.vision_tower(x, output_hidden_states)
 
+
 class Model(nn.Module):
     def __init__(self, config: ModelConfig):
         self.model_type = config.model_type
         self.config = config
 
         self.vision_tower = SigLipVisionTower(config.vision_config)
         self.language_model = LanguageModel(config.text_config)
@@ -127,17 +145,15 @@
         image_features = self.mm_projector(image_features)
 
         final_inputs_embeds = self._prepare_inputs_for_multimodal(
             image_features, inputs_embeds, input_ids
         )
         return final_inputs_embeds
 
-    def _prepare_inputs_for_multimodal(
-        self, image_features, inputs_embeds, input_ids
-    ):
+    def _prepare_inputs_for_multimodal(self, image_features, inputs_embeds, input_ids):
         image_token_index = self.config.image_token_index
         num_images, num_image_patches, embed_dim = image_features.shape
 
         # Positions of <image> tokens in input_ids, assuming batch size is 1
         image_positions = np.where(input_ids[0] == image_token_index)[0].tolist()
 
         if len(image_positions) != num_images:
@@ -157,20 +173,15 @@
         final_embeddings = [v for p in zip(text_segments, image_embeddings) for v in p]
         final_embeddings += [inputs_embeds[:, start_idx:]]
 
         # Create a final embedding of shape
         # (1, num_image_patches*num_images + sequence_len, embed_dim)
         return mx.concatenate(final_embeddings, axis=1)
 
-    def __call__(
-        self,
-        input_ids: mx.array,
-        pixel_values: mx.array,
-        cache=None
-    ):
+    def __call__(self, input_ids: mx.array, pixel_values: mx.array, cache=None):
         input_embeddings = self.get_input_embeddings(input_ids, pixel_values)
         logits, cache = self.language_model(
             inputs=input_ids, cache=cache, inputs_embeds=input_embeddings
         )
         return logits, cache
 
     @staticmethod
@@ -183,15 +194,14 @@
                     allow_patterns=[
                         "*.json",
                         "*.safetensors",
                         "*.py",
                         "tokenizer.model",
                         "*.tiktoken",
                     ],
-
                 )
             )
 
         with open(path / "config.json", "r") as f:
             config = json.load(f)
 
         siglip_config = AutoConfig.from_pretrained(config["mm_vision_tower"])
@@ -217,25 +227,53 @@
         weights = model.sanitize(weights=weights)
 
         weights = VisionModel(model_config.vision_config).sanitize(weights=weights)
         weights = LanguageModel(model_config.text_config).sanitize(weights=weights)
         model.load_weights(list(weights.items()))
         return model
 
-
     def sanitize(self, weights):
         weights = {
-            f"{k.split('.', 1)[1]}" if re.match(r'^model\.vision_tower', k) else
-            f"mm_projector.linear_1.{k.split('.')[-1]}" if re.match(r'^model\.mm_projector\.0', k) else
-            f"mm_projector.linear_2.{k.split('.')[-1]}" if re.match(r'^model\.mm_projector\.2', k) else
-            f"language_model.model.{k}" if re.match(r'^lm_head', k) else
-            f"language_model.{k}" if re.match(r'^model\.(embed_tokens|norm|layers)', k) else k: v
+            (
+                f"{k.split('.', 1)[1]}"
+                if re.match(r"^model\.vision_tower", k)
+                else (
+                    f"mm_projector.linear_1.{k.split('.')[-1]}"
+                    if re.match(r"^model\.mm_projector\.0", k)
+                    else (
+                        f"mm_projector.linear_2.{k.split('.')[-1]}"
+                        if re.match(r"^model\.mm_projector\.2", k)
+                        else (
+                            f"language_model.model.{k}"
+                            if re.match(r"^lm_head", k)
+                            else (
+                                f"language_model.{k}"
+                                if re.match(r"^model\.(embed_tokens|norm|layers)", k)
+                                else k
+                            )
+                        )
+                    )
+                )
+            ): v
             for k, v in weights.items()
         }
 
         weights = {
-            f"vision_tower.vision_tower.vision_model.head.attention.in_proj.bias" if re.match(r'^vision_tower\.vision_tower\.vision_model\.head\.attention\.in_proj_bias', k) else
-            f"vision_tower.vision_tower.vision_model.head.attention.in_proj.weight" if re.match(r'^vision_tower\.vision_tower\.vision_model\.head\.attention\.in_proj_weight', k) else k: v
+            (
+                f"vision_tower.vision_tower.vision_model.head.attention.in_proj.bias"
+                if re.match(
+                    r"^vision_tower\.vision_tower\.vision_model\.head\.attention\.in_proj_bias",
+                    k,
+                )
+                else (
+                    f"vision_tower.vision_tower.vision_model.head.attention.in_proj.weight"
+                    if re.match(
+                        r"^vision_tower\.vision_tower\.vision_model\.head\.attention\.in_proj_weight",
+                        k,
+                    )
+                    else k
+                )
+            ): v
             for k, v in weights.items()
         }
 
-        return weights
+        return weights
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/vision.py` & `mlx_vlm-0.0.4/mlx_vlm/models/nanoLlava/vision.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 import inspect
 from dataclasses import dataclass
 from typing import Optional
 
 import mlx.core as mx
 import mlx.nn as nn
 
@@ -28,14 +26,15 @@
             **{
                 k: v
                 for k, v in params.items()
                 if k in inspect.signature(cls).parameters
             }
         )
 
+
 def check_array_shape(arr):
     shape = arr.shape
 
     # Check if the shape has 4 dimensions
     if len(shape) != 4:
         return False
 
@@ -43,14 +42,15 @@
 
     # Check if out_channels is the largest, and kH and KW are the same
     if (out_channels >= kH) and (out_channels >= KW) and (kH == KW):
         return True
     else:
         return False
 
+
 class Attention(nn.Module):
     def __init__(
         self,
         dims: int,
         num_heads: int,
         query_input_dims: Optional[int] = None,
         key_input_dims: Optional[int] = None,
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm/sample_utils.py` & `mlx_vlm-0.0.4/mlx_vlm/sample_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.3/mlx_vlm/tokenizer_utils.py` & `mlx_vlm-0.0.4/mlx_vlm/tokenizer_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -325,8 +325,8 @@
 
     if return_tokenizer:
         return TokenizerWrapper(
             AutoTokenizer.from_pretrained(model_path, **tokenizer_config_extra),
             detokenizer_class,
         )
     else:
-        return detokenizer_class
+        return detokenizer_class
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm/utils.py` & `mlx_vlm-0.0.4/mlx_vlm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,51 @@
-
 import copy
-import re
 import glob
 import importlib
 import json
 import logging
+import re
 import shutil
 import time
 from pathlib import Path
 from textwrap import dedent
 from typing import Any, Callable, Dict, Generator, Optional, Tuple, Union
-import requests
 
 import mlx.core as mx
 import mlx.nn as nn
 import numpy as np
-from PIL import Image
+import requests
 from huggingface_hub import snapshot_download
 from mlx.utils import tree_flatten, tree_unflatten
-from transformers import AutoConfig, AutoProcessor, PreTrainedTokenizer, PreTrainedTokenizerFast
+from PIL import Image
+from transformers import (
+    AutoConfig,
+    AutoProcessor,
+    PreTrainedTokenizer,
+    PreTrainedTokenizerFast,
+)
 
-from .tokenizer_utils import TokenizerWrapper, load_tokenizer
 from .models.base import BaseImageProcessor
 from .sample_utils import top_p_sampling
+from .tokenizer_utils import TokenizerWrapper, load_tokenizer
 
 # Constants
 MODEL_REMAPPING = {
     "llava-qwen2": "nanoLlava",
 }
 
 MAX_FILE_SIZE_GB = 5
 
 linear_class_predicate = (
     lambda m: isinstance(m, nn.Linear)
     and m.weight.shape[0]
     != 8  # avoid quantizing gate layers, otherwise we have to re-quant and upload all the mixtral models
 )
 
+
 def get_model_and_args(config: dict):
     """
     Retrieve the model object based on the configuration.
 
     Args:
         config (dict): The model configuration.
 
@@ -52,15 +57,14 @@
     try:
         arch = importlib.import_module(f"mlx_vlm.models.{model_type}")
     except ImportError:
         msg = f"Model type {model_type} not supported."
         logging.error(msg)
         raise ValueError(msg)
 
-
     return arch, model_type
 
 
 def get_model_path(path_or_hf_repo: str, revision: Optional[str] = None) -> Path:
     """
     Ensures the model is available locally. If the path does not exist locally,
     it is downloaded from the Hugging Face Hub.
@@ -106,49 +110,62 @@
         nn.Module: The loaded and initialized model.
 
     Raises:
         FileNotFoundError: If the weight files (.safetensors) are not found.
         ValueError: If the model class or args class are not found or cannot be instantiated.
     """
 
-
     config = load_config(model_path)
     quantization = config.get("quantization", None)
 
-
     weight_files = glob.glob(str(model_path / "*.safetensors"))
     if not weight_files:
         logging.error(f"No safetensors found in {model_path}")
         raise FileNotFoundError(f"No safetensors found in {model_path}")
 
     weights = {}
     for wf in weight_files:
         weights.update(mx.load(wf))
 
-
     model_class, model_type = get_model_and_args(config=config)
 
     if model_type == "nanoLlava":
         vision_config = AutoConfig.from_pretrained(config["mm_vision_tower"])
         text_config = AutoConfig.from_pretrained(config["language_model"])
         vision_config = vision_config.to_dict()
         text_config = text_config.to_dict()
         config["vision_config"] = vision_config["vision_config"]
         config["text_config"] = text_config
+    if model_type == "idefics2":
+        config = AutoConfig.from_pretrained(model_path).to_dict()
 
     model_config = model_class.ModelConfig.from_dict(config)
-    model_config.vision_config = model_class.VisionConfig.from_dict(config["vision_config"])
+    model_config.vision_config = model_class.VisionConfig.from_dict(
+        config["vision_config"]
+    )
     model_config.text_config = model_class.TextConfig.from_dict(config["text_config"])
+
+    if hasattr(model_config, "perceiver_config"):
+        model_config.perceiver_config = model_class.PerceiverConfig.from_dict(
+            config["perceiver_config"]
+        )
     model = model_class.Model(model_config)
 
     if hasattr(model, "sanitize"):
         weights = model.sanitize(weights)
 
-    weights = model_class.VisionModel(model_config.vision_config).sanitize(weights=weights)
-    weights = model_class.LanguageModel(model_config.text_config).sanitize(weights=weights)
+    if hasattr(model_class.VisionModel, "sanitize"):
+        weights = model_class.VisionModel(model_config.vision_config).sanitize(
+            weights=weights
+        )
+
+    if hasattr(model_class.LanguageModel, "sanitize"):
+        weights = model_class.LanguageModel(model_config.text_config).sanitize(
+            weights=weights
+        )
 
     if (quantization := config.get("quantization", None)) is not None:
         # Handle legacy models which may not have everything quantized
         class_predicate = (
             lambda p, m: isinstance(m, (nn.Linear, nn.Embedding))
             and f"{p}.scales" in weights
         )
@@ -193,41 +210,51 @@
     model_path = get_model_path(path_or_hf_repo)
 
     model = load_model(model_path, lazy)
     processor = load_processor(model_path, processor_config=processor_config)
 
     return model, processor
 
+
 def load_config(model_path: Path) -> dict:
     try:
         with open(model_path / "config.json", "r") as f:
             config = json.load(f)
     except FileNotFoundError:
         logging.error(f"Config file not found in {model_path}")
         raise
     return config
 
-def load_image_processor(config: dict) -> BaseImageProcessor:
+
+def load_image_processor(model_path: Union[str, Path]) -> BaseImageProcessor:
+    if isinstance(model_path, str):
+        model_path = get_model_path(model_path)
+
+    config = load_config(model_path)
     model_class, _ = get_model_and_args(config)
     image_processor = None
 
     if hasattr(model_class, "ImageProcessor"):
         image_processor = model_class.ImageProcessor()
 
     return image_processor
 
-def load_processor(model_path, processor_config={"trust_remote_code": True}) -> Union[PreTrainedTokenizer, PreTrainedTokenizerFast]:
+
+def load_processor(
+    model_path, processor_config={"trust_remote_code": True}
+) -> Union[PreTrainedTokenizer, PreTrainedTokenizerFast]:
     processor = AutoProcessor.from_pretrained(model_path, **processor_config)
     detokenizer_class = load_tokenizer(model_path, return_tokenizer=False)
     if "tokenizer" in processor.__dict__.keys():
         processor.detokenizer = detokenizer_class(processor.tokenizer)
     else:
         processor.detokenizer = detokenizer_class(processor)
     return processor
 
+
 def fetch_from_hub(
     model_path: Path, lazy: bool = False
 ) -> Tuple[nn.Module, dict, PreTrainedTokenizer]:
     model = load_model(model_path, lazy)
     config = load_config(model_path)
     processor = load_processor(model_path)
 
@@ -266,14 +293,15 @@
         path (str): Local path to the model.
         upload_repo (str): Name of the HF repo to upload to.
         hf_path (str): Path to the original Hugging Face model.
     """
     import os
 
     from huggingface_hub import HfApi, ModelCard, logging
+
     from . import __version__
 
     card = ModelCard.load(hf_path)
     card.data.tags = ["mlx"] if card.data.tags is None else card.data.tags + ["mlx"]
     card.text = dedent(
         f"""
         # {upload_repo}
@@ -299,14 +327,15 @@
     api.upload_folder(
         folder_path=path,
         repo_id=upload_repo,
         repo_type="model",
     )
     print(f"Upload successful, go to https://huggingface.co/{upload_repo} for details.")
 
+
 def get_model_path(path_or_hf_repo: str, revision: Optional[str] = None) -> Path:
     """
     Ensures the model is available locally. If the path does not exist locally,
     it is downloaded from the Hugging Face Hub.
 
     Args:
         path_or_hf_repo (str): The local path or Hugging Face repository ID of the model.
@@ -353,14 +382,15 @@
         selected_logits = logits[:, indices]
         selected_logits = mx.where(
             selected_logits < 0, selected_logits * penalty, selected_logits / penalty
         )
         logits[:, indices] = selected_logits
     return logits
 
+
 def save_weights(
     save_path: Union[str, Path],
     weights: Dict[str, Any],
     *,
     donate_weights: bool = False,
 ) -> None:
     """Save model weights into specified directory."""
@@ -404,16 +434,14 @@
     with open(save_path / "model.safetensors.index.json", "w") as f:
         json.dump(
             index_data,
             f,
             indent=4,
         )
 
-def class_predicate(path, m):
-    return isinstance(m, nn.Linear) and not isinstance(m, nn.Embedding)
 
 def quantize_model(
     model: nn.Module, config: dict, q_group_size: int, q_bits: int
 ) -> Tuple:
     """
     Applies quantization to the model weights.
 
@@ -423,14 +451,21 @@
         q_group_size (int): Group size for quantization.
         q_bits (int): Bits per weight for quantization.
 
     Returns:
         Tuple: Tuple containing quantized weights and config.
     """
     quantized_config = copy.deepcopy(config)
+    vision_intermediate_size = model.config.vision_config.intermediate_size
+    class_predicate = lambda path, m: isinstance(m, nn.Linear) and (
+        path.split(".")[0] not in ["vision_model", "vision_tower"]
+        if any(vision_intermediate_size % size != 0 for size in [64, 128])
+        else not isinstance(m, nn.Embedding)
+    )
+
     nn.quantize(model, q_group_size, q_bits, class_predicate=class_predicate)
     quantized_config["quantization"] = {"group_size": q_group_size, "bits": q_bits}
     quantized_weights = dict(tree_flatten(model.parameters()))
 
     return quantized_weights, quantized_config
 
 
@@ -452,14 +487,15 @@
     # sort the config for better readability
     config = dict(sorted(config.items()))
 
     # write the updated config to the config_path (if provided)
     with open(config_path, "w") as fid:
         json.dump(config, fid, indent=4)
 
+
 def dequantize_model(model: nn.Module) -> nn.Module:
     """
     Dequantize the quantized linear layers in the model.
 
     Args:
         model (nn.Module): The model with quantized linear layers.
 
@@ -484,14 +520,15 @@
             if bias:
                 linear.bias = module.bias
             de_quantize_layers.append((name, linear))
     if len(de_quantize_layers) > 0:
         model.update_modules(tree_unflatten(de_quantize_layers))
     return model
 
+
 def convert(
     hf_path: str,
     mlx_path: str = "mlx_model",
     quantize: bool = False,
     q_group_size: int = 64,
     q_bits: int = 4,
     dtype: str = "float16",
@@ -526,24 +563,22 @@
     del model
     save_weights(mlx_path, weights, donate_weights=True)
 
     py_files = glob.glob(str(model_path / "*.py"))
     for file in py_files:
         shutil.copy(file, mlx_path)
 
-
     tokenizer.save_pretrained(mlx_path)
 
-
     save_config(config, config_path=mlx_path / "config.json")
 
-
     if upload_repo is not None:
         upload_to_hub(mlx_path, upload_repo, hf_path)
 
+
 def load_image(image_source):
     """
     Helper function to load an image from either a URL or file.
     """
     if image_source.startswith(("http://", "https://")):
         try:
             response = requests.get(image_source, stream=True)
@@ -559,48 +594,52 @@
         except IOError as e:
             raise ValueError(f"Failed to load image {image_source} with error: {e}")
     else:
         raise ValueError(
             f"The image {image_source} must be a valid URL or existing file."
         )
 
+
 def prepare_inputs(image_processor, processor, image, prompt):
+    from transformers.image_utils import load_image
+
     if isinstance(image, str):
         image = load_image(image)
 
     if image_processor is not None:
         text_chunks = [processor(chunk).input_ids for chunk in prompt.split("<image>")]
         input_ids = mx.array([text_chunks[0] + [-200] + text_chunks[1]])
         pixel_values = image_processor.preprocess(images=[image])[0]
         pixel_values = mx.array(np.expand_dims(pixel_values, axis=0))
     else:
         inputs = processor(prompt, image, return_tensors="np")
         pixel_values = mx.array(inputs["pixel_values"])
         input_ids = mx.array(inputs["input_ids"])
-
     return input_ids, pixel_values
 
-def sample(logits: mx.array, temp:float, top_p:float) -> Tuple[mx.array, float]:
+
+def sample(logits: mx.array, temp: float, top_p: float) -> Tuple[mx.array, float]:
     softmax_logits = mx.softmax(logits)
 
     if temp == 0:
         token = mx.argmax(logits, axis=-1)
     else:
         if top_p > 0 and top_p < 1.0:
             token = top_p_sampling(logits, top_p, temp)
         else:
             token = mx.random.categorical(logits * (1 / temp))
 
     prob = softmax_logits[0, token]
     return token, prob
 
+
 def generate_step(
     model: nn.Module,
     prompt: mx.array,
-    cache = None,
+    cache=None,
     temp: float = 0.0,
     repetition_penalty: Optional[float] = None,
     repetition_context_size: Optional[int] = 20,
     top_p: float = 1.0,
 ) -> Generator[Tuple[mx.array, mx.array], None, None]:
     """
     A generator producing text based on the given prompt from the model.
@@ -652,15 +691,15 @@
 
 
 def generate(
     model: nn.Module,
     processor: PreTrainedTokenizer,
     image: str,
     prompt: str,
-    image_processor = None,
+    image_processor=None,
     temp: float = 0.0,
     max_tokens: int = 100,
     verbose: bool = False,
     formatter: Optional[Callable] = None,
     repetition_penalty: Optional[float] = None,
     repetition_context_size: Optional[int] = None,
     top_p: float = 1.0,
@@ -682,28 +721,26 @@
        repetition_context_size (int, optional): The number of tokens to consider for repetition penalty.
     """
     if verbose:
         print("=" * 10)
         print("Image:", image, "\n")
         print("Prompt:", prompt)
 
-
     if image_processor is not None:
         prompt_tokens = mx.array(processor.encode(prompt))
         tokenizer = processor
     else:
         prompt_tokens = mx.array(processor.tokenizer.encode(prompt))
         tokenizer = processor.tokenizer
 
     input_ids, pixel_values = prepare_inputs(image_processor, processor, image, prompt)
     logits, cache = model(input_ids, pixel_values)
     logits = logits[:, -1, :]
     y, _ = sample(logits, temp, top_p)
 
-
     tic = time.perf_counter()
     detokenizer = processor.detokenizer
     detokenizer.reset()
 
     detokenizer.add_token(y.item())
 
     for (token, prob), n in zip(
@@ -722,15 +759,14 @@
         if n == 0:
             prompt_time = time.perf_counter() - tic
             tic = time.perf_counter()
 
         if token == tokenizer.eos_token_id:
             break
 
-
         detokenizer.add_token(token)
 
         if verbose:
             if formatter:
                 # We have to finalize so that the prob corresponds to the last segment
                 detokenizer.finalize()
                 formatter(detokenizer.last_segment, prob.item())
@@ -749,8 +785,8 @@
             return
         prompt_tps = prompt_tokens.size / prompt_time
         gen_tps = (token_count - 1) / gen_time
 
         print(f"Prompt: {prompt_tps:.3f} tokens-per-sec")
         print(f"Generation: {gen_tps:.3f} tokens-per-sec")
 
-    return detokenizer.text
+    return detokenizer.text
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm.egg-info/PKG-INFO` & `mlx_vlm-0.0.4/mlx_vlm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-vlm
-Version: 0.0.3
+Version: 0.0.4
 Summary: Vision LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/Blaizzy/mlx-vlm
 Author: Prince Canuma
 Author-email: prince.gdt@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx_vlm-0.0.3/mlx_vlm.egg-info/SOURCES.txt` & `mlx_vlm-0.0.4/mlx_vlm.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,26 +2,32 @@
 MANIFEST.in
 README.md
 setup.py
 ./requirements.txt
 mlx_vlm/__init__.py
 mlx_vlm/convert.py
 mlx_vlm/generate.py
+mlx_vlm/prompt_utils.py
 mlx_vlm/sample_utils.py
 mlx_vlm/tokenizer_utils.py
 mlx_vlm/utils.py
 mlx_vlm/version.py
 mlx_vlm.egg-info/PKG-INFO
 mlx_vlm.egg-info/SOURCES.txt
 mlx_vlm.egg-info/dependency_links.txt
 mlx_vlm.egg-info/requires.txt
 mlx_vlm.egg-info/top_level.txt
 mlx_vlm/models/__init__.py
 mlx_vlm/models/base.py
+mlx_vlm/models/idefics2/__init__.py
+mlx_vlm/models/idefics2/idefics2.py
+mlx_vlm/models/idefics2/language.py
+mlx_vlm/models/idefics2/vision.py
 mlx_vlm/models/llava/__init__.py
 mlx_vlm/models/llava/language.py
 mlx_vlm/models/llava/llava.py
 mlx_vlm/models/llava/vision.py
 mlx_vlm/models/nanoLlava/__init__.py
 mlx_vlm/models/nanoLlava/language.py
 mlx_vlm/models/nanoLlava/nanoLlava.py
-mlx_vlm/models/nanoLlava/vision.py
+mlx_vlm/models/nanoLlava/vision.py
+mlx_vlm/tests/test_models.py
```

### Comparing `mlx_vlm-0.0.3/setup.py` & `mlx_vlm-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 from pathlib import Path
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 # Get the project root directory
 root_dir = Path(__file__).parent
 
 # Add the package directory to the Python path
 package_dir = root_dir / "mlx_vlm"
 sys.path.append(str(package_dir))
@@ -27,8 +28,8 @@
     author_email="prince.gdt@gmail.com",
     author="Prince Canuma",
     url="https://github.com/Blaizzy/mlx-vlm",
     license="MIT",
     install_requires=requirements,
     packages=find_packages(where=root_dir),
     python_requires=">=3.8",
-)
+)
```


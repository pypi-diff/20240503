# Comparing `tmp/onnx_embedding_models-0.0.8.tar.gz` & `tmp/onnx_embedding_models-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx_embedding_models-0.0.8.tar", last modified: Sun Mar  3 01:44:40 2024, max compression
+gzip compressed data, was "onnx_embedding_models-0.0.9.tar", last modified: Sun Mar  3 01:54:09 2024, max compression
```

## Comparing `onnx_embedding_models-0.0.8.tar` & `onnx_embedding_models-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-03-03 01:44:40.087548 onnx_embedding_models-0.0.8/
--rw-r--r--   0 benjamin   (501) staff       (20)     1066 2024-01-16 20:19:37.000000 onnx_embedding_models-0.0.8/LICENSE
--rw-r--r--   0 benjamin   (501) staff       (20)      446 2024-03-03 01:44:40.087319 onnx_embedding_models-0.0.8/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)       84 2024-01-16 20:19:37.000000 onnx_embedding_models-0.0.8/README.md
--rw-r--r--   0 benjamin   (501) staff       (20)      437 2024-03-03 01:44:26.000000 onnx_embedding_models-0.0.8/pyproject.toml
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2024-03-03 01:44:40.087597 onnx_embedding_models-0.0.8/setup.cfg
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-03-03 01:44:40.085085 onnx_embedding_models-0.0.8/src/
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-03-03 01:44:40.086163 onnx_embedding_models-0.0.8/src/onnx_embedding_models/
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2024-01-16 20:21:45.000000 onnx_embedding_models-0.0.8/src/onnx_embedding_models/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)     6933 2024-02-28 05:39:05.000000 onnx_embedding_models-0.0.8/src/onnx_embedding_models/model.py
--rw-r--r--   0 benjamin   (501) staff       (20)     1567 2024-02-11 19:26:44.000000 onnx_embedding_models-0.0.8/src/onnx_embedding_models/registry.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-03-03 01:44:40.087104 onnx_embedding_models-0.0.8/src/onnx_embedding_models.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)      446 2024-03-03 01:44:40.000000 onnx_embedding_models-0.0.8/src/onnx_embedding_models.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      387 2024-03-03 01:44:40.000000 onnx_embedding_models-0.0.8/src/onnx_embedding_models.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2024-03-03 01:44:40.000000 onnx_embedding_models-0.0.8/src/onnx_embedding_models.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       47 2024-03-03 01:44:40.000000 onnx_embedding_models-0.0.8/src/onnx_embedding_models.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       22 2024-03-03 01:44:40.000000 onnx_embedding_models-0.0.8/src/onnx_embedding_models.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-03-03 01:54:09.123527 onnx_embedding_models-0.0.9/
+-rw-r--r--   0 benjamin   (501) staff       (20)     1066 2024-01-16 20:19:37.000000 onnx_embedding_models-0.0.9/LICENSE
+-rw-r--r--   0 benjamin   (501) staff       (20)      466 2024-03-03 01:54:09.123324 onnx_embedding_models-0.0.9/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)       84 2024-01-16 20:19:37.000000 onnx_embedding_models-0.0.9/README.md
+-rw-r--r--   0 benjamin   (501) staff       (20)      449 2024-03-03 01:53:50.000000 onnx_embedding_models-0.0.9/pyproject.toml
+-rw-r--r--   0 benjamin   (501) staff       (20)       38 2024-03-03 01:54:09.123574 onnx_embedding_models-0.0.9/setup.cfg
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-03-03 01:54:09.121506 onnx_embedding_models-0.0.9/src/
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-03-03 01:54:09.122261 onnx_embedding_models-0.0.9/src/onnx_embedding_models/
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2024-01-16 20:21:45.000000 onnx_embedding_models-0.0.9/src/onnx_embedding_models/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     7068 2024-03-03 01:53:36.000000 onnx_embedding_models-0.0.9/src/onnx_embedding_models/model.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     1567 2024-02-11 19:26:44.000000 onnx_embedding_models-0.0.9/src/onnx_embedding_models/registry.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-03-03 01:54:09.123139 onnx_embedding_models-0.0.9/src/onnx_embedding_models.egg-info/
+-rw-r--r--   0 benjamin   (501) staff       (20)      466 2024-03-03 01:54:09.000000 onnx_embedding_models-0.0.9/src/onnx_embedding_models.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      387 2024-03-03 01:54:09.000000 onnx_embedding_models-0.0.9/src/onnx_embedding_models.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2024-03-03 01:54:09.000000 onnx_embedding_models-0.0.9/src/onnx_embedding_models.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       52 2024-03-03 01:54:09.000000 onnx_embedding_models-0.0.9/src/onnx_embedding_models.egg-info/requires.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       22 2024-03-03 01:54:09.000000 onnx_embedding_models-0.0.9/src/onnx_embedding_models.egg-info/top_level.txt
```

### Comparing `onnx_embedding_models-0.0.8/LICENSE` & `onnx_embedding_models-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx_embedding_models-0.0.8/src/onnx_embedding_models/model.py` & `onnx_embedding_models-0.0.9/src/onnx_embedding_models/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import tqdm
 import shutil
 import tempfile
 from typing import Literal, Optional
 
 import numpy as np
 
 from .registry import registry
@@ -158,39 +159,40 @@
             return emb
         return emb.tolist()
 
     def embed_batch(
         self,
         texts: list[str],
         return_numpy: bool = False,
+        show_progress: bool = True,
     ):
         inputs = self.tokenizer(
             texts,
             truncation=True,
             padding=False,
             max_length=self.max_length,
         ) # dont return tensors, this adds unnecessary padding
         output_embs = []
-        for i in range(len(texts)):
+        for i in tqdm.tqdm(range(len(texts)), disable=not show_progress):
             outputs = self.session.run(None, {k: np.array(v[i]).reshape(1, -1) for k, v in inputs.items()})
             if len(outputs) == 2:
                 hidden_states, pooler_output = outputs
             else:
                 hidden_states, pooler_output = outputs[0], None
 
             emb = self._pool(hidden_states, pooler_output).flatten()
             output_embs.append(emb.tolist())
 
         if return_numpy:
             return np.array(output_embs)
         
         return output_embs
     
-    def encode(self, texts: list[str], return_numpy=False):
-        return self.embed_batch(texts, return_numpy=return_numpy)
+    def encode(self, texts: list[str], return_numpy=False, show_progress=True):
+        return self.embed_batch(texts, return_numpy=return_numpy, show_progress=show_progress)
     
     def __call__(self, texts: list[str], return_numpy=False):
         if isinstance(texts, str):
             return self.embed(texts, return_numpy=return_numpy)
         elif isinstance(texts, list):
             return self.embed_batch(texts, return_numpy=return_numpy)
```

### Comparing `onnx_embedding_models-0.0.8/src/onnx_embedding_models/registry.py` & `onnx_embedding_models-0.0.9/src/onnx_embedding_models/registry.py`

 * *Files identical despite different names*


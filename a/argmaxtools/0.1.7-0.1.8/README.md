# Comparing `tmp/argmaxtools-0.1.7.tar.gz` & `tmp/argmaxtools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argmaxtools-0.1.7.tar", last modified: Sun Mar  3 07:12:53 2024, max compression
+gzip compressed data, was "argmaxtools-0.1.8.tar", last modified: Thu May  2 22:01:03 2024, max compression
```

## Comparing `argmaxtools-0.1.7.tar` & `argmaxtools-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ati        (501) staff       (20)        0 2024-03-03 07:12:53.377892 argmaxtools-0.1.7/
--rw-r--r--   0 ati        (501) staff       (20)      849 2024-03-03 07:12:53.377809 argmaxtools-0.1.7/PKG-INFO
--rw-r--r--   0 ati        (501) staff       (20)       45 2024-02-19 23:35:04.000000 argmaxtools-0.1.7/README.md
-drwxr-xr-x   0 ati        (501) staff       (20)        0 2024-03-03 07:12:53.376291 argmaxtools-0.1.7/argmaxtools/
--rw-r--r--   0 ati        (501) staff       (20)        0 2024-02-05 05:59:16.000000 argmaxtools-0.1.7/argmaxtools/__init__.py
--rw-r--r--   0 ati        (501) staff       (20)     7021 2024-02-19 23:35:04.000000 argmaxtools-0.1.7/argmaxtools/_sdpa.py
--rw-r--r--   0 ati        (501) staff       (20)       22 2024-03-03 07:08:54.000000 argmaxtools-0.1.7/argmaxtools/_version.py
-drwxr-xr-x   0 ati        (501) staff       (20)        0 2024-03-03 07:12:53.377358 argmaxtools-0.1.7/argmaxtools/compress/
--rw-r--r--   0 ati        (501) staff       (20)       87 2024-02-19 23:35:04.000000 argmaxtools-0.1.7/argmaxtools/compress/__init__.py
--rw-r--r--   0 ati        (501) staff       (20)    28832 2024-02-29 00:18:56.000000 argmaxtools-0.1.7/argmaxtools/compress/palettize.py
--rw-r--r--   0 ati        (501) staff       (20)     4072 2024-02-19 23:35:04.000000 argmaxtools-0.1.7/argmaxtools/compress/sparse_outlier.py
--rw-r--r--   0 ati        (501) staff       (20)      704 2024-02-05 05:59:16.000000 argmaxtools-0.1.7/argmaxtools/compress/utils.py
--rw-r--r--   0 ati        (501) staff       (20)    11114 2024-02-29 00:18:56.000000 argmaxtools-0.1.7/argmaxtools/nn.py
--rw-r--r--   0 ati        (501) staff       (20)     2724 2024-02-19 23:35:04.000000 argmaxtools-0.1.7/argmaxtools/tensor_typing.py
--rw-r--r--   0 ati        (501) staff       (20)    17878 2024-02-29 00:29:30.000000 argmaxtools-0.1.7/argmaxtools/test_utils.py
--rw-r--r--   0 ati        (501) staff       (20)     5635 2024-03-03 07:12:12.000000 argmaxtools-0.1.7/argmaxtools/utils.py
-drwxr-xr-x   0 ati        (501) staff       (20)        0 2024-03-03 07:12:53.376849 argmaxtools-0.1.7/argmaxtools.egg-info/
--rw-r--r--   0 ati        (501) staff       (20)      849 2024-03-03 07:12:53.000000 argmaxtools-0.1.7/argmaxtools.egg-info/PKG-INFO
--rw-r--r--   0 ati        (501) staff       (20)      525 2024-03-03 07:12:53.000000 argmaxtools-0.1.7/argmaxtools.egg-info/SOURCES.txt
--rw-r--r--   0 ati        (501) staff       (20)        1 2024-03-03 07:12:53.000000 argmaxtools-0.1.7/argmaxtools.egg-info/dependency_links.txt
--rw-r--r--   0 ati        (501) staff       (20)       65 2024-03-03 07:12:53.000000 argmaxtools-0.1.7/argmaxtools.egg-info/requires.txt
--rw-r--r--   0 ati        (501) staff       (20)       12 2024-03-03 07:12:53.000000 argmaxtools-0.1.7/argmaxtools.egg-info/top_level.txt
--rw-r--r--   0 ati        (501) staff       (20)       70 2024-03-03 07:12:53.378093 argmaxtools-0.1.7/setup.cfg
--rw-r--r--   0 ati        (501) staff       (20)     1053 2024-02-05 05:59:16.000000 argmaxtools-0.1.7/setup.py
-drwxr-xr-x   0 ati        (501) staff       (20)        0 2024-03-03 07:12:53.377492 argmaxtools-0.1.7/tests/
--rw-r--r--   0 ati        (501) staff       (20)     8234 2024-02-05 05:59:16.000000 argmaxtools-0.1.7/tests/test_attention.py
+drwxr-xr-x   0 ati        (501) staff       (20)        0 2024-05-02 22:01:03.902029 argmaxtools-0.1.8/
+-rw-r--r--   0 ati        (501) staff       (20)      849 2024-05-02 22:01:03.901973 argmaxtools-0.1.8/PKG-INFO
+-rw-r--r--   0 ati        (501) staff       (20)       45 2024-02-19 23:35:04.000000 argmaxtools-0.1.8/README.md
+drwxr-xr-x   0 ati        (501) staff       (20)        0 2024-05-02 22:01:03.899767 argmaxtools-0.1.8/argmaxtools/
+-rw-r--r--   0 ati        (501) staff       (20)        0 2024-02-05 05:59:16.000000 argmaxtools-0.1.8/argmaxtools/__init__.py
+-rw-r--r--   0 ati        (501) staff       (20)     8307 2024-04-24 07:43:27.000000 argmaxtools-0.1.8/argmaxtools/_sdpa.py
+-rw-r--r--   0 ati        (501) staff       (20)       22 2024-04-24 07:48:00.000000 argmaxtools-0.1.8/argmaxtools/_version.py
+drwxr-xr-x   0 ati        (501) staff       (20)        0 2024-05-02 22:01:03.901370 argmaxtools-0.1.8/argmaxtools/compress/
+-rw-r--r--   0 ati        (501) staff       (20)       87 2024-02-19 23:35:04.000000 argmaxtools-0.1.8/argmaxtools/compress/__init__.py
+-rw-r--r--   0 ati        (501) staff       (20)    28832 2024-02-29 00:18:56.000000 argmaxtools-0.1.8/argmaxtools/compress/palettize.py
+-rw-r--r--   0 ati        (501) staff       (20)     4072 2024-02-19 23:35:04.000000 argmaxtools-0.1.8/argmaxtools/compress/sparse_outlier.py
+-rw-r--r--   0 ati        (501) staff       (20)      704 2024-02-05 05:59:16.000000 argmaxtools-0.1.8/argmaxtools/compress/utils.py
+-rw-r--r--   0 ati        (501) staff       (20)    11927 2024-05-02 21:26:25.000000 argmaxtools-0.1.8/argmaxtools/nn.py
+-rw-r--r--   0 ati        (501) staff       (20)     2856 2024-03-18 02:24:28.000000 argmaxtools-0.1.8/argmaxtools/tensor_typing.py
+-rw-r--r--   0 ati        (501) staff       (20)    18737 2024-05-02 21:28:03.000000 argmaxtools-0.1.8/argmaxtools/test_utils.py
+-rw-r--r--   0 ati        (501) staff       (20)     5647 2024-04-23 04:20:01.000000 argmaxtools-0.1.8/argmaxtools/utils.py
+drwxr-xr-x   0 ati        (501) staff       (20)        0 2024-05-02 22:01:03.900359 argmaxtools-0.1.8/argmaxtools.egg-info/
+-rw-r--r--   0 ati        (501) staff       (20)      849 2024-05-02 22:01:03.000000 argmaxtools-0.1.8/argmaxtools.egg-info/PKG-INFO
+-rw-r--r--   0 ati        (501) staff       (20)      525 2024-05-02 22:01:03.000000 argmaxtools-0.1.8/argmaxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 ati        (501) staff       (20)        1 2024-05-02 22:01:03.000000 argmaxtools-0.1.8/argmaxtools.egg-info/dependency_links.txt
+-rw-r--r--   0 ati        (501) staff       (20)       65 2024-05-02 22:01:03.000000 argmaxtools-0.1.8/argmaxtools.egg-info/requires.txt
+-rw-r--r--   0 ati        (501) staff       (20)       12 2024-05-02 22:01:03.000000 argmaxtools-0.1.8/argmaxtools.egg-info/top_level.txt
+-rw-r--r--   0 ati        (501) staff       (20)       70 2024-05-02 22:01:03.902206 argmaxtools-0.1.8/setup.cfg
+-rw-r--r--   0 ati        (501) staff       (20)     1053 2024-02-05 05:59:16.000000 argmaxtools-0.1.8/setup.py
+drwxr-xr-x   0 ati        (501) staff       (20)        0 2024-05-02 22:01:03.901584 argmaxtools-0.1.8/tests/
+-rw-r--r--   0 ati        (501) staff       (20)     8234 2024-02-05 05:59:16.000000 argmaxtools-0.1.8/tests/test_attention.py
```

### Comparing `argmaxtools-0.1.7/PKG-INFO` & `argmaxtools-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argmaxtools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Argmax Model Optimization Toolkit
 Home-page: https://github.com/argmaxinc/argmaxtools
 Author: Argmax, Inc.
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `argmaxtools-0.1.7/argmaxtools/_sdpa.py` & `argmaxtools-0.1.8/argmaxtools/_sdpa.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 #
 # For licensing see accompanying LICENSE.md file.
 # Copyright (C) 2023 Argmax, Inc. All Rights Reserved.
 #
 
 from abc import ABC, abstractmethod
 from beartype import beartype
+from typing import Optional
 import torch
 from argmaxtools import tensor_typing as tt
 
 
 __all__ = ["Cat", "SplitHeadsQ", "SplitKV"]
 
 
 @beartype
 class SDPAImplementation(ABC):
     """ Abstract base class for the non-parametric Scaled Dot Product Attention (SDPA)
     """
-    def __init__(self, embed_dim, n_heads):
+    def __init__(self, embed_dim, n_heads, scale=True):
         """
         Args:
             embed_dim:  The embedding dimensions of the input and output tensors
             n_heads:    The number of attention heads
         """
         assert embed_dim % n_heads == 0
         self.embed_dim = embed_dim
         self.n_heads = n_heads
         self.per_head_dim = self.embed_dim // self.n_heads
-        self.qk_denom = self.per_head_dim ** -0.5
+        self.qk_denom = self.per_head_dim ** -0.5 if scale else None
 
     @abstractmethod
     def sdpa(self,
              query: tt.SDPAQueryType,
              key: tt.SDPAKeyType,
              value: tt.SDPAValueType,
              key_padding_mask: tt.SDPAKeyPaddingMaskType,
              causal: bool,
-             return_w: bool = False
+             return_w: bool = False,
+             qk_mask: Optional[tt.SDPAQKMaskType] = None,
              ) -> tt.SDPAOutputType:
         pass
 
 
 class Cat(SDPAImplementation):
     """ Original SDPA
     """
-    def sdpa(self, query, key, value, key_padding_mask, causal, return_w=False):
+    def sdpa(self, query, key, value, key_padding_mask, causal, return_w=False, qk_mask=None):
         batch_size = query.shape[0]
         bhcx = (batch_size, self.n_heads, self.per_head_dim, -1)
 
-        mh_q = query.view(*bhcx) * self.qk_denom
+        mh_q = query.view(*bhcx)
+        if self.qk_denom is not None:
+            mh_q = mh_q * self.qk_denom
+
         mh_k = key.view(*bhcx)
         mh_w = torch.einsum('bhcq,bhck->bhqk', mh_q, mh_k)
 
         if key_padding_mask is not None:
             mh_w = mh_w + key_padding_mask[:, None, None, :]
 
         if causal:
@@ -59,14 +64,20 @@
             assert q_seq_len == k_seq_len
 
             causal_mask = torch.triu(
                 torch.ones(q_seq_len, k_seq_len, device=mh_w.device), 1
             )[None, None, :, :] * -1e4
             mh_w = mh_w + causal_mask
 
+        if qk_mask is not None:
+            # If qk_mask is same for all heads, broadcast it
+            if len(qk_mask.shape) == 3:
+                qk_mask = qk_mask.unsqueeze(1)
+            mh_w = mh_w + qk_mask
+
         mh_w = mh_w.softmax(dim=3)
 
         mh_v = value.view(*bhcx)
         attn = torch.einsum("bhqk,bhck->bhcq", [mh_w, mh_v])
         attn = attn.reshape(batch_size, self.embed_dim, 1, -1)
 
         if return_w:
@@ -77,15 +88,15 @@
 class SplitHeadsQ(SDPAImplementation):
     """ SDPA with explicit multi-head splits and query sequence chunking
     """
     # Runtime configurable
     num_chunks: int = 4
     min_split_seq_len: int = 256
 
-    def sdpa(self, query, key, value, key_padding_mask, causal, return_w=False):
+    def sdpa(self, query, key, value, key_padding_mask, causal, return_w=False, qk_mask=None):
         q_seq_length = query.size(3)
 
         if q_seq_length < self.min_split_seq_len:
             num_chunks = 1
             chunk_size = q_seq_length
         else:
             num_chunks = self.num_chunks
@@ -112,26 +123,47 @@
 
         mh_v = [
             value[:, head_idx * self.per_head_dim:(head_idx + 1) * self.per_head_dim, :, :]
             for head_idx in range(self.n_heads)
         ]
 
         mh_w = [[
-            torch.einsum("bchq,bkhc->bkhq", [qi_chunk, ki]) * self.qk_denom
+            torch.einsum("bchq,bkhc->bkhq", [qi_chunk, ki])
             for qi_chunk in h_q_chunked
         ] for h_q_chunked, ki in zip(mh_q_chunked, mh_k)]
 
+        if self.qk_denom is not None:
+            mh_w = [_mh_w * self.qk_denom for _mh_w in mh_w]
+
         if key_padding_mask is not None:
             for h in range(self.n_heads):
                 for chunk_idx in range(num_chunks):
                     mh_w[h][chunk_idx] = mh_w[h][chunk_idx] + key_padding_mask[:, :, None, None]
 
         if causal:
             raise NotImplementedError("TODO(atiorh)")
 
+        if qk_mask is not None:
+            if len(qk_mask.shape) == 4:
+                qk_mask = qk_mask.permute(0, 3, 1, 2)
+            elif len(qk_mask.shape) == 3:
+                qk_mask = qk_mask.transpose(1, 2)
+            else:
+                raise ValueError(qk_mask.shape)
+
+            for h in range(self.n_heads):
+                for chunk_idx in range(num_chunks):
+                    mh_w[h][chunk_idx] = mh_w[h][chunk_idx] + \
+                        qk_mask[
+                            :,
+                            :,
+                            None if len(qk_mask.shape) == 3 else h:h+1,
+                            chunk_idx*chunk_size:(chunk_idx + 1) * chunk_size
+                        ]
+
         attn_weights = [[
             aw_chunk.softmax(dim=1) for aw_chunk in aw_chunked]
             for aw_chunked in mh_w
         ]
 
         attn = [[
             torch.einsum("bkhq,bchk->bchq", wi_chunk, vi)
@@ -165,15 +197,18 @@
         else:
             assert k_seq_len % self.num_chunks == 0
             kv_chunk_size = k_seq_len // self.num_chunks
 
         # Reshape and scale query
         batch_size = query.shape[0]
         bhcx = (batch_size, self.n_heads, self.per_head_dim, -1)
-        mh_q = query.view(*bhcx) * self.qk_denom
+        mh_q = query.view(*bhcx)
+        if self.qk_denom is not None:
+            mh_q = mh_q * self.qk_denom
+
         mh_v = value.view(*bhcx).split(kv_chunk_size, dim=3)
 
         # Reshape and split key into chunks
         mh_k = key.view(*bhcx).split(kv_chunk_size, dim=3)
         mh_w = [torch.einsum('bhcq,bhck->bhqk', mh_q, ki) for ki in mh_k]
 
         if key_padding_mask is not None:
```

### Comparing `argmaxtools-0.1.7/argmaxtools/compress/palettize.py` & `argmaxtools-0.1.8/argmaxtools/compress/palettize.py`

 * *Files identical despite different names*

### Comparing `argmaxtools-0.1.7/argmaxtools/compress/sparse_outlier.py` & `argmaxtools-0.1.8/argmaxtools/compress/sparse_outlier.py`

 * *Files identical despite different names*

### Comparing `argmaxtools-0.1.7/argmaxtools/compress/utils.py` & `argmaxtools-0.1.8/argmaxtools/compress/utils.py`

 * *Files identical despite different names*

### Comparing `argmaxtools-0.1.7/argmaxtools/nn.py` & `argmaxtools-0.1.8/argmaxtools/nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 class AttentionType(Enum):
     SelfAttention = 1
     CausalSelfAttention = 2
     KVCachedSelfAttention = 3
     EncoderDecoderCrossAttention = 4
+    KVCachedEncoderDecoderCrossAttention = 5
 
 
 class AttentionHeadType(Enum):
     MultiHead = 1     # MHA: https://arxiv.org/abs/1706.03762
     GroupQuery = 2    # GQA: https://arxiv.org/abs/2305.13245
     MultiQuery = 3    # MQA: https://arxiv.org/pdf/1911.02150
 
@@ -117,37 +118,39 @@
 
     def forward(self,
                 input_embeds: tt.InputEmbedsType,
                 key_padding_mask: Optional[tt.AttentionMaskType] = None,
                 key_cache: Optional[tt.KVCacheType] = None,
                 value_cache: Optional[tt.KVCacheType] = None,
                 kv_cache_update_mask: Optional[tt.AttentionMaskType] = None,
-                encoder_output_embeds: Optional[tt.EncoderOutputEmbedsType] = None
+                encoder_output_embeds: Optional[tt.EncoderOutputEmbedsType] = None,
+                qk_mask: Optional[tt.SDPAQKMaskType] = None,
                 ) -> Union[
                     tt.SelfAttentionReturnType,
                     tt.EncoderDecoderAttentionReturnType,
                     tt.KVCachedSelfAttentionReturnType]:
 
         # Project input_embds to query, key and value
         query, current_key, current_value = self._qkv_proj(input_embeds,
-                                                           encoder_output_embeds,
-                                                           kv_cache_update_mask)
+                                                           encoder_output_embeds)
+
         # Configure the key and value tensors based on attention type
         key, value = self._finalize_kv(key_cache,
                                        value_cache,
                                        current_key,
                                        current_value,
                                        kv_cache_update_mask,
                                        encoder_output_embeds)
 
         # Compute scaled dot product attention
         attn = self._sdpa(query,
                           key,
                           value,
-                          key_padding_mask)
+                          key_padding_mask,
+                          qk_mask)
 
         if self._return_w:
             attn, attn_weights = attn
 
         # Final projection
         attn = self.o_proj(attn)
 
@@ -160,33 +163,35 @@
         if self._return_w:
             outputs += (attn_weights,)
 
         return outputs
 
     def _qkv_proj(self,
                   input_embeds,
-                  encoder_output_embeds,
-                  kv_cache_update_mask):
+                  encoder_output_embeds):
         """ Compute qkv projections prescribed by currently active input configurations
         """
         if encoder_output_embeds is not None:
             if self.attention_type != AttentionType.EncoderDecoderCrossAttention:
                 raise ValueError(
                     "`encoder_output_embeds` is only compatible with the "
                     "AttentionType.EncoderDecoderCrossAttention configuration")
 
             kv_proj_inputs = encoder_output_embeds
         else:
             kv_proj_inputs = input_embeds
 
         query = self.q_proj(input_embeds)
 
-        # TODO(atila): Support KVCachedEncoderDecoderCrossAttention
-        current_key = self.k_proj(kv_proj_inputs)
-        current_value = self.v_proj(kv_proj_inputs)
+        if not self.attention_type == AttentionType.KVCachedEncoderDecoderCrossAttention:
+            current_key = self.k_proj(kv_proj_inputs)
+            current_value = self.v_proj(kv_proj_inputs)
+        else:
+            current_key = None
+            current_value = None
 
         return query, current_key, current_value
 
     def _finalize_kv(self,
                      key_cache,
                      value_cache,
                      current_key,
@@ -194,56 +199,47 @@
                      kv_cache_update_mask,
                      encoder_output_embeds):
         """ Determine the key and value tensors based on attention type. If head_type is GQA or MQA,
         repeat key and value tensors to match the query tensor embedding dimensionality.
         """
         if self.attention_type == AttentionType.KVCachedSelfAttention:
             # Cache updates
+            assert key_cache is not None and value_cache is not None
             kv_cache_update_mask = kv_cache_update_mask[:, None, None, :]
             key = current_key * kv_cache_update_mask + key_cache * (1. - kv_cache_update_mask)
             value = current_value * kv_cache_update_mask + value_cache * (1. - kv_cache_update_mask)
 
-        elif self.attention_type == AttentionType.EncoderDecoderCrossAttention:
-            # Reuse static (encoder) cache
-            if key_cache is not None or value_cache is not None:
-                if encoder_output_embeds is not None:
-                    "Can not provide encoder_output_embeds and {key,value}_cache simultaneously"
-
-                logger.warning(
-                    "EncoderDecoderCrossAttention receiving {key,value}_cache inputs "
-                    "imply that decoder key and value projections were precomputed.")
-
-                key = key_cache
-                value = value_cache
-
-            elif encoder_output_embeds is not None:
-                key = current_key
-                value = current_value
-            else:
-                raise ValueError
+        elif self.attention_type == AttentionType.KVCachedEncoderDecoderCrossAttention:
+            assert key_cache is not None and value_cache is not None
+            assert current_key is None and current_value is None
+            key = key_cache
+            value = value_cache
 
         elif self.attention_type in [AttentionType.SelfAttention,
-                                     AttentionType.CausalSelfAttention]:
+                                     AttentionType.CausalSelfAttention,
+                                     AttentionType.EncoderDecoderCrossAttention]:
+            assert key_cache is None and value_cache is None
             key = current_key
             value = current_value
         else:
             raise ValueError(self.attention_type)
 
         # If not tiled upstream already
         key, value = self._maybe_tile(key, value)
 
         return key, value
 
-    def _sdpa(self, query, key, value, key_padding_mask):
+    def _sdpa(self, query, key, value, key_padding_mask, qk_mask):
         """ Compute Scaled Dot Product Attention
         """
         return self._sdpa_implementation.sdpa(
             query, key, value, key_padding_mask,
             causal=self.attention_type == AttentionType.CausalSelfAttention,
-            return_w=self._return_w
+            return_w=self._return_w,
+            qk_mask=qk_mask,
         )
 
 
 class FFN(nn.Module):
     def __init__(self, embed_dim, expansion_factor, activation_fn):
         super().__init__()
         self.fc1 = nn.Conv2d(embed_dim, embed_dim * expansion_factor, 1)
@@ -295,7 +291,38 @@
 
         if self.elementwise_affine:
             w = self.weight.view(1, self.num_channels, 1, 1)
             b = self.bias.view(1, self.num_channels, 1, 1)
             out = w * out + b
 
         return out
+
+
+class RMSNorm(nn.Module):
+    def __init__(self,
+                 num_channels,
+                 eps=1e-6,
+                 clip_mag=None,):
+
+        super().__init__()
+        self.num_channels = num_channels
+        self.eps = eps
+        self.clip_mag = clip_mag
+        self.weight = nn.Parameter(torch.Tensor(num_channels))
+        self.weight.data = torch.ones_like(self.weight.data)
+
+    def forward(self, inputs):
+        if self.clip_mag is not None:
+            inputs.clamp_(-self.clip_mag, self.clip_mag)
+
+        input_rank = len(inputs.size())
+        if input_rank != 4:
+            raise ValueError(f"Incorrect input rank (Expected 4, got {input_rank})")
+
+        inputs_sq = inputs * inputs
+        variance = inputs_sq.mean(dim=1, keepdim=True)
+        hidden_states = inputs * torch.rsqrt(variance + self.eps)
+
+        w = self.weight.view(1, self.num_channels, 1, 1)
+        out = w * hidden_states
+
+        return out
```

### Comparing `argmaxtools-0.1.7/argmaxtools/tensor_typing.py` & `argmaxtools-0.1.8/argmaxtools/tensor_typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 # _sdpa.SDPAImplementation type hints
 # Inputs
 SDPAQueryType = Float[Tensor, "batch embed_dim 1 q_seq_len"]
 SDPAKeyType = Float[Tensor, "batch embed_dim 1 kv_seq_len"]
 SDPAValueType = Float[Tensor, "batch embed_dim 1 kv_seq_len"]
 SDPAKeyPaddingMaskType = Float[Tensor, "batch kv_seq_len"]
+SDPAQKMaskType = Union[
+    Float[Tensor, "batch n_heads q_seq_len kv_seq_len"],
+    Float[Tensor, "batch q_seq_len kv_seq_len"],
+]
 
 # Outputs
 SDPAOutputAttnType = Float[Tensor, "batch embed_dim 1 q_seq_len"]
 SDPAOutputAttnWeightsType = Float[Tensor, "batch n_heads q_seq_len kv_seq_len"]
 SDPAOutputType = Union[
     SDPAOutputAttnType,
     Tuple[SDPAOutputAttnType, SDPAOutputAttnWeightsType]
```

### Comparing `argmaxtools-0.1.7/argmaxtools/test_utils.py` & `argmaxtools-0.1.8/argmaxtools/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 TEST_COMPUTE_UNIT = ct.ComputeUnit.CPU_AND_NE
 TEST_COMPRESSION_MIN_SPEEDUP = 0.95
 TEST_COREML_IO_FLOAT_DTYPE = np.float16
 TEST_WEIGHT_COMPRESS_NBITS = 1
 TEST_MIN_SPEEDUP_VS_CPU = 1.
 TEST_PSNR_THR = 35
 TEST_MIN_DEPLOYMENT_TARGET = ct.target.macOS13
-
+TEST_DEFAULT_NBITS = None
+TEST_COREML_PRECISION = ct.precision.FLOAT16
 
 # CoreMLPalettizerTests
 TEST_ALLOWED_NBITS = [1, 2, 4, 6, 8]
 TEST_DONT_PALETTIZE_TOP_K = 4
 
 
 class CoreMLTestsMixin(unittest.TestCase):
@@ -49,14 +50,17 @@
         assert hasattr(cls, "test_torch_inputs")
         assert hasattr(cls, "test_output_names")
 
         cls.test_coreml_inputs = _create_coreml_inputs(cls.test_torch_inputs)
         cls.test_coreml_model = _create_coreml_model(
             cls.test_torch_model, cls.test_torch_inputs, cls.test_output_names)
 
+        if TEST_DEFAULT_NBITS is not None:
+            cls.test_coreml_model = _compress_coreml_model(cls.test_coreml_model)
+
         cls.test_coreml_output = cls.test_coreml_model.predict(
             cls.test_coreml_inputs
         )[cls.test_output_names[0]].squeeze()
 
     @classmethod
     def tearDownClass(cls):
         cls.test_coreml_inputs = None
@@ -75,15 +79,17 @@
         assert hasattr(self, "test_torch_model")
         assert hasattr(self, "test_cache_dir")
 
         with self.subTest(phase="torch2coreml_correctness"):
             if hasattr(self, "test_torch_output"):
                 reference = self.test_torch_output
             else:
-                reference = self.test_torch_model(**self.test_torch_inputs)[0]
+                reference = self.test_torch_model(**self.test_torch_inputs)
+                if isinstance(reference, (list, tuple)):
+                    reference = reference[0]
 
             proxy = torch.from_numpy(self.test_coreml_output).to(reference)
             psnr = compute_psnr(reference, proxy)
 
             logger.info(f"torch2coreml PSNR={psnr:.3g}")
             self.assertGreater(psnr, TEST_PSNR_THR)
 
@@ -405,24 +411,40 @@
         ],
         outputs=[
             ct.TensorType(output_name, dtype=TEST_COREML_IO_FLOAT_DTYPE)
             for output_name in output_names
         ],
         minimum_deployment_target=TEST_MIN_DEPLOYMENT_TARGET,
         compute_units=TEST_COMPUTE_UNIT,
+        compute_precision=TEST_COREML_PRECISION,
+    )
+
+
+def _compress_coreml_model(mlmodel: ct.models.MLModel) -> ct.models.MLModel:
+    return ct.optimize.coreml.palettize_weights(
+        mlmodel,
+        config=ct.optimize.coreml.OptimizationConfig(
+            global_config=ct.optimize.coreml.OpPalettizerConfig(
+                mode="kmeans",
+                nbits=TEST_DEFAULT_NBITS,
+            ),
+        )
     )
 
 
 def _save_coreml_asset(coreml_model: ct.models.MLModel,
                        out_dir: str,
                        fname: str,
                        do_compile: bool = True) -> None:
     """ Helper function to save Core ML models (`.mlpackage`) to disk
     """
-    save_coreml_to = os.path.join(out_dir, f"{fname}.mlpackage")
+    if TEST_DEFAULT_NBITS is not None:
+        save_coreml_to = os.path.join(out_dir, f"{fname}_{TEST_DEFAULT_NBITS}-bit.mlpackage")
+    else:
+        save_coreml_to = os.path.join(out_dir, f"{fname}.mlpackage")
 
     logger.info(f"Saving Core ML test artifact to {save_coreml_to}")
     coreml_model.save(save_coreml_to)
 
     if do_compile:
         mlmodelc_path = _compile_coreml_model(save_coreml_to, out_dir, fname)
         logger.info(f"Compiled model at {mlmodelc_path}. Removing {save_coreml_to}")
```

### Comparing `argmaxtools-0.1.7/argmaxtools/utils.py` & `argmaxtools-0.1.8/argmaxtools/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,16 @@
     return linear_to_conv2d_map_base(common_name_mappings, state_dict, prefix, local_metadata,
                                      strict, missing_keys, unexpected_keys, error_msgs)
 
 
 def linear_to_conv2d_map_ffn(state_dict, prefix, local_metadata, strict,
                              missing_keys, unexpected_keys, error_msgs):
     common_name_mappings = {
-        "fc1": ["fc1"],
-        "fc2": ["fc2"],
+        "fc1": ["fc1", "wi"],
+        "fc2": ["fc2", "wo"],
     }
     return linear_to_conv2d_map_base(common_name_mappings, state_dict, prefix, local_metadata,
                                      strict, missing_keys, unexpected_keys, error_msgs)
 
 
 def linear_to_conv2d_map_base(common_name_mappings, state_dict, prefix, local_metadata,
                               strict, missing_keys, unexpected_keys, error_msgs):
```

### Comparing `argmaxtools-0.1.7/argmaxtools.egg-info/PKG-INFO` & `argmaxtools-0.1.8/argmaxtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argmaxtools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Argmax Model Optimization Toolkit
 Home-page: https://github.com/argmaxinc/argmaxtools
 Author: Argmax, Inc.
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `argmaxtools-0.1.7/argmaxtools.egg-info/SOURCES.txt` & `argmaxtools-0.1.8/argmaxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argmaxtools-0.1.7/setup.py` & `argmaxtools-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `argmaxtools-0.1.7/tests/test_attention.py` & `argmaxtools-0.1.8/tests/test_attention.py`

 * *Files identical despite different names*


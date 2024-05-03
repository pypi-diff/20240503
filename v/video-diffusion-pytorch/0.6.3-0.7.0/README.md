# Comparing `tmp/video-diffusion-pytorch-0.6.3.tar.gz` & `tmp/video_diffusion_pytorch-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video-diffusion-pytorch-0.6.3.tar", last modified: Tue Nov 28 14:46:01 2023, max compression
+gzip compressed data, was "video_diffusion_pytorch-0.7.0.tar", last modified: Fri May  3 16:59:28 2024, max compression
```

## Comparing `video-diffusion-pytorch-0.6.3.tar` & `video_diffusion_pytorch-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 14:46:01.087624 video-diffusion-pytorch-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-11-28 14:45:49.000000 video-diffusion-pytorch-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      916 2023-11-28 14:46:01.087624 video-diffusion-pytorch-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2023-11-28 14:45:49.000000 video-diffusion-pytorch-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 14:46:01.087624 video-diffusion-pytorch-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-11-28 14:45:49.000000 video-diffusion-pytorch-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 14:46:01.083624 video-diffusion-pytorch-0.6.3/video_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-28 14:45:49.000000 video-diffusion-pytorch-0.6.3/video_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-11-28 14:45:49.000000 video-diffusion-pytorch-0.6.3/video_diffusion_pytorch/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    33713 2023-11-28 14:45:49.000000 video-diffusion-pytorch-0.6.3/video_diffusion_pytorch/video_diffusion_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 14:46:01.087624 video-diffusion-pytorch-0.6.3/video_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2023-11-28 14:46:01.000000 video-diffusion-pytorch-0.6.3/video_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-11-28 14:46:01.000000 video-diffusion-pytorch-0.6.3/video_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 14:46:01.000000 video-diffusion-pytorch-0.6.3/video_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-11-28 14:46:01.000000 video-diffusion-pytorch-0.6.3/video_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-28 14:46:01.000000 video-diffusion-pytorch-0.6.3/video_diffusion_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:59:28.864784 video_diffusion_pytorch-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 16:59:24.000000 video_diffusion_pytorch-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-03 16:59:28.864784 video_diffusion_pytorch-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-05-03 16:59:24.000000 video_diffusion_pytorch-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:59:28.864784 video_diffusion_pytorch-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-03 16:59:24.000000 video_diffusion_pytorch-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:59:28.864784 video_diffusion_pytorch-0.7.0/video_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 16:59:24.000000 video_diffusion_pytorch-0.7.0/video_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-03 16:59:24.000000 video_diffusion_pytorch-0.7.0/video_diffusion_pytorch/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33849 2024-05-03 16:59:24.000000 video_diffusion_pytorch-0.7.0/video_diffusion_pytorch/video_diffusion_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:59:28.864784 video_diffusion_pytorch-0.7.0/video_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-03 16:59:28.000000 video_diffusion_pytorch-0.7.0/video_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-03 16:59:28.000000 video_diffusion_pytorch-0.7.0/video_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:59:28.000000 video_diffusion_pytorch-0.7.0/video_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 16:59:28.000000 video_diffusion_pytorch-0.7.0/video_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 16:59:28.000000 video_diffusion_pytorch-0.7.0/video_diffusion_pytorch.egg-info/top_level.txt
```

### Comparing `video-diffusion-pytorch-0.6.3/LICENSE` & `video_diffusion_pytorch-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `video-diffusion-pytorch-0.6.3/PKG-INFO` & `video_diffusion_pytorch-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-diffusion-pytorch
-Version: 0.6.3
+Version: 0.7.0
 Summary: Video Diffusion - Pytorch
 Home-page: https://github.com/lucidrains/video-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,denoising diffusion probabilistic models,video generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `video-diffusion-pytorch-0.6.3/README.md` & `video_diffusion_pytorch-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `video-diffusion-pytorch-0.6.3/setup.py` & `video_diffusion_pytorch-0.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='video-diffusion-pytorch',
     packages=find_packages(exclude=[]),
-    version='0.6.3',
+    version='0.7.0',
     license='MIT',
     description='Video Diffusion - Pytorch',
     long_description_content_type='text/markdown',
     author='Phil Wang',
     author_email='lucidrains@gmail.com',
     url='https://github.com/lucidrains/video-diffusion-pytorch',
     keywords=[
```

### Comparing `video-diffusion-pytorch-0.6.3/video_diffusion_pytorch/text.py` & `video_diffusion_pytorch-0.7.0/video_diffusion_pytorch/text.py`

 * *Files identical despite different names*

### Comparing `video-diffusion-pytorch-0.6.3/video_diffusion_pytorch/video_diffusion_pytorch.py` & `video_diffusion_pytorch-0.7.0/video_diffusion_pytorch/video_diffusion_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,54 +156,63 @@
         self.gamma = nn.Parameter(torch.ones(1, dim, 1, 1, 1))
 
     def forward(self, x):
         var = torch.var(x, dim = 1, unbiased = False, keepdim = True)
         mean = torch.mean(x, dim = 1, keepdim = True)
         return (x - mean) / (var + self.eps).sqrt() * self.gamma
 
+class RMSNorm(nn.Module):
+    def __init__(self, dim):
+        super().__init__()
+        self.scale = dim ** 0.5
+        self.gamma = nn.Parameter(torch.ones(dim, 1, 1, 1))
+
+    def forward(self, x):
+        return F.normalize(x, dim = 1) * self.scale * self.gamma
+
 class PreNorm(nn.Module):
     def __init__(self, dim, fn):
         super().__init__()
         self.fn = fn
         self.norm = LayerNorm(dim)
 
     def forward(self, x, **kwargs):
         x = self.norm(x)
         return self.fn(x, **kwargs)
 
 # building block modules
 
 
 class Block(nn.Module):
-    def __init__(self, dim, dim_out, groups = 8):
+    def __init__(self, dim, dim_out):
         super().__init__()
         self.proj = nn.Conv3d(dim, dim_out, (1, 3, 3), padding = (0, 1, 1))
-        self.norm = nn.GroupNorm(groups, dim_out)
+        self.norm = RMSNorm(dim_out)
         self.act = nn.SiLU()
 
     def forward(self, x, scale_shift = None):
         x = self.proj(x)
         x = self.norm(x)
 
         if exists(scale_shift):
             scale, shift = scale_shift
             x = x * (scale + 1) + shift
 
         return self.act(x)
 
 class ResnetBlock(nn.Module):
-    def __init__(self, dim, dim_out, *, time_emb_dim = None, groups = 8):
+    def __init__(self, dim, dim_out, *, time_emb_dim = None):
         super().__init__()
         self.mlp = nn.Sequential(
             nn.SiLU(),
             nn.Linear(time_emb_dim, dim_out * 2)
         ) if exists(time_emb_dim) else None
 
-        self.block1 = Block(dim, dim_out, groups = groups)
-        self.block2 = Block(dim_out, dim_out, groups = groups)
+        self.block1 = Block(dim, dim_out)
+        self.block2 = Block(dim_out, dim_out)
         self.res_conv = nn.Conv3d(dim, dim_out, 1) if dim != dim_out else nn.Identity()
 
     def forward(self, x, time_emb = None):
 
         scale_shift = None
         if exists(self.mlp):
             assert exists(time_emb), 'time emb must be passed in'
@@ -351,16 +360,15 @@
         channels = 3,
         attn_heads = 8,
         attn_dim_head = 32,
         use_bert_text_cond = False,
         init_dim = None,
         init_kernel_size = 7,
         use_sparse_linear_attn = True,
-        block_type = 'resnet',
-        resnet_groups = 8
+        block_type = 'resnet'
     ):
         super().__init__()
         self.channels = channels
 
         # temporal attention and its relative positional encoding
 
         rotary_emb = RotaryEmbedding(min(32, attn_dim_head))
@@ -408,15 +416,15 @@
         self.downs = nn.ModuleList([])
         self.ups = nn.ModuleList([])
 
         num_resolutions = len(in_out)
 
         # block type
 
-        block_klass = partial(ResnetBlock, groups = resnet_groups)
+        block_klass = ResnetBlock
         block_klass_cond = partial(block_klass, time_emb_dim = cond_dim)
 
         # modules for all layers
 
         for ind, (dim_in, dim_out) in enumerate(in_out):
             is_last = ind >= (num_resolutions - 1)
```

### Comparing `video-diffusion-pytorch-0.6.3/video_diffusion_pytorch.egg-info/PKG-INFO` & `video_diffusion_pytorch-0.7.0/video_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-diffusion-pytorch
-Version: 0.6.3
+Version: 0.7.0
 Summary: Video Diffusion - Pytorch
 Home-page: https://github.com/lucidrains/video-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,denoising diffusion probabilistic models,video generation
 Classifier: Development Status :: 4 - Beta
```


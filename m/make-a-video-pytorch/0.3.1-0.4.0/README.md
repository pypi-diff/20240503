# Comparing `tmp/make-a-video-pytorch-0.3.1.tar.gz` & `tmp/make_a_video_pytorch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make-a-video-pytorch-0.3.1.tar", last modified: Mon Jun 19 18:28:53 2023, max compression
+gzip compressed data, was "make_a_video_pytorch-0.4.0.tar", last modified: Fri May  3 17:34:45 2024, max compression
```

## Comparing `make-a-video-pytorch-0.3.1.tar` & `make_a_video_pytorch-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:28:53.274325 make-a-video-pytorch-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 18:28:43.000000 make-a-video-pytorch-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 18:28:53.274325 make-a-video-pytorch-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-19 18:28:43.000000 make-a-video-pytorch-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:28:53.270326 make-a-video-pytorch-0.3.1/make_a_video_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-19 18:28:43.000000 make-a-video-pytorch-0.3.1/make_a_video_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-06-19 18:28:43.000000 make-a-video-pytorch-0.3.1/make_a_video_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-06-19 18:28:43.000000 make-a-video-pytorch-0.3.1/make_a_video_pytorch/make_a_video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:28:53.274325 make-a-video-pytorch-0.3.1/make_a_video_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 18:28:53.000000 make-a-video-pytorch-0.3.1/make_a_video_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-19 18:28:53.000000 make-a-video-pytorch-0.3.1/make_a_video_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:28:53.000000 make-a-video-pytorch-0.3.1/make_a_video_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 18:28:53.000000 make-a-video-pytorch-0.3.1/make_a_video_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 18:28:53.000000 make-a-video-pytorch-0.3.1/make_a_video_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 18:28:53.274325 make-a-video-pytorch-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-19 18:28:43.000000 make-a-video-pytorch-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:34:45.298639 make_a_video_pytorch-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 17:34:41.000000 make_a_video_pytorch-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-03 17:34:45.298639 make_a_video_pytorch-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-03 17:34:41.000000 make_a_video_pytorch-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:34:45.298639 make_a_video_pytorch-0.4.0/make_a_video_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 17:34:41.000000 make_a_video_pytorch-0.4.0/make_a_video_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-03 17:34:41.000000 make_a_video_pytorch-0.4.0/make_a_video_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20450 2024-05-03 17:34:41.000000 make_a_video_pytorch-0.4.0/make_a_video_pytorch/make_a_video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:34:45.298639 make_a_video_pytorch-0.4.0/make_a_video_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-03 17:34:45.000000 make_a_video_pytorch-0.4.0/make_a_video_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-03 17:34:45.000000 make_a_video_pytorch-0.4.0/make_a_video_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:34:45.000000 make_a_video_pytorch-0.4.0/make_a_video_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 17:34:45.000000 make_a_video_pytorch-0.4.0/make_a_video_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 17:34:45.000000 make_a_video_pytorch-0.4.0/make_a_video_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:34:45.298639 make_a_video_pytorch-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-03 17:34:41.000000 make_a_video_pytorch-0.4.0/setup.py
```

### Comparing `make-a-video-pytorch-0.3.1/LICENSE` & `make_a_video_pytorch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `make-a-video-pytorch-0.3.1/PKG-INFO` & `make_a_video_pytorch-0.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: make-a-video-pytorch
-Version: 0.3.1
+Version: 0.4.0
 Summary: Make-A-Video - Pytorch
 Home-page: https://github.com/lucidrains/make-a-video-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism,text-to-video,axial convolutions
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: classifier-free-guidance-pytorch
+Requires-Dist: einops>=0.6
+Requires-Dist: torch>=1.6
```

### Comparing `make-a-video-pytorch-0.3.1/README.md` & `make_a_video_pytorch-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `make-a-video-pytorch-0.3.1/make_a_video_pytorch/attend.py` & `make_a_video_pytorch-0.4.0/make_a_video_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `make-a-video-pytorch-0.3.1/make_a_video_pytorch/make_a_video.py` & `make_a_video_pytorch-0.4.0/make_a_video_pytorch/make_a_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,20 +342,19 @@
 
 class Block(nn.Module):
     def __init__(
         self,
         dim,
         dim_out,
         kernel_size = 3,
-        temporal_kernel_size = None,
-        groups = 8
+        temporal_kernel_size = None
     ):
         super().__init__()
         self.project = PseudoConv3d(dim, dim_out, 3)
-        self.norm = nn.GroupNorm(groups, dim_out)
+        self.norm = RMSNorm(dim_out)
         self.act = nn.SiLU()
 
     def forward(
         self,
         x,
         scale_shift = None,
         enable_time = False
@@ -372,28 +371,27 @@
 class ResnetBlock(nn.Module):
     def __init__(
         self,
         dim,
         dim_out,
         *,
         timestep_cond_dim = None,
-        groups = 8
     ):
         super().__init__()
 
         self.timestep_mlp = None
 
         if exists(timestep_cond_dim):
             self.timestep_mlp = nn.Sequential(
                 nn.SiLU(),
                 nn.Linear(timestep_cond_dim, dim_out * 2)
             )
 
-        self.block1 = Block(dim, dim_out, groups = groups)
-        self.block2 = Block(dim_out, dim_out, groups = groups)
+        self.block1 = Block(dim, dim_out)
+        self.block2 = Block(dim_out, dim_out)
         self.res_conv = PseudoConv3d(dim, dim_out, 1) if dim != dim_out else nn.Identity()
 
     def forward(
         self,
         x,
         timestep_emb = None,
         enable_time = True
```

### Comparing `make-a-video-pytorch-0.3.1/make_a_video_pytorch.egg-info/PKG-INFO` & `make_a_video_pytorch-0.4.0/make_a_video_pytorch.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: make-a-video-pytorch
-Version: 0.3.1
+Version: 0.4.0
 Summary: Make-A-Video - Pytorch
 Home-page: https://github.com/lucidrains/make-a-video-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism,text-to-video,axial convolutions
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: classifier-free-guidance-pytorch
+Requires-Dist: einops>=0.6
+Requires-Dist: torch>=1.6
```

### Comparing `make-a-video-pytorch-0.3.1/setup.py` & `make_a_video_pytorch-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'make-a-video-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.1',
+  version = '0.4.0',
   license='MIT',
   description = 'Make-A-Video - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/make-a-video-pytorch',
   keywords = [
```


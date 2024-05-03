# Comparing `tmp/x-unet-0.3.1.tar.gz` & `tmp/x_unet-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-unet-0.3.1.tar", last modified: Fri Jul 14 14:42:29 2023, max compression
+gzip compressed data, was "x_unet-0.4.0.tar", last modified: Fri May  3 17:22:22 2024, max compression
```

## Comparing `x-unet-0.3.1.tar` & `x_unet-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:42:29.186716 x-unet-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-14 14:42:17.000000 x-unet-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 14:42:29.186716 x-unet-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-14 14:42:17.000000 x-unet-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:42:29.186716 x-unet-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-14 14:42:17.000000 x-unet-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:42:29.182716 x-unet-0.3.1/x_unet/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 14:42:17.000000 x-unet-0.3.1/x_unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19339 2023-07-14 14:42:17.000000 x-unet-0.3.1/x_unet/x_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:42:29.182716 x-unet-0.3.1/x_unet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 14:42:29.000000 x-unet-0.3.1/x_unet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-14 14:42:29.000000 x-unet-0.3.1/x_unet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:42:29.000000 x-unet-0.3.1/x_unet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 14:42:29.000000 x-unet-0.3.1/x_unet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 14:42:29.000000 x-unet-0.3.1/x_unet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:22:22.036175 x_unet-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 17:22:18.000000 x_unet-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-03 17:22:22.036175 x_unet-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-03 17:22:18.000000 x_unet-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:22:22.036175 x_unet-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-03 17:22:18.000000 x_unet-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:22:22.036175 x_unet-0.4.0/x_unet/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 17:22:18.000000 x_unet-0.4.0/x_unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19429 2024-05-03 17:22:18.000000 x_unet-0.4.0/x_unet/x_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:22:22.036175 x_unet-0.4.0/x_unet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-03 17:22:22.000000 x_unet-0.4.0/x_unet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-03 17:22:22.000000 x_unet-0.4.0/x_unet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:22:22.000000 x_unet-0.4.0/x_unet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-03 17:22:22.000000 x_unet-0.4.0/x_unet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 17:22:22.000000 x_unet-0.4.0/x_unet.egg-info/top_level.txt
```

### Comparing `x-unet-0.3.1/LICENSE` & `x_unet-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `x-unet-0.3.1/README.md` & `x_unet-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `x-unet-0.3.1/setup.py` & `x_unet-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'x-unet',
   packages = find_packages(exclude=[]),
-  version = '0.3.1',
+  version = '0.4.0',
   license='MIT',
   description = 'X-Unet',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/x-unet',
   keywords = [
```

### Comparing `x-unet-0.3.1/x_unet/x_unet.py` & `x_unet-0.4.0/x_unet/x_unet.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,23 @@
     def __init__(self, fn):
         super().__init__()
         self.fn = fn
 
     def forward(self, x):
         return self.fn(x) + x
 
+class RMSNorm(nn.Module):
+    def __init__(self, dim):
+        super().__init__()
+        self.scale = dim ** 0.5
+        self.gamma = nn.Parameter(torch.ones(dim, 1, 1, 1))
+
+    def forward(self, x):
+        return F.normalize(x, dim = 1) * self.scale * self.gamma
+
 class LayerNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.gamma = nn.Parameter(torch.ones(1, dim, 1, 1, 1))
 
     def forward(self, x):
         eps = 1e-5 if x.dtype == torch.float32 else 1e-3
@@ -92,40 +101,39 @@
         frame_kernel_size = 1
     ):
         super().__init__()
         kernel_conv_kwargs = partial(kernel_and_same_pad, frame_kernel_size)
         conv = nn.Conv3d if not weight_standardize else WeightStandardizedConv3d
 
         self.proj = conv(dim, dim_out, **kernel_conv_kwargs(3, 3))
-        self.norm = nn.GroupNorm(groups, dim_out)
+        self.norm = RMSNorm(dim_out)
         self.act = nn.SiLU()
 
     def forward(self, x):
         x = self.proj(x)
         x = self.norm(x)
         return self.act(x)
 
 class ResnetBlock(nn.Module):
     def __init__(
         self,
         dim,
         dim_out,
-        groups = 8,
         frame_kernel_size = 1,
         nested_unet_depth = 0,
         nested_unet_dim = 32,
         weight_standardize = False
     ):
         super().__init__()
-        self.block1 = Block(dim, dim_out, groups = groups, weight_standardize = weight_standardize, frame_kernel_size = frame_kernel_size)
+        self.block1 = Block(dim, dim_out, weight_standardize = weight_standardize, frame_kernel_size = frame_kernel_size)
 
         if nested_unet_depth > 0:
             self.block2 = NestedResidualUnet(dim_out, depth = nested_unet_depth, M = nested_unet_dim, frame_kernel_size = frame_kernel_size, weight_standardize = weight_standardize, add_residual = True)
         else:
-            self.block2 = Block(dim_out, dim_out, groups = groups, weight_standardize = weight_standardize, frame_kernel_size = frame_kernel_size)
+            self.block2 = Block(dim_out, dim_out, weight_standardize = weight_standardize, frame_kernel_size = frame_kernel_size)
 
         self.res_conv = nn.Conv3d(dim, dim_out, 1) if dim != dim_out else nn.Identity()
 
     def forward(self, x):
         h = self.block1(x)
         h = self.block2(h)
         return h + self.res_conv(x)
@@ -313,15 +321,14 @@
         dim_mults: MaybeTuple(int) = (1, 2, 4, 8),
         num_blocks_per_stage: MaybeTuple(int) = (2, 2, 2, 2),
         num_self_attn_per_stage: MaybeTuple(int) = (0, 0, 0, 1),
         nested_unet_depths: MaybeTuple(int) = (0, 0, 0, 0),
         nested_unet_dim = 32,
         channels = 3,
         use_convnext = False,
-        resnet_groups = 8,
         consolidate_upsample_fmaps = True,
         skip_scale = 2 ** -0.5,
         weight_standardize = False,
         attn_heads: MaybeTuple(int) = 8,
         attn_dim_head: MaybeTuple(int) = 32
     ):
         super().__init__()
@@ -340,15 +347,15 @@
         self.downs = nn.ModuleList([])
         self.ups = nn.ModuleList([])
 
         num_resolutions = len(in_out)
 
         # resnet or convnext
 
-        blocks = partial(ConvNextBlock, frame_kernel_size = frame_kernel_size) if use_convnext else partial(ResnetBlock, groups = resnet_groups, weight_standardize = weight_standardize, frame_kernel_size = frame_kernel_size)
+        blocks = partial(ConvNextBlock, frame_kernel_size = frame_kernel_size) if use_convnext else partial(ResnetBlock, weight_standardize = weight_standardize, frame_kernel_size = frame_kernel_size)
 
         # whether to use nested unet, as in unet squared paper
 
         nested_unet_depths = cast_tuple(nested_unet_depths, num_resolutions)
 
         # number of blocks per stage
 
@@ -553,15 +560,14 @@
         self,
         dim,
         *,
         depth,
         M = 32,
         frame_kernel_size = 1,
         add_residual = False,
-        groups = 4,
         skip_scale = 2 ** -0.5,
         weight_standardize = False
     ):
         super().__init__()
 
         self.depth = depth
         self.downs = nn.ModuleList([])
@@ -571,30 +577,30 @@
 
         for ind in range(depth):
             is_first = ind == 0
             dim_in = dim if is_first else M
 
             down = nn.Sequential(
                 conv(dim_in, M, (1, 4, 4), stride = (1, 2, 2), padding = (0, 1, 1)),
-                nn.GroupNorm(groups, M),
+                RMSNorm(M),
                 nn.SiLU()
             )
 
             up = nn.Sequential(
                 PixelShuffleUpsample(2 * M, dim_in),
-                nn.GroupNorm(groups, dim_in),
+                RMSNorm(dim_in),
                 nn.SiLU()
             )
 
             self.downs.append(down)
             self.ups.append(up)
 
         self.mid = nn.Sequential(
             conv(M, M, **kernel_and_same_pad(frame_kernel_size, 3, 3)),
-            nn.GroupNorm(groups, M),
+            RMSNorm(M),
             nn.SiLU()
         )
 
         self.skip_scale = skip_scale
         self.add_residual = add_residual
 
     def forward(self, x, residual = None):
```


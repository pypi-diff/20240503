# Comparing `tmp/MEGABYTE-pytorch-0.2.1.tar.gz` & `tmp/megabyte_pytorch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.2.1.tar", last modified: Thu Jun 15 20:13:26 2023, max compression
+gzip compressed data, was "megabyte_pytorch-0.3.0.tar", last modified: Fri May  3 02:14:19 2024, max compression
```

## Comparing `MEGABYTE-pytorch-0.2.1.tar` & `megabyte_pytorch-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:13:26.250526 MEGABYTE-pytorch-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-15 20:13:14.000000 MEGABYTE-pytorch-0.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:13:26.250526 MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 20:13:14.000000 MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-15 20:13:14.000000 MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    13595 2023-06-15 20:13:14.000000 MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:13:26.250526 MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 20:13:26.000000 MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 20:13:26.000000 MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:13:26.000000 MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 20:13:26.000000 MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 20:13:26.000000 MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 20:13:26.250526 MEGABYTE-pytorch-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-15 20:13:14.000000 MEGABYTE-pytorch-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:13:26.250526 MEGABYTE-pytorch-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-15 20:13:14.000000 MEGABYTE-pytorch-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:14:19.602111 megabyte_pytorch-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 02:14:11.000000 megabyte_pytorch-0.3.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:14:19.598111 megabyte_pytorch-0.3.0/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 02:14:11.000000 megabyte_pytorch-0.3.0/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-03 02:14:11.000000 megabyte_pytorch-0.3.0/MEGABYTE_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-05-03 02:14:11.000000 megabyte_pytorch-0.3.0/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:14:19.602111 megabyte_pytorch-0.3.0/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 02:14:19.000000 megabyte_pytorch-0.3.0/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-03 02:14:19.000000 megabyte_pytorch-0.3.0/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:14:19.000000 megabyte_pytorch-0.3.0/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 02:14:19.000000 megabyte_pytorch-0.3.0/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 02:14:19.000000 megabyte_pytorch-0.3.0/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 02:14:19.602111 megabyte_pytorch-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-03 02:14:11.000000 megabyte_pytorch-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:14:19.602111 megabyte_pytorch-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-03 02:14:11.000000 megabyte_pytorch-0.3.0/setup.py
```

### Comparing `MEGABYTE-pytorch-0.2.1/LICENSE` & `megabyte_pytorch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch/attend.py` & `megabyte_pytorch-0.3.0/MEGABYTE_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.2.1/MEGABYTE_pytorch/megabyte.py` & `megabyte_pytorch-0.3.0/MEGABYTE_pytorch/megabyte.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,23 +135,23 @@
             flash = flash,
             dropout = dropout
         )
 
         self.dropout = nn.Dropout(dropout)
         self.norm = RMSNorm(dim)
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
-        self.to_kv = nn.Linear(dim, dim_head * 2, bias = False)
+        self.to_kv = nn.Linear(dim, inner_dim * 2, bias = False)
         self.to_out = nn.Linear(inner_dim, dim, bias = False)
 
     def forward(self, x, rotary_emb = None):
         h, device = self.heads, x.device
 
         x = self.norm(x)
         q, k, v = (self.to_q(x), *self.to_kv(x).chunk(2, dim = -1))
-        q = rearrange(q, 'b n (h d) -> b h n d', h = h)
+        q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = h), (q, k, v))
 
         if exists(rotary_emb):
             q, k = map(lambda t: apply_rotary_pos_emb(rotary_emb, t), (q, k))
 
         out = self.attend(q, k, v)
 
         out = rearrange(out, 'b h n d -> b n (h d)')
```

### Comparing `MEGABYTE-pytorch-0.2.1/README.md` & `megabyte_pytorch-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.2.1/setup.py` & `megabyte_pytorch-0.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.2.1',
+  version = '0.3.0',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
```


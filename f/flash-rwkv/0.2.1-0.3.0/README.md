# Comparing `tmp/flash_rwkv-0.2.1-py3-none-any.whl.zip` & `tmp/flash_rwkv-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,15 @@
-Zip file size: 5416 bytes, number of entries: 9
--rw-r--r--  2.0 unx      136 b- defN 24-Apr-21 02:44 flash_rwkv/__init__.py
+Zip file size: 8405 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      260 b- defN 24-May-03 15:24 flash_rwkv/__init__.py
 -rw-r--r--  2.0 unx      138 b- defN 24-Apr-21 02:44 flash_rwkv/rwkv5/__init__.py
 -rw-r--r--  2.0 unx     6969 b- defN 24-Apr-21 02:44 flash_rwkv/rwkv5/wkv5_kernel.cu
 -rw-r--r--  2.0 unx     4814 b- defN 24-Apr-21 02:44 flash_rwkv/rwkv5/wkv5_op.cpp
 -rw-r--r--  2.0 unx     7211 b- defN 24-Apr-22 01:13 flash_rwkv/rwkv5/wkv5_op.py
--rw-r--r--  2.0 unx       87 b- defN 24-Apr-22 01:35 flash_rwkv-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 01:35 flash_rwkv-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-22 01:35 flash_rwkv-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      727 b- defN 24-Apr-22 01:35 flash_rwkv-0.2.1.dist-info/RECORD
-9 files, 20185 bytes uncompressed, 4158 bytes compressed:  79.4%
+-rw-r--r--  2.0 unx      138 b- defN 24-May-03 15:24 flash_rwkv/rwkv6/__init__.py
+-rw-r--r--  2.0 unx     2768 b- defN 24-May-03 15:24 flash_rwkv/rwkv6/wkv6_kernel.cu
+-rw-r--r--  2.0 unx     2249 b- defN 24-May-03 15:24 flash_rwkv/rwkv6/wkv6_op.cpp
+-rw-r--r--  2.0 unx     3408 b- defN 24-May-03 15:24 flash_rwkv/rwkv6/wkv6_op.py
+-rw-r--r--  2.0 unx       87 b- defN 24-May-03 15:26 flash_rwkv-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 15:26 flash_rwkv-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-03 15:26 flash_rwkv-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1068 b- defN 24-May-03 15:26 flash_rwkv-0.3.0.dist-info/RECORD
+13 files, 29213 bytes uncompressed, 6615 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -9,20 +9,32 @@
 
 Filename: flash_rwkv/rwkv5/wkv5_op.cpp
 Comment: 
 
 Filename: flash_rwkv/rwkv5/wkv5_op.py
 Comment: 
 
-Filename: flash_rwkv-0.2.1.dist-info/METADATA
+Filename: flash_rwkv/rwkv6/__init__.py
 Comment: 
 
-Filename: flash_rwkv-0.2.1.dist-info/WHEEL
+Filename: flash_rwkv/rwkv6/wkv6_kernel.cu
 Comment: 
 
-Filename: flash_rwkv-0.2.1.dist-info/top_level.txt
+Filename: flash_rwkv/rwkv6/wkv6_op.cpp
 Comment: 
 
-Filename: flash_rwkv-0.2.1.dist-info/RECORD
+Filename: flash_rwkv/rwkv6/wkv6_op.py
+Comment: 
+
+Filename: flash_rwkv-0.3.0.dist-info/METADATA
+Comment: 
+
+Filename: flash_rwkv-0.3.0.dist-info/WHEEL
+Comment: 
+
+Filename: flash_rwkv-0.3.0.dist-info/top_level.txt
+Comment: 
+
+Filename: flash_rwkv-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flash_rwkv/__init__.py

```diff
@@ -1,3 +1,4 @@
 from .rwkv5 import Rwkv5LinearAttention, rwkv5_cuda_linear_attention
+from .rwkv6 import Rwkv6LinearAttention, rwkv6_cuda_linear_attention
 
-__all__ = ["Rwkv5LinearAttention", "rwkv5_cuda_linear_attention"]
+__all__ = ["Rwkv5LinearAttention", "rwkv5_cuda_linear_attention", "Rwkv6LinearAttention", "rwkv6_cuda_linear_attention"]
```


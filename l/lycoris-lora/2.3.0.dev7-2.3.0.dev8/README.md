# Comparing `tmp/lycoris_lora-2.3.0.dev7.tar.gz` & `tmp/lycoris_lora-2.3.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-2.3.0.dev7.tar", last modified: Fri May  3 13:45:27 2024, max compression
+gzip compressed data, was "lycoris_lora-2.3.0.dev8.tar", last modified: Fri May  3 13:52:32 2024, max compression
```

## Comparing `lycoris_lora-2.3.0.dev7.tar` & `lycoris_lora-2.3.0.dev8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 13:45:27.487879 lycoris_lora-2.3.0.dev7/
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-2.3.0.dev7/LICENSE.md
--rw-rw-rw-   0        0        0      527 2024-05-03 13:45:27.487879 lycoris_lora-2.3.0.dev7/PKG-INFO
--rw-rw-rw-   0        0        0    11988 2024-03-15 08:57:27.000000 lycoris_lora-2.3.0.dev7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 13:45:27.449420 lycoris_lora-2.3.0.dev7/lycoris/
--rw-rw-rw-   0        0        0      550 2024-02-05 11:33:28.000000 lycoris_lora-2.3.0.dev7/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev7/lycoris/config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:45:27.454932 lycoris_lora-2.3.0.dev7/lycoris/hcp/
--rw-rw-rw-   0        0        0      156 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev7/lycoris/hcp/__init__.py
--rw-rw-rw-   0        0        0     5329 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev7/lycoris/hcp/base.py
--rw-rw-rw-   0        0        0     2281 2024-02-12 10:32:01.000000 lycoris_lora-2.3.0.dev7/lycoris/hcp/diag_oft.py
--rw-rw-rw-   0        0        0     3391 2024-03-04 15:01:10.000000 lycoris_lora-2.3.0.dev7/lycoris/hcp/loha.py
--rw-rw-rw-   0        0        0     5643 2024-03-04 15:01:21.000000 lycoris_lora-2.3.0.dev7/lycoris/hcp/lokr.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:45:27.459439 lycoris_lora-2.3.0.dev7/lycoris/kohya/
--rw-rw-rw-   0        0        0    31784 2024-04-08 09:27:28.000000 lycoris_lora-2.3.0.dev7/lycoris/kohya/__init__.py
--rw-rw-rw-   0        0        0    59991 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev7/lycoris/kohya/model_utils.py
--rw-rw-rw-   0        0        0    61070 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev7/lycoris/kohya/original_unet.py
--rw-rw-rw-   0        0        0    21297 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev7/lycoris/kohya/sdxl_model_util.py
--rw-rw-rw-   0        0        0    42690 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev7/lycoris/kohya/sdxl_original_unet.py
--rw-rw-rw-   0        0        0    19901 2024-03-11 06:16:36.000000 lycoris_lora-2.3.0.dev7/lycoris/kohya/test_hyperdream.py
--rw-rw-rw-   0        0        0     1514 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev7/lycoris/kohya/utils.py
--rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-2.3.0.dev7/lycoris/logging.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:45:27.468815 lycoris_lora-2.3.0.dev7/lycoris/modules/
--rw-rw-rw-   0        0        0     3998 2024-03-31 02:52:53.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     8185 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/attention.py
--rw-rw-rw-   0        0        0     7015 2024-05-03 13:35:33.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/base.py
--rw-rw-rw-   0        0        0     7430 2024-05-03 13:35:44.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/boft.py
--rw-rw-rw-   0        0        0     6159 2024-05-03 13:36:17.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/diag_oft.py
--rw-rw-rw-   0        0        0     4395 2024-05-03 12:40:31.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0     4518 2024-05-03 13:36:02.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/full.py
--rw-rw-rw-   0        0        0    11788 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/glokr.py
--rw-rw-rw-   0        0        0     4978 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/glora.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:45:27.471354 lycoris_lora-2.3.0.dev7/lycoris/modules/hypernet/
--rw-rw-rw-   0        0        0       79 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/hypernet/__init__.py
--rw-rw-rw-   0        0        0     8302 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/hypernet/generater.py
--rw-rw-rw-   0        0        0     8339 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/hypernet/text_encoder.py
--rw-rw-rw-   0        0        0     2078 2024-03-11 06:14:46.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0    12663 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/lilora.py
--rw-rw-rw-   0        0        0    10526 2024-05-03 13:36:50.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0    12851 2024-05-03 13:35:27.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    17858 2024-05-03 13:35:20.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/lokr.py
--rw-rw-rw-   0        0        0     2387 2024-05-03 13:35:13.000000 lycoris_lora-2.3.0.dev7/lycoris/modules/norms.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:45:27.474358 lycoris_lora-2.3.0.dev7/lycoris/utils/
--rw-rw-rw-   0        0        0    23287 2024-03-23 07:38:25.000000 lycoris_lora-2.3.0.dev7/lycoris/utils/__init__.py
--rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-2.3.0.dev7/lycoris/utils/bnb.py
--rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev7/lycoris/utils/logger.py
--rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev7/lycoris/utils/preset.py
--rw-rw-rw-   0        0        0      196 2024-03-16 16:01:30.000000 lycoris_lora-2.3.0.dev7/lycoris/utils/tensor_norm.py
--rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev7/lycoris/utils/xformers_utils.py
--rw-rw-rw-   0        0        0    18706 2024-03-16 16:01:01.000000 lycoris_lora-2.3.0.dev7/lycoris/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:45:27.487879 lycoris_lora-2.3.0.dev7/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      527 2024-05-03 13:45:27.000000 lycoris_lora-2.3.0.dev7/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1290 2024-05-03 13:45:27.000000 lycoris_lora-2.3.0.dev7/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 13:45:27.000000 lycoris_lora-2.3.0.dev7/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-2.3.0.dev7/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       53 2024-05-03 13:45:27.000000 lycoris_lora-2.3.0.dev7/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-03 13:45:27.000000 lycoris_lora-2.3.0.dev7/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 13:45:27.489381 lycoris_lora-2.3.0.dev7/setup.cfg
--rw-rw-rw-   0        0        0      638 2024-05-03 13:45:26.000000 lycoris_lora-2.3.0.dev7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.630822 lycoris_lora-2.3.0.dev8/
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-2.3.0.dev8/LICENSE.md
+-rw-rw-rw-   0        0        0      527 2024-05-03 13:52:32.630822 lycoris_lora-2.3.0.dev8/PKG-INFO
+-rw-rw-rw-   0        0        0    11988 2024-03-15 08:57:27.000000 lycoris_lora-2.3.0.dev8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.603990 lycoris_lora-2.3.0.dev8/lycoris/
+-rw-rw-rw-   0        0        0      550 2024-02-05 11:33:28.000000 lycoris_lora-2.3.0.dev8/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/config.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.605990 lycoris_lora-2.3.0.dev8/lycoris/hcp/
+-rw-rw-rw-   0        0        0      156 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/hcp/__init__.py
+-rw-rw-rw-   0        0        0     5329 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/hcp/base.py
+-rw-rw-rw-   0        0        0     2281 2024-02-12 10:32:01.000000 lycoris_lora-2.3.0.dev8/lycoris/hcp/diag_oft.py
+-rw-rw-rw-   0        0        0     3391 2024-03-04 15:01:10.000000 lycoris_lora-2.3.0.dev8/lycoris/hcp/loha.py
+-rw-rw-rw-   0        0        0     5643 2024-03-04 15:01:21.000000 lycoris_lora-2.3.0.dev8/lycoris/hcp/lokr.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.610507 lycoris_lora-2.3.0.dev8/lycoris/kohya/
+-rw-rw-rw-   0        0        0    31784 2024-04-08 09:27:28.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/__init__.py
+-rw-rw-rw-   0        0        0    59991 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/model_utils.py
+-rw-rw-rw-   0        0        0    61070 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/original_unet.py
+-rw-rw-rw-   0        0        0    21297 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/sdxl_model_util.py
+-rw-rw-rw-   0        0        0    42690 2023-12-02 03:39:51.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/sdxl_original_unet.py
+-rw-rw-rw-   0        0        0    19901 2024-03-11 06:16:36.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/test_hyperdream.py
+-rw-rw-rw-   0        0        0     1514 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/kohya/utils.py
+-rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-2.3.0.dev8/lycoris/logging.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.616511 lycoris_lora-2.3.0.dev8/lycoris/modules/
+-rw-rw-rw-   0        0        0     4201 2024-05-03 13:52:01.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     8185 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/attention.py
+-rw-rw-rw-   0        0        0     7015 2024-05-03 13:35:33.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/base.py
+-rw-rw-rw-   0        0        0     7430 2024-05-03 13:35:44.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/boft.py
+-rw-rw-rw-   0        0        0     6159 2024-05-03 13:36:17.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/diag_oft.py
+-rw-rw-rw-   0        0        0     4395 2024-05-03 12:40:31.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0     4518 2024-05-03 13:36:02.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/full.py
+-rw-rw-rw-   0        0        0    11788 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/glokr.py
+-rw-rw-rw-   0        0        0     4978 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/glora.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.617511 lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/
+-rw-rw-rw-   0        0        0       79 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/__init__.py
+-rw-rw-rw-   0        0        0     8302 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/generater.py
+-rw-rw-rw-   0        0        0     8339 2024-02-18 06:15:40.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/text_encoder.py
+-rw-rw-rw-   0        0        0     2078 2024-03-11 06:14:46.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0    12663 2024-04-08 09:27:20.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/lilora.py
+-rw-rw-rw-   0        0        0    10526 2024-05-03 13:36:50.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0    12851 2024-05-03 13:35:27.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    17858 2024-05-03 13:35:20.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/lokr.py
+-rw-rw-rw-   0        0        0     2387 2024-05-03 13:35:13.000000 lycoris_lora-2.3.0.dev8/lycoris/modules/norms.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.619014 lycoris_lora-2.3.0.dev8/lycoris/utils/
+-rw-rw-rw-   0        0        0    23287 2024-03-23 07:38:25.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/__init__.py
+-rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/bnb.py
+-rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/logger.py
+-rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/preset.py
+-rw-rw-rw-   0        0        0      196 2024-03-16 16:01:30.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/tensor_norm.py
+-rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-2.3.0.dev8/lycoris/utils/xformers_utils.py
+-rw-rw-rw-   0        0        0    18706 2024-03-16 16:01:01.000000 lycoris_lora-2.3.0.dev8/lycoris/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:52:32.629822 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-05-03 13:52:32.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1290 2024-05-03 13:52:32.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 13:52:32.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       53 2024-05-03 13:52:32.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-03 13:52:32.000000 lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 13:52:32.630822 lycoris_lora-2.3.0.dev8/setup.cfg
+-rw-rw-rw-   0        0        0      638 2024-05-03 13:52:25.000000 lycoris_lora-2.3.0.dev8/setup.py
```

### Comparing `lycoris_lora-2.3.0.dev7/LICENSE.md` & `lycoris_lora-2.3.0.dev8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/PKG-INFO` & `lycoris_lora-2.3.0.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lycoris_lora
-Version: 2.3.0.dev7
+Version: 2.3.0.dev8
 Summary: Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion
 Home-page: https://github.com/KohakuBlueleaf/LyCORIS
 Author: Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao
 Author-email: apolloyeh0123@gmail.com
 Requires-Python: >=3.10
 License-File: LICENSE.md
 Requires-Dist: torch
```

### Comparing `lycoris_lora-2.3.0.dev7/README.md` & `lycoris_lora-2.3.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/__init__.py` & `lycoris_lora-2.3.0.dev8/lycoris/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/config.py` & `lycoris_lora-2.3.0.dev8/lycoris/config.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/hcp/base.py` & `lycoris_lora-2.3.0.dev8/lycoris/hcp/base.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/hcp/diag_oft.py` & `lycoris_lora-2.3.0.dev8/lycoris/hcp/diag_oft.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/hcp/loha.py` & `lycoris_lora-2.3.0.dev8/lycoris/hcp/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/hcp/lokr.py` & `lycoris_lora-2.3.0.dev8/lycoris/hcp/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/kohya/__init__.py` & `lycoris_lora-2.3.0.dev8/lycoris/kohya/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/kohya/model_utils.py` & `lycoris_lora-2.3.0.dev8/lycoris/kohya/model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/kohya/original_unet.py` & `lycoris_lora-2.3.0.dev8/lycoris/kohya/original_unet.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/kohya/sdxl_model_util.py` & `lycoris_lora-2.3.0.dev8/lycoris/kohya/sdxl_model_util.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/kohya/sdxl_original_unet.py` & `lycoris_lora-2.3.0.dev8/lycoris/kohya/sdxl_original_unet.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/kohya/test_hyperdream.py` & `lycoris_lora-2.3.0.dev8/lycoris/kohya/test_hyperdream.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/kohya/utils.py` & `lycoris_lora-2.3.0.dev8/lycoris/kohya/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/logging.py` & `lycoris_lora-2.3.0.dev8/lycoris/logging.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/__init__.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import torch
+import torch.nn as nn
 
 from .full import FullModule
 from .norms import NormModule
 from .locon import LoConModule
 from .loha import LohaModule
 from .lokr import LokrModule, factorization
 from .ia3 import IA3Module
@@ -118,16 +119,19 @@
     elif lyco_type == "full":
         diff, diff_b = params
         module = FullModule(
             lora_name,
             orig_module,
             1,
         )
-        module.diff.copy_(diff)
+        module.weight.copy_(diff + orig_module[0].weight.data)
         if diff_b is not None:
-            module.diff_b.copy_(diff_b)
+            if orig_module[0].bias is not None:
+                module.bias.copy_(diff_b + orig_module[0].bias.data)
+            else:
+                module.bias = nn.Parameter(diff_b)
     elif lyco_type == "ia3":
         pass
     else:
         return None
 
     return module
```

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/attention.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/attention.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/base.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/base.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/boft.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/boft.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/diag_oft.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/diag_oft.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/dylora.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/full.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/full.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/glokr.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/glokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/glora.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/glora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/hypernet/generater.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/generater.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/hypernet/text_encoder.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/hypernet/text_encoder.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/ia3.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/lilora.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/lilora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/locon.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/loha.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/lokr.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/modules/norms.py` & `lycoris_lora-2.3.0.dev8/lycoris/modules/norms.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/utils/__init__.py` & `lycoris_lora-2.3.0.dev8/lycoris/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/utils/logger.py` & `lycoris_lora-2.3.0.dev8/lycoris/utils/logger.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris/wrapper.py` & `lycoris_lora-2.3.0.dev8/lycoris/wrapper.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/lycoris_lora.egg-info/PKG-INFO` & `lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lycoris_lora
-Version: 2.3.0.dev7
+Version: 2.3.0.dev8
 Summary: Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion
 Home-page: https://github.com/KohakuBlueleaf/LyCORIS
 Author: Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao
 Author-email: apolloyeh0123@gmail.com
 Requires-Python: >=3.10
 License-File: LICENSE.md
 Requires-Dist: torch
```

### Comparing `lycoris_lora-2.3.0.dev7/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-2.3.0.dev8/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-2.3.0.dev7/setup.py` & `lycoris_lora-2.3.0.dev8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="lycoris_lora",
     packages=find_packages(),
-    version="2.3.0.dev7",
+    version="2.3.0.dev8",
     url="https://github.com/KohakuBlueleaf/LyCORIS",
     description="Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion",
     author="Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao",
     author_email="apolloyeh0123@gmail.com",
     zip_safe=False,
     install_requires=[
         "torch",
```


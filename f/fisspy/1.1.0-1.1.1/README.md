# Comparing `tmp/fisspy-1.1.0.tar.gz` & `tmp/fisspy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fisspy-1.1.0.tar", last modified: Thu May  2 00:31:40 2024, max compression
+gzip compressed data, was "fisspy-1.1.1.tar", last modified: Fri May  3 00:39:10 2024, max compression
```

## Comparing `fisspy-1.1.0.tar` & `fisspy-1.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.488764 fisspy-1.1.0/
--rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.1.0/LICENSE.txt
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-02 00:31:40.488570 fisspy-1.1.0/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.1.0/README.md
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.483226 fisspy-1.1.0/fisspy/
--rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-04-30 00:20:03.000000 fisspy-1.1.0/fisspy/__init__.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.484455 fisspy-1.1.0/fisspy/align/
--rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/align/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.1.0/fisspy/align/alignment.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.1.0/fisspy/align/base.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.485333 fisspy-1.1.0/fisspy/analysis/
--rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/analysis/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.1.0/fisspy/analysis/doppler.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/analysis/filter.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.1.0/fisspy/analysis/forecast.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/analysis/ofe.py
--rw-r--r--   0 jhkang     (501) staff       (20)    35498 2024-04-25 11:29:47.000000 fisspy-1.1.0/fisspy/analysis/tdmap.py
--rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.1.0/fisspy/analysis/wavelet.py
--rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.1.0/fisspy/cm.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.485753 fisspy-1.1.0/fisspy/correction/
--rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/correction/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-05-01 13:33:13.000000 fisspy-1.1.0/fisspy/correction/correction.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-30 00:59:33.000000 fisspy-1.1.0/fisspy/correction/get_inform.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.486181 fisspy-1.1.0/fisspy/data/
--rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.1.0/fisspy/data/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.1.0/fisspy/data/_sample.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.1.0/fisspy/data/download.py
--rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.1.0/fisspy/data/sample.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.486534 fisspy-1.1.0/fisspy/image/
--rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.1.0/fisspy/image/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    30373 2024-05-01 08:46:52.000000 fisspy-1.1.0/fisspy/image/interactive_image.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12849 2024-05-01 06:38:35.000000 fisspy-1.1.0/fisspy/image/raster_set.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.486736 fisspy-1.1.0/fisspy/inversion/
--rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/inversion/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/inversion/_mlsi.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.486970 fisspy-1.1.0/fisspy/io/
--rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.1.0/fisspy/io/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.1.0/fisspy/io/read.py
--rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/makevideo.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.487536 fisspy-1.1.0/fisspy/preprocess/
--rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/preprocess/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    52752 2024-04-27 05:54:30.000000 fisspy-1.1.0/fisspy/preprocess/proc_base.py
--rw-r--r--   0 jhkang     (501) staff       (20)   146937 2024-04-27 10:55:16.000000 fisspy-1.1.0/fisspy/preprocess/proc_gui.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/preprocess/t_y_sh.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.488274 fisspy-1.1.0/fisspy/read/
--rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/read/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    50267 2024-05-01 14:11:45.000000 fisspy-1.1.0/fisspy/read/read_factory.py
--rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.1.0/fisspy/read/readbase.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.484084 fisspy-1.1.0/fisspy.egg-info/
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/SOURCES.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/dependency_links.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/not-zip-safe
--rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/requires.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/top_level.txt
--rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-05-02 00:31:40.488810 fisspy-1.1.0/setup.cfg
--rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-04-30 00:19:57.000000 fisspy-1.1.0/setup.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.677339 fisspy-1.1.1/
+-rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.1.1/LICENSE.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-03 00:39:10.677159 fisspy-1.1.1/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.1.1/README.md
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.672242 fisspy-1.1.1/fisspy/
+-rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-05-03 00:37:44.000000 fisspy-1.1.1/fisspy/__init__.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.673250 fisspy-1.1.1/fisspy/align/
+-rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/align/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.1.1/fisspy/align/alignment.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.1.1/fisspy/align/base.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.674174 fisspy-1.1.1/fisspy/analysis/
+-rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/analysis/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.1.1/fisspy/analysis/doppler.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/analysis/filter.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.1.1/fisspy/analysis/forecast.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/analysis/ofe.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    35498 2024-04-25 11:29:47.000000 fisspy-1.1.1/fisspy/analysis/tdmap.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.1.1/fisspy/analysis/wavelet.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.1.1/fisspy/cm.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.674617 fisspy-1.1.1/fisspy/correction/
+-rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/correction/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-05-01 13:33:13.000000 fisspy-1.1.1/fisspy/correction/correction.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-30 00:59:33.000000 fisspy-1.1.1/fisspy/correction/get_inform.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.675064 fisspy-1.1.1/fisspy/data/
+-rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.1.1/fisspy/data/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.1.1/fisspy/data/_sample.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.1.1/fisspy/data/download.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.1.1/fisspy/data/sample.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.675430 fisspy-1.1.1/fisspy/image/
+-rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.1.1/fisspy/image/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    30375 2024-05-03 00:32:43.000000 fisspy-1.1.1/fisspy/image/interactive_image.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12849 2024-05-01 06:38:35.000000 fisspy-1.1.1/fisspy/image/raster_set.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.675673 fisspy-1.1.1/fisspy/inversion/
+-rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/inversion/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/inversion/_mlsi.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.675890 fisspy-1.1.1/fisspy/io/
+-rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.1.1/fisspy/io/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.1.1/fisspy/io/read.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/makevideo.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.676504 fisspy-1.1.1/fisspy/preprocess/
+-rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/preprocess/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    52752 2024-04-27 05:54:30.000000 fisspy-1.1.1/fisspy/preprocess/proc_base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)   146937 2024-04-27 10:55:16.000000 fisspy-1.1.1/fisspy/preprocess/proc_gui.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/preprocess/t_y_sh.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.676874 fisspy-1.1.1/fisspy/read/
+-rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/read/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    50267 2024-05-01 14:11:45.000000 fisspy-1.1.1/fisspy/read/read_factory.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.1.1/fisspy/read/readbase.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.672880 fisspy-1.1.1/fisspy.egg-info/
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/not-zip-safe
+-rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/requires.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/top_level.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-05-03 00:39:10.677382 fisspy-1.1.1/setup.cfg
+-rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-05-03 00:37:41.000000 fisspy-1.1.1/setup.py
```

### Comparing `fisspy-1.1.0/LICENSE.txt` & `fisspy-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/PKG-INFO` & `fisspy-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.1.0
+Version: 1.1.1
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.1.0/README.md` & `fisspy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/align/alignment.py` & `fisspy-1.1.1/fisspy/align/alignment.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/align/base.py` & `fisspy-1.1.1/fisspy/align/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/analysis/doppler.py` & `fisspy-1.1.1/fisspy/analysis/doppler.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/analysis/filter.py` & `fisspy-1.1.1/fisspy/analysis/filter.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/analysis/forecast.py` & `fisspy-1.1.1/fisspy/analysis/forecast.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/analysis/ofe.py` & `fisspy-1.1.1/fisspy/analysis/ofe.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/analysis/tdmap.py` & `fisspy-1.1.1/fisspy/analysis/tdmap.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/analysis/wavelet.py` & `fisspy-1.1.1/fisspy/analysis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/cm.py` & `fisspy-1.1.1/fisspy/cm.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/correction/correction.py` & `fisspy-1.1.1/fisspy/correction/correction.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/correction/get_inform.py` & `fisspy-1.1.1/fisspy/correction/get_inform.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/data/_sample.py` & `fisspy-1.1.1/fisspy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/data/download.py` & `fisspy-1.1.1/fisspy/data/download.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/image/interactive_image.py` & `fisspy-1.1.1/fisspy/image/interactive_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -395,15 +395,15 @@
         Default is True
 
     Other Parameters
     ----------------
     **kwargs : `~matplotlib.pyplot` properties
     """
     def __init__(self, fissA, fissB, x=None, y=None, wvA=None, wvB=None,
-                 scale='minMax', sigFactor=3, helpBox=True, **kwargs):
+                 scale='log', sigFactor=3, helpBox=True, **kwargs):
 
         try:
             plt.rcParams['keymap.back'].remove('left')
             plt.rcParams['keymap.forward'].remove('right')
         except:
             pass
         from ..align import alignOffset, shiftImage3D
@@ -414,29 +414,31 @@
         self.nwvA = self.fissA.nwv
         self.nwvB = self.fissB.nwv
         self.dx = self.fissA.xDelt
         self.dy = self.fissA.yDelt
         self.dwvA = self.fissA.wvDelt
         self.dwvB = self.fissB.wvDelt
         if self.fissA.ny >= self.fissB.ny:
-            self.fissA.data = self.fissA.data[:self.fissB.ny]
+            self.dataA = self.fissA.data[:self.fissB.ny].copy()
+            self.dataB = self.fissB.data.copy()
             self.ny = self.fissB.ny
             self.extentRaster = self.fissB.extentRaster
         elif fissA.ny < fissB.ny:
-            self.fissB.data = self.fissB.data[:self.fissA.ny]
+            self.dataB = self.fissB.data[:self.fissA.ny].copy()
+            self.dataA = self.fissA.data.copy()
             self.ny = self.fissA.ny
             self.extentRaster = self.fissA.extentRaster
         self._xMin = self.extentRaster[0]
         self._xMax = self.extentRaster[1]
         self._yMin = self.extentRaster[2]
         self._yMax = self.extentRaster[3]
 
-        sh = alignOffset(self.fissB.data[:,:,50], self.fissA.data[:,:,-50])
+        sh = alignOffset(self.dataB[:,:,50], self.dataA[:,:,-50])
         tmp = shiftImage3D(fissB.data.transpose(2, 0, 1), -sh).transpose(1,2,0)
-        self.fissB.data = tmp
+        self.dataB = tmp
         tmp[tmp<10]=1
 
         if not x:
             X = self.nx//2*self.dx
         else:
             X = x
         if not y:
@@ -515,30 +517,30 @@
         self.axProfileB.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissB.band, self.wvB))
         self.axRasterA.set_xlim(self.extentRaster[0], self.extentRaster[1])
         self.axRasterB.set_xlim(self.extentRaster[0], self.extentRaster[1])
         self.axRasterA.set_ylim(self.extentRaster[2], self.extentRaster[3])
         self.axRasterB.set_ylim(self.extentRaster[2], self.extentRaster[3])
         self.axProfileA.set_xlim(self.fissA.wave.min(), self.fissA.wave.max())
         self.axProfileB.set_xlim(self.fissB.wave.min(), self.fissB.wave.max())
-        ym = self.fissA.data[self.yp, self.xp].min()
-        yM = self.fissA.data[self.yp, self.xp].max()
+        ym = self.dataA[self.yp, self.xp].min()
+        yM = self.dataA[self.yp, self.xp].max()
         margin = (yM-ym)*0.05
         self.axProfileA.set_ylim(ym-margin, yM+margin)
-        ym = self.fissB.data[self.yp, self.xp].min()
-        yM = self.fissB.data[self.yp, self.xp].max()
+        ym = self.dataB[self.yp, self.xp].min()
+        yM = self.dataB[self.yp, self.xp].max()
         margin = (yM-ym)*0.05
         self.axProfileB.set_ylim(ym-margin, yM+margin)
         self.axProfileA.minorticks_on()
         self.axProfileA.tick_params(which='both', direction='in')
         self.axProfileB.minorticks_on()
         self.axProfileB.tick_params(which='both', direction='in')
 
         #Draw
-        rasterA = _getRaster(self.fissA.data, self.fissA.wave, self.wvA, self.dwvA, hw=self.hw)
-        rasterB = _getRaster(self.fissB.data, self.fissB.wave, self.wvB, self.dwvB, hw=self.hw)
+        rasterA = _getRaster(self.dataA, self.fissA.wave, self.wvA, self.dwvA, hw=self.hw)
+        rasterB = _getRaster(self.dataB, self.fissB.wave, self.wvB, self.dwvB, hw=self.hw)
 
         MA = rasterA.max()
         if MA > 1e2:
             mA = rasterA[rasterA > 1e2].min()
         else:
             mA = rasterA.min()
         MB = rasterB.max()
@@ -553,16 +555,16 @@
             MA = np.log10(MA)
             mA = np.log10(mA)
             MB = np.log10(MB)
             mB = np.log10(mB)
         
         self.imRasterA = self.axRasterA.imshow(rasterA, self.fissA.cmap, origin='lower', extent=self.extentRaster, **kwargs)
         self.imRasterB = self.axRasterB.imshow(rasterB, self.fissB.cmap, origin='lower', extent=self.extentRaster, **kwargs)
-        self.plotProfileA = self.axProfileA.plot(self.fissA.wave, self.fissA.data[yp, xp], color='k')[0]
-        self.plotProfileB = self.axProfileB.plot(self.fissB.wave, self.fissB.data[yp, xp], color='k')[0]
+        self.plotProfileA = self.axProfileA.plot(self.fissA.wave, self.dataA[yp, xp], color='k')[0]
+        self.plotProfileB = self.axProfileB.plot(self.fissB.wave, self.dataB[yp, xp], color='k')[0]
 
         if self.scale == 'std':
             self.imRasterA.set_clim(np.median(rasterA)-rasterA.std()*self.sigFactor, np.median(rasterA)+rasterA.std()*self.sigFactor)
             self.imRasterB.set_clim(np.median(rasterB)-rasterB.std()*self.sigFactor, np.median(rasterB)+rasterB.std()*self.sigFactor)
         else:
             self.imRasterA.set_clim(mA, MA)
             self.imRasterB.set_clim(mB, MB)
@@ -730,31 +732,31 @@
             self._chSpect()
             self.xp0 = x
             self.yp0 = y
             self.wvpA0 = wvA
             self.wvpB0 = wvB
 
     def _chSpect(self):
-        self.plotProfileA.set_ydata(self.fissA.data[self.yp, self.xp])
-        self.plotProfileB.set_ydata(self.fissB.data[self.yp, self.xp])
+        self.plotProfileA.set_ydata(self.dataA[self.yp, self.xp])
+        self.plotProfileB.set_ydata(self.dataB[self.yp, self.xp])
         self.pointRasterA.set_offsets([self.x, self.y])
         self.pointRasterB.set_offsets([self.x, self.y])
 
-        ym = self.fissA.data[self.yp, self.xp].min()
-        yM = self.fissA.data[self.yp, self.xp].max()
+        ym = self.dataA[self.yp, self.xp].min()
+        yM = self.dataA[self.yp, self.xp].max()
         margin = (yM-ym)*0.05
         self.axProfileA.set_ylim(ym-margin, yM+margin)
-        ym = self.fissB.data[self.yp, self.xp].min()
-        yM = self.fissB.data[self.yp, self.xp].max()
+        ym = self.dataB[self.yp, self.xp].min()
+        yM = self.dataB[self.yp, self.xp].max()
         margin = (yM-ym)*0.05
         self.axProfileB.set_ylim(ym-margin, yM+margin)
         self.fig.canvas.draw_idle()
 
     def _chRasterA(self):
-        rasterA = _getRaster(self.fissA.data, self.fissA.wave, self.wvA, self.fissA.wvDelt, hw=self.hw)
+        rasterA = _getRaster(self.dataA, self.fissA.wave, self.wvA, self.fissA.wvDelt, hw=self.hw)
         M = rasterA.max()
         if M > 1e2:
             m = rasterA[rasterA > 1e2].min()
         else:
             m = rasterA.min()
         if self.scale == 'log':
             rasterA = np.log10(rasterA)
@@ -766,15 +768,15 @@
         if self.scale == 'std':
             self.imRasterA.set_clim(np.median(rasterA)-rasterA.std()*self.sigFactor, np.median(rasterA)+rasterA.std()*self.sigFactor)
         else:
             self.imRasterA.set_clim(m, M)
         self.fig.canvas.draw_idle()
 
     def _chRasterB(self):
-        rasterB = _getRaster(self.fissB.data, self.fissB.wave, self.wvB, self.fissB.wvDelt, hw=self.hw)
+        rasterB = _getRaster(self.dataB, self.fissB.wave, self.wvB, self.fissB.wvDelt, hw=self.hw)
         M = rasterB.max()
         if M > 1e2:
             m = rasterB[rasterB > 1e2].min()
         else:
             m = rasterB.min()
         if self.scale == 'log':
             rasterB = np.log10(rasterB)
```

### Comparing `fisspy-1.1.0/fisspy/image/raster_set.py` & `fisspy-1.1.1/fisspy/image/raster_set.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/io/read.py` & `fisspy-1.1.1/fisspy/io/read.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/makevideo.py` & `fisspy-1.1.1/fisspy/makevideo.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/preprocess/proc_base.py` & `fisspy-1.1.1/fisspy/preprocess/proc_base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/preprocess/proc_gui.py` & `fisspy-1.1.1/fisspy/preprocess/proc_gui.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/preprocess/t_y_sh.py` & `fisspy-1.1.1/fisspy/preprocess/t_y_sh.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/read/read_factory.py` & `fisspy-1.1.1/fisspy/read/read_factory.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy/read/readbase.py` & `fisspy-1.1.1/fisspy/read/readbase.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/fisspy.egg-info/PKG-INFO` & `fisspy-1.1.1/fisspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.1.0
+Version: 1.1.1
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.1.0/fisspy.egg-info/SOURCES.txt` & `fisspy-1.1.1/fisspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.0/setup.py` & `fisspy-1.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fisspy',
-    version='1.1.0',
+    version='1.1.1',
     description='fisspy: Python analysis tools for GST/FISS',
     url='http://fiss.snu.ac.kr',
     author='Juhyung Kang',
     author_email='jhkang@astro.snu.ac.kr',
     license='BSD-2',
     python_requires='>=3.6',
     packages=find_packages(exclude=['docs', 'logo']),
```


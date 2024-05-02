# Comparing `tmp/ml4xcube-0.0.3.tar.gz` & `tmp/ml4xcube-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml4xcube-0.0.3.tar", last modified: Thu May  2 18:04:55 2024, max compression
+gzip compressed data, was "ml4xcube-0.0.4.tar", last modified: Thu May  2 18:17:59 2024, max compression
```

## Comparing `ml4xcube-0.0.3.tar` & `ml4xcube-0.0.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/
--rw-rw-r--   0 julia     (1000) julia     (1000)     1113 2024-04-23 08:43:03.000000 ml4xcube-0.0.3/LICENSE
--rw-rw-r--   0 julia     (1000) julia     (1000)       33 2024-04-23 08:43:03.000000 ml4xcube-0.0.3/MANIFEST.in
--rw-r--r--   0 julia     (1000) julia     (1000)     3628 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/PKG-INFO
--rw-rw-r--   0 julia     (1000) julia     (1000)     1643 2024-05-02 18:02:31.000000 ml4xcube-0.0.3/README.md
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.995138 ml4xcube-0.0.3/mltools/
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-04-23 11:53:26.000000 ml4xcube-0.0.3/mltools/ml4xcube/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     5544 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/cube_utilities.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2378 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/data_assignment.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube/datasets/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-02 10:14:25.000000 ml4xcube-0.0.3/mltools/ml4xcube/datasets/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2765 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/datasets/pytorch_xr.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4292 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/datasets/tensorflow_xr.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4242 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/datasets/xr_dataset.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:35:17.000000 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    14356 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/gap_dataset.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    31651 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/gap_filling.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/helper/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:36:00.000000 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/helper/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4441 2024-05-01 14:21:50.000000 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/helper/lcc.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2365 2024-05-01 13:43:43.000000 ml4xcube-0.0.3/mltools/ml4xcube/geo_plots.py
--rw-rw-r--   0 julia     (1000) julia     (1000)      389 2024-05-01 13:43:43.000000 ml4xcube-0.0.3/mltools/ml4xcube/preprocessing.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     1384 2024-05-01 14:33:44.000000 ml4xcube-0.0.3/mltools/ml4xcube/statistics.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube/training/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:23:29.000000 ml4xcube-0.0.3/mltools/ml4xcube/training/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4560 2024-05-01 13:43:43.000000 ml4xcube-0.0.3/mltools/ml4xcube/training/pytorch.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     8840 2024-05-01 14:01:45.000000 ml4xcube-0.0.3/mltools/ml4xcube/training/pytorch_distributed.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     3776 2024-05-02 11:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube/training/sklearn.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2946 2024-05-01 13:43:43.000000 ml4xcube-0.0.3/mltools/ml4xcube/training/tensorflow.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/
--rw-r--r--   0 julia     (1000) julia     (1000)     3628 2024-05-02 18:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/PKG-INFO
--rw-rw-r--   0 julia     (1000) julia     (1000)     1036 2024-05-02 18:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/SOURCES.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)        1 2024-05-02 18:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/dependency_links.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)      169 2024-05-02 18:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/requires.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)        9 2024-05-02 18:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/top_level.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)      561 2024-05-02 17:57:36.000000 ml4xcube-0.0.3/pyproject.toml
--rw-rw-r--   0 julia     (1000) julia     (1000)       38 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/setup.cfg
--rw-rw-r--   0 julia     (1000) julia     (1000)      514 2024-05-02 17:57:26.000000 ml4xcube-0.0.3/setup.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:17:59.697388 ml4xcube-0.0.4/
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1113 2024-04-23 08:43:03.000000 ml4xcube-0.0.4/LICENSE
+-rw-rw-r--   0 julia     (1000) julia     (1000)       70 2024-05-02 18:14:05.000000 ml4xcube-0.0.4/MANIFEST.in
+-rw-r--r--   0 julia     (1000) julia     (1000)     3628 2024-05-02 18:17:59.697388 ml4xcube-0.0.4/PKG-INFO
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1643 2024-05-02 18:02:31.000000 ml4xcube-0.0.4/README.md
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:17:59.689388 ml4xcube-0.0.4/mltools/
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:17:59.689388 ml4xcube-0.0.4/mltools/ml4xcube/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-04-23 11:53:26.000000 ml4xcube-0.0.4/mltools/ml4xcube/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     5544 2024-05-02 16:06:56.000000 ml4xcube-0.0.4/mltools/ml4xcube/cube_utilities.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2378 2024-05-02 16:06:56.000000 ml4xcube-0.0.4/mltools/ml4xcube/data_assignment.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:17:59.689388 ml4xcube-0.0.4/mltools/ml4xcube/datasets/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-02 10:14:25.000000 ml4xcube-0.0.4/mltools/ml4xcube/datasets/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2765 2024-05-02 16:06:56.000000 ml4xcube-0.0.4/mltools/ml4xcube/datasets/pytorch_xr.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4292 2024-05-02 16:06:56.000000 ml4xcube-0.0.4/mltools/ml4xcube/datasets/tensorflow_xr.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4242 2024-05-02 16:06:56.000000 ml4xcube-0.0.4/mltools/ml4xcube/datasets/xr_dataset.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:17:59.689388 ml4xcube-0.0.4/mltools/ml4xcube/gapfilling/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:35:17.000000 ml4xcube-0.0.4/mltools/ml4xcube/gapfilling/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    14356 2024-05-02 16:06:56.000000 ml4xcube-0.0.4/mltools/ml4xcube/gapfilling/gap_dataset.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    31651 2024-05-02 16:06:56.000000 ml4xcube-0.0.4/mltools/ml4xcube/gapfilling/gap_filling.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:17:59.697388 ml4xcube-0.0.4/mltools/ml4xcube/gapfilling/helper/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:36:00.000000 ml4xcube-0.0.4/mltools/ml4xcube/gapfilling/helper/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)  9401362 2024-04-23 11:53:26.000000 ml4xcube-0.0.4/mltools/ml4xcube/gapfilling/helper/global_lcc.nc
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4441 2024-05-01 14:21:50.000000 ml4xcube-0.0.4/mltools/ml4xcube/gapfilling/helper/lcc.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2365 2024-05-01 13:43:43.000000 ml4xcube-0.0.4/mltools/ml4xcube/geo_plots.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)      389 2024-05-01 13:43:43.000000 ml4xcube-0.0.4/mltools/ml4xcube/preprocessing.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1384 2024-05-01 14:33:44.000000 ml4xcube-0.0.4/mltools/ml4xcube/statistics.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:17:59.697388 ml4xcube-0.0.4/mltools/ml4xcube/training/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:23:29.000000 ml4xcube-0.0.4/mltools/ml4xcube/training/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4560 2024-05-01 13:43:43.000000 ml4xcube-0.0.4/mltools/ml4xcube/training/pytorch.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     8840 2024-05-01 14:01:45.000000 ml4xcube-0.0.4/mltools/ml4xcube/training/pytorch_distributed.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     3776 2024-05-02 11:04:54.000000 ml4xcube-0.0.4/mltools/ml4xcube/training/sklearn.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2946 2024-05-01 13:43:43.000000 ml4xcube-0.0.4/mltools/ml4xcube/training/tensorflow.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:17:59.697388 ml4xcube-0.0.4/mltools/ml4xcube.egg-info/
+-rw-r--r--   0 julia     (1000) julia     (1000)     3628 2024-05-02 18:17:59.000000 ml4xcube-0.0.4/mltools/ml4xcube.egg-info/PKG-INFO
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1085 2024-05-02 18:17:59.000000 ml4xcube-0.0.4/mltools/ml4xcube.egg-info/SOURCES.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)        1 2024-05-02 18:17:59.000000 ml4xcube-0.0.4/mltools/ml4xcube.egg-info/dependency_links.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)      169 2024-05-02 18:17:59.000000 ml4xcube-0.0.4/mltools/ml4xcube.egg-info/requires.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)        9 2024-05-02 18:17:59.000000 ml4xcube-0.0.4/mltools/ml4xcube.egg-info/top_level.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)      628 2024-05-02 18:16:40.000000 ml4xcube-0.0.4/pyproject.toml
+-rw-rw-r--   0 julia     (1000) julia     (1000)       38 2024-05-02 18:17:59.697388 ml4xcube-0.0.4/setup.cfg
+-rw-rw-r--   0 julia     (1000) julia     (1000)      636 2024-05-02 18:13:34.000000 ml4xcube-0.0.4/setup.py
```

### Comparing `ml4xcube-0.0.3/LICENSE` & `ml4xcube-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/PKG-INFO` & `ml4xcube-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4xcube
-Version: 0.0.3
+Version: 0.0.4
 Summary: ML package for data cubes
 Author-email: Julia Peters <julia.peters@informatik.uni-leipzig.de>
 License: MIT License
         
         Copyright (c) 2022 by ScaDS.AI, the xcube development team and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ml4xcube-0.0.3/README.md` & `ml4xcube-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/cube_utilities.py` & `ml4xcube-0.0.4/mltools/ml4xcube/cube_utilities.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/data_assignment.py` & `ml4xcube-0.0.4/mltools/ml4xcube/data_assignment.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/datasets/pytorch_xr.py` & `ml4xcube-0.0.4/mltools/ml4xcube/datasets/pytorch_xr.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/datasets/tensorflow_xr.py` & `ml4xcube-0.0.4/mltools/ml4xcube/datasets/tensorflow_xr.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/datasets/xr_dataset.py` & `ml4xcube-0.0.4/mltools/ml4xcube/datasets/xr_dataset.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/gap_dataset.py` & `ml4xcube-0.0.4/mltools/ml4xcube/gapfilling/gap_dataset.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/gap_filling.py` & `ml4xcube-0.0.4/mltools/ml4xcube/gapfilling/gap_filling.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/helper/lcc.py` & `ml4xcube-0.0.4/mltools/ml4xcube/gapfilling/helper/lcc.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/geo_plots.py` & `ml4xcube-0.0.4/mltools/ml4xcube/geo_plots.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/statistics.py` & `ml4xcube-0.0.4/mltools/ml4xcube/statistics.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/training/pytorch.py` & `ml4xcube-0.0.4/mltools/ml4xcube/training/pytorch.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/training/pytorch_distributed.py` & `ml4xcube-0.0.4/mltools/ml4xcube/training/pytorch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/training/sklearn.py` & `ml4xcube-0.0.4/mltools/ml4xcube/training/sklearn.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube/training/tensorflow.py` & `ml4xcube-0.0.4/mltools/ml4xcube/training/tensorflow.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube.egg-info/PKG-INFO` & `ml4xcube-0.0.4/mltools/ml4xcube.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4xcube
-Version: 0.0.3
+Version: 0.0.4
 Summary: ML package for data cubes
 Author-email: Julia Peters <julia.peters@informatik.uni-leipzig.de>
 License: MIT License
         
         Copyright (c) 2022 by ScaDS.AI, the xcube development team and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ml4xcube-0.0.3/mltools/ml4xcube.egg-info/SOURCES.txt` & `ml4xcube-0.0.4/mltools/ml4xcube.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,13 +19,14 @@
 mltools/ml4xcube/datasets/pytorch_xr.py
 mltools/ml4xcube/datasets/tensorflow_xr.py
 mltools/ml4xcube/datasets/xr_dataset.py
 mltools/ml4xcube/gapfilling/__init__.py
 mltools/ml4xcube/gapfilling/gap_dataset.py
 mltools/ml4xcube/gapfilling/gap_filling.py
 mltools/ml4xcube/gapfilling/helper/__init__.py
+mltools/ml4xcube/gapfilling/helper/global_lcc.nc
 mltools/ml4xcube/gapfilling/helper/lcc.py
 mltools/ml4xcube/training/__init__.py
 mltools/ml4xcube/training/pytorch.py
 mltools/ml4xcube/training/pytorch_distributed.py
 mltools/ml4xcube/training/sklearn.py
 mltools/ml4xcube/training/tensorflow.py
```


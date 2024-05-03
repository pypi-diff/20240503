# Comparing `tmp/mapreader-1.3.0.tar.gz` & `tmp/mapreader-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapreader-1.3.0.tar", last modified: Mon Apr 29 15:18:33 2024, max compression
+gzip compressed data, was "mapreader-1.3.1.tar", last modified: Fri May  3 12:44:12 2024, max compression
```

## Comparing `mapreader-1.3.0.tar` & `mapreader-1.3.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.779410 mapreader-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-29 15:18:26.000000 mapreader-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-04-29 15:18:33.779410 mapreader-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-04-29 15:18:26.000000 mapreader-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.779410 mapreader-1.3.0/mapreader/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 15:18:33.779410 mapreader-1.3.0/mapreader/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.771410 mapreader-1.3.0/mapreader/annotate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34533 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/annotate/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    26473 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/annotate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.771410 mapreader-1.3.0/mapreader/classify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75056 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/classify/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/classify/custom_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/classify/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    31931 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/classify/load_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.771410 mapreader-1.3.0/mapreader/download/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46716 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/tile_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/tile_merging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/mapreader/load/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/load/geo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    98834 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/load/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/load/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/mapreader/process/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/process/post_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/process/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/mapreader/spot_text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/spot_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/spot_text/deepsolo_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/spot_text/dptext_detr_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/mapreader/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/utils/compute_and_save_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/utils/slice_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/mapreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-29 15:18:33.779410 mapreader-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-29 15:18:26.000000 mapreader-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-29 15:18:26.000000 mapreader-1.3.0/tests/test_annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-29 15:18:26.000000 mapreader-1.3.0/tests/test_geo_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-29 15:18:26.000000 mapreader-1.3.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-29 15:18:26.000000 mapreader-1.3.0/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    22537 2024-04-29 15:18:26.000000 mapreader-1.3.0/tests/test_sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    83834 2024-04-29 15:18:26.000000 mapreader-1.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:12.155579 mapreader-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-03 12:44:04.000000 mapreader-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-05-03 12:44:12.155579 mapreader-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-05-03 12:44:04.000000 mapreader-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:12.155579 mapreader-1.3.1/mapreader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-03 12:44:12.155579 mapreader-1.3.1/mapreader/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:12.147579 mapreader-1.3.1/mapreader/annotate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34533 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/annotate/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26473 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/annotate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:12.147579 mapreader-1.3.1/mapreader/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75056 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/classify/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/classify/custom_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/classify/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31931 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/classify/load_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:12.147579 mapreader-1.3.1/mapreader/download/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/download/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/download/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48381 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/download/sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/download/tile_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/download/tile_merging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:12.151579 mapreader-1.3.1/mapreader/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/load/geo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98834 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/load/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/load/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:12.151579 mapreader-1.3.1/mapreader/process/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/process/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/process/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:12.151579 mapreader-1.3.1/mapreader/spot_text/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/spot_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/spot_text/deepsolo_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/spot_text/dptext_detr_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:12.151579 mapreader-1.3.1/mapreader/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/utils/compute_and_save_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-03 12:44:04.000000 mapreader-1.3.1/mapreader/utils/slice_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:12.151579 mapreader-1.3.1/mapreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-05-03 12:44:12.000000 mapreader-1.3.1/mapreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-03 12:44:12.000000 mapreader-1.3.1/mapreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:44:12.000000 mapreader-1.3.1/mapreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 12:44:12.000000 mapreader-1.3.1/mapreader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:44:11.000000 mapreader-1.3.1/mapreader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-03 12:44:12.000000 mapreader-1.3.1/mapreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 12:44:12.000000 mapreader-1.3.1/mapreader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-03 12:44:12.155579 mapreader-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-03 12:44:04.000000 mapreader-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:44:12.151579 mapreader-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-03 12:44:05.000000 mapreader-1.3.1/tests/test_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-03 12:44:05.000000 mapreader-1.3.1/tests/test_geo_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-03 12:44:05.000000 mapreader-1.3.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-03 12:44:05.000000 mapreader-1.3.1/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26481 2024-05-03 12:44:05.000000 mapreader-1.3.1/tests/test_sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83834 2024-05-03 12:44:05.000000 mapreader-1.3.1/versioneer.py
```

### Comparing `mapreader-1.3.0/LICENSE` & `mapreader-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/PKG-INFO` & `mapreader-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.3.0
+Version: 1.3.1
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.3.0 Summary: A computer vision
+Metadata-Version: 2.1 Name: mapreader Version: 1.3.1 Summary: A computer vision
 pipeline for the semantic exploration of maps/images at scale Home-page: https:
 //github.com/Living-with-machines/MapReader Download-URL: https://github.com/
 Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
 team License: MIT License Keywords: Computer Vision,Classification,Deep
 Learning,living with machines Platform: OS Independent Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

### Comparing `mapreader-1.3.0/README.md` & `mapreader-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/__init__.py` & `mapreader-1.3.1/mapreader/__init__.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/annotate/annotator.py` & `mapreader-1.3.1/mapreader/annotate/annotator.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/annotate/utils.py` & `mapreader-1.3.1/mapreader/annotate/utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/classify/classifier.py` & `mapreader-1.3.1/mapreader/classify/classifier.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/classify/custom_models.py` & `mapreader-1.3.1/mapreader/classify/custom_models.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/classify/datasets.py` & `mapreader-1.3.1/mapreader/classify/datasets.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/classify/load_annotations.py` & `mapreader-1.3.1/mapreader/classify/load_annotations.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/download/data_structures.py` & `mapreader-1.3.1/mapreader/download/data_structures.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/download/downloader.py` & `mapreader-1.3.1/mapreader/download/downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/download/downloader_utils.py` & `mapreader-1.3.1/mapreader/download/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/download/sheet_downloader.py` & `mapreader-1.3.1/mapreader/download/sheet_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -529,83 +529,121 @@
         Parameters
         ----------
         path_save : str
             Path to save merged items (i.e. whole map sheets)
         """
         self.merger = TileMerger(output_folder=f"{path_save}/")
 
-    def _check_map_sheet_exists(self, feature: dict) -> bool:
+    def _check_map_sheet_exists(self, feature: dict, metadata_fname) -> bool:
         """
         Checks if a map sheet is already saved.
 
         Parameters
         ----------
         feature : dict
 
         Returns
         -------
         bool
-            True if file exists, False if not.
+            img_path if file exists, False if not.
         """
-        map_name = str("map_" + feature["properties"]["IMAGE"])
         path_save = self.merger.output_folder
-        if os.path.exists(f"{path_save}{map_name}.png"):
+
+        try:
+            # get image id with same coords in metadata
+            existing_metadata_df = pd.read_csv(
+                f"{path_save}{metadata_fname}", sep=",", index_col=0
+            )
+        except FileNotFoundError:
+            return False
+
+        polygon = get_polygon_from_grid_bb(feature["grid_bb"])
+        if str(polygon.bounds) in existing_metadata_df["coordinates"].values:
+            image_id = existing_metadata_df[
+                existing_metadata_df["coordinates"] == str(polygon.bounds)
+            ].iloc[0]["name"]
+        else:
+            return False  # coordinates not in metadata means image doesn't exist
+
+        if os.path.exists(f"{path_save}{image_id}"):
             try:
-                mpimg.imread(f"{path_save}{map_name}.png")
-                print(
-                    f'[INFO] "{path_save}{map_name}.png" already exists. Skipping download.'
-                )
-                return True
+                # check image is valid
+                mpimg.imread(f"{path_save}{image_id}")
+                return image_id
             except OSError:
                 return False
         return False
 
-    def _download_map(self, feature: dict, download_in_parallel: bool = True) -> bool:
+    def _download_map(
+        self,
+        feature: dict,
+        existing_id: str | bool,
+        download_in_parallel: bool = True,
+        overwrite: bool = False,
+    ) -> str | bool:
         """
         Downloads a single map sheet and saves as png file.
 
         Parameters
         ----------
         feature : dict
+            The feature for which to download the map sheet.
+        existing_id : str | bool
+            The existing image id if the map sheet already exists.
+        download_in_parallel : bool, optional
+            Whether to download tiles in parallel, by default ``True``.
+        overwrite : bool, optional
+            Whether to overwrite existing maps, by default ``False``.
 
         Returns
         -------
-        bool
-            True if map was downloaded successfully, False if not.
+        str or bool
+            image path if map was downloaded successfully, False if not.
         """
-        map_name = str("map_" + feature["properties"]["IMAGE"])
         self.downloader.download_tiles(
             feature["grid_bb"], download_in_parallel=download_in_parallel
         )
-        success = self.merger.merge(feature["grid_bb"], map_name)
-        if success:
-            print(f'[INFO] Downloaded "{map_name}.png"')
+
+        if existing_id is False:
+            map_name = f"map_{feature['properties']['IMAGE']}"
+        else:
+            map_name = existing_id[:-4]  # remove file extension (assuming .png)
+
+        img_path = self.merger.merge(
+            feature["grid_bb"], file_name=map_name, overwrite=overwrite
+        )
+
+        if img_path is not False:
+            print(f'[INFO] Downloaded "{img_path}"')
         else:
-            print(f'[WARNING] Download of "{map_name}.png" was unsuccessful.')
+            print(f'[WARNING] Download of "{img_path}" was unsuccessful.')
 
         shutil.rmtree(DEFAULT_TEMP_FOLDER)
-        return success
+        return img_path
 
     def _save_metadata(
         self,
         feature: dict,
         out_filepath: str,
+        img_path: str,
         metadata_to_save: dict | None = None,
         **kwargs: dict | None,
     ) -> None:
         """
         Creates list of selected metadata items and saves to a csv file.
         If file exists, metadata list is appended.
 
         Parameters
         ----------
         feature : dict
             The feature for which to extract the metadata from
         out_filepath : str
             The path to save metadata csv.
+        img_path : str
+            The path to the downloaded map sheet.
         metadata_to_save : dict, optional
             A dictionary containing column names (str) and metadata keys (str or list) to save to metadata csv.
             Multilayer keys should be passed as a list, i.e. ["key1","key2"] will search for ``self.features[i]["key1"]["key2"]``.
 
             e.g. ``{"county": ["properties", "COUNTY"], "id": "id"}``
         **kwargs: dict, optional
             Keyword arguments to pass to the ``extract_published_dates()`` method.
@@ -627,15 +665,15 @@
             "crs",
             "published_date",
             "grid_bb",
         ]
         metadata_dict = {col: None for col in metadata_cols}
 
         # get default metadata
-        metadata_dict["name"] = str("map_" + feature["properties"]["IMAGE"] + ".png")
+        metadata_dict["name"] = os.path.basename(img_path)
         metadata_dict["url"] = str(feature["properties"]["IMAGEURL"])
         if not self.published_dates:
             date_col = kwargs.get("date_col", None)
             self.extract_published_dates(date_col=date_col)
         metadata_dict["published_date"] = feature["properties"]["published_date"]
         metadata_dict["grid_bb"] = feature["grid_bb"]
         polygon = get_polygon_from_grid_bb(
@@ -701,24 +739,33 @@
         download_in_parallel : bool, optional
             Whether to download tiles in parallel, by default ``True``.
         **kwargs : dict, optional
             Keyword arguments to pass to the ``_save_metadata()`` method.
         """
 
         for feature in tqdm(features):
-            if not overwrite:
-                if self._check_map_sheet_exists(feature):
-                    continue
-            success = self._download_map(
-                feature, download_in_parallel=download_in_parallel
+            existing_id = self._check_map_sheet_exists(feature, metadata_fname)
+            if (
+                not overwrite and existing_id is not False
+            ):  # if map already exists and overwrite is False then skip
+                print(f'[INFO] "{existing_id}" already exists. Skipping download.')
+                continue
+            img_path = self._download_map(
+                feature,
+                existing_id,
+                download_in_parallel=download_in_parallel,
+                overwrite=overwrite,
             )
-            if success:
+            if img_path is not False:
                 metadata_path = f"{path_save}/{metadata_fname}"
                 self._save_metadata(
-                    feature=feature, out_filepath=metadata_path, **kwargs
+                    feature=feature,
+                    out_filepath=metadata_path,
+                    img_path=img_path,
+                    **kwargs,
                 )
 
     def download_all_map_sheets(
         self,
         path_save: str | None = "maps",
         metadata_fname: str | None = "metadata.csv",
         overwrite: bool | None = False,
```

### Comparing `mapreader-1.3.0/mapreader/download/tile_loading.py` & `mapreader-1.3.1/mapreader/download/tile_loading.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/download/tile_merging.py` & `mapreader-1.3.1/mapreader/download/tile_merging.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,28 +138,35 @@
         img_size = start_image.size
         assert (
             img_size[0] == img_size[1]
         ), f"Tiles must be quadratic. This tile, however, is rectangular: {img_size}"
         tile_size = img_size[0]
         return tile_size
 
-    def merge(self, grid_bb: GridBoundingBox, file_name: str | None = None) -> bool:
+    def merge(
+        self,
+        grid_bb: GridBoundingBox,
+        file_name: str | None = None,
+        overwrite: bool = False,
+    ) -> str | bool:
         """Merges cells contained within GridBoundingBox.
 
         Parameters
         ----------
         grid_bb : GridBoundingBox
             GridBoundingBox containing tiles to merge
         file_name : Union[str, None], optional
             Name to use when saving map
-
+            If None, default name will be used, by default None
+        overwrite : bool, optional
+            Whether or not to overwrite existing files, by default False
         Returns
         -------
-        bool
-            True if file has successfully downloaded, False if not.
+        str or bool
+            out path if file has successfully downloaded, False if not.
         """
         os.makedirs(self.output_folder, exist_ok=True)
 
         try:
             tile_size = self._load_tile_size(grid_bb)
         except FileNotFoundError:
             return False  # unsuccessful
@@ -187,15 +194,22 @@
 
         logger.info("Writing file..")
 
         if file_name is None:
             file_name = self._get_output_name(grid_bb)
 
         out_path = f"{self.output_folder}{file_name}.{self.img_output_format[0]}"
+        if not overwrite:
+            i = 1
+            while os.path.exists(out_path):
+                out_path = (
+                    f"{self.output_folder}{file_name}_{i}.{self.img_output_format[0]}"
+                )
+                i += 1
         merged_image.save(out_path, self.img_output_format[1])
-        success = True if os.path.exists(out_path) else False
-        if success:
-            logger.info(f"Merge successful! The image has been stored at '{out_path}'")
-        else:
+        success = out_path if os.path.exists(out_path) else False
+        if success is False:
             logger.warning(f"Merge unsuccessful! '{out_path}' not saved.")
+        else:
+            logger.info(f"Merge successful! The image has been stored at '{out_path}'")
 
         return success
```

### Comparing `mapreader-1.3.0/mapreader/load/geo_utils.py` & `mapreader-1.3.1/mapreader/load/geo_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/load/images.py` & `mapreader-1.3.1/mapreader/load/images.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/load/loader.py` & `mapreader-1.3.1/mapreader/load/loader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/process/post_process.py` & `mapreader-1.3.1/mapreader/process/post_process.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/process/process.py` & `mapreader-1.3.1/mapreader/process/process.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/spot_text/deepsolo_runner.py` & `mapreader-1.3.1/mapreader/spot_text/deepsolo_runner.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/spot_text/dptext_detr_runner.py` & `mapreader-1.3.1/mapreader/spot_text/dptext_detr_runner.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/utils/compute_and_save_stats.py` & `mapreader-1.3.1/mapreader/utils/compute_and_save_stats.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader/utils/slice_parallel.py` & `mapreader-1.3.1/mapreader/utils/slice_parallel.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader.egg-info/PKG-INFO` & `mapreader-1.3.1/mapreader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.3.0
+Version: 1.3.1
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.3.0 Summary: A computer vision
+Metadata-Version: 2.1 Name: mapreader Version: 1.3.1 Summary: A computer vision
 pipeline for the semantic exploration of maps/images at scale Home-page: https:
 //github.com/Living-with-machines/MapReader Download-URL: https://github.com/
 Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
 team License: MIT License Keywords: Computer Vision,Classification,Deep
 Learning,living with machines Platform: OS Independent Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

### Comparing `mapreader-1.3.0/mapreader.egg-info/SOURCES.txt` & `mapreader-1.3.1/mapreader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/mapreader.egg-info/requires.txt` & `mapreader-1.3.1/mapreader.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/setup.py` & `mapreader-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/tests/test_annotator.py` & `mapreader-1.3.1/tests/test_annotator.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/tests/test_geo_pipeline.py` & `mapreader-1.3.1/tests/test_geo_pipeline.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/tests/test_post_processing.py` & `mapreader-1.3.1/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.3.0/tests/test_sheet_downloader.py` & `mapreader-1.3.1/tests/test_sheet_downloader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from __future__ import annotations
 
 import os
+import re
 from ast import literal_eval
 from pathlib import Path
 
 import pandas as pd
 import pytest
+from PIL import Image
 from pytest import approx
 from shapely.geometry import LineString, MultiPolygon, Polygon
 
 from mapreader import SheetDownloader
 from mapreader.download.data_structures import GridBoundingBox
+from mapreader.download.tile_loading import TileDownloader
+from mapreader.download.tile_merging import TileMerger
 
 
 @pytest.fixture
 def sample_dir():
     return Path(__file__).resolve().parent / "sample_files"
 
 
 @pytest.fixture
 def sheet_downloader(sample_dir):
-    test_json = f"{sample_dir}/test_json.json"  # contains 4 features
+    test_json = f"{sample_dir}/test_json.json"  # contains 6 features
     download_url = "https://geo.nls.uk/maps/os/1inch_2nd_ed/{z}/{x}/{y}.png"
     return SheetDownloader(test_json, download_url)
 
 
 def test_init(sheet_downloader):
     sd = sheet_downloader
-    assert len(sd) == 4
+    assert len(sd) == 6
     assert sd.crs == "EPSG:4326"
 
 
 def test_init_errors(sample_dir):
     test_json = f"{sample_dir}/test_json.json"  # crs changed to EPSG:3857 (note: coordinates are wrong in file)
     download_url = "https://geo.nls.uk/maps/os/1inch_2nd_ed/{z}/{x}/{y}.png"
     with pytest.raises(ValueError, match="file not found"):
@@ -117,15 +121,15 @@
 
 def test_get_minmax_latlon(sheet_downloader, capfd):
     sd = sheet_downloader
     sd.get_minmax_latlon()
     out, _ = capfd.readouterr()
     assert (
         out
-        == "[INFO] Min lat: 51.49344796, max lat: 54.2089733 \n[INFO] Min lon: -2.62837527, max lon: -0.16093917\n"
+        == "[INFO] Min lat: 51.49344796, max lat: 54.2089733 \n[INFO] Min lon: -4.7682, max lon: -0.16093917\n"
     )
 
 
 # queries
 
 
 def test_query_by_wfs_ids(sheet_downloader):
@@ -276,110 +280,162 @@
     with pytest.raises(KeyError, match="not found in features dictionary"):
         sd.query_map_sheets_by_string("Nottinghamshire", ["fake_key"])
 
 
 # download
 
 
-def test_download_all(sheet_downloader, tmp_path):
+@pytest.fixture(scope="function")
+def mock_response(monkeypatch):
+    def mock_download_tiles(self, *args, **kwargs):
+        os.makedirs(self.temp_folder, exist_ok=True)
+        return
+
+    monkeypatch.setattr(TileDownloader, "download_tiles", mock_download_tiles)
+
+    def mock_merge(self, *args, **kwargs):
+        os.makedirs(self.output_folder, exist_ok=True)
+
+        merged_image = Image.new("RGBA", (10, 10))
+
+        if kwargs["file_name"] is None:
+            file_name = self._get_output_name(kwargs["grid_bb"])
+        else:
+            file_name = kwargs["file_name"]
+
+        out_path = f"{self.output_folder}{file_name}.{self.img_output_format[0]}"
+        if not kwargs["overwrite"]:
+            i = 1
+            while os.path.exists(out_path):
+                out_path = (
+                    f"{self.output_folder}{file_name}_{i}.{self.img_output_format[0]}"
+                )
+                i += 1
+        merged_image.save(out_path, self.img_output_format[1])
+        return out_path
+
+    monkeypatch.setattr(TileMerger, "merge", mock_merge)
+
+
+def test_download_all(sheet_downloader, tmp_path, mock_response):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
-    assert sd.grid_bbs is True
-    maps_path = tmp_path / "test_maps/"
+    # zoom level 14
+    sd.get_grid_bb(14)
+    maps_path = tmp_path / "test_maps_14/"
     metadata_fname = "test_metadata.csv"
     sd.download_all_map_sheets(maps_path, metadata_fname)
     assert os.path.exists(f"{maps_path}/map_102352861.png")
     assert os.path.exists(f"{maps_path}/{metadata_fname}")
     df = pd.read_csv(f"{maps_path}/{metadata_fname}", sep=",", index_col=0)
-    assert len(df) == 4
+    assert len(df) == 6
     assert list(df.columns) == [
         "name",
         "url",
         "coordinates",
         "crs",
         "published_date",
         "grid_bb",
     ]
-    assert list(df["name"]) == [
-        "map_101602026.png",
-        "map_101602038.png",
-        "map_102352861.png",
-        "map_91617032.png",
-    ]
+    assert all(
+        name in list(df["name"])
+        for name in [
+            "map_101602026.png",
+            "map_101602038.png",
+            "map_102352861.png",
+            "map_91617032.png",
+            "map_101603986.png",
+            "map_101603986_1.png",
+        ]
+    )
     # test coords
     assert literal_eval(df.loc[0, "coordinates"]) == approx(
-        (-1.0546875, 53.33087298301705, -0.703125, 53.54030739150021), rel=1e-6
+        (-0.98876953125, 53.448806835427575, -0.90087890625, 53.48804553605621),
+        rel=1e-6,
     )
-
-    sd.get_grid_bb(14)
-    maps_path = tmp_path / "test_maps_14/"
+    # zoom level 17
+    sd.get_grid_bb(17)
+    assert sd.grid_bbs is True
+    maps_path = tmp_path / "test_maps_17/"
     metadata_fname = "test_metadata.csv"
     sd.download_all_map_sheets(maps_path, metadata_fname)
     assert os.path.exists(f"{maps_path}/map_102352861.png")
     assert os.path.exists(f"{maps_path}/{metadata_fname}")
     df = pd.read_csv(f"{maps_path}/{metadata_fname}", sep=",", index_col=0)
-    assert len(df) == 4
+    assert len(df) == 6
     assert list(df.columns) == [
         "name",
         "url",
         "coordinates",
         "crs",
         "published_date",
         "grid_bb",
     ]
-    assert list(df["name"]) == [
-        "map_101602026.png",
-        "map_101602038.png",
-        "map_102352861.png",
-        "map_91617032.png",
-    ]
-    # test coords
-    assert literal_eval(df.loc[0, "coordinates"]) == approx(
-        (-0.98876953125, 53.448806835427575, -0.90087890625, 53.48804553605621),
-        rel=1e-6,
+    print(list(df["name"]))
+    assert all(
+        name in list(df["name"])
+        for name in [
+            "map_101602026.png",
+            "map_101602038.png",
+            "map_102352861.png",
+            "map_91617032.png",
+            "map_101603986.png",
+            "map_101603986_1.png",
+        ]
     )
 
 
 def test_download_all_kwargs(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
-    maps_path = tmp_path / "test_maps/"
+    # zoom level 14
+    sd.get_grid_bb(14)
+    maps_path = tmp_path / "test_maps_14/"
     metadata_fname = "test_metadata.csv"
     kwargs = {
         "metadata_to_save": {"test1": ["properties", "test"], "test2": "id"},
         "date_col": "test_date",
     }
     sd.download_all_map_sheets(maps_path, metadata_fname, **kwargs)
+    assert os.path.exists(f"{maps_path}/map_102352861.png")
     assert os.path.exists(f"{maps_path}/{metadata_fname}")
     df = pd.read_csv(f"{maps_path}/{metadata_fname}", sep=",", index_col=0)
-    assert len(df) == 4
+    assert len(df) == 6
     assert list(df.columns) == [
         "name",
         "url",
         "coordinates",
         "crs",
         "published_date",
         "grid_bb",
         "test1",
         "test2",
     ]
-    assert list(df["name"]) == [
-        "map_101602026.png",
-        "map_101602038.png",
-        "map_102352861.png",
-        "map_91617032.png",
-    ]
+    assert all(
+        name in list(df["name"])
+        for name in [
+            "map_101602026.png",
+            "map_101602038.png",
+            "map_102352861.png",
+            "map_91617032.png",
+            "map_101603986.png",
+            "map_101603986_1.png",
+        ]
+    )
+    # test coords
+    assert literal_eval(df.loc[0, "coordinates"]) == approx(
+        (-0.98876953125, 53.448806835427575, -0.90087890625, 53.48804553605621),
+        rel=1e-6,
+    )
     assert df.loc[3, "published_date"] == 2021
     assert df.loc[3, "test1"] == "test"
     assert df.loc[3, "test2"] == "Six_Inch_GB_WFS.132"
 
 
 def test_download_by_wfs_ids(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     sd.download_map_sheets_by_wfs_ids(
         16320, maps_path, metadata_fname
     )  # test single wfs_id
     assert os.path.exists(f"{maps_path}/map_101602026.png")
     assert os.path.exists(f"{maps_path}/{metadata_fname}")
@@ -407,31 +463,82 @@
     )  # test overwrite
     df = pd.read_csv(f"{maps_path}/{metadata_fname}", sep=",", index_col=0)
     assert len(df) == 2
     assert df.loc[0, "name"] == "map_101602026.png"
     assert df.loc[1, "name"] == "map_101602038.png"
 
 
+def test_download_same_image_names(sheet_downloader, tmp_path, capfd):
+    sd = sheet_downloader
+    sd.get_grid_bb(14)
+    maps_path = tmp_path / "test_maps/"
+    metadata_fname = "test_metadata.csv"
+    sd.download_map_sheets_by_wfs_ids(
+        [107, 116], maps_path, metadata_fname
+    )  # 107 and 116 both refer to https://maps.nls.uk/view/101603986
+    assert os.path.exists(f"{maps_path}/map_101603986.png")
+    assert os.path.exists(f"{maps_path}/map_101603986_1.png")
+    assert os.path.exists(f"{maps_path}/{metadata_fname}")
+    df = pd.read_csv(f"{maps_path}/{metadata_fname}", sep=",", index_col=0)
+    assert len(df) == 2
+    assert list(df.columns) == [
+        "name",
+        "url",
+        "coordinates",
+        "crs",
+        "published_date",
+        "grid_bb",
+    ]
+    assert df.loc[0, "name"] == "map_101603986.png"
+    assert df.loc[1, "name"] == "map_101603986_1.png"
+
+    # run again, nothing should happen
+    sd.download_map_sheets_by_wfs_ids([107, 116], maps_path, metadata_fname)
+    out, _ = capfd.readouterr()
+    assert out.endswith(
+        '[INFO] "map_101603986.png" already exists. Skipping download.\n[INFO] "map_101603986_1.png" already exists. Skipping download.\n'
+    )
+    df = pd.read_csv(f"{maps_path}/{metadata_fname}", sep=",", index_col=0)
+    assert len(df) == 2
+
+    # now overwrite them, but check we don't add new ones (_2, _3 etc.)
+    sd.download_map_sheets_by_wfs_ids(
+        [107, 116], maps_path, metadata_fname, overwrite=True
+    )  # 107 and 116 both refer to https://maps.nls.uk/view/101603986
+    out, _ = capfd.readouterr()
+    assert re.search(
+        r"\[INFO\] Downloaded \".*\/test_maps\/map_101603986.png\"\n\[INFO\] Downloaded \".*\/test_maps\/map_101603986_1.png\"\n$",
+        out,
+    )
+    assert os.path.exists(f"{maps_path}/map_101603986.png")
+    assert os.path.exists(f"{maps_path}/map_101603986_1.png")
+    assert os.path.exists(f"{maps_path}/{metadata_fname}")
+    df = pd.read_csv(f"{maps_path}/{metadata_fname}", sep=",", index_col=0)
+    assert len(df) == 2
+    assert df.loc[0, "name"] == "map_101603986.png"
+    assert df.loc[1, "name"] == "map_101603986_1.png"
+
+
 def test_download_by_wfs_ids_errors(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     with pytest.raises(ValueError, match="as int or list of ints"):
         sd.download_map_sheets_by_wfs_ids("string", maps_path, metadata_fname)
     with pytest.raises(ValueError, match="as int or list of ints"):
         sd.download_map_sheets_by_wfs_ids(21.4, maps_path, metadata_fname)
 
     with pytest.raises(ValueError, match="No map sheets"):
         sd.download_map_sheets_by_wfs_ids(12, maps_path, metadata_fname)
 
 
 def test_download_by_polygon(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     polygon = Polygon(
         [
             [-0.98078243, 53.45664144],
             [-0.9806354, 53.48556079],
             [-0.90790637, 53.48540701],
             [-0.90810282, 53.45648782],
             [-0.98078243, 53.45664144],
@@ -463,15 +570,15 @@
     df = pd.read_csv(f"{maps_path}/{metadata_fname}", sep=",", index_col=0)
     assert len(df) == 2  # should have only downloaded/added one extra map
     assert df.loc[1, "name"] == "map_101602038.png"
 
 
 def test_download_by_polygon_errors(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     polygon = Polygon([[0, 1], [1, 2], [2, 3], [3, 4], [0, 1]])
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     with pytest.raises(
         NotImplementedError, match='``mode="within"`` or ``mode="intersects"``'
     ):
         sd.download_map_sheets_by_polygon(
@@ -479,15 +586,15 @@
         )
     with pytest.raises(ValueError, match="out of map metadata bounds"):
         sd.download_map_sheets_by_polygon(polygon, maps_path, metadata_fname)
 
 
 def test_download_by_coords(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     sd.download_map_sheets_by_coordinates((-0.99, 53.43), maps_path, metadata_fname)
     assert os.path.exists(f"{maps_path}/map_101602038.png")
     assert os.path.exists(f"{maps_path}/{metadata_fname}")
     df = pd.read_csv(f"{maps_path}/{metadata_fname}", sep=",", index_col=0)
     assert len(df) == 1
@@ -500,24 +607,24 @@
         "grid_bb",
     ]
     assert df.loc[0, "name"] == "map_101602038.png"
 
 
 def test_download_by_coords_errors(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     with pytest.raises(ValueError, match="out of map metadata bounds"):
         sd.download_map_sheets_by_coordinates((0, 1), maps_path, metadata_fname)
 
 
 def test_download_by_line(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     line = LineString([(-0.99, 53.43), (-0.93, 53.46)])
     sd.download_map_sheets_by_line(line, maps_path, metadata_fname)
     assert os.path.exists(f"{maps_path}/map_101602026.png")
     assert os.path.exists(f"{maps_path}/{metadata_fname}")
     df = pd.read_csv(f"{maps_path}/{metadata_fname}", sep=",", index_col=0)
@@ -531,25 +638,25 @@
         "grid_bb",
     ]
     assert list(df["name"]) == ["map_101602026.png", "map_101602038.png"]
 
 
 def test_download_by_line_errors(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     line = LineString([(0, 1), (2, 3)])
     with pytest.raises(ValueError, match="out of map metadata bounds"):
         sd.download_map_sheets_by_line(line, maps_path, metadata_fname)
 
 
 def test_download_by_string(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     sd.download_map_sheets_by_string(
         "Westminster", ["properties", "PARISH"], maps_path, metadata_fname
     )  # test w/ keys list
     assert os.path.exists(f"{maps_path}/map_91617032.png")
     assert os.path.exists(f"{maps_path}/{metadata_fname}")
@@ -581,39 +688,39 @@
     df = pd.read_csv(f"{maps_path}/{metadata_fname}", sep=",", index_col=0)
     assert len(df) == 3
     assert df.loc[2, "name"] == "map_101602038.png"
 
 
 def test_download_by_string_value_errors(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     with pytest.raises(ValueError, match="pass ``string`` as a string"):
         sd.download_map_sheets_by_string(
             10, path_save=maps_path, metadata_fname=metadata_fname
         )
     with pytest.raises(ValueError, match="as string or list of strings"):
         sd.download_map_sheets_by_string("Westminster", 10, maps_path, metadata_fname)
 
 
 def test_download_by_string_key_errors(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     with pytest.raises(KeyError, match="not found in features dictionary"):
         sd.download_map_sheets_by_string(
             "Nottinghamshire", ["fake_key"], maps_path, metadata_fname
         )
 
 
 def test_download_by_queries(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     sd.query_map_sheets_by_wfs_ids([16320, 132])  # features[0] and [3]
     sd.query_map_sheets_by_coordinates((-0.23, 51.5), append=True)  # features[3]
     assert len(sd.found_queries) == 2
     sd.download_map_sheets_by_queries(maps_path, metadata_fname)
     assert os.path.exists(f"{maps_path}/map_101602026.png")
@@ -630,12 +737,12 @@
         "grid_bb",
     ]
     assert list(df["name"]) == ["map_101602026.png", "map_91617032.png"]
 
 
 def test_download_by_queries_errors(sheet_downloader, tmp_path):
     sd = sheet_downloader
-    sd.get_grid_bb(10)
+    sd.get_grid_bb(14)
     maps_path = tmp_path / "test_maps/"
     metadata_fname = "test_metadata.csv"
     with pytest.raises(ValueError, match="No query results"):
         sd.download_map_sheets_by_queries(maps_path, metadata_fname)
```

### Comparing `mapreader-1.3.0/versioneer.py` & `mapreader-1.3.1/versioneer.py`

 * *Files identical despite different names*


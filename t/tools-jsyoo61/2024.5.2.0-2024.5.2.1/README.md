# Comparing `tmp/tools-jsyoo61-2024.5.2.0.tar.gz` & `tmp/tools-jsyoo61-2024.5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tools-jsyoo61-2024.5.2.0.tar", last modified: Fri May  3 01:53:22 2024, max compression
+gzip compressed data, was "tools-jsyoo61-2024.5.2.1.tar", last modified: Fri May  3 01:54:45 2024, max compression
```

## Comparing `tools-jsyoo61-2024.5.2.0.tar` & `tools-jsyoo61-2024.5.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 01:53:22.854021 tools-jsyoo61-2024.5.2.0/
--rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1342 2024-05-03 01:53:22.853017 tools-jsyoo61-2024.5.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 01:53:22.854021 tools-jsyoo61-2024.5.2.0/setup.cfg
--rw-rw-rw-   0        0        0      821 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:53:22.792391 tools-jsyoo61-2024.5.2.0/tools/
--rw-rw-rw-   0        0        0      292 2024-05-03 01:53:08.000000 tools-jsyoo61-2024.5.2.0/tools/__init__.py
--rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/array.py
--rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/data.py
--rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/exp.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:53:22.794392 tools-jsyoo61-2024.5.2.0/tools/hydra/
--rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/hydra/__init__.py
--rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.5.2.0/tools/modules.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:53:22.799428 tools-jsyoo61-2024.5.2.0/tools/numpy/
--rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/numpy/__init__.py
--rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/numpy/_f.py
--rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/numpy/_utils.py
--rw-rw-rw-   0        0        0     1923 2024-05-03 01:48:36.000000 tools-jsyoo61-2024.5.2.0/tools/os.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:53:22.801395 tools-jsyoo61-2024.5.2.0/tools/pandas/
--rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:53:22.804394 tools-jsyoo61-2024.5.2.0/tools/plot/
--rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/plot/__init__.py
--rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/plot/sklearn.py
--rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/plot/utils.py
--rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/random.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:53:22.807396 tools-jsyoo61-2024.5.2.0/tools/sklearn/
--rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/sklearn/__init__.py
--rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.5.2.0/tools/sklearn/model_selection.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:53:22.808394 tools-jsyoo61-2024.5.2.0/tools/stats/
--rw-rw-rw-   0        0        0     1241 2024-03-19 18:49:39.000000 tools-jsyoo61-2024.5.2.0/tools/stats/__init__.py
--rw-rw-rw-   0        0        0    15661 2024-05-03 01:52:51.000000 tools-jsyoo61-2024.5.2.0/tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:53:22.821469 tools-jsyoo61-2024.5.2.0/tools/torch/
--rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/torch/__init__.py
--rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/torch/_pandas.py
--rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/torch/estimator.py
--rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/torch/federated_learning.py
--rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/torch/layers.py
--rw-rw-rw-   0        0        0    18008 2024-03-14 20:51:33.000000 tools-jsyoo61-2024.5.2.0/tools/torch/model.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:53:22.824479 tools-jsyoo61-2024.5.2.0/tools/torch/optim/
--rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/torch/optim/__init__.py
--rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/torch/optim/lr_scheduler.py
--rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.0/tools/torch/plot.py
--rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.5.2.0/tools/torch/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:53:22.852018 tools-jsyoo61-2024.5.2.0/tools_jsyoo61.egg-info/
--rw-rw-rw-   0        0        0     1342 2024-05-03 01:53:22.000000 tools-jsyoo61-2024.5.2.0/tools_jsyoo61.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2024-05-03 01:53:22.000000 tools-jsyoo61-2024.5.2.0/tools_jsyoo61.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 01:53:22.000000 tools-jsyoo61-2024.5.2.0/tools_jsyoo61.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-03 01:53:22.000000 tools-jsyoo61-2024.5.2.0/tools_jsyoo61.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 01:53:22.000000 tools-jsyoo61-2024.5.2.0/tools_jsyoo61.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 01:54:45.774362 tools-jsyoo61-2024.5.2.1/
+-rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1342 2024-05-03 01:54:45.772796 tools-jsyoo61-2024.5.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 01:54:45.774362 tools-jsyoo61-2024.5.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      821 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:54:45.723626 tools-jsyoo61-2024.5.2.1/tools/
+-rw-rw-rw-   0        0        0      292 2024-05-03 01:54:36.000000 tools-jsyoo61-2024.5.2.1/tools/__init__.py
+-rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/array.py
+-rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/data.py
+-rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/exp.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:54:45.725627 tools-jsyoo61-2024.5.2.1/tools/hydra/
+-rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/hydra/__init__.py
+-rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.5.2.1/tools/modules.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:54:45.728624 tools-jsyoo61-2024.5.2.1/tools/numpy/
+-rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/numpy/_f.py
+-rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/numpy/_utils.py
+-rw-rw-rw-   0        0        0     1923 2024-05-03 01:48:36.000000 tools-jsyoo61-2024.5.2.1/tools/os.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:54:45.729621 tools-jsyoo61-2024.5.2.1/tools/pandas/
+-rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:54:45.734676 tools-jsyoo61-2024.5.2.1/tools/plot/
+-rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/plot/__init__.py
+-rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/plot/sklearn.py
+-rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/plot/utils.py
+-rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/random.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:54:45.737623 tools-jsyoo61-2024.5.2.1/tools/sklearn/
+-rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/sklearn/__init__.py
+-rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.5.2.1/tools/sklearn/model_selection.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:54:45.739625 tools-jsyoo61-2024.5.2.1/tools/stats/
+-rw-rw-rw-   0        0        0     1241 2024-03-19 18:49:39.000000 tools-jsyoo61-2024.5.2.1/tools/stats/__init__.py
+-rw-rw-rw-   0        0        0    15659 2024-05-03 01:54:37.000000 tools-jsyoo61-2024.5.2.1/tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:54:45.752692 tools-jsyoo61-2024.5.2.1/tools/torch/
+-rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/torch/__init__.py
+-rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/torch/_pandas.py
+-rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/torch/estimator.py
+-rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/torch/federated_learning.py
+-rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/torch/layers.py
+-rw-rw-rw-   0        0        0    18008 2024-03-14 20:51:33.000000 tools-jsyoo61-2024.5.2.1/tools/torch/model.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:54:45.755671 tools-jsyoo61-2024.5.2.1/tools/torch/optim/
+-rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/torch/optim/__init__.py
+-rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/torch/optim/lr_scheduler.py
+-rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.1/tools/torch/plot.py
+-rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.5.2.1/tools/torch/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:54:45.771727 tools-jsyoo61-2024.5.2.1/tools_jsyoo61.egg-info/
+-rw-rw-rw-   0        0        0     1342 2024-05-03 01:54:44.000000 tools-jsyoo61-2024.5.2.1/tools_jsyoo61.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2024-05-03 01:54:45.000000 tools-jsyoo61-2024.5.2.1/tools_jsyoo61.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 01:54:45.000000 tools-jsyoo61-2024.5.2.1/tools_jsyoo61.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-03 01:54:45.000000 tools-jsyoo61-2024.5.2.1/tools_jsyoo61.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 01:54:45.000000 tools-jsyoo61-2024.5.2.1/tools_jsyoo61.egg-info/top_level.txt
```

### Comparing `tools-jsyoo61-2024.5.2.0/LICENSE.txt` & `tools-jsyoo61-2024.5.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/PKG-INFO` & `tools-jsyoo61-2024.5.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.5.2.0
+Version: 2024.5.2.1
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@korea.ac.kr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tools-jsyoo61-2024.5.2.0/README.md` & `tools-jsyoo61-2024.5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/setup.py` & `tools-jsyoo61-2024.5.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/array.py` & `tools-jsyoo61-2024.5.2.1/tools/array.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/data.py` & `tools-jsyoo61-2024.5.2.1/tools/data.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/exp.py` & `tools-jsyoo61-2024.5.2.1/tools/exp.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/modules.py` & `tools-jsyoo61-2024.5.2.1/tools/modules.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/numpy/_f.py` & `tools-jsyoo61-2024.5.2.1/tools/numpy/_f.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/numpy/_utils.py` & `tools-jsyoo61-2024.5.2.1/tools/numpy/_utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/os.py` & `tools-jsyoo61-2024.5.2.1/tools/os.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/plot/sklearn.py` & `tools-jsyoo61-2024.5.2.1/tools/plot/sklearn.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/plot/utils.py` & `tools-jsyoo61-2024.5.2.1/tools/plot/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/random.py` & `tools-jsyoo61-2024.5.2.1/tools/random.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/sklearn/model_selection.py` & `tools-jsyoo61-2024.5.2.1/tools/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/stats/__init__.py` & `tools-jsyoo61-2024.5.2.1/tools/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/tools.py` & `tools-jsyoo61-2024.5.2.1/tools/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 __all__ = \
 [
 #  'Filename',
 'Printer',
 'TDict',
 'Timer',
-#  'Path',
+ 'Path',
 'Wrapper',
 'append',
 'cmd',
 'equal',
 'equal_set',
 'equal_array',
 'iseven',
```

### Comparing `tools-jsyoo61-2024.5.2.0/tools/torch/estimator.py` & `tools-jsyoo61-2024.5.2.1/tools/torch/estimator.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/torch/federated_learning.py` & `tools-jsyoo61-2024.5.2.1/tools/torch/federated_learning.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/torch/model.py` & `tools-jsyoo61-2024.5.2.1/tools/torch/model.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/torch/optim/lr_scheduler.py` & `tools-jsyoo61-2024.5.2.1/tools/torch/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools/torch/utils.py` & `tools-jsyoo61-2024.5.2.1/tools/torch/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.0/tools_jsyoo61.egg-info/PKG-INFO` & `tools-jsyoo61-2024.5.2.1/tools_jsyoo61.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.5.2.0
+Version: 2024.5.2.1
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@korea.ac.kr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tools-jsyoo61-2024.5.2.0/tools_jsyoo61.egg-info/SOURCES.txt` & `tools-jsyoo61-2024.5.2.1/tools_jsyoo61.egg-info/SOURCES.txt`

 * *Files identical despite different names*


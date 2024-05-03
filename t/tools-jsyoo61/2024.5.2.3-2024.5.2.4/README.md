# Comparing `tmp/tools-jsyoo61-2024.5.2.3.tar.gz` & `tmp/tools-jsyoo61-2024.5.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tools-jsyoo61-2024.5.2.3.tar", last modified: Fri May  3 02:06:40 2024, max compression
+gzip compressed data, was "tools-jsyoo61-2024.5.2.4.tar", last modified: Fri May  3 18:26:15 2024, max compression
```

## Comparing `tools-jsyoo61-2024.5.2.3.tar` & `tools-jsyoo61-2024.5.2.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.379451 tools-jsyoo61-2024.5.2.3/
--rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1342 2024-05-03 02:06:40.377512 tools-jsyoo61-2024.5.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 02:06:40.379451 tools-jsyoo61-2024.5.2.3/setup.cfg
--rw-rw-rw-   0        0        0      821 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.323848 tools-jsyoo61-2024.5.2.3/tools/
--rw-rw-rw-   0        0        0      292 2024-05-03 02:05:01.000000 tools-jsyoo61-2024.5.2.3/tools/__init__.py
--rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/array.py
--rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/data.py
--rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/exp.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.324824 tools-jsyoo61-2024.5.2.3/tools/hydra/
--rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/hydra/__init__.py
--rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.5.2.3/tools/modules.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.329591 tools-jsyoo61-2024.5.2.3/tools/numpy/
--rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/numpy/__init__.py
--rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/numpy/_f.py
--rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/numpy/_utils.py
--rw-rw-rw-   0        0        0     2279 2024-05-03 02:04:50.000000 tools-jsyoo61-2024.5.2.3/tools/os.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.330588 tools-jsyoo61-2024.5.2.3/tools/pandas/
--rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.334596 tools-jsyoo61-2024.5.2.3/tools/plot/
--rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/plot/__init__.py
--rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/plot/sklearn.py
--rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/plot/utils.py
--rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/random.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.337834 tools-jsyoo61-2024.5.2.3/tools/sklearn/
--rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/sklearn/__init__.py
--rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.5.2.3/tools/sklearn/model_selection.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.339837 tools-jsyoo61-2024.5.2.3/tools/stats/
--rw-rw-rw-   0        0        0     1241 2024-03-19 18:49:39.000000 tools-jsyoo61-2024.5.2.3/tools/stats/__init__.py
--rw-rw-rw-   0        0        0    15599 2024-05-03 01:56:35.000000 tools-jsyoo61-2024.5.2.3/tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.354830 tools-jsyoo61-2024.5.2.3/tools/torch/
--rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/__init__.py
--rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/_pandas.py
--rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/estimator.py
--rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/federated_learning.py
--rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/layers.py
--rw-rw-rw-   0        0        0    18008 2024-03-14 20:51:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/model.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.357839 tools-jsyoo61-2024.5.2.3/tools/torch/optim/
--rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/optim/__init__.py
--rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/optim/lr_scheduler.py
--rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/plot.py
--rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.5.2.3/tools/torch/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.375491 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/
--rw-rw-rw-   0        0        0     1342 2024-05-03 02:06:39.000000 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2024-05-03 02:06:40.000000 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 02:06:39.000000 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-03 02:06:39.000000 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 02:06:39.000000 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 18:26:15.232150 tools-jsyoo61-2024.5.2.4/
+-rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1342 2024-05-03 18:26:15.230150 tools-jsyoo61-2024.5.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 18:26:15.233149 tools-jsyoo61-2024.5.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      821 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:26:15.152072 tools-jsyoo61-2024.5.2.4/tools/
+-rw-rw-rw-   0        0        0      292 2024-05-03 18:26:08.000000 tools-jsyoo61-2024.5.2.4/tools/__init__.py
+-rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/array.py
+-rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/data.py
+-rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/exp.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:26:15.155073 tools-jsyoo61-2024.5.2.4/tools/hydra/
+-rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/hydra/__init__.py
+-rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.5.2.4/tools/modules.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:26:15.159078 tools-jsyoo61-2024.5.2.4/tools/numpy/
+-rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/numpy/_f.py
+-rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/numpy/_utils.py
+-rw-rw-rw-   0        0        0     2279 2024-05-03 02:04:50.000000 tools-jsyoo61-2024.5.2.4/tools/os.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:26:15.160073 tools-jsyoo61-2024.5.2.4/tools/pandas/
+-rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:26:15.164079 tools-jsyoo61-2024.5.2.4/tools/plot/
+-rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/plot/__init__.py
+-rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/plot/sklearn.py
+-rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/plot/utils.py
+-rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/random.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:26:15.169103 tools-jsyoo61-2024.5.2.4/tools/sklearn/
+-rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/sklearn/__init__.py
+-rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.5.2.4/tools/sklearn/model_selection.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:26:15.171109 tools-jsyoo61-2024.5.2.4/tools/stats/
+-rw-rw-rw-   0        0        0     1241 2024-03-19 18:49:39.000000 tools-jsyoo61-2024.5.2.4/tools/stats/__init__.py
+-rw-rw-rw-   0        0        0    15593 2024-05-03 18:25:14.000000 tools-jsyoo61-2024.5.2.4/tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:26:15.189622 tools-jsyoo61-2024.5.2.4/tools/torch/
+-rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/torch/__init__.py
+-rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/torch/_pandas.py
+-rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/torch/estimator.py
+-rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/torch/federated_learning.py
+-rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/torch/layers.py
+-rw-rw-rw-   0        0        0    18008 2024-03-14 20:51:33.000000 tools-jsyoo61-2024.5.2.4/tools/torch/model.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:26:15.192810 tools-jsyoo61-2024.5.2.4/tools/torch/optim/
+-rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/torch/optim/__init__.py
+-rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/torch/optim/lr_scheduler.py
+-rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.4/tools/torch/plot.py
+-rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.5.2.4/tools/torch/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:26:15.228149 tools-jsyoo61-2024.5.2.4/tools_jsyoo61.egg-info/
+-rw-rw-rw-   0        0        0     1342 2024-05-03 18:26:14.000000 tools-jsyoo61-2024.5.2.4/tools_jsyoo61.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2024-05-03 18:26:14.000000 tools-jsyoo61-2024.5.2.4/tools_jsyoo61.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 18:26:14.000000 tools-jsyoo61-2024.5.2.4/tools_jsyoo61.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-03 18:26:14.000000 tools-jsyoo61-2024.5.2.4/tools_jsyoo61.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 18:26:14.000000 tools-jsyoo61-2024.5.2.4/tools_jsyoo61.egg-info/top_level.txt
```

### Comparing `tools-jsyoo61-2024.5.2.3/LICENSE.txt` & `tools-jsyoo61-2024.5.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/PKG-INFO` & `tools-jsyoo61-2024.5.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.5.2.3
+Version: 2024.5.2.4
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@korea.ac.kr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tools-jsyoo61-2024.5.2.3/README.md` & `tools-jsyoo61-2024.5.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/setup.py` & `tools-jsyoo61-2024.5.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/array.py` & `tools-jsyoo61-2024.5.2.4/tools/array.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/data.py` & `tools-jsyoo61-2024.5.2.4/tools/data.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/exp.py` & `tools-jsyoo61-2024.5.2.4/tools/exp.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/modules.py` & `tools-jsyoo61-2024.5.2.4/tools/modules.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/numpy/_f.py` & `tools-jsyoo61-2024.5.2.4/tools/numpy/_f.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/numpy/_utils.py` & `tools-jsyoo61-2024.5.2.4/tools/numpy/_utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/os.py` & `tools-jsyoo61-2024.5.2.4/tools/os.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/plot/sklearn.py` & `tools-jsyoo61-2024.5.2.4/tools/plot/sklearn.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/plot/utils.py` & `tools-jsyoo61-2024.5.2.4/tools/plot/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/random.py` & `tools-jsyoo61-2024.5.2.4/tools/random.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/sklearn/model_selection.py` & `tools-jsyoo61-2024.5.2.4/tools/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/stats/__init__.py` & `tools-jsyoo61-2024.5.2.4/tools/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/tools.py` & `tools-jsyoo61-2024.5.2.4/tools/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
         # if hasattr(self, 'path'):
         #     assert key != 'path', '"path" is a predefined attribute and must not be used. Use some other attribute name'
         #     super(Path, self).__setattr__(key, Path(os.path.join(self._path, value)))
         # else:
         #     super(Path, self).__setattr__(key, value)
 
     def join(self, *args):
-        return Path(os.path.join(self._path, *args))
+        return Path(os.path.join(self, *args))
 
     def makedirs(self, exist_ok=True):
         '''Make directories of all children paths
         Be sure to define all folders first, makedirs(), and then define files in Path(),
         since defining files before makedirs() will lead to creating directories with names of files.
         It is possible to ignore paths with "." as all files do, but there are hidden directories that
         start with "." which makes things complicated. Thus, defining folders -> makedirs() -> define files
```

### Comparing `tools-jsyoo61-2024.5.2.3/tools/torch/estimator.py` & `tools-jsyoo61-2024.5.2.4/tools/torch/estimator.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/torch/federated_learning.py` & `tools-jsyoo61-2024.5.2.4/tools/torch/federated_learning.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/torch/model.py` & `tools-jsyoo61-2024.5.2.4/tools/torch/model.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/torch/optim/lr_scheduler.py` & `tools-jsyoo61-2024.5.2.4/tools/torch/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools/torch/utils.py` & `tools-jsyoo61-2024.5.2.4/tools/torch/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/PKG-INFO` & `tools-jsyoo61-2024.5.2.4/tools_jsyoo61.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.5.2.3
+Version: 2024.5.2.4
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@korea.ac.kr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/SOURCES.txt` & `tools-jsyoo61-2024.5.2.4/tools_jsyoo61.egg-info/SOURCES.txt`

 * *Files identical despite different names*


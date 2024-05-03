# Comparing `tmp/tools-jsyoo61-2024.5.2.2.tar.gz` & `tmp/tools-jsyoo61-2024.5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tools-jsyoo61-2024.5.2.2.tar", last modified: Fri May  3 01:56:49 2024, max compression
+gzip compressed data, was "tools-jsyoo61-2024.5.2.3.tar", last modified: Fri May  3 02:06:40 2024, max compression
```

## Comparing `tools-jsyoo61-2024.5.2.2.tar` & `tools-jsyoo61-2024.5.2.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 01:56:49.094190 tools-jsyoo61-2024.5.2.2/
--rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1342 2024-05-03 01:56:49.093189 tools-jsyoo61-2024.5.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 01:56:49.094190 tools-jsyoo61-2024.5.2.2/setup.cfg
--rw-rw-rw-   0        0        0      821 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:56:49.043083 tools-jsyoo61-2024.5.2.2/tools/
--rw-rw-rw-   0        0        0      292 2024-05-03 01:56:42.000000 tools-jsyoo61-2024.5.2.2/tools/__init__.py
--rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/array.py
--rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/data.py
--rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/exp.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:56:49.045077 tools-jsyoo61-2024.5.2.2/tools/hydra/
--rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/hydra/__init__.py
--rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.5.2.2/tools/modules.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:56:49.049080 tools-jsyoo61-2024.5.2.2/tools/numpy/
--rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/numpy/__init__.py
--rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/numpy/_f.py
--rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/numpy/_utils.py
--rw-rw-rw-   0        0        0     1923 2024-05-03 01:48:36.000000 tools-jsyoo61-2024.5.2.2/tools/os.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:56:49.050082 tools-jsyoo61-2024.5.2.2/tools/pandas/
--rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:56:49.054074 tools-jsyoo61-2024.5.2.2/tools/plot/
--rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/plot/__init__.py
--rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/plot/sklearn.py
--rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/plot/utils.py
--rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/random.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:56:49.057074 tools-jsyoo61-2024.5.2.2/tools/sklearn/
--rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/sklearn/__init__.py
--rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.5.2.2/tools/sklearn/model_selection.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:56:49.059075 tools-jsyoo61-2024.5.2.2/tools/stats/
--rw-rw-rw-   0        0        0     1241 2024-03-19 18:49:39.000000 tools-jsyoo61-2024.5.2.2/tools/stats/__init__.py
--rw-rw-rw-   0        0        0    15599 2024-05-03 01:56:35.000000 tools-jsyoo61-2024.5.2.2/tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:56:49.070566 tools-jsyoo61-2024.5.2.2/tools/torch/
--rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/torch/__init__.py
--rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/torch/_pandas.py
--rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/torch/estimator.py
--rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/torch/federated_learning.py
--rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/torch/layers.py
--rw-rw-rw-   0        0        0    18008 2024-03-14 20:51:33.000000 tools-jsyoo61-2024.5.2.2/tools/torch/model.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:56:49.074610 tools-jsyoo61-2024.5.2.2/tools/torch/optim/
--rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/torch/optim/__init__.py
--rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/torch/optim/lr_scheduler.py
--rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.2/tools/torch/plot.py
--rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.5.2.2/tools/torch/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:56:49.091214 tools-jsyoo61-2024.5.2.2/tools_jsyoo61.egg-info/
--rw-rw-rw-   0        0        0     1342 2024-05-03 01:56:48.000000 tools-jsyoo61-2024.5.2.2/tools_jsyoo61.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2024-05-03 01:56:48.000000 tools-jsyoo61-2024.5.2.2/tools_jsyoo61.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 01:56:48.000000 tools-jsyoo61-2024.5.2.2/tools_jsyoo61.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-03 01:56:48.000000 tools-jsyoo61-2024.5.2.2/tools_jsyoo61.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 01:56:48.000000 tools-jsyoo61-2024.5.2.2/tools_jsyoo61.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.379451 tools-jsyoo61-2024.5.2.3/
+-rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1342 2024-05-03 02:06:40.377512 tools-jsyoo61-2024.5.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 02:06:40.379451 tools-jsyoo61-2024.5.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      821 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.323848 tools-jsyoo61-2024.5.2.3/tools/
+-rw-rw-rw-   0        0        0      292 2024-05-03 02:05:01.000000 tools-jsyoo61-2024.5.2.3/tools/__init__.py
+-rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/array.py
+-rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/data.py
+-rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/exp.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.324824 tools-jsyoo61-2024.5.2.3/tools/hydra/
+-rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/hydra/__init__.py
+-rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.5.2.3/tools/modules.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.329591 tools-jsyoo61-2024.5.2.3/tools/numpy/
+-rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/numpy/_f.py
+-rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/numpy/_utils.py
+-rw-rw-rw-   0        0        0     2279 2024-05-03 02:04:50.000000 tools-jsyoo61-2024.5.2.3/tools/os.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.330588 tools-jsyoo61-2024.5.2.3/tools/pandas/
+-rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.334596 tools-jsyoo61-2024.5.2.3/tools/plot/
+-rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/plot/__init__.py
+-rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/plot/sklearn.py
+-rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/plot/utils.py
+-rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/random.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.337834 tools-jsyoo61-2024.5.2.3/tools/sklearn/
+-rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/sklearn/__init__.py
+-rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.5.2.3/tools/sklearn/model_selection.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.339837 tools-jsyoo61-2024.5.2.3/tools/stats/
+-rw-rw-rw-   0        0        0     1241 2024-03-19 18:49:39.000000 tools-jsyoo61-2024.5.2.3/tools/stats/__init__.py
+-rw-rw-rw-   0        0        0    15599 2024-05-03 01:56:35.000000 tools-jsyoo61-2024.5.2.3/tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.354830 tools-jsyoo61-2024.5.2.3/tools/torch/
+-rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/__init__.py
+-rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/_pandas.py
+-rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/estimator.py
+-rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/federated_learning.py
+-rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/layers.py
+-rw-rw-rw-   0        0        0    18008 2024-03-14 20:51:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/model.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.357839 tools-jsyoo61-2024.5.2.3/tools/torch/optim/
+-rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/optim/__init__.py
+-rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/optim/lr_scheduler.py
+-rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.3/tools/torch/plot.py
+-rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.5.2.3/tools/torch/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:06:40.375491 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/
+-rw-rw-rw-   0        0        0     1342 2024-05-03 02:06:39.000000 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2024-05-03 02:06:40.000000 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 02:06:39.000000 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-03 02:06:39.000000 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 02:06:39.000000 tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/top_level.txt
```

### Comparing `tools-jsyoo61-2024.5.2.2/LICENSE.txt` & `tools-jsyoo61-2024.5.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/PKG-INFO` & `tools-jsyoo61-2024.5.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.5.2.2
+Version: 2024.5.2.3
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@korea.ac.kr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tools-jsyoo61-2024.5.2.2/README.md` & `tools-jsyoo61-2024.5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/setup.py` & `tools-jsyoo61-2024.5.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/array.py` & `tools-jsyoo61-2024.5.2.3/tools/array.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/data.py` & `tools-jsyoo61-2024.5.2.3/tools/data.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/exp.py` & `tools-jsyoo61-2024.5.2.3/tools/exp.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/modules.py` & `tools-jsyoo61-2024.5.2.3/tools/modules.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/numpy/_f.py` & `tools-jsyoo61-2024.5.2.3/tools/numpy/_f.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/numpy/_utils.py` & `tools-jsyoo61-2024.5.2.3/tools/numpy/_utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/os.py` & `tools-jsyoo61-2024.5.2.3/tools/os.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [
 'listdir',
 'makedirs'
 ]
 
 def makedirs(path, exist_ok=True):
     os.makedirs(path, exist_ok=exist_ok)
-    
+
 def listdir(path=None, isdir: bool=False, isfile: Union[bool, str]=False, join: bool=False):
     '''
     :func listdir:
 
     :param path:
     :param isdir:
     :param isfile:
@@ -24,29 +24,34 @@
         ext = isfile.lower() # extension
         isfile_str = True
         isfile = True
     else:
         isfile_str=False
     # assert type(isfile)==str or type(isfile)==bool, 'isfile can be either str or bool'
     # _isfile = True if type(isfile)==str else isfile
-    
     assert not (isdir and isfile), 'only one of argument "isdir" and "isfile" can be True'
+    # if path == None:
+    #     path = '.'
 
     dir_list = os.listdir(path)
 
+    # when path is referring to somewhere non-cwd, we need dir_list_joined to pass reference for isdir() or isfile().
+    if join or isdir or isfile:
+        dir_list_joined = dir_list if path is None else [os.path.join(path, dir) for dir in dir_list]
+
     if join:
-        dir_list = dir_list if path is None else [os.path.join(path, dir) for dir in dir_list]
+        dir_list = dir_list_joined
 
     if isdir:
-        return [dir for dir in dir_list if os.path.isdir(dir)]
+        return [dir for dir, dir_joined in zip(dir_list, dir_list_joined) if os.path.isdir(dir_joined)]
     elif isfile:
         if isfile_str:
-            return [dir for dir in dir_list if os.path.isfile(dir) and (os.path.splitext(dir)[1].lower() == ext)]
+            return [dir for dir, dir_joined in zip(dir_list, dir_list_joined) if os.path.isfile(dir_joined) and (os.path.splitext(dir)[1].lower() == ext)]
         else:
-            return [dir for dir in dir_list if os.path.isfile(dir)]
+            return [dir for dir, dir_joined in zip(dir_list, dir_list_joined) if os.path.isfile(dir_joined)]
     else:
         return dir_list
 
 # if __name__ == '__main__':
 #     listdir('torch', isdir=False, join=False)
 #     listdir('torch', isdir=False, join=True)
 #     listdir('torch', isdir=True, join=False)
```

### Comparing `tools-jsyoo61-2024.5.2.2/tools/plot/sklearn.py` & `tools-jsyoo61-2024.5.2.3/tools/plot/sklearn.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/plot/utils.py` & `tools-jsyoo61-2024.5.2.3/tools/plot/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/random.py` & `tools-jsyoo61-2024.5.2.3/tools/random.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/sklearn/model_selection.py` & `tools-jsyoo61-2024.5.2.3/tools/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/stats/__init__.py` & `tools-jsyoo61-2024.5.2.3/tools/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/tools.py` & `tools-jsyoo61-2024.5.2.3/tools/tools.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/torch/estimator.py` & `tools-jsyoo61-2024.5.2.3/tools/torch/estimator.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/torch/federated_learning.py` & `tools-jsyoo61-2024.5.2.3/tools/torch/federated_learning.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/torch/model.py` & `tools-jsyoo61-2024.5.2.3/tools/torch/model.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/torch/optim/lr_scheduler.py` & `tools-jsyoo61-2024.5.2.3/tools/torch/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools/torch/utils.py` & `tools-jsyoo61-2024.5.2.3/tools/torch/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.2/tools_jsyoo61.egg-info/PKG-INFO` & `tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.5.2.2
+Version: 2024.5.2.3
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@korea.ac.kr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tools-jsyoo61-2024.5.2.2/tools_jsyoo61.egg-info/SOURCES.txt` & `tools-jsyoo61-2024.5.2.3/tools_jsyoo61.egg-info/SOURCES.txt`

 * *Files identical despite different names*


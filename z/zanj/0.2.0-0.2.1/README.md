# Comparing `tmp/zanj-0.2.0.tar.gz` & `tmp/zanj-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zanj-0.2.0.tar", max compression
+gzip compressed data, was "zanj-0.2.1.tar", max compression
```

## Comparing `zanj-0.2.0.tar` & `zanj-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 zanj-0.2.0/LICENSE
--rw-r--r--   0        0        0     1177 2023-07-24 06:50:37.656207 zanj-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    10945 2023-06-14 19:11:26.380447 zanj-0.2.0/README.md
--rw-r--r--   0        0        0      146 2023-07-24 06:50:41.147372 zanj-0.2.0/zanj/__init__.py
--rw-r--r--   0        0        0     1468 2023-05-28 05:22:18.527493 zanj-0.2.0/zanj/externals.py
--rw-r--r--   0        0        0    15618 2023-05-28 05:22:18.537492 zanj-0.2.0/zanj/loading.py
--rw-r--r--   0        0        0        0 2023-06-13 22:16:55.290434 zanj-0.2.0/zanj/py.typed
--rw-r--r--   0        0        0     4143 2023-05-28 05:13:20.057826 zanj-0.2.0/zanj/readme.md
--rw-r--r--   0        0        0     8121 2023-05-28 05:22:18.541492 zanj-0.2.0/zanj/serializing.py
--rw-r--r--   0        0        0     9778 2023-06-14 03:53:30.489964 zanj-0.2.0/zanj/torchutil.py
--rw-r--r--   0        0        0     8468 2023-05-28 05:22:18.555490 zanj-0.2.0/zanj/zanj.py
--rw-r--r--   0        0        0    11702 1970-01-01 00:00:00.000000 zanj-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 zanj-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1177 2024-05-03 07:30:04.284160 zanj-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    10945 2023-06-14 19:11:26.380447 zanj-0.2.1/README.md
+-rw-r--r--   0        0        0      123 2023-09-04 08:05:22.215638 zanj-0.2.1/zanj/__init__.py
+-rw-r--r--   0        0        0     1468 2023-05-28 05:22:18.527493 zanj-0.2.1/zanj/externals.py
+-rw-r--r--   0        0        0    15618 2023-05-28 05:22:18.537492 zanj-0.2.1/zanj/loading.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:16:55.290434 zanj-0.2.1/zanj/py.typed
+-rw-r--r--   0        0        0     4143 2023-05-28 05:13:20.057826 zanj-0.2.1/zanj/readme.md
+-rw-r--r--   0        0        0     8121 2023-05-28 05:22:18.541492 zanj-0.2.1/zanj/serializing.py
+-rw-r--r--   0        0        0     9778 2024-05-03 07:29:18.068203 zanj-0.2.1/zanj/torchutil.py
+-rw-r--r--   0        0        0     8582 2024-05-03 07:26:02.706738 zanj-0.2.1/zanj/zanj.py
+-rw-r--r--   0        0        0    11702 1970-01-01 00:00:00.000000 zanj-0.2.1/PKG-INFO
```

### Comparing `zanj-0.2.0/LICENSE` & `zanj-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zanj-0.2.0/pyproject.toml` & `zanj-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zanj"
-version = "0.2.0"
+version = "0.2.1"
 description = "save and load complex objects to disk without pickling"
 license = "GPL-3.0-only"
 authors = ["mivanit <mivanits@umich.edu>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `zanj-0.2.0/README.md` & `zanj-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `zanj-0.2.0/zanj/externals.py` & `zanj-0.2.1/zanj/externals.py`

 * *Files identical despite different names*

### Comparing `zanj-0.2.0/zanj/loading.py` & `zanj-0.2.1/zanj/loading.py`

 * *Files identical despite different names*

### Comparing `zanj-0.2.0/zanj/readme.md` & `zanj-0.2.1/zanj/readme.md`

 * *Files identical despite different names*

### Comparing `zanj-0.2.0/zanj/serializing.py` & `zanj-0.2.1/zanj/serializing.py`

 * *Files identical despite different names*

### Comparing `zanj-0.2.0/zanj/torchutil.py` & `zanj-0.2.1/zanj/torchutil.py`

 * *Files identical despite different names*

### Comparing `zanj-0.2.0/zanj/zanj.py` & `zanj-0.2.1/zanj/zanj.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,18 @@
 
         # adjust extension
         file_path = str(file_path)
         if not file_path.endswith(".zanj"):
             file_path += ".zanj"
 
         # make directory
-        os.makedirs(os.path.dirname(file_path), exist_ok=True)
+        dir_path: str = os.path.dirname(file_path)
+        if dir_path != "":
+            if not os.path.exists(dir_path):
+                os.makedirs(dir_path, exist_ok=False)
 
         # clear the externals!
         self._externals = dict()
 
         # serialize the object -- this will populate self._externals
         # TODO: calling self.json_serialize again here might be slow
         json_data: JSONitem = self.json_serialize(self.json_serialize(obj))
```

### Comparing `zanj-0.2.0/PKG-INFO` & `zanj-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zanj
-Version: 0.2.0
+Version: 0.2.1
 Summary: save and load complex objects to disk without pickling
 Home-page: https://github.com/mivanit/ZANJ
 License: GPL-3.0-only
 Author: mivanit
 Author-email: mivanits@umich.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```


# Comparing `tmp/python_flux-1.3.1.tar.gz` & `tmp/python_flux-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.3.1.tar", max compression
+gzip compressed data, was "python_flux-1.3.2.tar", max compression
```

## Comparing `python_flux-1.3.1.tar` & `python_flux-1.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     8872 2024-04-26 12:27:05.738836 python_flux-1.3.1/README.rst
--rw-r--r--   0        0        0      741 2024-04-26 12:27:05.272758 python_flux-1.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.3.1/python_flux/__init__.py
--rw-r--r--   0        0        0    23514 2024-04-26 12:27:05.273713 python_flux-1.3.1/python_flux/flux.py
--rw-r--r--   0        0        0      759 2024-04-25 04:03:40.583703 python_flux-1.3.1/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1921 2024-04-25 04:03:40.584710 python_flux-1.3.1/python_flux/producers.py
--rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.3.1/python_flux/subscribers.py
--rw-r--r--   0        0        0     9603 1970-01-01 00:00:00.000000 python_flux-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     8872 2024-04-26 12:27:05.738836 python_flux-1.3.2/README.rst
+-rw-r--r--   0        0        0      741 2024-05-03 04:55:36.722355 python_flux-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.3.2/python_flux/__init__.py
+-rw-r--r--   0        0        0    23483 2024-05-03 04:55:16.370351 python_flux-1.3.2/python_flux/flux.py
+-rw-r--r--   0        0        0      759 2024-04-25 04:03:40.583703 python_flux-1.3.2/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1921 2024-04-25 04:03:40.584710 python_flux-1.3.2/python_flux/producers.py
+-rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.3.2/python_flux/subscribers.py
+-rw-r--r--   0        0        0     9603 1970-01-01 00:00:00.000000 python_flux-1.3.2/PKG-INFO
```

### Comparing `python_flux-1.3.1/README.rst` & `python_flux-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `python_flux-1.3.1/pyproject.toml` & `python_flux-1.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-flux"
-version = "1.3.1"
+version = "1.3.2"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
 authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `python_flux-1.3.1/python_flux/flux.py` & `python_flux-1.3.2/python_flux/flux.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,17 +396,16 @@
         self.value = None
         self.e = None
         self.ctx = None
         self.elapsed_time = 0
 
     def execute(self, sup, context):
         t = time.process_time_ns()
+        sup.prepare_next()
         self.value, self.e, self.ctx = sup.next(context)
-        if self.e is None:
-            sup.prepare_next()
         self.elapsed_time = (time.process_time_ns() - t) / 1000
 
 
 class FParallel(Stream):
     def __init__(self, pool, metric_func, flux):
         super().__init__(flux)
         self.pool_size = pool
```

### Comparing `python_flux-1.3.1/python_flux/flux_utilis.py` & `python_flux-1.3.2/python_flux/flux_utilis.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.3.1/python_flux/producers.py` & `python_flux-1.3.2/python_flux/producers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.3.1/python_flux/subscribers.py` & `python_flux-1.3.2/python_flux/subscribers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.3.1/PKG-INFO` & `python_flux-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.3.1
+Version: 1.3.2
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```


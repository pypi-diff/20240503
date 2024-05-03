# Comparing `tmp/montpy-0.1.1.tar.gz` & `tmp/montpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "montpy-0.1.1.tar", max compression
+gzip compressed data, was "montpy-0.1.2.tar", max compression
```

## Comparing `montpy-0.1.1.tar` & `montpy-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-04-07 11:11:46.590924 montpy-0.1.1/LICENSE
--rw-r--r--   0        0        0     1857 2024-04-07 11:46:58.610482 montpy-0.1.1/README.md
--rw-r--r--   0        0        0       36 2024-04-07 10:20:45.618460 montpy-0.1.1/montpy/__init__.py
--rw-r--r--   0        0        0     3663 2024-04-07 10:57:02.587328 montpy-0.1.1/montpy/mc.py
--rw-r--r--   0        0        0     5973 2024-04-07 10:57:08.819220 montpy-0.1.1/montpy/qmc.py
--rw-r--r--   0        0        0      395 2024-04-07 11:47:26.566089 montpy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 montpy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-03 19:42:06.302345 montpy-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1857 2024-05-03 19:42:06.302345 montpy-0.1.2/README.md
+-rw-r--r--   0        0        0       36 2024-05-03 19:42:06.302345 montpy-0.1.2/montpy/__init__.py
+-rw-r--r--   0        0        0     3663 2024-05-03 19:42:06.302345 montpy-0.1.2/montpy/mc.py
+-rw-r--r--   0        0        0     5973 2024-05-03 19:42:06.302345 montpy-0.1.2/montpy/qmc.py
+-rw-r--r--   0        0        0      394 2024-05-03 19:42:34.555806 montpy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2458 1970-01-01 00:00:00.000000 montpy-0.1.2/PKG-INFO
```

### Comparing `montpy-0.1.1/LICENSE` & `montpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `montpy-0.1.1/README.md` & `montpy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `montpy-0.1.1/montpy/mc.py` & `montpy-0.1.2/montpy/mc.py`

 * *Files identical despite different names*

### Comparing `montpy-0.1.1/montpy/qmc.py` & `montpy-0.1.2/montpy/qmc.py`

 * *Files identical despite different names*

### Comparing `montpy-0.1.1/PKG-INFO` & `montpy-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: montpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library implementing Monte Carlo and Quasi-Monte Carlo methods for integral evaluation
 Author: Pietro Zanotta
 Author-email: zanottapietro1@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >3.8
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
 Description-Content-Type: text/markdown
```


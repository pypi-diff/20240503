# Comparing `tmp/unico_device_setuper-0.3.0.tar.gz` & `tmp/unico_device_setuper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unico_device_setuper-0.3.0.tar", max compression
+gzip compressed data, was "unico_device_setuper-0.3.1.tar", max compression
```

## Comparing `unico_device_setuper-0.3.0.tar` & `unico_device_setuper-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2024-05-03 14:12:55.434511 unico_device_setuper-0.3.0/README.md
--rw-r--r--   0        0        0     4948 2024-05-03 14:12:55.386511 unico_device_setuper-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-03 14:12:55.386511 unico_device_setuper-0.3.0/unico_device_setuper/__init__.py
--rw-r--r--   0        0        0     1429 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.0/unico_device_setuper/adb.py
--rw-r--r--   0        0        0     1039 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.0/unico_device_setuper/cfg.py
--rw-r--r--   0        0        0      424 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.0/unico_device_setuper/cfg.toml
--rw-r--r--   0        0        0      936 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.0/unico_device_setuper/datadir.py
--rw-r--r--   0        0        0     1069 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.0/unico_device_setuper/dl.py
--rw-r--r--   0        0        0      656 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.0/unico_device_setuper/entrypoint.py
--rw-r--r--   0        0        0     1613 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.0/unico_device_setuper/helpers.py
--rw-r--r--   0        0        0      899 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.0/unico_device_setuper/local_db.py
--rw-r--r--   0        0        0      421 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.0/unico_device_setuper/main.py
--rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 unico_device_setuper-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-03 14:19:11.458703 unico_device_setuper-0.3.1/README.md
+-rw-r--r--   0        0        0     4948 2024-05-03 14:19:11.438703 unico_device_setuper-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-03 14:19:11.438703 unico_device_setuper-0.3.1/unico_device_setuper/__init__.py
+-rw-r--r--   0        0        0     1429 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.1/unico_device_setuper/adb.py
+-rw-r--r--   0        0        0     1039 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.1/unico_device_setuper/cfg.py
+-rw-r--r--   0        0        0      424 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.1/unico_device_setuper/cfg.toml
+-rw-r--r--   0        0        0      936 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.1/unico_device_setuper/datadir.py
+-rw-r--r--   0        0        0     1069 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.1/unico_device_setuper/dl.py
+-rw-r--r--   0        0        0      656 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.1/unico_device_setuper/entrypoint.py
+-rw-r--r--   0        0        0     1613 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.1/unico_device_setuper/helpers.py
+-rw-r--r--   0        0        0      899 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.1/unico_device_setuper/local_db.py
+-rw-r--r--   0        0        0      421 2024-05-03 13:36:58.809570 unico_device_setuper-0.3.1/unico_device_setuper/main.py
+-rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 unico_device_setuper-0.3.1/PKG-INFO
```

### Comparing `unico_device_setuper-0.3.0/pyproject.toml` & `unico_device_setuper-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unico_device_setuper"
-version = '0.3.0'
+version = '0.3.1'
 description = ""
 authors = ["Florian Daude <floriandaude@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.12,<3.13"
```

### Comparing `unico_device_setuper-0.3.0/unico_device_setuper/adb.py` & `unico_device_setuper-0.3.1/unico_device_setuper/adb.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.3.0/unico_device_setuper/cfg.py` & `unico_device_setuper-0.3.1/unico_device_setuper/cfg.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.3.0/unico_device_setuper/datadir.py` & `unico_device_setuper-0.3.1/unico_device_setuper/datadir.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.3.0/unico_device_setuper/dl.py` & `unico_device_setuper-0.3.1/unico_device_setuper/dl.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.3.0/unico_device_setuper/entrypoint.py` & `unico_device_setuper-0.3.1/unico_device_setuper/entrypoint.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.3.0/unico_device_setuper/helpers.py` & `unico_device_setuper-0.3.1/unico_device_setuper/helpers.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.3.0/unico_device_setuper/local_db.py` & `unico_device_setuper-0.3.1/unico_device_setuper/local_db.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.3.0/PKG-INFO` & `unico_device_setuper-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unico_device_setuper
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 License: MIT
 Author: Florian Daude
 Author-email: floriandaude@hotmail.fr
 Requires-Python: >=3.12,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


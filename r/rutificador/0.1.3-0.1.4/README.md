# Comparing `tmp/rutificador-0.1.3.tar.gz` & `tmp/rutificador-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.1.3.tar", max compression
+gzip compressed data, was "rutificador-0.1.4.tar", max compression
```

## Comparing `rutificador-0.1.3.tar` & `rutificador-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-02 23:41:01.721048 rutificador-0.1.3/LICENSE
--rw-r--r--   0        0        0     4068 2024-05-02 23:41:01.721048 rutificador-0.1.3/README.md
--rw-r--r--   0        0        0     1071 2024-05-02 23:41:01.721048 rutificador-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       87 2024-05-02 23:41:01.721048 rutificador-0.1.3/rutificador/__init__.py
--rw-r--r--   0        0        0     9113 2024-05-02 23:41:01.721048 rutificador-0.1.3/rutificador/main.py
--rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 rutificador-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-02 23:48:54.683780 rutificador-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4120 2024-05-02 23:48:54.683780 rutificador-0.1.4/README.md
+-rw-r--r--   0        0        0     1071 2024-05-02 23:48:54.683780 rutificador-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-05-02 23:48:54.683780 rutificador-0.1.4/rutificador/__init__.py
+-rw-r--r--   0        0        0     9113 2024-05-02 23:48:54.683780 rutificador-0.1.4/rutificador/main.py
+-rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 rutificador-0.1.4/PKG-INFO
```

### Comparing `rutificador-0.1.3/LICENSE` & `rutificador-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.1.3/README.md` & `rutificador-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
 [![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Build Status](URL_DE_LA_BADGE)](URL_A_LA_ACTION)
 
 # Rutificador
 
 Una biblioteca Python para validar y formatear RUTs (Rol Único Tributario) chilenos.
 
 ## Características
```

### Comparing `rutificador-0.1.3/pyproject.toml` & `rutificador-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rutificador"
-version = "0.1.3"
+version = "0.1.4"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo"]
 classifiers = [
```

### Comparing `rutificador-0.1.3/rutificador/main.py` & `rutificador-0.1.4/rutificador/main.py`

 * *Files identical despite different names*

### Comparing `rutificador-0.1.3/PKG-INFO` & `rutificador-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rutificador
-Version: 0.1.3
+Version: 0.1.4
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://
 License: MIT
 Keywords: RUT,Chile,validación,formateo
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -19,14 +19,15 @@
 Classifier: Topic :: Utilities
 Project-URL: Repository, https://github.com/cortega26/Rutificador
 Description-Content-Type: text/markdown
 
 [![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
 [![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Build Status](URL_DE_LA_BADGE)](URL_A_LA_ACTION)
 
 # Rutificador
 
 Una biblioteca Python para validar y formatear RUTs (Rol Único Tributario) chilenos.
 
 ## Características
```


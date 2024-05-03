# Comparing `tmp/rutificador-0.1.6.tar.gz` & `tmp/rutificador-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.1.6.tar", max compression
+gzip compressed data, was "rutificador-0.2.0.tar", max compression
```

## Comparing `rutificador-0.1.6.tar` & `rutificador-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-02 23:55:26.029734 rutificador-0.1.6/LICENSE
--rw-r--r--   0        0        0     4120 2024-05-02 23:55:26.029734 rutificador-0.1.6/README.md
--rw-r--r--   0        0        0     1071 2024-05-02 23:55:26.029734 rutificador-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       87 2024-05-02 23:55:26.029734 rutificador-0.1.6/rutificador/__init__.py
--rw-r--r--   0        0        0     9113 2024-05-02 23:55:26.029734 rutificador-0.1.6/rutificador/main.py
--rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 rutificador-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-03 15:30:50.476833 rutificador-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4229 2024-05-03 15:30:50.476833 rutificador-0.2.0/README.md
+-rw-r--r--   0        0        0     1071 2024-05-03 15:30:50.476833 rutificador-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-05-03 15:30:50.476833 rutificador-0.2.0/rutificador/__init__.py
+-rw-r--r--   0        0        0     9113 2024-05-03 15:30:50.476833 rutificador-0.2.0/rutificador/main.py
+-rw-r--r--   0        0        0     5140 1970-01-01 00:00:00.000000 rutificador-0.2.0/PKG-INFO
```

### Comparing `rutificador-0.1.6/LICENSE` & `rutificador-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.1.6/README.md` & `rutificador-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
 [![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Build Status](URL_DE_LA_BADGE)](URL_A_LA_ACTION)
+[![CI Workflow](https://github.com/cortega26/rutificador/actions/workflows/ci.yml/badge.svg)](https://github.com/cortega26/rutificador/actions/workflows/ci.yml)
 
 # Rutificador
 
 Una biblioteca Python para validar y formatear RUTs (Rol Único Tributario) chilenos.
 
 ## Características
```

### Comparing `rutificador-0.1.6/pyproject.toml` & `rutificador-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rutificador"
-version = "0.1.6"
+version = "0.2.0"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo"]
 classifiers = [
```

### Comparing `rutificador-0.1.6/rutificador/main.py` & `rutificador-0.2.0/rutificador/main.py`

 * *Files identical despite different names*

### Comparing `rutificador-0.1.6/PKG-INFO` & `rutificador-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rutificador
-Version: 0.1.6
+Version: 0.2.0
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://
 License: MIT
 Keywords: RUT,Chile,validación,formateo
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -19,15 +19,15 @@
 Classifier: Topic :: Utilities
 Project-URL: Repository, https://github.com/cortega26/Rutificador
 Description-Content-Type: text/markdown
 
 [![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
 [![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Build Status](URL_DE_LA_BADGE)](URL_A_LA_ACTION)
+[![CI Workflow](https://github.com/cortega26/rutificador/actions/workflows/ci.yml/badge.svg)](https://github.com/cortega26/rutificador/actions/workflows/ci.yml)
 
 # Rutificador
 
 Una biblioteca Python para validar y formatear RUTs (Rol Único Tributario) chilenos.
 
 ## Características
```


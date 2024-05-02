# Comparing `tmp/rutificador-0.1.4.tar.gz` & `tmp/rutificador-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.1.4.tar", max compression
+gzip compressed data, was "rutificador-0.1.5.tar", max compression
```

## Comparing `rutificador-0.1.4.tar` & `rutificador-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-02 23:48:54.683780 rutificador-0.1.4/LICENSE
--rw-r--r--   0        0        0     4120 2024-05-02 23:48:54.683780 rutificador-0.1.4/README.md
--rw-r--r--   0        0        0     1071 2024-05-02 23:48:54.683780 rutificador-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       87 2024-05-02 23:48:54.683780 rutificador-0.1.4/rutificador/__init__.py
--rw-r--r--   0        0        0     9113 2024-05-02 23:48:54.683780 rutificador-0.1.4/rutificador/main.py
--rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 rutificador-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-02 23:50:58.918222 rutificador-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4120 2024-05-02 23:50:58.918222 rutificador-0.1.5/README.md
+-rw-r--r--   0        0        0     1071 2024-05-02 23:50:58.918222 rutificador-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-05-02 23:50:58.918222 rutificador-0.1.5/rutificador/__init__.py
+-rw-r--r--   0        0        0     9113 2024-05-02 23:50:58.922222 rutificador-0.1.5/rutificador/main.py
+-rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 rutificador-0.1.5/PKG-INFO
```

### Comparing `rutificador-0.1.4/LICENSE` & `rutificador-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.1.4/README.md` & `rutificador-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rutificador-0.1.4/pyproject.toml` & `rutificador-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rutificador"
-version = "0.1.4"
+version = "0.1.5"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo"]
 classifiers = [
```

### Comparing `rutificador-0.1.4/rutificador/main.py` & `rutificador-0.1.5/rutificador/main.py`

 * *Files identical despite different names*

### Comparing `rutificador-0.1.4/PKG-INFO` & `rutificador-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rutificador
-Version: 0.1.4
+Version: 0.1.5
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://
 License: MIT
 Keywords: RUT,Chile,validación,formateo
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
```


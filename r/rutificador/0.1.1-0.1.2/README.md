# Comparing `tmp/rutificador-0.1.1.tar.gz` & `tmp/rutificador-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.1.1.tar", max compression
+gzip compressed data, was "rutificador-0.1.2.tar", max compression
```

## Comparing `rutificador-0.1.1.tar` & `rutificador-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-02 22:02:35.638292 rutificador-0.1.1/LICENSE
--rw-r--r--   0        0        0     4238 2024-05-02 22:02:35.638292 rutificador-0.1.1/README.md
--rw-r--r--   0        0        0     1072 2024-05-02 22:02:35.638292 rutificador-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       87 2024-05-02 22:02:35.638292 rutificador-0.1.1/rutificador/__init__.py
--rw-r--r--   0        0        0     9113 2024-05-02 22:02:35.638292 rutificador-0.1.1/rutificador/main.py
--rw-r--r--   0        0        0     5149 1970-01-01 00:00:00.000000 rutificador-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-02 22:30:46.671946 rutificador-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4506 2024-05-02 22:30:46.671946 rutificador-0.1.2/README.md
+-rw-r--r--   0        0        0     1072 2024-05-02 22:30:46.671946 rutificador-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-05-02 22:30:46.671946 rutificador-0.1.2/rutificador/__init__.py
+-rw-r--r--   0        0        0     9113 2024-05-02 22:30:46.671946 rutificador-0.1.2/rutificador/main.py
+-rw-r--r--   0        0        0     5417 1970-01-01 00:00:00.000000 rutificador-0.1.2/PKG-INFO
```

### Comparing `rutificador-0.1.1/LICENSE` & `rutificador-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.1.1/README.md` & `rutificador-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 9876543-3
 1234567-4
 18005183-k
 ```
 
 ## Contribuciones
 
-Las contribuciones son bienvenidas. Para colaborar solo debes abrir un 'issue' con el aporte deseado.
+Las contribuciones son bienvenidas. Para colaborar solo debes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, hacer el commit, el push y el pull request para migrar los cambios al 'master'. Finalmente, asegúrate de describir los cambios que realizaste y por qué crees son necesarios.
 
 ## Licencia
 
 Este proyecto está licenciado bajo la Licencia MIT.
 
 ## Créditos
```

### Comparing `rutificador-0.1.1/pyproject.toml` & `rutificador-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rutificador"
-version = "0.1.01"
+version = "0.1.02"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo"]
 classifiers = [
```

### Comparing `rutificador-0.1.1/rutificador/main.py` & `rutificador-0.1.2/rutificador/main.py`

 * *Files identical despite different names*

### Comparing `rutificador-0.1.1/PKG-INFO` & `rutificador-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rutificador
-Version: 0.1.1
+Version: 0.1.2
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://
 License: MIT
 Keywords: RUT,Chile,validación,formateo
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -148,15 +148,15 @@
 9876543-3
 1234567-4
 18005183-k
 ```
 
 ## Contribuciones
 
-Las contribuciones son bienvenidas. Para colaborar solo debes abrir un 'issue' con el aporte deseado.
+Las contribuciones son bienvenidas. Para colaborar solo debes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, hacer el commit, el push y el pull request para migrar los cambios al 'master'. Finalmente, asegúrate de describir los cambios que realizaste y por qué crees son necesarios.
 
 ## Licencia
 
 Este proyecto está licenciado bajo la Licencia MIT.
 
 ## Créditos
```


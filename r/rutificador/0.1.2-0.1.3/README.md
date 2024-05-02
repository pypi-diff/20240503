# Comparing `tmp/rutificador-0.1.2.tar.gz` & `tmp/rutificador-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.1.2.tar", max compression
+gzip compressed data, was "rutificador-0.1.3.tar", max compression
```

## Comparing `rutificador-0.1.2.tar` & `rutificador-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-02 22:30:46.671946 rutificador-0.1.2/LICENSE
--rw-r--r--   0        0        0     4506 2024-05-02 22:30:46.671946 rutificador-0.1.2/README.md
--rw-r--r--   0        0        0     1072 2024-05-02 22:30:46.671946 rutificador-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       87 2024-05-02 22:30:46.671946 rutificador-0.1.2/rutificador/__init__.py
--rw-r--r--   0        0        0     9113 2024-05-02 22:30:46.671946 rutificador-0.1.2/rutificador/main.py
--rw-r--r--   0        0        0     5417 1970-01-01 00:00:00.000000 rutificador-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-02 23:41:01.721048 rutificador-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4068 2024-05-02 23:41:01.721048 rutificador-0.1.3/README.md
+-rw-r--r--   0        0        0     1071 2024-05-02 23:41:01.721048 rutificador-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-05-02 23:41:01.721048 rutificador-0.1.3/rutificador/__init__.py
+-rw-r--r--   0        0        0     9113 2024-05-02 23:41:01.721048 rutificador-0.1.3/rutificador/main.py
+-rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 rutificador-0.1.3/PKG-INFO
```

### Comparing `rutificador-0.1.2/LICENSE` & `rutificador-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.1.2/README.md` & `rutificador-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 - **Separación de resultados:** Los resultados de los lotes se entregan por separado, mostrando RUTs válidos e inválidos, y pueden exportarse en varios formatos, incluidos CSV, XML y JSON.
 
 ## Instalación
 
 Puedes instalar la librería utilizando pip:
 
 ```python
-!pip install rutificador
+pip install rutificador
 ```
 
 ## Uso
 
 ### Importar la clase Rut
 
 ```python
@@ -71,21 +71,19 @@
 ## Validar y Formatear una lista de RUTs con y sin formato
 
 ```python
 # Sin formato
 ruts = ['12345678-5', '12345670-k', '98765432-1']
 ruts_validos = Rut.validar_lista_ruts(ruts)
 print(Rut.formatear_lista_ruts(ruts_validos, separador_miles=True, mayusculas=True))
-# Salida: 
+# Salida:
+# RUTs válidos:
 # 12.345.678-5
 # 12.345.670-K
 # 98.765.432-1
-# En caso de que hayan RUTs inválidos, el método validar_lista_ruts creará un diccionario dos listas:
-# una lista con los RUTs válidos (en el formato especificado) y otra con los inválidos.
-
 
 # En formato csv
 ruts = ['12.345.678', '9876543', '1.234.567-4', '18005183']
 csv_ruts = Rut.formatear_lista_ruts(ruts, formato='csv')
 print(csv_ruts)
 # Salida
 RUTs válidos:
@@ -111,25 +109,14 @@
 RUTs válidos:
 <root>
     <rut>12345678-5</rut>
     <rut>9876543-3</rut>
     <rut>1234567-4</rut>
     <rut>18005183-k</rut>
 </root>
-
-# Formato predeterminado (formato = None)
-ruts = ['12.345.678', '9876543', '1.234.567-4', '18005183']
-sin_formato_ruts = Rut.formatear_lista_ruts(ruts, formato=None)
-print(sin_formato_ruts)
-# Salida
-RUTs válidos:
-12345678-5
-9876543-3
-1234567-4
-18005183-k
 ```
 
 ## Contribuciones
 
 Las contribuciones son bienvenidas. Para colaborar solo debes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, hacer el commit, el push y el pull request para migrar los cambios al 'master'. Finalmente, asegúrate de describir los cambios que realizaste y por qué crees son necesarios.
 
 ## Licencia
```

### Comparing `rutificador-0.1.2/pyproject.toml` & `rutificador-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rutificador"
-version = "0.1.02"
+version = "0.1.3"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo"]
 classifiers = [
```

### Comparing `rutificador-0.1.2/rutificador/main.py` & `rutificador-0.1.3/rutificador/main.py`

 * *Files identical despite different names*

### Comparing `rutificador-0.1.2/PKG-INFO` & `rutificador-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rutificador
-Version: 0.1.2
+Version: 0.1.3
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://
 License: MIT
 Keywords: RUT,Chile,validación,formateo
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -39,15 +39,15 @@
 - **Separación de resultados:** Los resultados de los lotes se entregan por separado, mostrando RUTs válidos e inválidos, y pueden exportarse en varios formatos, incluidos CSV, XML y JSON.
 
 ## Instalación
 
 Puedes instalar la librería utilizando pip:
 
 ```python
-!pip install rutificador
+pip install rutificador
 ```
 
 ## Uso
 
 ### Importar la clase Rut
 
 ```python
@@ -93,21 +93,19 @@
 ## Validar y Formatear una lista de RUTs con y sin formato
 
 ```python
 # Sin formato
 ruts = ['12345678-5', '12345670-k', '98765432-1']
 ruts_validos = Rut.validar_lista_ruts(ruts)
 print(Rut.formatear_lista_ruts(ruts_validos, separador_miles=True, mayusculas=True))
-# Salida: 
+# Salida:
+# RUTs válidos:
 # 12.345.678-5
 # 12.345.670-K
 # 98.765.432-1
-# En caso de que hayan RUTs inválidos, el método validar_lista_ruts creará un diccionario dos listas:
-# una lista con los RUTs válidos (en el formato especificado) y otra con los inválidos.
-
 
 # En formato csv
 ruts = ['12.345.678', '9876543', '1.234.567-4', '18005183']
 csv_ruts = Rut.formatear_lista_ruts(ruts, formato='csv')
 print(csv_ruts)
 # Salida
 RUTs válidos:
@@ -133,25 +131,14 @@
 RUTs válidos:
 <root>
     <rut>12345678-5</rut>
     <rut>9876543-3</rut>
     <rut>1234567-4</rut>
     <rut>18005183-k</rut>
 </root>
-
-# Formato predeterminado (formato = None)
-ruts = ['12.345.678', '9876543', '1.234.567-4', '18005183']
-sin_formato_ruts = Rut.formatear_lista_ruts(ruts, formato=None)
-print(sin_formato_ruts)
-# Salida
-RUTs válidos:
-12345678-5
-9876543-3
-1234567-4
-18005183-k
 ```
 
 ## Contribuciones
 
 Las contribuciones son bienvenidas. Para colaborar solo debes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, hacer el commit, el push y el pull request para migrar los cambios al 'master'. Finalmente, asegúrate de describir los cambios que realizaste y por qué crees son necesarios.
 
 ## Licencia
```


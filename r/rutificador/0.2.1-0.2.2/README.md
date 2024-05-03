# Comparing `tmp/rutificador-0.2.1.tar.gz` & `tmp/rutificador-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.2.1.tar", max compression
+gzip compressed data, was "rutificador-0.2.2.tar", max compression
```

## Comparing `rutificador-0.2.1.tar` & `rutificador-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-03 18:15:41.426793 rutificador-0.2.1/LICENSE
--rw-r--r--   0        0        0     4327 2024-05-03 18:15:41.426793 rutificador-0.2.1/README.md
--rw-r--r--   0        0        0     1071 2024-05-03 18:15:41.426793 rutificador-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       87 2024-05-03 18:15:41.426793 rutificador-0.2.1/rutificador/__init__.py
--rw-r--r--   0        0        0     9113 2024-05-03 18:15:41.430793 rutificador-0.2.1/rutificador/main.py
--rw-r--r--   0        0        0     5238 1970-01-01 00:00:00.000000 rutificador-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-03 19:30:05.621079 rutificador-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4332 2024-05-03 19:30:05.621079 rutificador-0.2.2/README.md
+-rw-r--r--   0        0        0     1071 2024-05-03 19:30:05.621079 rutificador-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-05-03 19:30:05.621079 rutificador-0.2.2/rutificador/__init__.py
+-rw-r--r--   0        0        0     9113 2024-05-03 19:30:05.621079 rutificador-0.2.2/rutificador/main.py
+-rw-r--r--   0        0        0     5243 1970-01-01 00:00:00.000000 rutificador-0.2.2/PKG-INFO
```

### Comparing `rutificador-0.2.1/LICENSE` & `rutificador-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.2.1/README.md` & `rutificador-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,35 +30,35 @@
 
 ### Importar la clase Rut
 
 ```python
 from rutificador import Rut
 ```
 
-## Crear Un Objeto
+### Crear Un Objeto
 
 ```python
 rut1 = Rut('12345678-5')
 rut2 = Rut('12.345.670')
 ```
 
-## Validar un RUT
+### Validar un RUT
 
 La validación del RUT se realiza automáticamente al crear un objeto `Rut`. La clase 'Rut' acepta RUTs con y sin dígito verificador así como RUTs con y sin separador de miles. Si el RUT ingresado no es válido, se lanzará una excepción `RutInvalidoError`.
 
-## Calcular el Dígito Verificador de un RUT
+### Calcular el Dígito Verificador de un RUT
 
 ```python
 from rutificador import RutDigitoVerificador
 
 digito_verificador = RutDigitoVerificador('12345678').digito_verificador
 print(digito_verificador)  # Salida: 5
 ```
 
-## Formatear un RUT
+### Formatear un RUT
 
 ```python
 # Formato predeterminado
 print(rut1.formatear())  # Salida: 12345678-5
 
 # Con separador de miles
 print(rut1.formatear(separador_miles=True))  # Salida: 12.345.678-5
@@ -66,15 +66,15 @@
 # Formato predeterminado (Rut con dígito verificador = 'k')
 print(rut2.formatear())  # Salida: 12345670-k
 
 # Con separador de miles y en mayúsculas
 print(rut2.formatear(separador_miles=True, mayusculas=True))  # Salida: 12.345.670-K
 ```
 
-## Validar y Formatear una lista de RUTs con y sin formato
+### Validar y Formatear una lista de RUTs con y sin formato
 
 ```python
 # Sin formato
 ruts = ['12345678-5', '12345670-k', '98765432-1']
 ruts_validos = Rut.validar_lista_ruts(ruts)
 print(Rut.formatear_lista_ruts(ruts_validos, separador_miles=True, mayusculas=True))
 # Salida:
```

### Comparing `rutificador-0.2.1/pyproject.toml` & `rutificador-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rutificador"
-version = "0.2.1"
+version = "0.2.2"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo"]
 classifiers = [
```

### Comparing `rutificador-0.2.1/rutificador/main.py` & `rutificador-0.2.2/rutificador/main.py`

 * *Files identical despite different names*

### Comparing `rutificador-0.2.1/PKG-INFO` & `rutificador-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rutificador
-Version: 0.2.1
+Version: 0.2.2
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://
 License: MIT
 Keywords: RUT,Chile,validación,formateo
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -52,35 +52,35 @@
 
 ### Importar la clase Rut
 
 ```python
 from rutificador import Rut
 ```
 
-## Crear Un Objeto
+### Crear Un Objeto
 
 ```python
 rut1 = Rut('12345678-5')
 rut2 = Rut('12.345.670')
 ```
 
-## Validar un RUT
+### Validar un RUT
 
 La validación del RUT se realiza automáticamente al crear un objeto `Rut`. La clase 'Rut' acepta RUTs con y sin dígito verificador así como RUTs con y sin separador de miles. Si el RUT ingresado no es válido, se lanzará una excepción `RutInvalidoError`.
 
-## Calcular el Dígito Verificador de un RUT
+### Calcular el Dígito Verificador de un RUT
 
 ```python
 from rutificador import RutDigitoVerificador
 
 digito_verificador = RutDigitoVerificador('12345678').digito_verificador
 print(digito_verificador)  # Salida: 5
 ```
 
-## Formatear un RUT
+### Formatear un RUT
 
 ```python
 # Formato predeterminado
 print(rut1.formatear())  # Salida: 12345678-5
 
 # Con separador de miles
 print(rut1.formatear(separador_miles=True))  # Salida: 12.345.678-5
@@ -88,15 +88,15 @@
 # Formato predeterminado (Rut con dígito verificador = 'k')
 print(rut2.formatear())  # Salida: 12345670-k
 
 # Con separador de miles y en mayúsculas
 print(rut2.formatear(separador_miles=True, mayusculas=True))  # Salida: 12.345.670-K
 ```
 
-## Validar y Formatear una lista de RUTs con y sin formato
+### Validar y Formatear una lista de RUTs con y sin formato
 
 ```python
 # Sin formato
 ruts = ['12345678-5', '12345670-k', '98765432-1']
 ruts_validos = Rut.validar_lista_ruts(ruts)
 print(Rut.formatear_lista_ruts(ruts_validos, separador_miles=True, mayusculas=True))
 # Salida:
```


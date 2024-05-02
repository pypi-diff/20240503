# Comparing `tmp/soroban-0.7.0.tar.gz` & `tmp/soroban-0.7.1.tar.gz`

## Comparing `soroban-0.7.0.tar` & `soroban-0.7.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 soroban-0.7.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 soroban-0.7.0/tea.yaml
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/cli.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/create.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/deploy.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/invoke.py
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/models.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 soroban-0.7.0/.gitignore
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soroban-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 soroban-0.7.0/README.md
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 soroban-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 soroban-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 soroban-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 soroban-0.7.1/tea.yaml
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 soroban-0.7.1/src/soroban/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 soroban-0.7.1/src/soroban/cli.py
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 soroban-0.7.1/src/soroban/create.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 soroban-0.7.1/src/soroban/deploy.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 soroban-0.7.1/src/soroban/invoke.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 soroban-0.7.1/src/soroban/models.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 soroban-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soroban-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 soroban-0.7.1/README.md
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 soroban-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 soroban-0.7.1/PKG-INFO
```

### Comparing `soroban-0.7.0/CONTRIBUTING.md` & `soroban-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `soroban-0.7.0/src/soroban/cli.py` & `soroban-0.7.1/src/soroban/cli.py`

 * *Files identical despite different names*

### Comparing `soroban-0.7.0/src/soroban/create.py` & `soroban-0.7.1/src/soroban/create.py`

 * *Files identical despite different names*

### Comparing `soroban-0.7.0/src/soroban/deploy.py` & `soroban-0.7.1/src/soroban/deploy.py`

 * *Files identical despite different names*

### Comparing `soroban-0.7.0/src/soroban/invoke.py` & `soroban-0.7.1/src/soroban/invoke.py`

 * *Files identical despite different names*

### Comparing `soroban-0.7.0/src/soroban/models.py` & `soroban-0.7.1/src/soroban/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,20 +105,20 @@
         return network
 
 
 class Argument(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     type: str
-    value: int | str | xdr.SCVal
+    value: int | bytes | str | xdr.SCVal
 
 
 class Parameter(Argument):
     name: str
-    value: int | str | xdr.SCVal | list[Argument | xdr.SCVal]
+    value: int | bytes | str | xdr.SCVal | list[Argument | xdr.SCVal]
 
     @model_validator(mode="after")
     def value_to_scval(self) -> "Parameter":
         if isinstance(self.value, list):
             self.value = [self._value_to_scval(val) for val in self.value]
         self.value = self._value_to_scval(self)
         return self
```

### Comparing `soroban-0.7.0/LICENSE.txt` & `soroban-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soroban-0.7.0/README.md` & `soroban-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `soroban-0.7.0/pyproject.toml` & `soroban-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soroban-0.7.0/PKG-INFO` & `soroban-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: soroban
-Version: 0.7.0
+Version: 0.7.1
 Summary: API and CLI for Soroban contracts in Python
 Project-URL: homepage, https://github.com/tupui/soroban-cli-python
 Project-URL: documentation, https://github.com/tupui/soroban-cli-python
 Project-URL: source, https://github.com/tupui/soroban-cli-python
 Author: Pamphile Roy
 Maintainer: Soroban API/CLI contributors
 License-Expression: BSD-3-Clause
```


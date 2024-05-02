# Comparing `tmp/soroban-0.5.0.tar.gz` & `tmp/soroban-0.6.0.tar.gz`

## Comparing `soroban-0.5.0.tar` & `soroban-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 soroban-0.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 soroban-0.5.0/tea.yaml
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 soroban-0.5.0/src/soroban/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 soroban-0.5.0/src/soroban/cli.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 soroban-0.5.0/src/soroban/create.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 soroban-0.5.0/src/soroban/invoke.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 soroban-0.5.0/src/soroban/models.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 soroban-0.5.0/.gitignore
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soroban-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 soroban-0.5.0/README.md
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 soroban-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 soroban-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 soroban-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 soroban-0.6.0/tea.yaml
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/cli.py
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/create.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/deploy.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/invoke.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/models.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 soroban-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soroban-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 soroban-0.6.0/README.md
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 soroban-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 soroban-0.6.0/PKG-INFO
```

### Comparing `soroban-0.5.0/CONTRIBUTING.md` & `soroban-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `soroban-0.5.0/src/soroban/cli.py` & `soroban-0.6.0/src/soroban/cli.py`

 * *Files identical despite different names*

### Comparing `soroban-0.5.0/src/soroban/create.py` & `soroban-0.6.0/src/soroban/create.py`

 * *Files identical despite different names*

### Comparing `soroban-0.5.0/src/soroban/invoke.py` & `soroban-0.6.0/src/soroban/invoke.py`

 * *Files identical despite different names*

### Comparing `soroban-0.5.0/src/soroban/models.py` & `soroban-0.6.0/src/soroban/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class Identity(BaseSettings):
     seed_phrase: str | None = None
     secret_key: str | None = None
     public_key: str | None = None
     keypair: Keypair | None = None
 
     model_config = SettingsConfigDict(
-        env_file=["identity.toml", ".soroban/identity.toml"]
+        env_file=["identity.toml", ".soroban/identity/identity.toml"]
     )
 
     @model_validator(mode="after")
     def load_keys(self) -> "Identity":
         if (
             self.keypair is None
             and self.secret_key is None
```

### Comparing `soroban-0.5.0/LICENSE.txt` & `soroban-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soroban-0.5.0/README.md` & `soroban-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `soroban-0.5.0/pyproject.toml` & `soroban-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soroban-0.5.0/PKG-INFO` & `soroban-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: soroban
-Version: 0.5.0
+Version: 0.6.0
 Summary: API and CLI for Soroban contracts in Python
 Project-URL: homepage, https://github.com/tupui/soroban-cli-python
 Project-URL: documentation, https://github.com/tupui/soroban-cli-python
 Project-URL: source, https://github.com/tupui/soroban-cli-python
 Author: Pamphile Roy
 Maintainer: Soroban API/CLI contributors
 License-Expression: BSD-3-Clause
```


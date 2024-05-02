# Comparing `tmp/soroban-0.4.0.tar.gz` & `tmp/soroban-0.5.0.tar.gz`

## Comparing `soroban-0.4.0.tar` & `soroban-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 soroban-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 soroban-0.4.0/tea.yaml
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 soroban-0.4.0/src/soroban/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 soroban-0.4.0/src/soroban/cli.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 soroban-0.4.0/src/soroban/create.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 soroban-0.4.0/src/soroban/invoke.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 soroban-0.4.0/src/soroban/models.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 soroban-0.4.0/.gitignore
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soroban-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 soroban-0.4.0/README.md
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 soroban-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 soroban-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 soroban-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 soroban-0.5.0/tea.yaml
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 soroban-0.5.0/src/soroban/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 soroban-0.5.0/src/soroban/cli.py
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 soroban-0.5.0/src/soroban/create.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 soroban-0.5.0/src/soroban/invoke.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 soroban-0.5.0/src/soroban/models.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 soroban-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soroban-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 soroban-0.5.0/README.md
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 soroban-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 soroban-0.5.0/PKG-INFO
```

### Comparing `soroban-0.4.0/CONTRIBUTING.md` & `soroban-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `soroban-0.4.0/src/soroban/cli.py` & `soroban-0.5.0/src/soroban/cli.py`

 * *Files identical despite different names*

### Comparing `soroban-0.4.0/src/soroban/create.py` & `soroban-0.5.0/src/soroban/create.py`

 * *Files identical despite different names*

### Comparing `soroban-0.4.0/src/soroban/invoke.py` & `soroban-0.5.0/src/soroban/invoke.py`

 * *Files identical despite different names*

### Comparing `soroban-0.4.0/src/soroban/models.py` & `soroban-0.5.0/src/soroban/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,31 +23,40 @@
     elif global_config.is_file():
         return global_config
     else:
         raise ValueError(f"Cannot find a {kind!r} configuration for {id!r}")
 
 
 class Identity(BaseSettings):
+    seed_phrase: str | None = None
     secret_key: str | None = None
     public_key: str | None = None
     keypair: Keypair | None = None
 
-    model_config = SettingsConfigDict(env_file="identity.toml")
+    model_config = SettingsConfigDict(
+        env_file=["identity.toml", ".soroban/identity.toml"]
+    )
 
     @model_validator(mode="after")
     def load_keys(self) -> "Identity":
-        if self.keypair is None and self.secret_key is None:
+        if (
+            self.keypair is None
+            and self.secret_key is None
+            and self.seed_phrase is None
+        ):
             raise ValueError(
-                "Either provide a secret key or a Keypair object. Also look"
+                "Either provide a seed phrase, secret key or a Keypair object. Also look"
                 "in 'identity.toml'"
             )
         if self.keypair is not None:
             self.secret_key = self.keypair.secret
-        else:
+        elif self.secret_key is not None:
             self.keypair = Keypair.from_secret(self.secret_key)
+        else:
+            self.keypair = Keypair.from_mnemonic_phrase(self.seed_phrase)
         self.public_key = self.keypair.public_key
         return self
 
     @classmethod
     def from_source_account(
         cls, account: Keypair | str | pathlib.Path | None = None
     ) -> "Identity":
```

### Comparing `soroban-0.4.0/LICENSE.txt` & `soroban-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soroban-0.4.0/README.md` & `soroban-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `soroban-0.4.0/pyproject.toml` & `soroban-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -88,9 +88,9 @@
 
 [tool.pytest.ini_options]
 addopts = "--durations 10"
 testpaths = [
     "tests",
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "**/__init__.py" = ["F403", "F405"]
```

### Comparing `soroban-0.4.0/PKG-INFO` & `soroban-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: soroban
-Version: 0.4.0
+Version: 0.5.0
 Summary: API and CLI for Soroban contracts in Python
 Project-URL: homepage, https://github.com/tupui/soroban-cli-python
 Project-URL: documentation, https://github.com/tupui/soroban-cli-python
 Project-URL: source, https://github.com/tupui/soroban-cli-python
 Author: Pamphile Roy
 Maintainer: Soroban API/CLI contributors
 License-Expression: BSD-3-Clause
@@ -23,15 +23,17 @@
 Requires-Dist: stellar-sdk
 Requires-Dist: tomli-w
 Provides-Extra: cli
 Requires-Dist: typer[all]; extra == 'cli'
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
-Requires-Dist: soroban[cli,tests]; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: typer[all]; extra == 'dev'
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # API and CLI for Soroban contracts in Python
```


# Comparing `tmp/soroban-0.6.0.tar.gz` & `tmp/soroban-0.7.0.tar.gz`

## Comparing `soroban-0.6.0.tar` & `soroban-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 soroban-0.6.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 soroban-0.6.0/tea.yaml
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/cli.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/create.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/deploy.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/invoke.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 soroban-0.6.0/src/soroban/models.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 soroban-0.6.0/.gitignore
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soroban-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 soroban-0.6.0/README.md
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 soroban-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 soroban-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 soroban-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 soroban-0.7.0/tea.yaml
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/cli.py
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/create.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/deploy.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/invoke.py
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 soroban-0.7.0/src/soroban/models.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 soroban-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soroban-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 soroban-0.7.0/README.md
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 soroban-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 soroban-0.7.0/PKG-INFO
```

### Comparing `soroban-0.6.0/CONTRIBUTING.md` & `soroban-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `soroban-0.6.0/src/soroban/cli.py` & `soroban-0.7.0/src/soroban/cli.py`

 * *Files identical despite different names*

### Comparing `soroban-0.6.0/src/soroban/create.py` & `soroban-0.7.0/src/soroban/create.py`

 * *Files identical despite different names*

### Comparing `soroban-0.6.0/src/soroban/deploy.py` & `soroban-0.7.0/src/soroban/deploy.py`

 * *Files identical despite different names*

### Comparing `soroban-0.6.0/src/soroban/invoke.py` & `soroban-0.7.0/src/soroban/invoke.py`

 * *Files identical despite different names*

### Comparing `soroban-0.6.0/src/soroban/models.py` & `soroban-0.7.0/src/soroban/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 class Identity(BaseSettings):
     seed_phrase: str | None = None
     secret_key: str | None = None
     public_key: str | None = None
     keypair: Keypair | None = None
 
     model_config = SettingsConfigDict(
-        env_file=["identity.toml", ".soroban/identity/identity.toml"]
+        env_file=[
+            "identity.toml",
+            pathlib.Path(".soroban") / "identity" / "identity.toml",
+        ]
     )
 
     @model_validator(mode="after")
     def load_keys(self) -> "Identity":
         if (
             self.keypair is None
             and self.secret_key is None
@@ -77,15 +80,17 @@
 class NetworkConfig(BaseSettings):
     # https://horizon.publicnode.org
     horizon_url: HttpUrl = HttpUrl("https://horizon-testnet.stellar.org")
     rpc_url: HttpUrl = HttpUrl("https://soroban-testnet.stellar.org")
     network_passphrase: str = Network.TESTNET_NETWORK_PASSPHRASE
     base_fee: int = 100
 
-    model_config = SettingsConfigDict(env_file="network.toml")
+    model_config = SettingsConfigDict(
+        env_file=["network.toml", pathlib.Path(".soroban") / "network" / "network.toml"]
+    )
 
     @model_validator(mode="after")
     def load_urls(self) -> "NetworkConfig":
         # or use the Annotated construction
         self.horizon_url = str(self.horizon_url)
         self.rpc_url = str(self.rpc_url)
         return self
```

### Comparing `soroban-0.6.0/LICENSE.txt` & `soroban-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soroban-0.6.0/README.md` & `soroban-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 ```python
 import soroban
 
 soroban.invoke(contract_id="AAAA...", function_name="increment")
 ```
 
-Identity and Network configurations are automatically pulled from the global
-or local configuration.
+Identity and Network configurations are automatically pulled from the
+local configuration or the current working directory. See bellow.
 
 It also provides a CLI
 ```shell
 soroban invoke C... version --source-account=...
 ```
 
 ## Usage
```

### Comparing `soroban-0.6.0/pyproject.toml` & `soroban-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soroban-0.6.0/PKG-INFO` & `soroban-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: soroban
-Version: 0.6.0
+Version: 0.7.0
 Summary: API and CLI for Soroban contracts in Python
 Project-URL: homepage, https://github.com/tupui/soroban-cli-python
 Project-URL: documentation, https://github.com/tupui/soroban-cli-python
 Project-URL: source, https://github.com/tupui/soroban-cli-python
 Author: Pamphile Roy
 Maintainer: Soroban API/CLI contributors
 License-Expression: BSD-3-Clause
@@ -53,16 +53,16 @@
 
 ```python
 import soroban
 
 soroban.invoke(contract_id="AAAA...", function_name="increment")
 ```
 
-Identity and Network configurations are automatically pulled from the global
-or local configuration.
+Identity and Network configurations are automatically pulled from the
+local configuration or the current working directory. See bellow.
 
 It also provides a CLI
 ```shell
 soroban invoke C... version --source-account=...
 ```
 
 ## Usage
```


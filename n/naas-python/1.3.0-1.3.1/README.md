# Comparing `tmp/naas_python-1.3.0.tar.gz` & `tmp/naas_python-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naas_python-1.3.0.tar", max compression
+gzip compressed data, was "naas_python-1.3.1.tar", max compression
```

## Comparing `naas_python-1.3.0.tar` & `naas_python-1.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    34523 2024-03-18 08:41:16.109238 naas_python-1.3.0/LICENSE
--rw-r--r--   0        0        0       13 2024-03-18 08:41:16.109238 naas_python-1.3.0/README.md
--rw-r--r--   0        0        0      303 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/__init__.py
--rw-r--r--   0        0        0     1030 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/cli.py
--rw-r--r--   0        0        0     1398 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/registry/RegistryDomain.py
--rw-r--r--   0        0        0     2174 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/registry/RegistrySchema.py
--rw-r--r--   0        0        0     2006 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/registry/adaptors/primary/SDKRegistryAdaptor.py
--rw-r--r--   0        0        0     7354 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/registry/adaptors/primary/TyperRegistryAdaptor.py
--rw-r--r--   0        0        0     6393 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/registry/adaptors/secondary/NaasRegistryAPIAdaptor.py
--rw-r--r--   0        0        0      329 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/registry/handlers/CLIRegistryHandler.py
--rw-r--r--   0        0        0      323 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/registry/handlers/PythonHandler.py
--rw-r--r--   0        0        0     1220 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/secret/SecretDomain.py
--rw-r--r--   0        0        0     2119 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/secret/SecretSchema.py
--rw-r--r--   0        0        0     1392 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/secret/adaptors/primary/SDKSecretAdaptor.py
--rw-r--r--   0        0        0     5705 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/secret/adaptors/primary/TyperSecretAdaptor.py
--rw-r--r--   0        0        0     1331 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/secret/adaptors/primary/utils.py
--rw-r--r--   0        0        0     4660 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/secret/adaptors/secondary/NaasSecretAPIAdaptor.py
--rw-r--r--   0        0        0      523 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/secret/handlers/CLISecretHandler.py
--rw-r--r--   0        0        0      305 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/secret/handlers/PythonHandler.py
--rw-r--r--   0        0        0       45 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/secret/models/Secret.py
--rw-r--r--   0        0        0       26 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/secret/models/__init__.py
--rw-r--r--   0        0        0     1251 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/space/SpaceDomain.py
--rw-r--r--   0        0        0     2192 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/space/SpaceSchema.py
--rw-r--r--   0        0        0     7702 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/space/adaptors/primary/SDKSpaceAdaptor.py
--rw-r--r--   0        0        0    17679 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/space/adaptors/primary/TyperSpaceAdaptor.py
--rw-r--r--   0        0        0     1329 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/space/adaptors/primary/utils.py
--rw-r--r--   0        0        0     7609 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/space/adaptors/secondary/NaasSpaceAPIAdaptor.py
--rw-r--r--   0        0        0      512 2024-03-18 08:41:16.109238 naas_python-1.3.0/naas_python/domains/space/handlers/CLISpaceHandler.py
--rw-r--r--   0        0        0      296 2024-03-18 08:41:16.113238 naas_python-1.3.0/naas_python/domains/space/handlers/PythonHandler.py
--rw-r--r--   0        0        0       96 2024-03-18 08:41:16.113238 naas_python-1.3.0/naas_python/main.py
--rw-r--r--   0        0        0        0 2024-03-18 08:41:16.113238 naas_python-1.3.0/naas_python/utils/__init__.py
--rw-r--r--   0        0        0     2039 2024-03-18 08:41:16.113238 naas_python-1.3.0/naas_python/utils/cicd.py
--rw-r--r--   0        0        0        0 2024-03-18 08:41:16.113238 naas_python-1.3.0/naas_python/utils/domains_base/__init__.py
--rw-r--r--   0        0        0    15947 2024-03-18 08:41:16.113238 naas_python-1.3.0/naas_python/utils/domains_base/authorization.py
--rw-r--r--   0        0        0     4022 2024-03-18 08:41:16.113238 naas_python-1.3.0/naas_python/utils/domains_base/secondary/BaseAPIAdaptor.py
--rw-r--r--   0        0        0     3203 2024-03-18 08:41:16.113238 naas_python-1.3.0/naas_python/utils/exceptions.py
--rw-r--r--   0        0        0     1873 2024-03-18 08:41:16.113238 naas_python-1.3.0/naas_python/utils/log.py
--rw-r--r--   0        0        0      357 2024-03-18 08:41:16.113238 naas_python-1.3.0/naas_python/utils/workflow_template.j2
--rw-r--r--   0        0        0      856 2024-03-18 08:41:28.901217 naas_python-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 naas_python-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-19 08:02:25.540377 naas_python-1.3.1/LICENSE
+-rw-r--r--   0        0        0       13 2024-03-19 08:02:25.540377 naas_python-1.3.1/README.md
+-rw-r--r--   0        0        0      303 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/__init__.py
+-rw-r--r--   0        0        0     1030 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/cli.py
+-rw-r--r--   0        0        0     1398 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/registry/RegistryDomain.py
+-rw-r--r--   0        0        0     2174 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/registry/RegistrySchema.py
+-rw-r--r--   0        0        0     2006 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/registry/adaptors/primary/SDKRegistryAdaptor.py
+-rw-r--r--   0        0        0     7354 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/registry/adaptors/primary/TyperRegistryAdaptor.py
+-rw-r--r--   0        0        0     6393 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/registry/adaptors/secondary/NaasRegistryAPIAdaptor.py
+-rw-r--r--   0        0        0      329 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/registry/handlers/CLIRegistryHandler.py
+-rw-r--r--   0        0        0      323 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/registry/handlers/PythonHandler.py
+-rw-r--r--   0        0        0     1220 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/secret/SecretDomain.py
+-rw-r--r--   0        0        0     2119 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/secret/SecretSchema.py
+-rw-r--r--   0        0        0     1392 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/secret/adaptors/primary/SDKSecretAdaptor.py
+-rw-r--r--   0        0        0     5705 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/secret/adaptors/primary/TyperSecretAdaptor.py
+-rw-r--r--   0        0        0     1331 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/secret/adaptors/primary/utils.py
+-rw-r--r--   0        0        0     4660 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/secret/adaptors/secondary/NaasSecretAPIAdaptor.py
+-rw-r--r--   0        0        0      523 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/secret/handlers/CLISecretHandler.py
+-rw-r--r--   0        0        0      305 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/secret/handlers/PythonHandler.py
+-rw-r--r--   0        0        0       45 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/secret/models/Secret.py
+-rw-r--r--   0        0        0       26 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/secret/models/__init__.py
+-rw-r--r--   0        0        0     1251 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/space/SpaceDomain.py
+-rw-r--r--   0        0        0     2192 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/space/SpaceSchema.py
+-rw-r--r--   0        0        0     7702 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/space/adaptors/primary/SDKSpaceAdaptor.py
+-rw-r--r--   0        0        0    17679 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/space/adaptors/primary/TyperSpaceAdaptor.py
+-rw-r--r--   0        0        0     1329 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/space/adaptors/primary/utils.py
+-rw-r--r--   0        0        0     7609 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/space/adaptors/secondary/NaasSpaceAPIAdaptor.py
+-rw-r--r--   0        0        0      512 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/space/handlers/CLISpaceHandler.py
+-rw-r--r--   0        0        0      296 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/domains/space/handlers/PythonHandler.py
+-rw-r--r--   0        0        0       96 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/main.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/utils/__init__.py
+-rw-r--r--   0        0        0     2039 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/utils/cicd.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/utils/domains_base/__init__.py
+-rw-r--r--   0        0        0    15947 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/utils/domains_base/authorization.py
+-rw-r--r--   0        0        0     4022 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/utils/domains_base/secondary/BaseAPIAdaptor.py
+-rw-r--r--   0        0        0     3203 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/utils/exceptions.py
+-rw-r--r--   0        0        0     1873 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/utils/log.py
+-rw-r--r--   0        0        0      357 2024-03-19 08:02:25.540377 naas_python-1.3.1/naas_python/utils/workflow_template.j2
+-rw-r--r--   0        0        0      856 2024-03-19 08:02:38.792504 naas_python-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 naas_python-1.3.1/PKG-INFO
```

### Comparing `naas_python-1.3.0/LICENSE` & `naas_python-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/cli.py` & `naas_python-1.3.1/naas_python/cli.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/registry/RegistryDomain.py` & `naas_python-1.3.1/naas_python/domains/registry/RegistryDomain.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/registry/RegistrySchema.py` & `naas_python-1.3.1/naas_python/domains/registry/RegistrySchema.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/registry/adaptors/primary/SDKRegistryAdaptor.py` & `naas_python-1.3.1/naas_python/domains/registry/adaptors/primary/SDKRegistryAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/registry/adaptors/primary/TyperRegistryAdaptor.py` & `naas_python-1.3.1/naas_python/domains/registry/adaptors/primary/TyperRegistryAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/registry/adaptors/secondary/NaasRegistryAPIAdaptor.py` & `naas_python-1.3.1/naas_python/domains/registry/adaptors/secondary/NaasRegistryAPIAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/secret/SecretDomain.py` & `naas_python-1.3.1/naas_python/domains/secret/SecretDomain.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/secret/SecretSchema.py` & `naas_python-1.3.1/naas_python/domains/secret/SecretSchema.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/secret/adaptors/primary/SDKSecretAdaptor.py` & `naas_python-1.3.1/naas_python/domains/secret/adaptors/primary/SDKSecretAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/secret/adaptors/primary/TyperSecretAdaptor.py` & `naas_python-1.3.1/naas_python/domains/secret/adaptors/primary/TyperSecretAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/secret/adaptors/primary/utils.py` & `naas_python-1.3.1/naas_python/domains/secret/adaptors/primary/utils.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/secret/adaptors/secondary/NaasSecretAPIAdaptor.py` & `naas_python-1.3.1/naas_python/domains/secret/adaptors/secondary/NaasSecretAPIAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/secret/handlers/CLISecretHandler.py` & `naas_python-1.3.1/naas_python/domains/secret/handlers/CLISecretHandler.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/space/SpaceDomain.py` & `naas_python-1.3.1/naas_python/domains/space/SpaceDomain.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/space/SpaceSchema.py` & `naas_python-1.3.1/naas_python/domains/space/SpaceSchema.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/space/adaptors/primary/SDKSpaceAdaptor.py` & `naas_python-1.3.1/naas_python/domains/space/adaptors/primary/SDKSpaceAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/space/adaptors/primary/TyperSpaceAdaptor.py` & `naas_python-1.3.1/naas_python/domains/space/adaptors/primary/TyperSpaceAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/space/adaptors/primary/utils.py` & `naas_python-1.3.1/naas_python/domains/space/adaptors/primary/utils.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/space/adaptors/secondary/NaasSpaceAPIAdaptor.py` & `naas_python-1.3.1/naas_python/domains/space/adaptors/secondary/NaasSpaceAPIAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/domains/space/handlers/CLISpaceHandler.py` & `naas_python-1.3.1/naas_python/domains/space/handlers/CLISpaceHandler.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/utils/cicd.py` & `naas_python-1.3.1/naas_python/utils/cicd.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/utils/domains_base/authorization.py` & `naas_python-1.3.1/naas_python/utils/domains_base/authorization.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/utils/domains_base/secondary/BaseAPIAdaptor.py` & `naas_python-1.3.1/naas_python/utils/domains_base/secondary/BaseAPIAdaptor.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/utils/exceptions.py` & `naas_python-1.3.1/naas_python/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/naas_python/utils/log.py` & `naas_python-1.3.1/naas_python/utils/log.py`

 * *Files identical despite different names*

### Comparing `naas_python-1.3.0/pyproject.toml` & `naas_python-1.3.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "naas-python"
-version = "1.3.0"
+version = "1.3.1"
 description = "Naas Python SDK"
 authors = ["Maxime Jublou <maxime@naas.ai>"]
 license = "AGPL"
 readme = "README.md"
 packages = [{ include = "naas_python" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = { extras = ["all"], version = "^0.9.0" }
 requests = "^2.31.0"
 protobuf_to_pydantic = { version = "0.1.7.4" }
 cachetools = "^5.3.1"
 #naas-models = { git = "https://github.com/jupyter-naas/naas-models.git", tag = "v1.4.1", subdirectory = "python" }
 jinja2 = "^3.0.1"
-naas-models = "^1.4.1"
+naas-models = "^1.7.1"
 grpcio = "^1.60.0"
 pydash = "^7.0.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 requests = "^2.31.0"
 protobuf_to_pydantic = { version = "0.1.7.4" }
```

### Comparing `naas_python-1.3.0/PKG-INFO` & `naas_python-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: naas-python
-Version: 1.3.0
+Version: 1.3.1
 Summary: Naas Python SDK
 License: AGPL
 Author: Maxime Jublou
 Author-email: maxime@naas.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.0.1,<4.0.0)
-Requires-Dist: naas-models (>=1.4.1,<2.0.0)
+Requires-Dist: naas-models (>=1.7.1,<2.0.0)
 Requires-Dist: protobuf_to_pydantic (==0.1.7.4)
 Requires-Dist: pydash (>=7.0.7,<8.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # python-naas
```


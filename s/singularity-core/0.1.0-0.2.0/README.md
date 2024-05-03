# Comparing `tmp/singularity_core-0.1.0.tar.gz` & `tmp/singularity_core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singularity_core-0.1.0.tar", max compression
+gzip compressed data, was "singularity_core-0.2.0.tar", max compression
```

## Comparing `singularity_core-0.1.0.tar` & `singularity_core-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2024-03-24 20:43:29.699734 singularity_core-0.1.0/README.md
--rw-r--r--   0        0        0      781 2024-05-02 08:22:00.171277 singularity_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       68 2024-05-02 07:58:42.027765 singularity_core-0.1.0/singularity/__init__.py
--rw-r--r--   0        0        0     5095 2024-03-25 19:06:13.361933 singularity_core-0.1.0/singularity/config.py
--rw-r--r--   0        0        0        0 2024-03-25 13:04:54.065425 singularity_core-0.1.0/singularity/db/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 13:04:18.012332 singularity_core-0.1.0/singularity/db/mongo/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 21:10:42.790151 singularity_core-0.1.0/singularity/db/postgres/__init__.py
--rw-r--r--   0        0        0      490 2024-05-01 14:57:36.339766 singularity_core-0.1.0/singularity/db/postgres/main.py
--rw-r--r--   0        0        0     3988 2024-05-01 14:57:44.038615 singularity_core-0.1.0/singularity/db/postgres/models.py
--rw-r--r--   0        0        0     1352 2024-03-25 13:17:01.464925 singularity_core-0.1.0/singularity/db/postgres/schemas.py
--rw-r--r--   0        0        0      470 2024-05-01 14:57:47.173913 singularity_core-0.1.0/singularity/db/postgres/transactional.py
--rw-r--r--   0        0        0        0 2024-03-24 21:12:56.720132 singularity_core-0.1.0/singularity/exceptions/__init__.py
--rw-r--r--   0        0        0      584 2024-03-24 21:12:56.720560 singularity_core-0.1.0/singularity/exceptions/cache_exceptions.py
--rw-r--r--   0        0        0      272 2024-03-24 21:12:56.721639 singularity_core-0.1.0/singularity/exceptions/http_exceptions.py
--rw-r--r--   0        0        0      655 2024-03-24 21:11:58.447471 singularity_core-0.1.0/singularity/logger.py
--rw-r--r--   0        0        0     3271 2024-05-02 07:30:19.075475 singularity_core-0.1.0/singularity/main.py
--rw-r--r--   0        0        0     1905 2024-03-24 21:14:09.188974 singularity_core-0.1.0/singularity/middlewares/client_cache_middleware.py
--rw-r--r--   0        0        0     1313 2024-03-24 21:17:43.028912 singularity_core-0.1.0/singularity/schemas.py
--rw-r--r--   0        0        0      409 2024-03-29 05:52:16.255904 singularity_core-0.1.0/singularity/service.py
--rw-r--r--   0        0        0     7752 2024-03-25 13:23:50.148793 singularity_core-0.1.0/singularity/setup.py
--rw-r--r--   0        0        0        0 2024-03-24 21:13:05.898410 singularity_core-0.1.0/singularity/utils/__init__.py
--rw-r--r--   0        0        0    12867 2024-03-24 21:13:05.898657 singularity_core-0.1.0/singularity/utils/cache.py
--rw-r--r--   0        0        0       67 2024-03-24 21:13:05.899673 singularity_core-0.1.0/singularity/utils/queue.py
--rw-r--r--   0        0        0     1181 2024-05-01 14:57:50.337012 singularity_core-0.1.0/singularity/utils/rate_limit.py
--rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 singularity_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-24 20:43:29.699734 singularity_core-0.2.0/README.md
+-rw-r--r--   0        0        0      781 2024-05-03 16:18:53.503704 singularity_core-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       68 2024-05-02 07:58:42.027765 singularity_core-0.2.0/singularity/__init__.py
+-rw-r--r--   0        0        0     3267 2024-05-03 16:10:40.652232 singularity_core-0.2.0/singularity/config.py
+-rw-r--r--   0        0        0        0 2024-03-25 13:04:54.065425 singularity_core-0.2.0/singularity/db/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 13:04:18.012332 singularity_core-0.2.0/singularity/db/mongo/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 21:10:42.790151 singularity_core-0.2.0/singularity/db/postgres/__init__.py
+-rw-r--r--   0        0        0      499 2024-05-03 16:17:55.155120 singularity_core-0.2.0/singularity/db/postgres/main.py
+-rw-r--r--   0        0        0     3988 2024-05-01 14:57:44.038615 singularity_core-0.2.0/singularity/db/postgres/models.py
+-rw-r--r--   0        0        0     1352 2024-03-25 13:17:01.464925 singularity_core-0.2.0/singularity/db/postgres/schemas.py
+-rw-r--r--   0        0        0      470 2024-05-01 14:57:47.173913 singularity_core-0.2.0/singularity/db/postgres/transactional.py
+-rw-r--r--   0        0        0        0 2024-03-24 21:12:56.720132 singularity_core-0.2.0/singularity/exceptions/__init__.py
+-rw-r--r--   0        0        0      584 2024-03-24 21:12:56.720560 singularity_core-0.2.0/singularity/exceptions/cache_exceptions.py
+-rw-r--r--   0        0        0      272 2024-03-24 21:12:56.721639 singularity_core-0.2.0/singularity/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0      655 2024-03-24 21:11:58.447471 singularity_core-0.2.0/singularity/logger.py
+-rw-r--r--   0        0        0     3640 2024-05-03 16:17:03.652662 singularity_core-0.2.0/singularity/main.py
+-rw-r--r--   0        0        0     1905 2024-03-24 21:14:09.188974 singularity_core-0.2.0/singularity/middlewares/client_cache_middleware.py
+-rw-r--r--   0        0        0     1313 2024-03-24 21:17:43.028912 singularity_core-0.2.0/singularity/schemas.py
+-rw-r--r--   0        0        0      409 2024-03-29 05:52:16.255904 singularity_core-0.2.0/singularity/service.py
+-rw-r--r--   0        0        0     7752 2024-03-25 13:23:50.148793 singularity_core-0.2.0/singularity/setup.py
+-rw-r--r--   0        0        0        0 2024-03-24 21:13:05.898410 singularity_core-0.2.0/singularity/utils/__init__.py
+-rw-r--r--   0        0        0    12867 2024-03-24 21:13:05.898657 singularity_core-0.2.0/singularity/utils/cache.py
+-rw-r--r--   0        0        0       67 2024-03-24 21:13:05.899673 singularity_core-0.2.0/singularity/utils/queue.py
+-rw-r--r--   0        0        0     1181 2024-05-01 14:57:50.337012 singularity_core-0.2.0/singularity/utils/rate_limit.py
+-rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 singularity_core-0.2.0/PKG-INFO
```

### Comparing `singularity_core-0.1.0/pyproject.toml` & `singularity_core-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "singularity-core"
-version = "0.1.0"
+version = "0.2.0"
 description = "Funny backend"
 authors = ["Anandesh Sharma <anandeshsharma@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "singularity" }]
 
 [tool.poetry.dependencies]
```

### Comparing `singularity_core-0.1.0/singularity/db/postgres/models.py` & `singularity_core-0.2.0/singularity/db/postgres/models.py`

 * *Files identical despite different names*

### Comparing `singularity_core-0.1.0/singularity/db/postgres/schemas.py` & `singularity_core-0.2.0/singularity/db/postgres/schemas.py`

 * *Files identical despite different names*

### Comparing `singularity_core-0.1.0/singularity/exceptions/cache_exceptions.py` & `singularity_core-0.2.0/singularity/exceptions/cache_exceptions.py`

 * *Files identical despite different names*

### Comparing `singularity_core-0.1.0/singularity/logger.py` & `singularity_core-0.2.0/singularity/logger.py`

 * *Files identical despite different names*

### Comparing `singularity_core-0.1.0/singularity/main.py` & `singularity_core-0.2.0/singularity/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 import importlib.util
 import inspect
 import os
 from pathlib import Path
 
+from dotenv import load_dotenv
 from fastapi import APIRouter, FastAPI
 
 
 def service_name_validation(name: str) -> None | ValueError:
     if any(c in name for c in " /\\.:?\"<>|*[]=;,!@#$%^&(){}+`~'"):
         raise ValueError(
             f"Service name: {name} should contain only alphabets, numbers, and underscores."
         )
 
 
 class Singularity(FastAPI):
-    def __init__(self):
-        base_path = Path(inspect.stack()[1].filename).parent
-        self.services_folder = base_path / "services"
-
+    def __init__(self, env_path: str = None):
+        self.base_path = Path(inspect.stack()[1].filename).parent
+        self.services_folder = self.base_path / "services"
+        self._load_env_(env_path)
         self._setup_application_()
 
+    def _load_env_(self, path: str | None):
+        if path is None:
+            path = os.path.join(self.base_path, ".env")
+
+        if not os.path.exists(path):
+            raise ValueError(f"Environment file not found in {path}")
+
+        load_dotenv(dotenv_path=path)
+
     def _setup_application_(
         self,
     ):
         self.app = FastAPI()
         self.router = APIRouter()
         self.register_services()
         self.app.include_router(self.router)
```

### Comparing `singularity_core-0.1.0/singularity/middlewares/client_cache_middleware.py` & `singularity_core-0.2.0/singularity/middlewares/client_cache_middleware.py`

 * *Files identical despite different names*

### Comparing `singularity_core-0.1.0/singularity/schemas.py` & `singularity_core-0.2.0/singularity/schemas.py`

 * *Files identical despite different names*

### Comparing `singularity_core-0.1.0/singularity/setup.py` & `singularity_core-0.2.0/singularity/setup.py`

 * *Files identical despite different names*

### Comparing `singularity_core-0.1.0/singularity/utils/cache.py` & `singularity_core-0.2.0/singularity/utils/cache.py`

 * *Files identical despite different names*

### Comparing `singularity_core-0.1.0/singularity/utils/rate_limit.py` & `singularity_core-0.2.0/singularity/utils/rate_limit.py`

 * *Files identical despite different names*

### Comparing `singularity_core-0.1.0/PKG-INFO` & `singularity_core-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singularity-core
-Version: 0.1.0
+Version: 0.2.0
 Summary: Funny backend
 License: MIT
 Author: Anandesh Sharma
 Author-email: anandeshsharma@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


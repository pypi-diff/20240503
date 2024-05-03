# Comparing `tmp/supadantic-0.0.3.tar.gz` & `tmp/supadantic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supadantic-0.0.3.tar", max compression
+gzip compressed data, was "supadantic-0.0.4.tar", max compression
```

## Comparing `supadantic-0.0.3.tar` & `supadantic-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-04-22 16:28:37.091595 supadantic-0.0.3/LICENSE
--rw-r--r--   0        0        0     1315 2024-04-22 16:28:37.091595 supadantic-0.0.3/README.md
--rw-r--r--   0        0        0      676 2024-04-22 16:28:37.091595 supadantic-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 16:28:37.091595 supadantic-0.0.3/supadantic/__init__.py
--rw-r--r--   0        0        0     1865 2024-04-22 16:28:37.091595 supadantic-0.0.3/supadantic/models.py
--rw-r--r--   0        0        0     2412 2024-04-22 16:28:37.091595 supadantic-0.0.3/supadantic/q_set.py
--rw-r--r--   0        0        0     1608 2024-04-22 16:28:37.091595 supadantic-0.0.3/supadantic/supabase_client.py
--rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 supadantic-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-03 13:17:15.833989 supadantic-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2192 2024-05-03 13:17:15.833989 supadantic-0.0.4/README.md
+-rw-r--r--   0        0        0      676 2024-05-03 13:17:15.837989 supadantic-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 13:17:15.837989 supadantic-0.0.4/supadantic/__init__.py
+-rw-r--r--   0        0        0       37 2024-05-03 13:17:15.837989 supadantic-0.0.4/supadantic/clients/__init__.py
+-rw-r--r--   0        0        0      964 2024-05-03 13:17:15.837989 supadantic-0.0.4/supadantic/clients/base.py
+-rw-r--r--   0        0        0     1650 2024-05-03 13:17:15.837989 supadantic-0.0.4/supadantic/clients/supabase.py
+-rw-r--r--   0        0        0     2552 2024-05-03 13:17:15.837989 supadantic-0.0.4/supadantic/models.py
+-rw-r--r--   0        0        0     3694 2024-05-03 13:17:15.837989 supadantic-0.0.4/supadantic/q_set.py
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 supadantic-0.0.4/PKG-INFO
```

### Comparing `supadantic-0.0.3/LICENSE` & `supadantic-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `supadantic-0.0.3/pyproject.toml` & `supadantic-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supadantic"
-version = "0.0.3"
+version = "0.0.4"
 description = "Supabase integration for pydantic"
 authors = ["Alexey Makridenko <alexey.makridenko@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "supadantic"}]
 
 [tool.pytest.ini_options]
```

### Comparing `supadantic-0.0.3/supadantic/supabase_client.py` & `supadantic-0.0.4/supadantic/clients/supabase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 from typing import Any, Dict, Iterable, List
 
 from supabase.client import create_client
 
+from .base import BaseClient
 
-class SupabaseClient:
+
+class SupabaseClient(BaseClient):
     def __init__(self, table_name: str):
         url: str = os.getenv('SUPABASE_URL') or ''
         key: str = os.getenv('SUPABASE_KEY') or ''
         supabase_client = create_client(url, key)
         self.query = supabase_client.table(table_name=table_name)
 
     def insert(self, data: Dict[str, Any]) -> Dict[str, Any]:
```


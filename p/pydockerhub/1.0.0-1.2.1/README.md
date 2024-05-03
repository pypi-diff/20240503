# Comparing `tmp/pydockerhub-1.0.0.tar.gz` & `tmp/pydockerhub-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydockerhub-1.0.0.tar", max compression
+gzip compressed data, was "pydockerhub-1.2.1.tar", max compression
```

## Comparing `pydockerhub-1.0.0.tar` & `pydockerhub-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,23 @@
--rw-r--r--   0        0        0    11356 2024-05-02 10:29:23.661551 pydockerhub-1.0.0/LICENSE
--rw-r--r--   0        0        0     1458 2024-05-02 11:15:24.489240 pydockerhub-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-02 11:16:24.515270 pydockerhub-1.0.0/pydockerhub/__init__.py
--rw-r--r--   0        0        0     2251 2024-05-02 11:17:13.819242 pydockerhub-1.0.0/pydockerhub/client.py
--rw-r--r--   0        0        0       43 2024-05-02 09:03:41.425279 pydockerhub-1.0.0/pydockerhub/error.py
--rw-r--r--   0        0        0      884 2024-05-02 11:17:13.812708 pydockerhub-1.0.0/pydockerhub/exception.py
--rw-r--r--   0        0        0        0 2024-05-02 05:14:20.670793 pydockerhub-1.0.0/pydockerhub/http_calls/__init__.py
--rw-r--r--   0        0        0     1844 2024-05-02 11:17:13.770894 pydockerhub-1.0.0/pydockerhub/http_calls/caller.py
--rw-r--r--   0        0        0       96 2024-05-02 11:17:13.803355 pydockerhub-1.0.0/pydockerhub/http_calls/errors.py
--rw-r--r--   0        0        0      616 2024-05-02 10:33:38.609071 pydockerhub-1.0.0/pydockerhub/http_calls/request.py
--rw-r--r--   0        0        0      350 2024-05-02 10:33:38.613667 pydockerhub-1.0.0/pydockerhub/http_calls/response.py
--rw-r--r--   0        0        0        0 2024-05-02 05:06:17.021900 pydockerhub-1.0.0/pydockerhub/hub/__init__.py
--rw-r--r--   0        0        0       97 2024-05-02 11:17:13.816224 pydockerhub-1.0.0/pydockerhub/hub/errors.py
--rw-r--r--   0        0        0      765 2024-05-02 10:11:28.400476 pydockerhub-1.0.0/pydockerhub/hub/models.py
--rw-r--r--   0        0        0      427 2024-05-02 11:17:13.808210 pydockerhub-1.0.0/pydockerhub/hub/types.py
--rw-r--r--   0        0        0      473 2024-05-02 11:20:44.857334 pydockerhub-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pydockerhub-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-02 10:29:23.661551 pydockerhub-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1448 2024-05-03 00:10:33.824008 pydockerhub-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 11:16:24.515270 pydockerhub-1.2.1/pydockerhub/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 05:14:20.670793 pydockerhub-1.2.1/pydockerhub/api_calls/__init__.py
+-rw-r--r--   0        0        0     1639 2024-05-02 23:35:42.486766 pydockerhub-1.2.1/pydockerhub/api_calls/caller.py
+-rw-r--r--   0        0        0       95 2024-05-02 23:35:42.481562 pydockerhub-1.2.1/pydockerhub/api_calls/errors.py
+-rw-r--r--   0        0        0     1103 2024-05-02 20:34:35.418732 pydockerhub-1.2.1/pydockerhub/api_calls/request.py
+-rw-r--r--   0        0        0      438 2024-05-02 20:34:09.472750 pydockerhub-1.2.1/pydockerhub/api_calls/response.py
+-rw-r--r--   0        0        0      121 2024-05-02 19:45:05.990858 pydockerhub-1.2.1/pydockerhub/api_calls/types.py
+-rw-r--r--   0        0        0     2498 2024-05-03 00:10:33.816255 pydockerhub-1.2.1/pydockerhub/client.py
+-rw-r--r--   0        0        0       43 2024-05-02 09:03:41.425279 pydockerhub-1.2.1/pydockerhub/error.py
+-rw-r--r--   0        0        0      893 2024-05-02 23:35:42.477434 pydockerhub-1.2.1/pydockerhub/exception.py
+-rw-r--r--   0        0        0        0 2024-05-02 05:06:17.021900 pydockerhub-1.2.1/pydockerhub/hub/__init__.py
+-rw-r--r--   0        0        0     1368 2024-05-03 00:04:13.833163 pydockerhub-1.2.1/pydockerhub/hub/actions.py
+-rw-r--r--   0        0        0       97 2024-05-02 11:17:13.816224 pydockerhub-1.2.1/pydockerhub/hub/errors.py
+-rw-r--r--   0        0        0      845 2024-05-02 19:14:35.920764 pydockerhub-1.2.1/pydockerhub/hub/models.py
+-rw-r--r--   0        0        0      797 2024-05-02 23:22:27.102521 pydockerhub-1.2.1/pydockerhub/hub/types.py
+-rw-r--r--   0        0        0        0 2024-05-02 14:46:49.789836 pydockerhub-1.2.1/pydockerhub/raw_http/__init__.py
+-rw-r--r--   0        0        0     1581 2024-05-03 00:00:03.796716 pydockerhub-1.2.1/pydockerhub/raw_http/client.py
+-rw-r--r--   0        0        0      140 2024-05-02 15:37:59.556614 pydockerhub-1.2.1/pydockerhub/raw_http/errors.py
+-rw-r--r--   0        0        0      683 2024-05-02 20:03:04.904331 pydockerhub-1.2.1/pydockerhub/raw_http/types.py
+-rw-r--r--   0        0        0      518 2024-05-03 01:36:54.197018 pydockerhub-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 pydockerhub-1.2.1/PKG-INFO
```

### Comparing `pydockerhub-1.0.0/LICENSE` & `pydockerhub-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydockerhub-1.0.0/README.md` & `pydockerhub-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,9 +40,7 @@
 
 ```json
 {
   "username": "pinochcio",
   "password": "dckr_pat_9QNXBGGtZt7(...)"
 }
 ```
-
-## Usage
```

### Comparing `pydockerhub-1.0.0/pydockerhub/exception.py` & `pydockerhub-1.2.1/pydockerhub/exception.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import functools
 import logging
 
-from error import PyDockerHubError
-from pydockerhub.http_calls.errors import HttpCallError
+from pydockerhub.api_calls.errors import ApiCallError
+from pydockerhub.error import PyDockerHubError
 from pydockerhub.hub.errors import DockerHubError
 
 
 def handle_exception(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         logger = logging.getLogger("pydockerhub")
         logger.setLevel(logging.WARNING)
 
         try:
             return func(*args, **kwargs)
-        except HttpCallError as e:
+        except ApiCallError as e:
             logger.error(f'Error during HTTP call: {str(e)}')
             raise
         except DockerHubError as e:
             logger.error(f'Error during PyDockerHub call: {str(e)}')
             raise
         except PyDockerHubError as e:
             logger.error(f'PyDockerHub error: {str(e)}')
```

### Comparing `pydockerhub-1.0.0/pydockerhub/hub/models.py` & `pydockerhub-1.2.1/pydockerhub/hub/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,11 +34,16 @@
 
 
 class Tag(BaseModel):
     name: str
     created_at: datetime = Field(..., alias='last_updated')
 
 
+class PathParams(BaseModel):
+    namespace: str = ''
+    repository: str = ''
+
+
 class SearchQuery(BaseModel):
     page: int = 1
     page_size: int = 100
     ordering: str = 'name'
```

### Comparing `pydockerhub-1.0.0/PKG-INFO` & `pydockerhub-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydockerhub
-Version: 1.0.0
+Version: 1.2.1
 Summary: Extended Docker Hub API Client
 Home-page: https://github.com/9orky/py_dockerhub
 License: Apache-2.0
 Author: Tomasz Szpak
 Author-email: tomszp@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -59,9 +59,7 @@
 ```json
 {
   "username": "pinochcio",
   "password": "dckr_pat_9QNXBGGtZt7(...)"
 }
 ```
 
-## Usage
-
```


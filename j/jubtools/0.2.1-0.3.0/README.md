# Comparing `tmp/jubtools-0.2.1.tar.gz` & `tmp/jubtools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jubtools-0.2.1.tar", last modified: Wed Nov 29 09:16:33 2023, max compression
+gzip compressed data, was "jubtools-0.3.0.tar", last modified: Fri May  3 12:00:33 2024, max compression
```

## Comparing `jubtools-0.2.1.tar` & `jubtools-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-11-29 09:16:33.893900 jubtools-0.2.1/
--rw-rw-r--   0 andy      (1000) andy      (1000)    35149 2023-11-01 09:20:35.000000 jubtools-0.2.1/LICENSE
--rw-r--r--   0 andy      (1000) andy      (1000)    41008 2023-11-29 09:16:33.893900 jubtools-0.2.1/PKG-INFO
--rw-rw-r--   0 andy      (1000) andy      (1000)      141 2023-11-25 13:33:40.000000 jubtools-0.2.1/README.md
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-11-29 09:16:33.893900 jubtools-0.2.1/jubtools/
--rw-rw-r--   0 andy      (1000) andy      (1000)        0 2023-11-01 09:22:03.000000 jubtools-0.2.1/jubtools/__init__.py
--rw-rw-r--   0 andy      (1000) andy      (1000)     1325 2023-11-29 09:09:29.000000 jubtools-0.2.1/jubtools/config.py
--rw-rw-r--   0 andy      (1000) andy      (1000)      370 2023-11-01 09:22:03.000000 jubtools-0.2.1/jubtools/misctools.py
--rw-rw-r--   0 andy      (1000) andy      (1000)        0 2023-11-29 09:06:31.000000 jubtools-0.2.1/jubtools/py.typed
--rw-rw-r--   0 andy      (1000) andy      (1000)     1143 2023-11-01 09:22:03.000000 jubtools-0.2.1/jubtools/sqlt.py
--rw-rw-r--   0 andy      (1000) andy      (1000)     3080 2023-11-29 09:13:08.000000 jubtools-0.2.1/jubtools/systemtools.py
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-11-29 09:16:33.893900 jubtools-0.2.1/jubtools.egg-info/
--rw-r--r--   0 andy      (1000) andy      (1000)    41008 2023-11-29 09:16:33.000000 jubtools-0.2.1/jubtools.egg-info/PKG-INFO
--rw-rw-r--   0 andy      (1000) andy      (1000)      357 2023-11-29 09:16:33.000000 jubtools-0.2.1/jubtools.egg-info/SOURCES.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-11-29 09:16:33.000000 jubtools-0.2.1/jubtools.egg-info/dependency_links.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)        8 2023-11-29 09:16:33.000000 jubtools-0.2.1/jubtools.egg-info/requires.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)        9 2023-11-29 09:16:33.000000 jubtools-0.2.1/jubtools.egg-info/top_level.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)      488 2023-11-29 09:15:30.000000 jubtools-0.2.1/pyproject.toml
--rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-11-29 09:16:33.893900 jubtools-0.2.1/setup.cfg
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-11-29 09:16:33.893900 jubtools-0.2.1/tests/
--rw-rw-r--   0 andy      (1000) andy      (1000)     1214 2023-11-25 13:33:43.000000 jubtools-0.2.1/tests/test_config.py
--rw-rw-r--   0 andy      (1000) andy      (1000)      259 2023-11-25 13:33:43.000000 jubtools-0.2.1/tests/test_misctools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:00:33.074686 jubtools-0.3.0/
+-rw-r--r--   0 andy       (501) staff       (20)    35149 2023-11-25 11:26:03.000000 jubtools-0.3.0/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)    41009 2024-05-03 12:00:33.074467 jubtools-0.3.0/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      141 2023-11-25 12:22:01.000000 jubtools-0.3.0/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:00:33.072802 jubtools-0.3.0/jubtools/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2023-11-25 11:26:03.000000 jubtools-0.3.0/jubtools/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     1381 2024-05-03 11:18:05.000000 jubtools-0.3.0/jubtools/config.py
+-rw-r--r--   0 andy       (501) staff       (20)      370 2023-11-25 11:26:03.000000 jubtools-0.3.0/jubtools/misctools.py
+-rw-r--r--   0 andy       (501) staff       (20)     4698 2024-05-03 11:01:45.000000 jubtools-0.3.0/jubtools/psql.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-05-01 16:00:18.000000 jubtools-0.3.0/jubtools/py.typed
+-rw-r--r--   0 andy       (501) staff       (20)     1143 2024-05-03 11:07:09.000000 jubtools-0.3.0/jubtools/sqlt.py
+-rw-r--r--   0 andy       (501) staff       (20)     3654 2024-05-03 11:11:12.000000 jubtools-0.3.0/jubtools/systemtools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:00:33.074189 jubtools-0.3.0/jubtools.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)    41009 2024-05-03 12:00:33.000000 jubtools-0.3.0/jubtools.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      374 2024-05-03 12:00:33.000000 jubtools-0.3.0/jubtools.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-03 12:00:33.000000 jubtools-0.3.0/jubtools.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)        8 2024-05-03 12:00:33.000000 jubtools-0.3.0/jubtools.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)        9 2024-05-03 12:00:33.000000 jubtools-0.3.0/jubtools.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)      489 2024-05-03 11:59:27.000000 jubtools-0.3.0/pyproject.toml
+-rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-03 12:00:33.074730 jubtools-0.3.0/setup.cfg
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:00:33.073895 jubtools-0.3.0/tests/
+-rw-r--r--   0 andy       (501) staff       (20)     1214 2024-05-01 16:00:18.000000 jubtools-0.3.0/tests/test_config.py
+-rw-r--r--   0 andy       (501) staff       (20)      259 2024-05-01 16:00:18.000000 jubtools-0.3.0/tests/test_misctools.py
```

### Comparing `jubtools-0.2.1/LICENSE` & `jubtools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jubtools-0.2.1/PKG-INFO` & `jubtools-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.2.1
+Version: 0.3.0
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,15 +675,15 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Repository, https://github.com/Jubulani/jubtools.git
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
 
 # jubtools
 
 Shared tools for my own work
```

### Comparing `jubtools-0.2.1/jubtools/sqlt.py` & `jubtools-0.3.0/jubtools/sqlt.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.2.1/jubtools/systemtools.py` & `jubtools-0.3.0/jubtools/systemtools.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,68 @@
 import datetime as dt
+from enum import Enum
 import logging
 import os
 from typing import Any
 
 from fastapi import FastAPI, Response
 from pydantic import BaseModel
 
 # from errors import AuthError, FSError
 
-from jubtools import config, misctools, sqlt
+from api.jubtools import config, misctools
 
 logger = logging.getLogger(__name__)
 
-APP_NAME = "GreekServer"
 APP_START_TIME: dt.datetime
 
 
-def create_fastapi_app() -> FastAPI:
+class DBModule(Enum):
+    SQLITE = 1
+    POSTGRES = 2
+
+
+def create_fastapi_app(db_module: DBModule | None = None) -> FastAPI:
     global APP_START_TIME
 
-    fastapi_args: dict[str, Any] = {"title": APP_NAME}
+    fastapi_args: dict[str, Any] = {"title": config.get("app_name")}
     if config.get("fastapi.disable_docs"):
         fastapi_args["openapi_url"] = None
     app = FastAPI(**fastapi_args)
 
     APP_START_TIME = dt.datetime.now()
     app.add_api_route("/health", health_handler, methods=["GET"])
 
+    if db_module is not None:
+        init_db_module(db_module, app)
     # app.add_exception_handler(FSError, custom_exception_handler)
 
-    # app.add_event_handler("startup", psql.init)
-    # app.add_event_handler("shutdown", psql.shutdown)
-    app.add_middleware(sqlt.ConnMiddleware)
-
     # Add last, so it wraps everything
     app.add_middleware(TimerMiddleware)
 
     return app
 
 
+def init_db_module(db_module: DBModule, app: FastAPI):
+    """ Use dynamic imports here, so we don't need to install all db drivers """
+
+    match db_module:
+        case DBModule.SQLITE:
+            from api.jubtools import sqlt
+            app.add_middleware(sqlt.ConnMiddleware)
+
+        case DBModule.POSTGRES:
+            from api.jubtools import psql
+            app.add_event_handler("startup", psql.init)
+            app.add_event_handler("shutdown", psql.shutdown)
+
+        case _:
+            raise ValueError(f"Unknown db_module: {db_module}")
+
+
 class HealthResponse(BaseModel):
     request_ts: dt.datetime
     status: str
     uptime: str
     version: str
     env: str
```

### Comparing `jubtools-0.2.1/jubtools.egg-info/PKG-INFO` & `jubtools-0.3.0/jubtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.2.1
+Version: 0.3.0
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,15 +675,15 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Repository, https://github.com/Jubulani/jubtools.git
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi
 
 # jubtools
 
 Shared tools for my own work
```

### Comparing `jubtools-0.2.1/tests/test_config.py` & `jubtools-0.3.0/tests/test_config.py`

 * *Files identical despite different names*


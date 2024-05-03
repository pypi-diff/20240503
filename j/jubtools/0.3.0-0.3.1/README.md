# Comparing `tmp/jubtools-0.3.0.tar.gz` & `tmp/jubtools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jubtools-0.3.0.tar", last modified: Fri May  3 12:00:33 2024, max compression
+gzip compressed data, was "jubtools-0.3.1.tar", last modified: Fri May  3 12:10:20 2024, max compression
```

## Comparing `jubtools-0.3.0.tar` & `jubtools-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:00:33.074686 jubtools-0.3.0/
--rw-r--r--   0 andy       (501) staff       (20)    35149 2023-11-25 11:26:03.000000 jubtools-0.3.0/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)    41009 2024-05-03 12:00:33.074467 jubtools-0.3.0/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      141 2023-11-25 12:22:01.000000 jubtools-0.3.0/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:00:33.072802 jubtools-0.3.0/jubtools/
--rw-r--r--   0 andy       (501) staff       (20)        0 2023-11-25 11:26:03.000000 jubtools-0.3.0/jubtools/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1381 2024-05-03 11:18:05.000000 jubtools-0.3.0/jubtools/config.py
--rw-r--r--   0 andy       (501) staff       (20)      370 2023-11-25 11:26:03.000000 jubtools-0.3.0/jubtools/misctools.py
--rw-r--r--   0 andy       (501) staff       (20)     4698 2024-05-03 11:01:45.000000 jubtools-0.3.0/jubtools/psql.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-05-01 16:00:18.000000 jubtools-0.3.0/jubtools/py.typed
--rw-r--r--   0 andy       (501) staff       (20)     1143 2024-05-03 11:07:09.000000 jubtools-0.3.0/jubtools/sqlt.py
--rw-r--r--   0 andy       (501) staff       (20)     3654 2024-05-03 11:11:12.000000 jubtools-0.3.0/jubtools/systemtools.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:00:33.074189 jubtools-0.3.0/jubtools.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)    41009 2024-05-03 12:00:33.000000 jubtools-0.3.0/jubtools.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      374 2024-05-03 12:00:33.000000 jubtools-0.3.0/jubtools.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-03 12:00:33.000000 jubtools-0.3.0/jubtools.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)        8 2024-05-03 12:00:33.000000 jubtools-0.3.0/jubtools.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)        9 2024-05-03 12:00:33.000000 jubtools-0.3.0/jubtools.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)      489 2024-05-03 11:59:27.000000 jubtools-0.3.0/pyproject.toml
--rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-03 12:00:33.074730 jubtools-0.3.0/setup.cfg
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:00:33.073895 jubtools-0.3.0/tests/
--rw-r--r--   0 andy       (501) staff       (20)     1214 2024-05-01 16:00:18.000000 jubtools-0.3.0/tests/test_config.py
--rw-r--r--   0 andy       (501) staff       (20)      259 2024-05-01 16:00:18.000000 jubtools-0.3.0/tests/test_misctools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:10:20.904723 jubtools-0.3.1/
+-rw-r--r--   0 andy       (501) staff       (20)    35149 2023-11-25 11:26:03.000000 jubtools-0.3.1/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)    41051 2024-05-03 12:10:20.904338 jubtools-0.3.1/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      183 2024-05-03 12:01:13.000000 jubtools-0.3.1/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:10:20.902790 jubtools-0.3.1/jubtools/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2023-11-25 11:26:03.000000 jubtools-0.3.1/jubtools/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     1381 2024-05-03 11:18:05.000000 jubtools-0.3.1/jubtools/config.py
+-rw-r--r--   0 andy       (501) staff       (20)      370 2023-11-25 11:26:03.000000 jubtools-0.3.1/jubtools/misctools.py
+-rw-r--r--   0 andy       (501) staff       (20)     4694 2024-05-03 12:07:31.000000 jubtools-0.3.1/jubtools/psql.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-05-01 16:00:18.000000 jubtools-0.3.1/jubtools/py.typed
+-rw-r--r--   0 andy       (501) staff       (20)     1143 2024-05-03 11:07:09.000000 jubtools-0.3.1/jubtools/sqlt.py
+-rw-r--r--   0 andy       (501) staff       (20)     3642 2024-05-03 12:08:06.000000 jubtools-0.3.1/jubtools/systemtools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:10:20.904067 jubtools-0.3.1/jubtools.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)    41051 2024-05-03 12:10:20.000000 jubtools-0.3.1/jubtools.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      374 2024-05-03 12:10:20.000000 jubtools-0.3.1/jubtools.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-03 12:10:20.000000 jubtools-0.3.1/jubtools.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)        8 2024-05-03 12:10:20.000000 jubtools-0.3.1/jubtools.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)        9 2024-05-03 12:10:20.000000 jubtools-0.3.1/jubtools.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)      489 2024-05-03 12:08:22.000000 jubtools-0.3.1/pyproject.toml
+-rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-03 12:10:20.904781 jubtools-0.3.1/setup.cfg
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 12:10:20.903741 jubtools-0.3.1/tests/
+-rw-r--r--   0 andy       (501) staff       (20)     1214 2024-05-01 16:00:18.000000 jubtools-0.3.1/tests/test_config.py
+-rw-r--r--   0 andy       (501) staff       (20)      259 2024-05-01 16:00:18.000000 jubtools-0.3.1/tests/test_misctools.py
```

### Comparing `jubtools-0.3.0/LICENSE` & `jubtools-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jubtools-0.3.0/PKG-INFO` & `jubtools-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.3.0
+Version: 0.3.1
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,11 +686,12 @@
 
 # jubtools
 
 Shared tools for my own work
 
 ## Package
 
+* Update version number in pyproject.toml
 * `pip install build twine`
 * `rm -r dist`
 * `python -m build`
 * `twine upload dist/*`
```

### Comparing `jubtools-0.3.0/jubtools/config.py` & `jubtools-0.3.1/jubtools/config.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.3.0/jubtools/psql.py` & `jubtools-0.3.1/jubtools/psql.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import time
 from typing import List, Dict, Tuple, Iterable
 
 import asyncpg
 from fastapi import Request
 
-from api.jubtools import config, misctools
+from jubtools import config, misctools
 
 logger = logging.getLogger(__name__)
 
 _POOL = None
 _SQL = {}
```

### Comparing `jubtools-0.3.0/jubtools/sqlt.py` & `jubtools-0.3.1/jubtools/sqlt.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.3.0/jubtools/systemtools.py` & `jubtools-0.3.1/jubtools/systemtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any
 
 from fastapi import FastAPI, Response
 from pydantic import BaseModel
 
 # from errors import AuthError, FSError
 
-from api.jubtools import config, misctools
+from jubtools import config, misctools
 
 logger = logging.getLogger(__name__)
 
 APP_START_TIME: dt.datetime
 
 
 class DBModule(Enum):
@@ -43,19 +43,19 @@
 
 
 def init_db_module(db_module: DBModule, app: FastAPI):
     """ Use dynamic imports here, so we don't need to install all db drivers """
 
     match db_module:
         case DBModule.SQLITE:
-            from api.jubtools import sqlt
+            from jubtools import sqlt
             app.add_middleware(sqlt.ConnMiddleware)
 
         case DBModule.POSTGRES:
-            from api.jubtools import psql
+            from jubtools import psql
             app.add_event_handler("startup", psql.init)
             app.add_event_handler("shutdown", psql.shutdown)
 
         case _:
             raise ValueError(f"Unknown db_module: {db_module}")
```

### Comparing `jubtools-0.3.0/jubtools.egg-info/PKG-INFO` & `jubtools-0.3.1/jubtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.3.0
+Version: 0.3.1
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,11 +686,12 @@
 
 # jubtools
 
 Shared tools for my own work
 
 ## Package
 
+* Update version number in pyproject.toml
 * `pip install build twine`
 * `rm -r dist`
 * `python -m build`
 * `twine upload dist/*`
```

### Comparing `jubtools-0.3.0/tests/test_config.py` & `jubtools-0.3.1/tests/test_config.py`

 * *Files identical despite different names*


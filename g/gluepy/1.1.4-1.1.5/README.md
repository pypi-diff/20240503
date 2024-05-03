# Comparing `tmp/gluepy-1.1.4.tar.gz` & `tmp/gluepy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gluepy-1.1.4.tar", last modified: Wed Apr 24 13:07:11 2024, max compression
+gzip compressed data, was "gluepy-1.1.5.tar", last modified: Fri May  3 15:01:39 2024, max compression
```

## Comparing `gluepy-1.1.4.tar` & `gluepy-1.1.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.812246 gluepy-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 13:07:00.000000 gluepy-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:00.000000 gluepy-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 13:07:11.812246 gluepy-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 13:07:00.000000 gluepy-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.804246 gluepy-1.1.4/gluepy/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.804246 gluepy-1.1.4/gluepy/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/bin/gluepy-cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.808246 gluepy-1.1.4/gluepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/commands/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/commands/gluepy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/commands/startmodule.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/commands/startproject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.808246 gluepy-1.1.4/gluepy/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/conf/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.808246 gluepy-1.1.4/gluepy/exec/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/exec/boot.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/exec/dags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/exec/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.808246 gluepy-1.1.4/gluepy/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.808246 gluepy-1.1.4/gluepy/files/data/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/files/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/files/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/files/data/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.808246 gluepy-1.1.4/gluepy/files/storages/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/files/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/files/storages/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/files/storages/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/files/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/files/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/files/storages/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.812246 gluepy-1.1.4/gluepy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-24 13:07:00.000000 gluepy-1.1.4/gluepy/utils/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.812246 gluepy-1.1.4/gluepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 13:07:11.000000 gluepy-1.1.4/gluepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-24 13:07:11.000000 gluepy-1.1.4/gluepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:07:11.000000 gluepy-1.1.4/gluepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 13:07:11.000000 gluepy-1.1.4/gluepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 13:07:11.000000 gluepy-1.1.4/gluepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 13:07:11.000000 gluepy-1.1.4/gluepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:07:11.812246 gluepy-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-24 13:07:00.000000 gluepy-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:07:11.812246 gluepy-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 13:07:00.000000 gluepy-1.1.4/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.765578 gluepy-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 15:01:31.000000 gluepy-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:31.000000 gluepy-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-03 15:01:39.765578 gluepy-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 15:01:31.000000 gluepy-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.761578 gluepy-1.1.5/gluepy/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.761578 gluepy-1.1.5/gluepy/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/bin/gluepy-cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.761578 gluepy-1.1.5/gluepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/commands/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/commands/gluepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/commands/startmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/commands/startproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.761578 gluepy-1.1.5/gluepy/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/conf/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.761578 gluepy-1.1.5/gluepy/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/exec/boot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/exec/dags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/exec/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.761578 gluepy-1.1.5/gluepy/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.765578 gluepy-1.1.5/gluepy/files/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/files/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/files/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/files/data/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.765578 gluepy-1.1.5/gluepy/files/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/files/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/files/storages/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/files/storages/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/files/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/files/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/files/storages/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.765578 gluepy-1.1.5/gluepy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-03 15:01:31.000000 gluepy-1.1.5/gluepy/utils/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.765578 gluepy-1.1.5/gluepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-03 15:01:39.000000 gluepy-1.1.5/gluepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-03 15:01:39.000000 gluepy-1.1.5/gluepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:01:39.000000 gluepy-1.1.5/gluepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 15:01:39.000000 gluepy-1.1.5/gluepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 15:01:39.000000 gluepy-1.1.5/gluepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 15:01:39.000000 gluepy-1.1.5/gluepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:01:39.765578 gluepy-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-03 15:01:31.000000 gluepy-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:01:39.765578 gluepy-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 15:01:31.000000 gluepy-1.1.5/tests/test_sample.py
```

### Comparing `gluepy-1.1.4/LICENSE` & `gluepy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/PKG-INFO` & `gluepy-1.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluepy
-Version: 1.1.4
+Version: 1.1.5
 Summary: A framework for data scientists
 Home-page: https://github.com/gluepy/gluepy
 Author: Marcus Lind
 Author-email: marcuslind90@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gluepy-1.1.4/gluepy/commands/airflow.py` & `gluepy-1.1.5/gluepy/commands/airflow.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/commands/base.py` & `gluepy-1.1.5/gluepy/commands/base.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/commands/dag.py` & `gluepy-1.1.5/gluepy/commands/dag.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/commands/gluepy.py` & `gluepy-1.1.5/gluepy/commands/gluepy.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/conf/context.py` & `gluepy-1.1.5/gluepy/conf/context.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/exec/boot.py` & `gluepy-1.1.5/gluepy/exec/boot.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/exec/dags.py` & `gluepy-1.1.5/gluepy/exec/dags.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/exec/tasks.py` & `gluepy-1.1.5/gluepy/exec/tasks.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/files/data/pandas.py` & `gluepy-1.1.5/gluepy/files/data/pandas.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/files/storages/base.py` & `gluepy-1.1.5/gluepy/files/storages/base.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/files/storages/google.py` & `gluepy-1.1.5/gluepy/files/storages/google.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,49 @@
 import os
 import logging
 from pathlib import Path
 from typing import Union
 from io import StringIO, BytesIO
+import requests
+import requests.exceptions as requests_exceptions
 from google.cloud import storage
-from google.api_core.exceptions import NotFound as GoogleNotFound
+from google.api_core import retry
+from google.api_core import exceptions as api_exceptions
+from google.auth import exceptions as auth_exceptions
 from gluepy.conf import default_settings
 from .base import BaseStorage
 
 logger = logging.getLogger(__name__)
 
+_RETRYABLE_TYPES = (
+    api_exceptions.TooManyRequests,  # 429
+    api_exceptions.InternalServerError,  # 500
+    api_exceptions.BadGateway,  # 502
+    api_exceptions.ServiceUnavailable,  # 503
+    api_exceptions.GatewayTimeout,  # 504
+    ConnectionError,
+    requests.ConnectionError,
+    requests_exceptions.ChunkedEncodingError,
+    requests_exceptions.Timeout,
+)
+
+_ADDITIONAL_RETRYABLE_STATUS_CODES = (408,)
+
+
+def _should_retry(exc):
+    """Predicate for determining when to retry."""
+    if isinstance(exc, _RETRYABLE_TYPES):
+        return True
+    elif isinstance(exc, api_exceptions.GoogleAPICallError):
+        return exc.code in _ADDITIONAL_RETRYABLE_STATUS_CODES
+    elif isinstance(exc, auth_exceptions.TransportError):
+        return _should_retry(exc.args[0])
+    else:
+        return False
+
 
 class GoogleStorage(BaseStorage):
     """ "
     Storage support for Google Cloud Storage.
     """
 
     separator = "/"
@@ -38,15 +68,21 @@
         """
         assert not file_path.endswith(
             self.separator
         ), f"File name cannot end with '{self.separator}'."
         content.seek(0)
         if isinstance(content, StringIO):
             content = BytesIO(content.read().encode("utf-8"))
-        self.bucket.blob(self.abspath(file_path)).upload_from_file(content)
+
+        self.bucket.blob(self.abspath(file_path)).upload_from_file(
+            content,
+            rewind=True,
+            retry=retry.Retry(predicate=_should_retry),
+            size=len(content.read()),
+        )
 
     def open(self, file_path: str, mode: str = "rb") -> Union[str, bytes]:
         """Opens a blob at file_path
 
         Args:
             file_path (str): File path of blob we want to open
 
@@ -55,15 +91,15 @@
         """
         if mode != "rb":
             logger.warning(f"`mode` is not used for {self.__class__.__name__}")
 
         stream = BytesIO()
         try:
             self.bucket.blob(self.abspath(file_path)).download_to_file(stream)
-        except GoogleNotFound as exc:
+        except api_exceptions.NotFound as exc:
             raise FileNotFoundError(
                 f"File '{self.abspath(file_path)}' does not exist."
             ) from exc
         stream.seek(0)
         return stream.read()
 
     def rm(self, path: str, recursive: bool = False) -> None:
```

### Comparing `gluepy-1.1.4/gluepy/files/storages/local.py` & `gluepy-1.1.5/gluepy/files/storages/local.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/files/storages/s3.py` & `gluepy-1.1.5/gluepy/files/storages/s3.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/utils/dict.py` & `gluepy-1.1.5/gluepy/utils/dict.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy/utils/loading.py` & `gluepy-1.1.5/gluepy/utils/loading.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/gluepy.egg-info/PKG-INFO` & `gluepy-1.1.5/gluepy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluepy
-Version: 1.1.4
+Version: 1.1.5
 Summary: A framework for data scientists
 Home-page: https://github.com/gluepy/gluepy
 Author: Marcus Lind
 Author-email: marcuslind90@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gluepy-1.1.4/gluepy.egg-info/SOURCES.txt` & `gluepy-1.1.5/gluepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.4/setup.py` & `gluepy-1.1.5/setup.py`

 * *Files identical despite different names*


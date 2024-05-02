# Comparing `tmp/prl-cli-0.0.8.tar.gz` & `tmp/prl-cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prl-cli-0.0.8.tar", last modified: Thu Oct 26 16:44:20 2023, max compression
+gzip compressed data, was "prl-cli-0.0.9.tar", last modified: Fri Oct 27 02:24:39 2023, max compression
```

## Comparing `prl-cli-0.0.8.tar` & `prl-cli-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-10-26 16:44:20.936663 prl-cli-0.0.8/
--rw-r--r--   0 langston   (501) staff       (20)      227 2023-10-26 16:44:20.936214 prl-cli-0.0.8/PKG-INFO
--rw-r--r--   0 langston   (501) staff       (20)     2911 2023-10-26 16:43:11.000000 prl-cli-0.0.8/README.md
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-10-26 16:44:20.932771 prl-cli-0.0.8/prl/
--rw-r--r--   0 langston   (501) staff       (20)        0 2023-10-12 05:21:05.000000 prl-cli-0.0.8/prl/__init__.py
--rw-r--r--   0 langston   (501) staff       (20)     2549 2023-10-26 16:43:11.000000 prl-cli-0.0.8/prl/auth.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-10-26 16:44:20.933597 prl-cli-0.0.8/prl/jsonschemas/
--rw-r--r--   0 langston   (501) staff       (20)      551 2023-10-26 16:43:12.000000 prl-cli-0.0.8/prl/jsonschemas/run_params_schema.json
--rw-r--r--   0 langston   (501) staff       (20)     2533 2023-10-26 16:43:55.000000 prl-cli-0.0.8/prl/jsonschemas/suiteschema.json
--rw-r--r--   0 langston   (501) staff       (20)      208 2023-10-12 05:21:05.000000 prl-cli-0.0.8/prl/main.py
--rw-r--r--   0 langston   (501) staff       (20)     1810 2023-10-26 16:43:12.000000 prl-cli-0.0.8/prl/run.py
--rw-r--r--   0 langston   (501) staff       (20)     9505 2023-10-26 16:43:55.000000 prl-cli-0.0.8/prl/suite.py
--rw-r--r--   0 langston   (501) staff       (20)     2001 2023-10-26 16:43:12.000000 prl-cli-0.0.8/prl/util.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-10-26 16:44:20.935644 prl-cli-0.0.8/prl_cli.egg-info/
--rw-r--r--   0 langston   (501) staff       (20)      227 2023-10-26 16:44:20.000000 prl-cli-0.0.8/prl_cli.egg-info/PKG-INFO
--rw-r--r--   0 langston   (501) staff       (20)      354 2023-10-26 16:44:20.000000 prl-cli-0.0.8/prl_cli.egg-info/SOURCES.txt
--rw-r--r--   0 langston   (501) staff       (20)        1 2023-10-26 16:44:20.000000 prl-cli-0.0.8/prl_cli.egg-info/dependency_links.txt
--rw-r--r--   0 langston   (501) staff       (20)       37 2023-10-26 16:44:20.000000 prl-cli-0.0.8/prl_cli.egg-info/entry_points.txt
--rw-r--r--   0 langston   (501) staff       (20)       27 2023-10-26 16:44:20.000000 prl-cli-0.0.8/prl_cli.egg-info/requires.txt
--rw-r--r--   0 langston   (501) staff       (20)        4 2023-10-26 16:44:20.000000 prl-cli-0.0.8/prl_cli.egg-info/top_level.txt
--rw-r--r--   0 langston   (501) staff       (20)       38 2023-10-26 16:44:20.936760 prl-cli-0.0.8/setup.cfg
--rw-r--r--   0 langston   (501) staff       (20)      455 2023-10-26 16:44:06.000000 prl-cli-0.0.8/setup.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-10-27 02:24:39.619212 prl-cli-0.0.9/
+-rw-r--r--   0 langston   (501) staff       (20)      227 2023-10-27 02:24:39.618741 prl-cli-0.0.9/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)     2911 2023-10-26 16:43:11.000000 prl-cli-0.0.9/README.md
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-10-27 02:24:39.614787 prl-cli-0.0.9/prl/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2023-10-12 05:21:05.000000 prl-cli-0.0.9/prl/__init__.py
+-rw-r--r--   0 langston   (501) staff       (20)     2550 2023-10-27 02:21:26.000000 prl-cli-0.0.9/prl/auth.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-10-27 02:24:39.615753 prl-cli-0.0.9/prl/jsonschemas/
+-rw-r--r--   0 langston   (501) staff       (20)      551 2023-10-26 16:43:12.000000 prl-cli-0.0.9/prl/jsonschemas/run_params_schema.json
+-rw-r--r--   0 langston   (501) staff       (20)     2533 2023-10-26 16:43:55.000000 prl-cli-0.0.9/prl/jsonschemas/suiteschema.json
+-rw-r--r--   0 langston   (501) staff       (20)      208 2023-10-12 05:21:05.000000 prl-cli-0.0.9/prl/main.py
+-rw-r--r--   0 langston   (501) staff       (20)     1810 2023-10-26 16:43:12.000000 prl-cli-0.0.9/prl/run.py
+-rw-r--r--   0 langston   (501) staff       (20)     9598 2023-10-27 02:23:27.000000 prl-cli-0.0.9/prl/suite.py
+-rw-r--r--   0 langston   (501) staff       (20)     2001 2023-10-26 16:43:12.000000 prl-cli-0.0.9/prl/util.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-10-27 02:24:39.618190 prl-cli-0.0.9/prl_cli.egg-info/
+-rw-r--r--   0 langston   (501) staff       (20)      227 2023-10-27 02:24:39.000000 prl-cli-0.0.9/prl_cli.egg-info/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)      354 2023-10-27 02:24:39.000000 prl-cli-0.0.9/prl_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 langston   (501) staff       (20)        1 2023-10-27 02:24:39.000000 prl-cli-0.0.9/prl_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 langston   (501) staff       (20)       37 2023-10-27 02:24:39.000000 prl-cli-0.0.9/prl_cli.egg-info/entry_points.txt
+-rw-r--r--   0 langston   (501) staff       (20)       27 2023-10-27 02:24:39.000000 prl-cli-0.0.9/prl_cli.egg-info/requires.txt
+-rw-r--r--   0 langston   (501) staff       (20)        4 2023-10-27 02:24:39.000000 prl-cli-0.0.9/prl_cli.egg-info/top_level.txt
+-rw-r--r--   0 langston   (501) staff       (20)       38 2023-10-27 02:24:39.619323 prl-cli-0.0.9/setup.cfg
+-rw-r--r--   0 langston   (501) staff       (20)      455 2023-10-27 02:24:29.000000 prl-cli-0.0.9/setup.py
```

### Comparing `prl-cli-0.0.8/README.md` & `prl-cli-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `prl-cli-0.0.8/prl/auth.py` & `prl-cli-0.0.9/prl/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import sys
-import click
-import boto3
+import json
 import os
+import sys
 import time
-import json
+
+import boto3
+import click
 
 PRL_PATH = os.path.expanduser("~/.prl")
 CREDS_PATH = os.path.join(PRL_PATH, "creds.json")
 PLAYGROUND_ENV = os.getenv("PLAYGROUND_ENV")
 CLIENT_ID = (
-    "7kchsj7jf6mf6g5kb51riomhlh"
+    "59blf1klr2lejsd3uanpk3b0r4"
     if PLAYGROUND_ENV in ["LOCAL", "DEV"]
     else "7r5tn1kic6i262mv86g6etn3oj"
 )
 
 client = boto3.client("cognito-idp")
```

### Comparing `prl-cli-0.0.8/prl/jsonschemas/run_params_schema.json` & `prl-cli-0.0.9/prl/jsonschemas/run_params_schema.json`

 * *Files identical despite different names*

### Comparing `prl-cli-0.0.8/prl/jsonschemas/suiteschema.json` & `prl-cli-0.0.9/prl/jsonschemas/suiteschema.json`

 * *Files identical despite different names*

### Comparing `prl-cli-0.0.8/prl/run.py` & `prl-cli-0.0.9/prl/run.py`

 * *Files identical despite different names*

### Comparing `prl-cli-0.0.8/prl/suite.py` & `prl-cli-0.0.9/prl/suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, Dict
 
 import boto3
 import click
 import requests
 from gql import gql
 from jsonschema import ValidationError, validate
+from prl.auth import get_auth_token
 
 from .util import (
     BE_HOST,
     FE_HOST,
     SUITE_SCHEMA_PATH,
     display_error_and_exit,
     get_client,
@@ -115,14 +116,15 @@
 
 
 def upload_file(suite_id: str, file_path: str) -> str:
     with open(file_path, "rb") as f:
         response = requests.post(
             f"{BE_HOST}/upload_file/?test_suite_id={suite_id}",
             files={"file": f},
+            headers={"Authorization": get_auth_token()},
         )
         if response.status_code != 200:
             raise Exception(f"Failed to upload file {file_path}")
         return response.json()["file_id"]
 
 
 def upload_files(suite_id: str, data: Dict[str, Any]):
```

### Comparing `prl-cli-0.0.8/prl/util.py` & `prl-cli-0.0.9/prl/util.py`

 * *Files identical despite different names*


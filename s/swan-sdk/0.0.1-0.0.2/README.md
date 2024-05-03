# Comparing `tmp/swan_sdk-0.0.1.tar.gz` & `tmp/swan_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swan_sdk-0.0.1.tar", last modified: Sat Apr 27 21:43:29 2024, max compression
+gzip compressed data, was "swan_sdk-0.0.2.tar", last modified: Fri May  3 21:17:38 2024, max compression
```

## Comparing `swan_sdk-0.0.1.tar` & `swan_sdk-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-04-27 21:43:29.426415 swan_sdk-0.0.1/
--rw-r--r--   0 zihangchen   (501) staff       (20)     1072 2024-04-27 21:10:50.000000 swan_sdk-0.0.1/LICENSE
--rw-r--r--   0 zihangchen   (501) staff       (20)       32 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/MANIFEST.in
--rw-r--r--   0 zihangchen   (501) staff       (20)     3472 2024-04-27 21:43:29.426190 swan_sdk-0.0.1/PKG-INFO
--rw-r--r--   0 zihangchen   (501) staff       (20)     2932 2024-04-27 21:19:06.000000 swan_sdk-0.0.1/README.md
--rw-r--r--   0 zihangchen   (501) staff       (20)       38 2024-04-27 21:43:29.426456 swan_sdk-0.0.1/setup.cfg
--rw-r--r--   0 zihangchen   (501) staff       (20)     1179 2024-04-27 21:43:08.000000 swan_sdk-0.0.1/setup.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-04-27 21:43:29.421507 swan_sdk-0.0.1/swan/
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-04-27 21:43:29.422764 swan_sdk-0.0.1/swan/api/
--rw-r--r--   0 zihangchen   (501) staff       (20)       25 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/api/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)    21499 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/api/mcs_api.py
--rw-r--r--   0 zihangchen   (501) staff       (20)    12225 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/api/swan_api.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-04-27 21:43:29.423563 swan_sdk-0.0.1/swan/common/
--rw-r--r--   0 zihangchen   (501) staff       (20)      245 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/common/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     2348 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/common/constant.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     1600 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/common/exception.py
--rw-r--r--   0 zihangchen   (501) staff       (20)      447 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/common/file.py
--rw-r--r--   0 zihangchen   (501) staff       (20)       26 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/common/params.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     3323 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/common/utils.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-04-27 21:43:29.423810 swan_sdk-0.0.1/swan/contract/
--rw-r--r--   0 zihangchen   (501) staff       (20)       29 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/contract/__init__.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-04-27 21:43:29.424594 swan_sdk-0.0.1/swan/contract/abi/
--rw-r--r--   0 zihangchen   (501) staff       (20)     9074 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/contract/abi/ClientPayment.json
--rw-r--r--   0 zihangchen   (501) staff       (20)     9742 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/contract/abi/PaymentContract.json
--rw-r--r--   0 zihangchen   (501) staff       (20)     8855 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/contract/abi/SwanToken.json
--rw-r--r--   0 zihangchen   (501) staff       (20)       33 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/contract/abi/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     8797 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/contract/swan_contract.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-04-27 21:43:29.425179 swan_sdk-0.0.1/swan/object/
--rw-r--r--   0 zihangchen   (501) staff       (20)      189 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/object/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)      844 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/object/cp_config.py
--rw-r--r--   0 zihangchen   (501) staff       (20)    13416 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/object/source_uri.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     1198 2024-04-27 18:03:06.000000 swan_sdk-0.0.1/swan/object/task.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-04-27 21:43:29.425951 swan_sdk-0.0.1/swan_sdk.egg-info/
--rw-r--r--   0 zihangchen   (501) staff       (20)     3472 2024-04-27 21:43:29.000000 swan_sdk-0.0.1/swan_sdk.egg-info/PKG-INFO
--rw-r--r--   0 zihangchen   (501) staff       (20)      686 2024-04-27 21:43:29.000000 swan_sdk-0.0.1/swan_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 zihangchen   (501) staff       (20)        1 2024-04-27 21:43:29.000000 swan_sdk-0.0.1/swan_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 zihangchen   (501) staff       (20)       69 2024-04-27 21:43:29.000000 swan_sdk-0.0.1/swan_sdk.egg-info/requires.txt
--rw-r--r--   0 zihangchen   (501) staff       (20)        5 2024-04-27 21:43:29.000000 swan_sdk-0.0.1/swan_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.700455 swan_sdk-0.0.2/
+-rw-r--r--   0 zihangchen   (501) staff       (20)     1072 2024-04-27 21:10:50.000000 swan_sdk-0.0.2/LICENSE
+-rw-r--r--   0 zihangchen   (501) staff       (20)       32 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/MANIFEST.in
+-rw-r--r--   0 zihangchen   (501) staff       (20)     8723 2024-05-03 21:17:38.700163 swan_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 zihangchen   (501) staff       (20)     8184 2024-05-03 21:00:50.000000 swan_sdk-0.0.2/README.md
+-rw-r--r--   0 zihangchen   (501) staff       (20)       38 2024-05-03 21:17:38.700505 swan_sdk-0.0.2/setup.cfg
+-rw-------   0 zihangchen   (501) staff       (20)     1187 2024-05-03 21:17:23.000000 swan_sdk-0.0.2/setup.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.693312 swan_sdk-0.0.2/swan/
+-rw-r--r--   0 zihangchen   (501) staff       (20)      151 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/__init__.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.693920 swan_sdk-0.0.2/swan/api/
+-rw-r--r--   0 zihangchen   (501) staff       (20)       25 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/api/__init__.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)    12210 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/api/swan_api.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)     4279 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/api_client.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.696026 swan_sdk-0.0.2/swan/common/
+-rw-r--r--   0 zihangchen   (501) staff       (20)       27 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/common/__init__.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)      922 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/common/constant.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)      327 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/common/exception.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)      447 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/common/file.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)       26 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/common/params.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)     3256 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/common/utils.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.696565 swan_sdk-0.0.2/swan/contract/
+-rw-r--r--   0 zihangchen   (501) staff       (20)       29 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/__init__.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.698196 swan_sdk-0.0.2/swan/contract/abi/
+-rw-r--r--   0 zihangchen   (501) staff       (20)     9074 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/abi/ClientPayment.json
+-rw-r--r--   0 zihangchen   (501) staff       (20)     9742 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/abi/PaymentContract.json
+-rw-r--r--   0 zihangchen   (501) staff       (20)     8855 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/abi/SwanToken.json
+-rw-r--r--   0 zihangchen   (501) staff       (20)       33 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/abi/__init__.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)     8797 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/swan_contract.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.698813 swan_sdk-0.0.2/swan/object/
+-rw-r--r--   0 zihangchen   (501) staff       (20)      111 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/object/__init__.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)      844 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/object/cp_config.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)     1198 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/object/task.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.699834 swan_sdk-0.0.2/swan_sdk.egg-info/
+-rw-r--r--   0 zihangchen   (501) staff       (20)     8723 2024-05-03 21:17:38.000000 swan_sdk-0.0.2/swan_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 zihangchen   (501) staff       (20)      676 2024-05-03 21:17:38.000000 swan_sdk-0.0.2/swan_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zihangchen   (501) staff       (20)        1 2024-05-03 21:17:38.000000 swan_sdk-0.0.2/swan_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zihangchen   (501) staff       (20)       69 2024-05-03 21:17:38.000000 swan_sdk-0.0.2/swan_sdk.egg-info/requires.txt
+-rw-r--r--   0 zihangchen   (501) staff       (20)        5 2024-05-03 21:17:38.000000 swan_sdk-0.0.2/swan_sdk.egg-info/top_level.txt
```

### Comparing `swan_sdk-0.0.1/LICENSE` & `swan_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.1/setup.py` & `swan_sdk-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
         name="swan-sdk",
-        version="0.0.1",
-        packages=['swan.api', 'swan.common', 'swan.contract', 'swan.object', 'swan.contract.abi'],
+        version="0.0.2",
+        packages=['swan', 'swan.api', 'swan.common', 'swan.contract', 'swan.object', 'swan.contract.abi'],
         # package_data={'swan.contract.abi': ['swan/contract/abi/PaymentContract.json', 'swan/contract/abi/SwanToken.json']},
         include_package_data=True,
         description="A python developer tool kit for Swan Orchestrator services.",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/swanchain/orchestrator-sdk",
         author="SwanCloud",
```

### Comparing `swan_sdk-0.0.1/swan/api/swan_api.py` & `swan_sdk-0.0.2/swan/api/swan_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 
 from eth_account import Account
 from eth_account.messages import encode_defunct
 
 from swan.api_client import APIClient
 from swan.common.constant import *
-from swan.object import HardwareConfig, LagrangeSpace
+from swan.object import HardwareConfig
 from swan.common.exception import SwanAPIException
 
 class SwanAPI(APIClient):
   
     def __init__(self, api_key: str, login: bool = True, environment: str = None, verification: bool = True):
         """Initialize user configuration and login.
```

### Comparing `swan_sdk-0.0.1/swan/common/utils.py` & `swan_sdk-0.0.2/swan/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import requests
 import os
 import json
 import re
 import datetime
 import time
 from urllib.parse import urlparse
-# from swan_mcs import BucketAPI
-# from swan.common import mcs_api
 from swan.common.file import File
 
 def parse_params_to_str(params):
     url = "?"
     for key, value in params.items():
         url = url + str(key) + "=" + str(value) + "&"
     return url[0:-1]
```

### Comparing `swan_sdk-0.0.1/swan/contract/abi/ClientPayment.json` & `swan_sdk-0.0.2/swan/contract/abi/ClientPayment.json`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.1/swan/contract/abi/PaymentContract.json` & `swan_sdk-0.0.2/swan/contract/abi/PaymentContract.json`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.1/swan/contract/abi/SwanToken.json` & `swan_sdk-0.0.2/swan/contract/abi/SwanToken.json`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.1/swan/contract/swan_contract.py` & `swan_sdk-0.0.2/swan/contract/swan_contract.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.1/swan/object/cp_config.py` & `swan_sdk-0.0.2/swan/object/cp_config.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.1/swan/object/task.py` & `swan_sdk-0.0.2/swan/object/task.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.1/swan_sdk.egg-info/SOURCES.txt` & `swan_sdk-0.0.2/swan_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+swan/__init__.py
+swan/api_client.py
 swan/api/__init__.py
-swan/api/mcs_api.py
 swan/api/swan_api.py
 swan/common/__init__.py
 swan/common/constant.py
 swan/common/exception.py
 swan/common/file.py
 swan/common/params.py
 swan/common/utils.py
@@ -15,14 +16,13 @@
 swan/contract/swan_contract.py
 swan/contract/abi/ClientPayment.json
 swan/contract/abi/PaymentContract.json
 swan/contract/abi/SwanToken.json
 swan/contract/abi/__init__.py
 swan/object/__init__.py
 swan/object/cp_config.py
-swan/object/source_uri.py
 swan/object/task.py
 swan_sdk.egg-info/PKG-INFO
 swan_sdk.egg-info/SOURCES.txt
 swan_sdk.egg-info/dependency_links.txt
 swan_sdk.egg-info/requires.txt
 swan_sdk.egg-info/top_level.txt
```


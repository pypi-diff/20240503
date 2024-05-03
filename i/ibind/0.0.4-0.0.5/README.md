# Comparing `tmp/ibind-0.0.4.tar.gz` & `tmp/ibind-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibind-0.0.4.tar", last modified: Fri May  3 04:21:29 2024, max compression
+gzip compressed data, was "ibind-0.0.5.tar", last modified: Fri May  3 06:37:35 2024, max compression
```

## Comparing `ibind-0.0.4.tar` & `ibind-0.0.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.536932 ibind-0.0.4/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    22811 2024-05-03 04:21:29.535338 ibind-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8726 2024-05-02 11:03:33.000000 ibind-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.417988 ibind-0.0.4/ibind/
--rw-rw-rw-   0        0        0     1062 2024-05-02 11:52:19.000000 ibind-0.0.4/ibind/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.443046 ibind-0.0.4/ibind/base/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.0.4/ibind/base/__init__.py
--rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.0.4/ibind/base/queue_controller.py
--rw-rw-rw-   0        0        0     8546 2024-04-24 12:33:10.000000 ibind-0.0.4/ibind/base/rest_client.py
--rw-rw-rw-   0        0        0    16433 2024-05-02 04:33:50.000000 ibind-0.0.4/ibind/base/subscription_controller.py
--rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.0.4/ibind/base/ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.456116 ibind-0.0.4/ibind/client/
--rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.0.4/ibind/client/__init__.py
--rw-rw-rw-   0        0        0     3653 2024-05-03 03:15:23.000000 ibind-0.0.4/ibind/client/ibkr_client.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.481288 ibind-0.0.4/ibind/client/ibkr_client_mixins/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/__init__.py
--rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/accounts_mixin.py
--rw-rw-rw-   0        0        0    16132 2024-04-25 11:38:46.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/contract_mixin.py
--rw-rw-rw-   0        0        0    12508 2024-05-02 07:59:06.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/marketdata_mixin.py
--rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/order_mixin.py
--rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/portfolio_mixin.py
--rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/scanner_mixin.py
--rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/session_mixin.py
--rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/watchlist_mixin.py
--rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.0.4/ibind/client/ibkr_definitions.py
--rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.0.4/ibind/client/ibkr_utils.py
--rw-rw-rw-   0        0        0    23989 2024-05-03 04:14:38.000000 ibind-0.0.4/ibind/client/ibkr_ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.490800 ibind-0.0.4/ibind/support/
--rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.0.4/ibind/support/__init__.py
--rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.0.4/ibind/support/errors.py
--rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.0.4/ibind/support/logs.py
--rw-rw-rw-   0        0        0    11297 2024-05-02 07:22:22.000000 ibind-0.0.4/ibind/support/py_utils.py
--rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.0.4/ibind/var.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.532367 ibind-0.0.4/ibind.egg-info/
--rw-rw-rw-   0        0        0    22811 2024-05-03 04:21:29.000000 ibind-0.0.4/ibind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1595 2024-05-03 04:21:29.000000 ibind-0.0.4/ibind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 04:21:29.000000 ibind-0.0.4/ibind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-03 04:21:29.000000 ibind-0.0.4/ibind.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-03 04:21:29.000000 ibind-0.0.4/ibind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      997 2024-05-03 04:20:43.000000 ibind-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-05-03 04:21:29.538880 ibind-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      225 2024-05-02 11:52:19.000000 ibind-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.495825 ibind-0.0.4/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.0.4/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.498232 ibind-0.0.4/test/integration/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.4/test/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.508776 ibind-0.0.4/test/integration/base/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.0.4/test/integration/base/__init__.py
--rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.0.4/test/integration/base/test_rest_client_i.py
--rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.0.4/test/integration/base/test_websocket_client_i.py
--rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.0.4/test/integration/base/websocketapp_mock.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.521801 ibind-0.0.4/test/integration/client/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.0.4/test/integration/client/__init__.py
--rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.0.4/test/integration/client/ibkr_responses.py
--rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.0.4/test/integration/client/test_ibkr_client_i.py
--rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.0.4/test/integration/client/test_ibkr_utils_i.py
--rw-rw-rw-   0        0        0    18758 2024-04-24 11:56:20.000000 ibind-0.0.4/test/integration/client/test_ibkr_ws_client_i.py
--rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.0.4/test/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.524801 ibind-0.0.4/test/unit/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.4/test/unit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.529366 ibind-0.0.4/test/unit/support/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.0.4/test/unit/support/__init__.py
--rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.0.4/test/unit/support/test_py_utils_u.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.212948 ibind-0.0.5/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    22811 2024-05-03 06:37:35.210709 ibind-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8726 2024-05-02 11:03:33.000000 ibind-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.074068 ibind-0.0.5/ibind/
+-rw-rw-rw-   0        0        0     1062 2024-05-02 11:52:19.000000 ibind-0.0.5/ibind/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.103488 ibind-0.0.5/ibind/base/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.0.5/ibind/base/__init__.py
+-rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.0.5/ibind/base/queue_controller.py
+-rw-rw-rw-   0        0        0     8555 2024-05-03 06:26:53.000000 ibind-0.0.5/ibind/base/rest_client.py
+-rw-rw-rw-   0        0        0    16433 2024-05-03 05:09:05.000000 ibind-0.0.5/ibind/base/subscription_controller.py
+-rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.0.5/ibind/base/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.120566 ibind-0.0.5/ibind/client/
+-rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.0.5/ibind/client/__init__.py
+-rw-rw-rw-   0        0        0     3653 2024-05-03 03:15:23.000000 ibind-0.0.5/ibind/client/ibkr_client.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.151005 ibind-0.0.5/ibind/client/ibkr_client_mixins/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.0.5/ibind/client/ibkr_client_mixins/__init__.py
+-rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.0.5/ibind/client/ibkr_client_mixins/accounts_mixin.py
+-rw-rw-rw-   0        0        0    16132 2024-04-25 11:38:46.000000 ibind-0.0.5/ibind/client/ibkr_client_mixins/contract_mixin.py
+-rw-rw-rw-   0        0        0    12508 2024-05-02 07:59:06.000000 ibind-0.0.5/ibind/client/ibkr_client_mixins/marketdata_mixin.py
+-rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.0.5/ibind/client/ibkr_client_mixins/order_mixin.py
+-rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.0.5/ibind/client/ibkr_client_mixins/portfolio_mixin.py
+-rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.0.5/ibind/client/ibkr_client_mixins/scanner_mixin.py
+-rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.0.5/ibind/client/ibkr_client_mixins/session_mixin.py
+-rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.0.5/ibind/client/ibkr_client_mixins/watchlist_mixin.py
+-rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.0.5/ibind/client/ibkr_definitions.py
+-rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.0.5/ibind/client/ibkr_utils.py
+-rw-rw-rw-   0        0        0    28501 2024-05-03 06:27:53.000000 ibind-0.0.5/ibind/client/ibkr_ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.163597 ibind-0.0.5/ibind/support/
+-rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.0.5/ibind/support/__init__.py
+-rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.0.5/ibind/support/errors.py
+-rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.0.5/ibind/support/logs.py
+-rw-rw-rw-   0        0        0    11297 2024-05-03 05:07:31.000000 ibind-0.0.5/ibind/support/py_utils.py
+-rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.0.5/ibind/var.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.207680 ibind-0.0.5/ibind.egg-info/
+-rw-rw-rw-   0        0        0    22811 2024-05-03 06:37:34.000000 ibind-0.0.5/ibind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1595 2024-05-03 06:37:35.000000 ibind-0.0.5/ibind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 06:37:34.000000 ibind-0.0.5/ibind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-03 06:37:34.000000 ibind-0.0.5/ibind.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-03 06:37:34.000000 ibind-0.0.5/ibind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      997 2024-05-03 06:37:21.000000 ibind-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-05-03 06:37:35.214909 ibind-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      225 2024-05-02 11:52:19.000000 ibind-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.168597 ibind-0.0.5/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.0.5/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.171994 ibind-0.0.5/test/integration/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.5/test/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.183537 ibind-0.0.5/test/integration/base/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.0.5/test/integration/base/__init__.py
+-rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.0.5/test/integration/base/test_rest_client_i.py
+-rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.0.5/test/integration/base/test_websocket_client_i.py
+-rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.0.5/test/integration/base/websocketapp_mock.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.197130 ibind-0.0.5/test/integration/client/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.0.5/test/integration/client/__init__.py
+-rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.0.5/test/integration/client/ibkr_responses.py
+-rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.0.5/test/integration/client/test_ibkr_client_i.py
+-rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.0.5/test/integration/client/test_ibkr_utils_i.py
+-rw-rw-rw-   0        0        0    19149 2024-05-03 06:23:26.000000 ibind-0.0.5/test/integration/client/test_ibkr_ws_client_i.py
+-rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.0.5/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.199124 ibind-0.0.5/test/unit/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.5/test/unit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:37:35.203674 ibind-0.0.5/test/unit/support/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.0.5/test/unit/support/__init__.py
+-rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.0.5/test/unit/support/test_py_utils_u.py
```

### Comparing `ibind-0.0.4/LICENSE` & `ibind-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/PKG-INFO` & `ibind-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibind
-Version: 0.0.4
+Version: 0.0.5
 Summary: IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.
 Author-email: Voy Zan <voy1982@yahoo.co.uk>
 License: Copyright 2020 Voy Zan
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ibind-0.0.4/README.md` & `ibind-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/__init__.py` & `ibind-0.0.5/ibind/__init__.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/base/queue_controller.py` & `ibind-0.0.5/ibind/base/queue_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/base/rest_client.py` & `ibind-0.0.5/ibind/base/rest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from pathlib import Path
 from typing import Union, Optional, Dict, Any
 
 import requests
 from requests import ReadTimeout, Timeout
 
 from ibind import var
-from ibind.support.logs import new_daily_rotating_file_handler, project_logger
 from ibind.support.errors import ExternalBrokerError
+from ibind.support.logs import new_daily_rotating_file_handler, project_logger
 from ibind.support.py_utils import filter_none, UNDEFINED
 
 _LOGGER = project_logger(__file__)
 
 
 @dataclass
 class Result():
@@ -69,20 +69,21 @@
 
     Note:
         - This class is intended to be subclassed by specific API client implementations
           that can provide additional API-specific functionalities.
         - Logging is integrated into request methods, and each request is logged with the specified details.
     """
 
-    def __init__(self,
-                 url: str,
-                 cacert: Union[os.PathLike, bool] = False,
-                 timeout: float = 10,
-                 max_retries: int = 3,
-                 ) -> None:
+    def __init__(
+            self,
+            url: str,
+            cacert: Union[os.PathLike, bool] = False,
+            timeout: float = 10,
+            max_retries: int = 3,
+            ) -> None:
         """
         Parameters:
             url (str): The base URL for the REST API.
             cacert (Union[os.PathLike, bool], optional): Path to the CA certificate file for SSL verification,
                                                          or False to disable SSL verification. Defaults to False.
             timeout (float, optional): Timeout in seconds for the API requests. Defaults to 10.
             max_retries (int, optional): Maximum number of retries for failed API requests. Defaults to 3.
@@ -106,19 +107,18 @@
     def make_logger(self):
         self._logger = new_daily_rotating_file_handler('RestClient', os.path.join(var.LOGS_DIR, f'rest_client'))
 
     @property
     def logger(self):
         try:
             return self._logger
-        except AttributeError:
+        except AttributeError:  # pragma: no cover
             self.make_logger()
             return self._logger
 
-
     def get(self, path: str, params: Optional[Dict[str, Any]] = None, log: bool = True) -> Result:
         return self.request('GET', path, log=log, params=params)
 
     def post(self, path: str, params: Optional[Dict[str, Any]] = None, log: bool = True) -> Result:
         return self.request('POST', path, log=log, json=params)
 
     def delete(self, path: str, params: Optional[Dict[str, Any]] = None, log: bool = True) -> Result:
@@ -184,8 +184,8 @@
             raise ExternalBrokerError(f'{self}: Timeout error ({self._timeout}S)', status_code=response.status_code) from e
         # TODO: add further network exceptions for graceful handling
         # TODO: add JSON parse exception handling
         except Exception as e:
             raise ExternalBrokerError(f'{self}: response error {result} :: {response.status_code} :: {response.reason} :: {response.text}', status_code=response.status_code) from e
 
     def __str__(self):
-        return f'{self.__class__.__qualname__}'
+        return f'{self.__class__.__qualname__}'
```

### Comparing `ibind-0.0.4/ibind/base/subscription_controller.py` & `ibind-0.0.5/ibind/base/subscription_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/base/ws_client.py` & `ibind-0.0.5/ibind/base/ws_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_client.py` & `ibind-0.0.5/ibind/client/ibkr_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_client_mixins/accounts_mixin.py` & `ibind-0.0.5/ibind/client/ibkr_client_mixins/accounts_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_client_mixins/contract_mixin.py` & `ibind-0.0.5/ibind/client/ibkr_client_mixins/contract_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_client_mixins/marketdata_mixin.py` & `ibind-0.0.5/ibind/client/ibkr_client_mixins/marketdata_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_client_mixins/order_mixin.py` & `ibind-0.0.5/ibind/client/ibkr_client_mixins/order_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_client_mixins/portfolio_mixin.py` & `ibind-0.0.5/ibind/client/ibkr_client_mixins/portfolio_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_client_mixins/scanner_mixin.py` & `ibind-0.0.5/ibind/client/ibkr_client_mixins/scanner_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_client_mixins/session_mixin.py` & `ibind-0.0.5/ibind/client/ibkr_client_mixins/session_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_client_mixins/watchlist_mixin.py` & `ibind-0.0.5/ibind/client/ibkr_client_mixins/watchlist_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_definitions.py` & `ibind-0.0.5/ibind/client/ibkr_definitions.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_utils.py` & `ibind-0.0.5/ibind/client/ibkr_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/client/ibkr_ws_client.py` & `ibind-0.0.5/ibind/client/ibkr_ws_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,30 +24,32 @@
     https://ibkrcampus.com/ibkr-api-page/cpapi-v1/#websockets
 
     Enumeration of key types for IBKR WebSocket channels.
 
     This Enum class represents various types of data or subscription channels for IBKR WebSocket API.
 
     Subscriptions Enums:
-        * ACCOUNT_SUMMARY: Represents the 'ACCOUNT_SUMMARY' subscription.
-        * ACCOUNT_LEDGER: Represents the 'ACCOUNT_LEDGER' subscription.
-        * MARKET_DATA: Represents the 'MARKET_DATA' subscription.
-        * MARKET_HISTORY: Represents the 'MARKET_HISTORY' subscription.
+        * ACCOUNT_SUMMARY: Represents the 'ACCOUNT_SUMMARY' subscription. (S) (U)
+        * ACCOUNT_LEDGER: Represents the 'ACCOUNT_LEDGER' subscription. (S) (U)
+        * MARKET_DATA: Represents the 'MARKET_DATA' subscription. (S)
+        * MARKET_HISTORY: Represents the 'MARKET_HISTORY' subscription. (S) (U)
         * PRICE_LADDER: Represents the 'PRICE_LADDER' subscription.
         * ORDERS: Represents the 'ORDERS' subscription.
-        * PNL: Represents the 'PNL' subscription.
-        * TRADES: Represents the 'TRADES' subscription.
+        * PNL: Represents the 'PNL' subscription. (S)
+        * TRADES: Represents the 'TRADES' subscription. (S)
 
     Unsolicited Enums:
         * ACCOUNT_UPDATES: Represents the 'ACCOUNT_UPDATES' unsolicited message.
         * AUTHENTICATION: Represents the 'AUTHENTICATION' unsolicited message.
         * BULLETINS: Represents the 'BULLETINS' unsolicited message.
         * ERROR: Represents the 'ERROR' unsolicited message.
         * SYSTEM: Represents the 'SYSTEM' unsolicited message.
         * NOTIFICATIONS: Represents the 'NOTIFICATIONS' unsolicited message.
+
+    (S) marker indicates that the channel confirms its subscription, while (U) marker indicates that it confirms its unsubscription.
     """
     # subscription-based
     ACCOUNT_SUMMARY = 'ACCOUNT_SUMMARY'
     ACCOUNT_LEDGER = 'ACCOUNT_LEDGER'
     MARKET_DATA = 'MARKET_DATA'
     MARKET_HISTORY = 'MARKET_HISTORY'
     PRICE_LADDER = 'PRICE_LADDER'
@@ -106,14 +108,40 @@
             IbkrWsKey.MARKET_HISTORY: 'mh',
             IbkrWsKey.PRICE_LADDER: 'bd',
             IbkrWsKey.ORDERS: 'or',
             IbkrWsKey.PNL: 'pl',
             IbkrWsKey.TRADES: 'tr',
         }[self]
 
+    @property
+    def confirms_subscribing(self):
+        return {
+            IbkrWsKey.ACCOUNT_SUMMARY: True,
+            IbkrWsKey.ACCOUNT_LEDGER: True,
+            IbkrWsKey.MARKET_DATA: True,
+            IbkrWsKey.MARKET_HISTORY: True,
+            IbkrWsKey.PRICE_LADDER: False,
+            IbkrWsKey.ORDERS: False,
+            IbkrWsKey.PNL: True,
+            IbkrWsKey.TRADES: True,
+        }[self]
+
+    @property
+    def confirms_unsubscribing(self):
+        return {
+            IbkrWsKey.ACCOUNT_SUMMARY: True,
+            IbkrWsKey.ACCOUNT_LEDGER: True,
+            IbkrWsKey.MARKET_DATA: False,
+            IbkrWsKey.MARKET_HISTORY: True,
+            IbkrWsKey.PRICE_LADDER: False,
+            IbkrWsKey.ORDERS: False,
+            IbkrWsKey.PNL: False,
+            IbkrWsKey.TRADES: False,
+        }[self]
+
 
 class IbkrSubscriptionProcessor(SubscriptionProcessor):
     """
     A subscription processor for IBKR WebSocket channels. This class extends the SubscriptionProcessor.
     """
 
     def make_subscribe_payload(self, channel: str, data: dict = None) -> str:
@@ -373,14 +401,19 @@
         if 'message' in message:
             if 'Unsubscribed' in message['message']:
                 self._handle_market_history_unsubscribe(message)
                 return
             elif message['message'] == 'waiting for session':
                 _LOGGER.info(f'{self}: Waiting for an active IBKR session.')
                 return
+        elif 'result' in message:
+            if message['result'] == 'unsubscribed from summary':
+                return self.modify_subscription(f'sd+{self._account_id}', status=False)
+            elif message['result'] == 'unsubscribed from ledger':
+                return self.modify_subscription(f'ld+{self._account_id}', status=False)
 
         _LOGGER.error(f'{self}: Unrecognised message without a topic: {message}')
 
     def _preprocess_raw_message(self, raw_message: str):
         message = json.loads(raw_message)
         # print(message)
         topic = message.get('topic', UNDEFINED)
@@ -497,47 +530,107 @@
         """
         return self._queue_controller.new_queue_accessor(key)
 
     def subscribe(
             self,
             channel: str,
             data: dict = None,
-            needs_confirmation: bool = True,
+            needs_confirmation: bool = None,
             subscription_processor: SubscriptionProcessor = None,
     ) -> bool:  # pragma: no cover
         """
         Subscribes to a specific channel in the IBKR WebSocket.
 
         Initiates a subscription to a given channel, optionally including additional data in the subscription
         request. The method delegates the subscription logic to the SubscriptionController.
 
         From docs: "To receive all orders for the current day the endpoint /iserver/account/orders can be used. It is advised to query all orders for the current day first before subscribing to live orders."
 
         Parameters:
             channel (str): The channel to subscribe to.
             data (dict, optional): Additional data to be included in the subscription request. Defaults to None.
-            needs_confirmation (bool, optional): Specifies whether the subscription requires confirmation from the server. Defaults to True.
+            needs_confirmation (bool, optional): Specifies whether the subscription requires confirmation. If not specified it will be derived from the channel type. Defaults to None.
             subscription_processor (SubscriptionProcessor, optional): The subscription processor to use instead of the
                                                                       default one if provided. Defaults to None.
 
         Returns:
             bool: True if the subscription was successful, False otherwise.
         """
-        if channel == 'or':
+        if channel[:2] == 'or':
             if not self._ibkr_client.check_health():
                 return False
             self._ibkr_client.live_orders(force=True)
             self._ibkr_client.live_orders()
+
+        if needs_confirmation is None:
+            needs_confirmation = IbkrWsKey.from_channel(channel[:2]).confirms_subscribing
+
         return super().subscribe(channel, data, needs_confirmation, subscription_processor)
 
+    def unsubscribe(
+            self,
+            channel: str,
+            data: dict = None,
+            needs_confirmation: bool = None,
+            subscription_processor: SubscriptionProcessor = None,
+    ) -> bool:  # pragma: no cover
+        """
+        Unsubscribes from a specified channel.
+
+        Attempts to unsubscribe from a given channel using the WsClient. The method manages the
+        unsubscription logic, including sending the unsubscription payload and handling retries and timeouts.
+        The subscription status is updated accordingly within the class.
+
+        Parameters:
+            channel (str): The name of the channel to unsubscribe from.
+            data (dict, optional): Additional data to be included in the unsubscription request. Defaults to None.
+            needs_confirmation (bool, optional): Specifies whether the subscription requires confirmation. If not specified it will be derived from the channel type. Defaults to None.
+            subscription_processor (SubscriptionProcessor, optional): The subscription processor to use instead of the
+                                                                      default one if provided. Defaults to None.
+
+        Returns:
+            bool: True if the unsubscription was successful, False otherwise.
+        """
+        if needs_confirmation is None:
+            needs_confirmation = IbkrWsKey.from_channel(channel[:2]).confirms_unsubscribing
+
+        return super().unsubscribe(channel, data, needs_confirmation, subscription_processor)
+
     def _queue_accessor(self, ibkr_ws_key: IbkrWsKey):  # pragma: no cover
         try:
             return self._queue_accessors[ibkr_ws_key]
         except KeyError:
             self._queue_accessors[ibkr_ws_key] = self.new_queue_accessor(ibkr_ws_key)
             return self._queue_accessors[ibkr_ws_key]
 
     def get(self, ibkr_ws_key: IbkrWsKey, block: bool = False, timeout=None):  # pragma: no cover
+        """
+        Facilitates access to data queues by exposing the `get` method of internally-stored QueueAccessor objects.
+
+        Parameters:
+            ibkr_ws_key (IbkrWsKey): The IbkrWsKey of the queue to access.
+            block (bool, optional): Whether to block if the queue is empty. Defaults to False.
+            timeout (Optional[float]): The maximum time in seconds to block waiting for an item.
+                                       A value of None indicates an indefinite wait. Only effective if 'block' is True.
+
+        Returns:
+            The item retrieved from the queue, or None if the queue is empty and 'block' is False.
+
+        Note:
+            - This method is provided for convenience and should not be used in production code. A new QueueAccessor object should be acquired instead using `new_queue_accessor`.
+        """
         return self._queue_accessor(ibkr_ws_key).get(block=block, timeout=timeout)
 
     def empty(self, ibkr_ws_key: IbkrWsKey):  # pragma: no cover
+        """
+        Facilitates access to data queues by exposing the `empty` method of internally-stored QueueAccessor objects.
+
+        Parameters:
+            ibkr_ws_key (IbkrWsKey): The IbkrWsKey of the queue to access.
+
+        Returns:
+             bool: True if the queue is empty, False otherwise.
+
+        Note:
+            - This method is provided for convenience and should not be used in production code. A new QueueAccessor object should be acquired instead using `new_queue_accessor`.
+        """
         return self._queue_accessor(ibkr_ws_key).empty()
```

### Comparing `ibind-0.0.4/ibind/support/logs.py` & `ibind-0.0.5/ibind/support/logs.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/support/py_utils.py` & `ibind-0.0.5/ibind/support/py_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind/var.py` & `ibind-0.0.5/ibind/var.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/ibind.egg-info/PKG-INFO` & `ibind-0.0.5/ibind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibind
-Version: 0.0.4
+Version: 0.0.5
 Summary: IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.
 Author-email: Voy Zan <voy1982@yahoo.co.uk>
 License: Copyright 2020 Voy Zan
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ibind-0.0.4/ibind.egg-info/SOURCES.txt` & `ibind-0.0.5/ibind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/pyproject.toml` & `ibind-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ibind"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="Voy Zan", email="voy1982@yahoo.co.uk" },
 ]
 description = "IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API."
 readme = "README.md"
 requires-python = ">=3.8"
 license={ file = "LICENSE" }
```

### Comparing `ibind-0.0.4/test/integration/base/test_rest_client_i.py` & `ibind-0.0.5/test/integration/base/test_rest_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/test/integration/base/test_websocket_client_i.py` & `ibind-0.0.5/test/integration/base/test_websocket_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/test/integration/base/websocketapp_mock.py` & `ibind-0.0.5/test/integration/base/websocketapp_mock.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/test/integration/client/ibkr_responses.py` & `ibind-0.0.5/test/integration/client/ibkr_responses.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/test/integration/client/test_ibkr_client_i.py` & `ibind-0.0.5/test/integration/client/test_ibkr_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/test/integration/client/test_ibkr_utils_i.py` & `ibind-0.0.5/test/integration/client/test_ibkr_utils_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/test/integration/client/test_ibkr_ws_client_i.py` & `ibind-0.0.5/test/integration/client/test_ibkr_ws_client_i.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from threading import Thread
 from typing import Optional
 from unittest import TestCase
 from unittest.mock import MagicMock, patch, call
 
 import requests
 
+from ibind import Result
 from ibind.client.ibkr_client import IbkrClient
 from ibind.client.ibkr_ws_client import IbkrWsClient, IbkrSubscriptionProcessor, IbkrWsKey
 from test.integration.base.websocketapp_mock import create_wsa_mock, init_wsa_mock
 from ibind.support.logs import project_logger
 from test_utils import RaiseLogsContext, SafeAssertLogs
 
 
@@ -55,20 +56,20 @@
         self.max_ping_interval = 38
 
         self.url_rest = 'https://localhost:5000'
         self.account_id = 'TEST_ACCOUNT_ID'
         self.timeout = 8
         self.max_retries = 4
         self.subscription_retries = 3
-        self.client = IbkrClient(
+        self.client = MagicMock(spec=IbkrClient(
             url=self.url_rest,
             account_id=self.account_id,
             timeout=self.timeout,
             max_retries=self.max_retries,
-        )
+        ))
 
         self.SubscriptionProcessorClass = IbkrSubscriptionProcessor
 
         # Initialize the IbkrWsClient
         self.ws_client = IbkrWsClient(
             url=self.url,
             ibkr_client=self.client,
@@ -125,16 +126,16 @@
                 if response is None:
                     return
                 raw_message = json.dumps(response)
                 wsa_mock._on_message(wsa_mock, raw_message)
 
             self.ws_client.start()
             self.wsa_mock.on_message.side_effect = override_on_message
-            rv = self.ws_client.subscribe(**request)
-            self.ws_client.unsubscribe(**{'channel': request.get('channel'), 'data': request.get('data')})
+            rv = self.ws_client.subscribe(**{'channel': request.get('channel'), 'data': request.get('data'), 'needs_confirmation':request.get('needs_confirmation')})
+            self.ws_client.unsubscribe(**{'channel': request.get('channel'), 'data': request.get('data'), 'needs_confirmation': request.get('confirms_unsubscription')})
             self.ws_client.shutdown()
             return rv
 
         return self.run_in_test_context(run, expected_errors=expected_errors, expect_logs=expect_logs)
 
     def test_on_message_system_heartbeat(self):
         hb = 12345678
@@ -167,14 +168,16 @@
             f"IbkrWsClient: Unrecognised message without a topic: {{'session': {session_id}}}"  # in real scenario this doesn't appear but due to the way the tests are written, this is the expected behaviour
         ]
 
         response_mock = MagicMock(spec=requests.Response)
         response_mock.status_code = 200
         response_mock.json.return_value = {'session': session_id, 'data_to_be_ignored': '1234'}
 
+        self.client.tickle.return_value = Result(data=response_mock.json.return_value)
+
         with patch('ibind.base.rest_client.requests') as requests_mock:
             requests_mock.request.return_value = response_mock
             cm, success = self._send_payload(message_data, expected_errors=expected_errors)
 
         self.assertEqual(expected_errors, [r.msg for r in cm.records])
         self.wsa_mock.send.assert_called_with(f'{{"session": {session_id}}}')
 
@@ -228,15 +231,15 @@
 
         self.assertEqual({self.conid: {'_updated': self.update_time, 'conid': self.conid, 'topic': f'smd+{self.conid}', 'ask_price': '195.26', 'ask_size': '500', 'bid_price': '195.25', 'bid_size': '3,500', 'high': '195.34', 'low': '193.67', 'open': '194.10', 'service_params': '&serviceID1=122&serviceID2=123&serviceID3=203&serviceID4=775&serviceID5=204&serviceID6=206&serviceID7=108&serviceID8=109', 'symbol': 'AAPL', 'volume': '24.2M'}}, queue.get())
 
     def test_on_message_market_history_channel_handling(self):
         queue = self.ws_client.new_queue_accessor(IbkrWsKey.MARKET_HISTORY)
         server_id = 87567
         full_channel = f'{queue.key.channel}+{self.conid}'
-        request = {'channel': f'{full_channel}', 'data': {"period": '1min', "bar": "1min", "outsideRTH": True, "source": "trades", "format": "%o/%c/%h/%l"}}
+        request = {'channel': f'{full_channel}', 'data': {"period": '1min', "bar": "1min", "outsideRTH": True, "source": "trades", "format": "%o/%c/%h/%l"}, 'confirms_unsubscription':False}
         response = {'topic': f's{full_channel}', 'serverId': server_id, '_updated': self.update_time, 'conid': self.conid, 'foo': 'bar'}
 
         self.assertTrue(queue.empty(), 'Queue should be empty')
 
         with patch.object(self.ws_client, 'has_subscription', return_value=True):
             cm, success = self._subscribe(request, response)
             self.assertTrue(success)
@@ -270,21 +273,21 @@
 
         self.assertTrue(queue.empty(), 'Queue should be empty')
 
         with patch.object(self.ws_client, 'has_subscription', return_value=True):
             cm, success = self._subscribe(request, response)
             self.assertTrue(success)
 
-        self.assertEqual(self._logs_subscriptions(full_channel), [r.msg for r in cm.records])
+        self.assertEqual(self._logs_subscriptions(full_channel, None, True, True), [r.msg for r in cm.records])
         self.assertEqual(response, queue.get())
 
     def test_subscription_without_confirmation(self):
         channel = 'fake'
         full_channel = f'{channel}+{self.conid}'
-        request = {'channel': f'{full_channel}', 'needs_confirmation': False}
+        request = {'channel': f'{full_channel}', 'needs_confirmation': False, 'confirms_unsubscription':False}
         response = None
 
         expected_errors = [
             f'IbkrWsClient: Channel subscription timeout: s{full_channel} after {self.subscription_retries} attempts.'
         ]
 
         with patch.object(self.ws_client, 'has_subscription', return_value=True):
```

### Comparing `ibind-0.0.4/test/test_utils.py` & `ibind-0.0.5/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.4/test/unit/support/test_py_utils_u.py` & `ibind-0.0.5/test/unit/support/test_py_utils_u.py`

 * *Files identical despite different names*


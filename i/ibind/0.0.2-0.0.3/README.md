# Comparing `tmp/ibind-0.0.2.tar.gz` & `tmp/ibind-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibind-0.0.2.tar", last modified: Thu May  2 11:01:52 2024, max compression
+gzip compressed data, was "ibind-0.0.3.tar", last modified: Thu May  2 11:42:27 2024, max compression
```

## Comparing `ibind-0.0.2.tar` & `ibind-0.0.3.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.553327 ibind-0.0.2/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     9482 2024-05-02 11:01:52.551327 ibind-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8716 2024-05-02 10:25:06.000000 ibind-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.434199 ibind-0.0.2/ibind/
--rw-rw-rw-   0        0        0     1087 2024-05-02 11:00:44.000000 ibind-0.0.2/ibind/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.459377 ibind-0.0.2/ibind/base/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.0.2/ibind/base/__init__.py
--rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.0.2/ibind/base/queue_controller.py
--rw-rw-rw-   0        0        0     8546 2024-04-24 12:33:10.000000 ibind-0.0.2/ibind/base/rest_client.py
--rw-rw-rw-   0        0        0    16433 2024-05-02 04:33:50.000000 ibind-0.0.2/ibind/base/subscription_controller.py
--rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.0.2/ibind/base/ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.471910 ibind-0.0.2/ibind/client/
--rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.0.2/ibind/client/__init__.py
--rw-rw-rw-   0        0        0     3444 2024-05-02 10:30:13.000000 ibind-0.0.2/ibind/client/ibkr_client.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.494588 ibind-0.0.2/ibind/client/ibkr_client_mixins/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/__init__.py
--rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/accounts_mixin.py
--rw-rw-rw-   0        0        0    16132 2024-04-25 11:38:46.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/contract_mixin.py
--rw-rw-rw-   0        0        0    12508 2024-05-02 07:59:06.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/marketdata_mixin.py
--rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/order_mixin.py
--rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/portfolio_mixin.py
--rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/scanner_mixin.py
--rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/session_mixin.py
--rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/watchlist_mixin.py
--rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.0.2/ibind/client/ibkr_definitions.py
--rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.0.2/ibind/client/ibkr_utils.py
--rw-rw-rw-   0        0        0    22815 2024-05-02 07:55:01.000000 ibind-0.0.2/ibind/client/ibkr_ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.505138 ibind-0.0.2/ibind/support/
--rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.0.2/ibind/support/__init__.py
--rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.0.2/ibind/support/errors.py
--rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.0.2/ibind/support/logs.py
--rw-rw-rw-   0        0        0    11297 2024-05-02 07:22:22.000000 ibind-0.0.2/ibind/support/py_utils.py
--rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.0.2/ibind/var.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.549325 ibind-0.0.2/ibind.egg-info/
--rw-rw-rw-   0        0        0     9482 2024-05-02 11:01:52.000000 ibind-0.0.2/ibind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2024-05-02 11:01:52.000000 ibind-0.0.2/ibind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 11:01:52.000000 ibind-0.0.2/ibind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-02 11:01:52.000000 ibind-0.0.2/ibind.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 11:01:52.000000 ibind-0.0.2/ibind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-02 11:01:52.555328 ibind-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1328 2024-05-02 11:01:12.000000 ibind-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.510513 ibind-0.0.2/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.0.2/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.512543 ibind-0.0.2/test/integration/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.2/test/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.525039 ibind-0.0.2/test/integration/base/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.0.2/test/integration/base/__init__.py
--rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.0.2/test/integration/base/test_rest_client_i.py
--rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.0.2/test/integration/base/test_websocket_client_i.py
--rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.0.2/test/integration/base/websocketapp_mock.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.538105 ibind-0.0.2/test/integration/client/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.0.2/test/integration/client/__init__.py
--rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.0.2/test/integration/client/ibkr_responses.py
--rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.0.2/test/integration/client/test_ibkr_client_i.py
--rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.0.2/test/integration/client/test_ibkr_utils_i.py
--rw-rw-rw-   0        0        0    18758 2024-04-24 11:56:20.000000 ibind-0.0.2/test/integration/client/test_ibkr_ws_client_i.py
--rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.0.2/test/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.541104 ibind-0.0.2/test/unit/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.2/test/unit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.546104 ibind-0.0.2/test/unit/support/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.0.2/test/unit/support/__init__.py
--rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.0.2/test/unit/support/test_py_utils_u.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.661509 ibind-0.0.3/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     9537 2024-05-02 11:42:27.659505 ibind-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8726 2024-05-02 11:03:33.000000 ibind-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.546237 ibind-0.0.3/ibind/
+-rw-rw-rw-   0        0        0     1087 2024-05-02 11:00:44.000000 ibind-0.0.3/ibind/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.574657 ibind-0.0.3/ibind/base/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.0.3/ibind/base/__init__.py
+-rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.0.3/ibind/base/queue_controller.py
+-rw-rw-rw-   0        0        0     8546 2024-04-24 12:33:10.000000 ibind-0.0.3/ibind/base/rest_client.py
+-rw-rw-rw-   0        0        0    16433 2024-05-02 04:33:50.000000 ibind-0.0.3/ibind/base/subscription_controller.py
+-rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.0.3/ibind/base/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.585168 ibind-0.0.3/ibind/client/
+-rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.0.3/ibind/client/__init__.py
+-rw-rw-rw-   0        0        0     3444 2024-05-02 10:30:13.000000 ibind-0.0.3/ibind/client/ibkr_client.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.608198 ibind-0.0.3/ibind/client/ibkr_client_mixins/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/__init__.py
+-rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/accounts_mixin.py
+-rw-rw-rw-   0        0        0    16132 2024-04-25 11:38:46.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/contract_mixin.py
+-rw-rw-rw-   0        0        0    12508 2024-05-02 07:59:06.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/marketdata_mixin.py
+-rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/order_mixin.py
+-rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/portfolio_mixin.py
+-rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/scanner_mixin.py
+-rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/session_mixin.py
+-rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/watchlist_mixin.py
+-rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.0.3/ibind/client/ibkr_definitions.py
+-rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.0.3/ibind/client/ibkr_utils.py
+-rw-rw-rw-   0        0        0    22815 2024-05-02 07:55:01.000000 ibind-0.0.3/ibind/client/ibkr_ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.616716 ibind-0.0.3/ibind/support/
+-rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.0.3/ibind/support/__init__.py
+-rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.0.3/ibind/support/errors.py
+-rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.0.3/ibind/support/logs.py
+-rw-rw-rw-   0        0        0    11297 2024-05-02 07:22:22.000000 ibind-0.0.3/ibind/support/py_utils.py
+-rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.0.3/ibind/var.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.658316 ibind-0.0.3/ibind.egg-info/
+-rw-rw-rw-   0        0        0     9537 2024-05-02 11:42:27.000000 ibind-0.0.3/ibind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1595 2024-05-02 11:42:27.000000 ibind-0.0.3/ibind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 11:42:27.000000 ibind-0.0.3/ibind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-02 11:42:27.000000 ibind-0.0.3/ibind.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 11:42:27.000000 ibind-0.0.3/ibind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      890 2024-05-02 11:40:57.000000 ibind-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-05-02 11:42:27.662510 ibind-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1301 2024-05-02 11:42:13.000000 ibind-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.622227 ibind-0.0.3/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.0.3/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.624227 ibind-0.0.3/test/integration/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.3/test/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.635753 ibind-0.0.3/test/integration/base/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.0.3/test/integration/base/__init__.py
+-rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.0.3/test/integration/base/test_rest_client_i.py
+-rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.0.3/test/integration/base/test_websocket_client_i.py
+-rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.0.3/test/integration/base/websocketapp_mock.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.646776 ibind-0.0.3/test/integration/client/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.0.3/test/integration/client/__init__.py
+-rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.0.3/test/integration/client/ibkr_responses.py
+-rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.0.3/test/integration/client/test_ibkr_client_i.py
+-rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.0.3/test/integration/client/test_ibkr_utils_i.py
+-rw-rw-rw-   0        0        0    18758 2024-04-24 11:56:20.000000 ibind-0.0.3/test/integration/client/test_ibkr_ws_client_i.py
+-rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.0.3/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.650310 ibind-0.0.3/test/unit/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.3/test/unit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.655317 ibind-0.0.3/test/unit/support/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.0.3/test/unit/support/__init__.py
+-rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.0.3/test/unit/support/test_py_utils_u.py
```

### Comparing `ibind-0.0.2/LICENSE` & `ibind-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/PKG-INFO` & `ibind-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: ibind
-Version: 0.0.2
+Version: 0.0.3
 Summary: IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.
 Home-page: https://github.com/Voyz/ibind
 Author: Voy Zan
-Author-email: voy1982@yahoo.co.uk
-License: Apache-2.0
+Author-email: Voy Zan <voy1982@yahoo.co.uk>
+Project-URL: Homepage, https://github.com/Voyz/ibind
 Keywords: interactive brokers,rest api,python api,ibkr python api,ibkr web api,ib api,ibkr api,algo trading,algorithmic trading,quant,trading
 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.*
 Requires-Dist: websocket-client==1.7.*
 
 *This library is currently being beta-tested. See something that's broken? Did we get something
 wrong? [Create an issue and let us know!][issues]*
 
 
 
 <p align="center">
     <a id="ibind" href="#ibind">
-        <img src="https://github.com/Voyz/ibind/blob/master/media/ibind_logo.png" alt="IBind logo" title="IBind logo" width="600"/>
+        <img src="https://raw.githubusercontent.com/Voyz/ibind/master/media/ibind_logo.png" alt="IBind logo" title="IBind logo" width="600"/>
     </a>
 </p>
 <p align="center">
     <a href="https://opensource.org/licenses/Apache-2.0">
         <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"/>
     </a>
     <a href="https://github.com/Voyz/ibind/releases">
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: ibind Version: 0.0.2 Summary: IBind is a REST and
+Metadata-Version: 2.1 Name: ibind Version: 0.0.3 Summary: IBind is a REST and
 WebSocket client library for Interactive Brokers Client Portal Web API. Home-
-page: https://github.com/Voyz/ibind Author: Voy Zan Author-email:
-voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive brokers,rest
-api,python api,ibkr python api,ibkr web api,ib api,ibkr api,algo
-trading,algorithmic trading,quant,trading Classifier: Development Status :: 4 -
-Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Programming Language ::
-Python :: 3.12 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: requests==2.31.* Requires-Dist: websocket-client==1.7.* *This
-library is currently being beta-tested. See something that's broken? Did we get
-something wrong? [Create an issue and let us know!][issues]*
+page: https://github.com/Voyz/ibind Author: Voy Zan Author-email: Voy Zan
+yahoo.co.uk> Project-URL: Homepage, https://github.com/Voyz/ibind Keywords:
+interactive brokers,rest api,python api,ibkr python api,ibkr web api,ib
+api,ibkr api,algo trading,algorithmic trading,quant,trading Classifier:
+Development Status :: 4 - Beta Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: requests==2.31.* Requires-Dist:
+websocket-client==1.7.* *This library is currently being beta-tested. See
+something that's broken? Did we get something wrong? [Create an issue and let
+us know!][issues]*
                                  _[_I_B_i_n_d_ _l_o_g_o_]
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
                   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_i_b_i_n_d_?_l_a_b_e_l_=_v_e_r_s_i_o_n_]
 IBind is a REST and WebSocket client library for [Interactive Brokers Client
 Portal Web API.][ibkr-docs] ## Installation ```rich pip install ibind ``` Use
 [IBeam][ibeam] along with this library for easier authentication with IBKR. ##
 Documentation See full [IBind documentation][wiki]. * [Installation][wiki-
```

### Comparing `ibind-0.0.2/README.md` & `ibind-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 *This library is currently being beta-tested. See something that's broken? Did we get something
 wrong? [Create an issue and let us know!][issues]*
 
 
 
 <p align="center">
     <a id="ibind" href="#ibind">
-        <img src="https://github.com/Voyz/ibind/blob/master/media/ibind_logo.png" alt="IBind logo" title="IBind logo" width="600"/>
+        <img src="https://raw.githubusercontent.com/Voyz/ibind/master/media/ibind_logo.png" alt="IBind logo" title="IBind logo" width="600"/>
     </a>
 </p>
 <p align="center">
     <a href="https://opensource.org/licenses/Apache-2.0">
         <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"/>
     </a>
     <a href="https://github.com/Voyz/ibind/releases">
```

### Comparing `ibind-0.0.2/ibind/__init__.py` & `ibind-0.0.3/ibind/__init__.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/base/queue_controller.py` & `ibind-0.0.3/ibind/base/queue_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/base/rest_client.py` & `ibind-0.0.3/ibind/base/rest_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/base/subscription_controller.py` & `ibind-0.0.3/ibind/base/subscription_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/base/ws_client.py` & `ibind-0.0.3/ibind/base/ws_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_client.py` & `ibind-0.0.3/ibind/client/ibkr_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_client_mixins/accounts_mixin.py` & `ibind-0.0.3/ibind/client/ibkr_client_mixins/accounts_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_client_mixins/contract_mixin.py` & `ibind-0.0.3/ibind/client/ibkr_client_mixins/contract_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_client_mixins/marketdata_mixin.py` & `ibind-0.0.3/ibind/client/ibkr_client_mixins/marketdata_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_client_mixins/order_mixin.py` & `ibind-0.0.3/ibind/client/ibkr_client_mixins/order_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_client_mixins/portfolio_mixin.py` & `ibind-0.0.3/ibind/client/ibkr_client_mixins/portfolio_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_client_mixins/scanner_mixin.py` & `ibind-0.0.3/ibind/client/ibkr_client_mixins/scanner_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_client_mixins/session_mixin.py` & `ibind-0.0.3/ibind/client/ibkr_client_mixins/session_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_client_mixins/watchlist_mixin.py` & `ibind-0.0.3/ibind/client/ibkr_client_mixins/watchlist_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_definitions.py` & `ibind-0.0.3/ibind/client/ibkr_definitions.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_utils.py` & `ibind-0.0.3/ibind/client/ibkr_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/client/ibkr_ws_client.py` & `ibind-0.0.3/ibind/client/ibkr_ws_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/support/logs.py` & `ibind-0.0.3/ibind/support/logs.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/support/py_utils.py` & `ibind-0.0.3/ibind/support/py_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind/var.py` & `ibind-0.0.3/ibind/var.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/ibind.egg-info/PKG-INFO` & `ibind-0.0.3/ibind.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: ibind
-Version: 0.0.2
+Version: 0.0.3
 Summary: IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.
 Home-page: https://github.com/Voyz/ibind
 Author: Voy Zan
-Author-email: voy1982@yahoo.co.uk
-License: Apache-2.0
+Author-email: Voy Zan <voy1982@yahoo.co.uk>
+Project-URL: Homepage, https://github.com/Voyz/ibind
 Keywords: interactive brokers,rest api,python api,ibkr python api,ibkr web api,ib api,ibkr api,algo trading,algorithmic trading,quant,trading
 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.*
 Requires-Dist: websocket-client==1.7.*
 
 *This library is currently being beta-tested. See something that's broken? Did we get something
 wrong? [Create an issue and let us know!][issues]*
 
 
 
 <p align="center">
     <a id="ibind" href="#ibind">
-        <img src="https://github.com/Voyz/ibind/blob/master/media/ibind_logo.png" alt="IBind logo" title="IBind logo" width="600"/>
+        <img src="https://raw.githubusercontent.com/Voyz/ibind/master/media/ibind_logo.png" alt="IBind logo" title="IBind logo" width="600"/>
     </a>
 </p>
 <p align="center">
     <a href="https://opensource.org/licenses/Apache-2.0">
         <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"/>
     </a>
     <a href="https://github.com/Voyz/ibind/releases">
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: ibind Version: 0.0.2 Summary: IBind is a REST and
+Metadata-Version: 2.1 Name: ibind Version: 0.0.3 Summary: IBind is a REST and
 WebSocket client library for Interactive Brokers Client Portal Web API. Home-
-page: https://github.com/Voyz/ibind Author: Voy Zan Author-email:
-voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive brokers,rest
-api,python api,ibkr python api,ibkr web api,ib api,ibkr api,algo
-trading,algorithmic trading,quant,trading Classifier: Development Status :: 4 -
-Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Programming Language ::
-Python :: 3.12 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: requests==2.31.* Requires-Dist: websocket-client==1.7.* *This
-library is currently being beta-tested. See something that's broken? Did we get
-something wrong? [Create an issue and let us know!][issues]*
+page: https://github.com/Voyz/ibind Author: Voy Zan Author-email: Voy Zan
+yahoo.co.uk> Project-URL: Homepage, https://github.com/Voyz/ibind Keywords:
+interactive brokers,rest api,python api,ibkr python api,ibkr web api,ib
+api,ibkr api,algo trading,algorithmic trading,quant,trading Classifier:
+Development Status :: 4 - Beta Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: requests==2.31.* Requires-Dist:
+websocket-client==1.7.* *This library is currently being beta-tested. See
+something that's broken? Did we get something wrong? [Create an issue and let
+us know!][issues]*
                                  _[_I_B_i_n_d_ _l_o_g_o_]
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
                   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_i_b_i_n_d_?_l_a_b_e_l_=_v_e_r_s_i_o_n_]
 IBind is a REST and WebSocket client library for [Interactive Brokers Client
 Portal Web API.][ibkr-docs] ## Installation ```rich pip install ibind ``` Use
 [IBeam][ibeam] along with this library for easier authentication with IBKR. ##
 Documentation See full [IBind documentation][wiki]. * [Installation][wiki-
```

### Comparing `ibind-0.0.2/ibind.egg-info/SOURCES.txt` & `ibind-0.0.3/ibind.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 ibind/__init__.py
 ibind/var.py
 ibind.egg-info/PKG-INFO
 ibind.egg-info/SOURCES.txt
 ibind.egg-info/dependency_links.txt
```

### Comparing `ibind-0.0.2/setup.py` & `ibind-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='ibind',
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests", "examples", "docs", "out", "dist"]),
     version=ibind.__version__,
-    license='Apache-2.0',
     description='IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Voy Zan',
     author_email='voy1982@yahoo.co.uk',
     url='https://github.com/Voyz/ibind',
     keywords=['interactive brokers', 'rest api', 'python api', 'ibkr python api', 'ibkr web api', 'ib api', 'ibkr api', 'algo trading', 'algorithmic trading', 'quant', 'trading'],
```

### Comparing `ibind-0.0.2/test/integration/base/test_rest_client_i.py` & `ibind-0.0.3/test/integration/base/test_rest_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/test/integration/base/test_websocket_client_i.py` & `ibind-0.0.3/test/integration/base/test_websocket_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/test/integration/base/websocketapp_mock.py` & `ibind-0.0.3/test/integration/base/websocketapp_mock.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/test/integration/client/ibkr_responses.py` & `ibind-0.0.3/test/integration/client/ibkr_responses.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/test/integration/client/test_ibkr_client_i.py` & `ibind-0.0.3/test/integration/client/test_ibkr_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/test/integration/client/test_ibkr_utils_i.py` & `ibind-0.0.3/test/integration/client/test_ibkr_utils_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/test/integration/client/test_ibkr_ws_client_i.py` & `ibind-0.0.3/test/integration/client/test_ibkr_ws_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/test/test_utils.py` & `ibind-0.0.3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.2/test/unit/support/test_py_utils_u.py` & `ibind-0.0.3/test/unit/support/test_py_utils_u.py`

 * *Files identical despite different names*


# Comparing `tmp/ibind-0.0.3.tar.gz` & `tmp/ibind-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibind-0.0.3.tar", last modified: Thu May  2 11:42:27 2024, max compression
+gzip compressed data, was "ibind-0.0.4.tar", last modified: Fri May  3 04:21:29 2024, max compression
```

## Comparing `ibind-0.0.3.tar` & `ibind-0.0.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.661509 ibind-0.0.3/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     9537 2024-05-02 11:42:27.659505 ibind-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8726 2024-05-02 11:03:33.000000 ibind-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.546237 ibind-0.0.3/ibind/
--rw-rw-rw-   0        0        0     1087 2024-05-02 11:00:44.000000 ibind-0.0.3/ibind/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.574657 ibind-0.0.3/ibind/base/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.0.3/ibind/base/__init__.py
--rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.0.3/ibind/base/queue_controller.py
--rw-rw-rw-   0        0        0     8546 2024-04-24 12:33:10.000000 ibind-0.0.3/ibind/base/rest_client.py
--rw-rw-rw-   0        0        0    16433 2024-05-02 04:33:50.000000 ibind-0.0.3/ibind/base/subscription_controller.py
--rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.0.3/ibind/base/ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.585168 ibind-0.0.3/ibind/client/
--rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.0.3/ibind/client/__init__.py
--rw-rw-rw-   0        0        0     3444 2024-05-02 10:30:13.000000 ibind-0.0.3/ibind/client/ibkr_client.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.608198 ibind-0.0.3/ibind/client/ibkr_client_mixins/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/__init__.py
--rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/accounts_mixin.py
--rw-rw-rw-   0        0        0    16132 2024-04-25 11:38:46.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/contract_mixin.py
--rw-rw-rw-   0        0        0    12508 2024-05-02 07:59:06.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/marketdata_mixin.py
--rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/order_mixin.py
--rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/portfolio_mixin.py
--rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/scanner_mixin.py
--rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/session_mixin.py
--rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.0.3/ibind/client/ibkr_client_mixins/watchlist_mixin.py
--rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.0.3/ibind/client/ibkr_definitions.py
--rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.0.3/ibind/client/ibkr_utils.py
--rw-rw-rw-   0        0        0    22815 2024-05-02 07:55:01.000000 ibind-0.0.3/ibind/client/ibkr_ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.616716 ibind-0.0.3/ibind/support/
--rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.0.3/ibind/support/__init__.py
--rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.0.3/ibind/support/errors.py
--rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.0.3/ibind/support/logs.py
--rw-rw-rw-   0        0        0    11297 2024-05-02 07:22:22.000000 ibind-0.0.3/ibind/support/py_utils.py
--rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.0.3/ibind/var.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.658316 ibind-0.0.3/ibind.egg-info/
--rw-rw-rw-   0        0        0     9537 2024-05-02 11:42:27.000000 ibind-0.0.3/ibind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1595 2024-05-02 11:42:27.000000 ibind-0.0.3/ibind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 11:42:27.000000 ibind-0.0.3/ibind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-02 11:42:27.000000 ibind-0.0.3/ibind.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 11:42:27.000000 ibind-0.0.3/ibind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      890 2024-05-02 11:40:57.000000 ibind-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-05-02 11:42:27.662510 ibind-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1301 2024-05-02 11:42:13.000000 ibind-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.622227 ibind-0.0.3/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.0.3/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.624227 ibind-0.0.3/test/integration/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.3/test/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.635753 ibind-0.0.3/test/integration/base/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.0.3/test/integration/base/__init__.py
--rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.0.3/test/integration/base/test_rest_client_i.py
--rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.0.3/test/integration/base/test_websocket_client_i.py
--rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.0.3/test/integration/base/websocketapp_mock.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.646776 ibind-0.0.3/test/integration/client/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.0.3/test/integration/client/__init__.py
--rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.0.3/test/integration/client/ibkr_responses.py
--rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.0.3/test/integration/client/test_ibkr_client_i.py
--rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.0.3/test/integration/client/test_ibkr_utils_i.py
--rw-rw-rw-   0        0        0    18758 2024-04-24 11:56:20.000000 ibind-0.0.3/test/integration/client/test_ibkr_ws_client_i.py
--rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.0.3/test/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.650310 ibind-0.0.3/test/unit/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.3/test/unit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 11:42:27.655317 ibind-0.0.3/test/unit/support/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.0.3/test/unit/support/__init__.py
--rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.0.3/test/unit/support/test_py_utils_u.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.536932 ibind-0.0.4/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    22811 2024-05-03 04:21:29.535338 ibind-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8726 2024-05-02 11:03:33.000000 ibind-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.417988 ibind-0.0.4/ibind/
+-rw-rw-rw-   0        0        0     1062 2024-05-02 11:52:19.000000 ibind-0.0.4/ibind/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.443046 ibind-0.0.4/ibind/base/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.0.4/ibind/base/__init__.py
+-rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.0.4/ibind/base/queue_controller.py
+-rw-rw-rw-   0        0        0     8546 2024-04-24 12:33:10.000000 ibind-0.0.4/ibind/base/rest_client.py
+-rw-rw-rw-   0        0        0    16433 2024-05-02 04:33:50.000000 ibind-0.0.4/ibind/base/subscription_controller.py
+-rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.0.4/ibind/base/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.456116 ibind-0.0.4/ibind/client/
+-rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.0.4/ibind/client/__init__.py
+-rw-rw-rw-   0        0        0     3653 2024-05-03 03:15:23.000000 ibind-0.0.4/ibind/client/ibkr_client.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.481288 ibind-0.0.4/ibind/client/ibkr_client_mixins/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/__init__.py
+-rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/accounts_mixin.py
+-rw-rw-rw-   0        0        0    16132 2024-04-25 11:38:46.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/contract_mixin.py
+-rw-rw-rw-   0        0        0    12508 2024-05-02 07:59:06.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/marketdata_mixin.py
+-rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/order_mixin.py
+-rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/portfolio_mixin.py
+-rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/scanner_mixin.py
+-rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/session_mixin.py
+-rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.0.4/ibind/client/ibkr_client_mixins/watchlist_mixin.py
+-rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.0.4/ibind/client/ibkr_definitions.py
+-rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.0.4/ibind/client/ibkr_utils.py
+-rw-rw-rw-   0        0        0    23989 2024-05-03 04:14:38.000000 ibind-0.0.4/ibind/client/ibkr_ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.490800 ibind-0.0.4/ibind/support/
+-rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.0.4/ibind/support/__init__.py
+-rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.0.4/ibind/support/errors.py
+-rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.0.4/ibind/support/logs.py
+-rw-rw-rw-   0        0        0    11297 2024-05-02 07:22:22.000000 ibind-0.0.4/ibind/support/py_utils.py
+-rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.0.4/ibind/var.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.532367 ibind-0.0.4/ibind.egg-info/
+-rw-rw-rw-   0        0        0    22811 2024-05-03 04:21:29.000000 ibind-0.0.4/ibind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1595 2024-05-03 04:21:29.000000 ibind-0.0.4/ibind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 04:21:29.000000 ibind-0.0.4/ibind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-03 04:21:29.000000 ibind-0.0.4/ibind.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-03 04:21:29.000000 ibind-0.0.4/ibind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      997 2024-05-03 04:20:43.000000 ibind-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-05-03 04:21:29.538880 ibind-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      225 2024-05-02 11:52:19.000000 ibind-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.495825 ibind-0.0.4/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.0.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.498232 ibind-0.0.4/test/integration/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.4/test/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.508776 ibind-0.0.4/test/integration/base/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.0.4/test/integration/base/__init__.py
+-rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.0.4/test/integration/base/test_rest_client_i.py
+-rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.0.4/test/integration/base/test_websocket_client_i.py
+-rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.0.4/test/integration/base/websocketapp_mock.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.521801 ibind-0.0.4/test/integration/client/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.0.4/test/integration/client/__init__.py
+-rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.0.4/test/integration/client/ibkr_responses.py
+-rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.0.4/test/integration/client/test_ibkr_client_i.py
+-rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.0.4/test/integration/client/test_ibkr_utils_i.py
+-rw-rw-rw-   0        0        0    18758 2024-04-24 11:56:20.000000 ibind-0.0.4/test/integration/client/test_ibkr_ws_client_i.py
+-rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.0.4/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.524801 ibind-0.0.4/test/unit/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.4/test/unit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:21:29.529366 ibind-0.0.4/test/unit/support/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.0.4/test/unit/support/__init__.py
+-rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.0.4/test/unit/support/test_py_utils_u.py
```

### Comparing `ibind-0.0.3/LICENSE` & `ibind-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/PKG-INFO` & `ibind-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: ibind
-Version: 0.0.3
-Summary: IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.
-Home-page: https://github.com/Voyz/ibind
-Author: Voy Zan
-Author-email: Voy Zan <voy1982@yahoo.co.uk>
-Project-URL: Homepage, https://github.com/Voyz/ibind
-Keywords: interactive brokers,rest api,python api,ibkr python api,ibkr web api,ib api,ibkr api,algo trading,algorithmic trading,quant,trading
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests==2.31.*
-Requires-Dist: websocket-client==1.7.*
-
 *This library is currently being beta-tested. See something that's broken? Did we get something
 wrong? [Create an issue and let us know!][issues]*
 
 
 
 <p align="center">
     <a id="ibind" href="#ibind">
```

#### html2text {}

```diff
@@ -1,20 +1,9 @@
-Metadata-Version: 2.1 Name: ibind Version: 0.0.3 Summary: IBind is a REST and
-WebSocket client library for Interactive Brokers Client Portal Web API. Home-
-page: https://github.com/Voyz/ibind Author: Voy Zan Author-email: Voy Zan
-yahoo.co.uk> Project-URL: Homepage, https://github.com/Voyz/ibind Keywords:
-interactive brokers,rest api,python api,ibkr python api,ibkr web api,ib
-api,ibkr api,algo trading,algorithmic trading,quant,trading Classifier:
-Development Status :: 4 - Beta Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: requests==2.31.* Requires-Dist:
-websocket-client==1.7.* *This library is currently being beta-tested. See
-something that's broken? Did we get something wrong? [Create an issue and let
-us know!][issues]*
+*This library is currently being beta-tested. See something that's broken? Did
+we get something wrong? [Create an issue and let us know!][issues]*
                                  _[_I_B_i_n_d_ _l_o_g_o_]
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
                   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_i_b_i_n_d_?_l_a_b_e_l_=_v_e_r_s_i_o_n_]
 IBind is a REST and WebSocket client library for [Interactive Brokers Client
 Portal Web API.][ibkr-docs] ## Installation ```rich pip install ibind ``` Use
 [IBeam][ibeam] along with this library for easier authentication with IBKR. ##
 Documentation See full [IBind documentation][wiki]. * [Installation][wiki-
```

### Comparing `ibind-0.0.3/ibind/__init__.py` & `ibind-0.0.4/ibind/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,9 +25,7 @@
     'snapshot_keys_to_ids',
     'Result',
     'QueueAccessor',
     'execute_in_parallel',
     'ExternalBrokerError',
 ]
 
-__version__ = "0.0.2"
-
```

### Comparing `ibind-0.0.3/ibind/base/queue_controller.py` & `ibind-0.0.4/ibind/base/queue_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/base/rest_client.py` & `ibind-0.0.4/ibind/base/rest_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/base/subscription_controller.py` & `ibind-0.0.4/ibind/base/subscription_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/base/ws_client.py` & `ibind-0.0.4/ibind/base/ws_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/client/ibkr_client.py` & `ibind-0.0.4/ibind/client/ibkr_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 _LOGGER = project_logger(__file__)
 
 
 
 
 class IbkrClient(RestClient, AccountsMixin, ContractMixin, MarketdataMixin, OrderMixin, PortfolioMixin, ScannerMixin, SessionMixin, WatchlistMixin):
     """
-    A client class for interfacing with the Interactive Brokers API, extending the RestClient class.
+    A client class for interfacing with the IBKR API, extending the RestClient class.
 
-    This subclass of RestClient is specifically designed for the Interactive Brokers API. It inherits
+    This subclass of RestClient is specifically designed for the IBKR API. It inherits
     the foundational REST API interaction capabilities from RestClient and adds functionalities
-    particular to the Interactive Brokers API, such as specific endpoint handling.
+    particular to the IBKR API, such as specific endpoint handling.
 
-    The class provides methods to perform various operations with the Interactive Brokers API, such as
+    The class provides methods to perform various operations with the IBKR API, such as
     fetching stock data, submitting orders, and managing account information.
 
     See: https://interactivebrokers.github.io/cpwebapi/endpoints
 
     Note:
         - All endpoint mappings are defined as class mixins, categorised similar to the IBKR REST API documentation. See appropriate mixins for more information. 
     """
@@ -44,16 +44,19 @@
             base_route: str = '/v1/api/',
             cacert: Union[str, os.PathLike, bool] = var.IBIND_CACERT,
             timeout: float = 10,
             max_retries: int = 3,
     ) -> None:
         """
         Parameters:
-            url (str): The base URL for the REST API.
             account_id (str): An identifier for the account.
+            url (str): The base URL for the REST API.
+            host (str, optional): Host for the IBKR REST API. Defaults to 'localhost'.
+            port (str, optional): Port for the IBKR REST API. Defaults to '5000'
+            base_route (str, optional): Base route for the IBKR REST API. Defaults to '/v1/api/'.
             cacert (Union[os.PathLike, bool], optional): Path to the CA certificate file for SSL verification,
                                                          or False to disable SSL verification. Defaults to False.
             timeout (float, optional): Timeout in seconds for the API requests. Defaults to 10.
             max_retries (int, optional): Maximum number of retries for failed API requests. Defaults to 3.
         """
 
         if url is None:
```

### Comparing `ibind-0.0.3/ibind/client/ibkr_client_mixins/accounts_mixin.py` & `ibind-0.0.4/ibind/client/ibkr_client_mixins/accounts_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/client/ibkr_client_mixins/contract_mixin.py` & `ibind-0.0.4/ibind/client/ibkr_client_mixins/contract_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/client/ibkr_client_mixins/marketdata_mixin.py` & `ibind-0.0.4/ibind/client/ibkr_client_mixins/marketdata_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/client/ibkr_client_mixins/order_mixin.py` & `ibind-0.0.4/ibind/client/ibkr_client_mixins/order_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/client/ibkr_client_mixins/portfolio_mixin.py` & `ibind-0.0.4/ibind/client/ibkr_client_mixins/portfolio_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/client/ibkr_client_mixins/scanner_mixin.py` & `ibind-0.0.4/ibind/client/ibkr_client_mixins/scanner_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/client/ibkr_client_mixins/session_mixin.py` & `ibind-0.0.4/ibind/client/ibkr_client_mixins/session_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/client/ibkr_client_mixins/watchlist_mixin.py` & `ibind-0.0.4/ibind/client/ibkr_client_mixins/watchlist_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/client/ibkr_definitions.py` & `ibind-0.0.4/ibind/client/ibkr_definitions.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/client/ibkr_utils.py` & `ibind-0.0.4/ibind/client/ibkr_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/client/ibkr_ws_client.py` & `ibind-0.0.4/ibind/client/ibkr_ws_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 _LOGGER = project_logger(__file__)
 
 
 class IbkrWsKey(Enum):
     """
     https://ibkrcampus.com/ibkr-api-page/cpapi-v1/#websockets
 
-    Enumeration of key types for Interactive Brokers WebSocket channels.
+    Enumeration of key types for IBKR WebSocket channels.
 
-    This Enum class represents various types of data or subscription channels for Interactive Brokers WebSocket API.
+    This Enum class represents various types of data or subscription channels for IBKR WebSocket API.
 
     Subscriptions Enums:
         * ACCOUNT_SUMMARY: Represents the 'ACCOUNT_SUMMARY' subscription.
         * ACCOUNT_LEDGER: Represents the 'ACCOUNT_LEDGER' subscription.
         * MARKET_DATA: Represents the 'MARKET_DATA' subscription.
         * MARKET_HISTORY: Represents the 'MARKET_HISTORY' subscription.
         * PRICE_LADDER: Represents the 'PRICE_LADDER' subscription.
@@ -109,30 +109,30 @@
             IbkrWsKey.PNL: 'pl',
             IbkrWsKey.TRADES: 'tr',
         }[self]
 
 
 class IbkrSubscriptionProcessor(SubscriptionProcessor):
     """
-    A subscription processor for Interactive Brokers WebSocket channels. This class extends the SubscriptionProcessor.
+    A subscription processor for IBKR WebSocket channels. This class extends the SubscriptionProcessor.
     """
 
     def make_subscribe_payload(self, channel: str, data: dict = None) -> str:
         """
         Constructs a subscription payload for a specific channel with optional data.
 
         The payload format is a combination of a prefix 's', the channel identifier, and the JSON-serialized
         data if provided.
 
         Parameters:
             channel (str): The channel identifier to subscribe to.
             data (dict, optional): Additional data to be included in the subscription payload. Defaults to None.
 
         Returns:
-            str: A formatted subscription payload for the Interactive Brokers WebSocket.
+            str: A formatted subscription payload for the IBKR WebSocket.
 
         Example:
             - With data: make_subscribe_payload('md', {'foo': 'bar'}) returns "smd+{"foo": "bar"}"
             - Without data: make_subscribe_payload('md') returns "smd"
         """
         payload = f"s{channel}"
 
@@ -149,89 +149,99 @@
         data. If data is not provided, an empty dictionary is used.
 
         Parameters:
             channel (str): The channel identifier to unsubscribe from.
             data (dict, optional): Additional data to be included in the unsubscription payload. Defaults to None.
 
         Returns:
-            str: A formatted unsubscription payload for the Interactive Brokers WebSocket.
+            str: A formatted unsubscription payload for the IBKR WebSocket.
 
         Example:
             - With data: make_unsubscribe_payload('md', {'foo': 'bar'}) returns "umd+{"foo": "bar"}"
             - Without data: make_unsubscribe_payload('md') returns "umd+{}"
         """
         data = {} if data is None else data
         return f'u{channel}+{json.dumps(data)}'
 
 
 class IbkrWsClient(WsClient):
     """
-    A WebSocket client for Interactive Brokers, extending WsClient.
+    A WebSocket client for IBKR, extending WsClient.
 
-    This class handles WebSocket communications specific to Interactive Brokers, managing subscriptions,
+    This class handles WebSocket communications specific to IBKR, managing subscriptions,
     message processing, and maintaining the health of the WebSocket connection.
 
     See: https://interactivebrokers.github.io/cpwebapi/websockets
     """
 
     def __init__(
             self,
-            ibkr_client: IbkrClient,
             account_id: str = var.IBIND_ACCOUNT_ID,
             url: str = var.IBIND_WS_URL,
             host: str = 'localhost',
             port: str = '5000',
             base_route: str = '/v1/api/ws',
+            ibkr_client: IbkrClient = None,
             SubscriptionProcessorClass: Type[SubscriptionProcessor] = IbkrSubscriptionProcessor,
             QueueControllerClass: Type[QueueController] = QueueController[IbkrWsKey],
             log_raw_messages: bool = var.IBIND_WS_LOG_RAW_MESSAGES,
             unsolicited_channels_to_be_queued: List[IbkrWsKey] = None,
+            start: bool = False,
             # inherited
             ping_interval: int = var.IBIND_WS_PING_INTERVAL,
             max_ping_interval: int = var.IBIND_WS_MAX_PING_INTERVAL,
             timeout: float = var.IBIND_WS_TIMEOUT,
             restart_on_close: bool = True,
             restart_on_critical: bool = True,
             max_connection_attempts: int = 10,
             cacert: Union[str, bool] = var.IBIND_CACERT,
             # subscription controller
             subscription_retries: int = var.IBIND_WS_SUBSCRIPTION_RETRIES,
             subscription_timeout: float = var.IBIND_WS_SUBSCRIPTION_TIMEOUT,
     ) -> None:
         """
-        Initializes the IbkrWsClient, an Interactive Brokers WebSocket client.
+        Initializes the IbkrWsClient, an IBKR WebSocket client.
 
-        Sets up the client with necessary configurations for connecting to and interacting with the Interactive Brokers WebSocket.
+        Sets up the client with necessary configurations for connecting to and interacting with the IBKR WebSocket.
 
         Parameters:
-            url (str): URL for the Interactive Brokers WebSocket.
-            ibkr_client (IbkrClient): An instance of the IbkrClient for related operations.
-            account_id (str): Account ID for subscription management.
+            url (str, optional): URL for the IBKR WebSocket.
+            host (str, optional): Host for the IBKR WebSocket API. Defaults to 'localhost'.
+            port (str, optional): Port for the IBKR WebSocket API. Defaults to '5000'
+            base_route (str, optional): Base route for the IBKR WebSocket API. Defaults to '/v1/api/ws'.
+            account_id (str, optional): Account ID for subscription management.
+            ibkr_client (IbkrClient, optional): An instance of the IbkrClient for related operations.
             SubscriptionProcessorClass (Type[SubscriptionProcessor]): The class to process subscription payloads.
             QueueControllerClass (Type[QueueController[IbkrWsKey]], optional): The class to manage message queues. Defaults to QueueController[IbkrWsKey].
             unsolicited_channels_to_be_queued (List[IbkrWsKey], optional): List of unsolicited channels to be queued. Defaults to None.
+            start (bool, optional): Flag to start the client immediately after initialization. Defaults to False.
 
 
             Inherited parameters from WsClient:
 
             timeout (float, optional): Timeout for waiting on operations like connection and shutdown. Defaults to _DEFAULT_TIMEOUT.
             restart_on_close (bool, optional): Flag to restart the connection if it closes unexpectedly. Defaults to True.
             restart_on_critical (bool, optional): Flag to restart the connection on critical errors. Defaults to True.
             ping_interval (int, optional): Interval in seconds for sending pings to keep the connection alive. Defaults to _DEFAULT_PING_INTERVAL.
             max_ping_interval (int, optional): Maximum interval in seconds to wait for a ping response. Defaults to _DEFAULT_MAX_PING_INTERVAL.
             max_connection_attempts (int, optional): Maximum number of attempts for connecting to the WebSocket. Defaults to 10.
             cacert (Union[str, bool], optional): Path to the CA certificate file for SSL verification, or False to disable SSL verification. Defaults to False.
             subscription_retries (int, optional): Number of retries for subscription requests. Defaults to 5.
             subscription_timeout (float, optional): Timeout for subscription requests. Defaults to 2.
         """
-        self._ibkr_client = ibkr_client
+
         self._account_id = account_id
         if url is None:
             url = f'wss://{host}:{port}{base_route}'
 
+        if ibkr_client is None:
+            ibkr_client = IbkrClient(account_id=account_id, host=host, port=port, cacert=cacert)
+
+        self._ibkr_client = ibkr_client
+
         self._queue_controller = QueueControllerClass()
         self._subscription_processor = SubscriptionProcessorClass()
 
         self._log_raw_messages = log_raw_messages
         self._unsolicited_channels_to_be_queued = unsolicited_channels_to_be_queued if unsolicited_channels_to_be_queued is not None else []
 
         super().__init__(
@@ -250,15 +260,19 @@
 
         self._operational_lock = TimeoutLock(60)
 
         self._queue_controller.register_queues(list(IbkrWsKey))
 
         self._logged_in = False
         self._last_heartbeat = 0
-        self.server_id_conid_pairs: Dict[IbkrWsKey, Dict[str, int]] = defaultdict(dict)
+        self._server_id_conid_pairs: Dict[IbkrWsKey, Dict[str, int]] = defaultdict(dict)
+        self._queue_accessors: Dict[IbkrWsKey, QueueAccessor] = {}
+
+        if start:
+            self.start()
 
     def _login(self):
         status = self._ibkr_client.tickle()
         session_id = status.data['session']
         payload = {'session': session_id}
         self.send_json(payload)
 
@@ -277,15 +291,15 @@
         result = {'conid': message['conid'], '_updated': message['_updated'], 'topic': message['topic']}
         for key, value in message.items():
             if key in ibkr_definitions.snapshot_by_id:
                 result[ibkr_definitions.snapshot_by_id[key]] = value
         return {message['conid']: result}
 
     def _preprocess_market_history_message(self, message: dict):
-        mh_server_id_conid_pairs = self.server_id_conid_pairs[IbkrWsKey.MARKET_HISTORY]
+        mh_server_id_conid_pairs = self._server_id_conid_pairs[IbkrWsKey.MARKET_HISTORY]
         if 'serverId' in message and message['serverId'] not in mh_server_id_conid_pairs:
             mh_server_id_conid_pairs[message['serverId']] = extract_conid(message)
 
         return message
 
     def _handle_subscribed_message(self, channel: str, message: dict):
         try:
@@ -339,15 +353,15 @@
     def _handle_notification(self, data):  # pragma: no cover
         self._handle_unsolicited_message(IbkrWsKey.NOTIFICATIONS, data)
         for notification in data:
             _LOGGER.info(f'{self}: IBKR notification: {notification}')
 
     def _handle_market_history_unsubscribe(self, data):
         server_id = data['message'].split('Unsubscribed ')[-1]
-        mh_server_id_conid_pairs = self.server_id_conid_pairs[IbkrWsKey.MARKET_HISTORY]
+        mh_server_id_conid_pairs = self._server_id_conid_pairs[IbkrWsKey.MARKET_HISTORY]
         if server_id in mh_server_id_conid_pairs:
             conid = mh_server_id_conid_pairs[server_id]
             _LOGGER.info(f'{self}: Received unsubscribing confirmation for server_id={server_id!r}/conid={conid!r}.')
             if conid is None:
                 _LOGGER.warning(f'{self}: Unknown conid={conid!r}. Cannot mark the subscription as unsubscribed.')
                 return
 
@@ -427,15 +441,15 @@
                 _LOGGER.error(f'{self}: Topic "{topic}" unrecognised. Message: {message}')
 
     def check_health(self) -> bool:
         """
         Checks the overall health of the IbkrWsClient and its WebSocket connection.
 
         Verifies the health of the WebSocket connection by checking ping responses and heartbeat messages
-        from Interactive Brokers. If the connection is found to be unhealthy, a hard reset is initiated.
+        from IBKR. If the connection is found to be unhealthy, a hard reset is initiated.
 
         Returns:
             bool: True if the WebSocket connection is healthy, False otherwise.
         """
         if self._wsa is None:
             return True
 
@@ -462,15 +476,15 @@
 
         Parameters:
             key (IbkrWsKey): The key representing the subscription type.
 
         Returns:
             Optional[Dict[str, int]: The server IDs associated with the given key, or None if no server IDs are available.
         """
-        return self.server_id_conid_pairs[key]
+        return self._server_id_conid_pairs[key]
 
     def new_queue_accessor(self, key: IbkrWsKey) -> QueueAccessor[IbkrWsKey]:  # pragma: no cover
         """
         Creates a new queue accessor for a specified IbkrWsKey.
 
         Utilizes the internal queue controller to create an accessor for a queue associated with a specific
         IbkrWsKey. This accessor facilitates interaction with the queue for that particular type of subscription.
@@ -487,15 +501,15 @@
             self,
             channel: str,
             data: dict = None,
             needs_confirmation: bool = True,
             subscription_processor: SubscriptionProcessor = None,
     ) -> bool:  # pragma: no cover
         """
-        Subscribes to a specific channel in the Interactive Brokers WebSocket.
+        Subscribes to a specific channel in the IBKR WebSocket.
 
         Initiates a subscription to a given channel, optionally including additional data in the subscription
         request. The method delegates the subscription logic to the SubscriptionController.
 
         From docs: "To receive all orders for the current day the endpoint /iserver/account/orders can be used. It is advised to query all orders for the current day first before subscribing to live orders."
 
         Parameters:
@@ -510,7 +524,20 @@
         """
         if channel == 'or':
             if not self._ibkr_client.check_health():
                 return False
             self._ibkr_client.live_orders(force=True)
             self._ibkr_client.live_orders()
         return super().subscribe(channel, data, needs_confirmation, subscription_processor)
+
+    def _queue_accessor(self, ibkr_ws_key: IbkrWsKey):  # pragma: no cover
+        try:
+            return self._queue_accessors[ibkr_ws_key]
+        except KeyError:
+            self._queue_accessors[ibkr_ws_key] = self.new_queue_accessor(ibkr_ws_key)
+            return self._queue_accessors[ibkr_ws_key]
+
+    def get(self, ibkr_ws_key: IbkrWsKey, block: bool = False, timeout=None):  # pragma: no cover
+        return self._queue_accessor(ibkr_ws_key).get(block=block, timeout=timeout)
+
+    def empty(self, ibkr_ws_key: IbkrWsKey):  # pragma: no cover
+        return self._queue_accessor(ibkr_ws_key).empty()
```

### Comparing `ibind-0.0.3/ibind/support/logs.py` & `ibind-0.0.4/ibind/support/logs.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/support/py_utils.py` & `ibind-0.0.4/ibind/support/py_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind/var.py` & `ibind-0.0.4/ibind/var.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/ibind.egg-info/SOURCES.txt` & `ibind-0.0.4/ibind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/pyproject.toml` & `ibind-0.0.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [project]
 name = "ibind"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Voy Zan", email="voy1982@yahoo.co.uk" },
 ]
 description = "IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API."
 readme = "README.md"
 requires-python = ">=3.8"
+license={ file = "LICENSE" }
 dependencies = [
     "requests==2.31.*",
     "websocket-client==1.7.*"
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
+    "Intended Audience :: Financial and Insurance Industry",
+    "Topic :: Office/Business :: Financial :: Investment",
 ]
 keywords=['interactive brokers', 'rest api', 'python api', 'ibkr python api', 'ibkr web api', 'ib api', 'ibkr api', 'algo trading', 'algorithmic trading', 'quant', 'trading']
 
 [project.urls]
 Homepage = "https://github.com/Voyz/ibind"
 
 [build-system]
 requires = [
-    "setuptools",
-    "requests==2.31.*",
-    "websocket-client==1.7.*"
+    "setuptools"
 ]
```

### Comparing `ibind-0.0.3/test/integration/base/test_rest_client_i.py` & `ibind-0.0.4/test/integration/base/test_rest_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/test/integration/base/test_websocket_client_i.py` & `ibind-0.0.4/test/integration/base/test_websocket_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/test/integration/base/websocketapp_mock.py` & `ibind-0.0.4/test/integration/base/websocketapp_mock.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/test/integration/client/ibkr_responses.py` & `ibind-0.0.4/test/integration/client/ibkr_responses.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/test/integration/client/test_ibkr_client_i.py` & `ibind-0.0.4/test/integration/client/test_ibkr_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/test/integration/client/test_ibkr_utils_i.py` & `ibind-0.0.4/test/integration/client/test_ibkr_utils_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/test/integration/client/test_ibkr_ws_client_i.py` & `ibind-0.0.4/test/integration/client/test_ibkr_ws_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/test/test_utils.py` & `ibind-0.0.4/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.3/test/unit/support/test_py_utils_u.py` & `ibind-0.0.4/test/unit/support/test_py_utils_u.py`

 * *Files identical despite different names*


# Comparing `tmp/binance-connector-3.6.0.tar.gz` & `tmp/binance-connector-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-connector-3.6.0.tar", last modified: Thu Mar  7 11:59:09 2024, max compression
+gzip compressed data, was "binance-connector-3.7.0.tar", last modified: Fri May  3 08:18:50 2024, max compression
```

## Comparing `binance-connector-3.6.0.tar` & `binance-connector-3.7.0.tar`

### file list

```diff
@@ -1,64 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:08.997600 binance-connector-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-07 11:59:06.000000 binance-connector-3.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-07 11:59:06.000000 binance-connector-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-03-07 11:59:08.997600 binance-connector-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-03-07 11:59:06.000000 binance-connector-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:08.989601 binance-connector-3.6.0/binance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:08.989601 binance-connector-3.6.0/binance/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/lib/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/lib/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:08.993600 binance-connector-3.6.0/binance/spot/
--rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_auto_invest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_blvt.py
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_bswap.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_c2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19075 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_crypto_loan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_data_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_fiat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_gift_card.py
--rw-r--r--   0 runner    (1001) docker     (127)    30632 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_margin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_market.py
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_nft.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_pay.py
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_portfolio_margin.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_rebate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17285 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_simple_earn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_staking.py
--rw-r--r--   0 runner    (1001) docker     (127)    37864 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_sub_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)    17882 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/spot/_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:08.993600 binance-connector-3.6.0/binance/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/websocket/binance_socket_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:08.993600 binance-connector-3.6.0/binance/websocket/spot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/websocket/spot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:08.993600 binance-connector-3.6.0/binance/websocket/spot/websocket_api/
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/websocket/spot/websocket_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/websocket/spot/websocket_api/_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    24597 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/websocket/spot/websocket_api/_market.py
--rw-r--r--   0 runner    (1001) docker     (127)    38486 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/websocket/spot/websocket_api/_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/websocket/spot/websocket_api/_user_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/websocket/spot/websocket_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-03-07 11:59:06.000000 binance-connector-3.6.0/binance/websocket/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:08.997600 binance-connector-3.6.0/binance_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-03-07 11:59:08.000000 binance-connector-3.6.0/binance_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-07 11:59:08.000000 binance-connector-3.6.0/binance_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 11:59:08.000000 binance-connector-3.6.0/binance_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-07 11:59:08.000000 binance-connector-3.6.0/binance_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-07 11:59:08.000000 binance-connector-3.6.0/binance_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:08.997600 binance-connector-3.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:06.000000 binance-connector-3.6.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:59:08.997600 binance-connector-3.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-07 11:59:06.000000 binance-connector-3.6.0/requirements/common.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-07 11:59:08.997600 binance-connector-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-07 11:59:06.000000 binance-connector-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:50.455920 binance-connector-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 08:18:47.000000 binance-connector-3.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 08:18:47.000000 binance-connector-3.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-05-03 08:18:50.455920 binance-connector-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-05-03 08:18:47.000000 binance-connector-3.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:50.447920 binance-connector-3.7.0/binance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:50.447920 binance-connector-3.7.0/binance/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/lib/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/lib/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:50.451920 binance-connector-3.7.0/binance/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_auto_invest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_blvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_c2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_crypto_loan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_fiat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_gift_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_margin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_market.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_nft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_pay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_portfolio_margin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_rebate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17285 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_simple_earn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37864 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_sub_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/spot/_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:50.451920 binance-connector-3.7.0/binance/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/websocket/binance_socket_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:50.451920 binance-connector-3.7.0/binance/websocket/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/websocket/spot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:50.455920 binance-connector-3.7.0/binance/websocket/spot/websocket_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/websocket/spot/websocket_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/websocket/spot/websocket_api/_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24650 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/websocket/spot/websocket_api/_market.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38486 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/websocket/spot/websocket_api/_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/websocket/spot/websocket_api/_user_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/websocket/spot/websocket_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-03 08:18:47.000000 binance-connector-3.7.0/binance/websocket/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:50.455920 binance-connector-3.7.0/binance_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-05-03 08:18:50.000000 binance-connector-3.7.0/binance_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-03 08:18:50.000000 binance-connector-3.7.0/binance_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 08:18:50.000000 binance-connector-3.7.0/binance_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 08:18:50.000000 binance-connector-3.7.0/binance_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 08:18:50.000000 binance-connector-3.7.0/binance_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:50.455920 binance-connector-3.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:47.000000 binance-connector-3.7.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:18:50.455920 binance-connector-3.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 08:18:47.000000 binance-connector-3.7.0/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-03 08:18:50.455920 binance-connector-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-03 08:18:47.000000 binance-connector-3.7.0/setup.py
```

### Comparing `binance-connector-3.6.0/LICENSE.md` & `binance-connector-3.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/PKG-INFO` & `binance-connector-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-connector
-Version: 3.6.0
+Version: 3.7.0
 Summary: This is a lightweight library that works as a connector to Binance public API.
 Home-page: https://github.com/binance/binance-connector-python
 License: MIT
 Keywords: Binance,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binance-connector-3.6.0/README.md` & `binance-connector-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/api.py` & `binance-connector-3.7.0/binance/api.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/error.py` & `binance-connector-3.7.0/binance/error.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/lib/authentication.py` & `binance-connector-3.7.0/binance/lib/authentication.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/lib/enums.py` & `binance-connector-3.7.0/binance/lib/enums.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/lib/utils.py` & `binance-connector-3.7.0/binance/lib/utils.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/__init__.py` & `binance-connector-3.7.0/binance/spot/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     from binance.spot._market import trades
     from binance.spot._market import historical_trades
     from binance.spot._market import agg_trades
     from binance.spot._market import klines
     from binance.spot._market import ui_klines
     from binance.spot._market import avg_price
     from binance.spot._market import ticker_24hr
+    from binance.spot._market import trading_day_ticker
     from binance.spot._market import ticker_price
     from binance.spot._market import book_ticker
     from binance.spot._market import rolling_window_ticker
 
     # ACCOUNT (including orders and trades)
     from binance.spot._trade import new_order_test
     from binance.spot._trade import new_order
@@ -37,14 +38,16 @@
     from binance.spot._trade import get_oco_order
     from binance.spot._trade import get_oco_orders
     from binance.spot._trade import get_oco_open_orders
     from binance.spot._trade import account
     from binance.spot._trade import my_trades
     from binance.spot._trade import get_order_rate_limit
     from binance.spot._trade import query_prevented_matches
+    from binance.spot._trade import query_allocations
+    from binance.spot._trade import query_commission_rates
 
     # STREAMS
     from binance.spot._data_stream import new_listen_key
     from binance.spot._data_stream import renew_listen_key
     from binance.spot._data_stream import close_listen_key
     from binance.spot._data_stream import new_margin_listen_key
     from binance.spot._data_stream import renew_margin_listen_key
@@ -91,23 +94,17 @@
     from binance.spot._margin import margin_order_usage
     from binance.spot._margin import summary_of_margin_account
     from binance.spot._margin import cross_margin_collateral_ratio
     from binance.spot._margin import get_small_liability_exchange_coin_list
     from binance.spot._margin import get_small_liability_exchange_history
     from binance.spot._margin import get_a_future_hourly_interest_rate
     from binance.spot._margin import adjust_cross_margin_max_leverage
-
-    # Staking
-    from binance.spot._staking import staking_product_list
-    from binance.spot._staking import staking_purchase_product
-    from binance.spot._staking import staking_redeem_product
-    from binance.spot._staking import staking_product_position
-    from binance.spot._staking import staking_history
-    from binance.spot._staking import staking_set_auto_staking
-    from binance.spot._staking import staking_product_quota
+    from binance.spot._margin import margin_available_inventory
+    from binance.spot._margin import margin_manual_liquidation
+    from binance.spot._margin import liability_coin_leverage_bracket
 
     # WALLET
     from binance.spot._wallet import system_status
     from binance.spot._wallet import coin_info
     from binance.spot._wallet import account_snapshot
     from binance.spot._wallet import disable_fast_withdraw
     from binance.spot._wallet import enable_fast_withdraw
@@ -126,19 +123,21 @@
     from binance.spot._wallet import trade_fee
     from binance.spot._wallet import funding_wallet
     from binance.spot._wallet import user_asset
     from binance.spot._wallet import api_key_permissions
     from binance.spot._wallet import bnb_convertible_assets
     from binance.spot._wallet import convertible_coins
     from binance.spot._wallet import toggle_auto_convertion
+    from binance.spot._wallet import list_deposit_address
     from binance.spot._wallet import cloud_mining_trans_history
     from binance.spot._wallet import convert_transfer
     from binance.spot._wallet import convert_history
     from binance.spot._wallet import one_click_arrival_deposit_apply
     from binance.spot._wallet import balance
+    from binance.spot._wallet import delist_schedule_symbols
 
     # MINING
     from binance.spot._mining import mining_algo_list
     from binance.spot._mining import mining_coin_list
     from binance.spot._mining import mining_worker
     from binance.spot._mining import mining_worker_list
     from binance.spot._mining import mining_earnings_list
@@ -208,30 +207,14 @@
     from binance.spot._blvt import blvt_info
     from binance.spot._blvt import subscribe_blvt
     from binance.spot._blvt import subscription_record
     from binance.spot._blvt import redeem_blvt
     from binance.spot._blvt import redemption_record
     from binance.spot._blvt import user_limit_info
 
-    # BSwap
-    from binance.spot._bswap import bswap_pools
-    from binance.spot._bswap import bswap_liquidity
-    from binance.spot._bswap import bswap_liquidity_add
-    from binance.spot._bswap import bswap_liquidity_remove
-    from binance.spot._bswap import bswap_liquidity_operation_record
-    from binance.spot._bswap import bswap_request_quote
-    from binance.spot._bswap import bswap_swap
-    from binance.spot._bswap import bswap_swap_history
-    from binance.spot._bswap import bswap_pool_configure
-    from binance.spot._bswap import bswap_add_liquidity_preview
-    from binance.spot._bswap import bswap_remove_liquidity_preview
-    from binance.spot._bswap import bswap_unclaimed_rewards
-    from binance.spot._bswap import bswap_claim_rewards
-    from binance.spot._bswap import bswap_claimed_rewards
-
     # FIAT
     from binance.spot._fiat import fiat_order_history
     from binance.spot._fiat import fiat_payment_history
 
     # C2C
     from binance.spot._c2c import c2c_trade_history
 
@@ -248,33 +231,27 @@
     from binance.spot._crypto_loan import loan_vip_repay
     from binance.spot._crypto_loan import loan_vip_repay_history
     from binance.spot._crypto_loan import loan_vip_collateral_account
     from binance.spot._crypto_loan import loan_loanable_data
     from binance.spot._crypto_loan import loan_collateral_data
     from binance.spot._crypto_loan import loan_collateral_rate
     from binance.spot._crypto_loan import loan_customize_margin_call
-    from binance.spot._crypto_loan import flexible_loan_adjust_ltv
-    from binance.spot._crypto_loan import flexible_loan_assets_data
-    from binance.spot._crypto_loan import flexible_loan_borrow_history
-    from binance.spot._crypto_loan import flexible_loan_borrow
-    from binance.spot._crypto_loan import flexible_loan_collateral_assets_data
-    from binance.spot._crypto_loan import flexible_loan_ltv_adjustment_history
-    from binance.spot._crypto_loan import flexible_loan_ongoing_orders
-    from binance.spot._crypto_loan import flexible_loan_repay
-    from binance.spot._crypto_loan import flexible_loan_repayment_history
 
     # PAY
     from binance.spot._pay import pay_history
 
     # CONVERT
     from binance.spot._convert import list_all_convert_pairs
     from binance.spot._convert import query_order_quantity_precision_per_asset
     from binance.spot._convert import send_quote_request
     from binance.spot._convert import accept_quote
     from binance.spot._convert import order_status
+    from binance.spot._convert import place_limit_order
+    from binance.spot._convert import cancel_limit_order
+    from binance.spot._convert import query_limit_open_order
     from binance.spot._convert import get_convert_trade_history
 
     # REBATE
     from binance.spot._rebate import rebate_spot_history
 
     # NFT
     from binance.spot._nft import nft_transaction_history
```

### Comparing `binance-connector-3.6.0/binance/spot/_auto_invest.py` & `binance-connector-3.7.0/binance/spot/_auto_invest.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/_blvt.py` & `binance-connector-3.7.0/binance/spot/_blvt.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/_bswap.py` & `binance-connector-3.7.0/binance/spot/_crypto_loan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,333 +1,350 @@
-from binance.lib.utils import check_required_parameters
+from binance.lib.utils import check_required_parameters, check_required_parameter
 
 
-def bswap_pools(self):
-    """List All Swap Pools (MARKET_DATA)
-    Get metadata about all swap pools.
+def loan_history(self, asset: str, **kwargs):
+    """Get Crypto Loans Income History (USER_DATA)
 
-    GET /sapi/v1/bswap/pools
+    GET /sapi/v1/loan/income
 
-    https://binance-docs.github.io/apidocs/spot/en/#list-all-swap-pools-market_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-crypto-loans-income-history-user_data
 
+    Args:
+      asset (str)
+    Keyword Args:
+      type (str, optional): All types will be returned by default.
+                            borrowIn, collateralSpent, repayAmount, collateralReturn (collateral return after repayment),
+                            addCollateral, removeCollateral, collateralReturnAfterLiquidation
+      startTime (int, optional)
+      endTime (int, optional)
+      limit (int, optional): default 20, max 100
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    return self.limit_request("GET", "/sapi/v1/bswap/pools", {})
+    check_required_parameter(asset, "asset")
 
+    payload = {"asset": asset, **kwargs}
+    return self.sign_request("GET", "/sapi/v1/loan/income", payload)
 
-def bswap_liquidity(self, **kwargs):
-    """Get liquidity information of a pool (USER_DATA)
-    Get liquidity information and user share of a pool
 
-    GET /sapi/v1/bswap/liquidity
+def loan_borrow(self, loanCoin: str, collateralCoin: str, loanTerm: int, **kwargs):
+    """Crypto Loan Borrow (TRADE)
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-liquidity-information-of-a-pool-user_data
+    POST /sapi/v1/loan/borrow
 
-    Keyword Args:
-        poolId (int, optional)
-        recvWindow (int, optional): The value cannot be greater than 60000
+    https://binance-docs.github.io/apidocs/spot/en/#borrow-crypto-loan-borrow-trade
 
+    Args:
+      loanCoin (str)
+      collateralCoin (str)
+      loanTerm (int): 7/14/30/90/180 days
+    Keyword Args:
+      loanAmount (float, optional): Mandatory when collateralAmount is empty
+      collateralAmount (float, optional): Mandatory when loanAmount is empty
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
-    return self.sign_request("GET", "/sapi/v1/bswap/liquidity", kwargs)
+
+    check_required_parameters(
+        [
+            [loanCoin, "loanCoin"],
+            [collateralCoin, "collateralCoin"],
+            [loanTerm, "loanTerm"],
+        ]
+    )
+
+    payload = {
+        "loanCoin": loanCoin,
+        "collateralCoin": collateralCoin,
+        "loanTerm": loanTerm,
+        **kwargs,
+    }
+    return self.sign_request("POST", "/sapi/v1/loan/borrow", payload)
 
 
-def bswap_liquidity_add(self, poolId: int, asset: str, quantity: float, **kwargs):
-    """Add Liquidity (TRADE)
-    Add liquidity to a pool.
+def loan_borrow_history(self, **kwargs):
+    """Get Loan Borrow History (USER_DATA)
 
-    POST /sapi/v1/bswap/liquidityAdd
+    GET /sapi/v1/loan/borrow/history
 
-    https://binance-docs.github.io/apidocs/spot/en/#add-liquidity-trade
+    https://binance-docs.github.io/apidocs/spot/en/#borrow-get-loan-borrow-history-user_data
 
-    Args:
-        poolId (int)
-        asset (str)
-        quantity (float)
     Keyword Args:
-        type (str, optional): "Single" to add a single token; "Combination" to add dual tokens. Default "Single"
-        recvWindow (int, optional): The value cannot be greater than 60000
+      orderId (int, optional): orderId in POST /sapi/v1/loan/borrow
+      loanCoin (str, optional)
+      collateralCoin (str, optional)
+      startTime (int, optional)
+      endTime (int, optional)
+      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000.
+      limit (int, optional): Default: 10; max: 100
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
-    check_required_parameters(
-        [[poolId, "poolId"], [asset, "asset"], [quantity, "quantity"]]
-    )
-    payload = {"poolId": poolId, "asset": asset, "quantity": quantity, **kwargs}
 
-    return self.sign_request("POST", "/sapi/v1/bswap/liquidityAdd", payload)
+    return self.sign_request("GET", "/sapi/v1/loan/borrow/history", kwargs)
 
 
-def bswap_liquidity_remove(
-    self, poolId: str, type: str, asset: list, shareAmount, **kwargs
-):
-    """Remove Liquidity (TRADE)
-    Remove liquidity from a pool, type include SINGLE and COMBINATION, asset is mandatory for single asset removal
+def loan_ongoing_orders(self, **kwargs):
+    """Get Loan Ongoing Orders (USER_DATA)
+
+    GET /sapi/v1/loan/ongoing/orders
+
+    https://binance-docs.github.io/apidocs/spot/en/#borrow-get-loan-ongoing-orders-user_data
+
+    Keyword Args:
+      orderId (int, optional): orderId in POST /sapi/v1/loan/borrow
+      loanCoin (str, optional)
+      collateralCoin (str, optional)
+      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000
+      limit (int, optional): Default: 10; max: 100
+      recvWindow (int, optional): The value cannot be greater than 60000
+    """
 
-    POST /sapi/v1/bswap/liquidityRemove
+    return self.sign_request("GET", "/sapi/v1/loan/ongoing/orders", kwargs)
 
-    https://binance-docs.github.io/apidocs/spot/en/#remove-liquidity-trade
+
+def loan_repay(self, orderId: int, amount: float, **kwargs):
+    """Crypto Loan Repay (TRADE)
+
+    POST /sapi/v1/loan/repay
+
+    https://binance-docs.github.io/apidocs/spot/en/#repay-crypto-loan-repay-trade
 
     Args:
-        poolId (int)
-        type (str): SINGLE for single asset removal, COMBINATION for combination of all coins removal
-        asset (str)
-        shareAmount (float): Mandatory for liquidity removal
+      orderId (int)
+      amount (float)
     Keyword Args:
-        recvWindow (int, optional): The value cannot be greater than 60000
+      type (int, optional): Default: 1. 1 for "repay with borrowed coin"; 2 for "repay with collateral"
+      collateralReturn (boolean, optional): Default: TRUE. TRUE: Return extra collateral to spot account; FALSE: Keep extra collateral in the order.
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
-    check_required_parameters(
-        [
-            [poolId, "poolId"],
-            [type, "type"],
-            [asset, "asset"],
-            [shareAmount, "shareAmount"],
-        ]
-    )
-    payload = {
-        "poolId": poolId,
-        "type": type,
-        "asset": ",".join(asset),
-        "shareAmount": shareAmount,
-        **kwargs,
-    }
 
-    return self.sign_request("POST", "/sapi/v1/bswap/liquidityRemove", payload)
+    check_required_parameters([[orderId, "orderId"], [amount, "amount"]])
+
+    payload = {"orderId": orderId, "amount": amount, **kwargs}
+    return self.sign_request("POST", "/sapi/v1/loan/repay", payload)
 
 
-def bswap_liquidity_operation_record(self, **kwargs):
-    """Get Liquidity Operation Record (USER_DATA)
-    Get liquidity operation (add/remove) records.
+def loan_repay_history(self, **kwargs):
+    """Get Loan Repayment History (USER_DATA)
 
-    GET /sapi/v1/bswap/liquidityOps
+    GET /sapi/v1/loan/repay/history
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-liquidity-operation-record-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#repay-get-loan-repayment-history-user_data
 
     Keyword Args:
-        operationId (int, optional)
-        poolId (int, optional)
-        operation (str, optional): ADD or REMOVE
-        startTime (int, optional)
-        endTime (int, optional)
-        limit (int, optional): default 3, max 100
-        recvWindow (int, optional): The value cannot be greater than 60000
+      orderId (int, optional)
+      loanCoin (str, optional)
+      collateralCoin (str, optional)
+      startTime (int, optional)
+      endTime (int, optional)
+      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000.
+      limit (int, optional): Default: 10; max: 100
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
-    return self.sign_request("GET", "/sapi/v1/bswap/liquidityOps", kwargs)
 
+    return self.sign_request("GET", "/sapi/v1/loan/repay/history", kwargs)
 
-def bswap_request_quote(
-    self, quoteAsset: str, baseAsset: str, quoteQty: float, **kwargs
-):
-    """Request Quote (USER_DATA)
-    Request a quote for swap quote asset (selling asset) for base asset (buying asset), essentially price/exchange rates.
-    quoteQty is quantity of quote asset (to sell).
 
-    Please be noted the quote is for reference only, the actual price will change as the liquidity changes,
-    it's recommended to swap immediate after request a quote for slippage prevention.
+def loan_adjust_ltv(self, orderId: int, amount: float, direction: str, **kwargs):
+    """Crypto Loan Adjust LTV (TRADE)
 
-    GET /sapi/v1/bswap/quote
+    POST /sapi/v1/loan/adjust/ltv
 
-    https://binance-docs.github.io/apidocs/spot/en/#request-quote-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#adjust-ltv-crypto-loan-adjust-ltv-trade
 
     Args:
-        quoteAsset (str)
-        baseAsset (str)
-        quoteQty (float)
+      orderId (int)
+      amount (float)
+      direction (str): "ADDITIONAL", "REDUCED"
     Keyword Args:
-        recvWindow (int, optional): The value cannot be greater than 60000
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
 
     check_required_parameters(
-        [[quoteAsset, "quoteAsset"], [baseAsset, "baseAsset"], [quoteQty, "quoteQty"]]
+        [[orderId, "orderId"], [amount, "amount"], [direction, "direction"]]
     )
-    payload = {
-        "quoteAsset": quoteAsset,
-        "baseAsset": baseAsset,
-        "quoteQty": quoteQty,
-        **kwargs,
-    }
 
-    return self.sign_request("GET", "/sapi/v1/bswap/quote", payload)
+    payload = {"orderId": orderId, "amount": amount, "direction": direction, **kwargs}
+    return self.sign_request("POST", "/sapi/v1/loan/adjust/ltv", payload)
 
 
-def bswap_swap(self, quoteAsset: str, baseAsset: str, quoteQty: float, **kwargs):
-    """Swap (TRADE)
-    Swap quoteAsset for baseAsset.
+def loan_adjust_ltv_history(self, **kwargs):
+    """Get Loan LTV Adjustment History (USER_DATA)
 
-    POST /sapi/v1/bswap/swap
+    GET /sapi/v1/loan/ltv/adjustment/history
 
-    https://binance-docs.github.io/apidocs/spot/en/#swap-trade
+    https://binance-docs.github.io/apidocs/spot/en/#adjust-ltv-get-loan-ltv-adjustment-history-user_data
 
-    Args:
-        baseAsset (str)
-        quoteAsset (str)
-        quoteQty (float)
     Keyword Args:
-        recvWindow (int, optional): The value cannot be greater than 60000
+      orderId (int, optional)
+      loanCoin (str, optional)
+      collateralCoin (str, optional)
+      startTime (int, optional)
+      endTime (int, optional)
+      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000
+      limit (int, optional): Default: 10; max: 100
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
-    check_required_parameters(
-        [[quoteAsset, "quoteAsset"], [baseAsset, "baseAsset"], [quoteQty, "quoteQty"]]
-    )
-    payload = {
-        "quoteAsset": quoteAsset,
-        "baseAsset": baseAsset,
-        "quoteQty": quoteQty,
-        **kwargs,
-    }
-    return self.sign_request("POST", "/sapi/v1/bswap/swap", payload)
+
+    return self.sign_request("GET", "/sapi/v1/loan/ltv/adjustment/history", kwargs)
 
 
-def bswap_swap_history(self, **kwargs):
-    """Get Swap History (USER_DATA)
-    Get swap history.
+def loan_vip_ongoing_orders(self, **kwargs):
+    """Get VIP Loan Ongoing Orders (USER_DATA)
 
-    GET /sapi/v1/bswap/swap
+    GET /sapi/v1/loan/vip/ongoing/orders
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-swap-history-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-vip-loan-ongoing-orders-user_data
 
     Keyword Args:
-        swapId (int, optional)
-        startTime (int, optional)
-        endTime (int, optional)
-        status (int, optional)
-        baseAsset (str, optional)
-        quoteAsset (str, optional)
-        limit (int, optional)
-        recvWindow (int, optional): The value cannot be greater than 60000
+      orderId (int, optional)
+      collateralAccountId (int, optional)
+      loanCoin (str, optional)
+      collateralCoin (str, optional)
+      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000
+      limit (int, optional): Default: 10; max: 100
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
-    return self.sign_request("GET", "/sapi/v1/bswap/swap", kwargs)
 
+    return self.sign_request("GET", "/sapi/v1/loan/vip/ongoing/orders", kwargs)
 
-def bswap_pool_configure(self, **kwargs):
-    """Get Pool Configure (USER_DATA)
 
-    GET /sapi/v1/bswap/poolConfigure
+def loan_vip_repay(self, orderId: int, amount: float, **kwargs):
+    """VIP Loan Repay (TRADE)
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-pool-configure-user_data
+    POST /sapi/v1/loan/vip/repay
 
+    https://binance-docs.github.io/apidocs/spot/en/#vip-loan-repay-trade
+
+    Args:
+      orderId (int)
+      amount (float)
     Keyword Args:
-        poolId (int, optional)
-        recvWindow (int, optional): The value cannot be greater than 60000
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
-    return self.sign_request("GET", "/sapi/v1/bswap/poolConfigure", kwargs)
 
+    check_required_parameters([[orderId, "orderId"], [amount, "amount"]])
 
-def bswap_add_liquidity_preview(
-    self, poolId: int, type: str, quoteAsset: str, quoteQty: float, **kwargs
-):
-    """Add Liquidity Preview (USER_DATA)
-    Calculate expected share amount for adding liquidity in single or dual token.
+    payload = {"orderId": orderId, "amount": amount, **kwargs}
+    return self.sign_request("POST", "/sapi/v1/loan/vip/repay", payload)
 
-    GET /sapi/v1/bswap/addLiquidityPreview
 
-    https://binance-docs.github.io/apidocs/spot/en/#add-liquidity-preview-user_data
+def loan_vip_repay_history(self, **kwargs):
+    """Get VIP Loan Repayment History (USER_DATA)
+
+    GET /sapi/v1/loan/vip/repay/history
+
+    https://binance-docs.github.io/apidocs/spot/en/#get-vip-loan-repayment-history-user_data
 
-    Args:
-        poolId (int)
-        type (str): "SINGLE" for adding a single token;"COMBINATION" for adding dual tokens
-        quoteAsset (str)
-        quoteQty (float)
     Keyword Args:
-        recvWindow (int, optional): The value cannot be greater than 60000
+      orderId (int, optional)
+      loanCoin (str, optional)
+      startTime (int, optional)
+      endTime (int, optional)
+      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000
+      limit (int, optional): Default: 10; max: 100
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
-    check_required_parameters(
-        [
-            [poolId, "poolId"],
-            [type, "type"],
-            [quoteAsset, "quoteAsset"],
-            [quoteQty, "quoteQty"],
-        ]
-    )
-    payload = {
-        "poolId": poolId,
-        "type": type,
-        "quoteAsset": quoteAsset,
-        "quoteQty": quoteQty,
-        **kwargs,
-    }
-    return self.sign_request("GET", "/sapi/v1/bswap/addLiquidityPreview", payload)
 
+    return self.sign_request("GET", "/sapi/v1/loan/vip/repay/history", kwargs)
 
-def bswap_remove_liquidity_preview(
-    self, poolId: int, type: str, quoteAsset: str, shareAmount: float, **kwargs
-):
-    """Remove Liquidity Preview (USER_DATA)
-    Calculate the expected asset amount of single token redemption or dual token redemption.
 
-    GET /sapi/v1/bswap/removeLiquidityPreview
+def loan_vip_collateral_account(self, **kwargs):
+    """Check Locked Value of VIP Collateral Account (USER_DATA)
 
-    https://binance-docs.github.io/apidocs/spot/en/#remove-liquidity-preview-user_data
+    GET /sapi/v1/loan/vip/collateral/account
+
+    https://binance-docs.github.io/apidocs/spot/en/#check-locked-value-of-vip-collateral-account-user_data
 
-    Args:
-        poolId (int)
-        type (str): Type is "SINGLE", remove and obtain a single token;Type is "COMBINATION", remove and obtain dual token
-        quoteAsset (str)
-        shareAmount (float)
     Keyword Args:
-        recvWindow (int, optional): The value cannot be greater than 60000
+      orderId (int, optional)
+      collateralAccountId (int, optional)
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
-    check_required_parameters(
-        [
-            [poolId, "poolId"],
-            [type, "type"],
-            [quoteAsset, "quoteAsset"],
-            [shareAmount, "shareAmount"],
-        ]
-    )
-    payload = {
-        "poolId": poolId,
-        "type": type,
-        "quoteAsset": quoteAsset,
-        "shareAmount": shareAmount,
-        **kwargs,
-    }
-    return self.sign_request("GET", "/sapi/v1/bswap/removeLiquidityPreview", payload)
+
+    return self.sign_request("GET", "/sapi/v1/loan/vip/collateral/account", kwargs)
 
 
-def bswap_unclaimed_rewards(self, **kwargs):
-    """Get Unclaimed Rewards Record (USER_DATA)
-    Get unclaimed rewards record.
+def loan_loanable_data(self, **kwargs):
+    """Get Loanable Assets Data (USER_DATA)
 
-    GET /sapi/v1/bswap/unclaimedRewards
+    GET /sapi/v1/loan/loanable/data
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-unclaimed-rewards-record-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-loanable-assets-data-user_data
 
     Keyword Args:
-        type (int, optional): 0: Swap rewards,1:Liquidity rewards, default to 0
-        recvWindow (int, optional): The value cannot be greater than 60000
+      loanCoin (str, optional)
+      vipLevel (int, optional)
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    return self.sign_request("GET", "/sapi/v1/bswap/unclaimedRewards", kwargs)
+    return self.sign_request("GET", "/sapi/v1/loan/loanable/data", kwargs)
+
 
+def loan_collateral_data(self, **kwargs):
+    """Get Collateral Assets Data (USER_DATA)
 
-def bswap_claim_rewards(self, **kwargs):
-    """Claim rewards (TRADE)
-    Claim swap rewards or liquidity rewards
+    GET /sapi/v1/loan/collateral/data
+
+    https://binance-docs.github.io/apidocs/spot/en/#get-collateral-assets-data-user_data
+
+    Keyword Args:
+      collateralCoin (str, optional)
+      vipLevel (int, optional)
+      recvWindow (int, optional): The value cannot be greater than 60000
+    """
+
+    return self.sign_request("GET", "/sapi/v1/loan/collateral/data", kwargs)
+
+
+def loan_collateral_rate(
+    self, loanCoin: str, collateralCoin: str, repayAmount: float, **kwargs
+):
+    """Check Collateral Repay Rate (USER_DATA)
 
-    POST /sapi/v1/bswap/claimRewards
+    GET /sapi/v1/loan/repay/collateral/rate
 
-    https://binance-docs.github.io/apidocs/spot/en/#claim-rewards-trade
+    https://binance-docs.github.io/apidocs/spot/en/#check-collateral-repay-rate-user_data
 
+    Args:
+      loanCoin (str)
+      collateralCoin (str)
+      repayAmount (float)
     Keyword Args:
-        type (int, optional): 0: Swap rewards,1:Liquidity rewards, default to 0
-        recvWindow (int, optional): The value cannot be greater than 60000
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    return self.sign_request("POST", "/sapi/v1/bswap/claimRewards", kwargs)
+    check_required_parameters(
+        [
+            [loanCoin, "loanCoin"],
+            [collateralCoin, "collateralCoin"],
+            [repayAmount, "repayAmount"],
+        ]
+    )
+
+    payload = {
+        "loanCoin": loanCoin,
+        "collateralCoin": collateralCoin,
+        "repayAmount": repayAmount,
+        **kwargs,
+    }
+    return self.sign_request("GET", "/sapi/v1/loan/repay/collateral/rate", payload)
 
 
-def bswap_claimed_rewards(self, **kwargs):
-    """Get Claimed History (USER_DATA)
-    Get history of claimed rewards.
+def loan_customize_margin_call(self, marginCall: float, **kwargs):
+    """Customize Margin Call (USER_DATA)
 
-    GET /sapi/v1/bswap/claimedHistory
+    POST /sapi/v1/loan/customize/margin_call
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-claimed-history-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#crypto-loan-customize-margin-call-trade
 
+    Args:
+      marginCall (float)
     Keyword Args:
-        poolId (int, optional)
-        assetRewards (str, optional)
-        type (int, optional): 0: Swap rewards,1:Liquidity rewards, default to 0
-        startTime (int, optional)
-        endTime (int, optional)
-        limit (int, optional): default 3, max 100
-        recvWindow (int, optional): The value cannot be greater than 60000
+      orderId (int, optional)
+      collateralCoin (str, optional)
+      recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    return self.sign_request("GET", "/sapi/v1/bswap/claimedHistory", kwargs)
+    check_required_parameter(marginCall, "marginCall")
+
+    payload = {"marginCall": marginCall, **kwargs}
+    return self.sign_request("POST", "/sapi/v1/loan/customize/margin_call", payload)
```

### Comparing `binance-connector-3.6.0/binance/spot/_c2c.py` & `binance-connector-3.7.0/binance/spot/_c2c.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/_crypto_loan.py` & `binance-connector-3.7.0/binance/spot/_simple_earn.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,596 +1,530 @@
-from binance.lib.utils import check_required_parameters, check_required_parameter
+from binance.lib.utils import (
+    check_required_parameter,
+)
+from binance.lib.utils import check_required_parameters
 
 
-def loan_history(self, asset: str, **kwargs):
-    """Get Crypto Loans Income History (USER_DATA)
+def get_simple_earn_flexible_product_list(self, **kwargs):
+    """Get Simple Earn Flexible Product List (USER_DATA)
 
-    GET /sapi/v1/loan/income
+    Get available Simple Earn flexible product list
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-crypto-loans-income-history-user_data
+    Weight(IP): 150
+
+    GET /sapi/v1/simple-earn/flexible/list
+
+    https://binance-docs.github.io/apidocs/spot/en/#get-simple-earn-flexible-product-list-user_data
 
-    Args:
-      asset (str)
     Keyword Args:
-      type (str, optional): All types will be returned by default.
-                            borrowIn, collateralSpent, repayAmount, collateralReturn (collateral return after repayment),
-                            addCollateral, removeCollateral, collateralReturnAfterLiquidation
-      startTime (int, optional)
-      endTime (int, optional)
-      limit (int, optional): default 20, max 100
-      recvWindow (int, optional): The value cannot be greater than 60000
+        asset (str, optional)
+        current (int, optional): Current querying page. Start from 1. Default:1
+        size (int, optional): Default:10 Max:100
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    check_required_parameter(asset, "asset")
+    url_path = "/sapi/v1/simple-earn/flexible/list"
+    return self.sign_request("GET", url_path, {**kwargs})
 
-    payload = {"asset": asset, **kwargs}
-    return self.sign_request("GET", "/sapi/v1/loan/income", payload)
 
+def get_simple_earn_locked_product_list(self, **kwargs):
+    """Get Simple Earn Locked Product List (USER_DATA)
 
-def loan_borrow(self, loanCoin: str, collateralCoin: str, loanTerm: int, **kwargs):
-    """Crypto Loan Borrow (TRADE)
+    Weight(IP): 150
 
-    POST /sapi/v1/loan/borrow
+    GET /sapi/v1/simple-earn/locked/list
 
-    https://binance-docs.github.io/apidocs/spot/en/#borrow-crypto-loan-borrow-trade
+    https://binance-docs.github.io/apidocs/spot/en/#get-simple-earn-locked-product-list-user_data
 
-    Args:
-      loanCoin (str)
-      collateralCoin (str)
-      loanTerm (int): 7/14/30/90/180 days
     Keyword Args:
-      loanAmount (float, optional): Mandatory when collateralAmount is empty
-      collateralAmount (float, optional): Mandatory when loanAmount is empty
-      recvWindow (int, optional): The value cannot be greater than 60000
+        asset (str, optional)
+        current (int, optional): Current querying page. Start from 1. Default:1
+        size (int, optional): Default:10 Max:100
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    check_required_parameters(
-        [
-            [loanCoin, "loanCoin"],
-            [collateralCoin, "collateralCoin"],
-            [loanTerm, "loanTerm"],
-        ]
-    )
+    url_path = "/sapi/v1/simple-earn/locked/list"
+    return self.sign_request("GET", url_path, {**kwargs})
 
-    payload = {
-        "loanCoin": loanCoin,
-        "collateralCoin": collateralCoin,
-        "loanTerm": loanTerm,
-        **kwargs,
-    }
-    return self.sign_request("POST", "/sapi/v1/loan/borrow", payload)
 
+def subscribe_flexible_product(self, productId: str, amount: float, **kwargs):
+    """Subscribe Flexible Product (TRADE)
 
-def loan_borrow_history(self, **kwargs):
-    """Get Loan Borrow History (USER_DATA)
+    Weight(IP): 1
 
-    GET /sapi/v1/loan/borrow/history
+    Rate Limit: 1/3s per account
 
-    https://binance-docs.github.io/apidocs/spot/en/#borrow-get-loan-borrow-history-user_data
+    POST /sapi/v1/simple-earn/flexible/subscribe
 
+    https://binance-docs.github.io/apidocs/spot/en/#subscribe-flexible-product-trade
+
+    Args:
+        productId (str)
+        amount (float)
     Keyword Args:
-      orderId (int, optional): orderId in POST /sapi/v1/loan/borrow
-      loanCoin (str, optional)
-      collateralCoin (str, optional)
-      startTime (int, optional)
-      endTime (int, optional)
-      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000.
-      limit (int, optional): Default: 10; max: 100
-      recvWindow (int, optional): The value cannot be greater than 60000
+        autoSubscribe (boolean, optional): true or false, default true.
+        sourceAccount (str, optional): SPOT,FUND,ALL, default SPOT
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
+    check_required_parameters([[productId, "productId"], [amount, "amount"]])
 
-    return self.sign_request("GET", "/sapi/v1/loan/borrow/history", kwargs)
+    params = {"productId": productId, "amount": amount, **kwargs}
+    url_path = "/sapi/v1/simple-earn/flexible/subscribe"
+    return self.sign_request("POST", url_path, params)
 
 
-def loan_ongoing_orders(self, **kwargs):
-    """Get Loan Ongoing Orders (USER_DATA)
+def subscribe_locked_product(self, projectId: str, amount: float, **kwargs):
+    """Subscribe Locked Product (TRADE)
 
-    GET /sapi/v1/loan/ongoing/orders
+    Weight(IP): 1
 
-    https://binance-docs.github.io/apidocs/spot/en/#borrow-get-loan-ongoing-orders-user_data
-
-    Keyword Args:
-      orderId (int, optional): orderId in POST /sapi/v1/loan/borrow
-      loanCoin (str, optional)
-      collateralCoin (str, optional)
-      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000
-      limit (int, optional): Default: 10; max: 100
-      recvWindow (int, optional): The value cannot be greater than 60000
-    """
-
-    return self.sign_request("GET", "/sapi/v1/loan/ongoing/orders", kwargs)
+    Rate Limit: 1/3s per account
 
+    POST /sapi/v1/simple-earn/locked/subscribe
 
-def loan_repay(self, orderId: int, amount: float, **kwargs):
-    """Crypto Loan Repay (TRADE)
-
-    POST /sapi/v1/loan/repay
-
-    https://binance-docs.github.io/apidocs/spot/en/#repay-crypto-loan-repay-trade
+    https://binance-docs.github.io/apidocs/spot/en/#subscribe-locked-product-trade
 
     Args:
-      orderId (int)
-      amount (float)
+        projectId (str)
+        amount (float)
     Keyword Args:
-      type (int, optional): Default: 1. 1 for "repay with borrowed coin"; 2 for "repay with collateral"
-      collateralReturn (boolean, optional): Default: TRUE. TRUE: Return extra collateral to spot account; FALSE: Keep extra collateral in the order.
-      recvWindow (int, optional): The value cannot be greater than 60000
+        autoSubscribe (boolean, optional): true or false, default true.
+        sourceAccount (str, optional): SPOT,FUND,ALL, default SPOT
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
+    check_required_parameters([[projectId, "projectId"], [amount, "amount"]])
 
-    check_required_parameters([[orderId, "orderId"], [amount, "amount"]])
+    params = {"projectId": projectId, "amount": amount, **kwargs}
+    url_path = "/sapi/v1/simple-earn/locked/subscribe"
+    return self.sign_request("POST", url_path, params)
 
-    payload = {"orderId": orderId, "amount": amount, **kwargs}
-    return self.sign_request("POST", "/sapi/v1/loan/repay", payload)
 
+def redeem_flexible_product(self, productId: str, **kwargs):
+    """Redeem Flexible Product (TRADE)
 
-def loan_repay_history(self, **kwargs):
-    """Get Loan Repayment History (USER_DATA)
+    Weight(IP): 1
 
-    GET /sapi/v1/loan/repay/history
+    Rate Limit: 1/3s per account
 
-    https://binance-docs.github.io/apidocs/spot/en/#repay-get-loan-repayment-history-user_data
+    POST /sapi/v1/simple-earn/flexible/redeem
 
+    https://binance-docs.github.io/apidocs/spot/en/#redeem-flexible-product-trade
+
+    Args:
+        productId (str)
     Keyword Args:
-      orderId (int, optional)
-      loanCoin (str, optional)
-      collateralCoin (str, optional)
-      startTime (int, optional)
-      endTime (int, optional)
-      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000.
-      limit (int, optional): Default: 10; max: 100
-      recvWindow (int, optional): The value cannot be greater than 60000
+        redeemAll (boolean, optional): true or false, default to false
+        amount (float, optional): if redeemAll is false, amount is mandatory
+        destAccount (str, optional): SPOT,FUND,ALL, default SPOT
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
+    check_required_parameter(productId, "productId")
+
+    params = {"productId": productId, **kwargs}
+    url_path = "/sapi/v1/simple-earn/flexible/redeem"
+    return self.sign_request("POST", url_path, params)
 
-    return self.sign_request("GET", "/sapi/v1/loan/repay/history", kwargs)
 
+def redeem_locked_product(self, positionId: str, **kwargs):
+    """Redeem Locked Product (TRADE)
 
-def loan_adjust_ltv(self, orderId: int, amount: float, direction: str, **kwargs):
-    """Crypto Loan Adjust LTV (TRADE)
+    Weight(IP): 1
 
-    POST /sapi/v1/loan/adjust/ltv
+    Rate Limit: 1/3s per account
 
-    https://binance-docs.github.io/apidocs/spot/en/#adjust-ltv-crypto-loan-adjust-ltv-trade
+    POST /sapi/v1/simple-earn/locked/redeem
+
+    https://binance-docs.github.io/apidocs/spot/en/#redeem-locked-product-trade
 
     Args:
-      orderId (int)
-      amount (float)
-      direction (str): "ADDITIONAL", "REDUCED"
+        positionId (str)
     Keyword Args:
-      recvWindow (int, optional): The value cannot be greater than 60000
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
+    check_required_parameter(positionId, "positionId")
 
-    check_required_parameters(
-        [[orderId, "orderId"], [amount, "amount"], [direction, "direction"]]
-    )
+    params = {"positionId": positionId, **kwargs}
+    url_path = "/sapi/v1/simple-earn/locked/redeem"
+    return self.sign_request("POST", url_path, params)
 
-    payload = {"orderId": orderId, "amount": amount, "direction": direction, **kwargs}
-    return self.sign_request("POST", "/sapi/v1/loan/adjust/ltv", payload)
 
+def get_flexible_product_position(self, **kwargs):
+    """Get Flexible Product Position (USER_DATA)
 
-def loan_adjust_ltv_history(self, **kwargs):
-    """Get Loan LTV Adjustment History (USER_DATA)
+    Weight(IP): 150
 
-    GET /sapi/v1/loan/ltv/adjustment/history
+    GET /sapi/v1/simple-earn/flexible/position
 
-    https://binance-docs.github.io/apidocs/spot/en/#adjust-ltv-get-loan-ltv-adjustment-history-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-flexible-product-position-user_data
 
     Keyword Args:
-      orderId (int, optional)
-      loanCoin (str, optional)
-      collateralCoin (str, optional)
-      startTime (int, optional)
-      endTime (int, optional)
-      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000
-      limit (int, optional): Default: 10; max: 100
-      recvWindow (int, optional): The value cannot be greater than 60000
+        asset (str, optional)
+        productId (str, optional)
+        current (int, optional): Current querying page. Start from 1. Default:1
+        size (int, optional): Default:10 Max:100
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    return self.sign_request("GET", "/sapi/v1/loan/ltv/adjustment/history", kwargs)
+    url_path = "/sapi/v1/simple-earn/flexible/position"
+    return self.sign_request("GET", url_path, {**kwargs})
+
 
+def get_locked_product_position(self, **kwargs):
+    """Get Locked Product Position (USER_DATA)
 
-def loan_vip_ongoing_orders(self, **kwargs):
-    """Get VIP Loan Ongoing Orders (USER_DATA)
+    Weight(IP): 150
 
-    GET /sapi/v1/loan/vip/ongoing/orders
+    GET /sapi/v1/simple-earn/locked/position
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-vip-loan-ongoing-orders-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-locked-product-position-user_data
 
     Keyword Args:
-      orderId (int, optional)
-      collateralAccountId (int, optional)
-      loanCoin (str, optional)
-      collateralCoin (str, optional)
-      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000
-      limit (int, optional): Default: 10; max: 100
-      recvWindow (int, optional): The value cannot be greater than 60000
+        asset (str, optional)
+        positionId (str, optional)
+        projectId (str, optional)
+        current (int, optional): Current querying page. Start from 1. Default:1
+        size (int, optional): Default:10 Max:100
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    return self.sign_request("GET", "/sapi/v1/loan/vip/ongoing/orders", kwargs)
+    url_path = "/sapi/v1/simple-earn/locked/position"
+    return self.sign_request("GET", url_path, {**kwargs})
 
 
-def loan_vip_repay(self, orderId: int, amount: float, **kwargs):
-    """VIP Loan Repay (TRADE)
+def simple_account(self, **kwargs):
+    """Simple Account (USER_DATA)
 
-    POST /sapi/v1/loan/vip/repay
+    Weight(IP): 150
 
-    https://binance-docs.github.io/apidocs/spot/en/#vip-loan-repay-trade
+    GET /sapi/v1/simple-earn/account
+
+    https://binance-docs.github.io/apidocs/spot/en/#simple-account-user_data
 
-    Args:
-      orderId (int)
-      amount (float)
     Keyword Args:
-      recvWindow (int, optional): The value cannot be greater than 60000
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    check_required_parameters([[orderId, "orderId"], [amount, "amount"]])
+    url_path = "/sapi/v1/simple-earn/account"
+    return self.sign_request("GET", url_path, {**kwargs})
 
-    payload = {"orderId": orderId, "amount": amount, **kwargs}
-    return self.sign_request("POST", "/sapi/v1/loan/vip/repay", payload)
 
+def get_flexible_subscription_record(self, **kwargs):
+    """Get Flexible Subscription Record (USER_DATA)
 
-def loan_vip_repay_history(self, **kwargs):
-    """Get VIP Loan Repayment History (USER_DATA)
+    Weight(IP): 150
 
-    GET /sapi/v1/loan/vip/repay/history
+    GET /sapi/v1/simple-earn/flexible/history/subscriptionRecord
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-vip-loan-repayment-history-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-flexible-subscription-record-user_data
 
     Keyword Args:
-      orderId (int, optional)
-      loanCoin (str, optional)
-      startTime (int, optional)
-      endTime (int, optional)
-      current (int, optional): Current querying page. Start from 1; default: 1; max: 1000
-      limit (int, optional): Default: 10; max: 100
-      recvWindow (int, optional): The value cannot be greater than 60000
+        productId (str, optional)
+        purchaseId (str, optional)
+        asset (str, optional)
+        startTime (int, optional): UTC timestamp in ms
+        endTime (int, optional): UTC timestamp in ms
+        current (int, optional): Current querying page. Start from 1. Default:1
+        size (int, optional): Default:10 Max:100
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    return self.sign_request("GET", "/sapi/v1/loan/vip/repay/history", kwargs)
+    url_path = "/sapi/v1/simple-earn/flexible/history/subscriptionRecord"
+    return self.sign_request("GET", url_path, {**kwargs})
+
 
+def get_locked_subscription_record(self, **kwargs):
+    """Get Locked Subscription Record (USER_DATA)
 
-def loan_vip_collateral_account(self, **kwargs):
-    """Check Locked Value of VIP Collateral Account (USER_DATA)
+    Weight(IP): 150
 
-    GET /sapi/v1/loan/vip/collateral/account
+    GET /sapi/v1/simple-earn/locked/history/subscriptionRecord
 
-    https://binance-docs.github.io/apidocs/spot/en/#check-locked-value-of-vip-collateral-account-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-locked-subscription-record-user_data
 
     Keyword Args:
-      orderId (int, optional)
-      collateralAccountId (int, optional)
-      recvWindow (int, optional): The value cannot be greater than 60000
+        purchaseId (str, optional)
+        asset (str, optional)
+        startTime (int, optional): UTC timestamp in ms
+        endTime (int, optional): UTC timestamp in ms
+        current (int, optional): Current querying page. Start from 1. Default:1
+        size (int, optional): Default:10 Max:100
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    return self.sign_request("GET", "/sapi/v1/loan/vip/collateral/account", kwargs)
+    url_path = "/sapi/v1/simple-earn/locked/history/subscriptionRecord"
+    return self.sign_request("GET", url_path, {**kwargs})
+
 
+def get_flexible_redemption_record(self, **kwargs):
+    """Get Flexible Redemption Record (USER_DATA)
 
-def loan_loanable_data(self, **kwargs):
-    """Get Loanable Assets Data (USER_DATA)
+    Weight(IP): 150
 
-    GET /sapi/v1/loan/loanable/data
+    GET /sapi/v1/simple-earn/flexible/history/redemptionRecord
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-loanable-assets-data-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-flexible-redemption-record-user_data
 
     Keyword Args:
-      loanCoin (str, optional)
-      vipLevel (int, optional)
-      recvWindow (int, optional): The value cannot be greater than 60000
+        productId (str, optional)
+        redeemId (str, optional)
+        asset (str, optional)
+        startTime (int, optional): UTC timestamp in ms
+        endTime (int, optional): UTC timestamp in ms
+        current (int, optional): Current querying page. Start from 1. Default:1
+        size (int, optional): Default:10 Max:100
     """
 
-    return self.sign_request("GET", "/sapi/v1/loan/loanable/data", kwargs)
+    url_path = "/sapi/v1/simple-earn/flexible/history/redemptionRecord"
+    return self.sign_request("GET", url_path, {**kwargs})
+
 
+def get_locked_redemption_record(self, **kwargs):
+    """Get Locked Redemption Record (USER_DATA)
 
-def loan_collateral_data(self, **kwargs):
-    """Get Collateral Assets Data (USER_DATA)
+    Weight(IP): 150
 
-    GET /sapi/v1/loan/collateral/data
+    GET /sapi/v1/simple-earn/locked/history/redemptionRecord
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-collateral-assets-data-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-locked-redemption-record-user_data
 
     Keyword Args:
-      collateralCoin (str, optional)
-      vipLevel (int, optional)
-      recvWindow (int, optional): The value cannot be greater than 60000
+        positionId (str, optional)
+        redeemId (str, optional)
+        asset (str, optional)
+        startTime (int, optional): UTC timestamp in ms
+        endTime (int, optional): UTC timestamp in ms
+        current (int, optional): Current querying page. Start from 1. Default:1
+        size (int, optional): Default:10 Max:100
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    return self.sign_request("GET", "/sapi/v1/loan/collateral/data", kwargs)
+    url_path = "/sapi/v1/simple-earn/locked/history/redemptionRecord"
+    return self.sign_request("GET", url_path, {**kwargs})
+
 
+def get_flexible_rewards_history(self, type: str, **kwargs):
+    """Get Flexible Rewards History (USER_DATA)
 
-def loan_collateral_rate(
-    self, loanCoin: str, collateralCoin: str, repayAmount: float, **kwargs
-):
-    """Check Collateral Repay Rate (USER_DATA)
+    Weight(IP): 150
 
-    GET /sapi/v1/loan/repay/collateral/rate
+    GET /sapi/v1/simple-earn/flexible/history/rewardsRecord
 
-    https://binance-docs.github.io/apidocs/spot/en/#check-collateral-repay-rate-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-flexible-rewards-history-user_data
 
     Args:
-      loanCoin (str)
-      collateralCoin (str)
-      repayAmount (float)
+        type (str)
     Keyword Args:
-      recvWindow (int, optional): The value cannot be greater than 60000
+        productId (str, optional)
+        asset (str, optional)
+        startTime (int, optional): UTC timestamp in ms
+        endTime (int, optional): UTC timestamp in ms
     """
+    check_required_parameter(type, "type")
 
-    check_required_parameters(
-        [
-            [loanCoin, "loanCoin"],
-            [collateralCoin, "collateralCoin"],
-            [repayAmount, "repayAmount"],
-        ]
-    )
+    params = {"type": type, **kwargs}
+    url_path = "/sapi/v1/simple-earn/flexible/history/rewardsRecord"
+    return self.sign_request("GET", url_path, params)
 
-    payload = {
-        "loanCoin": loanCoin,
-        "collateralCoin": collateralCoin,
-        "repayAmount": repayAmount,
-        **kwargs,
-    }
-    return self.sign_request("GET", "/sapi/v1/loan/repay/collateral/rate", payload)
 
+def get_locked_rewards_history(self, **kwargs):
+    """Get Locked Rewards History (USER_DATA)
 
-def loan_customize_margin_call(self, marginCall: float, **kwargs):
-    """Customize Margin Call (USER_DATA)
+    Weight(IP): 150
 
-    POST /sapi/v1/loan/customize/margin_call
+    GET /sapi/v1/simple-earn/locked/history/rewardsRecord
 
-    https://binance-docs.github.io/apidocs/spot/en/#crypto-loan-customize-margin-call-trade
+    https://binance-docs.github.io/apidocs/spot/en/#get-locked-rewards-history-user_data
 
-    Args:
-      marginCall (float)
     Keyword Args:
-      orderId (int, optional)
-      collateralCoin (str, optional)
-      recvWindow (int, optional): The value cannot be greater than 60000
+        positionId (str, optional)
+        asset (str, optional)
+        startTime (int, optional): UTC timestamp in ms
+        endTime (int, optional): UTC timestamp in ms
+        current (int, optional): Currently querying the page. Start from 1. Default:1
+        size (int, optional): Default:10 Max:100
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    check_required_parameter(marginCall, "marginCall")
-
-    payload = {"marginCall": marginCall, **kwargs}
-    return self.sign_request("POST", "/sapi/v1/loan/customize/margin_call", payload)
+    url_path = "/sapi/v1/simple-earn/locked/history/rewardsRecord"
+    return self.sign_request("GET", url_path, {**kwargs})
 
 
-def flexible_loan_borrow(self, loanCoin: str, collateralCoin: str, **kwargs):
-    """Borrow - Flexible Loan Borrow (TRADE)
+def set_flexible_auto_subscribe(self, productId: str, autoSubscribe: bool, **kwargs):
+    """Set Flexible Auto Subscribe (USER_DATA)
 
-    Weight(UID): 6000
+    Weight(IP): 150
 
-    POST /sapi/v1/loan/flexible/borrow
+    POST /sapi/v1/simple-earn/flexible/setAutoSubscribe
 
-    https://binance-docs.github.io/apidocs/spot/en/#borrow-flexible-loan-borrow
+    https://binance-docs.github.io/apidocs/spot/en/#set-flexible-auto-subscribe-user_data
 
     Args:
-        loanCoin (str, optional): Coin loaned
-        collateralCoin (str, optional): Coin used as collateral
+        productId (str)
+        autoSubscribe (boolean)
     Keyword Args:
-        loanAmount (float, optional): Loan amount
-        collateralAmount (float, optional) Mandatory when loanAmount is empty
         recvWindow (int, optional): The value cannot be greater than 60000
     """
-
     check_required_parameters(
-        [[loanCoin, "loanCoin"], [collateralCoin, "collateralCoin"]]
+        [[productId, "productId"], [autoSubscribe, "autoSubscribe"]]
     )
 
-    payload = {
-        "loanCoin": loanCoin,
-        "collateralCoin": collateralCoin,
-        **kwargs,
-    }
+    params = {"productId": productId, "autoSubscribe": autoSubscribe, **kwargs}
+    url_path = "/sapi/v1/simple-earn/flexible/setAutoSubscribe"
+    return self.sign_request("POST", url_path, params)
 
-    url_path = "/sapi/v1/loan/flexible/borrow"
-    return self.sign_request("POST", url_path, payload)
 
+def set_locked_auto_subscribe(self, positionId: str, autoSubscribe: bool, **kwargs):
+    """Set Locked Auto Subscribe (USER_DATA)
 
-def flexible_loan_ongoing_orders(self, **kwargs):
-    """Borrow - Get Flexible Loan Ongoing Orders (USER_DATA)
+    Weight(IP): 150
 
-    Weight(IP): 300
+    POST /sapi/v1/simple-earn/locked/setAutoSubscribe
 
-    GET /sapi/v1/loan/flexible/ongoing/orders
-
-    https://binance-docs.github.io/apidocs/spot/en/#borrow-get-flexible-loan-ongoing-orders-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#set-locked-auto-subscribe-user_data
 
+    Args:
+        positionId (str)
+        autoSubscribe (boolean)
     Keyword Args:
-        loanCoin (str, optional): Coin loaned
-        collateralCoin (str, optional): Coin used as collateral
-        current (int, optional): Current querying page. Start from 1. Default:1
-        limit (int, optional): Default 500; max 1000.
         recvWindow (int, optional): The value cannot be greater than 60000
     """
+    check_required_parameters(
+        [[positionId, "positionId"], [autoSubscribe, "autoSubscribe"]]
+    )
 
-    url_path = "/sapi/v1/loan/flexible/ongoing/orders"
-    return self.sign_request("GET", url_path, {**kwargs})
+    params = {"positionId": positionId, "autoSubscribe": autoSubscribe, **kwargs}
+    url_path = "/sapi/v1/simple-earn/locked/setAutoSubscribe"
+    return self.sign_request("POST", url_path, params)
 
 
-def flexible_loan_borrow_history(self, **kwargs):
-    """Borrow - Get Flexible Loan Borrow History (USER_DATA)
+def get_flexible_personal_left_quota(self, productId: str, **kwargs):
+    """Get Flexible Personal Left Quota (USER_DATA)
 
-    Weight(IP): 400
+    Weight(IP): 150
 
-    GET /sapi/v1/loan/flexible/borrow/history
+    GET /sapi/v1/simple-earn/flexible/personalLeftQuota
 
-    https://binance-docs.github.io/apidocs/spot/en/#borrow-get-flexible-loan-borrow-history-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-flexible-personal-left-quota-user_data
 
+    Args:
+        productId (str)
     Keyword Args:
-        loanCoin (str, optional): Coin loaned
-        collateralCoin (str, optional): Coin used as collateral
-        startTime (int, optional): UTC timestamp in ms
-        endTime (int, optional): UTC timestamp in ms
-        current (int, optional): Current querying page. Start from 1. Default:1
-        limit (int, optional): Default 500; max 1000.
         recvWindow (int, optional): The value cannot be greater than 60000
     """
+    check_required_parameter(productId, "productId")
 
-    url_path = "/sapi/v1/loan/flexible/borrow/history"
-    return self.sign_request("GET", url_path, {**kwargs})
+    params = {"productId": productId, **kwargs}
+    url_path = "/sapi/v1/simple-earn/flexible/personalLeftQuota"
+    return self.sign_request("GET", url_path, params)
 
 
-def flexible_loan_repay(
-    self, loanCoin: str, collateralCoin: str, repayAmount: float, **kwargs
-):
-    """Repay - Flexible Loan Repay (TRADE)
+def get_locked_personal_left_quota(self, projectId: str, **kwargs):
+    """Get Locked Personal Left Quota (USER_DATA)
 
-    Weight(IP): 6000
+    Weight(IP): 150
 
-    POST /sapi/v1/loan/flexible/repay
+    GET /sapi/v1/simple-earn/locked/personalLeftQuota
 
-    https://binance-docs.github.io/apidocs/spot/en/#repay-flexible-loan-repay-trade
+    https://binance-docs.github.io/apidocs/spot/en/#get-locked-personal-left-quota-user_data
 
     Args:
-        loanCoin (str, optional): Coin loaned
-        collateralCoin (str, optional): Coin used as collateral
-        repayAmount (float)
+        projectId (str)
     Keyword Args:
-        collateralReturn (boolean, optional)
-        fullRepayment (boolean, optional)
         recvWindow (int, optional): The value cannot be greater than 60000
     """
-    check_required_parameters(
-        [
-            [repayAmount, "repayAmount"],
-            [collateralCoin, "collateralCoin"],
-            [loanCoin, "loanCoin"],
-        ]
-    )
-
-    payload = {
-        "repayAmount": repayAmount,
-        "collateralCoin": collateralCoin,
-        "loanCoin": loanCoin,
-        **kwargs,
-    }
-    url_path = "/sapi/v1/loan/flexible/repay"
-    return self.sign_request("POST", url_path, payload)
+    check_required_parameter(projectId, "projectId")
 
+    params = {"projectId": projectId, **kwargs}
+    url_path = "/sapi/v1/simple-earn/locked/personalLeftQuota"
+    return self.sign_request("GET", url_path, params)
 
-def flexible_loan_repayment_history(self, **kwargs):
-    """Repay - Get Flexible Loan Repayment History (USER_DATA)
 
+def get_flexible_subscription_preview(self, productId: str, amount: float, **kwargs):
+    """Get Flexible Subscription Preview (USER_DATA)
 
-    Weight(IP): 400
+    Weight(IP): 150
 
-    GET /sapi/v1/loan/flexible/repay/history
+    GET /sapi/v1/simple-earn/flexible/subscriptionPreview
 
-    https://binance-docs.github.io/apidocs/spot/en/#repay-get-flexible-loan-repayment-history-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-flexible-subscription-preview-user_data
 
+    Args:
+        productId (str)
+        amount (float)
     Keyword Args:
-        loanCoin (str, optional): Coin loaned
-        collateralCoin (str, optional): Coin used as collateral
-        startTime (int, optional): UTC timestamp in ms
-        endTime (int, optional): UTC timestamp in ms
-        current (int, optional): Current querying page. Start from 1. Default:1
-        limit (int, optional): Default 500; max 1000.
         recvWindow (int, optional): The value cannot be greater than 60000
     """
+    check_required_parameters([[productId, "productId"], [amount, "amount"]])
 
-    url_path = "/sapi/v1/loan/flexible/repay/history"
-    return self.sign_request("GET", url_path, {**kwargs})
-
+    params = {"productId": productId, "amount": amount, **kwargs}
+    url_path = "/sapi/v1/simple-earn/flexible/subscriptionPreview"
+    return self.sign_request("GET", url_path, params)
 
-def flexible_loan_adjust_ltv(
-    self,
-    loanCoin: str,
-    collateralCoin: str,
-    adjustmentAmount: float,
-    direction: str,
-    **kwargs
-):
-    """Adjust LTV - Flexible Loan Adjust LTV (TRADE)
 
+def get_locked_subscription_preview(self, projectId: str, amount: float, **kwargs):
+    """Get Locked Subscription Preview (USER_DATA)
 
-    Weight(UID): 6000
+    Weight(IP): 150
 
-    POST /sapi/v1/loan/flexible/adjust/ltv
+    GET /sapi/v1/simple-earn/locked/subscriptionPreview
 
-    https://binance-docs.github.io/apidocs/spot/en/#adjust-ltv-flexible-loan-adjust-ltv-trade
+    https://binance-docs.github.io/apidocs/spot/en/#get-locked-subscription-preview-user_data
 
     Args:
-        loanCoin (str)
-        collateralCoin (str)
-        adjustmentAmount (float)
-        direction (Direction)
+        projectId (str)
+        amount (float)
     Keyword Args:
+        autoSubscribe (boolean, optional): true or false, default true.
         recvWindow (int, optional): The value cannot be greater than 60000
     """
-    check_required_parameters(
-        [
-            [loanCoin, "loanCoin"],
-            [collateralCoin, "collateralCoin"],
-            [adjustmentAmount, "adjustmentAmount"],
-            [direction, "direction"],
-        ]
-    )
+    check_required_parameters([[projectId, "projectId"], [amount, "amount"]])
 
-    payload = {
-        "loanCoin": loanCoin,
-        "collateralCoin": collateralCoin,
-        "adjustmentAmount": adjustmentAmount,
-        "direction": direction,
-        **kwargs,
-    }
-    url_path = "/sapi/v1/loan/flexible/adjust/ltv"
-    return self.sign_request("POST", url_path, payload)
+    params = {"projectId": projectId, "amount": amount, **kwargs}
+    url_path = "/sapi/v1/simple-earn/locked/subscriptionPreview"
+    return self.sign_request("GET", url_path, params)
 
 
-def flexible_loan_ltv_adjustment_history(self, **kwargs):
-    """Adjust LTV - Get Flexible Loan LTV Adjustment History (USER_DATA)
+def get_rate_history(self, productId: str, **kwargs):
+    """Get Rate History (USER_DATA)
 
-    Weight(IP): 400
+    Weight(IP): 150
 
-    GET /sapi/v1/loan/flexible/ltv/adjustment/history
+    GET /sapi/v1/simple-earn/flexible/history/rateHistory
 
-    https://binance-docs.github.io/apidocs/spot/en/#adjust-ltv-get-flexible-loan-ltv-adjustment-history-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-rate-history-user_data
 
+    Args:
+        productId (str)
     Keyword Args:
-        loanCoin (str, optional): Coin loaned
-        collateralCoin (str, optional): Coin used as collateral
         startTime (int, optional): UTC timestamp in ms
         endTime (int, optional): UTC timestamp in ms
         current (int, optional): Current querying page. Start from 1. Default:1
-        limit (int, optional): Default 500; max 1000.
-        recvWindow (int, optional): The value cannot be greater than 60000
-    """
-
-    url_path = "/sapi/v1/loan/flexible/ltv/adjustment/history"
-    return self.sign_request("GET", url_path, {**kwargs})
-
-
-def flexible_loan_assets_data(self, **kwargs):
-    """Get Flexible Loan Assets Data (USER_DATA)
-
-    Get interest rate and borrow limit of flexible loanable assets. The borrow limit is shown in USD value.
-
-    Weight(IP): 400
-
-    GET /sapi/v1/loan/flexible/loanable/data
-
-    https://binance-docs.github.io/apidocs/spot/en/#get-flexible-loan-assets-data-user_data
-
-    Keyword Args:
-        loanCoin (str, optional): Coin loaned
+        size (int, optional): Default:10 Max:100
         recvWindow (int, optional): The value cannot be greater than 60000
     """
+    check_required_parameter(productId, "productId")
 
-    url_path = "/sapi/v1/loan/flexible/loanable/data"
-    return self.sign_request("GET", url_path, {**kwargs})
-
+    params = {"productId": productId, **kwargs}
+    url_path = "/sapi/v1/simple-earn/flexible/history/rateHistory"
+    return self.sign_request("GET", url_path, params)
 
-def flexible_loan_collateral_assets_data(self, **kwargs):
-    """Get Flexible Loan Collateral Assets Data (USER_DATA)
 
-    Get LTV information and collateral limit of flexible loan's collateral assets. The collateral limit is shown in USD value.
+def get_collateral_record(self, **kwargs):
+    """Get Collateral Record (USER_DATA)
 
-    Weight(IP): 400
+    Weight(IP): 150
 
-    GET /sapi/v1/loan/flexible/collateral/data
+    GET /sapi/v1/simple-earn/flexible/history/collateralRecord
 
-    https://binance-docs.github.io/apidocs/spot/en/#get-flexible-loan-collateral-assets-data-user_data
+    https://binance-docs.github.io/apidocs/spot/en/#get-collateral-record-user_data
 
     Keyword Args:
-        collateralCoin (str, optional): Coin used as collateral
+        productId (str, optional)
+        startTime (int, optional): UTC timestamp in ms
+        endTime (int, optional): UTC timestamp in ms
+        current (int, optional): Current querying page. Start from 1. Default:1
+        size (int, optional): Default:10 Max:100
         recvWindow (int, optional): The value cannot be greater than 60000
     """
 
-    url_path = "/sapi/v1/loan/flexible/collateral/data"
+    url_path = "/sapi/v1/simple-earn/flexible/history/collateralRecord"
     return self.sign_request("GET", url_path, {**kwargs})
```

### Comparing `binance-connector-3.6.0/binance/spot/_data_stream.py` & `binance-connector-3.7.0/binance/spot/_data_stream.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/_fiat.py` & `binance-connector-3.7.0/binance/spot/_fiat.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/_futures.py` & `binance-connector-3.7.0/binance/spot/_futures.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/_gift_card.py` & `binance-connector-3.7.0/binance/spot/_gift_card.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/_margin.py` & `binance-connector-3.7.0/binance/spot/_margin.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,17 +108,17 @@
         quoteOrderQty (float, optional)
         price (float, optional)
         stopPrice (float, optional): Used with STOP_LOSS,STOP_LOSS_LIMIT,TAKE_PROFIT and TAKE_PROFIT_LIMIT orders.
         newClientOrderId (str, optional): A unique id among open orders. Automatically generated if not sent.
         icebergQty (float, optional): Used with LIMIT, STOP_LOSS_LIMIT and TAKE_PROFIT_LIMIT to create an iceberg order.
         newOrderRespType (str, optional): Set the response JSON. ACK, RESULT or FULL;
                 MARKET and LIMIT order types default to FULL, all other orders default to ACK.
-        sideEffectType (str, optional): NO_SIDE_EFFECT, MARGIN_BUY, AUTO_REPAY; default NO_SIDE_EFFECT.
+        sideEffectType (str, optional): NO_SIDE_EFFECT, MARGIN_BUY, AUTO_REPAY,AUTO_BORROW_REPAY; default NO_SIDE_EFFECT.
         timeInForce (str, optional): GTC,IOC,FOK
-        isIsolated (str, optional): for isolated margin or not,"TRUE", "FALSE"，default "FALSE".
+        isIsolated (str, optional): for isolated margin or not,"TRUE", "FALSE" default "FALSE".
         recvWindow (int, optional): The value cannot be greater than 60000
     """
 
     check_required_parameters(
         [
             [symbol, "symbol"],
             [side, "side"],
@@ -508,15 +508,15 @@
         limitClientOrderId (str, optional): A unique Id for the limit order
         limitIcebergQty (float, optional)
         stopClientOrderId (str, optional): A unique Id for the stop loss/stop loss limit leg
         stopLimitPrice (float, optional): If provided, stopLimitTimeInForce is required
         stopIcebergQty (float, optional)
         stopLimitTimeInForce (str, optional): Valid values are GTC/FOK/IOC
         newOrderRespType (str, optional): Set the response JSON
-        sideEffectType (str, optional): NO_SIDE_EFFECT, MARGIN_BUY, AUTO_REPAY; default NO_SIDE_EFFECT
+        sideEffectType (str, optional): NO_SIDE_EFFECT, MARGIN_BUY, AUTO_REPAY,AUTO_BORROW_REPAY; default NO_SIDE_EFFECT
         recvWindow (int, optional): The value cannot be greater than 60000
     """
 
     check_required_parameters(
         [
             [symbol, "symbol"],
             [side, "side"],
@@ -626,15 +626,15 @@
     """Query Margin Account's Open OCO (USER_DATA)
 
     GET /sapi/v1/margin/openOrderList
 
     https://binance-docs.github.io/apidocs/spot/en/#query-margin-account-39-s-open-oco-user_data
 
     Keyword Args:
-        isIsolated (str, optional): For isolated margin or not "TRUE", "FALSE"，default "FALSE"
+        isIsolated (str, optional): For isolated margin or not "TRUE", "FALSE" default "FALSE"
         symbol (str, optional): Mandatory for isolated margin, not supported for cross margin
         recvWindow (int, optional): The value cannot be greater than 60000
     """
     if kwargs.get("isIsolated"):
         check_required_parameter(kwargs.get("symbol"), "symbol")
     return self.sign_request("GET", "/sapi/v1/margin/openOrderList", {**kwargs})
 
@@ -877,7 +877,55 @@
         recvWindow (int, optional): The value cannot be greater than 60000
     """
     check_required_parameter(maxLeverage, "maxLeverage")
 
     params = {"maxLeverage": maxLeverage, **kwargs}
     url_path = "/sapi/v1/margin/max-leverage"
     return self.sign_request("POST", url_path, params)
+
+
+def margin_available_inventory(self, type: str, **kwargs):
+    """Query Margin Available Inventory (USER_DATA)
+
+    GET /sapi/v1/margin/available-inventory
+
+    https://binance-docs.github.io/apidocs/spot/en/#query-margin-available-inventory-user_data
+
+    Args:
+        type (str): "MARGIN", "ISOLATED"
+    Keyword Args:
+        recvWindow (int, optional): The value cannot be greater than 60000
+    """
+    check_required_parameter(type, "type")
+    payload = {"type": type, **kwargs}
+    return self.sign_request("GET", "/sapi/v1/margin/available-inventory", payload)
+
+
+def margin_manual_liquidation(self, type: str, **kwargs):
+    """Margin manual liquidation(MARGIN)
+
+    POST /sapi/v1/margin/manual-liquidation
+
+    https://binance-docs.github.io/apidocs/spot/en/#margin-manual-liquidation-margin
+
+    Args:
+        type (str): "MARGIN", "ISOLATED"
+    Keyword Args:
+        symbol (str, optional): When type selects ISOLATED, symbol must be filled in
+        recvWindow (int, optional): The value cannot be greater than 60000
+    """
+    check_required_parameters([[type, "type"]])
+    payload = {"type": type, **kwargs}
+    return self.sign_request("POST", "/sapi/v1/margin/manual-liquidation", payload)
+
+
+def liability_coin_leverage_bracket(self, **kwargs):
+    """Query Liability Coin Leverage Bracket in Cross Margin Pro Mode(MARKET_DATA)
+
+    GET /sapi/v1/margin/leverageBracket
+
+    https://binance-docs.github.io/apidocs/spot/en/#query-liability-coin-leverage-bracket-in-cross-margin-pro-mode-market_data
+
+    Keyword Args:
+        recvWindow (int, optional): The value cannot be greater than 60000
+    """
+    return self.sign_request("GET", "/sapi/v1/margin/leverageBracket", kwargs)
```

### Comparing `binance-connector-3.6.0/binance/spot/_market.py` & `binance-connector-3.7.0/binance/spot/_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,36 @@
         "symbol": symbol,
         "symbols": convert_list_to_json_array(symbols),
         **kwargs,
     }
     return self.query("/api/v3/ticker/24hr", params)
 
 
+def trading_day_ticker(self, symbol: str = None, symbols: list = None):
+    """Trading Day Ticker
+
+    GET /api/v3/ticker/tradingDay
+
+    https://binance-docs.github.io/apidocs/spot/en/#trading-day-ticker
+
+    Args:
+        symbol (str, optional): Either symbol or symbols must be provided
+        symbols (list, optional): list of trading pairs
+    Keyword Args:
+        timeZone (str, optional): Default: 0 (UTC)
+        type (str, optional): Supported values: FULL or MINI. If none provided, the default is FULL.
+    """
+    if symbol and symbols:
+        raise ParameterArgumentError("symbol and symbols cannot be sent together.")
+
+    check_type_parameter(symbols, "symbols", list)
+    params = {"symbol": symbol, "symbols": convert_list_to_json_array(symbols)}
+    return self.query("/api/v3/ticker/tradingDay", params)
+
+
 def ticker_price(self, symbol: str = None, symbols: list = None):
     """Symbol Price Ticker
 
     GET /api/v3/ticker/price
 
     https://binance-docs.github.io/apidocs/spot/en/#symbol-price-ticker
```

### Comparing `binance-connector-3.6.0/binance/spot/_mining.py` & `binance-connector-3.7.0/binance/spot/_mining.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/_nft.py` & `binance-connector-3.7.0/binance/spot/_nft.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/_portfolio_margin.py` & `binance-connector-3.7.0/binance/spot/_portfolio_margin.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/_sub_account.py` & `binance-connector-3.7.0/binance/spot/_sub_account.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/spot/_trade.py` & `binance-connector-3.7.0/binance/spot/_trade.py`

 * *Files 3% similar despite different names*

```diff
@@ -438,15 +438,15 @@
     """
 
     url_path = "/api/v3/rateLimit/order"
     return self.sign_request("GET", url_path, {**kwargs})
 
 
 def query_prevented_matches(self, symbol: str, **kwargs):
-    """Query Prevented Matches
+    """Query Prevented Matches (USER_DATA)
 
     Displays the list of orders that were expired because of STP.
 
     For additional information on what a Prevented match is, as well as Self Trade Prevention (STP), please refer to our STP FAQ page.
 
     These are the combinations supported:
 
@@ -476,7 +476,50 @@
         recvWindow (int, optional): The value cannot be greater than 60000
     """
     check_required_parameter(symbol, "symbol")
 
     params = {"symbol": symbol, **kwargs}
     url_path = "/api/v3/myPreventedMatches"
     return self.sign_request("GET", url_path, params)
+
+
+def query_allocations(self, symbol: str, **kwargs):
+    """Query Cross-Collateral Information (USER_DATA)
+
+    GET /api/v3/myAllocations
+
+    https://binance-docs.github.io/apidocs/spot/en/#query-allocations-user_data
+
+    Args:
+        symbol (str)
+    Keyword Args:
+        startTime (int, optional)
+        endTime (int, optional)
+        fromAllocationId (int, optional)
+        limit (int, optional): Default Value: 500; Max Value: 1000
+        orderId (int, optional)
+        recvWindow (int, optional): The value cannot be greater than 60000
+    """
+    check_required_parameter(symbol, "symbol")
+
+    params = {"symbol": symbol, **kwargs}
+    url_path = "/api/v3/myAllocations"
+    return self.sign_request("GET", url_path, params)
+
+
+def query_commission_rates(self, symbol: str, **kwargs):
+    """Query Commission Rates (USER_DATA)
+
+    GET /api/v3/account/commission
+
+    https://binance-docs.github.io/apidocs/spot/en/#query-commission-rates-user_data
+
+    Args:
+        symbol (str)
+    Keyword Args:
+        recvWindow (int, optional): The value cannot be greater than 60000
+    """
+    check_required_parameter(symbol, "symbol")
+
+    params = {"symbol": symbol, **kwargs}
+    url_path = "/api/v3/account/commission"
+    return self.sign_request("GET", url_path, params)
```

### Comparing `binance-connector-3.6.0/binance/spot/_wallet.py` & `binance-connector-3.7.0/binance/spot/_wallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,17 @@
     Fetch small amounts of assets exchanged BNB records.
 
     GET /sapi/v1/asset/dribblet
 
     https://binance-docs.github.io/apidocs/spot/en/#dustlog-sapi-user_data
 
     Keyword Args:
+        accountType (str, optional): SPOT or MARGIN, default SPOT
+        startTime (int, optional)
+        endTime (int, optional)
         recvWindow (int, optional): The value cannot be greater than 60000
     """
 
     return self.sign_request("GET", "/sapi/v1/asset/dribblet", kwargs)
 
 
 def user_universal_transfer(self, type: str, asset: str, amount: str, **kwargs):
@@ -277,14 +280,15 @@
     POST /sapi/v1/asset/dust
 
     https://binance-docs.github.io/apidocs/spot/en/#dust-transfer-user_data
 
     Args:
         asset (str)
     Keyword Args:
+        accountType (str, optional): SPOT or MARGIN, default SPOT
         recvWindow (int, optional): The value cannot be greater than 60000
     """
 
     check_required_parameter(asset, "asset")
 
     payload = {"asset": ",".join(asset), **kwargs}
 
@@ -396,14 +400,15 @@
     """Get Assets That Can Be Converted Into BNB (USER_DATA)
 
     POST /sapi/v1/asset/dust-btc
 
     https://binance-docs.github.io/apidocs/spot/en/#get-assets-that-can-be-converted-into-bnb-user_data
 
     Keyword Args:
+        accountType (str, optional): SPOT or MARGIN, default SPOT
         recvWindow (int, optional): The value cannot be greater than 60000
     """
 
     return self.sign_request("POST", "/sapi/v1/asset/dust-btc", kwargs)
 
 
 def convertible_coins(self, **kwargs):
@@ -431,14 +436,31 @@
 
     payload = {"coin": coin, "enable": enable, **kwargs}
     return self.sign_request(
         "POST", "/sapi/v1/capital/contract/convertible-coins", payload
     )
 
 
+def list_deposit_address(self, coin: str, **kwargs):
+    """Fetch deposit address list with network(USER_DATA)
+
+    GET /sapi/v1/capital/deposit/address/list
+
+    https://binance-docs.github.io/apidocs/spot/en/#fetch-deposit-address-list-with-network-user_data
+
+    Args:
+        coin (str): coin refers to the parent network address format that the address is using
+    Keyword Args:
+        network (str, optional)
+    """
+    check_required_parameter(coin, "coin")
+    payload = {"coin": coin, **kwargs}
+    return self.sign_request("GET", "/sapi/v1/capital/deposit/address/list", payload)
+
+
 def cloud_mining_trans_history(self, startTime: int, endTime: int, **kwargs):
     """Get Cloud-Mining payment and refund history (USER_DATA)
 
     GET /sapi/v1/asset/ledger-transfer/cloud-mining/queryByPage
 
     https://binance-docs.github.io/apidocs/spot/en/#get-cloud-mining-payment-and-refund-history-user_data
 
@@ -556,12 +578,27 @@
     Weight(IP): 60
 
     GET /sapi/v1/asset/wallet/balance
 
     https://binance-docs.github.io/apidocs/spot/en/#query-user-wallet-balance-user_data
 
     Keyword Args:
-        recvWindow (LONG, optional)
+        recvWindow (int, optional): The value cannot be greater than 60000
     """
 
     url_path = "/sapi/v1/asset/wallet/balance"
     return self.sign_request("GET", url_path, {**kwargs})
+
+
+def delist_schedule_symbols(self, **kwargs):
+    """Get symbols delist schedule for spot (MARKET_DATA)
+
+    GET /sapi/v1/spot/delist-schedule
+
+    https://binance-docs.github.io/apidocs/spot/en/#get-symbols-delist-schedule-for-spot-market_data
+
+    Keyword Args:
+        recvWindow (int, optional): The value cannot be greater than 60000
+    """
+
+    url_path = "/sapi/v1/spot/delist-schedule"
+    return self.sign_request("GET", url_path, {**kwargs})
```

### Comparing `binance-connector-3.6.0/binance/websocket/binance_socket_manager.py` & `binance-connector-3.7.0/binance/websocket/binance_socket_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,18 +74,20 @@
             except WebSocketException as e:
                 if isinstance(e, WebSocketConnectionClosedException):
                     self.logger.error("Lost websocket connection")
                 elif isinstance(e, WebSocketTimeoutException):
                     self.logger.error("Websocket connection timeout")
                 else:
                     self.logger.error("Websocket exception: {}".format(e))
-                raise e
+                self._handle_exception(e)
+                break
             except Exception as e:
                 self.logger.error("Exception in read_data: {}".format(e))
-                raise e
+                self._handle_exception(e)
+                break
 
             self._handle_data(op_code, frame, data)
             self._handle_heartbeat(op_code, frame)
 
             if op_code == ABNF.OPCODE_CLOSE:
                 self.logger.warning(
                     "CLOSE frame received, closing websocket connection"
@@ -108,17 +110,21 @@
             self._callback(self.on_message, data)
 
     def close(self):
         if not self.ws.connected:
             self.logger.warning("Websocket already closed")
         else:
             self.ws.send_close()
-        return
 
     def _callback(self, callback, *args):
         if callback:
             try:
                 callback(self, *args)
             except Exception as e:
                 self.logger.error("Error from callback {}: {}".format(callback, e))
-                if self.on_error:
-                    self.on_error(self, e)
+                self._handle_exception(e)
+
+    def _handle_exception(self, e):
+        if self.on_error:
+            self.on_error(self, e)
+        else:
+            raise e
```

### Comparing `binance-connector-3.6.0/binance/websocket/spot/websocket_api/__init__.py` & `binance-connector-3.7.0/binance/websocket/spot/websocket_api/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/websocket/spot/websocket_api/_account.py` & `binance-connector-3.7.0/binance/websocket/spot/websocket_api/_account.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/websocket/spot/websocket_api/_market.py` & `binance-connector-3.7.0/binance/websocket/spot/websocket_api/_market.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,19 @@
     parameters = purge_map(parameters)
 
     if len(parameters) > 1:
         raise ParameterArgumentError(
             "Only one of symbol, symbols or permissions is required."
         )
 
-    payload = {"id": parameters.pop("id", get_uuid()), "method": "exchangeInfo"}
+    payload = {
+        "id": parameters.pop("id", get_uuid()),
+        "method": "exchangeInfo",
+        "params": parameters,
+    }
 
     self.send(payload)
 
 
 def order_book(self, symbol: str, **kwargs):
     """Order book
```

### Comparing `binance-connector-3.6.0/binance/websocket/spot/websocket_api/_trade.py` & `binance-connector-3.7.0/binance/websocket/spot/websocket_api/_trade.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/websocket/spot/websocket_api/_user_data.py` & `binance-connector-3.7.0/binance/websocket/spot/websocket_api/_user_data.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/websocket/spot/websocket_stream.py` & `binance-connector-3.7.0/binance/websocket/spot/websocket_stream.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance/websocket/websocket_client.py` & `binance-connector-3.7.0/binance/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.6.0/binance_connector.egg-info/PKG-INFO` & `binance-connector-3.7.0/binance_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-connector
-Version: 3.6.0
+Version: 3.7.0
 Summary: This is a lightweight library that works as a connector to Binance public API.
 Home-page: https://github.com/binance/binance-connector-python
 License: MIT
 Keywords: Binance,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binance-connector-3.6.0/binance_connector.egg-info/SOURCES.txt` & `binance-connector-3.7.0/binance_connector.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 binance/lib/__init__.py
 binance/lib/authentication.py
 binance/lib/enums.py
 binance/lib/utils.py
 binance/spot/__init__.py
 binance/spot/_auto_invest.py
 binance/spot/_blvt.py
-binance/spot/_bswap.py
 binance/spot/_c2c.py
 binance/spot/_convert.py
 binance/spot/_crypto_loan.py
 binance/spot/_data_stream.py
 binance/spot/_fiat.py
 binance/spot/_futures.py
 binance/spot/_gift_card.py
@@ -26,15 +25,14 @@
 binance/spot/_market.py
 binance/spot/_mining.py
 binance/spot/_nft.py
 binance/spot/_pay.py
 binance/spot/_portfolio_margin.py
 binance/spot/_rebate.py
 binance/spot/_simple_earn.py
-binance/spot/_staking.py
 binance/spot/_sub_account.py
 binance/spot/_trade.py
 binance/spot/_wallet.py
 binance/websocket/__init__.py
 binance/websocket/binance_socket_manager.py
 binance/websocket/websocket_client.py
 binance/websocket/spot/__init__.py
```

### Comparing `binance-connector-3.6.0/setup.py` & `binance-connector-3.7.0/setup.py`

 * *Files identical despite different names*


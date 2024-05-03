# Comparing `tmp/ttxt-0.0.6.1.tar.gz` & `tmp/ttxt-0.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttxt-0.0.6.1.tar", last modified: Wed May  1 15:59:51 2024, max compression
+gzip compressed data, was "ttxt-0.0.6.2.tar", last modified: Fri May  3 15:41:14 2024, max compression
```

## Comparing `ttxt-0.0.6.1.tar` & `ttxt-0.0.6.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.365886 ttxt-0.0.6.1/
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.6.1/LICENSE
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-01 15:59:51.365739 ttxt-0.0.6.1/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.6.1/README.md
--rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-05-01 15:59:51.365930 ttxt-0.0.6.1/setup.cfg
--rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-05-01 15:59:41.000000 ttxt-0.0.6.1/setup.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.355712 ttxt-0.0.6.1/ttxt/
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1040 2024-04-20 13:49:26.000000 ttxt-0.0.6.1/ttxt/__init__.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.356713 ttxt-0.0.6.1/ttxt/base/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.6.1/ttxt/base/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.6.1/ttxt/base/baseFuturesExchange.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.6.1/ttxt/base/baseSpotExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.363596 ttxt-0.0.6.1/ttxt/exchanges/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.6.1/ttxt/exchanges/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.6.1/ttxt/exchanges/biconomy.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.6.1/ttxt/exchanges/binance.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.6.1/ttxt/exchanges/bingx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.6.1/ttxt/exchanges/bitget.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.6.1/ttxt/exchanges/bitgetFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.6.1/ttxt/exchanges/bitmart.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    21581 2024-05-01 15:58:33.000000 ttxt-0.0.6.1/ttxt/exchanges/bybit.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.6.1/ttxt/exchanges/bybitFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.6.1/ttxt/exchanges/cryptocom.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.6.1/ttxt/exchanges/gateFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    15302 2024-03-22 17:13:33.000000 ttxt-0.0.6.1/ttxt/exchanges/gateio.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.6.1/ttxt/exchanges/huobi.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.6.1/ttxt/exchanges/kucoin.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.6.1/ttxt/exchanges/mexc.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11747 2024-04-05 05:36:24.000000 ttxt-0.0.6.1/ttxt/exchanges/okx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.6.1/ttxt/exchanges/xt.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.363800 ttxt-0.0.6.1/ttxt/tests/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.6.1/ttxt/tests/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    10063 2024-05-01 15:36:07.000000 ttxt-0.0.6.1/ttxt/tests/testExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.364293 ttxt-0.0.6.1/ttxt/types/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.6.1/ttxt/types/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.6.1/ttxt/types/baseTypes.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.364950 ttxt-0.0.6.1/ttxt/utils/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.6.1/ttxt/utils/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.6.1/ttxt/utils/general.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.6.1/ttxt/utils/xtUtils.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.356260 ttxt-0.0.6.1/ttxt.egg-info/
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-01 15:59:51.000000 ttxt-0.0.6.1/ttxt.egg-info/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)      844 2024-05-01 15:59:51.000000 ttxt-0.0.6.1/ttxt.egg-info/SOURCES.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-05-01 15:59:51.000000 ttxt-0.0.6.1/ttxt.egg-info/dependency_links.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-05-01 15:59:51.000000 ttxt-0.0.6.1/ttxt.egg-info/top_level.txt
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.864548 ttxt-0.0.6.2/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.6.2/LICENSE
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-03 15:41:14.864437 ttxt-0.0.6.2/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.6.2/README.md
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-05-03 15:41:14.864600 ttxt-0.0.6.2/setup.cfg
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-05-03 15:40:39.000000 ttxt-0.0.6.2/setup.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.854431 ttxt-0.0.6.2/ttxt/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1101 2024-05-03 15:38:46.000000 ttxt-0.0.6.2/ttxt/__init__.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.855608 ttxt-0.0.6.2/ttxt/base/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.6.2/ttxt/base/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.6.2/ttxt/base/baseFuturesExchange.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.6.2/ttxt/base/baseSpotExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.862036 ttxt-0.0.6.2/ttxt/exchanges/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.6.2/ttxt/exchanges/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11341 2024-05-03 15:38:46.000000 ttxt-0.0.6.2/ttxt/exchanges/ascendex.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.6.2/ttxt/exchanges/biconomy.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.6.2/ttxt/exchanges/binance.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.6.2/ttxt/exchanges/bingx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.6.2/ttxt/exchanges/bitget.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.6.2/ttxt/exchanges/bitgetFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.6.2/ttxt/exchanges/bitmart.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    21199 2024-05-02 08:57:55.000000 ttxt-0.0.6.2/ttxt/exchanges/bybit.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.6.2/ttxt/exchanges/bybitFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.6.2/ttxt/exchanges/cryptocom.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.6.2/ttxt/exchanges/gateFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    15302 2024-03-22 17:13:33.000000 ttxt-0.0.6.2/ttxt/exchanges/gateio.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.6.2/ttxt/exchanges/huobi.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.6.2/ttxt/exchanges/kucoin.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.6.2/ttxt/exchanges/mexc.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11747 2024-04-05 05:36:24.000000 ttxt-0.0.6.2/ttxt/exchanges/okx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.6.2/ttxt/exchanges/xt.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.862211 ttxt-0.0.6.2/ttxt/tests/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.6.2/ttxt/tests/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    10231 2024-05-03 15:38:46.000000 ttxt-0.0.6.2/ttxt/tests/testExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.862534 ttxt-0.0.6.2/ttxt/types/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.6.2/ttxt/types/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.6.2/ttxt/types/baseTypes.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.863424 ttxt-0.0.6.2/ttxt/utils/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.6.2/ttxt/utils/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.6.2/ttxt/utils/general.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.6.2/ttxt/utils/xtUtils.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.855051 ttxt-0.0.6.2/ttxt.egg-info/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-03 15:41:14.000000 ttxt-0.0.6.2/ttxt.egg-info/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      871 2024-05-03 15:41:14.000000 ttxt-0.0.6.2/ttxt.egg-info/SOURCES.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-05-03 15:41:14.000000 ttxt-0.0.6.2/ttxt.egg-info/dependency_links.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-05-03 15:41:14.000000 ttxt-0.0.6.2/ttxt.egg-info/top_level.txt
```

### Comparing `ttxt-0.0.6.1/LICENSE` & `ttxt-0.0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/__init__.py` & `ttxt-0.0.6.2/ttxt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ttxt.base import baseFuturesExchange, baseSpotExchange
+from ttxt.exchanges.ascendex import ascendex
 from ttxt.exchanges.gateFutures import gateFutures
 from ttxt.exchanges.bybitFutures import bybitFutures
 from ttxt.exchanges.bitgetFutures import bitgetFutures
 from ttxt.exchanges.bingx import bingx
 from ttxt.exchanges.biconomy import biconomy
 from ttxt.exchanges.mexc import mexc
 from ttxt.exchanges.gateio import gateio
@@ -12,14 +13,15 @@
 from ttxt.exchanges.bitmart import bitmart
 from ttxt.exchanges.cryptocom import cryptocom
 from ttxt.exchanges.bitget import bitget
 from ttxt.exchanges.binance import binance
 from ttxt.exchanges.kucoin import kucoin
 
 exchanges = [
+    "ascendex",
     "biconomy",
     "binance",
     "bingx",
     "bitgetFutures",
     "bitget",
     "bybitFutures",
     "gateFutures",
```

### Comparing `ttxt-0.0.6.1/ttxt/base/baseFuturesExchange.py` & `ttxt-0.0.6.2/ttxt/base/baseFuturesExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/base/baseSpotExchange.py` & `ttxt-0.0.6.2/ttxt/base/baseSpotExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/biconomy.py` & `ttxt-0.0.6.2/ttxt/exchanges/biconomy.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/binance.py` & `ttxt-0.0.6.2/ttxt/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/bingx.py` & `ttxt-0.0.6.2/ttxt/exchanges/bingx.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/bitget.py` & `ttxt-0.0.6.2/ttxt/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/bitgetFutures.py` & `ttxt-0.0.6.2/ttxt/exchanges/bitgetFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/bitmart.py` & `ttxt-0.0.6.2/ttxt/exchanges/bitmart.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/bybit.py` & `ttxt-0.0.6.2/ttxt/exchanges/bybit.py`

 * *Files 2% similar despite different names*

```diff
@@ -480,22 +480,14 @@
                 apiUrl = "/v5/asset/transfer/query-account-coins-balance"
             elif accountInfo['marginMode'] != 'REGULAR_MARGIN':
                 apiUrl = "/v5/spot-cross-margin-trade/account"
             else:
                 apiUrl = '/v5/account/wallet-balance'
             resp = self._signedRequest(method='GET', path=apiUrl, query=queryParams, auth=True)
             return self._parseBalance(resp)
-        except WrongAccountType as e:
-            apiUrl = "/v5/asset/transfer/query-account-coins-balance"
-            queryParams = {"accountType": "SPOT"}
-            try:
-                resp = self._signedRequest(method='GET', path=apiUrl, query=queryParams, auth=True)
-                return self._parseBalance(resp)
-            except Exception as e:
-                raise e
         except Exception as e:
             raise e
     
     def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}):
         apiUrl = '/v5/execution/list'
         queryParams = {"category": self.category}
         if symbol:
```

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/bybitFutures.py` & `ttxt-0.0.6.2/ttxt/exchanges/bybitFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/cryptocom.py` & `ttxt-0.0.6.2/ttxt/exchanges/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/gateFutures.py` & `ttxt-0.0.6.2/ttxt/exchanges/gateFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/gateio.py` & `ttxt-0.0.6.2/ttxt/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/huobi.py` & `ttxt-0.0.6.2/ttxt/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/kucoin.py` & `ttxt-0.0.6.2/ttxt/exchanges/kucoin.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/mexc.py` & `ttxt-0.0.6.2/ttxt/exchanges/mexc.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/exchanges/okx.py` & `ttxt-0.0.6.2/ttxt/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/tests/testExchange.py` & `ttxt-0.0.6.2/ttxt/tests/testExchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 DIR_NAME = os.path.dirname(os.path.abspath(__file__))
 root = os.path.dirname(os.path.dirname(DIR_NAME))
 sys.path.append(root)
 
 import ttxt
 
 def getTtxtExchange(exchangeName):
+    if exchangeName == "ascendex":
+        print('returned ascendex')
+        return ttxt.ascendex(key=os.getenv("KEY"), secret=os.getenv("SECRET"), password=os.getenv("PASSWORD"))
     if exchangeName == "gateFutures":
         print("returned gateFuture")
         return ttxt.gateFutures(key=os.getenv("KEY"), secret=os.getenv("SECRET"))
     if exchangeName == "bybitFutures":
         print("returned bybitFutures")
         return ttxt.bybitFutures(key=os.getenv("KEY"), secret=os.getenv("SECRET"))
     if exchangeName == "bitgetFutures":
@@ -78,24 +81,23 @@
             print(resp)
         except Exception as e:
             print("balance could not be fetched")
             print(e)
     if "createOrder" in params and params["createOrder"]:
         print("testing create order...")
         try:
-            resp = ttxtExchange.create_order(symbol=tickerToTest, order_type="limit", amount="5", side="sell", price=5)
+            resp = ttxtExchange.create_order(symbol=tickerToTest, order_type="market", amount="50", side="sell", price=0.3)
             print(f"createOrder response: {resp}")
         except Exception as e:
             print("order could not be created")
             print(e)
     if "createLimitOrder" in params and params["createLimitOrder"]:
         print("testing limit create order...")
         try:
-            params = {'timeInForce': 'PostOnly'}
-            resp = ttxtExchange.create_limit_order(symbol=tickerToTest, amount=100, side="buy", price=0.0494, params=params)
+            resp = ttxtExchange.create_limit_order(symbol=tickerToTest, amount=50, side="buy", price=0.2)
             print(f"createLimitOrder response: {resp}")
         except Exception as e:
             print("limit order could not be created")
             print(e)
     if "createMarketSellOrder" in params and params["createMarketSellOrder"]:
         print("testing market sell create order...")
         try:
@@ -111,31 +113,31 @@
             print(f"createMarketBuyOrder response: {resp}")
         except Exception as e:
             print("market buy order could not be created")
             print(e)
     if "create_market_order" in params and params["create_market_order"]:
         print("testing create market order...")
         try:
-            resp = ttxtExchange.create_market_order(symbol=tickerToTest, side="sell", amount=1)
+            resp = ttxtExchange.create_market_order(symbol=tickerToTest, side="sell", amount=50)
             print(f"create_market_order response: {resp}")
         except Exception as e:
             print("market order could not be created")
             print(e)
     if "fetchOrder" in params and params["fetchOrder"]:
         print("testing fetch order...")
         try:
-            resp = ttxtExchange.fetch_order(id=45577069671, symbol=tickerToTest)
+            resp = ttxtExchange.fetch_order(id="a18eae908f85U3317077942fPhjnp6nH", symbol=tickerToTest)
             print(f"fetchOrder response: {resp}")
         except Exception as e:
             print("order could not be fetched")
             print(e)
     if "cancelOrder" in params and params["cancelOrder"]:
         print("testing cancel order...")
         try:
-            resp = ttxtExchange.cancel_order(id=698922787, symbol=tickerToTest)
+            resp = ttxtExchange.cancel_order(id="a18eaf2a165cU3317077942BKbakNWlN", symbol=tickerToTest)
             print(f"cancelOrder response: {resp}")
         except Exception as e:
             print("order could not be canceled")
             print(e)
     if "fetchOpenOrders" in params and params["fetchOpenOrders"]:
         print("testing open orders...")
         try:
@@ -204,17 +206,17 @@
             print(resp)
         except Exception as e:
             print("account info could not be fetched")
             print(e)
 
 
 if __name__ == "__main__":
-    tickerToTest = "GALA/USDT"
+    tickerToTest = "OPUL/USDT"
     testingParams = {"ticker": False, 
-                     "balance": True, 
+                     "balance": False, 
                      "ohlcv": False, 
                      "createOrder": False, 
                      "fetchOrder": False, 
                      "cancelOrder": False, 
                      "fetchOpenOrders": False, 
                      "setLeverage": False, 
                      "createLimitOrder": False,
@@ -222,8 +224,8 @@
                      "createMarketBuyOrder": False, 
                      "orderbook": False, 
                      "candlestick": False,
                      "create_market_order": False, 
                      "cancelAllOrders": False, 
                      "myTrades": False,
                      "accountInfo": False}
-    test(params=testingParams, exchangeName="bybit")
+    test(params=testingParams, exchangeName="bybit")
```

### Comparing `ttxt-0.0.6.1/ttxt/types/baseTypes.py` & `ttxt-0.0.6.2/ttxt/types/baseTypes.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/utils/general.py` & `ttxt-0.0.6.2/ttxt/utils/general.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt/utils/xtUtils.py` & `ttxt-0.0.6.2/ttxt/utils/xtUtils.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.1/ttxt.egg-info/SOURCES.txt` & `ttxt-0.0.6.2/ttxt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ttxt.egg-info/SOURCES.txt
 ttxt.egg-info/dependency_links.txt
 ttxt.egg-info/top_level.txt
 ttxt/base/__init__.py
 ttxt/base/baseFuturesExchange.py
 ttxt/base/baseSpotExchange.py
 ttxt/exchanges/__init__.py
+ttxt/exchanges/ascendex.py
 ttxt/exchanges/biconomy.py
 ttxt/exchanges/binance.py
 ttxt/exchanges/bingx.py
 ttxt/exchanges/bitget.py
 ttxt/exchanges/bitgetFutures.py
 ttxt/exchanges/bitmart.py
 ttxt/exchanges/bybit.py
```


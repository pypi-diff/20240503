# Comparing `tmp/trio_binance-0.3.2.tar.gz` & `tmp/trio_binance-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trio_binance-0.3.2.tar", max compression
+gzip compressed data, was "trio_binance-0.3.3.tar", max compression
```

## Comparing `trio_binance-0.3.2.tar` & `trio_binance-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio_binance-0.3.2/LICENSE
--rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.000000 trio_binance-0.3.2/README.rst
--rw-r--r--   0        0        0     1055 2024-04-23 09:30:58.022220 trio_binance-0.3.2/pyproject.toml
--rwxr-xr-x   0        0        0       67 2024-04-23 09:30:58.019462 trio_binance-0.3.2/trio_binance/__init__.py
--rwxr-xr-x   0        0        0    78447 2024-04-23 09:30:39.726507 trio_binance-0.3.2/trio_binance/client.py
--rw-r--r--   0        0        0     1891 2024-04-23 01:56:20.850456 trio_binance-0.3.2/trio_binance/enums.py
--rw-r--r--   0        0        0     2260 2024-04-23 02:07:31.211547 trio_binance-0.3.2/trio_binance/exceptions.py
--rw-r--r--   0        0        0     1493 2024-04-23 02:07:31.211671 trio_binance-0.3.2/trio_binance/helpers.py
--rw-r--r--   0        0        0     3780 2024-04-23 05:34:24.595456 trio_binance-0.3.2/trio_binance/streams.py
--rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 trio_binance-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio_binance-0.3.3/LICENSE
+-rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.000000 trio_binance-0.3.3/README.rst
+-rw-r--r--   0        0        0     1055 2024-05-03 01:53:52.093160 trio_binance-0.3.3/pyproject.toml
+-rwxr-xr-x   0        0        0       67 2024-05-03 01:53:47.150389 trio_binance-0.3.3/trio_binance/__init__.py
+-rwxr-xr-x   0        0        0    78460 2024-05-03 01:52:58.369872 trio_binance-0.3.3/trio_binance/client.py
+-rw-r--r--   0        0        0     1891 2024-04-23 01:56:20.850456 trio_binance-0.3.3/trio_binance/enums.py
+-rw-r--r--   0        0        0     2260 2024-04-23 02:07:31.211547 trio_binance-0.3.3/trio_binance/exceptions.py
+-rw-r--r--   0        0        0     1493 2024-04-23 02:07:31.211671 trio_binance-0.3.3/trio_binance/helpers.py
+-rw-r--r--   0        0        0     3780 2024-04-23 05:34:24.595456 trio_binance-0.3.3/trio_binance/streams.py
+-rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 trio_binance-0.3.3/PKG-INFO
```

### Comparing `trio_binance-0.3.2/LICENSE` & `trio_binance-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.2/README.rst` & `trio_binance-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.2/pyproject.toml` & `trio_binance-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trio-binance"
-version = "0.3.2"
+version = "0.3.3"
 description = "trio based asynchronous binance SDK"
 authors = ["Shu Wang <halfelf.ronin@gmail.com>"]
 keywords = ["binance", "python-trio"]
 readme = "README.rst"
 license = "MIT"
 homepage = "https://github.com/halfelf/trio-binance"
 repository = "https://github.com/halfelf/trio-binance"
```

### Comparing `trio_binance-0.3.2/trio_binance/client.py` & `trio_binance-0.3.3/trio_binance/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -950,15 +950,15 @@
     async def futures_time(self):
         return await self._request_futures_api("get", "time")
 
     async def futures_exchange_info(self):
         return await self._request_futures_api("get", "exchangeInfo")
 
     async def futures_get_symbol_info(self, symbol) -> Optional[Dict]:
-        res = await self.get_exchange_info()
+        res = await self.futures_exchange_info()
 
         for item in res["symbols"]:
             if item["symbol"] == symbol.upper():
                 return item
 
         return None
 
@@ -1140,15 +1140,15 @@
     async def futures_coin_time(self):
         return await self._request_futures_coin_api("get", "time")
 
     async def futures_coin_exchange_info(self):
         return await self._request_futures_coin_api("get", "exchangeInfo")
 
     async def futures_coin_get_symbol_info(self, symbol) -> Optional[Dict]:
-        res = await self.get_exchange_info()
+        res = await self.futures_coin_exchange_info()
 
         for item in res["symbols"]:
             if item["symbol"] == symbol.upper():
                 return item
 
         return None
```

### Comparing `trio_binance-0.3.2/trio_binance/enums.py` & `trio_binance-0.3.3/trio_binance/enums.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.2/trio_binance/exceptions.py` & `trio_binance-0.3.3/trio_binance/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.2/trio_binance/helpers.py` & `trio_binance-0.3.3/trio_binance/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.2/trio_binance/streams.py` & `trio_binance-0.3.3/trio_binance/streams.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.2/PKG-INFO` & `trio_binance-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trio-binance
-Version: 0.3.2
+Version: 0.3.3
 Summary: trio based asynchronous binance SDK
 Home-page: https://github.com/halfelf/trio-binance
 License: MIT
 Keywords: binance,python-trio
 Author: Shu Wang
 Author-email: halfelf.ronin@gmail.com
 Requires-Python: >=3.11,<4.0
```


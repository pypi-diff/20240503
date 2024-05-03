# Comparing `tmp/ithaca_py-0.2.4.tar.gz` & `tmp/ithaca_py-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ithaca_py-0.2.4.tar", max compression
+gzip compressed data, was "ithaca_py-0.2.5.tar", max compression
```

## Comparing `ithaca_py-0.2.4.tar` & `ithaca_py-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      983 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/README.md
--rw-r--r--   0        0        0     5147 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/ithaca/__init__.py
--rw-r--r--   0        0        0     3656 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/ithaca/analytics.py
--rw-r--r--   0        0        0    10809 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/ithaca/auth.py
--rw-r--r--   0        0        0     5589 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/ithaca/calculation.py
--rw-r--r--   0        0        0     3206 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/ithaca/client.py
--rw-r--r--   0        0        0     1846 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/ithaca/constants.py
--rw-r--r--   0        0        0    12592 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/ithaca/fundlock.py
--rw-r--r--   0        0        0      603 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/ithaca/market.py
--rw-r--r--   0        0        0     7370 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/ithaca/orders.py
--rw-r--r--   0        0        0     1373 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/ithaca/protocol.py
--rw-r--r--   0        0        0     2406 2024-04-24 10:14:55.019061 ithaca_py-0.2.4/ithaca/socket.py
--rw-r--r--   0        0        0      929 2024-04-24 10:14:55.023061 ithaca_py-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      983 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/README.md
+-rw-r--r--   0        0        0     5147 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/ithaca/__init__.py
+-rw-r--r--   0        0        0     3870 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/ithaca/analytics.py
+-rw-r--r--   0        0        0    10809 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/ithaca/auth.py
+-rw-r--r--   0        0        0     5589 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/ithaca/calculation.py
+-rw-r--r--   0        0        0     3324 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/ithaca/client.py
+-rw-r--r--   0        0        0     1846 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/ithaca/constants.py
+-rw-r--r--   0        0        0    12592 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/ithaca/fundlock.py
+-rw-r--r--   0        0        0      603 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/ithaca/market.py
+-rw-r--r--   0        0        0     7370 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/ithaca/orders.py
+-rw-r--r--   0        0        0     1373 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/ithaca/protocol.py
+-rw-r--r--   0        0        0     2406 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/ithaca/socket.py
+-rw-r--r--   0        0        0      929 2024-05-03 01:29:03.775191 ithaca_py-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.5/PKG-INFO
```

### Comparing `ithaca_py-0.2.4/README.md` & `ithaca_py-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.4/ithaca/__init__.py` & `ithaca_py-0.2.5/ithaca/__init__.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.4/ithaca/analytics.py` & `ithaca_py-0.2.5/ithaca/analytics.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,21 @@
     def best_prices(self):
         """Get best bid and best ask in order list.
 
         POST  api/v1/clientapi/bestBidAsk
         """
         return self.parent.post("/clientapi/bestBidAsk")
 
+    def best_prices_precise(self):
+        """Get best bid and best ask in order list.
+
+        POST  api/v1/clientapi/bestBidAskPrecise
+        """
+        return self.parent.post("/clientapi/bestBidAskPrecise")
+
     def total_trading_volume(self):
         """Get total trading volume.
 
         GET  api/v1/analytics/{underlier}/{numeraire}/totalTradingVolume
         """
         return self.parent.get("/analytics/WETH/USDC/totalTradingVolume")
```

### Comparing `ithaca_py-0.2.4/ithaca/auth.py` & `ithaca_py-0.2.5/ithaca/auth.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.4/ithaca/calculation.py` & `ithaca_py-0.2.5/ithaca/calculation.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.4/ithaca/client.py` & `ithaca_py-0.2.5/ithaca/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,22 @@
         """Get client fundlock state.
 
         Returns:
             _type_: _description_
         """
         return self.parent.post("/clientapi/clientFundLockState")
 
+    def positions_lock_state(self):
+        """Get client locked positions collateral.
+
+        Returns:
+            _type_: _description_
+        """
+        return self.parent.post("/clientapi/getLockedCollateral")
+
     def current_positions(self, _filter=None, details=False):
         """Return a list of the clients positions.
 
         Args:
             filter (_type_, opt.): COMBINE_STRATEGIES | SHOW_ORDERS.
             details (bool, opt.): If True, returns a DF with contract details.
 
@@ -45,28 +53,24 @@
                 )
             ).set_index("contractId")
             return (
                 pd.DataFrame(res.get("payload")).set_index("contractId").join(contracts)
             )
         return res
 
-    def trade_history(self,
-                      date_from: int = None,
-                      date_to: int = None,
-                      offset: int = None,
-                      limit: int = None):
-
+    def trade_history(
+        self,
+        date_from: int = None,
+        date_to: int = None,
+        offset: int = None,
+        limit: int = None,
+    ):
         """Get trade history."""
         """date_from/to are timestamps in backend"""
-        body = {
-            "from": date_from,
-            "to": date_to,
-            "offset": offset,
-            "limit": limit
-        }
+        body = {"from": date_from, "to": date_to, "offset": offset, "limit": limit}
         if date_from or date_to or offset or limit:
             return self.parent.post("/clientapi/tradeHistory", json=body)
         else:
             return self.parent.post("/clientapi/tradeHistory")
 
     def historical_positions(self, expiry):
         """Get client historical positions."""
```

### Comparing `ithaca_py-0.2.4/ithaca/constants.py` & `ithaca_py-0.2.5/ithaca/constants.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.4/ithaca/fundlock.py` & `ithaca_py-0.2.5/ithaca/fundlock.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.4/ithaca/market.py` & `ithaca_py-0.2.5/ithaca/market.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.4/ithaca/orders.py` & `ithaca_py-0.2.5/ithaca/orders.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.4/ithaca/protocol.py` & `ithaca_py-0.2.5/ithaca/protocol.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.4/ithaca/socket.py` & `ithaca_py-0.2.5/ithaca/socket.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.4/pyproject.toml` & `ithaca_py-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ithaca_py"
-version = "0.2.4"
+version = "0.2.5"
 description = "Ithaca Protocol SDK"
 authors = ["nhaga <nhaga5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ithaca"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ithaca_py-0.2.4/PKG-INFO` & `ithaca_py-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ithaca_py
-Version: 0.2.4
+Version: 0.2.5
 Summary: Ithaca Protocol SDK
 Author: nhaga
 Author-email: nhaga5@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


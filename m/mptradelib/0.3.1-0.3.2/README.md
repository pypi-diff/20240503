# Comparing `tmp/mptradelib-0.3.1.tar.gz` & `tmp/mptradelib-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.3.1.tar", max compression
+gzip compressed data, was "mptradelib-0.3.2.tar", max compression
```

## Comparing `mptradelib-0.3.1.tar` & `mptradelib-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.1/mptradelib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.1/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.1/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.1/mptradelib/broker/session.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.1/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0     3889 2024-05-02 08:04:37.700859 mptradelib-0.3.1/mptradelib/feed.py
--rw-r--r--   0        0        0     1866 2024-05-02 08:01:45.468179 mptradelib-0.3.1/mptradelib/livetrading.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.1/mptradelib/shoonya.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.1/mptradelib/test_renko.py
--rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.3.1/mptradelib/utils.py
--rw-r--r--   0        0        0     4193 2024-05-02 14:00:12.492668 mptradelib-0.3.1/mptradelib/vectorised_backtest.py
--rw-r--r--   0        0        0      561 2024-05-02 14:00:55.094148 mptradelib-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.2/mptradelib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.2/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.2/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.2/mptradelib/broker/session.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.2/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0     4054 2024-05-03 03:52:00.848935 mptradelib-0.3.2/mptradelib/feed.py
+-rw-r--r--   0        0        0     1866 2024-05-02 08:01:45.468179 mptradelib-0.3.2/mptradelib/livetrading.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.2/mptradelib/shoonya.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.2/mptradelib/test_renko.py
+-rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.3.2/mptradelib/utils.py
+-rw-r--r--   0        0        0     4193 2024-05-02 14:00:12.492668 mptradelib-0.3.2/mptradelib/vectorised_backtest.py
+-rw-r--r--   0        0        0      561 2024-05-03 03:52:20.749789 mptradelib-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.3.2/PKG-INFO
```

### Comparing `mptradelib-0.3.1/README.md` & `mptradelib-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.1/mptradelib/broker/broker.py` & `mptradelib-0.3.2/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.1/mptradelib/broker/session.py` & `mptradelib-0.3.2/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.1/mptradelib/broker/ticker.py` & `mptradelib-0.3.2/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.1/mptradelib/feed.py` & `mptradelib-0.3.2/mptradelib/feed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import redis
 import json
 import threading
 import datetime as dt
 import pandas as pd
 from pydantic import BaseModel, Field
 from collections import OrderedDict
@@ -40,22 +41,28 @@
 
     @property
     def df(self):
         return pd.DataFrame(list(self))
 
 class Datas:
     _datas: dict = {}
+    _resample_period = 1
 
-    def __init__(self, r: redis.Redis, h: Historical, resample_period: int = 1) -> None:
+    def __init__(self, r: redis.Redis, h: Historical) -> None:
         self._r = r
-        self._resample_period = resample_period
         self._h = h
 
+    def resample(self, period=1):
+        self._resample_period = period
+        return self
+
     def _generate_key(self, a: dt.datetime):
-        return f"{a:%Y-%m-%d-%H-%M}"
+        b = copy.copy(a)
+        c = b - dt.timedelta(minutes=(b.minute % self._resample_period))
+        return f"{c:%Y-%m-%d-%H-%M}"
     
     def symbols(self):
         return self._datas.keys()
 
     def update(self, tick: Tick):
         key = self._generate_key(tick.datetime)
 
@@ -77,15 +84,15 @@
     def _load_worker(self, symbol: str, start_date: dt.datetime, end_date: dt.datetime):
         try:
             series = self._datas[symbol]
         except KeyError:
             self._datas[symbol] = OrderedDict()
             series = self._datas[symbol]
 
-        data = self._h.historical(symbol, 1, start_date, end_date)
+        data = self._h.historical(symbol, self._resample_period, start_date, end_date)
         for d in data.to_dict('records'):
             c = Candle.model_validate(d)
             key = self._generate_key(c.datetime)
             series[key] = c.model_dump()
 
     def load(self, symbols: List[str], period=7):
         end_date = dt.datetime.now()
@@ -119,9 +126,7 @@
                 on_message(tick)
             except Exception as e:
                 print(e)
 
     def run(self, channel, on_message: Callable[[Tick],None]):
         t = threading.Thread(target=self._listen, args=[channel, on_message])
         t.start()
-        
-
```

### Comparing `mptradelib-0.3.1/mptradelib/livetrading.py` & `mptradelib-0.3.2/mptradelib/livetrading.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.1/mptradelib/shoonya.py` & `mptradelib-0.3.2/mptradelib/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.1/mptradelib/test_renko.py` & `mptradelib-0.3.2/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.1/mptradelib/utils.py` & `mptradelib-0.3.2/mptradelib/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.1/mptradelib/vectorised_backtest.py` & `mptradelib-0.3.2/mptradelib/vectorised_backtest.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.1/pyproject.toml` & `mptradelib-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.3.1/PKG-INFO` & `mptradelib-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


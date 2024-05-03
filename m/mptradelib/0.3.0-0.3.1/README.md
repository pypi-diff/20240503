# Comparing `tmp/mptradelib-0.3.0.tar.gz` & `tmp/mptradelib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.3.0.tar", max compression
+gzip compressed data, was "mptradelib-0.3.1.tar", max compression
```

## Comparing `mptradelib-0.3.0.tar` & `mptradelib-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.0/mptradelib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.0/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.0/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.0/mptradelib/broker/session.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.0/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0     3889 2024-05-02 08:04:37.700859 mptradelib-0.3.0/mptradelib/feed.py
--rw-r--r--   0        0        0     1866 2024-05-02 08:01:45.468179 mptradelib-0.3.0/mptradelib/livetrading.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.0/mptradelib/shoonya.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.0/mptradelib/test_renko.py
--rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.3.0/mptradelib/utils.py
--rw-r--r--   0        0        0     4162 2024-04-30 11:43:56.632362 mptradelib-0.3.0/mptradelib/vectorised_backtest.py
--rw-r--r--   0        0        0      561 2024-05-02 08:05:22.046511 mptradelib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.1/mptradelib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.1/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.1/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.1/mptradelib/broker/session.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.1/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0     3889 2024-05-02 08:04:37.700859 mptradelib-0.3.1/mptradelib/feed.py
+-rw-r--r--   0        0        0     1866 2024-05-02 08:01:45.468179 mptradelib-0.3.1/mptradelib/livetrading.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.1/mptradelib/shoonya.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.1/mptradelib/test_renko.py
+-rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.3.1/mptradelib/utils.py
+-rw-r--r--   0        0        0     4193 2024-05-02 14:00:12.492668 mptradelib-0.3.1/mptradelib/vectorised_backtest.py
+-rw-r--r--   0        0        0      561 2024-05-02 14:00:55.094148 mptradelib-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.3.1/PKG-INFO
```

### Comparing `mptradelib-0.3.0/README.md` & `mptradelib-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.0/mptradelib/broker/broker.py` & `mptradelib-0.3.1/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.0/mptradelib/broker/session.py` & `mptradelib-0.3.1/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.0/mptradelib/broker/ticker.py` & `mptradelib-0.3.1/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.0/mptradelib/feed.py` & `mptradelib-0.3.1/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.0/mptradelib/livetrading.py` & `mptradelib-0.3.1/mptradelib/livetrading.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.0/mptradelib/shoonya.py` & `mptradelib-0.3.1/mptradelib/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.0/mptradelib/test_renko.py` & `mptradelib-0.3.1/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.0/mptradelib/utils.py` & `mptradelib-0.3.1/mptradelib/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.0/mptradelib/vectorised_backtest.py` & `mptradelib-0.3.1/mptradelib/vectorised_backtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         data['exit_price'] = data.open.shift(-1)
         data['trade_time'] = data.datetime.shift(-1)
 
         for row in data.itertuples():
             self._backtest(row)
         out_df = pd.DataFrame([asdict(o) for o in self.__orders])
         self.__orders = []
+        self.__position = None
         return out_df, data
 
     def _exit_position(self, row):
         self.__position.exit_price = row.exit_price
         self.__position.exit_time = row.trade_time
         self.__position.set_profit()
         self.__orders.append(self.__position)
```

### Comparing `mptradelib-0.3.0/pyproject.toml` & `mptradelib-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.3.0/PKG-INFO` & `mptradelib-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


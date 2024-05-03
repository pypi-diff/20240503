# Comparing `tmp/pyc3l-0.1.1.tar.gz` & `tmp/pyc3l-0.2.0.tar.gz`

## Comparing `pyc3l-0.1.1.tar` & `pyc3l-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyc3l-0.1.1/_version.py
--rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 pyc3l-0.1.1/src/pyc3l/ApiCommunication.py
--rw-r--r--   0        0        0    14372 2020-02-02 00:00:00.000000 pyc3l-0.1.1/src/pyc3l/ApiHandling.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pyc3l-0.1.1/src/pyc3l/CryptoAsim.py
--rw-r--r--   0        0        0    10126 2020-02-02 00:00:00.000000 pyc3l-0.1.1/src/pyc3l/__init__.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pyc3l-0.1.1/src/pyc3l/wallet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyc3l-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyc3l-0.1.1/tests/test_evm_data.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pyc3l-0.1.1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 pyc3l-0.1.1/LICENSE
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 pyc3l-0.1.1/README.md
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pyc3l-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 pyc3l-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyc3l-0.2.0/_version.py
+-rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 pyc3l-0.2.0/src/pyc3l/ApiCommunication.py
+-rw-r--r--   0        0        0    14418 2020-02-02 00:00:00.000000 pyc3l-0.2.0/src/pyc3l/ApiHandling.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pyc3l-0.2.0/src/pyc3l/CryptoAsim.py
+-rw-r--r--   0        0        0    10126 2020-02-02 00:00:00.000000 pyc3l-0.2.0/src/pyc3l/__init__.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pyc3l-0.2.0/src/pyc3l/wallet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyc3l-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyc3l-0.2.0/tests/test_evm_data.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pyc3l-0.2.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 pyc3l-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 pyc3l-0.2.0/README.md
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pyc3l-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 pyc3l-0.2.0/PKG-INFO
```

### Comparing `pyc3l-0.1.1/src/pyc3l/ApiCommunication.py` & `pyc3l-0.2.0/src/pyc3l/ApiCommunication.py`

 * *Files identical despite different names*

### Comparing `pyc3l-0.1.1/src/pyc3l/ApiHandling.py` & `pyc3l-0.2.0/src/pyc3l/ApiHandling.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 
     URLS = {
         "api": "/api.php",
         "config": "/ipns/QmaAAZor2uLKnrzGCwyXTSwogJqmPjJgvpYgpmtz5XcSmR/configs/",
         "endpoint_list": "/ipns/QmcRWARTpuEf9E87cdA4FfjBkv7rKTJyfvsLFTzXsGATbL",
         "keys": "/keys.php",
         "transactions": "/trnslist.php",
+        "lost_transactions": "/lost_trn.php",
     }
 
     def __init__(self, url):
         self._url = url
 
     def __getattr__(self, label):
         if label in ["get", "post"]:
```

### Comparing `pyc3l-0.1.1/src/pyc3l/CryptoAsim.py` & `pyc3l-0.2.0/src/pyc3l/CryptoAsim.py`

 * *Files identical despite different names*

### Comparing `pyc3l-0.1.1/src/pyc3l/__init__.py` & `pyc3l-0.2.0/src/pyc3l/__init__.py`

 * *Files identical despite different names*

### Comparing `pyc3l-0.1.1/src/pyc3l/wallet.py` & `pyc3l-0.2.0/src/pyc3l/wallet.py`

 * *Files identical despite different names*

### Comparing `pyc3l-0.1.1/tests/test_evm_data.py` & `pyc3l-0.2.0/tests/test_evm_data.py`

 * *Files identical despite different names*

### Comparing `pyc3l-0.1.1/.gitignore` & `pyc3l-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyc3l-0.1.1/LICENSE` & `pyc3l-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyc3l-0.1.1/README.md` & `pyc3l-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyc3l-0.1.1/pyproject.toml` & `pyc3l-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyc3l-0.1.1/PKG-INFO` & `pyc3l-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyc3l
-Version: 0.1.1
+Version: 0.2.0
 Summary: ComChain API client library
 Project-URL: Homepage, https://github.com/com-chain/pyc3l
 Project-URL: Bug Tracker, https://github.com/com-chain/pyc3l/issues
 Author-email: Florian Dubath <florian@dubath.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


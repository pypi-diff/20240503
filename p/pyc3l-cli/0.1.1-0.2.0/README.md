# Comparing `tmp/pyc3l_cli-0.1.1.tar.gz` & `tmp/pyc3l_cli-0.2.0.tar.gz`

## Comparing `pyc3l_cli-0.1.1.tar` & `pyc3l_cli-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/_version.py
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/pyc3l
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/__init__.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cli.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/__init__.py
--rwxr-xr-x   0        0        0     2799 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/account_info.py
--rwxr-xr-x   0        0        0     3988 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/batch_pledge.py
--rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/batch_pledge_simple.py
--rwxr-xr-x   0        0        0     5941 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/batch_transfer.py
--rwxr-xr-x   0        0        0     2039 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/block_rate.py
--rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/check_transaction.py
--rwxr-xr-x   0        0        0     1025 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/delegate.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/example_delegate.py
--rwxr-xr-x   0        0        0     1066 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/example_pledge.py
--rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/example_transfer.py
--rwxr-xr-x   0        0        0      509 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/nodes_info.py
--rwxr-xr-x   0        0        0     1039 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/pledge.py
--rwxr-xr-x   0        0        0     1485 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/transfer_on_behalf.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 pyc3l_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/_version.py
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/pyc3l
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/__init__.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cli.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/__init__.py
+-rwxr-xr-x   0        0        0     2799 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/account_info.py
+-rwxr-xr-x   0        0        0     3988 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/batch_pledge.py
+-rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/batch_pledge_simple.py
+-rwxr-xr-x   0        0        0     5941 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/batch_transfer.py
+-rwxr-xr-x   0        0        0     2039 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/block_rate.py
+-rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/check_transaction.py
+-rwxr-xr-x   0        0        0     1025 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/delegate.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/example_delegate.py
+-rwxr-xr-x   0        0        0     1066 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/example_pledge.py
+-rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/example_transfer.py
+-rwxr-xr-x   0        0        0     2294 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/lost_transactions.py
+-rwxr-xr-x   0        0        0      509 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/nodes_info.py
+-rwxr-xr-x   0        0        0     1039 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/pledge.py
+-rwxr-xr-x   0        0        0     1485 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/transfer_on_behalf.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 pyc3l_cli-0.2.0/PKG-INFO
```

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/__init__.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cli.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cli.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/common.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/common.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/account_info.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/account_info.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/batch_pledge.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/batch_pledge.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/batch_pledge_simple.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/batch_pledge_simple.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/batch_transfer.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/batch_transfer.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/block_rate.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/block_rate.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/delegate.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/delegate.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/example_delegate.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/example_delegate.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/example_pledge.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/example_pledge.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/example_transfer.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/example_transfer.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/pledge.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/pledge.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/src/pyc3l_cli/cmd/transfer_on_behalf.py` & `pyc3l_cli-0.2.0/src/pyc3l_cli/cmd/transfer_on_behalf.py`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/.gitignore` & `pyc3l_cli-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/LICENSE` & `pyc3l_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/README.md` & `pyc3l_cli-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/pyproject.toml` & `pyc3l_cli-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyc3l_cli-0.1.1/PKG-INFO` & `pyc3l_cli-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyc3l-cli
-Version: 0.1.1
+Version: 0.2.0
 Summary: ComChain API client library
 Project-URL: Homepage, https://github.com/com-chain/pyc3l-cli
 Project-URL: Bug Tracker, https://github.com/com-chain/pyc3l-cli/issues
 Author-email: Florian Dubath <florian@dubath.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


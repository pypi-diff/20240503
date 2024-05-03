# Comparing `tmp/upowpy-1.0.3.tar.gz` & `tmp/upowpy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upowpy-1.0.3.tar", last modified: Fri May  3 05:27:52 2024, max compression
+gzip compressed data, was "upowpy-1.0.4.tar", last modified: Fri May  3 08:00:09 2024, max compression
```

## Comparing `upowpy-1.0.3.tar` & `upowpy-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 05:27:52.251827 upowpy-1.0.3/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     7638 2024-05-03 05:27:52.251608 upowpy-1.0.3/PKG-INFO
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     6812 2024-05-02 06:41:37.000000 upowpy-1.0.3/README.md
--rw-r--r--   0 georgeprethesh   (501) staff       (20)       38 2024-05-03 05:27:52.251876 upowpy-1.0.3/setup.cfg
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      986 2024-05-03 05:27:13.000000 upowpy-1.0.3/setup.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 05:27:52.246685 upowpy-1.0.3/upowpy/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      510 2024-05-03 05:19:02.000000 upowpy-1.0.3/upowpy/__init__.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     4696 2024-05-02 06:13:22.000000 upowpy-1.0.3/upowpy/push.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 05:27:52.249884 upowpy-1.0.3/upowpy/upow_transactions/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:00.000000 upowpy-1.0.3/upowpy/upow_transactions/__init__.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     1441 2024-05-01 07:35:56.000000 upowpy-1.0.3/upowpy/upow_transactions/coinbase_transaction.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      211 2024-03-01 05:05:06.000000 upowpy-1.0.3/upowpy/upow_transactions/constants.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     5524 2024-03-10 06:13:43.000000 upowpy-1.0.3/upowpy/upow_transactions/helpers.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     8573 2024-05-01 07:36:55.000000 upowpy-1.0.3/upowpy/upow_transactions/transaction.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     4945 2024-05-01 07:36:18.000000 upowpy-1.0.3/upowpy/upow_transactions/transaction_input.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     1522 2024-05-01 07:36:30.000000 upowpy-1.0.3/upowpy/upow_transactions/transaction_output.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 05:27:52.250665 upowpy-1.0.3/upowpy/utils/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:03.000000 upowpy-1.0.3/upowpy/utils/__init__.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)    17563 2024-05-01 07:48:39.000000 upowpy-1.0.3/upowpy/utils/repository.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)    22657 2024-05-03 05:25:31.000000 upowpy-1.0.3/upowpy/utils/utils.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 05:27:52.251080 upowpy-1.0.3/upowpy.egg-info/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     7638 2024-05-03 05:27:52.000000 upowpy-1.0.3/upowpy.egg-info/PKG-INFO
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      568 2024-05-03 05:27:52.000000 upowpy-1.0.3/upowpy.egg-info/SOURCES.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        1 2024-05-03 05:27:52.000000 upowpy-1.0.3/upowpy.egg-info/dependency_links.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      233 2024-05-03 05:27:52.000000 upowpy-1.0.3/upowpy.egg-info/requires.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        7 2024-05-03 05:27:52.000000 upowpy-1.0.3/upowpy.egg-info/top_level.txt
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 08:00:09.598075 upowpy-1.0.4/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     7638 2024-05-03 08:00:09.597803 upowpy-1.0.4/PKG-INFO
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     6812 2024-05-02 06:41:37.000000 upowpy-1.0.4/README.md
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)       38 2024-05-03 08:00:09.598127 upowpy-1.0.4/setup.cfg
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      986 2024-05-03 07:58:43.000000 upowpy-1.0.4/setup.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 08:00:09.592932 upowpy-1.0.4/upowpy/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      510 2024-05-03 05:19:02.000000 upowpy-1.0.4/upowpy/__init__.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     4696 2024-05-02 06:13:22.000000 upowpy-1.0.4/upowpy/push.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 08:00:09.595916 upowpy-1.0.4/upowpy/upow_transactions/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:00.000000 upowpy-1.0.4/upowpy/upow_transactions/__init__.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     1441 2024-05-01 07:35:56.000000 upowpy-1.0.4/upowpy/upow_transactions/coinbase_transaction.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      211 2024-03-01 05:05:06.000000 upowpy-1.0.4/upowpy/upow_transactions/constants.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     5524 2024-03-10 06:13:43.000000 upowpy-1.0.4/upowpy/upow_transactions/helpers.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     8573 2024-05-01 07:36:55.000000 upowpy-1.0.4/upowpy/upow_transactions/transaction.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     4945 2024-05-01 07:36:18.000000 upowpy-1.0.4/upowpy/upow_transactions/transaction_input.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     1522 2024-05-01 07:36:30.000000 upowpy-1.0.4/upowpy/upow_transactions/transaction_output.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 08:00:09.596977 upowpy-1.0.4/upowpy/utils/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)       25 2024-05-03 07:59:33.000000 upowpy-1.0.4/upowpy/utils/__init__.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)    17563 2024-05-01 07:48:39.000000 upowpy-1.0.4/upowpy/utils/repository.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)    22656 2024-05-03 07:59:49.000000 upowpy-1.0.4/upowpy/utils/utils.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 08:00:09.597448 upowpy-1.0.4/upowpy.egg-info/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     7638 2024-05-03 08:00:09.000000 upowpy-1.0.4/upowpy.egg-info/PKG-INFO
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      568 2024-05-03 08:00:09.000000 upowpy-1.0.4/upowpy.egg-info/SOURCES.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        1 2024-05-03 08:00:09.000000 upowpy-1.0.4/upowpy.egg-info/dependency_links.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      233 2024-05-03 08:00:09.000000 upowpy-1.0.4/upowpy.egg-info/requires.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        7 2024-05-03 08:00:09.000000 upowpy-1.0.4/upowpy.egg-info/top_level.txt
```

### Comparing `upowpy-1.0.3/PKG-INFO` & `upowpy-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upowpy
-Version: 1.0.3
+Version: 1.0.4
 Summary: upowpy is a Python library for interacting with uPow blockchain transactions, including sending funds, staking, voting, and managing nodes and validators on the blockchain
 Home-page: https://github.com/upowai/upowpy
 Author: upow
 Author-email: contact@upow.ai
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: asttokens==2.4.1
```

### Comparing `upowpy-1.0.3/README.md` & `upowpy-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.3/setup.py` & `upowpy-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="upowpy",
-    version="1.0.3",
+    version="1.0.4",
     author="upow",
     author_email="contact@upow.ai",
     description="upowpy is a Python library for interacting with uPow blockchain transactions, including sending funds, staking, voting, and managing nodes and validators on the blockchain",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/upowai/upowpy",
     packages=find_packages(),
```

### Comparing `upowpy-1.0.3/upowpy/push.py` & `upowpy-1.0.4/upowpy/push.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.3/upowpy/upow_transactions/coinbase_transaction.py` & `upowpy-1.0.4/upowpy/upow_transactions/coinbase_transaction.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.3/upowpy/upow_transactions/helpers.py` & `upowpy-1.0.4/upowpy/upow_transactions/helpers.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.3/upowpy/upow_transactions/transaction.py` & `upowpy-1.0.4/upowpy/upow_transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.3/upowpy/upow_transactions/transaction_input.py` & `upowpy-1.0.4/upowpy/upow_transactions/transaction_input.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.3/upowpy/upow_transactions/transaction_output.py` & `upowpy-1.0.4/upowpy/upow_transactions/transaction_output.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.3/upowpy/utils/repository.py` & `upowpy-1.0.4/upowpy/utils/repository.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.3/upowpy/utils/utils.py` & `upowpy-1.0.4/upowpy/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     TransactionType,
 )
 from ..upow_transactions.transaction import Transaction
 from ..upow_transactions.transaction_output import TransactionOutput
 
 
 class Utils:
-
     def __init__(self, node_url="https://api.upow.ai"):
         self.NODE_URL = node_url
         self.repo = WalletRepository(self.NODE_URL)
 
     def get_balance_info(self, address: str):
         result = self.repo.get_balance_info(address)
         return result
```

### Comparing `upowpy-1.0.3/upowpy.egg-info/PKG-INFO` & `upowpy-1.0.4/upowpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upowpy
-Version: 1.0.3
+Version: 1.0.4
 Summary: upowpy is a Python library for interacting with uPow blockchain transactions, including sending funds, staking, voting, and managing nodes and validators on the blockchain
 Home-page: https://github.com/upowai/upowpy
 Author: upow
 Author-email: contact@upow.ai
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: asttokens==2.4.1
```

### Comparing `upowpy-1.0.3/upowpy.egg-info/SOURCES.txt` & `upowpy-1.0.4/upowpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


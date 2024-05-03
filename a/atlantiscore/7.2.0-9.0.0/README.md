# Comparing `tmp/atlantiscore-7.2.0.tar.gz` & `tmp/atlantiscore-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlantiscore-7.2.0.tar", last modified: Wed Apr 24 14:54:43 2024, max compression
+gzip compressed data, was "atlantiscore-9.0.0.tar", last modified: Fri May  3 10:18:39 2024, max compression
```

## Comparing `atlantiscore-7.2.0.tar` & `atlantiscore-9.0.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.830613 atlantiscore-7.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-24 14:54:43.830613 atlantiscore-7.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.814613 atlantiscore-7.2.0/atlantiscore/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.814613 atlantiscore-7.2.0/atlantiscore/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.818613 atlantiscore-7.2.0/atlantiscore/db/types/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/db/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.818613 atlantiscore-7.2.0/atlantiscore/db/types/evm/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/db/types/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/db/types/evm/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/db/types/evm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/db/types/evm/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.818613 atlantiscore-7.2.0/atlantiscore/hash/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/hash/ecdsa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.818613 atlantiscore-7.2.0/atlantiscore/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.822613 atlantiscore-7.2.0/atlantiscore/lib/abi/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/lib/abi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/lib/eth.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/lib/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.822613 atlantiscore-7.2.0/atlantiscore/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.822613 atlantiscore-7.2.0/atlantiscore/middleware/blockchain/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/middleware/blockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/middleware/blockchain/erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/middleware/blockchain/evm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.822613 atlantiscore-7.2.0/atlantiscore/types/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.822613 atlantiscore-7.2.0/atlantiscore/types/evm/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/types/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/types/evm/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/types/evm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/types/evm/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/atlantiscore/types/key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.826613 atlantiscore-7.2.0/atlantiscore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-24 14:54:43.000000 atlantiscore-7.2.0/atlantiscore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-24 14:54:43.000000 atlantiscore-7.2.0/atlantiscore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:54:43.000000 atlantiscore-7.2.0/atlantiscore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-24 14:54:43.000000 atlantiscore-7.2.0/atlantiscore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 14:54:43.000000 atlantiscore-7.2.0/atlantiscore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:54:43.830613 atlantiscore-7.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:54:43.826613 atlantiscore-7.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-24 14:53:36.000000 atlantiscore-7.2.0/tests/test_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.778532 atlantiscore-9.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-03 10:18:39.778532 atlantiscore-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.762531 atlantiscore-9.0.0/atlantiscore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.762531 atlantiscore-9.0.0/atlantiscore/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.766532 atlantiscore-9.0.0/atlantiscore/db/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/db/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.766532 atlantiscore-9.0.0/atlantiscore/db/types/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/db/types/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/db/types/evm/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/db/types/evm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/db/types/evm/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.766532 atlantiscore-9.0.0/atlantiscore/hash/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/hash/ecdsa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.766532 atlantiscore-9.0.0/atlantiscore/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.770532 atlantiscore-9.0.0/atlantiscore/lib/abi/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/lib/abi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/lib/eth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/lib/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.770532 atlantiscore-9.0.0/atlantiscore/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.770532 atlantiscore-9.0.0/atlantiscore/middleware/blockchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/middleware/blockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/middleware/blockchain/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/middleware/blockchain/evm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.770532 atlantiscore-9.0.0/atlantiscore/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.774532 atlantiscore-9.0.0/atlantiscore/types/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/types/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/types/evm/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/types/evm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/types/evm/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/atlantiscore/types/key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.774532 atlantiscore-9.0.0/atlantiscore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-03 10:18:39.000000 atlantiscore-9.0.0/atlantiscore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-03 10:18:39.000000 atlantiscore-9.0.0/atlantiscore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:18:39.000000 atlantiscore-9.0.0/atlantiscore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-03 10:18:39.000000 atlantiscore-9.0.0/atlantiscore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 10:18:39.000000 atlantiscore-9.0.0/atlantiscore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:18:39.778532 atlantiscore-9.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:18:39.774532 atlantiscore-9.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-03 10:17:29.000000 atlantiscore-9.0.0/tests/test_finder.py
```

### Comparing `atlantiscore-7.2.0/PKG-INFO` & `atlantiscore-9.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: atlantiscore
-Version: 7.2.0
+Version: 9.0.0
 Summary: atlantiscore
 Author-email: Atlantis Labs <r00tail@protonmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles~=23.2
-Requires-Dist: codercore~=5.0.0
+Requires-Dist: codercore~=6.0.1
 Requires-Dist: coincurve~=18.0
 Requires-Dist: eth-hash[pycryptodome]~=0.5
 Requires-Dist: eth-utils~=2.1
 Requires-Dist: pydantic~=2.5
 Requires-Dist: sqlalchemy[asyncio]~=2.0
 Requires-Dist: web3[ipfs]~=6.9
 Provides-Extra: test
 Requires-Dist: pytest~=7.2.0; extra == "test"
 Requires-Dist: pytest-asyncio~=0.20.1; extra == "test"
 Requires-Dist: pytest-cov~=4.0.0; extra == "test"
 Requires-Dist: pytest-mock~=3.10.0; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=3.0.2; extra == "test"
 Provides-Extra: dev
-Requires-Dist: alembic~=1.9; extra == "dev"
+Requires-Dist: alembic~=1.13; extra == "dev"
 Requires-Dist: black~=22.12; extra == "dev"
 Requires-Dist: bumpver~=2022.1120; extra == "dev"
 Requires-Dist: flake8~=6.0; extra == "dev"
 Requires-Dist: isort~=5.12; extra == "dev"
 Requires-Dist: pre-commit~=2.21; extra == "dev"
 
 # Atlantis Labs - Core
```

### Comparing `atlantiscore-7.2.0/atlantiscore/__init__.py` & `atlantiscore-9.0.0/atlantiscore/__init__.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/atlantiscore/db/types/evm/base.py` & `atlantiscore-9.0.0/atlantiscore/db/types/evm/base.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/atlantiscore/db/types/evm/transaction.py` & `atlantiscore-9.0.0/atlantiscore/db/types/evm/transaction.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/atlantiscore/hash/ecdsa.py` & `atlantiscore-9.0.0/atlantiscore/hash/ecdsa.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/atlantiscore/lib/eth.py` & `atlantiscore-9.0.0/atlantiscore/lib/eth.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/atlantiscore/lib/exceptions.py` & `atlantiscore-9.0.0/atlantiscore/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/atlantiscore/middleware/blockchain/erc20.py` & `atlantiscore-9.0.0/atlantiscore/middleware/blockchain/erc20.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/atlantiscore/middleware/blockchain/evm.py` & `atlantiscore-9.0.0/atlantiscore/middleware/blockchain/evm.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/atlantiscore/types/evm/address.py` & `atlantiscore-9.0.0/atlantiscore/types/evm/address.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/atlantiscore/types/evm/base.py` & `atlantiscore-9.0.0/atlantiscore/types/evm/base.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/atlantiscore/types/evm/transaction.py` & `atlantiscore-9.0.0/atlantiscore/types/evm/transaction.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/atlantiscore.egg-info/PKG-INFO` & `atlantiscore-9.0.0/atlantiscore.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: atlantiscore
-Version: 7.2.0
+Version: 9.0.0
 Summary: atlantiscore
 Author-email: Atlantis Labs <r00tail@protonmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles~=23.2
-Requires-Dist: codercore~=5.0.0
+Requires-Dist: codercore~=6.0.1
 Requires-Dist: coincurve~=18.0
 Requires-Dist: eth-hash[pycryptodome]~=0.5
 Requires-Dist: eth-utils~=2.1
 Requires-Dist: pydantic~=2.5
 Requires-Dist: sqlalchemy[asyncio]~=2.0
 Requires-Dist: web3[ipfs]~=6.9
 Provides-Extra: test
 Requires-Dist: pytest~=7.2.0; extra == "test"
 Requires-Dist: pytest-asyncio~=0.20.1; extra == "test"
 Requires-Dist: pytest-cov~=4.0.0; extra == "test"
 Requires-Dist: pytest-mock~=3.10.0; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=3.0.2; extra == "test"
 Provides-Extra: dev
-Requires-Dist: alembic~=1.9; extra == "dev"
+Requires-Dist: alembic~=1.13; extra == "dev"
 Requires-Dist: black~=22.12; extra == "dev"
 Requires-Dist: bumpver~=2022.1120; extra == "dev"
 Requires-Dist: flake8~=6.0; extra == "dev"
 Requires-Dist: isort~=5.12; extra == "dev"
 Requires-Dist: pre-commit~=2.21; extra == "dev"
 
 # Atlantis Labs - Core
```

### Comparing `atlantiscore-7.2.0/atlantiscore.egg-info/SOURCES.txt` & `atlantiscore-9.0.0/atlantiscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlantiscore-7.2.0/pyproject.toml` & `atlantiscore-9.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atlantiscore"
-version = "7.2.0"
+version = "9.0.0"
 description = "atlantiscore"
 readme = "README.md"
 authors = [{ name = "Atlantis Labs", email = "r00tail@protonmail.com" }]
 dependencies = [
     "aiofiles ~= 23.2",
-    "codercore ~= 5.0.0",
+    "codercore ~= 6.0.1",
     "coincurve ~= 18.0",
     "eth-hash[pycryptodome]~=0.5",
     "eth-utils ~= 2.1",
     "pydantic ~= 2.5",
     "sqlalchemy[asyncio] ~= 2.0",
     "web3[ipfs] ~= 6.9"
 ]
@@ -24,25 +24,25 @@
     "pytest ~= 7.2.0",
     "pytest-asyncio ~= 0.20.1",
     "pytest-cov ~= 4.0.0",
     "pytest-mock ~= 3.10.0",
     "pytest-xdist[psutil] ~= 3.0.2",
 ]
 dev = [
-    "alembic ~= 1.9",
+    "alembic ~= 1.13",
     "black ~= 22.12",
     "bumpver ~= 2022.1120",
     "flake8 ~= 6.0",
     "isort ~= 5.12",
     "pre-commit ~= 2.21",
 ]
 
 
 [tool.bumpver]
-current_version = "7.2.0"
+current_version = "9.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `atlantiscore-7.2.0/tests/test_finder.py` & `atlantiscore-9.0.0/tests/test_finder.py`

 * *Files identical despite different names*


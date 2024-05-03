# Comparing `tmp/aiotx-0.1.0.tar.gz` & `tmp/aiotx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-0.1.0.tar", last modified: Wed May  1 20:25:51 2024, max compression
+gzip compressed data, was "aiotx-0.2.0.tar", last modified: Fri May  3 07:48:55 2024, max compression
```

## Comparing `aiotx-0.1.0.tar` & `aiotx-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.036228 aiotx-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.028228 aiotx-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.032228 aiotx-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-01 20:25:44.000000 aiotx-0.1.0/.github/workflows/lint-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-01 20:25:44.000000 aiotx-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-01 20:25:44.000000 aiotx-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 20:25:44.000000 aiotx-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-01 20:25:44.000000 aiotx-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-01 20:25:51.036228 aiotx-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-01 20:25:44.000000 aiotx-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.032228 aiotx-0.1.0/aiotx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.032228 aiotx-0.1.0/aiotx/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/clients/_bitcoin_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/clients/_evm_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.032228 aiotx-0.1.0/aiotx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.036228 aiotx-0.1.0/aiotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-01 20:25:50.000000 aiotx-0.1.0/aiotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-01 20:25:51.000000 aiotx-0.1.0/aiotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:25:50.000000 aiotx-0.1.0/aiotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-01 20:25:50.000000 aiotx-0.1.0/aiotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 20:25:50.000000 aiotx-0.1.0/aiotx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-01 20:25:44.000000 aiotx-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 20:25:44.000000 aiotx-0.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-01 20:25:51.036228 aiotx-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-01 20:25:44.000000 aiotx-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.032228 aiotx-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/confest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.028228 aiotx-0.1.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.028228 aiotx-0.1.0/tests/fixtures/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.036228 aiotx-0.1.0/tests/fixtures/cassettes/bsc/
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/test_bsc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.315048 aiotx-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.307048 aiotx-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.307048 aiotx-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-03 07:48:44.000000 aiotx-0.2.0/.github/workflows/lint-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-03 07:48:44.000000 aiotx-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-03 07:48:44.000000 aiotx-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-03 07:48:44.000000 aiotx-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-03 07:48:44.000000 aiotx-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-03 07:48:55.315048 aiotx-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-03 07:48:44.000000 aiotx-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.307048 aiotx-0.2.0/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/clients/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/clients/_bitcoin_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11847 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/aiotx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/utils/bep20_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.315048 aiotx-0.2.0/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-03 07:48:55.000000 aiotx-0.2.0/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-03 07:48:55.000000 aiotx-0.2.0/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:48:55.000000 aiotx-0.2.0/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 07:48:55.000000 aiotx-0.2.0/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 07:48:55.000000 aiotx-0.2.0/aiotx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-03 07:48:44.000000 aiotx-0.2.0/examples/aiogram_notificator_bot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-03 07:48:44.000000 aiotx-0.2.0/examples/aiogram_notificator_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-03 07:48:44.000000 aiotx-0.2.0/examples/block_and_transactions_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-03 07:48:44.000000 aiotx-0.2.0/examples/two_block_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 07:48:44.000000 aiotx-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 07:48:44.000000 aiotx-0.2.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-03 07:48:44.000000 aiotx-0.2.0/scripts/build_and_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 07:48:55.315048 aiotx-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-03 07:48:44.000000 aiotx-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/confest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.307048 aiotx-0.2.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.307048 aiotx-0.2.0/tests/fixtures/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.315048 aiotx-0.2.0/tests/fixtures/cassettes/bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/test_bsc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/test_bsc_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/test_bsc_monitoring.py
```

### Comparing `aiotx-0.1.0/.github/workflows/lint-check.yml` & `aiotx-0.2.0/.github/workflows/lint-check.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/.github/workflows/python-publish.yml` & `aiotx-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/.github/workflows/test.yml` & `aiotx-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/.gitignore` & `aiotx-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/CHANGELOG.md` & `aiotx-0.2.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.2.0]
+- block/transactions monitoring added, examples of usage added, tx input decoding added
+
 ## [0.1.0]
 - EVM client base logic added (get_balance, send tokens)
 - tests added
 
 ## [0.0.10]
 - EVM networks wallet generation logic added
```

### Comparing `aiotx-0.1.0/PKG-INFO` & `aiotx-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.1.0
+Version: 0.2.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `aiotx-0.1.0/README.md` & `aiotx-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/aiotx/exceptions.py` & `aiotx-0.2.0/aiotx/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/aiotx.egg-info/PKG-INFO` & `aiotx-0.2.0/aiotx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.1.0
+Version: 0.2.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `aiotx-0.1.0/setup.py` & `aiotx-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "wallet",
         "transaction",
     ],
     use_scm_version=True,
     description="An asynchronous library for interacting with various cryptocurrencies and blockchains",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    packages=find_packages(exclude=("tests", "scripts")),
+    packages=find_packages(exclude=("tests", "scripts", "examples")),
     package_data={
         "aiotx": ["py.typed"],
     },
     setup_requires=[
         "setuptools_scm",
     ],
     install_requires=[
```

### Comparing `aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_balance.yaml` & `aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_last_block.yaml` & `aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml` & `aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_transaction.yaml` & `aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml` & `aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml` & `aiotx-0.2.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/tests/fixtures/cassettes/bsc/send_transaction.yaml` & `aiotx-0.2.0/tests/fixtures/cassettes/bsc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.1.0/tests/test_bsc_client.py` & `aiotx-0.2.0/tests/test_bsc_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,47 @@
 import os
 
 import pytest
-from confest import vcr_c
+from confest import bsc_client, vcr_c  # noqa
 
 from aiotx.clients import AioTxBSCClient
 from aiotx.exceptions import (
     InvalidArgumentError,
     TransactionNotFound,
 )
 
-node_url = "https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/"
-chain_id = 97
-client = AioTxBSCClient(node_url, chain_id)
-
 PRIVATE_KEY_TO_SEND_FROM = os.environ.get("TEST_BSC_WALLET_PRIVATE_KEY")
-MAIN_WALLET = client.get_address_from_private_key(PRIVATE_KEY_TO_SEND_FROM)
 CONTRACT = "0x337610d27c682E347C9cD60BD4b3b107C9d34dDd"
 DESTINATION_ADDRESS = "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a"
 
 
 @vcr_c.use_cassette("bsc/get_last_block.yaml")
-async def test_get_last_block():
-    block_id = await client.get_last_block()
+async def test_get_last_block(bsc_client: AioTxBSCClient):
+    block_id = await bsc_client.get_last_block()
     assert isinstance(block_id, int)
 
 @pytest.mark.parametrize(
     "wallet_address, expected_exception, expected_balance",
     [
-        (MAIN_WALLET, None, 22536431000980000),
         ("0x1284214b9b9c85549aB3D2b972df0dEEf66aC2c9", None, 10561622435613231665),
         ("0x3a82a5a2b77d33a12621e860d1d19cdfb8bf63b4", None, 99724094999968300),
         ("0x0e28BD8B2D4efb8A3128f7fB310f4e227E25DB6F", None, 691239109999999988),
         ("0xfb2bdebad0cb9486e714b053a2dbfaf7c05151c9", None, 271930000000000),
         ("0x040bA056435A7675847F4D577d3Cb8Fc2646A946", None, 421930000000000),
         ("0x040bA056435A7675847F4D577d3Cb8Fc2646A948", None, 0),
         ("040bA056435A7675847F4D577d3Cb8Fc2646A946", InvalidArgumentError, 0),
     ],
 )
 @vcr_c.use_cassette("bsc/get_balance.yaml")
-async def test_get_balance(wallet_address, expected_exception, expected_balance):
+async def test_get_balance(bsc_client: AioTxBSCClient, wallet_address, expected_exception, expected_balance):
     if expected_exception:
         with pytest.raises(expected_exception):
-            await client.get_balance(wallet_address)
+            await bsc_client.get_balance(wallet_address)
     else:
-        balance = await client.get_balance(wallet_address)
+        balance = await bsc_client.get_balance(wallet_address)
         assert isinstance(balance, int)
         assert balance == expected_balance
 
 
 @pytest.mark.parametrize(
     "tx_id, expected_exception",
     [
@@ -60,20 +54,21 @@
         ("0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b9451909111", TransactionNotFound),
         ("0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b945190911", InvalidArgumentError),
         ("41c8e2e03195c29cea37d67ad234d91c52258a514c78f9fcfd196aa5992209ae", InvalidArgumentError),
 
     ],
 )
 @vcr_c.use_cassette("bsc/get_transaction.yaml")
-async def test_get_transaction(tx_id, expected_exception):
+async def test_get_transaction(bsc_client: AioTxBSCClient, tx_id, expected_exception):
     if expected_exception:
         with pytest.raises(expected_exception):
-            await client.get_transaction(tx_id)
+            await bsc_client.get_transaction(tx_id)
     else:
-        await client.get_transaction(tx_id)
+        tx = await bsc_client.get_transaction(tx_id)
+        assert "aiotx_decoded_input" in tx.keys()
 
 
 
 @pytest.mark.parametrize(
     "wallet_address, contract, expected_exception, expected_balance",
     [
         ("0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", CONTRACT, None, 1000000001000000000),
@@ -83,21 +78,21 @@
         ("0xf6626A900e4Cc958D2cD0Eb2186Fd6B29EDB63ce", CONTRACT, None, 950000000000000000),
         ("0x2dbB5a4c235164B9f772179A43faca2c71a8abDB", CONTRACT, None, 32963423288412440122),
         ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", CONTRACT, None, 0),
         ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", "Eeaa7E347ee4557f9a6F71C", InvalidArgumentError, 0),
     ],
 )
 @vcr_c.use_cassette("bsc/get_token_balance.yaml")
-async def test_get_token_balance(wallet_address, contract, expected_exception, expected_balance):
+async def test_get_token_balance(bsc_client: AioTxBSCClient, wallet_address, contract, expected_exception, expected_balance):
     
     if expected_exception:
         with pytest.raises(expected_exception):
-            await client.get_token_balance(wallet_address, contract)
+            await bsc_client.get_token_balance(wallet_address, contract)
     else:
-        balance = await client.get_token_balance(wallet_address, contract)
+        balance = await bsc_client.get_token_balance(wallet_address, contract)
         assert isinstance(balance, int)
         assert expected_balance == balance
 
 
 @pytest.mark.parametrize(
     "wallet_address, expected_exception, expected_count",
     [
@@ -108,31 +103,31 @@
         ("0xf6626A900e4Cc958D2cD0Eb2186Fd6B29EDB63ce", None, 17),
         ("0x2dbB5a4c235164B9f772179A43faca2c71a8abDB", None, 1),
         ("2dbB5a4c235164B9f772179A43faca2c71a8abDB", InvalidArgumentError, 0),
         ("0x2dbB5a4c235164B9f772179A43faca2c71a8ab", InvalidArgumentError, 0),
     ],
 )
 @vcr_c.use_cassette("bsc/get_transaction_count.yaml")
-async def test_get_transaction_count(wallet_address, expected_exception, expected_count):
+async def test_get_transaction_count(bsc_client: AioTxBSCClient, wallet_address, expected_exception, expected_count):
     if expected_exception:
         with pytest.raises(expected_exception):
-            await client.get_transaction_count(wallet_address)
+            await bsc_client.get_transaction_count(wallet_address)
     else:
-        count = await client.get_transaction_count(wallet_address)
+        count = await bsc_client.get_transaction_count(wallet_address)
         assert isinstance(count, int)
         assert expected_count == count
 
 
 @vcr_c.use_cassette("bsc/send_transaction.yaml")
-async def test_send_transaction():
-    result = await client.send_transaction(PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 10000, 5000000000)
+async def test_send_transaction(bsc_client: AioTxBSCClient):
+    result = await bsc_client.send_transaction(PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 10000, 5000000000)
     assert isinstance(result, dict)
     assert "result" in result
 
 
 @vcr_c.use_cassette("bsc/send_token_transaction.yaml")
-async def test_send_token_transaction():
-    result = await client.send_token_transaction(
+async def test_send_token_transaction(bsc_client: AioTxBSCClient):
+    result = await bsc_client.send_token_transaction(
         PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1000000000000000000, 1000000000
     )
     assert isinstance(result, str)
     assert result.startswith("0x")
```


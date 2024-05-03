# Comparing `tmp/aiotx-0.2.0.tar.gz` & `tmp/aiotx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-0.2.0.tar", last modified: Fri May  3 07:48:55 2024, max compression
+gzip compressed data, was "aiotx-0.3.0.tar", last modified: Fri May  3 09:31:28 2024, max compression
```

## Comparing `aiotx-0.2.0.tar` & `aiotx-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.315048 aiotx-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.307048 aiotx-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.307048 aiotx-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-03 07:48:44.000000 aiotx-0.2.0/.github/workflows/lint-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-03 07:48:44.000000 aiotx-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-03 07:48:44.000000 aiotx-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-03 07:48:44.000000 aiotx-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-03 07:48:44.000000 aiotx-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-03 07:48:55.315048 aiotx-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-03 07:48:44.000000 aiotx-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.307048 aiotx-0.2.0/aiotx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/aiotx/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/clients/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/clients/_bitcoin_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11847 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/clients/_evm_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/aiotx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/aiotx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-03 07:48:44.000000 aiotx-0.2.0/aiotx/utils/bep20_abi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.315048 aiotx-0.2.0/aiotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-03 07:48:55.000000 aiotx-0.2.0/aiotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-03 07:48:55.000000 aiotx-0.2.0/aiotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:48:55.000000 aiotx-0.2.0/aiotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 07:48:55.000000 aiotx-0.2.0/aiotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 07:48:55.000000 aiotx-0.2.0/aiotx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-03 07:48:44.000000 aiotx-0.2.0/examples/aiogram_notificator_bot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-03 07:48:44.000000 aiotx-0.2.0/examples/aiogram_notificator_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-03 07:48:44.000000 aiotx-0.2.0/examples/block_and_transactions_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-03 07:48:44.000000 aiotx-0.2.0/examples/two_block_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 07:48:44.000000 aiotx-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 07:48:44.000000 aiotx-0.2.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-03 07:48:44.000000 aiotx-0.2.0/scripts/build_and_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 07:48:55.315048 aiotx-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-03 07:48:44.000000 aiotx-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.311048 aiotx-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/confest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.307048 aiotx-0.2.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.307048 aiotx-0.2.0/tests/fixtures/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:48:55.315048 aiotx-0.2.0/tests/fixtures/cassettes/bsc/
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/test_bsc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/test_bsc_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-03 07:48:44.000000 aiotx-0.2.0/tests/test_bsc_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.360614 aiotx-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.352614 aiotx-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.352614 aiotx-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-03 09:31:20.000000 aiotx-0.3.0/.github/workflows/lint-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-03 09:31:20.000000 aiotx-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-03 09:31:20.000000 aiotx-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-03 09:31:20.000000 aiotx-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-03 09:31:20.000000 aiotx-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-03 09:31:28.360614 aiotx-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-03 09:31:20.000000 aiotx-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.352614 aiotx-0.3.0/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/clients/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/clients/_bitcoin_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12459 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/aiotx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/utils/bep20_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.360614 aiotx-0.3.0/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-03 09:31:28.000000 aiotx-0.3.0/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-03 09:31:28.000000 aiotx-0.3.0/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:31:28.000000 aiotx-0.3.0/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 09:31:28.000000 aiotx-0.3.0/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 09:31:28.000000 aiotx-0.3.0/aiotx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-03 09:31:20.000000 aiotx-0.3.0/examples/aiogram_notificator_bot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-03 09:31:20.000000 aiotx-0.3.0/examples/aiogram_notificator_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-03 09:31:20.000000 aiotx-0.3.0/examples/block_and_transactions_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-03 09:31:20.000000 aiotx-0.3.0/examples/two_block_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 09:31:20.000000 aiotx-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 09:31:20.000000 aiotx-0.3.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-03 09:31:20.000000 aiotx-0.3.0/scripts/build_and_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 09:31:28.360614 aiotx-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-03 09:31:20.000000 aiotx-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/confest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.352614 aiotx-0.3.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.352614 aiotx-0.3.0/tests/fixtures/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/tests/fixtures/cassettes/bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/test_bsc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/test_bsc_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/test_bsc_monitoring.py
```

### Comparing `aiotx-0.2.0/.github/workflows/lint-check.yml` & `aiotx-0.3.0/.github/workflows/lint-check.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/.github/workflows/python-publish.yml` & `aiotx-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/.github/workflows/test.yml` & `aiotx-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/.gitignore` & `aiotx-0.3.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -154,8 +154,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
-.vscode/
+.vscode/
+test.py
```

### Comparing `aiotx-0.2.0/CHANGELOG.md` & `aiotx-0.3.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.3.0]
+- Function for getting current gas price is added and to_wai/from_wai functions are attached to EVM client now
+
 ## [0.2.0]
 - block/transactions monitoring added, examples of usage added, tx input decoding added
 
 ## [0.1.0]
 - EVM client base logic added (get_balance, send tokens)
 - tests added
```

### Comparing `aiotx-0.2.0/PKG-INFO` & `aiotx-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.2.0
+Version: 0.3.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `aiotx-0.2.0/README.md` & `aiotx-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/aiotx/clients/_base_client.py` & `aiotx-0.3.0/aiotx/clients/_base_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/aiotx/clients/_evm_base_client.py` & `aiotx-0.3.0/aiotx/clients/_evm_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import asyncio
+import decimal
 import json
 import secrets
+from typing import Union
 
 import aiohttp
 from eth_abi import decode, encode
 from eth_account import Account
 from eth_typing import HexStr
 from eth_utils import (
+    currency,
     decode_hex,
     function_signature_to_4byte_selector,
     keccak,
     to_checksum_address,
     to_hex,
 )
 
@@ -49,14 +52,22 @@
         self._bep20_abi = bep_20_abi
 
     def generate_address(self):
         private_key_bytes = secrets.token_hex(32)
         private_key = "0x" + private_key_bytes
         acct = Account.from_key(private_key)
         return private_key, acct.address
+    
+    @staticmethod
+    def from_wei(number: int, unit: str) -> Union[int, decimal.Decimal]:
+        return currency.from_wei(number, unit)
+    
+    @staticmethod
+    def to_wei(number: Union[int, float, str, decimal.Decimal], unit: str) -> int:
+        return currency.to_wei(number, unit)
 
     def get_address_from_private_key(self, private_key: str):
         sender_address = Account.from_key(private_key).address
         return to_checksum_address(sender_address)
 
     async def get_last_block(self) -> int:
         payload = {"method": "eth_blockNumber", "params": []}
@@ -66,15 +77,21 @@
 
     async def get_balance(self, address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
         payload = {"method": "eth_getBalance", "params": [address, block_parameter.value]}
 
         result = await self._make_rpc_call(payload)
         balance = result["result"]
         return 0 if balance == "0x" else int(result["result"], 16)
-
+    
+    async def get_gas_price(self) -> int:
+        payload = {"method": "eth_gasPrice", "params": []}
+        result = await self._make_rpc_call(payload)
+        price = result["result"]
+        return 0 if price == "0x" else int(result["result"], 16)
+        
     async def get_transaction(self, hash) -> dict:
         payload = {"method": "eth_getTransactionByHash", "params": [hash]}
         result = await self._make_rpc_call(payload)
         if result["result"] is None:
             raise TransactionNotFound(f"Transaction {hash} not found!")
         tx_data = result["result"]
         tx_data["aiotx_decoded_input"] = self.decode_transaction_input(tx_data["input"])
```

### Comparing `aiotx-0.2.0/aiotx/exceptions.py` & `aiotx-0.3.0/aiotx/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/aiotx/utils/bep20_abi.json` & `aiotx-0.3.0/aiotx/utils/bep20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/aiotx.egg-info/PKG-INFO` & `aiotx-0.3.0/aiotx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.2.0
+Version: 0.3.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `aiotx-0.2.0/aiotx.egg-info/SOURCES.txt` & `aiotx-0.3.0/aiotx.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 examples/two_block_parsers.py
 scripts/build_and_test.sh
 tests/confest.py
 tests/test_bsc_client.py
 tests/test_bsc_input_decoding.py
 tests/test_bsc_monitoring.py
 tests/fixtures/cassettes/bsc/get_balance.yaml
+tests/fixtures/cassettes/bsc/get_gas_price.yaml
 tests/fixtures/cassettes/bsc/get_last_block.yaml
 tests/fixtures/cassettes/bsc/get_token_balance.yaml
 tests/fixtures/cassettes/bsc/get_transaction.yaml
 tests/fixtures/cassettes/bsc/get_transaction_count.yaml
 tests/fixtures/cassettes/bsc/send_token_transaction.yaml
 tests/fixtures/cassettes/bsc/send_transaction.yaml
 tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
```

### Comparing `aiotx-0.2.0/examples/aiogram_notificator_bot.png` & `aiotx-0.3.0/examples/aiogram_notificator_bot.png`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/examples/aiogram_notificator_bot.py` & `aiotx-0.3.0/examples/aiogram_notificator_bot.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/examples/block_and_transactions_parser.py` & `aiotx-0.3.0/examples/block_and_transactions_parser.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/examples/two_block_parsers.py` & `aiotx-0.3.0/examples/two_block_parsers.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/setup.py` & `aiotx-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/tests/confest.py` & `aiotx-0.3.0/tests/confest.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_balance.yaml` & `aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_last_block.yaml` & `aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml` & `aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_transaction.yaml` & `aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml` & `aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml` & `aiotx-0.3.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/tests/fixtures/cassettes/bsc/send_transaction.yaml` & `aiotx-0.3.0/tests/fixtures/cassettes/bsc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml` & `aiotx-0.3.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/tests/test_bsc_client.py` & `aiotx-0.3.0/tests/test_bsc_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from aiotx.clients import AioTxBSCClient
 from aiotx.exceptions import (
     InvalidArgumentError,
     TransactionNotFound,
 )
 
 PRIVATE_KEY_TO_SEND_FROM = os.environ.get("TEST_BSC_WALLET_PRIVATE_KEY")
+assert PRIVATE_KEY_TO_SEND_FROM is not None, "Please provide TEST_BSC_WALLET_PRIVATE_KEY"
 CONTRACT = "0x337610d27c682E347C9cD60BD4b3b107C9d34dDd"
 DESTINATION_ADDRESS = "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a"
 
 
 @vcr_c.use_cassette("bsc/get_last_block.yaml")
 async def test_get_last_block(bsc_client: AioTxBSCClient):
     block_id = await bsc_client.get_last_block()
@@ -127,7 +128,14 @@
 @vcr_c.use_cassette("bsc/send_token_transaction.yaml")
 async def test_send_token_transaction(bsc_client: AioTxBSCClient):
     result = await bsc_client.send_token_transaction(
         PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1000000000000000000, 1000000000
     )
     assert isinstance(result, str)
     assert result.startswith("0x")
+
+
+@vcr_c.use_cassette("bsc/get_gas_price.yaml")
+async def test_send_token_transaction(bsc_client: AioTxBSCClient):
+    result = await bsc_client.get_gas_price()
+    assert isinstance(result, int)
+    assert result == 5000000000
```

### Comparing `aiotx-0.2.0/tests/test_bsc_input_decoding.py` & `aiotx-0.3.0/tests/test_bsc_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.2.0/tests/test_bsc_monitoring.py` & `aiotx-0.3.0/tests/test_bsc_monitoring.py`

 * *Files identical despite different names*


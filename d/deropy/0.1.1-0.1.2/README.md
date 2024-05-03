# Comparing `tmp/deropy-0.1.1.tar.gz` & `tmp/deropy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deropy-0.1.1.tar", last modified: Mon Apr 29 11:03:57 2024, max compression
+gzip compressed data, was "deropy-0.1.2.tar", last modified: Fri May  3 14:06:05 2024, max compression
```

## Comparing `deropy-0.1.1.tar` & `deropy-0.1.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:03:57.751215 deropy-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-29 11:03:57.751215 deropy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-29 11:03:53.000000 deropy-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:03:57.739215 deropy-0.1.1/deropy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:03:57.743215 deropy-0.1.1/deropy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/commands/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:03:57.743215 deropy-0.1.1/deropy/dvm/
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/Smartcontract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/Wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:03:57.751215 deropy-0.1.1/deropy/dvm/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/AddressRaw.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/AddressString.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/AssetValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Atoi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Blid.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/BlockHeight.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/BlockTimestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Dero.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/DeroValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Function.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/HexDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/IsAddressValid.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Itoa.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Load.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/MapDelete.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/MapExists.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/MapGet.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/MapStore.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Panic.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Random.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Scid.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/SendAssetToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/SendDeroToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Sha3256.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Signer.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Store.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Strlen.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Substr.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/Txid.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/UpdateScCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/dvm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-29 11:03:53.000000 deropy-0.1.1/deropy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:03:57.751215 deropy-0.1.1/deropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-29 11:03:57.000000 deropy-0.1.1/deropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-29 11:03:57.000000 deropy-0.1.1/deropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:03:57.000000 deropy-0.1.1/deropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 11:03:57.000000 deropy-0.1.1/deropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-29 11:03:57.000000 deropy-0.1.1/deropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 11:03:57.000000 deropy-0.1.1/deropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:03:57.751215 deropy-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-29 11:03:53.000000 deropy-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:03:57.751215 deropy-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-29 11:03:53.000000 deropy-0.1.1/tests/test_compute_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-29 11:03:53.000000 deropy-0.1.1/tests/test_map_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-29 11:03:53.000000 deropy-0.1.1/tests/test_storage_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.174662 deropy-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-03 14:05:59.000000 deropy-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-03 14:06:05.174662 deropy-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-03 14:05:59.000000 deropy-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.162662 deropy-0.1.2/deropy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.162662 deropy-0.1.2/deropy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/commands/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.166662 deropy-0.1.2/deropy/dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/Smartcontract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/Wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.170662 deropy-0.1.2/deropy/dvm/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/AddressRaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/AddressString.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/AssetValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Atoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Blid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/BlockHeight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/BlockTimestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Dero.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/DeroValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/HexDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/IsAddressValid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Itoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/MapDelete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/MapExists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/MapGet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/MapStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Panic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Scid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/SendAssetToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/SendDeroToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Sha3256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Strlen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Substr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Txid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/UpdateScCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.174662 deropy-0.1.2/deropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:06:05.174662 deropy-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-03 14:05:59.000000 deropy-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.174662 deropy-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-03 14:05:59.000000 deropy-0.1.2/tests/test_compute_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-03 14:05:59.000000 deropy-0.1.2/tests/test_map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-03 14:05:59.000000 deropy-0.1.2/tests/test_storage_functions.py
```

### Comparing `deropy-0.1.1/PKG-INFO` & `deropy-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: click==8.0.4
 Requires-Dist: requests==2.31.0
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: python-dotenv==0.20.0
 Requires-Dist: InquirerPy==0.3.4
 Requires-Dist: pycryptodome==3.20.0
```

### Comparing `deropy-0.1.1/README.md` & `deropy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/commands/configure.py` & `deropy-0.1.2/deropy/commands/configure.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/commands/deploy.py` & `deropy-0.1.2/deropy/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/commands/generate.py` & `deropy-0.1.2/deropy/commands/generate.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/Smartcontract.py` & `deropy-0.1.2/deropy/dvm/Smartcontract.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         sc = SmartContract.get_instance()
         sc.gasCompute = []
         sc.gasStorage = []
 
         print("-" * 120)
-        print("Function: ", func.__name__)
+        print("Function: ", func.func_name)
         value = func(*args, **kwargs)
         print('----')
 
         if sum(sc.gasCompute) > SmartContract.max_compute_gaz:
             print_red('total gas compute: ', sum(sc.gasCompute))
             print_red('total gas storage: ', sum(sc.gasStorage))
         else:
```

### Comparing `deropy-0.1.1/deropy/dvm/Wallet.py` & `deropy-0.1.2/deropy/dvm/Wallet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import hashlib
 
 
 class Wallet:
     def __init__(self, id):
         self.string_address = hashlib.sha256(str(id).encode()).hexdigest()
         self.raw_address = self.string_address[:33]
-        self.balance = 0
+        self.balance = {}
 
     @classmethod
     def from_public_key(cls, public_key):
         wallet = cls(public_key)
         wallet.string_address = public_key
         wallet.raw_address = public_key[:33]
         return wallet
+    
+    def get_balance(self, token):
+        return self.balance.get(token, 0)
+    
+    def set_balance(self, token, amount):
+        self.balance[token] = amount
 
 
 class WalletSimulator:
     active_wallet = None
     wallets = {}
 
     @staticmethod
@@ -36,14 +42,23 @@
 
     @staticmethod
     def find_wallet_id_from_raw(raw_address):
         for id, wallet in WalletSimulator.wallets.items():
             if wallet.raw_address == raw_address:
                 return id
         raise Exception("Wallet not found")
+    
+    @staticmethod
+    def get_wallet_from_raw(raw_address):
+        id = WalletSimulator.find_wallet_id_from_raw(raw_address)
+        return WalletSimulator.get_wallet_from_id(id)
+    
+    @staticmethod
+    def get_wallet_from_id(id):
+        return WalletSimulator.wallets[id]
 
     @staticmethod
     def get_raw_address():
         return WalletSimulator.wallets[WalletSimulator.active_wallet].raw_address
 
     @staticmethod
     def get_string_address():
```

### Comparing `deropy-0.1.1/deropy/dvm/functions/AddressRaw.py` & `deropy-0.1.2/deropy/dvm/functions/AddressRaw.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/AddressString.py` & `deropy-0.1.2/deropy/dvm/functions/AddressString.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/AssetValue.py` & `deropy-0.1.2/deropy/dvm/functions/AssetValue.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/Atoi.py` & `deropy-0.1.2/deropy/dvm/functions/Atoi.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/BlockHeight.py` & `deropy-0.1.2/deropy/dvm/functions/BlockHeight.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/Dero.py` & `deropy-0.1.2/deropy/dvm/functions/Dero.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/DeroValue.py` & `deropy-0.1.2/deropy/dvm/functions/DeroValue.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/Function.py` & `deropy-0.1.2/deropy/dvm/functions/Function.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/IsAddressValid.py` & `deropy-0.1.2/deropy/dvm/functions/IsAddressValid.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/Itoa.py` & `deropy-0.1.2/deropy/dvm/functions/Itoa.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/Keccak256.py` & `deropy-0.1.2/deropy/dvm/functions/Keccak256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/Load.py` & `deropy-0.1.2/deropy/dvm/functions/Load.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/MapExists.py` & `deropy-0.1.2/deropy/dvm/functions/MapExists.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/MapStore.py` & `deropy-0.1.2/deropy/dvm/functions/MapStore.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/Random.py` & `deropy-0.1.2/deropy/dvm/functions/Random.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/Scid.py` & `deropy-0.1.2/deropy/dvm/functions/Scid.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/SendAssetToAddress.py` & `deropy-0.1.2/deropy/dvm/functions/Store.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from deropy.dvm.functions.Function import Function
 
 
-class SendAssetToAddress(Function):
+class Store(Function):
     def __init__(self):
         func_parameters = {
-            "raw_address": {"type": "str", "value": None},
-            "amount": {"type": "int", "value": None},
-            "asset": {"type": "str", "value": None},
+            "key": {"type": "str", "value": None},
+            "value": {"type": "Any", "value": None},
         }
-        super().__init__("send_asset_to_address", 90_000, 0, func_parameters)
-
-    def _computeGasStorageCost(self):
-        return len(self.parameters["raw_address"]["value"]) + len(self.parameters["asset"]["value"])
+        super().__init__("store", 10_000, 0, func_parameters)
 
     def _exec(self, *args, **kwargs):
-        self.parameters["raw_address"]["value"] = kwargs["raw_address"]
-        self.parameters["amount"]["value"] = kwargs["amount"]
-        self.parameters["asset"]["value"] = kwargs["asset"]
-        return 0
+        self.parameters["key"]["value"] = kwargs["key"]
+        self.parameters["value"]["value"] = kwargs["value"]
+        self.sc.storage[kwargs["key"]] = kwargs["value"]
+
+    def _computeGasStorageCost(self):
+        if isinstance(self.parameters["value"]["value"], int):
+            return 8
+        else:
+            return len(self.parameters["value"]["value"])
 
 
-def send_asset_to_address(raw_address: str, amount: int, asset: str):
-    return SendAssetToAddress()(raw_address=raw_address, amount=amount, asset=asset)
+def store(variable: str, value):
+    return Store()(key=variable, value=value)
```

### Comparing `deropy-0.1.1/deropy/dvm/functions/SendDeroToAddress.py` & `deropy-0.1.2/deropy/dvm/functions/UpdateScCode.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from deropy.dvm.functions.Function import Function
 
 
-class SendDeroToAddress(Function):
+class UpdateScCode(Function):
     def __init__(self):
         func_parameters = {
-            "raw_address": {"type": "str", "value": None},
-            "amount": {"type": "int", "value": None},
+            "sc_code": {"type": "str", "value": None},
         }
-        super().__init__("send_dero_to_address", 70_000, 0, func_parameters)
+        super().__init__("update_sc_code", 5000, 0, func_parameters)
 
     def _computeGasStorageCost(self):
-        return len(self.parameters["raw_address"]["value"])
+        if isinstance(self.parameters["sc_code"]["value"], int):
+            return 1
+        else:
+            size = len(self.parameters["sc_code"]["value"])
+            return size * 2  # 2 gas per byte (1 for tx, 1 for storage)
 
     def _exec(self, *args, **kwargs):
-        self.parameters["raw_address"]["value"] = kwargs["raw_address"]
-        self.parameters["amount"]["value"] = kwargs["amount"]
+        self.parameters["sc_code"]["value"] = kwargs["sc_code"]
+        self.sc.storage["code"] = kwargs["sc_code"]
         return 0
 
 
-def send_dero_to_address(raw_address: str, amount: int):
-    return SendDeroToAddress()(raw_address=raw_address, amount=amount)
+def update_sc_code(sc_code: str):
+    return UpdateScCode()(sc_code=sc_code)
```

### Comparing `deropy-0.1.1/deropy/dvm/functions/Sha256.py` & `deropy-0.1.2/deropy/dvm/functions/Sha256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/Sha3256.py` & `deropy-0.1.2/deropy/dvm/functions/Sha3256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/Signer.py` & `deropy-0.1.2/deropy/dvm/functions/Signer.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/Substr.py` & `deropy-0.1.2/deropy/dvm/functions/Substr.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/functions/__init__.py` & `deropy-0.1.2/deropy/dvm/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy/dvm/utils.py` & `deropy-0.1.2/deropy/dvm/utils.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/deropy.egg-info/PKG-INFO` & `deropy-0.1.2/deropy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: click==8.0.4
 Requires-Dist: requests==2.31.0
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: python-dotenv==0.20.0
 Requires-Dist: InquirerPy==0.3.4
 Requires-Dist: pycryptodome==3.20.0
```

### Comparing `deropy-0.1.1/deropy.egg-info/SOURCES.txt` & `deropy-0.1.2/deropy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 deropy/__init__.py
 deropy/main.py
 deropy.egg-info/PKG-INFO
 deropy.egg-info/SOURCES.txt
 deropy.egg-info/dependency_links.txt
```

### Comparing `deropy-0.1.1/setup.py` & `deropy-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='deropy',
-    version=os.getenv('DEROPY_VERSION') or '0.1.1',
+    version=os.getenv('DEROPY_VERSION') or '0.1.2',
     url='https://github.com/dero-hyperbolic/deropy.git',
     author_email='leocances@gmail.com',
     description='A set of tool to help of DERO smart contract development',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

### Comparing `deropy-0.1.1/tests/test_compute_storage.py` & `deropy-0.1.2/tests/test_compute_storage.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/tests/test_map_functions.py` & `deropy-0.1.2/tests/test_map_functions.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.1/tests/test_storage_functions.py` & `deropy-0.1.2/tests/test_storage_functions.py`

 * *Files identical despite different names*


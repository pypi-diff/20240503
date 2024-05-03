# Comparing `tmp/hmx-v2-python-1.1.0.tar.gz` & `tmp/hmx-v2-python-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmx-v2-python-1.1.0.tar", last modified: Tue Apr 23 11:48:28 2024, max compression
+gzip compressed data, was "hmx-v2-python-1.2.0.tar", last modified: Fri May  3 14:46:09 2024, max compression
```

## Comparing `hmx-v2-python-1.1.0.tar` & `hmx-v2-python-1.2.0.tar`

### file list

```diff
@@ -1,75 +1,81 @@
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.150835 hmx-v2-python-1.1.0/
--rw-r--r--   0 adirut     (501) staff       (20)     1064 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/LICENSE
--rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-04-23 11:48:28.151065 hmx-v2-python-1.1.0/PKG-INFO
--rw-r--r--   0 adirut     (501) staff       (20)     3361 2024-04-14 03:17:48.000000 hmx-v2-python-1.1.0/README.md
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.139582 hmx-v2-python-1.1.0/hmx2/
--rw-r--r--   0 adirut     (501) staff       (20)       35 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.143667 hmx-v2-python-1.1.0/hmx2/abis/
--rw-r--r--   0 adirut     (501) staff       (20)     6094 2023-12-01 07:58:15.000000 hmx-v2-python-1.1.0/hmx2/abis/CIXPriceAdapter.json
--rw-r--r--   0 adirut     (501) staff       (20)    19788 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/abis/Calculator.json
--rw-r--r--   0 adirut     (501) staff       (20)    79531 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/ConfigStorage.json
--rw-r--r--   0 adirut     (501) staff       (20)    23809 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/CrossMarginHandler.json
--rw-r--r--   0 adirut     (501) staff       (20)     3685 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/ERC20.json
--rw-r--r--   0 adirut     (501) staff       (20)    11832 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/GlpManager.json
--rw-r--r--   0 adirut     (501) staff       (20)     5780 2023-12-01 07:58:15.000000 hmx-v2-python-1.1.0/hmx2/abis/GmPriceAdapter.json
--rw-r--r--   0 adirut     (501) staff       (20)    47380 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/LimitTradeHandler.json
--rw-r--r--   0 adirut     (501) staff       (20)     2419 2024-01-15 08:58:17.000000 hmx-v2-python-1.1.0/hmx2/abis/OnchainPricelens.json
--rw-r--r--   0 adirut     (501) staff       (20)    26127 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/PerpStorage.json
--rw-r--r--   0 adirut     (501) staff       (20)    27073 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/abis/TradeHelper.json
--rw-r--r--   0 adirut     (501) staff       (20)    24329 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/abis/VaultStorage.json
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.144902 hmx-v2-python-1.1.0/hmx2/constants/
--rw-r--r--   0 adirut     (501) staff       (20)      107 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     2053 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/assets.py
--rw-r--r--   0 adirut     (501) staff       (20)      330 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/common.py
--rw-r--r--   0 adirut     (501) staff       (20)     1769 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/contracts.py
--rw-r--r--   0 adirut     (501) staff       (20)       52 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/intent.py
--rw-r--r--   0 adirut     (501) staff       (20)     7448 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/markets.py
--rw-r--r--   0 adirut     (501) staff       (20)    10909 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/pricefeed.py
--rw-r--r--   0 adirut     (501) staff       (20)    10061 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/constants/tokens.py
--rw-r--r--   0 adirut     (501) staff       (20)      237 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/enum.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.145640 hmx-v2-python-1.1.0/hmx2/helpers/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/helpers/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)      347 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/helpers/contract_loader.py
--rw-r--r--   0 adirut     (501) staff       (20)      519 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/helpers/mapper.py
--rw-r--r--   0 adirut     (501) staff       (20)      741 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/helpers/util.py
--rw-r--r--   0 adirut     (501) staff       (20)     2771 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/hmx_client.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.145943 hmx-v2-python-1.1.0/hmx2/modules/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/modules/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.146163 hmx-v2-python-1.1.0/hmx2/modules/calculator/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/modules/calculator/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     6048 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/calculator/calculator.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.146789 hmx-v2-python-1.1.0/hmx2/modules/oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       48 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.147137 hmx-v2-python-1.1.0/hmx2/modules/oracle/cix_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 07:58:15.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/cix_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1315 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/cix_oracle/cix_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.147500 hmx-v2-python-1.1.0/hmx2/modules/oracle/glp_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/glp_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1003 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/glp_oracle/glp_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.147853 hmx-v2-python-1.1.0/hmx2/modules/oracle/gm_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       32 2023-12-01 07:58:15.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/gm_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1169 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/gm_oracle/gm_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.148523 hmx-v2-python-1.1.0/hmx2/modules/oracle/onchain_pricelens_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       59 2024-01-15 08:58:17.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)      788 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
--rw-r--r--   0 adirut     (501) staff       (20)     3321 2024-04-14 03:17:48.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/oracle_middleware.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.148781 hmx-v2-python-1.1.0/hmx2/modules/oracle/pyth_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       36 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/pyth_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1302 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
--rw-r--r--   0 adirut     (501) staff       (20)    19733 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/modules/private.py
--rw-r--r--   0 adirut     (501) staff       (20)    29817 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/hmx2/modules/public.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.149469 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/
--rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-04-23 11:48:28.000000 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/PKG-INFO
--rw-r--r--   0 adirut     (501) staff       (20)     1777 2024-04-23 11:48:28.000000 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/SOURCES.txt
--rw-r--r--   0 adirut     (501) staff       (20)        1 2024-04-23 11:48:28.000000 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/dependency_links.txt
--rw-r--r--   0 adirut     (501) staff       (20)      172 2024-04-23 11:48:28.000000 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/requires.txt
--rw-r--r--   0 adirut     (501) staff       (20)       11 2024-04-23 11:48:28.000000 hmx-v2-python-1.1.0/hmx_v2_python.egg-info/top_level.txt
--rw-r--r--   0 adirut     (501) staff       (20)       79 2024-04-23 11:48:28.151303 hmx-v2-python-1.1.0/setup.cfg
--rw-r--r--   0 adirut     (501) staff       (20)     1481 2024-04-23 11:48:11.000000 hmx-v2-python-1.1.0/setup.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-23 11:48:28.150726 hmx-v2-python-1.1.0/tests/
--rw-r--r--   0 adirut     (501) staff       (20)       46 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/tests/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     5934 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/tests/constants.py
--rw-r--r--   0 adirut     (501) staff       (20)     3117 2024-03-22 14:32:06.000000 hmx-v2-python-1.1.0/tests/test_create_market_order.py
--rw-r--r--   0 adirut     (501) staff       (20)     5522 2024-04-14 03:17:48.000000 hmx-v2-python-1.1.0/tests/test_deposit_collateral.py
--rw-r--r--   0 adirut     (501) staff       (20)     1307 2024-03-18 08:59:51.000000 hmx-v2-python-1.1.0/tests/test_get_adaptive_fee.py
--rw-r--r--   0 adirut     (501) staff       (20)     1221 2023-12-01 04:47:34.000000 hmx-v2-python-1.1.0/tests/test_init.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.988059 hmx-v2-python-1.2.0/
+-rw-r--r--   0 adirut     (501) staff       (20)     1064 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/LICENSE
+-rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-05-03 14:46:09.988295 hmx-v2-python-1.2.0/PKG-INFO
+-rw-r--r--   0 adirut     (501) staff       (20)     3361 2024-04-14 03:17:48.000000 hmx-v2-python-1.2.0/README.md
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.976149 hmx-v2-python-1.2.0/hmx2/
+-rw-r--r--   0 adirut     (501) staff       (20)       35 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.980510 hmx-v2-python-1.2.0/hmx2/abis/
+-rw-r--r--   0 adirut     (501) staff       (20)     2918 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/abis/AdaptiveFeeCalculator.json
+-rw-r--r--   0 adirut     (501) staff       (20)     6094 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.0/hmx2/abis/CIXPriceAdapter.json
+-rw-r--r--   0 adirut     (501) staff       (20)     3332 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/abis/CalcPricelens.json
+-rw-r--r--   0 adirut     (501) staff       (20)    19788 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/abis/Calculator.json
+-rw-r--r--   0 adirut     (501) staff       (20)    79643 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/abis/ConfigStorage.json
+-rw-r--r--   0 adirut     (501) staff       (20)    23809 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/abis/CrossMarginHandler.json
+-rw-r--r--   0 adirut     (501) staff       (20)     3685 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/abis/ERC20.json
+-rw-r--r--   0 adirut     (501) staff       (20)    11832 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/abis/GlpManager.json
+-rw-r--r--   0 adirut     (501) staff       (20)     5780 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.0/hmx2/abis/GmPriceAdapter.json
+-rw-r--r--   0 adirut     (501) staff       (20)    47380 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/abis/LimitTradeHandler.json
+-rw-r--r--   0 adirut     (501) staff       (20)     2419 2024-01-15 08:58:17.000000 hmx-v2-python-1.2.0/hmx2/abis/OnchainPricelens.json
+-rw-r--r--   0 adirut     (501) staff       (20)     6721 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/abis/OrderbookOracle.json
+-rw-r--r--   0 adirut     (501) staff       (20)    26489 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/abis/PerpStorage.json
+-rw-r--r--   0 adirut     (501) staff       (20)    27073 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/abis/TradeHelper.json
+-rw-r--r--   0 adirut     (501) staff       (20)    24329 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/abis/VaultStorage.json
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.981786 hmx-v2-python-1.2.0/hmx2/constants/
+-rw-r--r--   0 adirut     (501) staff       (20)      107 2024-04-23 11:48:11.000000 hmx-v2-python-1.2.0/hmx2/constants/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     2146 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/assets.py
+-rw-r--r--   0 adirut     (501) staff       (20)      397 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/common.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3263 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/contracts.py
+-rw-r--r--   0 adirut     (501) staff       (20)       52 2024-04-23 11:48:11.000000 hmx-v2-python-1.2.0/hmx2/constants/intent.py
+-rw-r--r--   0 adirut     (501) staff       (20)    14585 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/markets.py
+-rw-r--r--   0 adirut     (501) staff       (20)    20697 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/pricefeed.py
+-rw-r--r--   0 adirut     (501) staff       (20)    13833 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/tokens.py
+-rw-r--r--   0 adirut     (501) staff       (20)      237 2024-04-23 11:48:11.000000 hmx-v2-python-1.2.0/hmx2/enum.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.982230 hmx-v2-python-1.2.0/hmx2/helpers/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/helpers/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)      347 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/helpers/contract_loader.py
+-rw-r--r--   0 adirut     (501) staff       (20)      993 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/helpers/mapper.py
+-rw-r--r--   0 adirut     (501) staff       (20)      917 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/helpers/util.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3002 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/hmx_client.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.982609 hmx-v2-python-1.2.0/hmx2/modules/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/modules/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.982849 hmx-v2-python-1.2.0/hmx2/modules/calculator/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/modules/calculator/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     8423 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/calculator/calculator.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.983170 hmx-v2-python-1.2.0/hmx2/modules/oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       48 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.983424 hmx-v2-python-1.2.0/hmx2/modules/oracle/calc_pricelens_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       55 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/calc_pricelens_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1209 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.983731 hmx-v2-python-1.2.0/hmx2/modules/oracle/cix_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/cix_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1315 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/cix_oracle/cix_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.984234 hmx-v2-python-1.2.0/hmx2/modules/oracle/glp_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/glp_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1428 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/glp_oracle/glp_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.984532 hmx-v2-python-1.2.0/hmx2/modules/oracle/gm_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       32 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/gm_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1169 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/gm_oracle/gm_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.985031 hmx-v2-python-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       59 2024-01-15 08:58:17.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)      788 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3980 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/oracle_middleware.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.985424 hmx-v2-python-1.2.0/hmx2/modules/oracle/pyth_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       36 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/pyth_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1302 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
+-rw-r--r--   0 adirut     (501) staff       (20)    19728 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/private.py
+-rw-r--r--   0 adirut     (501) staff       (20)    41224 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/public.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.986247 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/
+-rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-05-03 14:46:09.000000 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/PKG-INFO
+-rw-r--r--   0 adirut     (501) staff       (20)     1995 2024-05-03 14:46:09.000000 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/SOURCES.txt
+-rw-r--r--   0 adirut     (501) staff       (20)        1 2024-05-03 14:46:09.000000 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/dependency_links.txt
+-rw-r--r--   0 adirut     (501) staff       (20)      161 2024-05-03 14:46:09.000000 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/requires.txt
+-rw-r--r--   0 adirut     (501) staff       (20)       11 2024-05-03 14:46:09.000000 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/top_level.txt
+-rw-r--r--   0 adirut     (501) staff       (20)       79 2024-05-03 14:46:09.988589 hmx-v2-python-1.2.0/setup.cfg
+-rw-r--r--   0 adirut     (501) staff       (20)     1464 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/setup.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.987894 hmx-v2-python-1.2.0/tests/
+-rw-r--r--   0 adirut     (501) staff       (20)       46 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/tests/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     5934 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/tests/constants.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3117 2024-03-22 14:32:06.000000 hmx-v2-python-1.2.0/tests/test_create_market_order.py
+-rw-r--r--   0 adirut     (501) staff       (20)     5522 2024-04-14 03:17:48.000000 hmx-v2-python-1.2.0/tests/test_deposit_collateral.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1307 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/tests/test_get_adaptive_fee.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1221 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/tests/test_init.py
```

### Comparing `hmx-v2-python-1.1.0/LICENSE` & `hmx-v2-python-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/PKG-INFO` & `hmx-v2-python-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python
-Version: 1.1.0
+Version: 1.2.0
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Platform: UNKNOWN
```

### Comparing `hmx-v2-python-1.1.0/README.md` & `hmx-v2-python-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/CIXPriceAdapter.json` & `hmx-v2-python-1.2.0/hmx2/abis/CIXPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/Calculator.json` & `hmx-v2-python-1.2.0/hmx2/abis/Calculator.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/ConfigStorage.json` & `hmx-v2-python-1.2.0/hmx2/abis/ConfigStorage.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8986810551558754%*

 * *Differences: {'111': "{'inputs': {insert: [(2, OrderedDict([('name', '_isAdaptiveFeeEnabled'), ('internalType', "*

 * *        "'bool'), ('type', 'bool')]))]}}",*

 * * '46': "{'inputs': {insert: [(1, OrderedDict([('name', '_isAdaptiveFeeEnabled'), ('internalType', "*

 * *       "'bool'), ('type', 'bool')]))]}}",*

 * * 'insert': "[(30, OrderedDict([('type', 'event'), ('anonymous', False), ('inputs', "*

 * *           "[OrderedDict([('name', 'marketIndex'), ('internalType', 'uint256'), ('type', "*

 * *           "'uint256'), ('indexed', False)]), Orde […]*

```diff
@@ -782,14 +782,39 @@
             {
                 "indexed": false,
                 "internalType": "uint256",
                 "name": "marketIndex",
                 "type": "uint256"
             },
             {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "makerFee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "takerFee",
+                "type": "uint256"
+            }
+        ],
+        "name": "LogSetMakerTakerFee",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            },
+            {
                 "components": [
                     {
                         "internalType": "bytes32",
                         "name": "assetId",
                         "type": "bytes32"
                     },
                     {
@@ -1031,14 +1056,50 @@
         "name": "LogSetServiceExecutor",
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "index",
+                "type": "uint256"
+            },
+            {
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "fromSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "toSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "minProfitDuration",
+                        "type": "uint256"
+                    }
+                ],
+                "indexed": false,
+                "internalType": "struct IConfigStorage.StepMinProfitDuration",
+                "name": "_stepMinProfitDuration",
+                "type": "tuple"
+            }
+        ],
+        "name": "LogSetStepMinProfitDuration",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
                 "components": [
                     {
                         "internalType": "uint32",
                         "name": "stablecoinSwapFeeRateBPS",
                         "type": "uint32"
                     },
                     {
@@ -1341,14 +1402,19 @@
                         "name": "fundingRate",
                         "type": "tuple"
                     }
                 ],
                 "internalType": "struct IConfigStorage.MarketConfig",
                 "name": "_newConfig",
                 "type": "tuple"
+            },
+            {
+                "internalType": "bool",
+                "name": "_isAdaptiveFeeEnabled",
+                "type": "bool"
             }
         ],
         "name": "addMarketConfig",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "_newMarketIndex",
@@ -1397,14 +1463,44 @@
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "fromSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "toSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "minProfitDuration",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct IConfigStorage.StepMinProfitDuration[]",
+                "name": "_stepMinProfitDurations",
+                "type": "tuple[]"
+            }
+        ],
+        "name": "addStepMinProfitDuration",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
         "name": "allowedLiquidators",
         "outputs": [
@@ -2164,14 +2260,68 @@
                 "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "sizeDelta",
+                "type": "uint256"
+            }
+        ],
+        "name": "getStepMinProfitDuration",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "getStepMinProfitDurations",
+        "outputs": [
+            {
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "fromSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "toSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "minProfitDuration",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct IConfigStorage.StepMinProfitDuration[]",
+                "name": "",
+                "type": "tuple[]"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [],
         "name": "getTradeServiceHooks",
         "outputs": [
             {
                 "internalType": "address[]",
                 "name": "",
                 "type": "address[]"
@@ -2251,14 +2401,52 @@
         "inputs": [],
         "name": "initialize",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            }
+        ],
+        "name": "isAdaptiveFeeEnabledByMarketIndex",
+        "outputs": [
+            {
+                "internalType": "bool",
+                "name": "isEnabled",
+                "type": "bool"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            }
+        ],
+        "name": "isStepMinProfitEnabledByMarketIndex",
+        "outputs": [
+            {
+                "internalType": "bool",
+                "name": "isStepMinProfitEnabled",
+                "type": "bool"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [],
         "name": "liquidationConfig",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "liquidationFeeUSDE30",
                 "type": "uint256"
@@ -2320,14 +2508,33 @@
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            }
+        ],
+        "name": "makerFeeE8ByMarketIndex",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "makerFeeE8",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
         "name": "marketConfigs",
         "outputs": [
             {
@@ -2488,14 +2695,21 @@
         "name": "removeAcceptedToken",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [],
+        "name": "removeLastStepMinProfitDuration",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [],
         "name": "renounceOwnership",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
@@ -2871,14 +3085,32 @@
         ],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "uint256[]",
+                "name": "marketIndexes",
+                "type": "uint256[]"
+            },
+            {
+                "internalType": "bool[]",
+                "name": "isEnableds",
+                "type": "bool[]"
+            }
+        ],
+        "name": "setIsStepMinProfitEnabledByMarketIndex",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "liquidationFeeUSDE30",
                         "type": "uint256"
                     }
                 ],
@@ -2964,14 +3196,37 @@
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "uint256[]",
+                "name": "marketIndexes",
+                "type": "uint256[]"
+            },
+            {
+                "internalType": "uint256[]",
+                "name": "makerFees",
+                "type": "uint256[]"
+            },
+            {
+                "internalType": "uint256[]",
+                "name": "takerFees",
+                "type": "uint256[]"
+            }
+        ],
+        "name": "setMakerTakerFeeByMarketIndexes",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "internalType": "uint256",
                 "name": "_marketIndex",
                 "type": "uint256"
             },
             {
                 "components": [
                     {
@@ -3046,14 +3301,19 @@
                         "name": "fundingRate",
                         "type": "tuple"
                     }
                 ],
                 "internalType": "struct IConfigStorage.MarketConfig",
                 "name": "_newConfig",
                 "type": "tuple"
+            },
+            {
+                "internalType": "bool",
+                "name": "_isAdaptiveFeeEnabled",
+                "type": "bool"
             }
         ],
         "name": "setMarketConfig",
         "outputs": [
             {
                 "components": [
                     {
@@ -3252,14 +3512,49 @@
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "uint256[]",
+                "name": "indexes",
+                "type": "uint256[]"
+            },
+            {
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "fromSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "toSize",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "minProfitDuration",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct IConfigStorage.StepMinProfitDuration[]",
+                "name": "_stepMinProfitDurations",
+                "type": "tuple[]"
+            }
+        ],
+        "name": "setStepMinProfitDuration",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "components": [
                     {
                         "internalType": "uint32",
                         "name": "stablecoinSwapFeeRateBPS",
                         "type": "uint32"
                     },
                     {
@@ -3362,14 +3657,43 @@
                 "type": "address"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "name": "stepMinProfitDurations",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "fromSize",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "toSize",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "minProfitDuration",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [],
         "name": "swapConfig",
         "outputs": [
             {
                 "internalType": "uint32",
                 "name": "stablecoinSwapFeeRateBPS",
                 "type": "uint32"
@@ -3394,14 +3718,33 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            }
+        ],
+        "name": "takerFeeE8ByMarketIndex",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "takerFeeE8",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
             {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
         "name": "tokenAssetIds",
```

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/CrossMarginHandler.json` & `hmx-v2-python-1.2.0/hmx2/abis/CrossMarginHandler.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/ERC20.json` & `hmx-v2-python-1.2.0/hmx2/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/GlpManager.json` & `hmx-v2-python-1.2.0/hmx2/abis/GlpManager.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/GmPriceAdapter.json` & `hmx-v2-python-1.2.0/hmx2/abis/GmPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/LimitTradeHandler.json` & `hmx-v2-python-1.2.0/hmx2/abis/LimitTradeHandler.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/OnchainPricelens.json` & `hmx-v2-python-1.2.0/hmx2/abis/OnchainPricelens.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/PerpStorage.json` & `hmx-v2-python-1.2.0/hmx2/abis/PerpStorage.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8297872340425532%*

 * *Differences: {'insert': "[(4, OrderedDict([('type', 'event'), ('anonymous', False), ('inputs', "*

 * *           "[OrderedDict([('name', 'length'), ('internalType', 'uint256'), ('type', 'uint256'), "*

 * *           "('indexed', False)]), OrderedDict([('name', 'interval'), ('internalType', 'uint256'), "*

 * *           "('type', 'uint256'), ('indexed', False)])]), ('name', 'LogSetMovingWindowConfig')])), "*

 * *           "(10, OrderedDict([('stateMutability', 'view'), ('type', 'function'), ('inputs', "*

 * *           "[OrderedDict([('name', ' […]*

```diff
@@ -27,14 +27,33 @@
         "name": "Initialized",
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "length",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "interval",
+                "type": "uint256"
+            }
+        ],
+        "name": "LogSetMovingWindowConfig",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
                 "indexed": true,
                 "internalType": "address",
                 "name": "executorAddress",
                 "type": "address"
             },
             {
                 "indexed": false,
@@ -145,14 +164,62 @@
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "timestamp",
+                "type": "uint256"
+            }
+        ],
+        "name": "epochVolumeBuy",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "buyVolume",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "timestamp",
+                "type": "uint256"
+            }
+        ],
+        "name": "epochVolumeSell",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "sellVolume",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "uint256",
                 "name": "_limit",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
                 "name": "_offset",
                 "type": "uint256"
@@ -312,14 +379,38 @@
                 "type": "tuple"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [
+            {
+                "internalType": "bool",
+                "name": "isBuy",
+                "type": "bool"
+            },
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            }
+        ],
+        "name": "getEpochVolume",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "epochVolume",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [],
         "name": "getGlobalState",
         "outputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
@@ -603,14 +694,37 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "bool",
+                "name": "isBuy",
+                "type": "bool"
+            },
+            {
+                "internalType": "uint256",
+                "name": "marketIndex",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "absSizeDelta",
+                "type": "uint256"
+            }
+        ],
+        "name": "increaseEpochVolume",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "internalType": "uint256",
                 "name": "_marketIndex",
                 "type": "uint256"
             },
             {
                 "internalType": "bool",
                 "name": "_isLong",
@@ -701,14 +815,40 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
+        "name": "movingWindowInterval",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "movingWindowLength",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
         "name": "owner",
         "outputs": [
             {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
@@ -898,14 +1038,32 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "uint256",
+                "name": "length",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "interval",
+                "type": "uint256"
+            }
+        ],
+        "name": "setMovingWindowConfig",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
                 "internalType": "address[]",
                 "name": "_executorAddresses",
                 "type": "address[]"
             },
             {
                 "internalType": "bool[]",
                 "name": "_isServiceExecutors",
```

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/TradeHelper.json` & `hmx-v2-python-1.2.0/hmx2/abis/TradeHelper.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/abis/VaultStorage.json` & `hmx-v2-python-1.2.0/hmx2/abis/VaultStorage.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/constants/assets.py` & `hmx-v2-python-1.2.0/hmx2/constants/assets.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,19 +57,22 @@
 ASSET_ICP = "ICP"
 ASSET_MANTA = "MANTA"
 ASSET_STRK = "STRK"
 ASSET_PYTH = "PYTH"
 ASSET_PENDLE = "PENDLE"
 ASSET_W = "W"
 ASSET_ENA = "ENA"
+ASSET_ybUSDB = "ybUSDB"
+ASSET_ybETH = "ybETH"
+ASSET_USDB = "USDB"
 
 ASSETS = [ASSET_ETH, ASSET_BTC, ASSET_AAPL, ASSET_JPY, ASSET_XAU, ASSET_AMZN,
           ASSET_MSFT, ASSET_TSLA, ASSET_EUR, ASSET_XAG, ASSET_AUD, ASSET_GBP,
           ASSET_ADA, ASSET_MATIC, ASSET_SUI, ASSET_ARB, ASSET_OP, ASSET_LTC,
           ASSET_COIN, ASSET_GOOG, ASSET_BNB, ASSET_SOL, ASSET_QQQ, ASSET_XRP,
           ASSET_USDC, ASSET_USDT, ASSET_DAI, ASSET_GLP, ASSET_NVDA, ASSET_LINK,
           ASSET_CHF, ASSET_DOGE, ASSET_CAD, ASSET_SGD, ASSET_CNH, ASSET_wstETH,
           ASSET_HKD, ASSET_BCH, ASSET_MEME, ASSET_gmBTC, ASSET_gmETH, ASSET_SEK,
           ASSET_DIX, ASSET_JTO, ASSET_STX, ASSET_ORDI, ASSET_TIA, ASSET_AVAX,
           ASSET_INJ, ASSET_DOT, ASSET_SEI, ASSET_ATOM, ASSET_1000SHIB, ASSET_1000PEPE,
           ASSET_ICP, ASSET_MANTA, ASSET_STRK, ASSET_PYTH, ASSET_USDCe, ASSET_PENDLE,
-          ASSET_W, ASSET_ENA]
+          ASSET_W, ASSET_ENA, ASSET_ybUSDB, ASSET_ybETH]
```

### Comparing `hmx-v2-python-1.1.0/hmx2/constants/pricefeed.py` & `hmx-v2-python-1.2.0/hmx2/constants/pricefeed.py`

 * *Files 21% similar despite different names*

```diff
@@ -181,9 +181,127 @@
     ASSET_ICP: "0xc9907d786c5821547777780a1e4f89484f3417cb14dd244f2b0a34ea7a554d67",
     ASSET_MANTA: "0xc3883bcf1101c111e9fcfe2465703c47f2b638e21fef2cce0502e6c8f416e0e2",
     ASSET_STRK: "0x6a182399ff70ccf3e06024898942028204125a819e519a335ffa4579e66cd870",
     ASSET_PYTH: "0x0bbf28e9a841a1cc788f6a361b17ca072d0ea3098a1e5df1c3922d06719579ff",
     ASSET_W: "0xeff7446475e218517566ea99e72a4abec2e1bd8498b43b7d8331e29dcb059389",
     ASSET_PENDLE: "0x9a4df90b25497f66b1afb012467e316e801ca3d839456db028892fe8c70c8016",
     ASSET_ENA: "0xb7910ba7322db020416fcac28b48c01212fd9cc8fbcbaf7d30477ed8605f6bd4",
+  },
+  81457: {
+    ASSET_ETH: "0xff61491a931112ddf1bd8147cd1b641375f79f5825126d665480874634fd0ace",
+    ASSET_BTC: "0xe62df6c8b4a85fe1a67db44dc12de5db330f7ac66b72dc658afedf0f4a415b43",
+    ASSET_DAI: "0xb0948a5e5313200c632b51bb5ca32f6de0d36e9950a942d19751e833f70dabfd",
+    ASSET_USDC: "0xeaa020c61cc479712813461ce153894a96a6c00b21ed0cfc2798d1f9a9e9c94a",
+    ASSET_USDT: "0x2b89b9dc8fdf9f34709a5b106b472f0f39bb6ca9ce04b0fd7f2e971688e2e53b",
+    ASSET_AAPL: "0x49f6b65cb1de6b10eaf75e7c03ca029c306d0357e91b5311b175084a5ad55688",
+    ASSET_XAU: "0x765d2ba906dbc32ca17cc11f5310a89e9ee1f6420508c63861f2f8ba4ee34bb2",
+    ASSET_JPY: "0xef2c98c804ba503c6a707e38be4dfbb16683775f195b091252bf24693042fd52",
+    ASSET_AMZN: "0xb5d0e0fa58a1f8b81498ae670ce93c872d14434b72c364885d4fa1b257cbb07a",
+    ASSET_MSFT: "0xd0ca23c1cc005e004ccf1db5bf76aeb6a49218f43dac3d4b275e92de12ded4d1",
+    ASSET_TSLA: "0x16dad506d7db8da01c87581c87ca897a012a153557d4d578c3b9c9e1bc0632f1",
+    ASSET_EUR: "0xa995d00bb36a63cef7fd2c287dc105fc8f3d93779f062f09551b0af3e81ec30b",
+    ASSET_XAG: "0xf2fb02c32b055c805e7238d628e5e9dadef274376114eb1f012337cabe93871e",
+    ASSET_AUD: "0x67a6f93030420c1c9e3fe37c1ab6b77966af82f995944a9fefce357a22854a80",
+    ASSET_GBP: "0x84c2dde9633d93d1bcad84e7dc41c9d56578b7ec52fabedc1f335d673df0a7c1",
+    ASSET_ADA: "0x2a01deaec9e51a579277b34b122399984d0bbf57e2458a7e42fecd2829867a0d",
+    ASSET_MATIC: "0x5de33a9112c2b700b8d30b8a3402c103578ccfa2765696471cc672bd5cf6ac52",
+    ASSET_SUI: "0x23d7315113f5b1d3ba7a83604c44b94d79f4fd69af77f804fc7f920a6dc65744",
+    ASSET_ARB: "0x3fa4252848f9f0a1480be62745a4629d9eb1322aebab8a791e344b3b9c1adcf5",
+    ASSET_OP: "0x385f64d993f7b77d8182ed5003d97c60aa3361f3cecfe711544d2d59165e9bdf",
+    ASSET_LTC: "0x6e3f3fa8253588df9326580180233eb791e03b443a3ba7a1d892e73874e19a54",
+    ASSET_COIN: "0xfee33f2a978bf32dd6b662b65ba8083c6773b494f8401194ec1870c640860245",
+    ASSET_GOOG: "0xe65ff435be42630439c96396653a342829e877e2aafaeaf1a10d0ee5fd2cf3f2",
+    ASSET_BNB: "0x2f95862b045670cd22bee3114c39763a4a08beeb663b145d283c31d7d1101c4f",
+    ASSET_SOL: "0xef0d8b6fda2ceba41da15d4095d1da392a0d2f8ed0c6c7bc0f4cfac8c280b56d",
+    ASSET_QQQ: "0x9695e2b96ea7b3859da9ed25b7a46a920a776e2fdae19a7bcfdf2b219230452d",
+    ASSET_XRP: "0xec5d399846a9209f3fe5881d70aae9268c94339ff9817e8d18ff19fa05eea1c8",
+    ASSET_NVDA: "0xb1073854ed24cbc755dc527418f52b7d271f6cc967bbf8d8129112b18860a593",
+    ASSET_LINK: "0x8ac0c70fff57e9aefdf5edf44b51d62c2d433653cbb2cf5cc06bb115af04d221",
+    ASSET_CHF: "0x0b1e3297e69f162877b577b0d6a47a0d63b2392bc8499e6540da4187a63e28f8",
+    ASSET_DOGE: "0xdcef50dd0a4cd2dcc17e45df1676dcb336a11a61c69df7a0299b0150c672d25c",
+    ASSET_CAD: "0x3112b03a41c910ed446852aacf67118cb1bec67b2cd0b9a214c58cc0eaa2ecca",
+    ASSET_SGD: "0x396a969a9c1480fa15ed50bc59149e2c0075a72fe8f458ed941ddec48bdb4918",
+    ASSET_CNH: "0xeef52e09c878ad41f6a81803e3640fe04dceea727de894edd4ea117e2e332e66",
+    ASSET_HKD: "0x19d75fde7fee50fe67753fdc825e583594eb2f51ae84e114a5246c4ab23aff4c",
+    ASSET_BCH: "0x3dd2b63686a450ec7290df3a1e0b583c0481f651351edfa7636f39aed55cf8a3",
+    ASSET_MEME: "0xcd2cee36951a571e035db0dfad138e6ecdb06b517cc3373cd7db5d3609b7927c",
+    ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
+    ASSET_JTO: "0xb43660a5f790c69354b0729a5ef9d50d68f1df92107540210b9cccba1f947cc2",
+    ASSET_STX: "0xec7a775f46379b5e943c3526b1c8d54cd49749176b0b98e02dde68d1bd335c17",
+    ASSET_ORDI: "0x193c739db502aadcef37c2589738b1e37bdb257d58cf1ab3c7ebc8e6df4e3ec0",
+    ASSET_TIA: "0x09f7c1d7dfbb7df2b8fe3d3d87ee94a2259d212da4f30c1f0540d066dfa44723",
+    ASSET_AVAX: "0x93da3352f9f1d105fdfe4971cfa80e9dd777bfc5d0f683ebb6e1294b92137bb7",
+    ASSET_INJ: "0x7a5bc1d2b56ad029048cd63964b3ad2776eadf812edc1a43a31406cb54bff592",
+    ASSET_DOT: "0xca3eed9b267293f6595901c734c7525ce8ef49adafe8284606ceb307afa2ca5b",
+    ASSET_SEI: "0x53614f1cb0c031d4af66c04cb9c756234adad0e1cee85303795091499a4084eb",
+    ASSET_ATOM: "0xb00b60f88b03a6a625a8d1c048c3f66653edf217439983d037e7222c4e612819",
+    ASSET_1000SHIB: "0xf0d57deca57b3da2fe63a493f4c25925fdfd8edf834b20f93e1f84dbd1504d4a",
+    ASSET_1000PEPE: "0xd69731a2e74ac1ce884fc3890f7ee324b6deb66147055249568869ed700882e4",
+    ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
+    ASSET_ICP: "0xc9907d786c5821547777780a1e4f89484f3417cb14dd244f2b0a34ea7a554d67",
+    ASSET_MANTA: "0xc3883bcf1101c111e9fcfe2465703c47f2b638e21fef2cce0502e6c8f416e0e2",
+    ASSET_STRK: "0x6a182399ff70ccf3e06024898942028204125a819e519a335ffa4579e66cd870",
+    ASSET_PYTH: "0x0bbf28e9a841a1cc788f6a361b17ca072d0ea3098a1e5df1c3922d06719579ff",
+    ASSET_W: "0xeff7446475e218517566ea99e72a4abec2e1bd8498b43b7d8331e29dcb059389",
+    ASSET_PENDLE: "0x9a4df90b25497f66b1afb012467e316e801ca3d839456db028892fe8c70c8016",
+    ASSET_ENA: "0xb7910ba7322db020416fcac28b48c01212fd9cc8fbcbaf7d30477ed8605f6bd4",
+  },
+  168587773: {
+    ASSET_ETH: "0xff61491a931112ddf1bd8147cd1b641375f79f5825126d665480874634fd0ace",
+    ASSET_BTC: "0xe62df6c8b4a85fe1a67db44dc12de5db330f7ac66b72dc658afedf0f4a415b43",
+    ASSET_DAI: "0xb0948a5e5313200c632b51bb5ca32f6de0d36e9950a942d19751e833f70dabfd",
+    ASSET_USDC: "0xeaa020c61cc479712813461ce153894a96a6c00b21ed0cfc2798d1f9a9e9c94a",
+    ASSET_USDT: "0x2b89b9dc8fdf9f34709a5b106b472f0f39bb6ca9ce04b0fd7f2e971688e2e53b",
+    ASSET_AAPL: "0x49f6b65cb1de6b10eaf75e7c03ca029c306d0357e91b5311b175084a5ad55688",
+    ASSET_XAU: "0x765d2ba906dbc32ca17cc11f5310a89e9ee1f6420508c63861f2f8ba4ee34bb2",
+    ASSET_JPY: "0xef2c98c804ba503c6a707e38be4dfbb16683775f195b091252bf24693042fd52",
+    ASSET_AMZN: "0xb5d0e0fa58a1f8b81498ae670ce93c872d14434b72c364885d4fa1b257cbb07a",
+    ASSET_MSFT: "0xd0ca23c1cc005e004ccf1db5bf76aeb6a49218f43dac3d4b275e92de12ded4d1",
+    ASSET_TSLA: "0x16dad506d7db8da01c87581c87ca897a012a153557d4d578c3b9c9e1bc0632f1",
+    ASSET_EUR: "0xa995d00bb36a63cef7fd2c287dc105fc8f3d93779f062f09551b0af3e81ec30b",
+    ASSET_XAG: "0xf2fb02c32b055c805e7238d628e5e9dadef274376114eb1f012337cabe93871e",
+    ASSET_AUD: "0x67a6f93030420c1c9e3fe37c1ab6b77966af82f995944a9fefce357a22854a80",
+    ASSET_GBP: "0x84c2dde9633d93d1bcad84e7dc41c9d56578b7ec52fabedc1f335d673df0a7c1",
+    ASSET_ADA: "0x2a01deaec9e51a579277b34b122399984d0bbf57e2458a7e42fecd2829867a0d",
+    ASSET_MATIC: "0x5de33a9112c2b700b8d30b8a3402c103578ccfa2765696471cc672bd5cf6ac52",
+    ASSET_SUI: "0x23d7315113f5b1d3ba7a83604c44b94d79f4fd69af77f804fc7f920a6dc65744",
+    ASSET_ARB: "0x3fa4252848f9f0a1480be62745a4629d9eb1322aebab8a791e344b3b9c1adcf5",
+    ASSET_OP: "0x385f64d993f7b77d8182ed5003d97c60aa3361f3cecfe711544d2d59165e9bdf",
+    ASSET_LTC: "0x6e3f3fa8253588df9326580180233eb791e03b443a3ba7a1d892e73874e19a54",
+    ASSET_COIN: "0xfee33f2a978bf32dd6b662b65ba8083c6773b494f8401194ec1870c640860245",
+    ASSET_GOOG: "0xe65ff435be42630439c96396653a342829e877e2aafaeaf1a10d0ee5fd2cf3f2",
+    ASSET_BNB: "0x2f95862b045670cd22bee3114c39763a4a08beeb663b145d283c31d7d1101c4f",
+    ASSET_SOL: "0xef0d8b6fda2ceba41da15d4095d1da392a0d2f8ed0c6c7bc0f4cfac8c280b56d",
+    ASSET_QQQ: "0x9695e2b96ea7b3859da9ed25b7a46a920a776e2fdae19a7bcfdf2b219230452d",
+    ASSET_XRP: "0xec5d399846a9209f3fe5881d70aae9268c94339ff9817e8d18ff19fa05eea1c8",
+    ASSET_NVDA: "0xb1073854ed24cbc755dc527418f52b7d271f6cc967bbf8d8129112b18860a593",
+    ASSET_LINK: "0x8ac0c70fff57e9aefdf5edf44b51d62c2d433653cbb2cf5cc06bb115af04d221",
+    ASSET_CHF: "0x0b1e3297e69f162877b577b0d6a47a0d63b2392bc8499e6540da4187a63e28f8",
+    ASSET_DOGE: "0xdcef50dd0a4cd2dcc17e45df1676dcb336a11a61c69df7a0299b0150c672d25c",
+    ASSET_CAD: "0x3112b03a41c910ed446852aacf67118cb1bec67b2cd0b9a214c58cc0eaa2ecca",
+    ASSET_SGD: "0x396a969a9c1480fa15ed50bc59149e2c0075a72fe8f458ed941ddec48bdb4918",
+    ASSET_CNH: "0xeef52e09c878ad41f6a81803e3640fe04dceea727de894edd4ea117e2e332e66",
+    ASSET_HKD: "0x19d75fde7fee50fe67753fdc825e583594eb2f51ae84e114a5246c4ab23aff4c",
+    ASSET_BCH: "0x3dd2b63686a450ec7290df3a1e0b583c0481f651351edfa7636f39aed55cf8a3",
+    ASSET_MEME: "0xcd2cee36951a571e035db0dfad138e6ecdb06b517cc3373cd7db5d3609b7927c",
+    ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
+    ASSET_JTO: "0xb43660a5f790c69354b0729a5ef9d50d68f1df92107540210b9cccba1f947cc2",
+    ASSET_STX: "0xec7a775f46379b5e943c3526b1c8d54cd49749176b0b98e02dde68d1bd335c17",
+    ASSET_ORDI: "0x193c739db502aadcef37c2589738b1e37bdb257d58cf1ab3c7ebc8e6df4e3ec0",
+    ASSET_TIA: "0x09f7c1d7dfbb7df2b8fe3d3d87ee94a2259d212da4f30c1f0540d066dfa44723",
+    ASSET_AVAX: "0x93da3352f9f1d105fdfe4971cfa80e9dd777bfc5d0f683ebb6e1294b92137bb7",
+    ASSET_INJ: "0x7a5bc1d2b56ad029048cd63964b3ad2776eadf812edc1a43a31406cb54bff592",
+    ASSET_DOT: "0xca3eed9b267293f6595901c734c7525ce8ef49adafe8284606ceb307afa2ca5b",
+    ASSET_SEI: "0x53614f1cb0c031d4af66c04cb9c756234adad0e1cee85303795091499a4084eb",
+    ASSET_ATOM: "0xb00b60f88b03a6a625a8d1c048c3f66653edf217439983d037e7222c4e612819",
+    ASSET_1000SHIB: "0xf0d57deca57b3da2fe63a493f4c25925fdfd8edf834b20f93e1f84dbd1504d4a",
+    ASSET_1000PEPE: "0xd69731a2e74ac1ce884fc3890f7ee324b6deb66147055249568869ed700882e4",
+    ASSET_SEK: "0x8ccb376aa871517e807358d4e3cf0bc7fe4950474dbe6c9ffc21ef64e43fc676",
+    ASSET_ICP: "0xc9907d786c5821547777780a1e4f89484f3417cb14dd244f2b0a34ea7a554d67",
+    ASSET_MANTA: "0xc3883bcf1101c111e9fcfe2465703c47f2b638e21fef2cce0502e6c8f416e0e2",
+    ASSET_STRK: "0x6a182399ff70ccf3e06024898942028204125a819e519a335ffa4579e66cd870",
+    ASSET_PYTH: "0x0bbf28e9a841a1cc788f6a361b17ca072d0ea3098a1e5df1c3922d06719579ff",
+    ASSET_W: "0xeff7446475e218517566ea99e72a4abec2e1bd8498b43b7d8331e29dcb059389",
+    ASSET_PENDLE: "0x9a4df90b25497f66b1afb012467e316e801ca3d839456db028892fe8c70c8016",
+    ASSET_ENA: "0xb7910ba7322db020416fcac28b48c01212fd9cc8fbcbaf7d30477ed8605f6bd4",
   }
 }
```

### Comparing `hmx-v2-python-1.1.0/hmx2/helpers/util.py` & `hmx-v2-python-1.2.0/hmx2/helpers/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,7 +25,15 @@
 def check_sub_account_id_param(sub_account_id: int):
   if sub_account_id not in range(0, 256):
     raise Exception("Invalid sub account id")
 
 
 def from_number_to_e30(n: float | int) -> int:
   return math.floor(n * 10 ** 8) * 10 ** 22
+
+
+def from_e30_to_e8(n: float | int) -> int:
+  return math.floor(n / 10 ** 22)
+
+
+def is_blast_chain(chain_id: int) -> bool:
+  return chain_id == 81457 or chain_id == 168587773
```

### Comparing `hmx-v2-python-1.1.0/hmx2/hmx_client.py` & `hmx-v2-python-1.2.0/hmx2/hmx_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from hmx2.modules.private import Private
 from hmx2.modules.public import Public
 from hmx2.modules.oracle.pyth_oracle import PythOracle
 from hmx2.modules.oracle.glp_oracle import GlpOracle
 from hmx2.modules.oracle.cix_oracle import CixOracle
 from hmx2.modules.oracle.gm_oracle import GmOracle
 from hmx2.modules.oracle.onchain_pricelens_oracle import OnchainPricelensOracle
+from hmx2.modules.oracle.calc_pricelens_oracle import CalcPricelensOracle
 from hmx2.modules.oracle.oracle_middleware import OracleMiddleware
 
 
 class Client(object):
   def __init__(self, rpc_url, eth_private_key=None, pyth_price_service_url=DEFAULT_PYTH_PRICE_SERVICE_URL):
     self.__eth_provider = Web3(Web3.HTTPProvider(
       rpc_url, request_kwargs={'timeout': 60}))
@@ -33,16 +34,19 @@
     gm_btc_oracle = GmOracle(contract_address["GM_BTC_PRICE_ADAPTER_ADDRESS"], [
                              ASSET_BTC, ASSET_BTC, ASSET_USDC], pyth_oracle, self.__eth_provider)
     gm_eth_oracle = GmOracle(contract_address["GM_ETH_PRICE_ADAPTER_ADDRESS"], [
         ASSET_ETH, ASSET_ETH, ASSET_USDC], pyth_oracle, self.__eth_provider)
     onchain_pricelens_oracle = OnchainPricelensOracle(
       contract_address["ONCHAIN_PRICELENS_ADDRESS"], pyth_oracle, self.__eth_provider)
 
+    calc_pricelens_oracle = CalcPricelensOracle(
+      contract_address["CALC_PRICELENS_ADDRESS"], pyth_oracle, self.__eth_provider)
+
     self.__oracle_middleware = OracleMiddleware(
-      pyth_oracle, glp_oracle, dix_oracle, gm_btc_oracle, gm_eth_oracle, onchain_pricelens_oracle)
+      pyth_oracle, glp_oracle, dix_oracle, gm_btc_oracle, gm_eth_oracle, onchain_pricelens_oracle, calc_pricelens_oracle)
 
     self.__private = None
     self.__public = Public(
       self.__chain_id, self.__eth_provider, self.__oracle_middleware)
 
   @property
   def public(self):
```

### Comparing `hmx-v2-python-1.1.0/hmx2/modules/oracle/cix_oracle/cix_oracle.py` & `hmx-v2-python-1.2.0/hmx2/modules/oracle/cix_oracle/cix_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/modules/oracle/gm_oracle/gm_oracle.py` & `hmx-v2-python-1.2.0/hmx2/modules/oracle/gm_oracle/gm_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py` & `hmx-v2-python-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/modules/oracle/oracle_middleware.py` & `hmx-v2-python-1.2.0/hmx2/modules/oracle/oracle_middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 from hmx2.modules.oracle.pyth_oracle import PythOracle
 from hmx2.modules.oracle.glp_oracle import GlpOracle
 from hmx2.modules.oracle.cix_oracle import CixOracle
 from hmx2.modules.oracle.gm_oracle import GmOracle
 from hmx2.modules.oracle.onchain_pricelens_oracle import OnchainPricelensOracle
+from hmx2.modules.oracle.calc_pricelens_oracle import CalcPricelensOracle
 from hmx2.constants.assets import (
   ASSETS,
   ASSET_USDCe,
   ASSET_gmBTC,
   ASSET_gmETH,
   ASSET_DIX,
   ASSET_GLP,
   ASSET_wstETH,
   ASSET_1000PEPE,
   ASSET_1000SHIB,
-  ASSET_JPY
+  ASSET_JPY,
+  ASSET_ybETH,
+  ASSET_ybUSDB,
 )
 from typing import List
 
 
 class OracleMiddleware(object):
   def __init__(self, pyth_oracle: PythOracle, glp_oracle: GlpOracle, dix_oracle: CixOracle,
-               gm_btc_oracle: GmOracle, gm_eth_oracle: GmOracle, onchain_pricelens_oracle: OnchainPricelensOracle):
+               gm_btc_oracle: GmOracle, gm_eth_oracle: GmOracle, onchain_pricelens_oracle: OnchainPricelensOracle,
+               calc_pricelens_oracle: CalcPricelensOracle):
     self.glp_oracle = glp_oracle
     self.pyth_oracle = pyth_oracle
     self.dix_oracle = dix_oracle
     self.gm_btc_oracle = gm_btc_oracle
     self.gm_eth_oracle = gm_eth_oracle
     self.onchain_pricelens_oracle = onchain_pricelens_oracle
+    self.calc_pricelens_oracle = calc_pricelens_oracle
 
   def get_price(self, asset_id: str):
     '''
     Get the latest price of the asset.
 
     :param asset_id: required
     :type asset_id: str in list ASSET_IDS
@@ -55,14 +60,17 @@
 
     if asset_id in [ASSET_1000PEPE, ASSET_1000SHIB]:
       return self.pyth_oracle.get_price(asset_id) * 1000
 
     if asset_id in [ASSET_JPY]:
       return 1 / self.pyth_oracle.get_price(asset_id)
 
+    if asset_id in [ASSET_ybETH, ASSET_ybUSDB]:
+      return self.calc_pricelens_oracle.get_price(asset_id)
+
     return self.pyth_oracle.get_price(asset_id)
 
   def get_multiple_price(self, asset_ids: List[str]):
 
     price_object = {}
 
     if set(asset_ids) - set(ASSETS):
@@ -88,14 +96,24 @@
       price_object[ASSET_wstETH] = self.onchain_pricelens_oracle.get_price(
         ASSET_wstETH)
       asset_ids.remove(ASSET_wstETH)
     if ASSET_USDCe in asset_ids:
       price_object[ASSET_USDCe] = self.get_price("USDC")
       asset_ids.remove(ASSET_USDCe)
 
+    if ASSET_ybETH in asset_ids:
+      price_object[ASSET_ybETH] = self.calc_pricelens_oracle.get_price(
+        ASSET_ybETH)
+      asset_ids.remove(ASSET_ybETH)
+
+    if ASSET_ybUSDB in asset_ids:
+      price_object[ASSET_ybUSDB] = self.calc_pricelens_oracle.get_price(
+        ASSET_ybUSDB)
+      asset_ids.remove(ASSET_ybUSDB)
+
     raw_prices = self.pyth_oracle.get_multiple_price(asset_ids)
 
     for index, asset_id in enumerate(asset_ids):
       if asset_id in [ASSET_1000PEPE, ASSET_1000SHIB]:
         price_object[asset_id] = raw_prices[index] * 1000
 
       elif asset_id in [ASSET_JPY]:
```

### Comparing `hmx-v2-python-1.1.0/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py` & `hmx-v2-python-1.2.0/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/hmx2/modules/private.py` & `hmx-v2-python-1.2.0/hmx2/modules/private.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from eth_abi.packed import encode_packed
+from eth_keys import keys
 from web3 import Web3, Account
 from web3.middleware.signing import construct_sign_and_send_raw_middleware
 from web3.logs import DISCARD
 from time import sleep
 from hmx2.constants.contracts import (
   CROSS_MARGIN_HANDLER_ABI_PATH,
   LIMIT_TRADE_HANDLER_ABI_PATH,
@@ -19,21 +20,19 @@
   BPS,
   MAX_UINT54,
   MINUTES
 )
 from hmx2.constants.intent import (
   INTENT_TRADE_API,
 )
-from hmx2.constants.markets import MARKET_PROFILE
 from hmx2.enum import (
   Action,
   Cmd,
 )
 from eth_account import Account
-from secp256k1 import PrivateKey
 
 from eth_account.messages import encode_typed_data
 from time import time
 from hmx2.helpers.contract_loader import load_contract
 from simple_multicall_v6 import Multicall
 from hmx2.helpers.mapper import (
   get_contract_address,
@@ -164,17 +163,19 @@
     :param amount: required
     :type amount: float
     '''
     check_sub_account_id_param(sub_account_id)
 
     amount_wei = int(amount * 10 ** 18)
 
+    eth_token = self.token_profile['WETH']['address']
+
     return self.cross_margin_handler_instance.functions.depositCollateral(
       sub_account_id,
-      self.token_profile['WETH']['address'],
+      eth_token,
       amount_wei,
       True
     ).transact({"from": self.eth_signer.address, "value": amount_wei})
 
   def create_market_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, reduce_only: bool, tp_token: str = ADDRESS_ZERO, intent=False):
     '''
     Post a market order
@@ -526,17 +527,22 @@
     encoded_data = encode_typed_data(full_message=full_message)
 
     sign_data = Account.sign_message(encoded_data, self.eth_signer.key)
 
     signature = encode_packed(['bytes32', 'bytes32', 'uint8'], [
         bytes.fromhex(hex(sign_data.r)[2:]), bytes.fromhex(hex(sign_data.s)[2:]), sign_data.v])
 
-    private_key = PrivateKey(
-      bytes(bytearray.fromhex(self.eth_signer.key.hex()[2:])))
-    pubkey_ser = private_key.pubkey.serialize(compressed=False).hex()
+    pk = keys.PrivateKey(self.eth_signer.key)
+
+    pubkey = pk.public_key
+
+    str_pubkey = str(pubkey)
+
+    # convert to secp256k1 format
+    pubkey_ser = str_pubkey[:2] + "04" + str_pubkey[2:]
 
     req_body = {
       "chainId": self.chain_id,
       "intentTradeOrders": [
         {
           "marketIndex": market_index,
           "sizeDeltaE30": str(size if buy else size * -1),
@@ -547,15 +553,15 @@
           "tpToken": tp_token,
           "createdTimestamp": created_timestamp,
           "expiryTimestamp": expired_timestamp,
           "account": self.eth_signer.address,
           "subAccountId": sub_account_id,
           "signature": "0x" + signature.hex(),
           "digest": sign_data.messageHash.hex(),
-          "publicKey": "0x" + pubkey_ser,
+          "publicKey": pubkey_ser,
         }
       ]
     }
     json_body = json.dumps(req_body)
 
     return json_body
```

### Comparing `hmx-v2-python-1.1.0/hmx2/modules/public.py` & `hmx-v2-python-1.2.0/hmx2/modules/public.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from web3 import Web3
 from hmx2.constants.contracts import (
+  ADAPTIVE_FEE_CALCULATOR_ABI,
   VAULT_STORAGE_ABI_PATH,
   PERP_STORAGE_ABI_PATH,
   CONFIG_STORAGE_ABI_PATH,
   TRADE_HELPER_ABI_PATH,
-  CALCULATOR_ABI_PATH
+  CALCULATOR_ABI_PATH,
+  ORDERBOOK_ORACLE_ABI
 )
 from hmx2.constants.intent import INTENT_TRADE_API
 from hmx2.constants.markets import (
-    MARKET_PROFILE,
     DELISTED_MARKET
 )
 from hmx2.constants.common import (
+  BPS,
   BYTE_ZERO,
   HOURS,
   DAYS,
   YEARS
 )
 from hmx2.enum import IntentOrderStatus
 from hmx2.helpers.contract_loader import load_contract
 from hmx2.helpers.mapper import (
   get_collateral_address_asset_map,
   get_collateral_address_list,
   get_contract_address,
   get_token_profile,
+  get_market_profile,
 )
-from hmx2.helpers.util import get_sub_account
+from hmx2.helpers.util import get_sub_account, is_blast_chain
 from hmx2.modules.oracle.oracle_middleware import OracleMiddleware
 from hmx2.modules.calculator.calculator import Calculator
 from simple_multicall_v6 import Multicall
 from eth_abi.abi import decode
 from typing import List
 import requests as r
 
@@ -48,16 +51,21 @@
       self.eth_provider, self.contract_address["VAULT_STORAGE_ADDRESS"], VAULT_STORAGE_ABI_PATH)
     self.trade_helper_instance = load_contract(
       self.eth_provider, self.contract_address["TRADE_HELPER_ADDRESS"], TRADE_HELPER_ABI_PATH
     )
     self.calculator_instance = load_contract(
       self.eth_provider, self.contract_address["CALCULATOR_ADDRESS"], CALCULATOR_ABI_PATH
     )
+    self.orderbook_oracle_instance = load_contract(
+      self.eth_provider, self.contract_address["ORDERBOOK_ORACLE_ADDRESS"], ORDERBOOK_ORACLE_ABI)
+    self.adaptive_fee_calculator_instance = load_contract(
+      self.eth_provider, self.contract_address["ADAPTIVE_FEE_CALCULATOR_ADDRESS"], ADAPTIVE_FEE_CALCULATOR_ABI)
     self.multicall_instance = Multicall(w3=self.eth_provider,
                                         custom_address=self.contract_address["MULTICALL_ADDRESS"])
+    self.market_profile = get_market_profile(chain_id)
 
   def __get_position(self, account: str, sub_account_id: int, market_index: int):
     position_id = self.get_position_id(account, sub_account_id, market_index)
     (
       primary_account,
       market_index,
       avg_entry_price_e30,
@@ -168,15 +176,15 @@
 
       position_data[sub_account_id] = sub_account_position
 
     return position_data
 
   def __multicall_all_market_data(self):
     ACTIVE_MARKET = [
-      x for x in MARKET_PROFILE.keys() if x not in DELISTED_MARKET]
+      x for x in self.market_profile.keys()]
     market_config_calls = list(map(lambda market_index: self.multicall_instance.create_call(
         self.config_storage_instance, "marketConfigs", [market_index]
       ), ACTIVE_MARKET))
 
     market_data_calls = list(map(lambda market_index: self.multicall_instance.create_call(
         self.perp_storage_instance, "markets", [market_index]
       ), ACTIVE_MARKET))
@@ -481,19 +489,19 @@
         size: size of position
 
       Returns:
         price object
     '''
 
     price = self.oracle_middleware.get_price(
-      MARKET_PROFILE[market_index]["asset"])
-    asset_decimal = MARKET_PROFILE[market_index]["display_decimal"]
+      self.market_profile[market_index]["asset"])
+    asset_decimal = self.market_profile[market_index]["display_decimal"]
     if buy is None and size is None:
       return {
-        "market": MARKET_PROFILE[market_index]["name"],
+        "market": self.market_profile[market_index]["name"],
         "price": round(price, asset_decimal),
         "adaptive_price": None,
         "price_impact": None,
       }
     data = self.__multicall_market_data(market_index)
     oracle_price = price * 10**30
     adaptive_price = Calculator.get_adaptive_price(
@@ -502,36 +510,37 @@
       data["market"]["short_position_size"],
       data["market_config"]["max_skew_scale_usd"],
       Web3.to_wei(size, "tether") if buy else -Web3.to_wei(size, "tether")
     )
     price_impact = (adaptive_price * 10**30 // oracle_price) - 10**30
 
     return {
-      "market": MARKET_PROFILE[market_index]["name"],
+      "market": self.market_profile[market_index]["name"],
       "price": round(oracle_price / 10**30, asset_decimal),
       "adaptive_price": round(adaptive_price / 10**30, asset_decimal),
       "price_impact": price_impact * 100 / 10**30,
     }
 
   def get_multiple_price(self, market_indices: List[int] = []):
     if not market_indices:
-      market_indices = list(set(MARKET_PROFILE.keys()) - set(DELISTED_MARKET))
+      market_indices = list(
+        set(self.market_profile.keys()) - set(DELISTED_MARKET))
 
     asset_ids = list(
-      map(lambda market_index: MARKET_PROFILE[market_index]["asset"], market_indices))
+      map(lambda market_index: self.market_profile[market_index]["asset"], market_indices))
 
     price_object = self.oracle_middleware.get_multiple_price(
         asset_ids
       )
 
     market_prices = {}
 
     for market_index in market_indices:
-      asset_id = MARKET_PROFILE[market_index]["asset"]
-      asset_decimal = MARKET_PROFILE[market_index]["display_decimal"]
+      asset_id = self.market_profile[market_index]["asset"]
+      asset_decimal = self.market_profile[market_index]["display_decimal"]
       price = round(
         price_object[asset_id], asset_decimal)
       market_prices[market_index] = price
 
     return market_prices
 
   def get_market_info(self, market_index: int):
@@ -556,15 +565,15 @@
       block["timestamp"],
     )
 
     borrowing_rate = Calculator.get_borrowing_rate(
       data["asset_class_config"], data["asset_class"], tvl)
 
     return {
-      "market": MARKET_PROFILE[market_index]["name"],
+      "market": self.market_profile[market_index]["name"],
       "price": price,
       "long_size": data["market"]["long_position_size"] / 10**30,
       "short_size": data["market"]["short_position_size"] / 10**30,
       "funding_rate": {
         "1H": funding_rate * HOURS / DAYS * 100 / 10**18,
         "8H": funding_rate * 8 * HOURS / DAYS * 100 / 10**18,
         "24H": funding_rate * 100 / 10**18,
@@ -588,30 +597,30 @@
     block = self.__get_block()
 
     market_info = {}
     raw_market_data = self.__multicall_all_market_data()
 
     market_prices = self.get_multiple_price()
 
-    for market_index in MARKET_PROFILE.keys():
+    for market_index in self.market_profile.keys():
       if market_index not in DELISTED_MARKET:
         current_raw_market_data = raw_market_data[market_index]
         price = market_prices[market_index]
         funding_rate = Calculator.get_funding_rate(
           current_raw_market_data["trading_config"],
           current_raw_market_data["market_config"],
           current_raw_market_data["market"],
           block["timestamp"],
         )
 
         borrowing_rate = Calculator.get_borrowing_rate(
           current_raw_market_data["asset_class_config"], current_raw_market_data["asset_class"], tvl)
 
         market_info[market_index] = {
-          "market": MARKET_PROFILE[market_index]["name"],
+          "market": self.market_profile[market_index]["name"],
           "price": price,
           "long_size": current_raw_market_data["market"]["long_position_size"] / 10**30,
           "short_size": current_raw_market_data["market"]["short_position_size"] / 10**30,
           "funding_rate": {
             "1H": funding_rate * HOURS / DAYS * 100 / 10**18,
             "8H": funding_rate * 8 * HOURS / DAYS * 100 / 10**18,
             "24H": funding_rate * 100 / 10**18,
@@ -629,26 +638,32 @@
 
   def get_position_id(self, account: str, sub_account_id: int, market_index: int):
     return Web3.solidity_keccak(
       ['address', 'uint256'],
       [get_sub_account(account, sub_account_id), market_index]
     )
 
-  def get_all_position_info(self, account: str, sub_account_id: List[int] = []):
+  def get_all_position_info(self, account: str, sub_account_id: int | List[int] = []):
+    if type(sub_account_id) == int:
+      sub_account_id = [sub_account_id]
     market_datas = self.__multicall_all_market_data()
     tvl = self.__get_hlp_tvl()
     block = self.__get_block()
 
     positions = self.__get_all_position(account, sub_account_id)
 
     positions_flat = [
         x for y in list(positions.values()) for x in y]
 
-    active_market_list = set(
-      map(lambda position: position['market_index'], positions_flat))
+    active_market_list = list(set(
+      map(lambda position: position['market_index'], positions_flat)))
+
+    adaptive_fee_infos = self.__get_adaptive_fee_infos(active_market_list)
+
+    maker_taker_fee_infos = self.__get_maker_taker_fee_e8(active_market_list)
 
     price_map = self.get_multiple_price(active_market_list)
 
     position_infos = []
 
     for position in positions_flat:
       market_index = position['market_index']
@@ -676,41 +691,55 @@
         block["timestamp"],
         market_data["asset_class"]['last_borrowing_time'],
         market_data["trading_config"]['funding_interval'])
 
       borrowing_fee = Calculator.get_borrowing_fee(reserved_value=position_reserved_value, sum_borrowing_rate=(
         sum_borrowing_rate + next_borrowing_rate), entry_borrowing_rate=entry_borrowing_rate)
 
+      base_fee_bps = market_data["market_config"]["decrease_position_fee_rate_bps"]
+
+      skew = market_data["market"]["long_position_size"] - \
+          market_data["market"]["short_position_size"]
+
+      trading_fee = Calculator.get_trading_fee(
+        position["position_size_e30"] * -1, base_fee_bps, skew, adaptive_fee_infos[market_index], maker_taker_fee_infos[market_index])
+
       position_info = {
         "primary_account": position["primary_account"],
         "sub_account_id": position["sub_account_id"],
-        "market": MARKET_PROFILE[market_index]["name"],
+        "market": self.market_profile[market_index]["name"],
         "position_size": position["position_size_e30"] / 10**30,
         "avg_entry_price": position["avg_entry_price_e30"] / 10**30,
         "pnl": pnl / 10**30,
         "funding_fee": funding_fee / 10**30,
         "borrowing_fee": borrowing_fee / 10**30,
+        "trading_fee": trading_fee / 10**30
       }
       position_infos.append(position_info)
 
     return position_infos
 
   def get_position_info(self, account: str, sub_account_id: int, market_index: int):
     market_data = self.__multicall_market_data(market_index)
     tvl = self.__get_hlp_tvl()
 
     position = self.__get_position(account, sub_account_id, market_index)
+
+    adaptive_fee_infos = self.__get_adaptive_fee_infos([market_index])
+
+    maker_taker_fee_infos = self.__get_maker_taker_fee_e8([market_index])
+
     position_reserved_value = position['reserve_value_e30']
     asset_class_reserved_value = market_data["asset_class"]["reserve_value_e30"]
 
     sum_borrowing_rate = market_data['asset_class']['sum_borrowing_rate']
     entry_borrowing_rate = position['entry_borrowing_rate']
     block = self.__get_block()
     price = int(self.oracle_middleware.get_price(
-        MARKET_PROFILE[market_index]["asset"]) * 10 ** 30)
+        self.market_profile[market_index]["asset"]) * 10 ** 30)
 
     pnl = Calculator.get_pnl(
       position, market_data["market"], market_data["market_config"], market_data["trading_config"], price, block["timestamp"])
 
     current_funding_accrued = Calculator.get_next_funding_accrued(
       market_data["trading_config"], market_data["market_config"], market_data["market"], block["timestamp"])
 
@@ -723,24 +752,32 @@
       tvl,
       block["timestamp"],
       market_data["asset_class"]['last_borrowing_time'],
       market_data["trading_config"]['funding_interval'])
 
     borrowing_fee = Calculator.get_borrowing_fee(reserved_value=position_reserved_value, sum_borrowing_rate=(
       sum_borrowing_rate + next_borrowing_rate), entry_borrowing_rate=entry_borrowing_rate)
+    base_fee_bps = market_data["market_config"]["decrease_position_fee_rate_bps"]
+
+    skew = market_data["market"]["long_position_size"] - \
+        market_data["market"]["short_position_size"]
+
+    trading_fee = Calculator.get_trading_fee(
+        position["position_size_e30"] * -1, base_fee_bps, skew, adaptive_fee_infos[market_index], maker_taker_fee_infos[market_index])
 
     return {
       "primary_account": position["primary_account"],
       "sub_account_id": position["sub_account_id"],
-      "market": MARKET_PROFILE[market_index]["name"],
+      "market": self.market_profile[market_index]["name"],
       "position_size": position["position_size_e30"] / 10**30,
       "avg_entry_price": position["avg_entry_price_e30"] / 10**30,
       "pnl": pnl / 10**30,
       "funding_fee": funding_fee / 10**30,
       "borrowing_fee": borrowing_fee / 10**30,
+      "trading_fee": trading_fee / 10**30
     }
 
   def get_adaptive_fee(self, size_delta: int, market_index: int, is_increase: bool):
     base_fee_bps = 7
     raw_market_config = self.config_storage_instance.functions.getMarketConfigByIndex(
       market_index).call()
     (
@@ -786,16 +823,46 @@
 
   def get_collaterals(self, account: str, sub_account_id: int):
 
     sub_account_address = get_sub_account(account, sub_account_id)
     collateral_address_list = get_collateral_address_list(self.chain_id)
     collateral_address_asset_map = get_collateral_address_asset_map(
       self.chain_id)
+
+    # filter for blast
+    if is_blast_chain(self.chain_id):
+      token_profile = get_token_profile(self.chain_id)
+      weth_address = token_profile["WETH"]["address"]
+      usdb_address = token_profile["USDB"]["address"]
+      collateral_address_list.remove(weth_address)
+      collateral_address_asset_map.pop(weth_address)
+      collateral_address_list.remove(usdb_address)
+      collateral_address_asset_map.pop(usdb_address)
+
     token_profile = get_token_profile(self.chain_id)
 
+    token_config_calls = [self.multicall_instance.create_call(
+      self.config_storage_instance,
+      "getCollateralTokenConfigs",
+      [token_address]
+    ) for token_address in collateral_address_list]
+
+    token_configs_raw = self.multicall_instance.call(token_config_calls)[1]
+
+    token_configs = {}
+
+    for index, token_config in enumerate(token_configs_raw):
+      collateral_address = collateral_address_list[index]
+      data = decode(['address', 'uint32', 'bool'], token_config)
+      token_configs[collateral_address] = {
+        "settle_strategy": data[0],
+        "collateral_factor_bps": data[1],
+        "accepted": data[2],
+      }
+
     calls = [
       self.multicall_instance.create_call(
         self.vault_storage_instance,
           "traderBalances",
           [sub_account_address, collateral],
       )
       for collateral in collateral_address_list
@@ -810,23 +877,258 @@
 
     results = self.multicall_instance.call(calls)
 
     ret = {}
     for index, collateral in enumerate(collateral_address_list):
       amount = int(
           results[1][index].hex(), 16) / 10 ** token_profile[collateral]["decimals"]
+      collatral_factor = token_configs[collateral]["collateral_factor_bps"] / BPS
       ret[token_profile[collateral]["symbol"]] = {
         'amount': amount,
-        'value_usd': amount * collateral_price_dict[token_profile[collateral]["asset"]]
+        'value_usd': amount * collateral_price_dict[token_profile[collateral]["asset"]] * collatral_factor,
+        'value_without_factor_usd': amount * collateral_price_dict[token_profile[collateral]["asset"]]
       }
 
     return ret
 
   def get_active_intent_orders(self, address: str, sub_account_id: int):
     return self.__get_intent_trade_orders_api(address, sub_account_id)
 
   def __get_intent_trade_orders_api(self, address: str, sub_account_id: int):
     params = {
       "chainId": self.chain_id,
       "status": IntentOrderStatus.Pending,
     }
     return r.get(f'{INTENT_TRADE_API}/v1/intent-handler/{address}/{sub_account_id}/trade-orders', headers={'Content-Type': 'application/json'}, params=params)
+
+  def get_collateral_without_factor_usd(self, account: str, sub_account_id: int):
+    collaterals = self.get_collaterals(account, sub_account_id)
+    total_value_without_factor_usd = sum(v["value_without_factor_usd"]
+                                         for v in collaterals.values())
+
+    return total_value_without_factor_usd
+
+  def get_collateral_usd(self, account: str, sub_account_id: int):
+    collaterals = self.get_collaterals(account, sub_account_id)
+    total_value_usd = sum(v["value_usd"] for v in collaterals.values())
+
+    return total_value_usd
+
+  def get_total_pnl_and_fee(self, account: str, sub_account_id: int):
+    positions = self.get_all_position_info(account, sub_account_id)
+    total_pnl_usd = sum(position["pnl"]
+                        for position in positions)
+    total_fee_usd = sum(position["funding_fee"] +
+                        position["borrowing_fee"] + position["trading_fee"]
+                        for position in positions)
+    return {
+      "total_pnl_usd": total_pnl_usd,
+      "total_fee_usd": total_fee_usd
+    }
+
+  def get_portfolio_value(self, account: str, sub_account_id: int):
+    vault_storage_state = self.__get_trader_vault_state(account, sub_account_id)
+    collateral_without_factor = self.get_collateral_without_factor_usd(
+      account, sub_account_id)
+
+    pnl_and_fee = self.get_total_pnl_and_fee(account, sub_account_id)
+
+    total_pnl_and_fee = pnl_and_fee["total_pnl_usd"] - \
+        pnl_and_fee["total_fee_usd"]
+
+    portfolio_value = collateral_without_factor \
+        + total_pnl_and_fee \
+        - vault_storage_state["trading_fee"] \
+        - vault_storage_state["borrowing_fee"] \
+        - vault_storage_state["funding_fee"] \
+        - vault_storage_state["loss_fee"]
+
+    return max(portfolio_value, 0)
+
+  def __get_adaptive_fee_infos(self, market_indices: List[int]):
+
+    adaptive_fee_info = {k: None for k in market_indices}
+
+    is_adaptive_fee_enabled_calls = [self.multicall_instance.create_call(
+      self.config_storage_instance,
+      "isAdaptiveFeeEnabledByMarketIndex",
+      [market_index]
+    ) for market_index in market_indices
+    ]
+
+    is_adaptive_fee_enabled_data_raw = self.multicall_instance.call(
+      is_adaptive_fee_enabled_calls)[1]
+
+    is_adaptive_fee_enabled_data = {}
+
+    for index, market_index in enumerate(market_indices):
+      is_adaptive_fee_enabled_data[market_index] = decode(
+        ['bool'], is_adaptive_fee_enabled_data_raw[index])[0]
+
+    adaptive_fee_market_indices = [
+      k for k, v in is_adaptive_fee_enabled_data.items() if v]
+
+    if len(adaptive_fee_market_indices) == 0:
+      return adaptive_fee_info
+
+    orderbook_calls = [self.multicall_instance.create_call(
+        self.orderbook_oracle_instance,
+        "getData",
+        [market_index]
+    ) for market_index in adaptive_fee_market_indices]
+
+    epoch_volume_buy_calls = [self.multicall_instance.create_call(
+      self.perp_storage_instance,
+      "getEpochVolume",
+      [True, market_index]
+    ) for market_index in adaptive_fee_market_indices]
+
+    epoch_volume_sell_calls = [self.multicall_instance.create_call(
+      self.perp_storage_instance,
+      "getEpochVolume",
+      [False, market_index]
+    ) for market_index in adaptive_fee_market_indices]
+
+    max_adaptive_fee_bps_call = self.multicall_instance.create_call(
+      self.trade_helper_instance,
+      "maxAdaptiveFeeBps",
+      []
+    )
+
+    k1_call = self.multicall_instance.create_call(
+      self.adaptive_fee_calculator_instance,
+      "k1",
+      []
+    )
+
+    k2_call = self.multicall_instance.create_call(
+      self.adaptive_fee_calculator_instance,
+      "k2",
+      []
+    )
+
+    adaptive_fee_calculator_calls = orderbook_calls + epoch_volume_buy_calls + \
+        epoch_volume_sell_calls + \
+        [max_adaptive_fee_bps_call] + [k1_call] + [k2_call]
+
+    contract_data = self.multicall_instance.call(
+      adaptive_fee_calculator_calls)
+    adaptive_fee_calculator_data_raw = contract_data[1]
+
+    orderbook_data_raw = adaptive_fee_calculator_data_raw[0: len(
+      adaptive_fee_market_indices)]
+    del adaptive_fee_calculator_data_raw[0: len(adaptive_fee_market_indices)]
+
+    epoch_volume_buy_data_raw = adaptive_fee_calculator_data_raw[0: len(
+      adaptive_fee_market_indices)]
+    del adaptive_fee_calculator_data_raw[0: len(adaptive_fee_market_indices)]
+
+    epoch_volume_sell_data_raw = adaptive_fee_calculator_data_raw[0: len(
+      adaptive_fee_market_indices)]
+    del adaptive_fee_calculator_data_raw[0: len(adaptive_fee_market_indices)]
+
+    orderbook_data = {}
+    epoch_volume_buy_data = {}
+    epoch_volume_sell_data = {}
+
+    for index, market_index in enumerate(adaptive_fee_market_indices):
+      orderbook_data[market_index] = decode(
+        ['uint256', 'uint256', 'uint256'], orderbook_data_raw[index])
+      epoch_volume_buy_data[market_index] = decode(
+        ['uint256'], epoch_volume_buy_data_raw[index])
+      epoch_volume_sell_data[market_index] = decode(
+        ['uint256'], epoch_volume_sell_data_raw[index])
+
+      max_adaptive_fee_bps, k1, k2 = (decode(
+        ['uint32'], adaptive_fee_calculator_data_raw[
+            0]),
+          decode(
+        ['uint256'], adaptive_fee_calculator_data_raw[
+            1]),
+          decode(
+        ['uint256'], adaptive_fee_calculator_data_raw[
+            2]))
+
+    for index, market_index in enumerate(adaptive_fee_market_indices):
+      adaptive_fee_info[market_index] = {
+        "ask": orderbook_data[market_index][0],
+        "bid": orderbook_data[market_index][1],
+        "coeff": orderbook_data[market_index][2],
+        "epoch_volume": {
+          "buy": epoch_volume_buy_data[market_index][0],
+          "sell": epoch_volume_sell_data[market_index][0],
+        },
+        "max_adaptive_fee_bps": max_adaptive_fee_bps[0],
+        "adaptive_fee_calculator": {
+          "k1": k1[0],
+          "k2": k2[0]
+        }
+      }
+
+    return adaptive_fee_info
+
+  def __get_maker_taker_fee_e8(self, market_indices: List[int]):
+
+    maker_taker_fee_infos = {
+      k: {
+          "maker_fee_e8": 0,
+          "taker_fee_e8": 0
+      } for k in market_indices}
+
+    contract_calls = [
+      self.multicall_instance.create_call(
+          self.config_storage_instance,
+          "makerFeeE8ByMarketIndex", [market_index]
+      ) for market_index in market_indices] + [
+      self.multicall_instance.create_call(
+          self.config_storage_instance,
+          "takerFeeE8ByMarketIndex", [market_index]
+      ) for market_index in market_indices]
+
+    contract_data = self.multicall_instance.call(contract_calls)[1]
+
+    maker_fee_raw = contract_data[0: len(
+      market_indices)]
+    del contract_data[0: len(market_indices)]
+
+    taker_fee_raw = contract_data[0: len(
+      market_indices)]
+    del contract_data[0: len(market_indices)]
+
+    for index, market_index in enumerate(market_indices):
+      maker_taker_fee_infos[market_index] = {
+        "maker_fee_e8": decode(['uint256'], maker_fee_raw[index])[0],
+        "taker_fee_e8": decode(['uint256'], taker_fee_raw[index])[0]
+      }
+
+    return maker_taker_fee_infos
+
+  def __get_trader_vault_state(self, account: str, sub_account_id: int):
+    sub_account = get_sub_account(account, sub_account_id)
+
+    trading_fee_call = self.multicall_instance.create_call(
+      self.vault_storage_instance, "tradingFeeDebt", [sub_account])
+    borrowing_fee_call = self.multicall_instance.create_call(
+      self.vault_storage_instance, "borrowingFeeDebt", [sub_account])
+    funding_fee_call = self.multicall_instance.create_call(
+      self.vault_storage_instance, "fundingFeeDebt", [sub_account])
+    loss_fee_call = self.multicall_instance.create_call(
+      self.vault_storage_instance, "lossDebt", [sub_account])
+
+    contract_calls = [trading_fee_call,
+                      borrowing_fee_call,
+                      funding_fee_call,
+                      loss_fee_call]
+
+    contract_raw_data = self.multicall_instance.call(contract_calls)[1]
+
+    trading_fee = decode(['uint256'], contract_raw_data[0])[0]
+    borrowing_fee = decode(['uint256'], contract_raw_data[1])[0]
+    funding_fee = decode(['uint256'], contract_raw_data[2])[0]
+    loss_fee = decode(['uint256'], contract_raw_data[3])[0]
+
+    return {
+      "trading_fee": trading_fee,
+      "borrowing_fee": borrowing_fee,
+      "funding_fee": funding_fee,
+      "loss_fee": loss_fee
+    }
```

### Comparing `hmx-v2-python-1.1.0/hmx_v2_python.egg-info/PKG-INFO` & `hmx-v2-python-1.2.0/hmx_v2_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python
-Version: 1.1.0
+Version: 1.2.0
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Platform: UNKNOWN
```

### Comparing `hmx-v2-python-1.1.0/hmx_v2_python.egg-info/SOURCES.txt` & `hmx-v2-python-1.2.0/hmx_v2_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 hmx2/__init__.py
 hmx2/enum.py
 hmx2/hmx_client.py
+hmx2/abis/AdaptiveFeeCalculator.json
 hmx2/abis/CIXPriceAdapter.json
+hmx2/abis/CalcPricelens.json
 hmx2/abis/Calculator.json
 hmx2/abis/ConfigStorage.json
 hmx2/abis/CrossMarginHandler.json
 hmx2/abis/ERC20.json
 hmx2/abis/GlpManager.json
 hmx2/abis/GmPriceAdapter.json
 hmx2/abis/LimitTradeHandler.json
 hmx2/abis/OnchainPricelens.json
+hmx2/abis/OrderbookOracle.json
 hmx2/abis/PerpStorage.json
 hmx2/abis/TradeHelper.json
 hmx2/abis/VaultStorage.json
 hmx2/constants/__init__.py
 hmx2/constants/assets.py
 hmx2/constants/common.py
 hmx2/constants/contracts.py
@@ -32,14 +35,16 @@
 hmx2/modules/__init__.py
 hmx2/modules/private.py
 hmx2/modules/public.py
 hmx2/modules/calculator/__init__.py
 hmx2/modules/calculator/calculator.py
 hmx2/modules/oracle/__init__.py
 hmx2/modules/oracle/oracle_middleware.py
+hmx2/modules/oracle/calc_pricelens_oracle/__init__.py
+hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py
 hmx2/modules/oracle/cix_oracle/__init__.py
 hmx2/modules/oracle/cix_oracle/cix_oracle.py
 hmx2/modules/oracle/glp_oracle/__init__.py
 hmx2/modules/oracle/glp_oracle/glp_oracle.py
 hmx2/modules/oracle/gm_oracle/__init__.py
 hmx2/modules/oracle/gm_oracle/gm_oracle.py
 hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
```

### Comparing `hmx-v2-python-1.1.0/setup.py` & `hmx-v2-python-1.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 
 LONG_DESCRIPTION = open('README.md').read()
 
 REQUIREMENTS = [
-    'eth_keys',
+    'eth_keys==0.5.0',
     'eth-account==0.10.0',
     'eth-abi>=4.0.0,<5.0.0',
     'uniswap-universal-router-decoder',
     'web3>=6.0.0,<7.0.0',
     'simple-multicall-v6',
     'responses',
     'python-dotenv>=1.0.0',
-    'secp256k1==0.14.0'
 ]
 
 setup(
     name='hmx-v2-python',
-    version='1.1.0',
+    version='1.2.0',
     packages=find_packages(),
     package_data={
       'hmx2': ['abis/*.json'],
     },
     description='HMXv2 Python SDK',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
```

### Comparing `hmx-v2-python-1.1.0/tests/constants.py` & `hmx-v2-python-1.2.0/tests/constants.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/tests/test_create_market_order.py` & `hmx-v2-python-1.2.0/tests/test_create_market_order.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/tests/test_deposit_collateral.py` & `hmx-v2-python-1.2.0/tests/test_deposit_collateral.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/tests/test_get_adaptive_fee.py` & `hmx-v2-python-1.2.0/tests/test_get_adaptive_fee.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.1.0/tests/test_init.py` & `hmx-v2-python-1.2.0/tests/test_init.py`

 * *Files identical despite different names*


# Comparing `tmp/hmx_v2_python_test-1.2.2.tar.gz` & `tmp/hmx_v2_python_test-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmx_v2_python_test-1.2.2.tar", last modified: Fri Apr 26 20:02:58 2024, max compression
+gzip compressed data, was "hmx_v2_python_test-1.2.3.tar", last modified: Fri May  3 06:58:46 2024, max compression
```

## Comparing `hmx_v2_python_test-1.2.2.tar` & `hmx_v2_python_test-1.2.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.249324 hmx_v2_python_test-1.2.2/
--rw-r--r--   0 lemon      (501) staff       (20)     1064 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/LICENSE
--rw-r--r--   0 lemon      (501) staff       (20)     4642 2024-04-26 20:02:58.249236 hmx_v2_python_test-1.2.2/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)     3361 2024-04-17 06:37:55.000000 hmx_v2_python_test-1.2.2/README.md
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.238265 hmx_v2_python_test-1.2.2/hmx2/
--rw-r--r--   0 lemon      (501) staff       (20)       35 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/hmx2/__init__.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.241226 hmx_v2_python_test-1.2.2/hmx2/abis/
--rw-r--r--   0 lemon      (501) staff       (20)     2918 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.2/hmx2/abis/AdaptiveFeeCalculator.json
--rw-r--r--   0 lemon      (501) staff       (20)     6094 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.2/hmx2/abis/CIXPriceAdapter.json
--rw-r--r--   0 lemon      (501) staff       (20)     3332 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.2/hmx2/abis/CalcPricelens.json
--rw-r--r--   0 lemon      (501) staff       (20)    19788 2024-03-07 09:18:43.000000 hmx_v2_python_test-1.2.2/hmx2/abis/Calculator.json
--rw-r--r--   0 lemon      (501) staff       (20)    79643 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.2/hmx2/abis/ConfigStorage.json
--rw-r--r--   0 lemon      (501) staff       (20)    23809 2024-03-05 11:40:21.000000 hmx_v2_python_test-1.2.2/hmx2/abis/CrossMarginHandler.json
--rw-r--r--   0 lemon      (501) staff       (20)     3685 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/hmx2/abis/ERC20.json
--rw-r--r--   0 lemon      (501) staff       (20)    11832 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/hmx2/abis/GlpManager.json
--rw-r--r--   0 lemon      (501) staff       (20)     5780 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.2/hmx2/abis/GmPriceAdapter.json
--rw-r--r--   0 lemon      (501) staff       (20)    47380 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/hmx2/abis/LimitTradeHandler.json
--rw-r--r--   0 lemon      (501) staff       (20)     2419 2024-01-18 07:42:57.000000 hmx_v2_python_test-1.2.2/hmx2/abis/OnchainPricelens.json
--rw-r--r--   0 lemon      (501) staff       (20)     6721 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.2/hmx2/abis/OrderbookOracle.json
--rw-r--r--   0 lemon      (501) staff       (20)    26489 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.2/hmx2/abis/PerpStorage.json
--rw-r--r--   0 lemon      (501) staff       (20)    27073 2024-01-30 10:28:55.000000 hmx_v2_python_test-1.2.2/hmx2/abis/TradeHelper.json
--rw-r--r--   0 lemon      (501) staff       (20)    24329 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/hmx2/abis/VaultStorage.json
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.242653 hmx_v2_python_test-1.2.2/hmx2/constants/
--rw-r--r--   0 lemon      (501) staff       (20)      107 2024-04-24 05:28:38.000000 hmx_v2_python_test-1.2.2/hmx2/constants/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     2146 2024-04-26 19:44:48.000000 hmx_v2_python_test-1.2.2/hmx2/constants/assets.py
--rw-r--r--   0 lemon      (501) staff       (20)      397 2024-04-26 11:31:42.000000 hmx_v2_python_test-1.2.2/hmx2/constants/common.py
--rw-r--r--   0 lemon      (501) staff       (20)     3263 2024-04-26 19:58:21.000000 hmx_v2_python_test-1.2.2/hmx2/constants/contracts.py
--rw-r--r--   0 lemon      (501) staff       (20)       52 2024-04-24 05:28:38.000000 hmx_v2_python_test-1.2.2/hmx2/constants/intent.py
--rw-r--r--   0 lemon      (501) staff       (20)    14585 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.2/hmx2/constants/markets.py
--rw-r--r--   0 lemon      (501) staff       (20)    20697 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.2/hmx2/constants/pricefeed.py
--rw-r--r--   0 lemon      (501) staff       (20)    13833 2024-04-26 19:52:32.000000 hmx_v2_python_test-1.2.2/hmx2/constants/tokens.py
--rw-r--r--   0 lemon      (501) staff       (20)      237 2024-04-24 05:28:38.000000 hmx_v2_python_test-1.2.2/hmx2/enum.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.243342 hmx_v2_python_test-1.2.2/hmx2/helpers/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/hmx2/helpers/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)      347 2024-04-25 10:10:59.000000 hmx_v2_python_test-1.2.2/hmx2/helpers/contract_loader.py
--rw-r--r--   0 lemon      (501) staff       (20)      993 2024-04-26 20:00:55.000000 hmx_v2_python_test-1.2.2/hmx2/helpers/mapper.py
--rw-r--r--   0 lemon      (501) staff       (20)      917 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.2/hmx2/helpers/util.py
--rw-r--r--   0 lemon      (501) staff       (20)     3002 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.2/hmx2/hmx_client.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.243801 hmx_v2_python_test-1.2.2/hmx2/modules/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/hmx2/modules/__init__.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.244122 hmx_v2_python_test-1.2.2/hmx2/modules/calculator/
--rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/hmx2/modules/calculator/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     8423 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.2/hmx2/modules/calculator/calculator.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.244541 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       48 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/__init__.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.244866 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/calc_pricelens_oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       55 2024-04-26 06:57:27.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/calc_pricelens_oracle/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     1209 2024-04-26 12:21:29.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.245215 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/cix_oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       34 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/cix_oracle/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     1315 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/cix_oracle/cix_oracle.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.245511 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/glp_oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       34 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/glp_oracle/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     1428 2024-04-25 10:13:28.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/glp_oracle/glp_oracle.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.245838 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/gm_oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       32 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/gm_oracle/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     1169 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/gm_oracle/gm_oracle.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.246185 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/onchain_pricelens_oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       59 2024-01-18 07:42:57.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)      788 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
--rw-r--r--   0 lemon      (501) staff       (20)     3980 2024-04-26 11:30:15.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/oracle_middleware.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.246524 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/pyth_oracle/
--rw-r--r--   0 lemon      (501) staff       (20)       36 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/pyth_oracle/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     1302 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.2/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
--rw-r--r--   0 lemon      (501) staff       (20)    19710 2024-04-26 20:02:11.000000 hmx_v2_python_test-1.2.2/hmx2/modules/private.py
--rw-r--r--   0 lemon      (501) staff       (20)    41224 2024-04-26 19:57:31.000000 hmx_v2_python_test-1.2.2/hmx2/modules/public.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.248894 hmx_v2_python_test-1.2.2/hmx_v2_python_test.egg-info/
--rw-r--r--   0 lemon      (501) staff       (20)     4642 2024-04-26 20:02:58.000000 hmx_v2_python_test-1.2.2/hmx_v2_python_test.egg-info/PKG-INFO
--rw-r--r--   0 lemon      (501) staff       (20)     2020 2024-04-26 20:02:58.000000 hmx_v2_python_test-1.2.2/hmx_v2_python_test.egg-info/SOURCES.txt
--rw-r--r--   0 lemon      (501) staff       (20)        1 2024-04-26 20:02:58.000000 hmx_v2_python_test-1.2.2/hmx_v2_python_test.egg-info/dependency_links.txt
--rw-r--r--   0 lemon      (501) staff       (20)      172 2024-04-26 20:02:58.000000 hmx_v2_python_test-1.2.2/hmx_v2_python_test.egg-info/requires.txt
--rw-r--r--   0 lemon      (501) staff       (20)       11 2024-04-26 20:02:58.000000 hmx_v2_python_test-1.2.2/hmx_v2_python_test.egg-info/top_level.txt
--rw-r--r--   0 lemon      (501) staff       (20)       79 2024-04-26 20:02:58.249624 hmx_v2_python_test-1.2.2/setup.cfg
--rw-r--r--   0 lemon      (501) staff       (20)     1486 2024-04-26 20:02:43.000000 hmx_v2_python_test-1.2.2/setup.py
-drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-04-26 20:02:58.248669 hmx_v2_python_test-1.2.2/tests/
--rw-r--r--   0 lemon      (501) staff       (20)       46 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.2/tests/__init__.py
--rw-r--r--   0 lemon      (501) staff       (20)     5934 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.2/tests/constants.py
--rw-r--r--   0 lemon      (501) staff       (20)     3117 2024-04-02 05:22:20.000000 hmx_v2_python_test-1.2.2/tests/test_create_market_order.py
--rw-r--r--   0 lemon      (501) staff       (20)     5522 2024-04-17 06:38:11.000000 hmx_v2_python_test-1.2.2/tests/test_deposit_collateral.py
--rw-r--r--   0 lemon      (501) staff       (20)     1307 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.2/tests/test_get_adaptive_fee.py
--rw-r--r--   0 lemon      (501) staff       (20)     1221 2023-11-30 06:57:41.000000 hmx_v2_python_test-1.2.2/tests/test_init.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.991184 hmx_v2_python_test-1.2.3/
+-rw-r--r--   0 lemon      (501) staff       (20)     1064 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/LICENSE
+-rw-r--r--   0 lemon      (501) staff       (20)     4616 2024-05-03 06:58:46.991078 hmx_v2_python_test-1.2.3/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)     3361 2024-04-17 06:37:55.000000 hmx_v2_python_test-1.2.3/README.md
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.952683 hmx_v2_python_test-1.2.3/hmx2/
+-rw-r--r--   0 lemon      (501) staff       (20)       35 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/hmx2/__init__.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.974546 hmx_v2_python_test-1.2.3/hmx2/abis/
+-rw-r--r--   0 lemon      (501) staff       (20)     2918 2024-05-02 08:43:10.000000 hmx_v2_python_test-1.2.3/hmx2/abis/AdaptiveFeeCalculator.json
+-rw-r--r--   0 lemon      (501) staff       (20)     6094 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.3/hmx2/abis/CIXPriceAdapter.json
+-rw-r--r--   0 lemon      (501) staff       (20)     3332 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/abis/CalcPricelens.json
+-rw-r--r--   0 lemon      (501) staff       (20)    19788 2024-03-07 09:18:43.000000 hmx_v2_python_test-1.2.3/hmx2/abis/Calculator.json
+-rw-r--r--   0 lemon      (501) staff       (20)    79643 2024-05-02 08:43:10.000000 hmx_v2_python_test-1.2.3/hmx2/abis/ConfigStorage.json
+-rw-r--r--   0 lemon      (501) staff       (20)    23809 2024-03-05 11:40:21.000000 hmx_v2_python_test-1.2.3/hmx2/abis/CrossMarginHandler.json
+-rw-r--r--   0 lemon      (501) staff       (20)     3685 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/hmx2/abis/ERC20.json
+-rw-r--r--   0 lemon      (501) staff       (20)    11832 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/hmx2/abis/GlpManager.json
+-rw-r--r--   0 lemon      (501) staff       (20)     5780 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.3/hmx2/abis/GmPriceAdapter.json
+-rw-r--r--   0 lemon      (501) staff       (20)    47380 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/hmx2/abis/LimitTradeHandler.json
+-rw-r--r--   0 lemon      (501) staff       (20)     2419 2024-01-18 07:42:57.000000 hmx_v2_python_test-1.2.3/hmx2/abis/OnchainPricelens.json
+-rw-r--r--   0 lemon      (501) staff       (20)     6721 2024-05-02 08:43:10.000000 hmx_v2_python_test-1.2.3/hmx2/abis/OrderbookOracle.json
+-rw-r--r--   0 lemon      (501) staff       (20)    26489 2024-05-02 08:43:10.000000 hmx_v2_python_test-1.2.3/hmx2/abis/PerpStorage.json
+-rw-r--r--   0 lemon      (501) staff       (20)    27073 2024-01-30 10:28:55.000000 hmx_v2_python_test-1.2.3/hmx2/abis/TradeHelper.json
+-rw-r--r--   0 lemon      (501) staff       (20)    24329 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/hmx2/abis/VaultStorage.json
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.976086 hmx_v2_python_test-1.2.3/hmx2/constants/
+-rw-r--r--   0 lemon      (501) staff       (20)      107 2024-04-24 05:28:38.000000 hmx_v2_python_test-1.2.3/hmx2/constants/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     2146 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/constants/assets.py
+-rw-r--r--   0 lemon      (501) staff       (20)      397 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/constants/common.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3263 2024-05-03 06:53:18.000000 hmx_v2_python_test-1.2.3/hmx2/constants/contracts.py
+-rw-r--r--   0 lemon      (501) staff       (20)       52 2024-04-30 06:21:29.000000 hmx_v2_python_test-1.2.3/hmx2/constants/intent.py
+-rw-r--r--   0 lemon      (501) staff       (20)    14585 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/constants/markets.py
+-rw-r--r--   0 lemon      (501) staff       (20)    20697 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/constants/pricefeed.py
+-rw-r--r--   0 lemon      (501) staff       (20)    13833 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/constants/tokens.py
+-rw-r--r--   0 lemon      (501) staff       (20)      237 2024-04-24 05:28:38.000000 hmx_v2_python_test-1.2.3/hmx2/enum.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.982989 hmx_v2_python_test-1.2.3/hmx2/helpers/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/hmx2/helpers/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)      347 2024-04-25 10:10:59.000000 hmx_v2_python_test-1.2.3/hmx2/helpers/contract_loader.py
+-rw-r--r--   0 lemon      (501) staff       (20)      993 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/helpers/mapper.py
+-rw-r--r--   0 lemon      (501) staff       (20)      917 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/helpers/util.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3002 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/hmx_client.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.983527 hmx_v2_python_test-1.2.3/hmx2/modules/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/hmx2/modules/__init__.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.983872 hmx_v2_python_test-1.2.3/hmx2/modules/calculator/
+-rw-r--r--   0 lemon      (501) staff       (20)        0 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/hmx2/modules/calculator/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     8423 2024-05-02 08:43:10.000000 hmx_v2_python_test-1.2.3/hmx2/modules/calculator/calculator.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.984284 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       48 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/__init__.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.984650 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/calc_pricelens_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       55 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/calc_pricelens_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1209 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.985935 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/cix_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       34 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/cix_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1315 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/cix_oracle/cix_oracle.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.986466 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/glp_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       34 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/glp_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1428 2024-05-02 08:43:10.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/glp_oracle/glp_oracle.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.986896 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/gm_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       32 2023-12-04 03:01:37.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/gm_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1169 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/gm_oracle/gm_oracle.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.987426 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/onchain_pricelens_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       59 2024-01-18 07:42:57.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)      788 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3980 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/oracle_middleware.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.987772 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/pyth_oracle/
+-rw-r--r--   0 lemon      (501) staff       (20)       36 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/pyth_oracle/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1302 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.3/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
+-rw-r--r--   0 lemon      (501) staff       (20)    19728 2024-05-03 06:53:18.000000 hmx_v2_python_test-1.2.3/hmx2/modules/private.py
+-rw-r--r--   0 lemon      (501) staff       (20)    41224 2024-05-03 06:53:16.000000 hmx_v2_python_test-1.2.3/hmx2/modules/public.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.990679 hmx_v2_python_test-1.2.3/hmx_v2_python_test.egg-info/
+-rw-r--r--   0 lemon      (501) staff       (20)     4616 2024-05-03 06:58:46.000000 hmx_v2_python_test-1.2.3/hmx_v2_python_test.egg-info/PKG-INFO
+-rw-r--r--   0 lemon      (501) staff       (20)     2020 2024-05-03 06:58:46.000000 hmx_v2_python_test-1.2.3/hmx_v2_python_test.egg-info/SOURCES.txt
+-rw-r--r--   0 lemon      (501) staff       (20)        1 2024-05-03 06:58:46.000000 hmx_v2_python_test-1.2.3/hmx_v2_python_test.egg-info/dependency_links.txt
+-rw-r--r--   0 lemon      (501) staff       (20)      161 2024-05-03 06:58:46.000000 hmx_v2_python_test-1.2.3/hmx_v2_python_test.egg-info/requires.txt
+-rw-r--r--   0 lemon      (501) staff       (20)       11 2024-05-03 06:58:46.000000 hmx_v2_python_test-1.2.3/hmx_v2_python_test.egg-info/top_level.txt
+-rw-r--r--   0 lemon      (501) staff       (20)       79 2024-05-03 06:58:46.991523 hmx_v2_python_test-1.2.3/setup.cfg
+-rw-r--r--   0 lemon      (501) staff       (20)     1469 2024-05-03 06:58:37.000000 hmx_v2_python_test-1.2.3/setup.py
+drwxr-xr-x   0 lemon      (501) staff       (20)        0 2024-05-03 06:58:46.990438 hmx_v2_python_test-1.2.3/tests/
+-rw-r--r--   0 lemon      (501) staff       (20)       46 2023-11-29 08:33:18.000000 hmx_v2_python_test-1.2.3/tests/__init__.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5934 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.3/tests/constants.py
+-rw-r--r--   0 lemon      (501) staff       (20)     3117 2024-04-02 05:22:20.000000 hmx_v2_python_test-1.2.3/tests/test_create_market_order.py
+-rw-r--r--   0 lemon      (501) staff       (20)     5522 2024-04-17 06:38:11.000000 hmx_v2_python_test-1.2.3/tests/test_deposit_collateral.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1307 2024-03-19 05:01:07.000000 hmx_v2_python_test-1.2.3/tests/test_get_adaptive_fee.py
+-rw-r--r--   0 lemon      (501) staff       (20)     1221 2023-11-30 06:57:41.000000 hmx_v2_python_test-1.2.3/tests/test_init.py
```

### Comparing `hmx_v2_python_test-1.2.2/LICENSE` & `hmx_v2_python_test-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/PKG-INFO` & `hmx_v2_python_test-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python-test
-Version: 1.2.2
+Version: 1.2.3
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Classifier: Intended Audience :: Developers
@@ -18,23 +18,22 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: eth_keys
+Requires-Dist: eth_keys==0.5.0
 Requires-Dist: eth-account==0.10.0
 Requires-Dist: eth-abi<5.0.0,>=4.0.0
 Requires-Dist: uniswap-universal-router-decoder
 Requires-Dist: web3<7.0.0,>=6.0.0
 Requires-Dist: simple-multicall-v6
 Requires-Dist: responses
 Requires-Dist: python-dotenv>=1.0.0
-Requires-Dist: secp256k1==0.14.0
 
 # Python SDK for HMXv2
 
 This library is tested against Python versions 2.7, 3.4, 3.5, 3.9, and 3.11.
 
 ## Installation
```

### Comparing `hmx_v2_python_test-1.2.2/README.md` & `hmx_v2_python_test-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/AdaptiveFeeCalculator.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/AdaptiveFeeCalculator.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/CIXPriceAdapter.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/CIXPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/CalcPricelens.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/CalcPricelens.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/Calculator.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/Calculator.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/ConfigStorage.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/ConfigStorage.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/CrossMarginHandler.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/CrossMarginHandler.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/ERC20.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/GlpManager.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/GlpManager.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/GmPriceAdapter.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/GmPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/LimitTradeHandler.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/LimitTradeHandler.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/OnchainPricelens.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/OnchainPricelens.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/OrderbookOracle.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/OrderbookOracle.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/PerpStorage.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/PerpStorage.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/TradeHelper.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/TradeHelper.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/abis/VaultStorage.json` & `hmx_v2_python_test-1.2.3/hmx2/abis/VaultStorage.json`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/constants/assets.py` & `hmx_v2_python_test-1.2.3/hmx2/constants/assets.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/constants/contracts.py` & `hmx_v2_python_test-1.2.3/hmx2/constants/contracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,14 @@
 CROSS_MARGIN_HANDLER_ABI_PATH = "abis/CrossMarginHandler.json"
 LIMIT_TRADE_HANDLER_ABI_PATH = "abis/LimitTradeHandler.json"
 VAULT_STORAGE_ABI_PATH = "abis/VaultStorage.json"
 GLP_MANAGER_ABI_PATH = "abis/GlpManager.json"
 PERP_STORAGE_ABI_PATH = "abis/PerpStorage.json"
 CONFIG_STORAGE_ABI_PATH = "abis/ConfigStorage.json"
 CIX_PRICE_ADAPTER_ABI_PATH = "abis/CIXPriceAdapter.json"
-GM_PRICE_ADAPTER_ABI_PATH = "abis/GMPriceAdapter.json"
+GM_PRICE_ADAPTER_ABI_PATH = "abis/GmPriceAdapter.json"
 TRADE_HELPER_ABI_PATH = "abis/TradeHelper.json"
 ONCHAIN_PRICELENS_ABI_PATH = "abis/OnchainPricelens.json"
 CALC_PRICELENS_ABI_PATH = "abis/CalcPricelens.json"
 CALCULATOR_ABI_PATH = "abis/Calculator.json"
 ORDERBOOK_ORACLE_ABI = "abis/OrderbookOracle.json"
 ADAPTIVE_FEE_CALCULATOR_ABI = "abis/AdaptiveFeeCalculator.json"
```

### Comparing `hmx_v2_python_test-1.2.2/hmx2/constants/markets.py` & `hmx_v2_python_test-1.2.3/hmx2/constants/markets.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/constants/pricefeed.py` & `hmx_v2_python_test-1.2.3/hmx2/constants/pricefeed.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/constants/tokens.py` & `hmx_v2_python_test-1.2.3/hmx2/constants/tokens.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/helpers/mapper.py` & `hmx_v2_python_test-1.2.3/hmx2/helpers/mapper.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/helpers/util.py` & `hmx_v2_python_test-1.2.3/hmx2/helpers/util.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/hmx_client.py` & `hmx_v2_python_test-1.2.3/hmx2/hmx_client.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/modules/calculator/calculator.py` & `hmx_v2_python_test-1.2.3/hmx2/modules/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py` & `hmx_v2_python_test-1.2.3/hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/modules/oracle/cix_oracle/cix_oracle.py` & `hmx_v2_python_test-1.2.3/hmx2/modules/oracle/cix_oracle/cix_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/modules/oracle/glp_oracle/glp_oracle.py` & `hmx_v2_python_test-1.2.3/hmx2/modules/oracle/glp_oracle/glp_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/modules/oracle/gm_oracle/gm_oracle.py` & `hmx_v2_python_test-1.2.3/hmx2/modules/oracle/gm_oracle/gm_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py` & `hmx_v2_python_test-1.2.3/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/modules/oracle/oracle_middleware.py` & `hmx_v2_python_test-1.2.3/hmx2/modules/oracle/oracle_middleware.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py` & `hmx_v2_python_test-1.2.3/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx2/modules/private.py` & `hmx_v2_python_test-1.2.3/hmx2/modules/private.py`

 * *Files 1% similar despite different names*

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
@@ -24,15 +25,14 @@
   INTENT_TRADE_API,
 )
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
@@ -527,17 +527,22 @@
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
@@ -548,15 +553,15 @@
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

### Comparing `hmx_v2_python_test-1.2.2/hmx2/modules/public.py` & `hmx_v2_python_test-1.2.3/hmx2/modules/public.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/hmx_v2_python_test.egg-info/PKG-INFO` & `hmx_v2_python_test-1.2.3/hmx_v2_python_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python-test
-Version: 1.2.2
+Version: 1.2.3
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Classifier: Intended Audience :: Developers
@@ -18,23 +18,22 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: eth_keys
+Requires-Dist: eth_keys==0.5.0
 Requires-Dist: eth-account==0.10.0
 Requires-Dist: eth-abi<5.0.0,>=4.0.0
 Requires-Dist: uniswap-universal-router-decoder
 Requires-Dist: web3<7.0.0,>=6.0.0
 Requires-Dist: simple-multicall-v6
 Requires-Dist: responses
 Requires-Dist: python-dotenv>=1.0.0
-Requires-Dist: secp256k1==0.14.0
 
 # Python SDK for HMXv2
 
 This library is tested against Python versions 2.7, 3.4, 3.5, 3.9, and 3.11.
 
 ## Installation
```

### Comparing `hmx_v2_python_test-1.2.2/hmx_v2_python_test.egg-info/SOURCES.txt` & `hmx_v2_python_test-1.2.3/hmx_v2_python_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/setup.py` & `hmx_v2_python_test-1.2.3/setup.py`

 * *Files 2% similar despite different names*

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
     name='hmx-v2-python-test',
-    version='1.2.2',
+    version='1.2.3',
     packages=find_packages(),
     package_data={
       'hmx2': ['abis/*.json'],
     },
     description='HMXv2 Python SDK',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
```

### Comparing `hmx_v2_python_test-1.2.2/tests/constants.py` & `hmx_v2_python_test-1.2.3/tests/constants.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/tests/test_create_market_order.py` & `hmx_v2_python_test-1.2.3/tests/test_create_market_order.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/tests/test_deposit_collateral.py` & `hmx_v2_python_test-1.2.3/tests/test_deposit_collateral.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/tests/test_get_adaptive_fee.py` & `hmx_v2_python_test-1.2.3/tests/test_get_adaptive_fee.py`

 * *Files identical despite different names*

### Comparing `hmx_v2_python_test-1.2.2/tests/test_init.py` & `hmx_v2_python_test-1.2.3/tests/test_init.py`

 * *Files identical despite different names*


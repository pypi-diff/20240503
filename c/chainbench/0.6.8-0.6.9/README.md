# Comparing `tmp/chainbench-0.6.8.tar.gz` & `tmp/chainbench-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.6.8.tar", max compression
+gzip compressed data, was "chainbench-0.6.9.tar", max compression
```

## Comparing `chainbench-0.6.8.tar` & `chainbench-0.6.9.tar`

### file list

```diff
@@ -1,53 +1,62 @@
--rw-r--r--   0        0        0    11357 2024-04-25 15:53:11.052962 chainbench-0.6.8/LICENSE
--rw-r--r--   0        0        0    12165 2024-04-25 15:53:11.052962 chainbench-0.6.8/README.md
--rw-r--r--   0        0        0        0 2024-04-25 15:53:11.052962 chainbench-0.6.8/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2024-04-25 15:53:11.052962 chainbench-0.6.8/chainbench/__main__.py
--rw-r--r--   0        0        0    15103 2024-04-25 15:53:11.052962 chainbench-0.6.8/chainbench/main.py
--rw-r--r--   0        0        0        0 2024-04-25 15:53:11.052962 chainbench-0.6.8/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3732 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/avalanche/general.py
--rw-r--r--   0        0        0     2760 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/bsc/general.py
--rw-r--r--   0        0        0     1158 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/ethereum/consensus.py
--rw-r--r--   0        0        0     2776 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/ethereum/general.py
--rw-r--r--   0        0        0      344 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/evm/all.py
--rw-r--r--   0        0        0     1272 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/evm/debug_trace.py
--rw-r--r--   0        0        0      427 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/evm/get_logs.py
--rw-r--r--   0        0        0     4252 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/evm/heavy.py
--rw-r--r--   0        0        0     1655 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/evm/light.py
--rw-r--r--   0        0        0     1931 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/oasis/general.py
--rw-r--r--   0        0        0     2897 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/polygon/general.py
--rw-r--r--   0        0        0      366 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/solana/all.py
--rw-r--r--   0        0        0     1415 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/solana/general.py
--rw-r--r--   0        0        0     2223 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/profile/starknet/wallet.py
--rw-r--r--   0        0        0      599 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     6482 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/blockchain.py
--rw-r--r--   0        0        0     5934 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/ethereum.py
--rw-r--r--   0        0        0    18785 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/evm.py
--rw-r--r--   0        0        0     6037 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/solana.py
--rw-r--r--   0        0        0     2284 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/test_data/starknet.py
--rw-r--r--   0        0        0       24 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/tools/__init__.py
--rw-r--r--   0        0        0       18 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/tools/discovery/__init__.py
--rw-r--r--   0        0        0      977 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/tools/discovery/clients.json
--rw-r--r--   0        0        0    55080 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/tools/discovery/methods.json
--rw-r--r--   0        0        0     5499 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/tools/discovery/rpc.py
--rw-r--r--   0        0        0      416 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/__init__.py
--rw-r--r--   0        0        0     2895 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/ethereum.py
--rw-r--r--   0        0        0     4622 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/evm.py
--rw-r--r--   0        0        0     5252 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/http.py
--rw-r--r--   0        0        0      889 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/methods/__init__.py
--rw-r--r--   0        0        0      516 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/methods/common.py
--rw-r--r--   0        0        0     9082 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/methods/ethereum.py
--rw-r--r--   0        0        0    10003 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/methods/evm.py
--rw-r--r--   0        0        0     9421 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/methods/solana.py
--rw-r--r--   0        0        0     7242 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/solana.py
--rw-r--r--   0        0        0     3680 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/user/starknet.py
--rw-r--r--   0        0        0        0 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/__init__.py
--rw-r--r--   0        0        0     6218 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/cli.py
--rw-r--r--   0        0        0    12953 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/event.py
--rw-r--r--   0        0        0     5766 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/http.py
--rw-r--r--   0        0        0     2419 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/monitor.py
--rw-r--r--   0        0        0     3453 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/notify.py
--rw-r--r--   0        0        0      870 2024-04-25 15:53:11.056962 chainbench-0.6.8/chainbench/util/rng.py
--rw-r--r--   0        0        0      337 2024-04-25 15:53:11.060962 chainbench-0.6.8/chainbench/util/rpc.py
--rw-r--r--   0        0        0      455 2024-04-25 15:53:11.060962 chainbench-0.6.8/chainbench/util/timer.py
--rw-r--r--   0        0        0      991 2024-04-25 15:53:11.060962 chainbench-0.6.8/pyproject.toml
--rw-r--r--   0        0        0    12837 1970-01-01 00:00:00.000000 chainbench-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-03 10:41:50.862102 chainbench-0.6.9/LICENSE
+-rw-r--r--   0        0        0    12165 2024-05-03 10:41:50.862102 chainbench-0.6.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/__main__.py
+-rw-r--r--   0        0        0    15103 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/main.py
+-rw-r--r--   0        0        0        0 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     1607 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/arbitrum/general.py
+-rw-r--r--   0        0        0     1392 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/avalanche/archive.py
+-rw-r--r--   0        0        0     1481 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/avalanche/general.py
+-rw-r--r--   0        0        0     1268 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/base/archive.py
+-rw-r--r--   0        0        0     1570 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/base/general.py
+-rw-r--r--   0        0        0     2760 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/bsc/general.py
+-rw-r--r--   0        0        0     1158 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/ethereum/consensus.py
+-rw-r--r--   0        0        0     2776 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/ethereum/general.py
+-rw-r--r--   0        0        0      344 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/evm/all.py
+-rw-r--r--   0        0        0     1272 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/evm/debug_trace.py
+-rw-r--r--   0        0        0      427 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/evm/get_logs.py
+-rw-r--r--   0        0        0     4252 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0     1655 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0     1005 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/fantom/archive.py
+-rw-r--r--   0        0        0     1245 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/fantom/general.py
+-rw-r--r--   0        0        0     1931 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/oasis/general.py
+-rw-r--r--   0        0        0     1183 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/optimism/archive.py
+-rw-r--r--   0        0        0     1523 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/optimism/general.py
+-rw-r--r--   0        0        0     2897 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/polygon/general.py
+-rw-r--r--   0        0        0     1121 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/ronin/general.py
+-rw-r--r--   0        0        0      366 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/solana/all.py
+-rw-r--r--   0        0        0     1415 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/solana/general.py
+-rw-r--r--   0        0        0     2223 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/starknet/wallet.py
+-rw-r--r--   0        0        0      599 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     6482 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/blockchain.py
+-rw-r--r--   0        0        0     5934 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/ethereum.py
+-rw-r--r--   0        0        0    18785 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0     6037 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/solana.py
+-rw-r--r--   0        0        0     2284 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/starknet.py
+-rw-r--r--   0        0        0       24 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/tools/__init__.py
+-rw-r--r--   0        0        0       18 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/tools/discovery/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/tools/discovery/clients.json
+-rw-r--r--   0        0        0    55080 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/tools/discovery/methods.json
+-rw-r--r--   0        0        0     5499 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/tools/discovery/rpc.py
+-rw-r--r--   0        0        0      416 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     2895 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/ethereum.py
+-rw-r--r--   0        0        0     4622 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/evm.py
+-rw-r--r--   0        0        0     5252 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/http.py
+-rw-r--r--   0        0        0      889 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/methods/__init__.py
+-rw-r--r--   0        0        0      516 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/methods/common.py
+-rw-r--r--   0        0        0     9082 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/methods/ethereum.py
+-rw-r--r--   0        0        0    10278 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/methods/evm.py
+-rw-r--r--   0        0        0     9421 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/methods/solana.py
+-rw-r--r--   0        0        0     7242 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/solana.py
+-rw-r--r--   0        0        0     3680 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/starknet.py
+-rw-r--r--   0        0        0        0 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     6218 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/util/cli.py
+-rw-r--r--   0        0        0    12953 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/util/event.py
+-rw-r--r--   0        0        0     6347 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/util/http.py
+-rw-r--r--   0        0        0     2419 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/util/monitor.py
+-rw-r--r--   0        0        0     3453 2024-05-03 10:41:50.870102 chainbench-0.6.9/chainbench/util/notify.py
+-rw-r--r--   0        0        0      870 2024-05-03 10:41:50.870102 chainbench-0.6.9/chainbench/util/rng.py
+-rw-r--r--   0        0        0      337 2024-05-03 10:41:50.870102 chainbench-0.6.9/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      455 2024-05-03 10:41:50.870102 chainbench-0.6.9/chainbench/util/timer.py
+-rw-r--r--   0        0        0      991 2024-05-03 10:41:50.870102 chainbench-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0    12837 1970-01-01 00:00:00.000000 chainbench-0.6.9/PKG-INFO
```

### Comparing `chainbench-0.6.8/LICENSE` & `chainbench-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/README.md` & `chainbench-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/main.py` & `chainbench-0.6.9/chainbench/main.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/profile/avalanche/general.py` & `chainbench-0.6.9/chainbench/profile/bsc/general.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,142 +1,106 @@
 """
-Avalanche profile.
+Bsc profile.
 
 Chart:
 ```mermaid
 %%{init: {'theme':'forest'}}%%
 pie title Methods Distribution
     "eth_call" : 100
-    "eth_getBlockByNumber" : 50
-    "eth_getLogs" : 24
-    "eth_getTransactionReceipt" : 17
-    "eth_chainId" : 15
-    "eth_blockNumber" : 15
-    "eth_getBalance" : 11
-    "Others" : 28
+    "eth_getTransactionReceipt" : 93
+    "eth_getLogs" : 36
+    "eth_blockNumber" : 28
+    "eth_chainId" : 18
+    "eth_getBlockByNumber" : 13
+    "Others" : 20
 ```
 """
 
 from locust import constant_pacing, tag, task
 
 from chainbench.user import EvmUser
 from chainbench.util.rng import get_rng
 
 
-class AvalancheProfile(EvmUser):
+class BscProfile(EvmUser):
     wait_time = constant_pacing(1)
-    weight = 91
+    weight = 89
 
     @task(100)
     def call_task(self):
         self.make_rpc_call(
             name="call",
             method="eth_call",
             params=[
                 {
-                    "to": "0x7325e3564B89968D102B3261189EA44c0f5f1a8e",
-                    "data": "0x18160ddd0000000000000000000000000000000000000000000000000000000000000000",  # noqa: E501
+                    "to": "0x55d398326f99059fF775485246999027B3197955",
+                    "data": "0x70a08231000000000000000000000000f977814e90da44bfa03b6295a0616a897441acec",  # noqa: E501
                 },
                 "latest",
             ],
         ),
 
-    @task(50)
-    def get_block_by_number_task(self):
-        self.make_rpc_call(
-            name="get_block_by_number",
-            method="eth_getBlockByNumber",
-            params=self._block_params_factory(),
-        ),
-
-    @task(17)
+    @task(93)
     def get_transaction_receipt_task(self):
         self.make_rpc_call(
             name="get_transaction_receipt",
             method="eth_getTransactionReceipt",
             params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
-    @task(15)
-    def chain_id_task(self):
-        self.make_rpc_call(
-            name="chain_id",
-            method="eth_chainId",
-        ),
-
-    @task(15)
+    @task(28)
     def block_number_task(self):
         self.make_rpc_call(
             name="block_number",
             method="eth_blockNumber",
         ),
 
-    @task(11)
-    def get_balance_task(self):
+    @task(18)
+    def chain_id_task(self):
         self.make_rpc_call(
-            name="get_balance",
-            method="eth_getBalance",
-            params=self._get_account_and_block_number_params_factory_latest(get_rng()),
+            name="chain_id",
+            method="eth_chainId",
         ),
 
-    @task(10)
+    @task(13)
+    def get_block_by_number_task(self):
+        self.make_rpc_call(
+            name="get_block_by_number",
+            method="eth_getBlockByNumber",
+            params=self._block_params_factory(),
+        ),
+
+    @task(9)
     def get_transaction_by_hash_task(self):
         self.make_rpc_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
             params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @task(5)
-    def estimate_gas_task(self):
-        self.make_rpc_call(
-            name="estimate_gas",
-            method="eth_estimateGas",
-            params=[
-                {
-                    "from": "0x9f8c163cBA728e99993ABe7495F06c0A3c8Ac8b9",
-                    "to": "0xC2DE4f542C2e2349ee050541F5AD25aa4BE1a00f",
-                    "value": "0xde0b6b3a7640000",
-                }
-            ],
-        ),
-
-    @task(4)
-    def client_version_task(self):
+    def get_balance_task(self):
         self.make_rpc_call(
-            name="client_version",
-            method="web3_clientVersion",
+            name="get_balance",
+            method="eth_getBalance",
+            params=self._get_account_and_block_number_params_factory_latest(get_rng()),
         ),
 
     @task(3)
     def get_block_by_hash_task(self):
         self.make_rpc_call(
             name="get_block_by_hash",
             method="eth_getBlockByHash",
             params=self._block_by_hash_params_factory(get_rng()),
         ),
 
-    @task(3)
-    def gas_price_task(self):
-        self.make_rpc_call(
-            name="gas_price",
-            method="eth_gasPrice",
-        ),
-
-    @task(3)
-    def max_priority_fee_per_gas_task(self):
-        self.make_rpc_call(
-            name="max_priority_fee_per_gas",
-            method="eth_maxPriorityFeePerGas",
-        ),
-
 
-class AvalancheGetLogsProfile(EvmUser):
+class BscGetLogsProfile(EvmUser):
     wait_time = constant_pacing(10)
-    weight = 9
+    weight = 12
 
     @tag("get-logs")
     @task
     def get_logs_task(self):
         self.make_rpc_call(
             name="get_logs",
             method="eth_getLogs",
```

### Comparing `chainbench-0.6.8/chainbench/profile/bsc/general.py` & `chainbench-0.6.9/chainbench/profile/ethereum/general.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,106 +1,109 @@
 """
-Bsc profile.
+Ethereum profile.
 
 Chart:
 ```mermaid
 %%{init: {'theme':'forest'}}%%
 pie title Methods Distribution
     "eth_call" : 100
-    "eth_getTransactionReceipt" : 93
-    "eth_getLogs" : 36
-    "eth_blockNumber" : 28
-    "eth_chainId" : 18
-    "eth_getBlockByNumber" : 13
-    "Others" : 20
+    "eth_getTransactionReceipt" : 24
+    "eth_blockNumber" : 19
+    "eth_getBalance" : 12
+    "eth_chainId" : 11
+    "eth_getBlockByNumber" : 9
+    "eth_getTransactionByHash" : 8
+    "Others" : 12
 ```
 """
 
 from locust import constant_pacing, tag, task
 
 from chainbench.user import EvmUser
 from chainbench.util.rng import get_rng
 
 
-class BscProfile(EvmUser):
+class EthereumProfile(EvmUser):
     wait_time = constant_pacing(1)
-    weight = 89
+    weight = 487
 
     @task(100)
     def call_task(self):
         self.make_rpc_call(
             name="call",
             method="eth_call",
-            params=[
-                {
-                    "to": "0x55d398326f99059fF775485246999027B3197955",
-                    "data": "0x70a08231000000000000000000000000f977814e90da44bfa03b6295a0616a897441acec",  # noqa: E501
-                },
-                "latest",
-            ],
+            params=self._erc20_eth_call_params_factory(get_rng()),
         ),
 
-    @task(93)
+    @task(24)
     def get_transaction_receipt_task(self):
         self.make_rpc_call(
             name="get_transaction_receipt",
             method="eth_getTransactionReceipt",
             params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
-    @task(28)
+    @task(19)
     def block_number_task(self):
         self.make_rpc_call(
             name="block_number",
             method="eth_blockNumber",
         ),
 
-    @task(18)
+    @task(12)
+    def get_balance_task(self):
+        self.make_rpc_call(
+            name="get_balance",
+            method="eth_getBalance",
+            params=self._get_account_and_block_number_params_factory_latest(get_rng()),
+        ),
+
+    @task(11)
     def chain_id_task(self):
         self.make_rpc_call(
             name="chain_id",
             method="eth_chainId",
         ),
 
-    @task(13)
+    @task(9)
     def get_block_by_number_task(self):
         self.make_rpc_call(
             name="get_block_by_number",
             method="eth_getBlockByNumber",
             params=self._block_params_factory(),
         ),
 
-    @task(9)
+    @task(8)
     def get_transaction_by_hash_task(self):
         self.make_rpc_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
             params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
-    @task(5)
-    def get_balance_task(self):
+    @tag("debug")
+    @task(3)
+    def trace_transaction_task(self):
         self.make_rpc_call(
-            name="get_balance",
-            method="eth_getBalance",
-            params=self._get_account_and_block_number_params_factory_latest(get_rng()),
+            name="trace_transaction",
+            method="debug_traceTransaction",
+            params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
-    @task(3)
-    def get_block_by_hash_task(self):
+    @task(2)
+    def client_version_task(self):
         self.make_rpc_call(
-            name="get_block_by_hash",
-            method="eth_getBlockByHash",
-            params=self._block_by_hash_params_factory(get_rng()),
+            name="client_version",
+            method="web3_clientVersion",
         ),
 
 
-class BscGetLogsProfile(EvmUser):
+class EthGetLogsProfile(EvmUser):
     wait_time = constant_pacing(10)
-    weight = 12
+    weight = 13
 
     @tag("get-logs")
     @task
     def get_logs_task(self):
         self.make_rpc_call(
             name="get_logs",
             method="eth_getLogs",
```

### Comparing `chainbench-0.6.8/chainbench/profile/ethereum/consensus.py` & `chainbench-0.6.9/chainbench/profile/ethereum/consensus.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/profile/ethereum/general.py` & `chainbench-0.6.9/chainbench/profile/starknet/wallet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,111 +1,83 @@
 """
-Ethereum profile.
+StarkNet profile.
 
 Chart:
 ```mermaid
 %%{init: {'theme':'forest'}}%%
 pie title Methods Distribution
-    "eth_call" : 100
-    "eth_getTransactionReceipt" : 24
-    "eth_blockNumber" : 19
-    "eth_getBalance" : 12
-    "eth_chainId" : 11
-    "eth_getBlockByNumber" : 9
-    "eth_getTransactionByHash" : 8
-    "Others" : 12
+    "starknet_call" : 54
+    "starket_chainId" : 25
+    "starknet_getClassHashAt" : 17
+    "starknet_getTransactionReceipt" : 3
+    "Others" : 1
 ```
 """
 
-from locust import constant_pacing, tag, task
+from locust import constant_pacing, task
 
-from chainbench.user import EvmUser
+from chainbench.user import StarkNetUser
 from chainbench.util.rng import get_rng
 
 
-class EthereumProfile(EvmUser):
+class StarkNetWalletProfile(StarkNetUser):
     wait_time = constant_pacing(1)
-    weight = 487
 
-    @task(100)
+    @task(435)
     def call_task(self):
-        self.make_rpc_call(
-            name="call",
-            method="eth_call",
-            params=self._erc20_eth_call_params_factory(get_rng()),
-        ),
-
-    @task(24)
-    def get_transaction_receipt_task(self):
-        self.make_rpc_call(
-            name="get_transaction_receipt",
-            method="eth_getTransactionReceipt",
-            params=self._transaction_by_hash_params_factory(get_rng()),
-        ),
-
-    @task(19)
-    def block_number_task(self):
-        self.make_rpc_call(
-            name="block_number",
-            method="eth_blockNumber",
-        ),
+        self.make_rpc_call(name="call", method="starknet_call", params=self._call_params_factory(get_rng())),
 
-    @task(12)
-    def get_balance_task(self):
+    @task(200)
+    def chain_id_task(self):
         self.make_rpc_call(
-            name="get_balance",
-            method="eth_getBalance",
-            params=self._get_account_and_block_number_params_factory_latest(get_rng()),
+            name="chain_id",
+            method="starknet_chainId",
         ),
 
-    @task(11)
-    def chain_id_task(self):
+    @task(133)
+    def get_class_hash_at_task(self):
         self.make_rpc_call(
-            name="chain_id",
-            method="eth_chainId",
+            name="get_class_hash_at",
+            method="starknet_getClassHashAt",
+            params=self._get_class_params_factory(get_rng()),
         ),
 
-    @task(9)
-    def get_block_by_number_task(self):
+    @task(21)
+    def get_transaction_receipt_task(self):
         self.make_rpc_call(
-            name="get_block_by_number",
-            method="eth_getBlockByNumber",
-            params=self._block_params_factory(),
+            name="get_transaction_receipt",
+            method="starknet_getTransactionReceipt",
+            params=self._get_tx_hash_params_factory(get_rng()),
         ),
 
-    @task(8)
-    def get_transaction_by_hash_task(self):
+    @task(3)
+    def get_class_at_task(self):
         self.make_rpc_call(
-            name="get_transaction_by_hash",
-            method="eth_getTransactionByHash",
-            params=self._transaction_by_hash_params_factory(get_rng()),
+            name="get_class_at",
+            method="starknet_getClassAt",
+            params=self._get_class_params_factory(get_rng()),
         ),
 
-    @tag("debug")
     @task(3)
-    def trace_transaction_task(self):
+    def get_nonce_task(self):
         self.make_rpc_call(
-            name="trace_transaction",
-            method="debug_traceTransaction",
-            params=self._transaction_by_hash_params_factory(get_rng()),
+            name="get_nonce",
+            method="starknet_getNonce",
+            params=["latest", self._get_contract_address(get_rng())],
         ),
 
     @task(2)
-    def client_version_task(self):
+    def simulate_transaction_task(self):
         self.make_rpc_call(
-            name="client_version",
-            method="web3_clientVersion",
+            name="simulate_transaction",
+            method="starknet_simulateTransaction",
+            params=self._simulate_transaction_params_factory(get_rng()),
+            path="/rpc/v0.3",
         ),
 
-
-class EthGetLogsProfile(EvmUser):
-    wait_time = constant_pacing(10)
-    weight = 13
-
-    @tag("get-logs")
-    @task
-    def get_logs_task(self):
+    @task(1)
+    def estimate_fee_task(self):
         self.make_rpc_call(
-            name="get_logs",
-            method="eth_getLogs",
-            params=self._get_logs_params_factory(get_rng()),
+            name="estimate_fee",
+            method="starknet_estimateFee",
+            params=self._estimate_fee_params_factory(get_rng()),
         ),
```

### Comparing `chainbench-0.6.8/chainbench/profile/evm/debug_trace.py` & `chainbench-0.6.9/chainbench/profile/evm/debug_trace.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/profile/evm/heavy.py` & `chainbench-0.6.9/chainbench/profile/evm/heavy.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/profile/evm/light.py` & `chainbench-0.6.9/chainbench/profile/evm/light.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/profile/oasis/general.py` & `chainbench-0.6.9/chainbench/profile/oasis/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/profile/polygon/general.py` & `chainbench-0.6.9/chainbench/profile/polygon/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/profile/solana/general.py` & `chainbench-0.6.9/chainbench/profile/solana/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/test_data/__init__.py` & `chainbench-0.6.9/chainbench/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/test_data/blockchain.py` & `chainbench-0.6.9/chainbench/test_data/blockchain.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/test_data/ethereum.py` & `chainbench-0.6.9/chainbench/test_data/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/test_data/evm.py` & `chainbench-0.6.9/chainbench/test_data/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/test_data/solana.py` & `chainbench-0.6.9/chainbench/test_data/solana.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/test_data/starknet.py` & `chainbench-0.6.9/chainbench/test_data/starknet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/tools/discovery/clients.json` & `chainbench-0.6.9/chainbench/tools/discovery/clients.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/tools/discovery/methods.json` & `chainbench-0.6.9/chainbench/tools/discovery/methods.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/tools/discovery/rpc.py` & `chainbench-0.6.9/chainbench/tools/discovery/rpc.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/user/ethereum.py` & `chainbench-0.6.9/chainbench/user/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/user/evm.py` & `chainbench-0.6.9/chainbench/user/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/user/http.py` & `chainbench-0.6.9/chainbench/user/http.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/user/methods/__init__.py` & `chainbench-0.6.9/chainbench/user/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/user/methods/common.py` & `chainbench-0.6.9/chainbench/user/methods/common.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/user/methods/ethereum.py` & `chainbench-0.6.9/chainbench/user/methods/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/user/methods/evm.py` & `chainbench-0.6.9/chainbench/user/methods/evm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import typing as t
 
-from locust import task
+from locust import tag, task
 
 from chainbench.user.evm import EvmUser
 
 
 class EvmMethods(EvmUser):
     abstract = True
 
@@ -177,73 +177,84 @@
         )
 
     def eth_syncing_task(self) -> None:
         self.make_rpc_call(
             method="eth_syncing",
         )
 
+    @tag("debug")
     def debug_get_bad_blocks_task(self) -> None:
         self.make_rpc_call(
             method="debug_getBadBlocks",
         )
 
+    @tag("debug")
     def debug_get_raw_block_by_number_task(self) -> None:
         self.make_rpc_call(
             method="debug_getRawBlock",
             params=[hex(self.test_data.get_random_block_number(self.rng.get_rng()))],
         )
 
+    @tag("debug")
     def debug_get_raw_header_by_number_task(self) -> None:
         self.make_rpc_call(
             method="debug_getRawHeader",
             params=[hex(self.test_data.get_random_block_number(self.rng.get_rng()))],
         )
 
+    @tag("debug")
     def debug_get_raw_receipts_by_number_task(self) -> None:
         self.make_rpc_call(
             method="debug_getRawReceipts",
             params=[hex(self.test_data.get_random_block_number(self.rng.get_rng()))],
         )
 
+    @tag("debug")
     def debug_get_raw_transaction_by_hash_task(self) -> None:
         self.make_rpc_call(
             method="debug_getRawTransaction",
             params=[self.test_data.get_random_tx_hash(self.rng.get_rng())],
         )
 
+    @tag("debug")
     def debug_trace_bad_block_task(self) -> None:
         self.make_rpc_call(
             method="debug_traceBadBlock",
             params=[self.test_data.get_random_block_hash(self.rng.get_rng())],
         )
 
+    @tag("debug")
     def debug_trace_block_task(self) -> None:
         self.make_rpc_call(
             method="debug_traceBlock",
             params=self._block_params_factory(),
         )
 
+    @tag("debug")
     def debug_trace_block_by_hash_task(self) -> None:
         self.make_rpc_call(
             method="debug_traceBlockByHash",
             params=self._debug_trace_block_by_hash_params_factory(self.rng.get_rng()),
         )
 
+    @tag("debug")
     def debug_trace_block_by_number_task(self) -> None:
         self.make_rpc_call(
             method="debug_traceBlockByNumber",
             params=self._debug_trace_block_by_number_params_factory(),
         )
 
+    @tag("debug")
     def debug_trace_call_task(self) -> None:
         self.make_rpc_call(
             method="debug_traceCall",
             params=self._debug_trace_call_params_factory(self.rng.get_rng()),
         )
 
+    @tag("debug")
     def debug_trace_transaction_task(self) -> None:
         self.make_rpc_call(
             method="debug_traceTransaction",
             params=self._debug_trace_transaction_params_factory(self.rng.get_rng()),
         )
 
     def net_listening_task(self) -> None:
@@ -257,32 +268,36 @@
         )
 
     def net_version_task(self) -> None:
         self.make_rpc_call(
             method="net_version",
         )
 
+    @tag("trace")
     def trace_block_task(self) -> None:
         self.make_rpc_call(
             method="trace_block",
             params=self._block_params_factory(),
         )
 
+    @tag("trace")
     def trace_replay_block_transactions_task(self) -> None:
         self.make_rpc_call(
             method="trace_replayBlockTransactions",
             params=self._trace_replay_block_transaction_params_factory(),
         )
 
+    @tag("trace")
     def trace_replay_transaction_task(self) -> None:
         self.make_rpc_call(
             method="trace_replayTransaction",
             params=self._trace_replay_transaction_params_factory(self.rng.get_rng()),
         )
 
+    @tag("trace")
     def trace_transaction_task(self) -> None:
         self.make_rpc_call(
             method="trace_transaction",
             params=[self.test_data.get_random_tx_hash(self.rng.get_rng())],
         )
 
     def web3_client_version_task(self) -> None:
```

### Comparing `chainbench-0.6.8/chainbench/user/methods/solana.py` & `chainbench-0.6.9/chainbench/user/methods/solana.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/user/solana.py` & `chainbench-0.6.9/chainbench/user/solana.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/user/starknet.py` & `chainbench-0.6.9/chainbench/user/starknet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/util/cli.py` & `chainbench-0.6.9/chainbench/util/cli.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/util/event.py` & `chainbench-0.6.9/chainbench/util/event.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/util/http.py` & `chainbench-0.6.9/chainbench/util/http.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import typing as t
+from base64 import b64encode
 from enum import IntEnum
 from functools import cached_property
 from json import JSONDecodeError
 from secrets import token_hex
 
 from geventhttpclient import URL, HTTPClient
 from geventhttpclient.response import HTTPSocketPoolResponse
@@ -62,24 +63,36 @@
             logger.debug(
                 f"Request to {request_uri} failed with HTTP Error {self.status_code} {self.status_message} code: "
                 f"{self.content}"
             )
             raise HttpStatusError(self.status_code, self.status_message)
 
 
+def basic_auth(username, password):
+    token = b64encode(f"{username}:{password}".encode("utf-8")).decode("ascii")
+    return f"Basic {token}"
+
+
 class HttpClient:
     def __init__(
         self,
         host: str,
         rpc_version: str = "2.0",
         timeout: int = 360,
         error_level: HttpErrorLevel = HttpErrorLevel.ClientError,
     ):
         self._rpc_version = rpc_version
         self._host = URL(host)
+        self._general_headers = {}
+        if "@" in host:
+            username_password = host.split("//")[1].split("@")[0].split(":")
+            username = username_password[0]
+            password = username_password[1]
+            self._general_headers["Authorization"] = f"{basic_auth(username, password)}"
+
         self._client = HTTPClient.from_url(self._host, connection_timeout=120, network_timeout=timeout)
         self.error_level = error_level
 
     @property
     def host(self) -> str:
         return str(self._host)
 
@@ -98,14 +111,15 @@
         headers: dict[str, t.Any] | None = None,
         error_level: HttpErrorLevel | None = None,
     ) -> Response:
         if headers is None:
             headers = {}
         if "Accept" not in headers:
             headers.update({"Accept": "application/json"})
+        headers.update(self._general_headers)
         response = self._client.get(
             self._request_uri(path, params),
             headers=headers,
         )
         response.__class__ = Response
         if error_level is None:
             error_level = self.error_level
@@ -122,14 +136,15 @@
     ) -> Response:
         if headers is None:
             headers = {}
         if "Content-Type" not in headers:
             headers.update({"Content-Type": "application/json"})
         if "Accept" not in headers:
             headers.update({"Accept": "application/json"})
+        headers.update(self._general_headers)
         if isinstance(data, dict):
             body = json.dumps(data).encode("utf-8")
         elif isinstance(data, bytes):
             body = data
         else:
             body = b""
         response = self._client.post(
```

### Comparing `chainbench-0.6.8/chainbench/util/monitor.py` & `chainbench-0.6.9/chainbench/util/monitor.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/util/notify.py` & `chainbench-0.6.9/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/chainbench/util/rng.py` & `chainbench-0.6.9/chainbench/util/rng.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.8/pyproject.toml` & `chainbench-0.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.6.8"
+version = "0.6.9"
 description = ""
 authors = [
     "Egor Molodik <egor.molodik@chainstack.com>",
     "Erwin Wee <erwin.wee@chainstack.com>"
 ]
 maintainers = ["Erwin Wee <erwin.wee@chainstack.com>"]
 readme = "README.md"
```

### Comparing `chainbench-0.6.8/PKG-INFO` & `chainbench-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.6.8
+Version: 0.6.9
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Maintainer: Erwin Wee
 Maintainer-email: erwin.wee@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```


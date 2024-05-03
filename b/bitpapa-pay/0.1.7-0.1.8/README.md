# Comparing `tmp/bitpapa_pay-0.1.7.tar.gz` & `tmp/bitpapa_pay-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitpapa_pay-0.1.7.tar", max compression
+gzip compressed data, was "bitpapa_pay-0.1.8.tar", max compression
```

## Comparing `bitpapa_pay-0.1.7.tar` & `bitpapa_pay-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1138 2024-04-12 18:48:56.761770 bitpapa_pay-0.1.7/README.md
--rw-r--r--   0        0        0       42 2024-04-11 08:47:40.794934 bitpapa_pay-0.1.7/bitpapa_pay/__init__.py
--rw-r--r--   0        0        0     6522 2024-04-24 17:55:52.551475 bitpapa_pay-0.1.7/bitpapa_pay/client.py
--rw-r--r--   0        0        0     3814 2024-04-24 17:55:43.319650 bitpapa_pay-0.1.7/bitpapa_pay/methods/addresses.py
--rw-r--r--   0        0        0      608 2024-04-12 20:23:58.411916 bitpapa_pay-0.1.7/bitpapa_pay/methods/base.py
--rw-r--r--   0        0        0      686 2024-04-12 20:26:00.463851 bitpapa_pay-0.1.7/bitpapa_pay/methods/exchange_rates.py
--rw-r--r--   0        0        0     2405 2024-04-24 16:33:12.237628 bitpapa_pay-0.1.7/bitpapa_pay/methods/telegram.py
--rw-r--r--   0        0        0      261 2024-04-12 20:22:45.616006 bitpapa_pay-0.1.7/bitpapa_pay/types/base.py
--rw-r--r--   0        0        0      124 2024-04-12 20:25:33.931857 bitpapa_pay-0.1.7/bitpapa_pay/types/exchange_rates.py
--rw-r--r--   0        0        0      816 2024-04-24 16:36:05.257339 bitpapa_pay-0.1.7/bitpapa_pay/types/telegram.py
--rw-r--r--   0        0        0       18 2024-04-27 17:24:11.552517 bitpapa_pay-0.1.7/bitpapa_pay/version.py
--rw-r--r--   0        0        0      371 2024-04-27 17:23:58.888122 bitpapa_pay-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 bitpapa_pay-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1138 2024-04-12 18:48:56.761770 bitpapa_pay-0.1.8/README.md
+-rw-r--r--   0        0        0       42 2024-04-11 08:47:40.794934 bitpapa_pay-0.1.8/bitpapa_pay/__init__.py
+-rw-r--r--   0        0        0     6522 2024-04-24 17:55:52.551475 bitpapa_pay-0.1.8/bitpapa_pay/client.py
+-rw-r--r--   0        0        0     3677 2024-05-03 00:31:25.500266 bitpapa_pay-0.1.8/bitpapa_pay/methods/addresses.py
+-rw-r--r--   0        0        0      608 2024-04-12 20:23:58.411916 bitpapa_pay-0.1.8/bitpapa_pay/methods/base.py
+-rw-r--r--   0        0        0      686 2024-04-12 20:26:00.463851 bitpapa_pay-0.1.8/bitpapa_pay/methods/exchange_rates.py
+-rw-r--r--   0        0        0     2405 2024-04-24 16:33:12.237628 bitpapa_pay-0.1.8/bitpapa_pay/methods/telegram.py
+-rw-r--r--   0        0        0      261 2024-04-12 20:22:45.616006 bitpapa_pay-0.1.8/bitpapa_pay/types/base.py
+-rw-r--r--   0        0        0      124 2024-04-12 20:25:33.931857 bitpapa_pay-0.1.8/bitpapa_pay/types/exchange_rates.py
+-rw-r--r--   0        0        0      816 2024-04-24 16:36:05.257339 bitpapa_pay-0.1.8/bitpapa_pay/types/telegram.py
+-rw-r--r--   0        0        0       18 2024-05-03 00:31:48.680230 bitpapa_pay-0.1.8/bitpapa_pay/version.py
+-rw-r--r--   0        0        0      371 2024-05-03 00:33:41.224060 bitpapa_pay-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 bitpapa_pay-0.1.8/PKG-INFO
```

### Comparing `bitpapa_pay-0.1.7/README.md` & `bitpapa_pay-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.7/bitpapa_pay/client.py` & `bitpapa_pay-0.1.8/bitpapa_pay/client.py`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.7/bitpapa_pay/methods/addresses.py` & `bitpapa_pay-0.1.8/bitpapa_pay/methods/addresses.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,14 @@
     address: Optional[str]
     currency: str
     network: str
     balance: Optional[Union[int, float]]
     label: str
 
 
-class NewAddress(BaseModel):
-    id: str
-    address: str
-    currency: str
-    balance: Optional[Union[int, float]]
-    label: str
-
-
 class GetAddressesOutputData(BaseModel):
     addresses: List[Address]
 
 
 class GetAddressesParams(BaseModel):
     currency: Optional[str] = None
     label: Optional[str] = None
@@ -35,15 +27,15 @@
 class CreateAddressInputData(BaseModel):
     currency: str
     network: str
     label: str
 
 
 class CreateAddressOutputData(BaseModel):
-    address: NewAddress
+    address: Address
 
 
 class GetTransactionsOutputData(BaseModel):
     transactions: List
 
 
 class GetAddresses(BaseMethod):
```

### Comparing `bitpapa_pay-0.1.7/bitpapa_pay/methods/base.py` & `bitpapa_pay-0.1.8/bitpapa_pay/methods/base.py`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.7/bitpapa_pay/methods/exchange_rates.py` & `bitpapa_pay-0.1.8/bitpapa_pay/methods/exchange_rates.py`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.7/bitpapa_pay/methods/telegram.py` & `bitpapa_pay-0.1.8/bitpapa_pay/methods/telegram.py`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.7/bitpapa_pay/types/telegram.py` & `bitpapa_pay-0.1.8/bitpapa_pay/types/telegram.py`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.7/PKG-INFO` & `bitpapa_pay-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitpapa-pay
-Version: 0.1.7
+Version: 0.1.8
 Summary: Bitpapa Pay async python wrapper
 Author: VasilevAlexandr97
 Author-email: vasilev.alex.work@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


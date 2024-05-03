# Comparing `tmp/bitpapa_pay-0.1.8.tar.gz` & `tmp/bitpapa_pay-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitpapa_pay-0.1.8.tar", max compression
+gzip compressed data, was "bitpapa_pay-0.1.9.tar", max compression
```

## Comparing `bitpapa_pay-0.1.8.tar` & `bitpapa_pay-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1138 2024-04-12 18:48:56.761770 bitpapa_pay-0.1.8/README.md
--rw-r--r--   0        0        0       42 2024-04-11 08:47:40.794934 bitpapa_pay-0.1.8/bitpapa_pay/__init__.py
--rw-r--r--   0        0        0     6522 2024-04-24 17:55:52.551475 bitpapa_pay-0.1.8/bitpapa_pay/client.py
--rw-r--r--   0        0        0     3677 2024-05-03 00:31:25.500266 bitpapa_pay-0.1.8/bitpapa_pay/methods/addresses.py
--rw-r--r--   0        0        0      608 2024-04-12 20:23:58.411916 bitpapa_pay-0.1.8/bitpapa_pay/methods/base.py
--rw-r--r--   0        0        0      686 2024-04-12 20:26:00.463851 bitpapa_pay-0.1.8/bitpapa_pay/methods/exchange_rates.py
--rw-r--r--   0        0        0     2405 2024-04-24 16:33:12.237628 bitpapa_pay-0.1.8/bitpapa_pay/methods/telegram.py
--rw-r--r--   0        0        0      261 2024-04-12 20:22:45.616006 bitpapa_pay-0.1.8/bitpapa_pay/types/base.py
--rw-r--r--   0        0        0      124 2024-04-12 20:25:33.931857 bitpapa_pay-0.1.8/bitpapa_pay/types/exchange_rates.py
--rw-r--r--   0        0        0      816 2024-04-24 16:36:05.257339 bitpapa_pay-0.1.8/bitpapa_pay/types/telegram.py
--rw-r--r--   0        0        0       18 2024-05-03 00:31:48.680230 bitpapa_pay-0.1.8/bitpapa_pay/version.py
--rw-r--r--   0        0        0      371 2024-05-03 00:33:41.224060 bitpapa_pay-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 bitpapa_pay-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1138 2024-04-12 18:48:56.761770 bitpapa_pay-0.1.9/README.md
+-rw-r--r--   0        0        0       42 2024-04-11 08:47:40.794934 bitpapa_pay-0.1.9/bitpapa_pay/__init__.py
+-rw-r--r--   0        0        0     6522 2024-04-24 17:55:52.551475 bitpapa_pay-0.1.9/bitpapa_pay/client.py
+-rw-r--r--   0        0        0     3381 2024-05-03 00:57:15.163653 bitpapa_pay-0.1.9/bitpapa_pay/methods/addresses.py
+-rw-r--r--   0        0        0      610 2024-05-03 00:56:47.291785 bitpapa_pay-0.1.9/bitpapa_pay/methods/base.py
+-rw-r--r--   0        0        0      688 2024-05-03 00:57:27.087597 bitpapa_pay-0.1.9/bitpapa_pay/methods/exchange_rates.py
+-rw-r--r--   0        0        0     2415 2024-05-03 00:57:40.267536 bitpapa_pay-0.1.9/bitpapa_pay/methods/telegram.py
+-rw-r--r--   0        0        0      659 2024-05-03 00:52:58.389040 bitpapa_pay-0.1.9/bitpapa_pay/schemas/addresses.py
+-rw-r--r--   0        0        0      261 2024-04-12 20:22:45.616006 bitpapa_pay-0.1.9/bitpapa_pay/schemas/base.py
+-rw-r--r--   0        0        0      124 2024-04-12 20:25:33.931857 bitpapa_pay-0.1.9/bitpapa_pay/schemas/exchange_rates.py
+-rw-r--r--   0        0        0      816 2024-04-24 16:36:05.257339 bitpapa_pay-0.1.9/bitpapa_pay/schemas/telegram.py
+-rw-r--r--   0        0        0       18 2024-05-03 00:58:33.903297 bitpapa_pay-0.1.9/bitpapa_pay/version.py
+-rw-r--r--   0        0        0      371 2024-05-03 00:58:49.419230 bitpapa_pay-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 bitpapa_pay-0.1.9/PKG-INFO
```

### Comparing `bitpapa_pay-0.1.8/README.md` & `bitpapa_pay-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.8/bitpapa_pay/client.py` & `bitpapa_pay-0.1.9/bitpapa_pay/client.py`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.8/bitpapa_pay/methods/addresses.py` & `bitpapa_pay-0.1.9/bitpapa_pay/methods/addresses.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,15 @@
-from typing import List, Literal, Optional, Type, Union
-from uuid import UUID
-
-from pydantic import BaseModel
+from typing import Literal, Optional, Type
 
 from bitpapa_pay.methods.base import BaseMethod, BaseOutData
-
-
-class Address(BaseModel):
-    id: UUID
-    address: Optional[str]
-    currency: str
-    network: str
-    balance: Optional[Union[int, float]]
-    label: str
-
-
-class GetAddressesOutputData(BaseModel):
-    addresses: List[Address]
-
-
-class GetAddressesParams(BaseModel):
-    currency: Optional[str] = None
-    label: Optional[str] = None
-
-
-class CreateAddressInputData(BaseModel):
-    currency: str
-    network: str
-    label: str
-
-
-class CreateAddressOutputData(BaseModel):
-    address: Address
-
-
-class GetTransactionsOutputData(BaseModel):
-    transactions: List
+from bitpapa_pay.schemas.addresses import (CreateAddressInputData,
+                                           CreateAddressOutputData,
+                                           GetAddressesOutputData,
+                                           GetAddressesParams,
+                                           GetTransactionsOutputData)
 
 
 class GetAddresses(BaseMethod):
     def __init__(
         self,
         currency: Optional[str] = None,
         label: Optional[str] = None
```

### Comparing `bitpapa_pay-0.1.8/bitpapa_pay/methods/base.py` & `bitpapa_pay-0.1.9/bitpapa_pay/methods/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import Any, Literal
 
-from bitpapa_pay.types.base import BaseOutData
+from bitpapa_pay.schemas.base import BaseOutData
 
 
 class BaseMethod(ABC):
     @property
     @abstractmethod
     def endpoint(self) -> str:
         pass
```

### Comparing `bitpapa_pay-0.1.8/bitpapa_pay/methods/exchange_rates.py` & `bitpapa_pay-0.1.9/bitpapa_pay/methods/exchange_rates.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Literal, Type
 
 from bitpapa_pay.methods.base import BaseMethod, BaseOutData
-from bitpapa_pay.types.exchange_rates import GetExchangeRatesOut
+from bitpapa_pay.schemas.exchange_rates import GetExchangeRatesOut
 
 
 class GetExchangeRates(BaseMethod):
     @property
     def endpoint(self) -> str:
         return "/api/v1/exchange_rates/all"
```

### Comparing `bitpapa_pay-0.1.8/bitpapa_pay/methods/telegram.py` & `bitpapa_pay-0.1.9/bitpapa_pay/methods/telegram.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Literal, Type, Union, Optional
+from typing import Literal, Optional, Type, Union
 
 from bitpapa_pay.methods.base import BaseMethod, BaseOutData
-from bitpapa_pay.types.telegram import (CreateTelegramInvoiceInputData,
-                                        CreateTelegramInvoiceOutputData,
-                                        GetTelegramInvoicesInputParams,
-                                        TelegramInvoiceInputData,
-                                        TelegramInvoices)
+from bitpapa_pay.schemas.telegram import (CreateTelegramInvoiceInputData,
+                                          CreateTelegramInvoiceOutputData,
+                                          GetTelegramInvoicesInputParams,
+                                          TelegramInvoiceInputData,
+                                          TelegramInvoices)
 
 
 class CreateTelegramInvoice(BaseMethod):
     def __init__(
         self,
         api_token: str,
         currency_code: str,
```

### Comparing `bitpapa_pay-0.1.8/bitpapa_pay/types/telegram.py` & `bitpapa_pay-0.1.9/bitpapa_pay/schemas/telegram.py`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.8/PKG-INFO` & `bitpapa_pay-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitpapa-pay
-Version: 0.1.8
+Version: 0.1.9
 Summary: Bitpapa Pay async python wrapper
 Author: VasilevAlexandr97
 Author-email: vasilev.alex.work@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


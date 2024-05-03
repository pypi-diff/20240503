# Comparing `tmp/novaposhta_python_client-0.1.5.tar.gz` & `tmp/novaposhta_python_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novaposhta_python_client-0.1.5.tar", max compression
+gzip compressed data, was "novaposhta_python_client-0.1.6.tar", max compression
```

## Comparing `novaposhta_python_client-0.1.5.tar` & `novaposhta_python_client-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1086 2023-10-25 11:55:01.000186 novaposhta_python_client-0.1.5/LICENSE.md
--rw-r--r--   0        0        0     4128 2024-01-10 10:15:13.965869 novaposhta_python_client-0.1.5/README.md
--rw-r--r--   0        0        0       58 2023-10-10 10:31:46.199224 novaposhta_python_client-0.1.5/novaposhta/__init__.py
--rw-r--r--   0        0        0     6266 2023-11-23 11:34:00.459771 novaposhta_python_client-0.1.5/novaposhta/client.py
--rw-r--r--   0        0        0        0 2023-10-10 10:31:46.199556 novaposhta_python_client-0.1.5/novaposhta/models/__init__.py
--rw-r--r--   0        0        0     7429 2023-10-10 10:31:46.200046 novaposhta_python_client-0.1.5/novaposhta/models/additional_service.py
--rw-r--r--   0        0        0     7441 2023-10-10 10:31:46.200284 novaposhta_python_client-0.1.5/novaposhta/models/address.py
--rw-r--r--   0        0        0     1590 2023-10-10 11:42:36.786733 novaposhta_python_client-0.1.5/novaposhta/models/base.py
--rw-r--r--   0        0        0     3368 2023-10-10 10:31:46.200537 novaposhta_python_client-0.1.5/novaposhta/models/common.py
--rw-r--r--   0        0        0     2106 2023-10-10 10:31:46.200664 novaposhta_python_client-0.1.5/novaposhta/models/contact_person.py
--rw-r--r--   0        0        0     4224 2023-10-10 10:31:46.200785 novaposhta_python_client-0.1.5/novaposhta/models/counterparty.py
--rw-r--r--   0        0        0    12493 2023-10-25 11:55:01.002033 novaposhta_python_client-0.1.5/novaposhta/models/internet_document.py
--rw-r--r--   0        0        0     1742 2023-10-10 10:31:46.201286 novaposhta_python_client-0.1.5/novaposhta/models/scan_sheet.py
--rw-r--r--   0        0        0      591 2023-10-10 10:31:46.201443 novaposhta_python_client-0.1.5/novaposhta/models/tracking_document.py
--rw-r--r--   0        0        0       20 2023-10-10 10:31:46.201754 novaposhta_python_client-0.1.5/novaposhta/mypi.ini
--rw-r--r--   0        0        0      488 2023-11-23 11:34:00.460542 novaposhta_python_client-0.1.5/novaposhta/types.py
--rw-r--r--   0        0        0     1196 2024-01-10 10:15:58.536676 novaposhta_python_client-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5136 1970-01-01 00:00:00.000000 novaposhta_python_client-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-10-25 11:55:01.000186 novaposhta_python_client-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0     4552 2024-05-03 10:13:28.947902 novaposhta_python_client-0.1.6/README.md
+-rw-r--r--   0        0        0       58 2023-10-10 10:31:46.199224 novaposhta_python_client-0.1.6/novaposhta/__init__.py
+-rw-r--r--   0        0        0     7766 2024-05-03 09:58:00.624776 novaposhta_python_client-0.1.6/novaposhta/client.py
+-rw-r--r--   0        0        0        0 2023-10-10 10:31:46.199556 novaposhta_python_client-0.1.6/novaposhta/models/__init__.py
+-rw-r--r--   0        0        0     7429 2023-10-10 10:31:46.200046 novaposhta_python_client-0.1.6/novaposhta/models/additional_service.py
+-rw-r--r--   0        0        0     7441 2023-10-10 10:31:46.200284 novaposhta_python_client-0.1.6/novaposhta/models/address.py
+-rw-r--r--   0        0        0     1590 2023-10-10 11:42:36.786733 novaposhta_python_client-0.1.6/novaposhta/models/base.py
+-rw-r--r--   0        0        0     3368 2023-10-10 10:31:46.200537 novaposhta_python_client-0.1.6/novaposhta/models/common.py
+-rw-r--r--   0        0        0     2106 2023-10-10 10:31:46.200664 novaposhta_python_client-0.1.6/novaposhta/models/contact_person.py
+-rw-r--r--   0        0        0     4224 2023-10-10 10:31:46.200785 novaposhta_python_client-0.1.6/novaposhta/models/counterparty.py
+-rw-r--r--   0        0        0    12493 2023-10-25 11:55:01.002033 novaposhta_python_client-0.1.6/novaposhta/models/internet_document.py
+-rw-r--r--   0        0        0     1742 2023-10-10 10:31:46.201286 novaposhta_python_client-0.1.6/novaposhta/models/scan_sheet.py
+-rw-r--r--   0        0        0      591 2023-10-10 10:31:46.201443 novaposhta_python_client-0.1.6/novaposhta/models/tracking_document.py
+-rw-r--r--   0        0        0       20 2023-10-10 10:31:46.201754 novaposhta_python_client-0.1.6/novaposhta/mypi.ini
+-rw-r--r--   0        0        0      488 2023-11-23 11:34:00.460542 novaposhta_python_client-0.1.6/novaposhta/types.py
+-rw-r--r--   0        0        0     1196 2024-05-03 10:15:55.463766 novaposhta_python_client-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5560 1970-01-01 00:00:00.000000 novaposhta_python_client-0.1.6/PKG-INFO
```

### Comparing `novaposhta_python_client-0.1.5/LICENSE.md` & `novaposhta_python_client-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `novaposhta_python_client-0.1.5/README.md` & `novaposhta_python_client-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -35,36 +35,56 @@
 # Example usage of different models
 settlements = client.address.search_settlements(city_name='Київ', limit=5)
 my_pack_list = client.common.get_pack_list(length=1, width=5)
 return_reason = client.additional_service.get_return_reasons()
 
 # Print results
 print(settlements, my_pack_list, return_reason)
+client.close_sync()
 ```
+Please, close the client whenever you are done with it to avoid resource leaks.
 
 You can also use async client:
 
 ```python
 import asyncio
 from novaposhta.client import NovaPoshtaApi
 
-async_client = NovaPoshtaApi('my-api-token', timeout=30, async_mode=True)
-a_address = async_client.address
-a_settlement = asyncio.run(a_address.search_settlements(city_name='Київ', limit=5))
-print(a_settlement)
+async def use_api_async():
+    async_client = NovaPoshtaApi('your_api_key', timeout=30, async_mode=True, raise_for_errors=True)
+    address = async_client.address
+    settlements = await address.search_settlements(city_name='Київ', limit=5)
+    print(settlements)
+    await async_client.close_async()
+asyncio.run(use_api_async())
+```
+
+You can use context manager to automatically close the client:
+
+```python
+from novaposhta.client import NovaPoshtaApi
+def use_api_sync():
+    with NovaPoshtaApi(api_key='your_api_key', async_mode=False) as api:
+        # Do something with the API
+        pass
+
+async def use_api_async():
+    async with NovaPoshtaApi(api_key='your_api_key', async_mode=True) as api:
+        # Do something with the API
+        pass
 ```
 
 ## Error handling
 
 ```python
 import httpx
 from novaposhta.client import NovaPoshtaApi, InvalidAPIKeyError, APIRequestError
 
 # Instantiate the client
-client = NovaPoshtaApi('my-api-token', timeout=30, raise_for_errors=True)
+client = NovaPoshtaApi('your_api_key', timeout=30, raise_for_errors=True)
 
 try:
     client.common.get_cargo_types()
 except httpx.HTTPError as error:
     print(f"HTTP error: {error}")
 except InvalidAPIKeyError as error:
     print(f"API key expired or otherwise invalid: {error}")
@@ -79,24 +99,15 @@
 While `httpx` is the default HTTP library, you can easily substitute it with requests or another library, provided it
 follows the same interface:
 
 ```python
 from novaposhta.client import NovaPoshtaApi
 import my_http_client
 
-client = NovaPoshtaApi('my-api-token', http_client=my_http_client.Client)
-```
-
-Custom client should support context manager, e.g:
-
-```python
-with self.http_client() as client:
-    response = client.post(
-        self.api_endpoint, json=request, headers=HEADERS, timeout=self.timeout
-    )
+client = NovaPoshtaApi('your_api_key', http_client=my_http_client.Client)
 ```
 
 ### Adding New Methods
 
 If a method isn’t implemented, or you prefer a custom implementation, extend the model as shown below:
 
 ```python
```

### Comparing `novaposhta_python_client-0.1.5/novaposhta/client.py` & `novaposhta_python_client-0.1.6/novaposhta/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,94 +1,100 @@
 """Client for Nova Poshta API. """
 
+from typing import Type, TypeVar, Optional, Callable
+
 import httpx
 
-from .models.base import BaseModel
+from .models.additional_service import AdditionalService
 from .models.address import Address
-from .models.counterparty import Counterparty
-from .models.contact_person import ContactPerson
-from .models.scan_sheet import ScanSheet
+from .models.base import BaseModel
 from .models.common import Common
-from .models.additional_service import AdditionalService
+from .models.contact_person import ContactPerson
+from .models.counterparty import Counterparty
 from .models.internet_document import InternetDocument
+from .models.scan_sheet import ScanSheet
 from .models.tracking_document import TrackingDocument
 from .types import DictStrAny, MaybeAsync
 
-from typing import Type, TypeVar, Union
-
 HEADERS = {"Content-Type": "application/json"}
 
 BaseModelType = TypeVar("BaseModelType", bound=BaseModel)
 
 
 class NovaPoshtaApi:
     """
     Base class that wraps call to the Nova Poshta API.
     Prepares requests and builds proper resource location.
     All API models can be accessed as instance properties.
     Info about models can be found here:
     https://developers.novaposhta.ua/documentation
     """
 
+    sync_http_client: Optional[httpx.Client] = None
+    async_http_client: Optional[httpx.AsyncClient] = None
+
     def __init__(
         self,
-        api_key,
-        api_endpoint="https://api.novaposhta.ua/v2.0/json/",
+        api_key: str,
+        api_endpoint: str = "https://api.novaposhta.ua/v2.0/json/",
         http_client=httpx,
-        timeout=10,
-        raise_for_errors=False,
-        async_mode=False,
+        timeout: int = 10,
+        raise_for_errors: bool = False,
+        async_mode: bool = False,
     ):
         """
         Initialize Nova Poshta API client.
 
         :param api_key: API key from Nova Poshta.
         :param api_endpoint: API endpoint to use.
         :param http_client: HTTP client to use. Defaults to httpx.
         :param timeout: Timeout for HTTP requests.
         :param raise_for_errors: Whether to check and raise errors as exceptions.
         :param async_mode: Whether to use async mode.
         """
         self.api_key = api_key
         self.api_endpoint = api_endpoint
-        self.http_client = (
-            http_client.Client if not async_mode else http_client.AsyncClient
-        )
         self.timeout = timeout
-        self.raise_for_errors = raise_for_errors
-        self.async_mode = async_mode
-        self._models_pool = {}
-
-        if self.async_mode:
+        self._send: Callable[[DictStrAny], MaybeAsync]
+        if async_mode:
+            self.async_http_client: Optional[
+                httpx.AsyncClient
+            ] = http_client.AsyncClient(timeout=timeout)
             self._send = self._send_async
-
         else:
+            self.sync_http_client: Optional[httpx.Client] = http_client.Client(
+                timeout=timeout
+            )
             self._send = self._send_sync
+        self.raise_for_errors = raise_for_errors
+        self.async_mode = async_mode
+        self._models_pool: DictStrAny = {}
 
     def _send_sync(self, request: DictStrAny) -> DictStrAny:
         """
         Sends sync request to the API.
 
         :param request: request dict.
         :return: response dict.
         """
-
-        with self.http_client() as client:
-            response = client.post(**request)
+        if not self.sync_http_client:
+            raise ValueError("Sync client is not initialized")
+        response = self.sync_http_client.post(**request)
         return self._maybe_check_errors(response.json())
 
     async def _send_async(self, request: DictStrAny) -> DictStrAny:
         """
         Sends async request to the API.
 
         :param request: request dict.
         :return: response dict.
         """
-        async with self.http_client() as client:
-            response = await client.post(**request)
+        if not self.async_http_client:
+            raise ValueError("Async client is not initialized")
+        response: httpx.Response = await self.async_http_client.post(**request)
         return self._maybe_check_errors(response.json())
 
     def send(
         self, model_name: str, api_method: str, method_props: DictStrAny
     ) -> MaybeAsync:
         """
         Sends request to the API.
@@ -123,35 +129,80 @@
         :param model: model to add.
         """
         if model.name in self._models_pool:
             del self._models_pool[model.name]
         self._models_pool[model.name] = model(self)
         return self._models_pool[model.name]
 
-    def get(self, name: str) -> Union[BaseModelType, None]:
+    def get(self, name: str) -> Optional[BaseModel]:
         """
         Get model from the pool.
 
         :param name: name of the model to get.
         """
         return self._models_pool.get(name)
 
-    def _maybe_check_errors(self, response):
+    def _maybe_check_errors(self, response: DictStrAny) -> DictStrAny:
+        """
+        Check response for errors.
+
+        :param response: response dict.
+        :return: response dict.
+        """
         if not self.raise_for_errors:
             return response
 
         if response["success"]:
             return response
 
         error = response["errors"][0]
         if error.startswith("API key"):
             raise InvalidAPIKeyError(error)
         else:
             raise APIRequestError(error)
 
+    def close_sync(self):
+        """
+        Close sync client.
+        """
+        if self.sync_http_client:
+            self.sync_http_client.close()
+
+    async def close_async(self):
+        """
+        Close async client.
+        """
+        if self.async_http_client:
+            await self.async_http_client.aclose()
+
+    def __enter__(self):
+        """
+        Enter the context.
+        """
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        """
+        Exit the context.
+        Close the client.
+        """
+        self.close_sync()
+
+    async def __aenter__(self):
+        """
+        Enter the async context.
+        """
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        """
+        Exit the async context.
+        """
+        await self.close_async()
+
     @property
     def address(self) -> Address:
         """
         Provide access to the Address model.
         """
         return self.new(Address)
```

### Comparing `novaposhta_python_client-0.1.5/novaposhta/models/additional_service.py` & `novaposhta_python_client-0.1.6/novaposhta/models/additional_service.py`

 * *Files identical despite different names*

### Comparing `novaposhta_python_client-0.1.5/novaposhta/models/address.py` & `novaposhta_python_client-0.1.6/novaposhta/models/address.py`

 * *Files identical despite different names*

### Comparing `novaposhta_python_client-0.1.5/novaposhta/models/base.py` & `novaposhta_python_client-0.1.6/novaposhta/models/base.py`

 * *Files identical despite different names*

### Comparing `novaposhta_python_client-0.1.5/novaposhta/models/common.py` & `novaposhta_python_client-0.1.6/novaposhta/models/common.py`

 * *Files identical despite different names*

### Comparing `novaposhta_python_client-0.1.5/novaposhta/models/contact_person.py` & `novaposhta_python_client-0.1.6/novaposhta/models/contact_person.py`

 * *Files identical despite different names*

### Comparing `novaposhta_python_client-0.1.5/novaposhta/models/counterparty.py` & `novaposhta_python_client-0.1.6/novaposhta/models/counterparty.py`

 * *Files identical despite different names*

### Comparing `novaposhta_python_client-0.1.5/novaposhta/models/internet_document.py` & `novaposhta_python_client-0.1.6/novaposhta/models/internet_document.py`

 * *Files identical despite different names*

### Comparing `novaposhta_python_client-0.1.5/novaposhta/models/scan_sheet.py` & `novaposhta_python_client-0.1.6/novaposhta/models/scan_sheet.py`

 * *Files identical despite different names*

### Comparing `novaposhta_python_client-0.1.5/novaposhta/models/tracking_document.py` & `novaposhta_python_client-0.1.6/novaposhta/models/tracking_document.py`

 * *Files identical despite different names*

### Comparing `novaposhta_python_client-0.1.5/pyproject.toml` & `novaposhta_python_client-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "novaposhta-python-client"
 packages = [
     { include = "novaposhta"}
 ]
-version = "0.1.5"
+version = "0.1.6"
 description = "Python client for Nova Poshta API"
 authors = ["Oleksii <semolex@live.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/semolex/novaposhta-python-client"
 repository = "https://github.com/semolex/novaposhta-python-client"
 keywords = [ "api", "nova-poshta", "novaposhta", "nova-poshta-api", "novaposhta-api"]
```

### Comparing `novaposhta_python_client-0.1.5/PKG-INFO` & `novaposhta_python_client-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novaposhta-python-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python client for Nova Poshta API
 Home-page: https://github.com/semolex/novaposhta-python-client
 License: MIT
 Keywords: api,nova-poshta,novaposhta,nova-poshta-api,novaposhta-api
 Author: Oleksii
 Author-email: semolex@live.com
 Requires-Python: >=3.9,<4.0
@@ -59,36 +59,56 @@
 # Example usage of different models
 settlements = client.address.search_settlements(city_name='Київ', limit=5)
 my_pack_list = client.common.get_pack_list(length=1, width=5)
 return_reason = client.additional_service.get_return_reasons()
 
 # Print results
 print(settlements, my_pack_list, return_reason)
+client.close_sync()
 ```
+Please, close the client whenever you are done with it to avoid resource leaks.
 
 You can also use async client:
 
 ```python
 import asyncio
 from novaposhta.client import NovaPoshtaApi
 
-async_client = NovaPoshtaApi('my-api-token', timeout=30, async_mode=True)
-a_address = async_client.address
-a_settlement = asyncio.run(a_address.search_settlements(city_name='Київ', limit=5))
-print(a_settlement)
+async def use_api_async():
+    async_client = NovaPoshtaApi('your_api_key', timeout=30, async_mode=True, raise_for_errors=True)
+    address = async_client.address
+    settlements = await address.search_settlements(city_name='Київ', limit=5)
+    print(settlements)
+    await async_client.close_async()
+asyncio.run(use_api_async())
+```
+
+You can use context manager to automatically close the client:
+
+```python
+from novaposhta.client import NovaPoshtaApi
+def use_api_sync():
+    with NovaPoshtaApi(api_key='your_api_key', async_mode=False) as api:
+        # Do something with the API
+        pass
+
+async def use_api_async():
+    async with NovaPoshtaApi(api_key='your_api_key', async_mode=True) as api:
+        # Do something with the API
+        pass
 ```
 
 ## Error handling
 
 ```python
 import httpx
 from novaposhta.client import NovaPoshtaApi, InvalidAPIKeyError, APIRequestError
 
 # Instantiate the client
-client = NovaPoshtaApi('my-api-token', timeout=30, raise_for_errors=True)
+client = NovaPoshtaApi('your_api_key', timeout=30, raise_for_errors=True)
 
 try:
     client.common.get_cargo_types()
 except httpx.HTTPError as error:
     print(f"HTTP error: {error}")
 except InvalidAPIKeyError as error:
     print(f"API key expired or otherwise invalid: {error}")
@@ -103,24 +123,15 @@
 While `httpx` is the default HTTP library, you can easily substitute it with requests or another library, provided it
 follows the same interface:
 
 ```python
 from novaposhta.client import NovaPoshtaApi
 import my_http_client
 
-client = NovaPoshtaApi('my-api-token', http_client=my_http_client.Client)
-```
-
-Custom client should support context manager, e.g:
-
-```python
-with self.http_client() as client:
-    response = client.post(
-        self.api_endpoint, json=request, headers=HEADERS, timeout=self.timeout
-    )
+client = NovaPoshtaApi('your_api_key', http_client=my_http_client.Client)
 ```
 
 ### Adding New Methods
 
 If a method isn’t implemented, or you prefer a custom implementation, extend the model as shown below:
 
 ```python
```


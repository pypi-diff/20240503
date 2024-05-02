# Comparing `tmp/liminal_sdk_python-2024.4.3.tar.gz` & `tmp/liminal_sdk_python-2024.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liminal_sdk_python-2024.4.3.tar", max compression
+gzip compressed data, was "liminal_sdk_python-2024.5.0b0.tar", max compression
```

## Comparing `liminal_sdk_python-2024.4.3.tar` & `liminal_sdk_python-2024.5.0b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/LICENSE
--rw-r--r--   0        0        0    13136 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/README.md
--rw-r--r--   0        0        0       82 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/__init__.py
--rw-r--r--   0        0        0      524 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/auth/__init__.py
--rw-r--r--   0        0        0       34 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/auth/microsoft/__init__.py
--rw-r--r--   0        0        0     2961 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/auth/microsoft/device_code_flow.py
--rw-r--r--   0        0        0      873 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/auth/microsoft/models.py
--rw-r--r--   0        0        0     8731 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/client.py
--rw-r--r--   0        0        0      165 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/const.py
--rw-r--r--   0        0        0       45 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/__init__.py
--rw-r--r--   0        0        0     2135 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/llm/__init__.py
--rw-r--r--   0        0        0     2284 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/llm/models.py
--rw-r--r--   0        0        0     5463 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/prompt/__init__.py
--rw-r--r--   0        0        0     3264 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/prompt/models.py
--rw-r--r--   0        0        0     2372 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/thread/__init__.py
--rw-r--r--   0        0        0     2162 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/thread/models.py
--rw-r--r--   0        0        0      400 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/errors.py
--rw-r--r--   0        0        0       22 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/helpers/__init__.py
--rw-r--r--   0        0        0      382 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/helpers/model.py
--rw-r--r--   0        0        0      109 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/helpers/typing.py
--rw-r--r--   0        0        0     8522 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/pyproject.toml
--rw-r--r--   0        0        0    14258 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/LICENSE
+-rw-r--r--   0        0        0    12819 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/README.md
+-rw-r--r--   0        0        0       82 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/__init__.py
+-rw-r--r--   0        0        0      524 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/auth/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/auth/microsoft/__init__.py
+-rw-r--r--   0        0        0     2961 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/auth/microsoft/device_code_flow.py
+-rw-r--r--   0        0        0      873 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/auth/microsoft/models.py
+-rw-r--r--   0        0        0     8055 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/client.py
+-rw-r--r--   0        0        0      165 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/const.py
+-rw-r--r--   0        0        0       45 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/__init__.py
+-rw-r--r--   0        0        0     2135 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/llm/__init__.py
+-rw-r--r--   0        0        0     2090 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/llm/models.py
+-rw-r--r--   0        0        0     5463 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/prompt/__init__.py
+-rw-r--r--   0        0        0     3264 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/prompt/models.py
+-rw-r--r--   0        0        0     2372 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/thread/__init__.py
+-rw-r--r--   0        0        0     2162 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/thread/models.py
+-rw-r--r--   0        0        0      400 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/errors.py
+-rw-r--r--   0        0        0       22 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/helpers/__init__.py
+-rw-r--r--   0        0        0      382 2024-05-02 23:19:50.761433 liminal_sdk_python-2024.5.0b0/liminal/helpers/model.py
+-rw-r--r--   0        0        0      109 2024-05-02 23:19:50.761433 liminal_sdk_python-2024.5.0b0/liminal/helpers/typing.py
+-rw-r--r--   0        0        0    13901 2024-05-02 23:19:50.761433 liminal_sdk_python-2024.5.0b0/pyproject.toml
+-rw-r--r--   0        0        0    13943 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.5.0b0/PKG-INFO
```

### Comparing `liminal_sdk_python-2024.4.3/LICENSE` & `liminal_sdk_python-2024.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.3/README.md` & `liminal_sdk_python-2024.5.0b0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 import asyncio
 
 from liminal import Client
 from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
 
 
 async def main() -> None:
-    """Create the aiohttp session and run the example."""
+    """Run!"""
     # Create an auth provider to authenticate the user:
     auth_provider = DeviceCodeFlowProvider("<TENANT_ID>", "<CLIENT_ID>")
 
     # Create the liminal SDK instance:
     liminal = Client(auth_provider, "<LIMINAL_API_SERVER_URL>")
 
 
@@ -98,15 +98,15 @@
 import asyncio
 
 from liminal import Client
 from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
 
 
 async def main() -> None:
-    """Create the aiohttp session and run the example."""
+    """Run!"""
     # Create an auth provider to authenticate the user:
     auth_provider = DeviceCodeFlowProvider("<TENANT_ID>", "<CLIENT_ID>")
 
     # Create the liminal SDK instance and authenticate it:
     liminal = Client(auth_provider, "<LIMINAL_API_SERVER_URL>")
     await liminal.authenticate_from_auth_provider()
 
@@ -124,81 +124,76 @@
 Leaving your application running, open a browser at that URL and input the code as
 instructed. Once you successfully complete authentication via Entra ID, your Liminal
 client object will automatically authenticate with your Liminal API server.
 
 # Ongoing Authentication
 
 After the initial authentication with your auth provider, the Liminal client object will
-internally store access and refresh tokens to ensure the ongoing ability to communicate
-with your Liminal API server. The client object will automatically handle using the
-stored refresh token to request new access tokens as appropriate.
-
-## Manually Interacting with the Refresh Token
-
-The Liminal client object provides a `add_refresh_token_callback` method to manually
-interact with refresh tokens as they are generated. This is useful in situations where
-you want to retrieve that token and do something else with (store it in a database, for
-example). Every time a new refresh token is generated by the client object, the
-registered callbacks will be called.
-
-Refresh token callbacks are methods that take a single `str` parameter (denoting the
-refresh token). These callbacks are not expected to return any value. Lastly, when
-calling `add_refresh_token_callback`, the returned method allows you to cancel the
+internally manage sessions to ensure the ongoing ability to communicate with your
+Liminal API server. The client object will automatically handle using the stored refresh
+token to request new access tokens as appropriate.
+
+## Manually Interacting with the Session ID
+
+The Liminal client object provides a `add_session_id_callback` method to manually
+interact with session IDs as they are generated. This is useful in situations where you
+want to retrieve that ID and do something else with (store it in a database, for
+example). Every time a new session is generated by the client object, the registered
+callbacks will be called.
+
+Session ID callbacks are methods that take a single `str` parameter (denoting the
+session ID itself). These callbacks are not expected to return any value. Lastly,
+when calling `add_session_id_callback`, the returned method allows you to cancel the
 callback at any time.
 
 ```python
 import asyncio
 
 from liminal import Client
 from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
 
 
 async def main() -> None:
-    """Create the aiohttp session and run the example."""
+    """Run!"""
     # Create an auth provider to authenticate the user:
     auth_provider = DeviceCodeFlowProvider("<TENANT_ID>", "<CLIENT_ID>")
 
     # Create the liminal SDK instance and authenticate it:
     liminal = Client(microsoft_auth_provider, "<LIMINAL_API_SERVER_URL>")
     await liminal.authenticate_from_auth_provider()
 
-    def do_something_with_refresh_token(refresh_token: str) -> None:
-        """Do something with the refresh token."""
-        pass
+    def print_session_id(session_id: str) -> None:
+        """Do something with the session ID."""
+        print(f"Session ID: {session_id}")
 
     # Register the refresh token callback:
-    remove_callback = liminal.add_refresh_token_callback(
-        do_something_with_refresh_token
-    )
+    remove_callback = liminal.add_session_id_callback(print_session_id)
 
     # Later, if you want to remove the callback:
     remove_callback()
 
 
 asyncio.run(main())
 ```
 
-## Creating a Liminal Client from a Stored Refresh Token
+## Creating a Liminal Client from a Stored Session ID
 
-Assuming you have a stored refresh token (collected from the callback process shown
-above), it is simple to create a new Limina client using that token:
+Assuming you have a stored session ID (collected from the callback process shown
+above), it is simple to create a new Liminal client using that ID:
 
 ```python
 import asyncio
 
 from liminal import Client
 
 
 async def main() -> None:
-    """Create the aiohttp session and run the example."""
-    # Retrieve your stored refresh_token:
-    refresh_token = "12345"
-
+    """Run!"""
     # Create the client:
-    liminal = await client.authenticate_from_refresh_token(refresh_token=refresh_token)
+    liminal = await client.authenticate_from_session_id(session="my-session-id")
 
 
 asyncio.run(main())
 ```
 
 # Endpoints
```

### Comparing `liminal_sdk_python-2024.4.3/liminal/auth/__init__.py` & `liminal_sdk_python-2024.5.0b0/liminal/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.3/liminal/auth/microsoft/device_code_flow.py` & `liminal_sdk_python-2024.5.0b0/liminal/auth/microsoft/device_code_flow.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.3/liminal/auth/microsoft/models.py` & `liminal_sdk_python-2024.5.0b0/liminal/auth/microsoft/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.3/liminal/client.py` & `liminal_sdk_python-2024.5.0b0/liminal/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Define the client module."""
 
 from __future__ import annotations
 
 import asyncio
 from collections.abc import Callable
-from datetime import UTC, datetime
 from json.decoder import JSONDecodeError
 from typing import Final
 
 from httpx import AsyncClient, Cookies, HTTPStatusError, Request, Response
 from mashumaro.codecs.json import json_decode
 from mashumaro.exceptions import (
     MissingField,
@@ -47,33 +46,31 @@
 
         """
         self._api_server_url = api_server_url
         self._auth_provider = auth_provider
         self._httpx_client = httpx_client
 
         # Token information:
-        self._access_token: str | None = None
-        self._access_token_expires_at: datetime | None = None
         self._refresh_lock = asyncio.Lock()
-        self._refresh_token: str | None = None
-        self._refresh_token_callbacks: list[Callable[[str], None]] = []
         self._refreshing = False
+        self._session_id: str | None = None
+        self._session_id_callbacks: list[Callable[[str], None]] = []
 
         # Define endpoints:
         self.llm = LLMEndpoint(self._request_and_validate)
         self.prompt = PromptEndpoint(self._request_and_validate)
         self.thread = ThreadEndpoint(self._request, self._request_and_validate)
 
     async def _request(
         self,
         method: str,
         endpoint: str,
         *,
         headers: dict[str, str] | None = None,
-        cookies: Cookies | None = None,
+        cookies: dict[str, str] | None = None,
         params: dict[str, str] | None = None,
         json: dict[str, str] | None = None,
     ) -> Response:
         """Make a request to the Liminal API server and return a Response.
 
         Args:
         ----
@@ -89,35 +86,33 @@
             An HTTPX Response object.
 
         Raises:
         ------
             RequestError: If the response fails for any reason.
 
         """
-        utcnow = datetime.now(tz=UTC)
-        if self._access_token_expires_at and utcnow >= self._access_token_expires_at:
-            LOGGER.debug("Access token expired, refreshing...")
-            self._access_token = None
-            self._access_token_expires_at = None
-            await self.authenticate_from_refresh_token()
-
         url = f"{self._api_server_url}{endpoint}"
 
-        if not headers:
-            headers = {}
-        if self._access_token:
-            headers["Authorization"] = f"Bearer {self._access_token}"
+        if not cookies:
+            cookies = {}
+        if self._session_id:
+            cookies["session"] = self._session_id
 
         if running_client := self._httpx_client and not self._httpx_client.is_closed:
             client = self._httpx_client
         else:
             client = AsyncClient()
 
         request = Request(
-            method, url, headers=headers, cookies=cookies, params=params, json=json
+            method,
+            url,
+            headers=headers,
+            cookies=Cookies(cookies),
+            params=params,
+            json=json,
         )
         response = await client.send(request)
 
         try:
             response.raise_for_status()
         except HTTPStatusError as err:
             msg = (
@@ -135,15 +130,15 @@
     async def _request_and_validate(
         self,
         method: str,
         endpoint: str,
         expected_response_type: type[ValidatedResponseT],
         *,
         headers: dict[str, str] | None = None,
-        cookies: Cookies | None = None,
+        cookies: dict[str, str] | None = None,
         params: dict[str, str] | None = None,
         json: dict[str, str] | None = None,
     ) -> ValidatedResponseT:
         """Make a request to the Liminal API server and validate the response.
 
         Args:
         ----
@@ -175,95 +170,92 @@
             MissingField,
             SuitableVariantNotFoundError,
             UnserializableDataError,
         ) as err:
             msg = f"Could not validate response: {err}"
             raise RequestError(msg) from err
 
-    def _save_tokens_from_auth_response(self, auth_response: Response) -> None:
-        """Save tokens from an auth response.
+    def _save_session_id_from_auth_response(self, auth_response: Response) -> None:
+        """Save a session cookie value from an auth response.
 
         Args:
         ----
             auth_response: The response from an auth request.
 
         """
-        LOGGER.debug("Saving tokens from auth response")
-        self._access_token = auth_response.cookies["accessToken"]
-        self._access_token_expires_at = datetime.fromtimestamp(
-            int(auth_response.cookies["accessTokenExpiresAt"]) / 1000, tz=UTC
-        )
-        self._refresh_token = auth_response.cookies["refreshToken"]
+        LOGGER.debug("Saving session cookie from auth response")
+        self._session_id = auth_response.cookies["session"]
 
-        for callback in self._refresh_token_callbacks:
-            callback(self._refresh_token)
+        if self._session_id:
+            for callback in self._session_id_callbacks:
+                callback(self._session_id)
 
-    def add_refresh_token_callback(
+    def add_session_id_callback(
         self, callback: Callable[[str], None]
     ) -> Callable[[], None]:
-        """Add a callback to be called when a new refresh token is generated.
+        """Add a callback to be called when a new session is generated.
 
-        The purpose of this is to allow the user to save the refresh token to a
+        The purpose of this is to allow the user to save the session ID to a
         persistent store using their own callback method.
 
         Args:
         ----
             callback: The callback to add.
 
         Returns:
         -------
             A method to cancel and remove the callback.
 
         """
-        self._refresh_token_callbacks.append(callback)
+        self._session_id_callbacks.append(callback)
 
         def cancel() -> None:
             """Cancel and remove the callback."""
-            self._refresh_token_callbacks.remove(callback)
+            self._session_id_callbacks.remove(callback)
 
         return cancel
 
     async def authenticate_from_auth_provider(self) -> None:
         """Authenticate with the Liminal API server (using the auth provider)."""
         provider_access_token = await self._auth_provider.get_access_token()
         liminal_auth_response = await self._request(
             "GET",
             "/api/v1/auth/login/oauth/access-token",
             headers={"Authorization": f"Bearer {provider_access_token}"},
         )
-        self._save_tokens_from_auth_response(liminal_auth_response)
+        self._save_session_id_from_auth_response(liminal_auth_response)
 
-    async def authenticate_from_refresh_token(
-        self, *, refresh_token: str | None = None
+    async def authenticate_from_session_id(
+        self, *, session_id: str | None = None
     ) -> None:
-        """Authenticate with the Liminal API server (using a refresh token).
+        """Authenticate with the Liminal API server (using a session).
 
         Args:
         ----
-            refresh_token: The refresh token to use. If not provided, the refresh token
-                that was used to authenticate the user initially will be used.
+            session_id: The session ID to use. If not provided, the session that was
+                used to authenticate the user initially will be used.
 
         Raises:
         ------
-            AuthError: If no refresh token is provided and the user has not been
-                authenticated yet.
+            AuthError: If no session is provided and the user has not been authenticated
+                yet.
 
         """
-        if not refresh_token:
-            refresh_token = self._refresh_token
+        if not session_id:
+            session_id = self._session_id
 
-        if not refresh_token:
-            msg = "No valid refresh token provided"
+        if not session_id:
+            msg = "No valid session ID provided"
             raise AuthError(msg)
 
         async with self._refresh_lock:
             self._refreshing = True
 
             try:
-                refresh_token_response = await self._request(
-                    "POST",
-                    "/api/v1/auth/refresh-token",
-                    cookies=Cookies({"refreshToken": refresh_token}),
+                session_id_response = await self._request(
+                    "GET",
+                    "/api/v1/users/me",
+                    cookies={"session": session_id},
                 )
-                self._save_tokens_from_auth_response(refresh_token_response)
+                self._save_session_id_from_auth_response(session_id_response)
             finally:
                 self._refreshing = False
```

### Comparing `liminal_sdk_python-2024.4.3/liminal/endpoints/llm/__init__.py` & `liminal_sdk_python-2024.5.0b0/liminal/endpoints/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.3/liminal/endpoints/llm/models.py` & `liminal_sdk_python-2024.5.0b0/liminal/endpoints/llm/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,20 +32,16 @@
 
     id: int
 
     # References:
     model_instance_id: int = field(metadata=field_options(alias="modelInstanceId"))
 
     # Fields:
-    api_key: str | None = field(default=None, metadata=field_options(alias="apiKey"))
-    masked_api_key: str | None = field(
-        default=None, metadata=field_options(alias="maskedApiKey")
-    )
+    credentials: dict[str, str] | None = field(default_factory=dict)
     model: str
-    params: dict[str, str] | None = field(default_factory=dict)
     provider_key: ModelProviderKey = field(metadata=field_options(alias="providerKey"))
 
     # Timestamps:
     created_at: datetime = field(metadata=field_options(alias="createdAt"))
     deleted_at: datetime | None = field(
         default=None, metadata=field_options(alias="deletedAt")
     )
```

### Comparing `liminal_sdk_python-2024.4.3/liminal/endpoints/prompt/__init__.py` & `liminal_sdk_python-2024.5.0b0/liminal/endpoints/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.3/liminal/endpoints/prompt/models.py` & `liminal_sdk_python-2024.5.0b0/liminal/endpoints/prompt/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.3/liminal/endpoints/thread/__init__.py` & `liminal_sdk_python-2024.5.0b0/liminal/endpoints/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.3/liminal/endpoints/thread/models.py` & `liminal_sdk_python-2024.5.0b0/liminal/endpoints/thread/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.3/PKG-INFO` & `liminal_sdk_python-2024.5.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liminal-sdk-python
-Version: 2024.4.3
+Version: 2024.5.0b0
 Summary: The Liminal SDK for Python
 Home-page: https://github.com/liminal-ai-security/liminal-sdk-python
 License: Apache-2.0
 Author: Aaron Bach
 Author-email: ab@liminal.ai
 Requires-Python: >=3.11.8,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -72,15 +72,15 @@
 import asyncio
 
 from liminal import Client
 from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
 
 
 async def main() -> None:
-    """Create the aiohttp session and run the example."""
+    """Run!"""
     # Create an auth provider to authenticate the user:
     auth_provider = DeviceCodeFlowProvider("<TENANT_ID>", "<CLIENT_ID>")
 
     # Create the liminal SDK instance:
     liminal = Client(auth_provider, "<LIMINAL_API_SERVER_URL>")
 
 
@@ -123,15 +123,15 @@
 import asyncio
 
 from liminal import Client
 from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
 
 
 async def main() -> None:
-    """Create the aiohttp session and run the example."""
+    """Run!"""
     # Create an auth provider to authenticate the user:
     auth_provider = DeviceCodeFlowProvider("<TENANT_ID>", "<CLIENT_ID>")
 
     # Create the liminal SDK instance and authenticate it:
     liminal = Client(auth_provider, "<LIMINAL_API_SERVER_URL>")
     await liminal.authenticate_from_auth_provider()
 
@@ -149,81 +149,76 @@
 Leaving your application running, open a browser at that URL and input the code as
 instructed. Once you successfully complete authentication via Entra ID, your Liminal
 client object will automatically authenticate with your Liminal API server.
 
 # Ongoing Authentication
 
 After the initial authentication with your auth provider, the Liminal client object will
-internally store access and refresh tokens to ensure the ongoing ability to communicate
-with your Liminal API server. The client object will automatically handle using the
-stored refresh token to request new access tokens as appropriate.
-
-## Manually Interacting with the Refresh Token
-
-The Liminal client object provides a `add_refresh_token_callback` method to manually
-interact with refresh tokens as they are generated. This is useful in situations where
-you want to retrieve that token and do something else with (store it in a database, for
-example). Every time a new refresh token is generated by the client object, the
-registered callbacks will be called.
-
-Refresh token callbacks are methods that take a single `str` parameter (denoting the
-refresh token). These callbacks are not expected to return any value. Lastly, when
-calling `add_refresh_token_callback`, the returned method allows you to cancel the
+internally manage sessions to ensure the ongoing ability to communicate with your
+Liminal API server. The client object will automatically handle using the stored refresh
+token to request new access tokens as appropriate.
+
+## Manually Interacting with the Session ID
+
+The Liminal client object provides a `add_session_id_callback` method to manually
+interact with session IDs as they are generated. This is useful in situations where you
+want to retrieve that ID and do something else with (store it in a database, for
+example). Every time a new session is generated by the client object, the registered
+callbacks will be called.
+
+Session ID callbacks are methods that take a single `str` parameter (denoting the
+session ID itself). These callbacks are not expected to return any value. Lastly,
+when calling `add_session_id_callback`, the returned method allows you to cancel the
 callback at any time.
 
 ```python
 import asyncio
 
 from liminal import Client
 from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
 
 
 async def main() -> None:
-    """Create the aiohttp session and run the example."""
+    """Run!"""
     # Create an auth provider to authenticate the user:
     auth_provider = DeviceCodeFlowProvider("<TENANT_ID>", "<CLIENT_ID>")
 
     # Create the liminal SDK instance and authenticate it:
     liminal = Client(microsoft_auth_provider, "<LIMINAL_API_SERVER_URL>")
     await liminal.authenticate_from_auth_provider()
 
-    def do_something_with_refresh_token(refresh_token: str) -> None:
-        """Do something with the refresh token."""
-        pass
+    def print_session_id(session_id: str) -> None:
+        """Do something with the session ID."""
+        print(f"Session ID: {session_id}")
 
     # Register the refresh token callback:
-    remove_callback = liminal.add_refresh_token_callback(
-        do_something_with_refresh_token
-    )
+    remove_callback = liminal.add_session_id_callback(print_session_id)
 
     # Later, if you want to remove the callback:
     remove_callback()
 
 
 asyncio.run(main())
 ```
 
-## Creating a Liminal Client from a Stored Refresh Token
+## Creating a Liminal Client from a Stored Session ID
 
-Assuming you have a stored refresh token (collected from the callback process shown
-above), it is simple to create a new Limina client using that token:
+Assuming you have a stored session ID (collected from the callback process shown
+above), it is simple to create a new Liminal client using that ID:
 
 ```python
 import asyncio
 
 from liminal import Client
 
 
 async def main() -> None:
-    """Create the aiohttp session and run the example."""
-    # Retrieve your stored refresh_token:
-    refresh_token = "12345"
-
+    """Run!"""
     # Create the client:
-    liminal = await client.authenticate_from_refresh_token(refresh_token=refresh_token)
+    liminal = await client.authenticate_from_session_id(session="my-session-id")
 
 
 asyncio.run(main())
 ```
 
 # Endpoints
```


# Comparing `tmp/filesender-client-1.1.0.tar.gz` & `tmp/filesender_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filesender-client-1.1.0.tar", last modified: Tue Mar  5 00:48:04 2024, max compression
+gzip compressed data, was "filesender_client-1.2.0.tar", last modified: Fri May  3 05:29:24 2024, max compression
```

## Comparing `filesender-client-1.1.0.tar` & `filesender_client-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-03-05 00:48:04.941350 filesender-client-1.1.0/
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     3238 2023-10-09 07:15:26.000000 filesender-client-1.1.0/.gitignore
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     1529 2023-10-09 07:15:26.000000 filesender-client-1.1.0/LICENSE
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      844 2024-03-05 00:48:04.941108 filesender-client-1.1.0/PKG-INFO
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      175 2024-01-15 03:27:56.000000 filesender-client-1.1.0/README.md
-drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-03-05 00:48:04.935788 filesender-client-1.1.0/docs/
-drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-03-05 00:48:04.936525 filesender-client-1.1.0/docs/Python API/
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     1732 2024-01-15 03:27:37.000000 filesender-client-1.1.0/docs/Python API/index.md
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      735 2024-01-15 03:27:37.000000 filesender-client-1.1.0/docs/Python API/request_types.md
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      790 2024-01-15 03:27:37.000000 filesender-client-1.1.0/docs/Python API/response_types.md
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      425 2024-03-05 00:45:22.000000 filesender-client-1.1.0/docs/changelog.md
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      136 2024-01-15 03:27:37.000000 filesender-client-1.1.0/docs/index.md
-drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-03-05 00:48:04.938333 filesender-client-1.1.0/filesender/
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      162 2024-01-15 03:27:37.000000 filesender-client-1.1.0/filesender/__init__.py
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)    13859 2024-03-04 23:46:23.000000 filesender-client-1.1.0/filesender/api.py
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     4503 2024-01-15 03:27:37.000000 filesender-client-1.1.0/filesender/auth.py
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      835 2023-10-23 01:20:24.000000 filesender-client-1.1.0/filesender/config.py
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     7854 2024-03-04 23:17:55.000000 filesender-client-1.1.0/filesender/main.py
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     2214 2024-01-15 03:27:37.000000 filesender-client-1.1.0/filesender/request_types.py
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     1559 2023-10-23 01:20:24.000000 filesender-client-1.1.0/filesender/response_types.py
-drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-03-05 00:48:04.940404 filesender-client-1.1.0/filesender_client.egg-info/
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      844 2024-03-05 00:48:04.000000 filesender-client-1.1.0/filesender_client.egg-info/PKG-INFO
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      652 2024-03-05 00:48:04.000000 filesender-client-1.1.0/filesender_client.egg-info/SOURCES.txt
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)        1 2024-03-05 00:48:04.000000 filesender-client-1.1.0/filesender_client.egg-info/dependency_links.txt
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)       51 2024-03-05 00:48:04.000000 filesender-client-1.1.0/filesender_client.egg-info/entry_points.txt
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      184 2024-03-05 00:48:04.000000 filesender-client-1.1.0/filesender_client.egg-info/requires.txt
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)       11 2024-03-05 00:48:04.000000 filesender-client-1.1.0/filesender_client.egg-info/top_level.txt
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      936 2024-01-15 03:27:37.000000 filesender-client-1.1.0/mkdocs.yml
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      831 2024-03-04 23:44:09.000000 filesender-client-1.1.0/pyproject.toml
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)       38 2024-03-05 00:48:04.941388 filesender-client-1.1.0/setup.cfg
-drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-03-05 00:48:04.940012 filesender-client-1.1.0/test/
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-01-15 03:27:37.000000 filesender-client-1.1.0/test/README.md
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      819 2024-01-08 06:49:45.000000 filesender-client-1.1.0/test/conftest.py
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     1798 2024-01-15 03:27:37.000000 filesender-client-1.1.0/test/test_cli.py
--rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     4008 2024-01-15 03:27:37.000000 filesender-client-1.1.0/test/test_client.py
+drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-05-03 05:29:24.942220 filesender_client-1.2.0/
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     3238 2023-10-09 07:15:26.000000 filesender_client-1.2.0/.gitignore
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     1529 2023-10-09 07:15:26.000000 filesender_client-1.2.0/LICENSE
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      967 2024-05-03 05:29:24.941965 filesender_client-1.2.0/PKG-INFO
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      175 2024-01-15 03:27:56.000000 filesender_client-1.2.0/README.md
+drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-05-03 05:29:24.936298 filesender_client-1.2.0/docs/
+drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-05-03 05:29:24.937381 filesender_client-1.2.0/docs/Python API/
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      181 2024-04-22 07:59:43.000000 filesender_client-1.2.0/docs/Python API/benchmark.md
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     1732 2024-01-15 03:27:37.000000 filesender_client-1.2.0/docs/Python API/index.md
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      735 2024-01-15 03:27:37.000000 filesender_client-1.2.0/docs/Python API/request_types.md
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      790 2024-01-15 03:27:37.000000 filesender_client-1.2.0/docs/Python API/response_types.md
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)   122574 2024-04-22 08:24:41.000000 filesender_client-1.2.0/docs/benchmark.ipynb
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     1260 2024-04-22 07:56:59.000000 filesender_client-1.2.0/docs/changelog.md
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      136 2024-01-15 03:27:37.000000 filesender_client-1.2.0/docs/index.md
+drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-05-03 05:29:24.939151 filesender_client-1.2.0/filesender/
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      162 2024-01-15 03:27:37.000000 filesender_client-1.2.0/filesender/__init__.py
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)    15123 2024-04-22 07:51:13.000000 filesender_client-1.2.0/filesender/api.py
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     4503 2024-01-15 03:27:37.000000 filesender_client-1.2.0/filesender/auth.py
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     4181 2024-04-22 08:09:14.000000 filesender_client-1.2.0/filesender/benchmark.py
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      835 2023-10-23 01:20:24.000000 filesender_client-1.2.0/filesender/config.py
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     8933 2024-04-22 07:51:13.000000 filesender_client-1.2.0/filesender/main.py
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     2214 2024-01-15 03:27:37.000000 filesender_client-1.2.0/filesender/request_types.py
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     1559 2023-10-23 01:20:24.000000 filesender_client-1.2.0/filesender/response_types.py
+drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-05-03 05:29:24.941121 filesender_client-1.2.0/filesender_client.egg-info/
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      967 2024-05-03 05:29:24.000000 filesender_client-1.2.0/filesender_client.egg-info/PKG-INFO
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      726 2024-05-03 05:29:24.000000 filesender_client-1.2.0/filesender_client.egg-info/SOURCES.txt
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)        1 2024-05-03 05:29:24.000000 filesender_client-1.2.0/filesender_client.egg-info/dependency_links.txt
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)       51 2024-05-03 05:29:24.000000 filesender_client-1.2.0/filesender_client.egg-info/entry_points.txt
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      214 2024-05-03 05:29:24.000000 filesender_client-1.2.0/filesender_client.egg-info/requires.txt
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)       11 2024-05-03 05:29:24.000000 filesender_client-1.2.0/filesender_client.egg-info/top_level.txt
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     1163 2024-04-22 08:00:07.000000 filesender_client-1.2.0/mkdocs.yml
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      882 2024-04-22 07:51:32.000000 filesender_client-1.2.0/pyproject.toml
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)       38 2024-05-03 05:29:24.942265 filesender_client-1.2.0/setup.cfg
+drwxr-xr-x   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-05-03 05:29:24.940673 filesender_client-1.2.0/test/
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)        0 2024-01-15 03:27:37.000000 filesender_client-1.2.0/test/README.md
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)      819 2024-01-08 06:49:45.000000 filesender_client-1.2.0/test/conftest.py
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     1798 2024-01-15 03:27:37.000000 filesender_client-1.2.0/test/test_cli.py
+-rw-r--r--   0 milton.m  (3119) WEHI\allstaff (10908)     4013 2024-04-22 07:05:54.000000 filesender_client-1.2.0/test/test_client.py
```

### Comparing `filesender-client-1.1.0/.gitignore` & `filesender_client-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `filesender-client-1.1.0/LICENSE` & `filesender_client-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `filesender-client-1.1.0/PKG-INFO` & `filesender_client-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filesender-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: FileSender Python CLI and API client
 License: BSD-3-Clause
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -17,10 +17,13 @@
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest_asyncio; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-typer; extra == "dev"
+Requires-Dist: mkdocs-jupyter; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Requires-Dist: pygments; extra == "dev"
 Requires-Dist: black; extra == "dev"
+Requires-Dist: seaborn; extra == "dev"
+Requires-Dist: pandas; extra == "dev"
```

### Comparing `filesender-client-1.1.0/docs/Python API/index.md` & `filesender_client-1.2.0/docs/Python API/index.md`

 * *Files identical despite different names*

### Comparing `filesender-client-1.1.0/docs/Python API/request_types.md` & `filesender_client-1.2.0/docs/Python API/request_types.md`

 * *Files identical despite different names*

### Comparing `filesender-client-1.1.0/docs/Python API/response_types.md` & `filesender_client-1.2.0/docs/Python API/response_types.md`

 * *Files identical despite different names*

### Comparing `filesender-client-1.1.0/filesender/api.py` & `filesender_client-1.2.0/filesender/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from dataclasses import dataclass
 from typing import Any, List, Optional, Tuple, AsyncIterator
 from bs4 import BeautifulSoup
 import filesender.response_types as response
 import filesender.request_types as request
 from urllib.parse import urlparse, urlunparse, unquote
 from filesender.auth import Auth
 from pathlib import Path
 from httpx import Request, AsyncClient, HTTPStatusError, RequestError
-from asyncio import TaskGroup
+from asyncio import TaskGroup, Semaphore
 import aiofiles
 from contextlib import contextmanager
 
 def url_without_scheme(url: str) -> str:
     """
     Returns the URL in the appropriate format for the signature calculation, namely:
     • Without a scheme
@@ -42,50 +41,64 @@
         while True:
             chunk = await fp.read(chunk_size)
             if not chunk:
                 break
             yield chunk, offset
             offset += len(chunk)
 
-@dataclass
 class FileSenderClient:
     """
     A client that can be used to programmatically interact with FileSender.
     """
     #: The base url of the file sender's API. For example https://filesender.aarnet.edu.au/rest.php
     base_url: str
     #: Size of upload chunks
     chunk_size: Optional[int]
     #: Authentication provider that will be used for all privileged requests
     auth: Auth
     # Session to use for all HTTP requests
     http_client: AsyncClient
+    #: Limits concurrent reads
+    _read_sem: Semaphore
+    #: Limits concurrent requests
+    _req_sem: Semaphore
 
     def __init__(
         self,
         base_url: str,
         chunk_size: Optional[int] = None,
         auth: Auth = Auth(),
+        concurrent_reads: Optional[int] = None,
+        concurrent_requests: Optional[int] = None
     ):
         """
         Args:
             base_url: The base URL for the FileSender instance you want to interact with.
                 This should just be a host name such as `https://filesender.aarnet.edu.au`, 
                 and should *not* include `/rest.php` or any other path element.
-            chunk_size: The chunk size used for uploading, which is the amount of data that is sent to the server per request.
+            chunk_size: The chunk size (in bytes) used for uploading, which is the amount of data that is sent to the server per request.
                 By default this is the maximum chunk size allowed by the server, but you might want to adjust this to reduce memory
                 usage or because you are getting timeout errors.
             auth: The authentication method.
                 This is optional, but you almost always want to provide it.
                 Generally you will want to use [`UserAuth`][filesender.UserAuth] or [`GuestAuth`][filesender.GuestAuth].
+            concurrent_reads: The maximum number of file chunks that can be processed at a time. Reducing this number will decrease the memory
+                usage of the application. None, the default value, sets no limit.
+                See <https://wehi-researchcomputing.github.io/FileSenderCli/benchmark> for a detailed explanation of this parameter.
+            concurrent_requests: The maximum number of API requests the client can be waiting for at a time. Reducing this number will decrease the memory
+                usage of the application. None, the default value, sets no limit.
+                See <https://wehi-researchcomputing.github.io/FileSenderCli/benchmark> for a detailed explanation of this parameter.
         """
         self.base_url = base_url
         self.auth = auth
         self.http_client = AsyncClient(timeout=None)
         self.chunk_size = chunk_size
+        # If we don't want a concurrency limit, we just use an infinitely large semaphore
+        self._read_sem = Semaphore(concurrent_reads or float("inf"))
+        self._req_sem = Semaphore(concurrent_requests or float("inf"))
 
     async def prepare(self) -> None:
         """
         Checks that the chunk size is appropriate and/or sets the chunk size based on the server info.
         This should always be run before using the client.
         """
         info = await self.get_server_info()
@@ -95,17 +108,18 @@
             raise Exception(f"--chunk-size can't be greater than the server's maximum supported chunk size. For this server, the maximum is {info['upload_chunk_size']}")
 
     async def _sign_send(self, request: Request) -> Any:
         """
         Signs a request and sends it, returning the JSON result
         """
         self.auth.sign(request, self.http_client)
-        with raise_status():
-            res = await self.http_client.send(request)
-            res.raise_for_status()
+        async with self._req_sem:
+            with raise_status():
+                res = await self.http_client.send(request)
+                res.raise_for_status()
         return res.json()
 
     async def create_transfer(
         self,
         body: request.Transfer,
     ) -> response.Transfer:
         """
@@ -183,21 +197,22 @@
         """
         if self.chunk_size is None:
             raise Exception(".prepare() has not been called!")
 
         # Upload each chunk concurrently
         async with TaskGroup() as tg:
             async for chunk, offset in yield_chunks(path, self.chunk_size):
-                tg.create_task(
-                    self._upload_chunk(
-                        chunk=chunk,
-                        offset=offset,
-                        file_info=file_info
+                async with self._read_sem:
+                    tg.create_task(
+                        self._upload_chunk(
+                            chunk=chunk,
+                            offset=offset,
+                            file_info=file_info
+                        )
                     )
-                )
 
     async def _upload_chunk(
         self,
         file_info: response.File,
         offset: int,
         chunk: bytes,
     ) -> None:
```

### Comparing `filesender-client-1.1.0/filesender/auth.py` & `filesender_client-1.2.0/filesender/auth.py`

 * *Files identical despite different names*

### Comparing `filesender-client-1.1.0/filesender/config.py` & `filesender_client-1.2.0/filesender/config.py`

 * *Files identical despite different names*

### Comparing `filesender-client-1.1.0/filesender/main.py` & `filesender_client-1.2.0/filesender/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
     return wrapper
 
 
 ChunkSize = Annotated[Optional[int], Option(help="The size of each chunk to read from the input file during the upload process. Larger values will result in a faster upload but use more memory. If the value exceeds the server's maximum chunk size, this command will fail.")]
 Verbose = Annotated[bool, Option(help="Enable more detailed outputs")]
 Delay = Annotated[int, Option(help="Delay the signature timestamp by N seconds. Increase this value if you have a slow connection. This value should be approximately the time it takes you to upload one chunk to the server.", metavar="N")]
+ConcurrentReads = Annotated[Optional[int], Option(help="The maximum number of file chunks that can be processed at a time. Reducing this number will decrease the memory usage of the application. None, the default value, sets no limit. See https://wehi-researchcomputing.github.io/FileSenderCli/benchmark for a detailed explanation of this parameter.")]
+ConcurrentReqs = Annotated[Optional[int], Option(help="The maximum number of API requests the client can be waiting for at a time. Reducing this number will decrease the memory usage of the application. None, the default value, sets no limit. See https://wehi-researchcomputing.github.io/FileSenderCli/benchmark for a detailed explanation of this parameter.")]
 
 context = {
     "default_map": get_defaults()
 }
 app = Typer(name="filesender")
 
 def version_callback(value: bool):
@@ -103,25 +105,29 @@
 @app.command(context_settings=context)
 @typer_async
 async def upload_voucher(
     files: Annotated[List[Path], Argument(file_okay=True, dir_okay=False, resolve_path=True, exists=True, help="Files to upload")],
     guest_token: Annotated[str, Option(help="The guest token. This is the part of the upload URL after 'vid='")],
     email: Annotated[str, Option(help="The email address that was invited to upload files")],
     context: Context,
+    concurrent_reads: ConcurrentReads = None,
+    concurrent_reqs: ConcurrentReqs = None,
     chunk_size: ChunkSize = None,
     verbose: Verbose = False
 ):
     """
     Uploads files to a voucher that you have been invited to
     """
     auth = GuestAuth(guest_token=guest_token)
     client = FileSenderClient(
         auth=auth,
         base_url=context.obj["base_url"],
         chunk_size = chunk_size,
+        concurrent_reads=concurrent_reads,
+        concurrent_requests=concurrent_reqs
     )
     await auth.prepare(client.http_client)
     await client.prepare()
     result: Transfer = await client.upload_workflow(files, {"from": email, "recipients": []})
     if verbose:
         print(result)
     print("Upload completed successfully")
@@ -131,28 +137,32 @@
 async def upload(
     username: Annotated[str, Option(help="Username of the user performing the upload")],
     apikey: Annotated[str, Option(help="API token of the user performing the upload")],
     files: Annotated[List[Path], Argument(file_okay=True, dir_okay=False, resolve_path=True, exists=True, help="Files to upload")],
     recipients: Annotated[List[str], Option(show_default=False, help="One or more email addresses to send the files")],
     context: Context,
     verbose: Verbose = False,
+    concurrent_reads: ConcurrentReads = None,
+    concurrent_reqs: ConcurrentReqs = None,
     chunk_size: ChunkSize = None,
     delay: Delay = 0
 ):
     """
     Sends files to an email of choice
     """
     client = FileSenderClient(
         auth=UserAuth(
             api_key=apikey,
             username=username,
             delay=delay
         ),
         base_url=context.obj["base_url"],
-        chunk_size=chunk_size
+        chunk_size=chunk_size,
+        concurrent_reads=concurrent_reads,
+        concurrent_requests=concurrent_reqs
     )
     await client.prepare()
     result: Transfer = await client.upload_workflow(files, {"recipients": recipients, "from": username})
     if verbose:
         print(result)
     print("Upload completed successfully")
```

### Comparing `filesender-client-1.1.0/filesender/request_types.py` & `filesender_client-1.2.0/filesender/request_types.py`

 * *Files identical despite different names*

### Comparing `filesender-client-1.1.0/filesender/response_types.py` & `filesender_client-1.2.0/filesender/response_types.py`

 * *Files identical despite different names*

### Comparing `filesender-client-1.1.0/filesender_client.egg-info/PKG-INFO` & `filesender_client-1.2.0/filesender_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filesender-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: FileSender Python CLI and API client
 License: BSD-3-Clause
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -17,10 +17,13 @@
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest_asyncio; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-typer; extra == "dev"
+Requires-Dist: mkdocs-jupyter; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Requires-Dist: pygments; extra == "dev"
 Requires-Dist: black; extra == "dev"
+Requires-Dist: seaborn; extra == "dev"
+Requires-Dist: pandas; extra == "dev"
```

### Comparing `filesender-client-1.1.0/filesender_client.egg-info/SOURCES.txt` & `filesender_client-1.2.0/filesender_client.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 .gitignore
 LICENSE
 README.md
 mkdocs.yml
 pyproject.toml
+docs/benchmark.ipynb
 docs/changelog.md
 docs/index.md
+docs/Python API/benchmark.md
 docs/Python API/index.md
 docs/Python API/request_types.md
 docs/Python API/response_types.md
 filesender/__init__.py
 filesender/api.py
 filesender/auth.py
+filesender/benchmark.py
 filesender/config.py
 filesender/main.py
 filesender/request_types.py
 filesender/response_types.py
 filesender_client.egg-info/PKG-INFO
 filesender_client.egg-info/SOURCES.txt
 filesender_client.egg-info/dependency_links.txt
```

### Comparing `filesender-client-1.1.0/mkdocs.yml` & `filesender_client-1.2.0/mkdocs.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 site_name: "FileSenderCLI"
 
+nav:
+  - index.md
+  - Python API:
+    - Python API/index.md
+    - Python API/request_types.md
+    - Python API/response_types.md
+    - Python API/benchmark.md
+  - changelog.md
+  - 'Benchmark': benchmark.ipynb
+
 theme:
   name: "material"
 
 plugins:
 - autorefs
 - mkdocstrings:
     default_handler: python
@@ -18,14 +28,15 @@
           show_signature_annotations: true
           separate_signature: true
           signature_crossrefs: true
           merge_init_into_class: true
           docstring_options:
             ignore_init_summary: false
             trim_doctest_flags: false
+- mkdocs-jupyter
 
 markdown_extensions:
   - toc:
   - pymdownx.highlight:
       use_pygments: true
       anchor_linenums: true
       default_lang: python
```

### Comparing `filesender-client-1.1.0/pyproject.toml` & `filesender_client-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "filesender-client"
 description = "FileSender Python CLI and API client"
-version = "1.1.0"
+version = "1.2.0"
 readme = "README.rst"
 requires-python = ">=3.11"
 keywords = ["one", "two"]
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
@@ -27,14 +27,17 @@
 dev = [
     "pytest",
     "pytest_asyncio",
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings[python]",
     "mkdocs-typer",
+    "mkdocs-jupyter",
     "pymdown-extensions",
     "pygments",
-    "black"
+    "black",
+    "seaborn",
+    "pandas"
 ]
 
 [project.scripts]
 filesender = "filesender.main:app"
```

### Comparing `filesender-client-1.1.0/test/conftest.py` & `filesender_client-1.2.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `filesender-client-1.1.0/test/test_cli.py` & `filesender_client-1.2.0/test/test_cli.py`

 * *Files identical despite different names*


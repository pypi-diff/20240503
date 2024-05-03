# Comparing `tmp/aiogtrans-1.1.5.tar.gz` & `tmp/aiogtrans-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogtrans-1.1.5.tar", last modified: Fri Jun  3 23:35:39 2022, max compression
+gzip compressed data, was "aiogtrans-1.1.6.tar", last modified: Fri May  3 02:07:48 2024, max compression
```

## Comparing `aiogtrans-1.1.5.tar` & `aiogtrans-1.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-06-03 23:35:39.593016 aiogtrans-1.1.5/
--rw-rw-rw-   0        0        0     1095 2022-06-01 20:39:07.000000 aiogtrans-1.1.5/LICENSE
--rw-rw-rw-   0        0        0     8239 2022-06-03 23:35:39.593016 aiogtrans-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     7108 2022-06-02 00:06:56.000000 aiogtrans-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2022-06-03 23:35:39.565991 aiogtrans-1.1.5/aiogtrans/
--rw-rw-rw-   0        0        0     1108 2022-06-03 22:44:41.000000 aiogtrans-1.1.5/aiogtrans/__init__.py
--rw-rw-rw-   0        0        0    10063 2022-06-03 23:34:13.000000 aiogtrans-1.1.5/aiogtrans/aiohttpclient.py
--rw-rw-rw-   0        0        0     8660 2022-06-02 00:08:37.000000 aiogtrans-1.1.5/aiogtrans/constants.py
--rw-rw-rw-   0        0        0     9552 2022-06-03 22:44:41.000000 aiogtrans-1.1.5/aiogtrans/httpxclient.py
--rw-rw-rw-   0        0        0     2720 2022-06-03 22:47:07.000000 aiogtrans-1.1.5/aiogtrans/models.py
--rw-rw-rw-   0        0        0      253 2022-06-03 22:57:08.000000 aiogtrans-1.1.5/aiogtrans/urls.py
-drwxrwxrwx   0        0        0        0 2022-06-03 23:35:39.592015 aiogtrans-1.1.5/aiogtrans.egg-info/
--rw-rw-rw-   0        0        0     8239 2022-06-03 23:35:39.000000 aiogtrans-1.1.5/aiogtrans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2022-06-03 23:35:39.000000 aiogtrans-1.1.5/aiogtrans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-03 23:35:39.000000 aiogtrans-1.1.5/aiogtrans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-06-03 23:35:39.000000 aiogtrans-1.1.5/aiogtrans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-06-03 23:35:39.000000 aiogtrans-1.1.5/aiogtrans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2022-06-03 23:35:39.594016 aiogtrans-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2003 2022-06-03 23:34:34.000000 aiogtrans-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:07:48.172580 aiogtrans-1.1.6/
+-rw-rw-rw-   0        0        0     1095 2022-06-01 20:39:07.000000 aiogtrans-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0     8179 2024-05-03 02:07:48.172580 aiogtrans-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7108 2022-06-02 00:06:56.000000 aiogtrans-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 02:07:48.157798 aiogtrans-1.1.6/aiogtrans/
+-rw-rw-rw-   0        0        0     1045 2022-08-12 20:04:16.000000 aiogtrans-1.1.6/aiogtrans/__init__.py
+-rw-rw-rw-   0        0        0     2256 2024-05-03 02:04:40.000000 aiogtrans-1.1.6/aiogtrans/cache.py
+-rw-rw-rw-   0        0        0     9834 2024-05-03 02:04:45.000000 aiogtrans-1.1.6/aiogtrans/client.py
+-rw-rw-rw-   0        0        0     9270 2022-06-04 02:53:21.000000 aiogtrans-1.1.6/aiogtrans/constants.py
+-rw-rw-rw-   0        0        0     3836 2024-05-03 02:04:37.000000 aiogtrans-1.1.6/aiogtrans/models.py
+-rw-rw-rw-   0        0        0      857 2022-08-12 02:34:40.000000 aiogtrans-1.1.6/aiogtrans/urls.py
+drwxrwxrwx   0        0        0        0 2024-05-03 02:07:48.170578 aiogtrans-1.1.6/aiogtrans.egg-info/
+-rw-rw-rw-   0        0        0     8179 2024-05-03 02:07:48.000000 aiogtrans-1.1.6/aiogtrans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2024-05-03 02:07:48.000000 aiogtrans-1.1.6/aiogtrans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 02:07:48.000000 aiogtrans-1.1.6/aiogtrans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-03 02:07:48.000000 aiogtrans-1.1.6/aiogtrans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-03 02:07:48.000000 aiogtrans-1.1.6/aiogtrans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2024-05-03 02:07:48.177579 aiogtrans-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1843 2024-05-03 02:05:22.000000 aiogtrans-1.1.6/setup.py
```

### Comparing `aiogtrans-1.1.5/LICENSE` & `aiogtrans-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.5/PKG-INFO` & `aiogtrans-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: aiogtrans
-Version: 1.1.5
+Version: 1.1.6
 Summary: An async and updated version of the googletrans package.
 Home-page: https://github.com/Leg3ndary/aiogtrans
 Author: Ben Z
 Author-email: bleg3ndary@gmail.com
 License: MIT
 Keywords: google translate translator async
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: Freeware
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Education
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx<=0.23.0
+Requires-Dist: setuptools==58.1.0
 
 # aiogtrans
 
 aiogtrans is a **free** and **unlimited** python library that implements the Google Translate API asynchronously. This uses the [Google Translate Ajax API](https://translate.google.com>) and [httpx](https://www.python-httpx.org) to make api calls.
 
 Compatible with Python 3.6+.
 
@@ -196,9 +195,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
-
```

### Comparing `aiogtrans-1.1.5/README.md` & `aiogtrans-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `aiogtrans-1.1.5/aiogtrans/__init__.py` & `aiogtrans-1.1.6/aiogtrans/urls.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,20 @@
+# -*- coding: utf-8 -*-
 """
-Free Google Translate API for Python. Translates totally free of charge.
-
-Forked by _Leg3ndary after original project was abandoned.
-
-Licensed Under MIT
-------------------
+Predefined URLs used to make google translate requests.
 
 Copyright (c) 2022 Ben Z
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 """
 
-__all__ = ("HttpXTranslator", "AiohttpTranslator")
-
-# Client
-from aiogtrans.httpxclient import HttpXTranslator
-from aiogtrans.aiohttpclient import AiohttpTranslator
-
-# Constants
-from aiogtrans.constants import LANGCODES, LANGUAGES
-
-# Models for typehinting
-from aiogtrans.models import Translated, Detected
+BASE = "https://translate.google.com"
+TRANSLATE = "https://{host}/translate_a/single"
+TRANSLATE_RPC = "https://{host}/_/TranslateWebserverUi/data/batchexecute"
```

### Comparing `aiogtrans-1.1.5/aiogtrans/aiohttpclient.py` & `aiogtrans-1.1.6/aiogtrans/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,170 +1,176 @@
 # -*- coding: utf-8 -*-
 """
 A Translation module.
 
-You can translate text using aiohttp in this module.
+You can translate text using httpx in this module.
+
+Copyright (c) 2022 Ben Z
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
 """
 import asyncio
-import functools
 import json
 import random
 import typing
 
-import aiohttp
+import httpx
 
 from aiogtrans import urls
 from aiogtrans.constants import (
     DEFAULT_CLIENT_SERVICE_URLS,
     DEFAULT_FALLBACK_SERVICE_URLS,
+    DEFAULT_RAISE_EXCEPTION,
     DEFAULT_USER_AGENT,
     LANGCODES,
     LANGUAGES,
     SPECIAL_CASES,
-    DEFAULT_RAISE_EXCEPTION
 )
-from aiogtrans.models import Translated, Detected, TranslatedPart
+from aiogtrans.models import Detected, Translated, TranslatedPart
 
 EXCLUDES = ("en", "ca", "fr")
 
 RPC_ID = "MkEWBc"
 
 
-class AiohttpTranslator:
-    """Google Translate Ajax API Translator class
+class Translator:
+    """
+    Google Translate Ajax API Translator class
 
     Create an instance of this class to access the API.
-
-    :param service_urls: google translate url list. URLs will be used randomly.
-        For example ``['translate.google.com', 'translate.google.co.kr']``
-        To preferably use the non webapp api, service url should be translate.googleapis.com
-    :type service_urls: a sequence of strings
-
-    :param user_agent: the User-Agent header to send when making requests.
-    :type user_agent: :class:`str`
-
-    :param proxies: proxies configuration.
-        Dictionary mapping protocol or protocol and host to the URL of the proxy
-        For example ``{'http': 'foo.bar:3128', 'http://host.name': 'foo.bar:4012'}``
-    :type proxies: dictionary
-
-    :param timeout: Definition of timeout for httpx library.
-                    Will be used for every request.
-    :type timeout: number or a double of numbers
-
-    :param proxies: proxies configuration.
-                    Dictionary mapping protocol or protocol and host to the URL of the proxy
-                    For example ``{'http': 'foo.bar:3128', 'http://host.name': 'foo.bar:4012'}``
-
-    :param raise_exception: if `True` then raise exception if smth will go wrong
-
-    :param http2: whether to use HTTP2 (default: True)
-
-    :param use_fallback: use a fallback method
-    :type raise_exception: boolean
     """
 
     def __init__(
         self,
-        loop: asyncio.AbstractEventLoop = asyncio.get_event_loop(),
-        session: aiohttp.ClientSession = None,
+        loop: asyncio.AbstractEventLoop = asyncio.new_event_loop(),
+        _aclient: httpx.AsyncClient = None,
         service_urls: typing.Union[list, tuple] = DEFAULT_CLIENT_SERVICE_URLS,
         user_agent: str = DEFAULT_USER_AGENT,
         raise_exception: bool = DEFAULT_RAISE_EXCEPTION,
-        timeout: typing.Union[int, float] = 60.0,
+        timeout: typing.Union[int, float] = 10.0,
         use_fallback: bool = False,
     ) -> None:
-        """Initiating the client with basic params and such.
-        
-        Document the rest later"""
+        """
+        Initiating the client with the given parameters.
+
+        Loop is the asyncio event loop to use.
+        the client
+        ServiceUrls is the list of service urls to use.
+        UserAgent is the user agent to use.
+        RaiseException is whether to raise an exception when an error occurs.
+        Timeout is the timeout to use for the requests.
+        UseFallback is whether to use the fallback service urls if the main service urls fail.
+        """
 
         self.loop = loop
         self.raise_exception = raise_exception
 
         if use_fallback:
             self.service_urls = DEFAULT_FALLBACK_SERVICE_URLS
             self.client_type = "gtx"
         else:
             self.service_urls = service_urls
             self.client_type = "tw-ob"
 
-        if not session:
+        if not _aclient:
             headers = {
                 "User-Agent": user_agent,
                 "Referer": "https://translate.google.com",
             }
-        
-            if timeout:
-                timeout = aiohttp.ClientTimeout(total=timeout)
-            else:
-                timeout = aiohttp.ClientTimeout(total=60.0)
 
-            self.session = loop.run_until_complete(self._create_session(loop, headers, timeout))
-        
+            self._aclient = httpx.AsyncClient(headers=headers, timeout=timeout)
+
         else:
-            self.session = session
+            self._aclient = _aclient
 
-    async def _create_session(self, loop: asyncio.AbstractEventLoop, headers: dict, timeout: aiohttp.ClientTimeout) -> aiohttp.ClientSession:
-        """Internal method to create an aiohttp client session to use for requests
+    async def close(self) -> None:
         """
-        session = await aiohttp.ClientSession(
-            loop=loop,
-            headers=headers,
-            timeout=timeout
-        )
-        return session
+        Close the client
+        """
+        if self._aclient:
+            await self._aclient.aclose()
+
+    async def __aenter__(self) -> "Translator":
+        """
+        Enter the context
+        """
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
+        """
+        Exit the context
+        """
+        await self.close()
 
     async def _build_rpc_request(self, text: str, dest: str, src: str) -> str:
-        """Build the rpc request"""
-        trans_info = await self.loop.run_in_executor(None, functools.partial(json.dumps, obj=[[text, src, dest, True], [None]], separators=(",", ":")))
-        rpc = await self.loop.run_in_executor(None, functools.partial(json.dumps, obj=[
+        """
+        Build the rpc request
+        """
+        return json.dumps(
+            [
                 [
                     [
                         RPC_ID,
-                        trans_info,
+                        json.dumps(
+                            [[text, src, dest, True], [None]], separators=(",", ":")
+                        ),
                         None,
                         "generic",
                     ],
                 ]
             ],
-            separators=(",", ":")
-        ))
-        return rpc
+            separators=(",", ":"),
+        )
 
     def _pick_service_url(self) -> str:
-        """Pick a service url randomly"""
+        """
+        Pick a service url
+        """
         if len(self.service_urls) == 1:
             return self.service_urls[0]
         return random.choice(self.service_urls)
 
-    async def _translate(self, text: str, dest: str, src: str) -> typing.Tuple[str, aiohttp.ClientResponse]:
-        """Translate method that actually requests info"""
+    async def _translate(
+        self, text: str, dest: str, src: str
+    ) -> typing.Tuple[str, httpx.Response]:
+        """
+        Translate protected method
+        """
         url = urls.TRANSLATE_RPC.format(host=self._pick_service_url())
         data = {
             "f.req": await self._build_rpc_request(text, dest, src),
         }
         params = {
             "rpcids": RPC_ID,
             "bl": "boq_translate-webserver_20201207.13_p0",
             "soc-app": 1,
             "soc-platform": 1,
             "soc-device": 1,
             "rt": "c",
         }
-        r = await self.session.post(url, params=params, data=data)
-
-        if r.status != 200 and self.raise_Exception:
+        request = await self._aclient.post(url, params=params, data=data)
+        if request.status_code != 200 and self.raise_exception:
             raise Exception(
-                f"""Unexpected status code "{r.status}" from {self.service_urls}"""
+                f"""Unexpected status code "{request.status_code}" from {self.service_urls}"""
             )
-        text = await r.text()
-        return text, r
+        text = request.text
+        return text, request
 
     async def _parse_extra_data(self, data: list) -> dict:
-        """Parsing extra data to be returned to the user"""
+        """
+        Parsing extra data to be returned to the user
+        """
         response_parts_name_mapping = {
             0: "translation",
             1: "all-translations",
             2: "original-language",
             5: "possible-translations",
             6: "confidence",
             7: "possible-mistakes",
@@ -180,16 +186,20 @@
         for index, category in response_parts_name_mapping.items():
             extra[category] = (
                 data[index] if (index < len(data) and data[index]) else None
             )
 
         return extra
 
-    async def translate(self, text: str, dest: str = "en", src: str = "auto") -> Translated:
-        """Translate text"""
+    async def translate(
+        self, text: str, dest: str = "en", src: str = "auto"
+    ) -> Translated:
+        """
+        Translate text
+        """
         dest = dest.lower().split("_", 1)[0]
         src = src.lower().split("_", 1)[0]
 
         if src != "auto" and src not in LANGUAGES:
             if src in SPECIAL_CASES:
                 src = SPECIAL_CASES[src]
             elif src in LANGCODES:
@@ -226,16 +236,23 @@
                     elif char == "]":
                         square_bracket_counts[1] += 1
 
             resp += line
             if square_bracket_counts[0] == square_bracket_counts[1]:
                 break
 
-        data = await self.loop.run_in_executor(None, json.loads, resp)
-        parsed = await self.loop.run_in_executor(None, json.loads, data[0][2])
+        # data = await self.loop.run_in_executor(None, json.loads, resp)
+        # parsed = await self.loop.run_in_executor(None, json.loads, data[0][2])
+        try:
+            data = json.loads(resp)
+            parsed = json.loads(data[0][2])
+        except Exception as e:
+            raise Exception(
+                f"Error occurred while loading data: {e} \n Response : {response}"
+            )
 
         should_spacing = parsed[1][0][0][3]
         translated_parts = list(
             map(
                 lambda part: TranslatedPart(part[0], part[1] if len(part) >= 2 else []),
                 parsed[1][0][0][5],
             )
```

### Comparing `aiogtrans-1.1.5/aiogtrans/constants.py` & `aiogtrans-1.1.6/aiogtrans/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+"""
+Copyright (c) 2022 Ben Z
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+"""
+
 DEFAULT_USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64)"
 
 DEFAULT_CLIENT_SERVICE_URLS = ("translate.google.com",)
 
 DEFAULT_FALLBACK_SERVICE_URLS = ("translate.googleapis.com",)
 
 DEFAULT_SERVICE_URLS = (
```

### Comparing `aiogtrans-1.1.5/aiogtrans.egg-info/PKG-INFO` & `aiogtrans-1.1.6/aiogtrans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: aiogtrans
-Version: 1.1.5
+Version: 1.1.6
 Summary: An async and updated version of the googletrans package.
 Home-page: https://github.com/Leg3ndary/aiogtrans
 Author: Ben Z
 Author-email: bleg3ndary@gmail.com
 License: MIT
 Keywords: google translate translator async
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: Freeware
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Education
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx<=0.23.0
+Requires-Dist: setuptools==58.1.0
 
 # aiogtrans
 
 aiogtrans is a **free** and **unlimited** python library that implements the Google Translate API asynchronously. This uses the [Google Translate Ajax API](https://translate.google.com>) and [httpx](https://www.python-httpx.org) to make api calls.
 
 Compatible with Python 3.6+.
 
@@ -196,9 +195,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
-
```

### Comparing `aiogtrans-1.1.5/setup.py` & `aiogtrans-1.1.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import os.path
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 
 def get_file(*paths):
     path = os.path.join(*paths)
     try:
         with open(path, "rb") as f:
             return f.read().decode("utf8")
     except IOError:
         pass
 
 
 def get_version():
-    version = "1.1.5"
+    version = "1.1.6"
     return version
 
 
 def get_description():
     description = """An async and updated version of the googletrans package."""
     return description
 
 
 def get_readme():
     return get_file(os.path.dirname(__file__), "README.md")
 
 
 def get_requirements():
-    requirements = [
-        "httpx<=0.23.0",
-        "setuptools==58.1.0",
-        "aiohttp<=3.8.1"
-    ]
+    requirements = ["httpx<=0.23.0", "setuptools==58.1.0"]
     return requirements
 
 
 def install():
     setup(
         name="aiogtrans",
         version=get_version(),
@@ -54,20 +50,18 @@
             "Intended Audience :: End Users/Desktop",
             "License :: Freeware",
             "Operating System :: POSIX",
             "Operating System :: Microsoft :: Windows",
             "Operating System :: MacOS :: MacOS X",
             "Topic :: Education",
             "Programming Language :: Python",
-            "Programming Language :: Python :: 3.6",
-            "Programming Language :: Python :: 3.7",
-            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
         ],
         packages=find_packages(exclude=["docs", "tests"]),
         keywords="google translate translator async",
         install_requires=get_requirements(),
-        python_requires=">=3.6",
+        python_requires=">=3.9",
     )
 
 
 if __name__ == "__main__":
     install()
```


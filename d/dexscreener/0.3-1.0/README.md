# Comparing `tmp/dexscreener-0.3.tar.gz` & `tmp/dexscreener-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexscreener-0.3.tar", last modified: Mon Sep 18 18:10:47 2023, max compression
+gzip compressed data, was "dexscreener-1.0.tar", last modified: Fri May  3 17:23:00 2024, max compression
```

## Comparing `dexscreener-0.3.tar` & `dexscreener-1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-09-18 18:10:47.016192 dexscreener-0.3/
--rw-rw-rw-   0        0        0     1090 2023-09-18 17:20:55.000000 dexscreener-0.3/LICENSE
--rw-rw-rw-   0        0        0     1602 2023-09-18 18:10:47.015200 dexscreener-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      734 2023-09-18 17:58:56.000000 dexscreener-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-09-18 18:10:47.011757 dexscreener-0.3/dexscreener/
--rw-rw-rw-   0        0        0       70 2023-09-18 17:20:55.000000 dexscreener-0.3/dexscreener/__init__.py
--rw-rw-rw-   0        0        0     2546 2023-09-18 17:52:11.000000 dexscreener-0.3/dexscreener/client.py
--rw-rw-rw-   0        0        0      954 2023-09-18 18:08:47.000000 dexscreener-0.3/dexscreener/http_client.py
--rw-rw-rw-   0        0        0     1562 2023-09-18 17:38:22.000000 dexscreener-0.3/dexscreener/models.py
--rw-rw-rw-   0        0        0     1471 2023-09-18 18:09:45.000000 dexscreener-0.3/dexscreener/ratelimit.py
-drwxrwxrwx   0        0        0        0 2023-09-18 18:10:47.014191 dexscreener-0.3/dexscreener.egg-info/
--rw-rw-rw-   0        0        0     1602 2023-09-18 18:10:46.000000 dexscreener-0.3/dexscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-09-18 18:10:47.000000 dexscreener-0.3/dexscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-18 18:10:46.000000 dexscreener-0.3/dexscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-09-18 18:10:46.000000 dexscreener-0.3/dexscreener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-09-18 18:10:46.000000 dexscreener-0.3/dexscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-18 18:10:47.016192 dexscreener-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1115 2023-09-18 17:59:13.000000 dexscreener-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:23:00.244497 dexscreener-1.0/
+-rw-rw-rw-   0        0        0     1090 2023-09-18 17:20:55.000000 dexscreener-1.0/LICENSE
+-rw-rw-rw-   0        0        0     1596 2024-05-03 17:23:00.243981 dexscreener-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      734 2023-09-18 17:58:56.000000 dexscreener-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 17:23:00.237285 dexscreener-1.0/dexscreener/
+-rw-rw-rw-   0        0        0       70 2023-09-18 17:20:55.000000 dexscreener-1.0/dexscreener/__init__.py
+-rw-rw-rw-   0        0        0     3081 2024-05-03 17:10:57.000000 dexscreener-1.0/dexscreener/client.py
+-rw-rw-rw-   0        0        0      954 2023-09-18 18:08:47.000000 dexscreener-1.0/dexscreener/http_client.py
+-rw-rw-rw-   0        0        0     1562 2023-09-18 17:38:22.000000 dexscreener-1.0/dexscreener/models.py
+-rw-rw-rw-   0        0        0     1471 2023-09-18 18:09:45.000000 dexscreener-1.0/dexscreener/ratelimit.py
+drwxrwxrwx   0        0        0        0 2024-05-03 17:23:00.243465 dexscreener-1.0/dexscreener.egg-info/
+-rw-rw-rw-   0        0        0     1596 2024-05-03 17:23:00.000000 dexscreener-1.0/dexscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-03 17:23:00.000000 dexscreener-1.0/dexscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 17:23:00.000000 dexscreener-1.0/dexscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-03 17:23:00.000000 dexscreener-1.0/dexscreener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-03 17:23:00.000000 dexscreener-1.0/dexscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 17:23:00.244497 dexscreener-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1109 2024-05-03 17:22:50.000000 dexscreener-1.0/setup.py
```

### Comparing `dexscreener-0.3/LICENSE` & `dexscreener-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dexscreener-0.3/PKG-INFO` & `dexscreener-1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dexscreener
-Version: 0.3
+Version: 1.0
 Summary: Python wrapper for the 'dexscreener.com' API
 Home-page: https://github.com/nixonjoshua98/dexscreener
 Download-URL: https://github.com/nixonjoshua98/dexscreener/releases
 Author: Joshua Nixon
-Author-email: joshuanixonofficial@gmail.com
+Author-email: nixonjoshua98@gmail.com
 License: MIT
 Keywords: dexscreener,crypto,cryptocurrency,bitcoin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dexscreener-0.3/README.md` & `dexscreener-1.0/README.md`

 * *Files identical despite different names*

### Comparing `dexscreener-0.3/dexscreener/client.py` & `dexscreener-1.0/dexscreener/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,90 @@
 from .models import TokenPair
 from .http_client import HttpClient
-
+from typing import Optional
 
 class DexscreenerClient:
     def __init__(self):
         self._client: HttpClient = HttpClient(100, 60)
 
-    def get_token_pair(self, chain: str, address: str) -> TokenPair:
+    def get_token_pair(self, chain: str, address: str) -> Optional[TokenPair]:
         """
         Fetch a pair on the provided chain id
 
         https://api.dexscreener.io/latest/dex/pairs/bsc/0x7213a321F1855CF1779f42c0CD85d3D95291D34C
 
         :param chain: Chain id
         :param address: Token address
         :return:
             Response as TokenPair model
         """
         resp = self._client.request("GET", f"dex/pairs/{chain}/{address}")
+        if resp["pair"]:
+            return TokenPair(**resp["pair"])
+        else:
+            pass #returns None for now but owner might want to raise Error
 
-        return TokenPair(**resp["pair"])
-
-    async def get_token_pair_async(self, chain: str, address: str) -> TokenPair:
+    async def get_token_pair_async(self, chain: str, address: str) -> Optional[TokenPair]:
         """
         Async version of `get_token_pair`
         """
         resp = await self._client.request_async("GET", f"dex/pairs/{chain}/{address}")
-
-        return TokenPair(**resp["pair"])
+        if resp["pair"]:
+            return TokenPair(**resp["pair"])
+        else:
+            pass
 
     def get_token_pairs(self, address: str) -> list[TokenPair]:
         """
         Get pairs matching base token address
 
         https://api.dexscreener.io/latest/dex/tokens/0x2170Ed0880ac9A755fd29B2688956BD959F933F8
 
         :param address: Token address
         :return:
             Response as list of TokenPair model
         """
         resp = self._client.request("GET",  f"dex/tokens/{address}")
 
-        return [TokenPair(**pair) for pair in resp["pairs"]]
+        if resp["pairs"]:
+            return [TokenPair(**pair) for pair in resp["pairs"]]
+        else:
+            return []
 
     async def get_token_pairs_async(self, address: str) -> list[TokenPair]:
         """
         Async version of `get_token_pairs`
         """
         resp = await self._client.request_async("GET", f"dex/tokens/{address}")
-
-        return [TokenPair(**pair) for pair in resp["pairs"]]
+        
+        if resp["pairs"]:        
+            return [TokenPair(**pair) for pair in resp["pairs"]]
+        else:
+            return []
 
     def search_pairs(self, search_query: str) -> list[TokenPair]:
         """
         Search for pairs matching query
 
         https://api.dexscreener.io/latest/dex/tokens/0x2170Ed0880ac9A755fd29B2688956BD959F933F8
 
         :param search_query: query (e.g.: WBTC or WBTC/USDC)
         :return:
             Response as list of TokenPair model
         """
         resp = self._client.request("GET", f"dex/search/?q={search_query}")
-
-        return [TokenPair(**pair) for pair in resp["pairs"]]
+        
+        if resp["pairs"]:
+            return [TokenPair(**pair) for pair in resp["pairs"]]
+        else:
+            return []
 
     async def search_pairs_async(self, search_query: str) -> list[TokenPair]:
         """
         Async version of `search_pairs`
         """
         resp = await self._client.request_async("GET", f"dex/search/?q={search_query}")
-
-        return [TokenPair(**pair) for pair in resp["pairs"]]
+        
+        if resp["pairs"]:
+            return [TokenPair(**pair) for pair in resp["pairs"]]
+        else:
+            return []
```

### Comparing `dexscreener-0.3/dexscreener/http_client.py` & `dexscreener-1.0/dexscreener/http_client.py`

 * *Files identical despite different names*

### Comparing `dexscreener-0.3/dexscreener/models.py` & `dexscreener-1.0/dexscreener/models.py`

 * *Files identical despite different names*

### Comparing `dexscreener-0.3/dexscreener/ratelimit.py` & `dexscreener-1.0/dexscreener/ratelimit.py`

 * *Files identical despite different names*

### Comparing `dexscreener-0.3/dexscreener.egg-info/PKG-INFO` & `dexscreener-1.0/dexscreener.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dexscreener
-Version: 0.3
+Version: 1.0
 Summary: Python wrapper for the 'dexscreener.com' API
 Home-page: https://github.com/nixonjoshua98/dexscreener
 Download-URL: https://github.com/nixonjoshua98/dexscreener/releases
 Author: Joshua Nixon
-Author-email: joshuanixonofficial@gmail.com
+Author-email: nixonjoshua98@gmail.com
 License: MIT
 Keywords: dexscreener,crypto,cryptocurrency,bitcoin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dexscreener-0.3/setup.py` & `dexscreener-1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # py -m build
 # py -m twine upload dist/*
 
 
 setup(
 	name="dexscreener",
 	packages=find_packages(),
-	version="0.3",
+	version="1.0",
 	license="MIT",
 
 	description="Python wrapper for the 'dexscreener.com' API",
 	long_description=read_file("README.md"),
 	long_description_content_type="text/markdown",
 
 	author="Joshua Nixon",
-	author_email="joshuanixonofficial@gmail.com",
+	author_email="nixonjoshua98@gmail.com",
 
 	url="https://github.com/nixonjoshua98/dexscreener",
 
 	download_url="https://github.com/nixonjoshua98/dexscreener/releases",
 
 	keywords=[
 		"dexscreener",
```


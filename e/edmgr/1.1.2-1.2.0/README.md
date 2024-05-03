# Comparing `tmp/edmgr-1.1.2.tar.gz` & `tmp/edmgr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edmgr-1.1.2.tar", last modified: Thu Jun  8 15:09:34 2023, max compression
+gzip compressed data, was "edmgr-1.2.0.tar", last modified: Fri May  3 10:52:03 2024, max compression
```

## Comparing `edmgr-1.1.2.tar` & `edmgr-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 15:09:34.336925 edmgr-1.1.2/
--rw-r--r--   0 vsts      (1001) docker     (123)     1072 2023-06-08 15:09:06.000000 edmgr-1.1.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       33 2023-06-08 15:09:06.000000 edmgr-1.1.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)    11250 2023-06-08 15:09:34.332925 edmgr-1.1.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    10710 2023-06-08 15:09:06.000000 edmgr-1.1.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 15:09:34.332925 edmgr-1.1.2/edmgr/
--rw-r--r--   0 vsts      (1001) docker     (123)      102 2023-06-08 15:09:06.000000 edmgr-1.1.2/edmgr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-06-08 15:09:06.000000 edmgr-1.1.2/edmgr/__version__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7709 2023-06-08 15:09:06.000000 edmgr-1.1.2/edmgr/auth.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16559 2023-06-08 15:09:06.000000 edmgr-1.1.2/edmgr/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2994 2023-06-08 15:09:06.000000 edmgr-1.1.2/edmgr/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3322 2023-06-08 15:09:06.000000 edmgr-1.1.2/edmgr/download.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16196 2023-06-08 15:09:06.000000 edmgr-1.1.2/edmgr/edmgrcli.py
--rw-r--r--   0 vsts      (1001) docker     (123)      441 2023-06-08 15:09:06.000000 edmgr-1.1.2/edmgr/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7162 2023-06-08 15:09:06.000000 edmgr-1.1.2/edmgr/formatters.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2870 2023-06-08 15:09:06.000000 edmgr-1.1.2/edmgr/requester.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1123 2023-06-08 15:09:06.000000 edmgr-1.1.2/edmgr/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 15:09:34.332925 edmgr-1.1.2/edmgr.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)    11250 2023-06-08 15:09:34.000000 edmgr-1.1.2/edmgr.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-06-08 15:09:34.000000 edmgr-1.1.2/edmgr.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-08 15:09:34.000000 edmgr-1.1.2/edmgr.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-06-08 15:09:34.000000 edmgr-1.1.2/edmgr.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       91 2023-06-08 15:09:34.000000 edmgr-1.1.2/edmgr.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-08 15:09:34.000000 edmgr-1.1.2/edmgr.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      183 2023-06-08 15:09:06.000000 edmgr-1.1.2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-08 15:09:34.336925 edmgr-1.1.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1602 2023-06-08 15:09:06.000000 edmgr-1.1.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 15:09:34.332925 edmgr-1.1.2/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)     2051 2023-06-08 15:09:06.000000 edmgr-1.1.2/tests/test_auth.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15038 2023-06-08 15:09:06.000000 edmgr-1.1.2/tests/test_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1842 2023-06-08 15:09:06.000000 edmgr-1.1.2/tests/test_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17637 2023-06-08 15:09:06.000000 edmgr-1.1.2/tests/test_edmgrcli.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3281 2023-06-08 15:09:06.000000 edmgr-1.1.2/tests/test_requester.py
--rw-r--r--   0 vsts      (1001) docker     (123)      803 2023-06-08 15:09:06.000000 edmgr-1.1.2/tests/test_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 10:52:03.846259 edmgr-1.2.0/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1072 2024-05-03 10:51:18.000000 edmgr-1.2.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-05-03 10:51:18.000000 edmgr-1.2.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    11450 2024-05-03 10:52:03.846259 edmgr-1.2.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    10711 2024-05-03 10:51:18.000000 edmgr-1.2.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 10:52:03.842260 edmgr-1.2.0/edmgr/
+-rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-05-03 10:51:18.000000 edmgr-1.2.0/edmgr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-03 10:51:18.000000 edmgr-1.2.0/edmgr/__version__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7726 2024-05-03 10:51:18.000000 edmgr-1.2.0/edmgr/auth.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17527 2024-05-03 10:51:18.000000 edmgr-1.2.0/edmgr/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3277 2024-05-03 10:51:18.000000 edmgr-1.2.0/edmgr/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3337 2024-05-03 10:51:18.000000 edmgr-1.2.0/edmgr/download.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16766 2024-05-03 10:51:18.000000 edmgr-1.2.0/edmgr/edmgrcli.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      441 2024-05-03 10:51:18.000000 edmgr-1.2.0/edmgr/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7200 2024-05-03 10:51:18.000000 edmgr-1.2.0/edmgr/formatters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2997 2024-05-03 10:51:18.000000 edmgr-1.2.0/edmgr/requester.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1123 2024-05-03 10:51:18.000000 edmgr-1.2.0/edmgr/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 10:52:03.846259 edmgr-1.2.0/edmgr.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11450 2024-05-03 10:52:03.000000 edmgr-1.2.0/edmgr.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-03 10:52:03.000000 edmgr-1.2.0/edmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-03 10:52:03.000000 edmgr-1.2.0/edmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-03 10:52:03.000000 edmgr-1.2.0/edmgr.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       91 2024-05-03 10:52:03.000000 edmgr-1.2.0/edmgr.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-03 10:52:03.000000 edmgr-1.2.0/edmgr.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-05-03 10:51:18.000000 edmgr-1.2.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-03 10:52:03.846259 edmgr-1.2.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1605 2024-05-03 10:51:18.000000 edmgr-1.2.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 10:52:03.846259 edmgr-1.2.0/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2051 2024-05-03 10:51:18.000000 edmgr-1.2.0/tests/test_auth.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16369 2024-05-03 10:51:18.000000 edmgr-1.2.0/tests/test_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1842 2024-05-03 10:51:18.000000 edmgr-1.2.0/tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20640 2024-05-03 10:51:18.000000 edmgr-1.2.0/tests/test_edmgrcli.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3281 2024-05-03 10:51:18.000000 edmgr-1.2.0/tests/test_requester.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      803 2024-05-03 10:51:18.000000 edmgr-1.2.0/tests/test_utils.py
```

### Comparing `edmgr-1.1.2/LICENSE` & `edmgr-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edmgr-1.1.2/PKG-INFO` & `edmgr-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 Metadata-Version: 2.1
 Name: edmgr
-Version: 1.1.2
+Version: 1.2.0
 Summary: Entitlements and Download Manager
 Author: Digital Delivery
 Author-email: digital-delivery@arm.com
 Maintainer: Arm Ltd.
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click~=8.1
+Requires-Dist: cryptography>=3.4
+Requires-Dist: msal~=1.28
+Requires-Dist: pyjwt~=2.8
+Requires-Dist: requests~=2.31
+Requires-Dist: tabulate~=0.9
+Requires-Dist: tqdm~=4.66
 
 # Entitlements and Download Manager
 
 This package installs a CLI that allows users to see their entitlements,
 released products for those entitlements and to download those products.
 
 
 ## Installation
 
 ### Basic Installation
 ```bash
 $ python -m pip install edmgr
 ```
-Python 3.8+ supported. Recommended Python 3.9+.
+Python 3.10+ supported. Recommended Python 3.12.
 
 
 ### IBM Aspera FASP Downloads
 In order to enable IBM Aspera FASP protocol for downloading artifacts, IBM
 aspera-cli and its FASP protocol extension are required.
 
 Please install it by following the instructions at
```

### Comparing `edmgr-1.1.2/README.md` & `edmgr-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Installation
 
 ### Basic Installation
 ```bash
 $ python -m pip install edmgr
 ```
-Python 3.8+ supported. Recommended Python 3.9+.
+Python 3.10+ supported. Recommended Python 3.12.
 
 
 ### IBM Aspera FASP Downloads
 In order to enable IBM Aspera FASP protocol for downloading artifacts, IBM
 aspera-cli and its FASP protocol extension are required.
 
 Please install it by following the instructions at
```

### Comparing `edmgr-1.1.2/edmgr/auth.py` & `edmgr-1.2.0/edmgr/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     token: str, check_signature: bool = True, check_claims: bool = True
 ) -> dict:
     """
     Validates a JWT string by decoding its payload and checking if expired
 
     :param token: Encoded JWT in string format
     :raises EdmAuthError: if the token is invalid or expired
-    :return: A tuple with the encoded JWT in string format and a TokenMeta instance with the payload
+    :return: A tuple with:
+        the encoded JWT in string format
+        and a TokenMeta instance with the payload
     """
     options = {
         "verify_signature": check_signature,
         "verify_exp": check_claims,
         "verify_aud": False,
         "verify_iss": check_claims,
         "verify_iat": False,
```

### Comparing `edmgr-1.1.2/edmgr/client.py` & `edmgr-1.2.0/edmgr/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     if response is not None:
         try:
             response.raise_for_status()
         except requests.HTTPError as http_err:
             logger.debug(str(http_err))
             if response.status_code == 401:
                 raise EdmAuthError("Unauthorized.")
+            elif response.status_code == 404:
+                return {}
             try:
                 response_body = response.json()
             except json.JSONDecodeError as e:
                 raise EdmAPIError(f"Cannot decode response body: {e}") from e
             if response_body.get("errorName"):
                 return response_body
             raise
@@ -141,15 +143,17 @@
                 cache=self.__msal_cache,
             )
             self._set_token(access_token, check_signature=False)
         elif not allow_null:
             raise EdmTokenNotFound("Access token not found.")
 
     def logout(self):
-        """Sign out, remove accout from MSAL cache and remove access token from Client"""
+        """
+        Sign out, remove account from MSAL cache and remove access token from Client
+        """
         if self.__msal_cache is not None:
             msal_logout(self.__msal_cache)
             self.__msal_cache = TokenCache()
         self.__token = None
 
     def get_entitlements(
         self,
@@ -213,15 +217,16 @@
         self,
         entitlement_id: str,
         release_id: Optional[str] = None,
         params: Optional[dict] = None,
         **kwargs,
     ) -> list:
         """
-        Call the entitlements API with the entitlement ID to get a list of product releases
+        Call the entitlements API with the entitlement ID
+        to get a list of product releases.
 
         :param entitlement_id: Entitlement ID
         :param release_id: Release ID
         :param params: Query params
         :raises EdmAPIError: If the response body is not a valid JSON
         :raises EdmAuthError: If token is not authorized
         :raises requests.HTTPError: For any unexpected HTTP Error response
@@ -251,15 +256,16 @@
         self,
         entitlement_id: str,
         release_id: str,
         artifact_id: Optional[str] = None,
         **kwargs,
     ) -> list:
         """
-        Call the entitlements API with the entitlement ID and release ID to get a list of artifacts
+        Call the entitlements API with the entitlement ID and release ID
+        to get a list of artifacts.
 
         :param entitlement_id: entitlement ID
         :param release_id: release ID
         :raises EdmAPIError: If the response body is not a valid JSON
         :raises EdmAuthError: If token is not authorized
         :raises requests.HTTPError: For any unexpected HTTP Error response
         :return: a list of artifacts
@@ -277,93 +283,131 @@
         if data:
             if artifact_id is not None:
                 return [data]
             return data.get("artifacts", [])
         return []
 
     def get_artifact_download_url(
-        self, entitlement_id: str, release_id: str, artifact_id: str, **kwargs
+        self,
+        entitlement_id: str,
+        release_id: str,
+        artifact_id: str,
+        country_code: str = None,
+        **kwargs,
     ) -> dict:
         """
-        Call the entitlements API with the entitlement ID, release ID, and artifact_id to get an artifact's HTTP
-        download url.
+        Call the entitlements API with the entitlement ID, release ID, and artifact_id
+        to get an artifact's HTTP download url.
         Then filters based on Artifact ID
 
         :param artifact_id: artifact ID
         :param entitlement_id: entitlement ID
         :param release_id: release ID
+        :param country_code: the country code to do controlled ip downloads
         :raises EdmAPIError: If the response body is not a valid JSON
         :raises EdmAuthError: If token is not authorized
         :raises requests.HTTPError: For any unexpected HTTP Error response
         :return: None or a list of artifacts
         """
         kwargs = {**self.__kwargs, **kwargs}
         self._acquire_token(timeout=kwargs.get("timeout"))
         response: Optional[requests.Response] = self.entitlements_api.get(
-            f"{entitlement_id}/rights/download/releases/{release_id}/artifact/{artifact_id}/http",
+            endpoint="/".join(
+                [
+                    entitlement_id,
+                    "rights/download/releases",
+                    release_id,
+                    "artifact",
+                    artifact_id,
+                    "http",
+                ]
+            ),
+            headers=(
+                {"declared-country-code": country_code}
+                if country_code is not None
+                else None
+            ),
             **kwargs,
         )
         data: Optional[dict] = _handle_response(response)
         if not data:
             raise EdmAPIError(
                 "Couldn't find download URL for"
-                f" Entitlement ID: {entitlement_id}, Release ID: {release_id} and Artifact ID: {artifact_id}"
+                f" Entitlement ID: {entitlement_id},"
+                f" Release ID: {release_id} and Artifact ID: {artifact_id}"
             )
         return data
 
     def get_artifact_fasp_spec(
         self, entitlement_id: str, release_id: str, artifact_id: str, **kwargs
     ) -> dict:
         """
-        Call the entitlements API with the entitlement ID, release ID, and artifact_id to get the FASP Specs for
-        downloading an artifact using IBM Aspera FASP protocol.
+        Call the entitlements API with the entitlement ID, release ID, and artifact_id
+        to get the FASP Specs for downloading artifacts using IBM Aspera FASP protocol.
         Then filters based on Artifact ID
 
         :param artifact_id: artifact ID
         :param entitlement_id: entitlement ID
         :param release_id: release ID
         :raises EdmAPIError: If the response body is not a valid JSON
         :raises EdmAuthError: If token is not authorized
         :raises requests.HTTPError: For any unexpected HTTP Error response
         :return: None or a list of artifacts
         """
         kwargs = {**self.__kwargs, **kwargs}
         self._acquire_token(timeout=kwargs.get("timeout"))
         response: Optional[requests.Response] = self.entitlements_api.get(
-            f"{entitlement_id}/rights/download/releases/{release_id}/artifact/{artifact_id}/fasp",
+            "/".join(
+                [
+                    entitlement_id,
+                    "rights/download/releases",
+                    release_id,
+                    "artifact",
+                    artifact_id,
+                    "fasp",
+                ]
+            ),
             **kwargs,
         )
         data: Optional[dict] = _handle_response(response)
         if not data:
             raise EdmAPIError(
                 "Couldn't find FASP spec for"
-                f" Entitlement ID: {entitlement_id}, Release ID: {release_id} and Artifact ID: {artifact_id}"
+                f" Entitlement ID: {entitlement_id},"
+                f" Release ID: {release_id} and Artifact ID: {artifact_id}"
             )
         return data
 
     def get_artifact_download_http(
-        self, entitlement_id: str, release_id: str, artifact_id: str, **kwargs
+        self,
+        entitlement_id: str,
+        release_id: str,
+        artifact_id: str,
+        country_code: str = None,
+        **kwargs,
     ) -> HTTPDownload:
         """
         Call the entitlements API with the entitlement ID, release ID, and artifact_id,
         (filter results based on Artifact ID) and use the obtained download URL
         to construct a HTTPDownload stream object.
 
         :param artifact_id: artifact ID
         :param entitlement_id: entitlement ID
         :param release_id: release ID
-        :raises EdmAPIError: If the response body is invalid or the dowload URL is not found
+        :param country_code: the country code to do controlled ip downloads
+        :raises EdmAPIError: If the response is invalid or the URL is not found
         :raises EdmAuthError: If token is not authorized
         :raises requests.HTTPError: For any unexpected HTTP Error response
         :return: HTTPDownload stream object
         """
         download_response: dict = self.get_artifact_download_url(
             entitlement_id=entitlement_id,
             release_id=release_id,
             artifact_id=artifact_id,
+            country_code=country_code,
             **kwargs,
         )
         error = _handle_eula_error(download_response)
         if error:
             return HTTPDownload(error=error)
         download_url = download_response.get("downloadUrl")
         if not download_url:
@@ -396,23 +440,23 @@
         entitlement_id: str,
         release_id: str,
         artifact_id: str,
         chunk_size: int = 1024,
         **kwargs,
     ) -> int:
         """
-        Attemp to download and write an artifact based on entitlement ID, release ID, and artifact ID
-        parameters.
+        Attemp to download and write an artifact,
+        based on entitlement ID, release ID, and artifact ID parameters.
 
         :param fp: A binary file-like object
         :param artifact_id: artifact ID
         :param entitlement_id: entitlement ID
         :param release_id: release ID
-        :param chunk_size: The artifact will be downloaded and written in chunks of chunk_size
-        :raises EdmAPIError: If the response body is invalid or the dowload URL is not found
+        :param chunk_size: chunk size the artifact will be written in
+        :raises EdmAPIError: If the response is invalid or the dowload URL is not found
         :raises EdmAuthError: If token is not authorized
         :raises requests.HTTPError: For any unexpected HTTP Error response
         :raises EdmEulaError: If EULA was not signed for the artifact
         :return: The number of bytes written
         """
         download_stream: HTTPDownload = self.get_artifact_download_http(
             entitlement_id=entitlement_id,
```

### Comparing `edmgr-1.1.2/edmgr/config.py` & `edmgr-1.2.0/edmgr/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 }
 
 
 def get_log_level(log_level: str) -> int:
     try:
         return LOG_LEVELS[log_level.lower()]
     except KeyError:
-        msg = f"Invalid log level. Please use one of the following: {', '.join(LOG_LEVELS.keys())}"
+        msg = (
+            "Invalid log level."
+            f" Please use one of the following: {', '.join(LOG_LEVELS.keys())}"
+        )
         raise ValueError(msg)
 
 
 def get_log_level_from_verbose(verbosity: int) -> int:
     levels = list(LOG_LEVELS)
     try:
         level = levels[verbosity + 1]
@@ -31,19 +34,28 @@
 
 
 try:
     WORK_DIR = Path.home()
 except (KeyError, RuntimeError):
     WORK_DIR = Path(".")
 
+TOKEN_HOST_URL = "https://account.arm.com"
 
 PROD = {
     "access_token": os.getenv("EDM_ACCESS_TOKEN"),
-    "authority": "https://armb2c.b2clogin.com/armb2c.onmicrosoft.com/B2C_1A_ROPC_Auth.ropc",
-    "jwks_uri": "https://armb2c.b2clogin.com/armb2c.onmicrosoft.com/b2c_1a_hv.sign-in.1.1.0/discovery/v2.0/keys",
+    "authority": "/".join(
+        [TOKEN_HOST_URL, "armb2c.onmicrosoft.com", "B2C_1A_ROPC_Auth.ropc"]
+    ),
+    "jwks_uri": "/".join(
+        [
+            TOKEN_HOST_URL,
+            "armb2c.onmicrosoft.com",
+            "b2c_1a_hv.sign-in.1.1.0/discovery/v2.0/keys",
+        ]
+    ),
     "client_id": "bcca11a6-8f8f-42d9-aa4d-0f46815d9c75",
     "account_scopes": ["openid bcca11a6-8f8f-42d9-aa4d-0f46815d9c75 offline_access"],
     "edm_root": str(Path(os.getenv("EDM_ROOT", f"{WORK_DIR}/.edm")).expanduser()),
     "downloads": str(
         Path(os.getenv("EDM_DOWNLOADS", f"{WORK_DIR}/Artifacts")).expanduser()
     ),
     "base_url": "https://api.arm.com",
@@ -53,16 +65,24 @@
     "no_progress_bar": False,
 }
 
 
 QA = {
     **PROD,
     "base_url": "https://qas.api.arm.com",
-    "authority": "https://armb2ctest.b2clogin.com/tfp/armb2ctest.onmicrosoft.com/B2C_1A_ROPC_Auth.ropc",
-    "jwks_uri": "https://armb2ctest.b2clogin.com/armb2ctest.onmicrosoft.com/discovery/v2.0/keys?p=b2c_1a_ropc_auth.ropc",
+    "authority": "/".join(
+        [TOKEN_HOST_URL, "armb2ctest.onmicrosoft.com", "B2C_1A_ROPC_Auth.ropc"]
+    ),
+    "jwks_uri": "/".join(
+        [
+            TOKEN_HOST_URL,
+            "armb2ctest.onmicrosoft.com",
+            "discovery/v2.0/keys?p=b2c_1a_ropc_auth.ropc",
+        ]
+    ),
     "client_id": "243bffb8-b622-471b-9474-05e26dd1e51a",
     "account_scopes": ["openid 243bffb8-b622-471b-9474-05e26dd1e51a offline_access"],
 }
 
 
 SANDBOX = {
     **QA,
@@ -93,14 +113,17 @@
 
     def get(self, key, default=None):
         return self._env.get(key, default)
 
     def set_env(self, env: str):
         env = env.upper()
         if env not in ENVS:
-            msg = f"Invalid environment name. Please use one of the following: {', '.join(ENVS)}"
+            msg = (
+                "Invalid environment name."
+                f" Please use one of the following: {', '.join(ENVS)}"
+            )
             raise ValueError(msg)
         self._env = deepcopy(globals()[env])
         return self
 
 
 settings = Settings()
```

### Comparing `edmgr-1.1.2/edmgr/download.py` & `edmgr-1.2.0/edmgr/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,16 @@
                 written_bytes += data_size
     return written_bytes
 
 
 def _fasp_download(file_path: Path, fasp_spec: FASPSpec) -> None:
     if not shutil.which("ascli"):
         raise RuntimeError(
-            "aspera-cli executable not found. Please follow https://github.com/IBM/aspera-cli#installation"
+            "aspera-cli executable not found."
+            " Please follow https://github.com/IBM/aspera-cli#installation"
         )
     fasp_spec.spec["paths"][0]["destination"] = str(file_path)
     cmd = [
         "ascli",
         "server",
         "download",
         f"--url={settings['aspera_url']}",
```

### Comparing `edmgr-1.1.2/edmgr/edmgrcli.py` & `edmgr-1.2.0/edmgr/edmgrcli.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,23 @@
 
 def pagination_params(offset: Optional[int], limit: int) -> dict:
     if offset is not None:
         return {"offset": offset, "limit": limit}
     return {}
 
 
+def decode_token():
+    token = get_current_token()
+    if not token:
+        raise EdmTokenNotFound("Access token not found.")
+    payload = auth.decode_jwt_token(token, check_signature=False, check_claims=False)
+    payload["token"] = token
+    return payload
+
+
 @contextmanager
 def cached_client() -> Generator[Client, None, None]:
     """
     Load access token from disk cache if found and return a context manager
     wrapping a Client instanciated with either a JWT token or a MSAL TokenCache.
 
     JWT string cache takes precedence if found, otherwise cached MSAL TokenCache
@@ -302,25 +311,21 @@
 
 
 @login.command(
     context_settings=CONTEXT_SETTINGS,
     help="Print Access Token as JWT string with some extra information.",
 )
 def show_token():
-    token = get_current_token()
-    if not token:
-        raise EdmTokenNotFound("Access token not found.")
-    payload = auth.decode_jwt_token(token, check_signature=False, check_claims=False)
-
+    payload = decode_token()
     msg = (
         "Client token:"
-        f"\n  - Token Owner: {payload.get('given_name')} {payload.get('family_name')}"
-        f"\n  - Email: {payload.get('emails')}"
-        f"\n  - Expires: {print_local_time(payload.get('exp'))}"
-        f"\n  - Access Token: {token}"
+        f"\n - Token Owner: {payload.get('given_name')} {payload.get('family_name')}"
+        f"\n - Email: {payload.get('emails')}"
+        f"\n - Expires: {print_local_time(payload.get('exp'))}"
+        f"\n - Access Token: {payload.get('token')}"
     )
     echo_info(msg)
 
 
 @cli.command(
     context_settings=CONTEXT_SETTINGS, help="Print a list of available entitlements."
 )
@@ -346,26 +351,22 @@
         else:
             entitlements = client.get_entitlements(
                 entitlement_id=entitlement_id, params=params, **kwargs
             )
     if entitlements:
         return cli_output(format_entitlements, entitlements, **kwargs)
     if entitlement_id or product_code:
-        return echo_error(
-            "Couldn't find Entitlements with the given filters"
-        )
+        return echo_error("Couldn't find Entitlements with the given filters")
     echo_error("Couldn't find any Entitlements")
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS, help="Print single entitlement details")
-@option(
-    "-p", "--product-code", type=str, help="Filter grouped entitlements by Product Code"
-)
-@paginate_options
+@option("-p", "--product-code", type=str, help="Filter by product code")
 @common_options
+@paginate_options
 @argument("entitlement_id")
 def entitlement(entitlement_id: str, product_code: Optional[str] = None, **kwargs):
     with cached_client() as client:
         entitlements: Optional[list] = client.get_entitlements(
             entitlement_id=entitlement_id
         )
     if entitlements:
@@ -425,19 +426,18 @@
         artifacts: Optional[list] = client.get_artifacts(
             entitlement_id=entitlement_id,
             release_id=release_id,
             artifact_id=artifact_id,
         )
     if artifacts:
         return cli_output(format_artifacts, artifacts, **kwargs)
-    if artifact_id:
-        return echo_error(
-            "Couldn't find artifact with the given Entitlement ID, Release ID & Artifact ID"
-        )
-    echo_error("Couldn't find any artifacts with the given Entitlement ID & Release ID")
+    msg_not_found_art = "Couldn't find artifacts with the given Entitlement"
+    echo_error(
+        f"{msg_not_found_art}{', Release & Artifact' if artifact_id else ' & Release'}"
+    )
 
 
 @cli.command(
     context_settings=CONTEXT_SETTINGS,
     help="Download all artifacts for a particular release or only a specific one.",
 )
 @option(
@@ -481,31 +481,43 @@
         download_dir = settings["downloads"]
 
     download_path = Path(download_dir).expanduser()
     download_path.mkdir(mode=0o700, parents=True, exist_ok=True)
 
     if not artifacts:
         return echo_error(
-            f"No artifact found for Entitlement ID: {entitlement_id} and Release ID: {release_id}"
+            f"No artifact found for Entitlement: {entitlement_id} Release: {release_id}"
         )
     get_download: Callable
     if mode == "http":
         get_download = client.get_artifact_download_http
     elif mode == "fasp":
         get_download = client._get_artifact_download_fasp
 
     for artifact in artifacts:
+        is_controlled = "controlled" in artifact.get("repository", "ipw")
         file_name = artifact.get("fileName")
         art_id = artifact.get("id")
         if not file_name:
             echo_error(f"API Error: Invalid artifact fileName: {file_name}")
 
-        download = get_download(
-            entitlement_id=entitlement_id, release_id=release_id, artifact_id=art_id
-        )
+        # Controlled ip can only be downloaded via http
+        if is_controlled:
+            echo_info("Controlled IP found. Starting download via http...")
+            country_code = decode_token().get("ip_country")
+            download = client.get_artifact_download_http(
+                entitlement_id=entitlement_id,
+                release_id=release_id,
+                artifact_id=art_id,
+                country_code=country_code,
+            )
+        else:
+            download = get_download(
+                entitlement_id=entitlement_id, release_id=release_id, artifact_id=art_id
+            )
 
         while download.error.get("name") == "eula-error":
             echo_error(download.error["description"])
             echo()
             if confirm(
                 "Do you want to open the EULA link in your default Web browser?",
                 default=True,
@@ -522,15 +534,15 @@
             )
             download = get_download(
                 entitlement_id=entitlement_id, release_id=release_id, artifact_id=art_id
             )
 
         file_path = (Path(download_path) / file_name).resolve()
         echo(f"Downloading {file_path}")
-        if mode == "http":
+        if mode == "http" or is_controlled:
             write_download(file_path, download)
         elif mode == "fasp":
             _fasp_download(file_path, download)
     echo_info("All done!")
 
 
 if __name__ == "__main__":
```

### Comparing `edmgr-1.1.2/edmgr/formatters.py` & `edmgr-1.2.0/edmgr/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,22 +168,24 @@
         limit = min(int(kwargs["limit"]), limit)
     start = (page - 1) * limit
     end = min(page * limit, total_virtual_entitlements)
     if total_virtual_entitlements:
         if start < end:
             sliced_virtual_entitlements = virtual_entitlements[start:end]
             output += (
-                f"\n\nShowing from {start + 1} to {end} of {total_virtual_entitlements} "
+                "\n\n"
+                f"Showing from {start + 1} to {end} of {total_virtual_entitlements} "
                 "Entitlements found:\n\n"
             )
             output += _format_table(
                 serialize_virtual_entitlements,
                 sliced_virtual_entitlements,
                 **kwargs,
             )
         else:
             output += (
                 "\n\nEntitlements page out of range. "
                 f"Please check offset ({offset}) and/or limit ({limit}) options. "
-                f"Total number of Entitlements found is {total_virtual_entitlements}\n\n"
+                f"Total number of Entitlements found is {total_virtual_entitlements}"
+                "\n\n"
             )
     return output
```

### Comparing `edmgr-1.1.2/edmgr/requester.py` & `edmgr-1.2.0/edmgr/requester.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,18 +72,24 @@
             )
         except RequestException as e:
             logger.error(str(e))
             if kwargs.get("raise_request_exc"):
                 raise
 
     def get(
-        self, endpoint: Optional[str] = None, params: Optional[dict] = None, **kwargs
+        self,
+        endpoint: Optional[str] = None,
+        params: Optional[dict] = None,
+        headers: Optional[dict] = None,
+        **kwargs,
     ) -> Optional[Response]:
         """Shortcut for invoking send() with method GET"""
-        return self.send("GET", endpoint, params, **kwargs)
+        return self.send(
+            method="GET", endpoint=endpoint, params=params, headers=headers, **kwargs
+        )
 
     @property
     def token(self) -> Optional[str]:
         return self.__token
 
     @token.setter
     def token(self, token: str) -> None:
```

### Comparing `edmgr-1.1.2/edmgr/utils.py` & `edmgr-1.2.0/edmgr/utils.py`

 * *Files identical despite different names*

### Comparing `edmgr-1.1.2/edmgr.egg-info/PKG-INFO` & `edmgr-1.2.0/edmgr.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 Metadata-Version: 2.1
 Name: edmgr
-Version: 1.1.2
+Version: 1.2.0
 Summary: Entitlements and Download Manager
 Author: Digital Delivery
 Author-email: digital-delivery@arm.com
 Maintainer: Arm Ltd.
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click~=8.1
+Requires-Dist: cryptography>=3.4
+Requires-Dist: msal~=1.28
+Requires-Dist: pyjwt~=2.8
+Requires-Dist: requests~=2.31
+Requires-Dist: tabulate~=0.9
+Requires-Dist: tqdm~=4.66
 
 # Entitlements and Download Manager
 
 This package installs a CLI that allows users to see their entitlements,
 released products for those entitlements and to download those products.
 
 
 ## Installation
 
 ### Basic Installation
 ```bash
 $ python -m pip install edmgr
 ```
-Python 3.8+ supported. Recommended Python 3.9+.
+Python 3.10+ supported. Recommended Python 3.12.
 
 
 ### IBM Aspera FASP Downloads
 In order to enable IBM Aspera FASP protocol for downloading artifacts, IBM
 aspera-cli and its FASP protocol extension are required.
 
 Please install it by following the instructions at
```

### Comparing `edmgr-1.1.2/edmgr.egg-info/SOURCES.txt` & `edmgr-1.2.0/edmgr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edmgr-1.1.2/setup.py` & `edmgr-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,34 +18,34 @@
         "Natural Language :: English",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Environment :: Console",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Operating System :: OS Independent",
     ],
     maintainer="Arm Ltd.",
     author="Digital Delivery",
     author_email="digital-delivery@arm.com",
     packages=find_packages(where=this_dir, exclude=["tests"]),
     include_package_data=True,
-    python_requires=">=3.8",
+    python_requires=">=3.10",
     install_requires=[
         "click~=8.1",
         "cryptography>=3.4",
-        "msal~=1.18",
-        "pyjwt~=2.4",
-        "requests~=2.28",
-        "tabulate~=0.8",
-        "tqdm~=4.64",
+        "msal~=1.28",
+        "pyjwt~=2.8",
+        "requests~=2.31",
+        "tabulate~=0.9",
+        "tqdm~=4.66",
     ],
     entry_points={
         "console_scripts": [
             "edmgr=edmgr.edmgrcli:main",
         ]
     },
 )
```

### Comparing `edmgr-1.1.2/tests/test_auth.py` & `edmgr-1.2.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `edmgr-1.1.2/tests/test_client.py` & `edmgr-1.2.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,21 @@
 def test_handle_response_valid_code_invalid_body():
     data = "Invalid JSON"
     response = make_response(data, 200)
     with pytest.raises(EdmAPIError):
         _handle_response(response)
 
 
+def test_handle_response_404_code():
+    data = {"errorCode": 404, "errorDescription": "Not Found"}
+    response = make_response(data, 404)
+    handled_response = _handle_response(response)
+    assert handled_response == {}
+
+
 def test_client_init_no_msal_token(test_settings_no_token, valid_token_from_msal):
     try:
         Client(msal_cache=TokenCache())
     except Exception as e:
         assert False, f"Caught exception: {e}"
 
 
@@ -176,14 +183,20 @@
 def test_get_entitlement_raises(test_settings, api_mock_empty):
     entitlement_id = api_mock_empty["entitlement_id"]
     client = Client(check_jwt_signature=False)
     with pytest.raises(EdmAPIError):
         client.get_entitlements(entitlement_id)
 
 
+def test_get_entitlement_404(test_settings, api_mock_empty_404):
+    entitlement_id = api_mock_empty_404["entitlement_id"]
+    client = Client(check_jwt_signature=False)
+    assert client.get_entitlements(entitlement_id) == []
+
+
 def test_find_entitlements(test_settings, api_mock):
     api_data = api_mock["entitlements_by_product"]
     product_code = api_mock["product_code"]
     client = Client(check_jwt_signature=False)
     query = {"product.id": product_code}
     assert client.find_entitlements(query) == api_data["items"]
 
@@ -191,14 +204,15 @@
 def test_get_releases(test_settings, api_mock):
     api_data = api_mock["releases"]
     entitlement_id = api_mock["entitlement_id"]
     client = Client(check_jwt_signature=False)
     assert client.get_releases(entitlement_id) == api_data["items"]
 
 
+@pytest.mark.parametrize("api_mock_empty", [404, 400, 500, 600], indirect=True)
 def test_get_releases_empty(test_settings, api_mock_empty):
     entitlement_id = api_mock_empty["entitlement_id"]
     client = Client(check_jwt_signature=False)
     assert client.get_releases(entitlement_id) == []
 
 
 def test_get_release(test_settings, api_mock):
@@ -233,14 +247,21 @@
     entitlement_id = api_mock_empty["entitlement_id"]
     release_id = api_mock_empty["release_id"]
     client = Client(check_jwt_signature=False)
     with pytest.raises(EdmAPIError):
         client.get_artifacts(entitlement_id, release_id)
 
 
+def test_get_artifacts_404(test_settings, api_mock_empty_404):
+    entitlement_id = api_mock_empty_404["entitlement_id"]
+    release_id = api_mock_empty_404["release_id"]
+    client = Client(check_jwt_signature=False)
+    assert client.get_artifacts(entitlement_id, release_id) == []
+
+
 def test_get_artifact(test_settings, api_mock):
     api_data = api_mock["releases"]
     entitlement_id = api_mock["entitlement_id"]
     release_id = api_mock["release_id"]
     artifact_id = api_mock["artifact_id"]
     client = Client(check_jwt_signature=False)
     res = client.get_artifacts(entitlement_id, release_id, artifact_id)[0]
@@ -252,14 +273,23 @@
     release_id = api_mock_empty["release_id"]
     artifact_id = api_mock_empty["artifact_id"]
     client = Client(check_jwt_signature=False)
     with pytest.raises(EdmAPIError):
         client.get_artifacts(entitlement_id, release_id, artifact_id)
 
 
+def test_get_artifact_404(test_settings, api_mock_empty_404):
+    entitlement_id = api_mock_empty_404["entitlement_id"]
+    release_id = api_mock_empty_404["release_id"]
+    artifact_id = api_mock_empty_404["artifact_id"]
+    client = Client(check_jwt_signature=False)
+    assert client.get_artifacts(entitlement_id, release_id, artifact_id) == []
+
+
+@pytest.mark.parametrize("api_mock_empty", [404, 400, 500, 600], indirect=True)
 def test_get_artifact_download_url_error(test_settings, api_mock_empty):
     entitlement_id = api_mock_empty["entitlement_id"]
     release_id = api_mock_empty["release_id"]
     artifact_id = api_mock_empty["artifact_id"]
     client = Client(check_jwt_signature=False)
     with pytest.raises(EdmAPIError):
         client.get_artifact_download_url(entitlement_id, release_id, artifact_id)
@@ -271,14 +301,15 @@
     release_id = api_mock_eula_error["release_id"]
     artifact_id = api_mock_eula_error["artifact_id"]
     client = Client(check_jwt_signature=False)
     res = client.get_artifact_download_url(entitlement_id, release_id, artifact_id)
     assert res == api_data
 
 
+@pytest.mark.parametrize("api_mock_empty", [404, 400, 500, 600], indirect=True)
 def test_get_artifact_fasp_spec_error(test_settings, api_mock_empty):
     entitlement_id = api_mock_empty["entitlement_id"]
     release_id = api_mock_empty["release_id"]
     artifact_id = api_mock_empty["artifact_id"]
     client = Client(check_jwt_signature=False)
     with pytest.raises(EdmAPIError):
         client.get_artifact_download_url(entitlement_id, release_id, artifact_id)
```

### Comparing `edmgr-1.1.2/tests/test_config.py` & `edmgr-1.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edmgr-1.1.2/tests/test_edmgrcli.py` & `edmgr-1.2.0/tests/test_edmgrcli.py`

 * *Files 6% similar despite different names*

```diff
@@ -223,15 +223,17 @@
 def test_virtual_entitlement_filter_by_product_empty(
     test_settings, cached_token_from_settings, api_mock
 ):
     items = api_mock["virtual_entitlements"]["items"]
     grouped_entitlements = items[0]["virtualEntitlements"]
     virtual_entitlements_id = api_mock["virtual_entitlements_id"]
     product_code = "00000"
-    assert product_code not in list(map(lambda x: x["product"]["id"], grouped_entitlements))
+    assert product_code not in list(
+        map(lambda x: x["product"]["id"], grouped_entitlements)
+    )
     runner = CliRunner()
     result = runner.invoke(
         edmgrcli.entitlement, [virtual_entitlements_id, "-p", product_code]
     )
     assert result.exit_code == 0
     assert items[0]["id"] in result.output
     assert items[0]["product"]["id"] in result.output
@@ -244,14 +246,24 @@
 def test_entitlement_raises(test_settings, cached_token_from_settings, api_mock_empty):
     entitlement_id = api_mock_empty["entitlement_id"]
     runner = CliRunner()
     result = runner.invoke(edmgrcli.entitlements, ["-e", entitlement_id])
     assert result.exit_code == 1
 
 
+def test_entitlement_not_found(
+    test_settings, cached_token_from_settings, api_mock_empty_404
+):
+    entitlement_id = api_mock_empty_404["entitlement_id"]
+    runner = CliRunner()
+    result = runner.invoke(edmgrcli.entitlements, ["-e", entitlement_id])
+    assert result.exit_code == 0
+    assert "Couldn't find Entitlement" in result.output
+
+
 def test_releases_json(test_settings, cached_token_from_settings, api_mock):
     items = api_mock["releases"]["items"]
     entitlement_id = api_mock["entitlement_id"]
     runner = CliRunner()
     result = runner.invoke(edmgrcli.releases, ["-e", entitlement_id, "-f", "json"])
     assert result.exit_code == 0
     assert json.loads(result.output) == items
@@ -292,14 +304,28 @@
     entitlement_id = api_mock_empty["entitlement_id"]
     release_id = api_mock_empty["release_id"]
     runner = CliRunner()
     result = runner.invoke(edmgrcli.releases, ["-e", entitlement_id, "-r", release_id])
     assert result.exit_code == 1
 
 
+def test_release_not_found(
+    test_settings, cached_token_from_settings, api_mock_empty_404
+):
+    entitlement_id = api_mock_empty_404["entitlement_id"]
+    release_id = api_mock_empty_404["release_id"]
+    runner = CliRunner()
+    result = runner.invoke(edmgrcli.releases, ["-e", entitlement_id, "-r", release_id])
+    assert result.exit_code == 0
+    assert (
+        "Couldn't find Release with the given Entitlement ID & Release ID"
+        in result.output
+    )
+
+
 def test_artifacts_json(test_settings, cached_token_from_settings, api_mock):
     items = api_mock["releases"]["items"][0]["artifacts"]
     entitlement_id = api_mock["entitlement_id"]
     release_id = api_mock["release_id"]
     runner = CliRunner()
     result = runner.invoke(
         edmgrcli.artifacts, ["-e", entitlement_id, "-r", release_id, "-f", "json"]
@@ -325,14 +351,28 @@
     entitlement_id = api_mock_empty["entitlement_id"]
     release_id = api_mock_empty["release_id"]
     runner = CliRunner()
     result = runner.invoke(edmgrcli.artifacts, ["-e", entitlement_id, "-r", release_id])
     assert result.exit_code == 1
 
 
+def test_artifacts_not_found(
+    test_settings, cached_token_from_settings, api_mock_empty_404
+):
+    entitlement_id = api_mock_empty_404["entitlement_id"]
+    release_id = api_mock_empty_404["release_id"]
+    runner = CliRunner()
+    result = runner.invoke(edmgrcli.artifacts, ["-e", entitlement_id, "-r", release_id])
+    assert result.exit_code == 0
+    assert (
+        result.output
+        == "Couldn't find artifacts with the given Entitlement & Release\n"
+    )
+
+
 def test_artifact(test_settings, cached_token_from_settings, api_mock):
     items = api_mock["releases"]["items"][0]["artifacts"]
     entitlement_id = api_mock["entitlement_id"]
     release_id = api_mock["release_id"]
     artifact_id = api_mock["artifact_id"]
     runner = CliRunner()
     result = runner.invoke(
@@ -352,14 +392,31 @@
     runner = CliRunner()
     result = runner.invoke(
         edmgrcli.artifacts, ["-e", entitlement_id, "-r", release_id, "-a", artifact_id]
     )
     assert result.exit_code == 1
 
 
+def test_artifact_not_found(
+    test_settings, cached_token_from_settings, api_mock_empty_404
+):
+    entitlement_id = api_mock_empty_404["entitlement_id"]
+    release_id = api_mock_empty_404["release_id"]
+    artifact_id = api_mock_empty_404["artifact_id"]
+    runner = CliRunner()
+    result = runner.invoke(
+        edmgrcli.artifacts, ["-e", entitlement_id, "-r", release_id, "-a", artifact_id]
+    )
+    assert result.exit_code == 0
+    assert (
+        result.output
+        == "Couldn't find artifacts with the given Entitlement, Release & Artifact\n"
+    )
+
+
 def test_download_artifacts_single(
     test_settings, cached_token_from_settings, api_mock_with_download
 ):
     entitlement_id = api_mock_with_download["entitlement_id"]
     release_id = api_mock_with_download["release_id"]
     artifact_id = api_mock_with_download["artifact_id"]
     mock_file = api_mock_with_download["mock_file"]
@@ -376,14 +433,43 @@
     try:
         mock_file.assert_called_once_with(file_path, mode="wb")
         mock_file().write.assert_called_once_with(file_data)
     except AssertionError as e:
         assert False, str(e)
 
 
+def test_download_controlled_artifacts_single(
+    test_settings, cached_token_from_settings, api_mock_with_download_controlled
+):
+    mock_file = api_mock_with_download_controlled["mock_file"]
+    file_data = api_mock_with_download_controlled["file_data"]
+    file_name = api_mock_with_download_controlled["file_name"]
+    file_path = (Path(settings["downloads"]) / file_name).expanduser().resolve()
+    runner = CliRunner()
+    result = runner.invoke(
+        edmgrcli.download_artifacts,
+        [
+            "-e",
+            api_mock_with_download_controlled["entitlement_id"],
+            "-r",
+            api_mock_with_download_controlled["release_id"],
+            "-a",
+            api_mock_with_download_controlled["artifact_id"],
+        ],
+    )
+    assert result.exit_code == 0
+    assert "Controlled IP found. Starting download via http..." in result.output
+    assert f"Downloading {file_path}" in result.output
+    try:
+        mock_file.assert_called_once_with(file_path, mode="wb")
+        mock_file().write.assert_called_once_with(file_data)
+    except AssertionError as e:
+        assert False, str(e)
+
+
 def test_download_artifacts_eula_error_abort(
     test_settings, cached_token_from_settings, api_mock_eula_error
 ):
     entitlement_id = api_mock_eula_error["entitlement_id"]
     release_id = api_mock_eula_error["release_id"]
     artifact_id = api_mock_eula_error["artifact_id"]
     runner = CliRunner()
@@ -439,15 +525,15 @@
 
     runner = CliRunner()
     result = runner.invoke(
         edmgrcli.download_artifacts,
         ["-e", entitlement_id, "-r", release_id, "-a", artifact_id],
         input="y\ny\n",
     )
-    assert result.exit_code == 0
+    # assert result.exit_code == 0
     assert eula_error_message in result.output
     assert f"Downloading {file_path}" in result.output
     try:
         mock_file.assert_called_once_with(file_path, mode="wb")
         mock_file().write.assert_called_once_with(file_data)
         webbrowser_open.assert_called_once_with(agreement_url)
     except AssertionError as e:
```

### Comparing `edmgr-1.1.2/tests/test_requester.py` & `edmgr-1.2.0/tests/test_requester.py`

 * *Files identical despite different names*

### Comparing `edmgr-1.1.2/tests/test_utils.py` & `edmgr-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*


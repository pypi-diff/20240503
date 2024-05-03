# Comparing `tmp/wipac-rest-tools-1.7.3.tar.gz` & `tmp/wipac-rest-tools-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-rest-tools-1.7.3.tar", last modified: Wed May  1 17:53:10 2024, max compression
+gzip compressed data, was "wipac-rest-tools-1.7.4.tar", last modified: Fri May  3 21:43:28 2024, max compression
```

## Comparing `wipac-rest-tools-1.7.3.tar` & `wipac-rest-tools-1.7.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.442392 wipac-rest-tools-1.7.3/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6052 2024-05-01 17:53:10.442392 wipac-rest-tools-1.7.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4958 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.438392 wipac-rest-tools-1.7.3/rest_tools/
--rw-r--r--   0 root         (0) root         (0)      513 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.438392 wipac-rest-tools-1.7.3/rest_tools/client/
--rw-r--r--   0 root         (0) root         (0)      638 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15182 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2008 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/client_credentials.py
--rw-r--r--   0 root         (0) root         (0)     7641 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/device_client.py
--rw-r--r--   0 root         (0) root         (0)     3118 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/openid_client.py
--rw-r--r--   0 root         (0) root         (0)     2523 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/session.py
--rw-r--r--   0 root         (0) root         (0)     2545 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/client/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.438392 wipac-rest-tools-1.7.3/rest_tools/server/
--rw-r--r--   0 root         (0) root         (0)      843 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8514 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/arghandler.py
--rw-r--r--   0 root         (0) root         (0)    17104 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/decorators.py
--rw-r--r--   0 root         (0) root         (0)    18655 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/handler.py
--rw-r--r--   0 root         (0) root         (0)     2251 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2348 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/server/stats.py
--rw-r--r--   0 root         (0) root         (0)     1781 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.442392 wipac-rest-tools-1.7.3/rest_tools/utils/
--rw-r--r--   0 root         (0) root         (0)      252 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/utils/auth.py
--rw-r--r--   0 root         (0) root         (0)      136 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/utils/config.py
--rw-r--r--   0 root         (0) root         (0)     6123 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/utils/daemon.py
--rw-r--r--   0 root         (0) root         (0)     4832 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/rest_tools/utils/json_util.py
--rw-r--r--   0 root         (0) root         (0)     2311 2024-05-01 17:53:10.442392 wipac-rest-tools-1.7.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2024-05-01 17:53:08.000000 wipac-rest-tools-1.7.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:53:10.442392 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6052 2024-05-01 17:53:10.000000 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      842 2024-05-01 17:53:10.000000 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 17:53:10.000000 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      583 2024-05-01 17:53:10.000000 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-01 17:53:10.000000 wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6052 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4958 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.354988 wipac-rest-tools-1.7.4/rest_tools/
+-rw-r--r--   0 root         (0) root         (0)      513 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.354988 wipac-rest-tools-1.7.4/rest_tools/client/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15182 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/client_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     7641 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/device_client.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/openid_client.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/session.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/rest_tools/server/
+-rw-r--r--   0 root         (0) root         (0)      843 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8514 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/arghandler.py
+-rw-r--r--   0 root         (0) root         (0)    17104 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/decorators.py
+-rw-r--r--   0 root         (0) root         (0)    18812 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/rest_tools/utils/
+-rw-r--r--   0 root         (0) root         (0)      252 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/utils/auth.py
+-rw-r--r--   0 root         (0) root         (0)      136 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/utils/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     4832 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/utils/json_util.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6052 2024-05-03 21:43:28.000000 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      842 2024-05-03 21:43:28.000000 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 21:43:28.000000 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-03 21:43:28.000000 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-03 21:43:28.000000 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/top_level.txt
```

### Comparing `wipac-rest-tools-1.7.3/LICENSE` & `wipac-rest-tools-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/PKG-INFO` & `wipac-rest-tools-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.7.3
+Version: 1.7.4
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
```

### Comparing `wipac-rest-tools-1.7.3/README.md` & `wipac-rest-tools-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/__init__.py` & `wipac-rest-tools-1.7.4/rest_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.7.3"
+__version__ = "1.7.4"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-rest-tools-1.7.3/rest_tools/client/__init__.py` & `wipac-rest-tools-1.7.4/rest_tools/client/__init__.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/client/client.py` & `wipac-rest-tools-1.7.4/rest_tools/client/client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/client/client_credentials.py` & `wipac-rest-tools-1.7.4/rest_tools/client/client_credentials.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/client/device_client.py` & `wipac-rest-tools-1.7.4/rest_tools/client/device_client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/client/openid_client.py` & `wipac-rest-tools-1.7.4/rest_tools/client/openid_client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/client/session.py` & `wipac-rest-tools-1.7.4/rest_tools/client/session.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/client/utils.py` & `wipac-rest-tools-1.7.4/rest_tools/client/utils.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/server/__init__.py` & `wipac-rest-tools-1.7.4/rest_tools/server/__init__.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/server/arghandler.py` & `wipac-rest-tools-1.7.4/rest_tools/server/arghandler.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/server/decorators.py` & `wipac-rest-tools-1.7.4/rest_tools/server/decorators.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/server/handler.py` & `wipac-rest-tools-1.7.4/rest_tools/server/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,20 +340,23 @@
             raise RuntimeError('OpenID Connect auth not set up')
         self._OAUTH_AUTHORIZE_URL = self.auth.provider_info['authorization_endpoint']
         self._OAUTH_ACCESS_TOKEN_URL = self.auth.provider_info['token_endpoint']
         self._OAUTH_LOGOUT_URL = self.auth.provider_info['end_session_endpoint']
         self._OAUTH_USERINFO_URL = self.auth.provider_info['userinfo_endpoint']
         self.oauth_client_id = oauth_client_id
         self.oauth_client_secret = oauth_client_secret
+
+        scopes = {'openid', 'profile'}
         if oauth_client_scope:
-            self.oauth_client_scope = oauth_client_scope.split()
+            scopes.update(oauth_client_scope.split())
         else:
-            self.oauth_client_scope = ['profile', 'groups']
-            if oauth_client_secret:
-                self.oauth_client_scope.append('offline_access')
+            scopes.add('groups')
+        if oauth_client_secret:
+            scopes.add('offline_access')
+        self.oauth_client_scope = list(scopes)
 
     @classmethod
     def create_pkce_challenge(cls) -> str:
         code_verifier = secrets.token_urlsafe(64)
         code_challenge = base64.urlsafe_b64encode(hashlib.sha256(code_verifier.encode('utf-8')).digest()).decode('utf-8').split('=')[0]
         cls._pkcs_challenges[code_challenge] = code_verifier
         return code_challenge
@@ -394,14 +397,17 @@
             response = await http.fetch(
                 self._OAUTH_USERINFO_URL,
                 method='GET',
                 headers={'Authorization': f'Bearer {ret["access_token"]}'},
             )
             ret['id_token'] = tornado.escape.json_decode(response.body)
 
+        if ret.get('id_token') and isinstance(ret['id_token'], str):
+            ret['id_token'] = self.auth.validate(ret['id_token'])
+
         try:
             self.auth.validate(ret['access_token'])
         except Exception:
             if self.debug:
                 LOGGER.debug(f'bad token: {ret}')
             raise
         return ret
```

### Comparing `wipac-rest-tools-1.7.3/rest_tools/server/server.py` & `wipac-rest-tools-1.7.4/rest_tools/server/server.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/server/stats.py` & `wipac-rest-tools-1.7.4/rest_tools/server/stats.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/telemetry.py` & `wipac-rest-tools-1.7.4/rest_tools/telemetry.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/utils/auth.py` & `wipac-rest-tools-1.7.4/rest_tools/utils/auth.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/utils/daemon.py` & `wipac-rest-tools-1.7.4/rest_tools/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/rest_tools/utils/json_util.py` & `wipac-rest-tools-1.7.4/rest_tools/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/setup.cfg` & `wipac-rest-tools-1.7.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/PKG-INFO` & `wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.7.3
+Version: 1.7.4
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
```

### Comparing `wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/SOURCES.txt` & `wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.3/wipac_rest_tools.egg-info/requires.txt` & `wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/requires.txt`

 * *Files identical despite different names*


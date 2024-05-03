# Comparing `tmp/authsys-0.0.1.tar.gz` & `tmp/authsys-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authsys-0.0.1.tar", last modified: Wed Apr 24 12:09:54 2024, max compression
+gzip compressed data, was "authsys-0.0.2.tar", last modified: Fri May  3 19:15:09 2024, max compression
```

## Comparing `authsys-0.0.1.tar` & `authsys-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ex        (1001) ex        (1001)        0 2024-04-24 12:09:54.831735 authsys-0.0.1/
-drwxr-xr-x   0 ex        (1001) ex        (1001)        0 2024-04-24 12:09:54.831735 authsys-0.0.1/AuthSys.egg-info/
--rw-r--r--   0 ex        (1001) ex        (1001)     2131 2024-04-24 12:09:54.000000 authsys-0.0.1/AuthSys.egg-info/PKG-INFO
--rw-r--r--   0 ex        (1001) ex        (1001)      211 2024-04-24 12:09:54.000000 authsys-0.0.1/AuthSys.egg-info/SOURCES.txt
--rw-r--r--   0 ex        (1001) ex        (1001)        1 2024-04-24 12:09:54.000000 authsys-0.0.1/AuthSys.egg-info/dependency_links.txt
--rw-r--r--   0 ex        (1001) ex        (1001)        9 2024-04-24 12:09:54.000000 authsys-0.0.1/AuthSys.egg-info/requires.txt
--rw-r--r--   0 ex        (1001) ex        (1001)        8 2024-04-24 12:09:54.000000 authsys-0.0.1/AuthSys.egg-info/top_level.txt
--rw-r--r--   0 ex        (1001) ex        (1001)     2131 2024-04-24 12:09:54.831735 authsys-0.0.1/PKG-INFO
--rw-rw-r--   0 ex        (1001) ex        (1001)     1284 2024-04-24 14:34:56.000000 authsys-0.0.1/README.md
-drwxr-xr-x   0 ex        (1001) ex        (1001)        0 2024-04-24 12:09:54.831735 authsys-0.0.1/authsys/
--rw-rw-r--   0 ex        (1001) ex        (1001)    22876 2024-04-22 12:55:44.000000 authsys-0.0.1/authsys/AuthSys.py
--rw-rw-r--   0 ex        (1001) ex        (1001)       29 2024-04-24 14:58:42.000000 authsys-0.0.1/authsys/__init__.py
--rw-r--r--   0 ex        (1001) ex        (1001)       38 2024-04-24 12:09:54.831735 authsys-0.0.1/setup.cfg
--rw-rw-r--   0 ex        (1001) ex        (1001)     2065 2024-04-24 14:59:48.000000 authsys-0.0.1/setup.py
+drwxr-xr-x   0 ex        (1001) ex        (1001)        0 2024-05-03 19:15:09.935013 authsys-0.0.2/
+drwxr-xr-x   0 ex        (1001) ex        (1001)        0 2024-05-03 19:15:09.935013 authsys-0.0.2/AuthSys.egg-info/
+-rw-r--r--   0 ex        (1001) ex        (1001)     2131 2024-05-03 19:15:09.000000 authsys-0.0.2/AuthSys.egg-info/PKG-INFO
+-rw-r--r--   0 ex        (1001) ex        (1001)      211 2024-05-03 19:15:09.000000 authsys-0.0.2/AuthSys.egg-info/SOURCES.txt
+-rw-r--r--   0 ex        (1001) ex        (1001)        1 2024-05-03 19:15:09.000000 authsys-0.0.2/AuthSys.egg-info/dependency_links.txt
+-rw-r--r--   0 ex        (1001) ex        (1001)        9 2024-05-03 19:15:09.000000 authsys-0.0.2/AuthSys.egg-info/requires.txt
+-rw-r--r--   0 ex        (1001) ex        (1001)        8 2024-05-03 19:15:09.000000 authsys-0.0.2/AuthSys.egg-info/top_level.txt
+-rw-r--r--   0 ex        (1001) ex        (1001)     2131 2024-05-03 19:15:09.935013 authsys-0.0.2/PKG-INFO
+-rw-rw-r--   0 ex        (1001) ex        (1001)     1284 2024-04-24 14:34:56.000000 authsys-0.0.2/README.md
+drwxr-xr-x   0 ex        (1001) ex        (1001)        0 2024-05-03 19:15:09.935013 authsys-0.0.2/authsys/
+-rw-rw-r--   0 ex        (1001) ex        (1001)    24479 2024-05-03 19:12:18.000000 authsys-0.0.2/authsys/AuthSys.py
+-rw-rw-r--   0 ex        (1001) ex        (1001)       29 2024-04-24 14:58:42.000000 authsys-0.0.2/authsys/__init__.py
+-rw-r--r--   0 ex        (1001) ex        (1001)       38 2024-05-03 19:15:09.935013 authsys-0.0.2/setup.cfg
+-rw-rw-r--   0 ex        (1001) ex        (1001)     2065 2024-05-03 19:13:18.000000 authsys-0.0.2/setup.py
```

### Comparing `authsys-0.0.1/AuthSys.egg-info/PKG-INFO` & `authsys-0.0.2/AuthSys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AuthSys
-Version: 0.0.1
+Version: 0.0.2
 Summary: AuthSys is a Python library Allows you to create a membership system, so you add keys to your tools.
 Home-page: https://github.com/IceBytes/AuthSys/
 Author: Just Ice
 Author-email: MrAws.developer@gmail.com
 Project-URL: Source, https://github.com/IceBytes/AuthSys/
 Project-URL: Bug Reports, https://github.com/IceBytes/AuthSys/issues
 Project-URL: Documentation, https://github.com/IceBytes/AuthSys/
```

### Comparing `authsys-0.0.1/PKG-INFO` & `authsys-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AuthSys
-Version: 0.0.1
+Version: 0.0.2
 Summary: AuthSys is a Python library Allows you to create a membership system, so you add keys to your tools.
 Home-page: https://github.com/IceBytes/AuthSys/
 Author: Just Ice
 Author-email: MrAws.developer@gmail.com
 Project-URL: Source, https://github.com/IceBytes/AuthSys/
 Project-URL: Bug Reports, https://github.com/IceBytes/AuthSys/issues
 Project-URL: Documentation, https://github.com/IceBytes/AuthSys/
```

### Comparing `authsys-0.0.1/README.md` & `authsys-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `authsys-0.0.1/authsys/AuthSys.py` & `authsys-0.0.2/authsys/AuthSys.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import shlex
 import socket
 import struct
 import sys
 import traceback
 import warnings
 from subprocess import check_output
+from typing import Dict, Optional
 
 try:  # Python 3
     from subprocess import DEVNULL  # type: ignore
 except ImportError:  # Python 2
     DEVNULL = open(os.devnull, "wb")  # type: ignore
 
 # Configure logging
@@ -640,35 +641,89 @@
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     s.connect(("1.1.1.1", 53))
     ip = s.getsockname()[0]
     s.close()  # NOTE: sockets don't have context manager in 2.7 :(
     return ip
 
 class AuthSys():
-    def __init__(self):
-        self.main_api = "http://188.34.187.210"
-        self.mac = str(get_mac_address())
-
-    def _send_request(self, endpoint: str, params: dict) -> dict:
-        req = requests.get(f"{self.main_api}/{endpoint}", params=params).text
-        response = json.loads(req)
+    def __init__(self) -> None:
+        self.main_api: str = "http://authsys.catway.org"
+        self.mac: str = str(get_mac_address())
+
+    def _send_request(self, endpoint: str, params: Dict[str, str]) -> Dict[str, str]:
+        """
+        Send a request to the API endpoint.
+
+        Args:
+            endpoint: The API endpoint to send the request to.
+            params: A dictionary containing the request parameters.
+
+        Returns:
+            A dictionary containing the API response.
+        """
+        req: str = requests.get(f"{self.main_api}/{endpoint}", params=params, timeout=10).text
+        response: Dict[str, str] = json.loads(req)
         return response
 
-    def login(self, key: str, access_token: str) -> dict:
-        params = {"key": key, "access_token": access_token, "mac": self.mac}
+    def login(self, key: str, access_token: str) -> Dict[str, str]:
+        """
+        Log in with the provided key and access token.
+
+        Args:
+            key: The user's key.
+            access_token: The user's access token.
+
+        Returns:
+            A dictionary containing the API response.
+        """
+        params: Dict[str, str] = {"key": key, "access_token": access_token, "mac": self.mac}
         return self._send_request("login", params)
 
-    def register(self, time: str) -> dict:
-        params = {"time": time}
+    def register(self, time: str) -> Dict[str, str]:
+        """
+        Register a new user with the provided time.
+
+        Args:
+            time: The registration time.
+
+        Returns:
+            A dictionary containing the API response.
+        """
+        params: Dict[str, str] = {"time": time}
         return self._send_request("register", params)
 
-    def remove(self, key: str, secret_auth: str) -> dict:
-        params = {"key": key, "auth": secret_auth}
+    def remove(self, key: str, secret_auth: str) -> Dict[str, str]:
+        """
+        Remove a user with the provided key and secret authentication.
+
+        Args:
+            key: The user's key.
+            secret_auth: The user's secret authentication.
+
+        Returns:
+            A dictionary containing the API response.
+        """
+        params: Dict[str, str] = {"key": key, "auth": secret_auth}
         return self._send_request("delete", params)
 
-    def edit(self, key: str, auth: str, mac: str = None, time: str = None) -> dict:
-        params = {"key": key, "auth": auth}
+    def edit(self, key: str, auth: str, mac: Optional[str] = None, time: Optional[str] = None) -> Dict[str, str]:
+        """
+        Edit user information.
+
+        Args:
+            key: The user's key.
+            auth: The user's authentication.
+            mac: (Optional) The new MAC address.
+            time: (Optional) The new time.
+
+        Returns:
+            A dictionary containing the API response.
+        """
+        params: Dict[str, str] = {"key": key, "auth": auth}
         if mac:
             params["mac"] = mac
         if time:
             params["time"] = time
         return self._send_request("edit", params)
+
+auth = AuthSys()
+print(auth.register("60"))
```

### Comparing `authsys-0.0.1/setup.py` & `authsys-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = "AuthSys is a Python library Allows you to create a membership system, so you add keys to your tools."
 
 LONG_DESCRIPTION = """
 AuthSys is a Python library designed to simplify Membership processes. With AuthSys, you can easily integrate secure user authentication and registration functionalities into your Python applications.
 
 ## Key Features:
 - **Simple Integration**: Easily integrate user authentication and registration functionalities into your Python projects.
```


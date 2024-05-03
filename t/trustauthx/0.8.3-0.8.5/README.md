# Comparing `tmp/trustauthx-0.8.3.tar.gz` & `tmp/trustauthx-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustauthx-0.8.3.tar", last modified: Thu Apr 25 15:31:15 2024, max compression
+gzip compressed data, was "trustauthx-0.8.5.tar", last modified: Fri May  3 17:39:46 2024, max compression
```

## Comparing `trustauthx-0.8.3.tar` & `trustauthx-0.8.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:15.623471 trustauthx-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 15:31:06.000000 trustauthx-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-25 15:31:15.623471 trustauthx-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-25 15:31:06.000000 trustauthx-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:31:15.623471 trustauthx-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-25 15:31:06.000000 trustauthx-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:15.619471 trustauthx-0.8.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-25 15:31:06.000000 trustauthx-0.8.3/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:15.623471 trustauthx-0.8.3/trustauthx/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-25 15:31:06.000000 trustauthx-0.8.3/trustauthx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41517 2024-04-25 15:31:06.000000 trustauthx-0.8.3/trustauthx/authlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-25 15:31:06.000000 trustauthx-0.8.3/trustauthx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-25 15:31:06.000000 trustauthx-0.8.3/trustauthx/llmai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-25 15:31:06.000000 trustauthx-0.8.3/trustauthx/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:15.623471 trustauthx-0.8.3/trustauthx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:46.721183 trustauthx-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-03 17:39:37.000000 trustauthx-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-05-03 17:39:46.721183 trustauthx-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-05-03 17:39:37.000000 trustauthx-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:39:46.721183 trustauthx-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-03 17:39:37.000000 trustauthx-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:46.721183 trustauthx-0.8.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-03 17:39:37.000000 trustauthx-0.8.5/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:46.721183 trustauthx-0.8.5/trustauthx/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 17:39:37.000000 trustauthx-0.8.5/trustauthx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41883 2024-05-03 17:39:37.000000 trustauthx-0.8.5/trustauthx/authlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-03 17:39:37.000000 trustauthx-0.8.5/trustauthx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-03 17:39:37.000000 trustauthx-0.8.5/trustauthx/llmai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-03 17:39:37.000000 trustauthx-0.8.5/trustauthx/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:46.721183 trustauthx-0.8.5/trustauthx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-05-03 17:39:46.000000 trustauthx-0.8.5/trustauthx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-03 17:39:46.000000 trustauthx-0.8.5/trustauthx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:39:46.000000 trustauthx-0.8.5/trustauthx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 17:39:46.000000 trustauthx-0.8.5/trustauthx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-03 17:39:46.000000 trustauthx-0.8.5/trustauthx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 17:39:46.000000 trustauthx-0.8.5/trustauthx.egg-info/top_level.txt
```

### Comparing `trustauthx-0.8.3/LICENSE` & `trustauthx-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trustauthx-0.8.3/PKG-INFO` & `trustauthx-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.8.3
+Version: 0.8.5
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trustauthx-0.8.3/README.md` & `trustauthx-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `trustauthx-0.8.3/setup.py` & `trustauthx-0.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="trustauthx",
-    version="0.8.3",
+    version="0.8.5",
     description="Official connector SDK for TrustAuthx",
     long_description=long_description,
     long_description_content_type="text/markdown",  # This is important!
     author="moonlightnexus",
     author_email="nexus@trustauthx.com",
     url="https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git",
     license="MIT",
```

### Comparing `trustauthx-0.8.3/trustauthx/authlite.py` & `trustauthx-0.8.5/trustauthx/authlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,22 @@
     def _EDGE_Wrapper(func):
 
         @wraps(func)
         def wrapper(*args, **kwargs):
             # Call the function
             response = func(*args, **kwargs)
             # Check for "X-EDGE"
+            if response.status_code <= 350:
+                pass
+            else:
+                raise HTTPError(
+                    "Request failed with status code : {} \n this code contains a msg : {}".format(
+                        response.status_code, response.text
+                    )
+                )
             x_edge = response.headers.get("X-EDGE")
             if x_edge:
                 if int(x_edge) != _EdgeDBRoleQuery.total_roles:
                     _EdgeDBRoleQuery.reinitialize_all()  # Add data
             return response
 
         return wrapper
@@ -713,14 +721,15 @@
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
             rtn = self.jwt_decode(self._secret_key, response.json())
             sub = json.loads(rtn["sub"])
             rtn.pop("sub")
             rtn["email"] = sub["email"]
             rtn["uid"] = sub["uid"]
+            rtn["scope"] = json.loads(rtn["scope"])
             if not return_class:
                 return rtn
             else:
                 return User(**rtn)
         else:
             raise HTTPError(
                 "Request failed with status code : {} \n this code contains a msg : {}".format(
@@ -1024,15 +1033,15 @@
             "org_id": self.org_id,
             "api_key": self._api_key,
             "signed_key": self._signed_key,
         }
         rols = []
         if isinstance(rol_ids, str):
             rols.append(rol_ids)
-        elif isinstance(rol_ids, list):
+        elif isinstance(rol_ids,list):
             rols = [i for i in rol_ids]
         else:
             raise TypeError()
         data = {
             "uid": uid,
             "rol_id": [],
             "inplace": rol_ids,
@@ -1096,15 +1105,15 @@
         if isinstance(rol_ids_to_add, str):
             rols_add.append(rol_ids_to_add)
         elif isinstance(rol_ids_to_add, list):
             rols_add = [i for i in rol_ids_to_add]
         else:
             raise TypeError()
         rols_rem = []
-        if isinstance(rol_ids_to_remove, str):
+        if isinstance(rol_ids_to_remove,str):
             rols_rem.append(rol_ids_to_remove)
         elif isinstance(rol_ids_to_remove, list):
             rols_rem = [i for i in rol_ids_to_remove]
         else:
             raise TypeError()
         data = {
             "uid": uid,
```

### Comparing `trustauthx-0.8.3/trustauthx/cli.py` & `trustauthx-0.8.5/trustauthx/cli.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.8.3/trustauthx/llmai.py` & `trustauthx-0.8.5/trustauthx/llmai.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.8.3/trustauthx/scheme.py` & `trustauthx-0.8.5/trustauthx/scheme.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.8.3/trustauthx.egg-info/PKG-INFO` & `trustauthx-0.8.5/trustauthx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.8.3
+Version: 0.8.5
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```


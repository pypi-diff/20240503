# Comparing `tmp/drafter-1.1.1.tar.gz` & `tmp/drafter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drafter-1.1.1.tar", last modified: Mon Apr 29 15:35:55 2024, max compression
+gzip compressed data, was "drafter-1.1.2.tar", last modified: Fri May  3 16:16:58 2024, max compression
```

## Comparing `drafter-1.1.1.tar` & `drafter-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 15:35:55.433184 drafter-1.1.1/
--rw-rw-rw-   0        0        0     1075 2021-09-26 08:48:54.000000 drafter-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      766 2024-04-29 15:35:55.433184 drafter-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-09-04 16:32:22.000000 drafter-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 15:35:55.419187 drafter-1.1.1/drafter/
--rw-rw-rw-   0        0        0      431 2024-04-29 15:35:52.000000 drafter-1.1.1/drafter/__init__.py
--rw-rw-rw-   0        0        0    12946 2024-04-26 19:40:44.000000 drafter-1.1.1/drafter/components.py
--rw-rw-rw-   0        0        0      190 2024-04-26 19:36:49.000000 drafter-1.1.1/drafter/constants.py
--rw-rw-rw-   0        0        0     6808 2024-04-25 03:04:30.000000 drafter-1.1.1/drafter/debug.py
--rw-rw-rw-   0        0        0     1000 2024-04-28 15:20:07.000000 drafter-1.1.1/drafter/deploy.py
--rw-rw-rw-   0        0        0     7129 2024-04-28 15:34:19.000000 drafter-1.1.1/drafter/files.py
--rw-rw-rw-   0        0        0     4868 2024-04-26 19:41:14.000000 drafter-1.1.1/drafter/history.py
--rw-rw-rw-   0        0        0     1980 2024-04-28 15:16:39.000000 drafter-1.1.1/drafter/page.py
--rw-rw-rw-   0        0        0      437 2024-04-25 00:00:05.000000 drafter-1.1.1/drafter/routes.py
--rw-rw-rw-   0        0        0    18688 2024-04-28 15:50:25.000000 drafter-1.1.1/drafter/server.py
--rw-rw-rw-   0        0        0      893 2024-04-24 23:42:42.000000 drafter-1.1.1/drafter/setup.py
--rw-rw-rw-   0        0        0     3205 2024-04-24 23:45:48.000000 drafter-1.1.1/drafter/styling.py
--rw-rw-rw-   0        0        0     2508 2024-04-25 03:10:45.000000 drafter-1.1.1/drafter/testing.py
--rw-rw-rw-   0        0        0     2210 2024-04-25 03:03:35.000000 drafter-1.1.1/drafter/urls.py
-drwxrwxrwx   0        0        0        0 2024-04-29 15:35:55.432188 drafter-1.1.1/drafter.egg-info/
--rw-rw-rw-   0        0        0      766 2024-04-29 15:35:55.000000 drafter-1.1.1/drafter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2024-04-29 15:35:55.000000 drafter-1.1.1/drafter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 15:35:55.000000 drafter-1.1.1/drafter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-29 15:35:55.000000 drafter-1.1.1/drafter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 15:35:55.000000 drafter-1.1.1/drafter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2023-08-30 14:30:23.000000 drafter-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 15:35:55.433184 drafter-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1218 2024-04-29 15:35:39.000000 drafter-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:16:58.656342 drafter-1.1.2/
+-rw-rw-rw-   0        0        0     1075 2021-09-26 08:48:54.000000 drafter-1.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      766 2024-05-03 16:16:58.656342 drafter-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2023-09-04 16:32:22.000000 drafter-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 16:16:58.633833 drafter-1.1.2/drafter/
+-rw-rw-rw-   0        0        0      431 2024-05-03 16:15:26.000000 drafter-1.1.2/drafter/__init__.py
+-rw-rw-rw-   0        0        0    12946 2024-04-26 19:40:44.000000 drafter-1.1.2/drafter/components.py
+-rw-rw-rw-   0        0        0      190 2024-04-26 19:36:49.000000 drafter-1.1.2/drafter/constants.py
+-rw-rw-rw-   0        0        0     6808 2024-04-25 03:04:30.000000 drafter-1.1.2/drafter/debug.py
+-rw-rw-rw-   0        0        0     1000 2024-04-28 15:20:07.000000 drafter-1.1.2/drafter/deploy.py
+-rw-rw-rw-   0        0        0     7129 2024-04-28 15:34:19.000000 drafter-1.1.2/drafter/files.py
+-rw-rw-rw-   0        0        0     4868 2024-04-26 19:41:14.000000 drafter-1.1.2/drafter/history.py
+-rw-rw-rw-   0        0        0     1980 2024-04-28 15:16:39.000000 drafter-1.1.2/drafter/page.py
+-rw-rw-rw-   0        0        0      437 2024-04-25 00:00:05.000000 drafter-1.1.2/drafter/routes.py
+-rw-rw-rw-   0        0        0    18995 2024-05-03 16:15:17.000000 drafter-1.1.2/drafter/server.py
+-rw-rw-rw-   0        0        0      893 2024-04-24 23:42:42.000000 drafter-1.1.2/drafter/setup.py
+-rw-rw-rw-   0        0        0     3205 2024-04-24 23:45:48.000000 drafter-1.1.2/drafter/styling.py
+-rw-rw-rw-   0        0        0     2508 2024-04-25 03:10:45.000000 drafter-1.1.2/drafter/testing.py
+-rw-rw-rw-   0        0        0     2210 2024-04-25 03:03:35.000000 drafter-1.1.2/drafter/urls.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:16:58.655450 drafter-1.1.2/drafter.egg-info/
+-rw-rw-rw-   0        0        0      766 2024-05-03 16:16:58.000000 drafter-1.1.2/drafter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-05-03 16:16:58.000000 drafter-1.1.2/drafter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 16:16:58.000000 drafter-1.1.2/drafter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 16:16:58.000000 drafter-1.1.2/drafter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-03 16:16:58.000000 drafter-1.1.2/drafter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2023-08-30 14:30:23.000000 drafter-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 16:16:58.656342 drafter-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2024-04-29 15:35:39.000000 drafter-1.1.2/setup.py
```

### Comparing `drafter-1.1.1/LICENSE.txt` & `drafter-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drafter-1.1.1/PKG-INFO` & `drafter-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafter
-Version: 1.1.1
+Version: 1.1.2
 Summary: Student-friendly full stack web development library.
 Home-page: https://github.com/drafter-edu/drafter
 Author: acbart
 Author-email: acbart@udel.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Education
```

### Comparing `drafter-1.1.1/drafter/components.py` & `drafter-1.1.2/drafter/components.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.1/drafter/debug.py` & `drafter-1.1.2/drafter/debug.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.1/drafter/deploy.py` & `drafter-1.1.2/drafter/deploy.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.1/drafter/files.py` & `drafter-1.1.2/drafter/files.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.1/drafter/history.py` & `drafter-1.1.2/drafter/history.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.1/drafter/page.py` & `drafter-1.1.2/drafter/page.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.1/drafter/server.py` & `drafter-1.1.2/drafter/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from drafter.setup import DEFAULT_BACKEND, Bottle, abort, request, static_file
 from drafter.history import VisitedPage, rehydrate_json, dehydrate_json, ConversionRecord, UnchangedRecord, get_params, \
     remap_hidden_form_parameters
 from drafter.page import Page
 from drafter.files import TEMPLATE_200, TEMPLATE_404, TEMPLATE_500, INCLUDE_STYLES, TEMPLATE_200_WITHOUT_HEADER
 from drafter.urls import remove_url_query_params
 
+import logging
+logger = logging.getLogger('drafter')
 
 """
 Images folder
     Specific folder
     Any adjacent file
 Current page title
 CSS style (skeleton, bootstrap, etc.)
@@ -41,14 +43,16 @@
     # Launch parameters
     host: str = "localhost"
     port: int = 8080
     debug: bool = True
     # "none", "flask", etc.
     backend: str = DEFAULT_BACKEND
     reloader: bool = False
+    # This makes the server not run (e.g., to only run tests)
+    skip: bool = os.environ.get('DRAFTER_SKIP', False)
 
     # Website configuration
     title: str = "Drafter Website"
     framed: bool = True
     skulpt: bool = os.environ.get('DRAFTER_SKULPT', True)
 
     # Page configuration
@@ -373,10 +377,13 @@
         content = DebugInformation(self._page_history, self._state, self.routes, self._conversion_record)
         return content.generate()
 
 
 MAIN_SERVER = Server()
 
 
-def start_server(initial_state=None, server: Server = MAIN_SERVER, **kwargs):
+def start_server(initial_state=None, server: Server = MAIN_SERVER, skip=False, **kwargs):
+    if server.configuration.skip or skip:
+        logger.info("Skipping server setup and execution")
+        return
     server.setup(initial_state)
-    server.run(**kwargs)
+    server.run(**kwargs)
```

### Comparing `drafter-1.1.1/drafter/setup.py` & `drafter-1.1.2/drafter/setup.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.1/drafter/styling.py` & `drafter-1.1.2/drafter/styling.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.1/drafter/testing.py` & `drafter-1.1.2/drafter/testing.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.1/drafter/urls.py` & `drafter-1.1.2/drafter/urls.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.1/drafter.egg-info/PKG-INFO` & `drafter-1.1.2/drafter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafter
-Version: 1.1.1
+Version: 1.1.2
 Summary: Student-friendly full stack web development library.
 Home-page: https://github.com/drafter-edu/drafter
 Author: acbart
 Author-email: acbart@udel.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Education
```

### Comparing `drafter-1.1.1/setup.py` & `drafter-1.1.2/setup.py`

 * *Files identical despite different names*


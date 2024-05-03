# Comparing `tmp/drafter-1.1.2.tar.gz` & `tmp/drafter-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drafter-1.1.2.tar", last modified: Fri May  3 16:16:58 2024, max compression
+gzip compressed data, was "drafter-1.1.3.tar", last modified: Fri May  3 16:30:31 2024, max compression
```

## Comparing `drafter-1.1.2.tar` & `drafter-1.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 16:16:58.656342 drafter-1.1.2/
--rw-rw-rw-   0        0        0     1075 2021-09-26 08:48:54.000000 drafter-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      766 2024-05-03 16:16:58.656342 drafter-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-09-04 16:32:22.000000 drafter-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 16:16:58.633833 drafter-1.1.2/drafter/
--rw-rw-rw-   0        0        0      431 2024-05-03 16:15:26.000000 drafter-1.1.2/drafter/__init__.py
--rw-rw-rw-   0        0        0    12946 2024-04-26 19:40:44.000000 drafter-1.1.2/drafter/components.py
--rw-rw-rw-   0        0        0      190 2024-04-26 19:36:49.000000 drafter-1.1.2/drafter/constants.py
--rw-rw-rw-   0        0        0     6808 2024-04-25 03:04:30.000000 drafter-1.1.2/drafter/debug.py
--rw-rw-rw-   0        0        0     1000 2024-04-28 15:20:07.000000 drafter-1.1.2/drafter/deploy.py
--rw-rw-rw-   0        0        0     7129 2024-04-28 15:34:19.000000 drafter-1.1.2/drafter/files.py
--rw-rw-rw-   0        0        0     4868 2024-04-26 19:41:14.000000 drafter-1.1.2/drafter/history.py
--rw-rw-rw-   0        0        0     1980 2024-04-28 15:16:39.000000 drafter-1.1.2/drafter/page.py
--rw-rw-rw-   0        0        0      437 2024-04-25 00:00:05.000000 drafter-1.1.2/drafter/routes.py
--rw-rw-rw-   0        0        0    18995 2024-05-03 16:15:17.000000 drafter-1.1.2/drafter/server.py
--rw-rw-rw-   0        0        0      893 2024-04-24 23:42:42.000000 drafter-1.1.2/drafter/setup.py
--rw-rw-rw-   0        0        0     3205 2024-04-24 23:45:48.000000 drafter-1.1.2/drafter/styling.py
--rw-rw-rw-   0        0        0     2508 2024-04-25 03:10:45.000000 drafter-1.1.2/drafter/testing.py
--rw-rw-rw-   0        0        0     2210 2024-04-25 03:03:35.000000 drafter-1.1.2/drafter/urls.py
-drwxrwxrwx   0        0        0        0 2024-05-03 16:16:58.655450 drafter-1.1.2/drafter.egg-info/
--rw-rw-rw-   0        0        0      766 2024-05-03 16:16:58.000000 drafter-1.1.2/drafter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2024-05-03 16:16:58.000000 drafter-1.1.2/drafter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 16:16:58.000000 drafter-1.1.2/drafter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 16:16:58.000000 drafter-1.1.2/drafter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-03 16:16:58.000000 drafter-1.1.2/drafter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2023-08-30 14:30:23.000000 drafter-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 16:16:58.656342 drafter-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1218 2024-04-29 15:35:39.000000 drafter-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:30:31.825971 drafter-1.1.3/
+-rw-rw-rw-   0        0        0     1075 2021-09-26 08:48:54.000000 drafter-1.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      766 2024-05-03 16:30:31.824972 drafter-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2023-09-04 16:32:22.000000 drafter-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 16:30:31.811373 drafter-1.1.3/drafter/
+-rw-rw-rw-   0        0        0      431 2024-05-03 16:30:21.000000 drafter-1.1.3/drafter/__init__.py
+-rw-rw-rw-   0        0        0    12946 2024-04-26 19:40:44.000000 drafter-1.1.3/drafter/components.py
+-rw-rw-rw-   0        0        0      190 2024-04-26 19:36:49.000000 drafter-1.1.3/drafter/constants.py
+-rw-rw-rw-   0        0        0     6808 2024-04-25 03:04:30.000000 drafter-1.1.3/drafter/debug.py
+-rw-rw-rw-   0        0        0     1000 2024-04-28 15:20:07.000000 drafter-1.1.3/drafter/deploy.py
+-rw-rw-rw-   0        0        0     7129 2024-04-28 15:34:19.000000 drafter-1.1.3/drafter/files.py
+-rw-rw-rw-   0        0        0     4868 2024-04-26 19:41:14.000000 drafter-1.1.3/drafter/history.py
+-rw-rw-rw-   0        0        0     1980 2024-04-28 15:16:39.000000 drafter-1.1.3/drafter/page.py
+-rw-rw-rw-   0        0        0      437 2024-04-25 00:00:05.000000 drafter-1.1.3/drafter/routes.py
+-rw-rw-rw-   0        0        0    18995 2024-05-03 16:15:17.000000 drafter-1.1.3/drafter/server.py
+-rw-rw-rw-   0        0        0      893 2024-04-24 23:42:42.000000 drafter-1.1.3/drafter/setup.py
+-rw-rw-rw-   0        0        0     3205 2024-04-24 23:45:48.000000 drafter-1.1.3/drafter/styling.py
+-rw-rw-rw-   0        0        0     2509 2024-05-03 16:29:03.000000 drafter-1.1.3/drafter/testing.py
+-rw-rw-rw-   0        0        0     2210 2024-04-25 03:03:35.000000 drafter-1.1.3/drafter/urls.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:30:31.824972 drafter-1.1.3/drafter.egg-info/
+-rw-rw-rw-   0        0        0      766 2024-05-03 16:30:31.000000 drafter-1.1.3/drafter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-05-03 16:30:31.000000 drafter-1.1.3/drafter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 16:30:31.000000 drafter-1.1.3/drafter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 16:30:31.000000 drafter-1.1.3/drafter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-03 16:30:31.000000 drafter-1.1.3/drafter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2023-08-30 14:30:23.000000 drafter-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 16:30:31.825971 drafter-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2024-04-29 15:35:39.000000 drafter-1.1.3/setup.py
```

### Comparing `drafter-1.1.2/LICENSE.txt` & `drafter-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drafter-1.1.2/PKG-INFO` & `drafter-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafter
-Version: 1.1.2
+Version: 1.1.3
 Summary: Student-friendly full stack web development library.
 Home-page: https://github.com/drafter-edu/drafter
 Author: acbart
 Author-email: acbart@udel.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Education
```

### Comparing `drafter-1.1.2/drafter/components.py` & `drafter-1.1.3/drafter/components.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.2/drafter/debug.py` & `drafter-1.1.3/drafter/debug.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.2/drafter/deploy.py` & `drafter-1.1.3/drafter/deploy.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.2/drafter/files.py` & `drafter-1.1.3/drafter/files.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.2/drafter/history.py` & `drafter-1.1.3/drafter/history.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.2/drafter/page.py` & `drafter-1.1.3/drafter/page.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.2/drafter/server.py` & `drafter-1.1.3/drafter/server.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.2/drafter/setup.py` & `drafter-1.1.3/drafter/setup.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.2/drafter/styling.py` & `drafter-1.1.3/drafter/styling.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.2/drafter/testing.py` & `drafter-1.1.3/drafter/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     args: tuple
     kwargs: dict
     result: Any
     line: int
     caller: str
 
 
-DEFAULT_STACK_DEPTH = 8
+DEFAULT_STACK_DEPTH = 10
 def get_line_code(depth = DEFAULT_STACK_DEPTH):
     # Load in extract_stack, or provide shim for environments without it.
     try:
         from traceback import extract_stack
         trace = extract_stack()
         frame = trace[len(trace) - depth]
         line = frame[1]
```

### Comparing `drafter-1.1.2/drafter/urls.py` & `drafter-1.1.3/drafter/urls.py`

 * *Files identical despite different names*

### Comparing `drafter-1.1.2/drafter.egg-info/PKG-INFO` & `drafter-1.1.3/drafter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafter
-Version: 1.1.2
+Version: 1.1.3
 Summary: Student-friendly full stack web development library.
 Home-page: https://github.com/drafter-edu/drafter
 Author: acbart
 Author-email: acbart@udel.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Education
```

### Comparing `drafter-1.1.2/setup.py` & `drafter-1.1.3/setup.py`

 * *Files identical despite different names*


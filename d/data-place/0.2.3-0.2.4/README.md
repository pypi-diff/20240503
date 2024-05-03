# Comparing `tmp/data-place-0.2.3.tar.gz` & `tmp/data-place-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-place-0.2.3.tar", last modified: Thu May  2 20:35:33 2024, max compression
+gzip compressed data, was "data-place-0.2.4.tar", last modified: Thu May  2 20:39:49 2024, max compression
```

## Comparing `data-place-0.2.3.tar` & `data-place-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 20:35:33.461681 data-place-0.2.3/
--rw-rw-rw-   0        0        0       44 2024-05-02 20:35:33.000000 data-place-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6073 2024-05-02 20:35:33.460676 data-place-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.2.3/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.2.3/build.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:35:33.459474 data-place-0.2.3/data_place.egg-info/
--rw-rw-rw-   0        0        0     6073 2024-05-02 20:35:33.000000 data-place-0.2.3/data_place.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2024-05-02 20:35:33.000000 data-place-0.2.3/data_place.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 20:35:33.000000 data-place-0.2.3/data_place.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-02 20:35:33.000000 data-place-0.2.3/data_place.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-02 20:35:33.000000 data-place-0.2.3/data_place.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 20:35:33.459474 data-place-0.2.3/dataplace/
--rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.2.3/dataplace/__init__.py
--rw-rw-rw-   0        0        0     1611 2024-01-24 19:26:19.000000 data-place-0.2.3/dataplace/base.py
--rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.2.3/dataplace/callback.py
--rw-rw-rw-   0        0        0     3146 2024-05-02 20:35:30.000000 data-place-0.2.3/dataplace/control.py
--rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.2.3/dataplace/handler.py
--rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.2.3/dataplace/io.py
--rw-rw-rw-   0        0        0     8302 2024-01-26 07:10:39.000000 data-place-0.2.3/dataplace/receive.py
--rw-rw-rw-   0        0        0    10585 2024-01-26 07:23:18.000000 data-place-0.2.3/dataplace/send.py
--rw-rw-rw-   0        0        0     7260 2024-04-27 12:38:35.000000 data-place-0.2.3/dataplace/store.py
--rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.2.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 20:35:33.461681 data-place-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1615 2024-05-02 20:35:30.000000 data-place-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:39:49.666396 data-place-0.2.4/
+-rw-rw-rw-   0        0        0       44 2024-05-02 20:39:49.000000 data-place-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6073 2024-05-02 20:39:49.665219 data-place-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.2.4/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.2.4/build.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:39:49.665219 data-place-0.2.4/data_place.egg-info/
+-rw-rw-rw-   0        0        0     6073 2024-05-02 20:39:49.000000 data-place-0.2.4/data_place.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-05-02 20:39:49.000000 data-place-0.2.4/data_place.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 20:39:49.000000 data-place-0.2.4/data_place.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-02 20:39:49.000000 data-place-0.2.4/data_place.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-02 20:39:49.000000 data-place-0.2.4/data_place.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 20:39:49.664214 data-place-0.2.4/dataplace/
+-rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.2.4/dataplace/__init__.py
+-rw-rw-rw-   0        0        0     1611 2024-01-24 19:26:19.000000 data-place-0.2.4/dataplace/base.py
+-rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.2.4/dataplace/callback.py
+-rw-rw-rw-   0        0        0     3178 2024-05-02 20:39:46.000000 data-place-0.2.4/dataplace/control.py
+-rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.2.4/dataplace/handler.py
+-rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.2.4/dataplace/io.py
+-rw-rw-rw-   0        0        0     8302 2024-01-26 07:10:39.000000 data-place-0.2.4/dataplace/receive.py
+-rw-rw-rw-   0        0        0    10585 2024-01-26 07:23:18.000000 data-place-0.2.4/dataplace/send.py
+-rw-rw-rw-   0        0        0     7260 2024-04-27 12:38:35.000000 data-place-0.2.4/dataplace/store.py
+-rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.2.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 20:39:49.666396 data-place-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2024-05-02 20:39:46.000000 data-place-0.2.4/setup.py
```

### Comparing `data-place-0.2.3/PKG-INFO` & `data-place-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.2.3
+Version: 0.2.4
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.2.3/README.md` & `data-place-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `data-place-0.2.3/build.py` & `data-place-0.2.4/build.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.3/data_place.egg-info/PKG-INFO` & `data-place-0.2.4/data_place.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.2.3
+Version: 0.2.4
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.2.3/dataplace/base.py` & `data-place-0.2.4/dataplace/base.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.3/dataplace/callback.py` & `data-place-0.2.4/dataplace/callback.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.3/dataplace/control.py` & `data-place-0.2.4/dataplace/control.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         results: list[T] = None
 ) -> list[T]:
 
     if results is None:
         results = []
 
     while controller.running:
-        results.append(await target(*args, **kwargs))
+        results.append(await target(*(args or ()), **(kwargs or {})))
 
         await controller.async_hold()
 
     return results
 
 def loop[T](
         controller: Controller,
@@ -126,12 +126,12 @@
         results: list[T] = None
 ) -> list[T]:
 
     if results is None:
         results = []
 
     while controller.running:
-        results.append(target(*args, **kwargs))
+        results.append(target(*(args or ()), **(kwargs or {})))
 
         controller.hold()
 
     return results
```

### Comparing `data-place-0.2.3/dataplace/handler.py` & `data-place-0.2.4/dataplace/handler.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.3/dataplace/io.py` & `data-place-0.2.4/dataplace/io.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.3/dataplace/receive.py` & `data-place-0.2.4/dataplace/receive.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.3/dataplace/send.py` & `data-place-0.2.4/dataplace/send.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.3/dataplace/store.py` & `data-place-0.2.4/dataplace/store.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.3/setup.py` & `data-place-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='data-place',
-        version='0.2.3',
+        version='0.2.4',
         description=(
             "A powerfull and flexible framework for designing async "
             "socket based data streaming and distribution systems, "
             "with automated parsing, dynamic data store and "
             "high-level control hooks."
         ),
         license='MIT',
```


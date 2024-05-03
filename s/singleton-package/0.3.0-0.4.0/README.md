# Comparing `tmp/singleton_package-0.3.0.tar.gz` & `tmp/singleton_package-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singleton_package-0.3.0.tar", last modified: Tue Apr 23 15:31:19 2024, max compression
+gzip compressed data, was "singleton_package-0.4.0.tar", last modified: Fri May  3 09:55:07 2024, max compression
```

## Comparing `singleton_package-0.3.0.tar` & `singleton_package-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:31:19.199177 singleton_package-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 15:31:19.199177 singleton_package-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-23 15:31:15.000000 singleton_package-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:31:19.199177 singleton_package-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-23 15:31:15.000000 singleton_package-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:31:19.195177 singleton_package-0.3.0/singleton/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 15:31:15.000000 singleton_package-0.3.0/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-23 15:31:15.000000 singleton_package-0.3.0/singleton/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-23 15:31:15.000000 singleton_package-0.3.0/singleton/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:31:19.199177 singleton_package-0.3.0/singleton_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 15:31:19.000000 singleton_package-0.3.0/singleton_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 15:31:19.000000 singleton_package-0.3.0/singleton_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:31:19.000000 singleton_package-0.3.0/singleton_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:31:19.000000 singleton_package-0.3.0/singleton_package.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 15:31:19.000000 singleton_package-0.3.0/singleton_package.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:07.182742 singleton_package-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-03 09:55:07.182742 singleton_package-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-03 09:55:03.000000 singleton_package-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:55:07.182742 singleton_package-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-03 09:55:03.000000 singleton_package-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:07.182742 singleton_package-0.4.0/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 09:55:03.000000 singleton_package-0.4.0/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-03 09:55:03.000000 singleton_package-0.4.0/singleton/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-03 09:55:03.000000 singleton_package-0.4.0/singleton/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:07.182742 singleton_package-0.4.0/singleton_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-03 09:55:07.000000 singleton_package-0.4.0/singleton_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-03 09:55:07.000000 singleton_package-0.4.0/singleton_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:55:07.000000 singleton_package-0.4.0/singleton_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:55:07.000000 singleton_package-0.4.0/singleton_package.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 09:55:07.000000 singleton_package-0.4.0/singleton_package.egg-info/top_level.txt
```

### Comparing `singleton_package-0.3.0/PKG-INFO` & `singleton_package-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singleton_package
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple Python package to create singleton objects
 Home-page: https://github.com/mahdikiani/singleton_package
 Author: Mahdi Kiani
 Author-email: mahdikiany@gmail.com
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -21,15 +21,15 @@
 pip install singleton_package
 ```
 
 ## Usage
 To use the Singleton metaclass in your classes, simply specify Singleton as the metaclass:
 
 ```python
-from singleton_package import Singleton
+from singleton import Singleton
 
 class MyClass(metaclass=Singleton):
     def __init__(self):
         # Your initialization code here
         pass
 
 # Usage
```

### Comparing `singleton_package-0.3.0/README.md` & `singleton_package-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 pip install singleton_package
 ```
 
 ## Usage
 To use the Singleton metaclass in your classes, simply specify Singleton as the metaclass:
 
 ```python
-from singleton_package import Singleton
+from singleton import Singleton
 
 class MyClass(metaclass=Singleton):
     def __init__(self):
         # Your initialization code here
         pass
 
 # Usage
```

### Comparing `singleton_package-0.3.0/setup.py` & `singleton_package-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `singleton_package-0.3.0/singleton/test.py` & `singleton_package-0.4.0/singleton/test.py`

 * *Files identical despite different names*

### Comparing `singleton_package-0.3.0/singleton_package.egg-info/PKG-INFO` & `singleton_package-0.4.0/singleton_package.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singleton_package
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple Python package to create singleton objects
 Home-page: https://github.com/mahdikiani/singleton_package
 Author: Mahdi Kiani
 Author-email: mahdikiany@gmail.com
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -21,15 +21,15 @@
 pip install singleton_package
 ```
 
 ## Usage
 To use the Singleton metaclass in your classes, simply specify Singleton as the metaclass:
 
 ```python
-from singleton_package import Singleton
+from singleton import Singleton
 
 class MyClass(metaclass=Singleton):
     def __init__(self):
         # Your initialization code here
         pass
 
 # Usage
```


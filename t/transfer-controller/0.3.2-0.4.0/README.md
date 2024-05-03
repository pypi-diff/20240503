# Comparing `tmp/transfer_controller-0.3.2.tar.gz` & `tmp/transfer_controller-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transfer_controller-0.3.2.tar", last modified: Sat Feb 10 18:39:57 2024, max compression
+gzip compressed data, was "transfer_controller-0.4.0.tar", last modified: Fri May  3 17:31:40 2024, max compression
```

## Comparing `transfer_controller-0.3.2.tar` & `transfer_controller-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 18:39:57.443590 transfer_controller-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-02-10 18:39:57.443590 transfer_controller-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-02-10 18:39:45.000000 transfer_controller-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-10 18:39:57.443590 transfer_controller-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-10 18:39:45.000000 transfer_controller-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 18:39:57.443590 transfer_controller-0.3.2/transfer_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-02-10 18:39:45.000000 transfer_controller-0.3.2/transfer_controller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 18:39:57.443590 transfer_controller-0.3.2/transfer_controller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-02-10 18:39:57.000000 transfer_controller-0.3.2/transfer_controller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-10 18:39:57.000000 transfer_controller-0.3.2/transfer_controller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 18:39:57.000000 transfer_controller-0.3.2/transfer_controller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-10 18:39:57.000000 transfer_controller-0.3.2/transfer_controller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:31:40.613103 transfer_controller-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-03 17:31:40.613103 transfer_controller-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-05-03 17:31:25.000000 transfer_controller-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:31:40.613103 transfer_controller-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-03 17:31:25.000000 transfer_controller-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:31:40.613103 transfer_controller-0.4.0/transfer_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-03 17:31:25.000000 transfer_controller-0.4.0/transfer_controller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:31:40.613103 transfer_controller-0.4.0/transfer_controller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-03 17:31:40.000000 transfer_controller-0.4.0/transfer_controller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 17:31:40.000000 transfer_controller-0.4.0/transfer_controller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:31:40.000000 transfer_controller-0.4.0/transfer_controller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 17:31:40.000000 transfer_controller-0.4.0/transfer_controller.egg-info/top_level.txt
```

### Comparing `transfer_controller-0.3.2/PKG-INFO` & `transfer_controller-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: transfer_controller
-Version: 0.3.2
+Version: 0.4.0
 Summary: A module for controlling transfer sequences.
 Author: Binho LLC
 Author-email: support@binho.io
 License: Private
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Transfer Controller
 
 A Python module for orchestrating asynchronous operations.
 
 ## Introduction
```

### Comparing `transfer_controller-0.3.2/README.md` & `transfer_controller-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `transfer_controller-0.3.2/setup.py` & `transfer_controller-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='transfer_controller',
-    version='0.3.2',
+    version='0.4.0',
     description='A module for controlling transfer sequences.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Binho LLC',
     author_email='support@binho.io',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-    python_requires='>=3.10',
+    python_requires='>=3.9',
     license='Private'
 )
```

### Comparing `transfer_controller-0.3.2/transfer_controller/__init__.py` & `transfer_controller-0.4.0/transfer_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `transfer_controller-0.3.2/transfer_controller.egg-info/PKG-INFO` & `transfer_controller-0.4.0/transfer_controller.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: transfer-controller
-Version: 0.3.2
+Version: 0.4.0
 Summary: A module for controlling transfer sequences.
 Author: Binho LLC
 Author-email: support@binho.io
 License: Private
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Transfer Controller
 
 A Python module for orchestrating asynchronous operations.
 
 ## Introduction
```


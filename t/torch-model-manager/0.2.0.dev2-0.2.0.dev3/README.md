# Comparing `tmp/torch_model_manager-0.2.0.dev2.tar.gz` & `tmp/torch_model_manager-0.2.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.2.0.dev2.tar", last modified: Thu May  2 13:44:32 2024, max compression
+gzip compressed data, was "torch_model_manager-0.2.0.dev3.tar", last modified: Fri May  3 01:46:26 2024, max compression
```

## Comparing `torch_model_manager-0.2.0.dev2.tar` & `torch_model_manager-0.2.0.dev3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.067510 torch_model_manager-0.2.0.dev2/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 13:44:32.067510 torch_model_manager-0.2.0.dev2/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-02 13:44:32.067510 torch_model_manager-0.2.0.dev2/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1504 2024-05-02 13:44:26.000000 torch_model_manager-0.2.0.dev2/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.043510 torch_model_manager-0.2.0.dev2/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.047510 torch_model_manager-0.2.0.dev2/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.051510 torch_model_manager-0.2.0.dev2/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.051510 torch_model_manager-0.2.0.dev2/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22463 2024-05-02 13:38:54.000000 torch_model_manager-0.2.0.dev2/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev2/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.067510 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 13:44:32.000000 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-02 13:44:32.000000 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-02 13:44:32.000000 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-02 13:44:32.000000 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-02 13:44:32.000000 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.067510 torch_model_manager-0.2.0.dev2/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.2.0.dev2/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.214004 torch_model_manager-0.2.0.dev3/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 01:46:26.198004 torch_model_manager-0.2.0.dev3/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-03 01:46:26.214004 torch_model_manager-0.2.0.dev3/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1504 2024-05-03 01:46:19.000000 torch_model_manager-0.2.0.dev3/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.190004 torch_model_manager-0.2.0.dev3/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.190004 torch_model_manager-0.2.0.dev3/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.190004 torch_model_manager-0.2.0.dev3/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.194004 torch_model_manager-0.2.0.dev3/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22490 2024-05-03 01:43:00.000000 torch_model_manager-0.2.0.dev3/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev3/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.198004 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 01:46:26.000000 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-03 01:46:26.000000 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-03 01:46:26.000000 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-03 01:46:26.000000 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-03 01:46:26.000000 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.194004 torch_model_manager-0.2.0.dev3/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.2.0.dev3/utils/helpers.py
```

### Comparing `torch_model_manager-0.2.0.dev2/PKG-INFO` & `torch_model_manager-0.2.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev2
+Version: 0.2.0.dev3
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev2/README.md` & `torch_model_manager-0.2.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev2/setup.py` & `torch_model_manager-0.2.0.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 version = '0.2.0.dev1'
 setup(
     name='torch-model-manager',
-    version='0.2.0.dev2',
+    version='0.2.0.dev3',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.2.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.2.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev2/tests/test_utils/test_helpers.py` & `torch_model_manager-0.2.0.dev3/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev2/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.2.0.dev3/torch_model_manager/neptune_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,23 +347,23 @@
                 args: The arguments to log.
                 namespace (str): The namespace to log the arguments.
             """
             self.run[namespace] = args
             
             print(Fore.GREEN+"The arguments are successfully logged to Neptune.", Fore.WHITE)
         
-        def delete_data(self, namespaces):
+        def delete_data(self, namespaces, wait = False):
             """
             Delete data from the run.
 
             Args:
                 namespaces: The namespaces to delete.
             """
             for namespace in namespaces:
-                self.run.pop(namespace)
+                self.run.pop(namespace, wait = wait)
 
         def stop_run(self):
             """
             Stop the run.
             """
             self.run.stop()
```

### Comparing `torch_model_manager-0.2.0.dev2/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.2.0.dev3/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev2
+Version: 0.2.0.dev3
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev2/utils/helpers.py` & `torch_model_manager-0.2.0.dev3/utils/helpers.py`

 * *Files identical despite different names*


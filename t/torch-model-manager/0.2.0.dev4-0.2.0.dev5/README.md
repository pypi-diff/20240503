# Comparing `tmp/torch_model_manager-0.2.0.dev4.tar.gz` & `tmp/torch_model_manager-0.2.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.2.0.dev4.tar", last modified: Fri May  3 09:58:04 2024, max compression
+gzip compressed data, was "torch_model_manager-0.2.0.dev5.tar", last modified: Fri May  3 10:03:00 2024, max compression
```

## Comparing `torch_model_manager-0.2.0.dev4.tar` & `torch_model_manager-0.2.0.dev5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.772145 torch_model_manager-0.2.0.dev4/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 09:58:04.772145 torch_model_manager-0.2.0.dev4/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-03 09:58:04.772145 torch_model_manager-0.2.0.dev4/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1482 2024-05-03 09:58:00.000000 torch_model_manager-0.2.0.dev4/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.764145 torch_model_manager-0.2.0.dev4/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.768145 torch_model_manager-0.2.0.dev4/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.768145 torch_model_manager-0.2.0.dev4/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.768145 torch_model_manager-0.2.0.dev4/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22627 2024-05-03 09:55:35.000000 torch_model_manager-0.2.0.dev4/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev4/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.772145 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 09:58:04.000000 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-03 09:58:04.000000 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-03 09:58:04.000000 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-03 09:58:04.000000 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-03 09:58:04.000000 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.772145 torch_model_manager-0.2.0.dev4/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     7112 2024-05-03 09:50:17.000000 torch_model_manager-0.2.0.dev4/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.270626 torch_model_manager-0.2.0.dev5/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 10:03:00.270626 torch_model_manager-0.2.0.dev5/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-03 10:03:00.274626 torch_model_manager-0.2.0.dev5/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1482 2024-05-03 10:02:57.000000 torch_model_manager-0.2.0.dev5/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.266626 torch_model_manager-0.2.0.dev5/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.266626 torch_model_manager-0.2.0.dev5/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.266626 torch_model_manager-0.2.0.dev5/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.270626 torch_model_manager-0.2.0.dev5/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22544 2024-05-03 10:00:24.000000 torch_model_manager-0.2.0.dev5/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev5/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.270626 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 10:03:00.000000 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-03 10:03:00.000000 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-03 10:03:00.000000 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-03 10:03:00.000000 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-03 10:03:00.000000 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.270626 torch_model_manager-0.2.0.dev5/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     7112 2024-05-03 09:50:17.000000 torch_model_manager-0.2.0.dev5/utils/helpers.py
```

### Comparing `torch_model_manager-0.2.0.dev4/PKG-INFO` & `torch_model_manager-0.2.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev4
+Version: 0.2.0.dev5
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev4/README.md` & `torch_model_manager-0.2.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev4/setup.py` & `torch_model_manager-0.2.0.dev5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.2.0.dev4',
+    version='0.2.0.dev5',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.2.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.2.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev4/tests/test_utils/test_helpers.py` & `torch_model_manager-0.2.0.dev5/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev4/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.2.0.dev5/torch_model_manager/neptune_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,14 @@
             Delete data from the run.
 
             Args:
                 namespaces: The namespaces to delete.
             """
             for namespace in namespaces:
                 self.run.pop(namespace, wait = wait)
-                helpers.delete_json_item(NeptuneManager.run_ids_path, [self.name])
 
         def stop_run(self):
             """
             Stop the run.
             """
             self.run.stop()
```

### Comparing `torch_model_manager-0.2.0.dev4/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.2.0.dev5/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev4
+Version: 0.2.0.dev5
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev4/utils/helpers.py` & `torch_model_manager-0.2.0.dev5/utils/helpers.py`

 * *Files identical despite different names*


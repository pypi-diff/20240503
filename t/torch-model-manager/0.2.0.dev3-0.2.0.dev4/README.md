# Comparing `tmp/torch_model_manager-0.2.0.dev3.tar.gz` & `tmp/torch_model_manager-0.2.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.2.0.dev3.tar", last modified: Fri May  3 01:46:26 2024, max compression
+gzip compressed data, was "torch_model_manager-0.2.0.dev4.tar", last modified: Fri May  3 09:58:04 2024, max compression
```

## Comparing `torch_model_manager-0.2.0.dev3.tar` & `torch_model_manager-0.2.0.dev4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.214004 torch_model_manager-0.2.0.dev3/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 01:46:26.198004 torch_model_manager-0.2.0.dev3/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-03 01:46:26.214004 torch_model_manager-0.2.0.dev3/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1504 2024-05-03 01:46:19.000000 torch_model_manager-0.2.0.dev3/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.190004 torch_model_manager-0.2.0.dev3/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.190004 torch_model_manager-0.2.0.dev3/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.190004 torch_model_manager-0.2.0.dev3/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.194004 torch_model_manager-0.2.0.dev3/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22490 2024-05-03 01:43:00.000000 torch_model_manager-0.2.0.dev3/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev3/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.198004 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 01:46:26.000000 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-03 01:46:26.000000 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-03 01:46:26.000000 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-03 01:46:26.000000 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-03 01:46:26.000000 torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 01:46:26.194004 torch_model_manager-0.2.0.dev3/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev3/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.2.0.dev3/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.772145 torch_model_manager-0.2.0.dev4/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 09:58:04.772145 torch_model_manager-0.2.0.dev4/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-03 09:58:04.772145 torch_model_manager-0.2.0.dev4/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1482 2024-05-03 09:58:00.000000 torch_model_manager-0.2.0.dev4/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.764145 torch_model_manager-0.2.0.dev4/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.768145 torch_model_manager-0.2.0.dev4/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.768145 torch_model_manager-0.2.0.dev4/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.768145 torch_model_manager-0.2.0.dev4/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22627 2024-05-03 09:55:35.000000 torch_model_manager-0.2.0.dev4/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev4/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.772145 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 09:58:04.000000 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-03 09:58:04.000000 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-03 09:58:04.000000 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-03 09:58:04.000000 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-03 09:58:04.000000 torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 09:58:04.772145 torch_model_manager-0.2.0.dev4/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev4/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     7112 2024-05-03 09:50:17.000000 torch_model_manager-0.2.0.dev4/utils/helpers.py
```

### Comparing `torch_model_manager-0.2.0.dev3/PKG-INFO` & `torch_model_manager-0.2.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev3
+Version: 0.2.0.dev4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev3/README.md` & `torch_model_manager-0.2.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev3/setup.py` & `torch_model_manager-0.2.0.dev4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = '0.2.0.dev1'
+
 setup(
     name='torch-model-manager',
-    version='0.2.0.dev3',
+    version='0.2.0.dev4',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.2.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.2.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev3/tests/test_utils/test_helpers.py` & `torch_model_manager-0.2.0.dev4/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev3/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.2.0.dev4/torch_model_manager/neptune_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,46 +119,47 @@
                 description (str, optional): The description of the run. Defaults to None.
                 tags (list, optional): The tags of the run. Defaults to None.
                 source_files (list, optional): The source files of the run. Defaults to None.
                 capture_strerr (bool, optional): Whether to capture stderr. Defaults to True.
                 git_ref (str, optional): The git reference of the run. Defaults to None.
             """
             self.run = None
+            self.name = name
             # Try to read the JSON file
             try:
                 run_ids = helpers.read_json_file(NeptuneManager.run_ids_path)
                 # If the name of the run already exists in the JSON file, load the run with the same name.
-                if name in list(run_ids.keys()): 
+                if self.name in list(run_ids.keys()): 
                     if run_ids is not None:
                         self.run = neptune.init_run(
                             project=NeptuneManager.project_name,
                             api_token=NeptuneManager.api_token,
-                            with_id=run_ids[name],
+                            with_id=run_ids[self.name],
                             **kwargs
                         )
                         
                 else:
                     # Create a new run
                     # The names of the runs should all be different
-                    assert name not in list(run_ids.keys()), "Run with the same name already exists. Please choose a different name."    
+                    assert self.name not in list(run_ids.keys()), "Run with the same name already exists. Please choose a different name."    
                     
                     self.run = neptune.init_run(
                         project=NeptuneManager.project_name,
                         api_token=NeptuneManager.api_token,
-                        name=name,
+                        name=self.name,
                         description=description,
                         tags=tags,
                         source_files=source_files,
                         capture_stderr=capture_strerr,
                         git_ref=git_ref,
                         **kwargs
                     ) 
                     # Retrieve the id of the run and store it in the file with its associated name
                     self.run_id = self.run["sys/id"].fetch()
-                    helpers.add_to_json_file(NeptuneManager.run_ids_path, name, self.run_id)
+                    helpers.add_to_json_file(NeptuneManager.run_ids_path, self.name, self.run_id)
             except:
                 print(Fore.RED+"The JSON file is not found. Please check the path."+Fore.WHITE)
             
         def log_tensors(self, 
                         tensors, 
                         descriptions: List[str] = None, 
                         names: List[str] = None, 
@@ -356,14 +357,15 @@
             Delete data from the run.
 
             Args:
                 namespaces: The namespaces to delete.
             """
             for namespace in namespaces:
                 self.run.pop(namespace, wait = wait)
+                helpers.delete_json_item(NeptuneManager.run_ids_path, [self.name])
 
         def stop_run(self):
             """
             Stop the run.
             """
             self.run.stop()
```

### Comparing `torch_model_manager-0.2.0.dev3/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.2.0.dev4/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev3
+Version: 0.2.0.dev4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev3/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.2.0.dev4/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev3/utils/helpers.py` & `torch_model_manager-0.2.0.dev4/utils/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -201,7 +201,27 @@
 
     Returns:
         The content of the JSON file.
     """
     with open(file_path, 'r') as json_file:
         data = json.load(json_file)
     return data
+
+
+def delete_json_item(json_file, key_list):
+    # Load JSON data from file
+    with open(json_file, 'r') as f:
+        data = json.load(f)
+    
+    # Function to recursively search and delete item by key list
+    def recursive_delete(d, keys):
+        if len(keys) == 1:
+            del d[keys[0]]
+        else:
+            recursive_delete(d[keys[0]], keys[1:])
+    
+    # Recursively search and delete item by key list
+    recursive_delete(data, key_list)
+    
+    # Save the modified JSON data back to the file
+    with open(json_file, 'w') as f:
+        json.dump(data, f, indent=4)
```


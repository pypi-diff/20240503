# Comparing `tmp/torch_model_manager-0.2.0.dev1.tar.gz` & `tmp/torch_model_manager-0.2.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.2.0.dev1.tar", last modified: Thu May  2 07:24:56 2024, max compression
+gzip compressed data, was "torch_model_manager-0.2.0.dev2.tar", last modified: Thu May  2 13:44:32 2024, max compression
```

## Comparing `torch_model_manager-0.2.0.dev1.tar` & `torch_model_manager-0.2.0.dev2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.085000 torch_model_manager-0.2.0.dev1/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-02 07:24:56.085000 torch_model_manager-0.2.0.dev1/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-02 07:24:50.000000 torch_model_manager-0.2.0.dev1/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.077000 torch_model_manager-0.2.0.dev1/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22434 2024-05-02 07:24:44.000000 torch_model_manager-0.2.0.dev1/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev1/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 07:24:56.000000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-02 07:24:56.000000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-02 07:24:56.000000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-02 07:24:56.000000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-02 07:24:56.000000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.2.0.dev1/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.067510 torch_model_manager-0.2.0.dev2/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 13:44:32.067510 torch_model_manager-0.2.0.dev2/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-02 13:44:32.067510 torch_model_manager-0.2.0.dev2/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1504 2024-05-02 13:44:26.000000 torch_model_manager-0.2.0.dev2/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.043510 torch_model_manager-0.2.0.dev2/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.047510 torch_model_manager-0.2.0.dev2/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.051510 torch_model_manager-0.2.0.dev2/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.051510 torch_model_manager-0.2.0.dev2/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22463 2024-05-02 13:38:54.000000 torch_model_manager-0.2.0.dev2/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev2/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.067510 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 13:44:32.000000 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-02 13:44:32.000000 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-02 13:44:32.000000 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-02 13:44:32.000000 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-02 13:44:32.000000 torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 13:44:32.067510 torch_model_manager-0.2.0.dev2/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev2/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.2.0.dev2/utils/helpers.py
```

### Comparing `torch_model_manager-0.2.0.dev1/PKG-INFO` & `torch_model_manager-0.2.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev1
+Version: 0.2.0.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev1/README.md` & `torch_model_manager-0.2.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev1/setup.py` & `torch_model_manager-0.2.0.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 version = '0.2.0.dev1'
 setup(
     name='torch-model-manager',
-    version=version,
+    version='0.2.0.dev2',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh', 
                                     'resources.md',
                                     'torch_model_manager/src/run_ids.json',
                                     '.pypirc',
                                     'torch_model_manager/src/__pycache__',
-                                    'torch_model_manager/src/.neptune']),
+                                    'torch_model_manager/src/.neptune',
+                                    'upload.py']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
     keywords=['PyTorch', 'Deep Learning', 'Machine Learning', 'High Level Programming'],
     install_requires=[
         'torch',
         'numpy',
```

### Comparing `torch_model_manager-0.2.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.2.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev1/tests/test_utils/test_helpers.py` & `torch_model_manager-0.2.0.dev2/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev1/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.2.0.dev2/torch_model_manager/neptune_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,19 +475,19 @@
             
                 print(Fore.GREEN+"The data is successfully fetched from Neptune.", Fore.WHITE)
                 return data
                 
             except:
                 print(Fore.RED+"The data is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
 
-        def load_model_checkpoint(self, namespace):
+        def load_model_checkpoint(self, namespace, **kwargs):
             tmp_file = tempfile.NamedTemporaryFile(delete=True)
             try:
                 self.run[namespace].download(tmp_file.name)
-                state_dict = torch.load(tmp_file.name)
+                state_dict = torch.load(tmp_file.name, **kwargs)
                 
                 return state_dict
             except:
                 print(Fore.RED+"The checkpoint is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
 
         def fetch_files(self, namespace):
             ns = namespace.split("/")
@@ -497,14 +497,15 @@
                 struct = struct[elem]
             
             return list(struct.keys())
         
         def fetch_data(self, namespace):
             return self.run[namespace].fetch_values()
         
+        
 # nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
 #                     api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
 #                     run_ids_path="run_ids.json")
 
 # from torchvision import models
 # parameters = {
 #     "lr": 1e-2,
```

### Comparing `torch_model_manager-0.2.0.dev1/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.2.0.dev2/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev1
+Version: 0.2.0.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.2.0.dev2/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev1/utils/helpers.py` & `torch_model_manager-0.2.0.dev2/utils/helpers.py`

 * *Files identical despite different names*


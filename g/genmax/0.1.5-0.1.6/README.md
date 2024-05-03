# Comparing `tmp/genmax-0.1.5.tar.gz` & `tmp/genmax-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genmax-0.1.5.tar", last modified: Tue Mar 12 23:21:03 2024, max compression
+gzip compressed data, was "genmax-0.1.6.tar", last modified: Fri May  3 04:17:15 2024, max compression
```

## Comparing `genmax-0.1.5.tar` & `genmax-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-03-12 23:21:03.498755 genmax-0.1.5/
--rw-r--r--   0 raza       (501) staff       (20)    11342 2024-01-10 00:50:20.000000 genmax-0.1.5/LICENSE
--rw-r--r--   0 raza       (501) staff       (20)     3341 2024-03-12 23:21:03.497844 genmax-0.1.5/PKG-INFO
--rw-r--r--   0 raza       (501) staff       (20)     2714 2024-02-28 05:36:01.000000 genmax-0.1.5/README.md
-drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-03-12 23:21:03.497062 genmax-0.1.5/genmax.egg-info/
--rw-r--r--   0 raza       (501) staff       (20)     3341 2024-03-12 23:21:03.000000 genmax-0.1.5/genmax.egg-info/PKG-INFO
--rw-r--r--   0 raza       (501) staff       (20)      509 2024-03-12 23:21:03.000000 genmax-0.1.5/genmax.egg-info/SOURCES.txt
--rw-r--r--   0 raza       (501) staff       (20)        1 2024-03-12 23:21:03.000000 genmax-0.1.5/genmax.egg-info/dependency_links.txt
--rw-r--r--   0 raza       (501) staff       (20)       37 2024-03-12 23:21:03.000000 genmax-0.1.5/genmax.egg-info/entry_points.txt
--rw-r--r--   0 raza       (501) staff       (20)       79 2024-03-12 23:21:03.000000 genmax-0.1.5/genmax.egg-info/requires.txt
--rw-r--r--   0 raza       (501) staff       (20)        4 2024-03-12 23:21:03.000000 genmax-0.1.5/genmax.egg-info/top_level.txt
-drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-03-12 23:21:03.490675 genmax-0.1.5/gmx/
--rw-r--r--   0 raza       (501) staff       (20)        0 2024-01-10 02:41:55.000000 genmax-0.1.5/gmx/__init__.py
-drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-03-12 23:21:03.492444 genmax-0.1.5/gmx/cmd/
--rw-r--r--   0 raza       (501) staff       (20)        0 2023-11-12 17:23:49.000000 genmax-0.1.5/gmx/cmd/__init__.py
--rw-r--r--   0 raza       (501) staff       (20)      843 2024-02-28 02:56:14.000000 genmax-0.1.5/gmx/cmd/initialize.py
--rw-r--r--   0 raza       (501) staff       (20)     2900 2024-01-18 05:26:27.000000 genmax-0.1.5/gmx/cmd/project.py
--rw-r--r--   0 raza       (501) staff       (20)      997 2024-02-28 02:44:15.000000 genmax-0.1.5/gmx/cmd/workflow.py
--rw-r--r--   0 raza       (501) staff       (20)     1415 2024-02-28 05:29:54.000000 genmax-0.1.5/gmx/extensions.py
-drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-03-12 23:21:03.496366 genmax-0.1.5/gmx/logic/
--rw-r--r--   0 raza       (501) staff       (20)        0 2024-01-10 02:47:59.000000 genmax-0.1.5/gmx/logic/__init__.py
--rw-r--r--   0 raza       (501) staff       (20)     1091 2024-01-18 04:47:59.000000 genmax-0.1.5/gmx/logic/common.py
--rw-r--r--   0 raza       (501) staff       (20)      556 2024-02-28 02:03:08.000000 genmax-0.1.5/gmx/logic/fileops.py
--rw-r--r--   0 raza       (501) staff       (20)     2203 2024-03-09 04:30:25.000000 genmax-0.1.5/gmx/logic/generation.py
--rw-r--r--   0 raza       (501) staff       (20)     1495 2024-01-14 01:43:19.000000 genmax-0.1.5/gmx/logic/preference.py
--rw-r--r--   0 raza       (501) staff       (20)     3010 2024-01-18 02:14:52.000000 genmax-0.1.5/gmx/logic/project.py
--rw-r--r--   0 raza       (501) staff       (20)      248 2024-02-26 20:32:50.000000 genmax-0.1.5/gmx/logic/runner.py
--rw-r--r--   0 raza       (501) staff       (20)     2649 2024-03-09 04:29:47.000000 genmax-0.1.5/gmx/logic/workflow.py
--rw-r--r--   0 raza       (501) staff       (20)      582 2024-01-14 23:24:29.000000 genmax-0.1.5/gmx/main.py
--rw-r--r--   0 raza       (501) staff       (20)       38 2024-03-12 23:21:03.498955 genmax-0.1.5/setup.cfg
--rw-r--r--   0 raza       (501) staff       (20)     1046 2024-03-09 04:27:19.000000 genmax-0.1.5/setup.py
+drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-03 04:17:15.931185 genmax-0.1.6/
+-rw-r--r--   0 raza       (501) staff       (20)    11342 2024-01-10 00:50:20.000000 genmax-0.1.6/LICENSE
+-rw-r--r--   0 raza       (501) staff       (20)     3341 2024-05-03 04:17:15.930442 genmax-0.1.6/PKG-INFO
+-rw-r--r--   0 raza       (501) staff       (20)     2714 2024-02-28 05:36:01.000000 genmax-0.1.6/README.md
+drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-03 04:17:15.929421 genmax-0.1.6/genmax.egg-info/
+-rw-r--r--   0 raza       (501) staff       (20)     3341 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/PKG-INFO
+-rw-r--r--   0 raza       (501) staff       (20)      509 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/SOURCES.txt
+-rw-r--r--   0 raza       (501) staff       (20)        1 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/dependency_links.txt
+-rw-r--r--   0 raza       (501) staff       (20)       37 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/entry_points.txt
+-rw-r--r--   0 raza       (501) staff       (20)       79 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/requires.txt
+-rw-r--r--   0 raza       (501) staff       (20)        4 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/top_level.txt
+drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-03 04:17:15.922685 genmax-0.1.6/gmx/
+-rw-r--r--   0 raza       (501) staff       (20)        0 2024-01-10 02:41:55.000000 genmax-0.1.6/gmx/__init__.py
+drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-03 04:17:15.924330 genmax-0.1.6/gmx/cmd/
+-rw-r--r--   0 raza       (501) staff       (20)        0 2023-11-12 17:23:49.000000 genmax-0.1.6/gmx/cmd/__init__.py
+-rw-r--r--   0 raza       (501) staff       (20)      843 2024-02-28 02:56:14.000000 genmax-0.1.6/gmx/cmd/initialize.py
+-rw-r--r--   0 raza       (501) staff       (20)     2900 2024-01-18 05:26:27.000000 genmax-0.1.6/gmx/cmd/project.py
+-rw-r--r--   0 raza       (501) staff       (20)      997 2024-02-28 02:44:15.000000 genmax-0.1.6/gmx/cmd/workflow.py
+-rw-r--r--   0 raza       (501) staff       (20)     1415 2024-02-28 05:29:54.000000 genmax-0.1.6/gmx/extensions.py
+drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-03 04:17:15.928626 genmax-0.1.6/gmx/logic/
+-rw-r--r--   0 raza       (501) staff       (20)        0 2024-01-10 02:47:59.000000 genmax-0.1.6/gmx/logic/__init__.py
+-rw-r--r--   0 raza       (501) staff       (20)     1091 2024-01-18 04:47:59.000000 genmax-0.1.6/gmx/logic/common.py
+-rw-r--r--   0 raza       (501) staff       (20)      556 2024-02-28 02:03:08.000000 genmax-0.1.6/gmx/logic/fileops.py
+-rw-r--r--   0 raza       (501) staff       (20)     2203 2024-03-09 04:30:25.000000 genmax-0.1.6/gmx/logic/generation.py
+-rw-r--r--   0 raza       (501) staff       (20)     1495 2024-01-14 01:43:19.000000 genmax-0.1.6/gmx/logic/preference.py
+-rw-r--r--   0 raza       (501) staff       (20)     3117 2024-05-03 04:13:58.000000 genmax-0.1.6/gmx/logic/project.py
+-rw-r--r--   0 raza       (501) staff       (20)      248 2024-02-26 20:32:50.000000 genmax-0.1.6/gmx/logic/runner.py
+-rw-r--r--   0 raza       (501) staff       (20)     2653 2024-05-03 04:11:30.000000 genmax-0.1.6/gmx/logic/workflow.py
+-rw-r--r--   0 raza       (501) staff       (20)      582 2024-01-14 23:24:29.000000 genmax-0.1.6/gmx/main.py
+-rw-r--r--   0 raza       (501) staff       (20)       38 2024-05-03 04:17:15.931420 genmax-0.1.6/setup.cfg
+-rw-r--r--   0 raza       (501) staff       (20)     1046 2024-05-03 04:15:33.000000 genmax-0.1.6/setup.py
```

### Comparing `genmax-0.1.5/LICENSE` & `genmax-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `genmax-0.1.5/PKG-INFO` & `genmax-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genmax
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple code generation tool.
 Home-page: https://https://github.com/razaibi/genmax/
 Author: Raza Balbale
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/razaibi/genmax/README.md
 Project-URL: Source, https://github.com/razaibi/genmax
 Project-URL: Tracker, https://github.com/razaibi/genmax/
```

### Comparing `genmax-0.1.5/README.md` & `genmax-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `genmax-0.1.5/genmax.egg-info/PKG-INFO` & `genmax-0.1.6/genmax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genmax
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple code generation tool.
 Home-page: https://https://github.com/razaibi/genmax/
 Author: Raza Balbale
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/razaibi/genmax/README.md
 Project-URL: Source, https://github.com/razaibi/genmax
 Project-URL: Tracker, https://github.com/razaibi/genmax/
```

### Comparing `genmax-0.1.5/gmx/cmd/initialize.py` & `genmax-0.1.6/gmx/cmd/initialize.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.5/gmx/cmd/project.py` & `genmax-0.1.6/gmx/cmd/project.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.5/gmx/cmd/workflow.py` & `genmax-0.1.6/gmx/cmd/workflow.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.5/gmx/extensions.py` & `genmax-0.1.6/gmx/extensions.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.5/gmx/logic/common.py` & `genmax-0.1.6/gmx/logic/common.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.5/gmx/logic/fileops.py` & `genmax-0.1.6/gmx/logic/fileops.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.5/gmx/logic/generation.py` & `genmax-0.1.6/gmx/logic/generation.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.5/gmx/logic/preference.py` & `genmax-0.1.6/gmx/logic/preference.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.5/gmx/logic/project.py` & `genmax-0.1.6/gmx/logic/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,21 @@
   action: "generate"
   template: "sample_template.j2"
   output: "sample>SampleOutput.txt"
 
 - action: "write_to_file"
   template: "sample_text.j2"
   output: "sample>SampleTextFile.txt"
+
+{% for i in range(1, 6) %}
+- action: "run_command"
+  command: 'echo "Hello {{ i }}"'    
+{% endfor %}
         """
-        with open(os.path.join(flow_path, "sample.yml"), "w") as f:
+        with open(os.path.join(flow_path, "sample.yaml.j2"), "w") as f:
             f.write(sample_flow_content)
 
     def _add_sample_template(self, template_path: str):
         sample_template_content = """using System.ComponentModel.DataAnnotations;
 using System.ComponentModel.DataAnnotations.Schema;
 using System.Runtime.Serialization;
```

### Comparing `genmax-0.1.5/gmx/logic/workflow.py` & `genmax-0.1.6/gmx/logic/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     def run_workflows(self, project_name: str, flows: list, flow_data_file: str = None):
         project_path = CommonLogic.get_gmx_folder_path(os.path.join("gmx", project_name))
         for flow in flows:
             self._process_flow(flow, project_path, flow_data_file)
 
     def _process_flow(self, flow: str, project_path: str, flow_data_file: str = None):
-        flow_path = os.path.join(project_path, 'flows', f'{flow}.yml')
+        flow_path = os.path.join(project_path, 'flows', f'{flow}.yaml.j2')
         print(f'Processing Flow: {flow_path}.')
         try:
             if flow_data_file:
                 flow_data_path = os.path.join(project_path, 'data', f'{flow_data_file}.yml')
                 with open(flow_data_path) as data_file:
                     flow_data = yaml.load(data_file, Loader=yaml.FullLoader)
                 with open(flow_path, 'r') as file:
```

### Comparing `genmax-0.1.5/gmx/main.py` & `genmax-0.1.6/gmx/main.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.5/setup.py` & `genmax-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='genmax',
-    version='0.1.5',
+    version='0.1.6',
     author='Raza Balbale',
     description='A simple code generation tool.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://https://github.com/razaibi/genmax/',
     project_urls={
         'Documentation': 'https://github.com/razaibi/genmax/README.md',
```


# Comparing `tmp/molcas_suite-1.31.1.tar.gz` & `tmp/molcas_suite-1.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molcas_suite-1.31.1.tar", last modified: Tue Apr 30 14:21:10 2024, max compression
+gzip compressed data, was "molcas_suite-1.32.0.tar", last modified: Fri May  3 04:34:32 2024, max compression
```

## Comparing `molcas_suite-1.31.1.tar` & `molcas_suite-1.32.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:21:10.426656 molcas_suite-1.31.1/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3803 2024-04-30 14:21:10.426656 molcas_suite-1.31.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2952 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:21:10.425656 molcas_suite-1.31.1/molcas_suite/
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-30 14:21:05.000000 molcas_suite-1.31.1/molcas_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     6311 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/barrier.py
--rw-rw-rw-   0 root         (0) root         (0)     1440 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/cfp.py
--rw-rw-rw-   0 root         (0) root         (0)    31142 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    34861 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)    18445 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/generate_input.py
--rw-rw-rw-   0 root         (0) root         (0)    25242 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/generate_job.py
--rw-rw-rw-   0 root         (0) root         (0)     6412 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/h5tools.py
--rw-rw-rw-   0 root         (0) root         (0)    27067 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/orbs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:21:10.426656 molcas_suite-1.31.1/molcas_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3803 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      507 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 14:21:10.426656 molcas_suite-1.31.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1458 2024-04-30 14:21:05.000000 molcas_suite-1.31.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 04:34:32.693779 molcas_suite-1.32.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3804 2024-05-03 04:34:32.693779 molcas_suite-1.32.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2952 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 04:34:32.691779 molcas_suite-1.32.0/molcas_suite/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/molcas_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-05-03 04:34:28.000000 molcas_suite-1.32.0/molcas_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6311 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/molcas_suite/barrier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/molcas_suite/cfp.py
+-rw-rw-rw-   0 root         (0) root         (0)    31142 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/molcas_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    34861 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/molcas_suite/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    18445 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/molcas_suite/generate_input.py
+-rw-rw-rw-   0 root         (0) root         (0)    25692 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/molcas_suite/generate_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     6412 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/molcas_suite/h5tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    27067 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/molcas_suite/orbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 04:34:32.693779 molcas_suite-1.32.0/molcas_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3804 2024-05-03 04:34:32.000000 molcas_suite-1.32.0/molcas_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      507 2024-05-03 04:34:32.000000 molcas_suite-1.32.0/molcas_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 04:34:32.000000 molcas_suite-1.32.0/molcas_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-03 04:34:32.000000 molcas_suite-1.32.0/molcas_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-03 04:34:32.000000 molcas_suite-1.32.0/molcas_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-03 04:34:32.000000 molcas_suite-1.32.0/molcas_suite.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-03 04:33:58.000000 molcas_suite-1.32.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 04:34:32.694779 molcas_suite-1.32.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2024-05-03 04:34:28.000000 molcas_suite-1.32.0/setup.py
```

### Comparing `molcas_suite-1.31.1/LICENSE` & `molcas_suite-1.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.1/PKG-INFO` & `molcas_suite-1.32.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas_suite
-Version: 1.31.1
+Version: 1.32.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: h5py
-Requires-Dist: xyz_py>=5.6.1
+Requires-Dist: xyz_py>=5.11.0
 Requires-Dist: angmom_suite>=1.18.0
 Requires-Dist: hpc_suite>=1.8.0
 Requires-Dist: matplotlib
 
 # molcas_suite
 
 `molcas_suite` is a python package for working with OpenMOLCAS input and output files.
```

### Comparing `molcas_suite-1.31.1/README.md` & `molcas_suite-1.32.0/README.md`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.1/molcas_suite/barrier.py` & `molcas_suite-1.32.0/molcas_suite/barrier.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.1/molcas_suite/cfp.py` & `molcas_suite-1.32.0/molcas_suite/cfp.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.1/molcas_suite/cli.py` & `molcas_suite-1.32.0/molcas_suite/cli.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.1/molcas_suite/extractor.py` & `molcas_suite-1.32.0/molcas_suite/extractor.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.1/molcas_suite/generate_input.py` & `molcas_suite-1.32.0/molcas_suite/generate_input.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.1/molcas_suite/generate_job.py` & `molcas_suite-1.32.0/molcas_suite/generate_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,69 +58,81 @@
     else:
         machine = args.profile
 
     supported_machines = [
         "cerberus",
         "medusa",
         "csf3",
-        "csf4"
+        "csf4",
+        "gadi"
     ]
 
     if machine not in supported_machines:
         sys.exit("Error: Unsupported machine")
-
+    
     default_mod = {
         "cerberus": None,
         "medusa": None,
         "csf3": "chiltongroup/openmolcas/23.02",
-        "csf4": "chiltongroup/openmolcas/23.02"
+        "csf4": "chiltongroup/openmolcas/23.02",
+        "gadi": "chiltongroup/openmolcas/23.02"
     }
 
     default_path = {
         "cerberus": "/opt/OpenMolcas-21.06-hyperion",
         "medusa": "/opt/OpenMolcas-30jun21",
         "csf3": None,
-        "csf4": None
+        "csf4": None,
+        "gadi": None
     }
-
     default_mem = {
         "cerberus": {
             None: 30000
         },
         "medusa": {
             None: 30000
         },
         "csf3": {
-            None: 4000,
-            "high_mem": 16000
+            None: 4000 * args.omp,
+            "high_mem": 16000 * args.omp
         },
         "csf4": {
-            None: 4000
+            None: 4000 * args.omp
+        },
+        "gadi": {
+            None: 3500 * args.omp,
+            "normal":3500 * args.omp,
+            "normalbw":3500 * args.omp,
+            "hugemem":30000 * args.omp,
+            "hugemembw":36000 * args.omp,
         },
     }
 
     default_disk = {
         "cerberus": 20000,
         "medusa": 20000,
         "csf3": 20000,
-        "csf4": 20000
+        "csf4": 20000,
+        "gadi": 20000,
     }
 
     default_scratch = {
         "cerberus": r"$CurrDir/scratch",
         "medusa": r"$CurrDir/scratch",
         "csf3": r"/scratch/$USER/$MOLCAS_PROJECT",
-        "csf4": r"/scratch/$USER/$MOLCAS_PROJECT"
+        "csf4": r"/scratch/$USER/$MOLCAS_PROJECT",
+        "gadi": r"/scratch/ls80/$USER/$MOLCAS_PROJECT"
     }
 
     default_in_scratch = {
         "cerberus": True,
         "medusa": True,
         "csf3": False,
-        "csf4": False
+        "csf4": False,
+        "gadi": False,
     }
 
     # Fetch defaults if not set explicitly
     if molcas_module is None and molcas_path is None:
         molcas_module = default_mod[machine]
         molcas_path = default_path[machine]
 
@@ -182,15 +194,14 @@
             "    $MOLCAS/Tools/pymolcas/pymolcas_ {pymolcas_args}\n"
             "else\n"
             '    echo "Warning: Using system-wide pymolcas installation!"\n'
             "    pymolcas {pymolcas_args}\n"
             "fi\n").format(pymolcas_args=pymolcas_args)
 
     args.body = '\n'.join([body_mkdir, body_cd, body])
-
     # Generate job submission script
     hpc.generate_job_func(args)
 
 
 def gen_submission_csf_array(input_name, output_name, n_jobs, orbital,
                              dir_list_file='dir_list.txt',
                              remove_output=True, extractor='',
```

### Comparing `molcas_suite-1.31.1/molcas_suite/h5tools.py` & `molcas_suite-1.32.0/molcas_suite/h5tools.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.1/molcas_suite/orbs.py` & `molcas_suite-1.32.0/molcas_suite/orbs.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.1/molcas_suite.egg-info/PKG-INFO` & `molcas_suite-1.32.0/molcas_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas_suite
-Version: 1.31.1
+Version: 1.32.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: h5py
-Requires-Dist: xyz_py>=5.6.1
+Requires-Dist: xyz_py>=5.11.0
 Requires-Dist: angmom_suite>=1.18.0
 Requires-Dist: hpc_suite>=1.8.0
 Requires-Dist: matplotlib
 
 # molcas_suite
 
 `molcas_suite` is a python package for working with OpenMOLCAS input and output files.
```

### Comparing `molcas_suite-1.31.1/pyproject.toml` & `molcas_suite-1.32.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.1/setup.py` & `molcas_suite-1.32.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.31.1"
+__version__ = "1.32.0"
 
 setuptools.setup(
     name='molcas_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for dealing with OpenMOLCAS input and output files',
@@ -30,15 +30,15 @@
         'Operating System :: OS Independent'
         ],
     python_requires='>=3.9',
     install_requires=[
         'numpy',
         'scipy',
         'h5py',
-        'xyz_py>=5.6.1',
+        'xyz_py>=5.11.0',
         'angmom_suite>=1.18.0',
         'hpc_suite>=1.8.0',
         'matplotlib'
         ],
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
```


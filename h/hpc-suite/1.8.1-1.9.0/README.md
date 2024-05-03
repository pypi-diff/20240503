# Comparing `tmp/hpc-suite-1.8.1.tar.gz` & `tmp/hpc-suite-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpc-suite-1.8.1.tar", last modified: Thu Mar 30 12:12:55 2023, max compression
+gzip compressed data, was "hpc-suite-1.9.0.tar", last modified: Wed Aug  9 13:40:08 2023, max compression
```

## Comparing `hpc-suite-1.8.1.tar` & `hpc-suite-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:12:55.047601 hpc-suite-1.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    35077 2023-03-30 12:12:15.000000 hpc-suite-1.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3330 2023-03-30 12:12:55.045601 hpc-suite-1.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2689 2023-03-30 12:12:15.000000 hpc-suite-1.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:12:55.041600 hpc-suite-1.8.1/hpc_suite/
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-03-30 12:12:15.000000 hpc-suite-1.8.1/hpc_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-03-30 12:12:51.000000 hpc-suite-1.8.1/hpc_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     3275 2023-03-30 12:12:15.000000 hpc-suite-1.8.1/hpc_suite/action.py
--rw-rw-rw-   0 root         (0) root         (0)    10435 2023-03-30 12:12:15.000000 hpc-suite-1.8.1/hpc_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    10903 2023-03-30 12:12:15.000000 hpc-suite-1.8.1/hpc_suite/generate_job.py
--rw-rw-rw-   0 root         (0) root         (0)    16114 2023-03-30 12:12:15.000000 hpc-suite-1.8.1/hpc_suite/store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:12:55.045601 hpc-suite-1.8.1/hpc_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3330 2023-03-30 12:12:54.000000 hpc-suite-1.8.1/hpc_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      370 2023-03-30 12:12:54.000000 hpc-suite-1.8.1/hpc_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 12:12:54.000000 hpc-suite-1.8.1/hpc_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-03-30 12:12:54.000000 hpc-suite-1.8.1/hpc_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-30 12:12:54.000000 hpc-suite-1.8.1/hpc_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-30 12:12:54.000000 hpc-suite-1.8.1/hpc_suite.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-03-30 12:12:15.000000 hpc-suite-1.8.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 12:12:55.047601 hpc-suite-1.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-03-30 12:12:51.000000 hpc-suite-1.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 13:40:08.276598 hpc-suite-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35077 2023-08-09 13:39:44.000000 hpc-suite-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-08-09 13:40:08.276598 hpc-suite-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2023-08-09 13:39:44.000000 hpc-suite-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 13:40:08.274598 hpc-suite-1.9.0/hpc_suite/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-08-09 13:39:44.000000 hpc-suite-1.9.0/hpc_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-08-09 13:40:05.000000 hpc-suite-1.9.0/hpc_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2023-08-09 13:39:44.000000 hpc-suite-1.9.0/hpc_suite/action.py
+-rw-rw-rw-   0 root         (0) root         (0)    10489 2023-08-09 13:39:44.000000 hpc-suite-1.9.0/hpc_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    10895 2023-08-09 13:39:44.000000 hpc-suite-1.9.0/hpc_suite/generate_job.py
+-rw-rw-rw-   0 root         (0) root         (0)    16114 2023-08-09 13:39:44.000000 hpc-suite-1.9.0/hpc_suite/store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 13:40:08.275598 hpc-suite-1.9.0/hpc_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-08-09 13:40:08.000000 hpc-suite-1.9.0/hpc_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      370 2023-08-09 13:40:08.000000 hpc-suite-1.9.0/hpc_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 13:40:08.000000 hpc-suite-1.9.0/hpc_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-08-09 13:40:08.000000 hpc-suite-1.9.0/hpc_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-09 13:40:08.000000 hpc-suite-1.9.0/hpc_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-09 13:40:08.000000 hpc-suite-1.9.0/hpc_suite.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-08-09 13:39:44.000000 hpc-suite-1.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-09 13:40:08.276598 hpc-suite-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-08-09 13:40:05.000000 hpc-suite-1.9.0/setup.py
```

### Comparing `hpc-suite-1.8.1/LICENSE` & `hpc-suite-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hpc-suite-1.8.1/PKG-INFO` & `hpc-suite-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpc-suite
-Version: 1.8.1
+Version: 1.9.0
 Summary: A package for working with data on HPC platforms
 Home-page: https://gitlab.com/chilton-group/hpc_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/hpc_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/hpc_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hpc-suite-1.8.1/README.md` & `hpc-suite-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `hpc-suite-1.8.1/hpc_suite/action.py` & `hpc-suite-1.9.0/hpc_suite/action.py`

 * *Files identical despite different names*

### Comparing `hpc-suite-1.8.1/hpc_suite/cli.py` & `hpc-suite-1.9.0/hpc_suite/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,18 @@
 
 
 def filter_parser_args(args):
     return {key: val for key, val in vars(args).items()
             if key not in ["prog", "func",  "help", "Help"]}
 
 
+def parse_index(x):
+    return int(x) - 1
+
+
 def read_args(arg_list=None):
 
     description = '''
     A package for HPC applications.
     '''
 
     epilog = '''
@@ -305,15 +309,15 @@
         metavar='flag=value'
     )
 
     module = job.add_argument_group('Module arguments')
 
     module.add_argument(
         '--purge_modules',
-        type=bool,
+        action='store_true',
         help='Run "module purge" to remove all pre-loaded modules.'
     )
 
     module.add_argument(
         '--modules',
         nargs='+',
         default=[],
```

### Comparing `hpc-suite-1.8.1/hpc_suite/generate_job.py` & `hpc-suite-1.9.0/hpc_suite/generate_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 class Modules(Generic):
 
     def __init__(self, purge_modules=False, modules=[], env=[], **kwargs):
 
         if purge_modules is None:
             _purge_modules = []
         else:
-            _purge_modules = ["module purge_modules"] if purge_modules else []
+            _purge_modules = ["module purge"] if purge_modules else []
 
         if modules is None:
             _modules = []
         else:
             _modules = ["module load {}".format(mod) for mod in modules]
 
         _env = _purge_modules + _modules + env
```

### Comparing `hpc-suite-1.8.1/hpc_suite/store.py` & `hpc-suite-1.9.0/hpc_suite/store.py`

 * *Files identical despite different names*

### Comparing `hpc-suite-1.8.1/hpc_suite.egg-info/PKG-INFO` & `hpc-suite-1.9.0/hpc_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpc-suite
-Version: 1.8.1
+Version: 1.9.0
 Summary: A package for working with data on HPC platforms
 Home-page: https://gitlab.com/chilton-group/hpc_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/hpc_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/hpc_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hpc-suite-1.8.1/setup.py` & `hpc-suite-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.8.1"
+__version__ = "1.9.0"
 
 setuptools.setup(
     name='hpc-suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for working with data on HPC platforms',
```


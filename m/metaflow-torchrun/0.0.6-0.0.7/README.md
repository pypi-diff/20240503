# Comparing `tmp/metaflow-torchrun-0.0.6.tar.gz` & `tmp/metaflow_torchrun-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-torchrun-0.0.6.tar", last modified: Thu Apr  4 18:37:48 2024, max compression
+gzip compressed data, was "metaflow_torchrun-0.0.7.tar", last modified: Fri May  3 18:40:45 2024, max compression
```

## Comparing `metaflow-torchrun-0.0.6.tar` & `metaflow_torchrun-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.639755 metaflow-torchrun-0.0.6/
--rw-r--r--   0 eddie      (501) staff       (20)      175 2024-04-04 18:37:48.639497 metaflow-torchrun-0.0.6/PKG-INFO
--rw-r--r--   0 eddie      (501) staff       (20)     2908 2023-11-02 22:18:03.000000 metaflow-torchrun-0.0.6/README.md
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.636291 metaflow-torchrun-0.0.6/metaflow_extensions/
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.636345 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.637146 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/
--rw-r--r--   0 eddie      (501) staff       (20)      147 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/mfextinit_torchrun.py
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.638458 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/
--rw-r--r--   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/__init__.py
--rw-r--r--   0 eddie      (501) staff       (20)       74 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/constants.py
--rw-r--r--   0 eddie      (501) staff       (20)     7927 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/datastore.py
--rw-r--r--   0 eddie      (501) staff       (20)     1586 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/exceptions.py
--rw-r--r--   0 eddie      (501) staff       (20)     8923 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/executor.py
--rw-r--r--   0 eddie      (501) staff       (20)     3752 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/status_notifier.py
--rw-r--r--   0 eddie      (501) staff       (20)     1022 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/torch_distributed_setup.py
--rw-r--r--   0 eddie      (501) staff       (20)     2835 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/torchrun_decorator.py
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.639191 metaflow-torchrun-0.0.6/metaflow_torchrun.egg-info/
--rw-r--r--   0 eddie      (501) staff       (20)      175 2024-04-04 18:37:48.000000 metaflow-torchrun-0.0.6/metaflow_torchrun.egg-info/PKG-INFO
--rw-r--r--   0 eddie      (501) staff       (20)      781 2024-04-04 18:37:48.000000 metaflow-torchrun-0.0.6/metaflow_torchrun.egg-info/SOURCES.txt
--rw-r--r--   0 eddie      (501) staff       (20)        1 2024-04-04 18:37:48.000000 metaflow-torchrun-0.0.6/metaflow_torchrun.egg-info/dependency_links.txt
--rw-r--r--   0 eddie      (501) staff       (20)       20 2024-04-04 18:37:48.000000 metaflow-torchrun-0.0.6/metaflow_torchrun.egg-info/top_level.txt
--rw-r--r--   0 eddie      (501) staff       (20)       38 2024-04-04 18:37:48.639813 metaflow-torchrun-0.0.6/setup.cfg
--rw-r--r--   0 eddie      (501) staff       (20)      423 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.478519 metaflow_torchrun-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-03 18:40:45.478519 metaflow_torchrun-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.474519 metaflow_torchrun-0.0.7/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.474519 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.474519 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/mfextinit_torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.478519 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/status_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/torch_distributed_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/torchrun_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.478519 metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-03 18:40:45.000000 metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-03 18:40:45.000000 metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:40:45.000000 metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 18:40:45.000000 metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:40:45.478519 metaflow_torchrun-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/setup.py
```

### Comparing `metaflow-torchrun-0.0.6/README.md` & `metaflow_torchrun-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/datastore.py` & `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/exceptions.py` & `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/exceptions.py`

 * *Files identical despite different names*

### Comparing `metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/executor.py` & `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                     text = stdout.decode("utf-8")
                 except UnicodeDecodeError:
                     text = ""
                 print(
                     text, end="", flush=True
                 )
             if process.returncode != 0:
-                return False, process.stderr.read().decode("utf-8")
+                return False, "Process exited with errors (see above for details)"
             return True, None
 
     def _ensure_torch_installed(self):
         try:
             import torch
         except ImportError:
             raise TorchNotInstalledException()
```

### Comparing `metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/status_notifier.py` & `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/status_notifier.py`

 * *Files identical despite different names*

### Comparing `metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/torch_distributed_setup.py` & `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/torch_distributed_setup.py`

 * *Files identical despite different names*

### Comparing `metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/torchrun_decorator.py` & `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/torchrun_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-torchrun-0.0.6/metaflow_torchrun.egg-info/SOURCES.txt` & `metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/SOURCES.txt`

 * *Files identical despite different names*


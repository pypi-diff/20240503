# Comparing `tmp/torchrun_jsc-0.0.2.tar.gz` & `tmp/torchrun_jsc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchrun_jsc-0.0.2.tar", last modified: Thu Feb 29 17:38:05 2024, max compression
+gzip compressed data, was "torchrun_jsc-0.0.3.tar", last modified: Fri May  3 18:23:27 2024, max compression
```

## Comparing `torchrun_jsc-0.0.2.tar` & `torchrun_jsc-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 fzjan     (1000) fzjan     (1000)        0 2024-02-29 17:38:05.407767 torchrun_jsc-0.0.2/
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)    11340 2024-01-26 15:59:52.000000 torchrun_jsc-0.0.2/LICENSE
--rw-r--r--   0 fzjan     (1000) fzjan     (1000)      520 2024-02-29 17:38:05.407767 torchrun_jsc-0.0.2/PKG-INFO
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1896 2024-02-29 17:26:30.000000 torchrun_jsc-0.0.2/README.md
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       81 2024-02-29 16:51:51.000000 torchrun_jsc-0.0.2/pyproject.toml
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       38 2024-02-29 17:38:05.407767 torchrun_jsc-0.0.2/setup.cfg
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1210 2024-02-29 17:37:47.000000 torchrun_jsc-0.0.2/setup.py
-drwxrwxr-x   0 fzjan     (1000) fzjan     (1000)        0 2024-02-29 17:38:05.403767 torchrun_jsc-0.0.2/src/
-drwxrwxr-x   0 fzjan     (1000) fzjan     (1000)        0 2024-02-29 17:38:05.403767 torchrun_jsc-0.0.2/src/torchrun_jsc/
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1209 2024-02-29 17:14:13.000000 torchrun_jsc-0.0.2/src/torchrun_jsc/__init__.py
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       58 2024-02-29 15:34:02.000000 torchrun_jsc-0.0.2/src/torchrun_jsc/__main__.py
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1567 2024-02-29 17:17:59.000000 torchrun_jsc-0.0.2/src/torchrun_jsc/arg_patching.py
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1078 2024-02-29 17:05:15.000000 torchrun_jsc-0.0.2/src/torchrun_jsc/parsing.py
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1434 2024-02-29 17:17:04.000000 torchrun_jsc-0.0.2/src/torchrun_jsc/run.py
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1748 2024-02-29 17:37:20.000000 torchrun_jsc-0.0.2/src/torchrun_jsc/run_old.py
-drwxrwxr-x   0 fzjan     (1000) fzjan     (1000)        0 2024-02-29 17:38:05.407767 torchrun_jsc-0.0.2/src/torchrun_jsc.egg-info/
--rw-r--r--   0 fzjan     (1000) fzjan     (1000)      520 2024-02-29 17:38:05.000000 torchrun_jsc-0.0.2/src/torchrun_jsc.egg-info/PKG-INFO
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)      454 2024-02-29 17:38:05.000000 torchrun_jsc-0.0.2/src/torchrun_jsc.egg-info/SOURCES.txt
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)        1 2024-02-29 17:38:05.000000 torchrun_jsc-0.0.2/src/torchrun_jsc.egg-info/dependency_links.txt
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       55 2024-02-29 17:38:05.000000 torchrun_jsc-0.0.2/src/torchrun_jsc.egg-info/entry_points.txt
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       21 2024-02-29 17:38:05.000000 torchrun_jsc-0.0.2/src/torchrun_jsc.egg-info/requires.txt
--rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       13 2024-02-29 17:38:05.000000 torchrun_jsc-0.0.2/src/torchrun_jsc.egg-info/top_level.txt
+drwxrwxr-x   0 fzjan     (1000) fzjan     (1000)        0 2024-05-03 18:23:27.799026 torchrun_jsc-0.0.3/
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)    11340 2024-01-26 15:59:52.000000 torchrun_jsc-0.0.3/LICENSE
+-rw-r--r--   0 fzjan     (1000) fzjan     (1000)      520 2024-05-03 18:23:27.799026 torchrun_jsc-0.0.3/PKG-INFO
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1877 2024-05-03 18:18:02.000000 torchrun_jsc-0.0.3/README.md
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       81 2024-02-29 16:51:51.000000 torchrun_jsc-0.0.3/pyproject.toml
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       38 2024-05-03 18:23:27.799026 torchrun_jsc-0.0.3/setup.cfg
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1210 2024-04-23 07:30:12.000000 torchrun_jsc-0.0.3/setup.py
+drwxrwxr-x   0 fzjan     (1000) fzjan     (1000)        0 2024-05-03 18:23:27.795026 torchrun_jsc-0.0.3/src/
+drwxrwxr-x   0 fzjan     (1000) fzjan     (1000)        0 2024-05-03 18:23:27.795026 torchrun_jsc-0.0.3/src/torchrun_jsc/
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1199 2024-04-23 07:33:20.000000 torchrun_jsc-0.0.3/src/torchrun_jsc/__init__.py
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       58 2024-02-29 15:34:02.000000 torchrun_jsc-0.0.3/src/torchrun_jsc/__main__.py
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1551 2024-04-23 06:36:45.000000 torchrun_jsc-0.0.3/src/torchrun_jsc/arg_patching.py
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1078 2024-02-29 17:05:15.000000 torchrun_jsc-0.0.3/src/torchrun_jsc/parsing.py
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1494 2024-04-23 07:29:09.000000 torchrun_jsc-0.0.3/src/torchrun_jsc/run.py
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)     1763 2024-04-23 06:56:48.000000 torchrun_jsc-0.0.3/src/torchrun_jsc/run_old.py
+drwxrwxr-x   0 fzjan     (1000) fzjan     (1000)        0 2024-05-03 18:23:27.795026 torchrun_jsc-0.0.3/src/torchrun_jsc.egg-info/
+-rw-r--r--   0 fzjan     (1000) fzjan     (1000)      520 2024-05-03 18:23:27.000000 torchrun_jsc-0.0.3/src/torchrun_jsc.egg-info/PKG-INFO
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)      454 2024-05-03 18:23:27.000000 torchrun_jsc-0.0.3/src/torchrun_jsc.egg-info/SOURCES.txt
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)        1 2024-05-03 18:23:27.000000 torchrun_jsc-0.0.3/src/torchrun_jsc.egg-info/dependency_links.txt
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       55 2024-05-03 18:23:27.000000 torchrun_jsc-0.0.3/src/torchrun_jsc.egg-info/entry_points.txt
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       21 2024-05-03 18:23:27.000000 torchrun_jsc-0.0.3/src/torchrun_jsc.egg-info/requires.txt
+-rw-rw-r--   0 fzjan     (1000) fzjan     (1000)       13 2024-05-03 18:23:27.000000 torchrun_jsc-0.0.3/src/torchrun_jsc.egg-info/top_level.txt
```

### Comparing `torchrun_jsc-0.0.2/LICENSE` & `torchrun_jsc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchrun_jsc-0.0.2/PKG-INFO` & `torchrun_jsc-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchrun_jsc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fixed version of `torchrun` on Jülich Supercomputing Centre. Requires Slurm usage.
 Home-page: https://github.com/HelmholtzAI-FZJ/torchrun_jsc
 Author: Jan Ebert
 Author-email: ja.ebert@fz-juelich.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `torchrun_jsc-0.0.2/README.md` & `torchrun_jsc-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,14 @@
 `--rdzv_conf` argument's `is_host` configuration so that the correct
 process is recognized as the host process for setting up the
 communication server.
 
 After that, depending on your PyTorch version, there are various modes
 of functionality to achieve that the correct address is used for
 rendezvousing:
-1. PyTorch ≥3: Patch the `--local_addr` argument and emit a warning.
-2. PyTorch ≥2: Patch the `--local_addr` argument.
-3. PyTorch ≥1.9 <2: Monkey-patch the function used to obtain the
+1. PyTorch ≥3: Monkey-patch the function used to obtain the rendezvous
+   hostname and emit a warning.
+3. PyTorch ≥1.9 <3: Monkey-patch the function used to obtain the
    rendezvous hostname.
 4. PyTorch <1.9: If this package is somehow installed for a
    non-matching PyTorch version, it will error out because the
    `torchrun` API does not exist in these versions.
```

### Comparing `torchrun_jsc-0.0.2/setup.py` & `torchrun_jsc-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='torchrun_jsc',
     python_requires='>=3.6,<4',
-    version='0.0.2',
+    version='0.0.3',
     install_requires=[
         'packaging',
         # PyTorch 1.9 introduced the `torchrun` API.
         #
         # Since that version is already quite old in the fast-moving
         # field of deep learning and this package is concerned only with
         # fixing `torchrun` issues, we do not support earlier versions
```

### Comparing `torchrun_jsc-0.0.2/src/torchrun_jsc/__init__.py` & `torchrun_jsc-0.0.3/src/torchrun_jsc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,19 +30,19 @@
     if torch_ver.major >= 2:
         if torch_ver.major > 2:
             print(
                 'WARNING: This version of PyTorch is not officially supported '
                 'by `torchrun_jsc`. You may be able to ignore this warning.'
             )
 
-        from .run import main as run_main
-        run_main()
-    elif torch_ver.major < 1 or torch_ver.major == 1 and torch_ver.minor < 9:
+        from .run_old import main as run_main_old
+        run_main_old()
+    elif torch_ver.major == 1 and torch_ver.minor >= 9:
+        from .run_old import main as run_main_old
+        run_main_old()
+    else:
         print(
             'This version of PyTorch is not supported by `torchrun_jsc` '
             'because it does not have the `torchrun` API implemented. '
             'Please use another launch API.'
         )
         exit(1)
-    else:
-        from .run_old import main as run_main_old
-        run_main_old()
```

### Comparing `torchrun_jsc-0.0.2/src/torchrun_jsc/arg_patching.py` & `torchrun_jsc-0.0.3/src/torchrun_jsc/arg_patching.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Common patching routines for `torchrun` arguments.
 """
 
 import os
 import sys
 
 
-def fix_is_host(is_host, conf, is_host_envvar):
+def fix_is_host(is_host, conf):
     if is_host is None:
-        slurm_is_host = int(os.getenv(is_host_envvar, '0') == '0')
+        slurm_is_host = int(os.getenv('SLURM_NODEID', '0') == '0')
 
         if not conf:
             insertion_index = min(len(sys.argv), 1)
             sys.argv.insert(insertion_index, '--rdzv_conf=')
 
         # Since `torchrun` only uses standard `argparse` for
         # parsing, we do not need to worry about discerning multiple
```

### Comparing `torchrun_jsc-0.0.2/src/torchrun_jsc/parsing.py` & `torchrun_jsc-0.0.3/src/torchrun_jsc/parsing.py`

 * *Files identical despite different names*

### Comparing `torchrun_jsc-0.0.2/src/torchrun_jsc/run.py` & `torchrun_jsc-0.0.3/src/torchrun_jsc/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """
+WARNING: Currently broken, do not use. Leads to indeterministic
+deadlocks.
+
 Fixed version of `torchrun` on Jülich Supercomputing Centre for PyTorch
 versions ≥2. Requires Slurm usage.
 
 To use, modify your execution like the following:
 
 Old
 ```shell
@@ -50,13 +53,13 @@
         insertion_index = min(len(sys.argv), 1)
         sys.argv.insert(insertion_index, f'--local_addr={host}')
 
 
 def main():
     host, conf, is_host, local_addr = parse_args()
     fix_get_hostname(host, local_addr)
-    arg_patching.fix_is_host(is_host, conf, 'SLURM_PROCID')
+    arg_patching.fix_is_host(is_host, conf)
     runpy.run_module('torch.distributed.run', run_name='__main__')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `torchrun_jsc-0.0.2/src/torchrun_jsc/run_old.py` & `torchrun_jsc-0.0.3/src/torchrun_jsc/run_old.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 New
 ```shell
 python /path/to/torchrun_jsc/run_old.py [...]
 # or if `torchrun_jsc` is on `PYTHONPATH`
 python -m torchrun_jsc.run_old [...]
 ```
+
+Tested for PyTorch <2, 2.1.2
 """
 
 from argparse import ArgumentParser
 import ipaddress
 import runpy
 import socket
 
@@ -65,14 +67,14 @@
         new_get_fq_hostname = _orig_get_fq_hostname
 
     sapi._get_fq_hostname = new_get_fq_hostname
 
 
 def main():
     host, conf, is_host = parse_args()
-    arg_patching.fix_is_host(is_host, conf, 'SLURM_NODEID')
+    arg_patching.fix_is_host(is_host, conf)
     fix_torch_run(host)
     runpy.run_module('torch.distributed.run', run_name='__main__')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `torchrun_jsc-0.0.2/src/torchrun_jsc.egg-info/PKG-INFO` & `torchrun_jsc-0.0.3/src/torchrun_jsc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchrun_jsc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fixed version of `torchrun` on Jülich Supercomputing Centre. Requires Slurm usage.
 Home-page: https://github.com/HelmholtzAI-FZJ/torchrun_jsc
 Author: Jan Ebert
 Author-email: ja.ebert@fz-juelich.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```


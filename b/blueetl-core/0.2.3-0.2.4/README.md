# Comparing `tmp/blueetl-core-0.2.3.tar.gz` & `tmp/blueetl_core-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueetl-core-0.2.3.tar", last modified: Thu Apr 11 16:09:46 2024, max compression
+gzip compressed data, was "blueetl_core-0.2.4.tar", last modified: Fri May  3 11:01:21 2024, max compression
```

## Comparing `blueetl-core-0.2.3.tar` & `blueetl_core-0.2.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.567743 blueetl-core-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.555743 blueetl-core-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.559743 blueetl-core-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-11 16:09:46.563743 blueetl-core-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.559743 blueetl-core-0.2.3/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.559743 blueetl-core-0.2.3/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.559743 blueetl-core-0.2.3/doc/source/_images/
--rw-r--r--   0 runner    (1001) docker     (127)   186341 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/source/_images/BlueETL.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:09:46.567743 blueetl-core-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.555743 blueetl-core-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.563743 blueetl-core-0.2.3/src/blueetl_core/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/etl.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    17484 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.563743 blueetl-core-0.2.3/src/blueetl_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.563743 blueetl-core-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17938 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_etl_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_etl_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_etl_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    19985 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:21.067389 blueetl_core-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:21.055389 blueetl_core-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:21.059389 blueetl_core-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-03 11:01:21.067389 blueetl_core-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:21.059389 blueetl_core-0.2.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:21.059389 blueetl_core-0.2.4/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:21.059389 blueetl_core-0.2.4/doc/source/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)   186341 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/doc/source/_images/BlueETL.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:01:21.067389 blueetl_core-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:21.059389 blueetl_core-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:21.063389 blueetl_core-0.2.4/src/blueetl_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/src/blueetl_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 11:01:20.000000 blueetl_core-0.2.4/src/blueetl_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/src/blueetl_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/src/blueetl_core/etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/src/blueetl_core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/src/blueetl_core/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17484 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/src/blueetl_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:21.063389 blueetl_core-0.2.4/src/blueetl_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-03 11:01:21.000000 blueetl_core-0.2.4/src/blueetl_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-03 11:01:21.000000 blueetl_core-0.2.4/src/blueetl_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:01:21.000000 blueetl_core-0.2.4/src/blueetl_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 11:01:21.000000 blueetl_core-0.2.4/src/blueetl_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 11:01:21.000000 blueetl_core-0.2.4/src/blueetl_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:21.063389 blueetl_core-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17938 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/tests/test_etl_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/tests/test_etl_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/tests/test_etl_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19985 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-03 11:01:11.000000 blueetl_core-0.2.4/tox.ini
```

### Comparing `blueetl-core-0.2.3/.github/workflows/publish-sdist.yml` & `blueetl_core-0.2.4/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/.github/workflows/run-tox.yml` & `blueetl_core-0.2.4/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/CHANGELOG.rst` & `blueetl_core-0.2.4/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+Version 0.2.4
+-------------
+
+Bug fixes
+~~~~~~~~~
+
+- Do not call ``get_reusable_executor().shutdown()`` when tasks are run serially in ``run_parallel()``.
+
 Version 0.2.3
 -------------
 
 Improvements
 ~~~~~~~~~~~~
 
 - In ``blueetl_core.utils.is_subfilter()``, add the ``strict`` parameter.
```

### Comparing `blueetl-core-0.2.3/LICENSE.txt` & `blueetl_core-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/PKG-INFO` & `blueetl_core-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueetl-core
-Version: 0.2.3
+Version: 0.2.4
 Summary: Core transformations for BlueETL
 Author: Blue Brain Project, EPFL
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/BlueBrain/blueetl-core
 Project-URL: Repository, https://github.com/BlueBrain/blueetl-core.git
 Project-URL: Documentation, https://blueetl-core.readthedocs.io/
 Project-URL: Tracker, https://github.com/BlueBrain/blueetl-core/issues
```

### Comparing `blueetl-core-0.2.3/README.rst` & `blueetl_core-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/doc/Makefile` & `blueetl_core-0.2.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/doc/source/_images/BlueETL.jpeg` & `blueetl_core-0.2.4/doc/source/_images/BlueETL.jpeg`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/doc/source/conf.py` & `blueetl_core-0.2.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/pyproject.toml` & `blueetl_core-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/src/blueetl_core/constants.py` & `blueetl_core-0.2.4/src/blueetl_core/constants.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/src/blueetl_core/etl.py` & `blueetl_core-0.2.4/src/blueetl_core/etl.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/src/blueetl_core/parallel.py` & `blueetl_core-0.2.4/src/blueetl_core/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                     seed=None if base_seed is None else base_seed + i,
                     ppid=os.getpid(),
                 )
             )
             for i, task in enumerate(tasks)
         )
     finally:
-        if shutdown_executor and (not backend or backend == "loky"):
+        if shutdown_executor and (not backend or backend == "loky") and jobs != 1:
             # shutdown the pool of processes used by loky
             get_reusable_executor().shutdown(wait=True)
 
 
 def isolated(func):
     """Isolate a function to be executed in a separate process.
```

### Comparing `blueetl-core-0.2.3/src/blueetl_core/utils.py` & `blueetl_core-0.2.4/src/blueetl_core/utils.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/src/blueetl_core.egg-info/PKG-INFO` & `blueetl_core-0.2.4/src/blueetl_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueetl-core
-Version: 0.2.3
+Version: 0.2.4
 Summary: Core transformations for BlueETL
 Author: Blue Brain Project, EPFL
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/BlueBrain/blueetl-core
 Project-URL: Repository, https://github.com/BlueBrain/blueetl-core.git
 Project-URL: Documentation, https://blueetl-core.readthedocs.io/
 Project-URL: Tracker, https://github.com/BlueBrain/blueetl-core/issues
```

### Comparing `blueetl-core-0.2.3/src/blueetl_core.egg-info/SOURCES.txt` & `blueetl_core-0.2.4/src/blueetl_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/tests/conftest.py` & `blueetl_core-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/tests/test_etl_dataframe.py` & `blueetl_core-0.2.4/tests/test_etl_dataframe.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/tests/test_etl_index.py` & `blueetl_core-0.2.4/tests/test_etl_index.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/tests/test_etl_series.py` & `blueetl_core-0.2.4/tests/test_etl_series.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/tests/test_parallel.py` & `blueetl_core-0.2.4/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/tests/test_utils.py` & `blueetl_core-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.3/tox.ini` & `blueetl_core-0.2.4/tox.ini`

 * *Files identical despite different names*


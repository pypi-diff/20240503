# Comparing `tmp/botocore-a-la-carte-forecast-1.34.96.tar.gz` & `tmp/botocore-a-la-carte-forecast-1.34.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-forecast-1.34.96.tar", last modified: Thu May  2 01:01:26 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-forecast-1.34.97.tar", last modified: Fri May  3 01:04:44 2024, max compression
```

## Comparing `botocore-a-la-carte-forecast-1.34.96.tar` & `botocore-a-la-carte-forecast-1.34.97.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:26.761082 botocore-a-la-carte-forecast-1.34.96/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-02 01:01:26.000000 botocore-a-la-carte-forecast-1.34.96/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-02 01:01:26.761082 botocore-a-la-carte-forecast-1.34.96/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:26.761082 botocore-a-la-carte-forecast-1.34.96/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:26.761082 botocore-a-la-carte-forecast-1.34.96/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:26.761082 botocore-a-la-carte-forecast-1.34.96/botocore/data/forecast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:26.761082 botocore-a-la-carte-forecast-1.34.96/botocore/data/forecast/2018-06-26/
--rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-05-02 01:01:05.000000 botocore-a-la-carte-forecast-1.34.96/botocore/data/forecast/2018-06-26/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 01:01:05.000000 botocore-a-la-carte-forecast-1.34.96/botocore/data/forecast/2018-06-26/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-02 01:01:05.000000 botocore-a-la-carte-forecast-1.34.96/botocore/data/forecast/2018-06-26/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   310389 2024-05-02 01:01:05.000000 botocore-a-la-carte-forecast-1.34.96/botocore/data/forecast/2018-06-26/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:26.761082 botocore-a-la-carte-forecast-1.34.96/botocore_a_la_carte_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-02 01:01:26.000000 botocore-a-la-carte-forecast-1.34.96/botocore_a_la_carte_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-02 01:01:26.000000 botocore-a-la-carte-forecast-1.34.96/botocore_a_la_carte_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:01:26.000000 botocore-a-la-carte-forecast-1.34.96/botocore_a_la_carte_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 01:01:26.000000 botocore-a-la-carte-forecast-1.34.96/botocore_a_la_carte_forecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:01:26.761082 botocore-a-la-carte-forecast-1.34.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-02 01:01:26.000000 botocore-a-la-carte-forecast-1.34.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:04:44.811524 botocore-a-la-carte-forecast-1.34.97/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-03 01:04:44.000000 botocore-a-la-carte-forecast-1.34.97/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 01:04:44.811524 botocore-a-la-carte-forecast-1.34.97/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:04:44.811524 botocore-a-la-carte-forecast-1.34.97/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:04:44.811524 botocore-a-la-carte-forecast-1.34.97/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:04:44.811524 botocore-a-la-carte-forecast-1.34.97/botocore/data/forecast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:04:44.811524 botocore-a-la-carte-forecast-1.34.97/botocore/data/forecast/2018-06-26/
+-rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-05-03 01:04:25.000000 botocore-a-la-carte-forecast-1.34.97/botocore/data/forecast/2018-06-26/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 01:04:25.000000 botocore-a-la-carte-forecast-1.34.97/botocore/data/forecast/2018-06-26/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-03 01:04:25.000000 botocore-a-la-carte-forecast-1.34.97/botocore/data/forecast/2018-06-26/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   310389 2024-05-03 01:04:25.000000 botocore-a-la-carte-forecast-1.34.97/botocore/data/forecast/2018-06-26/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:04:44.811524 botocore-a-la-carte-forecast-1.34.97/botocore_a_la_carte_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 01:04:44.000000 botocore-a-la-carte-forecast-1.34.97/botocore_a_la_carte_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-03 01:04:44.000000 botocore-a-la-carte-forecast-1.34.97/botocore_a_la_carte_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:04:44.000000 botocore-a-la-carte-forecast-1.34.97/botocore_a_la_carte_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 01:04:44.000000 botocore-a-la-carte-forecast-1.34.97/botocore_a_la_carte_forecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 01:04:44.811524 botocore-a-la-carte-forecast-1.34.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-03 01:04:44.000000 botocore-a-la-carte-forecast-1.34.97/setup.py
```

### Comparing `botocore-a-la-carte-forecast-1.34.96/LICENSE.txt` & `botocore-a-la-carte-forecast-1.34.97/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-forecast-1.34.96/PKG-INFO` & `botocore-a-la-carte-forecast-1.34.97/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-forecast
-Version: 1.34.96
+Version: 1.34.97
 Summary: forecast data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-forecast-1.34.96/botocore/data/forecast/2018-06-26/endpoint-rule-set-1.json` & `botocore-a-la-carte-forecast-1.34.97/botocore/data/forecast/2018-06-26/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-forecast-1.34.96/botocore/data/forecast/2018-06-26/paginators-1.json` & `botocore-a-la-carte-forecast-1.34.97/botocore/data/forecast/2018-06-26/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-forecast-1.34.96/botocore/data/forecast/2018-06-26/service-2.json` & `botocore-a-la-carte-forecast-1.34.97/botocore/data/forecast/2018-06-26/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-forecast-1.34.96/botocore_a_la_carte_forecast.egg-info/PKG-INFO` & `botocore-a-la-carte-forecast-1.34.97/botocore_a_la_carte_forecast.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-forecast
-Version: 1.34.96
+Version: 1.34.97
 Summary: forecast data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-forecast-1.34.96/setup.py` & `botocore-a-la-carte-forecast-1.34.97/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-forecast',
-    version="1.34.96",
+    version="1.34.97",
     description='forecast data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/forecast/*/*.json'],
```


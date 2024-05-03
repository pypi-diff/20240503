# Comparing `tmp/flightplotting-0.2.4.tar.gz` & `tmp/flightplotting-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightplotting-0.2.4.tar", last modified: Wed May  1 09:02:29 2024, max compression
+gzip compressed data, was "flightplotting-0.2.5.tar", last modified: Fri May  3 08:19:43 2024, max compression
```

## Comparing `flightplotting-0.2.4.tar` & `flightplotting-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:02:29.066512 flightplotting-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-01 09:01:47.000000 flightplotting-0.2.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 09:01:47.000000 flightplotting-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-01 09:02:29.066512 flightplotting-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-01 09:01:47.000000 flightplotting-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:02:29.062512 flightplotting-0.2.4/flightplotting/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:02:29.066512 flightplotting-0.2.4/flightplotting/data/
--rw-r--r--   0 runner    (1001) docker     (127)   142015 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/data/ColdDraftF3APlane.obj
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/titlerenderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/traces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:02:29.066512 flightplotting-0.2.4/flightplotting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-01 09:02:29.000000 flightplotting-0.2.4/flightplotting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-01 09:02:29.000000 flightplotting-0.2.4/flightplotting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:02:29.000000 flightplotting-0.2.4/flightplotting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 09:02:29.000000 flightplotting-0.2.4/flightplotting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 09:02:29.000000 flightplotting-0.2.4/flightplotting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-01 09:02:29.066512 flightplotting-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-01 09:01:47.000000 flightplotting-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:02:29.066512 flightplotting-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-01 09:01:47.000000 flightplotting-0.2.4/tests/test_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:43.366389 flightplotting-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:43.338389 flightplotting-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:43.342389 flightplotting-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-03 08:19:09.000000 flightplotting-0.2.5/.github/workflows/publish_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-03 08:19:09.000000 flightplotting-0.2.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:43.342389 flightplotting-0.2.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 08:19:09.000000 flightplotting-0.2.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-03 08:19:09.000000 flightplotting-0.2.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 08:19:09.000000 flightplotting-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-03 08:19:43.366389 flightplotting-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 08:19:09.000000 flightplotting-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:43.342389 flightplotting-0.2.5/flightplotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-03 08:19:09.000000 flightplotting-0.2.5/flightplotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:43.342389 flightplotting-0.2.5/flightplotting/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   142015 2024-05-03 08:19:09.000000 flightplotting-0.2.5/flightplotting/data/ColdDraftF3APlane.obj
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:09.000000 flightplotting-0.2.5/flightplotting/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-03 08:19:09.000000 flightplotting-0.2.5/flightplotting/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-03 08:19:09.000000 flightplotting-0.2.5/flightplotting/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-03 08:19:09.000000 flightplotting-0.2.5/flightplotting/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-03 08:19:09.000000 flightplotting-0.2.5/flightplotting/titlerenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-03 08:19:09.000000 flightplotting-0.2.5/flightplotting/traces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:43.366389 flightplotting-0.2.5/flightplotting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-03 08:19:43.000000 flightplotting-0.2.5/flightplotting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 08:19:43.000000 flightplotting-0.2.5/flightplotting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 08:19:43.000000 flightplotting-0.2.5/flightplotting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 08:19:43.000000 flightplotting-0.2.5/flightplotting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 08:19:43.000000 flightplotting-0.2.5/flightplotting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-03 08:19:09.000000 flightplotting-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 08:19:09.000000 flightplotting-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 08:19:43.370389 flightplotting-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:43.342389 flightplotting-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:09.000000 flightplotting-0.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:43.346389 flightplotting-0.2.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 08:19:09.000000 flightplotting-0.2.5/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127) 19266131 2024-05-03 08:19:10.000000 flightplotting-0.2.5/tests/data/p23_flight.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-03 08:19:10.000000 flightplotting-0.2.5/tests/test_plots.py
```

### Comparing `flightplotting-0.2.4/COPYING` & `flightplotting-0.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.4/PKG-INFO` & `flightplotting-0.2.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Metadata-Version: 2.1
 Name: flightplotting
-Version: 0.2.4
+Version: 0.2.5
 Summary: Tools for Plotting Flight Data in Plotly
-Home-page: https://github.com/PyFlightCoach/FlightPlotting
-Author: Thomas David
-Author-email: thomasdavid0@gmail.com
+Author-email: Thomas David <thomasdavid0@gmail.com>
+License: GNU GPL v3
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: pfc-geometry>=0.2.4
 Requires-Dist: flightdata>=0.2.6
 Requires-Dist: flightanalysis>=0.2.6
 
 # FlightPlotting
 
 
 This module contains utilities for plotting flight data using plotly
+
+
+```bash
+pip install flightplotting
+```
+
+```bash
+pip install -e .
+```
```

### Comparing `flightplotting-0.2.4/flightplotting/data/ColdDraftF3APlane.obj` & `flightplotting-0.2.5/flightplotting/data/ColdDraftF3APlane.obj`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.4/flightplotting/model.py` & `flightplotting-0.2.5/flightplotting/model.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.4/flightplotting/plots.py` & `flightplotting-0.2.5/flightplotting/plots.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.4/flightplotting/templates.py` & `flightplotting-0.2.5/flightplotting/templates.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.4/flightplotting/titlerenderer.py` & `flightplotting-0.2.5/flightplotting/titlerenderer.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.4/flightplotting/traces.py` & `flightplotting-0.2.5/flightplotting/traces.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.4/flightplotting.egg-info/PKG-INFO` & `flightplotting-0.2.5/flightplotting.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Metadata-Version: 2.1
 Name: flightplotting
-Version: 0.2.4
+Version: 0.2.5
 Summary: Tools for Plotting Flight Data in Plotly
-Home-page: https://github.com/PyFlightCoach/FlightPlotting
-Author: Thomas David
-Author-email: thomasdavid0@gmail.com
+Author-email: Thomas David <thomasdavid0@gmail.com>
+License: GNU GPL v3
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: pfc-geometry>=0.2.4
 Requires-Dist: flightdata>=0.2.6
 Requires-Dist: flightanalysis>=0.2.6
 
 # FlightPlotting
 
 
 This module contains utilities for plotting flight data using plotly
+
+
+```bash
+pip install flightplotting
+```
+
+```bash
+pip install -e .
+```
```


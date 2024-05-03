# Comparing `tmp/pytribs-0.2.0.tar.gz` & `tmp/pytribs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytribs-0.2.0.tar", last modified: Thu Apr 25 20:54:56 2024, max compression
+gzip compressed data, was "pytribs-0.3.0.tar", last modified: Fri May  3 18:10:52 2024, max compression
```

## Comparing `pytribs-0.2.0.tar` & `pytribs-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.300489 pytribs-0.2.0/
--rw-r--r--   0 lraming    (503) staff       (20)    18005 2024-03-30 00:40:45.000000 pytribs-0.2.0/LICENSE
--rw-r--r--   0 lraming    (503) staff       (20)     1835 2024-04-25 20:54:56.300253 pytribs-0.2.0/PKG-INFO
--rw-r--r--   0 lraming    (503) staff       (20)     1138 2024-04-25 20:49:07.000000 pytribs-0.2.0/README.md
--rw-r--r--   0 lraming    (503) staff       (20)      760 2024-04-25 20:54:50.000000 pytribs-0.2.0/pyproject.toml
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.294355 pytribs-0.2.0/pytRIBS/
--rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/__init__.py
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.295531 pytribs-0.2.0/pytRIBS/aux/
--rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/aux/__init__.py
--rw-r--r--   0 lraming    (503) staff       (20)    16128 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/aux/tol_colors.py
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.296360 pytribs-0.2.0/pytRIBS/mixins/
--rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/mixins/__init__.py
--rw-r--r--   0 lraming    (503) staff       (20)    29738 2024-04-08 22:28:13.000000 pytribs-0.2.0/pytRIBS/mixins/infile_mixin.py
--rw-r--r--   0 lraming    (503) staff       (20)    20162 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/mixins/shared_mixin.py
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.297870 pytribs-0.2.0/pytRIBS/model/
--rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/model/__init__.py
--rw-r--r--   0 lraming    (503) staff       (20)     7059 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/model/aux.py
--rw-r--r--   0 lraming    (503) staff       (20)     5522 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/model/diagnose.py
--rw-r--r--   0 lraming    (503) staff       (20)    29398 2024-04-24 23:54:17.000000 pytribs-0.2.0/pytRIBS/model/inout.py
--rw-r--r--   0 lraming    (503) staff       (20)    28724 2024-04-24 23:27:57.000000 pytribs-0.2.0/pytRIBS/model/preprocess.py
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.298684 pytribs-0.2.0/pytRIBS/results/
--rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/results/__init__.py
--rw-r--r--   0 lraming    (503) staff       (20)        3 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/results/post.py
--rw-r--r--   0 lraming    (503) staff       (20)    12450 2024-04-24 23:27:57.000000 pytribs-0.2.0/pytRIBS/results/waterbalance.py
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.299292 pytribs-0.2.0/pytRIBS/scratch/
--rw-r--r--   0 lraming    (503) staff       (20)       98 2024-04-24 23:29:13.000000 pytribs-0.2.0/pytRIBS/scratch/debug.py
--rw-r--r--   0 lraming    (503) staff       (20)     2467 2024-04-08 21:51:37.000000 pytribs-0.2.0/pytRIBS/scratch/print_input_template.py
--rw-r--r--   0 lraming    (503) staff       (20)     2511 2024-04-25 19:08:01.000000 pytribs-0.2.0/pytRIBS/tmodel.py
--rw-r--r--   0 lraming    (503) staff       (20)    12970 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/tresults.py
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.299950 pytribs-0.2.0/pytRIBS.egg-info/
--rw-r--r--   0 lraming    (503) staff       (20)     1835 2024-04-25 20:54:56.000000 pytribs-0.2.0/pytRIBS.egg-info/PKG-INFO
--rw-r--r--   0 lraming    (503) staff       (20)      656 2024-04-25 20:54:56.000000 pytribs-0.2.0/pytRIBS.egg-info/SOURCES.txt
--rw-r--r--   0 lraming    (503) staff       (20)        1 2024-04-25 20:54:56.000000 pytribs-0.2.0/pytRIBS.egg-info/dependency_links.txt
--rw-r--r--   0 lraming    (503) staff       (20)       97 2024-04-25 20:54:56.000000 pytribs-0.2.0/pytRIBS.egg-info/requires.txt
--rw-r--r--   0 lraming    (503) staff       (20)        8 2024-04-25 20:54:56.000000 pytribs-0.2.0/pytRIBS.egg-info/top_level.txt
--rw-r--r--   0 lraming    (503) staff       (20)       38 2024-04-25 20:54:56.300539 pytribs-0.2.0/setup.cfg
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-05-03 18:10:52.401128 pytribs-0.3.0/
+-rw-r--r--   0 lraming    (503) staff       (20)    18005 2024-03-30 00:40:45.000000 pytribs-0.3.0/LICENSE
+-rw-r--r--   0 lraming    (503) staff       (20)     2238 2024-05-03 18:10:52.400860 pytribs-0.3.0/PKG-INFO
+-rw-r--r--   0 lraming    (503) staff       (20)     1541 2024-05-03 18:08:49.000000 pytribs-0.3.0/README.md
+-rw-r--r--   0 lraming    (503) staff       (20)      760 2024-05-03 18:10:23.000000 pytribs-0.3.0/pyproject.toml
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-05-03 18:10:52.395543 pytribs-0.3.0/pytRIBS/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.3.0/pytRIBS/__init__.py
+-rw-r--r--   0 lraming    (503) staff       (20)     6189 2024-05-02 22:40:07.000000 pytribs-0.3.0/pytRIBS/classes.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-05-03 18:10:52.396454 pytribs-0.3.0/pytRIBS/land/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-04-25 21:09:14.000000 pytribs-0.3.0/pytRIBS/land/__init__.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-05-03 18:10:52.396584 pytribs-0.3.0/pytRIBS/mesh/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-04-25 21:09:01.000000 pytribs-0.3.0/pytRIBS/mesh/__init__.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-05-03 18:10:52.396711 pytribs-0.3.0/pytRIBS/met/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-04-25 21:10:32.000000 pytribs-0.3.0/pytRIBS/met/__init__.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-05-03 18:10:52.397368 pytribs-0.3.0/pytRIBS/model/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.3.0/pytRIBS/model/__init__.py
+-rw-r--r--   0 lraming    (503) staff       (20)     5522 2024-03-30 00:40:45.000000 pytribs-0.3.0/pytRIBS/model/diagnose.py
+-rw-r--r--   0 lraming    (503) staff       (20)     8507 2024-04-30 19:06:42.000000 pytribs-0.3.0/pytRIBS/model/preprocess.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-05-03 18:10:52.398157 pytribs-0.3.0/pytRIBS/results/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.3.0/pytRIBS/results/__init__.py
+-rw-r--r--   0 lraming    (503) staff       (20)     6075 2024-04-25 22:18:27.000000 pytribs-0.3.0/pytRIBS/results/read.py
+-rw-r--r--   0 lraming    (503) staff       (20)     5815 2024-04-25 22:28:19.000000 pytribs-0.3.0/pytRIBS/results/visualize.py
+-rw-r--r--   0 lraming    (503) staff       (20)    12450 2024-04-24 23:27:57.000000 pytribs-0.3.0/pytRIBS/results/waterbalance.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-05-03 18:10:52.399095 pytribs-0.3.0/pytRIBS/shared/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.3.0/pytRIBS/shared/__init__.py
+-rw-r--r--   0 lraming    (503) staff       (20)     8347 2024-04-30 19:06:42.000000 pytribs-0.3.0/pytRIBS/shared/aux.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-05-03 18:10:52.399402 pytribs-0.3.0/pytRIBS/shared/color/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-04-30 19:06:42.000000 pytribs-0.3.0/pytRIBS/shared/color/__init__.py
+-rw-r--r--   0 lraming    (503) staff       (20)    16128 2024-04-30 19:06:42.000000 pytribs-0.3.0/pytRIBS/shared/color/tol_colors.py
+-rw-r--r--   0 lraming    (503) staff       (20)    29625 2024-05-02 21:41:05.000000 pytribs-0.3.0/pytRIBS/shared/infile_mixin.py
+-rw-r--r--   0 lraming    (503) staff       (20)    26693 2024-04-30 19:06:42.000000 pytribs-0.3.0/pytRIBS/shared/inout.py
+-rw-r--r--   0 lraming    (503) staff       (20)    20391 2024-05-02 22:40:07.000000 pytribs-0.3.0/pytRIBS/shared/shared_mixin.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-05-03 18:10:52.399739 pytribs-0.3.0/pytRIBS/soil/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-04-25 21:08:38.000000 pytribs-0.3.0/pytRIBS/soil/__init__.py
+-rw-r--r--   0 lraming    (503) staff       (20)    24974 2024-05-02 22:40:07.000000 pytribs-0.3.0/pytRIBS/soil/soil.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-05-03 18:10:52.400577 pytribs-0.3.0/pytRIBS.egg-info/
+-rw-r--r--   0 lraming    (503) staff       (20)     2238 2024-05-03 18:10:52.000000 pytribs-0.3.0/pytRIBS.egg-info/PKG-INFO
+-rw-r--r--   0 lraming    (503) staff       (20)      741 2024-05-03 18:10:52.000000 pytribs-0.3.0/pytRIBS.egg-info/SOURCES.txt
+-rw-r--r--   0 lraming    (503) staff       (20)        1 2024-05-03 18:10:52.000000 pytribs-0.3.0/pytRIBS.egg-info/dependency_links.txt
+-rw-r--r--   0 lraming    (503) staff       (20)       97 2024-05-03 18:10:52.000000 pytribs-0.3.0/pytRIBS.egg-info/requires.txt
+-rw-r--r--   0 lraming    (503) staff       (20)        8 2024-05-03 18:10:52.000000 pytribs-0.3.0/pytRIBS.egg-info/top_level.txt
+-rw-r--r--   0 lraming    (503) staff       (20)       38 2024-05-03 18:10:52.401185 pytribs-0.3.0/setup.cfg
```

### Comparing `pytribs-0.2.0/LICENSE` & `pytribs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytribs-0.2.0/PKG-INFO` & `pytribs-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytRIBS
-Version: 0.2.0
+Version: 0.3.0
 Summary: A pre-to-post processing python package for the distributed hydrological model tRIBS
 Author-email: "L. Wren Raming" <lraming@asu.edu>, "C. Josh Cederstrom" <cjceders@asu.edu>, "Enrique R. Vivoni" <evivoni@asu.edu>
 License: GPL-version 2
 Project-URL: Repository, https://github.com/tribshms/pytRIBS
 Keywords: hydrology,modeling
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,14 +23,22 @@
 A pre-to-post processing python package designed to allow users to setup, simulate, and analyze TIN-based Real-time Integrated Basin Simulator (tRIBS) model runs through a python interface.
 Note this packages is currently under development and is subject to further changes. Additionally, much of the functionality here has had limited testing, consequently responsibility is on the user to verify package functionality. 
 
 ## Release/Version Notes
 PytRIBS uses semantic versioning. Currently, we are in the initial development phase--anything MAY change at any time and
 this package SHOULD NOT be considered stable.
 
+### Version 0.3.0 (5/03/2024)
+* Removed tmodel/tresults, replaced with classes
+* added new classes Soil, Mesh, Met, Land
+* renamed mixins folder to shared
+* created results/visualize.py
+* created soil/soil.py --moved soil related content from preprocess to here.
+* updated create_soil_map to return a soil table in .sdt format.
+* updated read/write soil tables to include options for including texture.
 ### Version 0.2.0 (4/25/2024)
 This minor update includes:
 * updates to the infile_mixin, with updates for 
 model documentation
 * addition of Paul Tol's colormaps (https://personal.sron.nl/~pault/)
 * In shared mixin:
   * added processor # to the attribute voronoi
```

### Comparing `pytribs-0.2.0/pyproject.toml` & `pytribs-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,11 +19,11 @@
     "shapely",
     "rasterio",
     "scipy",
     "rosetta-soil",
     "owslib",
     "matplotlib_scalebar"
 ]
-version = "0.2.0"
+version = "0.3.0"
 
 [project.urls]
 Repository = "https://github.com/tribshms/pytRIBS"
```

### Comparing `pytribs-0.2.0/pytRIBS/aux/tol_colors.py` & `pytribs-0.3.0/pytRIBS/shared/color/tol_colors.py`

 * *Files identical despite different names*

### Comparing `pytribs-0.2.0/pytRIBS/mixins/infile_mixin.py` & `pytribs-0.3.0/pytRIBS/shared/infile_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,333 +30,333 @@
         """
         input_file = {
 
             # ==================================================================================================
             # TIME PARAMETERS
             # ==================================================================================================
 
-            "startdate": {"key_word": "STARTDATE:", "describe": "Starting time (MM/DD/YYYY/HH/MM)", "value": None,
+            "startdate": {"keyword": "STARTDATE:", "describe": "Starting time (MM/DD/YYYY/HH/MM)", "value": None,
                           "tags": ["time"]},
-            "runtime": {"key_word": "RUNTIME:", "describe": "Simulation length in hours", "value": None,
+            "runtime": {"keyword": "RUNTIME:", "describe": "Simulation length in hours", "value": None,
                         "tags": ["time"]},
-            "rainsearch": {"key_word": "RAINSEARCH:", "describe": "Rainfall search interval (hours)", "value": 24,
+            "rainsearch": {"keyword": "RAINSEARCH:", "describe": "Rainfall search interval (hours)", "value": 24,
                            "tags": ["time"]},
-            "timestep": {"key_word": "TIMESTEP:", "describe": "Unsaturated zone computational time step (mins)",
+            "timestep": {"keyword": "TIMESTEP:", "describe": "Unsaturated zone computational time step (mins)",
                          "value": 3.75, "tags": ["time"]},
-            "gwstep": {"key_word": "GWSTEP:", "describe": "Saturated zone computational time step (mins)",
+            "gwstep": {"keyword": "GWSTEP:", "describe": "Saturated zone computational time step (mins)",
                        "value": 30.0, "tags": ["time"]},
-            "metstep": {"key_word": "METSTEP:", "describe": "Meteorological data time step (mins)", "value": 60.0,
+            "metstep": {"keyword": "METSTEP:", "describe": "Meteorological data time step (mins)", "value": 60.0,
                         "tags": ["time"]},
-            "etistep": {"key_word": "ETISTEP:", "describe": "ET, interception and snow time step (hours)", "value": 1,
+            "etistep": {"keyword": "ETISTEP:", "describe": "ET, interception and snow time step (hours)", "value": 1,
                         "tags": ["time"]},
-            "rainintrvl": {"key_word": "RAININTRVL:", "describe": "Time interval in rainfall input (hours)",
+            "rainintrvl": {"keyword": "RAININTRVL:", "describe": "Time interval in rainfall input (hours)",
                            "value": 1, "tags": ["time"]},
-            "intstormmax": {"key_word": "INTSTORMMAX:", "describe": "Interstorm interval (hours)", "value": 10000,
+            "intstormmax": {"keyword": "INTSTORMMAX:", "describe": "Interstorm interval (hours)", "value": 10000,
                             "tags": ["time"]},
             # ==================================================================================================
             # MESH PARAMETERS
             # ==================================================================================================
-            "optmeshinput": {"key_word": "OPTMESHINPUT:", "describe": "Mesh input data option\n" + \
+            "optmeshinput": {"keyword": "OPTMESHINPUT:", "describe": "Mesh input data option\n" + \
                                                                       "1  tMesh data\n" + \
                                                                       "2  Point file\n" + \
                                                                       "3  ArcGrid (random)\n" + \
                                                                       "4  ArcGrid (hex)\n" + \
                                                                       "5  Arc/Info *.net\n" + \
                                                                       "6  Arc/Info *.lin,*.pnt\n" + \
                                                                       "7  Scratch\n" + \
                                                                       "8  Point Triangulator", "value": 8,
                              "tags": ["mesh"]},
-            "inputdatafile": {"key_word": "INPUTDATAFILE:", "describe": "tMesh input file base name for Mesh files",
+            "inputdatafile": {"keyword": "INPUTDATAFILE:", "describe": "tMesh input file base name for Mesh files",
                               "value": None, "tags": ["mesh"]},
-            "inputtime": {"key_word": "INPUTTIME:", "describe": "Deprecated, will be removed", "value": None, "tags": ["mesh"]},
-            "arcinfofilename": {"key_word": "ARCINFOFILENAME:", "describe": "tMesh input file base name Arc files",
+            "inputtime": {"keyword": "INPUTTIME:", "describe": "Deprecated, will be removed", "value": None, "tags": ["mesh"]},
+            "arcinfofilename": {"keyword": "ARCINFOFILENAME:", "describe": "tMesh input file base name Arc files",
                                 "value": None, "tags": ["mesh"]},
-            "pointfilename": {"key_word": "POINTFILENAME:", "describe": "tMesh input file name Points files",
+            "pointfilename": {"keyword": "POINTFILENAME:", "describe": "tMesh input file name Points files",
                               "value": None, "tags": ["mesh"]},
             # ==================================================================================================
             # ROUTING PARAMETERS
             # ==================================================================================================
 
-            "baseflow": {"key_word": "BASEFLOW:", "describe": "Baseflow discharge (m3/s)", "value": 0.2,
+            "baseflow": {"keyword": "BASEFLOW:", "describe": "Baseflow discharge (m3/s)", "value": 0.2,
                          "tags": ["flow"]},
-            "velocitycoef": {"key_word": "VELOCITYCOEF:", "describe": "Discharge-velocity coefficient", "value": 1.2,
+            "velocitycoef": {"keyword": "VELOCITYCOEF:", "describe": "Discharge-velocity coefficient", "value": 1.2,
                              "tags": ["flow"]},
-            "kinemvelcoef": {"key_word": "KINEMVELCOEF:", "describe": "Kinematic routing velocity coefficient",
+            "kinemvelcoef": {"keyword": "KINEMVELCOEF:", "describe": "Kinematic routing velocity coefficient",
                              "value": 3, "tags": ["flow"]},
-            "velocityratio": {"key_word": "VELOCITYRATIO:", "describe": "Stream to hillslope velocity coefficient",
+            "velocityratio": {"keyword": "VELOCITYRATIO:", "describe": "Stream to hillslope velocity coefficient",
                               "value": 60, "tags": ["flow"]},
-            "flowexp": {"key_word": "FLOWEXP:", "describe": "Nonlinear discharge coefficient", "value": 0.3,
+            "flowexp": {"keyword": "FLOWEXP:", "describe": "Nonlinear discharge coefficient", "value": 0.3,
                         "tags": ["flow"]},
-            "channelroughness": {"key_word": "CHANNELROUGHNESS:", "describe": "Uniform channel roughness value",
+            "channelroughness": {"keyword": "CHANNELROUGHNESS:", "describe": "Uniform channel roughness value",
                                  "value": 0.15, "tags": ["flow"]},
-            "channelwidth": {"key_word": "CHANNELWIDTH:", "describe": "Uniform channel width  (meters)", "value": 12,
+            "channelwidth": {"keyword": "CHANNELWIDTH:", "describe": "Uniform channel width  (meters)", "value": 12,
                              "tags": ["flow"]},
-            "channelwidthcoeff": {"key_word": "CHANNELWIDTHCOEFF:",
+            "channelwidthcoeff": {"keyword": "CHANNELWIDTHCOEFF:",
                                   "describe": "Coefficient in width-area relationship", "value": 2.33,
                                   "tags": ["flow"]},
-            "channelwidthexpnt": {"key_word": "CHANNELWIDTHEXPNT:", "describe": "Exponent in width-area relationship",
+            "channelwidthexpnt": {"keyword": "CHANNELWIDTHEXPNT:", "describe": "Exponent in width-area relationship",
                                   "value": 0.54, "tags": ["flow"]},
-            "channelwidthfile": {"key_word": "CHANNELWIDTHFILE:", "describe": "Filename that contains channel widths",
+            "channelwidthfile": {"keyword": "CHANNELWIDTHFILE:", "describe": "Filename that contains channel widths",
                                  "value": None, "tags": ["flow"]},
-            "widthinterpolation": {"key_word": "WIDTHINTERPOLATION:",
+            "widthinterpolation": {"keyword": "WIDTHINTERPOLATION:",
                                    "describe": "Option for interpolating width values", "value": 0, "tags": ["flow"]},
 
             # ==================================================================================================
             # HYDROLOGIC PARAMETERS
             # ==================================================================================================
 
-            "optevapotrans": {"key_word": "OPTEVAPOTRANS:", "describe": "Option for evapoTranspiration scheme\n" + \
+            "optevapotrans": {"keyword": "OPTEVAPOTRANS:", "describe": "Option for evapoTranspiration scheme\n" + \
                                                                         "0  Inactive evapotranspiration\n" + \
                                                                         "1  Penman-Monteith method\n" + \
                                                                         "2  Deardorff method\n" + \
                                                                         "3  Priestley-Taylor method\n" + \
                                                                         "4  Pan evaporation measurements", "value": 1,
                               "tags": ["hydro"]},
-            "optintercept": {"key_word": "OPTINTERCEPT:", "describe": "Option for interception scheme\n" + \
+            "optintercept": {"keyword": "OPTINTERCEPT:", "describe": "Option for interception scheme\n" + \
                                                                       "0  Inactive interception\n" + \
                                                                       "1  Canopy storage method\n" + \
                                                                       "2  Canopy water balance method", "value": 2,
                              "tags": ["hydro"]},
-            "optlanduse": {"key_word": "OPTLANDUSE:", "describe": "Option for static or dynamic land cover\n" + \
+            "optlanduse": {"keyword": "OPTLANDUSE:", "describe": "Option for static or dynamic land cover\n" + \
                                                                   "0  Static land cover maps\n" + \
                                                                   "1  Dynamic updating of land cover maps", "value": 0,
                            "tags": ["hydro"]},
-            "optluinterp": {"key_word": "OPTLUINTERP:", "describe": "Option for interpolation of land cover\n" + \
+            "optluinterp": {"keyword": "OPTLUINTERP:", "describe": "Option for interpolation of land cover\n" + \
                                                                     "0  Constant (previous) values between land cover\n" + \
                                                                     "1  Linear interpolation between land cover",
                             "value": 1, "tags": ["hydro"]},
-            "optsoiltype": {"key_word": "OPTSOILTYPE:", "describe": "Option for soil input type: 0 soil table, 1 soil "
+            "optsoiltype": {"keyword": "OPTSOILTYPE:", "describe": "Option for soil input type: 0 soil table, 1 soil "
                                                                     "rasters\n See SCGRID, SOILTABLENAME, and SOILMAPNAME",
                             "value": 0, "tags": ["hydro"]},
-            "gfluxoption": {"key_word": "GFLUXOPTION:", "describe": "Option for ground heat flux\n" + \
+            "gfluxoption": {"keyword": "GFLUXOPTION:", "describe": "Option for ground heat flux\n" + \
                                                                     "0  Inactive ground heat flux\n" + \
                                                                     "1  Temperature gradient method\n" + \
                                                                     "2  Force_Restore method", "value": 2,
                              "tags": ["hydro"]},
-            "optbedrock": {"key_word": "OPTBEDROCK:", "describe": "Option for uniform or variable depth\n"
+            "optbedrock": {"keyword": "OPTBEDROCK:", "describe": "Option for uniform or variable depth\n"
                                                                   "0 Uniform bedrock depth\n"
                                                                   "1 Spatial grid of bedrock depth\n"
                                                                   "See DEPTHTOBEDROCK and BEDROCKFILE\n", "value": 0,
                            "tags": ["hydro"]},
-            "optgroundwater": {"key_word": "OPTGROUNDWATER","describe": "Option for groundwater module, 0 off, 1 on",
+            "optgroundwater": {"keyword": "OPTGROUNDWATER","describe": "Option for groundwater module, 0 off, 1 on",
                                 "value": 1, "tags": ['hydro']},
 
-            "optgwfile": {"key_word": "OPTGWFILE:", "describe": "Option for groundwater initial file\n" + \
+            "optgwfile": {"keyword": "OPTGWFILE:", "describe": "Option for groundwater initial file\n" + \
                                                                 "0 Resample ASCII grid file in GWATERFILE\n" + \
                                                                 "1 Read in Voronoi polygon file with GW levels",
                           "value": 0, "tags": ["hydro"]},
 
-            "optrunon": {"key_word": "OPTRUNON:", "describe": "Option for runon in overland flow paths [IN DEVELOPMENT]: 0 off, 1 on", "value": 0,
+            "optrunon": {"keyword": "OPTRUNON:", "describe": "Option for runon in overland flow paths [IN DEVELOPMENT]: 0 off, 1 on", "value": 0,
                          "tags": ["hydro"]},
-            "optreservoir": {"key_word": "OPTRESERVOIR:", "describe": 'Option for leve pool routing: 0 off, 1 on',
+            "optreservoir": {"keyword": "OPTRESERVOIR:", "describe": 'Option for leve pool routing: 0 off, 1 on',
                              "value": 0, "tags": ["hydro"]},
             ### added
-            "respolygonid": {"key_word": "RESPOLYGONID:", "describe": "Path to file of node IDs representing reservoirs",
+            "respolygonid": {"keyword": "RESPOLYGONID:", "describe": "Path to file of node IDs representing reservoirs",
                              "value":None, "tags": ["hydro"]},
-            "resdata": {"key_word": "RESDATA:", "describe": "Path to file of elevation-discharge-storage information for each type of reservoir",
+            "resdata": {"keyword": "RESDATA:", "describe": "Path to file of elevation-discharge-storage information for each type of reservoir",
                         "value":None,"tags": ["hydro"]},
 
-            "optsnow": {"key_word": "OPTSNOW:", "describe": "Enable single layer snow module : 0 off, 1 on", "value": 1,
+            "optsnow": {"keyword": "OPTSNOW:", "describe": "Enable single layer snow module : 0 off, 1 on", "value": 1,
                         "tags": ["hydro"]},
-            "minsntemp": {"key_word": "MINSNTEMP:", "describe": "Minimum snow temperature", "value": -50.0,
+            "minsntemp": {"keyword": "MINSNTEMP:", "describe": "Minimum snow temperature", "value": -50.0,
                           "tags": ["hydro"]},
-            "snliqfrac": {"key_word": "SNLIQFRAC:", "describe": "Maximum fraction of liquid water in snowpack",
+            "snliqfrac": {"keyword": "SNLIQFRAC:", "describe": "Maximum fraction of liquid water in snowpack",
                           "value": 0.065, "tags": ["hydro"]},
-            "depthtobedrock": {"key_word": "DEPTHTOBEDROCK:", "describe": "Uniform depth to bedrock (meters), see OPTBEDROCK",
+            "depthtobedrock": {"keyword": "DEPTHTOBEDROCK:", "describe": "Uniform depth to bedrock (meters), see OPTBEDROCK",
                                "value": 15, "tags": ["hydro"]},
-            "optpercolation": {"key_word": "OPTPERCOLATION:", "describe": "Option to for percolation losses from channels\n"
+            "optpercolation": {"keyword": "OPTPERCOLATION:", "describe": "Option to for percolation losses from channels\n"
                                "0 off\n1 on"
 
                 , "value": 0,
                                "tags": ["hydro"]},
-            "channelconductivity": {"key_word": "CHANNELCONDUCTIVITY:", "describe": "Conductivity in channel", "value": 0,
+            "channelconductivity": {"keyword": "CHANNELCONDUCTIVITY:", "describe": "Conductivity in channel", "value": 0,
                                     "tags": ["hydro"]},
-            "transientconductivity": {"key_word": "TRANSIENTCONDUCTIVITY:", "describe": "Conductivity during transient period",
+            "transientconductivity": {"keyword": "TRANSIENTCONDUCTIVITY:", "describe": "Conductivity during transient period",
                                       "value": 0, "tags": ["hydro"]},
-            "transienttime": {"key_word": "TRANSIENTTIME:", "describe": "Time until transient period ends", "value": 0,
+            "transienttime": {"keyword": "TRANSIENTTIME:", "describe": "Time until transient period ends", "value": 0,
                               "tags": ["hydro"]},
-            "channelporosity": {"key_word": "CHANNELPOROSITY:", "describe": "Porosity in channel", "value": 0,
+            "channelporosity": {"keyword": "CHANNELPOROSITY:", "describe": "Porosity in channel", "value": 0,
                                 "tags": ["hydro"]},
-            "chanporeindex": {"key_word": "CHANPOREINDEX:", "describe": "Channel pore index in channel", "value": 0,
+            "chanporeindex": {"keyword": "CHANPOREINDEX:", "describe": "Channel pore index in channel", "value": 0,
                               "tags": ["hydro"]},
-            "chanpsib": {"key_word": "CHANPSIB:", "describe": "Matric potential in channel", "value": 0, "tags": ["hydro"]},
+            "chanpsib": {"keyword": "CHANPSIB:", "describe": "Matric potential in channel", "value": 0, "tags": ["hydro"]},
             # ==================================================================================================
             # GRID RESAMPLE
             # ==================================================================================================
 
-            "lugrid": {"key_word": "LUGRID:", "describe": "Land cover grid data file (*.gdf)", "value": None,
+            "lugrid": {"keyword": "LUGRID:", "describe": "Land cover grid data file (*.gdf)", "value": None,
                        "tags": ["spatial"]},
-            "scgrid": {"key_word": "SCGRID:", "describe": "Soil grid data file (*.gdf). Note OPTSOILTYPE must = 1 if "
+            "scgrid": {"keyword": "SCGRID:", "describe": "Soil grid data file (*.gdf). Note OPTSOILTYPE must = 1 if "
                                                           "inputing soil grids", "value": None,
                        "tags": ["spatial"]},
-            "soiltablename": {"key_word": "SOILTABLENAME:", "describe": "Soil parameter reference table (*.sdt)",
+            "soiltablename": {"keyword": "SOILTABLENAME:", "describe": "Soil parameter reference table (*.sdt)",
                               "value": None, "tags": ["spatial"]},
-            "soilmapname": {"key_word": "SOILMAPNAME:", "describe": "Soil texture ASCII grid (*.soi)", "value": None,
+            "soilmapname": {"keyword": "SOILMAPNAME:", "describe": "Soil texture ASCII grid (*.soi)", "value": None,
                             "tags": ["spatial"]},
-            "landtablename": {"key_word": "LANDTABLENAME:", "describe": "Land use parameter reference table",
+            "landtablename": {"keyword": "LANDTABLENAME:", "describe": "Land use parameter reference table",
                               "value": None, "tags": ["spatial"]},
-            "landmapname": {"key_word": "LANDMAPNAME:", "describe": "Land use ASCII grid (*.lan)", "value": None,
+            "landmapname": {"keyword": "LANDMAPNAME:", "describe": "Land use ASCII grid (*.lan)", "value": None,
                             "tags": ["spatial"]},
-            "gwaterfile": {"key_word": "GWATERFILE:", "describe": "Ground water ASCII grid (*iwt)", "value": None,
+            "gwaterfile": {"keyword": "GWATERFILE:", "describe": "Ground water ASCII grid (*iwt)", "value": None,
                            "tags": ["spatial"]},
-            "bedrockfile": {"key_word": "BEDROCKFILE:", "describe": "Bedrock depth ASCII grid (*.brd), see OPTBEDROCK", "value": None,
+            "bedrockfile": {"keyword": "BEDROCKFILE:", "describe": "Bedrock depth ASCII grid (*.brd), see OPTBEDROCK", "value": None,
                             "tags": ["spatial"]},
-            "demfile": {"key_word": "DEMFILE:", "describe": "DEM ASCII grid for sky and land view factors (*.dem)",
+            "demfile": {"keyword": "DEMFILE:", "describe": "DEM ASCII grid for sky and land view factors (*.dem)",
                         "value": None, "tags": ["spatial"]},
 
             # ==================================================================================================
             # METEROLOGICAL DATA
             # ==================================================================================================
-            "rainsource": {"key_word": "RAINSOURCE:", "describe": "Rainfall data source option\n" +
+            "rainsource": {"keyword": "RAINSOURCE:", "describe": "Rainfall data source option\n" +
                                                                   "1  Stage III radar\n" +
                                                                   "2  WSI radar\n" +
                                                                   "3  Rain gauges", "value": 3, "tags": ["meterological"]},
-            "rainfile": {"key_word": "RAINFILE:", "describe": "Base name of the radar ASCII grid", "value": None,
+            "rainfile": {"keyword": "RAINFILE:", "describe": "Base name of the radar ASCII grid", "value": None,
                          "tags": ["meterological"]},
-            "rainextension": {"key_word": "RAINEXTENSION:", "describe": "Extension for the radar ASCII grid",
+            "rainextension": {"keyword": "RAINEXTENSION:", "describe": "Extension for the radar ASCII grid",
                               "value": None, "tags": ["meterological"]},
-            "metdataoption": {"key_word": "METDATAOPTION:", "describe": "Option for meteorological data\n" + \
+            "metdataoption": {"keyword": "METDATAOPTION:", "describe": "Option for meteorological data\n" + \
                                                                         "0  Inactive meteorological data\n" + \
                                                                         "1  Weather station point data\n" +
                                                                         "2  Gridded meteorological data", "value": 1,
                               "tags": ["meterological"]},
-            "hydrometstations": {"key_word": "HYDROMETSTATIONS:",
+            "hydrometstations": {"keyword": "HYDROMETSTATIONS:",
                                  "describe": "Hydrometeorological station file (*.sdf)", "value": None, "tags": ["meterological"]},
-            "hydrometgrid": {"key_word": "HYDROMETGRID:", "describe": "Hydrometeorological grid data file (*.gdf)",
+            "hydrometgrid": {"keyword": "HYDROMETGRID:", "describe": "Hydrometeorological grid data file (*.gdf)",
                              "value": None, "tags": ["meterological"]},
-            "hydrometconvert": {"key_word": "HYDROMETCONVERT:",
+            "hydrometconvert": {"keyword": "HYDROMETCONVERT:",
                                 "describe": "Hydrometeorological data conversion file (*.mdi)", "value": None,
                                 "tags": ["meterological"]},
-            "hydrometbasename": {"key_word": "HYDROMETBASENAME:",
+            "hydrometbasename": {"keyword": "HYDROMETBASENAME:",
                                  "describe": "Hydrometeorological data BASE name (*.mdf)", "value": None,
                                  "tags": ["meterological"]},
-            "gaugestations": {"key_word": "GAUGESTATIONS:", "describe": "Rain Gauge station file (*.sdf)",
+            "gaugestations": {"keyword": "GAUGESTATIONS:", "describe": "Rain Gauge station file (*.sdf)",
                               "value": None, "tags": ["meterological"]},
-            "gaugeconvert": {"key_word": "GAUGECONVERT:", "describe": "Rain Gauge data conversion file (*.mdi)",
+            "gaugeconvert": {"keyword": "GAUGECONVERT:", "describe": "Rain Gauge data conversion file (*.mdi)",
                              "value": None, "tags": ["meterological"]},
-            "gaugebasename": {"key_word": "GAUGEBASENAME:", "describe": "Rain Gauge data BASE name (*.mdf)",
+            "gaugebasename": {"keyword": "GAUGEBASENAME:", "describe": "Rain Gauge data BASE name (*.mdf)",
                               "value": None, "tags": ["meterological"]},
-            "outhydroextension": {"key_word": "OUTHYDROEXTENSION:", "describe": "Extension for hydrograph output",
+            "outhydroextension": {"keyword": "OUTHYDROEXTENSION:", "describe": "Extension for hydrograph output",
                                   "value": "mrf", "tags": ["meterological"]},
-            "ribshydoutput": {"key_word": "RIBSHYDOUTPUT:", "describe": "Compatibility with RIBS User Interphase,\nDepracted and will be removed.",
+            "ribshydoutput": {"keyword": "RIBSHYDOUTPUT:", "describe": "Compatibility with RIBS User Interphase,\nDepracted and will be removed.",
                               "value": 0, "tags": ["meterological"]},
-            "convertdata": {"key_word": "CONVERTDATA:", "describe": "Option to convert met data format", "value": 0,
+            "convertdata": {"keyword": "CONVERTDATA:", "describe": "Option to convert met data format", "value": 0,
                             "tags": ["meterological"]},
-            "templapse": {"key_word": "TEMPLAPSE:", "describe": "Temperature lapse rate", "value": -0.0065,
+            "templapse": {"keyword": "TEMPLAPSE:", "describe": "Temperature lapse rate", "value": -0.0065,
                           "tags": ["meterological"]},
-            "preclapse": {"key_word": "PRECLAPSE:", "describe": "Precipitation lapse rate", "value": 0,
+            "preclapse": {"keyword": "PRECLAPSE:", "describe": "Precipitation lapse rate", "value": 0,
                           "tags": ["meterological"]},
-            "hillalbopt": {"key_word": "HILLALBOPT:", "describe": "Option for albedo of surrounding hillslopes\n" + \
+            "hillalbopt": {"keyword": "HILLALBOPT:", "describe": "Option for albedo of surrounding hillslopes\n" + \
                                                                   "0  Snow albedo for hillslopes\n" + \
                                                                   "1  Land-cover albedo for hillslopes\n" + \
                                                                   "2  Dynamic albedo for hillslopes", "value": 0,
                            "tags": ["meterological"]},
-            "optradshelt": {"key_word": "OPTRADSHELT:", "describe": "Option for local and remote radiation sheltering" +
+            "optradshelt": {"keyword": "OPTRADSHELT:", "describe": "Option for local and remote radiation sheltering" +
                                                                     "0  Local controls on shortwave radiation\n" + \
                                                                     "1  Remote controls on diffuse shortwave\n" + \
                                                                     "2  Remote controls on entire shortwave\n" + \
                                                                     "3  No sheltering", "value": 0, "tags": ["meterological"]},
-            "tlinke": {"key_word": "TLINKE:", "describe": "Atmospheric turbidity parameter", "value": 2.5,
+            "tlinke": {"keyword": "TLINKE:", "describe": "Atmospheric turbidity parameter", "value": 2.5,
                        "tags": ["meterological"]},
             # ==================================================================================================
             # OUTPUT DATA
             # ==================================================================================================
-            "outfilename": {"key_word": "OUTFILENAME:", "describe": "Base name of the tMesh and variable",
+            "outfilename": {"keyword": "OUTFILENAME:", "describe": "Base name of the tMesh and variable",
                             "value": None, "tags": ["output"]},
-            "outhydrofilename": {"key_word": "OUTHYDROFILENAME:", "describe": "Base name for hydrograph output",
+            "outhydrofilename": {"keyword": "OUTHYDROFILENAME:", "describe": "Base name for hydrograph output",
                                  "value": None, "tags": ["output"]},
-            "optspatial": {"key_word": "OPTSPATIAL:", "describe": "Enable dynamic spatial output", "value": 0,
+            "optspatial": {"keyword": "OPTSPATIAL:", "describe": "Enable dynamic spatial output", "value": 0,
                            "tags": ["output"]},
-            "optinterhydro": {"key_word": "OPTINTERHYDRO:", "describe": "Enable intermediate hydrograph output",
+            "optinterhydro": {"keyword": "OPTINTERHYDRO:", "describe": "Enable intermediate hydrograph output",
                               "value": 0, "tags": ["output"]},
-            "optheader": {"key_word": "OPTHEADER:", "describe": "Enable headers in output files", "value": 1,
+            "optheader": {"keyword": "OPTHEADER:", "describe": "Enable headers in output files", "value": 1,
                           "tags": ["output"]},
-            "optviz": {"key_word": "OPTVIZ:", "describe": "Option to write binary output files for visualization\n" + \
+            "optviz": {"keyword": "OPTVIZ:", "describe": "Option to write binary output files for visualization\n" + \
                                                           "0  Do NOT write binary output files for viz\n" + \
                                                           "1  Write binary output files for viz", "value": 0,
                        "tags": ["output"]},
-            "outvizfilename": {"key_word": "OUTVIZFILENAME:", "describe": "Filename for viz binary files",
+            "outvizfilename": {"keyword": "OUTVIZFILENAME:", "describe": "Filename for viz binary files",
                                "value": None, "tags": ["output"]},
-            "nodeoutputlist": {"key_word": "NODEOUTPUTLIST:",
+            "nodeoutputlist": {"keyword": "NODEOUTPUTLIST:",
                                "describe": "Filename with Nodes for Dynamic Output (*.nol)", "value": None,
                                "tags": ["output"]},
-            "hydronodelist": {"key_word": "HYDRONODELIST:",
+            "hydronodelist": {"keyword": "HYDRONODELIST:",
                               "describe": "Filename with Nodes for HydroModel Output (*.nol)", "value": None,
                               "tags": ["output"]},
-            "outletnodelist": {"key_word": "OUTLETNODELIST:",
+            "outletnodelist": {"keyword": "OUTLETNODELIST:",
                                "describe": "Filename with Interior Nodes for  Output (*.nol)", "value": None,
                                "tags": ["output"]},
-            "opintrvl": {"key_word": "OPINTRVL:", "describe": "Output interval (hours)", "value": 1, "tags": ["output"]},
-            "spopintrvl": {"key_word": "SPOPINTRVL:", "describe": "Spatial output interval (hours)", "value": 50000,
+            "opintrvl": {"keyword": "OPINTRVL:", "describe": "Output interval (hours)", "value": 1, "tags": ["output"]},
+            "spopintrvl": {"keyword": "SPOPINTRVL:", "describe": "Spatial output interval (hours)", "value": 50000,
                            "tags": ["output"]},
             # ==================================================================================================
             # FORECAST MODE
             # ==================================================================================================
-            "forecastmode": {"key_word": "FORECASTMODE:", "describe": "Rainfall Forecasting Mode Option", "value": 0,
+            "forecastmode": {"keyword": "FORECASTMODE:", "describe": "Rainfall Forecasting Mode Option", "value": 0,
                              "tags": ["forecast"]},
             # TODO need to update model mode descriptions
-            "forecasttime": {"key_word": "FORECASTTIME:", "describe": "Forecast Time (hours from start)", "value": 0,
+            "forecasttime": {"keyword": "FORECASTTIME:", "describe": "Forecast Time (hours from start)", "value": 0,
                              "tags": ["forecast"]},
-            "forecastleadtime": {"key_word": "FORECASTLEADTIME:", "describe": "Forecast Lead Time (hours) ",
+            "forecastleadtime": {"keyword": "FORECASTLEADTIME:", "describe": "Forecast Lead Time (hours) ",
                                  "value": 0, "tags": ["forecast"]},
-            "forecastlength": {"key_word": "FORECASTLENGTH:", "describe": "Forecast Window Length (hours)", "value": 0,
+            "forecastlength": {"keyword": "FORECASTLENGTH:", "describe": "Forecast Window Length (hours)", "value": 0,
                                "tags": ["forecast"]},
-            "forecastfile": {"key_word": "FORECASTFILE:", "describe": "Base name of the radar QPF grids",
+            "forecastfile": {"keyword": "FORECASTFILE:", "describe": "Base name of the radar QPF grids",
                              "value": None, "tags": ["forecast"]},
-            "climatology": {"key_word": "CLIMATOLOGY:", "describe": "Rainfall climatology (mm/hr)", "value": 0,
+            "climatology": {"keyword": "CLIMATOLOGY:", "describe": "Rainfall climatology (mm/hr)", "value": 0,
                             "tags": ["forecast"]},
-            "raindistribution": {"key_word": "RAINDISTRIBUTION:", "describe": "Distributed or MAP radar rainfall",
+            "raindistribution": {"keyword": "RAINDISTRIBUTION:", "describe": "Distributed or MAP radar rainfall",
                                  "value": 0, "tags": ["forecast"]},
             # ==================================================================================================
             # STOCHASTIC MODE
             # ==================================================================================================
-            "stochasticmode": {"key_word": "STOCHASTICMODE:", "describe": "Stochastic Climate Mode Option", "value": 0,
+            "stochasticmode": {"keyword": "STOCHASTICMODE:", "describe": "Stochastic Climate Mode Option", "value": 0,
                                "tags": ["stochastic"]},
-            "pmean": {"key_word": "PMEAN:", "describe": "Mean rainfall intensity (mm/hr)	", "value": 0,
+            "pmean": {"keyword": "PMEAN:", "describe": "Mean rainfall intensity (mm/hr)	", "value": 0,
                       "tags": ["stochastic"]},
-            "stdur": {"key_word": "STDUR:", "describe": "Mean storm duration (hours)", "value": 0,
+            "stdur": {"keyword": "STDUR:", "describe": "Mean storm duration (hours)", "value": 0,
                       "tags": ["stochastic"]},
-            "istdur": {"key_word": "ISTDUR:", "describe": "Mean time interval between storms (hours)", "value": 0,
+            "istdur": {"keyword": "ISTDUR:", "describe": "Mean time interval between storms (hours)", "value": 0,
                        "tags": ["stochastic"]},
-            "seed": {"key_word": "SEED:", "describe": "Random seed", "value": 0, "tags": ["stochastic"]},
-            "period": {"key_word": "PERIOD:", "describe": "Period of variation (hours)", "value": 0,
+            "seed": {"keyword": "SEED:", "describe": "Random seed", "value": 0, "tags": ["stochastic"]},
+            "period": {"keyword": "PERIOD:", "describe": "Period of variation (hours)", "value": 0,
                        "tags": ["stochastic"]},
-            "maxpmean": {"key_word": "MAXPMEAN:", "describe": "Maximum value of mean rainfall intensity (mm/hr)",
+            "maxpmean": {"keyword": "MAXPMEAN:", "describe": "Maximum value of mean rainfall intensity (mm/hr)",
                          "value": 0, "tags": ["stochastic"]},
-            "maxstdurmn": {"key_word": "MAXSTDURMN:", "describe": "Maximum value of mean storm duration (hours)",
+            "maxstdurmn": {"keyword": "MAXSTDURMN:", "describe": "Maximum value of mean storm duration (hours)",
                            "value": 0, "tags": ["stochastic"]},
-            "maxistdurmn": {"key_word": "MAXISTDURMN:", "describe": "Maximum value of mean interstorm period (hours)",
+            "maxistdurmn": {"keyword": "MAXISTDURMN:", "describe": "Maximum value of mean interstorm period (hours)",
                             "value": 0, "tags": ["stochastic"]},
-            "weathertablename": {"key_word": "WEATHERTABLENAME:", "describe": "File with Stochastic Weather Table",
+            "weathertablename": {"keyword": "WEATHERTABLENAME:", "describe": "File with Stochastic Weather Table",
                                  "value": None, "tags": ["stochastic"]},
             # ==================================================================================================
             # RESTART MODE
             # ==================================================================================================
-            "restartmode": {"key_word": "RESTARTMODE:", "describe": "Restart Mode Option\n" + \
+            "restartmode": {"keyword": "RESTARTMODE:", "describe": "Restart Mode Option\n" + \
                                                                     "0 No reading or writing of restart\n" + \
                                                                     "1 Write files (only for initial runs)\n" + \
                                                                     "2 Read file only (to start at some specified time)\n" + \
                                                                     "Read a restart file and continue to write",
                             "value": 0, "tags": ["restart"]},
-            "restartintrvl": {"key_word": "RESTARTINTRVL:", "describe": "Time set for restart output (hours)",
+            "restartintrvl": {"keyword": "RESTARTINTRVL:", "describe": "Time set for restart output (hours)",
                               "value": None, "tags": ["restart"]},
-            "restartdir": {"key_word": "RESTARTDIR:", "describe": "Path of directory for restart output",
+            "restartdir": {"keyword": "RESTARTDIR:", "describe": "Path of directory for restart output",
                            "value": None, "tags": ["restart"]},
-            "restartfile": {"key_word": "RESTARTFILE:", "describe": "Actual file to restart a run", "value": None,
+            "restartfile": {"keyword": "RESTARTFILE:", "describe": "Actual file to restart a run", "value": None,
                             "tags": ["restart"]},
             # ==================================================================================================
             # PARALLEL MODE
             # ==================================================================================================
-            "parallelmode": {"key_word": "PARALLELMODE:", "describe": "Parallel or Serial Mode Option\n" + \
+            "parallelmode": {"keyword": "PARALLELMODE:", "describe": "Parallel or Serial Mode Option\n" + \
                                                                       "0  Run in serial mode\n" + \
                                                                       "1  Run in parallel mode",
                              "value": 0, "tags": ["parallel"]},
-            "graphoption": {"key_word": "GRAPHOPTION:", "describe": "Graph File Type Option\n" + \
+            "graphoption": {"keyword": "GRAPHOPTION:", "describe": "Graph File Type Option\n" + \
                                                                     "0  Default partitioning of the graph\n" + \
                                                                     "1  Reach-based partitioning\n" + \
                                                                     "2  Inlet/outlet-based partitioning", "value": 0,
                             "tags": ["parallel"]},
-            "graphfile": {"key_word": "GRAPHFILE:", "describe": "Reach connectivity filename (graph file option 1,2)",
+            "graphfile": {"keyword": "GRAPHFILE:", "describe": "Reach connectivity filename (graph file option 1,2)",
                           "value": None, "tags": ["parallel"]}
         }
 
         return input_file
```

### Comparing `pytribs-0.2.0/pytRIBS/mixins/shared_mixin.py` & `pytribs-0.3.0/pytRIBS/shared/shared_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 import geopandas as gpd
 import pandas as pd
 import pyvista as pv
 from shapely.geometry import LineString
 from shapely.geometry import Point
 from shapely.geometry import Polygon
 
+class GeoMixin:
+    def __init__(self):
+        self.geo = {"UTM_Zone": None, "EPSG": None, "Projection": None}
+
 
 class SharedMixin:
     """
     Shared methods betweens the pytRIBS Classes Model & Results.
     """
 
     def read_input_file(self, file_path):
@@ -219,14 +223,15 @@
 
         :param join: Data frame of dynamic or integrated tRIBS model output (optional).
         :param save: Set to True to save geodataframe (optional, default True).
         :param result_path: Path to save geodateframe (optional, default OUTFILENAME).
         :param format: Driver options for writing geodateframe (optional, default = ESRI Shapefile)
 
         :return: GeoDataFrame
+
         """
 
         outfilename = self.options["outfilename"]["value"]
         path_components = outfilename.split(os.path.sep)
         # Exclude the last directory as its actually base name
         outfilename = os.path.sep.join(path_components[:-1])
 
@@ -281,14 +286,15 @@
         :param int dtime : Option to specify time step at which to start merge of files.
         :param bool write: Option to write dataframes to file.
         :param bool header: Set to False if headers are not provided with spatial files.
         :param bool colnames: If header = False, column names can be provided for the dataframe--but it is expected the first column is ID.
         :param bool single: If single = True then only spatial files specified at dtime are merged.
         :return: Dictionary of pandas dataframes.
         # TODO add a clean option to store .0 t0 .n files, then zip, probably would only want this if you are saving them out.
+        # TODO also return file names if saved out, also add serial version or a serial flag...so people can reaou
         """
 
         runtime = int(self.options["runtime"]["value"])
         spopintrvl = int(self.options["spopintrvl"]["value"])
         outfilename = self.options["outfilename"]["value"]
 
         dyn_data = {}
```

### Comparing `pytribs-0.2.0/pytRIBS/model/aux.py` & `pytribs-0.3.0/pytRIBS/shared/aux.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,43 @@
 import subprocess
 import os
 import shutil
 import pandas as pd
+import rasterio
+from rasterio import fill
+
 
 class Aux:
+
+    @staticmethod
+    def fillnodata(files, overwrite=False, **kwargs):
+        """
+        Fills nodata gaps in raster files based on a maximum search distance.
+
+        Parameters:
+        files (list): List of paths to raster files.
+        overwrite (bool): If True, the original files will be overwritten with filled data. If False, new files with "_filled" suffix will be created.
+        **kwargs: Additional keyword arguments to be passed to rasterio.fill.fillnodata.
+
+        Note:
+        This function essentially wraps rasterio.fill.fillnodata.
+        """
+        for file_path in files:
+            with rasterio.open(file_path) as src:
+                data = src.read(1)
+                msk = src.read_masks(1)
+                filled_data = fill.fillnodata(data, mask=msk, **kwargs)
+                if overwrite:
+                    with rasterio.open(file_path, 'w', **src.profile) as dst:
+                        dst.write(filled_data, 1)
+                else:
+                    base_name, ext = os.path.splitext(file_path)
+                    filled_file_path = f"{base_name}_filled{ext}"
+                    with rasterio.open(filled_file_path, 'w', **src.profile) as dst:
+                        dst.write(filled_data, 1)
     @staticmethod
     def convert_to_datetime(starting_date):
         """
         Returns a pandas date-time object.
 
         :param starting_date: The start date of a given model simulation, note needs to be in tRIBS format.
         :type starting_date: str
```

### Comparing `pytribs-0.2.0/pytRIBS/model/diagnose.py` & `pytribs-0.3.0/pytRIBS/model/diagnose.py`

 * *Files identical despite different names*

### Comparing `pytribs-0.2.0/pytRIBS/model/inout.py` & `pytribs-0.3.0/pytRIBS/shared/inout.py`

 * *Files 3% similar despite different names*

```diff
@@ -344,89 +344,14 @@
 
             # Write station information
             for station in station_list:
                 line = f"{station['station_id']} {station['file_path']} {station['lat_dd']} {station['y']} {station['long_dd']} {station['x']} " \
                        f"{station['GMT']} {station['record_length']} {station['num_parameters']} {station['other']}\n"
                 file.write(line)
 
-
-    def read_soil_table(self, file_path=None):
-        """
-        Soil Reclassification Table Structure (*.sdt)
-        #Types #Params
-        ID Ks thetaS thetaR m PsiB f As Au n ks Cs
-        """
-        if file_path is None:
-            file_path = self.options["soiltablename"]["value"]
-
-            if file_path is None:
-                print(self.options["soiltablename"]["key_word"] + "is not specified.")
-                return None
-
-        soil_list = []
-
-        with open(file_path, 'r') as file:
-            lines = file.readlines()
-
-        metadata = lines.pop(0)
-        num_types, num_params = map(int, metadata.strip().split())
-        param_standard = 12
-
-        if num_params != param_standard:
-            print(f"The number parameters in {file_path} do not conform with standard soil .sdt format.")
-            return
-
-        for l in lines:
-            soil_info = l.strip().split()
-
-            if len(soil_info) == param_standard:
-                _id, ks, theta_s, theta_r, m, psi_b, f, a_s, a_u, n, _ks, c_s = soil_info
-                station = {
-                    "ID": _id,
-                    "Ks": ks,
-                    "thetaS": theta_s,
-                    "thetaR": theta_r,
-                    "m": m,
-                    "PsiB": psi_b,
-                    "f": f,
-                    "As": a_s,
-                    "Au": a_u,
-                    "n": n,
-                    "ks": _ks,
-                    "Cs": c_s
-                }
-                soil_list.append(station)
-
-        if len(soil_list) != num_types:
-            print("Error: Number of soil types does not match the specified count.")
-
-        return soil_list
-    @staticmethod
-    def write_soil_table(soil_list,file_path):
-        """
-        Writes out Soil Reclassification Table(*.sdt) file with the following format:
-        #Types #Params
-        ID Ks thetaS thetaR m PsiB f As Au n ks Cs
-
-        :param soil_list: List of dictionaries containing soil information specified by .sdt structure above.
-        :param file_path: Path to save *.sdt file.
-        """
-        param_standard = 12
-
-        with open(file_path, 'w') as file:
-            # Write metadata line
-            metadata = f"{len(soil_list)} {param_standard}\n"
-            file.write(metadata)
-
-            # Write station information
-            for type in soil_list:
-                line = f"{str(type['ID'])}   {str(type['Ks'])}    {str(type['thetaS'])}    {str(type['thetaR'])}    {str(type['m'])}    {str(type['PsiB'])}    " \
-                       f"{str(type['f'])}    {str(type['As'])}    {str(type['Au'])}    {str(type['n'])}    {str(type['ks'])}    {str(type['Cs'])}\n"
-                file.write(line)
-
     def read_landuse_table(self, file_path=None):
         """
         Returns list of dictionaries for each type of landuse specified in the .ldt file.
 
         Land Use Reclassification Table Structure (*.ldt, see tRIBS documentation for more details)
         #Types	#Params
         ID	a	b1	 P	S	K	b2	Al	 h	Kt	Rs	V LAI theta*_s theta*_t
```

### Comparing `pytribs-0.2.0/pytRIBS/model/preprocess.py` & `pytribs-0.3.0/pytRIBS/soil/soil.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,224 +1,150 @@
-import os
 import re
+import os
 
 import numpy as np
-import rasterio
-import rasterio.fill as fill
-from scipy.optimize import curve_fit
-from scipy.ndimage import map_coordinates
-from shapely.geometry import LineString, Point
 from owslib.wcs import WebCoverageService
-import geopandas as gpd
 from rosetta import rosetta, SoilData
+from scipy.optimize import curve_fit
+from pytRIBS.shared.inout import InOut
+from pytRIBS.shared.aux import Aux
 
-from pytRIBS.model.inout import InOut
-
-
-### PREPROCESSING
-# 1 delineate watersheds (pyshed)
-# 1.create points file for hydrological conditioned tin Mesh
-# 2 ingest soil and land use (pyshed)
-# 3 apply pedotransfer functions
-# others?
-
-class Preprocess(InOut):
-    """
 
-    """
+class _Soil:
+    # Assigning references to the methods
 
-    # MESH TOOLS
     @staticmethod
-    def remove_duplicates_points(gdf, radius):
-        # Create a new column with a buffer around each point
-        gdf['buffer'] = gdf['geometry'].buffer(radius)
-
-        # Iterate through each row and check if there are other points within the buffer
-        to_remove = set()
-        for idx, row in gdf.iterrows():
-            if idx not in to_remove:
-                # Extract the buffer of the current row
-                current_buffer = row['buffer']
-
-                # Check for overlapping points within the buffer
-                overlapping_points = gdf[gdf['geometry'].within(current_buffer) & (gdf.index != idx)]
-
-                # Mark overlapping points for removal, excluding those with 'bc' equal to 2
-                to_remove.update(overlapping_points[overlapping_points['bc'] != 2].index)
+    def fillnodata(files, overwrite=False, **kwargs):
+        Aux.fillnodata(files, overwrite=overwrite, **kwargs)
 
-        # Drop unnecessary columns
-        result = gdf.drop(to_remove, axis=0).drop('buffer', axis=1)
+    @staticmethod
+    def write_ascii(raster_dict, output_file_path,dtype='float32'):
+        InOut.write_ascii(raster_dict, output_file_path, dtype)
 
-        return result
+    @staticmethod
+    def read_ascii(file_path):
+        raster = InOut.read_ascii(file_path)
+        return raster
 
     @staticmethod
-    def generate_points_along_stream(gdf, points_per_meter):
-        """
-        Generate evenly distributed points along each stream segment in a GeoDataFrame.
+    def read_json(raster_dict, output_file_path, dtype='float32'):
+        input = InOut.read_json(raster_dict, output_file_path, dtype)
+        return input
 
-        Parameters:
-        - gdf: GeoDataFrame
-            GeoDataFrame containing the stream network with LineString geometries.
-        - points_per_meter: int
-            Number of points to generate per meter along each stream segment.
-
-        Returns:
-        GeoDataFrame
-            GeoDataFrame containing the generated points.
+    def read_soil_table(self, textures=False, file_path=None):
+        """
+        Soil Reclassification Table Structure (*.sdt)
+        #Types #Params
+        ID Ks thetaS thetaR m PsiB f As Au n ks Cs
+        an o
+        :param textures: Optional True/False for writing texture classes to the .sdt file.
+        :param file_path: Specify file_path to soil table not assigned to the .
         """
-        # Create an empty GeoDataFrame to store the generated points
-        points_list = []
+        if file_path is None:
+            file_path = self.soil_table["value"]
 
-        # Iterate over each stream segment in the GeoDataFrame
-        for idx, row in gdf.iterrows():
-            # Extract the LineString geometry for the current stream segment
-            line = row['geometry']
+            if file_path is None:
+                print(self.soil_table["key_word"] + "is not specified.")
+                return None
 
-            # Calculate the total length of the stream segment
-            total_length = line.length
+        soil_list = []
 
-            # Calculate the total number of points based on the total length and points_per_meter
-            total_points = int(total_length * points_per_meter)
+        with open(file_path, 'r') as file:
+            lines = file.readlines()
 
-            # Generate evenly distributed points along the stream segment
-            points = [line.interpolate(i / total_points, normalized=True) for i in range(total_points + 1)]
+        metadata = lines.pop(0)
+        num_types, num_params = map(int, metadata.strip().split())
+        param_standard = 12
 
-            # Add the points to the list
-            points_list.extend({'geometry': Point(p)} for p in points)
+        if textures:
+            param_standard += 1
 
-        # Create the GeoDataFrame from the list of dictionaries
-        points_gdf = gpd.GeoDataFrame(points_list)
+        if num_params != param_standard:
+            print(f"The number parameters in {file_path} do not conform with standard soil .sdt format.")
+            return
 
-        return points_gdf
+        for l in lines:
+            soil_info = l.strip().split()
+
+            if len(soil_info) == param_standard:
+                if textures:
+                    _id, ks, theta_s, theta_r, m, psi_b, f, a_s, a_u, n, _ks, c_s, textures = soil_info
+                    station = {
+                        "ID": _id,
+                        "Ks": ks,
+                        "thetaS": theta_s,
+                        "thetaR": theta_r,
+                        "m": m,
+                        "PsiB": psi_b,
+                        "f": f,
+                        "As": a_s,
+                        "Au": a_u,
+                        "n": n,
+                        "ks": _ks,
+                        "Cs": c_s,
+                        "Texture": textures
+                    }
+                else:
+                    _id, ks, theta_s, theta_r, m, psi_b, f, a_s, a_u, n, _ks, c_s = soil_info
+                    station = {
+                        "ID": _id,
+                        "Ks": ks,
+                        "thetaS": theta_s,
+                        "thetaR": theta_r,
+                        "m": m,
+                        "PsiB": psi_b,
+                        "f": f,
+                        "As": a_s,
+                        "Au": a_u,
+                        "n": n,
+                        "ks": _ks,
+                        "Cs": c_s
+                    }
+
+                soil_list.append(station)
+
+        if len(soil_list) != num_types:
+            print("Error: Number of soil types does not match the specified count.")
+        return soil_list
 
     @staticmethod
-    def generate_buffer_points_along_stream(network, resolution=20, buffer_distance=25):
-        # Create buffer geometries
-        buffer_geoms = [line.buffer(buffer_distance) for line in network['geometry']]
-        buffer_gdf = gpd.GeoDataFrame(geometry=buffer_geoms)
-        combined_geometry = buffer_gdf.unary_union
-
-        # Get bounds of the combined geometry
-        latmin, lonmin, latmax, lonmax = combined_geometry.bounds
-
-        # Generate points within the specified resolution
-        points = []
-
-        for lat in np.arange(latmin, latmax, resolution):
-            for lon in np.arange(lonmin, lonmax, resolution):
-                point = Point(round(lat, 4), round(lon, 4))
-
-                # Calculate the distance to the nearest point on the stream network
-                distance_to_stream = min(point.distance(line) for line in network['geometry'])
-
-                # Adjust the point density based on distance (you can customize this function)
-                weight = 1 / (1 + distance_to_stream)
-
-                # Randomly discard points with a probability based on the weight
-                if np.random.rand() < weight and combined_geometry.contains(point):
-                    points.append(point)
-
-        # Create a GeoDataFrame with empty columns 'bc' and 'elevation'
-        columns = ['bc', 'elevation']
-        valid_points_gdf = gpd.GeoDataFrame(geometry=points, columns=columns)
-
-        return valid_points_gdf
-
-    # def generate_buffer_points_along_stream(network, resolution=20, buffer_distance=25):
-    #     # Create buffer geometries
-    #     buffer_geoms = [line.buffer(buffer_distance) for line in network['geometry']]
-    #     buffer_gdf = gpd.GeoDataFrame(geometry=buffer_geoms)
-    #     combined_geometry = buffer_gdf.unary_union
-    #
-    #     # Get bounds of the combined geometry
-    #     latmin, lonmin, latmax, lonmax = combined_geometry.bounds
-    #
-    #     # Generate points within the specified resolution
-    #     points = [Point((round(lat, 4), round(lon, 4)))
-    #               for lat in np.arange(latmin, latmax, resolution)
-    #               for lon in np.arange(lonmin, lonmax, resolution)]
-    #
-    #     # Filter valid points inside the shape
-    #     valid_points = [point for point in points if combined_geometry.contains(point)]
-    #
-    #     # Create a GeoDataFrame with empty columns 'bc' and 'elevation'
-    #     columns = ['bc', 'elevation']
-    #     valid_points_gdf = gpd.GeoDataFrame(geometry=valid_points, columns=columns)
-    #
-    #     return valid_points_gdf
-    @staticmethod
-    def remove_points_near_boundary(points_gdf, boundary_gdf, distance_threshold):
+    def write_soil_table(soil_list, file_path, textures=False):
         """
-        Removes points from the points file (points_gdf) that are closer than distance_threshold to the boundary of
-        the watershed (boundary_gdf).
+        Writes out Soil Reclassification Table(*.sdt) file with the following format:
+        #Types #Params
+        ID Ks thetaS thetaR m PsiB f As Au n ks Cs
 
-        Parameters:
-        - points_gdf: GeoDataFrame containing points with a 'geometry' column.
-        - boundary_gdf: GeoDataFrame containing the boundary with a 'geometry' column.
-        - distance_threshold: Threshold distance for removing points near the boundary.
+        :param soil_list: List of dictionaries containing soil information specified by .sdt structure above.
+        :param file_path: Path to save *.sdt file.
+        :param textures: Optional True/False for writing texture classes to the .sdt file.
 
-        Returns:
-        - GeoDataFrame with points removed near the boundary.
         """
+        param_standard = 12
 
-        # Ensure the GeoDataFrames have 'geometry' columns with appropriate geometries
-        if 'geometry' not in points_gdf.columns or not isinstance(points_gdf['geometry'].iloc[0], Point):
-            raise ValueError("points_gdf must have a 'geometry' column with Point geometries.")
-
-        if 'geometry' not in boundary_gdf.columns:
-            raise ValueError("boundary_gdf must have a 'geometry' column.")
-
-        # Make a copy of the DataFrame
-        points_gdf_copy = points_gdf.copy()
-
-        # Calculate distances from points to the boundary
-        dist = np.array([boundary_gdf.boundary.distance(points_gdf_copy.iloc[x].geometry).min() for x in
-                         range(len(points_gdf_copy))])
-        points_gdf_copy['dist'] = dist
-        idx = (points_gdf_copy['dist'] < distance_threshold) & (
-                (points_gdf_copy['bc'] == 0) | (points_gdf_copy['bc'] == 3))
+        if textures:
+            param_standard += 1
 
-        # Remove points within the distance threshold
-        points_gdf_copy = points_gdf_copy[~idx]
+        with open(file_path, 'w') as file:
+            # Write metadata line
+            metadata = f"{len(soil_list)} {param_standard}\n"
+            file.write(metadata)
 
-        return points_gdf_copy
+            # Write station information
+            for type in soil_list:
 
-    @staticmethod
-    def update_elevation_from_dem(gdf, dem_path, elevation_column='elevation'):
-        """
-        Update the elevation column in a GeoDataFrame using values from a Digital Elevation Model (DEM).
-
-        Parameters:
-        - gdf: GeoDataFrame
-            GeoDataFrame containing points with coordinates.
-        - dem_path: str
-            Path to the Digital Elevation Model (DEM) raster file.
-        - elevation_column: str, optional
-            Name of the column to be updated with elevation values. Default is 'elevation'.
-
-        Returns:
-        GeoDataFrame
-            GeoDataFrame with updated elevation values.
-        """
-        # Open the DEM raster using rasterio
-        with rasterio.open(dem_path) as dem:
-            # Loop through each point in the GeoDataFrame
-            for index, point in gdf.iterrows():
-                # Get the coordinates of the point
-                lon, lat = point['geometry'].x, point['geometry'].y
-
-                # Sample elevation from the DEM raster at the point coordinates
-                for val in dem.sample([(lon, lat)]):
-                    # Update the elevation column in the GeoDataFrame
-                    gdf.at[index, elevation_column] = val[0]
+                if textures:
+                    line = f"{str(type['ID'])}   {str(type['Ks'])}    {str(type['thetaS'])}    {str(type['thetaR'])}    {str(type['m'])}    {str(type['PsiB'])}    " \
+                           f"{str(type['f'])}    {str(type['As'])}    {str(type['Au'])}    {str(type['n'])}    {str(type['ks'])}    {str(type['Cs'])} {str(type['Texture'])}\n"
+                else:
+                    line = f"{str(type['ID'])}   {str(type['Ks'])}    {str(type['thetaS'])}    {str(type['thetaR'])}    {str(type['m'])}    {str(type['PsiB'])}    " \
+                           f"{str(type['f'])}    {str(type['As'])}    {str(type['Au'])}    {str(type['n'])}    {str(type['ks'])}    {str(type['Cs'])}\n"
 
-        return gdf
+                file.write(line)
 
-    ### SOIL PRE-PROCESSING
-    def getSoil250(self, bbox, depths, soil_vars, stats, replace=False):
+    def get_soil_grids(self, bbox, depths, soil_vars, stats, replace=False):
         """
         Retrieves soil data from ISRIC WCS service and saves it as GeoTIFFs and returns list of paths to downloaded files.
 
         Args:
             bbox (list): The bounding box coordinates in the format [x1, y1, x2, y2].
             depths (list): List of soil depths to retrieve data for.
             soil_vars (list): List of soil variables to retrieve.
@@ -275,44 +201,19 @@
             print('Download of SoilGrids250 data complete')
         else:
             print('No SoilGrids250 data was downloaded check inputs or set replace == False.')
 
         os.chdir('..')
         return files
 
-    @staticmethod
-    def fillnodata(files, overwrite=False, **kwargs):
-        """
-        Fills nodata gaps in raster files based on a maximum search distance.
-
-        Parameters:
-        files (list): List of paths to raster files.
-        overwrite (bool): If True, the original files will be overwritten with filled data. If False, new files with "_filled" suffix will be created.
-        **kwargs: Additional keyword arguments to be passed to rasterio.fill.fillnodata.
-
-        Note:
-        This function essentially wraps rasterio.fill.fillnodata.
-        """
-        for file_path in files:
-            with rasterio.open(file_path) as src:
-                data = src.read(1)
-                msk = src.read_masks(1)
-                filled_data = fill.fillnodata(data, mask=msk, **kwargs)
-                if overwrite:
-                    with rasterio.open(file_path, 'w', **src.profile) as dst:
-                        dst.write(filled_data, 1)
-                else:
-                    base_name, ext = os.path.splitext(file_path)
-                    filled_file_path = f"{base_name}_filled{ext}"
-                    with rasterio.open(filled_file_path, 'w', **src.profile) as dst:
-                        dst.write(filled_data, 1)
-
-    # Compute Soil Texture Class
     def create_soil_map(self, grid_input, output=None):
         """
+        Writes out an ascii file with soil classes assigned by soil texture classification and returns a soil classification table
+        with associated parameters.
+
         Parameters:
         - grid_input (list of dict or str): If a dictionary list, keys are "grid_type" and "path" for each soil property.
                                     Format of dictionary list follows:
                                     [{'type':'sand', 'path':'path/to/grid'},
                                     {'type':'clay', 'path':'path/to/grid'},
         """
 
@@ -343,23 +244,23 @@
                 textural_class = 2  # loamy sand
             elif (clay >= 7 and clay < 20 and sand > 52 and silt + 2 * clay >= 30) or (
                     clay < 7 and silt < 50 and silt + 2 * clay >= 30):
                 textural_class = 3  # sandy loam
             elif clay >= 7 and clay < 27 and silt >= 28 and silt < 50 and sand <= 52:
                 textural_class = 4  # loam
             elif (silt >= 50 and clay >= 12 and clay < 27) or (silt >= 50 and silt < 80 and clay < 12):
-                textural_class = 5 # silt loam
+                textural_class = 5  # silt loam
             elif silt >= 80 and clay < 12:
                 textural_class = 6  # silt
             elif clay >= 20 and clay < 35 and silt < 28 and sand > 45:
                 textural_class = 7  # 'sandy clay loam'
             elif clay >= 27 and clay < 40 and sand > 20 and sand <= 45:
                 textural_class = 8  # 'clay loam'
             elif clay >= 27 and clay < 40 and sand <= 20:
-                textural_class = 9 # 'silty clay loam'
+                textural_class = 9  # 'silty clay loam'
             elif clay >= 35 and sand > 45:
                 textural_class = 10  # 'sandy clay'
             elif clay >= 40 and silt >= 40:
                 textural_class = 11  # 'silty clay'
             elif clay >= 40 > silt and sand <= 45:
                 textural_class = 12
             else:
@@ -383,15 +284,15 @@
             if grid_type == 'sand':
                 array = array / 1000 * 100  # convert SSC from g/kg to % SSC
                 texture_data[0, :, :] = array
             elif grid_type == 'clay':
                 array = array / 1000 * 100  # convert SSC from g/kg to % SSC
                 texture_data[1, :, :] = array
 
-        soil_class = np.zeros((1, size[0], size[1]),dtype=int)
+        soil_class = np.zeros((1, size[0], size[1]), dtype=int)
 
         for i in range(0, size[0]):
             for j in range(0, size[1]):
                 # Organize array for input into packag
                 data = [texture_data[x, i, j] for x in np.arange(0, 2)]
                 sand = data[0]
                 clay = data[1]
@@ -408,19 +309,45 @@
         count = 1
         for key in soil_classification.keys():
             if key in classes:
                 filtered_classes[count] = soil_classification[key]
                 soil_class[soil_class == key] = int(count)
                 count += 1
 
-        # Need to re-write soil map so that classes start from 1 and sequentially there after
+        # Need to re-write soil map so that classes start from 1 and sequentially thereafter
         soi_raster = {'data': soil_class[0], 'profile': geo_tiff['profile']}
-        self.write_ascii(soi_raster, output_file,dtype='int16')
+        self.write_ascii(soi_raster, output_file, dtype='int16')
+
+        # create soil table with  nodata for rasyes
+        parameters = ['ID', 'Ks', 'thetaS', 'thetaR', 'm', 'PsiB', 'f', 'As', 'Au', 'n', 'ks', 'Cs', 'Texture']
+        soil_list = []
+        count = 1
+        nodata = 9999.99
+        ndefined = 'undefined'
+
+        for key, item in filtered_classes.items():
+            d = {}
+            for p in parameters:
+                # reset ID
+                if p == 'ID':
+                    d.update({p: count})
+                elif p == 'Texture':
+                    d.update({p: item})
+                # give textural class that need to be updated via user or calibration
+                elif p in (['As', 'Au', 'Cs', 'ks' ]):
+                    d.update({p: ndefined})
+
+                # set grid data to nodata value in table
+                else:
+                    d.update({p: nodata})
+            count += 1
+
+            soil_list.append(d)
 
-        return filtered_classes
+        return soil_list
 
     def process_raw_soil(self, grid_input, output=None, ks_only=False):
         """
         Writes ascii grids Ks, theta_s, theta_r, psib, and m from gridded soil data for % sand, silt, clay, bulk density, and volumetric water content at 33 and 1500 kPa.
 
         Parameters:
         - grid_input (list of dict or str): If a dictionary list, keys are "grid_type" and "path" for each soil property.
```

### Comparing `pytribs-0.2.0/pytRIBS/results/waterbalance.py` & `pytribs-0.3.0/pytRIBS/results/waterbalance.py`

 * *Files identical despite different names*

### Comparing `pytribs-0.2.0/pytRIBS.egg-info/PKG-INFO` & `pytribs-0.3.0/pytRIBS.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytRIBS
-Version: 0.2.0
+Version: 0.3.0
 Summary: A pre-to-post processing python package for the distributed hydrological model tRIBS
 Author-email: "L. Wren Raming" <lraming@asu.edu>, "C. Josh Cederstrom" <cjceders@asu.edu>, "Enrique R. Vivoni" <evivoni@asu.edu>
 License: GPL-version 2
 Project-URL: Repository, https://github.com/tribshms/pytRIBS
 Keywords: hydrology,modeling
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,14 +23,22 @@
 A pre-to-post processing python package designed to allow users to setup, simulate, and analyze TIN-based Real-time Integrated Basin Simulator (tRIBS) model runs through a python interface.
 Note this packages is currently under development and is subject to further changes. Additionally, much of the functionality here has had limited testing, consequently responsibility is on the user to verify package functionality. 
 
 ## Release/Version Notes
 PytRIBS uses semantic versioning. Currently, we are in the initial development phase--anything MAY change at any time and
 this package SHOULD NOT be considered stable.
 
+### Version 0.3.0 (5/03/2024)
+* Removed tmodel/tresults, replaced with classes
+* added new classes Soil, Mesh, Met, Land
+* renamed mixins folder to shared
+* created results/visualize.py
+* created soil/soil.py --moved soil related content from preprocess to here.
+* updated create_soil_map to return a soil table in .sdt format.
+* updated read/write soil tables to include options for including texture.
 ### Version 0.2.0 (4/25/2024)
 This minor update includes:
 * updates to the infile_mixin, with updates for 
 model documentation
 * addition of Paul Tol's colormaps (https://personal.sron.nl/~pault/)
 * In shared mixin:
   * added processor # to the attribute voronoi
```


# Comparing `tmp/relentless-0.1.0.tar.gz` & `tmp/relentless-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relentless-0.1.0.tar", last modified: Thu Nov 16 05:09:43 2023, max compression
+gzip compressed data, was "relentless-0.1.1.tar", last modified: Fri May  3 04:52:52 2024, max compression
```

## Comparing `relentless-0.1.0.tar` & `relentless-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:09:43.024511 relentless-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-11-16 05:09:34.000000 relentless-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-11-16 05:09:43.024511 relentless-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2023-11-16 05:09:34.000000 relentless-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-11-16 05:09:34.000000 relentless-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-11-16 05:09:43.024511 relentless-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 05:09:34.000000 relentless-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:09:43.016512 relentless-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:09:43.016512 relentless-0.1.0/src/relentless/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14066 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:09:43.020511 relentless-0.1.0/src/relentless/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/model/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    22878 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/model/extent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:09:43.020511 relentless-0.1.0/src/relentless/model/potential/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/model/potential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42225 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/model/potential/pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/model/potential/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)    33000 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/model/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10433 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:09:43.020511 relentless-0.1.0/src/relentless/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13279 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/optimize/criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    21541 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/optimize/method.py
--rw-r--r--   0 runner    (1001) docker     (127)    18179 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/optimize/objective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:09:43.020511 relentless-0.1.0/src/relentless/simulate/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/simulate/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/simulate/dilute.py
--rw-r--r--   0 runner    (1001) docker     (127)    58573 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/simulate/hoomd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9475 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/simulate/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    55932 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/simulate/lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/simulate/md.py
--rw-r--r--   0 runner    (1001) docker     (127)    23200 2023-11-16 05:09:34.000000 relentless-0.1.0/src/relentless/simulate/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:09:43.020511 relentless-0.1.0/src/relentless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-11-16 05:09:43.000000 relentless-0.1.0/src/relentless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-11-16 05:09:43.000000 relentless-0.1.0/src/relentless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 05:09:43.000000 relentless-0.1.0/src/relentless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-16 05:09:43.000000 relentless-0.1.0/src/relentless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-16 05:09:43.000000 relentless-0.1.0/src/relentless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:09:43.024511 relentless-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10351 2023-11-16 05:09:34.000000 relentless-0.1.0/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    12459 2023-11-16 05:09:34.000000 relentless-0.1.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2023-11-16 05:09:34.000000 relentless-0.1.0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2023-11-16 05:09:34.000000 relentless-0.1.0/tests/test_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:52:52.383819 relentless-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-03 04:52:42.000000 relentless-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-03 04:52:52.383819 relentless-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-03 04:52:42.000000 relentless-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-03 04:52:42.000000 relentless-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-03 04:52:52.383819 relentless-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 04:52:42.000000 relentless-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:52:52.375820 relentless-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:52:52.379819 relentless-0.1.1/src/relentless/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:52:52.379819 relentless-0.1.1/src/relentless/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/model/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22881 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/model/extent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:52:52.379819 relentless-0.1.1/src/relentless/model/potential/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/model/potential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42225 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/model/potential/pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/model/potential/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33001 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/model/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:52:52.379819 relentless-0.1.1/src/relentless/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/optimize/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/optimize/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18180 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/optimize/objective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:52:52.383819 relentless-0.1.1/src/relentless/simulate/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/simulate/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/simulate/dilute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62102 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/simulate/hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/simulate/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58530 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/simulate/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/simulate/md.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23201 2024-05-03 04:52:42.000000 relentless-0.1.1/src/relentless/simulate/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:52:52.383819 relentless-0.1.1/src/relentless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-03 04:52:52.000000 relentless-0.1.1/src/relentless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-03 04:52:52.000000 relentless-0.1.1/src/relentless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 04:52:52.000000 relentless-0.1.1/src/relentless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-03 04:52:52.000000 relentless-0.1.1/src/relentless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 04:52:52.000000 relentless-0.1.1/src/relentless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:52:52.383819 relentless-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-05-03 04:52:42.000000 relentless-0.1.1/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12460 2024-05-03 04:52:42.000000 relentless-0.1.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-03 04:52:42.000000 relentless-0.1.1/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-03 04:52:42.000000 relentless-0.1.1/tests/test_mpi.py
```

### Comparing `relentless-0.1.0/LICENSE` & `relentless-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `relentless-0.1.0/PKG-INFO` & `relentless-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relentless
-Version: 0.1.0
+Version: 0.1.1
 Summary: Computational materials design, with less code
 Home-page: https://github.com/mphowardlab/relentless
 Author: Michael P. Howard
 Author-email: mphoward@auburn.edu
 Project-URL: Documentation, https://relentless.readthedocs.io
 Project-URL: Source Code, https://github.com/mphowardlab/relentless
 Project-URL: Issue Tracker, https://github.com/mphowardlab/relentless/issues
```

### Comparing `relentless-0.1.0/README.rst` & `relentless-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `relentless-0.1.0/setup.cfg` & `relentless-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.1.1
 commit = False
 tag = False
 
 [bumpversion:file:src/relentless/__init__.py]
 
 [bumpversion:file:doc/source/conf.py]
```

### Comparing `relentless-0.1.0/src/relentless/collections.py` & `relentless-0.1.1/src/relentless/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     :toctree: generated/
 
     DefaultDict
     FixedKeyDict
     PairMatrix
 
 """
+
 import collections
 import copy
 
 
 class FixedKeyDict(collections.abc.MutableMapping):
     """Dictionary with fixed keys.
```

### Comparing `relentless-0.1.0/src/relentless/data.py` & `relentless-0.1.1/src/relentless/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 .. autosummary::
     :toctree: generated/
 
     Directory
 
 """
+
 import os
 import pathlib
 import shutil
 import uuid
 
 
 class Directory:
```

### Comparing `relentless-0.1.0/src/relentless/math.py` & `relentless-0.1.1/src/relentless/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     :toctree: generated/
 
     Interpolator
     AkimaSpline
     KeyedArray
 
 """
+
 import numpy
 import scipy.interpolate
 
 from .collections import FixedKeyDict
 
 
 class Interpolator:
```

### Comparing `relentless-0.1.0/src/relentless/model/__init__.py` & `relentless-0.1.1/src/relentless/model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     :toctree: generated/
 
     Variable
     Constant
     variable.VariableGraph
 
 """
+
 from . import potential
 from .ensemble import RDF, Ensemble
 from .extent import (
     Area,
     Cube,
     Cuboid,
     Extent,
```

### Comparing `relentless-0.1.0/src/relentless/model/ensemble.py` & `relentless-0.1.1/src/relentless/model/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 .. autoclass:: Ensemble
     :members:
 .. autoclass:: RDF
     :members:
 
 """
+
 import copy
 import json
 
 from relentless import math, mpi
 from relentless.collections import FixedKeyDict, PairMatrix
 
 from . import extent
```

### Comparing `relentless-0.1.0/src/relentless/model/extent.py` & `relentless-0.1.1/src/relentless/model/extent.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     [0.0 3.0 0.0]
     >>> print(v.c)
     [0.0 0.0 3.0]
     >>> print(v.extent)
     27.0
 
 """
+
 import abc
 
 import numpy
 
 
 class Extent(abc.ABC):
     r"""Abstract base class defining a region of space.
@@ -73,14 +74,15 @@
 
     A Volume can be any region of space; typically, it is a simulation "box."
     Any deriving class must implement the volume method that computes the scalar
     volume of the region. Additionally, methods to serialize and deserialize a
     Volume must be specified so that the object can be saved to disk.
 
     """
+
     pass
 
 
 class TriclinicBox(Volume):
     r"""Triclinic box.
 
     A TriclinicBox is defined by three edge vectors **a**, **b**, and **c** that form
@@ -480,14 +482,15 @@
 
     An Area can be any 2d region of space; typically, it is a simulation "box."
     Any deriving class must implement the volume method that computes the scalar
     area of the region. Additionally, methods to serialize and deserialize a
     Area must be specified so that the object can be saved to disk.
 
     """
+
     pass
 
 
 class ObliqueArea(Area):
     r"""Oblique area.
 
     An ObliqueArea is defined by two edge vectors **a** and **b** that form
```

### Comparing `relentless-0.1.0/src/relentless/model/potential/__init__.py` & `relentless-0.1.1/src/relentless/model/potential/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     Potential
     Parameters
     PairPotential
     PairParameters
 
 """
+
 from .pair import (
     Depletion,
     LennardJones,
     PairParameters,
     PairPotential,
     PairSpline,
     Yukawa,
```

### Comparing `relentless-0.1.0/src/relentless/model/potential/pair.py` & `relentless-0.1.1/src/relentless/model/potential/pair.py`

 * *Files identical despite different names*

### Comparing `relentless-0.1.0/src/relentless/model/potential/potential.py` & `relentless-0.1.1/src/relentless/model/potential/potential.py`

 * *Files identical despite different names*

### Comparing `relentless-0.1.0/src/relentless/model/variable.py` & `relentless-0.1.1/src/relentless/model/variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 distinguish between two types of variables: an :class:`IndependentVariable`, which
 does not depend on other variables, and a :class:`DependentVariable`, which does.
 Typically, the :class:`IndependentVariable` is a quantity that will be
 adjusted, while a :class:`DependentVariable` is a function of other
 these values.
 
 """
+
 import abc
 
 import networkx
 import numpy
 
 
 class Variable(abc.ABC):
```

### Comparing `relentless-0.1.0/src/relentless/mpi.py` & `relentless-0.1.1/src/relentless/mpi.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 .. autosummary::
     :toctree: generated/
     :nosignatures:
 
     Communicator
 
 """
+
 import json
 import os
 
 import numpy
 
 _mpi_env_hints = (
     "MV2_COMM_WORLD_LOCAL_RANK",
```

### Comparing `relentless-0.1.0/src/relentless/optimize/__init__.py` & `relentless-0.1.1/src/relentless/optimize/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     ObjectiveFunctionResult
     Optimizer
     ConvergenceTest
     LogicTest
 
 
 """
+
 from .criteria import (
     AllTest,
     AndTest,
     AnyTest,
     ConvergenceTest,
     GradientTest,
     LogicTest,
```

### Comparing `relentless-0.1.0/src/relentless/optimize/criteria.py` & `relentless-0.1.1/src/relentless/optimize/criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 .. autoclass:: AndTest
     :member-order: bysource
 
 .. autoclass:: OrTest
     :member-order: bysource
 
 """
+
 import abc
 
 import numpy
 
 from relentless import collections
 from relentless.model import variable
```

### Comparing `relentless-0.1.0/src/relentless/optimize/method.py` & `relentless-0.1.1/src/relentless/optimize/method.py`

 * *Files identical despite different names*

### Comparing `relentless-0.1.0/src/relentless/optimize/objective.py` & `relentless-0.1.1/src/relentless/optimize/objective.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 .. autoclass:: RelativeEntropy
     :member-order: bysource
     :members: compute,
         compute_gradient,
         target
 
 """
+
 import abc
 import json
 import tempfile
 
 import numpy
 import scipy.integrate
```

### Comparing `relentless-0.1.0/src/relentless/simulate/__init__.py` & `relentless-0.1.1/src/relentless/simulate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     Simulation
     SimulationOperation
     AnalysisOperation
     Barostat
     Thermostat
 
 """
+
 from .analyze import EnsembleAverage, Record, WriteTrajectory
 from .dilute import Dilute
 from .hoomd import HOOMD
 from .initialize import InitializeFromFile, InitializeRandomly
 from .lammps import LAMMPS
 from .md import (
     Barostat,
```

### Comparing `relentless-0.1.0/src/relentless/simulate/analyze.py` & `relentless-0.1.1/src/relentless/simulate/analyze.py`

 * *Files identical despite different names*

### Comparing `relentless-0.1.0/src/relentless/simulate/dilute.py` & `relentless-0.1.1/src/relentless/simulate/dilute.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 This module implements the :class:`Dilute` simulation backend and its specific
 operations. It is best to interface with these operations using the frontend in
 :mod:`relentless.simulate`.
 
 .. autoclass:: NullOperation
 
 """
+
 import abc
 
 import numpy
 
 from relentless import mpi
 from relentless.model import ensemble, extent
```

### Comparing `relentless-0.1.0/src/relentless/simulate/hoomd.py` & `relentless-0.1.1/src/relentless/simulate/hoomd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import enum
 import os
 import shutil
 import warnings
 
+import freud
 import gsd.hoomd
 import lammpsio
 import numpy
 import packaging.version
 
 from relentless import collections, mpi
 from relentless.model import ensemble, extent
@@ -45,21 +46,14 @@
 except AttributeError:
     _gsd_version = gsd.__version__
 if packaging.version.Version(_gsd_version) >= packaging.version.Version("2.8.0"):
     _gsd_write_mode = "w"
 else:
     _gsd_write_mode = "wb"
 
-try:
-    import freud
-
-    _freud_found = True
-except ImportError:
-    _freud_found = False
-
 
 # initializers
 class InitializationOperation(simulate.InitializationOperation):
     def __call__(self, sim):
         SimulationOperation.__call__(self, sim)
 
     def _call_v3(self, sim):
@@ -67,15 +61,14 @@
         sim.dimension = sim["engine"]["_hoomd"].state.box.dimensions
         sim.types = sim["engine"]["_hoomd"].state.particle_types
 
         # parse masses by type
         snap = sim["engine"]["_hoomd"].state.get_snapshot()
         sim.masses = self._get_masses_from_snapshot(sim, snap)
         self._assert_dimension_safe(sim, snap)
-
         # create the potentials, defer attaching until later
         neighbor_list = hoomd.md.nlist.Tree(buffer=sim.potentials.pair.neighbor_buffer)
         pair_potential = hoomd.md.pair.Table(nlist=neighbor_list)
         r, u, f = sim.potentials.pair.pairwise_energy_and_force(
             sim.types, tight=True, minimum_num=2
         )
         for i, j in sim.pairs:
@@ -208,15 +201,40 @@
                 gsd_filename = sim.directory.temporary_file(".gsd")
                 with gsd.hoomd.open(gsd_filename, _gsd_write_mode) as f:
                     f.append(frame)
             else:
                 gsd_filename = None
             gsd_filename = mpi.world.bcast(gsd_filename)
         else:
-            gsd_filename = self.filename
+            if mpi.world.rank_is_root:
+                gsd_filename = self.filename
+                with gsd.hoomd.open(self.filename) as trajectory:
+                    frame = trajectory[0]
+                    if frame.configuration.dimensions == 2:
+                        if (
+                            _hoomd_version.major >= 3
+                            and frame.configuration.box[2] != 0
+                        ):
+                            # fix for HOOMD 2 style used in HOOMD 3
+                            frame.configuration.box[2] = 0
+                            gsd_filename = sim.directory.temporary_file(".gsd")
+                            with gsd.hoomd.open(gsd_filename, _gsd_write_mode) as f:
+                                f.append(frame)
+                        elif (
+                            _hoomd_version.major == 2
+                            and frame.configuration.box[2] == 0
+                        ):
+                            # fix for HOOMD 3 style used in HOOMD 2
+                            frame.configuration.box[2] = 1
+                            gsd_filename = sim.directory.temporary_file(".gsd")
+                            with gsd.hoomd.open(gsd_filename, _gsd_write_mode) as f:
+                                f.append(frame)
+            else:
+                gsd_filename = None
+            gsd_filename = mpi.world.bcast(gsd_filename)
 
         return gsd_filename
 
 
 class InitializeRandomly(InitializationOperation):
     """Initialize a randomly generated simulation box.
 
@@ -1108,15 +1126,21 @@
 
     _get_rdf_params = analyze.EnsembleAverage._get_rdf_params
 
     class EnsembleAverageAction(Action):
         flags = [Action.Flags.PRESSURE_TENSOR]
 
         def __init__(
-            self, types, dimension, thermo, system, rdf_params=None, constraints=None
+            self,
+            types,
+            dimension,
+            thermo,
+            system,
+            rdf_params=None,
+            constraints=None,
         ):
             if dimension not in (2, 3):
                 raise ValueError("Only 2 or 3 dimensions supported")
 
             self.types = types
             self.dimension = dimension
             self.thermo = thermo
@@ -1156,65 +1180,83 @@
                     snap = self.system.get_snapshot()
                 elif _hoomd_version.major == 2:
                     snap = self.system.take_snapshot()
                 else:
                     raise NotImplementedError(f"HOOMD {_hoomd_version} not supported")
 
                 if mpi.world.rank == 0:
-                    if _hoomd_version.major == 3:
-                        dimensions = snap.configuration.dimensions
-                        box_array = numpy.array(snap.configuration.box)
-                    elif _hoomd_version.major == 2:
-                        dimensions = snap.box.dimensions
-                        box_array = numpy.array(
-                            [
-                                snap.box.Lx,
-                                snap.box.Ly,
-                                snap.box.Lz,
-                                snap.box.xy,
-                                snap.box.xz,
-                                snap.box.yz,
-                            ]
-                        )
-                        if snap.box.dimensions == 2:
-                            box_array[2] = 0.0
-                            box_array[-2:] = 0.0
-                    else:
-                        raise NotImplementedError(
-                            f"HOOMD {_hoomd_version} not supported"
-                        )
-
-                    box = freud.box.Box.from_box(box_array, dimensions=dimensions)
-                    # pre build aabbs per type and count particles by type
-                    aabbs = {}
+                    # compute number of particles of each type
+                    # save type masks for use in RDF calculations if needed
                     type_masks = {}
+                    N = {}
                     for i in self.types:
-                        type_masks[
-                            i
-                        ] = snap.particles.typeid == snap.particles.types.index(i)
+                        type_masks[i] = (
+                            snap.particles.typeid == snap.particles.types.index(i)
+                        )
                         if "N" not in self.constraints:
-                            self._N[i] += numpy.sum(type_masks[i])
+                            N[i] = numpy.sum(type_masks[i])
+                            self._N[i] += N[i]
+                        else:
+                            N[i] = self.constraints["N"][i]
 
-                        if compute_rdf:
-                            aabbs[i] = freud.locality.AABBQuery(
-                                box, snap.particles.position[type_masks[i]]
-                            )
-                    # then do rdfs using the AABBs
+                    # then do rdf if requested
                     if compute_rdf:
-                        for i, j in self._rdf:
-                            query_args = dict(self._rdf[i, j].default_query_args)
-                            query_args.update(exclude_ii=(i == j))
-                            # resetting when the samples are zero clears the RDF
-                            self._rdf[i, j].compute(
-                                aabbs[j],
-                                snap.particles.position[type_masks[i]],
-                                neighbors=query_args,
-                                reset=(self.num_samples == 0),
+                        if _hoomd_version.major == 3:
+                            dimensions = snap.configuration.dimensions
+                            box_array = numpy.array(snap.configuration.box)
+                        elif _hoomd_version.major == 2:
+                            dimensions = snap.box.dimensions
+                            box_array = numpy.array(
+                                [
+                                    snap.box.Lx,
+                                    snap.box.Ly,
+                                    snap.box.Lz,
+                                    snap.box.xy,
+                                    snap.box.xz,
+                                    snap.box.yz,
+                                ]
+                            )
+                            if snap.box.dimensions == 2:
+                                box_array[2] = 0.0
+                                box_array[-2:] = 0.0
+                        else:
+                            raise NotImplementedError(
+                                f"HOOMD {_hoomd_version} not supported"
                             )
+                        box = freud.box.Box.from_box(box_array, dimensions=dimensions)
 
+                        # calculate average density per type
+                        for i in self.types:
+                            self._rdf_density[i] += N[i] / box.volume
+                            self._rdf_num_origins[i] += N[i]
+
+                        # build aabb of all particles and generate a parent
+                        # neighbor list with the RDF cutoff
+                        aabb = freud.locality.AABBQuery(box, snap.particles.position)
+                        neighbors = aabb.query(
+                            snap.particles.position,
+                            dict(
+                                mode="ball",
+                                r_max=self.rdf_params["stop"],
+                                exclude_ii=True,
+                            ),
+                        ).toNeighborList()
+
+                        for i in self.types:
+                            for j in self.types:
+                                filter_ij = numpy.logical_and(
+                                    type_masks[i][neighbors[:, 0]],
+                                    type_masks[j][neighbors[:, 1]],
+                                )
+                                counts, _ = numpy.histogram(
+                                    neighbors.distances[filter_ij],
+                                    bins=self.rdf_params["bins"],
+                                    range=(0, self.rdf_params["stop"]),
+                                )
+                                self._rdf_counts[i, j] += counts
             self.num_samples += 1
             if compute_rdf:
                 self.num_rdf_samples += 1
 
         def reset(self):
             """Resets sample number, ``T``, ``P``, and all ``V`` parameters to 0."""
             self._T = 0.0
@@ -1232,23 +1274,28 @@
                 self._V = {"Lx": 0.0, "Ly": 0.0, "xy": 0.0}
 
             self._N = collections.FixedKeyDict(self.types)
             for i in self.types:
                 self._N[i] = 0
 
             if self.rdf_params is not None:
-                self._rdf = collections.PairMatrix(self.types)
-                for i, j in self._rdf:
-                    self._rdf[i, j] = freud.density.RDF(
-                        bins=self.rdf_params["bins"],
-                        r_max=self.rdf_params["stop"],
-                        normalize=(i == j),
-                    )
+                self._rdf_counts = {}
+                self._rdf_density = {}
+                self._rdf_num_origins = {}
+                for i in self.types:
+                    self._rdf_density[i] = 0
+                    self._rdf_num_origins[i] = 0
+                    for j in self.types:
+                        self._rdf_counts[i, j] = numpy.zeros(
+                            self.rdf_params["bins"], dtype=int
+                        )
             else:
-                self._rdf = None
+                self._rdf_counts = None
+                self._rdf_density = None
+                self._rdf_num_origins = None
 
             self.num_samples = 0
             self.num_rdf_samples = 0
 
         @property
         def T(self):
             """float: Average temperature across samples."""
@@ -1309,24 +1356,57 @@
 
         @property
         def rdf(self):
             """:class:`~relentless.collections.PairMatrix`:
             Radial distribution functions.
             """
             if self.num_rdf_samples > 0:
+                bin_edges = numpy.linspace(
+                    0, self.rdf_params["stop"], self.rdf_params["bins"] + 1
+                )
+                bin_centers = 0.5 * (bin_edges[:-1] + bin_edges[1:])
+                if self.dimension == 3:
+                    bin_extents = (4 * numpy.pi / 3) * (
+                        bin_edges[1:] ** 3 - bin_edges[:-1] ** 3
+                    )
+                elif self.dimension == 2:
+                    bin_extents = numpy.pi * (bin_edges[1:] ** 2 - bin_edges[:-1] ** 2)
+
                 rdf = collections.PairMatrix(self.types)
-                for pair in rdf:
+                for i, j in rdf:
                     if mpi.world.rank == 0:
-                        gr = numpy.column_stack(
-                            (self._rdf[pair].bin_centers, self._rdf[pair].rdf)
-                        )
+                        density = {
+                            k: self._rdf_density[k] / self.num_rdf_samples
+                            for k in self.types
+                        }
+                        g = numpy.zeros_like(bin_centers)
+                        if i == j:
+                            if self._rdf_num_origins[i] > 0 and density[i] > 0:
+                                g = self._rdf_counts[i, i] / (
+                                    self._rdf_num_origins[i] * density[i] * bin_extents
+                                )
+                        else:
+                            # this takes the weighted average of g_ij and g_ji
+                            num_ij_origins = (
+                                self._rdf_num_origins[i] + self._rdf_num_origins[j]
+                            )
+                            if num_ij_origins > 0:
+                                if density[j] > 0:
+                                    g += self._rdf_counts[i, j] / (
+                                        num_ij_origins * density[j] * bin_extents
+                                    )
+                                if density[i] > 0:
+                                    g += self._rdf_counts[j, i] / (
+                                        num_ij_origins * density[i] * bin_extents
+                                    )
+                        gr = numpy.column_stack((bin_centers, g))
                     else:
                         gr = None
                     gr = mpi.world.bcast_numpy(gr, root=0)
-                    rdf[pair] = ensemble.RDF(gr[:, 0], gr[:, 1])
+                    rdf[i, j] = ensemble.RDF(gr[:, 0], gr[:, 1])
                 return rdf
             else:
                 return None
 
 
 class Record(AnalysisOperation):
     def __init__(self, filename, every, quantities):
@@ -1504,48 +1584,34 @@
     A simulation is performed using
     `HOOMD-blue <https://hoomd-blue.readthedocs.io/en/stable>`_.
     HOOMD-blue is a molecular dynamics program that can execute on both CPUs and
     GPUs, as a single process or with MPI parallelism. The launch configuration
     will be automatically selected for you when the simulation is run. Both
     HOOMD 2.x and 3.x are supported.
 
-    The `freud <https://freud.readthedocs.io>`_ analysis package (version 2.x)
-    is also required for initialization and analysis. To use this simulation backend,
-    you will need to install both :mod:`hoomd` and :mod:`freud` into your Python
-    environment. :mod:`hoomd` is available through conda-forge or can be built
-    from source, while :mod`freud` is available through both PyPI and conda-forge.
-    Please refer to the package documentation for details of how to install these.
-
     .. warning::
 
         HOOMD requires that tabulated pair potentials be finite. A common place to
         have an infinite value is at :math:`r=0`, since potentials like
         :class:`~relentless.potential.pair.LennardJones` diverge there. You should
         make sure to exclude these values from the tabulated potentials,
         e.g., setting :attr:`~relentless.simulate.PairPotentialTabulator.rmin` to a
         small value larger than 0.
 
     Raises
     ------
     ImportError
         If the :mod:`hoomd` package is not found or is not version 2.x.
-    ImportError
-        If the :mod:`freud` package is not found or is not version 2.x.
 
     """
 
     def __init__(self, initializer, operations=None):
         if not _hoomd_found:
             raise ImportError("HOOMD not found.")
 
-        if not _freud_found:
-            raise ImportError("freud not found.")
-        elif packaging.version.parse(freud.__version__).major != 2:
-            raise ImportError("Only freud 2.x is supported.")
-
         super().__init__(initializer, operations)
 
     def _initialize_engine(self, sim):
         sim["engine"]["version"] = _hoomd_version
 
         if _hoomd_version.major == 3:
             device = hoomd.device.auto_select(
```

### Comparing `relentless-0.1.0/src/relentless/simulate/initialize.py` & `relentless-0.1.1/src/relentless/simulate/initialize.py`

 * *Files identical despite different names*

### Comparing `relentless-0.1.0/src/relentless/simulate/lammps.py` & `relentless-0.1.1/src/relentless/simulate/lammps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1123,22 +1123,24 @@
 
         # extract rdfs from trajectory
         if "_rdf_params" in sim[self]:
             sim[self]["_rdf_dump"].process(sim, sim_op)
             rdf = collections.PairMatrix(sim.types)
             num_rdf_samples = 0
             if mpi.world.rank_is_root:
-                rdf_ = collections.PairMatrix(sim.types)
-                for i, j in rdf_:
-                    rdf_[i, j] = freud.density.RDF(
-                        bins=sim[self]["_rdf_params"]["bins"],
-                        r_max=sim[self]["_rdf_params"]["stop"],
-                        normalize=(i == j),
-                    )
-
+                _rdf_counts = {}
+                _rdf_density = {}
+                _rdf_num_origins = {}
+                for i in sim.types:
+                    _rdf_density[i] = 0
+                    _rdf_num_origins[i] = 0
+                    for j in sim.types:
+                        _rdf_counts[i, j] = numpy.zeros(
+                            sim[self]["_rdf_params"]["bins"], dtype=int
+                        )
                 traj = lammpsio.DumpFile(sim[self]["_rdf_file"])
                 for snap in traj:
                     # get freud box
                     L = snap.box.high - snap.box.low
                     tilt = snap.box.tilt
                     if tilt is not None:
                         # scale tilt factors to HOOMD convention
@@ -1152,39 +1154,84 @@
                         [L[0], L[1], L[2], tilt[0], tilt[1], tilt[2]]
                     )
                     if sim.dimension == 2:
                         box_array[2] = 0.0
                         box_array[-2:] = 0.0
                     box = freud.box.Box.from_box(box_array, dimensions=sim.dimension)
 
-                    # pre build aabbs per type and count particles by type
-                    aabbs = {}
+                    # determine type masks for RDF calculations
+                    # number of particles of each type was already determined above
                     type_masks = {}
                     for i in sim.types:
                         type_masks[i] = snap.typeid == sim["engine"]["types"][i]
-                        aabbs[i] = freud.locality.AABBQuery(
-                            box, snap.position[type_masks[i]]
-                        )
+                    # build aabb of all particles and generate a parent
+                    # neighbor list with the RDF cutoff
+                    aabb = freud.locality.AABBQuery(box, snap.position)
+                    neighbors = aabb.query(
+                        snap.position,
+                        dict(
+                            mode="ball",
+                            r_max=sim[self]["_rdf_params"]["stop"],
+                            exclude_ii=True,
+                        ),
+                    ).toNeighborList()
+                    for i in sim.types:
+                        _rdf_density[i] += N[i] / box.volume
+                        _rdf_num_origins[i] += N[i]
+                        for j in sim.types:
+                            filter_ij = numpy.logical_and(
+                                type_masks[i][neighbors[:, 0]],
+                                type_masks[j][neighbors[:, 1]],
+                            )
+                            counts, _ = numpy.histogram(
+                                neighbors.distances[filter_ij],
+                                bins=sim[self]["_rdf_params"]["bins"],
+                                range=(0, sim[self]["_rdf_params"]["stop"]),
+                            )
+                            _rdf_counts[i, j] += counts
                     # then do rdfs using the AABBs
-                    for i, j in rdf_:
-                        query_args = dict(rdf_[i, j].default_query_args)
-                        query_args.update(exclude_ii=(i == j))
-                        rdf_[i, j].compute(
-                            aabbs[j],
-                            snap.position[type_masks[i]],
-                            neighbors=query_args,
-                            reset=False,
-                        )
 
                     num_rdf_samples += 1
 
-                for pair in rdf:
-                    rdf[pair] = numpy.column_stack(
-                        (rdf_[pair].bin_centers, rdf_[pair].rdf)
-                    )
+                for i, j in rdf:
+                    if num_rdf_samples > 0:
+                        bin_edges = numpy.linspace(
+                            0,
+                            sim[self]["_rdf_params"]["stop"],
+                            sim[self]["_rdf_params"]["bins"] + 1,
+                        )
+                        bin_centers = 0.5 * (bin_edges[:-1] + bin_edges[1:])
+                    if sim.dimension == 3:
+                        bin_extents = (4 * numpy.pi / 3) * (
+                            bin_edges[1:] ** 3 - bin_edges[:-1] ** 3
+                        )
+                    elif sim.dimension == 2:
+                        bin_extents = numpy.pi * (
+                            bin_edges[1:] ** 2 - bin_edges[:-1] ** 2
+                        )
+                    density = {k: _rdf_density[k] / num_rdf_samples for k in sim.types}
+                    g = numpy.zeros_like(bin_centers)
+                    if i == j:
+                        if _rdf_num_origins[i] > 0 and density[i] > 0:
+                            g = _rdf_counts[i, i] / (
+                                _rdf_num_origins[i] * density[i] * bin_extents
+                            )
+                    else:
+                        # this takes the weighted average of g_ij and g_ji
+                        num_ij_origins = _rdf_num_origins[i] + _rdf_num_origins[j]
+                        if num_ij_origins > 0:
+                            if density[j] > 0:
+                                g += _rdf_counts[i, j] / (
+                                    num_ij_origins * density[j] * bin_extents
+                                )
+                            if density[i] > 0:
+                                g += _rdf_counts[j, i] / (
+                                    num_ij_origins * density[i] * bin_extents
+                                )
+                    rdf[i, j] = numpy.column_stack((bin_centers, g))
             # sync across ranks and convert to RDF object
             num_rdf_samples = mpi.world.bcast(num_rdf_samples)
             for pair in rdf:
                 gr = mpi.world.bcast_numpy(rdf[pair])
                 ens.rdf[pair] = ensemble.RDF(gr[:, 0], gr[:, 1])
 
             del sim[self]["_rdf_dump"]
@@ -1419,15 +1466,14 @@
     enabled; however, it will typically be a bit slower than running LAMMPS via
     Python. To run LAMMPS as an executable with MPI support, you should **not**
     launch ``relentless`` with ``mpirexec``, and instead should include the
     ``mpiexec` command and options in the ``executable``::
 
         relentless.simulate.LAMMPS(init, ops, executable="mpiexec -n 8 lmp_mpi")
 
-
     .. warning::
 
         LAMMPS requires that tabulated pair potentials do not include an entry for
         :math:`r = 0`. Make sure to set
         :attr:`~relentless.simulate.PairPotentialTabulator.rmin` to a small value
         larger than 0.
```

### Comparing `relentless-0.1.0/src/relentless/simulate/md.py` & `relentless-0.1.1/src/relentless/simulate/md.py`

 * *Files identical despite different names*

### Comparing `relentless-0.1.0/src/relentless/simulate/simulate.py` & `relentless-0.1.1/src/relentless/simulate/simulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Simulation interface
 ====================
 
 See :mod:`relentless.simulate` for module level documentation.
 
 """
+
 import abc
 
 import numpy
 
 from relentless import collections, data, mpi
 from relentless.model import variable
```

### Comparing `relentless-0.1.0/src/relentless.egg-info/PKG-INFO` & `relentless-0.1.1/src/relentless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relentless
-Version: 0.1.0
+Version: 0.1.1
 Summary: Computational materials design, with less code
 Home-page: https://github.com/mphowardlab/relentless
 Author: Michael P. Howard
 Author-email: mphoward@auburn.edu
 Project-URL: Documentation, https://relentless.readthedocs.io
 Project-URL: Source Code, https://github.com/mphowardlab/relentless
 Project-URL: Issue Tracker, https://github.com/mphowardlab/relentless/issues
```

### Comparing `relentless-0.1.0/src/relentless.egg-info/SOURCES.txt` & `relentless-0.1.1/src/relentless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relentless-0.1.0/tests/test_collections.py` & `relentless-0.1.1/tests/test_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit tests for collections module."""
+
 import unittest
 
 import relentless
 
 
 class test_FixedKeyDict(unittest.TestCase):
     """Unit tests for relentless.collections.FixedKeyDict."""
```

### Comparing `relentless-0.1.0/tests/test_data.py` & `relentless-0.1.1/tests/test_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit tests for core.data module."""
+
 import os
 import shutil
 import tempfile
 import unittest
 
 import relentless
```

### Comparing `relentless-0.1.0/tests/test_math.py` & `relentless-0.1.1/tests/test_math.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit tests for core.math module."""
+
 import unittest
 
 import numpy
 
 import relentless
```

### Comparing `relentless-0.1.0/tests/test_mpi.py` & `relentless-0.1.1/tests/test_mpi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit tests for mpi module."""
+
 import os
 import tempfile
 import unittest
 
 import numpy
 
 import relentless
```


# Comparing `tmp/rosetta-soil-0.1.1.tar.gz` & `tmp/rosetta_soil-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-soil-0.1.1.tar", last modified: Wed Jun 23 01:19:53 2021, max compression
+gzip compressed data, was "rosetta_soil-0.1.2.tar", last modified: Fri May  3 00:16:48 2024, max compression
```

## Comparing `rosetta-soil-0.1.1.tar` & `rosetta_soil-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 tskaggs   (1000) tskaggs   (1000)        0 2021-06-23 01:19:53.014685 rosetta-soil-0.1.1/
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)    18093 2020-12-16 02:04:07.000000 rosetta-soil-0.1.1/LICENSE
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)      210 2021-06-22 23:50:34.000000 rosetta-soil-0.1.1/LICENSE.notes
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)     1014 2021-06-23 01:19:53.014685 rosetta-soil-0.1.1/PKG-INFO
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)     9933 2021-06-23 00:51:59.000000 rosetta-soil-0.1.1/README.rst
-drwxrwxr-x   0 tskaggs   (1000) tskaggs   (1000)        0 2021-06-23 01:19:53.006685 rosetta-soil-0.1.1/rosetta/
--rwxr-xr-x   0 tskaggs   (1000) tskaggs   (1000)    29925 2021-06-22 14:34:03.000000 rosetta-soil-0.1.1/rosetta/ANN_Module.py
--rwxr-xr-x   0 tskaggs   (1000) tskaggs   (1000)     3925 2020-12-16 02:04:07.000000 rosetta-soil-0.1.1/rosetta/DB_Module.py
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)       62 2021-06-18 22:30:57.000000 rosetta-soil-0.1.1/rosetta/__init__.py
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)       22 2021-06-23 01:18:01.000000 rosetta-soil-0.1.1/rosetta/__version__.py
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)     7897 2021-06-22 15:59:43.000000 rosetta-soil-0.1.1/rosetta/rosetta.py
-drwxrwxr-x   0 tskaggs   (1000) tskaggs   (1000)        0 2021-06-23 01:19:53.006685 rosetta-soil-0.1.1/rosetta/sqlite/
--rw-r--r--   0 tskaggs   (1000) tskaggs   (1000) 11145216 2020-12-16 02:04:07.000000 rosetta-soil-0.1.1/rosetta/sqlite/Rosetta.sqlite
-drwxrwxr-x   0 tskaggs   (1000) tskaggs   (1000)        0 2021-06-23 01:19:53.014685 rosetta-soil-0.1.1/rosetta_soil.egg-info/
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)     1014 2021-06-23 01:19:52.000000 rosetta-soil-0.1.1/rosetta_soil.egg-info/PKG-INFO
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)      390 2021-06-23 01:19:53.000000 rosetta-soil-0.1.1/rosetta_soil.egg-info/SOURCES.txt
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)        1 2021-06-23 01:19:52.000000 rosetta-soil-0.1.1/rosetta_soil.egg-info/dependency_links.txt
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)        1 2021-06-23 00:05:01.000000 rosetta-soil-0.1.1/rosetta_soil.egg-info/not-zip-safe
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)        6 2021-06-23 01:19:52.000000 rosetta-soil-0.1.1/rosetta_soil.egg-info/requires.txt
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)        8 2021-06-23 01:19:52.000000 rosetta-soil-0.1.1/rosetta_soil.egg-info/top_level.txt
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)       38 2021-06-23 01:19:53.014685 rosetta-soil-0.1.1/setup.cfg
--rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)     1432 2021-06-23 01:09:13.000000 rosetta-soil-0.1.1/setup.py
+drwxrwxr-x   0 tskaggs   (1000) tskaggs   (1000)        0 2024-05-03 00:16:48.588568 rosetta_soil-0.1.2/
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)    18093 2020-12-16 02:04:07.000000 rosetta_soil-0.1.2/LICENSE
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)      210 2021-06-22 23:50:34.000000 rosetta_soil-0.1.2/LICENSE.notes
+-rw-r--r--   0 tskaggs   (1000) tskaggs   (1000)      867 2024-05-03 00:16:48.588568 rosetta_soil-0.1.2/PKG-INFO
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)     9941 2021-06-23 13:24:38.000000 rosetta_soil-0.1.2/README.rst
+drwxrwxr-x   0 tskaggs   (1000) tskaggs   (1000)        0 2024-05-03 00:16:48.572568 rosetta_soil-0.1.2/rosetta/
+-rwxr-xr-x   0 tskaggs   (1000) tskaggs   (1000)    29925 2021-06-22 14:34:03.000000 rosetta_soil-0.1.2/rosetta/ANN_Module.py
+-rwxr-xr-x   0 tskaggs   (1000) tskaggs   (1000)     3925 2020-12-16 02:04:07.000000 rosetta_soil-0.1.2/rosetta/DB_Module.py
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)       62 2021-06-18 22:30:57.000000 rosetta_soil-0.1.2/rosetta/__init__.py
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)       22 2024-05-03 00:08:17.000000 rosetta_soil-0.1.2/rosetta/__version__.py
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)     7919 2024-05-03 00:08:17.000000 rosetta_soil-0.1.2/rosetta/rosetta.py
+drwxrwxr-x   0 tskaggs   (1000) tskaggs   (1000)        0 2024-05-03 00:16:48.576568 rosetta_soil-0.1.2/rosetta/sqlite/
+-rw-r--r--   0 tskaggs   (1000) tskaggs   (1000) 11145216 2020-12-16 02:04:07.000000 rosetta_soil-0.1.2/rosetta/sqlite/Rosetta.sqlite
+drwxrwxr-x   0 tskaggs   (1000) tskaggs   (1000)        0 2024-05-03 00:16:48.588568 rosetta_soil-0.1.2/rosetta_soil.egg-info/
+-rw-r--r--   0 tskaggs   (1000) tskaggs   (1000)      867 2024-05-03 00:16:48.000000 rosetta_soil-0.1.2/rosetta_soil.egg-info/PKG-INFO
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)      412 2024-05-03 00:16:48.000000 rosetta_soil-0.1.2/rosetta_soil.egg-info/SOURCES.txt
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)        1 2024-05-03 00:16:48.000000 rosetta_soil-0.1.2/rosetta_soil.egg-info/dependency_links.txt
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)        1 2021-06-23 00:05:01.000000 rosetta_soil-0.1.2/rosetta_soil.egg-info/not-zip-safe
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)        6 2024-05-03 00:16:48.000000 rosetta_soil-0.1.2/rosetta_soil.egg-info/requires.txt
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)        8 2024-05-03 00:16:48.000000 rosetta_soil-0.1.2/rosetta_soil.egg-info/top_level.txt
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)       38 2024-05-03 00:16:48.588568 rosetta_soil-0.1.2/setup.cfg
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)     1286 2024-05-03 00:08:17.000000 rosetta_soil-0.1.2/setup.py
+drwxrwxr-x   0 tskaggs   (1000) tskaggs   (1000)        0 2024-05-03 00:16:48.588568 rosetta_soil-0.1.2/tests/
+-rw-rw-r--   0 tskaggs   (1000) tskaggs   (1000)     7313 2024-05-03 00:08:17.000000 rosetta_soil-0.1.2/tests/test_rosetta.py
```

### Comparing `rosetta-soil-0.1.1/LICENSE` & `rosetta_soil-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-soil-0.1.1/README.rst` & `rosetta_soil-0.1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             [20, 60, 20],
             [55, 25, 20, 1.1],
         ]
     }
 
     def url(rosetta_version: int) -> str:
         return f"http://www.handbook60.org/api/v1/rosetta/{rosetta_version}"
+
     r = requests.post(url(3), json=data)
 
 returns the following::
 
     print(r.json())
 
     {'model_codes': [5, 2, 3], 'rosetta_version': 3, 'stdev': 
@@ -96,15 +97,15 @@
 
 Rosetta provides four models for predicting the five parameters from soil
 characterization data. The models differ in the required input data
 
 +------------+------------------------+
 | Model Code | Input Data             |
 +============+========================+
-|      2     | sa, si, cl (SSC) |
+|      2     | sa, si, cl (SSC)       |
 +------------+------------------------+
 |      3     | SSC, bulk density (BD) |
 +------------+------------------------+
 |      4     | SSC, BD, th33          |
 +------------+------------------------+
 |      5     | SSC, BD, th33, th1500  |
 +------------+------------------------+
@@ -215,15 +216,15 @@
 +------+--------------------------------------------------------+
 |   -1 | no result returned, inadequate or erroneous data       |
 +------+--------------------------------------------------------+
 
 Alternative usage
 -----------------
 
-Predictions can also be made using the Rostta class
+Predictions can also be made using the Rosetta class
 ::
 
     import numpy as np
     from rosetta import Rosetta
 
 The class is instantiated for a particular Rosetta version and model.
 Predictions are then made using a numpy array of soil data.
```

### Comparing `rosetta-soil-0.1.1/rosetta/ANN_Module.py` & `rosetta_soil-0.1.2/rosetta/ANN_Module.py`

 * *Files identical despite different names*

### Comparing `rosetta-soil-0.1.1/rosetta/DB_Module.py` & `rosetta_soil-0.1.2/rosetta/DB_Module.py`

 * *Files identical despite different names*

### Comparing `rosetta-soil-0.1.1/rosetta/rosetta.py` & `rosetta_soil-0.1.2/rosetta/rosetta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
-import pkg_resources
+from importlib import resources
 from typing import NamedTuple, Sequence, Tuple, Union, Optional, List
+from . import sqlite
 
 import numpy as np
 
 from . import ANN_Module
 from . import DB_Module
 
 Array1D = Union[np.ndarray]
 Array2D = Union[np.ndarray]
 
-ROSETTA_DB = pkg_resources.resource_filename("rosetta", "sqlite/Rosetta.sqlite")
 ROSETTA_VERSIONS = {1, 2, 3}
 ROSETTA_MODEL_CODES = {2, 3, 4, 5}
 ROSE2_COEFFICIENTS = {
     2: [(0.969, 0.000), (1.103, -0.048), (1.050, 0.159), (0.655, 0.004)],
     3: [(0.995, 0.000), (1.000, 0.002), (1.028, 0.162), (0.660, 0.003)],
     4: [(1.156, 0.000), (0.974, 0.011), (1.039, 0.067), (0.796, 0.006)],
     5: [(1.220, 0.000), (1.045, -0.020), (0.956, -0.040), (0.877, -0.003)],
@@ -86,21 +86,21 @@
             self.is_valid_fieldcap(),
             self.is_valid_fieldcap_and_wiltpoint(),
         ]
         return all(tests[: index - 2])
 
     def best_index(self) -> int:
         """Max value of index for which self.is_valid(index) is True."""
-        count = 0
+        best = 0
         for index in range(3, len(self) + 1):
             if self.is_valid(index):
-                count = index
+                best = index
             else:
                 break
-        return count
+        return best
 
 
 class SoilData(List[SoilDatum]):
     @classmethod
     def from_array(cls, array: Array2D) -> SoilData:
         return SoilData([SoilDatum(*to_floats(row)) for row in array])
 
@@ -117,15 +117,16 @@
         if rosetta_version not in ROSETTA_VERSIONS:
             raise RosettaError(f"rosetta_version must be in {ROSETTA_VERSIONS}")
         if model_code not in ROSETTA_MODEL_CODES:
             raise RosettaError(f"model_code must be in {ROSETTA_MODEL_CODES}")
         self.rosetta_version = rosetta_version
         self.model_code = model_code
         code = model_code if rosetta_version == 3 else model_code + 100
-        with DB_Module.DB(0, 0, 0, sqlite_path=ROSETTA_DB) as db:
+        rosetta_db_path = resources.files(sqlite) / 'Rosetta.sqlite'
+        with DB_Module.DB(0, 0, 0, sqlite_path=rosetta_db_path) as db:
             self.ptf_model = ANN_Module.PTF_MODEL(code, db)
 
     def predict(self, X: Array2D) -> Tuple[Array2D, Array2D]:
         predicted_params = self.ptf_model.predict(X.T, sum_data=True)
         mean = predicted_params["sum_res_mean"].T
         stdev = predicted_params["sum_res_std"].T
```

### Comparing `rosetta-soil-0.1.1/rosetta/sqlite/Rosetta.sqlite` & `rosetta_soil-0.1.2/rosetta/sqlite/Rosetta.sqlite`

 * *Files identical despite different names*

### Comparing `rosetta-soil-0.1.1/setup.py` & `rosetta_soil-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,22 +21,19 @@
     name="rosetta-soil",
     version=version["__version__"],
     description=SHORT,
     long_description=LONG,
     url="https://github.com/usda-ars-ussl/rosetta-soil",
     packages=["rosetta"],
     package_data={"rosetta": ["sqlite/Rosetta.sqlite"]},
-    python_requires=">=3.7",
+    python_requires=">=3.10",
     install_requires=["numpy"],
     zip_safe=False,
     license="License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
     author="Todd Skaggs",
     author_email="todd.skaggs@usda.gov",
     classifiers=[
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
     ],
 )
```


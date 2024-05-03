# Comparing `tmp/geojikuu-0.27.53.tar.gz` & `tmp/geojikuu-0.27.54.tar.gz`

## Comparing `geojikuu-0.27.53.tar` & `geojikuu-0.27.54.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.53/VERSION v0.27.53.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.53/__init__.py.txt
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 geojikuu-0.27.53/pyproject.toml.bak
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/aggregation/__init__.py.txt
--rw-r--r--   0        0        0    40348 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/aggregation/point_aggregators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/descriptives/__init__.py.txt
--rw-r--r--   0        0        0    11640 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/descriptives/spacetime_distribution.py
--rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/descriptives/spatial_distribution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/hypothesis_testing/__init__.py.txt
--rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/hypothesis_testing/autocorrelation.py
--rw-r--r--   0        0        0    17754 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/hypothesis_testing/hot_spot_analysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/preprocessing/__init__.py.txt
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/preprocessing/conversion_tools.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/preprocessing/normalisation.py
--rw-r--r--   0        0        0    18814 2020-02-02 00:00:00.000000 geojikuu-0.27.53/geojikuu/preprocessing/projection.py
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 geojikuu-0.27.53/LICENSE.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.53/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 geojikuu-0.27.53/pyproject.toml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 geojikuu-0.27.53/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.54/VERSION v0.27.54.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.54/__init__.py.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/aggregation/__init__.py.txt
+-rw-r--r--   0        0        0    40357 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/aggregation/point_aggregators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/descriptives/__init__.py.txt
+-rw-r--r--   0        0        0    11640 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/descriptives/spacetime_distribution.py
+-rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/descriptives/spatial_distribution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/hypothesis_testing/__init__.py.txt
+-rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/hypothesis_testing/autocorrelation.py
+-rw-r--r--   0        0        0    17754 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/hypothesis_testing/hot_spot_analysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/preprocessing/__init__.py.txt
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/preprocessing/conversion_tools.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/preprocessing/normalisation.py
+-rw-r--r--   0        0        0    18814 2020-02-02 00:00:00.000000 geojikuu-0.27.54/geojikuu/preprocessing/projection.py
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 geojikuu-0.27.54/LICENSE.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geojikuu-0.27.54/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 geojikuu-0.27.54/pyproject.toml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 geojikuu-0.27.54/PKG-INFO
```

### Comparing `geojikuu-0.27.53/geojikuu/aggregation/point_aggregators.py` & `geojikuu-0.27.54/geojikuu/aggregation/point_aggregators.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 License: Apache 2.0 (see LICENSE file for details)
 
 Copyright (c) 2023, Kaine Usher.
 """
 
 import pandas as pd
 import numpy as np
-from preprocessing.normalisation import MinMaxScaler
+from geojikuu.preprocessing.normalisation import MinMaxScaler
 
 class KNearestNeighbours:
     
     def __init__(self, data, coordinate_label):
         self.__data = data.to_dict()
         self.__coordinate_label = coordinate_label
```

### Comparing `geojikuu-0.27.53/geojikuu/descriptives/spacetime_distribution.py` & `geojikuu-0.27.54/geojikuu/descriptives/spacetime_distribution.py`

 * *Files identical despite different names*

### Comparing `geojikuu-0.27.53/geojikuu/descriptives/spatial_distribution.py` & `geojikuu-0.27.54/geojikuu/descriptives/spatial_distribution.py`

 * *Files identical despite different names*

### Comparing `geojikuu-0.27.53/geojikuu/hypothesis_testing/autocorrelation.py` & `geojikuu-0.27.54/geojikuu/hypothesis_testing/autocorrelation.py`

 * *Files identical despite different names*

### Comparing `geojikuu-0.27.53/geojikuu/hypothesis_testing/hot_spot_analysis.py` & `geojikuu-0.27.54/geojikuu/hypothesis_testing/hot_spot_analysis.py`

 * *Files identical despite different names*

### Comparing `geojikuu-0.27.53/geojikuu/preprocessing/conversion_tools.py` & `geojikuu-0.27.54/geojikuu/preprocessing/conversion_tools.py`

 * *Files identical despite different names*

### Comparing `geojikuu-0.27.53/geojikuu/preprocessing/normalisation.py` & `geojikuu-0.27.54/geojikuu/preprocessing/normalisation.py`

 * *Files identical despite different names*

### Comparing `geojikuu-0.27.53/geojikuu/preprocessing/projection.py` & `geojikuu-0.27.54/geojikuu/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `geojikuu-0.27.53/LICENSE.txt` & `geojikuu-0.27.54/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geojikuu-0.27.53/pyproject.toml` & `geojikuu-0.27.54/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "GeoJikuu"
-version = "0.27.53"
+version = "0.27.54"
 authors = [
   { name="Kaine Usher", email="kaine.usher1@gmail.com" },
 ]
 description = "GeoJikuu is a Python library for analysing geographical data that contains both spatial and spatiotemporal variables."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `geojikuu-0.27.53/PKG-INFO` & `geojikuu-0.27.54/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: GeoJikuu
-Version: 0.27.53
+Version: 0.27.54
 Summary: GeoJikuu is a Python library for analysing geographical data that contains both spatial and spatiotemporal variables.
 Project-URL: Homepage, https://github.com/kainedusher/GeoJikuu
 Author-email: Kaine Usher <kaine.usher1@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


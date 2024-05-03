# Comparing `tmp/bmxp-0.0.9.tar.gz` & `tmp/bmxp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmxp-0.0.9.tar", last modified: Tue Jan  3 23:14:18 2023, max compression
+gzip compressed data, was "bmxp-0.1.0.tar", last modified: Fri May  3 15:54:00 2024, max compression
```

## Comparing `bmxp-0.0.9.tar` & `bmxp-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.621991 bmxp-0.0.9/
--rw-rw-rw-   0        0        0     1093 2022-11-18 17:19:36.000000 bmxp-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      189 2022-12-21 20:29:36.000000 bmxp-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1257 2023-01-03 23:14:18.621991 bmxp-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      750 2022-11-22 21:07:50.000000 bmxp-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.569976 bmxp-0.0.9/bmxp/
-drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.595820 bmxp-0.0.9/bmxp/eclipse/
--rw-rw-rw-   0        0        0    47118 2022-11-18 17:19:36.000000 bmxp-0.0.9/bmxp/eclipse/__init__.py
--rw-rw-rw-   0        0        0     4347 2022-11-18 17:19:36.000000 bmxp-0.0.9/bmxp/eclipse/eclipse_example.py
-drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.604455 bmxp-0.0.9/bmxp/gravity/
--rw-rw-rw-   0        0        0     9327 2023-01-03 23:12:59.000000 bmxp-0.0.9/bmxp/gravity/__init__.py
--rw-rw-rw-   0        0        0     7896 2023-01-03 23:10:35.000000 bmxp-0.0.9/bmxp/gravity/correlation.c
--rw-rw-rw-   0        0        0    17408 2023-01-03 23:10:39.000000 bmxp-0.0.9/bmxp/gravity/correlation.dll
--rw-rw-rw-   0        0        0    16120 2023-01-03 23:10:39.000000 bmxp-0.0.9/bmxp/gravity/correlation.so
--rw-rw-rw-   0        0        0      615 2023-01-03 18:46:44.000000 bmxp-0.0.9/bmxp/gravity/gravity_example.py
-drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.593823 bmxp-0.0.9/bmxp.egg-info/
--rw-rw-rw-   0        0        0     1257 2023-01-03 23:14:18.000000 bmxp-0.0.9/bmxp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2023-01-03 23:14:18.000000 bmxp-0.0.9/bmxp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-03 23:14:18.000000 bmxp-0.0.9/bmxp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-01-03 23:14:18.000000 bmxp-0.0.9/bmxp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-01-03 23:14:18.000000 bmxp-0.0.9/bmxp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2022-11-18 17:19:36.000000 bmxp-0.0.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-01-03 23:14:18.623051 bmxp-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1178 2023-01-03 23:12:40.000000 bmxp-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.617886 bmxp-0.0.9/tests/
-drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.620002 bmxp-0.0.9/tests/__pycache__/
--rw-rw-rw-   0        0        0    18126 2022-11-21 22:24:15.000000 bmxp-0.0.9/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0    18988 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/example1.csv
--rw-rw-rw-   0        0        0      202 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/make_pickle.py
--rw-rw-rw-   0        0        0   118411 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/mseclipse.pickle
--rw-rw-rw-   0        0        0    13087 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/test1.csv
--rw-rw-rw-   0        0        0    12512 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/test2.csv
--rw-rw-rw-   0        0        0     1239 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/test3.csv
--rw-rw-rw-   0        0        0    78529 2022-11-22 21:07:50.000000 bmxp-0.0.9/tests/test_gravity.csv
--rw-rw-rw-   0        0        0      562 2022-11-22 21:07:50.000000 bmxp-0.0.9/tests/test_gravity.py
--rw-rw-rw-   0        0        0     9433 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/test_mseclipse.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.089717 bmxp-0.1.0/
+-rw-rw-rw-   0        0        0     1093 2022-09-27 19:05:11.000000 bmxp-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      189 2023-01-09 17:26:29.000000 bmxp-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5478 2024-05-03 15:54:00.088707 bmxp-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4810 2024-05-03 15:53:51.000000 bmxp-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.021101 bmxp-0.1.0/bmxp/
+drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.048101 bmxp-0.1.0/bmxp/blueshift/
+-rw-rw-rw-   0        0        0    25428 2024-05-03 15:53:51.000000 bmxp-0.1.0/bmxp/blueshift/__init__.py
+-rw-rw-rw-   0        0        0     2226 2024-04-29 17:37:08.000000 bmxp-0.1.0/bmxp/blueshift/blueshift_example.py
+-rw-rw-rw-   0        0        0      227 2024-03-06 21:12:28.000000 bmxp-0.1.0/bmxp/blueshift/run_blueshift.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.054103 bmxp-0.1.0/bmxp/eclipse/
+-rw-rw-rw-   0        0        0    49812 2024-05-03 15:53:51.000000 bmxp-0.1.0/bmxp/eclipse/__init__.py
+-rw-rw-rw-   0        0        0     4367 2024-04-29 17:37:08.000000 bmxp-0.1.0/bmxp/eclipse/eclipse_example.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.063102 bmxp-0.1.0/bmxp/gravity/
+-rw-rw-rw-   0        0        0    10337 2024-05-03 15:53:51.000000 bmxp-0.1.0/bmxp/gravity/__init__.py
+-rw-rw-rw-   0        0        0     8807 2023-09-18 17:18:55.000000 bmxp-0.1.0/bmxp/gravity/correlation.c
+-rw-rw-rw-   0        0        0    17408 2024-02-22 18:27:08.000000 bmxp-0.1.0/bmxp/gravity/correlation.dll
+-rw-rw-rw-   0        0        0    16088 2024-03-06 21:23:01.000000 bmxp-0.1.0/bmxp/gravity/correlation.so
+-rw-rw-rw-   0        0        0     3725 2023-01-31 21:44:10.000000 bmxp-0.1.0/bmxp/gravity/fallback.py
+-rw-rw-rw-   0        0        0      558 2023-03-27 15:45:05.000000 bmxp-0.1.0/bmxp/gravity/gravity_example.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.041100 bmxp-0.1.0/bmxp.egg-info/
+-rw-rw-rw-   0        0        0     5478 2024-05-03 15:53:59.000000 bmxp-0.1.0/bmxp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1178 2024-05-03 15:53:59.000000 bmxp-0.1.0/bmxp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:53:59.000000 bmxp-0.1.0/bmxp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-03 15:53:59.000000 bmxp-0.1.0/bmxp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 15:53:59.000000 bmxp-0.1.0/bmxp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2022-09-27 19:05:11.000000 bmxp-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 15:54:00.089717 bmxp-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1289 2024-05-03 15:53:51.000000 bmxp-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.082891 bmxp-0.1.0/tests/
+-rw-rw-rw-   0        0        0     8551 2024-04-29 17:37:08.000000 bmxp-0.1.0/tests/DCinfo1.csv
+-rw-rw-rw-   0        0        0     9374 2024-04-29 17:37:08.000000 bmxp-0.1.0/tests/DCinfo2.csv
+-rw-rw-rw-   0        0        0   177687 2024-04-29 17:37:08.000000 bmxp-0.1.0/tests/DCinput1.csv
+-rw-rw-rw-   0        0        0   451309 2024-04-29 17:37:13.000000 bmxp-0.1.0/tests/DCinput2.csv
+drwxrwxrwx   0        0        0        0 2024-05-03 15:54:00.087975 bmxp-0.1.0/tests/__pycache__/
+-rw-rw-rw-   0        0        0    46139 2024-04-30 18:17:48.000000 bmxp-0.1.0/tests/__pycache__/test_blueshift.cpython-311-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0    14842 2024-04-29 20:44:55.000000 bmxp-0.1.0/tests/__pycache__/test_blueshift.cpython-38-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0     1438 2024-04-29 20:44:39.000000 bmxp-0.1.0/tests/__pycache__/test_gravity.cpython-311-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0     1020 2024-04-29 20:44:55.000000 bmxp-0.1.0/tests/__pycache__/test_gravity.cpython-38-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0    58914 2024-05-02 16:46:35.000000 bmxp-0.1.0/tests/__pycache__/test_mseclipse.cpython-311-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0    18250 2024-04-29 20:44:56.000000 bmxp-0.1.0/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.4.0.pyc
+-rw-rw-rw-   0        0        0  1376588 2024-04-29 17:37:08.000000 bmxp-0.1.0/tests/blueshift.pickle
+-rw-rw-rw-   0        0        0    18988 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/example1.csv
+-rw-rw-rw-   0        0        0      202 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/make_pickle.py
+-rw-rw-rw-   0        0        0   118411 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/mseclipse.pickle
+-rw-rw-rw-   0        0        0    13087 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/test1.csv
+-rw-rw-rw-   0        0        0    12512 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/test2.csv
+-rw-rw-rw-   0        0        0     1239 2022-09-27 19:05:11.000000 bmxp-0.1.0/tests/test3.csv
+-rw-rw-rw-   0        0        0     8887 2024-05-03 15:53:51.000000 bmxp-0.1.0/tests/test_blueshift.py
+-rw-rw-rw-   0        0        0    78529 2023-01-09 17:26:29.000000 bmxp-0.1.0/tests/test_gravity.csv
+-rw-rw-rw-   0        0        0      606 2024-04-29 17:37:08.000000 bmxp-0.1.0/tests/test_gravity.py
+-rw-rw-rw-   0        0        0    11452 2024-05-03 15:53:51.000000 bmxp-0.1.0/tests/test_mseclipse.py
```

### Comparing `bmxp-0.0.9/LICENSE` & `bmxp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.9/bmxp/eclipse/__init__.py` & `bmxp-0.1.0/bmxp/eclipse/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 import networkx as nx
 import numpy as np
 import pandas as pd
 from scipy import interpolate
 import statsmodels.api as sm
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_pdf import PdfPages
+from bmxp import FMDATA
 
 logging.basicConfig()
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.INFO)
 
 np.random.seed(0)
 
 lowess = sm.nonparametric.lowess
-__version__ = "0.0.3"
+__version__ = "0.1.0"
 
 
 def dataset_loops(attr=None):
     """
     Wraps a function with a double For-loop for iterating over the datasets.
     It converts the supplied datasets, which may be None, 1 dataset, or multiple,
     to a list.
@@ -82,35 +83,68 @@
 
 class MSAligner:  # pylint: disable=too-many-instance-attributes
     """
     MSAligner stores 2 or more MS Datasets and performs matching, scaling, and
     alignments between them.
     """
 
-    def __init__(self, *args, names=None):
+    # references FMDATA keys, not schema values
+    # values are evaluated in __init__
+    descriptors = {"RT": "linear", "MZ": "ppm", "Intensity": "log10"}
+    default_cutoff = 6
+    default_weight = 1
+    default_cutoffs = {}
+    default_weights = {}
+    default_coarse_params = {
+        "RT": {"upper": 0.5, "lower": -0.5},
+        "MZ": {"upper": 15, "lower": -15},
+        "Intensity": {"upper": 2, "lower": -2},
+    }
+    default_scaler_params = {
+        "smoothing_method": "lowess",
+        "smoothing_params": {"frac": 0.1},
+    }
+    feature_name = "Compound_ID"
+    intensity_col = "Intensity"
+
+    def __init__(self, *args, names=None, schema_labels=None):
         """
         Initializes the MSAligner object with a collection of datasets and their names.
 
         :param args: tuple[str], filepaths of .csv datasets
         :param names: list[str], names of datasets
         """
-        self.descriptors = {"RT": "linear", "MZ": "ppm", "Intensity": "log10"}
-        self.default_cutoffs = {"RT": 6, "Intensity": 6, "MZ": 6}
-        self.default_weights = {"RT": 1, "Intensity": 1, "MZ": 1}
-        self.default_coarse_params = {
-            "RT": {"upper": 0.5, "lower": -0.5},
-            "MZ": {"upper": 15, "lower": -15},
-            "Intensity": {"upper": 2, "lower": -2},
+
+        fmdata = FMDATA.copy()
+        if schema_labels is not None:
+            fmdata.update(schema_labels)
+
+        self.descriptors = {fmdata[k]: v for k, v in MSAligner.descriptors.items()}
+        self.default_cutoff = MSAligner.default_cutoff
+        self.default_weight = MSAligner.default_weight
+        self.default_weights = {
+            fmdata[k]: v for k, v in MSAligner.default_weights.items()
+        }
+        self.default_cutoffs = {
+            fmdata[k]: v for k, v in MSAligner.default_cutoffs.items()
         }
-        self.default_scaler_params = {
-            "smoothing_method": "lowess",
-            "smoothing_params": {"frac": 0.1},
+
+        # for k in MSAligner.descriptors:
+        #     if k not in MSAligner.default_weights:
+        if MSAligner.default_weights is None:
+            self.default_weights = {
+                fmdata[k]: self.default_weight for k in MSAligner.descriptors
+            }
+
+        self.default_coarse_params = {
+            fmdata[k]: v for k, v in MSAligner.default_coarse_params.items()
         }
-        self.feature_name = "Compound_ID"
-        self.anchor_priority = "Intensity"
+        self.default_scaler_params = MSAligner.default_scaler_params
+        self.feature_name = fmdata[MSAligner.feature_name]
+        self.intensity_col = fmdata[MSAligner.intensity_col]
         self.datasets = collections.OrderedDict()
         self.anchors = {}
         self.coarse_matches = {}
         self.scalers = {}
         self.scaled_values = {}
         self.stds = {}
         self.matches = {}
@@ -178,45 +212,58 @@
         elif isinstance(names, str):
             names = [names]
 
         # Check all datasets included in the names
         for name in names:
             ds = self.datasets[name]
             # calculate intensity if needed
-            if "Intensity" not in ds.columns and "Intensity" in self.descriptors:
+            if (
+                self.intensity_col not in ds.columns
+                and self.intensity_col in self.descriptors
+            ):
                 gen_intensity(
                     ds,
-                    ignore=[descr for descr in self.descriptors if descr != "Intensity"]
+                    self.intensity_col,
+                    ignore=[
+                        descr
+                        for descr in self.descriptors
+                        if descr != self.intensity_col
+                    ]
                     + [self.feature_name],
                 )
 
             # Check required columns
             required_columns = [*self.descriptors, self.feature_name]
             for req_col in required_columns:
                 if req_col not in ds.columns:
                     raise ValueError(f"Column {req_col} not found in dataset {name}.")
 
-    def set_defaults(self, params):
+    def set_instance_defaults(self, params):
         """
         Updates default values for weights and cutoffs.
         """
 
         for key, item in params.items():
-            if key.lower() == "cutoffs":
-                self.default_cutoffs.update(item)
+            if key.lower() == "weight":
+                self.default_weight = item
+            elif key.lower() == "cutoff":
+                self.default_cutoff = item
             elif key.lower() == "weights":
                 self.default_weights.update(item)
+            elif key.lower() == "cutoffs":
+                self.default_cutoffs.update(item)
             elif key.lower() == "coarse_params":
                 self.default_coarse_params.update(item)
             elif key.lower() == "scaler_params":
                 self.default_scaler_params.update(item)
             else:
                 raise KeyError(
-                    f"Unknown value: {key}. Acceptable values are 'cutoffs', 'weights',"
-                    " 'coarse_params', and 'scaler_params'."
+                    f"Unknown value: {key}. Acceptable values are "
+                    " 'weight', 'weights', 'cutoff', 'cutoffs',"
+                    " 'coarse_params' and 'scaler_params'."
                 )
 
     def set_params(self, params, rec=True):
         """
         Sets weights, cutoffs, and scalers for any dataset pairs
         For example:
         {"scalers": {
@@ -427,26 +474,26 @@
                         self.weights[ds2][ds1] = {}
                     self.weights[ds2][ds1].update(weights[ds1][ds2])
 
     def set_coarse_params(
         self, coarse_params, rec=True
     ):  # pylint: disable=too-many-branches
         """
-                Function to set custom cutoffs. If rec is true, apply reciprocal cutoffs
-                {
-                    'DS1': {
-                        'DS2':{
-                            'rt_minus': -.7,
-                            'ppm_plus': 4
-                        }
-                    }
+        Function to set custom cutoffs. If rec is true, apply reciprocal cutoffs
+        {
+            'DS1': {
+                'DS2':{
+                    'rt_minus': -.7,
+                    'ppm_plus': 4
                 }
-                :param coarse_params: dict
-                :param rec: bool
-                """
+            }
+        }
+        :param coarse_params: dict
+        :param rec: bool
+        """
         coarse_params = coarse_params.copy()
         for ds1 in coarse_params:
             # make coarse_params dicts if they don't exist
             if ds1 not in self.coarse_params:
                 self.coarse_params[ds1] = {}
             for ds2 in coarse_params[ds1]:
                 if ds2 not in self.coarse_params[ds1]:
@@ -691,15 +738,15 @@
         coarse_match = self.coarse_matches[ds1][ds2]
         ds1_matches = self.datasets[ds1].loc[coarse_match[ds1], :]
         ds2_matches = self.datasets[ds2].loc[coarse_match[ds2], :]
         if ds2 not in self.scalers[ds1]:
             self.scalers[ds1][ds2] = {}
 
         scalers = {}
-        for (descr, mode) in self.descriptors.items():
+        for descr, mode in self.descriptors.items():
             if descr not in self.scalers[ds1][ds2]:
                 scaled = calc_scalers(
                     ds1_matches[descr].values,
                     ds2_matches[descr].values,
                     smoothing=scaler_params["smoothing_method"],
                     mode=mode,
                     **scaler_params["smoothing_params"],
@@ -712,15 +759,15 @@
         """
         Scales the rt, mz, and intensity values for all datasets
         """
         LOGGER.info(f"Scaling {ds1} -> {ds2}...")
         # extract anchors, match, and convert results to a dataframe
         scaled = pd.DataFrame(index=self.datasets[ds1].index)
         scalers = self.scalers[ds1][ds2]
-        for (descr, mode) in self.descriptors.items():
+        for descr, mode in self.descriptors.items():
             scaled[descr] = scale_to(
                 self.datasets[ds1][descr],
                 scalers[descr]["x"],
                 scalers[descr]["y"],
                 mode=mode,
             )
         self.scaled_values[ds1][ds2] = scaled
@@ -730,15 +777,15 @@
         """
         Calculates standard deviations to be used for matching.
         """
         LOGGER.info(f"Calculating variance from {ds1} -> {ds2}...")
         coarse_matches = self.coarse_matches[ds1][ds2]
         scalers = self.scalers[ds1][ds2]
         self.stds[ds1][ds2] = {}
-        for (descr, mode) in self.descriptors.items():
+        for descr, mode in self.descriptors.items():
             ds1_vals = self.datasets[ds1].loc[coarse_matches[ds1], descr]
             ds2_vals = self.datasets[ds2].loc[coarse_matches[ds2], descr]
             s_ds1_vals = scale_to(
                 ds1_vals, scalers[descr]["x"], scalers[descr]["y"], mode=mode
             )
             if mode == "linear":
                 res = (s_ds1_vals - ds2_vals).values
@@ -752,25 +799,33 @@
     @dataset_loops("matches")
     def gen_matches(self, ds1, ds2):
         """
         Generates best matches for each dataset
         """
         LOGGER.info(f"Matching {ds1} -> {ds2}...")
         # generate the weights and cutoffs
-        cutoffs = self.default_cutoffs.copy()
-        try:
-            cutoffs.update(self.cutoffs[ds1][ds2])
-        except KeyError:
-            pass
-
-        weights = self.default_weights.copy()
-        try:
-            weights.update(self.weights[ds1][ds2])
-        except KeyError:
-            pass
+        # if no "custom" cutoffs or weights are present, use default
+        cutoffs = {}
+        weights = {}
+        for descr in self.descriptors:
+            try:
+                cutoffs[descr] = self.cutoffs[ds1][ds2][descr]
+            except KeyError:
+                try:
+                    cutoffs[descr] = self.default_cutoffs[descr]
+                except KeyError:
+                    cutoffs[descr] = self.default_cutoff
+            try:
+                weights[descr] = self.weights[ds1][ds2][descr]
+
+            except KeyError:
+                try:
+                    weights[descr] = self.default_weights[descr]
+                except KeyError:
+                    weights[descr] = self.default_weight
 
         self.matches[ds1][ds2] = score_match(
             self.scaled_values[ds1][ds2],
             self.datasets[ds2],
             self.stds[ds1][ds2],
             self.descriptors,
             cutoffs,
@@ -800,15 +855,19 @@
             targets = [ds2 + "__" + str(name) for name in targets]
             edges.extend(
                 [tuple([s, t, {"rank": col}]) for s, t in zip(sources, targets)]
             )
         self.graph.add_edges_from(edges)
 
     def report(
-        self, datasets_1=None, datasets_2=None, filepath="report.pdf", to_bytes=False,
+        self,
+        datasets_1=None,
+        datasets_2=None,
+        filepath="report.pdf",
+        to_bytes=False,
     ):
         """
         Creates a report of the alignment parameters.
         """
         if datasets_1 is None:
             datasets_1 = list(self.datasets)
         if isinstance(datasets_1, str):
@@ -823,36 +882,101 @@
         else:
             file_handle = filepath
 
         # create scaling report
         with PdfPages(file_handle) as pdf:
             for ds1 in datasets_1:
                 for ds2 in datasets_2:
-                    if ds1 == ds2:
+                    if (
+                        ds1 == ds2
+                        or ds1 not in self.scalers
+                        or ds2 not in self.scalers[ds1]
+                    ):
                         continue
                     eval_chart(self, ds1, ds2, show=False)
                     pdf.savefig()
                     plt.close("all")
+                    if ds1 not in self.matches or ds2 not in self.matches[ds1]:
+                        continue
                     eval_chart(self, ds1, ds2, show=False, results=True)
                     pdf.savefig()
                     plt.close("all")
         if to_bytes:
             file_handle.seek(0)
             return file_handle
         return None
 
 
-def score_match(df1, df2, stds, descriptors, cutoffs, weights, top_n=3):
+def calc_scalers(x1, x2, smoothing=None, mode="linear", **kwargs):
+    """
+    Creates and returns scalers from X1 and X2 coordinates
+    i.e. Dataset 1 RTs - [7.1, 8.43, 9.5]
+         Dataset 2 RTs - [7.24, 8.74, 9.7]
+    Returns scalers in the proper space, e.g. log10 space for intensity, ppm for mz
+         Dataset 1 RTs -     [7.1, 8.43, 9.5]
+         Dataset 2 Scalers - [0.14, 0.31, 0.2]
+
+    :param x1: Array or List
+    :param x2: Array or List
+    :param smoothing: str, Smoothing mode (None or "lowess" currently)
+    :param mode: str, "linear" or "ppm"
+    :return: Numpy array
+    """
+    x1 = np.array(x1)
+    x2 = np.array(x2)
+
+    if mode == "linear":
+        y = x2 - x1
+    elif mode == "ppm":
+        y = (x2 - x1) / x1 * 1000000
+    elif mode == "log10":
+        y = np.log10(x2) - np.log10(x1)
+        x1 = np.log10(x1)
+    else:
+        raise NotImplementedError(f"We do not have a scaling method for {mode}.")
+    if smoothing is None:
+        return (x1, y)
+
+    # +/- <0.5 ppt random noise to break ties
+    np.random.seed(0)
+    noise = (np.random.random(size=len(x1)) - 0.5) * x1 / 10**12
+
+    # allow us to override frac via kwargs
+    temp_kwargs = kwargs.copy()
+    if "frac" not in temp_kwargs:
+        temp_kwargs["frac"] = 0.1
+
+    delta = 0.01 * (max(x1) - min(x1))
+    scalers = lowess(y, x1 + noise, return_sorted=False, delta=delta, **temp_kwargs)
+
+    # On failure, depending on statsmodels version, either returns NaNs, or
+    # the residuals. Try adding more until it works or reaches 1. On reaching 1,
+    # it should be obvious that smoothing failed or it is over smoothed.
+    while np.isnan(scalers).all() or np.array_equal(scalers, y):
+        temp_kwargs["frac"] += 0.01
+        if temp_kwargs["frac"] >= 1.0:
+            break
+        scalers = lowess(
+            y,
+            x1 + noise,
+            return_sorted=False,
+            delta=delta,
+            **temp_kwargs,
+        )
+    return (x1, scalers)
+
+
+def score_match(df1, df2, stds, descriptors, cutoffs, weights, top_n=1):
     """
     Returns scored best matches for a dataframe to another
     :param df1: DataFrame, first dataset
     :param df2: DataFrame, second dataset
     :param stds: Dict, standard deviations for "RT", "MT", and "Intensity"
-    :param weights: Dict, Multipliers for weights
     :param cutoffs: Dict, Multipliers for finding cutoffs
+    :param weights: Dict, Multipliers for weights
     :param top_n: Int, number of potential matches to record
     :return: Dataframe, df1 index as index, and matching df2 index in top_n columns
     """
     results = []
 
     np1 = df1[list(descriptors)].values
     np2 = df2[list(descriptors)].values
@@ -882,83 +1006,33 @@
                     10 ** (np.log10(ds1_values[descr]) + cutoffs[descr] * stds[descr]),
                 )
             else:
                 raise NotImplementedError("Not sure how to handle the mode ", mode)
 
             # whittle hits down to list
             potential_hits = potential_hits & (
-                (np2[:, i] > bounds[0]) & (np2[:, i] < bounds[1])
+                (np2[:, i] >= bounds[0]) & (np2[:, i] <= bounds[1])
             )
 
         hits_index = df2.index[potential_hits]
 
         # score and sort results
         scores = []
         for hit in np2[potential_hits]:
             ds2_values = {descr: hit[i] for i, descr in enumerate(list(descriptors))}
             scores.append(
                 calc_score(ds1_values, ds2_values, descriptors, stds, weights)
             )
 
-        # append the top 3
+        # append the top n
         results.append([score for _, score in sorted(zip(scores, hits_index))][:top_n])
     results = pd.DataFrame(results, index=df1.index)
     return results
 
 
-def calc_scalers(x1, x2, smoothing=None, mode="linear", **kwargs):
-    """
-    Creates and returns scalers from X1 and X2 coordinates
-    i.e. Dataset 1 RTs - [7.1, 8.43, 9.5]
-         Dataset 2 RTs - [7.24, 8.74, 9.7]
-    Returns scalers in the proper space, e.g. log10 space for intensity, ppm for mz
-         Dataset 1 RTs -     [7.1, 8.43, 9.5]
-         Dataset 2 Scalers - [0.14, 0.31, 0.2]
-
-    :param x1: Array or List
-    :param x2: Array or List
-    :param smoothing: str, Smoothing mode (None or "lowess" currently)
-    :param mode: str, "linear" or "ppm"
-    :return: Numpy array
-    """
-    x1 = np.array(x1)
-    x2 = np.array(x2)
-
-    if mode == "linear":
-        y = x2 - x1
-    elif mode == "ppm":
-        y = (x2 - x1) / x1 * 1000000
-    elif mode == "log10":
-        y = np.log10(x2) - np.log10(x1)
-        x1 = np.log10(x1)
-    else:
-        raise NotImplementedError(f"We do not have a scaling method for {mode}.")
-    if smoothing is None:
-        return (x1, y)
-
-    # +/- <0.5 ppt random noise to break ties
-    np.random.seed(0)
-    noise = (np.random.random(size=len(x1)) - 0.5) * x1 / 10 ** 12
-
-    # allow us to override frac via kwargs
-    if "frac" not in kwargs:
-        kwargs["frac"] = 0.1
-
-    # If we get NaN for all our answers, add a bit to the frac and try again.
-    # Or give up. It will be obvious in the report that it failed
-    delta = 0.01 * (max(x1) - min(x1))
-    scalers = lowess(y, x1 + noise, return_sorted=False, delta=delta, **kwargs)
-    while np.isnan(scalers).all():
-        kwargs["frac"] += 0.01
-        if kwargs["frac"] >= 1.0:
-            break
-        scalers = lowess(y, x1 + noise, return_sorted=False, delta=delta, **kwargs,)
-    return (x1, scalers)
-
-
 def anchors(ds, match_params, remove_all=True, priority="Intensity"):
     """
     Creates a list of anchors for a given dataset.
     :param ds: DataFrame
     :param match_params: dict, parameters for matching
     :param remove_all: bool, flag to indicate removing all confusable feature
     :param priority: str, the column indicating the which features are highest quality
@@ -972,15 +1046,14 @@
     # convert to numpy for performance
     index = ds.index
     ds = ds.values
 
     inclusion = set()
     exclusion = set()
     for i, row in enumerate(ds):
-
         # if a feature has been marked for removal, skip it.
         # important for non-remove all algorithm
         if not remove_all and index[i] in exclusion:
             continue
         bool_array = np.full(len(index), True, dtype=bool)
         for j, param in enumerate(match_params.values()):
             descr_val = row[j]
@@ -1045,29 +1118,30 @@
             elif param["mode"] == "log10":
                 lower = descr_val * 10 ** param["lower"]
                 upper = descr_val * 10 ** param["upper"]
             bool_array = bool_array & (np2[:, j] > lower) & (np2[:, j] < upper)
 
         for result in df2.index[bool_array]:
             results.append([df1.index[i], result])
+
     return results
 
 
-def gen_intensity(dataset, ignore=None):
+def gen_intensity(dataset, intensity_col="Intensity", ignore=None):
     """
     calculate an intensity column, using all columns that are not named '
      RT','MZ','Compound_ID'
-    overwrites the existing dataframe with another one where Intensity is on the far end
+    overwrites the existing dataframe with another one where Intensity is at index 1
 
     :param dataset: pandas Dataframe where there are intensities to calculate
     """
     if ignore:
         calc_df = dataset.drop(columns=ignore)
     calc_df.fillna(0, inplace=True)
-    dataset["Intensity"] = calc_df.mean(axis=1)
+    dataset.insert(1, intensity_col, calc_df.mean(axis=1, numeric_only=True))
 
 
 def scale_to(x, x_scalers, y_scalers, mode="linear"):
     """
     Adjusts the x values to the scalers provided.
 
     :param x: Numpy Array, unscaled values
@@ -1088,15 +1162,15 @@
     x_max_y = y_scalers.iloc[np.argmax(x_scalers)]
     scaled = x + interpolate.interp1d(
         x_scalers, y_scalers, bounds_error=False, fill_value=(x_min_y, x_max_y)
     )(x)
     if isinstance(scaled, pd.Series):
         scaled = scaled.values
     if mode == "log10":
-        scaled = 10 ** scaled
+        scaled = 10**scaled
     return scaled
 
 
 def is_outlier(points, thresh=3.5):
     """
     Returns a boolean array with True if points are outliers and False
     otherwise.
@@ -1126,16 +1200,15 @@
 def calc_score(v1, v2, descriptors, stds, weights):
     """
     Returns the score of two features, provided their parameters, standard deviations,
      and scoring weights
     :return: float, score
     """
     penalty = 0
-    for (descr, mode) in descriptors.items():
-
+    for descr, mode in descriptors.items():
         if mode == "linear":
             penalty += ((v1[descr] - v2[descr]) / stds[descr]) ** 2 * weights[descr]
         elif mode == "ppm":
             penalty += (
                 (((v1[descr] - v2[descr]) / v1[descr]) * 1_000_000) / stds[descr]
             ) ** 2 * weights[descr]
         elif mode == "log10":
@@ -1191,35 +1264,46 @@
             y_vals = np.log10(descr_2) - np.log10(descr_1)
             s_y_vals = np.log10(descr_2) - np.log10(s_descr_1)
             descr_1 = np.log10(descr_1)
 
         # plot the deltas
         plt.subplot(len(self.descriptors), 3, 3 * i + 1)
         plt.scatter(
-            descr_1, y_vals, alpha=0.4, s=3, rasterized=True,
+            descr_1,
+            y_vals,
+            alpha=0.4,
+            s=3,
+            rasterized=True,
         )
         plt.title(f"{descr} {key1} vs {key2}")
         plt.xlabel(f"{title} {descr} {key1}")
         plt.ylabel(f"{title} {descr} ({key2} - {key1}) : {mode}")
         plt.plot(scalers["x"], scalers["y"], color="red", rasterized=True)
 
         # plot the scaled
         plt.subplot(len(self.descriptors), 3, 3 * i + 2)
         plt.scatter(
-            descr_1, s_y_vals, alpha=0.4, s=3, rasterized=True,
+            descr_1,
+            s_y_vals,
+            alpha=0.4,
+            s=3,
+            rasterized=True,
         )
         plt.title(f"{descr} {key1} vs {key2}")
         plt.xlabel(f"{title} {descr} {key1}")
         plt.ylabel(f"{title} {descr} ({key2} - {key1}) : {mode}")
         plt.axhline(y=0, color="red", rasterized=True)
 
         # plot histogram
         plt.subplot(len(self.descriptors), 3, 3 * i + 3)
         plt.hist(
-            x=(s_y_vals), bins="auto", alpha=0.7, rwidth=0.85,
+            x=(s_y_vals),
+            bins="auto",
+            alpha=0.7,
+            rwidth=0.85,
         )
         plt.title(f"{descr} Histograms")
         plt.xlabel(f"{title} {descr} ({key2} - {key1})")
         plt.tight_layout()
 
     if show:
         plt.show()
```

### Comparing `bmxp-0.0.9/bmxp/eclipse/eclipse_example.py` & `bmxp-0.1.0/bmxp/eclipse/eclipse_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,26 +152,30 @@
 
 # Scales DS1 to DS2 based on generated scalers
 a.gen_scaled_values("DS1", "DS2")
 
 a.gen_matches("DS1", "DS2")
 
 a.report(
-    datasets_1="DS1", datasets_2="DS2", filepath="one-way-results.pdf",
+    datasets_1="DS1",
+    datasets_2="DS2",
+    filepath="one-way-results.pdf",
 )
 
 
 ############
 # Example 4 - Two way unsupervised alignment to one or more other datasets
 ############
 a = MSAligner(*datasets, names=["DS1", "DS2", "DS3"])
 
 # Align the
 a.align("DS1", ["DS2", "DS3"])
 a.align(["DS2", "DS3"], "DS1")
 
 a.report(datasets_1="DS1", datasets_2=["DS2", "DS3"], filepath="DS1_to.pdf")
 a.report(
-    datasets_1=["DS2", "DS3"], datasets_2="DS1", filepath="DS1_from.pdf",
+    datasets_1=["DS2", "DS3"],
+    datasets_2="DS1",
+    filepath="DS1_from.pdf",
 )
 
 a.to_csv("DS1", union_only=False)
```

### Comparing `bmxp-0.0.9/bmxp/gravity/__init__.py` & `bmxp-0.1.0/bmxp/gravity/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,109 +13,108 @@
 
 Pearson - Fill NaNs with Zeroes (Fill in Python, call by_corr)
 Pearson - Drop NaNs (Don't fill, call by_rt)
 
 
 """
 
-
 import logging
 import math
-import pandas as pd
-import networkx as nx
 from ctypes import CDLL, c_double, c_int32, c_void_p
 import os
 import platform
+import pandas as pd
+import networkx as nx
 import numpy as np
+from bmxp.gravity import fallback
+from bmxp import FMDATA
 
 dir_path = os.path.dirname(os.path.realpath(__file__))
-if platform.system() == "Windows":
+correlation = None
+if platform.system() == "Windows" and os.path.exists(
+    os.path.join(dir_path, "correlation.dll")
+):
     correlation = CDLL(os.path.join(dir_path, "correlation.dll"))
-else:
+elif platform.system() == "Linux" and os.path.exists(
+    os.path.join(dir_path, "correlation.so")
+):
     correlation = CDLL(os.path.join(dir_path, "correlation.so"))
 
 c_array = np.ctypeslib.ndpointer(dtype=np.float64, flags="C_CONTIGUOUS")
 int32_array = np.ctypeslib.ndpointer(dtype=np.int32, flags="C_CONTIGUOUS")
 
-correlation.free_p.argtypes = [c_void_p]
-
-correlation.pearson_array.argtypes = [
-    c_array,
-    c_int32,
-    c_int32,
-    c_int32,
-]
-correlation.pearson_array.restype = c_double
+if correlation:
+    correlation.free_p.argtypes = [c_void_p]
 
-correlation.spearman_array.argtypes = [c_array, c_int32, c_int32, c_int32, c_int32]
-correlation.spearman_array.restype = c_double
+    correlation.pearson_array.argtypes = [c_array, c_int32, c_int32, c_int32]
+    correlation.pearson_array.restype = c_double
 
-correlation.pearson.argtypes = [c_array, c_array, c_int32]
-correlation.pearson.restype = c_double
+    correlation.spearman_array.argtypes = [
+        c_array,  # arr
+        c_int32,  # r1_start
+        c_int32,  # r2_start
+        c_int32,  # size
+        c_int32,  # dropNan
+        c_int32,  # legacyMode
+    ]
+    correlation.spearman_array.restype = c_double
+    correlation.pearson.argtypes = [c_array, c_array, c_int32]
+    correlation.pearson.restype = c_double
 
-correlation.spearman.argtypes = [c_array, c_array, c_int32, c_int32]
-correlation.spearman.restype = c_double
+    correlation.spearman.argtypes = [c_array, c_array, c_int32, c_int32, c_int32]
+    correlation.spearman.restype = c_double
+else:
+    correlation = fallback
 
 logging.basicConfig()
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.INFO)
 
-__version__ = "0.0.4"
-ECLIPSE_COLUMNS = [
-    "RT",
-    "MZ",
-    "Intensity",
-    "Non_Quant",
-    "Compound_ID",
-    "Adduct",
-    "Annotation_ID",
-    "Metabolite",
-    "Cluster_Num",
-    "Cluster_Size",
-]
+__version__ = "0.1.0"
 
 
 def free_p(p):
     correlation.free_p(p)
 
 
 def pearson_array(arr1, r1_start, r2_start):
-    r_p = correlation.pearson_array(arr1, r1_start, r2_start, len(arr1[0]),)
+    r_p = correlation.pearson_array(
+        arr1,
+        r1_start,
+        r2_start,
+        len(arr1[0]),
+    )
     return r_p
 
 
-def spearman_array(arr1, r1_start, r2_start, nan_policy="fill"):
-    drop_nan = False
-    if nan_policy != "fill":
-        drop_nan = True
-    r_p = correlation.spearman_array(arr1, r1_start, r2_start, len(arr1[0]), drop_nan)
+def spearman_array(arr1, r1_start, r2_start, nan_policy="fill", legacy_mode=False):
+    drop_nan = nan_policy != "fill"
+    r_p = correlation.spearman_array(
+        arr1, r1_start, r2_start, len(arr1[0]), drop_nan, legacy_mode
+    )
     return r_p
 
 
 def pearson(x, y):
-    if isinstance(x, list):
-        x = np.array(x).astype(np.float64)
-    if isinstance(y, list):
-        y = np.array(y).astype(np.float64)
+    x = np.array(x).astype(np.float64)
+    y = np.array(y).astype(np.float64)
     return correlation.pearson(x, y, len(x))
 
 
-def spearman(x, y, nan_policy="fill"):
-    if isinstance(x, list):
-        x = np.array(x).astype(np.float64)
-    if isinstance(y, list):
-        y = np.array(y).astype(np.float64)
-    drop_nan = False
-    if nan_policy != "fill":
-        drop_nan = True
-    return correlation.spearman(x, y, len(x), drop_nan)
+def spearman(x, y, nan_policy="fill", legacy_mode=False):
+    x = np.array(x).astype(np.float64)
+    y = np.array(y).astype(np.float64)
+    drop_nan = nan_policy != "fill"
+    return correlation.spearman(x, y, len(x), drop_nan, legacy_mode)
 
 
-def deconvolute(df_index, graph):
-    cluster_df = pd.DataFrame({"Cluster_Num": None, "Cluster_Size": 1}, index=df_index)
+def deconvolute(df_index, graph, fmdata):
+    num_label = fmdata["Cluster_Num"]
+    size_label = fmdata["Cluster_Size"]
+    cluster_df = pd.DataFrame({num_label: None, size_label: 1}, index=df_index)
     i = 0
     while True:
         # delete singletons
         graph.remove_nodes_from(list(nx.isolates(graph)))
 
         # build list of cliques of the largest size
         cliques = []
@@ -139,16 +138,16 @@
         # sort by best corr
         cliques.sort(key=lambda x: x[1], reverse=True)
         to_remove = set()
         while len(cliques) > 0:
             # add the best one
             best_clique = cliques[0]
             features = list(best_clique[0])
-            cluster_df.loc[features, "Cluster_Num"] = i
-            cluster_df.loc[features, "Cluster_Size"] = max_size
+            cluster_df.loc[features, num_label] = i
+            cluster_df.loc[features, size_label] = max_size
             if i % 50 == 0:
                 LOGGER.info(f"On cluster {i}, which contains {max_size} features.")
             i += 1
 
             # search the clique for ones to remove
             cliques = [
                 clique
@@ -159,105 +158,125 @@
             to_remove.update(best_clique[0])
         graph.remove_nodes_from(to_remove)
         if max_size == 2:
             break
     return cluster_df
 
 
-def corr_array(i, j, rt_series, df, corr_value, rt_thresh, method, nan_policy):
-
+def corr_array(
+    i, j, rt_series, df, corr_value, rt_thresh, method, nan_policy, legacy_mode
+):
     # long winded way to find RT differences and the indices
     # similar to pd.stack
     np_batch_a = rt_series.iloc[i[0] : i[1]].values
     np_batch_b = rt_series.iloc[j[0] : j[1]].values
     rt_flattened = np.absolute(np.subtract.outer(np_batch_b, np_batch_a)).flatten()
     a_index = np.tile(np.fromiter(range(i[0], i[1]), int), (j[1] - j[0]))
     b_index = np.tile(np.fromiter(range(j[0], j[1]), int), ((i[1] - i[0]), 1)).flatten(
         order="F"
     )
-    to_keep = (rt_flattened <= rt_thresh) & (a_index != b_index)
+    to_keep = (rt_flattened < rt_thresh) & (a_index != b_index)
     a_index = a_index[to_keep]
     b_index = b_index[to_keep]
     corr_results = np.empty(len(a_index))
-    for k in range(len(a_index)):
-        a_val = a_index[k]
+    for k, a_val in enumerate(a_index):
         b_val = b_index[k]
         if method == "spearman":
-            corr_results[k] = spearman_array(df, a_val, b_val, nan_policy)
+            corr_results[k] = spearman_array(df, a_val, b_val, nan_policy, legacy_mode)
         else:
             corr_results[k] = pearson_array(df, a_val, b_val)
     to_return = corr_results > corr_value
     return a_index[to_return], b_index[to_return], corr_results[to_return]
 
 
+def gen_batches(num_features, batch_size):
+    """
+    Generates batches for clustering, based on number of features and batch size
+    """
+    num_batches = math.ceil(num_features / batch_size)
+    for i in range(num_batches):
+        for j in range(i, num_batches):
+            i_indices = [
+                i * batch_size,
+                min((i + 1) * batch_size, num_features),
+            ]
+            j_indices = [
+                j * batch_size,
+                min((j + 1) * batch_size, num_features),
+            ]
+            yield {
+                "i": i,
+                "j": j,
+                "i_indices": i_indices,
+                "j_indices": j_indices,
+                "num_batches": num_batches,
+            }
+
+
 def cluster(
     df,
     rt_thresh=0.02,
     corr_value=0.8,
     batch_size=1000,
     method="spearman",
     nan_policy="fill",
+    legacy_mode=False,
+    schema_labels=None,
 ):
     """
     Cluster aggregates LCMS features into groups based on sample-correlation and
         retention time. It builds a network based on retention time difference and
         correlation. Then it labels the largest clique as a cluster, deletes the
         features from the network, and identifies the next largest clique. Ties are
         broken but a summation of correlations in the cluster.
 
     df: Dataframe, Eclipse compatible
     rt_thresh: float, maximum Rt different for clustering
     corr_value: float, correlation cutoff
     batch_size: int, batch size for calculating correlations
     method: string, "Spearman" or "Pearson" correlation
+    legacy_mode: boolean, when True, NaNs are filled with 0s when correlating features
+    with very few overlapping non-NaN values (Spearman only)
     Returns
     Dataframe, containing cluster number and number of members for each feature. -1
        indicates a single, unclustered feature.
     """
-    rt_series = df["RT"]
+    fmdata = FMDATA.copy()
+    if schema_labels is not None:
+        fmdata.update(schema_labels)
+    rt_series = df[fmdata["RT"]]
     rt_series.index.name = None  # otherwise it crashes during stack
-    sample_df = df.copy().drop(ECLIPSE_COLUMNS, axis=1, errors="ignore")
+    sample_df = df.copy().drop(list(fmdata.keys()), axis=1, errors="ignore")
 
     num_features = len(sample_df.index)
-    num_batches = math.ceil(num_features / batch_size)
     graph = nx.Graph()
     sample_df = sample_df.values.copy()
     if nan_policy == "zeroes":
-        sample_df = sample_df.nan_to_num()
-    for i in range(num_batches):
-        LOGGER.info(f"Correlating Batch {i + 1}/{num_batches}...")
-        for j in range(i, num_batches):
-            i_indices = [
-                i * batch_size,
-                min((i + 1) * batch_size, num_features),
-            ]
-            j_indices = [
-                j * batch_size,
-                min((j + 1) * batch_size, num_features),
-            ]
-            a_index, b_index, corrs = corr_array(
-                i_indices,
-                j_indices,
-                rt_series,
-                sample_df,
-                corr_value,
-                rt_thresh,
-                method,
-                nan_policy,
-            )
-            a_index = df.index[a_index]
-            b_index = df.index[b_index]
-
-            edges = [
-                (s, t, {"coor": coor}) for s, t, coor in zip(a_index, b_index, corrs)
-            ]
-            graph.add_nodes_from(a_index)
-            graph.add_nodes_from(b_index)
-            graph.add_edges_from(edges)
-    return deconvolute(df.index, graph)
+        sample_df = np.nan_to_num(sample_df)
+    for batch_info in gen_batches(num_features, batch_size):
+        num_batches = batch_info["num_batches"]
+        LOGGER.info(f"Correlating Batch { batch_info['i'] + 1}/{num_batches}...")
+        a_index, b_index, corrs = corr_array(
+            batch_info["i_indices"],
+            batch_info["j_indices"],
+            rt_series,
+            sample_df,
+            corr_value,
+            rt_thresh,
+            method,
+            nan_policy,
+            legacy_mode,
+        )
+        a_index = df.index[a_index]
+        b_index = df.index[b_index]
+        edges = [(s, t, {"coor": coor}) for s, t, coor in zip(a_index, b_index, corrs)]
+        graph.add_nodes_from(a_index)
+        graph.add_nodes_from(b_index)
+        graph.add_edges_from(edges)
+    return deconvolute(df.index, graph, fmdata)
 
 
 if __name__ == "__main__":
     data = pd.read_csv(
         r"C:\Users\danie\work\beta-muricholate.csv", index_col="Compound_ID"
     )
     data = data.replace(0, np.nan)
```

### Comparing `bmxp-0.0.9/bmxp/gravity/correlation.c` & `bmxp-0.1.0/bmxp/gravity/correlation.c`

 * *Files 10% similar despite different names*

```diff
@@ -68,33 +68,61 @@
   double stdevY = stdev_m(y, meanY, size, mask, mask_size);
   free(mask);
   return cov / (stdevX * stdevY);
 }
 
 void free_p(void* ptr) { free(ptr); }
 
-double spearman(double* x, double* y, int32_t size, int32_t dropNan) {
+double spearman(double* x, double* y, int32_t size, int32_t dropNan, int32_t legacyMode) {
   Ranking* sortedX = malloc(sizeof(Ranking) * size);
   Ranking* sortedY = malloc(sizeof(Ranking) * size);
   int32_t* eitherNan = malloc(sizeof(int32_t) * size);
   double* xRanks = malloc(sizeof(double) * size);
   double* yRanks = malloc(sizeof(double) * size);
+  double* xCopy = NULL;
+  double* yCopy = NULL;
+  int32_t i = 0;
+  int32_t j = 0;
+
+  if (legacyMode) {
+    xCopy = malloc(sizeof(double) * size);
+    yCopy = malloc(sizeof(double) * size);
+
+    // copy x and y so we don't modify original values, then point "x" and "y" pointers to the copies for ease of use
+    for (int32_t i = 0; i < size; i++) {
+      memcpy(&xCopy[i], &x[i], 8);
+      memcpy(&yCopy[i], &y[i], 8);
+    }
+    x = xCopy;
+    y = yCopy;
+
+    // match behavior of old clustering algorithm
+    int32_t totalNansToDrop = 0;
+    for (i = 0; i < size; i++) {
+      totalNansToDrop += (x[i] != x[i]) || (y[i] != y[i]);
+    }
+    if (size - totalNansToDrop < 10) {
+      for (i = 0; i < size; i++) {
+        if (y[i] != y[i]) y[i] = 0;
+        if (x[i] != x[i]) x[i] = 0;
+      }
+    }
+  }
+
   for (int32_t i = 0; i < size; i++) {
-    xRanks[i] = x[i];
-    yRanks[i] = y[i];
+    memcpy(&xRanks[i], &x[i], 8);
+    memcpy(&yRanks[i], &y[i], 8);
   }
 
   int32_t x_pos = 0;
   int32_t y_pos = 0;
   int32_t y_nan = -1;
   int32_t x_nan = -1;
   int32_t x_is_nan = 0;
   int32_t y_is_nan = 0;
-  int32_t i = 0;
-  int32_t j = 0;
   for (i = 0; i < size; i++) {
     // move to back
     if (x[i] != x[i]) {
       sortedX[size + x_nan].value = NAN;
       sortedX[size + x_nan].index = i;
       x_nan--;
     } else {
@@ -208,15 +236,15 @@
       fillIndex = sortedX[i + j].index;
       if (eitherNan[fillIndex]) {
         continue;
       }
       filled += 1;
       xRanks[fillIndex] = tieRank;
     }
-    i += numToFill - 1;
+    i += j - 1;
     next_x += numToFill;
   }
 
   // fill in remaining X's, where there is a real value in y
   for (i = 0; i < y_pos; i++) {
     index = sortedY[i].index;
     if (eitherNan[index]) {
@@ -242,29 +270,32 @@
       fillIndex = sortedY[i + j].index;
       if (eitherNan[fillIndex]) {
         continue;
       }
       filled += 1;
       yRanks[fillIndex] = tieRank;
     }
-    i += numToFill - 1;
+    i += j - 1;
     next_y += numToFill;
   }
 
   double result = pearson(xRanks, yRanks, size);
   free(sortedX);
   free(sortedY);
   free(xRanks);
   free(yRanks);
   free(eitherNan);
   free(y_idx_to_fill);
   free(x_idx_to_fill);
+  free(xCopy);
+  free(yCopy);
   return result;
 }
 
-double spearman_array(double* arr, int32_t r1_start, int32_t r2_start, int32_t size, int32_t dropNan) {
-  return spearman(&arr[r1_start * size], &arr[r2_start * size], size, dropNan);
+double spearman_array(double* arr, int32_t r1_start, int32_t r2_start, int32_t size, int32_t dropNan,
+                      int32_t legacyMode) {
+  return spearman(&arr[r1_start * size], &arr[r2_start * size], size, dropNan, legacyMode);
 }
 
 double pearson_array(double* arr, int32_t r1_start, int32_t r2_start, int32_t size) {
   return pearson(&arr[r1_start * size], &arr[r2_start * size], size);
 }
```

### Comparing `bmxp-0.0.9/bmxp/gravity/correlation.dll` & `bmxp-0.1.0/bmxp/gravity/correlation.dll`

 * *Files 22% similar despite different names*

#### objdump

```diff
@@ -1,144 +1,144 @@
 
 architecture: i386:x86-64, flags 0x00000103:
 HAS_RELOC, EXEC_P, D_PAGED
-start address 0x00000002e2311350
+start address 0x00000002e2311320
 
 Characteristics 0x222e
 	executable
 	line numbers stripped
 	symbols stripped
 	large address aware
 	debugging information removed
 	DLL
 
-Time/Date		Tue Jan  3 23:10:39 2023
+Time/Date		Thu Feb 22 18:27:08 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
-MinorLinkerVersion	38
+MinorLinkerVersion	41
 SizeOfCode		0000000000002400
 SizeOfInitializedData	0000000000004000
 SizeOfUninitializedData	0000000000000200
-AddressOfEntryPoint	0000000000001350
+AddressOfEntryPoint	0000000000001320
 BaseOfCode		0000000000001000
 ImageBase		00000002e2310000
 SectionAlignment	00001000
 FileAlignment		00000200
 MajorOSystemVersion	4
 MinorOSystemVersion	0
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		0000e000
 SizeOfHeaders		00000400
-CheckSum		000058b6
+CheckSum		0000497e
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
 NumberOfRvaAndSizes	00000010
 
 The Data Directory
 Entry 0 0000000000009000 000000ff Export Directory [.edata (or where ever we found it)]
-Entry 1 000000000000a000 00000404 Import Directory [parts of .idata]
+Entry 1 000000000000a000 00000408 Import Directory [parts of .idata]
 Entry 2 0000000000000000 00000000 Resource Directory [.rsrc]
-Entry 3 0000000000006000 00000264 Exception Directory [.pdata]
+Entry 3 0000000000006000 00000258 Exception Directory [.pdata]
 Entry 4 0000000000000000 00000000 Security Directory
 Entry 5 000000000000d000 00000060 Base Relocation Directory [.reloc]
 Entry 6 0000000000000000 00000000 Debug Directory
 Entry 7 0000000000000000 00000000 Description Directory
 Entry 8 0000000000000000 00000000 Special Directory
 Entry 9 0000000000005040 00000028 Thread Storage Directory [.tls]
 Entry a 0000000000000000 00000000 Load Configuration Directory
 Entry b 0000000000000000 00000000 Bound Import Directory
-Entry c 000000000000a124 000000e8 Import Address Table Directory
+Entry c 000000000000a128 000000e8 Import Address Table Directory
 Entry d 0000000000000000 00000000 Delay Import Directory
 Entry e 0000000000000000 00000000 CLR Runtime Header
 Entry f 0000000000000000 00000000 Reserved
 
 There is an import table in .idata at 0x2e231a000
 
 The Import Tables (interpreted .idata section contents)
  vma:            Hint    Time      Forward  DLL       First
                  Table   Stamp     Chain    Name      Thunk
- 0000a000	0000a03c 00000000 00000000 0000a3a0 0000a124
+ 0000a000	0000a040 00000000 00000000 0000a3a4 0000a128
 
 	DLL Name: KERNEL32.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	a20c	  283  DeleteCriticalSection
-	a224	  319  EnterCriticalSection
-	a23c	  630  GetLastError
-	a24c	  892  InitializeCriticalSection
-	a268	  984  LeaveCriticalSection
-	a280	 1410  Sleep
-	a288	 1445  TlsGetValue
-	a296	 1492  VirtualProtect
-	a2a8	 1494  VirtualQuery
+	a210	  281  DeleteCriticalSection
+	a228	  317  EnterCriticalSection
+	a240	  628  GetLastError
+	a250	  890  InitializeCriticalSection
+	a26c	  982  LeaveCriticalSection
+	a284	 1407  Sleep
+	a28c	 1442  TlsGetValue
+	a29a	 1489  VirtualProtect
+	a2ac	 1491  VirtualQuery
 
- 0000a014	0000a08c 00000000 00000000 0000a3f8 0000a174
+ 0000a014	0000a090 00000000 00000000 0000a3fc 0000a178
 
 	DLL Name: msvcrt.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	a2b8	   84  __iob_func
-	a2c6	   99  __setusermatherr
-	a2da	  121  _amsg_exit
-	a2e8	  190  _errno
-	a2f2	  285  _initterm
-	a2fe	  387  _lock
-	a306	  714  _unlock
-	a310	  906  abort
-	a318	  923  calloc
-	a322	  963  free
-	a32a	  976  fwrite
-	a334	 1023  malloc
-	a33e	 1031  memcpy
-	a348	 1048  qsort
-	a350	 1052  realloc
-	a35a	 1086  strlen
-	a364	 1089  strncmp
-	a36e	 1123  vfprintf
+	a2bc	   84  __iob_func
+	a2ca	   99  __setusermatherr
+	a2de	  120  _amsg_exit
+	a2ec	  188  _errno
+	a2f6	  285  _initterm
+	a302	  387  _lock
+	a30a	  714  _unlock
+	a314	  903  abort
+	a31c	  920  calloc
+	a326	  960  free
+	a32e	  973  fwrite
+	a338	 1021  malloc
+	a342	 1029  memcpy
+	a34c	 1046  qsort
+	a354	 1050  realloc
+	a35e	 1084  strlen
+	a368	 1087  strncmp
+	a372	 1120  vfprintf
 
  0000a028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x2e2319000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		63b4b5ef
+Time/Date stamp 		65d791fc
 Major/Minor 			0/0
 Name 				000000000000908c correlation.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		0000000a
 	[Name Pointer/Ordinal] Table	0000000a
 Table Addresses
 	Export Address Table 		0000000000009028
 	Name Pointer Table 		0000000000009050
 	Ordinal Table 			0000000000009078
 
 Export Address Table -- Ordinal Base 1
-	[   0] +base[   1] 13a0 Export RVA
-	[   1] +base[   2] 1400 Export RVA
-	[   2] +base[   3] 18b0 Export RVA
-	[   3] +base[   4] 1500 Export RVA
-	[   4] +base[   5] 1590 Export RVA
-	[   5] +base[   6] 2010 Export RVA
-	[   6] +base[   7] 18c0 Export RVA
-	[   7] +base[   8] 1fe0 Export RVA
-	[   8] +base[   9] 1470 Export RVA
-	[   9] +base[  10] 13c0 Export RVA
+	[   0] +base[   1] 1370 Export RVA
+	[   1] +base[   2] 13d0 Export RVA
+	[   2] +base[   3] 1840 Export RVA
+	[   3] +base[   4] 14a0 Export RVA
+	[   4] +base[   5] 1520 Export RVA
+	[   5] +base[   6] 2120 Export RVA
+	[   6] +base[   7] 1850 Export RVA
+	[   7] +base[   8] 20f0 Export RVA
+	[   8] +base[   9] 1430 Export RVA
+	[   9] +base[  10] 1390 Export RVA
 
 [Ordinal/Name Pointer] Table
 	[   0] comparator
 	[   1] covariance_m
 	[   2] free_p
 	[   3] nanMask
 	[   4] pearson
@@ -147,383 +147,372 @@
 	[   7] spearman_array
 	[   8] stdev_m
 	[   9] sum_m
 
 The Function Table (interpreted .pdata section contents)
 vma:			BeginAddress	 EndAddress	  UnwindData
  00000002e2316000:	00000002e2311000 00000002e231100c 00000002e2317000
- 00000002e231600c:	00000002e2311010 00000002e23111ff 00000002e2317004
- 00000002e2316018:	00000002e2311200 00000002e2311344 00000002e2317018
- 00000002e2316024:	00000002e2311350 00000002e2311362 00000002e2317028
- 00000002e2316030:	00000002e2311370 00000002e231137f 00000002e231702c
- 00000002e231603c:	00000002e2311380 00000002e231138c 00000002e2317030
- 00000002e2316048:	00000002e2311390 00000002e2311391 00000002e2317034
- 00000002e2316054:	00000002e23113a0 00000002e23113b9 00000002e2317038
- 00000002e2316060:	00000002e23113c0 00000002e23113f5 00000002e231703c
- 00000002e231606c:	00000002e2311400 00000002e2311461 00000002e2317040
- 00000002e2316078:	00000002e2311470 00000002e23114f3 00000002e2317044
- 00000002e2316084:	00000002e2311500 00000002e2311581 00000002e2317048
- 00000002e2316090:	00000002e2311590 00000002e23118a6 00000002e2317058
- 00000002e231609c:	00000002e23118b0 00000002e23118b5 00000002e231707c
- 00000002e23160a8:	00000002e23118c0 00000002e2311fdc 00000002e2317080
- 00000002e23160b4:	00000002e2311fe0 00000002e2312009 00000002e231709c
- 00000002e23160c0:	00000002e2312010 00000002e2312031 00000002e23170a0
- 00000002e23160cc:	00000002e2312040 00000002e231207a 00000002e23170a4
- 00000002e23160d8:	00000002e2312080 00000002e23120ea 00000002e23170ac
- 00000002e23160e4:	00000002e23120f0 00000002e231210f 00000002e23170b8
- 00000002e23160f0:	00000002e2312110 00000002e231213f 00000002e23170bc
- 00000002e23160fc:	00000002e2312140 00000002e23121c1 00000002e23170c4
- 00000002e2316108:	00000002e23121d0 00000002e23121d3 00000002e23170d0
- 00000002e2316114:	00000002e23121e0 00000002e231224a 00000002e23170d4
- 00000002e2316120:	00000002e2312250 00000002e231246d 00000002e23170e0
- 00000002e231612c:	00000002e2312470 00000002e2312755 00000002e23170f0
- 00000002e2316138:	00000002e2312760 00000002e23127cb 00000002e2317108
- 00000002e2316144:	00000002e23127d0 00000002e2312848 00000002e2317118
- 00000002e2316150:	00000002e2312850 00000002e23128d9 00000002e2317124
- 00000002e231615c:	00000002e23128e0 00000002e23129c0 00000002e231712c
- 00000002e2316168:	00000002e23129c0 00000002e23129de 00000002e2317134
- 00000002e2316174:	00000002e23129e0 00000002e23129f3 00000002e2317138
- 00000002e2316180:	00000002e2312a00 00000002e2312a48 00000002e231713c
- 00000002e231618c:	00000002e2312a50 00000002e2312aef 00000002e2317140
- 00000002e2316198:	00000002e2312af0 00000002e2312b71 00000002e231714c
- 00000002e23161a4:	00000002e2312b80 00000002e2312bab 00000002e2317154
- 00000002e23161b0:	00000002e2312bb0 00000002e2312c1c 00000002e231715c
- 00000002e23161bc:	00000002e2312c20 00000002e2312c48 00000002e2317164
- 00000002e23161c8:	00000002e2312c50 00000002e2312cd5 00000002e231716c
- 00000002e23161d4:	00000002e2312ce0 00000002e2312d92 00000002e2317174
- 00000002e23161e0:	00000002e2312da0 00000002e2312da3 00000002e231717c
- 00000002e23161ec:	00000002e2312df0 00000002e2312df6 00000002e2317180
- 00000002e23161f8:	00000002e2312e00 00000002e2312e06 00000002e2317184
- 00000002e2316204:	00000002e2312e10 00000002e2312f4f 00000002e2317188
- 00000002e2316210:	00000002e2312fc0 00000002e2312fe5 00000002e2317194
- 00000002e231621c:	00000002e2312ff0 00000002e23130c4 00000002e2317198
- 00000002e2316228:	00000002e23130d0 00000002e2313141 00000002e23171a8
- 00000002e2316234:	00000002e2313150 00000002e231316f 00000002e23171b4
- 00000002e2316240:	00000002e23131e0 00000002e2313221 00000002e23171bc
- 00000002e231624c:	00000002e2313230 00000002e231323c 00000002e23171c4
- 00000002e2316258:	00000002e2313250 00000002e2313255 00000002e23171c8
+ 00000002e231600c:	00000002e2311010 00000002e23111cf 00000002e2317004
+ 00000002e2316018:	00000002e23111d0 00000002e2311314 00000002e2317018
+ 00000002e2316024:	00000002e2311320 00000002e2311332 00000002e2317028
+ 00000002e2316030:	00000002e2311340 00000002e231134f 00000002e231702c
+ 00000002e231603c:	00000002e2311350 00000002e231135c 00000002e2317030
+ 00000002e2316048:	00000002e2311360 00000002e2311361 00000002e2317034
+ 00000002e2316054:	00000002e2311370 00000002e2311389 00000002e2317038
+ 00000002e2316060:	00000002e2311390 00000002e23113c5 00000002e231703c
+ 00000002e231606c:	00000002e23113d0 00000002e2311429 00000002e2317040
+ 00000002e2316078:	00000002e2311430 00000002e231149b 00000002e2317044
+ 00000002e2316084:	00000002e23114a0 00000002e2311519 00000002e2317048
+ 00000002e2316090:	00000002e2311520 00000002e231183c 00000002e2317058
+ 00000002e231609c:	00000002e2311840 00000002e2311845 00000002e2317078
+ 00000002e23160a8:	00000002e2311850 00000002e23120ef 00000002e231707c
+ 00000002e23160b4:	00000002e23120f0 00000002e2312120 00000002e2317098
+ 00000002e23160c0:	00000002e2312120 00000002e2312141 00000002e231709c
+ 00000002e23160cc:	00000002e2312150 00000002e231218a 00000002e23170a0
+ 00000002e23160d8:	00000002e2312190 00000002e23121fa 00000002e23170a8
+ 00000002e23160e4:	00000002e2312200 00000002e231221f 00000002e23170b4
+ 00000002e23160f0:	00000002e2312220 00000002e231224f 00000002e23170b8
+ 00000002e23160fc:	00000002e2312250 00000002e23122d1 00000002e23170c0
+ 00000002e2316108:	00000002e23122e0 00000002e23122e3 00000002e23170cc
+ 00000002e2316114:	00000002e23122f0 00000002e2312359 00000002e23170d0
+ 00000002e2316120:	00000002e2312360 00000002e23124c2 00000002e23170dc
+ 00000002e231612c:	00000002e23124d0 00000002e231282b 00000002e23170e8
+ 00000002e2316138:	00000002e2312830 00000002e23128a0 00000002e2317100
+ 00000002e2316144:	00000002e23128a0 00000002e231290f 00000002e2317110
+ 00000002e2316150:	00000002e2312910 00000002e2312991 00000002e231711c
+ 00000002e231615c:	00000002e23129a0 00000002e2312a92 00000002e2317128
+ 00000002e2316168:	00000002e2312aa0 00000002e2312acc 00000002e2317130
+ 00000002e2316174:	00000002e2312ad0 00000002e2312b20 00000002e2317134
+ 00000002e2316180:	00000002e2312b20 00000002e2312bbd 00000002e2317138
+ 00000002e231618c:	00000002e2312bc0 00000002e2312c40 00000002e2317144
+ 00000002e2316198:	00000002e2312c40 00000002e2312c77 00000002e2317148
+ 00000002e23161a4:	00000002e2312c80 00000002e2312cf3 00000002e231714c
+ 00000002e23161b0:	00000002e2312d00 00000002e2312d36 00000002e2317150
+ 00000002e23161bc:	00000002e2312d40 00000002e2312dc9 00000002e2317154
+ 00000002e23161c8:	00000002e2312dd0 00000002e2312e96 00000002e2317158
+ 00000002e23161d4:	00000002e2312ea0 00000002e2312ea3 00000002e231715c
+ 00000002e23161e0:	00000002e2312ef0 00000002e2312ef6 00000002e2317160
+ 00000002e23161ec:	00000002e2312f00 00000002e2312f06 00000002e2317164
+ 00000002e23161f8:	00000002e2312f10 00000002e2313043 00000002e2317168
+ 00000002e2316204:	00000002e2313050 00000002e231306f 00000002e2317174
+ 00000002e2316210:	00000002e2313070 00000002e231308d 00000002e231717c
+ 00000002e231621c:	00000002e2313090 00000002e2313160 00000002e2317180
+ 00000002e2316228:	00000002e2313160 00000002e23131c7 00000002e2317190
+ 00000002e2316234:	00000002e23132b0 00000002e23132ee 00000002e231719c
+ 00000002e2316240:	00000002e23132f0 00000002e23132fc 00000002e23171a4
+ 00000002e231624c:	00000002e2313310 00000002e2313315 00000002e23171a8
 
 Dump of .xdata
  00000002e2317000 (rva: 00007000): 00000002e2311000 - 00000002e231100c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317004 (rva: 00007004): 00000002e2311010 - 00000002e23111ff
+ 00000002e2317004 (rva: 00007004): 00000002e2311010 - 00000002e23111cf
 	Version: 1, Flags: none
 	Nbr codes: 7, Prologue size: 0x0c, Frame offset: 0x0, Frame reg: none
 	  pc+0x0c: alloc small area: rsp = rsp - 0x28
 	  pc+0x08: push rbx
 	  pc+0x07: push rsi
 	  pc+0x06: push rdi
 	  pc+0x05: push rbp
 	  pc+0x04: push r12
 	  pc+0x02: push r13
- 00000002e2317018 (rva: 00007018): 00000002e2311200 - 00000002e2311344
+ 00000002e2317018 (rva: 00007018): 00000002e23111d0 - 00000002e2311314
 	Version: 1, Flags: none
-	Nbr codes: 6, Prologue size: 0x0c, Frame offset: 0x0, Frame reg: none
-	  pc+0x0c: alloc small area: rsp = rsp - 0x20
-	  pc+0x08: push rbx
-	  pc+0x07: push rsi
-	  pc+0x06: push r12
-	  pc+0x04: push r13
-	  pc+0x02: push r14
- 00000002e2317028 (rva: 00007028): 00000002e2311350 - 00000002e2311362
+	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
+	  pc+0x0a: alloc small area: rsp = rsp - 0x20
+	  pc+0x06: push rbx
+	  pc+0x05: push rsi
+	  pc+0x04: push rdi
+	  pc+0x03: push rbp
+	  pc+0x02: push r12
+ 00000002e2317028 (rva: 00007028): 00000002e2311320 - 00000002e2311332
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e231702c (rva: 0000702c): 00000002e2311370 - 00000002e231137f
+ 00000002e231702c (rva: 0000702c): 00000002e2311340 - 00000002e231134f
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317030 (rva: 00007030): 00000002e2311380 - 00000002e231138c
+ 00000002e2317030 (rva: 00007030): 00000002e2311350 - 00000002e231135c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317034 (rva: 00007034): 00000002e2311390 - 00000002e2311391
+ 00000002e2317034 (rva: 00007034): 00000002e2311360 - 00000002e2311361
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317038 (rva: 00007038): 00000002e23113a0 - 00000002e23113b9
+ 00000002e2317038 (rva: 00007038): 00000002e2311370 - 00000002e2311389
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e231703c (rva: 0000703c): 00000002e23113c0 - 00000002e23113f5
+ 00000002e231703c (rva: 0000703c): 00000002e2311390 - 00000002e23113c5
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317040 (rva: 00007040): 00000002e2311400 - 00000002e2311461
+ 00000002e2317040 (rva: 00007040): 00000002e23113d0 - 00000002e2311429
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317044 (rva: 00007044): 00000002e2311470 - 00000002e23114f3
+ 00000002e2317044 (rva: 00007044): 00000002e2311430 - 00000002e231149b
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317048 (rva: 00007048): 00000002e2311500 - 00000002e2311581
+ 00000002e2317048 (rva: 00007048): 00000002e23114a0 - 00000002e2311519
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000002e2317058 (rva: 00007058): 00000002e2311590 - 00000002e23118a6
+ 00000002e2317058 (rva: 00007058): 00000002e2311520 - 00000002e231183c
 	Version: 1, Flags: none
-	Nbr codes: 16, Prologue size: 0x27, Frame offset: 0x0, Frame reg: none
-	  pc+0x27: save xmm10 at rsp + 0x70
-	  pc+0x21: save xmm9 at rsp + 0x60
-	  pc+0x1b: save xmm8 at rsp + 0x50
-	  pc+0x15: save xmm7 at rsp + 0x40
-	  pc+0x10: save xmm6 at rsp + 0x30
-	  pc+0x0b: alloc large area: rsp = rsp - 0x88
+	Nbr codes: 13, Prologue size: 0x1e, Frame offset: 0x0, Frame reg: none
+	  pc+0x1e: save xmm9 at rsp + 0x60
+	  pc+0x18: save xmm8 at rsp + 0x50
+	  pc+0x12: save xmm7 at rsp + 0x40
+	  pc+0x0d: save xmm6 at rsp + 0x30
+	  pc+0x08: alloc small area: rsp = rsp - 0x78
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000002e231707c (rva: 0000707c): 00000002e23118b0 - 00000002e23118b5
+ 00000002e2317078 (rva: 00007078): 00000002e2311840 - 00000002e2311845
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317080 (rva: 00007080): 00000002e23118c0 - 00000002e2311fdc
+ 00000002e231707c (rva: 0000707c): 00000002e2311850 - 00000002e23120ef
 	Version: 1, Flags: none
 	Nbr codes: 11, Prologue size: 0x15, Frame offset: 0x0, Frame reg: none
-	  pc+0x15: save xmm6 at rsp + 0x50
-	  pc+0x10: alloc small area: rsp = rsp - 0x68
+	  pc+0x15: save xmm6 at rsp + 0x60
+	  pc+0x10: alloc small area: rsp = rsp - 0x78
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push rbp
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 00000002e231709c (rva: 0000709c): 00000002e2311fe0 - 00000002e2312009
+ 00000002e2317098 (rva: 00007098): 00000002e23120f0 - 00000002e2312120
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e23170a0 (rva: 000070a0): 00000002e2312010 - 00000002e2312031
+ 00000002e231709c (rva: 0000709c): 00000002e2312120 - 00000002e2312141
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e23170a4 (rva: 000070a4): 00000002e2312040 - 00000002e231207a
+ 00000002e23170a0 (rva: 000070a0): 00000002e2312150 - 00000002e231218a
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e23170ac (rva: 000070ac): 00000002e2312080 - 00000002e23120ea
+ 00000002e23170a8 (rva: 000070a8): 00000002e2312190 - 00000002e23121fa
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000002e23170b8 (rva: 000070b8): 00000002e23120f0 - 00000002e231210f
+ 00000002e23170b4 (rva: 000070b4): 00000002e2312200 - 00000002e231221f
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e23170bc (rva: 000070bc): 00000002e2312110 - 00000002e231213f
+ 00000002e23170b8 (rva: 000070b8): 00000002e2312220 - 00000002e231224f
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e23170c4 (rva: 000070c4): 00000002e2312140 - 00000002e23121c1
+ 00000002e23170c0 (rva: 000070c0): 00000002e2312250 - 00000002e23122d1
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000002e23170d0 (rva: 000070d0): 00000002e23121d0 - 00000002e23121d3
+ 00000002e23170cc (rva: 000070cc): 00000002e23122e0 - 00000002e23122e3
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e23170d4 (rva: 000070d4): 00000002e23121e0 - 00000002e231224a
+ 00000002e23170d0 (rva: 000070d0): 00000002e23122f0 - 00000002e2312359
 	Version: 1, Flags: none
-	Nbr codes: 3, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
-	  pc+0x07: alloc small area: rsp = rsp - 0x38
-	  pc+0x03: push rbx
-	  pc+0x02: push r12
- 00000002e23170e0 (rva: 000070e0): 00000002e2312250 - 00000002e231246d
+	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
+	  pc+0x06: alloc small area: rsp = rsp - 0x38
+	  pc+0x02: push rbx
+	  pc+0x01: push rsi
+ 00000002e23170dc (rva: 000070dc): 00000002e2312360 - 00000002e23124c2
 	Version: 1, Flags: none
-	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
-	  pc+0x0a: alloc small area: rsp = rsp - 0x50
-	  pc+0x06: push rbx
-	  pc+0x05: push rsi
-	  pc+0x04: push rdi
-	  pc+0x03: push rbp
-	  pc+0x02: push r12
- 00000002e23170f0 (rva: 000070f0): 00000002e2312470 - 00000002e2312755
+	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
+	  pc+0x07: alloc small area: rsp = rsp - 0x50
+	  pc+0x03: push rbx
+	  pc+0x02: push rsi
+	  pc+0x01: push rdi
+ 00000002e23170e8 (rva: 000070e8): 00000002e23124d0 - 00000002e231282b
 	Version: 1, Flags: none
-	Nbr codes: 10, Prologue size: 0x18, Frame offset: 0x8, Frame reg: rbp
-	  pc+0x18: FPReg: rbp = rsp + 0x80 (info = 0x0)
-	  pc+0x10: alloc small area: rsp = rsp - 0x38
+	Nbr codes: 10, Prologue size: 0x15, Frame offset: 0x4, Frame reg: rbp
+	  pc+0x15: FPReg: rbp = rsp + 0x40 (info = 0x0)
+	  pc+0x10: alloc small area: rsp = rsp - 0x48
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push r12
 	  pc+0x07: push r13
 	  pc+0x05: push r14
 	  pc+0x03: push r15
 	  pc+0x01: push rbp
- 00000002e2317108 (rva: 00007108): 00000002e2312760 - 00000002e23127cb
+ 00000002e2317100 (rva: 00007100): 00000002e2312830 - 00000002e23128a0
 	Version: 1, Flags: none
-	Nbr codes: 5, Prologue size: 0x09, Frame offset: 0x0, Frame reg: none
-	  pc+0x09: alloc small area: rsp = rsp - 0x28
-	  pc+0x05: push rbx
-	  pc+0x04: push rsi
-	  pc+0x03: push rdi
+	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
+	  pc+0x0a: alloc small area: rsp = rsp - 0x20
+	  pc+0x06: push rbx
+	  pc+0x05: push rsi
+	  pc+0x04: push rdi
+	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000002e2317118 (rva: 00007118): 00000002e23127d0 - 00000002e2312848
+ 00000002e2317110 (rva: 00007110): 00000002e23128a0 - 00000002e231290f
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000002e2317124 (rva: 00007124): 00000002e2312850 - 00000002e23128d9
+ 00000002e231711c (rva: 0000711c): 00000002e2312910 - 00000002e2312991
 	Version: 1, Flags: none
-	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
-	  pc+0x05: alloc small area: rsp = rsp - 0x20
-	  pc+0x01: push rbx
- 00000002e231712c (rva: 0000712c): 00000002e23128e0 - 00000002e23129c0
+	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
+	  pc+0x06: alloc small area: rsp = rsp - 0x28
+	  pc+0x02: push rbx
+	  pc+0x01: push rsi
+ 00000002e2317128 (rva: 00007128): 00000002e23129a0 - 00000002e2312a92
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000002e2317134 (rva: 00007134): 00000002e23129c0 - 00000002e23129de
+ 00000002e2317130 (rva: 00007130): 00000002e2312aa0 - 00000002e2312acc
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317138 (rva: 00007138): 00000002e23129e0 - 00000002e23129f3
+ 00000002e2317134 (rva: 00007134): 00000002e2312ad0 - 00000002e2312b20
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e231713c (rva: 0000713c): 00000002e2312a00 - 00000002e2312a48
+ 00000002e2317138 (rva: 00007138): 00000002e2312b20 - 00000002e2312bbd
 	Version: 1, Flags: none
-	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317140 (rva: 00007140): 00000002e2312a50 - 00000002e2312aef
-	Version: 1, Flags: none
-	Nbr codes: 4, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
-	  pc+0x08: alloc small area: rsp = rsp - 0x20
-	  pc+0x04: push rbx
-	  pc+0x03: push rsi
-	  pc+0x02: push r12
- 00000002e231714c (rva: 0000714c): 00000002e2312af0 - 00000002e2312b71
+	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
+	  pc+0x07: alloc small area: rsp = rsp - 0x20
+	  pc+0x03: push rbx
+	  pc+0x02: push rsi
+	  pc+0x01: push rdi
+ 00000002e2317144 (rva: 00007144): 00000002e2312bc0 - 00000002e2312c40
 	Version: 1, Flags: none
-	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
-	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e2317154 (rva: 00007154): 00000002e2312b80 - 00000002e2312bab
+	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
+ 00000002e2317148 (rva: 00007148): 00000002e2312c40 - 00000002e2312c77
 	Version: 1, Flags: none
-	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
-	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e231715c (rva: 0000715c): 00000002e2312bb0 - 00000002e2312c1c
+	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
+ 00000002e231714c (rva: 0000714c): 00000002e2312c80 - 00000002e2312cf3
 	Version: 1, Flags: none
-	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
-	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e2317164 (rva: 00007164): 00000002e2312c20 - 00000002e2312c48
+	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
+ 00000002e2317150 (rva: 00007150): 00000002e2312d00 - 00000002e2312d36
 	Version: 1, Flags: none
-	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
-	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e231716c (rva: 0000716c): 00000002e2312c50 - 00000002e2312cd5
+	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
+ 00000002e2317154 (rva: 00007154): 00000002e2312d40 - 00000002e2312dc9
 	Version: 1, Flags: none
-	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
-	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e2317174 (rva: 00007174): 00000002e2312ce0 - 00000002e2312d92
+	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
+ 00000002e2317158 (rva: 00007158): 00000002e2312dd0 - 00000002e2312e96
 	Version: 1, Flags: none
-	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
-	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e231717c (rva: 0000717c): 00000002e2312da0 - 00000002e2312da3
+	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
+ 00000002e231715c (rva: 0000715c): 00000002e2312ea0 - 00000002e2312ea3
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317180 (rva: 00007180): 00000002e2312df0 - 00000002e2312df6
+ 00000002e2317160 (rva: 00007160): 00000002e2312ef0 - 00000002e2312ef6
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317184 (rva: 00007184): 00000002e2312e00 - 00000002e2312e06
+ 00000002e2317164 (rva: 00007164): 00000002e2312f00 - 00000002e2312f06
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317188 (rva: 00007188): 00000002e2312e10 - 00000002e2312f4f
+ 00000002e2317168 (rva: 00007168): 00000002e2312f10 - 00000002e2313043
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x40
 	  pc+0x05: alloc small area: rsp = rsp - 0x50
 	  pc+0x01: push rbx
- 00000002e2317194 (rva: 00007194): 00000002e2312fc0 - 00000002e2312fe5
+ 00000002e2317174 (rva: 00007174): 00000002e2313050 - 00000002e231306f
+	Version: 1, Flags: none
+	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
+	  pc+0x05: alloc small area: rsp = rsp - 0x20
+	  pc+0x01: push rbx
+ 00000002e231717c (rva: 0000717c): 00000002e2313070 - 00000002e231308d
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317198 (rva: 00007198): 00000002e2312ff0 - 00000002e23130c4
+ 00000002e2317180 (rva: 00007180): 00000002e2313090 - 00000002e2313160
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000002e23171a8 (rva: 000071a8): 00000002e23130d0 - 00000002e2313141
-	Version: 1, Flags: none
-	Nbr codes: 4, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
-	  pc+0x08: alloc small area: rsp = rsp - 0x20
-	  pc+0x04: push rbx
-	  pc+0x03: push rsi
-	  pc+0x02: push r12
- 00000002e23171b4 (rva: 000071b4): 00000002e2313150 - 00000002e231316f
+ 00000002e2317190 (rva: 00007190): 00000002e2313160 - 00000002e23131c7
 	Version: 1, Flags: none
-	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
-	  pc+0x05: alloc small area: rsp = rsp - 0x20
-	  pc+0x01: push rbx
- 00000002e23171bc (rva: 000071bc): 00000002e23131e0 - 00000002e2313221
+	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
+	  pc+0x07: alloc small area: rsp = rsp - 0x20
+	  pc+0x03: push rbx
+	  pc+0x02: push rsi
+	  pc+0x01: push rdi
+ 00000002e231719c (rva: 0000719c): 00000002e23132b0 - 00000002e23132ee
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x58
- 00000002e23171c4 (rva: 000071c4): 00000002e2313230 - 00000002e231323c
+ 00000002e23171a4 (rva: 000071a4): 00000002e23132f0 - 00000002e23132fc
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e23171c8 (rva: 000071c8): 00000002e2313250 - 00000002e2313255
+ 00000002e23171a8 (rva: 000071a8): 00000002e2313310 - 00000002e2313315
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 
 
 PE File Base Relocations (interpreted .reloc section contents)
 
 Virtual Address: 00003000 Chunk size 12 (0xc) Number of fixups 2
-	reloc    0 offset  268 [3268] DIR64
+	reloc    0 offset  328 [3328] DIR64
 	reloc    1 offset    0 [3000] ABSOLUTE
 
 Virtual Address: 00004000 Chunk size 20 (0x14) Number of fixups 6
 	reloc    0 offset   10 [4010] DIR64
 	reloc    1 offset   40 [4040] DIR64
-	reloc    2 offset   48 [4048] DIR64
-	reloc    3 offset   50 [4050] DIR64
+	reloc    2 offset   50 [4050] DIR64
+	reloc    3 offset   58 [4058] DIR64
 	reloc    4 offset   60 [4060] DIR64
 	reloc    5 offset    0 [4000] ABSOLUTE
 
 Virtual Address: 00005000 Chunk size 48 (0x30) Number of fixups 20
 	reloc    0 offset   20 [5020] DIR64
 	reloc    1 offset   40 [5040] DIR64
 	reloc    2 offset   48 [5048] DIR64
 	reloc    3 offset   50 [5050] DIR64
 	reloc    4 offset   58 [5058] DIR64
-	reloc    5 offset  1c0 [51c0] DIR64
-	reloc    6 offset  1d0 [51d0] DIR64
-	reloc    7 offset  1e0 [51e0] DIR64
-	reloc    8 offset  1f0 [51f0] DIR64
-	reloc    9 offset  200 [5200] DIR64
-	reloc   10 offset  210 [5210] DIR64
-	reloc   11 offset  220 [5220] DIR64
-	reloc   12 offset  230 [5230] DIR64
-	reloc   13 offset  240 [5240] DIR64
-	reloc   14 offset  250 [5250] DIR64
-	reloc   15 offset  260 [5260] DIR64
-	reloc   16 offset  270 [5270] DIR64
-	reloc   17 offset  280 [5280] DIR64
-	reloc   18 offset  290 [5290] DIR64
+	reloc    5 offset  210 [5210] DIR64
+	reloc    6 offset  220 [5220] DIR64
+	reloc    7 offset  230 [5230] DIR64
+	reloc    8 offset  240 [5240] DIR64
+	reloc    9 offset  250 [5250] DIR64
+	reloc   10 offset  260 [5260] DIR64
+	reloc   11 offset  270 [5270] DIR64
+	reloc   12 offset  280 [5280] DIR64
+	reloc   13 offset  290 [5290] DIR64
+	reloc   14 offset  2a0 [52a0] DIR64
+	reloc   15 offset  2b0 [52b0] DIR64
+	reloc   16 offset  2c0 [52c0] DIR64
+	reloc   17 offset  2d0 [52d0] DIR64
+	reloc   18 offset  2e0 [52e0] DIR64
 	reloc   19 offset    0 [5000] ABSOLUTE
 
 Virtual Address: 0000b000 Chunk size 16 (0x10) Number of fixups 4
 	reloc    0 offset   18 [b018] DIR64
 	reloc    1 offset   30 [b030] DIR64
 	reloc    2 offset   38 [b038] DIR64
 	reloc    3 offset    0 [b000] ABSOLUTE
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
-  0 .text         00002288  00000002e2311000  00000002e2311000  00000400  2**4
+  0 .text         00002348  00000002e2311000  00000002e2311000  00000400  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE, DATA
   1 .data         00000070  00000002e2314000  00000002e2314000  00002800  2**4
                   CONTENTS, ALLOC, LOAD, DATA
-  2 .rdata        00000560  00000002e2315000  00000002e2315000  00002a00  2**4
+  2 .rdata        000005b0  00000002e2315000  00000002e2315000  00002a00  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  3 .pdata        00000264  00000002e2316000  00000002e2316000  00003000  2**2
+  3 .pdata        00000258  00000002e2316000  00000002e2316000  00003000  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  4 .xdata        000001cc  00000002e2317000  00000002e2317000  00003400  2**2
+  4 .xdata        000001ac  00000002e2317000  00000002e2317000  00003400  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  5 .bss          00000110  00000002e2318000  00000002e2318000  00000000  2**4
+  5 .bss          00000120  00000002e2318000  00000002e2318000  00000000  2**4
                   ALLOC
   6 .edata        000000ff  00000002e2319000  00000002e2319000  00003600  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  7 .idata        00000404  00000002e231a000  00000002e231a000  00003800  2**2
+  7 .idata        00000408  00000002e231a000  00000002e231a000  00003800  2**2
                   CONTENTS, ALLOC, LOAD, DATA
   8 .CRT          00000058  00000002e231b000  00000002e231b000  00003e00  2**2
                   CONTENTS, ALLOC, LOAD, DATA
   9 .tls          00000010  00000002e231c000  00000002e231c000  00004000  2**2
                   CONTENTS, ALLOC, LOAD, DATA
  10 .reloc        00000060  00000002e231d000  00000002e231d000  00004200  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
@@ -532,2544 +521,2575 @@
 
 
 
 Disassembly of section .text:
 
 00000002e2311000 <.text>:
    2e2311000:	lea    0x6ff9(%rip),%rcx        # 0x2e2318000
-   2e2311007:	jmp    0x2e2312fc0
+   2e2311007:	jmp    0x2e2313070
    2e231100c:	nopl   0x0(%rax)
    2e2311010:	push   %r13
    2e2311012:	push   %r12
    2e2311014:	push   %rbp
    2e2311015:	push   %rdi
    2e2311016:	push   %rsi
    2e2311017:	push   %rbx
    2e2311018:	sub    $0x28,%rsp
-   2e231101c:	mov    %rcx,%r12
+   2e231101c:	mov    %rcx,%rdi
    2e231101f:	mov    %r8,%r13
    2e2311022:	test   %edx,%edx
    2e2311024:	jne    0x2e23110a0
-   2e2311026:	mov    0x6fec(%rip),%edx        # 0x2e2318018
-   2e231102c:	xor    %eax,%eax
-   2e231102e:	test   %edx,%edx
-   2e2311030:	jle    0x2e2311090
-   2e2311032:	sub    $0x1,%edx
-   2e2311035:	mov    0x41f4(%rip),%rbx        # 0x2e2315230
-   2e231103c:	xor    %r12d,%r12d
-   2e231103f:	mov    $0x1,%edi
-   2e2311044:	mov    %edx,0x6fce(%rip)        # 0x2e2318018
-   2e231104a:	mov    0x90fb(%rip),%rbp        # 0x2e231a14c
-   2e2311051:	jmp    0x2e231105f
-   2e2311053:	nopl   0x0(%rax,%rax,1)
-   2e2311058:	mov    $0x3e8,%ecx
-   2e231105d:	call   *%rbp
-   2e231105f:	mov    %r12,%rax
-   2e2311062:	lock cmpxchg %rdi,(%rbx)
-   2e2311067:	mov    %rax,%rsi
-   2e231106a:	test   %rax,%rax
-   2e231106d:	jne    0x2e2311058
-   2e231106f:	mov    0x41ca(%rip),%rdi        # 0x2e2315240
-   2e2311076:	mov    (%rdi),%eax
-   2e2311078:	cmp    $0x2,%eax
-   2e231107b:	je     0x2e2311170
-   2e2311081:	mov    $0x1f,%ecx
-   2e2311086:	call   0x2e2312fb0
-   2e231108b:	mov    $0x1,%eax
-   2e2311090:	add    $0x28,%rsp
-   2e2311094:	pop    %rbx
-   2e2311095:	pop    %rsi
-   2e2311096:	pop    %rdi
-   2e2311097:	pop    %rbp
-   2e2311098:	pop    %r12
-   2e231109a:	pop    %r13
-   2e231109c:	ret
-   2e231109d:	nopl   (%rax)
+   2e2311026:	mov    0x6fec(%rip),%eax        # 0x2e2318018
+   2e231102c:	test   %eax,%eax
+   2e231102e:	jle    0x2e2311089
+   2e2311030:	sub    $0x1,%eax
+   2e2311033:	mov    0x4256(%rip),%rbx        # 0x2e2315290
+   2e231103a:	xor    %ebp,%ebp
+   2e231103c:	mov    $0x1,%edi
+   2e2311041:	mov    %eax,0x6fd1(%rip)        # 0x2e2318018
+   2e2311047:	mov    0x9102(%rip),%r12        # 0x2e231a150
+   2e231104e:	jmp    0x2e2311058
+   2e2311050:	mov    $0x3e8,%ecx
+   2e2311055:	call   *%r12
+   2e2311058:	mov    %rbp,%rax
+   2e231105b:	lock cmpxchg %rdi,(%rbx)
+   2e2311060:	mov    %rax,%rsi
+   2e2311063:	test   %rax,%rax
+   2e2311066:	jne    0x2e2311050
+   2e2311068:	mov    0x4231(%rip),%rdi        # 0x2e23152a0
+   2e231106f:	mov    (%rdi),%eax
+   2e2311071:	cmp    $0x2,%eax
+   2e2311074:	je     0x2e2311140
+   2e231107a:	mov    $0x1f,%ecx
+   2e231107f:	call   0x2e23131d8
+   2e2311084:	mov    $0x1,%edx
+   2e2311089:	mov    %edx,%eax
+   2e231108b:	add    $0x28,%rsp
+   2e231108f:	pop    %rbx
+   2e2311090:	pop    %rsi
+   2e2311091:	pop    %rdi
+   2e2311092:	pop    %rbp
+   2e2311093:	pop    %r12
+   2e2311095:	pop    %r13
+   2e2311097:	ret
+   2e2311098:	nopl   0x0(%rax,%rax,1)
    2e23110a0:	cmp    $0x1,%edx
-   2e23110a3:	jne    0x2e2311158
-   2e23110a9:	mov    %gs:0x30,%rax
-   2e23110b2:	mov    0x4177(%rip),%rbx        # 0x2e2315230
-   2e23110b9:	mov    0x8(%rax),%rsi
-   2e23110bd:	xor    %edi,%edi
-   2e23110bf:	mov    0x9086(%rip),%rbp        # 0x2e231a14c
-   2e23110c6:	jmp    0x2e23110e0
-   2e23110c8:	nopl   0x0(%rax,%rax,1)
-   2e23110d0:	cmp    %rax,%rsi
-   2e23110d3:	je     0x2e2311190
-   2e23110d9:	mov    $0x3e8,%ecx
-   2e23110de:	call   *%rbp
-   2e23110e0:	mov    %rdi,%rax
-   2e23110e3:	lock cmpxchg %rsi,(%rbx)
-   2e23110e8:	test   %rax,%rax
-   2e23110eb:	jne    0x2e23110d0
-   2e23110ed:	xor    %edi,%edi
-   2e23110ef:	mov    0x414a(%rip),%rsi        # 0x2e2315240
-   2e23110f6:	mov    (%rsi),%eax
-   2e23110f8:	cmp    $0x1,%eax
-   2e23110fb:	je     0x2e23111f0
-   2e2311101:	mov    (%rsi),%eax
-   2e2311103:	test   %eax,%eax
-   2e2311105:	je     0x2e23111b0
-   2e231110b:	mov    (%rsi),%eax
-   2e231110d:	cmp    $0x1,%eax
-   2e2311110:	je     0x2e23111d0
-   2e2311116:	test   %edi,%edi
-   2e2311118:	je     0x2e23111a0
-   2e231111e:	mov    0x40db(%rip),%rax        # 0x2e2315200
-   2e2311125:	mov    (%rax),%rax
-   2e2311128:	test   %rax,%rax
-   2e231112b:	je     0x2e231113a
-   2e231112d:	mov    %r13,%r8
-   2e2311130:	mov    $0x2,%edx
-   2e2311135:	mov    %r12,%rcx
-   2e2311138:	call   *%rax
-   2e231113a:	addl   $0x1,0x6ed7(%rip)        # 0x2e2318018
-   2e2311141:	mov    $0x1,%eax
-   2e2311146:	add    $0x28,%rsp
-   2e231114a:	pop    %rbx
-   2e231114b:	pop    %rsi
-   2e231114c:	pop    %rdi
-   2e231114d:	pop    %rbp
-   2e231114e:	pop    %r12
-   2e2311150:	pop    %r13
-   2e2311152:	ret
-   2e2311153:	nopl   0x0(%rax,%rax,1)
-   2e2311158:	mov    $0x1,%eax
-   2e231115d:	add    $0x28,%rsp
-   2e2311161:	pop    %rbx
-   2e2311162:	pop    %rsi
-   2e2311163:	pop    %rdi
-   2e2311164:	pop    %rbp
-   2e2311165:	pop    %r12
-   2e2311167:	pop    %r13
-   2e2311169:	ret
-   2e231116a:	nopw   0x0(%rax,%rax,1)
-   2e2311170:	lea    0x6e89(%rip),%rcx        # 0x2e2318000
-   2e2311177:	call   0x2e23130d0
-   2e231117c:	movl   $0x0,(%rdi)
-   2e2311182:	xchg   %rsi,(%rbx)
-   2e2311185:	mov    $0x1,%eax
-   2e231118a:	jmp    0x2e2311090
-   2e231118f:	nop
-   2e2311190:	mov    $0x1,%edi
-   2e2311195:	jmp    0x2e23110ef
-   2e231119a:	nopw   0x0(%rax,%rax,1)
-   2e23111a0:	xor    %eax,%eax
-   2e23111a2:	xchg   %rax,(%rbx)
-   2e23111a5:	jmp    0x2e231111e
-   2e23111aa:	nopw   0x0(%rax,%rax,1)
-   2e23111b0:	mov    0x40c9(%rip),%rdx        # 0x2e2315280
-   2e23111b7:	mov    0x40b2(%rip),%rcx        # 0x2e2315270
-   2e23111be:	movl   $0x1,(%rsi)
-   2e23111c4:	call   0x2e2312fa0
-   2e23111c9:	jmp    0x2e231110b
-   2e23111ce:	xchg   %ax,%ax
-   2e23111d0:	mov    0x4089(%rip),%rdx        # 0x2e2315260
-   2e23111d7:	mov    0x4072(%rip),%rcx        # 0x2e2315250
-   2e23111de:	call   0x2e2312fa0
-   2e23111e3:	movl   $0x2,(%rsi)
-   2e23111e9:	jmp    0x2e2311116
-   2e23111ee:	xchg   %ax,%ax
-   2e23111f0:	mov    $0x1f,%ecx
-   2e23111f5:	call   0x2e2312fb0
-   2e23111fa:	jmp    0x2e231110b
-   2e23111ff:	nop
-   2e2311200:	push   %r14
-   2e2311202:	push   %r13
-   2e2311204:	push   %r12
-   2e2311206:	push   %rsi
-   2e2311207:	push   %rbx
-   2e2311208:	sub    $0x20,%rsp
-   2e231120c:	mov    0x400d(%rip),%rsi        # 0x2e2315220
-   2e2311213:	mov    %rcx,%r13
-   2e2311216:	mov    %edx,(%rsi)
-   2e2311218:	mov    %edx,%r12d
-   2e231121b:	mov    %r8,%rbx
-   2e231121e:	test   %edx,%edx
-   2e2311220:	jne    0x2e2311280
-   2e2311222:	mov    0x6df0(%rip),%eax        # 0x2e2318018
-   2e2311228:	test   %eax,%eax
-   2e231122a:	je     0x2e2311261
-   2e231122c:	call   0x2e2312470
-   2e2311231:	mov    %rbx,%r8
-   2e2311234:	xor    %edx,%edx
-   2e2311236:	mov    %r13,%rcx
-   2e2311239:	call   0x2e2312e00
-   2e231123e:	mov    %rbx,%r8
-   2e2311241:	mov    %r12d,%edx
-   2e2311244:	mov    %r13,%rcx
-   2e2311247:	call   0x2e2312df0
-   2e231124c:	mov    %rbx,%r8
-   2e231124f:	mov    %r12d,%edx
-   2e2311252:	mov    %r13,%rcx
-   2e2311255:	mov    %eax,%r14d
-   2e2311258:	call   0x2e2311010
-   2e231125d:	test   %eax,%eax
-   2e231125f:	jne    0x2e2311264
-   2e2311261:	xor    %r14d,%r14d
-   2e2311264:	mov    %r14d,%eax
-   2e2311267:	movl   $0xffffffff,(%rsi)
-   2e231126d:	add    $0x20,%rsp
-   2e2311271:	pop    %rbx
-   2e2311272:	pop    %rsi
-   2e2311273:	pop    %r12
-   2e2311275:	pop    %r13
-   2e2311277:	pop    %r14
-   2e2311279:	ret
-   2e231127a:	nopw   0x0(%rax,%rax,1)
-   2e2311280:	call   0x2e2312470
-   2e2311285:	lea    -0x1(%r12),%eax
-   2e231128a:	mov    %rbx,%r8
-   2e231128d:	mov    %r12d,%edx
-   2e2311290:	mov    %r13,%rcx
-   2e2311293:	cmp    $0x1,%eax
-   2e2311296:	ja     0x2e2311308
-   2e2311298:	call   0x2e2311010
-   2e231129d:	test   %eax,%eax
-   2e231129f:	je     0x2e2311261
-   2e23112a1:	mov    %rbx,%r8
-   2e23112a4:	mov    %r12d,%edx
-   2e23112a7:	mov    %r13,%rcx
-   2e23112aa:	call   0x2e2312df0
-   2e23112af:	mov    %eax,%r14d
-   2e23112b2:	test   %eax,%eax
-   2e23112b4:	je     0x2e2311320
-   2e23112b6:	cmp    $0x1,%r12d
-   2e23112ba:	jne    0x2e231132c
-   2e23112bc:	call   0x2e23120f0
-   2e23112c1:	mov    %rbx,%r8
-   2e23112c4:	mov    $0x1,%edx
-   2e23112c9:	mov    %r13,%rcx
-   2e23112cc:	call   0x2e2312e00
-   2e23112d1:	mov    %eax,%r14d
-   2e23112d4:	test   %eax,%eax
-   2e23112d6:	jne    0x2e2311264
-   2e23112d8:	mov    %rbx,%r8
-   2e23112db:	xor    %edx,%edx
-   2e23112dd:	mov    %r13,%rcx
-   2e23112e0:	call   0x2e2312e00
-   2e23112e5:	mov    %rbx,%r8
-   2e23112e8:	xor    %edx,%edx
-   2e23112ea:	mov    %r13,%rcx
-   2e23112ed:	call   0x2e2312df0
-   2e23112f2:	mov    %rbx,%r8
-   2e23112f5:	xor    %edx,%edx
-   2e23112f7:	mov    %r13,%rcx
-   2e23112fa:	call   0x2e2311010
-   2e23112ff:	jmp    0x2e2311264
+   2e23110a3:	jne    0x2e2311084
+   2e23110a5:	mov    %gs:0x30,%rax
+   2e23110ae:	mov    0x41db(%rip),%rbx        # 0x2e2315290
+   2e23110b5:	mov    0x8(%rax),%rsi
+   2e23110b9:	xor    %ebp,%ebp
+   2e23110bb:	mov    0x908e(%rip),%r12        # 0x2e231a150
+   2e23110c2:	jmp    0x2e23110d9
+   2e23110c4:	nopl   0x0(%rax)
+   2e23110c8:	cmp    %rax,%rsi
+   2e23110cb:	je     0x2e2311160
+   2e23110d1:	mov    $0x3e8,%ecx
+   2e23110d6:	call   *%r12
+   2e23110d9:	mov    %rbp,%rax
+   2e23110dc:	lock cmpxchg %rsi,(%rbx)
+   2e23110e1:	test   %rax,%rax
+   2e23110e4:	jne    0x2e23110c8
+   2e23110e6:	xor    %ebp,%ebp
+   2e23110e8:	mov    0x41b1(%rip),%rsi        # 0x2e23152a0
+   2e23110ef:	mov    (%rsi),%eax
+   2e23110f1:	cmp    $0x1,%eax
+   2e23110f4:	je     0x2e23111c0
+   2e23110fa:	mov    (%rsi),%eax
+   2e23110fc:	test   %eax,%eax
+   2e23110fe:	je     0x2e2311180
+   2e2311104:	mov    (%rsi),%eax
+   2e2311106:	cmp    $0x1,%eax
+   2e2311109:	je     0x2e23111a0
+   2e231110f:	test   %ebp,%ebp
+   2e2311111:	je     0x2e2311170
+   2e2311113:	mov    0x4136(%rip),%rax        # 0x2e2315250
+   2e231111a:	mov    (%rax),%rax
+   2e231111d:	test   %rax,%rax
+   2e2311120:	je     0x2e231112f
+   2e2311122:	mov    %r13,%r8
+   2e2311125:	mov    $0x2,%edx
+   2e231112a:	mov    %rdi,%rcx
+   2e231112d:	call   *%rax
+   2e231112f:	addl   $0x1,0x6ee2(%rip)        # 0x2e2318018
+   2e2311136:	mov    $0x1,%edx
+   2e231113b:	jmp    0x2e2311089
+   2e2311140:	lea    0x6eb9(%rip),%rcx        # 0x2e2318000
+   2e2311147:	call   0x2e2313160
+   2e231114c:	movl   $0x0,(%rdi)
+   2e2311152:	xchg   %rsi,(%rbx)
+   2e2311155:	jmp    0x2e2311084
+   2e231115a:	nopw   0x0(%rax,%rax,1)
+   2e2311160:	mov    $0x1,%ebp
+   2e2311165:	jmp    0x2e23110e8
+   2e2311167:	nopw   0x0(%rax,%rax,1)
+   2e2311170:	xor    %eax,%eax
+   2e2311172:	xchg   %rax,(%rbx)
+   2e2311175:	jmp    0x2e2311113
+   2e2311177:	nopw   0x0(%rax,%rax,1)
+   2e2311180:	mov    0x4159(%rip),%rdx        # 0x2e23152e0
+   2e2311187:	mov    0x4142(%rip),%rcx        # 0x2e23152d0
+   2e231118e:	movl   $0x1,(%rsi)
+   2e2311194:	call   0x2e23131e8
+   2e2311199:	jmp    0x2e2311104
+   2e231119e:	xchg   %ax,%ax
+   2e23111a0:	mov    0x4119(%rip),%rdx        # 0x2e23152c0
+   2e23111a7:	mov    0x4102(%rip),%rcx        # 0x2e23152b0
+   2e23111ae:	call   0x2e23131e8
+   2e23111b3:	movl   $0x2,(%rsi)
+   2e23111b9:	jmp    0x2e231110f
+   2e23111be:	xchg   %ax,%ax
+   2e23111c0:	mov    $0x1f,%ecx
+   2e23111c5:	call   0x2e23131d8
+   2e23111ca:	jmp    0x2e2311104
+   2e23111cf:	nop
+   2e23111d0:	push   %r12
+   2e23111d2:	push   %rbp
+   2e23111d3:	push   %rdi
+   2e23111d4:	push   %rsi
+   2e23111d5:	push   %rbx
+   2e23111d6:	sub    $0x20,%rsp
+   2e23111da:	mov    0x409f(%rip),%r12        # 0x2e2315280
+   2e23111e1:	mov    %rcx,%rsi
+   2e23111e4:	mov    %edx,(%r12)
+   2e23111e8:	mov    %edx,%ebx
+   2e23111ea:	mov    %r8,%rdi
+   2e23111ed:	test   %edx,%edx
+   2e23111ef:	jne    0x2e2311238
+   2e23111f1:	mov    0x6e21(%rip),%eax        # 0x2e2318018
+   2e23111f7:	test   %eax,%eax
+   2e23111f9:	je     0x2e231125a
+   2e23111fb:	call   0x2e23124d0
+   2e2311200:	mov    %rdi,%r8
+   2e2311203:	mov    %ebx,%edx
+   2e2311205:	mov    %rsi,%rcx
+   2e2311208:	call   0x2e2312f00
+   2e231120d:	mov    %eax,%ebp
+   2e231120f:	test   %ebx,%ebx
+   2e2311211:	je     0x2e23112c8
+   2e2311217:	cmp    $0x3,%ebx
+   2e231121a:	je     0x2e23112c8
+   2e2311220:	mov    %ebp,%eax
+   2e2311222:	movl   $0xffffffff,(%r12)
+   2e231122a:	add    $0x20,%rsp
+   2e231122e:	pop    %rbx
+   2e231122f:	pop    %rsi
+   2e2311230:	pop    %rdi
+   2e2311231:	pop    %rbp
+   2e2311232:	pop    %r12
+   2e2311234:	ret
+   2e2311235:	nopl   (%rax)
+   2e2311238:	call   0x2e23124d0
+   2e231123d:	lea    -0x1(%rbx),%eax
+   2e2311240:	mov    %rdi,%r8
+   2e2311243:	mov    %ebx,%edx
+   2e2311245:	mov    %rsi,%rcx
+   2e2311248:	cmp    $0x1,%eax
+   2e231124b:	ja     0x2e23112f8
+   2e2311251:	call   0x2e2311010
+   2e2311256:	test   %eax,%eax
+   2e2311258:	jne    0x2e2311260
+   2e231125a:	xor    %ebp,%ebp
+   2e231125c:	jmp    0x2e2311220
+   2e231125e:	xchg   %ax,%ax
+   2e2311260:	mov    %rdi,%r8
+   2e2311263:	mov    %ebx,%edx
+   2e2311265:	mov    %rsi,%rcx
+   2e2311268:	call   0x2e2312ef0
+   2e231126d:	test   %eax,%eax
+   2e231126f:	je     0x2e2311308
+   2e2311275:	cmp    $0x1,%ebx
+   2e2311278:	jne    0x2e2311200
+   2e231127a:	call   0x2e2312200
+   2e231127f:	mov    %rdi,%r8
+   2e2311282:	mov    $0x1,%edx
+   2e2311287:	mov    %rsi,%rcx
+   2e231128a:	call   0x2e2312f00
+   2e231128f:	mov    %eax,%ebp
+   2e2311291:	test   %eax,%eax
+   2e2311293:	jne    0x2e2311220
+   2e2311295:	mov    %rdi,%r8
+   2e2311298:	xor    %edx,%edx
+   2e231129a:	mov    %rsi,%rcx
+   2e231129d:	call   0x2e2312f00
+   2e23112a2:	mov    %rdi,%r8
+   2e23112a5:	xor    %edx,%edx
+   2e23112a7:	mov    %rsi,%rcx
+   2e23112aa:	call   0x2e2312ef0
+   2e23112af:	mov    %rdi,%r8
+   2e23112b2:	xor    %edx,%edx
+   2e23112b4:	mov    %rsi,%rcx
+   2e23112b7:	xor    %ebp,%ebp
+   2e23112b9:	call   0x2e2311010
+   2e23112be:	jmp    0x2e2311220
+   2e23112c3:	nopl   0x0(%rax,%rax,1)
+   2e23112c8:	mov    %rdi,%r8
+   2e23112cb:	mov    %ebx,%edx
+   2e23112cd:	mov    %rsi,%rcx
+   2e23112d0:	call   0x2e2312ef0
+   2e23112d5:	mov    %rdi,%r8
+   2e23112d8:	mov    %ebx,%edx
+   2e23112da:	mov    %rsi,%rcx
+   2e23112dd:	mov    %eax,%ebp
+   2e23112df:	call   0x2e2311010
+   2e23112e4:	test   %eax,%eax
+   2e23112e6:	jne    0x2e2311220
+   2e23112ec:	xor    %ebp,%ebp
+   2e23112ee:	jmp    0x2e2311220
+   2e23112f3:	nopl   0x0(%rax,%rax,1)
+   2e23112f8:	call   0x2e2312f00
+   2e23112fd:	mov    %eax,%ebp
+   2e23112ff:	jmp    0x2e231120f
    2e2311304:	nopl   0x0(%rax)
-   2e2311308:	call   0x2e2312e00
-   2e231130d:	mov    %eax,%r14d
-   2e2311310:	cmp    $0x3,%r12d
-   2e2311314:	jne    0x2e2311264
-   2e231131a:	jmp    0x2e231123e
+   2e2311308:	cmp    $0x1,%ebx
+   2e231130b:	je     0x2e23112af
+   2e231130d:	xor    %ebp,%ebp
+   2e231130f:	jmp    0x2e2311220
+   2e2311314:	data16 cs nopw 0x0(%rax,%rax,1)
    2e231131f:	nop
-   2e2311320:	cmp    $0x1,%r12d
-   2e2311324:	jne    0x2e2311261
-   2e231132a:	jmp    0x2e23112f2
-   2e231132c:	mov    %rbx,%r8
-   2e231132f:	mov    $0x2,%edx
-   2e2311334:	mov    %r13,%rcx
-   2e2311337:	call   0x2e2312e00
-   2e231133c:	mov    %eax,%r14d
-   2e231133f:	jmp    0x2e2311264
-   2e2311344:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e2311320:	mov    0x3f49(%rip),%rax        # 0x2e2315270
+   2e2311327:	movl   $0x0,(%rax)
+   2e231132d:	jmp    0x2e23111d0
+   2e2311332:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e231133d:	nopl   (%rax)
+   2e2311340:	mov    %rcx,%rdx
+   2e2311343:	lea    0x6cb6(%rip),%rcx        # 0x2e2318000
+   2e231134a:	jmp    0x2e2313090
    2e231134f:	nop
-   2e2311350:	mov    0x3f39(%rip),%rax        # 0x2e2315290
-   2e2311357:	movl   $0x0,(%rax)
-   2e231135d:	jmp    0x2e2311200
-   2e2311362:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e231136d:	nopl   (%rax)
-   2e2311370:	mov    %rcx,%rdx
-   2e2311373:	lea    0x6c86(%rip),%rcx        # 0x2e2318000
-   2e231137a:	jmp    0x2e2312ff0
-   2e231137f:	nop
-   2e2311380:	lea    0x9(%rip),%rcx        # 0x2e2311390
-   2e2311387:	jmp    0x2e2311370
-   2e231138c:	nopl   0x0(%rax)
-   2e2311390:	ret
-   2e2311391:	nop
-   2e2311392:	nop
-   2e2311393:	nop
-   2e2311394:	nop
-   2e2311395:	nop
-   2e2311396:	nop
-   2e2311397:	nop
-   2e2311398:	nop
-   2e2311399:	nop
-   2e231139a:	nop
-   2e231139b:	nop
-   2e231139c:	nop
-   2e231139d:	nop
-   2e231139e:	nop
-   2e231139f:	nop
-   2e23113a0:	mov    $0x1,%eax
-   2e23113a5:	movsd  (%rcx),%xmm0
-   2e23113a9:	movsd  (%rdx),%xmm1
-   2e23113ad:	comisd %xmm1,%xmm0
-   2e23113b1:	ja     0x2e23113b8
-   2e23113b3:	mov    $0xffffffff,%eax
-   2e23113b8:	ret
-   2e23113b9:	nopl   0x0(%rax)
-   2e23113c0:	test   %edx,%edx
-   2e23113c2:	jle    0x2e23113f0
-   2e23113c4:	movslq %edx,%rdx
-   2e23113c7:	xor    %eax,%eax
-   2e23113c9:	pxor   %xmm0,%xmm0
-   2e23113cd:	nopl   (%rax)
-   2e23113d0:	mov    (%r8,%rax,4),%r9d
-   2e23113d4:	test   %r9d,%r9d
-   2e23113d7:	je     0x2e23113de
-   2e23113d9:	addsd  (%rcx,%rax,8),%xmm0
-   2e23113de:	add    $0x1,%rax
-   2e23113e2:	cmp    %rdx,%rax
-   2e23113e5:	jne    0x2e23113d0
-   2e23113e7:	ret
-   2e23113e8:	nopl   0x0(%rax,%rax,1)
-   2e23113f0:	pxor   %xmm0,%xmm0
-   2e23113f4:	ret
-   2e23113f5:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e2311400:	mov    %rdx,%r9
-   2e2311403:	movslq 0x28(%rsp),%rdx
-   2e2311408:	mov    %rcx,%r8
-   2e231140b:	mov    0x30(%rsp),%rcx
-   2e2311410:	test   %edx,%edx
-   2e2311412:	jle    0x2e2311458
-   2e2311414:	xor    %eax,%eax
-   2e2311416:	pxor   %xmm4,%xmm4
-   2e231141a:	nopw   0x0(%rax,%rax,1)
-   2e2311420:	mov    (%rcx,%rax,4),%r10d
-   2e2311424:	test   %r10d,%r10d
-   2e2311427:	je     0x2e2311445
-   2e2311429:	movsd  (%r8,%rax,8),%xmm0
-   2e231142f:	movsd  (%r9,%rax,8),%xmm1
-   2e2311435:	subsd  %xmm2,%xmm0
-   2e2311439:	subsd  %xmm3,%xmm1
-   2e231143d:	mulsd  %xmm1,%xmm0
-   2e2311441:	addsd  %xmm0,%xmm4
-   2e2311445:	add    $0x1,%rax
-   2e2311449:	cmp    %rax,%rdx
-   2e231144c:	jne    0x2e2311420
-   2e231144e:	movupd %xmm4,%xmm0
-   2e2311452:	ret
-   2e2311453:	nopl   0x0(%rax,%rax,1)
-   2e2311458:	pxor   %xmm4,%xmm4
-   2e231145c:	movupd %xmm4,%xmm0
-   2e2311460:	ret
-   2e2311461:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e231146c:	nopl   0x0(%rax)
-   2e2311470:	mov    0x28(%rsp),%edx
-   2e2311474:	test   %r8d,%r8d
-   2e2311477:	jle    0x2e23114e0
-   2e2311479:	pxor   %xmm3,%xmm3
-   2e231147d:	movslq %r8d,%r8
-   2e2311480:	xor    %eax,%eax
-   2e2311482:	movupd %xmm3,%xmm2
-   2e2311486:	jmp    0x2e2311499
-   2e2311488:	nopl   0x0(%rax,%rax,1)
-   2e2311490:	add    $0x1,%rax
-   2e2311494:	cmp    %rax,%r8
-   2e2311497:	je     0x2e23114bc
-   2e2311499:	mov    (%r9,%rax,4),%r10d
-   2e231149d:	test   %r10d,%r10d
-   2e23114a0:	je     0x2e2311490
-   2e23114a2:	movsd  (%rcx,%rax,8),%xmm0
-   2e23114a7:	add    $0x1,%rax
-   2e23114ab:	subsd  %xmm1,%xmm0
-   2e23114af:	mulsd  %xmm0,%xmm0
-   2e23114b3:	addsd  %xmm0,%xmm2
-   2e23114b7:	cmp    %rax,%r8
-   2e23114ba:	jne    0x2e2311499
-   2e23114bc:	pxor   %xmm0,%xmm0
-   2e23114c0:	cvtsi2sd %edx,%xmm0
-   2e23114c4:	divsd  %xmm0,%xmm2
-   2e23114c8:	ucomisd %xmm2,%xmm3
-   2e23114cc:	ja     0x2e23114ea
-   2e23114ce:	sqrtsd %xmm2,%xmm2
-   2e23114d2:	movupd %xmm2,%xmm0
-   2e23114d6:	ret
-   2e23114d7:	nopw   0x0(%rax,%rax,1)
-   2e23114e0:	pxor   %xmm3,%xmm3
-   2e23114e4:	movupd %xmm3,%xmm2
-   2e23114e8:	jmp    0x2e23114bc
-   2e23114ea:	movupd %xmm2,%xmm0
-   2e23114ee:	jmp    0x2e2312e10
-   2e23114f3:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e23114fe:	xchg   %ax,%ax
-   2e2311500:	push   %rbp
-   2e2311501:	push   %rdi
-   2e2311502:	push   %rsi
-   2e2311503:	push   %rbx
-   2e2311504:	sub    $0x28,%rsp
-   2e2311508:	movslq %r8d,%rsi
-   2e231150b:	mov    %rcx,%rbx
-   2e231150e:	mov    %rdx,%rdi
-   2e2311511:	lea    0x0(,%rsi,4),%rcx
-   2e2311519:	call   0x2e2312f78
-   2e231151e:	mov    %rax,%r9
-   2e2311521:	test   %esi,%esi
-   2e2311523:	jle    0x2e231155c
-   2e2311525:	xor    %eax,%eax
-   2e2311527:	nopw   0x0(%rax,%rax,1)
-   2e2311530:	movsd  (%rbx,%rax,8),%xmm0
-   2e2311535:	ucomisd %xmm0,%xmm0
-   2e2311539:	jp     0x2e2311570
-   2e231153b:	jne    0x2e2311570
-   2e231153d:	movsd  (%rdi,%rax,8),%xmm0
-   2e2311542:	mov    $0x1,%edx
-   2e2311547:	ucomisd %xmm0,%xmm0
-   2e231154b:	jp     0x2e2311570
-   2e231154d:	jne    0x2e2311570
-   2e231154f:	mov    %edx,(%r9,%rax,4)
-   2e2311553:	add    $0x1,%rax
-   2e2311557:	cmp    %rax,%rsi
-   2e231155a:	jne    0x2e2311530
-   2e231155c:	mov    %r9,%rax
-   2e231155f:	add    $0x28,%rsp
-   2e2311563:	pop    %rbx
-   2e2311564:	pop    %rsi
-   2e2311565:	pop    %rdi
-   2e2311566:	pop    %rbp
-   2e2311567:	ret
-   2e2311568:	nopl   0x0(%rax,%rax,1)
-   2e2311570:	xor    %edx,%edx
-   2e2311572:	mov    %edx,(%r9,%rax,4)
-   2e2311576:	add    $0x1,%rax
-   2e231157a:	cmp    %rax,%rsi
-   2e231157d:	jne    0x2e2311530
-   2e231157f:	jmp    0x2e231155c
-   2e2311581:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e231158c:	nopl   0x0(%rax)
-   2e2311590:	push   %rbp
-   2e2311591:	push   %rdi
-   2e2311592:	push   %rsi
-   2e2311593:	push   %rbx
-   2e2311594:	sub    $0x88,%rsp
-   2e231159b:	movups %xmm6,0x30(%rsp)
-   2e23115a0:	movups %xmm7,0x40(%rsp)
-   2e23115a5:	movups %xmm8,0x50(%rsp)
-   2e23115ab:	movups %xmm9,0x60(%rsp)
-   2e23115b1:	movups %xmm10,0x70(%rsp)
-   2e23115b7:	movslq %r8d,%rdi
-   2e23115ba:	mov    %rcx,%rbx
-   2e23115bd:	mov    %rdx,%rsi
-   2e23115c0:	lea    0x0(,%rdi,4),%rcx
-   2e23115c8:	mov    %rdi,%rbp
-   2e23115cb:	call   0x2e2312f78
-   2e23115d0:	mov    %rax,%rcx
-   2e23115d3:	test   %edi,%edi
-   2e23115d5:	jle    0x2e2311830
-   2e23115db:	lea    -0x1(%rdi),%r8d
-   2e23115df:	mov    %edi,%edx
-   2e23115e1:	xor    %eax,%eax
-   2e23115e3:	nopl   0x0(%rax,%rax,1)
-   2e23115e8:	movsd  (%rbx,%rax,8),%xmm0
-   2e23115ed:	ucomisd %xmm0,%xmm0
-   2e23115f1:	jp     0x2e2311610
-   2e23115f3:	jne    0x2e2311610
-   2e23115f5:	movsd  (%rsi,%rax,8),%xmm0
-   2e23115fa:	mov    $0x1,%r9d
-   2e2311600:	ucomisd %xmm0,%xmm0
-   2e2311604:	jp     0x2e2311610
-   2e2311606:	je     0x2e2311613
-   2e2311608:	nopl   0x0(%rax,%rax,1)
-   2e2311610:	xor    %r9d,%r9d
-   2e2311613:	mov    %r9d,(%rcx,%rax,4)
-   2e2311617:	add    $0x1,%rax
-   2e231161b:	cmp    %rdx,%rax
-   2e231161e:	jne    0x2e23115e8
-   2e2311620:	cmp    $0x3,%r8d
-   2e2311624:	jbe    0x2e2311862
-   2e231162a:	mov    %ebp,%r8d
-   2e231162d:	mov    %rcx,%rax
-   2e2311630:	pxor   %xmm0,%xmm0
-   2e2311634:	shr    $0x2,%r8d
-   2e2311638:	shl    $0x4,%r8
-   2e231163c:	add    %rcx,%r8
-   2e231163f:	nop
-   2e2311640:	movdqu (%rax),%xmm3
-   2e2311644:	add    $0x10,%rax
-   2e2311648:	paddd  %xmm3,%xmm0
-   2e231164c:	cmp    %r8,%rax
-   2e231164f:	jne    0x2e2311640
-   2e2311651:	movdqu %xmm0,%xmm1
-   2e2311655:	mov    %ebp,%eax
-   2e2311657:	psrldq $0x8,%xmm1
-   2e231165c:	and    $0xfffffffc,%eax
-   2e231165f:	paddd  %xmm1,%xmm0
-   2e2311663:	movdqu %xmm0,%xmm1
-   2e2311667:	psrldq $0x4,%xmm1
-   2e231166c:	paddd  %xmm1,%xmm0
-   2e2311670:	movd   %xmm0,%r8d
-   2e2311675:	test   $0x3,%bpl
-   2e2311679:	je     0x2e23116af
-   2e231167b:	movslq %eax,%r9
-   2e231167e:	add    (%rcx,%r9,4),%r8d
-   2e2311682:	lea    0x1(%rax),%r9d
-   2e2311686:	cmp    %r9d,%ebp
-   2e2311689:	jle    0x2e23116af
-   2e231168b:	movslq %r9d,%r9
-   2e231168e:	add    (%rcx,%r9,4),%r8d
-   2e2311692:	lea    0x2(%rax),%r9d
-   2e2311696:	cmp    %r9d,%ebp
-   2e2311699:	jle    0x2e23116af
-   2e231169b:	movslq %r9d,%r9
-   2e231169e:	add    $0x3,%eax
-   2e23116a1:	add    (%rcx,%r9,4),%r8d
-   2e23116a5:	cmp    %eax,%ebp
-   2e23116a7:	jle    0x2e23116af
-   2e23116a9:	cltq
-   2e23116ab:	add    (%rcx,%rax,4),%r8d
-   2e23116af:	pxor   %xmm8,%xmm8
-   2e23116b4:	xor    %eax,%eax
-   2e23116b6:	movupd %xmm8,%xmm1
-   2e23116bb:	nopl   0x0(%rax,%rax,1)
-   2e23116c0:	mov    (%rcx,%rax,4),%r11d
-   2e23116c4:	test   %r11d,%r11d
-   2e23116c7:	je     0x2e23116ce
-   2e23116c9:	addsd  (%rbx,%rax,8),%xmm1
-   2e23116ce:	add    $0x1,%rax
-   2e23116d2:	cmp    %rdx,%rax
-   2e23116d5:	jne    0x2e23116c0
-   2e23116d7:	pxor   %xmm9,%xmm9
-   2e23116dc:	xor    %eax,%eax
-   2e23116de:	movupd %xmm8,%xmm6
-   2e23116e3:	cvtsi2sd %r8d,%xmm9
-   2e23116e8:	divsd  %xmm9,%xmm1
-   2e23116ed:	nopl   (%rax)
-   2e23116f0:	mov    (%rcx,%rax,4),%r10d
-   2e23116f4:	test   %r10d,%r10d
-   2e23116f7:	je     0x2e23116fe
-   2e23116f9:	addsd  (%rsi,%rax,8),%xmm6
-   2e23116fe:	add    $0x1,%rax
-   2e2311702:	cmp    %rdx,%rax
-   2e2311705:	jne    0x2e23116f0
-   2e2311707:	xor    %eax,%eax
-   2e2311709:	movupd %xmm8,%xmm7
-   2e231170e:	divsd  %xmm9,%xmm6
-   2e2311713:	nopl   0x0(%rax,%rax,1)
-   2e2311718:	mov    (%rcx,%rax,4),%r9d
-   2e231171c:	test   %r9d,%r9d
-   2e231171f:	je     0x2e231173b
-   2e2311721:	movsd  (%rbx,%rax,8),%xmm0
-   2e2311726:	movsd  (%rsi,%rax,8),%xmm2
-   2e231172b:	subsd  %xmm1,%xmm0
-   2e231172f:	subsd  %xmm6,%xmm2
-   2e2311733:	mulsd  %xmm2,%xmm0
-   2e2311737:	addsd  %xmm0,%xmm7
-   2e231173b:	add    $0x1,%rax
-   2e231173f:	cmp    %rdx,%rax
-   2e2311742:	jne    0x2e2311718
-   2e2311744:	xor    %eax,%eax
-   2e2311746:	movupd %xmm8,%xmm10
-   2e231174b:	divsd  %xmm9,%xmm7
-   2e2311750:	jmp    0x2e2311761
-   2e2311752:	nopw   0x0(%rax,%rax,1)
-   2e2311758:	add    $0x1,%rax
-   2e231175c:	cmp    %rdx,%rax
-   2e231175f:	je     0x2e2311785
-   2e2311761:	mov    (%rcx,%rax,4),%r8d
-   2e2311765:	test   %r8d,%r8d
-   2e2311768:	je     0x2e2311758
-   2e231176a:	movsd  (%rbx,%rax,8),%xmm0
-   2e231176f:	add    $0x1,%rax
-   2e2311773:	subsd  %xmm1,%xmm0
-   2e2311777:	mulsd  %xmm0,%xmm0
-   2e231177b:	addsd  %xmm0,%xmm10
-   2e2311780:	cmp    %rdx,%rax
-   2e2311783:	jne    0x2e2311761
-   2e2311785:	divsd  %xmm9,%xmm10
-   2e231178a:	ucomisd %xmm10,%xmm8
-   2e231178f:	ja     0x2e2311888
-   2e2311795:	sqrtsd %xmm10,%xmm10
-   2e231179a:	test   %ebp,%ebp
-   2e231179c:	jle    0x2e2311858
-   2e23117a2:	xor    %eax,%eax
-   2e23117a4:	movupd %xmm8,%xmm1
-   2e23117a9:	jmp    0x2e23117b9
-   2e23117ab:	nopl   0x0(%rax,%rax,1)
-   2e23117b0:	add    $0x1,%rax
-   2e23117b4:	cmp    %rdi,%rax
-   2e23117b7:	je     0x2e23117da
-   2e23117b9:	mov    (%rcx,%rax,4),%edx
-   2e23117bc:	test   %edx,%edx
-   2e23117be:	je     0x2e23117b0
-   2e23117c0:	movsd  (%rsi,%rax,8),%xmm0
-   2e23117c5:	add    $0x1,%rax
-   2e23117c9:	subsd  %xmm6,%xmm0
-   2e23117cd:	mulsd  %xmm0,%xmm0
-   2e23117d1:	addsd  %xmm0,%xmm1
-   2e23117d5:	cmp    %rdi,%rax
-   2e23117d8:	jne    0x2e23117b9
-   2e23117da:	divsd  %xmm9,%xmm1
-   2e23117df:	ucomisd %xmm1,%xmm8
-   2e23117e4:	ja     0x2e231186c
-   2e23117ea:	movupd %xmm1,%xmm6
-   2e23117ee:	sqrtsd %xmm6,%xmm6
-   2e23117f2:	call   0x2e2312f88
-   2e23117f7:	mulsd  %xmm10,%xmm6
-   2e23117fc:	movups 0x50(%rsp),%xmm8
-   2e2311802:	movups 0x60(%rsp),%xmm9
-   2e2311808:	movups 0x70(%rsp),%xmm10
-   2e231180e:	divsd  %xmm6,%xmm7
-   2e2311812:	movups 0x30(%rsp),%xmm6
-   2e2311817:	movupd %xmm7,%xmm0
-   2e231181b:	movups 0x40(%rsp),%xmm7
-   2e2311820:	add    $0x88,%rsp
-   2e2311827:	pop    %rbx
-   2e2311828:	pop    %rsi
-   2e2311829:	pop    %rdi
-   2e231182a:	pop    %rbp
-   2e231182b:	ret
-   2e231182c:	nopl   0x0(%rax)
-   2e2311830:	pxor   %xmm8,%xmm8
-   2e2311835:	movupd %xmm8,%xmm6
-   2e231183a:	movupd %xmm8,%xmm9
-   2e231183f:	divsd  %xmm8,%xmm6
-   2e2311844:	movupd %xmm6,%xmm10
-   2e2311849:	movupd %xmm6,%xmm7
-   2e231184d:	jmp    0x2e231178a
-   2e2311852:	nopw   0x0(%rax,%rax,1)
-   2e2311858:	movupd %xmm8,%xmm1
-   2e231185d:	jmp    0x2e23117da
-   2e2311862:	xor    %eax,%eax
-   2e2311864:	xor    %r8d,%r8d
-   2e2311867:	jmp    0x2e231167b
-   2e231186c:	movupd %xmm1,%xmm0
-   2e2311870:	mov    %rcx,0x28(%rsp)
-   2e2311875:	call   0x2e2312e10
-   2e231187a:	mov    0x28(%rsp),%rcx
-   2e231187f:	movupd %xmm0,%xmm6
-   2e2311883:	jmp    0x2e23117f2
-   2e2311888:	movupd %xmm10,%xmm0
-   2e231188d:	mov    %rcx,0x28(%rsp)
-   2e2311892:	call   0x2e2312e10
-   2e2311897:	mov    0x28(%rsp),%rcx
-   2e231189c:	movupd %xmm0,%xmm10
-   2e23118a1:	jmp    0x2e231179a
-   2e23118a6:	cs nopw 0x0(%rax,%rax,1)
-   2e23118b0:	jmp    0x2e2312f88
-   2e23118b5:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e23118c0:	push   %r15
-   2e23118c2:	push   %r14
-   2e23118c4:	push   %r13
-   2e23118c6:	push   %r12
-   2e23118c8:	push   %rbp
-   2e23118c9:	push   %rdi
-   2e23118ca:	push   %rsi
-   2e23118cb:	push   %rbx
-   2e23118cc:	sub    $0x68,%rsp
-   2e23118d0:	movups %xmm6,0x50(%rsp)
-   2e23118d5:	movslq %r8d,%rdi
-   2e23118d8:	mov    %rcx,%rsi
-   2e23118db:	mov    %rdx,%rbx
-   2e23118de:	mov    %r9d,%ebp
-   2e23118e1:	mov    %rdi,%r12
-   2e23118e4:	mov    %r8d,0xc0(%rsp)
-   2e23118ec:	shl    $0x4,%r12
-   2e23118f0:	mov    %r12,%rcx
-   2e23118f3:	call   0x2e2312f78
-   2e23118f8:	mov    %r12,%rcx
-   2e23118fb:	mov    %rax,%r14
-   2e23118fe:	call   0x2e2312f78
-   2e2311903:	lea    0x0(,%rdi,4),%rcx
-   2e231190b:	mov    %rax,%r13
-   2e231190e:	call   0x2e2312f78
-   2e2311913:	lea    0x0(,%rdi,8),%r8
-   2e231191b:	mov    %r8,%rcx
-   2e231191e:	mov    %r8,0x28(%rsp)
-   2e2311923:	mov    %rax,%r12
-   2e2311926:	call   0x2e2312f78
-   2e231192b:	mov    0x28(%rsp),%r8
-   2e2311930:	mov    %rax,0x20(%rsp)
-   2e2311935:	mov    %r8,%rcx
-   2e2311938:	call   0x2e2312f78
-   2e231193d:	mov    0xc0(%rsp),%r8d
-   2e2311945:	mov    %rax,%r15
-   2e2311948:	test   %r8d,%r8d
-   2e231194b:	jle    0x2e2311f6a
-   2e2311951:	mov    0x28(%rsp),%r8
-   2e2311956:	mov    0x20(%rsp),%rcx
-   2e231195b:	mov    %rsi,%rdx
-   2e231195e:	call   0x2e2312f70
-   2e2311963:	mov    0x28(%rsp),%r8
-   2e2311968:	mov    %r15,%rcx
-   2e231196b:	mov    %rbx,%rdx
-   2e231196e:	call   0x2e2312f70
-   2e2311973:	mov    %r12,0x28(%rsp)
-   2e2311978:	xor    %eax,%eax
-   2e231197a:	xor    %r10d,%r10d
-   2e231197d:	movsd  0x367b(%rip),%xmm1        # 0x2e2315000
-   2e2311985:	mov    0xc0(%rsp),%r12d
-   2e231198d:	mov    $0xffffffff,%r9d
-   2e2311993:	xor    %ecx,%ecx
-   2e2311995:	mov    $0xffffffff,%r8d
-   2e231199b:	nopl   0x0(%rax,%rax,1)
-   2e23119a0:	movsd  (%rsi,%rax,8),%xmm0
-   2e23119a5:	mov    %eax,%r11d
-   2e23119a8:	ucomisd %xmm0,%xmm0
-   2e23119ac:	jp     0x2e2311bce
-   2e23119b2:	movslq %ecx,%rdx
-   2e23119b5:	add    $0x1,%ecx
-   2e23119b8:	shl    $0x4,%rdx
-   2e23119bc:	add    %r14,%rdx
-   2e23119bf:	mov    %eax,0x8(%rdx)
-   2e23119c2:	movq   %xmm0,(%rdx)
-   2e23119c6:	movsd  (%rbx,%rax,8),%xmm0
-   2e23119cb:	ucomisd %xmm0,%xmm0
-   2e23119cf:	jp     0x2e2311baf
-   2e23119d5:	movslq %r10d,%rdx
-   2e23119d8:	add    $0x1,%r10d
-   2e23119dc:	shl    $0x4,%rdx
-   2e23119e0:	add    %r13,%rdx
-   2e23119e3:	mov    %r11d,0x8(%rdx)
-   2e23119e7:	movq   %xmm0,(%rdx)
-   2e23119eb:	add    $0x1,%rax
-   2e23119ef:	cmp    %rax,%rdi
-   2e23119f2:	jne    0x2e23119a0
-   2e23119f4:	mov    %r10d,%edi
-   2e23119f7:	movslq %ecx,%rdx
-   2e23119fa:	mov    0x28(%rsp),%r12
-   2e23119ff:	lea    -0x666(%rip),%r9        # 0x2e23113a0
-   2e2311a06:	mov    %ecx,0x28(%rsp)
-   2e2311a0a:	mov    $0x10,%r8d
-   2e2311a10:	mov    %r14,%rcx
-   2e2311a13:	call   0x2e2312f68
-   2e2311a18:	movslq %edi,%rdx
-   2e2311a1b:	lea    -0x682(%rip),%r9        # 0x2e23113a0
-   2e2311a22:	mov    %r13,%rcx
-   2e2311a25:	mov    $0x10,%r8d
-   2e2311a2b:	call   0x2e2312f68
-   2e2311a30:	mov    0x28(%rsp),%eax
-   2e2311a34:	mov    %edi,0x40(%rsp)
-   2e2311a38:	cmp    %edi,%eax
-   2e2311a3a:	cmovle %eax,%edi
-   2e2311a3d:	movslq %edi,%rcx
-   2e2311a40:	shl    $0x2,%rcx
-   2e2311a44:	mov    %rcx,0x30(%rsp)
-   2e2311a49:	call   0x2e2312f78
-   2e2311a4e:	mov    0x30(%rsp),%rcx
-   2e2311a53:	mov    %rax,0x38(%rsp)
-   2e2311a58:	call   0x2e2312f78
-   2e2311a5d:	mov    %rax,0x30(%rsp)
-   2e2311a62:	test   %ebp,%ebp
-   2e2311a64:	jne    0x2e2311bf0
-   2e2311a6a:	mov    0x40(%rsp),%ecx
-   2e2311a6e:	test   %edi,%edi
-   2e2311a70:	setg   %al
-   2e2311a73:	test   %ecx,%ecx
-   2e2311a75:	mov    0x28(%rsp),%ecx
-   2e2311a79:	setg   %r9b
-   2e2311a7d:	and    %eax,%r9d
-   2e2311a80:	test   %ecx,%ecx
-   2e2311a82:	jle    0x2e2311fd5
-   2e2311a88:	test   %al,%al
-   2e2311a8a:	je     0x2e2311fd5
-   2e2311a90:	lea    -0x1(%rcx),%eax
-   2e2311a93:	mov    0x38(%rsp),%r10
-   2e2311a98:	xor    %edx,%edx
-   2e2311a9a:	cltq
-   2e2311a9c:	nopl   0x0(%rax)
-   2e2311aa0:	mov    %rax,%rcx
-   2e2311aa3:	shl    $0x4,%rcx
-   2e2311aa7:	movslq 0x8(%r14,%rcx,1),%r8
-   2e2311aac:	movsd  (%rbx,%r8,8),%xmm0
-   2e2311ab2:	mov    %r8,%rcx
-   2e2311ab5:	ucomisd %xmm0,%xmm0
-   2e2311ab9:	jnp    0x2e2311ac5
-   2e2311abb:	movslq %edx,%r8
-   2e2311abe:	add    $0x1,%edx
-   2e2311ac1:	mov    %ecx,(%r10,%r8,4)
-   2e2311ac5:	test   %eax,%eax
-   2e2311ac7:	setg   %r8b
-   2e2311acb:	cmp    %edi,%edx
-   2e2311acd:	setl   %cl
-   2e2311ad0:	sub    $0x1,%rax
-   2e2311ad4:	test   %cl,%r8b
-   2e2311ad7:	jne    0x2e2311aa0
-   2e2311ad9:	mov    0x40(%rsp),%eax
-   2e2311add:	sub    $0x1,%eax
-   2e2311ae0:	cltq
-   2e2311ae2:	test   %r9b,%r9b
-   2e2311ae5:	je     0x2e2311fc2
-   2e2311aeb:	mov    0x30(%rsp),%r9
-   2e2311af0:	mov    %rax,%rcx
-   2e2311af3:	shl    $0x4,%rcx
-   2e2311af7:	movslq 0x8(%r13,%rcx,1),%r8
-   2e2311afc:	movsd  (%rsi,%r8,8),%xmm0
-   2e2311b02:	mov    %r8,%rcx
-   2e2311b05:	ucomisd %xmm0,%xmm0
-   2e2311b09:	jnp    0x2e2311b15
-   2e2311b0b:	movslq %ebp,%r8
-   2e2311b0e:	add    $0x1,%ebp
-   2e2311b11:	mov    %ecx,(%r9,%r8,4)
-   2e2311b15:	test   %eax,%eax
-   2e2311b17:	setg   %r8b
-   2e2311b1b:	cmp    %edi,%ebp
-   2e2311b1d:	setl   %cl
-   2e2311b20:	sub    $0x1,%rax
-   2e2311b24:	test   %cl,%r8b
-   2e2311b27:	jne    0x2e2311af0
-   2e2311b29:	test   %ebp,%ebp
-   2e2311b2b:	je     0x2e2311fc2
-   2e2311b31:	mov    0x20(%rsp),%r10
-   2e2311b36:	mov    0x30(%rsp),%r11
-   2e2311b3b:	movslq %ebp,%rax
-   2e2311b3e:	lea    0x1(%rbp),%r9d
-   2e2311b42:	nopw   0x0(%rax,%rax,1)
-   2e2311b48:	mov    %r9d,%r8d
-   2e2311b4b:	pxor   %xmm0,%xmm0
-   2e2311b4f:	movslq -0x4(%r11,%rax,4),%rcx
-   2e2311b54:	sub    %eax,%r8d
-   2e2311b57:	sub    $0x1,%rax
-   2e2311b5b:	cvtsi2sd %r8d,%xmm0
-   2e2311b60:	movsd  %xmm0,(%r10,%rcx,8)
-   2e2311b66:	test   %eax,%eax
-   2e2311b68:	jne    0x2e2311b48
-   2e2311b6a:	mov    %r9d,%r11d
-   2e2311b6d:	test   %edx,%edx
-   2e2311b6f:	je     0x2e2311fb5
-   2e2311b75:	mov    0x38(%rsp),%r9
-   2e2311b7a:	movslq %edx,%rax
-   2e2311b7d:	lea    0x1(%rdx),%r8d
+   2e2311350:	lea    0x9(%rip),%rcx        # 0x2e2311360
+   2e2311357:	jmp    0x2e2311340
+   2e231135c:	nopl   0x0(%rax)
+   2e2311360:	ret
+   2e2311361:	nop
+   2e2311362:	nop
+   2e2311363:	nop
+   2e2311364:	nop
+   2e2311365:	nop
+   2e2311366:	nop
+   2e2311367:	nop
+   2e2311368:	nop
+   2e2311369:	nop
+   2e231136a:	nop
+   2e231136b:	nop
+   2e231136c:	nop
+   2e231136d:	nop
+   2e231136e:	nop
+   2e231136f:	nop
+   2e2311370:	mov    $0x1,%eax
+   2e2311375:	movsd  (%rcx),%xmm0
+   2e2311379:	movsd  (%rdx),%xmm1
+   2e231137d:	comisd %xmm1,%xmm0
+   2e2311381:	ja     0x2e2311388
+   2e2311383:	mov    $0xffffffff,%eax
+   2e2311388:	ret
+   2e2311389:	nopl   0x0(%rax)
+   2e2311390:	test   %edx,%edx
+   2e2311392:	jle    0x2e23113c0
+   2e2311394:	movslq %edx,%rdx
+   2e2311397:	xor    %eax,%eax
+   2e2311399:	pxor   %xmm0,%xmm0
+   2e231139d:	nopl   (%rax)
+   2e23113a0:	mov    (%r8,%rax,4),%r9d
+   2e23113a4:	test   %r9d,%r9d
+   2e23113a7:	je     0x2e23113ae
+   2e23113a9:	addsd  (%rcx,%rax,8),%xmm0
+   2e23113ae:	add    $0x1,%rax
+   2e23113b2:	cmp    %rax,%rdx
+   2e23113b5:	jne    0x2e23113a0
+   2e23113b7:	ret
+   2e23113b8:	nopl   0x0(%rax,%rax,1)
+   2e23113c0:	pxor   %xmm0,%xmm0
+   2e23113c4:	ret
+   2e23113c5:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e23113d0:	movslq 0x28(%rsp),%r8
+   2e23113d5:	mov    0x30(%rsp),%r9
+   2e23113da:	test   %r8d,%r8d
+   2e23113dd:	jle    0x2e2311420
+   2e23113df:	xor    %eax,%eax
+   2e23113e1:	pxor   %xmm4,%xmm4
+   2e23113e5:	nopl   (%rax)
+   2e23113e8:	mov    (%r9,%rax,4),%r10d
+   2e23113ec:	test   %r10d,%r10d
+   2e23113ef:	je     0x2e231140b
+   2e23113f1:	movsd  (%rcx,%rax,8),%xmm0
+   2e23113f6:	movsd  (%rdx,%rax,8),%xmm1
+   2e23113fb:	subsd  %xmm2,%xmm0
+   2e23113ff:	subsd  %xmm3,%xmm1
+   2e2311403:	mulsd  %xmm1,%xmm0
+   2e2311407:	addsd  %xmm0,%xmm4
+   2e231140b:	add    $0x1,%rax
+   2e231140f:	cmp    %rax,%r8
+   2e2311412:	jne    0x2e23113e8
+   2e2311414:	movupd %xmm4,%xmm0
+   2e2311418:	ret
+   2e2311419:	nopl   0x0(%rax)
+   2e2311420:	pxor   %xmm4,%xmm4
+   2e2311424:	movupd %xmm4,%xmm0
+   2e2311428:	ret
+   2e2311429:	nopl   0x0(%rax)
+   2e2311430:	mov    0x28(%rsp),%edx
+   2e2311434:	test   %r8d,%r8d
+   2e2311437:	jle    0x2e2311490
+   2e2311439:	movslq %r8d,%r8
+   2e231143c:	xor    %eax,%eax
+   2e231143e:	pxor   %xmm0,%xmm0
+   2e2311442:	jmp    0x2e2311451
+   2e2311444:	nopl   0x0(%rax)
+   2e2311448:	add    $0x1,%rax
+   2e231144c:	cmp    %rax,%r8
+   2e231144f:	je     0x2e2311474
+   2e2311451:	mov    (%r9,%rax,4),%r10d
+   2e2311455:	test   %r10d,%r10d
+   2e2311458:	je     0x2e2311448
+   2e231145a:	movsd  (%rcx,%rax,8),%xmm2
+   2e231145f:	add    $0x1,%rax
+   2e2311463:	subsd  %xmm1,%xmm2
+   2e2311467:	mulsd  %xmm2,%xmm2
+   2e231146b:	addsd  %xmm2,%xmm0
+   2e231146f:	cmp    %rax,%r8
+   2e2311472:	jne    0x2e2311451
+   2e2311474:	pxor   %xmm1,%xmm1
+   2e2311478:	cvtsi2sd %edx,%xmm1
+   2e231147c:	divsd  %xmm1,%xmm0
+   2e2311480:	pxor   %xmm1,%xmm1
+   2e2311484:	ucomisd %xmm0,%xmm1
+   2e2311488:	ja     0x2e2311496
+   2e231148a:	sqrtsd %xmm0,%xmm0
+   2e231148e:	ret
+   2e231148f:	nop
+   2e2311490:	pxor   %xmm0,%xmm0
+   2e2311494:	jmp    0x2e2311474
+   2e2311496:	jmp    0x2e2312f10
+   2e231149b:	nopl   0x0(%rax,%rax,1)
+   2e23114a0:	push   %rbp
+   2e23114a1:	push   %rdi
+   2e23114a2:	push   %rsi
+   2e23114a3:	push   %rbx
+   2e23114a4:	sub    $0x28,%rsp
+   2e23114a8:	movslq %r8d,%rsi
+   2e23114ab:	mov    %rcx,%rbx
+   2e23114ae:	mov    %rdx,%rdi
+   2e23114b1:	lea    0x0(,%rsi,4),%rcx
+   2e23114b9:	call   0x2e2313220
+   2e23114be:	test   %esi,%esi
+   2e23114c0:	jle    0x2e23114f0
+   2e23114c2:	xor    %ecx,%ecx
+   2e23114c4:	nopl   0x0(%rax)
+   2e23114c8:	movsd  (%rbx,%rcx,8),%xmm0
+   2e23114cd:	ucomisd %xmm0,%xmm0
+   2e23114d1:	jp     0x2e2311500
+   2e23114d3:	movsd  (%rdi,%rcx,8),%xmm0
+   2e23114d8:	xor    %r8d,%r8d
+   2e23114db:	ucomisd %xmm0,%xmm0
+   2e23114df:	setnp  %r8b
+   2e23114e3:	mov    %r8d,(%rax,%rcx,4)
+   2e23114e7:	add    $0x1,%rcx
+   2e23114eb:	cmp    %rcx,%rsi
+   2e23114ee:	jne    0x2e23114c8
+   2e23114f0:	add    $0x28,%rsp
+   2e23114f4:	pop    %rbx
+   2e23114f5:	pop    %rsi
+   2e23114f6:	pop    %rdi
+   2e23114f7:	pop    %rbp
+   2e23114f8:	ret
+   2e23114f9:	nopl   0x0(%rax)
+   2e2311500:	movl   $0x0,(%rax,%rcx,4)
+   2e2311507:	add    $0x1,%rcx
+   2e231150b:	cmp    %rcx,%rsi
+   2e231150e:	jne    0x2e23114c8
+   2e2311510:	add    $0x28,%rsp
+   2e2311514:	pop    %rbx
+   2e2311515:	pop    %rsi
+   2e2311516:	pop    %rdi
+   2e2311517:	pop    %rbp
+   2e2311518:	ret
+   2e2311519:	nopl   0x0(%rax)
+   2e2311520:	push   %rbp
+   2e2311521:	push   %rdi
+   2e2311522:	push   %rsi
+   2e2311523:	push   %rbx
+   2e2311524:	sub    $0x78,%rsp
+   2e2311528:	movups %xmm6,0x30(%rsp)
+   2e231152d:	movups %xmm7,0x40(%rsp)
+   2e2311532:	movups %xmm8,0x50(%rsp)
+   2e2311538:	movups %xmm9,0x60(%rsp)
+   2e231153e:	movslq %r8d,%rbx
+   2e2311541:	mov    %rcx,%rsi
+   2e2311544:	mov    %rdx,%rdi
+   2e2311547:	lea    0x0(,%rbx,4),%rcx
+   2e231154f:	mov    %rbx,%rbp
+   2e2311552:	call   0x2e2313220
+   2e2311557:	mov    %rax,%rcx
+   2e231155a:	test   %ebx,%ebx
+   2e231155c:	jle    0x2e23117b0
+   2e2311562:	xor    %eax,%eax
+   2e2311564:	nopl   0x0(%rax)
+   2e2311568:	movsd  (%rsi,%rax,8),%xmm0
+   2e231156d:	ucomisd %xmm0,%xmm0
+   2e2311571:	jp     0x2e2311790
+   2e2311577:	movsd  (%rdi,%rax,8),%xmm0
+   2e231157c:	xor    %edx,%edx
+   2e231157e:	ucomisd %xmm0,%xmm0
+   2e2311582:	setnp  %dl
+   2e2311585:	mov    %edx,(%rcx,%rax,4)
+   2e2311588:	add    $0x1,%rax
+   2e231158c:	cmp    %rax,%rbx
+   2e231158f:	jne    0x2e2311568
+   2e2311591:	lea    -0x1(%rbp),%eax
+   2e2311594:	cmp    $0x2,%eax
+   2e2311597:	jbe    0x2e23117d6
+   2e231159d:	mov    %ebp,%edx
+   2e231159f:	mov    %rcx,%rax
+   2e23115a2:	pxor   %xmm0,%xmm0
+   2e23115a6:	shr    $0x2,%edx
+   2e23115a9:	shl    $0x4,%rdx
+   2e23115ad:	add    %rcx,%rdx
+   2e23115b0:	movdqu (%rax),%xmm3
+   2e23115b4:	add    $0x10,%rax
+   2e23115b8:	paddd  %xmm3,%xmm0
+   2e23115bc:	cmp    %rax,%rdx
+   2e23115bf:	jne    0x2e23115b0
+   2e23115c1:	movdqu %xmm0,%xmm1
+   2e23115c5:	psrldq $0x8,%xmm1
+   2e23115ca:	paddd  %xmm1,%xmm0
+   2e23115ce:	movdqu %xmm0,%xmm1
+   2e23115d2:	psrldq $0x4,%xmm1
+   2e23115d7:	paddd  %xmm1,%xmm0
+   2e23115db:	movd   %xmm0,%r9d
+   2e23115e0:	test   $0x3,%bpl
+   2e23115e4:	je     0x2e2311612
+   2e23115e6:	mov    %ebp,%eax
+   2e23115e8:	and    $0xfffffffc,%eax
+   2e23115eb:	movslq %eax,%rdx
+   2e23115ee:	lea    0x0(,%rdx,4),%r8
+   2e23115f6:	add    (%rcx,%rdx,4),%r9d
+   2e23115fa:	lea    0x1(%rax),%edx
+   2e23115fd:	cmp    %edx,%ebp
+   2e23115ff:	jle    0x2e2311612
+   2e2311601:	add    $0x2,%eax
+   2e2311604:	add    0x4(%rcx,%r8,1),%r9d
+   2e2311609:	cmp    %eax,%ebp
+   2e231160b:	jle    0x2e2311612
+   2e231160d:	add    0x8(%rcx,%r8,1),%r9d
+   2e2311612:	xor    %eax,%eax
+   2e2311614:	pxor   %xmm0,%xmm0
+   2e2311618:	jmp    0x2e2311623
+   2e231161a:	nopw   0x0(%rax,%rax,1)
+   2e2311620:	mov    %rdx,%rax
+   2e2311623:	mov    (%rcx,%rax,4),%r11d
+   2e2311627:	test   %r11d,%r11d
+   2e231162a:	je     0x2e2311631
+   2e231162c:	addsd  (%rsi,%rax,8),%xmm0
+   2e2311631:	lea    0x1(%rax),%rdx
+   2e2311635:	cmp    %rdx,%rbx
+   2e2311638:	jne    0x2e2311620
+   2e231163a:	pxor   %xmm7,%xmm7
+   2e231163e:	xor    %edx,%edx
+   2e2311640:	pxor   %xmm6,%xmm6
+   2e2311644:	cvtsi2sd %r9d,%xmm7
+   2e2311649:	divsd  %xmm7,%xmm0
+   2e231164d:	jmp    0x2e2311653
+   2e231164f:	nop
+   2e2311650:	mov    %r8,%rdx
+   2e2311653:	mov    (%rcx,%rdx,4),%r10d
+   2e2311657:	test   %r10d,%r10d
+   2e231165a:	je     0x2e2311661
+   2e231165c:	addsd  (%rdi,%rdx,8),%xmm6
+   2e2311661:	lea    0x1(%rdx),%r8
+   2e2311665:	cmp    %rdx,%rax
+   2e2311668:	jne    0x2e2311650
+   2e231166a:	divsd  %xmm7,%xmm6
+   2e231166e:	xor    %edx,%edx
+   2e2311670:	pxor   %xmm8,%xmm8
+   2e2311675:	jmp    0x2e2311683
+   2e2311677:	nopw   0x0(%rax,%rax,1)
+   2e2311680:	mov    %r8,%rdx
+   2e2311683:	mov    (%rcx,%rdx,4),%r9d
+   2e2311687:	test   %r9d,%r9d
+   2e231168a:	je     0x2e23116a7
+   2e231168c:	movsd  (%rsi,%rdx,8),%xmm1
+   2e2311691:	movsd  (%rdi,%rdx,8),%xmm2
+   2e2311696:	subsd  %xmm0,%xmm1
+   2e231169a:	subsd  %xmm6,%xmm2
+   2e231169e:	mulsd  %xmm2,%xmm1
+   2e23116a2:	addsd  %xmm1,%xmm8
+   2e23116a7:	lea    0x1(%rdx),%r8
+   2e23116ab:	cmp    %rax,%rdx
+   2e23116ae:	jne    0x2e2311680
+   2e23116b0:	divsd  %xmm7,%xmm8
+   2e23116b5:	xor    %edx,%edx
+   2e23116b7:	pxor   %xmm9,%xmm9
+   2e23116bc:	jmp    0x2e23116cc
+   2e23116be:	xchg   %ax,%ax
+   2e23116c0:	lea    0x1(%rdx),%r8
+   2e23116c4:	cmp    %rdx,%rax
+   2e23116c7:	je     0x2e23116f0
+   2e23116c9:	mov    %r8,%rdx
+   2e23116cc:	mov    (%rcx,%rdx,4),%r8d
+   2e23116d0:	test   %r8d,%r8d
+   2e23116d3:	je     0x2e23116c0
+   2e23116d5:	movsd  (%rsi,%rdx,8),%xmm1
+   2e23116da:	lea    0x1(%rdx),%r8
+   2e23116de:	subsd  %xmm0,%xmm1
+   2e23116e2:	mulsd  %xmm1,%xmm1
+   2e23116e6:	addsd  %xmm1,%xmm9
+   2e23116eb:	cmp    %rdx,%rax
+   2e23116ee:	jne    0x2e23116c9
+   2e23116f0:	divsd  %xmm7,%xmm9
+   2e23116f5:	pxor   %xmm0,%xmm0
+   2e23116f9:	ucomisd %xmm9,%xmm0
+   2e23116fe:	ja     0x2e231181e
+   2e2311704:	sqrtsd %xmm9,%xmm9
+   2e2311709:	xor    %eax,%eax
+   2e231170b:	pxor   %xmm0,%xmm0
+   2e231170f:	jmp    0x2e2311721
+   2e2311711:	nopl   0x0(%rax)
+   2e2311718:	add    $0x1,%rax
+   2e231171c:	cmp    %rax,%rbx
+   2e231171f:	je     0x2e2311742
+   2e2311721:	mov    (%rcx,%rax,4),%edx
+   2e2311724:	test   %edx,%edx
+   2e2311726:	je     0x2e2311718
+   2e2311728:	movsd  (%rdi,%rax,8),%xmm1
+   2e231172d:	add    $0x1,%rax
+   2e2311731:	subsd  %xmm6,%xmm1
+   2e2311735:	mulsd  %xmm1,%xmm1
+   2e2311739:	addsd  %xmm1,%xmm0
+   2e231173d:	cmp    %rax,%rbx
+   2e2311740:	jne    0x2e2311721
+   2e2311742:	divsd  %xmm7,%xmm0
+   2e2311746:	pxor   %xmm1,%xmm1
+   2e231174a:	ucomisd %xmm0,%xmm1
+   2e231174e:	ja     0x2e23117e0
+   2e2311754:	movupd %xmm0,%xmm6
+   2e2311758:	sqrtsd %xmm6,%xmm6
+   2e231175c:	call   0x2e2313210
+   2e2311761:	mulsd  %xmm9,%xmm6
+   2e2311766:	movupd %xmm8,%xmm0
+   2e231176b:	movups 0x40(%rsp),%xmm7
+   2e2311770:	movups 0x50(%rsp),%xmm8
+   2e2311776:	movups 0x60(%rsp),%xmm9
+   2e231177c:	divsd  %xmm6,%xmm0
+   2e2311780:	movups 0x30(%rsp),%xmm6
+   2e2311785:	add    $0x78,%rsp
+   2e2311789:	pop    %rbx
+   2e231178a:	pop    %rsi
+   2e231178b:	pop    %rdi
+   2e231178c:	pop    %rbp
+   2e231178d:	ret
+   2e231178e:	xchg   %ax,%ax
+   2e2311790:	movl   $0x0,(%rcx,%rax,4)
+   2e2311797:	add    $0x1,%rax
+   2e231179b:	cmp    %rax,%rbx
+   2e231179e:	jne    0x2e2311568
+   2e23117a4:	jmp    0x2e2311591
+   2e23117a9:	nopl   0x0(%rax)
+   2e23117b0:	pxor   %xmm0,%xmm0
+   2e23117b4:	movupd %xmm0,%xmm8
+   2e23117b9:	divsd  %xmm0,%xmm8
+   2e23117be:	ucomisd %xmm8,%xmm0
+   2e23117c3:	ja     0x2e23117f8
+   2e23117c5:	movupd %xmm8,%xmm9
+   2e23117ca:	sqrtsd %xmm9,%xmm9
+   2e23117cf:	movupd %xmm9,%xmm6
+   2e23117d4:	jmp    0x2e231175c
+   2e23117d6:	xor    %eax,%eax
+   2e23117d8:	xor    %r9d,%r9d
+   2e23117db:	jmp    0x2e23115eb
+   2e23117e0:	mov    %rcx,0x28(%rsp)
+   2e23117e5:	call   0x2e2312f10
+   2e23117ea:	mov    0x28(%rsp),%rcx
+   2e23117ef:	movupd %xmm0,%xmm6
+   2e23117f3:	jmp    0x2e231175c
+   2e23117f8:	movupd %xmm8,%xmm0
+   2e23117fd:	mov    %rax,0x28(%rsp)
+   2e2311802:	pxor   %xmm7,%xmm7
+   2e2311806:	call   0x2e2312f10
+   2e231180b:	mov    0x28(%rsp),%rcx
+   2e2311810:	movupd %xmm0,%xmm9
+   2e2311815:	movupd %xmm7,%xmm0
+   2e2311819:	jmp    0x2e2311742
+   2e231181e:	movupd %xmm9,%xmm0
+   2e2311823:	mov    %rcx,0x28(%rsp)
+   2e2311828:	call   0x2e2312f10
+   2e231182d:	mov    0x28(%rsp),%rcx
+   2e2311832:	movupd %xmm0,%xmm9
+   2e2311837:	jmp    0x2e2311709
+   2e231183c:	nopl   0x0(%rax)
+   2e2311840:	jmp    0x2e2313210
+   2e2311845:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e2311850:	push   %r15
+   2e2311852:	push   %r14
+   2e2311854:	push   %r13
+   2e2311856:	push   %r12
+   2e2311858:	push   %rbp
+   2e2311859:	push   %rdi
+   2e231185a:	push   %rsi
+   2e231185b:	push   %rbx
+   2e231185c:	sub    $0x78,%rsp
+   2e2311860:	movups %xmm6,0x60(%rsp)
+   2e2311865:	movslq %r8d,%rsi
+   2e2311868:	mov    %rcx,%rdi
+   2e231186b:	mov    %rdx,0xc8(%rsp)
+   2e2311873:	mov    %rsi,%rbx
+   2e2311876:	mov    %r8d,0xd0(%rsp)
+   2e231187e:	lea    0x0(,%rsi,8),%r13
+   2e2311886:	shl    $0x4,%rbx
+   2e231188a:	mov    %r9d,0xd8(%rsp)
+   2e2311892:	mov    %rbx,%rcx
+   2e2311895:	mov    %rsi,0x28(%rsp)
+   2e231189a:	call   0x2e2313220
+   2e231189f:	mov    %rbx,%rcx
+   2e23118a2:	mov    %rax,%r15
+   2e23118a5:	call   0x2e2313220
+   2e23118aa:	lea    0x0(,%rsi,4),%rcx
+   2e23118b2:	mov    %rax,%r14
+   2e23118b5:	call   0x2e2313220
+   2e23118ba:	mov    %r13,%rcx
+   2e23118bd:	mov    %rax,%rbx
+   2e23118c0:	call   0x2e2313220
+   2e23118c5:	mov    %r13,%rcx
+   2e23118c8:	mov    %rax,%r12
+   2e23118cb:	call   0x2e2313220
+   2e23118d0:	mov    0xe0(%rsp),%ecx
+   2e23118d7:	mov    %rax,%rbp
+   2e23118da:	test   %ecx,%ecx
+   2e23118dc:	jne    0x2e2311f60
+   2e23118e2:	movq   $0x0,0x30(%rsp)
+   2e23118eb:	mov    0xd0(%rsp),%esi
+   2e23118f2:	movq   $0x0,0x48(%rsp)
+   2e23118fb:	test   %esi,%esi
+   2e23118fd:	jle    0x2e23120ba
+   2e2311903:	mov    0xd0(%rsp),%eax
+   2e231190a:	mov    %rdi,%rdx
+   2e231190d:	mov    %r12,%rcx
+   2e2311910:	sub    $0x1,%eax
+   2e2311913:	lea    0x8(,%rax,8),%r13
+   2e231191b:	mov    0xd0(%rsp),%eax
+   2e2311922:	test   %eax,%eax
+   2e2311924:	mov    $0x8,%eax
+   2e2311929:	cmovle %rax,%r13
+   2e231192d:	mov    %r13,%r8
+   2e2311930:	call   0x2e2313228
+   2e2311935:	mov    0xc8(%rsp),%rdx
+   2e231193d:	mov    %r13,%r8
+   2e2311940:	mov    %rbp,%rcx
+   2e2311943:	xor    %r13d,%r13d
+   2e2311946:	call   0x2e2313228
+   2e231194b:	mov    %rbx,0x40(%rsp)
+   2e2311950:	xor    %eax,%eax
+   2e2311952:	xor    %r10d,%r10d
+   2e2311955:	movsd  0x36a3(%rip),%xmm1        # 0x2e2315000
+   2e231195d:	mov    0x28(%rsp),%rbx
+   2e2311962:	mov    $0xffffffff,%r9d
+   2e2311968:	mov    $0xffffffff,%r8d
+   2e231196e:	mov    0xc8(%rsp),%r11
+   2e2311976:	mov    0xd0(%rsp),%esi
+   2e231197d:	jmp    0x2e23119c7
+   2e231197f:	nop
+   2e2311980:	lea    (%rsi,%r9,1),%edx
+   2e2311984:	movsd  (%r11,%rax,8),%xmm0
+   2e231198a:	sub    $0x1,%r9d
+   2e231198e:	movslq %edx,%rdx
+   2e2311991:	shl    $0x4,%rdx
+   2e2311995:	add    %r15,%rdx
+   2e2311998:	ucomisd %xmm0,%xmm0
+   2e231199c:	mov    %eax,0x8(%rdx)
+   2e231199f:	movsd  %xmm1,(%rdx)
+   2e23119a3:	jnp    0x2e23119f5
+   2e23119a5:	lea    (%rsi,%r8,1),%edx
+   2e23119a9:	add    $0x1,%rax
+   2e23119ad:	sub    $0x1,%r8d
+   2e23119b1:	movslq %edx,%rdx
+   2e23119b4:	shl    $0x4,%rdx
+   2e23119b8:	add    %r14,%rdx
+   2e23119bb:	mov    %ecx,0x8(%rdx)
+   2e23119be:	movsd  %xmm1,(%rdx)
+   2e23119c2:	cmp    %rax,%rbx
+   2e23119c5:	je     0x2e2311a13
+   2e23119c7:	movsd  (%rdi,%rax,8),%xmm0
+   2e23119cc:	mov    %eax,%ecx
+   2e23119ce:	ucomisd %xmm0,%xmm0
+   2e23119d2:	jp     0x2e2311980
+   2e23119d4:	movslq %r13d,%rdx
+   2e23119d7:	add    $0x1,%r13d
+   2e23119db:	shl    $0x4,%rdx
+   2e23119df:	add    %r15,%rdx
+   2e23119e2:	movsd  %xmm0,(%rdx)
+   2e23119e6:	movsd  (%r11,%rax,8),%xmm0
+   2e23119ec:	mov    %eax,0x8(%rdx)
+   2e23119ef:	ucomisd %xmm0,%xmm0
+   2e23119f3:	jp     0x2e23119a5
+   2e23119f5:	movslq %r10d,%rdx
+   2e23119f8:	add    $0x1,%rax
+   2e23119fc:	add    $0x1,%r10d
+   2e2311a00:	shl    $0x4,%rdx
+   2e2311a04:	add    %r14,%rdx
+   2e2311a07:	mov    %ecx,0x8(%rdx)
+   2e2311a0a:	movsd  %xmm0,(%rdx)
+   2e2311a0e:	cmp    %rax,%rbx
+   2e2311a11:	jne    0x2e23119c7
+   2e2311a13:	cmp    %r10d,%r13d
+   2e2311a16:	mov    %r10d,%r11d
+   2e2311a19:	mov    0x40(%rsp),%rbx
+   2e2311a1e:	mov    %r10d,0x38(%rsp)
+   2e2311a23:	cmovle %r13d,%r11d
+   2e2311a27:	movslq %r13d,%rdx
+   2e2311a2a:	movslq %r10d,%rsi
+   2e2311a2d:	movslq %r11d,%rax
+   2e2311a30:	shl    $0x2,%rax
+   2e2311a34:	mov    %rax,0x40(%rsp)
+   2e2311a39:	lea    -0x6d0(%rip),%r9        # 0x2e2311370
+   2e2311a40:	mov    $0x10,%r8d
+   2e2311a46:	mov    %r15,%rcx
+   2e2311a49:	mov    %r11d,0x50(%rsp)
+   2e2311a4e:	call   0x2e2313230
+   2e2311a53:	mov    %rsi,%rdx
+   2e2311a56:	lea    -0x6ed(%rip),%r9        # 0x2e2311370
+   2e2311a5d:	mov    %r14,%rcx
+   2e2311a60:	mov    $0x10,%r8d
+   2e2311a66:	call   0x2e2313230
+   2e2311a6b:	mov    0x40(%rsp),%rsi
+   2e2311a70:	mov    %rsi,%rcx
+   2e2311a73:	call   0x2e2313220
+   2e2311a78:	mov    %rsi,%rcx
+   2e2311a7b:	mov    %rax,0x40(%rsp)
+   2e2311a80:	call   0x2e2313220
+   2e2311a85:	mov    0xd8(%rsp),%r11d
+   2e2311a8d:	mov    %rax,%rsi
+   2e2311a90:	test   %r11d,%r11d
+   2e2311a93:	jne    0x2e2311ee8
+   2e2311a99:	mov    0x50(%rsp),%r11d
+   2e2311a9e:	test   %r11d,%r11d
+   2e2311aa1:	setg   %al
+   2e2311aa4:	test   %r13d,%r13d
+   2e2311aa7:	jle    0x2e2311ecf
+   2e2311aad:	test   %al,%al
+   2e2311aaf:	je     0x2e2311ecf
+   2e2311ab5:	lea    -0x1(%r13),%eax
+   2e2311ab9:	mov    0x40(%rsp),%r9
+   2e2311abe:	mov    0xc8(%rsp),%r8
+   2e2311ac6:	xor    %edx,%edx
+   2e2311ac8:	cltq
+   2e2311aca:	nopw   0x0(%rax,%rax,1)
+   2e2311ad0:	mov    %rax,%rcx
+   2e2311ad3:	shl    $0x4,%rcx
+   2e2311ad7:	movslq 0x8(%r15,%rcx,1),%r10
+   2e2311adc:	movsd  (%r8,%r10,8),%xmm0
+   2e2311ae2:	mov    %r10,%rcx
+   2e2311ae5:	ucomisd %xmm0,%xmm0
+   2e2311ae9:	jnp    0x2e2311af5
+   2e2311aeb:	movslq %edx,%r10
+   2e2311aee:	add    $0x1,%edx
+   2e2311af1:	mov    %ecx,(%r9,%r10,4)
+   2e2311af5:	test   %eax,%eax
+   2e2311af7:	setg   %r10b
+   2e2311afb:	cmp    %r11d,%edx
+   2e2311afe:	setl   %cl
+   2e2311b01:	sub    $0x1,%rax
+   2e2311b05:	test   %cl,%r10b
+   2e2311b08:	jne    0x2e2311ad0
+   2e2311b0a:	mov    0x38(%rsp),%r9d
+   2e2311b0f:	test   %r9d,%r9d
+   2e2311b12:	jle    0x2e23120da
+   2e2311b18:	mov    0x38(%rsp),%eax
+   2e2311b1c:	mov    0xd8(%rsp),%ecx
+   2e2311b23:	sub    $0x1,%eax
+   2e2311b26:	cltq
+   2e2311b28:	nopl   0x0(%rax,%rax,1)
+   2e2311b30:	mov    %rax,%r8
+   2e2311b33:	shl    $0x4,%r8
+   2e2311b37:	movslq 0x8(%r14,%r8,1),%r9
+   2e2311b3c:	movsd  (%rdi,%r9,8),%xmm0
+   2e2311b42:	mov    %r9,%r8
+   2e2311b45:	ucomisd %xmm0,%xmm0
+   2e2311b49:	jnp    0x2e2311b55
+   2e2311b4b:	movslq %ecx,%r9
+   2e2311b4e:	add    $0x1,%ecx
+   2e2311b51:	mov    %r8d,(%rsi,%r9,4)
+   2e2311b55:	test   %eax,%eax
+   2e2311b57:	setg   %r9b
+   2e2311b5b:	cmp    %r11d,%ecx
+   2e2311b5e:	setl   %r8b
+   2e2311b62:	sub    $0x1,%rax
+   2e2311b66:	test   %r8b,%r9b
+   2e2311b69:	jne    0x2e2311b30
+   2e2311b6b:	mov    %ecx,0xd8(%rsp)
+   2e2311b72:	test   %ecx,%ecx
+   2e2311b74:	je     0x2e23120da
+   2e2311b7a:	movslq %ecx,%rax
+   2e2311b7d:	lea    0x1(%rcx),%r9d
    2e2311b81:	nopl   0x0(%rax)
-   2e2311b88:	mov    %r8d,%ecx
+   2e2311b88:	mov    %r9d,%r8d
    2e2311b8b:	pxor   %xmm0,%xmm0
-   2e2311b8f:	movslq -0x4(%r9,%rax,4),%rdx
-   2e2311b94:	sub    %eax,%ecx
-   2e2311b96:	sub    $0x1,%rax
-   2e2311b9a:	cvtsi2sd %ecx,%xmm0
-   2e2311b9e:	movsd  %xmm0,(%r15,%rdx,8)
-   2e2311ba4:	test   %eax,%eax
-   2e2311ba6:	jne    0x2e2311b88
-   2e2311ba8:	mov    %r8d,0x44(%rsp)
-   2e2311bad:	jmp    0x2e2311bfe
-   2e2311baf:	lea    (%r12,%r8,1),%edx
-   2e2311bb3:	sub    $0x1,%r8d
-   2e2311bb7:	movslq %edx,%rdx
-   2e2311bba:	shl    $0x4,%rdx
-   2e2311bbe:	add    %r13,%rdx
-   2e2311bc1:	mov    %r11d,0x8(%rdx)
-   2e2311bc5:	movsd  %xmm1,(%rdx)
-   2e2311bc9:	jmp    0x2e23119eb
-   2e2311bce:	lea    (%r12,%r9,1),%edx
-   2e2311bd2:	sub    $0x1,%r9d
-   2e2311bd6:	movslq %edx,%rdx
-   2e2311bd9:	shl    $0x4,%rdx
-   2e2311bdd:	add    %r14,%rdx
-   2e2311be0:	mov    %eax,0x8(%rdx)
-   2e2311be3:	movsd  %xmm1,(%rdx)
-   2e2311be7:	jmp    0x2e23119c6
-   2e2311bec:	nopl   0x0(%rax)
-   2e2311bf0:	movl   $0x1,0x44(%rsp)
-   2e2311bf8:	mov    $0x1,%r11d
-   2e2311bfe:	mov    0xc0(%rsp),%eax
-   2e2311c05:	mov    0x20(%rsp),%r8
-   2e2311c0a:	lea    -0x1(%rax),%ecx
-   2e2311c0d:	xor    %eax,%eax
-   2e2311c0f:	jmp    0x2e2311c1b
-   2e2311c11:	nopl   0x0(%rax)
-   2e2311c18:	mov    %rdx,%rax
-   2e2311c1b:	movsd  (%r15,%rax,8),%xmm0
-   2e2311c21:	ucomisd %xmm0,%xmm0
-   2e2311c25:	jp     0x2e2311f38
-   2e2311c2b:	movsd  (%r8,%rax,8),%xmm0
-   2e2311c31:	xor    %edx,%edx
-   2e2311c33:	ucomisd %xmm0,%xmm0
-   2e2311c37:	setp   %dl
-   2e2311c3a:	mov    %edx,(%r12,%rax,4)
-   2e2311c3e:	lea    0x1(%rax),%rdx
-   2e2311c42:	cmp    %rax,%rcx
-   2e2311c45:	jne    0x2e2311c18
-   2e2311c47:	mov    0x28(%rsp),%edx
-   2e2311c4b:	movsd  0x33b5(%rip),%xmm2        # 0x2e2315008
-   2e2311c53:	xor    %edi,%edi
-   2e2311c55:	test   %edx,%edx
-   2e2311c57:	je     0x2e2311d94
-   2e2311c5d:	mov    %r13,0x48(%rsp)
-   2e2311c62:	mov    0x20(%rsp),%rbp
-   2e2311c67:	mov    0x28(%rsp),%r13d
-   2e2311c6c:	mov    %rbx,0xb8(%rsp)
-   2e2311c74:	mov    %r15,0x28(%rsp)
-   2e2311c79:	mov    %r11d,%r15d
-   2e2311c7c:	jmp    0x2e2311c8c
-   2e2311c7e:	xchg   %ax,%ax
-   2e2311c80:	add    $0x1,%edi
-   2e2311c83:	cmp    %r13d,%edi
-   2e2311c86:	jge    0x2e2311d82
-   2e2311c8c:	movslq %edi,%rax
-   2e2311c8f:	shl    $0x4,%rax
-   2e2311c93:	add    %r14,%rax
-   2e2311c96:	movslq 0x8(%rax),%rdx
-   2e2311c9a:	mov    (%r12,%rdx,4),%r10d
-   2e2311c9e:	test   %r10d,%r10d
-   2e2311ca1:	jne    0x2e2311c80
-   2e2311ca3:	movsd  (%rsi,%rdx,8),%xmm0
-   2e2311ca8:	mov    %r13d,%edx
-   2e2311cab:	sub    %edi,%edx
-   2e2311cad:	test   %edx,%edx
-   2e2311caf:	jle    0x2e2311f52
-   2e2311cb5:	lea    -0x1(%rdi,%rdx,1),%ebx
-   2e2311cb9:	mov    %edi,%r11d
-   2e2311cbc:	mov    %edi,%edx
-   2e2311cbe:	mov    %rax,%rcx
-   2e2311cc1:	xor    %r8d,%r8d
-   2e2311cc4:	xor    %r9d,%r9d
-   2e2311cc7:	jmp    0x2e2311cdb
+   2e2311b8f:	movslq -0x4(%rsi,%rax,4),%rcx
+   2e2311b94:	sub    %eax,%r8d
+   2e2311b97:	sub    $0x1,%rax
+   2e2311b9b:	cvtsi2sd %r8d,%xmm0
+   2e2311ba0:	movsd  %xmm0,(%r12,%rcx,8)
+   2e2311ba6:	test   %eax,%eax
+   2e2311ba8:	jne    0x2e2311b88
+   2e2311baa:	mov    %r9d,%ecx
+   2e2311bad:	test   %edx,%edx
+   2e2311baf:	je     0x2e23120e4
+   2e2311bb5:	mov    0x40(%rsp),%r10
+   2e2311bba:	movslq %edx,%rax
+   2e2311bbd:	lea    0x1(%rdx),%r9d
+   2e2311bc1:	nopl   0x0(%rax)
+   2e2311bc8:	mov    %r9d,%r8d
+   2e2311bcb:	pxor   %xmm0,%xmm0
+   2e2311bcf:	movslq -0x4(%r10,%rax,4),%rdx
+   2e2311bd4:	sub    %eax,%r8d
+   2e2311bd7:	sub    $0x1,%rax
+   2e2311bdb:	cvtsi2sd %r8d,%xmm0
+   2e2311be0:	movsd  %xmm0,0x0(%rbp,%rdx,8)
+   2e2311be6:	test   %eax,%eax
+   2e2311be8:	jne    0x2e2311bc8
+   2e2311bea:	mov    0xd0(%rsp),%r8d
+   2e2311bf2:	mov    %r9d,%r10d
+   2e2311bf5:	xor    %eax,%eax
+   2e2311bf7:	test   %r8d,%r8d
+   2e2311bfa:	jg     0x2e2311f10
+   2e2311c00:	movsd  0x3400(%rip),%xmm2        # 0x2e2315008
+   2e2311c08:	xor    %r8d,%r8d
+   2e2311c0b:	test   %r13d,%r13d
+   2e2311c0e:	je     0x2e2311d25
+   2e2311c14:	mov    %r10d,0x28(%rsp)
+   2e2311c19:	mov    %r14,0x50(%rsp)
+   2e2311c1e:	mov    %rbp,0x58(%rsp)
+   2e2311c23:	jmp    0x2e2311c35
+   2e2311c25:	nopl   (%rax)
+   2e2311c28:	add    $0x1,%r8d
+   2e2311c2c:	cmp    %r13d,%r8d
+   2e2311c2f:	jge    0x2e2311d16
+   2e2311c35:	movslq %r8d,%rax
+   2e2311c38:	mov    %rax,%rdx
+   2e2311c3b:	shl    $0x4,%rdx
+   2e2311c3f:	add    %r15,%rdx
+   2e2311c42:	movslq 0x8(%rdx),%r9
+   2e2311c46:	mov    (%rbx,%r9,4),%ebp
+   2e2311c4a:	test   %ebp,%ebp
+   2e2311c4c:	jne    0x2e2311c28
+   2e2311c4e:	mov    %r13d,%r14d
+   2e2311c51:	movsd  (%rdi,%r9,8),%xmm0
+   2e2311c57:	xor    %r11d,%r11d
+   2e2311c5a:	xor    %r10d,%r10d
+   2e2311c5d:	sub    %r8d,%r14d
+   2e2311c60:	movslq %r14d,%r14
+   2e2311c63:	add    %rax,%r14
+   2e2311c66:	mov    %rdx,%rax
+   2e2311c69:	shl    $0x4,%r14
+   2e2311c6d:	add    %r15,%r14
+   2e2311c70:	jmp    0x2e2311c80
+   2e2311c72:	nopw   0x0(%rax,%rax,1)
+   2e2311c78:	movslq 0x8(%rax),%r9
+   2e2311c7c:	mov    (%rbx,%r9,4),%r11d
+   2e2311c80:	movslq 0x8(%rax),%r9
+   2e2311c84:	test   %r11d,%r11d
+   2e2311c87:	jne    0x2e2311c97
+   2e2311c89:	ucomisd (%rdi,%r9,8),%xmm0
+   2e2311c8f:	jp     0x2e2311ca0
+   2e2311c91:	jne    0x2e2311ca0
+   2e2311c93:	add    $0x1,%r10d
+   2e2311c97:	add    $0x10,%rax
+   2e2311c9b:	cmp    %r14,%rax
+   2e2311c9e:	jne    0x2e2311c78
+   2e2311ca0:	lea    -0x1(%r10),%eax
+   2e2311ca4:	pxor   %xmm0,%xmm0
+   2e2311ca8:	pxor   %xmm1,%xmm1
+   2e2311cac:	cvtsi2sd %eax,%xmm0
+   2e2311cb0:	cvtsi2sd %ecx,%xmm1
+   2e2311cb4:	mulsd  %xmm2,%xmm0
+   2e2311cb8:	addsd  %xmm1,%xmm0
+   2e2311cbc:	test   %r10d,%r10d
+   2e2311cbf:	je     0x2e2312095
+   2e2311cc5:	xor    %eax,%eax
+   2e2311cc7:	jmp    0x2e2311cf5
    2e2311cc9:	nopl   0x0(%rax)
-   2e2311cd0:	movslq 0x8(%rcx),%r8
-   2e2311cd4:	add    $0x1,%edx
-   2e2311cd7:	mov    (%r12,%r8,4),%r8d
-   2e2311cdb:	test   %r8d,%r8d
-   2e2311cde:	jne    0x2e2311d00
-   2e2311ce0:	movslq %edx,%r8
-   2e2311ce3:	shl    $0x4,%r8
-   2e2311ce7:	movslq 0x8(%r14,%r8,1),%r8
-   2e2311cec:	ucomisd (%rsi,%r8,8),%xmm0
-   2e2311cf2:	jp     0x2e2311d08
-   2e2311cf4:	comisd (%rsi,%r8,8),%xmm0
-   2e2311cfa:	jne    0x2e2311d08
-   2e2311cfc:	add    $0x1,%r9d
-   2e2311d00:	add    $0x10,%rcx
-   2e2311d04:	cmp    %edx,%ebx
-   2e2311d06:	jne    0x2e2311cd0
-   2e2311d08:	lea    -0x1(%r9),%ecx
-   2e2311d0c:	pxor   %xmm0,%xmm0
-   2e2311d10:	pxor   %xmm1,%xmm1
-   2e2311d14:	cvtsi2sd %ecx,%xmm0
-   2e2311d18:	cvtsi2sd %r15d,%xmm1
-   2e2311d1d:	add    %r9d,%r15d
-   2e2311d20:	mulsd  %xmm2,%xmm0
-   2e2311d24:	addsd  %xmm1,%xmm0
-   2e2311d28:	test   %r9d,%r9d
-   2e2311d2b:	je     0x2e2311d74
-   2e2311d2d:	xor    %edx,%edx
-   2e2311d2f:	jmp    0x2e2311d63
-   2e2311d31:	nopl   0x0(%rax)
-   2e2311d38:	movslq %r11d,%rdx
-   2e2311d3b:	add    $0x1,%r10d
-   2e2311d3f:	add    $0x10,%rax
-   2e2311d43:	add    $0x1,%r11d
-   2e2311d47:	shl    $0x4,%rdx
-   2e2311d4b:	movslq 0x8(%r14,%rdx,1),%rdx
-   2e2311d50:	movsd  %xmm0,0x0(%rbp,%rdx,8)
-   2e2311d56:	cmp    %r9d,%r10d
-   2e2311d59:	jge    0x2e2311d74
-   2e2311d5b:	movslq 0x8(%rax),%rdx
-   2e2311d5f:	mov    (%r12,%rdx,4),%edx
-   2e2311d63:	test   %edx,%edx
-   2e2311d65:	je     0x2e2311d38
-   2e2311d67:	add    $0x10,%rax
-   2e2311d6b:	add    $0x1,%r11d
-   2e2311d6f:	cmp    %r10d,%r9d
-   2e2311d72:	jg     0x2e2311d5b
-   2e2311d74:	add    %ecx,%edi
-   2e2311d76:	add    $0x1,%edi
-   2e2311d79:	cmp    %r13d,%edi
-   2e2311d7c:	jl     0x2e2311c8c
-   2e2311d82:	mov    0x48(%rsp),%r13
-   2e2311d87:	mov    0x28(%rsp),%r15
-   2e2311d8c:	mov    0xb8(%rsp),%rbx
-   2e2311d94:	mov    0x40(%rsp),%eax
-   2e2311d98:	movsd  0x3268(%rip),%xmm2        # 0x2e2315008
-   2e2311da0:	xor    %esi,%esi
-   2e2311da2:	test   %eax,%eax
-   2e2311da4:	je     0x2e2311ec6
-   2e2311daa:	mov    %r14,0x28(%rsp)
-   2e2311daf:	mov    0x40(%rsp),%ebp
-   2e2311db3:	mov    0x44(%rsp),%r14d
-   2e2311db8:	jmp    0x2e2311dcb
-   2e2311dba:	nopw   0x0(%rax,%rax,1)
-   2e2311dc0:	add    $0x1,%esi
-   2e2311dc3:	cmp    %ebp,%esi
-   2e2311dc5:	jge    0x2e2311ec1
-   2e2311dcb:	movslq %esi,%rax
-   2e2311dce:	shl    $0x4,%rax
-   2e2311dd2:	add    %r13,%rax
-   2e2311dd5:	movslq 0x8(%rax),%rdx
-   2e2311dd9:	mov    (%r12,%rdx,4),%r10d
-   2e2311ddd:	test   %r10d,%r10d
-   2e2311de0:	jne    0x2e2311dc0
-   2e2311de2:	movsd  (%rbx,%rdx,8),%xmm0
-   2e2311de7:	mov    %ebp,%edx
-   2e2311de9:	sub    %esi,%edx
-   2e2311deb:	test   %edx,%edx
-   2e2311ded:	jle    0x2e2311f5e
-   2e2311df3:	lea    -0x1(%rsi,%rdx,1),%edi
-   2e2311df7:	mov    %esi,%r11d
-   2e2311dfa:	mov    %esi,%edx
-   2e2311dfc:	mov    %rax,%rcx
-   2e2311dff:	xor    %r8d,%r8d
-   2e2311e02:	xor    %r9d,%r9d
-   2e2311e05:	jmp    0x2e2311e1b
-   2e2311e07:	nopw   0x0(%rax,%rax,1)
-   2e2311e10:	movslq 0x8(%rcx),%r8
-   2e2311e14:	add    $0x1,%edx
-   2e2311e17:	mov    (%r12,%r8,4),%r8d
-   2e2311e1b:	test   %r8d,%r8d
-   2e2311e1e:	jne    0x2e2311e40
-   2e2311e20:	movslq %edx,%r8
-   2e2311e23:	shl    $0x4,%r8
-   2e2311e27:	movslq 0x8(%r13,%r8,1),%r8
-   2e2311e2c:	ucomisd (%rbx,%r8,8),%xmm0
-   2e2311e32:	jp     0x2e2311e48
-   2e2311e34:	comisd (%rbx,%r8,8),%xmm0
-   2e2311e3a:	jne    0x2e2311e48
-   2e2311e3c:	add    $0x1,%r9d
-   2e2311e40:	add    $0x10,%rcx
-   2e2311e44:	cmp    %edi,%edx
-   2e2311e46:	jne    0x2e2311e10
-   2e2311e48:	lea    -0x1(%r9),%ecx
-   2e2311e4c:	pxor   %xmm0,%xmm0
-   2e2311e50:	pxor   %xmm1,%xmm1
-   2e2311e54:	cvtsi2sd %ecx,%xmm0
-   2e2311e58:	cvtsi2sd %r14d,%xmm1
-   2e2311e5d:	add    %r9d,%r14d
-   2e2311e60:	mulsd  %xmm2,%xmm0
-   2e2311e64:	addsd  %xmm1,%xmm0
-   2e2311e68:	test   %r9d,%r9d
-   2e2311e6b:	je     0x2e2311eb4
-   2e2311e6d:	xor    %edx,%edx
-   2e2311e6f:	jmp    0x2e2311ea3
-   2e2311e71:	nopl   0x0(%rax)
-   2e2311e78:	movslq %r11d,%rdx
-   2e2311e7b:	add    $0x1,%r10d
-   2e2311e7f:	add    $0x10,%rax
-   2e2311e83:	add    $0x1,%r11d
-   2e2311e87:	shl    $0x4,%rdx
-   2e2311e8b:	movslq 0x8(%r13,%rdx,1),%rdx
-   2e2311e90:	movsd  %xmm0,(%r15,%rdx,8)
-   2e2311e96:	cmp    %r9d,%r10d
-   2e2311e99:	jge    0x2e2311eb4
-   2e2311e9b:	movslq 0x8(%rax),%rdx
-   2e2311e9f:	mov    (%r12,%rdx,4),%edx
-   2e2311ea3:	test   %edx,%edx
-   2e2311ea5:	je     0x2e2311e78
-   2e2311ea7:	add    $0x10,%rax
-   2e2311eab:	add    $0x1,%r11d
-   2e2311eaf:	cmp    %r10d,%r9d
-   2e2311eb2:	jg     0x2e2311e9b
-   2e2311eb4:	add    %ecx,%esi
-   2e2311eb6:	add    $0x1,%esi
-   2e2311eb9:	cmp    %ebp,%esi
-   2e2311ebb:	jl     0x2e2311dcb
-   2e2311ec1:	mov    0x28(%rsp),%r14
-   2e2311ec6:	mov    0x20(%rsp),%rdi
-   2e2311ecb:	mov    0xc0(%rsp),%r8d
-   2e2311ed3:	mov    %r15,%rdx
-   2e2311ed6:	mov    %rdi,%rcx
-   2e2311ed9:	call   0x2e2311590
-   2e2311ede:	mov    %r14,%rcx
-   2e2311ee1:	movupd %xmm0,%xmm6
-   2e2311ee5:	call   0x2e2312f88
-   2e2311eea:	mov    %r13,%rcx
-   2e2311eed:	call   0x2e2312f88
-   2e2311ef2:	mov    %rdi,%rcx
-   2e2311ef5:	call   0x2e2312f88
-   2e2311efa:	mov    %r15,%rcx
-   2e2311efd:	call   0x2e2312f88
-   2e2311f02:	mov    %r12,%rcx
-   2e2311f05:	call   0x2e2312f88
-   2e2311f0a:	mov    0x38(%rsp),%rcx
-   2e2311f0f:	call   0x2e2312f88
-   2e2311f14:	mov    0x30(%rsp),%rcx
-   2e2311f19:	call   0x2e2312f88
-   2e2311f1e:	movupd %xmm6,%xmm0
-   2e2311f22:	movups 0x50(%rsp),%xmm6
-   2e2311f27:	add    $0x68,%rsp
-   2e2311f2b:	pop    %rbx
-   2e2311f2c:	pop    %rsi
-   2e2311f2d:	pop    %rdi
-   2e2311f2e:	pop    %rbp
-   2e2311f2f:	pop    %r12
-   2e2311f31:	pop    %r13
-   2e2311f33:	pop    %r14
-   2e2311f35:	pop    %r15
-   2e2311f37:	ret
-   2e2311f38:	movl   $0x1,(%r12,%rax,4)
-   2e2311f40:	lea    0x1(%rax),%rdx
-   2e2311f44:	cmp    %rax,%rcx
-   2e2311f47:	jne    0x2e2311c18
-   2e2311f4d:	jmp    0x2e2311c47
-   2e2311f52:	mov    $0xffffffff,%ecx
-   2e2311f57:	add    %ecx,%edi
-   2e2311f59:	jmp    0x2e2311d76
-   2e2311f5e:	mov    $0xffffffff,%ecx
-   2e2311f63:	add    %ecx,%esi
-   2e2311f65:	jmp    0x2e2311eb6
-   2e2311f6a:	lea    -0xbd1(%rip),%r9        # 0x2e23113a0
-   2e2311f71:	mov    $0x10,%r8d
-   2e2311f77:	xor    %edx,%edx
-   2e2311f79:	mov    %r14,%rcx
-   2e2311f7c:	call   0x2e2312f68
-   2e2311f81:	mov    $0x10,%r8d
-   2e2311f87:	xor    %edx,%edx
-   2e2311f89:	mov    %r13,%rcx
-   2e2311f8c:	lea    -0xbf3(%rip),%r9        # 0x2e23113a0
-   2e2311f93:	call   0x2e2312f68
-   2e2311f98:	xor    %ecx,%ecx
-   2e2311f9a:	call   0x2e2312f78
-   2e2311f9f:	xor    %ecx,%ecx
-   2e2311fa1:	mov    %rax,0x38(%rsp)
-   2e2311fa6:	call   0x2e2312f78
-   2e2311fab:	mov    %rax,0x30(%rsp)
-   2e2311fb0:	jmp    0x2e2311ec6
-   2e2311fb5:	movl   $0x1,0x44(%rsp)
-   2e2311fbd:	jmp    0x2e2311bfe
-   2e2311fc2:	test   %edx,%edx
-   2e2311fc4:	je     0x2e2311bf0
-   2e2311fca:	mov    $0x1,%r11d
-   2e2311fd0:	jmp    0x2e2311b75
-   2e2311fd5:	xor    %edx,%edx
-   2e2311fd7:	jmp    0x2e2311ad9
-   2e2311fdc:	nopl   0x0(%rax)
-   2e2311fe0:	imul   %r9d,%r8d
-   2e2311fe4:	mov    %r9d,%eax
-   2e2311fe7:	imul   %r9d,%edx
-   2e2311feb:	mov    0x28(%rsp),%r9d
-   2e2311ff0:	movslq %r8d,%r8
-   2e2311ff3:	lea    (%rcx,%r8,8),%r10
-   2e2311ff7:	movslq %edx,%rdx
-   2e2311ffa:	mov    %eax,%r8d
-   2e2311ffd:	lea    (%rcx,%rdx,8),%rcx
-   2e2312001:	mov    %r10,%rdx
-   2e2312004:	jmp    0x2e23118c0
-   2e2312009:	nopl   0x0(%rax)
-   2e2312010:	imul   %r9d,%r8d
-   2e2312014:	imul   %r9d,%edx
-   2e2312018:	movslq %r8d,%r8
-   2e231201b:	lea    (%rcx,%r8,8),%r10
-   2e231201f:	movslq %edx,%rdx
-   2e2312022:	mov    %r9d,%r8d
-   2e2312025:	lea    (%rcx,%rdx,8),%rcx
-   2e2312029:	mov    %r10,%rdx
-   2e231202c:	jmp    0x2e2311590
-   2e2312031:	nop
-   2e2312032:	nop
-   2e2312033:	nop
-   2e2312034:	nop
-   2e2312035:	nop
-   2e2312036:	nop
-   2e2312037:	nop
-   2e2312038:	nop
-   2e2312039:	nop
-   2e231203a:	nop
-   2e231203b:	nop
-   2e231203c:	nop
-   2e231203d:	nop
-   2e231203e:	nop
-   2e231203f:	nop
-   2e2312040:	sub    $0x28,%rsp
-   2e2312044:	mov    0x1fc5(%rip),%rax        # 0x2e2314010
-   2e231204b:	mov    (%rax),%rax
-   2e231204e:	test   %rax,%rax
-   2e2312051:	je     0x2e2312075
-   2e2312053:	nopl   0x0(%rax,%rax,1)
-   2e2312058:	call   *%rax
-   2e231205a:	mov    0x1faf(%rip),%rax        # 0x2e2314010
-   2e2312061:	lea    0x8(%rax),%rdx
-   2e2312065:	mov    0x8(%rax),%rax
-   2e2312069:	mov    %rdx,0x1fa0(%rip)        # 0x2e2314010
-   2e2312070:	test   %rax,%rax
-   2e2312073:	jne    0x2e2312058
-   2e2312075:	add    $0x28,%rsp
-   2e2312079:	ret
-   2e231207a:	nopw   0x0(%rax,%rax,1)
-   2e2312080:	push   %rsi
-   2e2312081:	push   %rbx
-   2e2312082:	sub    $0x28,%rsp
-   2e2312086:	mov    0x3143(%rip),%rdx        # 0x2e23151d0
-   2e231208d:	mov    (%rdx),%rax
-   2e2312090:	mov    %eax,%ecx
-   2e2312092:	cmp    $0xffffffff,%eax
-   2e2312095:	je     0x2e23120d0
-   2e2312097:	test   %ecx,%ecx
-   2e2312099:	je     0x2e23120bb
-   2e231209b:	mov    %ecx,%eax
-   2e231209d:	sub    $0x1,%ecx
-   2e23120a0:	lea    (%rdx,%rax,8),%rbx
-   2e23120a4:	sub    %rcx,%rax
-   2e23120a7:	lea    -0x8(%rdx,%rax,8),%rsi
-   2e23120ac:	nopl   0x0(%rax)
-   2e23120b0:	call   *(%rbx)
-   2e23120b2:	sub    $0x8,%rbx
-   2e23120b6:	cmp    %rsi,%rbx
-   2e23120b9:	jne    0x2e23120b0
-   2e23120bb:	lea    -0x82(%rip),%rcx        # 0x2e2312040
-   2e23120c2:	add    $0x28,%rsp
-   2e23120c6:	pop    %rbx
-   2e23120c7:	pop    %rsi
-   2e23120c8:	jmp    0x2e2311370
-   2e23120cd:	nopl   (%rax)
-   2e23120d0:	xor    %eax,%eax
-   2e23120d2:	nopw   0x0(%rax,%rax,1)
-   2e23120d8:	lea    0x1(%rax),%r8d
-   2e23120dc:	mov    %eax,%ecx
-   2e23120de:	cmpq   $0x0,(%rdx,%r8,8)
-   2e23120e3:	mov    %r8,%rax
-   2e23120e6:	jne    0x2e23120d8
-   2e23120e8:	jmp    0x2e2312097
-   2e23120ea:	nopw   0x0(%rax,%rax,1)
-   2e23120f0:	mov    0x5f2a(%rip),%eax        # 0x2e2318020
-   2e23120f6:	test   %eax,%eax
-   2e23120f8:	je     0x2e2312100
-   2e23120fa:	ret
-   2e23120fb:	nopl   0x0(%rax,%rax,1)
-   2e2312100:	movl   $0x1,0x5f16(%rip)        # 0x2e2318020
-   2e231210a:	jmp    0x2e2312080
-   2e231210f:	nop
-   2e2312110:	sub    $0x28,%rsp
-   2e2312114:	cmp    $0x3,%edx
-   2e2312117:	je     0x2e2312130
-   2e2312119:	test   %edx,%edx
-   2e231211b:	je     0x2e2312130
-   2e231211d:	mov    $0x1,%eax
-   2e2312122:	add    $0x28,%rsp
-   2e2312126:	ret
-   2e2312127:	nopw   0x0(%rax,%rax,1)
-   2e2312130:	call   0x2e23128e0
-   2e2312135:	mov    $0x1,%eax
-   2e231213a:	add    $0x28,%rsp
-   2e231213e:	ret
-   2e231213f:	nop
-   2e2312140:	push   %rsi
-   2e2312141:	push   %rbx
-   2e2312142:	sub    $0x28,%rsp
-   2e2312146:	mov    0x3073(%rip),%rax        # 0x2e23151c0
-   2e231214d:	cmpl   $0x2,(%rax)
-   2e2312150:	je     0x2e2312158
-   2e2312152:	movl   $0x2,(%rax)
-   2e2312158:	cmp    $0x2,%edx
-   2e231215b:	je     0x2e2312170
-   2e231215d:	cmp    $0x1,%edx
-   2e2312160:	je     0x2e23121b0
-   2e2312162:	mov    $0x1,%eax
-   2e2312167:	add    $0x28,%rsp
-   2e231216b:	pop    %rbx
-   2e231216c:	pop    %rsi
-   2e231216d:	ret
-   2e231216e:	xchg   %ax,%ax
-   2e2312170:	lea    0x8ed9(%rip),%rbx        # 0x2e231b050
-   2e2312177:	lea    0x8ed2(%rip),%rsi        # 0x2e231b050
-   2e231217e:	cmp    %rbx,%rsi
-   2e2312181:	je     0x2e2312162
-   2e2312183:	nopl   0x0(%rax,%rax,1)
-   2e2312188:	mov    (%rbx),%rax
-   2e231218b:	test   %rax,%rax
-   2e231218e:	je     0x2e2312192
-   2e2312190:	call   *%rax
-   2e2312192:	add    $0x8,%rbx
-   2e2312196:	cmp    %rbx,%rsi
-   2e2312199:	jne    0x2e2312188
-   2e231219b:	mov    $0x1,%eax
-   2e23121a0:	add    $0x28,%rsp
-   2e23121a4:	pop    %rbx
-   2e23121a5:	pop    %rsi
-   2e23121a6:	ret
-   2e23121a7:	nopw   0x0(%rax,%rax,1)
-   2e23121b0:	call   0x2e23128e0
-   2e23121b5:	mov    $0x1,%eax
-   2e23121ba:	add    $0x28,%rsp
-   2e23121be:	pop    %rbx
-   2e23121bf:	pop    %rsi
-   2e23121c0:	ret
-   2e23121c1:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e23121cc:	nopl   0x0(%rax)
-   2e23121d0:	xor    %eax,%eax
-   2e23121d2:	ret
-   2e23121d3:	nop
-   2e23121d4:	nop
-   2e23121d5:	nop
-   2e23121d6:	nop
-   2e23121d7:	nop
-   2e23121d8:	nop
-   2e23121d9:	nop
-   2e23121da:	nop
-   2e23121db:	nop
-   2e23121dc:	nop
-   2e23121dd:	nop
-   2e23121de:	nop
-   2e23121df:	nop
-   2e23121e0:	push   %r12
-   2e23121e2:	push   %rbx
-   2e23121e3:	sub    $0x38,%rsp
-   2e23121e7:	mov    %rcx,%r12
-   2e23121ea:	lea    0x58(%rsp),%rax
-   2e23121ef:	mov    $0x2,%ecx
-   2e23121f4:	mov    %rdx,0x58(%rsp)
-   2e23121f9:	mov    %r8,0x60(%rsp)
-   2e23121fe:	mov    %r9,0x68(%rsp)
-   2e2312203:	mov    %rax,0x28(%rsp)
-   2e2312208:	call   0x2e2313150
-   2e231220d:	mov    $0x1b,%r8d
-   2e2312213:	mov    $0x1,%edx
-   2e2312218:	lea    0x2e61(%rip),%rcx        # 0x2e2315080
-   2e231221f:	mov    %rax,%r9
-   2e2312222:	call   0x2e2312f80
-   2e2312227:	mov    0x28(%rsp),%rbx
-   2e231222c:	mov    $0x2,%ecx
-   2e2312231:	call   0x2e2313150
-   2e2312236:	mov    %r12,%rdx
-   2e2312239:	mov    %rax,%rcx
-   2e231223c:	mov    %rbx,%r8
-   2e231223f:	call   0x2e2312f50
-   2e2312244:	call   0x2e2312f98
-   2e2312249:	nop
-   2e231224a:	nopw   0x0(%rax,%rax,1)
-   2e2312250:	push   %r12
-   2e2312252:	push   %rbp
-   2e2312253:	push   %rdi
-   2e2312254:	push   %rsi
-   2e2312255:	push   %rbx
-   2e2312256:	sub    $0x50,%rsp
-   2e231225a:	movslq 0x5df3(%rip),%rdi        # 0x2e2318054
-   2e2312261:	mov    %rcx,%r12
-   2e2312264:	mov    %rdx,%rsi
-   2e2312267:	mov    %r8,%rbx
-   2e231226a:	test   %edi,%edi
-   2e231226c:	jle    0x2e2312400
-   2e2312272:	mov    0x5ddf(%rip),%rax        # 0x2e2318058
-   2e2312279:	xor    %ecx,%ecx
-   2e231227b:	add    $0x18,%rax
-   2e231227f:	nop
-   2e2312280:	mov    (%rax),%rdx
-   2e2312283:	cmp    %rdx,%r12
-   2e2312286:	jb     0x2e231229c
-   2e2312288:	mov    0x8(%rax),%r8
-   2e231228c:	mov    0x8(%r8),%r8d
-   2e2312290:	add    %r8,%rdx
-   2e2312293:	cmp    %rdx,%r12
-   2e2312296:	jb     0x2e2312327
-   2e231229c:	add    $0x1,%ecx
-   2e231229f:	add    $0x28,%rax
-   2e23122a3:	cmp    %edi,%ecx
-   2e23122a5:	jne    0x2e2312280
-   2e23122a7:	mov    %r12,%rcx
-   2e23122aa:	call   0x2e2312af0
-   2e23122af:	mov    %rax,%rbp
-   2e23122b2:	test   %rax,%rax
-   2e23122b5:	je     0x2e231245d
-   2e23122bb:	mov    0x5d96(%rip),%rax        # 0x2e2318058
-   2e23122c2:	lea    (%rdi,%rdi,4),%rdi
-   2e23122c6:	shl    $0x3,%rdi
-   2e23122ca:	add    %rdi,%rax
-   2e23122cd:	mov    %rbp,0x20(%rax)
-   2e23122d1:	movl   $0x0,(%rax)
-   2e23122d7:	call   0x2e2312c20
-   2e23122dc:	mov    0xc(%rbp),%ecx
-   2e23122df:	lea    0x20(%rsp),%rdx
-   2e23122e4:	mov    $0x30,%r8d
-   2e23122ea:	add    %rax,%rcx
-   2e23122ed:	mov    0x5d64(%rip),%rax        # 0x2e2318058
-   2e23122f4:	mov    %rcx,0x18(%rax,%rdi,1)
-   2e23122f9:	call   *0x7e65(%rip)        # 0x2e231a164
-   2e23122ff:	test   %rax,%rax
-   2e2312302:	je     0x2e2312442
-   2e2312308:	mov    0x44(%rsp),%eax
-   2e231230c:	lea    -0x40(%rax),%edx
-   2e231230f:	and    $0xffffffbf,%edx
-   2e2312312:	je     0x2e2312320
-   2e2312314:	lea    -0x4(%rax),%edx
-   2e2312317:	and    $0xfffffffb,%edx
-   2e231231a:	jne    0x2e23123b0
-   2e2312320:	addl   $0x1,0x5d2d(%rip)        # 0x2e2318054
-   2e2312327:	cmp    $0x8,%ebx
-   2e231232a:	jae    0x2e2312358
-   2e231232c:	test   $0x4,%bl
-   2e231232f:	jne    0x2e2312410
-   2e2312335:	test   %ebx,%ebx
-   2e2312337:	je     0x2e2312349
-   2e2312339:	movzbl (%rsi),%eax
-   2e231233c:	mov    %al,(%r12)
-   2e2312340:	test   $0x2,%bl
-   2e2312343:	jne    0x2e2312430
-   2e2312349:	add    $0x50,%rsp
-   2e231234d:	pop    %rbx
-   2e231234e:	pop    %rsi
-   2e231234f:	pop    %rdi
-   2e2312350:	pop    %rbp
-   2e2312351:	pop    %r12
-   2e2312353:	ret
-   2e2312354:	nopl   0x0(%rax)
-   2e2312358:	mov    (%rsi),%rax
-   2e231235b:	lea    0x8(%r12),%rcx
-   2e2312360:	and    $0xfffffffffffffff8,%rcx
-   2e2312364:	mov    %rax,(%r12)
-   2e2312368:	mov    %ebx,%eax
-   2e231236a:	mov    -0x8(%rsi,%rax,1),%rdx
-   2e231236f:	mov    %rdx,-0x8(%r12,%rax,1)
-   2e2312374:	sub    %rcx,%r12
-   2e2312377:	add    %r12d,%ebx
-   2e231237a:	sub    %r12,%rsi
-   2e231237d:	and    $0xfffffff8,%ebx
-   2e2312380:	cmp    $0x8,%ebx
-   2e2312383:	jb     0x2e2312349
-   2e2312385:	and    $0xfffffff8,%ebx
-   2e2312388:	xor    %eax,%eax
-   2e231238a:	mov    %eax,%edx
-   2e231238c:	add    $0x8,%eax
-   2e231238f:	mov    (%rsi,%rdx,1),%r8
-   2e2312393:	mov    %r8,(%rcx,%rdx,1)
-   2e2312397:	cmp    %ebx,%eax
-   2e2312399:	jb     0x2e231238a
-   2e231239b:	add    $0x50,%rsp
-   2e231239f:	pop    %rbx
-   2e23123a0:	pop    %rsi
-   2e23123a1:	pop    %rdi
-   2e23123a2:	pop    %rbp
-   2e23123a3:	pop    %r12
-   2e23123a5:	ret
-   2e23123a6:	cs nopw 0x0(%rax,%rax,1)
-   2e23123b0:	cmp    $0x2,%eax
-   2e23123b3:	mov    0x20(%rsp),%rcx
-   2e23123b8:	mov    0x38(%rsp),%rdx
-   2e23123bd:	mov    $0x4,%r8d
-   2e23123c3:	mov    $0x40,%eax
-   2e23123c8:	cmovne %eax,%r8d
-   2e23123cc:	add    0x5c85(%rip),%rdi        # 0x2e2318058
-   2e23123d3:	mov    %rcx,0x8(%rdi)
-   2e23123d7:	mov    %rdi,%r9
-   2e23123da:	mov    %rdx,0x10(%rdi)
-   2e23123de:	call   *0x7d78(%rip)        # 0x2e231a15c
-   2e23123e4:	test   %eax,%eax
-   2e23123e6:	jne    0x2e2312320
-   2e23123ec:	call   *0x7d42(%rip)        # 0x2e231a134
-   2e23123f2:	lea    0x2cff(%rip),%rcx        # 0x2e23150f8
-   2e23123f9:	mov    %eax,%edx
-   2e23123fb:	call   0x2e23121e0
-   2e2312400:	xor    %edi,%edi
-   2e2312402:	jmp    0x2e23122a7
-   2e2312407:	nopw   0x0(%rax,%rax,1)
-   2e2312410:	mov    (%rsi),%eax
-   2e2312412:	mov    %ebx,%ebx
-   2e2312414:	mov    %eax,(%r12)
-   2e2312418:	mov    -0x4(%rsi,%rbx,1),%eax
-   2e231241c:	mov    %eax,-0x4(%r12,%rbx,1)
-   2e2312421:	jmp    0x2e2312349
-   2e2312426:	cs nopw 0x0(%rax,%rax,1)
-   2e2312430:	mov    %ebx,%ebx
-   2e2312432:	movzwl -0x2(%rsi,%rbx,1),%eax
-   2e2312437:	mov    %ax,-0x2(%r12,%rbx,1)
-   2e231243d:	jmp    0x2e2312349
-   2e2312442:	mov    0x5c0f(%rip),%rax        # 0x2e2318058
-   2e2312449:	mov    0x8(%rbp),%edx
-   2e231244c:	lea    0x2c6d(%rip),%rcx        # 0x2e23150c0
-   2e2312453:	mov    0x18(%rax,%rdi,1),%r8
-   2e2312458:	call   0x2e23121e0
-   2e231245d:	mov    %r12,%rdx
-   2e2312460:	lea    0x2c39(%rip),%rcx        # 0x2e23150a0
-   2e2312467:	call   0x2e23121e0
-   2e231246c:	nop
-   2e231246d:	nopl   (%rax)
-   2e2312470:	push   %rbp
-   2e2312471:	push   %r15
-   2e2312473:	push   %r14
-   2e2312475:	push   %r13
-   2e2312477:	push   %r12
-   2e2312479:	push   %rdi
-   2e231247a:	push   %rsi
-   2e231247b:	push   %rbx
-   2e231247c:	sub    $0x38,%rsp
-   2e2312480:	lea    0x80(%rsp),%rbp
-   2e2312488:	mov    0x5bc2(%rip),%esi        # 0x2e2318050
-   2e231248e:	test   %esi,%esi
-   2e2312490:	je     0x2e23124a8
-   2e2312492:	lea    -0x48(%rbp),%rsp
-   2e2312496:	pop    %rbx
-   2e2312497:	pop    %rsi
-   2e2312498:	pop    %rdi
-   2e2312499:	pop    %r12
-   2e231249b:	pop    %r13
-   2e231249d:	pop    %r14
-   2e231249f:	pop    %r15
-   2e23124a1:	pop    %rbp
-   2e23124a2:	ret
-   2e23124a3:	nopl   0x0(%rax,%rax,1)
-   2e23124a8:	movl   $0x1,0x5b9e(%rip)        # 0x2e2318050
-   2e23124b2:	call   0x2e2312b80
-   2e23124b7:	cltq
-   2e23124b9:	lea    (%rax,%rax,4),%rax
-   2e23124bd:	lea    0xf(,%rax,8),%rax
-   2e23124c5:	and    $0xfffffffffffffff0,%rax
-   2e23124c9:	call   0x2e2312db0
-   2e23124ce:	mov    0x2d0b(%rip),%r12        # 0x2e23151e0
-   2e23124d5:	mov    0x2d14(%rip),%rbx        # 0x2e23151f0
-   2e23124dc:	movl   $0x0,0x5b6e(%rip)        # 0x2e2318054
-   2e23124e6:	sub    %rax,%rsp
-   2e23124e9:	lea    0x20(%rsp),%rax
-   2e23124ee:	mov    %rax,0x5b63(%rip)        # 0x2e2318058
-   2e23124f5:	mov    %r12,%rax
-   2e23124f8:	sub    %rbx,%rax
-   2e23124fb:	cmp    $0x7,%rax
-   2e23124ff:	jle    0x2e2312492
-   2e2312501:	mov    (%rbx),%edx
-   2e2312503:	cmp    $0xb,%rax
-   2e2312507:	jg     0x2e2312658
-   2e231250d:	test   %edx,%edx
-   2e231250f:	jne    0x2e23126e0
-   2e2312515:	mov    0x4(%rbx),%eax
-   2e2312518:	test   %eax,%eax
-   2e231251a:	jne    0x2e23126e0
-   2e2312520:	mov    0x8(%rbx),%edx
-   2e2312523:	cmp    $0x1,%edx
-   2e2312526:	jne    0x2e2312748
-   2e231252c:	add    $0xc,%rbx
-   2e2312530:	lea    -0x58(%rbp),%r15
-   2e2312534:	mov    0x2cd5(%rip),%r13        # 0x2e2315210
-   2e231253b:	movabs $0xffffffff00000000,%r14
-   2e2312545:	cmp    %r12,%rbx
-   2e2312548:	jb     0x2e2312589
-   2e231254a:	jmp    0x2e2312492
-   2e231254f:	nop
-   2e2312550:	movzbl (%rcx),%r8d
-   2e2312554:	mov    %r15,%rdi
-   2e2312557:	mov    %r8,%r10
-   2e231255a:	or     $0xffffffffffffff00,%r10
-   2e2312561:	test   %r8b,%r8b
-   2e2312564:	cmovs  %r10,%r8
-   2e2312568:	sub    %rdx,%r8
-   2e231256b:	mov    %r15,%rdx
-   2e231256e:	add    %r9,%r8
-   2e2312571:	mov    %r8,-0x58(%rbp)
-   2e2312575:	mov    $0x1,%r8d
-   2e231257b:	call   0x2e2312250
-   2e2312580:	add    $0xc,%rbx
-   2e2312584:	cmp    %r12,%rbx
-   2e2312587:	jae    0x2e2312600
-   2e2312589:	mov    (%rbx),%edx
-   2e231258b:	mov    0x4(%rbx),%ecx
-   2e231258e:	movzbl 0x8(%rbx),%r8d
-   2e2312593:	add    %r13,%rdx
-   2e2312596:	add    %r13,%rcx
-   2e2312599:	mov    (%rdx),%r9
-   2e231259c:	cmp    $0x20,%r8d
-   2e23125a0:	je     0x2e23126b0
-   2e23125a6:	ja     0x2e2312680
-   2e23125ac:	cmp    $0x8,%r8d
-   2e23125b0:	je     0x2e2312550
-   2e23125b2:	cmp    $0x10,%r8d
-   2e23125b6:	jne    0x2e2312731
-   2e23125bc:	movzwl (%rcx),%r8d
-   2e23125c0:	mov    %r15,%rdi
-   2e23125c3:	mov    %r8,%r10
-   2e23125c6:	or     $0xffffffffffff0000,%r10
-   2e23125cd:	test   %r8w,%r8w
-   2e23125d1:	cmovs  %r10,%r8
-   2e23125d5:	add    $0xc,%rbx
-   2e23125d9:	sub    %rdx,%r8
-   2e23125dc:	mov    %r15,%rdx
-   2e23125df:	add    %r9,%r8
-   2e23125e2:	mov    %r8,-0x58(%rbp)
-   2e23125e6:	mov    $0x2,%r8d
-   2e23125ec:	call   0x2e2312250
-   2e23125f1:	cmp    %r12,%rbx
-   2e23125f4:	jb     0x2e2312589
-   2e23125f6:	cs nopw 0x0(%rax,%rax,1)
-   2e2312600:	mov    0x5a4e(%rip),%eax        # 0x2e2318054
-   2e2312606:	test   %eax,%eax
-   2e2312608:	jle    0x2e2312492
-   2e231260e:	mov    0x7b47(%rip),%r12        # 0x2e231a15c
-   2e2312615:	xor    %ebx,%ebx
-   2e2312617:	nopw   0x0(%rax,%rax,1)
-   2e2312620:	mov    0x5a31(%rip),%rax        # 0x2e2318058
-   2e2312627:	add    %rbx,%rax
-   2e231262a:	mov    (%rax),%r8d
-   2e231262d:	test   %r8d,%r8d
-   2e2312630:	je     0x2e2312640
-   2e2312632:	mov    0x10(%rax),%rdx
-   2e2312636:	mov    0x8(%rax),%rcx
-   2e231263a:	mov    %rdi,%r9
-   2e231263d:	call   *%r12
-   2e2312640:	add    $0x1,%esi
-   2e2312643:	add    $0x28,%rbx
-   2e2312647:	cmp    0x5a07(%rip),%esi        # 0x2e2318054
-   2e231264d:	jl     0x2e2312620
-   2e231264f:	jmp    0x2e2312492
-   2e2312654:	nopl   0x0(%rax)
-   2e2312658:	test   %edx,%edx
-   2e231265a:	jne    0x2e23126e0
-   2e2312660:	mov    0x4(%rbx),%eax
-   2e2312663:	mov    %eax,%edi
-   2e2312665:	or     0x8(%rbx),%edi
-   2e2312668:	jne    0x2e2312518
-   2e231266e:	mov    0xc(%rbx),%edx
-   2e2312671:	add    $0xc,%rbx
-   2e2312675:	jmp    0x2e231250d
-   2e231267a:	nopw   0x0(%rax,%rax,1)
-   2e2312680:	cmp    $0x40,%r8d
-   2e2312684:	jne    0x2e2312731
-   2e231268a:	mov    (%rcx),%rax
-   2e231268d:	mov    $0x8,%r8d
-   2e2312693:	mov    %r15,%rdi
-   2e2312696:	sub    %rdx,%rax
-   2e2312699:	mov    %r15,%rdx
-   2e231269c:	add    %r9,%rax
-   2e231269f:	mov    %rax,-0x58(%rbp)
-   2e23126a3:	call   0x2e2312250
-   2e23126a8:	jmp    0x2e2312580
-   2e23126ad:	nopl   (%rax)
-   2e23126b0:	mov    (%rcx),%eax
-   2e23126b2:	mov    %r15,%rdi
-   2e23126b5:	mov    %rax,%r8
-   2e23126b8:	or     %r14,%rax
-   2e23126bb:	test   %r8d,%r8d
-   2e23126be:	cmovns %r8,%rax
-   2e23126c2:	mov    $0x4,%r8d
-   2e23126c8:	sub    %rdx,%rax
-   2e23126cb:	mov    %r15,%rdx
-   2e23126ce:	add    %r9,%rax
-   2e23126d1:	mov    %rax,-0x58(%rbp)
-   2e23126d5:	call   0x2e2312250
-   2e23126da:	jmp    0x2e2312580
-   2e23126df:	nop
-   2e23126e0:	cmp    %r12,%rbx
-   2e23126e3:	jae    0x2e2312492
-   2e23126e9:	sub    $0x1,%r12
-   2e23126ed:	mov    0x2b1c(%rip),%r13        # 0x2e2315210
-   2e23126f4:	lea    -0x58(%rbp),%rdi
-   2e23126f8:	sub    %rbx,%r12
-   2e23126fb:	shr    $0x3,%r12
-   2e23126ff:	lea    0x8(%rbx,%r12,8),%r12
-   2e2312704:	nopl   0x0(%rax)
-   2e2312708:	mov    0x4(%rbx),%ecx
-   2e231270b:	mov    (%rbx),%eax
-   2e231270d:	mov    $0x4,%r8d
-   2e2312713:	mov    %rdi,%rdx
-   2e2312716:	add    $0x8,%rbx
-   2e231271a:	add    %r13,%rcx
-   2e231271d:	add    (%rcx),%eax
-   2e231271f:	mov    %eax,-0x58(%rbp)
-   2e2312722:	call   0x2e2312250
-   2e2312727:	cmp    %r12,%rbx
-   2e231272a:	jne    0x2e2312708
-   2e231272c:	jmp    0x2e2312600
-   2e2312731:	mov    %r8d,%edx
-   2e2312734:	lea    0x2a1d(%rip),%rcx        # 0x2e2315158
-   2e231273b:	movq   $0x0,-0x58(%rbp)
-   2e2312743:	call   0x2e23121e0
-   2e2312748:	lea    0x29d1(%rip),%rcx        # 0x2e2315120
-   2e231274f:	call   0x2e23121e0
-   2e2312754:	nop
-   2e2312755:	nop
-   2e2312756:	nop
-   2e2312757:	nop
-   2e2312758:	nop
-   2e2312759:	nop
-   2e231275a:	nop
-   2e231275b:	nop
-   2e231275c:	nop
-   2e231275d:	nop
-   2e231275e:	nop
-   2e231275f:	nop
-   2e2312760:	push   %r12
-   2e2312762:	push   %rdi
-   2e2312763:	push   %rsi
-   2e2312764:	push   %rbx
-   2e2312765:	sub    $0x28,%rsp
-   2e2312769:	lea    0x5910(%rip),%rcx        # 0x2e2318080
-   2e2312770:	call   *0x79b6(%rip)        # 0x2e231a12c
-   2e2312776:	mov    0x58e3(%rip),%rbx        # 0x2e2318060
-   2e231277d:	test   %rbx,%rbx
-   2e2312780:	je     0x2e23127b4
-   2e2312782:	mov    0x79cb(%rip),%rdi        # 0x2e231a154
-   2e2312789:	mov    0x79a4(%rip),%rsi        # 0x2e231a134
-   2e2312790:	mov    (%rbx),%ecx
-   2e2312792:	call   *%rdi
-   2e2312794:	mov    %rax,%r12
-   2e2312797:	call   *%rsi
-   2e2312799:	test   %eax,%eax
-   2e231279b:	jne    0x2e23127ab
-   2e231279d:	test   %r12,%r12
-   2e23127a0:	je     0x2e23127ab
-   2e23127a2:	mov    0x8(%rbx),%rax
-   2e23127a6:	mov    %r12,%rcx
-   2e23127a9:	call   *%rax
-   2e23127ab:	mov    0x10(%rbx),%rbx
-   2e23127af:	test   %rbx,%rbx
-   2e23127b2:	jne    0x2e2312790
-   2e23127b4:	lea    0x58c5(%rip),%rcx        # 0x2e2318080
-   2e23127bb:	add    $0x28,%rsp
-   2e23127bf:	pop    %rbx
-   2e23127c0:	pop    %rsi
-   2e23127c1:	pop    %rdi
-   2e23127c2:	pop    %r12
-   2e23127c4:	rex.W jmp *0x7979(%rip)        # 0x2e231a144
-   2e23127cb:	nopl   0x0(%rax,%rax,1)
-   2e23127d0:	push   %rdi
-   2e23127d1:	push   %rsi
-   2e23127d2:	push   %rbx
-   2e23127d3:	sub    $0x20,%rsp
-   2e23127d7:	mov    0x588b(%rip),%eax        # 0x2e2318068
-   2e23127dd:	mov    %ecx,%edi
-   2e23127df:	mov    %rdx,%rsi
-   2e23127e2:	test   %eax,%eax
-   2e23127e4:	jne    0x2e23127f0
-   2e23127e6:	add    $0x20,%rsp
-   2e23127ea:	pop    %rbx
-   2e23127eb:	pop    %rsi
-   2e23127ec:	pop    %rdi
-   2e23127ed:	ret
-   2e23127ee:	xchg   %ax,%ax
-   2e23127f0:	mov    $0x18,%edx
-   2e23127f5:	mov    $0x1,%ecx
-   2e23127fa:	call   0x2e2312f90
-   2e23127ff:	mov    %rax,%rbx
-   2e2312802:	test   %rax,%rax
-   2e2312805:	je     0x2e2312843
-   2e2312807:	mov    %edi,(%rax)
-   2e2312809:	lea    0x5870(%rip),%rcx        # 0x2e2318080
-   2e2312810:	mov    %rsi,0x8(%rax)
-   2e2312814:	call   *0x7912(%rip)        # 0x2e231a12c
-   2e231281a:	mov    0x583f(%rip),%rax        # 0x2e2318060
-   2e2312821:	lea    0x5858(%rip),%rcx        # 0x2e2318080
-   2e2312828:	mov    %rbx,0x5831(%rip)        # 0x2e2318060
-   2e231282f:	mov    %rax,0x10(%rbx)
-   2e2312833:	call   *0x790b(%rip)        # 0x2e231a144
-   2e2312839:	xor    %eax,%eax
-   2e231283b:	add    $0x20,%rsp
-   2e231283f:	pop    %rbx
-   2e2312840:	pop    %rsi
-   2e2312841:	pop    %rdi
-   2e2312842:	ret
-   2e2312843:	or     $0xffffffff,%eax
-   2e2312846:	jmp    0x2e23127e6
-   2e2312848:	nopl   0x0(%rax,%rax,1)
-   2e2312850:	push   %rbx
-   2e2312851:	sub    $0x20,%rsp
-   2e2312855:	mov    0x580d(%rip),%eax        # 0x2e2318068
-   2e231285b:	mov    %ecx,%ebx
-   2e231285d:	test   %eax,%eax
-   2e231285f:	jne    0x2e2312870
-   2e2312861:	xor    %eax,%eax
-   2e2312863:	add    $0x20,%rsp
-   2e2312867:	pop    %rbx
-   2e2312868:	ret
-   2e2312869:	nopl   0x0(%rax)
-   2e2312870:	lea    0x5809(%rip),%rcx        # 0x2e2318080
-   2e2312877:	call   *0x78af(%rip)        # 0x2e231a12c
-   2e231287d:	mov    0x57dc(%rip),%rcx        # 0x2e2318060
-   2e2312884:	test   %rcx,%rcx
-   2e2312887:	je     0x2e23128b3
-   2e2312889:	xor    %edx,%edx
-   2e231288b:	jmp    0x2e231289b
-   2e231288d:	nopl   (%rax)
-   2e2312890:	mov    %rcx,%rdx
-   2e2312893:	test   %rax,%rax
-   2e2312896:	je     0x2e23128b3
-   2e2312898:	mov    %rax,%rcx
-   2e231289b:	mov    (%rcx),%eax
-   2e231289d:	cmp    %ebx,%eax
-   2e231289f:	mov    0x10(%rcx),%rax
-   2e23128a3:	jne    0x2e2312890
-   2e23128a5:	test   %rdx,%rdx
-   2e23128a8:	je     0x2e23128d0
-   2e23128aa:	mov    %rax,0x10(%rdx)
-   2e23128ae:	call   0x2e2312f88
-   2e23128b3:	lea    0x57c6(%rip),%rcx        # 0x2e2318080
-   2e23128ba:	call   *0x7884(%rip)        # 0x2e231a144
-   2e23128c0:	xor    %eax,%eax
-   2e23128c2:	add    $0x20,%rsp
-   2e23128c6:	pop    %rbx
-   2e23128c7:	ret
-   2e23128c8:	nopl   0x0(%rax,%rax,1)
-   2e23128d0:	mov    %rax,0x5789(%rip)        # 0x2e2318060
-   2e23128d7:	jmp    0x2e23128ae
-   2e23128d9:	nopl   0x0(%rax)
-   2e23128e0:	push   %rbx
-   2e23128e1:	sub    $0x20,%rsp
-   2e23128e5:	cmp    $0x2,%edx
-   2e23128e8:	je     0x2e23129b0
-   2e23128ee:	ja     0x2e2312918
-   2e23128f0:	test   %edx,%edx
-   2e23128f2:	je     0x2e2312940
-   2e23128f4:	mov    0x576e(%rip),%eax        # 0x2e2318068
-   2e23128fa:	test   %eax,%eax
-   2e23128fc:	je     0x2e2312930
-   2e23128fe:	movl   $0x1,0x5760(%rip)        # 0x2e2318068
-   2e2312908:	mov    $0x1,%eax
-   2e231290d:	add    $0x20,%rsp
-   2e2312911:	pop    %rbx
-   2e2312912:	ret
-   2e2312913:	nopl   0x0(%rax,%rax,1)
-   2e2312918:	cmp    $0x3,%edx
-   2e231291b:	jne    0x2e2312908
-   2e231291d:	mov    0x5745(%rip),%eax        # 0x2e2318068
-   2e2312923:	test   %eax,%eax
-   2e2312925:	je     0x2e2312908
-   2e2312927:	call   0x2e2312760
-   2e231292c:	jmp    0x2e2312908
-   2e231292e:	xchg   %ax,%ax
-   2e2312930:	lea    0x5749(%rip),%rcx        # 0x2e2318080
-   2e2312937:	call   *0x77ff(%rip)        # 0x2e231a13c
-   2e231293d:	jmp    0x2e23128fe
-   2e231293f:	nop
-   2e2312940:	mov    0x5722(%rip),%eax        # 0x2e2318068
-   2e2312946:	test   %eax,%eax
-   2e2312948:	je     0x2e231294f
-   2e231294a:	call   0x2e2312760
-   2e231294f:	mov    0x5713(%rip),%eax        # 0x2e2318068
-   2e2312955:	cmp    $0x1,%eax
-   2e2312958:	jne    0x2e2312908
-   2e231295a:	mov    0x56ff(%rip),%rbx        # 0x2e2318060
-   2e2312961:	test   %rbx,%rbx
-   2e2312964:	je     0x2e2312981
-   2e2312966:	cs nopw 0x0(%rax,%rax,1)
-   2e2312970:	mov    %rbx,%rcx
-   2e2312973:	mov    0x10(%rbx),%rbx
-   2e2312977:	call   0x2e2312f88
-   2e231297c:	test   %rbx,%rbx
-   2e231297f:	jne    0x2e2312970
-   2e2312981:	lea    0x56f8(%rip),%rcx        # 0x2e2318080
-   2e2312988:	movq   $0x0,0x56cd(%rip)        # 0x2e2318060
-   2e2312993:	movl   $0x0,0x56cb(%rip)        # 0x2e2318068
-   2e231299d:	call   *0x7781(%rip)        # 0x2e231a124
-   2e23129a3:	jmp    0x2e2312908
-   2e23129a8:	nopl   0x0(%rax,%rax,1)
-   2e23129b0:	call   0x2e2312da0
-   2e23129b5:	mov    $0x1,%eax
-   2e23129ba:	add    $0x20,%rsp
-   2e23129be:	pop    %rbx
-   2e23129bf:	ret
-   2e23129c0:	movslq 0x3c(%rcx),%rax
-   2e23129c4:	lea    (%rax,%rcx,1),%rdx
-   2e23129c8:	xor    %eax,%eax
-   2e23129ca:	cmpl   $0x4550,(%rdx)
-   2e23129d0:	jne    0x2e23129dd
-   2e23129d2:	xor    %eax,%eax
-   2e23129d4:	cmpw   $0x20b,0x18(%rdx)
-   2e23129da:	sete   %al
-   2e23129dd:	ret
-   2e23129de:	xchg   %ax,%ax
-   2e23129e0:	cmpw   $0x5a4d,(%rcx)
-   2e23129e5:	jne    0x2e23129f0
-   2e23129e7:	jmp    0x2e23129c0
-   2e23129e9:	nopl   0x0(%rax)
-   2e23129f0:	xor    %eax,%eax
-   2e23129f2:	ret
-   2e23129f3:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e23129fe:	xchg   %ax,%ax
-   2e2312a00:	movslq 0x3c(%rcx),%rax
-   2e2312a04:	add    %rax,%rcx
-   2e2312a07:	movzwl 0x14(%rcx),%eax
-   2e2312a0b:	lea    0x18(%rcx,%rax,1),%rax
-   2e2312a10:	movzwl 0x6(%rcx),%ecx
-   2e2312a14:	test   %ecx,%ecx
-   2e2312a16:	je     0x2e2312a45
-   2e2312a18:	sub    $0x1,%ecx
-   2e2312a1b:	lea    (%rcx,%rcx,4),%rcx
-   2e2312a1f:	lea    0x28(%rax,%rcx,8),%r9
-   2e2312a24:	nopl   0x0(%rax)
-   2e2312a28:	mov    0xc(%rax),%r8d
-   2e2312a2c:	mov    %r8,%rcx
-   2e2312a2f:	cmp    %rdx,%r8
-   2e2312a32:	ja     0x2e2312a3c
-   2e2312a34:	add    0x8(%rax),%ecx
-   2e2312a37:	cmp    %rdx,%rcx
-   2e2312a3a:	ja     0x2e2312a47
-   2e2312a3c:	add    $0x28,%rax
-   2e2312a40:	cmp    %r9,%rax
-   2e2312a43:	jne    0x2e2312a28
-   2e2312a45:	xor    %eax,%eax
-   2e2312a47:	ret
-   2e2312a48:	nopl   0x0(%rax,%rax,1)
-   2e2312a50:	push   %r12
-   2e2312a52:	push   %rsi
-   2e2312a53:	push   %rbx
-   2e2312a54:	sub    $0x20,%rsp
-   2e2312a58:	mov    %rcx,%rbx
-   2e2312a5b:	call   0x2e2312f60
-   2e2312a60:	cmp    $0x8,%rax
-   2e2312a64:	ja     0x2e2312ae0
-   2e2312a66:	mov    0x27a3(%rip),%rcx        # 0x2e2315210
-   2e2312a6d:	xor    %r12d,%r12d
-   2e2312a70:	cmpw   $0x5a4d,(%rcx)
-   2e2312a75:	jne    0x2e2312ace
-   2e2312a77:	call   0x2e23129c0
-   2e2312a7c:	test   %eax,%eax
-   2e2312a7e:	je     0x2e2312ace
-   2e2312a80:	movslq 0x3c(%rcx),%rax
-   2e2312a84:	add    %rax,%rcx
-   2e2312a87:	movzwl 0x14(%rcx),%eax
-   2e2312a8b:	lea    0x18(%rcx,%rax,1),%r12
-   2e2312a90:	movzwl 0x6(%rcx),%eax
-   2e2312a94:	test   %eax,%eax
-   2e2312a96:	je     0x2e2312ae0
-   2e2312a98:	sub    $0x1,%eax
-   2e2312a9b:	lea    (%rax,%rax,4),%rax
-   2e2312a9f:	lea    0x28(%r12,%rax,8),%rsi
-   2e2312aa4:	jmp    0x2e2312ab9
-   2e2312aa6:	cs nopw 0x0(%rax,%rax,1)
-   2e2312ab0:	add    $0x28,%r12
-   2e2312ab4:	cmp    %rsi,%r12
-   2e2312ab7:	je     0x2e2312ae0
-   2e2312ab9:	mov    $0x8,%r8d
-   2e2312abf:	mov    %rbx,%rdx
-   2e2312ac2:	mov    %r12,%rcx
-   2e2312ac5:	call   0x2e2312f58
-   2e2312aca:	test   %eax,%eax
-   2e2312acc:	jne    0x2e2312ab0
-   2e2312ace:	mov    %r12,%rax
-   2e2312ad1:	add    $0x20,%rsp
-   2e2312ad5:	pop    %rbx
-   2e2312ad6:	pop    %rsi
-   2e2312ad7:	pop    %r12
-   2e2312ad9:	ret
-   2e2312ada:	nopw   0x0(%rax,%rax,1)
-   2e2312ae0:	xor    %r12d,%r12d
-   2e2312ae3:	mov    %r12,%rax
-   2e2312ae6:	add    $0x20,%rsp
-   2e2312aea:	pop    %rbx
-   2e2312aeb:	pop    %rsi
-   2e2312aec:	pop    %r12
-   2e2312aee:	ret
-   2e2312aef:	nop
-   2e2312af0:	sub    $0x28,%rsp
-   2e2312af4:	mov    0x2715(%rip),%r10        # 0x2e2315210
-   2e2312afb:	xor    %r8d,%r8d
-   2e2312afe:	cmpw   $0x5a4d,(%r10)
-   2e2312b04:	mov    %rcx,%r9
-   2e2312b07:	jne    0x2e2312b69
-   2e2312b09:	mov    %r10,%rcx
-   2e2312b0c:	call   0x2e23129c0
-   2e2312b11:	test   %eax,%eax
-   2e2312b13:	je     0x2e2312b69
-   2e2312b15:	movslq 0x3c(%r10),%rax
-   2e2312b19:	mov    %r9,%rcx
-   2e2312b1c:	sub    %r10,%rcx
-   2e2312b1f:	add    %rax,%r10
-   2e2312b22:	movzwl 0x14(%r10),%eax
-   2e2312b27:	lea    0x18(%r10,%rax,1),%r8
-   2e2312b2c:	movzwl 0x6(%r10),%eax
-   2e2312b31:	test   %eax,%eax
-   2e2312b33:	je     0x2e2312b66
-   2e2312b35:	sub    $0x1,%eax
-   2e2312b38:	lea    (%rax,%rax,4),%rax
-   2e2312b3c:	lea    0x28(%r8,%rax,8),%r9
-   2e2312b41:	nopl   0x0(%rax)
-   2e2312b48:	mov    0xc(%r8),%edx
-   2e2312b4c:	mov    %rdx,%rax
-   2e2312b4f:	cmp    %rdx,%rcx
-   2e2312b52:	jb     0x2e2312b5d
-   2e2312b54:	add    0x8(%r8),%eax
-   2e2312b58:	cmp    %rax,%rcx
-   2e2312b5b:	jb     0x2e2312b69
-   2e2312b5d:	add    $0x28,%r8
-   2e2312b61:	cmp    %r9,%r8
-   2e2312b64:	jne    0x2e2312b48
-   2e2312b66:	xor    %r8d,%r8d
-   2e2312b69:	mov    %r8,%rax
-   2e2312b6c:	add    $0x28,%rsp
-   2e2312b70:	ret
-   2e2312b71:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e2311cd0:	movslq 0x8(%rdx),%r9
+   2e2311cd4:	add    $0x1,%eax
+   2e2311cd7:	add    $0x10,%rdx
+   2e2311cdb:	movsd  %xmm0,(%r12,%r9,8)
+   2e2311ce1:	lea    0x1(%r8),%r9d
+   2e2311ce5:	cmp    %r10d,%eax
+   2e2311ce8:	jge    0x2e2311d06
+   2e2311cea:	movslq 0x8(%rdx),%r8
+   2e2311cee:	mov    (%rbx,%r8,4),%ebp
+   2e2311cf2:	mov    %r9d,%r8d
+   2e2311cf5:	test   %ebp,%ebp
+   2e2311cf7:	je     0x2e2311cd0
+   2e2311cf9:	add    $0x10,%rdx
+   2e2311cfd:	lea    0x1(%r8),%r9d
+   2e2311d01:	cmp    %eax,%r10d
+   2e2311d04:	jg     0x2e2311cea
+   2e2311d06:	add    %r10d,%ecx
+   2e2311d09:	add    $0x1,%r8d
+   2e2311d0d:	cmp    %r13d,%r8d
+   2e2311d10:	jl     0x2e2311c35
+   2e2311d16:	mov    0x28(%rsp),%r10d
+   2e2311d1b:	mov    0x50(%rsp),%r14
+   2e2311d20:	mov    0x58(%rsp),%rbp
+   2e2311d25:	mov    0x38(%rsp),%edx
+   2e2311d29:	movsd  0x32d7(%rip),%xmm2        # 0x2e2315008
+   2e2311d31:	xor    %r8d,%r8d
+   2e2311d34:	test   %edx,%edx
+   2e2311d36:	je     0x2e2311e50
+   2e2311d3c:	mov    %r15,0x28(%rsp)
+   2e2311d41:	mov    0xc8(%rsp),%r13
+   2e2311d49:	mov    0x38(%rsp),%r15d
+   2e2311d4e:	mov    %r12,0x38(%rsp)
+   2e2311d53:	jmp    0x2e2311d65
+   2e2311d55:	nopl   (%rax)
+   2e2311d58:	add    $0x1,%r8d
+   2e2311d5c:	cmp    %r15d,%r8d
+   2e2311d5f:	jge    0x2e2311e46
+   2e2311d65:	movslq %r8d,%rax
+   2e2311d68:	mov    %rax,%rdx
+   2e2311d6b:	shl    $0x4,%rdx
+   2e2311d6f:	add    %r14,%rdx
+   2e2311d72:	movslq 0x8(%rdx),%rcx
+   2e2311d76:	mov    (%rbx,%rcx,4),%edi
+   2e2311d79:	test   %edi,%edi
+   2e2311d7b:	jne    0x2e2311d58
+   2e2311d7d:	mov    %r15d,%r12d
+   2e2311d80:	movsd  0x0(%r13,%rcx,8),%xmm0
+   2e2311d87:	xor    %r11d,%r11d
+   2e2311d8a:	xor    %r9d,%r9d
+   2e2311d8d:	sub    %r8d,%r12d
+   2e2311d90:	movslq %r12d,%r12
+   2e2311d93:	add    %rax,%r12
+   2e2311d96:	mov    %rdx,%rax
+   2e2311d99:	shl    $0x4,%r12
+   2e2311d9d:	add    %r14,%r12
+   2e2311da0:	jmp    0x2e2311db0
+   2e2311da2:	nopw   0x0(%rax,%rax,1)
+   2e2311da8:	movslq 0x8(%rax),%rcx
+   2e2311dac:	mov    (%rbx,%rcx,4),%r11d
+   2e2311db0:	movslq 0x8(%rax),%rcx
+   2e2311db4:	test   %r11d,%r11d
+   2e2311db7:	jne    0x2e2311dc8
+   2e2311db9:	ucomisd 0x0(%r13,%rcx,8),%xmm0
+   2e2311dc0:	jp     0x2e2311dd1
+   2e2311dc2:	jne    0x2e2311dd1
+   2e2311dc4:	add    $0x1,%r9d
+   2e2311dc8:	add    $0x10,%rax
+   2e2311dcc:	cmp    %r12,%rax
+   2e2311dcf:	jne    0x2e2311da8
+   2e2311dd1:	lea    -0x1(%r9),%eax
+   2e2311dd5:	pxor   %xmm0,%xmm0
+   2e2311dd9:	pxor   %xmm1,%xmm1
+   2e2311ddd:	cvtsi2sd %eax,%xmm0
+   2e2311de1:	cvtsi2sd %r10d,%xmm1
+   2e2311de6:	mulsd  %xmm2,%xmm0
+   2e2311dea:	addsd  %xmm1,%xmm0
+   2e2311dee:	test   %r9d,%r9d
+   2e2311df1:	je     0x2e23120a1
+   2e2311df7:	xor    %eax,%eax
+   2e2311df9:	jmp    0x2e2311e25
+   2e2311dfb:	nopl   0x0(%rax,%rax,1)
+   2e2311e00:	movslq 0x8(%rdx),%rcx
+   2e2311e04:	add    $0x1,%eax
+   2e2311e07:	add    $0x10,%rdx
+   2e2311e0b:	movsd  %xmm0,0x0(%rbp,%rcx,8)
+   2e2311e11:	lea    0x1(%r8),%ecx
+   2e2311e15:	cmp    %r9d,%eax
+   2e2311e18:	jge    0x2e2311e36
+   2e2311e1a:	movslq 0x8(%rdx),%r8
+   2e2311e1e:	mov    (%rbx,%r8,4),%edi
+   2e2311e22:	mov    %ecx,%r8d
+   2e2311e25:	test   %edi,%edi
+   2e2311e27:	je     0x2e2311e00
+   2e2311e29:	add    $0x10,%rdx
+   2e2311e2d:	lea    0x1(%r8),%ecx
+   2e2311e31:	cmp    %eax,%r9d
+   2e2311e34:	jg     0x2e2311e1a
+   2e2311e36:	add    %r9d,%r10d
+   2e2311e39:	add    $0x1,%r8d
+   2e2311e3d:	cmp    %r15d,%r8d
+   2e2311e40:	jl     0x2e2311d65
+   2e2311e46:	mov    0x28(%rsp),%r15
+   2e2311e4b:	mov    0x38(%rsp),%r12
+   2e2311e50:	mov    0xd0(%rsp),%r8d
+   2e2311e58:	mov    %rbp,%rdx
+   2e2311e5b:	mov    %r12,%rcx
+   2e2311e5e:	call   0x2e2311520
+   2e2311e63:	mov    %r15,%rcx
+   2e2311e66:	movupd %xmm0,%xmm6
+   2e2311e6a:	call   0x2e2313210
+   2e2311e6f:	mov    %r14,%rcx
+   2e2311e72:	call   0x2e2313210
+   2e2311e77:	mov    %r12,%rcx
+   2e2311e7a:	call   0x2e2313210
+   2e2311e7f:	mov    %rbp,%rcx
+   2e2311e82:	call   0x2e2313210
+   2e2311e87:	mov    %rbx,%rcx
+   2e2311e8a:	call   0x2e2313210
+   2e2311e8f:	mov    0x40(%rsp),%rcx
+   2e2311e94:	call   0x2e2313210
+   2e2311e99:	mov    %rsi,%rcx
+   2e2311e9c:	call   0x2e2313210
+   2e2311ea1:	mov    0x48(%rsp),%rcx
+   2e2311ea6:	call   0x2e2313210
+   2e2311eab:	mov    0x30(%rsp),%rcx
+   2e2311eb0:	call   0x2e2313210
+   2e2311eb5:	movupd %xmm6,%xmm0
+   2e2311eb9:	movups 0x60(%rsp),%xmm6
+   2e2311ebe:	add    $0x78,%rsp
+   2e2311ec2:	pop    %rbx
+   2e2311ec3:	pop    %rsi
+   2e2311ec4:	pop    %rdi
+   2e2311ec5:	pop    %rbp
+   2e2311ec6:	pop    %r12
+   2e2311ec8:	pop    %r13
+   2e2311eca:	pop    %r14
+   2e2311ecc:	pop    %r15
+   2e2311ece:	ret
+   2e2311ecf:	mov    0x38(%rsp),%r10d
+   2e2311ed4:	test   %r10d,%r10d
+   2e2311ed7:	jle    0x2e2311ee8
+   2e2311ed9:	xor    %edx,%edx
+   2e2311edb:	test   %al,%al
+   2e2311edd:	jne    0x2e2311b18
+   2e2311ee3:	nopl   0x0(%rax,%rax,1)
+   2e2311ee8:	mov    $0x1,%r10d
+   2e2311eee:	mov    $0x1,%ecx
+   2e2311ef3:	mov    0xd0(%rsp),%r8d
+   2e2311efb:	xor    %eax,%eax
+   2e2311efd:	test   %r8d,%r8d
+   2e2311f00:	jle    0x2e2311c00
+   2e2311f06:	cs nopw 0x0(%rax,%rax,1)
+   2e2311f10:	movsd  0x0(%rbp,%rax,8),%xmm0
+   2e2311f16:	ucomisd %xmm0,%xmm0
+   2e2311f1a:	jp     0x2e2311f49
+   2e2311f1c:	movsd  (%r12,%rax,8),%xmm0
+   2e2311f22:	xor    %edx,%edx
+   2e2311f24:	ucomisd %xmm0,%xmm0
+   2e2311f28:	setp   %dl
+   2e2311f2b:	mov    %edx,(%rbx,%rax,4)
+   2e2311f2e:	add    $0x1,%rax
+   2e2311f32:	cmp    %rax,0x28(%rsp)
+   2e2311f37:	je     0x2e2311c00
+   2e2311f3d:	movsd  0x0(%rbp,%rax,8),%xmm0
+   2e2311f43:	ucomisd %xmm0,%xmm0
+   2e2311f47:	jnp    0x2e2311f1c
+   2e2311f49:	movl   $0x1,(%rbx,%rax,4)
+   2e2311f50:	add    $0x1,%rax
+   2e2311f54:	cmp    %rax,0x28(%rsp)
+   2e2311f59:	jne    0x2e2311f10
+   2e2311f5b:	jmp    0x2e2311c00
+   2e2311f60:	mov    %r13,%rcx
+   2e2311f63:	call   0x2e2313220
+   2e2311f68:	mov    %r13,%rcx
+   2e2311f6b:	mov    %rax,0x48(%rsp)
+   2e2311f70:	call   0x2e2313220
+   2e2311f75:	mov    0xd0(%rsp),%edx
+   2e2311f7c:	mov    %rax,0x30(%rsp)
+   2e2311f81:	test   %edx,%edx
+   2e2311f83:	jle    0x2e23120ad
+   2e2311f89:	mov    0xd0(%rsp),%eax
+   2e2311f90:	mov    %rdi,%rdx
+   2e2311f93:	mov    0x48(%rsp),%rdi
+   2e2311f98:	lea    0x0(,%rax,8),%rsi
+   2e2311fa0:	mov    %rdi,%rcx
+   2e2311fa3:	mov    %rsi,%r8
+   2e2311fa6:	call   0x2e2313228
+   2e2311fab:	mov    0xc8(%rsp),%rdx
+   2e2311fb3:	mov    0x30(%rsp),%rcx
+   2e2311fb8:	mov    %rsi,%r8
+   2e2311fbb:	call   0x2e2313228
+   2e2311fc0:	xor    %eax,%eax
+   2e2311fc2:	xor    %edx,%edx
+   2e2311fc4:	mov    %rdi,%rcx
+   2e2311fc7:	nopw   0x0(%rax,%rax,1)
+   2e2311fd0:	movsd  (%rcx,%rax,1),%xmm0
+   2e2311fd5:	ucomisd %xmm0,%xmm0
+   2e2311fd9:	jp     0x2e2312080
+   2e2311fdf:	mov    0x30(%rsp),%rsi
+   2e2311fe4:	xor    %r8d,%r8d
+   2e2311fe7:	movsd  (%rsi,%rax,1),%xmm0
+   2e2311fec:	ucomisd %xmm0,%xmm0
+   2e2311ff0:	setp   %r8b
+   2e2311ff4:	add    $0x8,%rax
+   2e2311ff8:	add    %r8d,%edx
+   2e2311ffb:	cmp    %rax,%r13
+   2e2311ffe:	jne    0x2e2311fd0
+   2e2312000:	mov    0xd0(%rsp),%eax
+   2e2312007:	mov    0x30(%rsp),%rcx
+   2e231200c:	sub    %edx,%eax
+   2e231200e:	mov    0x48(%rsp),%rdx
+   2e2312013:	mov    %rcx,0xc8(%rsp)
+   2e231201b:	mov    %rdx,%rdi
+   2e231201e:	cmp    $0x9,%eax
+   2e2312021:	jg     0x2e2311903
+   2e2312027:	xor    %eax,%eax
+   2e2312029:	nopl   0x0(%rax)
+   2e2312030:	movsd  (%rcx,%rax,1),%xmm0
+   2e2312035:	ucomisd %xmm0,%xmm0
+   2e2312039:	jnp    0x2e2312043
+   2e231203b:	movq   $0x0,(%rcx,%rax,1)
+   2e2312043:	movsd  (%rdx,%rax,1),%xmm0
+   2e2312048:	ucomisd %xmm0,%xmm0
+   2e231204c:	jnp    0x2e2312056
+   2e231204e:	movq   $0x0,(%rdx,%rax,1)
+   2e2312056:	add    $0x8,%rax
+   2e231205a:	cmp    %rax,%r13
+   2e231205d:	jne    0x2e2312030
+   2e231205f:	mov    0x30(%rsp),%rax
+   2e2312064:	mov    0x48(%rsp),%rdi
+   2e2312069:	mov    %rax,0xc8(%rsp)
+   2e2312071:	jmp    0x2e2311903
+   2e2312076:	cs nopw 0x0(%rax,%rax,1)
+   2e2312080:	add    $0x8,%rax
+   2e2312084:	add    $0x1,%edx
+   2e2312087:	cmp    %rax,%r13
+   2e231208a:	jne    0x2e2311fd0
+   2e2312090:	jmp    0x2e2312000
+   2e2312095:	sub    $0x1,%r8d
+   2e2312099:	add    %r10d,%ecx
+   2e231209c:	jmp    0x2e2311d09
+   2e23120a1:	sub    $0x1,%r8d
+   2e23120a5:	add    %r9d,%r10d
+   2e23120a8:	jmp    0x2e2311e39
+   2e23120ad:	mov    %rax,0xc8(%rsp)
+   2e23120b5:	mov    0x48(%rsp),%rdi
+   2e23120ba:	movq   $0x0,0x40(%rsp)
+   2e23120c3:	xor    %esi,%esi
+   2e23120c5:	xor    %edx,%edx
+   2e23120c7:	xor    %r11d,%r11d
+   2e23120ca:	movl   $0x0,0x38(%rsp)
+   2e23120d2:	xor    %r13d,%r13d
+   2e23120d5:	jmp    0x2e2311a39
+   2e23120da:	mov    $0x1,%ecx
+   2e23120df:	jmp    0x2e2311bad
+   2e23120e4:	mov    $0x1,%r10d
+   2e23120ea:	jmp    0x2e2311ef3
+   2e23120ef:	nop
+   2e23120f0:	mov    %r9d,%eax
+   2e23120f3:	mov    0x28(%rsp),%r9d
+   2e23120f8:	imul   %eax,%r8d
+   2e23120fc:	imul   %eax,%edx
+   2e23120ff:	movslq %r8d,%r8
+   2e2312102:	movslq %edx,%rdx
+   2e2312105:	lea    (%rcx,%r8,8),%r10
+   2e2312109:	mov    %eax,%r8d
+   2e231210c:	lea    (%rcx,%rdx,8),%rcx
+   2e2312110:	mov    0x30(%rsp),%edx
+   2e2312114:	mov    %edx,0x28(%rsp)
+   2e2312118:	mov    %r10,%rdx
+   2e231211b:	jmp    0x2e2311850
+   2e2312120:	imul   %r9d,%r8d
+   2e2312124:	imul   %r9d,%edx
+   2e2312128:	movslq %r8d,%r8
+   2e231212b:	lea    (%rcx,%r8,8),%rax
+   2e231212f:	movslq %edx,%rdx
+   2e2312132:	mov    %r9d,%r8d
+   2e2312135:	lea    (%rcx,%rdx,8),%rcx
+   2e2312139:	mov    %rax,%rdx
+   2e231213c:	jmp    0x2e2311520
+   2e2312141:	nop
+   2e2312142:	nop
+   2e2312143:	nop
+   2e2312144:	nop
+   2e2312145:	nop
+   2e2312146:	nop
+   2e2312147:	nop
+   2e2312148:	nop
+   2e2312149:	nop
+   2e231214a:	nop
+   2e231214b:	nop
+   2e231214c:	nop
+   2e231214d:	nop
+   2e231214e:	nop
+   2e231214f:	nop
+   2e2312150:	sub    $0x28,%rsp
+   2e2312154:	mov    0x1eb5(%rip),%rax        # 0x2e2314010
+   2e231215b:	mov    (%rax),%rax
+   2e231215e:	test   %rax,%rax
+   2e2312161:	je     0x2e2312185
+   2e2312163:	nopl   0x0(%rax,%rax,1)
+   2e2312168:	call   *%rax
+   2e231216a:	mov    0x1e9f(%rip),%rax        # 0x2e2314010
+   2e2312171:	lea    0x8(%rax),%rdx
+   2e2312175:	mov    0x8(%rax),%rax
+   2e2312179:	mov    %rdx,0x1e90(%rip)        # 0x2e2314010
+   2e2312180:	test   %rax,%rax
+   2e2312183:	jne    0x2e2312168
+   2e2312185:	add    $0x28,%rsp
+   2e2312189:	ret
+   2e231218a:	nopw   0x0(%rax,%rax,1)
+   2e2312190:	push   %rsi
+   2e2312191:	push   %rbx
+   2e2312192:	sub    $0x28,%rsp
+   2e2312196:	mov    0x3083(%rip),%rdx        # 0x2e2315220
+   2e231219d:	mov    (%rdx),%rax
+   2e23121a0:	mov    %eax,%ecx
+   2e23121a2:	cmp    $0xffffffff,%eax
+   2e23121a5:	je     0x2e23121e0
+   2e23121a7:	test   %ecx,%ecx
+   2e23121a9:	je     0x2e23121cb
+   2e23121ab:	mov    %ecx,%eax
+   2e23121ad:	sub    $0x1,%ecx
+   2e23121b0:	lea    (%rdx,%rax,8),%rbx
+   2e23121b4:	sub    %rcx,%rax
+   2e23121b7:	lea    -0x8(%rdx,%rax,8),%rsi
+   2e23121bc:	nopl   0x0(%rax)
+   2e23121c0:	call   *(%rbx)
+   2e23121c2:	sub    $0x8,%rbx
+   2e23121c6:	cmp    %rsi,%rbx
+   2e23121c9:	jne    0x2e23121c0
+   2e23121cb:	lea    -0x82(%rip),%rcx        # 0x2e2312150
+   2e23121d2:	add    $0x28,%rsp
+   2e23121d6:	pop    %rbx
+   2e23121d7:	pop    %rsi
+   2e23121d8:	jmp    0x2e2311340
+   2e23121dd:	nopl   (%rax)
+   2e23121e0:	xor    %eax,%eax
+   2e23121e2:	nopw   0x0(%rax,%rax,1)
+   2e23121e8:	lea    0x1(%rax),%r8d
+   2e23121ec:	mov    %eax,%ecx
+   2e23121ee:	cmpq   $0x0,(%rdx,%r8,8)
+   2e23121f3:	mov    %r8,%rax
+   2e23121f6:	jne    0x2e23121e8
+   2e23121f8:	jmp    0x2e23121a7
+   2e23121fa:	nopw   0x0(%rax,%rax,1)
+   2e2312200:	mov    0x5e1a(%rip),%eax        # 0x2e2318020
+   2e2312206:	test   %eax,%eax
+   2e2312208:	je     0x2e2312210
+   2e231220a:	ret
+   2e231220b:	nopl   0x0(%rax,%rax,1)
+   2e2312210:	movl   $0x1,0x5e06(%rip)        # 0x2e2318020
+   2e231221a:	jmp    0x2e2312190
+   2e231221f:	nop
+   2e2312220:	sub    $0x28,%rsp
+   2e2312224:	cmp    $0x3,%edx
+   2e2312227:	je     0x2e2312240
+   2e2312229:	test   %edx,%edx
+   2e231222b:	je     0x2e2312240
+   2e231222d:	mov    $0x1,%eax
+   2e2312232:	add    $0x28,%rsp
+   2e2312236:	ret
+   2e2312237:	nopw   0x0(%rax,%rax,1)
+   2e2312240:	call   0x2e23129a0
+   2e2312245:	mov    $0x1,%eax
+   2e231224a:	add    $0x28,%rsp
+   2e231224e:	ret
+   2e231224f:	nop
+   2e2312250:	push   %rsi
+   2e2312251:	push   %rbx
+   2e2312252:	sub    $0x28,%rsp
+   2e2312256:	mov    0x2fb3(%rip),%rax        # 0x2e2315210
+   2e231225d:	cmpl   $0x2,(%rax)
+   2e2312260:	je     0x2e2312268
+   2e2312262:	movl   $0x2,(%rax)
+   2e2312268:	cmp    $0x2,%edx
+   2e231226b:	je     0x2e2312280
+   2e231226d:	cmp    $0x1,%edx
+   2e2312270:	je     0x2e23122c0
+   2e2312272:	mov    $0x1,%eax
+   2e2312277:	add    $0x28,%rsp
+   2e231227b:	pop    %rbx
+   2e231227c:	pop    %rsi
+   2e231227d:	ret
+   2e231227e:	xchg   %ax,%ax
+   2e2312280:	lea    0x8dc9(%rip),%rbx        # 0x2e231b050
+   2e2312287:	lea    0x8dc2(%rip),%rsi        # 0x2e231b050
+   2e231228e:	cmp    %rbx,%rsi
+   2e2312291:	je     0x2e2312272
+   2e2312293:	nopl   0x0(%rax,%rax,1)
+   2e2312298:	mov    (%rbx),%rax
+   2e231229b:	test   %rax,%rax
+   2e231229e:	je     0x2e23122a2
+   2e23122a0:	call   *%rax
+   2e23122a2:	add    $0x8,%rbx
+   2e23122a6:	cmp    %rbx,%rsi
+   2e23122a9:	jne    0x2e2312298
+   2e23122ab:	mov    $0x1,%eax
+   2e23122b0:	add    $0x28,%rsp
+   2e23122b4:	pop    %rbx
+   2e23122b5:	pop    %rsi
+   2e23122b6:	ret
+   2e23122b7:	nopw   0x0(%rax,%rax,1)
+   2e23122c0:	call   0x2e23129a0
+   2e23122c5:	mov    $0x1,%eax
+   2e23122ca:	add    $0x28,%rsp
+   2e23122ce:	pop    %rbx
+   2e23122cf:	pop    %rsi
+   2e23122d0:	ret
+   2e23122d1:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e23122dc:	nopl   0x0(%rax)
+   2e23122e0:	xor    %eax,%eax
+   2e23122e2:	ret
+   2e23122e3:	nop
+   2e23122e4:	nop
+   2e23122e5:	nop
+   2e23122e6:	nop
+   2e23122e7:	nop
+   2e23122e8:	nop
+   2e23122e9:	nop
+   2e23122ea:	nop
+   2e23122eb:	nop
+   2e23122ec:	nop
+   2e23122ed:	nop
+   2e23122ee:	nop
+   2e23122ef:	nop
+   2e23122f0:	push   %rsi
+   2e23122f1:	push   %rbx
+   2e23122f2:	sub    $0x38,%rsp
+   2e23122f6:	mov    %rcx,%rbx
+   2e23122f9:	lea    0x58(%rsp),%rax
+   2e23122fe:	mov    $0x2,%ecx
+   2e2312303:	mov    %rdx,0x58(%rsp)
+   2e2312308:	mov    %r8,0x60(%rsp)
+   2e231230d:	mov    %r9,0x68(%rsp)
+   2e2312312:	mov    %rax,0x28(%rsp)
+   2e2312317:	call   0x2e2313050
+   2e231231c:	mov    $0x1b,%r8d
+   2e2312322:	mov    $0x1,%edx
+   2e2312327:	lea    0x2d52(%rip),%rcx        # 0x2e2315080
+   2e231232e:	mov    %rax,%r9
+   2e2312331:	call   0x2e2313218
+   2e2312336:	mov    0x28(%rsp),%rsi
+   2e231233b:	mov    $0x2,%ecx
+   2e2312340:	call   0x2e2313050
+   2e2312345:	mov    %rbx,%rdx
+   2e2312348:	mov    %rax,%rcx
+   2e231234b:	mov    %rsi,%r8
+   2e231234e:	call   0x2e2313250
+   2e2312353:	call   0x2e2313200
+   2e2312358:	nop
+   2e2312359:	nopl   0x0(%rax)
+   2e2312360:	push   %rdi
+   2e2312361:	push   %rsi
+   2e2312362:	push   %rbx
+   2e2312363:	sub    $0x50,%rsp
+   2e2312367:	movslq 0x5cf6(%rip),%rsi        # 0x2e2318064
+   2e231236e:	mov    %rcx,%rbx
+   2e2312371:	test   %esi,%esi
+   2e2312373:	jle    0x2e2312490
+   2e2312379:	mov    0x5ce8(%rip),%rax        # 0x2e2318068
+   2e2312380:	xor    %r9d,%r9d
+   2e2312383:	add    $0x18,%rax
+   2e2312387:	nopw   0x0(%rax,%rax,1)
+   2e2312390:	mov    (%rax),%r8
+   2e2312393:	cmp    %r8,%rbx
+   2e2312396:	jb     0x2e23123ab
+   2e2312398:	mov    0x8(%rax),%rdx
+   2e231239c:	mov    0x8(%rdx),%edx
+   2e231239f:	add    %rdx,%r8
+   2e23123a2:	cmp    %r8,%rbx
+   2e23123a5:	jb     0x2e2312435
+   2e23123ab:	add    $0x1,%r9d
+   2e23123af:	add    $0x28,%rax
+   2e23123b3:	cmp    %esi,%r9d
+   2e23123b6:	jne    0x2e2312390
+   2e23123b8:	mov    %rbx,%rcx
+   2e23123bb:	call   0x2e2312bc0
+   2e23123c0:	mov    %rax,%rdi
+   2e23123c3:	test   %rax,%rax
+   2e23123c6:	je     0x2e23124b2
+   2e23123cc:	mov    0x5c95(%rip),%rax        # 0x2e2318068
+   2e23123d3:	lea    (%rsi,%rsi,4),%rbx
+   2e23123d7:	shl    $0x3,%rbx
+   2e23123db:	add    %rbx,%rax
+   2e23123de:	mov    %rdi,0x20(%rax)
+   2e23123e2:	movl   $0x0,(%rax)
+   2e23123e8:	call   0x2e2312d00
+   2e23123ed:	mov    0xc(%rdi),%edx
+   2e23123f0:	mov    $0x30,%r8d
+   2e23123f6:	lea    (%rax,%rdx,1),%rcx
+   2e23123fa:	mov    0x5c67(%rip),%rax        # 0x2e2318068
+   2e2312401:	lea    0x20(%rsp),%rdx
+   2e2312406:	mov    %rcx,0x18(%rax,%rbx,1)
+   2e231240b:	call   *0x7d57(%rip)        # 0x2e231a168
+   2e2312411:	test   %rax,%rax
+   2e2312414:	je     0x2e2312497
+   2e231241a:	mov    0x44(%rsp),%eax
+   2e231241e:	lea    -0x40(%rax),%edx
+   2e2312421:	and    $0xffffffbf,%edx
+   2e2312424:	je     0x2e231242e
+   2e2312426:	lea    -0x4(%rax),%edx
+   2e2312429:	and    $0xfffffffb,%edx
+   2e231242c:	jne    0x2e2312440
+   2e231242e:	addl   $0x1,0x5c2f(%rip)        # 0x2e2318064
+   2e2312435:	add    $0x50,%rsp
+   2e2312439:	pop    %rbx
+   2e231243a:	pop    %rsi
+   2e231243b:	pop    %rdi
+   2e231243c:	ret
+   2e231243d:	nopl   (%rax)
+   2e2312440:	cmp    $0x2,%eax
+   2e2312443:	mov    0x20(%rsp),%rcx
+   2e2312448:	mov    0x38(%rsp),%rdx
+   2e231244d:	mov    $0x40,%r8d
+   2e2312453:	mov    $0x4,%eax
+   2e2312458:	cmove  %eax,%r8d
+   2e231245c:	add    0x5c05(%rip),%rbx        # 0x2e2318068
+   2e2312463:	mov    %rcx,0x8(%rbx)
+   2e2312467:	mov    %rbx,%r9
+   2e231246a:	mov    %rdx,0x10(%rbx)
+   2e231246e:	call   *0x7cec(%rip)        # 0x2e231a160
+   2e2312474:	test   %eax,%eax
+   2e2312476:	jne    0x2e231242e
+   2e2312478:	call   *0x7cba(%rip)        # 0x2e231a138
+   2e231247e:	lea    0x2c73(%rip),%rcx        # 0x2e23150f8
+   2e2312485:	mov    %eax,%edx
+   2e2312487:	call   0x2e23122f0
+   2e231248c:	nopl   0x0(%rax)
+   2e2312490:	xor    %esi,%esi
+   2e2312492:	jmp    0x2e23123b8
+   2e2312497:	mov    0x5bca(%rip),%rax        # 0x2e2318068
+   2e231249e:	mov    0x8(%rdi),%edx
+   2e23124a1:	lea    0x2c18(%rip),%rcx        # 0x2e23150c0
+   2e23124a8:	mov    0x18(%rax,%rbx,1),%r8
+   2e23124ad:	call   0x2e23122f0
+   2e23124b2:	mov    %rbx,%rdx
+   2e23124b5:	lea    0x2be4(%rip),%rcx        # 0x2e23150a0
+   2e23124bc:	call   0x2e23122f0
+   2e23124c1:	nop
+   2e23124c2:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e23124cd:	nopl   (%rax)
+   2e23124d0:	push   %rbp
+   2e23124d1:	push   %r15
+   2e23124d3:	push   %r14
+   2e23124d5:	push   %r13
+   2e23124d7:	push   %r12
+   2e23124d9:	push   %rdi
+   2e23124da:	push   %rsi
+   2e23124db:	push   %rbx
+   2e23124dc:	sub    $0x48,%rsp
+   2e23124e0:	lea    0x40(%rsp),%rbp
+   2e23124e5:	mov    0x5b74(%rip),%r12d        # 0x2e2318060
+   2e23124ec:	test   %r12d,%r12d
+   2e23124ef:	je     0x2e2312508
+   2e23124f1:	lea    0x8(%rbp),%rsp
+   2e23124f5:	pop    %rbx
+   2e23124f6:	pop    %rsi
+   2e23124f7:	pop    %rdi
+   2e23124f8:	pop    %r12
+   2e23124fa:	pop    %r13
+   2e23124fc:	pop    %r14
+   2e23124fe:	pop    %r15
+   2e2312500:	pop    %rbp
+   2e2312501:	ret
+   2e2312502:	nopw   0x0(%rax,%rax,1)
+   2e2312508:	movl   $0x1,0x5b4e(%rip)        # 0x2e2318060
+   2e2312512:	call   0x2e2312c40
+   2e2312517:	cltq
+   2e2312519:	lea    (%rax,%rax,4),%rax
+   2e231251d:	lea    0xf(,%rax,8),%rax
+   2e2312525:	and    $0xfffffffffffffff0,%rax
+   2e2312529:	call   0x2e2312eb0
+   2e231252e:	mov    0x2cfb(%rip),%r13        # 0x2e2315230
+   2e2312535:	mov    0x2d04(%rip),%rbx        # 0x2e2315240
+   2e231253c:	movl   $0x0,0x5b1e(%rip)        # 0x2e2318064
+   2e2312546:	sub    %rax,%rsp
+   2e2312549:	lea    0x30(%rsp),%rax
+   2e231254e:	mov    %rax,0x5b13(%rip)        # 0x2e2318068
+   2e2312555:	mov    %r13,%rax
+   2e2312558:	sub    %rbx,%rax
+   2e231255b:	cmp    $0x7,%rax
+   2e231255f:	jle    0x2e23124f1
+   2e2312561:	mov    (%rbx),%edx
+   2e2312563:	cmp    $0xb,%rax
+   2e2312567:	jg     0x2e23126e8
+   2e231256d:	mov    (%rbx),%eax
+   2e231256f:	test   %eax,%eax
+   2e2312571:	jne    0x2e23127e0
+   2e2312577:	mov    0x4(%rbx),%eax
+   2e231257a:	test   %eax,%eax
+   2e231257c:	jne    0x2e23127e0
+   2e2312582:	mov    0x8(%rbx),%edx
+   2e2312585:	cmp    $0x1,%edx
+   2e2312588:	jne    0x2e231281e
+   2e231258e:	add    $0xc,%rbx
+   2e2312592:	cmp    %r13,%rbx
+   2e2312595:	jae    0x2e23124f1
+   2e231259b:	mov    0x2cbe(%rip),%r14        # 0x2e2315260
+   2e23125a2:	movabs $0xffffffff7fffffff,%r15
+   2e23125ac:	jmp    0x2e2312602
+   2e23125ae:	xchg   %ax,%ax
+   2e23125b0:	movzbl (%rdi),%esi
+   2e23125b3:	and    $0xc0,%ecx
+   2e23125b9:	test   %sil,%sil
+   2e23125bc:	jns    0x2e23127c8
+   2e23125c2:	or     $0xffffffffffffff00,%rsi
+   2e23125c9:	sub    %rax,%rsi
+   2e23125cc:	add    %r9,%rsi
+   2e23125cf:	test   %ecx,%ecx
+   2e23125d1:	jne    0x2e23125ea
+   2e23125d3:	cmp    $0xff,%rsi
+   2e23125da:	jg     0x2e231272f
+   2e23125e0:	cmp    $0xffffffffffffff80,%rsi
+   2e23125e4:	jl     0x2e231272f
+   2e23125ea:	mov    %rdi,%rcx
+   2e23125ed:	call   0x2e2312360
+   2e23125f2:	mov    %sil,(%rdi)
+   2e23125f5:	add    $0xc,%rbx
+   2e23125f9:	cmp    %r13,%rbx
+   2e23125fc:	jae    0x2e2312690
+   2e2312602:	mov    (%rbx),%eax
+   2e2312604:	mov    0x8(%rbx),%ecx
+   2e2312607:	mov    0x4(%rbx),%edi
+   2e231260a:	add    %r14,%rax
+   2e231260d:	movzbl %cl,%edx
+   2e2312610:	mov    (%rax),%r9
+   2e2312613:	add    %r14,%rdi
+   2e2312616:	cmp    $0x20,%edx
+   2e2312619:	je     0x2e2312748
+   2e231261f:	ja     0x2e2312710
+   2e2312625:	cmp    $0x8,%edx
+   2e2312628:	je     0x2e23125b0
+   2e231262a:	cmp    $0x10,%edx
+   2e231262d:	jne    0x2e2312812
+   2e2312633:	movzwl (%rdi),%esi
+   2e2312636:	and    $0xc0,%ecx
+   2e231263c:	test   %si,%si
+   2e231263f:	jns    0x2e23127b0
+   2e2312645:	or     $0xffffffffffff0000,%rsi
+   2e231264c:	sub    %rax,%rsi
+   2e231264f:	add    %r9,%rsi
+   2e2312652:	test   %ecx,%ecx
+   2e2312654:	jne    0x2e2312670
+   2e2312656:	cmp    $0xffffffffffff8000,%rsi
+   2e231265d:	jl     0x2e231272f
+   2e2312663:	cmp    $0xffff,%rsi
+   2e231266a:	jg     0x2e231272f
+   2e2312670:	mov    %rdi,%rcx
+   2e2312673:	add    $0xc,%rbx
+   2e2312677:	call   0x2e2312360
+   2e231267c:	mov    %si,(%rdi)
+   2e231267f:	cmp    %r13,%rbx
+   2e2312682:	jb     0x2e2312602
+   2e2312688:	nopl   0x0(%rax,%rax,1)
+   2e2312690:	mov    0x59ce(%rip),%edx        # 0x2e2318064
+   2e2312696:	test   %edx,%edx
+   2e2312698:	jle    0x2e23124f1
+   2e231269e:	mov    0x7abb(%rip),%rsi        # 0x2e231a160
+   2e23126a5:	xor    %ebx,%ebx
+   2e23126a7:	lea    -0x4(%rbp),%rdi
+   2e23126ab:	nopl   0x0(%rax,%rax,1)
+   2e23126b0:	mov    0x59b1(%rip),%rax        # 0x2e2318068
+   2e23126b7:	add    %rbx,%rax
+   2e23126ba:	mov    (%rax),%r8d
+   2e23126bd:	test   %r8d,%r8d
+   2e23126c0:	je     0x2e23126cf
+   2e23126c2:	mov    0x10(%rax),%rdx
+   2e23126c6:	mov    0x8(%rax),%rcx
+   2e23126ca:	mov    %rdi,%r9
+   2e23126cd:	call   *%rsi
+   2e23126cf:	add    $0x1,%r12d
+   2e23126d3:	add    $0x28,%rbx
+   2e23126d7:	cmp    0x5986(%rip),%r12d        # 0x2e2318064
+   2e23126de:	jl     0x2e23126b0
+   2e23126e0:	jmp    0x2e23124f1
+   2e23126e5:	nopl   (%rax)
+   2e23126e8:	test   %edx,%edx
+   2e23126ea:	jne    0x2e23127e0
+   2e23126f0:	mov    0x4(%rbx),%eax
+   2e23126f3:	mov    %eax,%edx
+   2e23126f5:	or     0x8(%rbx),%edx
+   2e23126f8:	jne    0x2e231257a
+   2e23126fe:	add    $0xc,%rbx
+   2e2312702:	jmp    0x2e231256d
+   2e2312707:	nopw   0x0(%rax,%rax,1)
+   2e2312710:	cmp    $0x40,%edx
+   2e2312713:	jne    0x2e2312812
+   2e2312719:	mov    (%rdi),%rsi
+   2e231271c:	sub    %rax,%rsi
+   2e231271f:	add    %r9,%rsi
+   2e2312722:	and    $0xc0,%ecx
+   2e2312728:	jne    0x2e2312790
+   2e231272a:	test   %rsi,%rsi
+   2e231272d:	js     0x2e2312790
+   2e231272f:	mov    %rsi,0x20(%rsp)
+   2e2312734:	mov    %rdi,%r8
+   2e2312737:	lea    0x2a4a(%rip),%rcx        # 0x2e2315188
+   2e231273e:	call   0x2e23122f0
+   2e2312743:	nopl   0x0(%rax,%rax,1)
+   2e2312748:	mov    (%rdi),%esi
+   2e231274a:	and    $0xc0,%ecx
+   2e2312750:	test   %esi,%esi
+   2e2312752:	jns    0x2e23127a0
+   2e2312754:	movabs $0xffffffff00000000,%r11
+   2e231275e:	or     %r11,%rsi
+   2e2312761:	sub    %rax,%rsi
+   2e2312764:	add    %r9,%rsi
+   2e2312767:	test   %ecx,%ecx
+   2e2312769:	jne    0x2e231277a
+   2e231276b:	cmp    %r15,%rsi
+   2e231276e:	jle    0x2e231272f
+   2e2312770:	mov    $0xffffffff,%eax
+   2e2312775:	cmp    %rax,%rsi
+   2e2312778:	jg     0x2e231272f
+   2e231277a:	mov    %rdi,%rcx
+   2e231277d:	call   0x2e2312360
+   2e2312782:	mov    %esi,(%rdi)
+   2e2312784:	jmp    0x2e23125f5
+   2e2312789:	nopl   0x0(%rax)
+   2e2312790:	mov    %rdi,%rcx
+   2e2312793:	call   0x2e2312360
+   2e2312798:	mov    %rsi,(%rdi)
+   2e231279b:	jmp    0x2e23125f5
+   2e23127a0:	sub    %rax,%rsi
+   2e23127a3:	add    %r9,%rsi
+   2e23127a6:	test   %ecx,%ecx
+   2e23127a8:	je     0x2e231276b
+   2e23127aa:	jmp    0x2e231277a
+   2e23127ac:	nopl   0x0(%rax)
+   2e23127b0:	sub    %rax,%rsi
+   2e23127b3:	add    %r9,%rsi
+   2e23127b6:	test   %ecx,%ecx
+   2e23127b8:	je     0x2e2312656
+   2e23127be:	jmp    0x2e2312670
+   2e23127c3:	nopl   0x0(%rax,%rax,1)
+   2e23127c8:	sub    %rax,%rsi
+   2e23127cb:	add    %r9,%rsi
+   2e23127ce:	test   %ecx,%ecx
+   2e23127d0:	je     0x2e23125d3
+   2e23127d6:	jmp    0x2e23125ea
+   2e23127db:	nopl   0x0(%rax,%rax,1)
+   2e23127e0:	cmp    %r13,%rbx
+   2e23127e3:	jae    0x2e23124f1
+   2e23127e9:	mov    0x2a70(%rip),%r14        # 0x2e2315260
+   2e23127f0:	mov    0x4(%rbx),%esi
+   2e23127f3:	mov    (%rbx),%edi
+   2e23127f5:	add    $0x8,%rbx
+   2e23127f9:	add    %r14,%rsi
+   2e23127fc:	add    (%rsi),%edi
+   2e23127fe:	mov    %rsi,%rcx
+   2e2312801:	call   0x2e2312360
+   2e2312806:	mov    %edi,(%rsi)
+   2e2312808:	cmp    %r13,%rbx
+   2e231280b:	jb     0x2e23127f0
+   2e231280d:	jmp    0x2e2312690
+   2e2312812:	lea    0x293f(%rip),%rcx        # 0x2e2315158
+   2e2312819:	call   0x2e23122f0
+   2e231281e:	lea    0x28fb(%rip),%rcx        # 0x2e2315120
+   2e2312825:	call   0x2e23122f0
+   2e231282a:	nop
+   2e231282b:	nop
+   2e231282c:	nop
+   2e231282d:	nop
+   2e231282e:	nop
+   2e231282f:	nop
+   2e2312830:	push   %r12
+   2e2312832:	push   %rbp
+   2e2312833:	push   %rdi
+   2e2312834:	push   %rsi
+   2e2312835:	push   %rbx
+   2e2312836:	sub    $0x20,%rsp
+   2e231283a:	lea    0x585f(%rip),%r12        # 0x2e23180a0
+   2e2312841:	mov    %r12,%rcx
+   2e2312844:	call   *0x78e6(%rip)        # 0x2e231a130
+   2e231284a:	mov    0x582f(%rip),%rbx        # 0x2e2318080
+   2e2312851:	test   %rbx,%rbx
+   2e2312854:	je     0x2e231288c
+   2e2312856:	mov    0x78fb(%rip),%rbp        # 0x2e231a158
+   2e231285d:	mov    0x78d4(%rip),%rdi        # 0x2e231a138
+   2e2312864:	nopl   0x0(%rax)
+   2e2312868:	mov    (%rbx),%ecx
+   2e231286a:	call   *%rbp
+   2e231286c:	mov    %rax,%rsi
+   2e231286f:	call   *%rdi
+   2e2312871:	test   %eax,%eax
+   2e2312873:	jne    0x2e2312883
+   2e2312875:	test   %rsi,%rsi
+   2e2312878:	je     0x2e2312883
+   2e231287a:	mov    0x8(%rbx),%rax
+   2e231287e:	mov    %rsi,%rcx
+   2e2312881:	call   *%rax
+   2e2312883:	mov    0x10(%rbx),%rbx
+   2e2312887:	test   %rbx,%rbx
+   2e231288a:	jne    0x2e2312868
+   2e231288c:	mov    %r12,%rcx
+   2e231288f:	add    $0x20,%rsp
+   2e2312893:	pop    %rbx
+   2e2312894:	pop    %rsi
+   2e2312895:	pop    %rdi
+   2e2312896:	pop    %rbp
+   2e2312897:	pop    %r12
+   2e2312899:	rex.W jmp *0x78a8(%rip)        # 0x2e231a148
+   2e23128a0:	push   %rdi
+   2e23128a1:	push   %rsi
+   2e23128a2:	push   %rbx
+   2e23128a3:	sub    $0x20,%rsp
+   2e23128a7:	mov    0x57db(%rip),%eax        # 0x2e2318088
+   2e23128ad:	mov    %ecx,%edi
+   2e23128af:	mov    %rdx,%rsi
+   2e23128b2:	test   %eax,%eax
+   2e23128b4:	jne    0x2e23128c0
+   2e23128b6:	xor    %eax,%eax
+   2e23128b8:	add    $0x20,%rsp
+   2e23128bc:	pop    %rbx
+   2e23128bd:	pop    %rsi
+   2e23128be:	pop    %rdi
+   2e23128bf:	ret
+   2e23128c0:	mov    $0x18,%edx
+   2e23128c5:	mov    $0x1,%ecx
+   2e23128ca:	call   0x2e2313208
+   2e23128cf:	mov    %rax,%rbx
+   2e23128d2:	test   %rax,%rax
+   2e23128d5:	je     0x2e231290a
+   2e23128d7:	mov    %rsi,0x8(%rax)
+   2e23128db:	lea    0x57be(%rip),%rsi        # 0x2e23180a0
+   2e23128e2:	mov    %edi,(%rax)
+   2e23128e4:	mov    %rsi,%rcx
+   2e23128e7:	call   *0x7843(%rip)        # 0x2e231a130
+   2e23128ed:	mov    0x578c(%rip),%rax        # 0x2e2318080
+   2e23128f4:	mov    %rsi,%rcx
+   2e23128f7:	mov    %rbx,0x5782(%rip)        # 0x2e2318080
+   2e23128fe:	mov    %rax,0x10(%rbx)
+   2e2312902:	call   *0x7840(%rip)        # 0x2e231a148
+   2e2312908:	jmp    0x2e23128b6
+   2e231290a:	or     $0xffffffff,%eax
+   2e231290d:	jmp    0x2e23128b8
+   2e231290f:	nop
+   2e2312910:	push   %rsi
+   2e2312911:	push   %rbx
+   2e2312912:	sub    $0x28,%rsp
+   2e2312916:	mov    0x576c(%rip),%eax        # 0x2e2318088
+   2e231291c:	mov    %ecx,%ebx
+   2e231291e:	test   %eax,%eax
+   2e2312920:	jne    0x2e2312930
+   2e2312922:	xor    %eax,%eax
+   2e2312924:	add    $0x28,%rsp
+   2e2312928:	pop    %rbx
+   2e2312929:	pop    %rsi
+   2e231292a:	ret
+   2e231292b:	nopl   0x0(%rax,%rax,1)
+   2e2312930:	lea    0x5769(%rip),%rsi        # 0x2e23180a0
+   2e2312937:	mov    %rsi,%rcx
+   2e231293a:	call   *0x77f0(%rip)        # 0x2e231a130
+   2e2312940:	mov    0x5739(%rip),%rcx        # 0x2e2318080
+   2e2312947:	test   %rcx,%rcx
+   2e231294a:	je     0x2e2312973
+   2e231294c:	xor    %edx,%edx
+   2e231294e:	jmp    0x2e231295b
+   2e2312950:	mov    %rcx,%rdx
+   2e2312953:	test   %rax,%rax
+   2e2312956:	je     0x2e2312973
+   2e2312958:	mov    %rax,%rcx
+   2e231295b:	mov    (%rcx),%eax
+   2e231295d:	cmp    %ebx,%eax
+   2e231295f:	mov    0x10(%rcx),%rax
+   2e2312963:	jne    0x2e2312950
+   2e2312965:	test   %rdx,%rdx
+   2e2312968:	je     0x2e2312988
+   2e231296a:	mov    %rax,0x10(%rdx)
+   2e231296e:	call   0x2e2313210
+   2e2312973:	mov    %rsi,%rcx
+   2e2312976:	call   *0x77cc(%rip)        # 0x2e231a148
+   2e231297c:	xor    %eax,%eax
+   2e231297e:	add    $0x28,%rsp
+   2e2312982:	pop    %rbx
+   2e2312983:	pop    %rsi
+   2e2312984:	ret
+   2e2312985:	nopl   (%rax)
+   2e2312988:	mov    %rax,0x56f1(%rip)        # 0x2e2318080
+   2e231298f:	jmp    0x2e231296e
+   2e2312991:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e231299c:	nopl   0x0(%rax)
+   2e23129a0:	push   %rbx
+   2e23129a1:	sub    $0x20,%rsp
+   2e23129a5:	cmp    $0x2,%edx
+   2e23129a8:	je     0x2e2312a60
+   2e23129ae:	ja     0x2e23129e0
+   2e23129b0:	test   %edx,%edx
+   2e23129b2:	je     0x2e2312a00
+   2e23129b4:	mov    0x56ce(%rip),%eax        # 0x2e2318088
+   2e23129ba:	test   %eax,%eax
+   2e23129bc:	je     0x2e2312a80
+   2e23129c2:	movl   $0x1,0x56bc(%rip)        # 0x2e2318088
+   2e23129cc:	mov    $0x1,%eax
+   2e23129d1:	add    $0x20,%rsp
+   2e23129d5:	pop    %rbx
+   2e23129d6:	ret
+   2e23129d7:	nopw   0x0(%rax,%rax,1)
+   2e23129e0:	cmp    $0x3,%edx
+   2e23129e3:	jne    0x2e23129cc
+   2e23129e5:	mov    0x569d(%rip),%eax        # 0x2e2318088
+   2e23129eb:	test   %eax,%eax
+   2e23129ed:	je     0x2e23129cc
+   2e23129ef:	call   0x2e2312830
+   2e23129f4:	jmp    0x2e23129cc
+   2e23129f6:	cs nopw 0x0(%rax,%rax,1)
+   2e2312a00:	mov    0x5682(%rip),%eax        # 0x2e2318088
+   2e2312a06:	test   %eax,%eax
+   2e2312a08:	jne    0x2e2312a70
+   2e2312a0a:	mov    0x5678(%rip),%eax        # 0x2e2318088
+   2e2312a10:	cmp    $0x1,%eax
+   2e2312a13:	jne    0x2e23129cc
+   2e2312a15:	mov    0x5664(%rip),%rbx        # 0x2e2318080
+   2e2312a1c:	test   %rbx,%rbx
+   2e2312a1f:	je     0x2e2312a39
+   2e2312a21:	nopl   0x0(%rax)
+   2e2312a28:	mov    %rbx,%rcx
+   2e2312a2b:	mov    0x10(%rbx),%rbx
+   2e2312a2f:	call   0x2e2313210
+   2e2312a34:	test   %rbx,%rbx
+   2e2312a37:	jne    0x2e2312a28
+   2e2312a39:	lea    0x5660(%rip),%rcx        # 0x2e23180a0
+   2e2312a40:	movq   $0x0,0x5635(%rip)        # 0x2e2318080
+   2e2312a4b:	movl   $0x0,0x5633(%rip)        # 0x2e2318088
+   2e2312a55:	call   *0x76cd(%rip)        # 0x2e231a128
+   2e2312a5b:	jmp    0x2e23129cc
+   2e2312a60:	call   0x2e2312ea0
+   2e2312a65:	mov    $0x1,%eax
+   2e2312a6a:	add    $0x20,%rsp
+   2e2312a6e:	pop    %rbx
+   2e2312a6f:	ret
+   2e2312a70:	call   0x2e2312830
+   2e2312a75:	jmp    0x2e2312a0a
+   2e2312a77:	nopw   0x0(%rax,%rax,1)
+   2e2312a80:	lea    0x5619(%rip),%rcx        # 0x2e23180a0
+   2e2312a87:	call   *0x76b3(%rip)        # 0x2e231a140
+   2e2312a8d:	jmp    0x2e23129c2
+   2e2312a92:	nop
+   2e2312a93:	nop
+   2e2312a94:	nop
+   2e2312a95:	nop
+   2e2312a96:	nop
+   2e2312a97:	nop
+   2e2312a98:	nop
+   2e2312a99:	nop
+   2e2312a9a:	nop
+   2e2312a9b:	nop
+   2e2312a9c:	nop
+   2e2312a9d:	nop
+   2e2312a9e:	nop
+   2e2312a9f:	nop
+   2e2312aa0:	xor    %eax,%eax
+   2e2312aa2:	cmpw   $0x5a4d,(%rcx)
+   2e2312aa7:	jne    0x2e2312ab8
+   2e2312aa9:	movslq 0x3c(%rcx),%rdx
+   2e2312aad:	add    %rdx,%rcx
+   2e2312ab0:	cmpl   $0x4550,(%rcx)
+   2e2312ab6:	je     0x2e2312ac0
+   2e2312ab8:	ret
+   2e2312ab9:	nopl   0x0(%rax)
+   2e2312ac0:	xor    %eax,%eax
+   2e2312ac2:	cmpw   $0x20b,0x18(%rcx)
+   2e2312ac8:	sete   %al
+   2e2312acb:	ret
+   2e2312acc:	nopl   0x0(%rax)
+   2e2312ad0:	movslq 0x3c(%rcx),%rax
+   2e2312ad4:	add    %rax,%rcx
+   2e2312ad7:	movzwl 0x14(%rcx),%eax
+   2e2312adb:	movzwl 0x6(%rcx),%r8d
+   2e2312ae0:	lea    0x18(%rcx,%rax,1),%rax
+   2e2312ae5:	test   %r8w,%r8w
+   2e2312ae9:	je     0x2e2312b1d
+   2e2312aeb:	lea    -0x1(%r8),%ecx
+   2e2312aef:	lea    (%rcx,%rcx,4),%rcx
+   2e2312af3:	lea    0x28(%rax,%rcx,8),%r9
+   2e2312af8:	nopl   0x0(%rax,%rax,1)
+   2e2312b00:	mov    0xc(%rax),%r8d
+   2e2312b04:	mov    %r8,%rcx
+   2e2312b07:	cmp    %r8,%rdx
+   2e2312b0a:	jb     0x2e2312b14
+   2e2312b0c:	add    0x8(%rax),%ecx
+   2e2312b0f:	cmp    %rcx,%rdx
+   2e2312b12:	jb     0x2e2312b1f
+   2e2312b14:	add    $0x28,%rax
+   2e2312b18:	cmp    %r9,%rax
+   2e2312b1b:	jne    0x2e2312b00
+   2e2312b1d:	xor    %eax,%eax
+   2e2312b1f:	ret
+   2e2312b20:	push   %rdi
+   2e2312b21:	push   %rsi
+   2e2312b22:	push   %rbx
+   2e2312b23:	sub    $0x20,%rsp
+   2e2312b27:	mov    %rcx,%rsi
+   2e2312b2a:	call   0x2e2313240
+   2e2312b2f:	cmp    $0x8,%rax
+   2e2312b33:	ja     0x2e2312bb0
+   2e2312b35:	mov    0x2724(%rip),%rdx        # 0x2e2315260
+   2e2312b3c:	xor    %ebx,%ebx
+   2e2312b3e:	cmpw   $0x5a4d,(%rdx)
+   2e2312b43:	jne    0x2e2312b9e
+   2e2312b45:	movslq 0x3c(%rdx),%rax
+   2e2312b49:	add    %rdx,%rax
+   2e2312b4c:	cmpl   $0x4550,(%rax)
+   2e2312b52:	jne    0x2e2312b9e
+   2e2312b54:	cmpw   $0x20b,0x18(%rax)
+   2e2312b5a:	jne    0x2e2312b9e
+   2e2312b5c:	movzwl 0x14(%rax),%edx
+   2e2312b60:	lea    0x18(%rax,%rdx,1),%rbx
+   2e2312b65:	movzwl 0x6(%rax),%edx
+   2e2312b69:	test   %dx,%dx
+   2e2312b6c:	je     0x2e2312bb0
+   2e2312b6e:	lea    -0x1(%rdx),%eax
+   2e2312b71:	lea    (%rax,%rax,4),%rax
+   2e2312b75:	lea    0x28(%rbx,%rax,8),%rdi
+   2e2312b7a:	jmp    0x2e2312b89
    2e2312b7c:	nopl   0x0(%rax)
-   2e2312b80:	sub    $0x28,%rsp
-   2e2312b84:	mov    0x2685(%rip),%rcx        # 0x2e2315210
-   2e2312b8b:	xor    %eax,%eax
-   2e2312b8d:	cmpw   $0x5a4d,(%rcx)
-   2e2312b92:	jne    0x2e2312ba6
-   2e2312b94:	call   0x2e23129c0
-   2e2312b99:	test   %eax,%eax
-   2e2312b9b:	je     0x2e2312ba6
-   2e2312b9d:	movslq 0x3c(%rcx),%rax
-   2e2312ba1:	movzwl 0x6(%rax,%rcx,1),%eax
-   2e2312ba6:	add    $0x28,%rsp
-   2e2312baa:	ret
-   2e2312bab:	nopl   0x0(%rax,%rax,1)
-   2e2312bb0:	sub    $0x28,%rsp
-   2e2312bb4:	xor    %r8d,%r8d
-   2e2312bb7:	mov    %rcx,%r9
-   2e2312bba:	mov    0x264f(%rip),%rcx        # 0x2e2315210
-   2e2312bc1:	cmpw   $0x5a4d,(%rcx)
-   2e2312bc6:	jne    0x2e2312c14
-   2e2312bc8:	call   0x2e23129c0
-   2e2312bcd:	test   %eax,%eax
-   2e2312bcf:	je     0x2e2312c14
-   2e2312bd1:	movslq 0x3c(%rcx),%rax
-   2e2312bd5:	add    %rax,%rcx
-   2e2312bd8:	movzwl 0x14(%rcx),%eax
-   2e2312bdc:	lea    0x18(%rcx,%rax,1),%r8
-   2e2312be1:	movzwl 0x6(%rcx),%eax
-   2e2312be5:	test   %eax,%eax
-   2e2312be7:	je     0x2e2312c11
-   2e2312be9:	sub    $0x1,%eax
-   2e2312bec:	lea    (%rax,%rax,4),%rax
-   2e2312bf0:	lea    0x28(%r8,%rax,8),%rax
-   2e2312bf5:	nopl   (%rax)
-   2e2312bf8:	testb  $0x20,0x27(%r8)
-   2e2312bfd:	je     0x2e2312c08
-   2e2312bff:	test   %r9,%r9
-   2e2312c02:	je     0x2e2312c14
-   2e2312c04:	sub    $0x1,%r9
-   2e2312c08:	add    $0x28,%r8
-   2e2312c0c:	cmp    %rax,%r8
-   2e2312c0f:	jne    0x2e2312bf8
-   2e2312c11:	xor    %r8d,%r8d
-   2e2312c14:	mov    %r8,%rax
-   2e2312c17:	add    $0x28,%rsp
-   2e2312c1b:	ret
-   2e2312c1c:	nopl   0x0(%rax)
-   2e2312c20:	sub    $0x28,%rsp
-   2e2312c24:	mov    0x25e5(%rip),%rcx        # 0x2e2315210
-   2e2312c2b:	xor    %r8d,%r8d
-   2e2312c2e:	cmpw   $0x5a4d,(%rcx)
-   2e2312c33:	jne    0x2e2312c40
-   2e2312c35:	call   0x2e23129c0
-   2e2312c3a:	test   %eax,%eax
-   2e2312c3c:	cmovne %rcx,%r8
-   2e2312c40:	mov    %r8,%rax
-   2e2312c43:	add    $0x28,%rsp
-   2e2312c47:	ret
-   2e2312c48:	nopl   0x0(%rax,%rax,1)
-   2e2312c50:	sub    $0x28,%rsp
-   2e2312c54:	mov    0x25b5(%rip),%r9        # 0x2e2315210
-   2e2312c5b:	xor    %eax,%eax
-   2e2312c5d:	cmpw   $0x5a4d,(%r9)
-   2e2312c63:	mov    %rcx,%r8
-   2e2312c66:	jne    0x2e2312cbf
-   2e2312c68:	mov    %r9,%rcx
-   2e2312c6b:	call   0x2e23129c0
-   2e2312c70:	test   %eax,%eax
-   2e2312c72:	je     0x2e2312cbf
-   2e2312c74:	movslq 0x3c(%r9),%rax
-   2e2312c78:	mov    %r8,%rcx
-   2e2312c7b:	sub    %r9,%rcx
-   2e2312c7e:	add    %rax,%r9
-   2e2312c81:	movzwl 0x14(%r9),%eax
-   2e2312c86:	movzwl 0x6(%r9),%edx
-   2e2312c8b:	lea    0x18(%r9,%rax,1),%rax
-   2e2312c90:	test   %edx,%edx
-   2e2312c92:	je     0x2e2312cbd
-   2e2312c94:	sub    $0x1,%edx
-   2e2312c97:	lea    (%rdx,%rdx,4),%rdx
-   2e2312c9b:	lea    0x28(%rax,%rdx,8),%r9
-   2e2312ca0:	mov    0xc(%rax),%r8d
-   2e2312ca4:	mov    %r8,%rdx
-   2e2312ca7:	cmp    %r8,%rcx
-   2e2312caa:	jb     0x2e2312cb4
-   2e2312cac:	add    0x8(%rax),%edx
-   2e2312caf:	cmp    %rdx,%rcx
-   2e2312cb2:	jb     0x2e2312cc8
-   2e2312cb4:	add    $0x28,%rax
-   2e2312cb8:	cmp    %r9,%rax
-   2e2312cbb:	jne    0x2e2312ca0
-   2e2312cbd:	xor    %eax,%eax
-   2e2312cbf:	add    $0x28,%rsp
-   2e2312cc3:	ret
-   2e2312cc4:	nopl   0x0(%rax)
-   2e2312cc8:	mov    0x24(%rax),%eax
-   2e2312ccb:	not    %eax
-   2e2312ccd:	shr    $0x1f,%eax
-   2e2312cd0:	add    $0x28,%rsp
-   2e2312cd4:	ret
-   2e2312cd5:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e2312ce0:	sub    $0x28,%rsp
-   2e2312ce4:	mov    0x2525(%rip),%r11        # 0x2e2315210
-   2e2312ceb:	xor    %r9d,%r9d
-   2e2312cee:	cmpw   $0x5a4d,(%r11)
-   2e2312cf4:	mov    %ecx,%r8d
-   2e2312cf7:	jne    0x2e2312d58
-   2e2312cf9:	mov    %r11,%rcx
-   2e2312cfc:	call   0x2e23129c0
-   2e2312d01:	test   %eax,%eax
-   2e2312d03:	je     0x2e2312d58
-   2e2312d05:	movslq 0x3c(%r11),%rcx
-   2e2312d09:	add    %r11,%rcx
-   2e2312d0c:	mov    0x90(%rcx),%eax
-   2e2312d12:	test   %eax,%eax
-   2e2312d14:	je     0x2e2312d58
-   2e2312d16:	movzwl 0x14(%rcx),%edx
-   2e2312d1a:	lea    0x18(%rcx,%rdx,1),%rdx
-   2e2312d1f:	movzwl 0x6(%rcx),%ecx
-   2e2312d23:	test   %ecx,%ecx
-   2e2312d25:	je     0x2e2312d58
-   2e2312d27:	sub    $0x1,%ecx
-   2e2312d2a:	lea    (%rcx,%rcx,4),%rcx
-   2e2312d2e:	lea    0x28(%rdx,%rcx,8),%r10
-   2e2312d33:	nopl   0x0(%rax,%rax,1)
-   2e2312d38:	mov    0xc(%rdx),%r9d
-   2e2312d3c:	mov    %r9,%rcx
-   2e2312d3f:	cmp    %r9,%rax
-   2e2312d42:	jb     0x2e2312d4c
-   2e2312d44:	add    0x8(%rdx),%ecx
-   2e2312d47:	cmp    %rcx,%rax
-   2e2312d4a:	jb     0x2e2312d60
-   2e2312d4c:	add    $0x28,%rdx
-   2e2312d50:	cmp    %r10,%rdx
-   2e2312d53:	jne    0x2e2312d38
-   2e2312d55:	xor    %r9d,%r9d
-   2e2312d58:	mov    %r9,%rax
-   2e2312d5b:	add    $0x28,%rsp
-   2e2312d5f:	ret
-   2e2312d60:	add    %r11,%rax
-   2e2312d63:	jmp    0x2e2312d70
-   2e2312d65:	nopl   (%rax)
-   2e2312d68:	sub    $0x1,%r8d
-   2e2312d6c:	add    $0x14,%rax
-   2e2312d70:	mov    0x4(%rax),%ecx
-   2e2312d73:	test   %ecx,%ecx
-   2e2312d75:	jne    0x2e2312d7e
-   2e2312d77:	mov    0xc(%rax),%edx
-   2e2312d7a:	test   %edx,%edx
-   2e2312d7c:	je     0x2e2312d55
-   2e2312d7e:	test   %r8d,%r8d
-   2e2312d81:	jg     0x2e2312d68
-   2e2312d83:	mov    0xc(%rax),%r9d
-   2e2312d87:	add    %r11,%r9
-   2e2312d8a:	mov    %r9,%rax
-   2e2312d8d:	add    $0x28,%rsp
-   2e2312d91:	ret
-   2e2312d92:	nop
-   2e2312d93:	nop
-   2e2312d94:	nop
-   2e2312d95:	nop
-   2e2312d96:	nop
-   2e2312d97:	nop
-   2e2312d98:	nop
-   2e2312d99:	nop
-   2e2312d9a:	nop
-   2e2312d9b:	nop
-   2e2312d9c:	nop
-   2e2312d9d:	nop
-   2e2312d9e:	nop
-   2e2312d9f:	nop
-   2e2312da0:	fninit
-   2e2312da2:	ret
-   2e2312da3:	nop
-   2e2312da4:	nop
-   2e2312da5:	nop
-   2e2312da6:	nop
-   2e2312da7:	nop
-   2e2312da8:	nop
-   2e2312da9:	nop
-   2e2312daa:	nop
-   2e2312dab:	nop
-   2e2312dac:	nop
-   2e2312dad:	nop
-   2e2312dae:	nop
-   2e2312daf:	nop
-   2e2312db0:	push   %rcx
-   2e2312db1:	push   %rax
-   2e2312db2:	cmp    $0x1000,%rax
-   2e2312db8:	lea    0x18(%rsp),%rcx
-   2e2312dbd:	jb     0x2e2312dd8
-   2e2312dbf:	sub    $0x1000,%rcx
-   2e2312dc6:	orq    $0x0,(%rcx)
-   2e2312dca:	sub    $0x1000,%rax
-   2e2312dd0:	cmp    $0x1000,%rax
-   2e2312dd6:	ja     0x2e2312dbf
-   2e2312dd8:	sub    %rax,%rcx
-   2e2312ddb:	orq    $0x0,(%rcx)
-   2e2312ddf:	pop    %rax
-   2e2312de0:	pop    %rcx
-   2e2312de1:	ret
-   2e2312de2:	nop
-   2e2312de3:	nop
-   2e2312de4:	nop
-   2e2312de5:	nop
-   2e2312de6:	nop
-   2e2312de7:	nop
-   2e2312de8:	nop
-   2e2312de9:	nop
-   2e2312dea:	nop
-   2e2312deb:	nop
-   2e2312dec:	nop
-   2e2312ded:	nop
-   2e2312dee:	nop
-   2e2312def:	nop
-   2e2312df0:	mov    $0x1,%eax
+   2e2312b80:	add    $0x28,%rbx
+   2e2312b84:	cmp    %rdi,%rbx
+   2e2312b87:	je     0x2e2312bb0
+   2e2312b89:	mov    $0x8,%r8d
+   2e2312b8f:	mov    %rsi,%rdx
+   2e2312b92:	mov    %rbx,%rcx
+   2e2312b95:	call   0x2e2313248
+   2e2312b9a:	test   %eax,%eax
+   2e2312b9c:	jne    0x2e2312b80
+   2e2312b9e:	mov    %rbx,%rax
+   2e2312ba1:	add    $0x20,%rsp
+   2e2312ba5:	pop    %rbx
+   2e2312ba6:	pop    %rsi
+   2e2312ba7:	pop    %rdi
+   2e2312ba8:	ret
+   2e2312ba9:	nopl   0x0(%rax)
+   2e2312bb0:	xor    %ebx,%ebx
+   2e2312bb2:	mov    %rbx,%rax
+   2e2312bb5:	add    $0x20,%rsp
+   2e2312bb9:	pop    %rbx
+   2e2312bba:	pop    %rsi
+   2e2312bbb:	pop    %rdi
+   2e2312bbc:	ret
+   2e2312bbd:	nopl   (%rax)
+   2e2312bc0:	mov    0x2699(%rip),%rdx        # 0x2e2315260
+   2e2312bc7:	xor    %eax,%eax
+   2e2312bc9:	cmpw   $0x5a4d,(%rdx)
+   2e2312bce:	jne    0x2e2312be0
+   2e2312bd0:	movslq 0x3c(%rdx),%r8
+   2e2312bd4:	add    %rdx,%r8
+   2e2312bd7:	cmpl   $0x4550,(%r8)
+   2e2312bde:	je     0x2e2312be8
+   2e2312be0:	ret
+   2e2312be1:	nopl   0x0(%rax)
+   2e2312be8:	cmpw   $0x20b,0x18(%r8)
+   2e2312bef:	jne    0x2e2312be0
+   2e2312bf1:	movzwl 0x14(%r8),%eax
+   2e2312bf6:	sub    %rdx,%rcx
+   2e2312bf9:	lea    0x18(%r8,%rax,1),%rax
+   2e2312bfe:	movzwl 0x6(%r8),%r8d
+   2e2312c03:	test   %r8w,%r8w
+   2e2312c07:	je     0x2e2312c3d
+   2e2312c09:	lea    -0x1(%r8),%edx
+   2e2312c0d:	lea    (%rdx,%rdx,4),%rdx
+   2e2312c11:	lea    0x28(%rax,%rdx,8),%r9
+   2e2312c16:	cs nopw 0x0(%rax,%rax,1)
+   2e2312c20:	mov    0xc(%rax),%r8d
+   2e2312c24:	mov    %r8,%rdx
+   2e2312c27:	cmp    %r8,%rcx
+   2e2312c2a:	jb     0x2e2312c34
+   2e2312c2c:	add    0x8(%rax),%edx
+   2e2312c2f:	cmp    %rdx,%rcx
+   2e2312c32:	jb     0x2e2312be0
+   2e2312c34:	add    $0x28,%rax
+   2e2312c38:	cmp    %r9,%rax
+   2e2312c3b:	jne    0x2e2312c20
+   2e2312c3d:	xor    %eax,%eax
+   2e2312c3f:	ret
+   2e2312c40:	mov    0x2619(%rip),%rax        # 0x2e2315260
+   2e2312c47:	xor    %ecx,%ecx
+   2e2312c49:	cmpw   $0x5a4d,(%rax)
+   2e2312c4e:	jne    0x2e2312c5f
+   2e2312c50:	movslq 0x3c(%rax),%rdx
+   2e2312c54:	add    %rdx,%rax
+   2e2312c57:	cmpl   $0x4550,(%rax)
+   2e2312c5d:	je     0x2e2312c68
+   2e2312c5f:	mov    %ecx,%eax
+   2e2312c61:	ret
+   2e2312c62:	nopw   0x0(%rax,%rax,1)
+   2e2312c68:	cmpw   $0x20b,0x18(%rax)
+   2e2312c6e:	jne    0x2e2312c5f
+   2e2312c70:	movzwl 0x6(%rax),%ecx
+   2e2312c74:	mov    %ecx,%eax
+   2e2312c76:	ret
+   2e2312c77:	nopw   0x0(%rax,%rax,1)
+   2e2312c80:	mov    0x25d9(%rip),%r8        # 0x2e2315260
+   2e2312c87:	xor    %eax,%eax
+   2e2312c89:	cmpw   $0x5a4d,(%r8)
+   2e2312c8f:	jne    0x2e2312ca0
+   2e2312c91:	movslq 0x3c(%r8),%rdx
+   2e2312c95:	add    %r8,%rdx
+   2e2312c98:	cmpl   $0x4550,(%rdx)
+   2e2312c9e:	je     0x2e2312ca8
+   2e2312ca0:	ret
+   2e2312ca1:	nopl   0x0(%rax)
+   2e2312ca8:	cmpw   $0x20b,0x18(%rdx)
+   2e2312cae:	jne    0x2e2312ca0
+   2e2312cb0:	movzwl 0x14(%rdx),%eax
+   2e2312cb4:	movzwl 0x6(%rdx),%r8d
+   2e2312cb9:	lea    0x18(%rdx,%rax,1),%rax
+   2e2312cbe:	test   %r8w,%r8w
+   2e2312cc2:	je     0x2e2312cf0
+   2e2312cc4:	lea    -0x1(%r8),%edx
+   2e2312cc8:	lea    (%rdx,%rdx,4),%rdx
+   2e2312ccc:	lea    0x28(%rax,%rdx,8),%rdx
+   2e2312cd1:	nopl   0x0(%rax)
+   2e2312cd8:	testb  $0x20,0x27(%rax)
+   2e2312cdc:	je     0x2e2312ce7
+   2e2312cde:	test   %rcx,%rcx
+   2e2312ce1:	je     0x2e2312ca0
+   2e2312ce3:	sub    $0x1,%rcx
+   2e2312ce7:	add    $0x28,%rax
+   2e2312ceb:	cmp    %rdx,%rax
+   2e2312cee:	jne    0x2e2312cd8
+   2e2312cf0:	xor    %eax,%eax
+   2e2312cf2:	ret
+   2e2312cf3:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e2312cfe:	xchg   %ax,%ax
+   2e2312d00:	mov    0x2559(%rip),%rax        # 0x2e2315260
+   2e2312d07:	xor    %edx,%edx
+   2e2312d09:	cmpw   $0x5a4d,(%rax)
+   2e2312d0e:	jne    0x2e2312d1f
+   2e2312d10:	movslq 0x3c(%rax),%rcx
+   2e2312d14:	add    %rax,%rcx
+   2e2312d17:	cmpl   $0x4550,(%rcx)
+   2e2312d1d:	je     0x2e2312d28
+   2e2312d1f:	mov    %rdx,%rax
+   2e2312d22:	ret
+   2e2312d23:	nopl   0x0(%rax,%rax,1)
+   2e2312d28:	cmpw   $0x20b,0x18(%rcx)
+   2e2312d2e:	cmove  %rax,%rdx
+   2e2312d32:	mov    %rdx,%rax
+   2e2312d35:	ret
+   2e2312d36:	cs nopw 0x0(%rax,%rax,1)
+   2e2312d40:	mov    0x2519(%rip),%rdx        # 0x2e2315260
+   2e2312d47:	xor    %eax,%eax
+   2e2312d49:	cmpw   $0x5a4d,(%rdx)
+   2e2312d4e:	jne    0x2e2312d60
+   2e2312d50:	movslq 0x3c(%rdx),%r8
+   2e2312d54:	add    %rdx,%r8
+   2e2312d57:	cmpl   $0x4550,(%r8)
+   2e2312d5e:	je     0x2e2312d68
+   2e2312d60:	ret
+   2e2312d61:	nopl   0x0(%rax)
+   2e2312d68:	cmpw   $0x20b,0x18(%r8)
+   2e2312d6f:	jne    0x2e2312d60
+   2e2312d71:	sub    %rdx,%rcx
+   2e2312d74:	movzwl 0x6(%r8),%r9d
+   2e2312d79:	movzwl 0x14(%r8),%edx
+   2e2312d7e:	lea    0x18(%r8,%rdx,1),%rdx
+   2e2312d83:	test   %r9w,%r9w
+   2e2312d87:	je     0x2e2312d60
+   2e2312d89:	lea    -0x1(%r9),%eax
+   2e2312d8d:	lea    (%rax,%rax,4),%rax
+   2e2312d91:	lea    0x28(%rdx,%rax,8),%r9
+   2e2312d96:	cs nopw 0x0(%rax,%rax,1)
+   2e2312da0:	mov    0xc(%rdx),%r8d
+   2e2312da4:	mov    %r8,%rax
+   2e2312da7:	cmp    %r8,%rcx
+   2e2312daa:	jb     0x2e2312db4
+   2e2312dac:	add    0x8(%rdx),%eax
+   2e2312daf:	cmp    %rax,%rcx
+   2e2312db2:	jb     0x2e2312dc0
+   2e2312db4:	add    $0x28,%rdx
+   2e2312db8:	cmp    %rdx,%r9
+   2e2312dbb:	jne    0x2e2312da0
+   2e2312dbd:	xor    %eax,%eax
+   2e2312dbf:	ret
+   2e2312dc0:	mov    0x24(%rdx),%eax
+   2e2312dc3:	not    %eax
+   2e2312dc5:	shr    $0x1f,%eax
+   2e2312dc8:	ret
+   2e2312dc9:	nopl   0x0(%rax)
+   2e2312dd0:	mov    0x2489(%rip),%r11        # 0x2e2315260
+   2e2312dd7:	xor    %r9d,%r9d
+   2e2312dda:	cmpw   $0x5a4d,(%r11)
+   2e2312de0:	jne    0x2e2312df2
+   2e2312de2:	movslq 0x3c(%r11),%r8
+   2e2312de6:	add    %r11,%r8
+   2e2312de9:	cmpl   $0x4550,(%r8)
+   2e2312df0:	je     0x2e2312e00
+   2e2312df2:	mov    %r9,%rax
    2e2312df5:	ret
-   2e2312df6:	nop
-   2e2312df7:	nop
-   2e2312df8:	nop
-   2e2312df9:	nop
-   2e2312dfa:	nop
-   2e2312dfb:	nop
-   2e2312dfc:	nop
-   2e2312dfd:	nop
-   2e2312dfe:	nop
-   2e2312dff:	nop
-   2e2312e00:	mov    $0x1,%eax
-   2e2312e05:	ret
-   2e2312e06:	nop
-   2e2312e07:	nop
-   2e2312e08:	nop
-   2e2312e09:	nop
-   2e2312e0a:	nop
-   2e2312e0b:	nop
-   2e2312e0c:	nop
-   2e2312e0d:	nop
-   2e2312e0e:	nop
-   2e2312e0f:	nop
-   2e2312e10:	push   %rbx
-   2e2312e11:	sub    $0x50,%rsp
-   2e2312e15:	movups %xmm6,0x40(%rsp)
-   2e2312e1a:	movq   %xmm0,%rdx
-   2e2312e1f:	movq   %xmm0,%rbx
-   2e2312e24:	shr    $0x20,%rdx
-   2e2312e28:	mov    %edx,%eax
-   2e2312e2a:	mov    %edx,%ecx
-   2e2312e2c:	and    $0xfffff,%eax
-   2e2312e31:	and    $0x7ff00000,%ecx
-   2e2312e37:	or     %ebx,%eax
-   2e2312e39:	mov    %eax,%r8d
-   2e2312e3c:	or     %ecx,%r8d
-   2e2312e3f:	je     0x2e2312ee8
-   2e2312e45:	test   %ecx,%ecx
-   2e2312e47:	je     0x2e2312e51
-   2e2312e49:	cmp    $0x7ff00000,%ecx
-   2e2312e4f:	je     0x2e2312e90
-   2e2312e51:	test   %edx,%edx
-   2e2312e53:	js     0x2e2312ea0
-   2e2312e55:	movq   %rbx,%xmm1
-   2e2312e5a:	ucomisd 0x234e(%rip),%xmm1        # 0x2e23151b0
-   2e2312e62:	jnp    0x2e2312f48
-   2e2312e68:	mov    %rbx,0x38(%rsp)
-   2e2312e6d:	fldl   0x38(%rsp)
-   2e2312e71:	fsqrt
-   2e2312e73:	fstpl  0x38(%rsp)
-   2e2312e77:	movsd  0x38(%rsp),%xmm0
-   2e2312e7d:	movups 0x40(%rsp),%xmm6
-   2e2312e82:	add    $0x50,%rsp
-   2e2312e86:	pop    %rbx
-   2e2312e87:	ret
-   2e2312e88:	nopl   0x0(%rax,%rax,1)
-   2e2312e90:	test   %eax,%eax
-   2e2312e92:	jne    0x2e2312f08
-   2e2312e94:	movsd  0x22fc(%rip),%xmm0        # 0x2e2315198
-   2e2312e9c:	test   %edx,%edx
-   2e2312e9e:	jns    0x2e2312e7d
-   2e2312ea0:	call   0x2e2312fa8
-   2e2312ea5:	pxor   %xmm3,%xmm3
-   2e2312ea9:	movsd  0x22ef(%rip),%xmm6        # 0x2e23151a0
-   2e2312eb1:	movq   %rbx,%xmm2
-   2e2312eb6:	movl   $0x21,(%rax)
-   2e2312ebc:	lea    0x22cd(%rip),%rdx        # 0x2e2315190
-   2e2312ec3:	mov    $0x1,%ecx
-   2e2312ec8:	movsd  %xmm6,0x20(%rsp)
-   2e2312ece:	call   0x2e23131e0
-   2e2312ed3:	movupd %xmm6,%xmm0
-   2e2312ed7:	movups 0x40(%rsp),%xmm6
-   2e2312edc:	add    $0x50,%rsp
-   2e2312ee0:	pop    %rbx
+   2e2312df6:	cs nopw 0x0(%rax,%rax,1)
+   2e2312e00:	cmpw   $0x20b,0x18(%r8)
+   2e2312e07:	jne    0x2e2312df2
+   2e2312e09:	mov    0x90(%r8),%eax
+   2e2312e10:	test   %eax,%eax
+   2e2312e12:	je     0x2e2312df2
+   2e2312e14:	movzwl 0x14(%r8),%edx
+   2e2312e19:	movzwl 0x6(%r8),%r10d
+   2e2312e1e:	lea    0x18(%r8,%rdx,1),%rdx
+   2e2312e23:	test   %r10w,%r10w
+   2e2312e27:	je     0x2e2312df2
+   2e2312e29:	lea    -0x1(%r10),%r8d
+   2e2312e2d:	lea    (%r8,%r8,4),%r8
+   2e2312e31:	lea    0x28(%rdx,%r8,8),%r10
+   2e2312e36:	cs nopw 0x0(%rax,%rax,1)
+   2e2312e40:	mov    0xc(%rdx),%r9d
+   2e2312e44:	mov    %r9,%r8
+   2e2312e47:	cmp    %r9,%rax
+   2e2312e4a:	jb     0x2e2312e55
+   2e2312e4c:	add    0x8(%rdx),%r8d
+   2e2312e50:	cmp    %r8,%rax
+   2e2312e53:	jb     0x2e2312e68
+   2e2312e55:	add    $0x28,%rdx
+   2e2312e59:	cmp    %r10,%rdx
+   2e2312e5c:	jne    0x2e2312e40
+   2e2312e5e:	xor    %r9d,%r9d
+   2e2312e61:	mov    %r9,%rax
+   2e2312e64:	ret
+   2e2312e65:	nopl   (%rax)
+   2e2312e68:	add    %r11,%rax
+   2e2312e6b:	jmp    0x2e2312e77
+   2e2312e6d:	nopl   (%rax)
+   2e2312e70:	sub    $0x1,%ecx
+   2e2312e73:	add    $0x14,%rax
+   2e2312e77:	mov    0x4(%rax),%r8d
+   2e2312e7b:	test   %r8d,%r8d
+   2e2312e7e:	jne    0x2e2312e87
+   2e2312e80:	mov    0xc(%rax),%edx
+   2e2312e83:	test   %edx,%edx
+   2e2312e85:	je     0x2e2312e5e
+   2e2312e87:	test   %ecx,%ecx
+   2e2312e89:	jg     0x2e2312e70
+   2e2312e8b:	mov    0xc(%rax),%r9d
+   2e2312e8f:	add    %r11,%r9
+   2e2312e92:	mov    %r9,%rax
+   2e2312e95:	ret
+   2e2312e96:	nop
+   2e2312e97:	nop
+   2e2312e98:	nop
+   2e2312e99:	nop
+   2e2312e9a:	nop
+   2e2312e9b:	nop
+   2e2312e9c:	nop
+   2e2312e9d:	nop
+   2e2312e9e:	nop
+   2e2312e9f:	nop
+   2e2312ea0:	fninit
+   2e2312ea2:	ret
+   2e2312ea3:	nop
+   2e2312ea4:	nop
+   2e2312ea5:	nop
+   2e2312ea6:	nop
+   2e2312ea7:	nop
+   2e2312ea8:	nop
+   2e2312ea9:	nop
+   2e2312eaa:	nop
+   2e2312eab:	nop
+   2e2312eac:	nop
+   2e2312ead:	nop
+   2e2312eae:	nop
+   2e2312eaf:	nop
+   2e2312eb0:	push   %rcx
+   2e2312eb1:	push   %rax
+   2e2312eb2:	cmp    $0x1000,%rax
+   2e2312eb8:	lea    0x18(%rsp),%rcx
+   2e2312ebd:	jb     0x2e2312ed8
+   2e2312ebf:	sub    $0x1000,%rcx
+   2e2312ec6:	orq    $0x0,(%rcx)
+   2e2312eca:	sub    $0x1000,%rax
+   2e2312ed0:	cmp    $0x1000,%rax
+   2e2312ed6:	ja     0x2e2312ebf
+   2e2312ed8:	sub    %rax,%rcx
+   2e2312edb:	orq    $0x0,(%rcx)
+   2e2312edf:	pop    %rax
+   2e2312ee0:	pop    %rcx
    2e2312ee1:	ret
-   2e2312ee2:	nopw   0x0(%rax,%rax,1)
-   2e2312ee8:	movsd  0x22b8(%rip),%xmm0        # 0x2e23151a8
-   2e2312ef0:	test   %edx,%edx
-   2e2312ef2:	js     0x2e2312e7d
-   2e2312ef4:	movups 0x40(%rsp),%xmm6
-   2e2312ef9:	pxor   %xmm0,%xmm0
-   2e2312efd:	add    $0x50,%rsp
-   2e2312f01:	pop    %rbx
-   2e2312f02:	ret
-   2e2312f03:	nopl   0x0(%rax,%rax,1)
-   2e2312f08:	call   0x2e2312fa8
-   2e2312f0d:	pxor   %xmm3,%xmm3
-   2e2312f11:	movq   %rbx,%xmm2
-   2e2312f16:	lea    0x2273(%rip),%rdx        # 0x2e2315190
-   2e2312f1d:	movl   $0x21,(%rax)
-   2e2312f23:	mov    $0x1,%ecx
-   2e2312f28:	mov    %rbx,0x20(%rsp)
-   2e2312f2d:	call   0x2e23131e0
-   2e2312f32:	nop
-   2e2312f33:	movups 0x40(%rsp),%xmm6
-   2e2312f38:	movq   %rbx,%xmm0
-   2e2312f3d:	add    $0x50,%rsp
-   2e2312f41:	pop    %rbx
-   2e2312f42:	ret
-   2e2312f43:	nopl   0x0(%rax,%rax,1)
-   2e2312f48:	je     0x2e2312f33
-   2e2312f4a:	jmp    0x2e2312e68
-   2e2312f4f:	nop
-   2e2312f50:	jmp    *0x72a6(%rip)        # 0x2e231a1fc
-   2e2312f56:	nop
-   2e2312f57:	nop
-   2e2312f58:	jmp    *0x7296(%rip)        # 0x2e231a1f4
-   2e2312f5e:	nop
-   2e2312f5f:	nop
-   2e2312f60:	jmp    *0x7286(%rip)        # 0x2e231a1ec
-   2e2312f66:	nop
-   2e2312f67:	nop
-   2e2312f68:	jmp    *0x726e(%rip)        # 0x2e231a1dc
-   2e2312f6e:	nop
-   2e2312f6f:	nop
-   2e2312f70:	jmp    *0x725e(%rip)        # 0x2e231a1d4
-   2e2312f76:	nop
-   2e2312f77:	nop
-   2e2312f78:	jmp    *0x724e(%rip)        # 0x2e231a1cc
-   2e2312f7e:	nop
-   2e2312f7f:	nop
-   2e2312f80:	jmp    *0x723e(%rip)        # 0x2e231a1c4
-   2e2312f86:	nop
-   2e2312f87:	nop
-   2e2312f88:	jmp    *0x722e(%rip)        # 0x2e231a1bc
-   2e2312f8e:	nop
-   2e2312f8f:	nop
-   2e2312f90:	jmp    *0x721e(%rip)        # 0x2e231a1b4
-   2e2312f96:	nop
-   2e2312f97:	nop
-   2e2312f98:	jmp    *0x720e(%rip)        # 0x2e231a1ac
-   2e2312f9e:	nop
-   2e2312f9f:	nop
-   2e2312fa0:	jmp    *0x71ee(%rip)        # 0x2e231a194
-   2e2312fa6:	nop
-   2e2312fa7:	nop
-   2e2312fa8:	jmp    *0x71de(%rip)        # 0x2e231a18c
-   2e2312fae:	nop
-   2e2312faf:	nop
-   2e2312fb0:	jmp    *0x71ce(%rip)        # 0x2e231a184
-   2e2312fb6:	nop
-   2e2312fb7:	nop
-   2e2312fb8:	nopl   0x0(%rax,%rax,1)
-   2e2312fc0:	test   %rcx,%rcx
-   2e2312fc3:	je     0x2e2312fdf
-   2e2312fc5:	xor    %eax,%eax
-   2e2312fc7:	movq   $0x0,0x10(%rcx)
-   2e2312fcf:	movq   $0x0,0x8(%rcx)
-   2e2312fd7:	movq   $0x0,(%rcx)
-   2e2312fde:	ret
-   2e2312fdf:	mov    $0xffffffff,%eax
-   2e2312fe4:	ret
-   2e2312fe5:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e2312ff0:	push   %rbp
-   2e2312ff1:	push   %rdi
-   2e2312ff2:	push   %rsi
-   2e2312ff3:	push   %rbx
-   2e2312ff4:	sub    $0x28,%rsp
-   2e2312ff8:	mov    %rcx,%rbx
-   2e2312ffb:	mov    %rdx,%rdi
-   2e2312ffe:	test   %rcx,%rcx
-   2e2313001:	je     0x2e23130ab
-   2e2313007:	mov    $0x8,%ecx
-   2e231300c:	call   0x2e2313180
-   2e2313011:	cmpq   $0x0,(%rbx)
-   2e2313015:	je     0x2e2313080
-   2e2313017:	mov    0x8(%rbx),%rax
-   2e231301b:	mov    0x10(%rbx),%rdx
-   2e231301f:	cmp    %rax,%rdx
-   2e2313022:	je     0x2e2313048
-   2e2313024:	lea    0x8(%rax),%rdx
-   2e2313028:	mov    $0x8,%ecx
-   2e231302d:	mov    %rdx,0x8(%rbx)
-   2e2313031:	mov    %rdi,(%rax)
-   2e2313034:	call   0x2e2313178
-   2e2313039:	xor    %eax,%eax
-   2e231303b:	add    $0x28,%rsp
-   2e231303f:	pop    %rbx
-   2e2313040:	pop    %rsi
-   2e2313041:	pop    %rdi
-   2e2313042:	pop    %rbp
-   2e2313043:	ret
-   2e2313044:	nopl   0x0(%rax)
-   2e2313048:	mov    (%rbx),%rcx
-   2e231304b:	sub    %rcx,%rax
-   2e231304e:	mov    %rax,%rdx
-   2e2313051:	mov    %rax,%rsi
-   2e2313054:	sar    $0x3,%rdx
-   2e2313058:	shl    $0x4,%rdx
-   2e231305c:	mov    %rdx,%rbp
-   2e231305f:	call   0x2e2313170
-   2e2313064:	mov    %rax,%rdx
-   2e2313067:	test   %rax,%rax
-   2e231306a:	je     0x2e23130b2
-   2e231306c:	add    %rbp,%rdx
-   2e231306f:	mov    %rax,(%rbx)
-   2e2313072:	lea    (%rax,%rsi,1),%rax
-   2e2313076:	mov    %rdx,0x10(%rbx)
-   2e231307a:	jmp    0x2e2313024
-   2e231307c:	nopl   0x0(%rax)
-   2e2313080:	mov    $0x8,%edx
-   2e2313085:	mov    $0x20,%ecx
-   2e231308a:	call   0x2e2312f90
-   2e231308f:	mov    %rax,(%rbx)
-   2e2313092:	test   %rax,%rax
-   2e2313095:	je     0x2e23130b2
-   2e2313097:	lea    0x100(%rax),%rdx
-   2e231309e:	mov    %rax,0x8(%rbx)
-   2e23130a2:	mov    %rdx,0x10(%rbx)
-   2e23130a6:	jmp    0x2e231301f
-   2e23130ab:	mov    $0xffffffff,%eax
-   2e23130b0:	jmp    0x2e231303b
-   2e23130b2:	mov    $0x8,%ecx
-   2e23130b7:	call   0x2e2313178
-   2e23130bc:	or     $0xffffffff,%eax
-   2e23130bf:	jmp    0x2e231303b
-   2e23130c4:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e23130cf:	nop
-   2e23130d0:	push   %r12
-   2e23130d2:	push   %rsi
-   2e23130d3:	push   %rbx
-   2e23130d4:	sub    $0x20,%rsp
-   2e23130d8:	mov    %rcx,%rsi
-   2e23130db:	mov    $0x8,%ecx
-   2e23130e0:	call   0x2e2313180
-   2e23130e5:	mov    (%rsi),%r12
-   2e23130e8:	mov    0x8(%rsi),%rbx
-   2e23130ec:	movq   $0x0,0x10(%rsi)
-   2e23130f4:	movq   $0x0,0x8(%rsi)
-   2e23130fc:	mov    $0x8,%ecx
-   2e2313101:	movq   $0x0,(%rsi)
-   2e2313108:	call   0x2e2313178
-   2e231310d:	test   %r12,%r12
-   2e2313110:	je     0x2e2313136
-   2e2313112:	sub    $0x8,%rbx
-   2e2313116:	cmp    %rbx,%r12
-   2e2313119:	ja     0x2e231312e
-   2e231311b:	mov    (%rbx),%rax
-   2e231311e:	test   %rax,%rax
-   2e2313121:	je     0x2e2313112
-   2e2313123:	call   *%rax
-   2e2313125:	sub    $0x8,%rbx
-   2e2313129:	cmp    %rbx,%r12
-   2e231312c:	jbe    0x2e231311b
-   2e231312e:	mov    %r12,%rcx
-   2e2313131:	call   0x2e2312f88
-   2e2313136:	xor    %eax,%eax
-   2e2313138:	add    $0x20,%rsp
-   2e231313c:	pop    %rbx
-   2e231313d:	pop    %rsi
-   2e231313e:	pop    %r12
-   2e2313140:	ret
-   2e2313141:	nop
-   2e2313142:	nop
-   2e2313143:	nop
-   2e2313144:	nop
-   2e2313145:	nop
-   2e2313146:	nop
-   2e2313147:	nop
-   2e2313148:	nop
-   2e2313149:	nop
-   2e231314a:	nop
-   2e231314b:	nop
-   2e231314c:	nop
-   2e231314d:	nop
-   2e231314e:	nop
-   2e231314f:	nop
-   2e2313150:	push   %rbx
-   2e2313151:	sub    $0x20,%rsp
-   2e2313155:	mov    %ecx,%ebx
-   2e2313157:	call   0x2e2313188
-   2e231315c:	mov    %ebx,%ecx
-   2e231315e:	lea    (%rcx,%rcx,2),%rdx
-   2e2313162:	shl    $0x4,%rdx
-   2e2313166:	add    %rdx,%rax
-   2e2313169:	add    $0x20,%rsp
-   2e231316d:	pop    %rbx
-   2e231316e:	ret
-   2e231316f:	nop
-   2e2313170:	jmp    *0x706e(%rip)        # 0x2e231a1e4
-   2e2313176:	nop
-   2e2313177:	nop
-   2e2313178:	jmp    *0x7026(%rip)        # 0x2e231a1a4
-   2e231317e:	nop
-   2e231317f:	nop
-   2e2313180:	jmp    *0x7016(%rip)        # 0x2e231a19c
-   2e2313186:	nop
-   2e2313187:	nop
-   2e2313188:	jmp    *0x6fe6(%rip)        # 0x2e231a174
-   2e231318e:	nop
-   2e231318f:	nop
-   2e2313190:	jmp    *0x6fce(%rip)        # 0x2e231a164
-   2e2313196:	nop
-   2e2313197:	nop
-   2e2313198:	jmp    *0x6fbe(%rip)        # 0x2e231a15c
-   2e231319e:	nop
-   2e231319f:	nop
-   2e23131a0:	jmp    *0x6fae(%rip)        # 0x2e231a154
-   2e23131a6:	nop
-   2e23131a7:	nop
-   2e23131a8:	jmp    *0x6f9e(%rip)        # 0x2e231a14c
-   2e23131ae:	nop
-   2e23131af:	nop
-   2e23131b0:	jmp    *0x6f8e(%rip)        # 0x2e231a144
-   2e23131b6:	nop
-   2e23131b7:	nop
-   2e23131b8:	jmp    *0x6f7e(%rip)        # 0x2e231a13c
-   2e23131be:	nop
-   2e23131bf:	nop
-   2e23131c0:	jmp    *0x6f6e(%rip)        # 0x2e231a134
-   2e23131c6:	nop
+   2e2312ee2:	nop
+   2e2312ee3:	nop
+   2e2312ee4:	nop
+   2e2312ee5:	nop
+   2e2312ee6:	nop
+   2e2312ee7:	nop
+   2e2312ee8:	nop
+   2e2312ee9:	nop
+   2e2312eea:	nop
+   2e2312eeb:	nop
+   2e2312eec:	nop
+   2e2312eed:	nop
+   2e2312eee:	nop
+   2e2312eef:	nop
+   2e2312ef0:	mov    $0x1,%eax
+   2e2312ef5:	ret
+   2e2312ef6:	nop
+   2e2312ef7:	nop
+   2e2312ef8:	nop
+   2e2312ef9:	nop
+   2e2312efa:	nop
+   2e2312efb:	nop
+   2e2312efc:	nop
+   2e2312efd:	nop
+   2e2312efe:	nop
+   2e2312eff:	nop
+   2e2312f00:	mov    $0x1,%eax
+   2e2312f05:	ret
+   2e2312f06:	nop
+   2e2312f07:	nop
+   2e2312f08:	nop
+   2e2312f09:	nop
+   2e2312f0a:	nop
+   2e2312f0b:	nop
+   2e2312f0c:	nop
+   2e2312f0d:	nop
+   2e2312f0e:	nop
+   2e2312f0f:	nop
+   2e2312f10:	push   %rbx
+   2e2312f11:	sub    $0x50,%rsp
+   2e2312f15:	movups %xmm6,0x40(%rsp)
+   2e2312f1a:	movq   %xmm0,%rbx
+   2e2312f1f:	mov    %rbx,%rdx
+   2e2312f22:	shr    $0x20,%rdx
+   2e2312f26:	mov    %edx,%eax
+   2e2312f28:	mov    %edx,%ecx
+   2e2312f2a:	and    $0xfffff,%eax
+   2e2312f2f:	and    $0x7ff00000,%ecx
+   2e2312f35:	or     %ebx,%eax
+   2e2312f37:	mov    %eax,%r8d
+   2e2312f3a:	or     %ecx,%r8d
+   2e2312f3d:	je     0x2e2312fe8
+   2e2312f43:	test   %ecx,%ecx
+   2e2312f45:	je     0x2e2312f4f
+   2e2312f47:	cmp    $0x7ff00000,%ecx
+   2e2312f4d:	je     0x2e2312f90
+   2e2312f4f:	test   %edx,%edx
+   2e2312f51:	js     0x2e2312fa0
+   2e2312f53:	movq   %rbx,%xmm1
+   2e2312f58:	ucomisd 0x22a0(%rip),%xmm1        # 0x2e2315200
+   2e2312f60:	jp     0x2e2312f69
+   2e2312f62:	movq   %rbx,%xmm0
+   2e2312f67:	je     0x2e2312f7e
+   2e2312f69:	mov    %rbx,0x38(%rsp)
+   2e2312f6e:	fldl   0x38(%rsp)
+   2e2312f72:	fsqrt
+   2e2312f74:	fstpl  0x38(%rsp)
+   2e2312f78:	movsd  0x38(%rsp),%xmm0
+   2e2312f7e:	movups 0x40(%rsp),%xmm6
+   2e2312f83:	add    $0x50,%rsp
+   2e2312f87:	pop    %rbx
+   2e2312f88:	ret
+   2e2312f89:	nopl   0x0(%rax)
+   2e2312f90:	test   %eax,%eax
+   2e2312f92:	jne    0x2e2313008
+   2e2312f94:	movsd  0x225c(%rip),%xmm0        # 0x2e23151f8
+   2e2312f9c:	test   %edx,%edx
+   2e2312f9e:	jns    0x2e2312f7e
+   2e2312fa0:	call   0x2e23131e0
+   2e2312fa5:	pxor   %xmm3,%xmm3
+   2e2312fa9:	movsd  0x223f(%rip),%xmm6        # 0x2e23151f0
+   2e2312fb1:	movq   %rbx,%xmm2
+   2e2312fb6:	movl   $0x21,(%rax)
+   2e2312fbc:	lea    0x221d(%rip),%rdx        # 0x2e23151e0
+   2e2312fc3:	mov    $0x1,%ecx
+   2e2312fc8:	movsd  %xmm6,0x20(%rsp)
+   2e2312fce:	call   0x2e23132b0
+   2e2312fd3:	movupd %xmm6,%xmm0
+   2e2312fd7:	movups 0x40(%rsp),%xmm6
+   2e2312fdc:	add    $0x50,%rsp
+   2e2312fe0:	pop    %rbx
+   2e2312fe1:	ret
+   2e2312fe2:	nopw   0x0(%rax,%rax,1)
+   2e2312fe8:	movsd  0x21f8(%rip),%xmm0        # 0x2e23151e8
+   2e2312ff0:	test   %edx,%edx
+   2e2312ff2:	js     0x2e2312f7e
+   2e2312ff4:	movups 0x40(%rsp),%xmm6
+   2e2312ff9:	pxor   %xmm0,%xmm0
+   2e2312ffd:	add    $0x50,%rsp
+   2e2313001:	pop    %rbx
+   2e2313002:	ret
+   2e2313003:	nopl   0x0(%rax,%rax,1)
+   2e2313008:	call   0x2e23131e0
+   2e231300d:	pxor   %xmm3,%xmm3
+   2e2313011:	movq   %rbx,%xmm2
+   2e2313016:	lea    0x21c3(%rip),%rdx        # 0x2e23151e0
+   2e231301d:	movl   $0x21,(%rax)
+   2e2313023:	mov    $0x1,%ecx
+   2e2313028:	mov    %rbx,0x20(%rsp)
+   2e231302d:	call   0x2e23132b0
+   2e2313032:	nop
+   2e2313033:	movups 0x40(%rsp),%xmm6
+   2e2313038:	movq   %rbx,%xmm0
+   2e231303d:	add    $0x50,%rsp
+   2e2313041:	pop    %rbx
+   2e2313042:	ret
+   2e2313043:	nop
+   2e2313044:	nop
+   2e2313045:	nop
+   2e2313046:	nop
+   2e2313047:	nop
+   2e2313048:	nop
+   2e2313049:	nop
+   2e231304a:	nop
+   2e231304b:	nop
+   2e231304c:	nop
+   2e231304d:	nop
+   2e231304e:	nop
+   2e231304f:	nop
+   2e2313050:	push   %rbx
+   2e2313051:	sub    $0x20,%rsp
+   2e2313055:	mov    %ecx,%ebx
+   2e2313057:	call   0x2e23131d0
+   2e231305c:	mov    %ebx,%ecx
+   2e231305e:	lea    (%rcx,%rcx,2),%rdx
+   2e2313062:	shl    $0x4,%rdx
+   2e2313066:	add    %rdx,%rax
+   2e2313069:	add    $0x20,%rsp
+   2e231306d:	pop    %rbx
+   2e231306e:	ret
+   2e231306f:	nop
+   2e2313070:	test   %rcx,%rcx
+   2e2313073:	je     0x2e2313087
+   2e2313075:	pxor   %xmm0,%xmm0
+   2e2313079:	xor    %eax,%eax
+   2e231307b:	movq   $0x0,0x10(%rcx)
+   2e2313083:	movups %xmm0,(%rcx)
+   2e2313086:	ret
+   2e2313087:	mov    $0xffffffff,%eax
+   2e231308c:	ret
+   2e231308d:	nopl   (%rax)
+   2e2313090:	push   %rbp
+   2e2313091:	push   %rdi
+   2e2313092:	push   %rsi
+   2e2313093:	push   %rbx
+   2e2313094:	sub    $0x28,%rsp
+   2e2313098:	mov    %rcx,%rbx
+   2e231309b:	mov    %rdx,%rdi
+   2e231309e:	test   %rcx,%rcx
+   2e23130a1:	je     0x2e2313158
+   2e23130a7:	mov    $0x8,%ecx
+   2e23130ac:	call   0x2e23131f0
+   2e23130b1:	cmpq   $0x0,(%rbx)
+   2e23130b5:	je     0x2e2313120
+   2e23130b7:	mov    0x8(%rbx),%rdx
+   2e23130bb:	mov    0x10(%rbx),%rax
+   2e23130bf:	cmp    %rdx,%rax
+   2e23130c2:	je     0x2e23130e8
+   2e23130c4:	lea    0x8(%rdx),%rax
+   2e23130c8:	mov    $0x8,%ecx
+   2e23130cd:	mov    %rax,0x8(%rbx)
+   2e23130d1:	mov    %rdi,(%rdx)
+   2e23130d4:	call   0x2e23131f8
+   2e23130d9:	xor    %eax,%eax
+   2e23130db:	add    $0x28,%rsp
+   2e23130df:	pop    %rbx
+   2e23130e0:	pop    %rsi
+   2e23130e1:	pop    %rdi
+   2e23130e2:	pop    %rbp
+   2e23130e3:	ret
+   2e23130e4:	nopl   0x0(%rax)
+   2e23130e8:	mov    (%rbx),%rcx
+   2e23130eb:	mov    %rdx,%rsi
+   2e23130ee:	sub    %rcx,%rsi
+   2e23130f1:	mov    %rsi,%rbp
+   2e23130f4:	sar    $0x3,%rbp
+   2e23130f8:	shl    $0x4,%rbp
+   2e23130fc:	mov    %rbp,%rdx
+   2e23130ff:	call   0x2e2313238
+   2e2313104:	test   %rax,%rax
+   2e2313107:	je     0x2e231314e
+   2e2313109:	mov    %rax,(%rbx)
+   2e231310c:	lea    (%rax,%rsi,1),%rdx
+   2e2313110:	add    %rbp,%rax
+   2e2313113:	mov    %rax,0x10(%rbx)
+   2e2313117:	jmp    0x2e23130c4
+   2e2313119:	nopl   0x0(%rax)
+   2e2313120:	mov    $0x8,%edx
+   2e2313125:	mov    $0x20,%ecx
+   2e231312a:	call   0x2e2313208
+   2e231312f:	mov    %rax,(%rbx)
+   2e2313132:	mov    %rax,%rdx
+   2e2313135:	test   %rax,%rax
+   2e2313138:	je     0x2e231314e
+   2e231313a:	mov    %rax,0x8(%rbx)
+   2e231313e:	lea    0x100(%rax),%rax
+   2e2313145:	mov    %rax,0x10(%rbx)
+   2e2313149:	jmp    0x2e23130bf
+   2e231314e:	mov    $0x8,%ecx
+   2e2313153:	call   0x2e23131f8
+   2e2313158:	or     $0xffffffff,%eax
+   2e231315b:	jmp    0x2e23130db
+   2e2313160:	push   %rdi
+   2e2313161:	push   %rsi
+   2e2313162:	push   %rbx
+   2e2313163:	sub    $0x20,%rsp
+   2e2313167:	mov    %rcx,%rdi
+   2e231316a:	mov    $0x8,%ecx
+   2e231316f:	call   0x2e23131f0
+   2e2313174:	mov    (%rdi),%rsi
+   2e2313177:	pxor   %xmm0,%xmm0
+   2e231317b:	mov    0x8(%rdi),%rbx
+   2e231317f:	movq   $0x0,0x10(%rdi)
+   2e2313187:	mov    $0x8,%ecx
+   2e231318c:	movups %xmm0,(%rdi)
+   2e231318f:	call   0x2e23131f8
+   2e2313194:	test   %rsi,%rsi
+   2e2313197:	je     0x2e23131bd
+   2e2313199:	sub    $0x8,%rbx
+   2e231319d:	cmp    %rsi,%rbx
+   2e23131a0:	jb     0x2e23131b5
+   2e23131a2:	mov    (%rbx),%rax
+   2e23131a5:	test   %rax,%rax
+   2e23131a8:	je     0x2e2313199
+   2e23131aa:	call   *%rax
+   2e23131ac:	sub    $0x8,%rbx
+   2e23131b0:	cmp    %rsi,%rbx
+   2e23131b3:	jae    0x2e23131a2
+   2e23131b5:	mov    %rsi,%rcx
+   2e23131b8:	call   0x2e2313210
+   2e23131bd:	xor    %eax,%eax
+   2e23131bf:	add    $0x20,%rsp
+   2e23131c3:	pop    %rbx
+   2e23131c4:	pop    %rsi
+   2e23131c5:	pop    %rdi
+   2e23131c6:	ret
    2e23131c7:	nop
-   2e23131c8:	jmp    *0x6f5e(%rip)        # 0x2e231a12c
+   2e23131c8:	nop
+   2e23131c9:	nop
+   2e23131ca:	nop
+   2e23131cb:	nop
+   2e23131cc:	nop
+   2e23131cd:	nop
    2e23131ce:	nop
    2e23131cf:	nop
-   2e23131d0:	jmp    *0x6f4e(%rip)        # 0x2e231a124
+   2e23131d0:	jmp    *0x6fa2(%rip)        # 0x2e231a178
    2e23131d6:	nop
    2e23131d7:	nop
-   2e23131d8:	nopl   0x0(%rax,%rax,1)
-   2e23131e0:	sub    $0x58,%rsp
-   2e23131e4:	mov    0x4f05(%rip),%rax        # 0x2e23180f0
-   2e23131eb:	test   %rax,%rax
-   2e23131ee:	je     0x2e231321c
-   2e23131f0:	movsd  0x80(%rsp),%xmm0
-   2e23131f9:	mov    %ecx,0x20(%rsp)
-   2e23131fd:	lea    0x20(%rsp),%rcx
-   2e2313202:	mov    %rdx,0x28(%rsp)
-   2e2313207:	movsd  %xmm2,0x30(%rsp)
-   2e231320d:	movsd  %xmm3,0x38(%rsp)
-   2e2313213:	movsd  %xmm0,0x40(%rsp)
-   2e2313219:	call   *%rax
-   2e231321b:	nop
-   2e231321c:	add    $0x58,%rsp
-   2e2313220:	ret
-   2e2313221:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e231322c:	nopl   0x0(%rax)
-   2e2313230:	mov    %rcx,0x4eb9(%rip)        # 0x2e23180f0
-   2e2313237:	jmp    0x2e2313240
-   2e231323c:	nop
-   2e231323d:	nop
+   2e23131d8:	jmp    *0x6faa(%rip)        # 0x2e231a188
+   2e23131de:	nop
+   2e23131df:	nop
+   2e23131e0:	jmp    *0x6faa(%rip)        # 0x2e231a190
+   2e23131e6:	nop
+   2e23131e7:	nop
+   2e23131e8:	jmp    *0x6faa(%rip)        # 0x2e231a198
+   2e23131ee:	nop
+   2e23131ef:	nop
+   2e23131f0:	jmp    *0x6faa(%rip)        # 0x2e231a1a0
+   2e23131f6:	nop
+   2e23131f7:	nop
+   2e23131f8:	jmp    *0x6faa(%rip)        # 0x2e231a1a8
+   2e23131fe:	nop
+   2e23131ff:	nop
+   2e2313200:	jmp    *0x6faa(%rip)        # 0x2e231a1b0
+   2e2313206:	nop
+   2e2313207:	nop
+   2e2313208:	jmp    *0x6faa(%rip)        # 0x2e231a1b8
+   2e231320e:	nop
+   2e231320f:	nop
+   2e2313210:	jmp    *0x6faa(%rip)        # 0x2e231a1c0
+   2e2313216:	nop
+   2e2313217:	nop
+   2e2313218:	jmp    *0x6faa(%rip)        # 0x2e231a1c8
+   2e231321e:	nop
+   2e231321f:	nop
+   2e2313220:	jmp    *0x6faa(%rip)        # 0x2e231a1d0
+   2e2313226:	nop
+   2e2313227:	nop
+   2e2313228:	jmp    *0x6faa(%rip)        # 0x2e231a1d8
+   2e231322e:	nop
+   2e231322f:	nop
+   2e2313230:	jmp    *0x6faa(%rip)        # 0x2e231a1e0
+   2e2313236:	nop
+   2e2313237:	nop
+   2e2313238:	jmp    *0x6faa(%rip)        # 0x2e231a1e8
    2e231323e:	nop
    2e231323f:	nop
-   2e2313240:	jmp    *0x6f36(%rip)        # 0x2e231a17c
+   2e2313240:	jmp    *0x6faa(%rip)        # 0x2e231a1f0
    2e2313246:	nop
    2e2313247:	nop
-   2e2313248:	nopl   0x0(%rax,%rax,1)
-   2e2313250:	jmp    0x2e2311380
-   2e2313255:	nop
+   2e2313248:	jmp    *0x6faa(%rip)        # 0x2e231a1f8
+   2e231324e:	nop
+   2e231324f:	nop
+   2e2313250:	jmp    *0x6faa(%rip)        # 0x2e231a200
    2e2313256:	nop
    2e2313257:	nop
-   2e2313258:	nop
-   2e2313259:	nop
-   2e231325a:	nop
-   2e231325b:	nop
-   2e231325c:	nop
-   2e231325d:	nop
-   2e231325e:	nop
-   2e231325f:	nop
-   2e2313260:	(bad)
-   2e2313261:	(bad)
-   2e2313262:	(bad)
-   2e2313263:	(bad)
-   2e2313264:	(bad)
-   2e2313265:	(bad)
-   2e2313266:	(bad)
-   2e2313267:	call   *0x32(%rax)
-   2e231326a:	xor    %esp,%edx
-   2e231326c:	add    (%rax),%al
-	...
-   2e2313276:	add    %al,(%rax)
-   2e2313278:	(bad)
-   2e2313279:	(bad)
-   2e231327a:	(bad)
-   2e231327b:	(bad)
-   2e231327c:	(bad)
-   2e231327d:	(bad)
-   2e231327e:	(bad)
-   2e231327f:	incl   (%rax)
-   2e2313281:	add    %al,(%rax)
-   2e2313283:	add    %al,(%rax)
-   2e2313285:	add    %al,(%rax)
+   2e2313258:	nopl   0x0(%rax,%rax,1)
+   2e2313260:	jmp    *0x6f02(%rip)        # 0x2e231a168
+   2e2313266:	nop
+   2e2313267:	nop
+   2e2313268:	jmp    *0x6ef2(%rip)        # 0x2e231a160
+   2e231326e:	nop
+   2e231326f:	nop
+   2e2313270:	jmp    *0x6ee2(%rip)        # 0x2e231a158
+   2e2313276:	nop
+   2e2313277:	nop
+   2e2313278:	jmp    *0x6ed2(%rip)        # 0x2e231a150
+   2e231327e:	nop
+   2e231327f:	nop
+   2e2313280:	jmp    *0x6ec2(%rip)        # 0x2e231a148
+   2e2313286:	nop
+   2e2313287:	nop
+   2e2313288:	jmp    *0x6eb2(%rip)        # 0x2e231a140
+   2e231328e:	nop
+   2e231328f:	nop
+   2e2313290:	jmp    *0x6ea2(%rip)        # 0x2e231a138
+   2e2313296:	nop
+   2e2313297:	nop
+   2e2313298:	jmp    *0x6e92(%rip)        # 0x2e231a130
+   2e231329e:	nop
+   2e231329f:	nop
+   2e23132a0:	jmp    *0x6e82(%rip)        # 0x2e231a128
+   2e23132a6:	nop
+   2e23132a7:	nop
+   2e23132a8:	nopl   0x0(%rax,%rax,1)
+   2e23132b0:	sub    $0x58,%rsp
+   2e23132b4:	mov    0x4e55(%rip),%rax        # 0x2e2318110
+   2e23132bb:	unpcklpd %xmm3,%xmm2
+   2e23132bf:	test   %rax,%rax
+   2e23132c2:	je     0x2e23132e9
+   2e23132c4:	movsd  0x80(%rsp),%xmm0
+   2e23132cd:	mov    %ecx,0x20(%rsp)
+   2e23132d1:	lea    0x20(%rsp),%rcx
+   2e23132d6:	mov    %rdx,0x28(%rsp)
+   2e23132db:	movups %xmm2,0x30(%rsp)
+   2e23132e0:	movsd  %xmm0,0x40(%rsp)
+   2e23132e6:	call   *%rax
+   2e23132e8:	nop
+   2e23132e9:	add    $0x58,%rsp
+   2e23132ed:	ret
+   2e23132ee:	xchg   %ax,%ax
+   2e23132f0:	mov    %rcx,0x4e19(%rip)        # 0x2e2318110
+   2e23132f7:	jmp    0x2e2313300
+   2e23132fc:	nop
+   2e23132fd:	nop
+   2e23132fe:	nop
+   2e23132ff:	nop
+   2e2313300:	jmp    *0x6e7a(%rip)        # 0x2e231a180
+   2e2313306:	nop
+   2e2313307:	nop
+   2e2313308:	nopl   0x0(%rax,%rax,1)
+   2e2313310:	jmp    0x2e2311350
+   2e2313315:	nop
+   2e2313316:	nop
+   2e2313317:	nop
+   2e2313318:	nop
+   2e2313319:	nop
+   2e231331a:	nop
+   2e231331b:	nop
+   2e231331c:	nop
+   2e231331d:	nop
+   2e231331e:	nop
+   2e231331f:	nop
+   2e2313320:	(bad)
+   2e2313321:	(bad)
+   2e2313322:	(bad)
+   2e2313323:	(bad)
+   2e2313324:	(bad)
+   2e2313325:	(bad)
+   2e2313326:	(bad)
+   2e2313327:	call   *(%rax)
+   2e2313329:	xor    (%rcx),%esi
+   2e231332b:	loop   0x2e231332f
+	...
+   2e2313335:	add    %al,(%rax)
+   2e2313337:	add    %bh,%bh
+   2e2313339:	(bad)
+   2e231333a:	(bad)
+   2e231333b:	(bad)
+   2e231333c:	(bad)
+   2e231333d:	(bad)
+   2e231333e:	(bad)
+   2e231333f:	incl   (%rax)
+   2e2313341:	add    %al,(%rax)
+   2e2313343:	add    %al,(%rax)
+   2e2313345:	add    %al,(%rax)
 	...
 
 Disassembly of section .data:
 
 00000002e2314000 <.data>:
    2e2314000:	add    %eax,(%rax)
 	...
    2e231400e:	add    %al,(%rax)
-   2e2314010:	xorb   $0x31,(%rdx)
+   2e2314010:	rex xor (%rcx),%esi
    2e2314013:	loop   0x2e2314017
 	...
    2e231401d:	add    %al,(%rax)
    2e231401f:	add    %bh,%bh
    2e2314021:	(bad)
    2e2314022:	(bad)
    2e2314023:	(bad)
@@ -3079,28 +3099,26 @@
    2e2314027:	incl   (%rax)
    2e2314029:	add    %al,(%rax)
    2e231402b:	add    %al,(%rax)
    2e231402d:	add    %al,(%rax)
    2e231402f:	add    %al,(%rdx)
 	...
    2e231403d:	add    %al,(%rax)
-   2e231403f:	add    %dl,%al
-   2e2314041:	xor    %dh,(%rcx)
-   2e2314043:	loop   0x2e2314047
-   2e2314045:	add    %al,(%rax)
-   2e2314047:	add    %dh,%al
-   2e2314049:	(bad)
-   2e231404a:	xor    %esp,%edx
-   2e231404c:	add    (%rax),%al
+   2e231403f:	add    %dl,0x30(%rax)
+   2e2314042:	xor    %esp,%edx
+   2e2314044:	add    (%rax),%al
+	...
    2e231404e:	add    %al,(%rax)
-   2e2314050:	shrb   $0x31,(%rdi)
+   2e2314050:	(bad)
+   2e2314051:	xor    %esi,(%rcx)
    2e2314053:	loop   0x2e2314057
-	...
+   2e2314055:	add    %al,(%rax)
+   2e2314057:	add    %dl,0x2e23130(%rax)
    2e231405d:	add    %al,(%rax)
-   2e231405f:	add    %dl,0x31(%rax)
+   2e231405f:	add    %dh,0x30(%rax)
    2e2314062:	xor    %esp,%edx
    2e2314064:	add    (%rax),%al
 	...
 
 Disassembly of section .rdata:
 
 00000002e2315000 <.rdata>:
@@ -3110,26 +3128,26 @@
    2e2315006:	clc
    2e2315007:	jg     0x2e2315009
    2e2315009:	add    %al,(%rax)
    2e231500b:	add    %al,(%rax)
    2e231500d:	add    %ah,%al
    2e231500f:	(bad)
 	...
-   2e2315020:	rex and %esi,(%rcx)
+   2e2315020:	push   %rax
+   2e2315021:	and    (%rcx),%dh
    2e2315023:	loop   0x2e2315027
 	...
    2e2315041:	shlb   $0xe2,(%rcx)
    2e2315044:	add    (%rax),%al
    2e2315046:	add    %al,(%rax)
    2e2315048:	or     %al,%al
    2e231504a:	xor    %esp,%edx
    2e231504c:	add    (%rax),%al
    2e231504e:	add    %al,(%rax)
-   2e2315050:	cmp    $0x80,%al
-   2e2315052:	xor    %esp,%edx
+   2e2315050:	rex.WR xorb $0xe2,(%rcx)
    2e2315054:	add    (%rax),%al
    2e2315056:	add    %al,(%rax)
    2e2315058:	xor    %dh,0x2e231(%rax)
 	...
    2e231507e:	add    %al,(%rax)
    2e2315080:	imul   $0x36772d77,0x67(%r14),%r13
    2e2315088:	xor    $0x20,%al
@@ -3216,635 +3234,575 @@
    2e231516b:	insb   (%dx),%es:(%rdi)
    2e231516c:	outsl  %ds:(%rsi),(%dx)
    2e231516d:	movsxd 0x74(%rcx),%esp
    2e2315170:	imul   $0x74696220,0x6e(%rdi),%ebp
    2e2315177:	and    %dh,0x69(%rbx)
    2e231517a:	jp     0x2e23151e1
    2e231517c:	and    %ah,0xa2e64(%rip)        # 0x2e23b7fe6
+   2e2315182:	add    %al,(%rax)
+   2e2315184:	add    %al,(%rax)
+   2e2315186:	add    %al,(%rax)
+   2e2315188:	and    $0x69622064,%eax
+   2e231518d:	je     0x2e23151af
+   2e231518f:	jo     0x2e2315204
+   2e2315191:	gs jne 0x2e23151f8
+   2e2315194:	outsl  %ds:(%rsi),(%dx)
+   2e2315195:	and    %dh,0x65(%rdx)
+   2e2315198:	insb   (%dx),%es:(%rdi)
+   2e2315199:	outsl  %ds:(%rsi),(%dx)
+   2e231519a:	movsxd 0x74(%rcx),%esp
+   2e231519d:	imul   $0x20746120,0x6e(%rdi),%ebp
+   2e23151a4:	and    $0x756f2070,%eax
+   2e23151a9:	je     0x2e23151cb
+   2e23151ab:	outsl  %ds:(%rsi),(%dx)
+   2e23151ac:	data16 and %dh,0x61(%rdx)
+   2e23151b0:	outsb  %ds:(%rsi),(%dx)
+   2e23151b1:	addr32 gs sub $0x20,%al
+   2e23151b5:	je     0x2e2315218
+   2e23151b7:	jb     0x2e2315220
+   2e23151b9:	gs je  0x2e2315225
+   2e23151bc:	outsb  %ds:(%rsi),(%dx)
+   2e23151bd:	and    %ah,0x79202c70(%eip)        # 0x35b517e34
+   2e23151c4:	imul   $0x676e6964,0x6c(%rbp),%esp
+   2e23151cb:	and    %dh,0x65(%rax,%rbp,2)
+   2e23151cf:	and    %dh,0x61(%rsi)
+   2e23151d2:	insb   (%dx),%es:(%rdi)
+   2e23151d3:	jne    0x2e231523a
+   2e23151d5:	and    %ah,0xa2e70(%rip)        # 0x2e23b804b
+   2e23151db:	add    %al,(%rax)
+   2e23151dd:	add    %al,(%rax)
+   2e23151df:	add    %dh,0x71(%rbx)
+   2e23151e2:	jb     0x2e2315258
+	...
+   2e23151ec:	add    %al,(%rax)
+   2e23151ee:	add    %al,0x0(%rax)
+   2e23151f4:	add    %al,(%rax)
+   2e23151f6:	clc
+   2e23151f7:	incl   (%rax)
+   2e23151f9:	add    %al,(%rax)
+   2e23151fb:	add    %al,(%rax)
+   2e23151fd:	add    %dh,%al
+   2e23151ff:	jg     0x2e2315201
+   2e2315201:	add    %al,(%rax)
+   2e2315203:	add    %al,(%rax)
+   2e2315205:	add    %dh,%al
+   2e2315207:	(bad)
 	...
-   2e231518e:	add    %al,(%rax)
-   2e2315190:	jae    0x2e2315203
-   2e2315192:	jb     0x2e2315208
-	...
-   2e231519c:	add    %al,(%rax)
-   2e231519e:	lock jg 0x2e23151a1
-   2e23151a1:	add    %al,(%rax)
-   2e23151a3:	add    %al,(%rax)
-   2e23151a5:	add    %bh,%al
-   2e23151a7:	incl   (%rax)
-   2e23151a9:	add    %al,(%rax)
-   2e23151ab:	add    %al,(%rax)
-   2e23151ad:	add    %al,(%rax)
-   2e23151af:	addb   $0x0,(%rax)
-   2e23151b2:	add    %al,(%rax)
-   2e23151b4:	add    %al,(%rax)
-   2e23151b6:	lock (bad)
-	...
-   2e23151c0:	xor    %al,0x31(%rax)
-   2e23151c3:	loop   0x2e23151c7
-	...
-   2e23151cd:	add    %al,(%rax)
-   2e23151cf:	add    %ah,0x32(%rax)
-   2e23151d2:	xor    %esp,%edx
-   2e23151d4:	add    (%rax),%al
-	...
-   2e23151de:	add    %al,(%rax)
-   2e23151e0:	(bad)
-   2e23151e1:	push   %rbp
-   2e23151e2:	xor    %esp,%edx
-   2e23151e4:	add    (%rax),%al
-	...
-   2e23151ee:	add    %al,(%rax)
-   2e23151f0:	(bad)
-   2e23151f1:	push   %rbp
-   2e23151f2:	xor    %esp,%edx
-   2e23151f4:	add    (%rax),%al
-	...
-   2e23151fe:	add    %al,(%rax)
-   2e2315200:	and    %dl,0x31(%rax)
-   2e2315203:	loop   0x2e2315207
-	...
-   2e2315211:	add    %dh,(%rcx)
+   2e2315210:	xor    %al,0x31(%rax)
    2e2315213:	loop   0x2e2315217
 	...
    2e231521d:	add    %al,(%rax)
-   2e231521f:	add    %ah,(%rax,%rax,2)
-   2e2315222:	xor    %esp,%edx
-   2e2315224:	add    (%rax),%al
+   2e231521f:	add    %ah,(%rax)
+   2e2315221:	xor    (%rcx),%esi
+   2e2315223:	loop   0x2e2315227
+	...
+   2e231522d:	add    %al,(%rax)
+   2e231522f:	add    %dh,0x2e23155(%rax)
+	...
+   2e231523d:	add    %al,(%rax)
+   2e231523f:	add    %dh,0x2e23155(%rax)
+	...
+   2e231524d:	add    %al,(%rax)
+   2e231524f:	add    %ah,(%rax)
+   2e2315251:	push   %rax
+   2e2315252:	xor    %esp,%edx
+   2e2315254:	add    (%rax),%al
 	...
-   2e231522e:	add    %al,(%rax)
-   2e2315230:	or     %al,0x2e231(%rcx)
-	...
-   2e231523e:	add    %al,(%rax)
-   2e2315240:	add    %al,0x2e231(%rcx)
-	...
-   2e231524e:	add    %al,(%rax)
-   2e2315250:	add    %dh,0x2e231(%rax)
-	...
-   2e231525e:	add    %al,(%rax)
-   2e2315260:	or     %dh,0x2e231(%rax)
+   2e2315262:	xor    %esp,%edx
+   2e2315264:	add    (%rax),%al
 	...
    2e231526e:	add    %al,(%rax)
-   2e2315270:	adc    %dh,0x2e231(%rax)
+   2e2315270:	push   %rax
+   2e2315271:	xorb   $0xe2,(%rcx)
+   2e2315274:	add    (%rax),%al
 	...
    2e231527e:	add    %al,(%rax)
-   2e2315280:	and    %dh,0x2e231(%rax)
+   2e2315280:	and    $0x40,%al
+   2e2315282:	xor    %esp,%edx
+   2e2315284:	add    (%rax),%al
 	...
    2e231528e:	add    %al,(%rax)
-   2e2315290:	rex xorb $0xe2,(%rcx)
-   2e2315294:	add    (%rax),%al
+   2e2315290:	xor    %al,0x2e231(%rax)
 	...
    2e231529e:	add    %al,(%rax)
-   2e23152a0:	rex.RXB
-   2e23152a1:	rex.XB
-   2e23152a2:	rex.XB cmp (%r8),%spl
-   2e23152a5:	sub    %al,0x4e(%rdi)
-   2e23152a8:	push   %rbp
-   2e23152a9:	sub    %esp,(%rax)
-   2e23152ab:	cmp    %ebp,(%rsi)
-   2e23152ad:	xor    0x336e6977(%rip),%ebp        # 0x3159fbc2a
-   2e23152b3:	xor    (%rax),%ah
-   2e23152b5:	xor    (%rax),%dh
-   2e23152b7:	xor    (%rax),%dh
-   2e23152b9:	xor    %dh,(%rbx)
-   2e23152bb:	xor    (%rax),%dh
-   2e23152bd:	add    %al,(%rax)
-   2e23152bf:	add    %al,0x43(%rdi)
-   2e23152c2:	rex.XB cmp (%r8),%spl
-   2e23152c5:	sub    %al,0x4e(%rdi)
-   2e23152c8:	push   %rbp
-   2e23152c9:	sub    %esp,(%rax)
-   2e23152cb:	xor    %esi,(%rax)
-   2e23152cd:	sub    $0x336e6977,%eax
-   2e23152d2:	xor    (%rax),%ah
-   2e23152d4:	xor    (%rax),%dh
-   2e23152d6:	xor    (%rdx),%dh
-   2e23152d8:	xor    %dh,(%rcx)
-   2e23152da:	xor    %esi,(%rbx)
-   2e23152dc:	add    %al,(%rax)
+   2e23152a0:	cmp    %al,0x2e231(%rax)
+	...
+   2e23152ae:	add    %al,(%rax)
+   2e23152b0:	add    %dh,0x2e231(%rax)
+	...
+   2e23152be:	add    %al,(%rax)
+   2e23152c0:	or     %dh,0x2e231(%rax)
+	...
+   2e23152ce:	add    %al,(%rax)
+   2e23152d0:	adc    %dh,0x2e231(%rax)
+	...
    2e23152de:	add    %al,(%rax)
-   2e23152e0:	rex.RXB
-   2e23152e1:	rex.XB
-   2e23152e2:	rex.XB cmp (%r8),%spl
-   2e23152e5:	sub    %al,0x4e(%rdi)
-   2e23152e8:	push   %rbp
-   2e23152e9:	sub    %esp,(%rax)
-   2e23152eb:	xor    %esi,(%rax)
-   2e23152ed:	sub    $0x336e6977,%eax
-   2e23152f2:	xor    (%rax),%ah
-   2e23152f4:	xor    (%rax),%dh
-   2e23152f6:	xor    (%rdx),%dh
-   2e23152f8:	xor    %dh,(%rcx)
-   2e23152fa:	xor    %esi,(%rbx)
-   2e23152fc:	add    %al,(%rax)
-   2e23152fe:	add    %al,(%rax)
-   2e2315300:	rex.RXB
-   2e2315301:	rex.XB
-   2e2315302:	rex.XB cmp (%r8),%spl
-   2e2315305:	sub    %al,0x4e(%rdi)
-   2e2315308:	push   %rbp
-   2e2315309:	sub    %esp,(%rax)
-   2e231530b:	cmp    %ebp,(%rsi)
-   2e231530d:	xor    0x336e6977(%rip),%ebp        # 0x3159fbc8a
-   2e2315313:	xor    (%rax),%ah
-   2e2315315:	xor    (%rax),%dh
-   2e2315317:	xor    (%rax),%dh
-   2e2315319:	xor    %dh,(%rbx)
-   2e231531b:	xor    (%rax),%dh
-   2e231531d:	add    %al,(%rax)
-   2e231531f:	add    %al,0x43(%rdi)
-   2e2315322:	rex.XB cmp (%r8),%spl
-   2e2315325:	sub    %al,0x4e(%rdi)
-   2e2315328:	push   %rbp
-   2e2315329:	sub    %esp,(%rax)
-   2e231532b:	cmp    %ebp,(%rsi)
-   2e231532d:	xor    0x336e6977(%rip),%ebp        # 0x3159fbcaa
-   2e2315333:	xor    (%rax),%ah
-   2e2315335:	xor    (%rax),%dh
-   2e2315337:	xor    (%rax),%dh
-   2e2315339:	xor    %dh,(%rbx)
-   2e231533b:	xor    (%rax),%dh
-   2e231533d:	add    %al,(%rax)
-   2e231533f:	add    %al,0x43(%rdi)
-   2e2315342:	rex.XB cmp (%r8),%spl
-   2e2315345:	sub    %al,0x4e(%rdi)
-   2e2315348:	push   %rbp
-   2e2315349:	sub    %esp,(%rax)
-   2e231534b:	cmp    %ebp,(%rsi)
-   2e231534d:	xor    0x336e6977(%rip),%ebp        # 0x3159fbcca
-   2e2315353:	xor    (%rax),%ah
-   2e2315355:	xor    (%rax),%dh
-   2e2315357:	xor    (%rax),%dh
-   2e2315359:	xor    %dh,(%rbx)
-   2e231535b:	xor    (%rax),%dh
-   2e231535d:	add    %al,(%rax)
-   2e231535f:	add    %al,0x43(%rdi)
-   2e2315362:	rex.XB cmp (%r8),%spl
-   2e2315365:	sub    %al,0x4e(%rdi)
-   2e2315368:	push   %rbp
-   2e2315369:	sub    %esp,(%rax)
-   2e231536b:	cmp    %ebp,(%rsi)
-   2e231536d:	xor    0x336e6977(%rip),%ebp        # 0x3159fbcea
-   2e2315373:	xor    (%rax),%ah
-   2e2315375:	xor    (%rax),%dh
-   2e2315377:	xor    (%rax),%dh
-   2e2315379:	xor    %dh,(%rbx)
-   2e231537b:	xor    (%rax),%dh
-   2e231537d:	add    %al,(%rax)
-   2e231537f:	add    %al,0x43(%rdi)
-   2e2315382:	rex.XB cmp (%r8),%spl
-   2e2315385:	sub    %al,0x4e(%rdi)
-   2e2315388:	push   %rbp
-   2e2315389:	sub    %esp,(%rax)
-   2e231538b:	cmp    %ebp,(%rsi)
-   2e231538d:	xor    0x336e6977(%rip),%ebp        # 0x3159fbd0a
-   2e2315393:	xor    (%rax),%ah
-   2e2315395:	xor    (%rax),%dh
-   2e2315397:	xor    (%rax),%dh
-   2e2315399:	xor    %dh,(%rbx)
-   2e231539b:	xor    (%rax),%dh
-   2e231539d:	add    %al,(%rax)
-   2e231539f:	add    %al,0x43(%rdi)
-   2e23153a2:	rex.XB cmp (%r8),%spl
-   2e23153a5:	sub    %al,0x4e(%rdi)
-   2e23153a8:	push   %rbp
-   2e23153a9:	sub    %esp,(%rax)
-   2e23153ab:	cmp    %ebp,(%rsi)
-   2e23153ad:	xor    0x336e6977(%rip),%ebp        # 0x3159fbd2a
-   2e23153b3:	xor    (%rax),%ah
-   2e23153b5:	xor    (%rax),%dh
-   2e23153b7:	xor    (%rax),%dh
-   2e23153b9:	xor    %dh,(%rbx)
-   2e23153bb:	xor    (%rax),%dh
-   2e23153bd:	add    %al,(%rax)
-   2e23153bf:	add    %al,0x43(%rdi)
-   2e23153c2:	rex.XB cmp (%r8),%spl
-   2e23153c5:	sub    %al,0x4e(%rdi)
-   2e23153c8:	push   %rbp
-   2e23153c9:	sub    %esp,(%rax)
-   2e23153cb:	cmp    %ebp,(%rsi)
-   2e23153cd:	xor    0x336e6977(%rip),%ebp        # 0x3159fbd4a
-   2e23153d3:	xor    (%rax),%ah
-   2e23153d5:	xor    (%rax),%dh
-   2e23153d7:	xor    (%rax),%dh
-   2e23153d9:	xor    %dh,(%rbx)
-   2e23153db:	xor    (%rax),%dh
-   2e23153dd:	add    %al,(%rax)
-   2e23153df:	add    %al,0x43(%rdi)
-   2e23153e2:	rex.XB cmp (%r8),%spl
-   2e23153e5:	sub    %al,0x4e(%rdi)
-   2e23153e8:	push   %rbp
-   2e23153e9:	sub    %esp,(%rax)
-   2e23153eb:	cmp    %ebp,(%rsi)
-   2e23153ed:	xor    0x336e6977(%rip),%ebp        # 0x3159fbd6a
-   2e23153f3:	xor    (%rax),%ah
-   2e23153f5:	xor    (%rax),%dh
-   2e23153f7:	xor    (%rax),%dh
-   2e23153f9:	xor    %dh,(%rbx)
-   2e23153fb:	xor    (%rax),%dh
-   2e23153fd:	add    %al,(%rax)
-   2e23153ff:	add    %al,0x43(%rdi)
-   2e2315402:	rex.XB cmp (%r8),%spl
-   2e2315405:	sub    %al,0x4e(%rdi)
-   2e2315408:	push   %rbp
-   2e2315409:	sub    %esp,(%rax)
-   2e231540b:	cmp    %ebp,(%rsi)
-   2e231540d:	xor    0x336e6977(%rip),%ebp        # 0x3159fbd8a
-   2e2315413:	xor    (%rax),%ah
-   2e2315415:	xor    (%rax),%dh
-   2e2315417:	xor    (%rax),%dh
-   2e2315419:	xor    %dh,(%rbx)
-   2e231541b:	xor    (%rax),%dh
-   2e231541d:	add    %al,(%rax)
-   2e231541f:	add    %al,0x43(%rdi)
-   2e2315422:	rex.XB cmp (%r8),%spl
-   2e2315425:	sub    %al,0x4e(%rdi)
-   2e2315428:	push   %rbp
-   2e2315429:	sub    %esp,(%rax)
-   2e231542b:	cmp    %ebp,(%rsi)
-   2e231542d:	xor    0x336e6977(%rip),%ebp        # 0x3159fbdaa
-   2e2315433:	xor    (%rax),%ah
-   2e2315435:	xor    (%rax),%dh
-   2e2315437:	xor    (%rax),%dh
-   2e2315439:	xor    %dh,(%rbx)
-   2e231543b:	xor    (%rax),%dh
-   2e231543d:	add    %al,(%rax)
-   2e231543f:	add    %al,0x43(%rdi)
-   2e2315442:	rex.XB cmp (%r8),%spl
-   2e2315445:	sub    %al,0x4e(%rdi)
-   2e2315448:	push   %rbp
-   2e2315449:	sub    %esp,(%rax)
-   2e231544b:	cmp    %ebp,(%rsi)
-   2e231544d:	xor    0x336e6977(%rip),%ebp        # 0x3159fbdca
-   2e2315453:	xor    (%rax),%ah
-   2e2315455:	xor    (%rax),%dh
-   2e2315457:	xor    (%rax),%dh
-   2e2315459:	xor    %dh,(%rbx)
-   2e231545b:	xor    (%rax),%dh
-   2e231545d:	add    %al,(%rax)
-   2e231545f:	add    %al,0x43(%rdi)
-   2e2315462:	rex.XB cmp (%r8),%spl
-   2e2315465:	sub    %al,0x4e(%rdi)
-   2e2315468:	push   %rbp
-   2e2315469:	sub    %esp,(%rax)
-   2e231546b:	xor    %esi,(%rax)
-   2e231546d:	sub    $0x336e6977,%eax
-   2e2315472:	xor    (%rax),%ah
-   2e2315474:	xor    (%rax),%dh
-   2e2315476:	xor    (%rdx),%dh
-   2e2315478:	xor    %dh,(%rcx)
-   2e231547a:	xor    %esi,(%rbx)
-   2e231547c:	add    %al,(%rax)
-   2e231547e:	add    %al,(%rax)
-   2e2315480:	rex.RXB
-   2e2315481:	rex.XB
-   2e2315482:	rex.XB cmp (%r8),%spl
-   2e2315485:	sub    %al,0x4e(%rdi)
-   2e2315488:	push   %rbp
-   2e2315489:	sub    %esp,(%rax)
-   2e231548b:	cmp    %ebp,(%rsi)
-   2e231548d:	xor    0x336e6977(%rip),%ebp        # 0x3159fbe0a
-   2e2315493:	xor    (%rax),%ah
-   2e2315495:	xor    (%rax),%dh
-   2e2315497:	xor    (%rax),%dh
-   2e2315499:	xor    %dh,(%rbx)
-   2e231549b:	xor    (%rax),%dh
-   2e231549d:	add    %al,(%rax)
-   2e231549f:	add    %al,0x43(%rdi)
-   2e23154a2:	rex.XB cmp (%r8),%spl
-   2e23154a5:	sub    %al,0x4e(%rdi)
-   2e23154a8:	push   %rbp
-   2e23154a9:	sub    %esp,(%rax)
-   2e23154ab:	cmp    %ebp,(%rsi)
-   2e23154ad:	xor    0x336e6977(%rip),%ebp        # 0x3159fbe2a
-   2e23154b3:	xor    (%rax),%ah
-   2e23154b5:	xor    (%rax),%dh
-   2e23154b7:	xor    (%rax),%dh
-   2e23154b9:	xor    %dh,(%rbx)
-   2e23154bb:	xor    (%rax),%dh
-   2e23154bd:	add    %al,(%rax)
-   2e23154bf:	add    %al,0x43(%rdi)
-   2e23154c2:	rex.XB cmp (%r8),%spl
-   2e23154c5:	sub    %al,0x4e(%rdi)
-   2e23154c8:	push   %rbp
-   2e23154c9:	sub    %esp,(%rax)
-   2e23154cb:	cmp    %ebp,(%rsi)
-   2e23154cd:	xor    0x336e6977(%rip),%ebp        # 0x3159fbe4a
-   2e23154d3:	xor    (%rax),%ah
-   2e23154d5:	xor    (%rax),%dh
-   2e23154d7:	xor    (%rax),%dh
-   2e23154d9:	xor    %dh,(%rbx)
-   2e23154db:	xor    (%rax),%dh
-   2e23154dd:	add    %al,(%rax)
-   2e23154df:	add    %al,0x43(%rdi)
-   2e23154e2:	rex.XB cmp (%r8),%spl
-   2e23154e5:	sub    %al,0x4e(%rdi)
-   2e23154e8:	push   %rbp
-   2e23154e9:	sub    %esp,(%rax)
-   2e23154eb:	cmp    %ebp,(%rsi)
-   2e23154ed:	xor    0x336e6977(%rip),%ebp        # 0x3159fbe6a
-   2e23154f3:	xor    (%rax),%ah
-   2e23154f5:	xor    (%rax),%dh
-   2e23154f7:	xor    (%rax),%dh
-   2e23154f9:	xor    %dh,(%rbx)
-   2e23154fb:	xor    (%rax),%dh
-   2e23154fd:	add    %al,(%rax)
-   2e23154ff:	add    %al,0x43(%rdi)
-   2e2315502:	rex.XB cmp (%r8),%spl
-   2e2315505:	sub    %al,0x4e(%rdi)
-   2e2315508:	push   %rbp
-   2e2315509:	sub    %esp,(%rax)
-   2e231550b:	cmp    %ebp,(%rsi)
-   2e231550d:	xor    0x336e6977(%rip),%ebp        # 0x3159fbe8a
-   2e2315513:	xor    (%rax),%ah
-   2e2315515:	xor    (%rax),%dh
-   2e2315517:	xor    (%rax),%dh
-   2e2315519:	xor    %dh,(%rbx)
-   2e231551b:	xor    (%rax),%dh
-   2e231551d:	add    %al,(%rax)
-   2e231551f:	add    %al,0x43(%rdi)
-   2e2315522:	rex.XB cmp (%r8),%spl
-   2e2315525:	sub    %al,0x4e(%rdi)
-   2e2315528:	push   %rbp
-   2e2315529:	sub    %esp,(%rax)
-   2e231552b:	cmp    %ebp,(%rsi)
-   2e231552d:	xor    0x336e6977(%rip),%ebp        # 0x3159fbeaa
-   2e2315533:	xor    (%rax),%ah
-   2e2315535:	xor    (%rax),%dh
-   2e2315537:	xor    (%rax),%dh
-   2e2315539:	xor    %dh,(%rbx)
-   2e231553b:	xor    (%rax),%dh
-   2e231553d:	add    %al,(%rax)
-   2e231553f:	add    %al,0x43(%rdi)
-   2e2315542:	rex.XB cmp (%r8),%spl
-   2e2315545:	sub    %al,0x4e(%rdi)
-   2e2315548:	push   %rbp
-   2e2315549:	sub    %esp,(%rax)
-   2e231554b:	xor    %esi,(%rax)
-   2e231554d:	sub    $0x336e6977,%eax
-   2e2315552:	xor    (%rax),%ah
-   2e2315554:	xor    (%rax),%dh
-   2e2315556:	xor    (%rdx),%dh
-   2e2315558:	xor    %dh,(%rcx)
-   2e231555a:	xor    %esi,(%rbx)
-   2e231555c:	add    %al,(%rax)
+   2e23152e0:	and    %dh,0x2e231(%rax)
+	...
+   2e23152ee:	add    %al,(%rax)
+   2e23152f0:	rex.RXB
+   2e23152f1:	rex.XB
+   2e23152f2:	rex.XB cmp (%r8),%spl
+   2e23152f5:	sub    %al,0x4e(%rdi)
+   2e23152f8:	push   %rbp
+   2e23152f9:	sub    %esp,(%rax)
+   2e23152fb:	xor    %esi,(%rdx)
+   2e23152fd:	sub    $0x336e6977,%eax
+   2e2315302:	xor    (%rax),%al
+	...
+   2e2315310:	rex.RXB
+   2e2315311:	rex.XB
+   2e2315312:	rex.XB cmp (%r8),%spl
+   2e2315315:	sub    %al,0x4e(%rdi)
+   2e2315318:	push   %rbp
+   2e2315319:	sub    %esp,(%rax)
+   2e231531b:	xor    %esi,(%rdx)
+   2e231531d:	sub    $0x336e6977,%eax
+   2e2315322:	xor    (%rax),%al
+	...
+   2e2315330:	rex.RXB
+   2e2315331:	rex.XB
+   2e2315332:	rex.XB cmp (%r8),%spl
+   2e2315335:	sub    %al,0x4e(%rdi)
+   2e2315338:	push   %rbp
+   2e2315339:	sub    %esp,(%rax)
+   2e231533b:	xor    %esi,(%rdx)
+   2e231533d:	sub    $0x336e6977,%eax
+   2e2315342:	xor    (%rax),%al
+	...
+   2e2315350:	rex.RXB
+   2e2315351:	rex.XB
+   2e2315352:	rex.XB cmp (%r8),%spl
+   2e2315355:	sub    %al,0x4e(%rdi)
+   2e2315358:	push   %rbp
+   2e2315359:	sub    %esp,(%rax)
+   2e231535b:	xor    %esi,(%rdx)
+   2e231535d:	sub    $0x336e6977,%eax
+   2e2315362:	xor    (%rax),%al
+	...
+   2e2315370:	rex.RXB
+   2e2315371:	rex.XB
+   2e2315372:	rex.XB cmp (%r8),%spl
+   2e2315375:	sub    %al,0x4e(%rdi)
+   2e2315378:	push   %rbp
+   2e2315379:	sub    %esp,(%rax)
+   2e231537b:	xor    %esi,(%rdx)
+   2e231537d:	sub    $0x336e6977,%eax
+   2e2315382:	xor    (%rax),%al
+	...
+   2e2315390:	rex.RXB
+   2e2315391:	rex.XB
+   2e2315392:	rex.XB cmp (%r8),%spl
+   2e2315395:	sub    %al,0x4e(%rdi)
+   2e2315398:	push   %rbp
+   2e2315399:	sub    %esp,(%rax)
+   2e231539b:	xor    %esi,(%rdx)
+   2e231539d:	sub    $0x336e6977,%eax
+   2e23153a2:	xor    (%rax),%al
+	...
+   2e23153b0:	rex.RXB
+   2e23153b1:	rex.XB
+   2e23153b2:	rex.XB cmp (%r8),%spl
+   2e23153b5:	sub    %al,0x4e(%rdi)
+   2e23153b8:	push   %rbp
+   2e23153b9:	sub    %esp,(%rax)
+   2e23153bb:	xor    %esi,(%rdx)
+   2e23153bd:	sub    $0x336e6977,%eax
+   2e23153c2:	xor    (%rax),%al
+	...
+   2e23153d0:	rex.RXB
+   2e23153d1:	rex.XB
+   2e23153d2:	rex.XB cmp (%r8),%spl
+   2e23153d5:	sub    %al,0x4e(%rdi)
+   2e23153d8:	push   %rbp
+   2e23153d9:	sub    %esp,(%rax)
+   2e23153db:	xor    %esi,(%rdx)
+   2e23153dd:	sub    $0x336e6977,%eax
+   2e23153e2:	xor    (%rax),%al
+	...
+   2e23153f0:	rex.RXB
+   2e23153f1:	rex.XB
+   2e23153f2:	rex.XB cmp (%r8),%spl
+   2e23153f5:	sub    %al,0x4e(%rdi)
+   2e23153f8:	push   %rbp
+   2e23153f9:	sub    %esp,(%rax)
+   2e23153fb:	xor    %esi,(%rdx)
+   2e23153fd:	sub    $0x336e6977,%eax
+   2e2315402:	xor    (%rax),%al
+	...
+   2e2315410:	rex.RXB
+   2e2315411:	rex.XB
+   2e2315412:	rex.XB cmp (%r8),%spl
+   2e2315415:	sub    %al,0x4e(%rdi)
+   2e2315418:	push   %rbp
+   2e2315419:	sub    %esp,(%rax)
+   2e231541b:	xor    %esi,(%rdx)
+   2e231541d:	sub    $0x336e6977,%eax
+   2e2315422:	xor    (%rax),%al
+	...
+   2e2315430:	rex.RXB
+   2e2315431:	rex.XB
+   2e2315432:	rex.XB cmp (%r8),%spl
+   2e2315435:	sub    %al,0x4e(%rdi)
+   2e2315438:	push   %rbp
+   2e2315439:	sub    %esp,(%rax)
+   2e231543b:	xor    %esi,(%rdx)
+   2e231543d:	sub    $0x336e6977,%eax
+   2e2315442:	xor    (%rax),%al
+	...
+   2e2315450:	rex.RXB
+   2e2315451:	rex.XB
+   2e2315452:	rex.XB cmp (%r8),%spl
+   2e2315455:	sub    %al,0x4e(%rdi)
+   2e2315458:	push   %rbp
+   2e2315459:	sub    %esp,(%rax)
+   2e231545b:	xor    %esi,(%rdx)
+   2e231545d:	sub    $0x336e6977,%eax
+   2e2315462:	xor    (%rax),%al
+	...
+   2e2315470:	rex.RXB
+   2e2315471:	rex.XB
+   2e2315472:	rex.XB cmp (%r8),%spl
+   2e2315475:	sub    %al,0x4e(%rdi)
+   2e2315478:	push   %rbp
+   2e2315479:	sub    %esp,(%rax)
+   2e231547b:	xor    %esi,(%rdx)
+   2e231547d:	sub    $0x336e6977,%eax
+   2e2315482:	xor    (%rax),%al
+	...
+   2e2315490:	rex.RXB
+   2e2315491:	rex.XB
+   2e2315492:	rex.XB cmp (%r8),%spl
+   2e2315495:	sub    %al,0x4e(%rdi)
+   2e2315498:	push   %rbp
+   2e2315499:	sub    %esp,(%rax)
+   2e231549b:	xor    %esi,(%rdx)
+   2e231549d:	sub    $0x336e6977,%eax
+   2e23154a2:	xor    (%rax),%al
+	...
+   2e23154b0:	rex.RXB
+   2e23154b1:	rex.XB
+   2e23154b2:	rex.XB cmp (%r8),%spl
+   2e23154b5:	sub    %al,0x4e(%rdi)
+   2e23154b8:	push   %rbp
+   2e23154b9:	sub    %esp,(%rax)
+   2e23154bb:	xor    %esi,(%rdx)
+   2e23154bd:	sub    $0x336e6977,%eax
+   2e23154c2:	xor    (%rax),%al
+	...
+   2e23154d0:	rex.RXB
+   2e23154d1:	rex.XB
+   2e23154d2:	rex.XB cmp (%r8),%spl
+   2e23154d5:	sub    %al,0x4e(%rdi)
+   2e23154d8:	push   %rbp
+   2e23154d9:	sub    %esp,(%rax)
+   2e23154db:	xor    %esi,(%rdx)
+   2e23154dd:	sub    $0x336e6977,%eax
+   2e23154e2:	xor    (%rax),%al
+	...
+   2e23154f0:	rex.RXB
+   2e23154f1:	rex.XB
+   2e23154f2:	rex.XB cmp (%r8),%spl
+   2e23154f5:	sub    %al,0x4e(%rdi)
+   2e23154f8:	push   %rbp
+   2e23154f9:	sub    %esp,(%rax)
+   2e23154fb:	xor    %esi,(%rdx)
+   2e23154fd:	sub    $0x336e6977,%eax
+   2e2315502:	xor    (%rax),%al
+	...
+   2e2315510:	rex.RXB
+   2e2315511:	rex.XB
+   2e2315512:	rex.XB cmp (%r8),%spl
+   2e2315515:	sub    %al,0x4e(%rdi)
+   2e2315518:	push   %rbp
+   2e2315519:	sub    %esp,(%rax)
+   2e231551b:	xor    %esi,(%rdx)
+   2e231551d:	sub    $0x336e6977,%eax
+   2e2315522:	xor    (%rax),%al
+	...
+   2e2315530:	rex.RXB
+   2e2315531:	rex.XB
+   2e2315532:	rex.XB cmp (%r8),%spl
+   2e2315535:	sub    %al,0x4e(%rdi)
+   2e2315538:	push   %rbp
+   2e2315539:	sub    %esp,(%rax)
+   2e231553b:	xor    %esi,(%rdx)
+   2e231553d:	sub    $0x336e6977,%eax
+   2e2315542:	xor    (%rax),%al
+	...
+   2e2315550:	rex.RXB
+   2e2315551:	rex.XB
+   2e2315552:	rex.XB cmp (%r8),%spl
+   2e2315555:	sub    %al,0x4e(%rdi)
+   2e2315558:	push   %rbp
+   2e2315559:	sub    %esp,(%rax)
+   2e231555b:	xor    %esi,(%rdx)
+   2e231555d:	sub    $0x336e6977,%eax
+   2e2315562:	xor    (%rax),%al
+	...
+   2e2315570:	rex.RXB
+   2e2315571:	rex.XB
+   2e2315572:	rex.XB cmp (%r8),%spl
+   2e2315575:	sub    %al,0x4e(%rdi)
+   2e2315578:	push   %rbp
+   2e2315579:	sub    %esp,(%rax)
+   2e231557b:	xor    %esi,(%rdx)
+   2e231557d:	sub    $0x336e6977,%eax
+   2e2315582:	xor    (%rax),%al
+	...
+   2e2315590:	rex.RXB
+   2e2315591:	rex.XB
+   2e2315592:	rex.XB cmp (%r8),%spl
+   2e2315595:	sub    %al,0x4e(%rdi)
+   2e2315598:	push   %rbp
+   2e2315599:	sub    %esp,(%rax)
+   2e231559b:	xor    %esi,(%rdx)
+   2e231559d:	sub    $0x336e6977,%eax
+   2e23155a2:	xor    (%rax),%al
 	...
 
 Disassembly of section .pdata:
 
 00000002e2316000 <.pdata>:
    2e2316000:	add    %dl,(%rax)
    2e2316002:	add    %al,(%rax)
    2e2316004:	or     $0x10,%al
    2e2316006:	add    %al,(%rax)
    2e2316008:	add    %dh,0x0(%rax)
    2e231600b:	add    %dl,(%rax)
    2e231600d:	adc    %al,(%rax)
-   2e231600f:	add    %bh,%bh
+   2e231600f:	add    %cl,%bh
    2e2316011:	adc    %eax,(%rax)
    2e2316013:	add    %al,(%rax,%rsi,2)
    2e2316016:	add    %al,(%rax)
-   2e2316018:	add    %dl,(%rdx)
+   2e2316018:	rclb   $1,(%rcx)
    2e231601a:	add    %al,(%rax)
-   2e231601c:	adc    (%rax),%r8d
-   2e231601f:	add    %bl,(%rax)
-   2e2316021:	jo     0x2e2316023
-   2e2316023:	add    %dl,0x13(%rax)
-   2e2316026:	add    %al,(%rax)
-   2e2316028:	(bad)
+   2e231601c:	adc    $0x13,%al
+   2e231601e:	add    %al,(%rax)
+   2e2316020:	sbb    %dh,0x0(%rax)
+   2e2316023:	add    %ah,(%rax)
+   2e2316025:	adc    (%rax),%eax
+   2e2316027:	add    %dh,(%rdx)
+   2e2316029:	adc    (%rax),%eax
+   2e231602b:	add    %ch,(%rax)
    2e231602d:	jo     0x2e231602f
-   2e231602f:	add    %dh,0x13(%rax)
+   2e231602f:	add    %al,0x13(%rax)
    2e2316032:	add    %al,(%rax)
-   2e2316034:	jg     0x2e2316049
-   2e2316036:	add    %al,(%rax)
-   2e2316038:	sub    $0x70,%al
+   2e2316034:	rex.WRXB adc (%r8),%r8
+   2e2316037:	add    %ch,(%rax,%rsi,2)
    2e231603a:	add    %al,(%rax)
-   2e231603c:	adcb   $0x0,(%rbx)
-   2e231603f:	add    %cl,0x70300000(%rbx,%rdx,1)
-   2e2316046:	add    %al,(%rax)
-   2e2316048:	nop
-   2e2316049:	adc    (%rax),%eax
-   2e231604b:	add    %dl,0x34000013(%rcx)
-   2e2316051:	jo     0x2e2316053
-   2e2316053:	add    %ah,-0x46ffffed(%rax)
-   2e2316059:	adc    (%rax),%eax
-   2e231605b:	add    %bh,(%rax)
-   2e231605d:	jo     0x2e231605f
-   2e231605f:	add    %al,%al
-   2e2316061:	adc    (%rax),%eax
-   2e2316063:	add    %dh,%ch
+   2e231603c:	push   %rax
+   2e231603d:	adc    (%rax),%eax
+   2e231603f:	add    %bl,0x0(%rbx,%rdx,1)
+   2e2316043:	add    %dh,(%rax)
+   2e2316045:	jo     0x2e2316047
+   2e2316047:	add    %ah,0x13(%rax)
+   2e231604a:	add    %al,(%rax)
+   2e231604c:	(bad)
+   2e231604d:	adc    (%rax),%eax
+   2e231604f:	add    %dh,(%rax,%rsi,2)
+   2e2316052:	add    %al,(%rax)
+   2e2316054:	jo     0x2e2316069
+   2e2316056:	add    %al,(%rax)
+   2e2316058:	mov    %edx,(%rbx)
+   2e231605a:	add    %al,(%rax)
+   2e231605c:	cmp    %dh,0x0(%rax)
+   2e231605f:	add    %dl,-0x3affffed(%rax)
    2e2316065:	adc    (%rax),%eax
    2e2316067:	add    %bh,(%rax,%rsi,2)
    2e231606a:	add    %al,(%rax)
-   2e231606c:	add    %dl,(%rax,%rax,1)
-   2e231606f:	add    %ah,0x14(%rcx)
-   2e2316072:	add    %al,(%rax)
-   2e2316074:	rex jo 0x2e2316077
-   2e2316077:	add    %dh,0x14(%rax)
-   2e231607a:	add    %al,(%rax)
-   2e231607c:	repz adc $0x0,%al
-   2e231607f:	add    %al,0x0(%rax,%rsi,2)
-   2e2316083:	add    %al,(%rax)
-   2e2316085:	adc    $0x15810000,%eax
-   2e231608a:	add    %al,(%rax)
-   2e231608c:	rex.W jo 0x2e231608f
-   2e231608f:	add    %dl,-0x59ffffeb(%rax)
-   2e2316095:	sbb    %al,(%rax)
-   2e2316097:	add    %bl,0x70(%rax)
-   2e231609a:	add    %al,(%rax)
-   2e231609c:	mov    $0x18,%al
+   2e231606c:	rclb   $1,(%rbx)
+   2e231606e:	add    %al,(%rax)
+   2e2316070:	sub    %edx,(%rax,%rax,1)
+   2e2316073:	add    %al,0x70(%rax)
+   2e2316076:	add    %al,(%rax)
+   2e2316078:	xor    %dl,(%rax,%rax,1)
+   2e231607b:	add    %bl,0x44000014(%rbx)
+   2e2316081:	jo     0x2e2316083
+   2e2316083:	add    %ah,0x19000014(%rax)
+   2e2316089:	adc    $0x70480000,%eax
+   2e231608e:	add    %al,(%rax)
+   2e2316090:	and    %dl,0x183c0000(%rip)        # 0x2fa6d6096
+   2e2316096:	add    %al,(%rax)
+   2e2316098:	pop    %rax
+   2e2316099:	jo     0x2e231609b
+   2e231609b:	add    %al,0x18(%rax)
    2e231609e:	add    %al,(%rax)
-   2e23160a0:	mov    $0x18,%ch
-   2e23160a2:	add    %al,(%rax)
-   2e23160a4:	jl     0x2e2316116
+   2e23160a0:	sbb    %r8b,(%r8)
+   2e23160a3:	add    %bh,0x70(%rax)
    2e23160a6:	add    %al,(%rax)
-   2e23160a8:	rcrb   $0x0,(%rax)
-   2e23160ab:	add    %bl,%ah
-   2e23160ad:	(bad)
-   2e23160ae:	add    %al,(%rax)
-   2e23160b0:	xorb   $0x0,0x0(%rax)
-   2e23160b4:	loopne 0x2e23160d5
-   2e23160b6:	add    %al,(%rax)
-   2e23160b8:	or     %esp,(%rax)
-   2e23160ba:	add    %al,(%rax)
-   2e23160bc:	pushf
-   2e23160bd:	jo     0x2e23160bf
-   2e23160bf:	add    %dl,(%rax)
-   2e23160c1:	and    %al,(%rax)
-   2e23160c3:	add    %dh,(%rcx)
-   2e23160c5:	and    %al,(%rax)
-   2e23160c7:	add    %ah,0x40000070(%rax)
-   2e23160cd:	and    %al,(%rax)
-   2e23160cf:	add    %bh,0x20(%rdx)
+   2e23160a8:	push   %rax
+   2e23160a9:	sbb    %al,(%rax)
+   2e23160ab:	add    %ch,%bh
+   2e23160ad:	and    %al,(%rax)
+   2e23160af:	add    %bh,0x0(%rax,%rsi,2)
+   2e23160b3:	add    %dh,%al
+   2e23160b5:	and    %al,(%rax)
+   2e23160b7:	add    %ah,(%rax)
+   2e23160b9:	and    %eax,(%rax)
+   2e23160bb:	add    %bl,0x20000070(%rax)
+   2e23160c1:	and    %eax,(%rax)
+   2e23160c3:	add    %al,0x21(%rcx)
+   2e23160c6:	add    %al,(%rax)
+   2e23160c8:	pushf
+   2e23160c9:	jo     0x2e23160cb
+   2e23160cb:	add    %dl,0x21(%rax)
+   2e23160ce:	add    %al,(%rax)
+   2e23160d0:	mov    (%rcx),%ah
    2e23160d2:	add    %al,(%rax)
-   2e23160d4:	movsb  %ds:(%rsi),%es:(%rdi)
-   2e23160d5:	jo     0x2e23160d7
-   2e23160d7:	add    %al,-0x15ffffe0(%rax)
-   2e23160dd:	and    %al,(%rax)
-   2e23160df:	add    %ch,0x20f00000(%rax,%rsi,2)
-   2e23160e6:	add    %al,(%rax)
-   2e23160e8:	mov    %db0,%rax
-   2e23160eb:	add    %bh,0x10000070(%rax)
-   2e23160f1:	and    %eax,(%rax)
-   2e23160f3:	add    %bh,(%rdi)
-   2e23160f5:	and    %eax,(%rax)
-   2e23160f7:	add    %bh,0x21400000(%rax,%rsi,2)
-   2e23160fe:	add    %al,(%rax)
-   2e2316100:	shll   $0x0,(%rcx)
-   2e2316103:	add    %al,%ah
+   2e23160d4:	movabs 0xfa00002190000070,%al
+   2e23160dd:	and    %eax,(%rax)
+   2e23160df:	add    %ch,0x70(%rax)
+   2e23160e5:	and    (%rax),%al
+   2e23160e7:	add    %bl,(%rdi)
+   2e23160e9:	and    (%rax),%al
+   2e23160eb:	add    %dh,0x22200000(%rax,%rsi,2)
+   2e23160f2:	add    %al,(%rax)
+   2e23160f4:	rex.WRXB and (%r8),%r8b
+   2e23160f7:	add    %bh,0x50000070(%rax)
+   2e23160fd:	and    (%rax),%al
+   2e23160ff:	add    %dl,%cl
+   2e2316101:	and    (%rax),%al
+   2e2316103:	add    %al,%al
    2e2316105:	jo     0x2e2316107
-   2e2316107:	add    %dl,%al
-   2e2316109:	and    %eax,(%rax)
-   2e231610b:	add    %dl,%bl
-   2e231610d:	and    %eax,(%rax)
-   2e231610f:	add    %dl,%al
+   2e2316107:	add    %ah,%al
+   2e2316109:	and    (%rax),%al
+   2e231610b:	add    %ah,%bl
+   2e231610d:	and    (%rax),%al
+   2e231610f:	add    %cl,%ah
    2e2316111:	jo     0x2e2316113
-   2e2316113:	add    %ah,%al
-   2e2316115:	and    %eax,(%rax)
-   2e2316117:	add    %cl,0x22(%rdx)
+   2e2316113:	add    %dh,%al
+   2e2316115:	and    (%rax),%al
+   2e2316117:	add    %bl,0x23(%rcx)
    2e231611a:	add    %al,(%rax)
-   2e231611c:	(bad)
-   2e231611d:	jo     0x2e231611f
-   2e231611f:	add    %dl,0x22(%rax)
+   2e231611c:	shlb   $1,0x0(%rax)
+   2e231611f:	add    %ah,0x23(%rax)
    2e2316122:	add    %al,(%rax)
-   2e2316124:	insl   (%dx),%es:(%rdi)
-   2e2316125:	and    $0x0,%al
-   2e2316127:	add    %ah,%al
+   2e2316124:	ret    $0x24
+   2e2316127:	add    %bl,%ah
    2e2316129:	jo     0x2e231612b
-   2e231612b:	add    %dh,0x24(%rax)
-   2e231612e:	add    %al,(%rax)
-   2e2316130:	push   %rbp
-   2e2316131:	(bad)
-   2e2316132:	add    %al,(%rax)
-   2e2316134:	lock jo 0x2e2316137
-   2e2316137:	add    %ah,0x27(%rax)
-   2e231613a:	add    %al,(%rax)
-   2e231613c:	lret
-   2e231613d:	(bad)
-   2e231613e:	add    %al,(%rax)
-   2e2316140:	or     %dh,0x0(%rcx)
-   2e2316143:	add    %dl,%al
-   2e2316145:	(bad)
-   2e2316146:	add    %al,(%rax)
-   2e2316148:	rex.W sub %al,(%rax)
-   2e231614b:	add    %bl,(%rax)
+   2e231612b:	add    %dl,%al
+   2e231612d:	and    $0x0,%al
+   2e231612f:	add    %ch,(%rbx)
+   2e2316131:	sub    %al,(%rax)
+   2e2316133:	add    %ch,%al
+   2e2316135:	jo     0x2e2316137
+   2e2316137:	add    %dh,(%rax)
+   2e2316139:	sub    %al,(%rax)
+   2e231613b:	add    %ah,0x28(%rax)
+   2e2316141:	jno    0x2e2316143
+   2e2316143:	add    %ah,0xf000028(%rax)
+   2e2316149:	sub    %eax,(%rax)
+   2e231614b:	add    %dl,(%rax)
    2e231614d:	jno    0x2e231614f
-   2e231614f:	add    %dl,0x28(%rax)
-   2e2316152:	add    %al,(%rax)
-   2e2316154:	fldcw  (%rax)
-   2e2316156:	add    %al,(%rax)
-   2e2316158:	and    $0x71,%al
-   2e231615a:	add    %al,(%rax)
-   2e231615c:	loopne 0x2e2316186
-   2e231615e:	add    %al,(%rax)
-   2e2316160:	shrb   $0x0,(%rcx)
-   2e2316163:	add    %ch,(%rcx,%rsi,2)
-   2e2316166:	add    %al,(%rax)
-   2e2316168:	shrb   $0x0,(%rcx)
-   2e231616b:	add    %bl,%dh
-   2e231616d:	sub    %eax,(%rax)
-   2e231616f:	add    %dh,(%rcx,%rsi,2)
-   2e2316172:	add    %al,(%rax)
-   2e2316174:	loopne 0x2e231619f
-   2e2316176:	add    %al,(%rax)
-   2e2316178:	repz sub %eax,(%rax)
-   2e231617b:	add    %bh,(%rax)
-   2e231617d:	jno    0x2e231617f
-   2e231617f:	add    %al,(%rax)
-   2e2316181:	sub    (%rax),%al
-   2e2316183:	add    %cl,0x2a(%rax)
-   2e2316186:	add    %al,(%rax)
-   2e2316188:	cmp    $0x71,%al
-   2e231618a:	add    %al,(%rax)
-   2e231618c:	push   %rax
-   2e231618d:	sub    (%rax),%al
-   2e231618f:	add    %ch,%bh
-   2e2316191:	sub    (%rax),%al
-   2e2316193:	add    %al,0x71(%rax)
-   2e2316196:	add    %al,(%rax)
-   2e2316198:	lock sub (%rax),%al
-   2e231619b:	add    %dh,0x2b(%rcx)
+   2e231614f:	add    %dl,(%rax)
+   2e2316151:	sub    %eax,(%rax)
+   2e2316153:	add    %dl,0x1c000029(%rcx)
+   2e2316159:	jno    0x2e231615b
+   2e231615b:	add    %ah,-0x6dffffd7(%rax)
+   2e2316161:	sub    (%rax),%al
+   2e2316163:	add    %ch,(%rax)
+   2e2316165:	jno    0x2e2316167
+   2e2316167:	add    %ah,-0x33ffffd6(%rax)
+   2e231616d:	sub    (%rax),%al
+   2e231616f:	add    %dh,(%rax)
+   2e2316171:	jno    0x2e2316173
+   2e2316173:	add    %dl,%al
+   2e2316175:	sub    (%rax),%al
+   2e2316177:	add    %ah,(%rax)
+   2e2316179:	sub    (%rax),%eax
+   2e231617b:	add    %dh,(%rcx,%rsi,2)
+   2e231617e:	add    %al,(%rax)
+   2e2316180:	and    %ch,(%rbx)
+   2e2316182:	add    %al,(%rax)
+   2e2316184:	mov    $0x3800002b,%ebp
+   2e2316189:	jno    0x2e231618b
+   2e231618b:	add    %al,%al
+   2e231618d:	sub    (%rax),%eax
+   2e231618f:	add    %al,0x2c(%rax)
+   2e2316192:	add    %al,(%rax)
+   2e2316194:	rex.R jno 0x2e2316197
+   2e2316197:	add    %al,0x2c(%rax)
+   2e231619a:	add    %al,(%rax)
+   2e231619c:	ja     0x2e23161ca
    2e231619e:	add    %al,(%rax)
-   2e23161a0:	rex.WR jno 0x2e23161a3
-   2e23161a3:	add    %al,-0x54ffffd5(%rax)
-   2e23161a9:	sub    (%rax),%eax
-   2e23161ab:	add    %dl,0x0(%rcx,%rsi,2)
-   2e23161af:	add    %dh,0x1c00002b(%rax)
-   2e23161b5:	sub    $0x0,%al
-   2e23161b7:	add    %bl,0x0(%rcx,%rsi,2)
-   2e23161bb:	add    %ah,(%rax)
-   2e23161bd:	sub    $0x0,%al
-   2e23161bf:	add    %cl,0x2c(%rax)
-   2e23161c2:	add    %al,(%rax)
-   2e23161c4:	fs jno 0x2e23161c7
-   2e23161c7:	add    %dl,0x2c(%rax)
-   2e23161ca:	add    %al,(%rax)
-   2e23161cc:	{rex2 0x2c} add %r8b,(%rax)
-   2e23161d0:	insb   (%dx),%es:(%rdi)
+   2e23161a0:	rex.W jno 0x2e23161a3
+   2e23161a3:	add    %al,-0xcffffd4(%rax)
+   2e23161a9:	sub    $0x0,%al
+   2e23161ab:	add    %cl,0x0(%rcx,%rsi,2)
+   2e23161af:	add    %al,(%rax)
+   2e23161b1:	sub    $0x2d360000,%eax
+   2e23161b6:	add    %al,(%rax)
+   2e23161b8:	push   %rax
+   2e23161b9:	jno    0x2e23161bb
+   2e23161bb:	add    %al,0x2d(%rax)
+   2e23161be:	add    %al,(%rax)
+   2e23161c0:	leave
+   2e23161c1:	sub    $0x71540000,%eax
+   2e23161c6:	add    %al,(%rax)
+   2e23161c8:	shrb   $1,0x2e960000(%rip)        # 0x310c761ce
+   2e23161ce:	add    %al,(%rax)
+   2e23161d0:	pop    %rax
    2e23161d1:	jno    0x2e23161d3
-   2e23161d3:	add    %ah,%al
-   2e23161d5:	sub    $0x0,%al
-   2e23161d7:	add    %dl,0x7400002d(%rdx)
+   2e23161d3:	add    %ah,-0x5cffffd2(%rax)
+   2e23161d9:	cs add %al,(%rax)
+   2e23161dc:	pop    %rsp
    2e23161dd:	jno    0x2e23161df
-   2e23161df:	add    %ah,-0x5cffffd3(%rax)
-   2e23161e5:	sub    $0x717c0000,%eax
-   2e23161ea:	add    %al,(%rax)
-   2e23161ec:	lock sub $0x2df60000,%eax
+   2e23161df:	add    %dh,%al
+   2e23161e1:	cs add %al,(%rax)
+   2e23161e4:	imulb  (%rsi)
+   2e23161e6:	add    %al,(%rax)
+   2e23161e8:	(bad)
+   2e23161e9:	jno    0x2e23161eb
+   2e23161eb:	add    %al,(%rax)
+   2e23161ed:	(bad)
+   2e23161ee:	add    %al,(%rax)
+   2e23161f0:	(bad)
+   2e23161f1:	(bad)
    2e23161f2:	add    %al,(%rax)
-   2e23161f4:	xorb   $0x0,0x0(%rcx)
-   2e23161f8:	add    %ch,(%rsi)
+   2e23161f4:	fs jno 0x2e23161f7
+   2e23161f7:	add    %dl,(%rax)
+   2e23161f9:	(bad)
    2e23161fa:	add    %al,(%rax)
-   2e23161fc:	(bad)
-   2e23161fd:	cs add %al,(%rax)
-   2e2316200:	test   %dh,0x0(%rcx)
-   2e2316203:	add    %dl,(%rax)
-   2e2316205:	cs add %al,(%rax)
-   2e2316208:	rex.WRXB (bad)
+   2e23161fc:	rex.XB xor %al,(%r8)
+   2e23161ff:	add    %ch,0x71(%rax)
+   2e2316202:	add    %al,(%rax)
+   2e2316204:	push   %rax
+   2e2316205:	xor    %al,(%rax)
+   2e2316207:	add    %ch,0x30(%rdi)
    2e231620a:	add    %al,(%rax)
-   2e231620c:	mov    %dh,0x0(%rcx)
-   2e231620f:	add    %al,%al
-   2e2316211:	(bad)
+   2e231620c:	je     0x2e231627f
+   2e231620e:	add    %al,(%rax)
+   2e2316210:	jo     0x2e2316242
    2e2316212:	add    %al,(%rax)
-   2e2316214:	in     $0x2f,%eax
+   2e2316214:	lea    (%rax),%esi
    2e2316216:	add    %al,(%rax)
-   2e2316218:	xchg   %eax,%esp
-   2e2316219:	jno    0x2e231621b
-   2e231621b:	add    %dh,%al
-   2e231621d:	(bad)
-   2e231621e:	add    %al,(%rax)
-   2e2316220:	(bad)
-   2e2316221:	xor    %al,(%rax)
-   2e2316223:	add    %bl,-0x2fffff8f(%rax)
-   2e2316229:	xor    %al,(%rax)
-   2e231622b:	add    %al,0x31(%rcx)
-   2e231622e:	add    %al,(%rax)
-   2e2316230:	test   $0x71,%al
-   2e2316232:	add    %al,(%rax)
-   2e2316234:	push   %rax
-   2e2316235:	xor    %eax,(%rax)
-   2e2316237:	add    %ch,0x31(%rdi)
-   2e231623a:	add    %al,(%rax)
-   2e231623c:	mov    $0x71,%ah
-   2e231623e:	add    %al,(%rax)
-   2e2316240:	loopne 0x2e2316273
+   2e2316218:	jl     0x2e231628b
+   2e231621a:	add    %al,(%rax)
+   2e231621c:	nop
+   2e231621d:	xor    %al,(%rax)
+   2e231621f:	add    %ah,0x31(%rax)
+   2e2316222:	add    %al,(%rax)
+   2e2316224:	xorb   $0x0,0x0(%rcx)
+   2e2316228:	(bad)
+   2e2316229:	xor    %eax,(%rax)
+   2e231622b:	add    %al,%bh
+   2e231622d:	xor    %eax,(%rax)
+   2e231622f:	add    %dl,-0x4fffff8f(%rax)
+   2e2316235:	xor    (%rax),%al
+   2e2316237:	add    %ch,%dh
+   2e2316239:	xor    (%rax),%al
+   2e231623b:	add    %bl,0x32f00000(%rcx,%rsi,2)
    2e2316242:	add    %al,(%rax)
-   2e2316244:	and    %esi,(%rdx)
-   2e2316246:	add    %al,(%rax)
-   2e2316248:	mov    $0x30000071,%esp
-   2e231624d:	xor    (%rax),%al
-   2e231624f:	add    %bh,(%rdx,%rsi,1)
-   2e2316252:	add    %al,(%rax)
-   2e2316254:	(bad)
+   2e2316244:	cld
+   2e2316245:	xor    (%rax),%al
+   2e2316247:	add    %ah,0x33100000(%rcx,%rsi,2)
+   2e231624e:	add    %al,(%rax)
+   2e2316250:	adc    $0xa8000033,%eax
    2e2316255:	jno    0x2e2316257
-   2e2316257:	add    %dl,0x32(%rax)
-   2e231625a:	add    %al,(%rax)
-   2e231625c:	push   %rbp
-   2e231625d:	xor    (%rax),%al
-   2e231625f:	add    %cl,%al
-   2e2316261:	jno    0x2e2316263
 	...
 
 Disassembly of section .xdata:
 
 00000002e2317000 <.xdata>:
    2e2317000:	add    %eax,(%rax)
    2e2317002:	add    %al,(%rax)
@@ -3855,234 +3813,233 @@
    2e231700d:	(bad)
    2e231700e:	(bad)
    2e231700f:	jo     0x2e2317016
    2e2317011:	push   %rax
    2e2317012:	add    $0xc0,%al
    2e2317014:	add    %al,%dl
    2e2317016:	add    %al,(%rax)
-   2e2317018:	add    %ecx,(%rsi,%rax,1)
-   2e231701b:	add    %cl,(%rdx,%rsi,1)
-   2e231701e:	or     %dh,(%rax)
-   2e2317020:	(bad)
-   2e2317021:	(bad)
-   2e2317022:	(bad)
-   2e2317023:	rolb   $0x2,(%rax,%rdx,8)
-   2e2317027:	loopne 0x2e231702a
-   2e2317029:	add    %al,(%rax)
-   2e231702b:	add    %al,(%rcx)
-   2e231702d:	add    %al,(%rax)
-   2e231702f:	add    %al,(%rcx)
-   2e2317031:	add    %al,(%rax)
-   2e2317033:	add    %al,(%rcx)
-   2e2317035:	add    %al,(%rax)
-   2e2317037:	add    %al,(%rcx)
-   2e2317039:	add    %al,(%rax)
-   2e231703b:	add    %al,(%rcx)
-   2e231703d:	add    %al,(%rax)
-   2e231703f:	add    %al,(%rcx)
-   2e2317041:	add    %al,(%rax)
-   2e2317043:	add    %al,(%rcx)
-   2e2317045:	add    %al,(%rax)
-   2e2317047:	add    %al,(%rcx)
-   2e2317049:	or     %al,0x4420800(%rip)        # 0x2e673784f
+   2e2317018:	add    %ecx,(%rdx)
+   2e231701a:	(bad)
+   2e231701b:	add    %cl,(%rdx)
+   2e231701d:	xor    (%rsi),%al
+   2e231701f:	xor    %al,0x3700460(%rip)        # 0x2e5a17485
+   2e2317025:	push   %rax
+   2e2317026:	add    %al,%al
+   2e2317028:	add    %eax,(%rax)
+   2e231702a:	add    %al,(%rax)
+   2e231702c:	add    %eax,(%rax)
+   2e231702e:	add    %al,(%rax)
+   2e2317030:	add    %eax,(%rax)
+   2e2317032:	add    %al,(%rax)
+   2e2317034:	add    %eax,(%rax)
+   2e2317036:	add    %al,(%rax)
+   2e2317038:	add    %eax,(%rax)
+   2e231703a:	add    %al,(%rax)
+   2e231703c:	add    %eax,(%rax)
+   2e231703e:	add    %al,(%rax)
+   2e2317040:	add    %eax,(%rax)
+   2e2317042:	add    %al,(%rax)
+   2e2317044:	add    %eax,(%rax)
+   2e2317046:	add    %al,(%rax)
+   2e2317048:	add    %ecx,(%rax)
+   2e231704a:	add    $0x4420800,%eax
    2e231704f:	xor    %al,(%rbx)
    2e2317051:	(bad)
    2e2317052:	add    0x1(%rax),%dh
    2e2317055:	push   %rax
    2e2317056:	add    %al,(%rax)
-   2e2317058:	add    %esp,(%rdi)
-   2e231705a:	adc    %al,(%rax)
-   2e231705c:	(bad)
-   2e231705d:	test   $0x7,%al
-   2e231705f:	add    %ah,(%rcx)
-   2e2317061:	cwtl
-   2e2317062:	(bad)
-   2e2317063:	add    %bl,(%rbx)
-   2e2317065:	mov    %al,0x4781500(%rip)        # 0x2e6a9856b
-   2e231706b:	add    %dl,(%rax)
-   2e231706d:	push   $0x10b0003
-   2e2317072:	adc    %eax,(%rax)
-   2e2317074:	add    $0x30,%al
-   2e2317076:	add    0x2(%rax),%esp
-   2e2317079:	jo     0x2e231707c
-   2e231707b:	push   %rax
-   2e231707c:	add    %eax,(%rax)
-   2e231707e:	add    %al,(%rax)
-   2e2317080:	add    %edx,0x6815000b(%rip)        # 0x34a467091
-   2e2317086:	add    $0xcc21000,%eax
-   2e231708b:	xor    %cl,(%rbx)
-   2e231708d:	(bad)
-   2e231708e:	or     0x9(%rax),%dh
-   2e2317091:	push   %rax
-   2e2317092:	or     %al,%al
-   2e2317094:	(bad)
-   2e2317095:	rolb   $1,(%rax,%riz,8)
-   2e2317098:	add    %al,%dh
+   2e2317058:	add    %ebx,(%rsi)
+   2e231705a:	or     $0x6981e00,%eax
+   2e231705f:	add    %bl,(%rax)
+   2e2317061:	mov    %al,0x4781200(%rip)        # 0x2e6a98267
+   2e2317067:	add    %cl,0x8000368(%rip)        # 0x2ea3173d5
+   2e231706d:	loop   0x2e2317073
+   2e231706f:	xor    %al,(%rbx)
+   2e2317071:	(bad)
+   2e2317072:	add    0x1(%rax),%dh
+   2e2317075:	push   %rax
+   2e2317076:	add    %al,(%rax)
+   2e2317078:	add    %eax,(%rax)
+   2e231707a:	add    %al,(%rax)
+   2e231707c:	add    %edx,0x6815000b(%rip)        # 0x34a46708d
+   2e2317082:	(bad)
+   2e2317083:	add    %dl,(%rax)
+   2e2317085:	loop   0x2e2317093
+   2e2317087:	xor    %cl,(%rbx)
+   2e2317089:	(bad)
+   2e231708a:	or     0x9(%rax),%dh
+   2e231708d:	push   %rax
+   2e231708e:	or     %al,%al
+   2e2317090:	(bad)
+   2e2317091:	rolb   $1,(%rax,%riz,8)
+   2e2317094:	add    %al,%dh
+   2e2317096:	add    %al,(%rax)
+   2e2317098:	add    %eax,(%rax)
    2e231709a:	add    %al,(%rax)
    2e231709c:	add    %eax,(%rax)
    2e231709e:	add    %al,(%rax)
-   2e23170a0:	add    %eax,(%rax)
-   2e23170a2:	add    %al,(%rax)
-   2e23170a4:	add    %eax,(%rcx,%rax,1)
-   2e23170a7:	add    %al,(%rdx,%rax,2)
-   2e23170aa:	add    %al,(%rax)
-   2e23170ac:	add    %eax,(%rsi)
-   2e23170ae:	add    (%rax),%eax
-   2e23170b0:	(bad)
-   2e23170b1:	rex.X add (%rax),%sil
-   2e23170b4:	add    %esp,0x0(%rax)
+   2e23170a0:	add    %eax,(%rcx,%rax,1)
+   2e23170a3:	add    %al,(%rdx,%rax,2)
+   2e23170a6:	add    %al,(%rax)
+   2e23170a8:	add    %eax,(%rsi)
+   2e23170aa:	add    (%rax),%eax
+   2e23170ac:	(bad)
+   2e23170ad:	rex.X add (%rax),%sil
+   2e23170b0:	add    %esp,0x0(%rax)
+   2e23170b3:	add    %al,(%rcx)
+   2e23170b5:	add    %al,(%rax)
    2e23170b7:	add    %al,(%rcx)
-   2e23170b9:	add    %al,(%rax)
-   2e23170bb:	add    %al,(%rcx)
-   2e23170bd:	add    $0x1,%al
-   2e23170bf:	add    %al,(%rdx,%rax,2)
-   2e23170c2:	add    %al,(%rax)
-   2e23170c4:	add    %eax,(%rsi)
-   2e23170c6:	add    (%rax),%eax
-   2e23170c8:	(bad)
-   2e23170c9:	rex.X add (%rax),%sil
-   2e23170cc:	add    %esp,0x0(%rax)
+   2e23170b9:	add    $0x1,%al
+   2e23170bb:	add    %al,(%rdx,%rax,2)
+   2e23170be:	add    %al,(%rax)
+   2e23170c0:	add    %eax,(%rsi)
+   2e23170c2:	add    (%rax),%eax
+   2e23170c4:	(bad)
+   2e23170c5:	rex.X add (%rax),%sil
+   2e23170c8:	add    %esp,0x0(%rax)
+   2e23170cb:	add    %al,(%rcx)
+   2e23170cd:	add    %al,(%rax)
    2e23170cf:	add    %al,(%rcx)
-   2e23170d1:	add    %al,(%rax)
-   2e23170d3:	add    %al,(%rcx)
+   2e23170d1:	(bad)
+   2e23170d2:	add    (%rax),%eax
+   2e23170d4:	(bad)
    2e23170d5:	(bad)
-   2e23170d6:	add    (%rax),%eax
-   2e23170d8:	(bad)
-   2e23170d9:	(bad)
-   2e23170de:	add    %al,(%rax)
-   2e23170e0:	add    %ecx,(%rdx)
-   2e23170e2:	(bad)
-   2e23170e3:	add    %cl,(%rdx)
-   2e23170e5:	xchg   %eax,%edx
-   2e23170e6:	(bad)
-   2e23170e7:	xor    %al,0x3700460(%rip)        # 0x2e5a1754d
-   2e23170ed:	push   %rax
-   2e23170ee:	add    %al,%al
-   2e23170f0:	add    %ebx,(%rax)
-   2e23170f2:	or     0x62100318(%rbp),%al
-   2e23170f8:	or     $0x30,%al
-   2e23170fa:	or     0xa(%rax),%esp
-   2e23170fd:	jo     0x2e2317108
-   2e23170ff:	rolb   $0xd0,(%rdi)
-   2e2317102:	add    $0x1f003e0,%eax
-   2e2317107:	push   %rax
-   2e2317108:	add    %ecx,(%rcx)
-   2e231710a:	add    $0x5420900,%eax
-   2e231710f:	xor    %al,(%rax,%riz,2)
-   2e2317112:	add    0x2(%rax),%esi
-   2e2317115:	rolb   $0x0,(%rax)
-   2e2317118:	add    %eax,(%rdi)
-   2e231711a:	add    $0x0,%al
-   2e231711c:	(bad)
-   2e231711d:	xor    (%rbx),%al
-   2e231711f:	xor    %al,(%rdx)
-   2e2317121:	(bad)
-   2e2317122:	add    %esi,0x1(%rax)
-   2e2317125:	add    $0x32050002,%eax
-   2e231712a:	add    %esi,(%rax)
-   2e231712c:	add    %eax,0x32050002(%rip)        # 0x314367134
-   2e2317132:	add    %esi,(%rax)
+   2e23170da:	add    %al,(%rax)
+   2e23170dc:	add    %eax,(%rdi)
+   2e23170de:	add    $0x0,%al
+   2e23170e0:	(bad)
+   2e23170e1:	xchg   %eax,%edx
+   2e23170e2:	add    (%rax),%esi
+   2e23170e4:	add    0x1(%rax),%ah
+   2e23170e7:	jo     0x2e23170ea
+   2e23170e9:	adc    $0x315450a,%eax
+   2e23170ee:	adc    %al,0x600b300c(%rdx)
+   2e23170f4:	or     0x9(%rax),%dh
+   2e23170f7:	rolb   $0xd0,(%rdi)
+   2e23170fa:	add    $0x1f003e0,%eax
+   2e23170ff:	push   %rax
+   2e2317100:	add    %ecx,(%rdx)
+   2e2317102:	(bad)
+   2e2317103:	add    %cl,(%rdx)
+   2e2317105:	xor    (%rsi),%al
+   2e2317107:	xor    %al,0x3700460(%rip)        # 0x2e5a1756d
+   2e231710d:	push   %rax
+   2e231710e:	add    %al,%al
+   2e2317110:	add    %eax,(%rdi)
+   2e2317112:	add    $0x0,%al
+   2e2317114:	(bad)
+   2e2317115:	xor    (%rbx),%al
+   2e2317117:	xor    %al,(%rdx)
+   2e2317119:	(bad)
+   2e231711a:	add    %esi,0x1(%rax)
+   2e231711d:	(bad)
+   2e231711e:	add    (%rax),%eax
+   2e2317120:	(bad)
+   2e2317121:	rex.X add (%rax),%sil
+   2e2317124:	add    %esp,0x0(%rax)
+   2e2317127:	add    %al,(%rcx)
+   2e2317129:	add    $0x32050002,%eax
+   2e231712e:	add    %esi,(%rax)
+   2e2317130:	add    %eax,(%rax)
+   2e2317132:	add    %al,(%rax)
    2e2317134:	add    %eax,(%rax)
    2e2317136:	add    %al,(%rax)
-   2e2317138:	add    %eax,(%rax)
-   2e231713a:	add    %al,(%rax)
-   2e231713c:	add    %eax,(%rax)
-   2e231713e:	add    %al,(%rax)
-   2e2317140:	add    %ecx,(%rax)
-   2e2317142:	add    $0x0,%al
-   2e2317144:	or     %dh,(%rdx)
-   2e2317146:	add    $0x30,%al
-   2e2317148:	add    0x2(%rax),%esp
-   2e231714b:	rolb   $0x4,(%rcx)
-   2e231714e:	add    %eax,(%rax)
-   2e2317150:	add    $0x42,%al
-   2e2317152:	add    %al,(%rax)
-   2e2317154:	add    %eax,(%rcx,%rax,1)
-   2e2317157:	add    %al,(%rdx,%rax,2)
-   2e231715a:	add    %al,(%rax)
-   2e231715c:	add    %eax,(%rcx,%rax,1)
-   2e231715f:	add    %al,(%rdx,%rax,2)
-   2e2317162:	add    %al,(%rax)
-   2e2317164:	add    %eax,(%rcx,%rax,1)
-   2e2317167:	add    %al,(%rdx,%rax,2)
-   2e231716a:	add    %al,(%rax)
-   2e231716c:	add    %eax,(%rcx,%rax,1)
-   2e231716f:	add    %al,(%rdx,%rax,2)
-   2e2317172:	add    %al,(%rax)
-   2e2317174:	add    %eax,(%rcx,%rax,1)
-   2e2317177:	add    %al,(%rdx,%rax,2)
-   2e231717a:	add    %al,(%rax)
+   2e2317138:	add    %eax,(%rdi)
+   2e231713a:	add    $0x0,%al
+   2e231713c:	(bad)
+   2e231713d:	xor    (%rbx),%al
+   2e231713f:	xor    %al,(%rdx)
+   2e2317141:	(bad)
+   2e2317142:	add    %esi,0x1(%rax)
+   2e2317145:	add    %al,(%rax)
+   2e2317147:	add    %al,(%rcx)
+   2e2317149:	add    %al,(%rax)
+   2e231714b:	add    %al,(%rcx)
+   2e231714d:	add    %al,(%rax)
+   2e231714f:	add    %al,(%rcx)
+   2e2317151:	add    %al,(%rax)
+   2e2317153:	add    %al,(%rcx)
+   2e2317155:	add    %al,(%rax)
+   2e2317157:	add    %al,(%rcx)
+   2e2317159:	add    %al,(%rax)
+   2e231715b:	add    %al,(%rcx)
+   2e231715d:	add    %al,(%rax)
+   2e231715f:	add    %al,(%rcx)
+   2e2317161:	add    %al,(%rax)
+   2e2317163:	add    %al,(%rcx)
+   2e2317165:	add    %al,(%rax)
+   2e2317167:	add    %al,(%rcx)
+   2e2317169:	or     (%rax,%rax,1),%al
+   2e231716c:	or     0x4(%rax),%ch
+   2e231716f:	add    %al,0x1300192(%rip)        # 0x2e3617307
+   2e2317175:	add    $0x32050002,%eax
+   2e231717a:	add    %esi,(%rax)
    2e231717c:	add    %eax,(%rax)
    2e231717e:	add    %al,(%rax)
-   2e2317180:	add    %eax,(%rax)
-   2e2317182:	add    %al,(%rax)
-   2e2317184:	add    %eax,(%rax)
-   2e2317186:	add    %al,(%rax)
-   2e2317188:	add    %ecx,(%rdx)
-   2e231718a:	add    $0x0,%al
-   2e231718c:	or     0x4(%rax),%ch
-   2e231718f:	add    %al,0x1300192(%rip)        # 0x2e3617327
-   2e2317195:	add    %al,(%rax)
-   2e2317197:	add    %al,(%rcx)
-   2e2317199:	or     %al,0x4420800(%rip)        # 0x2e673799f
-   2e231719f:	xor    %al,(%rbx)
-   2e23171a1:	(bad)
-   2e23171a2:	add    0x1(%rax),%dh
-   2e23171a5:	push   %rax
+   2e2317180:	add    %ecx,(%rax)
+   2e2317182:	add    $0x4420800,%eax
+   2e2317187:	xor    %al,(%rbx)
+   2e2317189:	(bad)
+   2e231718a:	add    0x1(%rax),%dh
+   2e231718d:	push   %rax
+   2e231718e:	add    %al,(%rax)
+   2e2317190:	add    %eax,(%rdi)
+   2e2317192:	add    $0x0,%al
+   2e2317194:	(bad)
+   2e2317195:	xor    (%rbx),%al
+   2e2317197:	xor    %al,(%rdx)
+   2e2317199:	(bad)
+   2e231719a:	add    %esi,0x1(%rax)
+   2e231719d:	add    $0x1,%al
+   2e231719f:	add    %al,(%rdx,%riz,4)
+   2e23171a2:	add    %al,(%rax)
+   2e23171a4:	add    %eax,(%rax)
    2e23171a6:	add    %al,(%rax)
-   2e23171a8:	add    %ecx,(%rax)
-   2e23171aa:	add    $0x0,%al
-   2e23171ac:	or     %dh,(%rdx)
-   2e23171ae:	add    $0x30,%al
-   2e23171b0:	add    0x2(%rax),%esp
-   2e23171b3:	rolb   $0x5,(%rcx)
-   2e23171b6:	add    (%rax),%al
-   2e23171b8:	add    $0x1300132,%eax
-   2e23171bd:	add    $0x1,%al
-   2e23171bf:	add    %al,(%rdx,%riz,4)
-   2e23171c2:	add    %al,(%rax)
-   2e23171c4:	add    %eax,(%rax)
-   2e23171c6:	add    %al,(%rax)
-   2e23171c8:	add    %eax,(%rax)
+   2e23171a8:	add    %eax,(%rax)
 	...
 
 Disassembly of section .edata:
 
 00000002e2319000 <.edata>:
    2e2319000:	add    %al,(%rax)
    2e2319002:	add    %al,(%rax)
-   2e2319004:	out    %eax,(%dx)
-   2e2319005:	mov    $0xb4,%ch
-   2e2319007:	movsxd (%rax),%eax
-   2e2319009:	add    %al,(%rax)
-   2e231900b:	add    %cl,0x10000(%rax,%rdx,4)
+   2e2319004:	cld
+   2e2319005:	xchg   %eax,%ecx
+   2e2319006:	xlat   %ds:(%rbx)
+   2e2319007:	add    %al,%gs:(%rax)
+   2e231900a:	add    %al,(%rax)
+   2e231900c:	mov    %ss,0x10000(%rax)
    2e2319012:	add    %al,(%rax)
    2e2319014:	or     (%rax),%al
    2e2319016:	add    %al,(%rax)
    2e2319018:	or     (%rax),%al
    2e231901a:	add    %al,(%rax)
    2e231901c:	sub    %dl,-0x6fb00000(%rax)
    2e2319022:	add    %al,(%rax)
    2e2319024:	js     0x2e2318fb6
    2e2319026:	add    %al,(%rax)
-   2e2319028:	movabs 0xb000001400000013,%al
-   2e2319031:	sbb    %al,(%rax)
-   2e2319033:	add    %al,(%rax)
-   2e2319035:	adc    $0x15900000,%eax
-   2e231903a:	add    %al,(%rax)
-   2e231903c:	adc    %ah,(%rax)
+   2e2319028:	jo     0x2e231903d
+   2e231902a:	add    %al,(%rax)
+   2e231902c:	rclb   $1,(%rbx)
+   2e231902e:	add    %al,(%rax)
+   2e2319030:	rex sbb %al,(%rax)
+   2e2319033:	add    %ah,0x20000014(%rax)
+   2e2319039:	adc    $0x21200000,%eax
    2e231903e:	add    %al,(%rax)
-   2e2319040:	rcrb   $0x0,(%rax)
-   2e2319043:	add    %ah,%al
-   2e2319045:	(bad)
-   2e2319046:	add    %al,(%rax)
-   2e2319048:	jo     0x2e231905e
-   2e231904a:	add    %al,(%rax)
-   2e231904c:	rclb   $0x0,(%rbx)
-   2e231904f:	add    %bl,-0x6f590000(%rax,%rdx,4)
+   2e2319040:	push   %rax
+   2e2319041:	sbb    %al,(%rax)
+   2e2319043:	add    %dh,%al
+   2e2319045:	and    %al,(%rax)
+   2e2319047:	add    %dh,(%rax)
+   2e2319049:	adc    $0x0,%al
+   2e231904b:	add    %dl,-0x63ffffed(%rax)
+   2e2319051:	nop
+   2e2319052:	add    %al,(%rax)
+   2e2319054:	cmpsl  %es:(%rdi),%ds:(%rsi)
+   2e2319055:	nop
    2e2319056:	add    %al,(%rax)
    2e2319058:	mov    $0x90,%ah
    2e231905a:	add    %al,(%rax)
    2e231905c:	mov    $0xc3000090,%ebx
    2e2319061:	nop
    2e2319062:	add    %al,(%rax)
    2e2319064:	lret
@@ -4172,331 +4129,321 @@
    2e23190fc:	pop    %rdi
    2e23190fd:	insl   (%dx),%es:(%rdi)
 	...
 
 Disassembly of section .idata:
 
 00000002e231a000 <.idata>:
-   2e231a000:	cmp    $0xa0,%al
-	...
+   2e231a000:	rex movabs 0x0,%al
    2e231a00a:	add    %al,(%rax)
-   2e231a00c:	movabs 0x8c0000a1240000a3,%al
-   2e231a015:	movabs 0x0,%al
+   2e231a00c:	movsb  %ds:(%rsi),%es:(%rdi)
+   2e231a00d:	movabs %eax,0xa0900000a1280000
+	...
    2e231a01e:	add    %al,(%rax)
-   2e231a020:	clc
-   2e231a021:	movabs %eax,0xa1740000
+   2e231a020:	cld
+   2e231a021:	movabs %eax,0xa1780000
 	...
-   2e231a03a:	add    %al,(%rax)
-   2e231a03c:	or     $0xa2,%al
    2e231a03e:	add    %al,(%rax)
-   2e231a040:	add    %al,(%rax)
-   2e231a042:	add    %al,(%rax)
-   2e231a044:	and    $0xa2,%al
+   2e231a040:	adc    %ah,0x0(%rdx)
    2e231a046:	add    %al,(%rax)
-   2e231a048:	add    %al,(%rax)
-   2e231a04a:	add    %al,(%rax)
-   2e231a04c:	cmp    $0xa2,%al
+   2e231a048:	sub    %ah,0x0(%rdx)
    2e231a04e:	add    %al,(%rax)
-   2e231a050:	add    %al,(%rax)
-   2e231a052:	add    %al,(%rax)
-   2e231a054:	rex.WR movabs %al,0xa268000000000000
+   2e231a050:	rex movabs %al,0xa250000000000000
+   2e231a05a:	add    %al,(%rax)
+   2e231a05c:	add    %al,(%rax)
    2e231a05e:	add    %al,(%rax)
-   2e231a060:	add    %al,(%rax)
-   2e231a062:	add    %al,(%rax)
-   2e231a064:	andb   $0x0,0x0(%rdx)
-   2e231a06b:	add    %cl,0xa2(%rax)
-   2e231a071:	add    %al,(%rax)
-   2e231a073:	add    %dl,0xa2(%rsi)
-   2e231a079:	add    %al,(%rax)
-   2e231a07b:	add    %ch,0xa2(%rax)
-	...
-   2e231a089:	add    %al,(%rax)
-   2e231a08b:	add    %bh,0xa2(%rax)
-   2e231a091:	add    %al,(%rax)
-   2e231a093:	add    %al,%dh
-   2e231a095:	movabs %al,0xa2da000000000000
-   2e231a09e:	add    %al,(%rax)
-   2e231a0a0:	add    %al,(%rax)
+   2e231a060:	insb   (%dx),%es:(%rdi)
+   2e231a061:	movabs %al,0xa284000000000000
+   2e231a06a:	add    %al,(%rax)
+   2e231a06c:	add    %al,(%rax)
+   2e231a06e:	add    %al,(%rax)
+   2e231a070:	mov    %fs,0x0(%rdx)
+   2e231a076:	add    %al,(%rax)
+   2e231a078:	(bad)
+   2e231a079:	movabs %al,0xa2ac000000000000
+	...
+   2e231a08e:	add    %al,(%rax)
+   2e231a090:	mov    $0xa2,%esp
+   2e231a095:	add    %al,(%rax)
+   2e231a097:	add    %cl,%dl
+   2e231a099:	movabs %al,0xa2de000000000000
    2e231a0a2:	add    %al,(%rax)
-   2e231a0a4:	call   0x2e231a14b
-   2e231a0a9:	add    %al,(%rax)
-   2e231a0ab:	add    %dh,%dl
-   2e231a0ad:	movabs %al,0xa2fe000000000000
+   2e231a0a4:	add    %al,(%rax)
+   2e231a0a6:	add    %al,(%rax)
+   2e231a0a8:	in     (%dx),%al
+   2e231a0a9:	movabs %al,0xa2f6000000000000
+   2e231a0b2:	add    %al,(%rax)
+   2e231a0b4:	add    %al,(%rax)
    2e231a0b6:	add    %al,(%rax)
-   2e231a0b8:	add    %al,(%rax)
-   2e231a0ba:	add    %al,(%rax)
-   2e231a0bc:	(bad)
-   2e231a0bd:	movabs %eax,0xa310000000000000
+   2e231a0b8:	add    0x0(%rbx),%ah
+   2e231a0be:	add    %al,(%rax)
+   2e231a0c0:	or     0x0(%rbx),%ah
    2e231a0c6:	add    %al,(%rax)
-   2e231a0c8:	add    %al,(%rax)
+   2e231a0c8:	adc    $0xa3,%al
    2e231a0ca:	add    %al,(%rax)
-   2e231a0cc:	sbb    %ah,0x0(%rbx)
+   2e231a0cc:	add    %al,(%rax)
+   2e231a0ce:	add    %al,(%rax)
+   2e231a0d0:	sbb    $0xa3,%al
    2e231a0d2:	add    %al,(%rax)
-   2e231a0d4:	and    0x0(%rbx),%ah
-   2e231a0da:	add    %al,(%rax)
-   2e231a0dc:	sub    0x0(%rbx),%ah
+   2e231a0d4:	add    %al,(%rax)
+   2e231a0d6:	add    %al,(%rax)
+   2e231a0d8:	es movabs %eax,0xa32e000000000000
    2e231a0e2:	add    %al,(%rax)
-   2e231a0e4:	xor    $0xa3,%al
+   2e231a0e4:	add    %al,(%rax)
    2e231a0e6:	add    %al,(%rax)
-   2e231a0e8:	add    %al,(%rax)
-   2e231a0ea:	add    %al,(%rax)
-   2e231a0ec:	ds movabs %eax,0xa348000000000000
-   2e231a0f6:	add    %al,(%rax)
-   2e231a0f8:	add    %al,(%rax)
+   2e231a0e8:	cmp    %ah,0x0(%rbx)
+   2e231a0ee:	add    %al,(%rax)
+   2e231a0f0:	rex.X movabs %eax,0xa34c000000000000
    2e231a0fa:	add    %al,(%rax)
-   2e231a0fc:	push   %rax
-   2e231a0fd:	movabs %eax,0xa35a000000000000
-   2e231a106:	add    %al,(%rax)
-   2e231a108:	add    %al,(%rax)
+   2e231a0fc:	add    %al,(%rax)
+   2e231a0fe:	add    %al,(%rax)
+   2e231a100:	push   %rsp
+   2e231a101:	movabs %eax,0xa35e000000000000
    2e231a10a:	add    %al,(%rax)
-   2e231a10c:	movabs %eax,%fs:0xa36e000000000000
+   2e231a10c:	add    %al,(%rax)
+   2e231a10e:	add    %al,(%rax)
+   2e231a110:	push   $0xa3
+   2e231a115:	add    %al,(%rax)
+   2e231a117:	add    %dh,-0x5d(%rdx)
 	...
-   2e231a122:	add    %al,(%rax)
-   2e231a124:	or     $0xa2,%al
    2e231a126:	add    %al,(%rax)
-   2e231a128:	add    %al,(%rax)
-   2e231a12a:	add    %al,(%rax)
-   2e231a12c:	and    $0xa2,%al
+   2e231a128:	adc    %ah,0x0(%rdx)
    2e231a12e:	add    %al,(%rax)
-   2e231a130:	add    %al,(%rax)
-   2e231a132:	add    %al,(%rax)
-   2e231a134:	cmp    $0xa2,%al
+   2e231a130:	sub    %ah,0x0(%rdx)
    2e231a136:	add    %al,(%rax)
-   2e231a138:	add    %al,(%rax)
-   2e231a13a:	add    %al,(%rax)
-   2e231a13c:	rex.WR movabs %al,0xa268000000000000
+   2e231a138:	rex movabs %al,0xa250000000000000
+   2e231a142:	add    %al,(%rax)
+   2e231a144:	add    %al,(%rax)
    2e231a146:	add    %al,(%rax)
-   2e231a148:	add    %al,(%rax)
-   2e231a14a:	add    %al,(%rax)
-   2e231a14c:	andb   $0x0,0x0(%rdx)
-   2e231a153:	add    %cl,0xa2(%rax)
-   2e231a159:	add    %al,(%rax)
-   2e231a15b:	add    %dl,0xa2(%rsi)
-   2e231a161:	add    %al,(%rax)
-   2e231a163:	add    %ch,0xa2(%rax)
-	...
-   2e231a171:	add    %al,(%rax)
-   2e231a173:	add    %bh,0xa2(%rax)
-   2e231a179:	add    %al,(%rax)
-   2e231a17b:	add    %al,%dh
-   2e231a17d:	movabs %al,0xa2da000000000000
-   2e231a186:	add    %al,(%rax)
-   2e231a188:	add    %al,(%rax)
+   2e231a148:	insb   (%dx),%es:(%rdi)
+   2e231a149:	movabs %al,0xa284000000000000
+   2e231a152:	add    %al,(%rax)
+   2e231a154:	add    %al,(%rax)
+   2e231a156:	add    %al,(%rax)
+   2e231a158:	mov    %fs,0x0(%rdx)
+   2e231a15e:	add    %al,(%rax)
+   2e231a160:	(bad)
+   2e231a161:	movabs %al,0xa2ac000000000000
+	...
+   2e231a176:	add    %al,(%rax)
+   2e231a178:	mov    $0xa2,%esp
+   2e231a17d:	add    %al,(%rax)
+   2e231a17f:	add    %cl,%dl
+   2e231a181:	movabs %al,0xa2de000000000000
    2e231a18a:	add    %al,(%rax)
-   2e231a18c:	call   0x2e231a233
-   2e231a191:	add    %al,(%rax)
-   2e231a193:	add    %dh,%dl
-   2e231a195:	movabs %al,0xa2fe000000000000
+   2e231a18c:	add    %al,(%rax)
+   2e231a18e:	add    %al,(%rax)
+   2e231a190:	in     (%dx),%al
+   2e231a191:	movabs %al,0xa2f6000000000000
+   2e231a19a:	add    %al,(%rax)
+   2e231a19c:	add    %al,(%rax)
    2e231a19e:	add    %al,(%rax)
-   2e231a1a0:	add    %al,(%rax)
-   2e231a1a2:	add    %al,(%rax)
-   2e231a1a4:	(bad)
-   2e231a1a5:	movabs %eax,0xa310000000000000
+   2e231a1a0:	add    0x0(%rbx),%ah
+   2e231a1a6:	add    %al,(%rax)
+   2e231a1a8:	or     0x0(%rbx),%ah
    2e231a1ae:	add    %al,(%rax)
-   2e231a1b0:	add    %al,(%rax)
+   2e231a1b0:	adc    $0xa3,%al
    2e231a1b2:	add    %al,(%rax)
-   2e231a1b4:	sbb    %ah,0x0(%rbx)
+   2e231a1b4:	add    %al,(%rax)
+   2e231a1b6:	add    %al,(%rax)
+   2e231a1b8:	sbb    $0xa3,%al
    2e231a1ba:	add    %al,(%rax)
-   2e231a1bc:	and    0x0(%rbx),%ah
-   2e231a1c2:	add    %al,(%rax)
-   2e231a1c4:	sub    0x0(%rbx),%ah
+   2e231a1bc:	add    %al,(%rax)
+   2e231a1be:	add    %al,(%rax)
+   2e231a1c0:	es movabs %eax,0xa32e000000000000
    2e231a1ca:	add    %al,(%rax)
-   2e231a1cc:	xor    $0xa3,%al
+   2e231a1cc:	add    %al,(%rax)
    2e231a1ce:	add    %al,(%rax)
-   2e231a1d0:	add    %al,(%rax)
-   2e231a1d2:	add    %al,(%rax)
-   2e231a1d4:	ds movabs %eax,0xa348000000000000
-   2e231a1de:	add    %al,(%rax)
-   2e231a1e0:	add    %al,(%rax)
+   2e231a1d0:	cmp    %ah,0x0(%rbx)
+   2e231a1d6:	add    %al,(%rax)
+   2e231a1d8:	rex.X movabs %eax,0xa34c000000000000
    2e231a1e2:	add    %al,(%rax)
-   2e231a1e4:	push   %rax
-   2e231a1e5:	movabs %eax,0xa35a000000000000
-   2e231a1ee:	add    %al,(%rax)
-   2e231a1f0:	add    %al,(%rax)
+   2e231a1e4:	add    %al,(%rax)
+   2e231a1e6:	add    %al,(%rax)
+   2e231a1e8:	push   %rsp
+   2e231a1e9:	movabs %eax,0xa35e000000000000
    2e231a1f2:	add    %al,(%rax)
-   2e231a1f4:	movabs %eax,%fs:0xa36e000000000000
-	...
-   2e231a20a:	add    %al,(%rax)
-   2e231a20c:	sbb    (%rcx),%eax
-   2e231a20e:	rex.R
-   2e231a20f:	gs insb (%dx),%es:(%rdi)
-   2e231a211:	gs je  0x2e231a279
-   2e231a214:	rex.XB jb 0x2e231a280
-   2e231a217:	je     0x2e231a282
-   2e231a219:	movsxd 0x6c(%rcx),%esp
-   2e231a21c:	push   %rbx
-   2e231a21d:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   2e231a222:	outsb  %ds:(%rsi),(%dx)
-   2e231a223:	add    %bh,(%rdi)
-   2e231a225:	add    %eax,0x6e(%rbp)
-   2e231a228:	je     0x2e231a28f
-   2e231a22a:	jb     0x2e231a26f
-   2e231a22c:	jb     0x2e231a297
-   2e231a22e:	je     0x2e231a299
-   2e231a230:	movsxd 0x6c(%rcx),%esp
-   2e231a233:	push   %rbx
-   2e231a234:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   2e231a239:	outsb  %ds:(%rsi),(%dx)
-   2e231a23a:	add    %al,(%rax)
-   2e231a23c:	jbe    0x2e231a240
-   2e231a23e:	rex.RXB
-   2e231a23f:	gs je  0x2e231a28e
-   2e231a242:	(bad)
-   2e231a243:	jae    0x2e231a2b9
-   2e231a245:	rex.RB jb 0x2e231a2ba
-   2e231a248:	outsl  %ds:(%rsi),(%dx)
-   2e231a249:	jb     0x2e231a24b
-   2e231a24b:	add    %bh,0x49(%rbx,%rax,1)
-   2e231a24f:	outsb  %ds:(%rsi),(%dx)
-   2e231a250:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
-   2e231a258:	rex.XB jb 0x2e231a2c4
-   2e231a25b:	je     0x2e231a2c6
-   2e231a25d:	movsxd 0x6c(%rcx),%esp
-   2e231a260:	push   %rbx
-   2e231a261:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   2e231a266:	outsb  %ds:(%rsi),(%dx)
-   2e231a267:	add    %bl,%al
-   2e231a269:	add    0x61(%rbp,%riz,2),%ecx
-   2e231a26d:	jbe    0x2e231a2d4
-   2e231a26f:	rex.XB jb 0x2e231a2db
-   2e231a272:	je     0x2e231a2dd
-   2e231a274:	movsxd 0x6c(%rcx),%esp
-   2e231a277:	push   %rbx
-   2e231a278:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   2e231a27d:	outsb  %ds:(%rsi),(%dx)
-   2e231a27e:	add    %al,(%rax)
-   2e231a280:	(bad)
-   2e231a281:	add    $0x65656c53,%eax
-   2e231a286:	jo     0x2e231a288
-   2e231a288:	movsl  %ds:(%rsi),%es:(%rdi)
-   2e231a289:	add    $0x47736c54,%eax
-   2e231a28e:	gs je  0x2e231a2e7
-   2e231a291:	(bad)
-   2e231a292:	insb   (%dx),%es:(%rdi)
-   2e231a293:	jne    0x2e231a2fa
-   2e231a295:	add    %dl,%ah
-   2e231a297:	add    $0x74726956,%eax
-   2e231a29c:	jne    0x2e231a2ff
-   2e231a29e:	insb   (%dx),%es:(%rdi)
-   2e231a29f:	push   %rax
-   2e231a2a0:	jb     0x2e231a311
-   2e231a2a2:	je     0x2e231a309
-   2e231a2a4:	movsxd 0x0(%rax,%rax,1),%esi
-   2e231a2a8:	(bad)
-   2e231a2a9:	add    $0x74726956,%eax
-   2e231a2ae:	jne    0x2e231a311
-   2e231a2b0:	insb   (%dx),%es:(%rdi)
-   2e231a2b1:	push   %rcx
-   2e231a2b2:	jne    0x2e231a319
-   2e231a2b4:	jb     0x2e231a32f
-   2e231a2b6:	add    %al,(%rax)
-   2e231a2b8:	push   %rsp
-   2e231a2b9:	add    %bl,0x5f(%rdi)
-   2e231a2bc:	imul   $0x6e75665f,0x62(%rdi),%ebp
-   2e231a2c3:	movsxd (%rax),%eax
-   2e231a2c5:	add    %ah,0x0(%rbx)
-   2e231a2c8:	pop    %rdi
-   2e231a2c9:	pop    %rdi
-   2e231a2ca:	jae    0x2e231a331
-   2e231a2cc:	je     0x2e231a343
+   2e231a1f4:	add    %al,(%rax)
+   2e231a1f6:	add    %al,(%rax)
+   2e231a1f8:	push   $0xa3
+   2e231a1fd:	add    %al,(%rax)
+   2e231a1ff:	add    %dh,-0x5d(%rdx)
+	...
+   2e231a20e:	add    %al,(%rax)
+   2e231a210:	sbb    %eax,(%rcx)
+   2e231a212:	rex.R
+   2e231a213:	gs insb (%dx),%es:(%rdi)
+   2e231a215:	gs je  0x2e231a27d
+   2e231a218:	rex.XB jb 0x2e231a284
+   2e231a21b:	je     0x2e231a286
+   2e231a21d:	movsxd 0x6c(%rcx),%esp
+   2e231a220:	push   %rbx
+   2e231a221:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   2e231a226:	outsb  %ds:(%rsi),(%dx)
+   2e231a227:	add    %bh,0x746e4501(%rip)        # 0x3569fe72e
+   2e231a22d:	gs jb  0x2e231a273
+   2e231a230:	jb     0x2e231a29b
+   2e231a232:	je     0x2e231a29d
+   2e231a234:	movsxd 0x6c(%rcx),%esp
+   2e231a237:	push   %rbx
+   2e231a238:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   2e231a23d:	outsb  %ds:(%rsi),(%dx)
+   2e231a23e:	add    %al,(%rax)
+   2e231a240:	je     0x2e231a244
+   2e231a242:	rex.RXB
+   2e231a243:	gs je  0x2e231a292
+   2e231a246:	(bad)
+   2e231a247:	jae    0x2e231a2bd
+   2e231a249:	rex.RB jb 0x2e231a2be
+   2e231a24c:	outsl  %ds:(%rsi),(%dx)
+   2e231a24d:	jb     0x2e231a24f
+   2e231a24f:	add    %bh,0x3(%rdx)
+   2e231a252:	rex.WB outsb %ds:(%rsi),(%dx)
+   2e231a254:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   2e231a25c:	rex.XB jb 0x2e231a2c8
+   2e231a25f:	je     0x2e231a2ca
+   2e231a261:	movsxd 0x6c(%rcx),%esp
+   2e231a264:	push   %rbx
+   2e231a265:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   2e231a26a:	outsb  %ds:(%rsi),(%dx)
+   2e231a26b:	add    %dl,%dh
+   2e231a26d:	add    0x61(%rbp,%riz,2),%ecx
+   2e231a271:	jbe    0x2e231a2d8
+   2e231a273:	rex.XB jb 0x2e231a2df
+   2e231a276:	je     0x2e231a2e1
+   2e231a278:	movsxd 0x6c(%rcx),%esp
+   2e231a27b:	push   %rbx
+   2e231a27c:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   2e231a281:	outsb  %ds:(%rsi),(%dx)
+   2e231a282:	add    %al,(%rax)
+   2e231a284:	jg     0x2e231a28b
+   2e231a286:	push   %rbx
+   2e231a287:	insb   (%dx),%es:(%rdi)
+   2e231a288:	gs gs jo 0x2e231a28c
+   2e231a28c:	movabs %al,0x56746547736c5405
+   2e231a295:	(bad)
+   2e231a296:	insb   (%dx),%es:(%rdi)
+   2e231a297:	jne    0x2e231a2fe
+   2e231a299:	add    %dl,%cl
+   2e231a29b:	add    $0x74726956,%eax
+   2e231a2a0:	jne    0x2e231a303
+   2e231a2a2:	insb   (%dx),%es:(%rdi)
+   2e231a2a3:	push   %rax
+   2e231a2a4:	jb     0x2e231a315
+   2e231a2a6:	je     0x2e231a30d
+   2e231a2a8:	movsxd 0x0(%rax,%rax,1),%esi
+   2e231a2ac:	roll   %cl,0x74726956(%rip)        # 0x356a40c08
+   2e231a2b2:	jne    0x2e231a315
+   2e231a2b4:	insb   (%dx),%es:(%rdi)
+   2e231a2b5:	push   %rcx
+   2e231a2b6:	jne    0x2e231a31d
+   2e231a2b8:	jb     0x2e231a333
+   2e231a2ba:	add    %al,(%rax)
+   2e231a2bc:	push   %rsp
+   2e231a2bd:	add    %bl,0x5f(%rdi)
+   2e231a2c0:	imul   $0x6e75665f,0x62(%rdi),%ebp
+   2e231a2c7:	movsxd (%rax),%eax
+   2e231a2c9:	add    %ah,0x0(%rbx)
+   2e231a2cc:	pop    %rdi
+   2e231a2cd:	pop    %rdi
    2e231a2ce:	jae    0x2e231a335
-   2e231a2d0:	jb     0x2e231a33f
-   2e231a2d2:	(bad)
-   2e231a2d3:	je     0x2e231a33d
-   2e231a2d5:	gs jb  0x2e231a34a
-   2e231a2d8:	add    %al,(%rax)
-   2e231a2da:	jns    0x2e231a2dc
-   2e231a2dc:	pop    %rdi
-   2e231a2dd:	(bad)
-   2e231a2de:	insl   (%dx),%es:(%rdi)
-   2e231a2df:	jae    0x2e231a348
-   2e231a2e1:	pop    %rdi
-   2e231a2e2:	gs js  0x2e231a34e
-   2e231a2e5:	je     0x2e231a2e7
-   2e231a2e7:	add    %bh,0x72655f00(%rsi)
-   2e231a2ed:	jb     0x2e231a35d
-   2e231a2ef:	outsl  %ds:(%rsi),(%dx)
-   2e231a2f0:	add    %al,(%rax)
-   2e231a2f2:	sbb    $0x6e695f01,%eax
-   2e231a2f7:	imul   $0x83006d72,0x65(%rsp,%rsi,2),%esi
-   2e231a2ff:	add    %ebx,0x6c(%rdi)
-   2e231a302:	outsl  %ds:(%rsi),(%dx)
-   2e231a303:	movsxd 0x0(%rbx),%ebp
-   2e231a306:	lret   $0x5f02
-   2e231a309:	jne    0x2e231a379
-   2e231a30b:	insb   (%dx),%es:(%rdi)
-   2e231a30c:	outsl  %ds:(%rsi),(%dx)
-   2e231a30d:	movsxd 0x0(%rbx),%ebp
-   2e231a310:	mov    (%rbx),%al
-   2e231a312:	(bad)
-   2e231a313:	(bad)
-   2e231a318:	fwait
-   2e231a319:	add    0x61(%rbx),%esp
-   2e231a31c:	insb   (%dx),%es:(%rdi)
-   2e231a31d:	insb   (%dx),%es:(%rdi)
-   2e231a31e:	outsl  %ds:(%rsi),(%dx)
-   2e231a31f:	movsxd (%rax),%eax
-   2e231a321:	add    %al,%bl
-   2e231a323:	add    0x72(%rsi),%esp
-   2e231a326:	gs add %al,%gs:(%rax)
-   2e231a32a:	rolb   $1,(%rbx)
-   2e231a32c:	data16 ja 0x2e231a3a1
-   2e231a32f:	imul   $0x6d03ff00,0x0(%rbp,%riz,2),%esi
-   2e231a337:	(bad)
-   2e231a338:	insb   (%dx),%es:(%rdi)
-   2e231a339:	insb   (%dx),%es:(%rdi)
-   2e231a33a:	outsl  %ds:(%rsi),(%dx)
-   2e231a33b:	movsxd (%rax),%eax
-   2e231a33d:	add    %al,(%rdi)
-   2e231a33f:	add    $0x6d,%al
-   2e231a341:	gs insl (%dx),%es:(%rdi)
-   2e231a343:	movsxd 0x79(%rax),%esi
-   2e231a346:	add    %al,(%rax)
-   2e231a348:	sbb    %al,(%rcx,%rsi,2)
-   2e231a34b:	jae    0x2e231a3bc
-   2e231a34d:	jb     0x2e231a3c3
-   2e231a34f:	add    %bl,(%rsp,%rax,1)
-   2e231a352:	jb     0x2e231a3b9
-   2e231a354:	(bad)
-   2e231a355:	insb   (%dx),%es:(%rdi)
-   2e231a356:	insb   (%dx),%es:(%rdi)
-   2e231a357:	outsl  %ds:(%rsi),(%dx)
-   2e231a358:	movsxd (%rax),%eax
-   2e231a35a:	ds add $0x73,%al
-   2e231a35d:	je     0x2e231a3d1
-   2e231a35f:	insb   (%dx),%es:(%rdi)
-   2e231a360:	outsb  %gs:(%rsi),(%dx)
-   2e231a362:	add    %al,(%rax)
-   2e231a364:	rex.B add $0x73,%al
-   2e231a367:	je     0x2e231a3db
-   2e231a369:	outsb  %ds:(%rsi),(%dx)
-   2e231a36a:	movsxd 0x70(%rbp),%ebp
-   2e231a36d:	add    %ah,0x4(%rbx)
-   2e231a370:	jbe    0x2e231a3d8
-   2e231a372:	jo     0x2e231a3e6
-   2e231a374:	imul   $0x66,0x74(%rsi),%ebp
-   2e231a37b:	add    %al,(%rax)
-   2e231a37d:	movabs 0xa0000000a0000000,%al
-   2e231a386:	add    %al,(%rax)
-   2e231a388:	add    %ah,-0x60000000(%rax)
-   2e231a38e:	add    %al,(%rax)
-   2e231a390:	add    %ah,-0x60000000(%rax)
-   2e231a396:	add    %al,(%rax)
-   2e231a398:	add    %ah,-0x60000000(%rax)
-   2e231a39e:	add    %al,(%rax)
-   2e231a3a0:	rex.WXB
-   2e231a3a1:	rex.RB push %r10
-   2e231a3a3:	rex.WRX
-   2e231a3a4:	rex.RB
-   2e231a3a5:	xor    (%rdx),%r14
-   2e231a3a8:	cs fs insb (%dx),%es:(%rdi)
-   2e231a3ab:	insb   (%dx),%es:(%rdi)
-   2e231a3ac:	add    %al,(%rax)
-   2e231a3ae:	add    %al,(%rax)
-   2e231a3b0:	adc    $0xa0,%al
+   2e231a2d0:	je     0x2e231a347
+   2e231a2d2:	jae    0x2e231a339
+   2e231a2d4:	jb     0x2e231a343
+   2e231a2d6:	(bad)
+   2e231a2d7:	je     0x2e231a341
+   2e231a2d9:	gs jb  0x2e231a34e
+   2e231a2dc:	add    %al,(%rax)
+   2e231a2de:	js     0x2e231a2e0
+   2e231a2e0:	pop    %rdi
+   2e231a2e1:	(bad)
+   2e231a2e2:	insl   (%dx),%es:(%rdi)
+   2e231a2e3:	jae    0x2e231a34c
+   2e231a2e5:	pop    %rdi
+   2e231a2e6:	gs js  0x2e231a352
+   2e231a2e9:	je     0x2e231a2eb
+   2e231a2eb:	add    %bh,0x7272655f(%rax,%rax,1)
+   2e231a2f2:	outsb  %ds:(%rsi),(%dx)
+   2e231a2f3:	outsl  %ds:(%rsi),(%dx)
+   2e231a2f4:	add    %al,(%rax)
+   2e231a2f6:	sbb    $0x6e695f01,%eax
+   2e231a2fb:	imul   $0x83006d72,0x65(%rsp,%rsi,2),%esi
+   2e231a303:	add    %ebx,0x6c(%rdi)
+   2e231a306:	outsl  %ds:(%rsi),(%dx)
+   2e231a307:	movsxd 0x0(%rbx),%ebp
+   2e231a30a:	lret   $0x5f02
+   2e231a30d:	jne    0x2e231a37d
+   2e231a30f:	insb   (%dx),%es:(%rdi)
+   2e231a310:	outsl  %ds:(%rsi),(%dx)
+   2e231a311:	movsxd 0x0(%rbx),%ebp
+   2e231a314:	xchg   %eax,(%rbx)
+   2e231a316:	(bad)
+   2e231a317:	(bad)
+   2e231a31c:	cwtl
+   2e231a31d:	add    0x61(%rbx),%esp
+   2e231a320:	insb   (%dx),%es:(%rdi)
+   2e231a321:	insb   (%dx),%es:(%rdi)
+   2e231a322:	outsl  %ds:(%rsi),(%dx)
+   2e231a323:	movsxd (%rax),%eax
+   2e231a325:	add    %al,%al
+   2e231a327:	add    0x72(%rsi),%esp
+   2e231a32a:	gs add %al,%gs:(%rax)
+   2e231a32e:	int    $0x3
+   2e231a330:	data16 ja 0x2e231a3a5
+   2e231a333:	imul   $0x6d03fd00,0x0(%rbp,%riz,2),%esi
+   2e231a33b:	(bad)
+   2e231a33c:	insb   (%dx),%es:(%rdi)
+   2e231a33d:	insb   (%dx),%es:(%rdi)
+   2e231a33e:	outsl  %ds:(%rsi),(%dx)
+   2e231a33f:	movsxd (%rax),%eax
+   2e231a341:	add    %al,0x6d656d04(%rip)        # 0x34f97104b
+   2e231a347:	movsxd 0x79(%rax),%esi
+   2e231a34a:	add    %al,(%rax)
+   2e231a34c:	(bad)
+   2e231a34d:	add    $0x71,%al
+   2e231a34f:	jae    0x2e231a3c0
+   2e231a351:	jb     0x2e231a3c7
+   2e231a353:	add    %bl,(%rdx)
+   2e231a355:	add    $0x72,%al
+   2e231a357:	gs (bad)
+   2e231a359:	insb   (%dx),%es:(%rdi)
+   2e231a35a:	insb   (%dx),%es:(%rdi)
+   2e231a35b:	outsl  %ds:(%rsi),(%dx)
+   2e231a35c:	movsxd (%rax),%eax
+   2e231a35e:	cmp    $0x4,%al
+   2e231a360:	jae    0x2e231a3d6
+   2e231a362:	jb     0x2e231a3d0
+   2e231a364:	outsb  %gs:(%rsi),(%dx)
+   2e231a366:	add    %al,(%rax)
+   2e231a368:	(bad)
+   2e231a369:	add    $0x73,%al
+   2e231a36b:	je     0x2e231a3df
+   2e231a36d:	outsb  %ds:(%rsi),(%dx)
+   2e231a36e:	movsxd 0x70(%rbp),%ebp
+   2e231a371:	add    %ah,0x4(%rax)
+   2e231a374:	jbe    0x2e231a3dc
+   2e231a376:	jo     0x2e231a3ea
+   2e231a378:	imul   $0x66,0x74(%rsi),%ebp
+   2e231a37f:	add    %al,(%rax)
+   2e231a381:	movabs 0xa0000000a0000000,%al
+   2e231a38a:	add    %al,(%rax)
+   2e231a38c:	add    %ah,-0x60000000(%rax)
+   2e231a392:	add    %al,(%rax)
+   2e231a394:	add    %ah,-0x60000000(%rax)
+   2e231a39a:	add    %al,(%rax)
+   2e231a39c:	add    %ah,-0x60000000(%rax)
+   2e231a3a2:	add    %al,(%rax)
+   2e231a3a4:	rex.WXB
+   2e231a3a5:	rex.RB push %r10
+   2e231a3a7:	rex.WRX
+   2e231a3a8:	rex.RB
+   2e231a3a9:	xor    (%rdx),%r14
+   2e231a3ac:	cs fs insb (%dx),%es:(%rdi)
+   2e231a3af:	insb   (%dx),%es:(%rdi)
+   2e231a3b0:	add    %al,(%rax)
    2e231a3b2:	add    %al,(%rax)
    2e231a3b4:	adc    $0xa0,%al
    2e231a3b6:	add    %al,(%rax)
    2e231a3b8:	adc    $0xa0,%al
    2e231a3ba:	add    %al,(%rax)
    2e231a3bc:	adc    $0xa0,%al
    2e231a3be:	add    %al,(%rax)
@@ -4524,35 +4471,38 @@
    2e231a3ea:	add    %al,(%rax)
    2e231a3ec:	adc    $0xa0,%al
    2e231a3ee:	add    %al,(%rax)
    2e231a3f0:	adc    $0xa0,%al
    2e231a3f2:	add    %al,(%rax)
    2e231a3f4:	adc    $0xa0,%al
    2e231a3f6:	add    %al,(%rax)
-   2e231a3f8:	insl   (%dx),%es:(%rdi)
-   2e231a3f9:	jae    0x2e231a471
-   2e231a3fb:	movsxd 0x74(%rdx),%esi
-   2e231a3fe:	cs fs insb (%dx),%es:(%rdi)
-   2e231a401:	insb   (%dx),%es:(%rdi)
+   2e231a3f8:	adc    $0xa0,%al
+   2e231a3fa:	add    %al,(%rax)
+   2e231a3fc:	insl   (%dx),%es:(%rdi)
+   2e231a3fd:	jae    0x2e231a475
+   2e231a3ff:	movsxd 0x74(%rdx),%esi
+   2e231a402:	cs fs insb (%dx),%es:(%rdi)
+   2e231a405:	insb   (%dx),%es:(%rdi)
 	...
 
 Disassembly of section .CRT:
 
 00000002e231b000 <.CRT>:
 	...
    2e231b018:	add    %dl,(%rax)
    2e231b01a:	xor    %esp,%edx
    2e231b01c:	add    (%rax),%al
 	...
    2e231b02e:	add    %al,(%rax)
-   2e231b030:	rex and %esi,(%rcx)
+   2e231b030:	push   %rax
+   2e231b031:	and    (%rcx),%dh
    2e231b033:	loop   0x2e231b037
    2e231b035:	add    %al,(%rax)
-   2e231b037:	add    %dl,(%rax)
-   2e231b039:	and    %esi,(%rcx)
+   2e231b037:	add    %ah,(%rax)
+   2e231b039:	and    (%rcx),%dh
    2e231b03b:	loop   0x2e231b03f
 	...
 
 Disassembly of section .tls:
 
 00000002e231c000 <.tls>:
 	...
@@ -4560,26 +4510,28 @@
 Disassembly of section .reloc:
 
 00000002e231d000 <.reloc>:
    2e231d000:	add    %dh,(%rax)
    2e231d002:	add    %al,(%rax)
    2e231d004:	or     $0x0,%al
    2e231d006:	add    %al,(%rax)
-   2e231d008:	push   $0xa2
-   2e231d00d:	rex add %al,(%rax)
+   2e231d008:	sub    %ah,0x40000000(%rbx)
+   2e231d00e:	add    %al,(%rax)
    2e231d010:	adc    $0x0,%al
    2e231d012:	add    %al,(%rax)
-   2e231d014:	adc    %ah,-0x5fb75fc0(%rax)
-   2e231d01a:	push   %rax
+   2e231d014:	adc    %ah,-0x5faf5fc0(%rax)
+   2e231d01a:	pop    %rax
    2e231d01b:	movabs 0x50000000a060,%al
    2e231d024:	xor    %al,(%rax)
    2e231d026:	add    %al,(%rax)
    2e231d028:	and    %ah,-0x5fb75fc0(%rax)
    2e231d02e:	push   %rax
-   2e231d02f:	movabs 0xa1e0a1d0a1c0a058,%al
-   2e231d038:	lock movabs 0xa230a220a210a200,%eax
-   2e231d042:	rex movabs %al,0xa280a270a260a250
-   2e231d04c:	nop
-   2e231d04d:	movabs %al,0x100000b0000000
+   2e231d02f:	movabs 0xa230a220a210a058,%al
+   2e231d038:	rex movabs %al,0xa280a270a260a250
+   2e231d042:	nop
+   2e231d043:	movabs %al,0xa2d0a2c0a2b0a2a0
+   2e231d04c:	loopne 0x2e231cff0
+   2e231d04e:	add    %al,(%rax)
+   2e231d050:	add    %dh,0x100000(%rax)
    2e231d056:	add    %al,(%rax)
    2e231d058:	sbb    %ah,-0x5fc75fd0(%rax)
 	...
```

### Comparing `bmxp-0.0.9/bmxp/gravity/correlation.so` & `bmxp-0.1.0/bmxp/gravity/correlation.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 24% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          14200 (bytes into file)
+  Start of section headers:          14168 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         11
   Size of section headers:           64 (bytes)
   Number of section headers:         30
   Section header string table index: 29
```

#### readelf --wide --program-header {}

```diff
@@ -2,24 +2,24 @@
 Elf file type is DYN (Shared object file)
 Entry point 0x0
 There are 11 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
   LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000838 0x000838 R   0x1000
-  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000d55 0x000d55 R E 0x1000
-  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x000254 0x000254 R   0x1000
-  LOAD           0x002e08 0x0000000000003e08 0x0000000000003e08 0x000270 0x000278 RW  0x1000
-  DYNAMIC        0x002e18 0x0000000000003e18 0x0000000000003e18 0x0001c0 0x0001c0 RW  0x8
+  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000ec1 0x000ec1 R E 0x1000
+  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x000268 0x000268 R   0x1000
+  LOAD           0x002df0 0x0000000000003df0 0x0000000000003df0 0x000270 0x000278 RW  0x1000
+  DYNAMIC        0x002e00 0x0000000000003e00 0x0000000000003e00 0x0001c0 0x0001c0 RW  0x8
   NOTE           0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   NOTE           0x0002c8 0x00000000000002c8 0x00000000000002c8 0x000024 0x000024 R   0x4
   GNU_PROPERTY   0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   GNU_EH_FRAME   0x002010 0x0000000000002010 0x0000000000002010 0x000074 0x000074 R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
-  GNU_RELRO      0x002e08 0x0000000000003e08 0x0000000000003e08 0x0001f8 0x0001f8 R   0x1
+  GNU_RELRO      0x002df0 0x0000000000003df0 0x0000000000003df0 0x000210 0x000210 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     .note.gnu.property .note.gnu.build-id .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt 
    01     .init .plt .plt.got .plt.sec .text .fini 
    02     .rodata .eh_frame_hdr .eh_frame 
    03     .init_array .fini_array .dynamic .got .got.plt .data .bss
```

#### readelf --wide --sections {}

```diff
@@ -1,8 +1,8 @@
-There are 30 section headers, starting at offset 0x3778:
+There are 30 section headers, starting at offset 0x3758:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.property NOTE            00000000000002a8 0002a8 000020 00   A  0   0  8
   [ 2] .note.gnu.build-id NOTE            00000000000002c8 0002c8 000024 00   A  0   0  4
   [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 00004c 00   A  4   0  8
@@ -12,28 +12,28 @@
   [ 7] .gnu.version_r    VERNEED         0000000000000640 000640 000030 00   A  5   1  8
   [ 8] .rela.dyn         RELA            0000000000000670 000670 0000c0 18   A  4   0  8
   [ 9] .rela.plt         RELA            0000000000000730 000730 000108 18  AI  4  23  8
   [10] .init             PROGBITS        0000000000001000 001000 00001b 00  AX  0   0  4
   [11] .plt              PROGBITS        0000000000001020 001020 0000c0 10  AX  0   0 16
   [12] .plt.got          PROGBITS        00000000000010e0 0010e0 000010 10  AX  0   0 16
   [13] .plt.sec          PROGBITS        00000000000010f0 0010f0 0000b0 10  AX  0   0 16
-  [14] .text             PROGBITS        00000000000011a0 0011a0 000ba6 00  AX  0   0 16
-  [15] .fini             PROGBITS        0000000000001d48 001d48 00000d 00  AX  0   0  4
+  [14] .text             PROGBITS        00000000000011a0 0011a0 000d13 00  AX  0   0 16
+  [15] .fini             PROGBITS        0000000000001eb4 001eb4 00000d 00  AX  0   0  4
   [16] .rodata           PROGBITS        0000000000002000 002000 000010 08  AM  0   0  8
   [17] .eh_frame_hdr     PROGBITS        0000000000002010 002010 000074 00   A  0   0  4
-  [18] .eh_frame         PROGBITS        0000000000002088 002088 0001cc 00   A  0   0  8
-  [19] .init_array       INIT_ARRAY      0000000000003e08 002e08 000008 08  WA  0   0  8
-  [20] .fini_array       FINI_ARRAY      0000000000003e10 002e10 000008 08  WA  0   0  8
-  [21] .dynamic          DYNAMIC         0000000000003e18 002e18 0001c0 10  WA  5   0  8
-  [22] .got              PROGBITS        0000000000003fd8 002fd8 000028 08  WA  0   0  8
-  [23] .got.plt          PROGBITS        0000000000004000 003000 000070 08  WA  0   0  8
-  [24] .data             PROGBITS        0000000000004070 003070 000008 00  WA  0   0  8
-  [25] .bss              NOBITS          0000000000004078 003078 000008 00  WA  0   0  1
-  [26] .comment          PROGBITS        0000000000000000 003078 00002b 01  MS  0   0  1
-  [27] .symtab           SYMTAB          0000000000000000 0030a8 0003a8 18     28  20  8
-  [28] .strtab           STRTAB          0000000000000000 003450 000218 00      0   0  1
-  [29] .shstrtab         STRTAB          0000000000000000 003668 00010d 00      0   0  1
+  [18] .eh_frame         PROGBITS        0000000000002088 002088 0001e0 00   A  0   0  8
+  [19] .init_array       INIT_ARRAY      0000000000003df0 002df0 000008 08  WA  0   0  8
+  [20] .fini_array       FINI_ARRAY      0000000000003df8 002df8 000008 08  WA  0   0  8
+  [21] .dynamic          DYNAMIC         0000000000003e00 002e00 0001c0 10  WA  5   0  8
+  [22] .got              PROGBITS        0000000000003fc0 002fc0 000028 08  WA  0   0  8
+  [23] .got.plt          PROGBITS        0000000000003fe8 002fe8 000070 08  WA  0   0  8
+  [24] .data             PROGBITS        0000000000004058 003058 000008 00  WA  0   0  8
+  [25] .bss              NOBITS          0000000000004060 003060 000008 00  WA  0   0  1
+  [26] .comment          PROGBITS        0000000000000000 003060 000025 01  MS  0   0  1
+  [27] .symtab           SYMTAB          0000000000000000 003088 0003a8 18     28  20  8
+  [28] .strtab           STRTAB          0000000000000000 003430 000218 00      0   0  1
+  [29] .shstrtab         STRTAB          0000000000000000 003648 00010d 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -8,58 +8,58 @@
      4: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
      5: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_2.14 (3)
      6: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5 (2)
      7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND sqrt
      8: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
      9: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (2)
     10: 00000000000015b0     9 FUNC    GLOBAL DEFAULT   14 free_p
-    11: 0000000000001390   111 FUNC    GLOBAL DEFAULT   14 nanMask
-    12: 0000000000001400   418 FUNC    GLOBAL DEFAULT   14 pearson
-    13: 0000000000001d20    38 FUNC    GLOBAL DEFAULT   14 pearson_array
-    14: 0000000000001cf0    41 FUNC    GLOBAL DEFAULT   14 spearman_array
+    11: 0000000000001390   131 FUNC    GLOBAL DEFAULT   14 nanMask
+    12: 0000000000001420   400 FUNC    GLOBAL DEFAULT   14 pearson
+    13: 0000000000001e90    35 FUNC    GLOBAL DEFAULT   14 pearson_array
+    14: 0000000000001e60    41 FUNC    GLOBAL DEFAULT   14 spearman_array
     15: 0000000000001280    53 FUNC    GLOBAL DEFAULT   14 sum_m
-    16: 0000000000001310   119 FUNC    GLOBAL DEFAULT   14 stdev_m
+    16: 0000000000001310   114 FUNC    GLOBAL DEFAULT   14 stdev_m
     17: 0000000000001260    29 FUNC    GLOBAL DEFAULT   14 comparator
     18: 00000000000012c0    77 FUNC    GLOBAL DEFAULT   14 covariance_m
-    19: 00000000000015c0  1838 FUNC    GLOBAL DEFAULT   14 spearman
+    19: 00000000000015c0  2195 FUNC    GLOBAL DEFAULT   14 spearman
 
 Symbol table '.symtab' contains 39 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
      2: 00000000000011a0     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
      3: 00000000000011d0     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
      4: 0000000000001210     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
-     5: 0000000000004078     1 OBJECT  LOCAL  DEFAULT   25 completed.0
-     6: 0000000000003e10     0 OBJECT  LOCAL  DEFAULT   20 __do_global_dtors_aux_fini_array_entry
+     5: 0000000000004060     1 OBJECT  LOCAL  DEFAULT   25 completed.0
+     6: 0000000000003df8     0 OBJECT  LOCAL  DEFAULT   20 __do_global_dtors_aux_fini_array_entry
      7: 0000000000001250     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
-     8: 0000000000003e08     0 OBJECT  LOCAL  DEFAULT   19 __frame_dummy_init_array_entry
+     8: 0000000000003df0     0 OBJECT  LOCAL  DEFAULT   19 __frame_dummy_init_array_entry
      9: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS correlation.c
     10: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    11: 0000000000002250     0 OBJECT  LOCAL  DEFAULT   18 __FRAME_END__
+    11: 0000000000002264     0 OBJECT  LOCAL  DEFAULT   18 __FRAME_END__
     12: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
-    13: 0000000000001d48     0 FUNC    LOCAL  DEFAULT   15 _fini
-    14: 0000000000004070     0 OBJECT  LOCAL  DEFAULT   24 __dso_handle
-    15: 0000000000003e18     0 OBJECT  LOCAL  DEFAULT   21 _DYNAMIC
+    13: 0000000000001eb4     0 FUNC    LOCAL  DEFAULT   15 _fini
+    14: 0000000000004058     0 OBJECT  LOCAL  DEFAULT   24 __dso_handle
+    15: 0000000000003e00     0 OBJECT  LOCAL  DEFAULT   21 _DYNAMIC
     16: 0000000000002010     0 NOTYPE  LOCAL  DEFAULT   17 __GNU_EH_FRAME_HDR
-    17: 0000000000004078     0 OBJECT  LOCAL  DEFAULT   24 __TMC_END__
-    18: 0000000000004000     0 OBJECT  LOCAL  DEFAULT   23 _GLOBAL_OFFSET_TABLE_
+    17: 0000000000004060     0 OBJECT  LOCAL  DEFAULT   24 __TMC_END__
+    18: 0000000000003fe8     0 OBJECT  LOCAL  DEFAULT   23 _GLOBAL_OFFSET_TABLE_
     19: 0000000000001000     0 FUNC    LOCAL  DEFAULT   10 _init
     20: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5
     21: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
     22: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND qsort@GLIBC_2.2.5
     23: 00000000000015b0     9 FUNC    GLOBAL DEFAULT   14 free_p
-    24: 0000000000001390   111 FUNC    GLOBAL DEFAULT   14 nanMask
-    25: 0000000000001400   418 FUNC    GLOBAL DEFAULT   14 pearson
+    24: 0000000000001390   131 FUNC    GLOBAL DEFAULT   14 nanMask
+    25: 0000000000001420   400 FUNC    GLOBAL DEFAULT   14 pearson
     26: 00000000000012c0    77 FUNC    GLOBAL DEFAULT   14 covariance_m
-    27: 0000000000001d20    38 FUNC    GLOBAL DEFAULT   14 pearson_array
+    27: 0000000000001e90    35 FUNC    GLOBAL DEFAULT   14 pearson_array
     28: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
     29: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_2.14
-    30: 00000000000015c0  1838 FUNC    GLOBAL DEFAULT   14 spearman
-    31: 0000000000001cf0    41 FUNC    GLOBAL DEFAULT   14 spearman_array
+    30: 00000000000015c0  2195 FUNC    GLOBAL DEFAULT   14 spearman
+    31: 0000000000001e60    41 FUNC    GLOBAL DEFAULT   14 spearman_array
     32: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5
-    33: 0000000000001310   119 FUNC    GLOBAL DEFAULT   14 stdev_m
+    33: 0000000000001310   114 FUNC    GLOBAL DEFAULT   14 stdev_m
     34: 0000000000001260    29 FUNC    GLOBAL DEFAULT   14 comparator
     35: 0000000000001280    53 FUNC    GLOBAL DEFAULT   14 sum_m
     36: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND sqrt
     37: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
     38: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
```

#### readelf --wide --relocs {}

```diff
@@ -1,25 +1,25 @@
 
 Relocation section '.rela.dyn' at offset 0x670 contains 8 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000003e08  0000000000000008 R_X86_64_RELATIVE                         1250
-0000000000003e10  0000000000000008 R_X86_64_RELATIVE                         1210
-0000000000004070  0000000000000008 R_X86_64_RELATIVE                         4070
-0000000000003fd8  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
-0000000000003fe0  0000000400000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
-0000000000003fe8  0000001100000006 R_X86_64_GLOB_DAT      0000000000001260 comparator + 0
-0000000000003ff0  0000000800000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
-0000000000003ff8  0000000900000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
+0000000000003df0  0000000000000008 R_X86_64_RELATIVE                         1250
+0000000000003df8  0000000000000008 R_X86_64_RELATIVE                         1210
+0000000000004058  0000000000000008 R_X86_64_RELATIVE                         4058
+0000000000003fc0  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
+0000000000003fc8  0000000400000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
+0000000000003fd0  0000001100000006 R_X86_64_GLOB_DAT      0000000000001260 comparator + 0
+0000000000003fd8  0000000800000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+0000000000003fe0  0000000900000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
 
 Relocation section '.rela.plt' at offset 0x730 contains 11 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000004018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
-0000000000004020  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 qsort@GLIBC_2.2.5 + 0
-0000000000004028  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000001390 nanMask + 0
-0000000000004030  0000000c00000007 R_X86_64_JUMP_SLOT     0000000000001400 pearson + 0
-0000000000004038  0000001200000007 R_X86_64_JUMP_SLOT     00000000000012c0 covariance_m + 0
-0000000000004040  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 memcpy@GLIBC_2.14 + 0
-0000000000004048  0000001300000007 R_X86_64_JUMP_SLOT     00000000000015c0 spearman + 0
-0000000000004050  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
-0000000000004058  0000001000000007 R_X86_64_JUMP_SLOT     0000000000001310 stdev_m + 0
-0000000000004060  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000001280 sum_m + 0
-0000000000004068  0000000700000007 R_X86_64_JUMP_SLOT     0000000000000000 sqrt + 0
+0000000000004000  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
+0000000000004008  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 qsort@GLIBC_2.2.5 + 0
+0000000000004010  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000001390 nanMask + 0
+0000000000004018  0000000c00000007 R_X86_64_JUMP_SLOT     0000000000001420 pearson + 0
+0000000000004020  0000001200000007 R_X86_64_JUMP_SLOT     00000000000012c0 covariance_m + 0
+0000000000004028  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 memcpy@GLIBC_2.14 + 0
+0000000000004030  0000001300000007 R_X86_64_JUMP_SLOT     00000000000015c0 spearman + 0
+0000000000004038  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
+0000000000004040  0000001000000007 R_X86_64_JUMP_SLOT     0000000000001310 stdev_m + 0
+0000000000004048  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000001280 sum_m + 0
+0000000000004050  0000000700000007 R_X86_64_JUMP_SLOT     0000000000000000 sqrt + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -1,23 +1,23 @@
 
-Dynamic section at offset 0x2e18 contains 24 entries:
+Dynamic section at offset 0x2e00 contains 24 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000c (INIT)               0x1000
- 0x000000000000000d (FINI)               0x1d48
- 0x0000000000000019 (INIT_ARRAY)         0x3e08
+ 0x000000000000000d (FINI)               0x1eb4
+ 0x0000000000000019 (INIT_ARRAY)         0x3df0
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
- 0x000000000000001a (FINI_ARRAY)         0x3e10
+ 0x000000000000001a (FINI_ARRAY)         0x3df8
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x2f0
  0x0000000000000005 (STRTAB)             0x520
  0x0000000000000006 (SYMTAB)             0x340
  0x000000000000000a (STRSZ)              247 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
- 0x0000000000000003 (PLTGOT)             0x4000
+ 0x0000000000000003 (PLTGOT)             0x3fe8
  0x0000000000000002 (PLTRELSZ)           264 (bytes)
  0x0000000000000014 (PLTREL)             RELA
  0x0000000000000017 (JMPREL)             0x730
  0x0000000000000007 (RELA)               0x670
  0x0000000000000008 (RELASZ)             192 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
  0x000000006ffffffe (VERNEED)            0x640
```

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 55b563f5edb0298427cea5249818a28dbbf662a3
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 696bf528ec6378c12d4aa8f4b23e908f5f14a0ce
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -14,15 +14,15 @@
   DW_CFA_nop
 
 00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000001020..00000000000010e0
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 6 to 0000000000001026
   DW_CFA_def_cfa_offset: 24
   DW_CFA_advance_loc: 10 to 0000000000001030
-  DW_CFA_def_cfa_expression (DW_OP_breg7 (rsp): 8; DW_OP_breg16 (rip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit10; DW_OP_ge; DW_OP_lit3; DW_OP_shl; DW_OP_plus)
+  DW_CFA_def_cfa_expression (DW_OP_breg7 (rsp): 8; DW_OP_breg16 (rip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit9; DW_OP_ge; DW_OP_lit3; DW_OP_shl; DW_OP_plus)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
 00000040 0000000000000014 00000044 FDE cie=00000000 pc=00000000000010e0..00000000000010f0
   DW_CFA_nop
@@ -53,132 +53,148 @@
   DW_CFA_nop
 
 00000098 0000000000000010 0000009c FDE cie=00000000 pc=00000000000012c0..000000000000130d
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000ac 0000000000000010 000000b0 FDE cie=00000000 pc=0000000000001310..0000000000001387
+000000ac 0000000000000010 000000b0 FDE cie=00000000 pc=0000000000001310..0000000000001382
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000c0 0000000000000034 000000c4 FDE cie=00000000 pc=0000000000001390..00000000000013ff
+000000c0 0000000000000048 000000c4 FDE cie=00000000 pc=0000000000001390..0000000000001413
   DW_CFA_advance_loc: 6 to 0000000000001396
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
   DW_CFA_advance_loc: 2 to 0000000000001398
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
   DW_CFA_advance_loc: 4 to 000000000000139c
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
   DW_CFA_advance_loc: 4 to 00000000000013a0
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
   DW_CFA_advance_loc: 15 to 00000000000013af
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc1: 73 to 00000000000013f8
+  DW_CFA_advance_loc: 59 to 00000000000013ea
+  DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 00000000000013f9
+  DW_CFA_advance_loc: 1 to 00000000000013eb
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 00000000000013fa
+  DW_CFA_advance_loc: 1 to 00000000000013ec
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000013fc
+  DW_CFA_advance_loc: 2 to 00000000000013ee
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000013fe
+  DW_CFA_advance_loc: 2 to 00000000000013f0
   DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 8 to 00000000000013f8
+  DW_CFA_restore_state
+  DW_CFA_advance_loc: 20 to 000000000000140c
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 1 to 000000000000140d
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 1 to 000000000000140e
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 0000000000001410
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 0000000000001412
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
 
-000000f8 0000000000000040 000000fc FDE cie=00000000 pc=0000000000001400..00000000000015a2
-  DW_CFA_advance_loc: 6 to 0000000000001406
+0000010c 0000000000000040 00000110 FDE cie=00000000 pc=0000000000001420..00000000000015b0
+  DW_CFA_advance_loc: 6 to 0000000000001426
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 5 to 000000000000140b
+  DW_CFA_offset: r14 (r14) at cfa-16
+  DW_CFA_advance_loc: 5 to 000000000000142b
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 5 to 0000000000001410
+  DW_CFA_offset: r13 (r13) at cfa-24
+  DW_CFA_advance_loc: 5 to 0000000000001430
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000001412
+  DW_CFA_offset: r12 (r12) at cfa-32
+  DW_CFA_advance_loc: 1 to 0000000000001431
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000001413
+  DW_CFA_offset: r6 (rbp) at cfa-40
+  DW_CFA_advance_loc: 3 to 0000000000001434
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 6 to 0000000000001419
+  DW_CFA_offset: r3 (rbx) at cfa-48
+  DW_CFA_advance_loc: 4 to 0000000000001438
   DW_CFA_def_cfa_offset: 80
-  DW_CFA_advance_loc2: 356 to 000000000000157d
+  DW_CFA_advance_loc2: 340 to 000000000000158c
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000157e
+  DW_CFA_advance_loc: 1 to 000000000000158d
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001580
+  DW_CFA_advance_loc: 1 to 000000000000158e
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001582
+  DW_CFA_advance_loc: 2 to 0000000000001590
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001584
+  DW_CFA_advance_loc: 2 to 0000000000001592
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001586
+  DW_CFA_advance_loc: 2 to 0000000000001594
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 10 to 0000000000001590
+  DW_CFA_advance_loc: 12 to 00000000000015a0
   DW_CFA_restore_state
 
-0000013c 0000000000000010 00000140 FDE cie=00000000 pc=00000000000015b0..00000000000015b9
+00000150 0000000000000010 00000154 FDE cie=00000000 pc=00000000000015b0..00000000000015b9
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000150 000000000000004c 00000154 FDE cie=00000000 pc=00000000000015c0..0000000000001cee
+00000164 000000000000004c 00000168 FDE cie=00000000 pc=00000000000015c0..0000000000001e53
   DW_CFA_advance_loc: 6 to 00000000000015c6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000015c8
+  DW_CFA_advance_loc: 5 to 00000000000015cb
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 5 to 00000000000015cd
+  DW_CFA_advance_loc: 2 to 00000000000015cd
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_advance_loc: 2 to 00000000000015cf
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000015d0
+  DW_CFA_advance_loc: 4 to 00000000000015d3
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 00000000000015d1
+  DW_CFA_advance_loc: 4 to 00000000000015d7
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 00000000000015d8
-  DW_CFA_def_cfa_offset: 128
-  DW_CFA_advance_loc2: 1654 to 0000000000001c4e
+  DW_CFA_advance_loc: 14 to 00000000000015e5
+  DW_CFA_def_cfa_offset: 160
+  DW_CFA_advance_loc2: 1590 to 0000000000001c1b
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000001c4f
+  DW_CFA_advance_loc: 1 to 0000000000001c1c
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000001c50
+  DW_CFA_advance_loc: 1 to 0000000000001c1d
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001c52
+  DW_CFA_advance_loc: 2 to 0000000000001c1f
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001c54
+  DW_CFA_advance_loc: 2 to 0000000000001c21
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001c56
+  DW_CFA_advance_loc: 2 to 0000000000001c23
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001c58
+  DW_CFA_advance_loc: 2 to 0000000000001c25
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000001c59
+  DW_CFA_advance_loc: 1 to 0000000000001c26
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001a0 0000000000000010 000001a4 FDE cie=00000000 pc=0000000000001cf0..0000000000001d19
+000001b4 0000000000000010 000001b8 FDE cie=00000000 pc=0000000000001e60..0000000000001e89
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001b4 0000000000000010 000001b8 FDE cie=00000000 pc=0000000000001d20..0000000000001d46
+000001c8 0000000000000010 000001cc FDE cie=00000000 pc=0000000000001e90..0000000000001eb3
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001c8 ZERO terminator
+000001dc ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -6,17 +6,17 @@
 covariance_m
 spearman
 spearman_array
 pearson_array
 libc.so.6
 GLIBC_2.14
 GLIBC_2.2.5
- ]A\A]A^A_
-H[]A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+ []A\A]A^
+h[]A\A]A^A_
+GCC: (Ubuntu 13.2.0-4ubuntu3) 13.2.0
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.0
 __do_global_dtors_aux_fini_array_entry
 frame_dummy
 __frame_dummy_init_array_entry
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.init {}

```diff
@@ -3,13 +3,13 @@
 
 Disassembly of section .init:
 
 0000000000001000 <_init>:
 _init():
 	endbr64
 	sub    $0x8,%rsp
-	mov    0x2fd1(%rip),%rax        
+	mov    0x2fb9(%rip),%rax        
 	test   %rax,%rax
 	je     1016 <_init+0x16>
 	call   *%rax
 	add    $0x8,%rsp
 	ret
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -1,53 +1,53 @@
 
 
 
 Disassembly of section .plt:
 
 0000000000001020 <.plt>:
-	push   0x2fe2(%rip)        
-	bnd jmp *0x2fe3(%rip)        
-	nopl   (%rax)
+	push   0x2fca(%rip)        
+	jmp    *0x2fcc(%rip)        
+	nopl   0x0(%rax)
 	endbr64
 	push   $0x0
-	bnd jmp 1020 <_init+0x20>
-	nop
+	jmp    1020 <_init+0x20>
+	xchg   %ax,%ax
 	endbr64
 	push   $0x1
-	bnd jmp 1020 <_init+0x20>
-	nop
+	jmp    1020 <_init+0x20>
+	xchg   %ax,%ax
 	endbr64
 	push   $0x2
-	bnd jmp 1020 <_init+0x20>
-	nop
+	jmp    1020 <_init+0x20>
+	xchg   %ax,%ax
 	endbr64
 	push   $0x3
-	bnd jmp 1020 <_init+0x20>
-	nop
+	jmp    1020 <_init+0x20>
+	xchg   %ax,%ax
 	endbr64
 	push   $0x4
-	bnd jmp 1020 <_init+0x20>
-	nop
+	jmp    1020 <_init+0x20>
+	xchg   %ax,%ax
 	endbr64
 	push   $0x5
-	bnd jmp 1020 <_init+0x20>
-	nop
+	jmp    1020 <_init+0x20>
+	xchg   %ax,%ax
 	endbr64
 	push   $0x6
-	bnd jmp 1020 <_init+0x20>
-	nop
+	jmp    1020 <_init+0x20>
+	xchg   %ax,%ax
 	endbr64
 	push   $0x7
-	bnd jmp 1020 <_init+0x20>
-	nop
+	jmp    1020 <_init+0x20>
+	xchg   %ax,%ax
 	endbr64
 	push   $0x8
-	bnd jmp 1020 <_init+0x20>
-	nop
+	jmp    1020 <_init+0x20>
+	xchg   %ax,%ax
 	endbr64
 	push   $0x9
-	bnd jmp 1020 <_init+0x20>
-	nop
+	jmp    1020 <_init+0x20>
+	xchg   %ax,%ax
 	endbr64
 	push   $0xa
-	bnd jmp 1020 <_init+0x20>
-	nop
+	jmp    1020 <_init+0x20>
+	xchg   %ax,%ax
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.got {}

```diff
@@ -1,9 +1,9 @@
 
 
 
 Disassembly of section .plt.got:
 
 00000000000010e0 <__cxa_finalize@plt>:
 	endbr64
-	bnd jmp *0x2f0d(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2ef6(%rip)        
+	nopw   0x0(%rax,%rax,1)
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.sec {}

```diff
@@ -1,59 +1,59 @@
 
 
 
 Disassembly of section .plt.sec:
 
 00000000000010f0 <free@plt>:
 	endbr64
-	bnd jmp *0x2f1d(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2f06(%rip)        
+	nopw   0x0(%rax,%rax,1)
 
 0000000000001100 <qsort@plt>:
 	endbr64
-	bnd jmp *0x2f15(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2efe(%rip)        
+	nopw   0x0(%rax,%rax,1)
 
 0000000000001110 <nanMask@plt>:
 	endbr64
-	bnd jmp *0x2f0d(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2ef6(%rip)        
+	nopw   0x0(%rax,%rax,1)
 
 0000000000001120 <pearson@plt>:
 	endbr64
-	bnd jmp *0x2f05(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2eee(%rip)        
+	nopw   0x0(%rax,%rax,1)
 
 0000000000001130 <covariance_m@plt>:
 	endbr64
-	bnd jmp *0x2efd(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2ee6(%rip)        
+	nopw   0x0(%rax,%rax,1)
 
 0000000000001140 <memcpy@plt>:
 	endbr64
-	bnd jmp *0x2ef5(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2ede(%rip)        
+	nopw   0x0(%rax,%rax,1)
 
 0000000000001150 <spearman@plt>:
 	endbr64
-	bnd jmp *0x2eed(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2ed6(%rip)        
+	nopw   0x0(%rax,%rax,1)
 
 0000000000001160 <malloc@plt>:
 	endbr64
-	bnd jmp *0x2ee5(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2ece(%rip)        
+	nopw   0x0(%rax,%rax,1)
 
 0000000000001170 <stdev_m@plt>:
 	endbr64
-	bnd jmp *0x2edd(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2ec6(%rip)        
+	nopw   0x0(%rax,%rax,1)
 
 0000000000001180 <sum_m@plt>:
 	endbr64
-	bnd jmp *0x2ed5(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2ebe(%rip)        
+	nopw   0x0(%rax,%rax,1)
 
 0000000000001190 <sqrt@plt>:
 	endbr64
-	bnd jmp *0x2ecd(%rip)        
-	nopl   0x0(%rax,%rax,1)
+	jmp    *0x2eb6(%rip)        
+	nopw   0x0(%rax,%rax,1)
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,58 +1,58 @@
 
 
 
 Disassembly of section .text:
 
 00000000000011a0 <deregister_tm_clones>:
 deregister_tm_clones():
-	lea    0x2ed1(%rip),%rdi        
-	lea    0x2eca(%rip),%rax        
+	lea    0x2eb9(%rip),%rdi        
+	lea    0x2eb2(%rip),%rax        
 	cmp    %rdi,%rax
 	je     11c8 <deregister_tm_clones+0x28>
-	mov    0x2e1e(%rip),%rax        
+	mov    0x2e06(%rip),%rax        
 	test   %rax,%rax
 	je     11c8 <deregister_tm_clones+0x28>
 	jmp    *%rax
 	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
 
 00000000000011d0 <register_tm_clones>:
 register_tm_clones():
-	lea    0x2ea1(%rip),%rdi        
-	lea    0x2e9a(%rip),%rsi        
+	lea    0x2e89(%rip),%rdi        
+	lea    0x2e82(%rip),%rsi        
 	sub    %rdi,%rsi
 	mov    %rsi,%rax
 	shr    $0x3f,%rsi
 	sar    $0x3,%rax
 	add    %rax,%rsi
 	sar    $1,%rsi
 	je     1208 <register_tm_clones+0x38>
-	mov    0x2df5(%rip),%rax        
+	mov    0x2ddd(%rip),%rax        
 	test   %rax,%rax
 	je     1208 <register_tm_clones+0x38>
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 	ret
 	nopl   0x0(%rax)
 
 0000000000001210 <__do_global_dtors_aux>:
 __do_global_dtors_aux():
 	endbr64
-	cmpb   $0x0,0x2e5d(%rip)        
+	cmpb   $0x0,0x2e45(%rip)        
 	jne    1248 <__do_global_dtors_aux+0x38>
 	push   %rbp
-	cmpq   $0x0,0x2dd2(%rip)        
+	cmpq   $0x0,0x2dba(%rip)        
 	mov    %rsp,%rbp
 	je     1237 <__do_global_dtors_aux+0x27>
-	mov    0x2e3e(%rip),%rdi        
+	mov    0x2e26(%rip),%rdi        
 	call   10e0 <__cxa_finalize@plt>
 	call   11a0 <deregister_tm_clones>
-	movb   $0x1,0x2e35(%rip)        
+	movb   $0x1,0x2e1d(%rip)        
 	pop    %rbp
 	ret
 	nopl   (%rax)
 	ret
 	nopl   0x0(%rax)
 
 0000000000001250 <frame_dummy>:
@@ -83,15 +83,15 @@
 	pxor   %xmm0,%xmm0
 	nopl   0x0(%rax)
 	mov    (%rdx,%rax,4),%ecx
 	test   %ecx,%ecx
 	je     12a4 <sum_m+0x24>
 	addsd  (%rdi,%rax,8),%xmm0
 	add    $0x1,%rax
-	cmp    %rsi,%rax
+	cmp    %rax,%rsi
 	jne    1298 <sum_m+0x18>
 	ret
 	xchg   %ax,%ax
 	pxor   %xmm0,%xmm0
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 
@@ -122,49 +122,51 @@
 	pxor   %xmm0,%xmm0
 	ret
 	nopl   (%rax)
 
 0000000000001310 <stdev_m>:
 stdev_m():
 	endbr64
+	pxor   %xmm3,%xmm3
 	movapd %xmm0,%xmm2
+	cvtsi2sd %ecx,%xmm3
 	test   %esi,%esi
-	jle    1378 <stdev_m+0x68>
-	pxor   %xmm3,%xmm3
+	jle    1370 <stdev_m+0x60>
 	movslq %esi,%rsi
 	xor    %eax,%eax
-	movapd %xmm3,%xmm0
+	pxor   %xmm0,%xmm0
 	jmp    1339 <stdev_m+0x29>
-	nopl   0x0(%rax,%rax,1)
+	nop
 	add    $0x1,%rax
 	cmp    %rax,%rsi
-	je     135c <stdev_m+0x4c>
-	mov    (%rdx,%rax,4),%r8d
-	test   %r8d,%r8d
+	je     135a <stdev_m+0x4a>
+	mov    (%rdx,%rax,4),%ecx
+	test   %ecx,%ecx
 	je     1330 <stdev_m+0x20>
 	movsd  (%rdi,%rax,8),%xmm1
 	add    $0x1,%rax
 	subsd  %xmm2,%xmm1
 	mulsd  %xmm1,%xmm1
 	addsd  %xmm1,%xmm0
 	cmp    %rax,%rsi
 	jne    1339 <stdev_m+0x29>
+	divsd  %xmm3,%xmm0
 	pxor   %xmm1,%xmm1
-	cvtsi2sd %ecx,%xmm1
-	divsd  %xmm1,%xmm0
-	ucomisd %xmm0,%xmm3
-	ja     1382 <stdev_m+0x72>
+	ucomisd %xmm0,%xmm1
+	ja     137d <stdev_m+0x6d>
+	sqrtsd %xmm0,%xmm0
+	ret
+	nopl   (%rax)
+	pxor   %xmm0,%xmm0
+	divsd  %xmm3,%xmm0
 	sqrtsd %xmm0,%xmm0
 	ret
-	nopl   0x0(%rax,%rax,1)
-	pxor   %xmm3,%xmm3
-	movapd %xmm3,%xmm0
-	jmp    135c <stdev_m+0x4c>
 	jmp    1190 <sqrt@plt>
-	nopw   0x0(%rax,%rax,1)
+	data16 cs nopw 0x0(%rax,%rax,1)
+	nopl   (%rax)
 
 0000000000001390 <nanMask>:
 nanMask():
 	endbr64
 	push   %r13
 	push   %r12
 	mov    %rsi,%r12
@@ -172,678 +174,766 @@
 	movslq %edx,%rbp
 	push   %rbx
 	mov    %rdi,%rbx
 	lea    0x0(,%rbp,4),%rdi
 	sub    $0x8,%rsp
 	call   1160 <malloc@plt>
 	test   %ebp,%ebp
-	jle    13f4 <nanMask+0x64>
+	jle    13e6 <nanMask+0x56>
 	xor    %edx,%edx
-	jmp    13db <nanMask+0x4b>
-	nopl   0x0(%rax)
+	nopw   0x0(%rax,%rax,1)
+	movsd  (%rbx,%rdx,8),%xmm0
+	ucomisd %xmm0,%xmm0
+	jp     13f8 <nanMask+0x68>
 	movsd  (%r12,%rdx,8),%xmm0
 	xor    %ecx,%ecx
 	ucomisd %xmm0,%xmm0
 	setnp  %cl
 	mov    %ecx,(%rax,%rdx,4)
 	add    $0x1,%rdx
-	cmp    %rbp,%rdx
-	je     13f4 <nanMask+0x64>
-	movsd  (%rbx,%rdx,8),%xmm0
-	ucomisd %xmm0,%xmm0
-	jnp    13c0 <nanMask+0x30>
-	xor    %ecx,%ecx
-	mov    %ecx,(%rax,%rdx,4)
+	cmp    %rdx,%rbp
+	jne    13c0 <nanMask+0x30>
+	add    $0x8,%rsp
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	ret
+	nopl   0x0(%rax)
+	movl   $0x0,(%rax,%rdx,4)
 	add    $0x1,%rdx
-	cmp    %rbp,%rdx
-	jne    13db <nanMask+0x4b>
+	cmp    %rdx,%rbp
+	jne    13c0 <nanMask+0x30>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
-	nop
+	data16 cs nopw 0x0(%rax,%rax,1)
+	xchg   %ax,%ax
 
-0000000000001400 <pearson>:
+0000000000001420 <pearson>:
 pearson():
 	endbr64
-	push   %r15
-	mov    %rdi,%r15
 	push   %r14
-	mov    %rsi,%r14
+	mov    %rdi,%r14
 	push   %r13
+	mov    %rsi,%r13
 	push   %r12
 	push   %rbp
 	mov    %edx,%ebp
+	push   %rbx
 	sub    $0x20,%rsp
 	call   1110 <nanMask@plt>
-	mov    %rax,%r13
+	mov    %rax,%r12
 	test   %ebp,%ebp
-	jle    1590 <pearson+0x190>
+	jle    15a0 <pearson+0x180>
 	lea    -0x1(%rbp),%eax
 	cmp    $0x2,%eax
-	jbe    1598 <pearson+0x198>
+	jbe    15a7 <pearson+0x187>
 	mov    %ebp,%edx
-	mov    %r13,%rax
+	mov    %r12,%rax
 	pxor   %xmm0,%xmm0
 	shr    $0x2,%edx
 	shl    $0x4,%rdx
-	add    %r13,%rdx
-	nopl   0x0(%rax,%rax,1)
-	movdqu (%rax),%xmm4
+	add    %r12,%rdx
+	nopw   0x0(%rax,%rax,1)
+	movdqu (%rax),%xmm3
 	add    $0x10,%rax
-	paddd  %xmm4,%xmm0
+	paddd  %xmm3,%xmm0
 	cmp    %rdx,%rax
-	jne    1450 <pearson+0x50>
+	jne    1470 <pearson+0x50>
 	movdqa %xmm0,%xmm1
 	mov    %ebp,%eax
 	psrldq $0x8,%xmm1
 	and    $0xfffffffc,%eax
 	paddd  %xmm1,%xmm0
 	movdqa %xmm0,%xmm1
 	psrldq $0x4,%xmm1
 	paddd  %xmm1,%xmm0
-	movd   %xmm0,%r12d
+	movd   %xmm0,%ebx
 	test   $0x3,%bpl
-	je     14b3 <pearson+0xb3>
+	je     14d1 <pearson+0xb1>
 	movslq %eax,%rdx
 	lea    0x0(,%rdx,4),%rcx
-	add    0x0(%r13,%rdx,4),%r12d
+	add    (%r12,%rdx,4),%ebx
 	lea    0x1(%rax),%edx
 	cmp    %edx,%ebp
-	jle    14b3 <pearson+0xb3>
+	jle    14d1 <pearson+0xb1>
 	add    $0x2,%eax
-	add    0x4(%r13,%rcx,1),%r12d
+	add    0x4(%r12,%rcx,1),%ebx
 	cmp    %eax,%ebp
-	jle    14b3 <pearson+0xb3>
-	add    0x8(%r13,%rcx,1),%r12d
-	mov    %r13,%rdx
+	jle    14d1 <pearson+0xb1>
+	add    0x8(%r12,%rcx,1),%ebx
+	mov    %r12,%rdx
 	mov    %ebp,%esi
-	mov    %r15,%rdi
+	mov    %r14,%rdi
 	call   1180 <sum_m@plt>
-	pxor   %xmm5,%xmm5
-	mov    %r13,%rdx
+	pxor   %xmm4,%xmm4
+	mov    %r12,%rdx
 	mov    %ebp,%esi
-	cvtsi2sd %r12d,%xmm5
-	movapd %xmm0,%xmm3
-	mov    %r14,%rdi
-	divsd  %xmm5,%xmm3
-	movsd  %xmm5,(%rsp)
-	movsd  %xmm3,0x8(%rsp)
+	cvtsi2sd %ebx,%xmm4
+	mov    %r13,%rdi
+	divsd  %xmm4,%xmm0
+	movsd  %xmm4,(%rsp)
+	movsd  %xmm0,0x8(%rsp)
 	call   1180 <sum_m@plt>
-	movsd  0x8(%rsp),%xmm3
-	mov    %r13,%rcx
+	mov    %r12,%rcx
 	mov    %ebp,%edx
-	mov    %r14,%rsi
-	mov    %r15,%rdi
+	mov    %r13,%rsi
 	movapd %xmm0,%xmm1
+	movsd  0x8(%rsp),%xmm0
+	mov    %r14,%rdi
 	divsd  (%rsp),%xmm1
-	movapd %xmm3,%xmm0
 	movsd  %xmm1,0x18(%rsp)
 	call   1130 <covariance_m@plt>
-	movsd  0x8(%rsp),%xmm3
-	mov    %r12d,%ecx
+	mov    %ebx,%ecx
+	mov    %r12,%rdx
 	mov    %ebp,%esi
-	mov    %r13,%rdx
-	mov    %r15,%rdi
 	movapd %xmm0,%xmm2
+	movsd  0x8(%rsp),%xmm0
+	mov    %r14,%rdi
 	divsd  (%rsp),%xmm2
-	movapd %xmm3,%xmm0
 	movsd  %xmm2,0x10(%rsp)
 	call   1170 <stdev_m@plt>
 	movsd  0x18(%rsp),%xmm1
-	mov    %r12d,%ecx
-	mov    %ebp,%esi
+	mov    %ebx,%ecx
+	mov    %r12,%rdx
 	movsd  %xmm0,(%rsp)
-	mov    %r13,%rdx
-	mov    %r14,%rdi
+	mov    %ebp,%esi
+	mov    %r13,%rdi
 	movapd %xmm1,%xmm0
 	call   1170 <stdev_m@plt>
-	mov    %r13,%rdi
+	mov    %r12,%rdi
 	movsd  %xmm0,0x8(%rsp)
 	call   10f0 <free@plt>
-	movsd  (%rsp),%xmm6
-	mulsd  0x8(%rsp),%xmm6
+	movsd  (%rsp),%xmm5
+	mulsd  0x8(%rsp),%xmm5
 	movsd  0x10(%rsp),%xmm2
 	add    $0x20,%rsp
+	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
-	pop    %r15
-	divsd  %xmm6,%xmm2
+	divsd  %xmm5,%xmm2
 	movapd %xmm2,%xmm0
 	ret
-	nop
-	xor    %r12d,%r12d
-	jmp    14b3 <pearson+0xb3>
-	xor    %eax,%eax
-	xor    %r12d,%r12d
-	jmp    148b <pearson+0x8b>
-	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
+	xor    %ebx,%ebx
+	jmp    14d1 <pearson+0xb1>
+	xor    %eax,%eax
+	xor    %ebx,%ebx
+	jmp    14aa <pearson+0x8a>
 
 00000000000015b0 <free_p>:
 free_p():
 	endbr64
 	jmp    10f0 <free@plt>
 	nopl   0x0(%rax)
 
 00000000000015c0 <spearman>:
 spearman():
 	endbr64
 	push   %r15
+	movslq %edx,%r10
 	push   %r14
-	mov    %rdi,%r14
 	push   %r13
 	push   %r12
+	mov    %rdi,%r12
 	push   %rbp
+	mov    %r8d,%ebp
 	push   %rbx
-	mov    %rsi,%rbx
-	sub    $0x48,%rsp
-	mov    %ecx,0x28(%rsp)
-	movslq %edx,%rcx
-	mov    %rcx,%rbp
-	mov    %edx,0x1c(%rsp)
-	shl    $0x4,%rbp
-	mov    %rcx,0x8(%rsp)
-	mov    %rbp,%rdi
+	mov    %r10,%rbx
+	shl    $0x4,%rbx
+	mov    %rbx,%rdi
+	sub    $0x68,%rsp
+	mov    %rsi,0x18(%rsp)
+	mov    %edx,(%rsp)
+	mov    %ecx,0x38(%rsp)
+	mov    %r10,0x8(%rsp)
 	call   1160 <malloc@plt>
-	mov    %rbp,%rdi
-	mov    %rax,%r13
+	mov    %rbx,%rdi
+	mov    %rax,%r14
 	call   1160 <malloc@plt>
-	mov    0x8(%rsp),%rcx
-	mov    %rax,%r12
-	lea    0x0(,%rcx,4),%rdi
+	mov    0x8(%rsp),%r10
+	mov    %rax,%r15
+	lea    0x0(,%r10,4),%rdi
 	call   1160 <malloc@plt>
-	mov    0x8(%rsp),%rcx
-	mov    %rax,%rbp
-	lea    0x0(,%rcx,8),%rdx
-	mov    %rcx,0x20(%rsp)
-	mov    %rdx,%rdi
-	mov    %rdx,0x10(%rsp)
+	mov    0x8(%rsp),%r10
+	mov    %rax,%rbx
+	lea    0x0(,%r10,8),%r8
+	mov    %r10,0x20(%rsp)
+	mov    %r8,%rdi
+	mov    %r8,0x8(%rsp)
 	call   1160 <malloc@plt>
-	mov    0x10(%rsp),%rdi
-	mov    %rax,0x8(%rsp)
+	mov    0x8(%rsp),%rdi
+	mov    %rax,0x10(%rsp)
 	call   1160 <malloc@plt>
-	mov    0x1c(%rsp),%edi
+	test   %ebp,%ebp
 	mov    0x8(%rsp),%r8
-	mov    %rax,%r15
-	test   %edi,%edi
-	jle    1c75 <spearman+0x6b5>
-	mov    0x10(%rsp),%rdx
-	mov    %r8,%rdi
-	mov    %r14,%rsi
+	mov    0x10(%rsp),%r9
+	mov    0x20(%rsp),%r10
+	mov    %rax,%r13
+	jne    1cae <spearman+0x6ee>
+	movq   $0x0,0x8(%rsp)
+	mov    (%rsp),%eax
+	movq   $0x0,0x30(%rsp)
+	test   %eax,%eax
+	jle    1e1c <spearman+0x85c>
+	mov    %eax,%ebp
+	shl    $0x3,%rbp
+	mov    %r9,%rdi
+	mov    %r12,%rsi
+	mov    %r10,0x20(%rsp)
+	mov    %rbp,%rdx
+	mov    %r9,0x10(%rsp)
 	call   1140 <memcpy@plt>
-	mov    0x10(%rsp),%rdx
-	mov    %rbx,%rsi
-	mov    %r15,%rdi
+	mov    %rbp,%rdx
+	mov    0x18(%rsp),%rbp
+	mov    %r13,%rdi
+	mov    %rbp,%rsi
 	call   1140 <memcpy@plt>
-	mov    0x8(%rsp),%r8
-	xor    %edx,%edx
-	xor    %r10d,%r10d
-	mov    0x28(%rsp),%r9d
-	mov    0x20(%rsp),%rcx
+	mov    0x10(%rsp),%r9
+	xor    %edi,%edi
+	mov    (%rsp),%r11d
+	mov    0x20(%rsp),%r10
 	xor    %eax,%eax
-	mov    $0xffffffff,%edi
-	mov    %r8,0x10(%rsp)
-	movsd  0x95c(%rip),%xmm1        
 	mov    $0xffffffff,%esi
-	mov    %r10d,%r8d
-	mov    %r9d,0x20(%rsp)
-	mov    0x1c(%rsp),%r11d
-	mov    %edx,%r9d
-	jmp    1705 <spearman+0x145>
-	nopl   0x0(%rax,%rax,1)
-	lea    (%r11,%rdi,1),%edx
-	movsd  (%rbx,%rax,8),%xmm0
-	sub    $0x1,%edi
+	xor    %r8d,%r8d
+	mov    %r9,0x20(%rsp)
+	movsd  0x925(%rip),%xmm1        
+	mov    $0xffffffff,%ecx
+	mov    %edi,%r9d
+	jmp    172d <spearman+0x16d>
+	nopl   (%rax)
+	lea    (%r11,%rsi,1),%edx
+	movsd  0x0(%rbp,%rax,8),%xmm0
+	sub    $0x1,%esi
 	movslq %edx,%rdx
 	shl    $0x4,%rdx
-	add    %r13,%rdx
+	add    %r14,%rdx
 	ucomisd %xmm0,%xmm0
 	mov    %eax,0x8(%rdx)
 	movsd  %xmm1,(%rdx)
-	jnp    1734 <spearman+0x174>
-	lea    (%r11,%rsi,1),%edx
+	jnp    175c <spearman+0x19c>
+	lea    (%r11,%rcx,1),%edx
 	add    $0x1,%rax
-	sub    $0x1,%esi
+	sub    $0x1,%ecx
 	movslq %edx,%rdx
 	shl    $0x4,%rdx
-	add    %r12,%rdx
-	mov    %r10d,0x8(%rdx)
+	add    %r15,%rdx
+	mov    %edi,0x8(%rdx)
 	movsd  %xmm1,(%rdx)
-	cmp    %rax,%rcx
-	je     1753 <spearman+0x193>
-	movsd  (%r14,%rax,8),%xmm0
-	mov    %eax,%r10d
+	cmp    %rax,%r10
+	je     177a <spearman+0x1ba>
+	movsd  (%r12,%rax,8),%xmm0
+	mov    %eax,%edi
 	ucomisd %xmm0,%xmm0
-	jp     16c0 <spearman+0x100>
+	jp     16e8 <spearman+0x128>
 	movslq %r8d,%rdx
 	add    $0x1,%r8d
 	shl    $0x4,%rdx
-	add    %r13,%rdx
+	add    %r14,%rdx
 	movsd  %xmm0,(%rdx)
-	movsd  (%rbx,%rax,8),%xmm0
+	movsd  0x0(%rbp,%rax,8),%xmm0
 	mov    %eax,0x8(%rdx)
 	ucomisd %xmm0,%xmm0
-	jp     16e3 <spearman+0x123>
+	jp     170c <spearman+0x14c>
 	movslq %r9d,%rdx
 	add    $0x1,%rax
 	add    $0x1,%r9d
 	shl    $0x4,%rdx
-	add    %r12,%rdx
-	mov    %r10d,0x8(%rdx)
+	add    %r15,%rdx
+	mov    %edi,0x8(%rdx)
 	movsd  %xmm0,(%rdx)
-	cmp    %rax,%rcx
-	jne    1705 <spearman+0x145>
+	cmp    %rax,%r10
+	jne    172d <spearman+0x16d>
+	movslq %r9d,%rbp
+	mov    0x20(%rsp),%r9
 	movslq %r8d,%rsi
-	mov    %r9d,0x8(%rsp)
-	mov    0x10(%rsp),%r8
-	mov    %r13,%rdi
-	mov    0x20(%rsp),%r9d
-	mov    0x2879(%rip),%rcx        
+	cmp    %ebp,%r8d
+	mov    %rbp,%rax
+	mov    %ebp,0x10(%rsp)
+	cmovle %r8d,%eax
+	mov    %eax,%r11d
+	cltq
+	shl    $0x2,%rax
+	mov    %rax,0x20(%rsp)
+	mov    0x2828(%rip),%rcx        
 	mov    $0x10,%edx
-	mov    %esi,0x10(%rsp)
-	mov    %r8,0x30(%rsp)
-	mov    %r9d,0x38(%rsp)
+	mov    %r14,%rdi
+	mov    %r9,0x50(%rsp)
+	mov    %r8d,0x48(%rsp)
+	mov    %r10,0x40(%rsp)
+	mov    %r11d,0x5c(%rsp)
 	call   1100 <qsort@plt>
-	movslq 0x8(%rsp),%rsi
+	mov    %rbp,%rsi
 	mov    $0x10,%edx
-	mov    %r12,%rdi
-	mov    0x284d(%rip),%rcx        
+	mov    %r15,%rdi
+	mov    0x27f5(%rip),%rcx        
 	call   1100 <qsort@plt>
-	mov    0x10(%rsp),%eax
-	mov    0x8(%rsp),%ecx
-	cmp    %ecx,%eax
-	cmovle %eax,%ecx
-	movslq %ecx,%rdi
-	mov    %ecx,0x3c(%rsp)
-	shl    $0x2,%rdi
-	mov    %rdi,0x28(%rsp)
+	mov    0x20(%rsp),%rbp
+	mov    %rbp,%rdi
 	call   1160 <malloc@plt>
-	mov    0x28(%rsp),%rdi
+	mov    %rbp,%rdi
 	mov    %rax,0x20(%rsp)
 	call   1160 <malloc@plt>
-	mov    0x38(%rsp),%r9d
-	mov    0x30(%rsp),%r8
+	mov    0x38(%rsp),%edi
+	mov    0x40(%rsp),%r10
+	mov    0x48(%rsp),%r8d
+	mov    0x50(%rsp),%r9
 	mov    %rax,0x28(%rsp)
-	test   %r9d,%r9d
-	jne    1930 <spearman+0x370>
-	mov    0x3c(%rsp),%ecx
-	mov    0x8(%rsp),%esi
-	test   %ecx,%ecx
+	test   %edi,%edi
+	jne    1c40 <spearman+0x680>
+	mov    0x5c(%rsp),%r11d
+	test   %r11d,%r11d
 	setg   %al
-	test   %esi,%esi
-	mov    0x10(%rsp),%esi
-	setg   %dl
-	and    %eax,%edx
-	mov    %edx,%r10d
-	test   %esi,%esi
-	jle    1ce7 <spearman+0x727>
+	test   %r8d,%r8d
+	jle    1c26 <spearman+0x666>
 	test   %al,%al
-	je     1ce7 <spearman+0x727>
-	lea    -0x1(%rsi),%eax
+	je     1c26 <spearman+0x666>
+	lea    -0x1(%r8),%eax
 	mov    0x20(%rsp),%rdi
+	mov    0x18(%rsp),%rsi
 	xor    %edx,%edx
 	cltq
-	mov    %rax,%rsi
-	shl    $0x4,%rsi
-	movslq 0x8(%r13,%rsi,1),%r11
-	movsd  (%rbx,%r11,8),%xmm0
-	mov    %r11,%rsi
+	nopl   0x0(%rax,%rax,1)
+	mov    %rax,%rcx
+	shl    $0x4,%rcx
+	movslq 0x8(%r14,%rcx,1),%rbp
+	movsd  (%rsi,%rbp,8),%xmm0
+	mov    %rbp,%rcx
 	ucomisd %xmm0,%xmm0
-	jnp    1845 <spearman+0x285>
-	movslq %edx,%r11
+	jnp    1873 <spearman+0x2b3>
+	movslq %edx,%rbp
 	add    $0x1,%edx
-	mov    %esi,(%rdi,%r11,4)
+	mov    %ecx,(%rdi,%rbp,4)
 	test   %eax,%eax
-	setg   %r11b
-	cmp    %ecx,%edx
-	setl   %sil
+	setg   %bpl
+	cmp    %r11d,%edx
+	setl   %cl
 	sub    $0x1,%rax
-	test   %sil,%r11b
-	jne    1820 <spearman+0x260>
-	mov    0x8(%rsp),%eax
+	test   %cl,%bpl
+	jne    1850 <spearman+0x290>
+	mov    0x10(%rsp),%ecx
+	test   %ecx,%ecx
+	jle    1e3c <spearman+0x87c>
+	mov    0x10(%rsp),%eax
+	mov    0x28(%rsp),%rdi
+	mov    0x38(%rsp),%ecx
 	sub    $0x1,%eax
 	cltq
-	test   %r10b,%r10b
-	je     1cd4 <spearman+0x714>
-	mov    0x28(%rsp),%r10
-	nopl   0x0(%rax)
+	cs nopw 0x0(%rax,%rax,1)
 	mov    %rax,%rsi
 	shl    $0x4,%rsi
-	movslq 0x8(%r12,%rsi,1),%rdi
-	movsd  (%r14,%rdi,8),%xmm0
-	mov    %rdi,%rsi
+	movslq 0x8(%r15,%rsi,1),%rbp
+	movsd  (%r12,%rbp,8),%xmm0
+	mov    %rbp,%rsi
 	ucomisd %xmm0,%xmm0
-	jnp    189e <spearman+0x2de>
-	movslq %r9d,%rdi
-	add    $0x1,%r9d
-	mov    %esi,(%r10,%rdi,4)
+	jnp    18d4 <spearman+0x314>
+	movslq %ecx,%rbp
+	add    $0x1,%ecx
+	mov    %esi,(%rdi,%rbp,4)
 	test   %eax,%eax
-	setg   %dil
-	cmp    %ecx,%r9d
+	setg   %bpl
+	cmp    %r11d,%ecx
 	setl   %sil
 	sub    $0x1,%rax
-	test   %sil,%dil
-	jne    1878 <spearman+0x2b8>
-	test   %r9d,%r9d
-	je     1cd4 <spearman+0x714>
-	movslq %r9d,%rax
-	lea    0x1(%r9),%edi
-	mov    0x28(%rsp),%r9
-	nopl   0x0(%rax)
+	test   %sil,%bpl
+	jne    18b0 <spearman+0x2f0>
+	test   %ecx,%ecx
+	jle    1e3c <spearman+0x87c>
+	mov    0x28(%rsp),%r11
+	movslq %ecx,%rax
+	lea    0x1(%rcx),%edi
+	nopl   (%rax)
 	mov    %edi,%esi
 	pxor   %xmm0,%xmm0
-	movslq -0x4(%r9,%rax,4),%rcx
+	movslq -0x4(%r11,%rax,4),%rcx
 	sub    %eax,%esi
 	sub    $0x1,%rax
 	cvtsi2sd %esi,%xmm0
-	movsd  %xmm0,(%r8,%rcx,8)
+	movsd  %xmm0,(%r9,%rcx,8)
 	test   %eax,%eax
-	jne    18d0 <spearman+0x310>
-	mov    %edi,%r10d
+	jg     1900 <spearman+0x340>
+	mov    %edi,0x38(%rsp)
 	test   %edx,%edx
-	je     1cc7 <spearman+0x707>
+	jle    1e49 <spearman+0x889>
 	mov    0x20(%rsp),%rdi
 	movslq %edx,%rax
 	lea    0x1(%rdx),%esi
-	nopl   (%rax)
+	cs nopw 0x0(%rax,%rax,1)
 	mov    %esi,%ecx
 	pxor   %xmm0,%xmm0
 	movslq -0x4(%rdi,%rax,4),%rdx
 	sub    %eax,%ecx
 	sub    $0x1,%rax
 	cvtsi2sd %ecx,%xmm0
-	movsd  %xmm0,(%r15,%rdx,8)
+	movsd  %xmm0,0x0(%r13,%rdx,8)
 	test   %eax,%eax
-	jne    1908 <spearman+0x348>
-	mov    %esi,0x38(%rsp)
-	jmp    193e <spearman+0x37e>
-	nopl   (%rax)
-	movl   $0x1,0x38(%rsp)
-	mov    $0x1,%r10d
-	mov    0x1c(%rsp),%eax
-	lea    -0x1(%rax),%ecx
+	jg     1940 <spearman+0x380>
+	mov    (%rsp),%edx
+	mov    %esi,%ebp
 	xor    %eax,%eax
-	jmp    196f <spearman+0x3af>
-	nopl   0x0(%rax)
-	movsd  (%r8,%rax,8),%xmm0
-	xor    %edx,%edx
-	ucomisd %xmm0,%xmm0
-	setp   %dl
-	mov    %edx,0x0(%rbp,%rax,4)
-	lea    0x1(%rax),%rdx
-	cmp    %rax,%rcx
-	je     198c <spearman+0x3cc>
-	mov    %rdx,%rax
-	movsd  (%r15,%rax,8),%xmm0
-	ucomisd %xmm0,%xmm0
-	jnp    1950 <spearman+0x390>
-	movl   $0x1,0x0(%rbp,%rax,4)
-	lea    0x1(%rax),%rdx
-	cmp    %rax,%rcx
-	jne    196c <spearman+0x3ac>
-	mov    0x10(%rsp),%edx
-	movsd  0x670(%rip),%xmm2        
-	xor    %r11d,%r11d
 	test   %edx,%edx
-	je     1ac1 <spearman+0x501>
-	mov    %r12,0x30(%rsp)
-	mov    0x10(%rsp),%r12d
-	mov    %r15,0x10(%rsp)
-	mov    %r10d,%r15d
-	jmp    19cd <spearman+0x40d>
-	nopw   0x0(%rax,%rax,1)
+	jg     1c60 <spearman+0x6a0>
+	nop
+	movsd  0x690(%rip),%xmm2        
+	xor    %r11d,%r11d
+	test   %r8d,%r8d
+	jle    1a8c <spearman+0x4cc>
+	mov    %r15,0x48(%rsp)
+	mov    0x38(%rsp),%r15d
+	mov    %ebp,0x40(%rsp)
+	jmp    19a5 <spearman+0x3e5>
+	nopl   0x0(%rax)
 	add    $0x1,%r11d
-	cmp    %r12d,%r11d
-	jge    1ab7 <spearman+0x4f7>
+	cmp    %r8d,%r11d
+	jge    1a83 <spearman+0x4c3>
 	movslq %r11d,%rax
 	mov    %rax,%rdx
 	shl    $0x4,%rdx
-	add    %r13,%rdx
+	add    %r14,%rdx
 	movslq 0x8(%rdx),%rcx
-	mov    0x0(%rbp,%rcx,4),%edi
-	test   %edi,%edi
-	jne    19c0 <spearman+0x400>
-	movsd  (%r14,%rcx,8),%xmm0
-	mov    %r12d,%ecx
-	sub    %r11d,%ecx
-	test   %ecx,%ecx
-	jle    1c59 <spearman+0x699>
-	lea    -0x1(%rcx),%r10d
-	xor    %r9d,%r9d
+	mov    (%rbx,%rcx,4),%r10d
+	test   %r10d,%r10d
+	jne    1998 <spearman+0x3d8>
+	mov    %r8d,%ebp
+	movsd  (%r12,%rcx,8),%xmm0
+	xor    %edi,%edi
 	xor    %esi,%esi
-	add    %rax,%r10
+	sub    %r11d,%ebp
+	movslq %ebp,%rbp
+	add    %rax,%rbp
 	mov    %rdx,%rax
-	shl    $0x4,%r10
-	add    %r13,%r10
-	jmp    1a25 <spearman+0x465>
-	nopw   0x0(%rax,%rax,1)
-	movslq 0x18(%rax),%rcx
-	add    $0x10,%rax
-	mov    0x0(%rbp,%rcx,4),%r9d
+	shl    $0x4,%rbp
+	add    %r14,%rbp
+	jmp    19ef <spearman+0x42f>
+	nopl   0x0(%rax)
+	movslq 0x8(%rax),%rcx
+	mov    (%rbx,%rcx,4),%edi
 	movslq 0x8(%rax),%rcx
-	test   %r9d,%r9d
-	jne    1a3b <spearman+0x47b>
-	ucomisd (%r14,%rcx,8),%xmm0
-	jp     1a40 <spearman+0x480>
-	jne    1a40 <spearman+0x480>
+	test   %edi,%edi
+	jne    1a04 <spearman+0x444>
+	ucomisd (%r12,%rcx,8),%xmm0
+	jp     1a0d <spearman+0x44d>
+	jne    1a0d <spearman+0x44d>
 	add    $0x1,%esi
-	cmp    %rax,%r10
-	jne    1a18 <spearman+0x458>
-	lea    -0x1(%rsi),%r9d
+	add    $0x10,%rax
+	cmp    %rbp,%rax
+	jne    19e8 <spearman+0x428>
+	lea    -0x1(%rsi),%eax
 	pxor   %xmm0,%xmm0
 	pxor   %xmm1,%xmm1
-	cvtsi2sd %r9d,%xmm0
+	cvtsi2sd %eax,%xmm0
 	cvtsi2sd %r15d,%xmm1
-	add    %esi,%r15d
 	mulsd  %xmm2,%xmm0
 	addsd  %xmm1,%xmm0
 	test   %esi,%esi
-	je     1aa7 <spearman+0x4e7>
+	jle    1dfb <spearman+0x83b>
 	mov    %r11d,%eax
 	xor    %ecx,%ecx
-	jmp    1a98 <spearman+0x4d8>
-	nopl   0x0(%rax)
-	movslq %eax,%rcx
-	add    $0x1,%edi
+	jmp    1a60 <spearman+0x4a0>
+	nopl   0x0(%rax,%rax,1)
+	movslq 0x8(%rdx),%rdi
+	add    $0x1,%ecx
 	add    $0x10,%rdx
 	add    $0x1,%eax
-	shl    $0x4,%rcx
-	movslq 0x8(%r13,%rcx,1),%rcx
-	movsd  %xmm0,(%r8,%rcx,8)
-	cmp    %esi,%edi
-	jge    1aa7 <spearman+0x4e7>
-	movslq 0x8(%rdx),%rcx
-	mov    0x0(%rbp,%rcx,4),%ecx
-	test   %ecx,%ecx
-	je     1a70 <spearman+0x4b0>
+	movsd  %xmm0,(%r9,%rdi,8)
+	cmp    %esi,%ecx
+	jge    1a73 <spearman+0x4b3>
+	movslq 0x8(%rdx),%rdi
+	mov    (%rbx,%rdi,4),%r10d
+	mov    %eax,%r11d
+	test   %r10d,%r10d
+	je     1a40 <spearman+0x480>
 	add    $0x10,%rdx
 	add    $0x1,%eax
-	cmp    %edi,%esi
-	jg     1a90 <spearman+0x4d0>
-	add    %r9d,%r11d
+	cmp    %ecx,%esi
+	jg     1a58 <spearman+0x498>
+	add    %esi,%r15d
 	add    $0x1,%r11d
-	cmp    %r12d,%r11d
-	jl     19cd <spearman+0x40d>
-	mov    0x30(%rsp),%r12
-	mov    0x10(%rsp),%r15
-	mov    0x8(%rsp),%eax
-	movsd  0x53b(%rip),%xmm2        
-	xor    %r11d,%r11d
+	cmp    %r8d,%r11d
+	jl     19a5 <spearman+0x3e5>
+	mov    0x40(%rsp),%ebp
+	mov    0x48(%rsp),%r15
+	mov    0x10(%rsp),%eax
+	movsd  0x570(%rip),%xmm2        
+	xor    %r10d,%r10d
 	test   %eax,%eax
-	je     1bec <spearman+0x62c>
-	mov    %r13,0x10(%rsp)
-	mov    0x38(%rsp),%r14d
-	mov    0x8(%rsp),%r13d
-	jmp    1afd <spearman+0x53d>
-	nopl   0x0(%rax)
-	add    $0x1,%r11d
-	cmp    %r13d,%r11d
-	jge    1be7 <spearman+0x627>
-	movslq %r11d,%rax
+	jle    1ba8 <spearman+0x5e8>
+	mov    %r14,0x38(%rsp)
+	mov    0x18(%rsp),%r12
+	mov    0x10(%rsp),%r14d
+	jmp    1ac5 <spearman+0x505>
+	nopl   0x0(%rax)
+	add    $0x1,%r10d
+	cmp    %r14d,%r10d
+	jge    1ba3 <spearman+0x5e3>
+	movslq %r10d,%rax
 	mov    %rax,%rdx
 	shl    $0x4,%rdx
-	add    %r12,%rdx
+	add    %r15,%rdx
 	movslq 0x8(%rdx),%rcx
-	mov    0x0(%rbp,%rcx,4),%edi
-	test   %edi,%edi
-	jne    1af0 <spearman+0x530>
-	movsd  (%rbx,%rcx,8),%xmm0
-	mov    %r13d,%ecx
-	sub    %r11d,%ecx
-	test   %ecx,%ecx
-	jle    1c67 <spearman+0x6a7>
-	lea    -0x1(%rcx),%r10d
-	xor    %r9d,%r9d
+	mov    (%rbx,%rcx,4),%r8d
+	test   %r8d,%r8d
+	jne    1ab8 <spearman+0x4f8>
+	mov    %r14d,%r11d
+	movsd  (%r12,%rcx,8),%xmm0
+	xor    %edi,%edi
 	xor    %esi,%esi
-	add    %rax,%r10
+	sub    %r10d,%r11d
+	movslq %r11d,%r11
+	add    %rax,%r11
 	mov    %rdx,%rax
-	shl    $0x4,%r10
-	add    %r12,%r10
-	jmp    1b55 <spearman+0x595>
+	shl    $0x4,%r11
+	add    %r15,%r11
+	jmp    1b0f <spearman+0x54f>
 	nopl   0x0(%rax)
-	movslq 0x18(%rax),%rcx
-	add    $0x10,%rax
-	mov    0x0(%rbp,%rcx,4),%r9d
 	movslq 0x8(%rax),%rcx
-	test   %r9d,%r9d
-	jne    1b6a <spearman+0x5aa>
-	ucomisd (%rbx,%rcx,8),%xmm0
-	jp     1b6f <spearman+0x5af>
-	jne    1b6f <spearman+0x5af>
+	mov    (%rbx,%rcx,4),%edi
+	movslq 0x8(%rax),%rcx
+	test   %edi,%edi
+	jne    1b24 <spearman+0x564>
+	ucomisd (%r12,%rcx,8),%xmm0
+	jp     1b2d <spearman+0x56d>
+	jne    1b2d <spearman+0x56d>
 	add    $0x1,%esi
-	cmp    %r10,%rax
-	jne    1b48 <spearman+0x588>
-	lea    -0x1(%rsi),%r9d
+	add    $0x10,%rax
+	cmp    %r11,%rax
+	jne    1b08 <spearman+0x548>
+	lea    -0x1(%rsi),%eax
 	pxor   %xmm0,%xmm0
 	pxor   %xmm1,%xmm1
-	cvtsi2sd %r9d,%xmm0
-	cvtsi2sd %r14d,%xmm1
-	add    %esi,%r14d
+	cvtsi2sd %eax,%xmm0
+	cvtsi2sd %ebp,%xmm1
 	mulsd  %xmm2,%xmm0
 	addsd  %xmm1,%xmm0
 	test   %esi,%esi
-	je     1bd7 <spearman+0x617>
-	mov    %r11d,%eax
+	jle    1e07 <spearman+0x847>
+	mov    %r10d,%eax
 	xor    %ecx,%ecx
-	jmp    1bc8 <spearman+0x608>
-	nopl   0x0(%rax,%rax,1)
-	movslq %eax,%rcx
-	add    $0x1,%edi
+	jmp    1b81 <spearman+0x5c1>
+	nopw   0x0(%rax,%rax,1)
+	movslq 0x8(%rdx),%rdi
+	add    $0x1,%ecx
 	add    $0x10,%rdx
 	add    $0x1,%eax
-	shl    $0x4,%rcx
-	movslq 0x8(%r12,%rcx,1),%rcx
-	movsd  %xmm0,(%r15,%rcx,8)
-	cmp    %esi,%edi
-	jge    1bd7 <spearman+0x617>
-	movslq 0x8(%rdx),%rcx
-	mov    0x0(%rbp,%rcx,4),%ecx
-	test   %ecx,%ecx
-	je     1ba0 <spearman+0x5e0>
+	movsd  %xmm0,0x0(%r13,%rdi,8)
+	cmp    %esi,%ecx
+	jge    1b94 <spearman+0x5d4>
+	movslq 0x8(%rdx),%rdi
+	mov    (%rbx,%rdi,4),%r8d
+	mov    %eax,%r10d
+	test   %r8d,%r8d
+	je     1b60 <spearman+0x5a0>
 	add    $0x10,%rdx
 	add    $0x1,%eax
-	cmp    %edi,%esi
-	jg     1bc0 <spearman+0x600>
-	add    %r9d,%r11d
-	add    $0x1,%r11d
-	cmp    %r13d,%r11d
-	jl     1afd <spearman+0x53d>
-	mov    0x10(%rsp),%r13
-	mov    0x1c(%rsp),%edx
-	mov    %r15,%rsi
-	mov    %r8,%rdi
-	mov    %r8,0x10(%rsp)
+	cmp    %ecx,%esi
+	jg     1b79 <spearman+0x5b9>
+	add    %esi,%ebp
+	add    $0x1,%r10d
+	cmp    %r14d,%r10d
+	jl     1ac5 <spearman+0x505>
+	mov    0x38(%rsp),%r14
+	mov    (%rsp),%edx
+	mov    %r13,%rsi
+	mov    %r9,%rdi
+	mov    %r9,0x10(%rsp)
 	call   1120 <pearson@plt>
-	mov    %r13,%rdi
-	movsd  %xmm0,0x8(%rsp)
+	mov    %r14,%rdi
+	movsd  %xmm0,(%rsp)
 	call   10f0 <free@plt>
-	mov    %r12,%rdi
+	mov    %r15,%rdi
 	call   10f0 <free@plt>
 	mov    0x10(%rsp),%rdi
 	call   10f0 <free@plt>
-	mov    %r15,%rdi
+	mov    %r13,%rdi
 	call   10f0 <free@plt>
-	mov    %rbp,%rdi
+	mov    %rbx,%rdi
 	call   10f0 <free@plt>
 	mov    0x20(%rsp),%rdi
 	call   10f0 <free@plt>
 	mov    0x28(%rsp),%rdi
 	call   10f0 <free@plt>
-	movsd  0x8(%rsp),%xmm0
-	add    $0x48,%rsp
+	mov    0x30(%rsp),%rdi
+	call   10f0 <free@plt>
+	mov    0x8(%rsp),%rdi
+	call   10f0 <free@plt>
+	movsd  (%rsp),%xmm0
+	add    $0x68,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
-	mov    $0xffffffff,%r9d
-	add    %r9d,%r11d
-	jmp    1aaa <spearman+0x4ea>
-	mov    $0xffffffff,%r9d
-	add    %r9d,%r11d
-	jmp    1bda <spearman+0x61a>
-	mov    $0x10,%edx
-	xor    %esi,%esi
-	mov    %r13,%rdi
-	mov    %r8,0x8(%rsp)
-	mov    0x235d(%rip),%r14        
-	mov    %r14,%rcx
-	call   1100 <qsort@plt>
-	mov    %r14,%rcx
-	mov    $0x10,%edx
-	xor    %esi,%esi
-	mov    %r12,%rdi
-	call   1100 <qsort@plt>
-	xor    %edi,%edi
-	call   1160 <malloc@plt>
-	xor    %edi,%edi
-	mov    %rax,0x20(%rsp)
-	call   1160 <malloc@plt>
-	mov    0x8(%rsp),%r8
-	mov    %rax,0x28(%rsp)
-	jmp    1bec <spearman+0x62c>
+	mov    0x10(%rsp),%esi
+	test   %esi,%esi
+	jle    1c40 <spearman+0x680>
+	xor    %edx,%edx
+	test   %al,%al
+	jne    1894 <spearman+0x2d4>
+	nopl   0x0(%rax,%rax,1)
 	movl   $0x1,0x38(%rsp)
-	jmp    193e <spearman+0x37e>
+	mov    $0x1,%ebp
+	mov    (%rsp),%edx
+	xor    %eax,%eax
 	test   %edx,%edx
-	je     1930 <spearman+0x370>
-	mov    $0x1,%r10d
-	jmp    18fa <spearman+0x33a>
+	jle    1970 <spearman+0x3b0>
+	nopw   0x0(%rax,%rax,1)
+	movsd  0x0(%r13,%rax,8),%xmm0
+	ucomisd %xmm0,%xmm0
+	jp     1c99 <spearman+0x6d9>
+	movsd  (%r9,%rax,8),%xmm0
+	xor    %edx,%edx
+	ucomisd %xmm0,%xmm0
+	setp   %dl
+	mov    %edx,(%rbx,%rax,4)
+	add    $0x1,%rax
+	cmp    %rax,%r10
+	je     1970 <spearman+0x3b0>
+	movsd  0x0(%r13,%rax,8),%xmm0
+	ucomisd %xmm0,%xmm0
+	jnp    1c6d <spearman+0x6ad>
+	movl   $0x1,(%rbx,%rax,4)
+	add    $0x1,%rax
+	cmp    %rax,%r10
+	jne    1c60 <spearman+0x6a0>
+	jmp    1970 <spearman+0x3b0>
+	mov    %r8,%rdi
+	mov    %r9,0x20(%rsp)
+	mov    %r10,0x10(%rsp)
+	call   1160 <malloc@plt>
+	mov    0x8(%rsp),%r8
+	mov    %rax,0x30(%rsp)
+	mov    %r8,%rdi
+	mov    %r8,0x28(%rsp)
+	call   1160 <malloc@plt>
+	mov    (%rsp),%esi
+	mov    0x10(%rsp),%r10
+	mov    %rax,0x8(%rsp)
+	mov    0x20(%rsp),%r9
+	test   %esi,%esi
+	jle    1e12 <spearman+0x852>
+	mov    %esi,%ebp
+	mov    %r12,%rsi
+	mov    0x30(%rsp),%r12
+	mov    %r9,0x40(%rsp)
+	lea    0x0(,%rbp,8),%rdx
+	mov    %r10,0x20(%rsp)
+	mov    %r12,%rdi
+	mov    %rdx,0x10(%rsp)
+	call   1140 <memcpy@plt>
+	mov    0x10(%rsp),%rdx
+	mov    0x18(%rsp),%rsi
+	mov    0x8(%rsp),%rdi
+	call   1140 <memcpy@plt>
+	mov    0x20(%rsp),%r10
+	xor    %eax,%eax
 	xor    %edx,%edx
-	jmp    185a <spearman+0x29a>
+	mov    0x28(%rsp),%r8
+	mov    0x40(%rsp),%r9
+	mov    %r12,%rcx
+	nopl   0x0(%rax)
+	movsd  (%rcx,%rax,1),%xmm0
+	ucomisd %xmm0,%xmm0
+	jp     1d90 <spearman+0x7d0>
+	mov    0x8(%rsp),%rsi
+	movsd  (%rsi,%rax,1),%xmm0
+	xor    %esi,%esi
+	ucomisd %xmm0,%xmm0
+	setp   %sil
+	add    $0x8,%rax
+	add    %esi,%edx
+	cmp    %rax,%r8
+	jne    1d48 <spearman+0x788>
+	mov    (%rsp),%eax
+	sub    %edx,%eax
+	cmp    $0x9,%eax
+	jle    1da6 <spearman+0x7e6>
+	mov    0x8(%rsp),%rax
+	mov    0x30(%rsp),%r12
+	mov    %rax,0x18(%rsp)
+	jmp    1685 <spearman+0xc5>
+	add    $0x8,%rax
+	add    $0x1,%edx
+	cmp    %rax,%r8
+	jne    1d48 <spearman+0x788>
+	mov    (%rsp),%eax
+	sub    %edx,%eax
+	cmp    $0x9,%eax
+	jg     1d7c <spearman+0x7bc>
+	mov    0x8(%rsp),%rdx
+	mov    0x30(%rsp),%rcx
+	xor    %eax,%eax
+	nopw   0x0(%rax,%rax,1)
+	movsd  (%rdx,%rax,1),%xmm0
+	ucomisd %xmm0,%xmm0
+	jnp    1dcb <spearman+0x80b>
+	movq   $0x0,(%rdx,%rax,1)
+	movsd  (%rcx,%rax,1),%xmm0
+	ucomisd %xmm0,%xmm0
+	jnp    1dde <spearman+0x81e>
+	movq   $0x0,(%rcx,%rax,1)
+	add    $0x8,%rax
+	cmp    %rax,%r8
+	jne    1db8 <spearman+0x7f8>
+	mov    0x8(%rsp),%rax
+	mov    0x30(%rsp),%r12
+	mov    %rax,0x18(%rsp)
+	jmp    1685 <spearman+0xc5>
+	sub    $0x1,%r11d
+	add    %esi,%r15d
+	jmp    1a76 <spearman+0x4b6>
+	sub    $0x1,%r10d
+	add    %esi,%ebp
+	jmp    1b96 <spearman+0x5d6>
+	mov    %rax,0x18(%rsp)
+	mov    0x30(%rsp),%r12
+	movq   $0x0,0x20(%rsp)
+	xor    %r11d,%r11d
+	xor    %ebp,%ebp
+	xor    %esi,%esi
+	movl   $0x0,0x10(%rsp)
+	xor    %r8d,%r8d
+	jmp    17a1 <spearman+0x1e1>
+	movl   $0x1,0x38(%rsp)
+	jmp    1923 <spearman+0x363>
+	mov    $0x1,%ebp
+	jmp    1c4d <spearman+0x68d>
+	data16 cs nopw 0x0(%rax,%rax,1)
 	xchg   %ax,%ax
 
-0000000000001cf0 <spearman_array>:
+0000000000001e60 <spearman_array>:
 spearman_array():
 	endbr64
-	mov    %edx,%r9d
+	mov    %edx,%eax
 	mov    %ecx,%edx
 	mov    %r8d,%ecx
-	imul   %edx,%r9d
+	mov    %r9d,%r8d
+	imul   %edx,%eax
 	imul   %edx,%esi
-	movslq %r9d,%r9
-	lea    (%rdi,%r9,8),%r8
+	cltq
+	lea    (%rdi,%rax,8),%rax
 	movslq %esi,%rsi
 	lea    (%rdi,%rsi,8),%rdi
-	mov    %r8,%rsi
+	mov    %rax,%rsi
 	jmp    1150 <spearman@plt>
 	nopl   0x0(%rax)
 
-0000000000001d20 <pearson_array>:
+0000000000001e90 <pearson_array>:
 pearson_array():
 	endbr64
-	mov    %edx,%r8d
+	mov    %edx,%eax
 	imul   %ecx,%esi
 	mov    %ecx,%edx
-	imul   %ecx,%r8d
+	imul   %ecx,%eax
 	movslq %esi,%rsi
-	movslq %r8d,%r8
-	lea    (%rdi,%r8,8),%r8
+	cltq
+	lea    (%rdi,%rax,8),%rax
 	lea    (%rdi,%rsi,8),%rdi
-	mov    %r8,%rsi
+	mov    %rax,%rsi
 	jmp    1120 <pearson@plt>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,11 +1,11 @@
 
 
 
 Disassembly of section .fini:
 
-0000000000001d48 <_fini>:
+0000000000001eb4 <_fini>:
 _fini():
 	endbr64
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,11 +1,11 @@
 
 Hex dump of section '.eh_frame_hdr':
   0x00002010 011b033b 74000000 0d000000 10f0ffff ...;t...........
   0x00002020 90000000 d0f0ffff b8000000 e0f0ffff ................
   0x00002030 d0000000 50f2ffff e8000000 70f2ffff ....P.......p...
   0x00002040 fc000000 b0f2ffff 10010000 00f3ffff ................
-  0x00002050 24010000 80f3ffff 38010000 f0f3ffff $.......8.......
-  0x00002060 70010000 a0f5ffff b4010000 b0f5ffff p...............
-  0x00002070 c8010000 e0fcffff 18020000 10fdffff ................
-  0x00002080 2c020000                            ,...
+  0x00002050 24010000 80f3ffff 38010000 10f4ffff $.......8.......
+  0x00002060 84010000 a0f5ffff c8010000 b0f5ffff ................
+  0x00002070 dc010000 50feffff 2c020000 80feffff ....P...,.......
+  0x00002080 40020000                            @...
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,32 +1,33 @@
 
 Hex dump of section '.eh_frame':
   0x00002088 14000000 00000000 017a5200 01781001 .........zR..x..
   0x00002098 1b0c0708 90010000 24000000 1c000000 ........$.......
   0x000020a8 78efffff c0000000 000e1046 0e184a0f x..........F..J.
-  0x000020b8 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
+  0x000020b8 0b770880 003f1a39 2a332422 00000000 .w...?.9*3$"....
   0x000020c8 14000000 44000000 10f0ffff 10000000 ....D...........
   0x000020d8 00000000 00000000 14000000 5c000000 ............\...
   0x000020e8 08f0ffff b0000000 00000000 00000000 ................
   0x000020f8 10000000 74000000 60f1ffff 1d000000 ....t...`.......
   0x00002108 00000000 10000000 88000000 6cf1ffff ............l...
   0x00002118 35000000 00000000 10000000 9c000000 5...............
   0x00002128 98f1ffff 4d000000 00000000 10000000 ....M...........
-  0x00002138 b0000000 d4f1ffff 77000000 00000000 ........w.......
-  0x00002148 34000000 c4000000 40f2ffff 6f000000 4.......@...o...
+  0x00002138 b0000000 d4f1ffff 72000000 00000000 ........r.......
+  0x00002148 48000000 c4000000 40f2ffff 83000000 H.......@.......
   0x00002158 00460e10 8d02420e 188c0344 0e208604 .F....B....D. ..
-  0x00002168 440e2883 054f0e30 02490e28 410e2041 D.(..O.0.I.(A. A
-  0x00002178 0e18420e 10420e08 40000000 fc000000 ..B..B..@.......
-  0x00002188 78f2ffff a2010000 00460e10 8f02450e x........F....E.
-  0x00002198 188e0345 0e208d04 420e288c 05410e30 ...E. ..B.(..A.0
-  0x000021a8 8606460e 50036401 0a0e3041 0e28420e ..F.P.d...0A.(B.
-  0x000021b8 20420e18 420e1042 0e084a0b 10000000  B..B..B..J.....
-  0x000021c8 40010000 e4f3ffff 09000000 00000000 @...............
-  0x000021d8 4c000000 54010000 e0f3ffff 2e070000 L...T...........
-  0x000021e8 00460e10 8f02420e 188e0345 0e208d04 .F....B....E. ..
-  0x000021f8 420e288c 05410e30 8606410e 38830747 B.(..A.0..A.8..G
-  0x00002208 0e800103 76060a0e 38410e30 410e2842 ....v...8A.0A.(B
-  0x00002218 0e20420e 18420e10 420e0841 0b000000 . B..B..B..A....
-  0x00002228 10000000 a4010000 c0faffff 29000000 ............)...
-  0x00002238 00000000 10000000 b8010000 dcfaffff ................
-  0x00002248 26000000 00000000 00000000          &...........
+  0x00002168 440e2883 054f0e30 7b0a0e28 410e2041 D.(..O.0{..(A. A
+  0x00002178 0e18420e 10420e08 480b540e 28410e20 ..B..B..H.T.(A. 
+  0x00002188 410e1842 0e10420e 08000000 40000000 A..B..B.....@...
+  0x00002198 10010000 84f2ffff 90010000 00460e10 .............F..
+  0x000021a8 8e02450e 188d0345 0e208c04 410e2886 ..E....E. ..A.(.
+  0x000021b8 05430e30 8306440e 50035401 0a0e3041 .C.0..D.P.T...0A
+  0x000021c8 0e28410e 20420e18 420e1042 0e084c0b .(A. B..B..B..L.
+  0x000021d8 10000000 54010000 d0f3ffff 09000000 ....T...........
+  0x000021e8 00000000 4c000000 68010000 ccf3ffff ....L...h.......
+  0x000021f8 93080000 00460e10 8f02450e 188e0342 .....F....E....B
+  0x00002208 0e208d04 420e288c 05440e30 8606440e . ..B.(..D.0..D.
+  0x00002218 3883074e 0ea00103 36060a0e 38410e30 8..N....6...8A.0
+  0x00002228 410e2842 0e20420e 18420e10 420e0841 A.(B. B..B..B..A
+  0x00002238 0b000000 10000000 b8010000 1cfcffff ................
+  0x00002248 29000000 00000000 10000000 cc010000 )...............
+  0x00002258 38fcffff 23000000 00000000 00000000 8...#...........
```

#### readelf --wide --decompress --hex-dump=.init_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.init_array':
-  0x00003e08 50120000 00000000                   P.......
+  0x00003df0 50120000 00000000                   P.......
```

#### readelf --wide --decompress --hex-dump=.fini_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.fini_array':
-  0x00003e10 10120000 00000000                   ........
+  0x00003df8 10120000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.got {}

```diff
@@ -1,6 +1,6 @@
 
 Hex dump of section '.got':
-  0x00003fd8 00000000 00000000 00000000 00000000 ................
-  0x00003fe8 00000000 00000000 00000000 00000000 ................
-  0x00003ff8 00000000 00000000                   ........
+  0x00003fc0 00000000 00000000 00000000 00000000 ................
+  0x00003fd0 00000000 00000000 00000000 00000000 ................
+  0x00003fe0 00000000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.got.plt {}

```diff
@@ -1,11 +1,11 @@
 
 Hex dump of section '.got.plt':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
-  0x00004000 183e0000 00000000 00000000 00000000 .>..............
-  0x00004010 00000000 00000000 30100000 00000000 ........0.......
-  0x00004020 40100000 00000000 50100000 00000000 @.......P.......
-  0x00004030 60100000 00000000 70100000 00000000 `.......p.......
-  0x00004040 80100000 00000000 90100000 00000000 ................
-  0x00004050 a0100000 00000000 b0100000 00000000 ................
-  0x00004060 c0100000 00000000 d0100000 00000000 ................
+  0x00003fe8 003e0000 00000000 00000000 00000000 .>..............
+  0x00003ff8 00000000 00000000 30100000 00000000 ........0.......
+  0x00004008 40100000 00000000 50100000 00000000 @.......P.......
+  0x00004018 60100000 00000000 70100000 00000000 `.......p.......
+  0x00004028 80100000 00000000 90100000 00000000 ................
+  0x00004038 a0100000 00000000 b0100000 00000000 ................
+  0x00004048 c0100000 00000000 d0100000 00000000 ................
```

#### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.data':
-  0x00004070 70400000 00000000                   p@......
+  0x00004058 58400000 00000000                   X@......
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     0]  GCC: (Ubuntu 13.2.0-4ubuntu3) 13.2.0
```

### Comparing `bmxp-0.0.9/setup.py` & `bmxp-0.1.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,24 +11,32 @@
 with open(os.path.join(HERE, "requirements.txt"), encoding="utf-8") as f:
     REQUIREMENTS = f.read()
 
 module1 = Extension
 setup(
     name="bmxp",
     install_requires=REQUIREMENTS.split("\n"),
-    version="0.0.9",
+    version="0.1.0",
     description="LCMS Processing tools used by the Metabolomics Platform at the Broad"
     " Institute.",
     packages=find_namespace_packages(include=["bmxp.*"]),
     license="MIT",
     author="Daniel S. Hitchcock",
     author_email="daniel.s.hitchcock@gmail.com",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
-    keywords=["LCMS", "Alignment", "Processing", "Metabolomics", "Clustering"],
+    keywords=[
+        "LCMS",
+        "Alignment",
+        "Processing",
+        "Metabolomics",
+        "Clustering",
+        "Batch Correction",
+        "Drift Correction",
+    ],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
     package_data={"": ["*.dll", "*.so"]},
     url="https://github.com/broadinstitute/bmxp",
 )
```

### Comparing `bmxp-0.0.9/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.1.2.pyc` & `bmxp-0.1.0/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Nov 18 17:19:36 2022 UTC, .py size: 9433 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,1133 +1,1141 @@
-00000000: 550d 0d0a 0000 0000 a8be 7763 d924 0000  U.........wc.$..
+00000000: 550d 0d0a 0000 0000 c4da 2f66 5b26 0000  U........./f[&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 1201 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 0e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
-00000040: 6d04 0200 0100 6d05 5a06 0100 6401 6402  m.....m.Z...d.d.
-00000050: 6c07 5a07 6401 6402 6c08 5a08 6401 6402  l.Z.d.d.l.Z.d.d.
-00000060: 6c09 5a09 6401 6402 6c0a 5a0a 6401 6402  l.Z.d.d.l.Z.d.d.
-00000070: 6c0b 5a0c 6401 6402 6c0d 5a0e 6401 6402  l.Z.d.d.l.Z.d.d.
-00000080: 6c0f 6d10 5a11 0100 650a a012 a100 6403  l.m.Z...e.....d.
-00000090: 6404 8400 8301 5a13 650a a012 a100 6405  d.....Z.e.....d.
-000000a0: 6406 8400 8301 5a14 650a a012 a100 6407  d.....Z.e.....d.
-000000b0: 6408 8400 8301 5a15 650a a012 a100 6409  d.....Z.e.....d.
-000000c0: 640a 8400 8301 5a16 650a a012 a100 640b  d.....Z.e.....d.
-000000d0: 640c 8400 8301 5a17 650a a012 a100 640d  d.....Z.e.....d.
-000000e0: 640e 8400 8301 5a18 650a a012 a100 640f  d.....Z.e.....d.
-000000f0: 6410 8400 8301 5a19 6411 6412 8400 5a1a  d.....Z.d.d...Z.
-00000100: 6413 6414 8400 5a1b 6415 6416 8400 5a1c  d.d...Z.d.d...Z.
-00000110: 6417 6418 8400 5a1d 650a 6a1e a01f 6419  d.d...Z.e.j...d.
-00000120: a101 641a 641b 8400 8301 5a20 641c 641d  ..d.d.....Z d.d.
-00000130: 8400 5a21 641e 641f 8400 5a22 6402 5300  ..Z!d.d...Z"d.S.
-00000140: 2920 7a15 0a54 6573 7473 2066 6f72 204d  ) z..Tests for M
-00000150: 5345 636c 6970 7365 0ae9 0000 0000 4e63  SEclipse......Nc
-00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000170: 0400 0000 4300 0000 7312 0000 0074 0064  ....C...s....t.d
-00000180: 0174 01a0 02a1 0083 0201 0064 0253 0029  .t.........d.S.)
-00000190: 037a 220a 2020 2020 4669 7273 7420 6669  .z".    First fi
+00000040: 6d04 0200 0100 6d05 5a06 0100 6401 6403  m.....m.Z...d.d.
+00000050: 6c07 6d08 5a08 0100 6401 6402 6c09 5a09  l.m.Z...d.d.l.Z.
+00000060: 6401 6402 6c0a 5a0a 6401 6402 6c0b 5a0c  d.d.l.Z.d.d.l.Z.
+00000070: 6401 6402 6c0d 5a0e 6401 6402 6c0f 6d10  d.d.l.Z.d.d.l.m.
+00000080: 5a11 0100 650a a012 a100 6404 6405 8400  Z...e.....d.d...
+00000090: 8301 5a13 650a a012 a100 6406 6407 8400  ..Z.e.....d.d...
+000000a0: 8301 5a14 650a a012 a100 6408 6409 8400  ..Z.e.....d.d...
+000000b0: 8301 5a15 650a a012 a100 640a 640b 8400  ..Z.e.....d.d...
+000000c0: 8301 5a16 650a a012 a100 640c 640d 8400  ..Z.e.....d.d...
+000000d0: 8301 5a17 650a a012 a100 640e 640f 8400  ..Z.e.....d.d...
+000000e0: 8301 5a18 650a a012 a100 6410 6411 8400  ..Z.e.....d.d...
+000000f0: 8301 5a19 6412 6413 8400 5a1a 6414 6415  ..Z.d.d...Z.d.d.
+00000100: 8400 5a1b 6416 6417 8400 5a1c 6418 6419  ..Z.d.d...Z.d.d.
+00000110: 8400 5a1d 650a 6a1e a01f 641a a101 641b  ..Z.e.j...d...d.
+00000120: 641c 8400 8301 5a20 641d 641e 8400 5a21  d.....Z d.d...Z!
+00000130: 641f 6420 8400 5a22 6402 5300 2921 7a15  d.d ..Z"d.S.)!z.
+00000140: 0a54 6573 7473 2066 6f72 204d 5345 636c  .Tests for MSEcl
+00000150: 6970 7365 0ae9 0000 0000 4e29 01da 0450  ipse......N)...P
+00000160: 6174 6863 0000 0000 0000 0000 0000 0000  athc............
+00000170: 0000 0000 0200 0000 4300 0000 730e 0000  ........C...s...
+00000180: 0074 0074 0183 016a 0264 011b 0053 0029  .t.t...j.d...S.)
+00000190: 027a 220a 2020 2020 4669 7273 7420 6669  .z".    First fi
 000001a0: 6c65 2070 6174 6820 666f 7220 7465 7374  le path for test
-000001b0: 0a20 2020 207a 112a 2a2a 2a2a 2a2a 2a2a  .    z.*********
-000001c0: 2a2a 2a2a 2a2a 2a2a 7a0f 7465 7374 732f  ********z.tests/
-000001d0: 7465 7374 312e 6373 7629 03da 0570 7269  test1.csv)...pri
-000001e0: 6e74 da02 6f73 da06 6765 7463 7764 a900  nt..os..getcwd..
-000001f0: 7205 0000 0072 0500 0000 fa39 433a 5c55  r....r.....9C:\U
-00000200: 7365 7273 5c64 616e 6965 5c6d 7870 2d74  sers\danie\mxp-t
-00000210: 6f6f 6c73 5c73 7263 5c62 6d78 705c 7465  ools\src\bmxp\te
-00000220: 7374 735c 7465 7374 5f6d 7365 636c 6970  sts\test_mseclip
-00000230: 7365 2e70 79da 0a66 696c 6570 6174 685f  se.py..filepath_
-00000240: 310e 0000 0073 0400 0000 0005 0e01 7207  1....s........r.
-00000250: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000260: 0000 0000 0100 0000 4300 0000 7304 0000  ........C...s...
-00000270: 0064 0153 0029 027a 230a 2020 2020 5365  .d.S.).z#.    Se
-00000280: 636f 6e64 2066 696c 6520 7061 7468 2066  cond file path f
-00000290: 6f72 2074 6573 740a 2020 2020 7a0f 7465  or test.    z.te
-000002a0: 7374 732f 7465 7374 322e 6373 7672 0500  sts/test2.csvr..
-000002b0: 0000 7205 0000 0072 0500 0000 7205 0000  ..r....r....r...
-000002c0: 0072 0600 0000 da0a 6669 6c65 7061 7468  .r......filepath
-000002d0: 5f32 1700 0000 7302 0000 0000 0572 0800  _2....s......r..
-000002e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000002f0: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
-00000300: 6401 5300 2902 7a22 0a20 2020 2054 6869  d.S.).z".    Thi
-00000310: 7264 2066 696c 6520 7061 7468 2066 6f72  rd file path for
-00000320: 2074 6573 740a 2020 2020 7a0f 7465 7374   test.    z.test
-00000330: 732f 7465 7374 332e 6373 7672 0500 0000  s/test3.csvr....
-00000340: 7205 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
-00000350: 0600 0000 da0a 6669 6c65 7061 7468 5f33  ......filepath_3
-00000360: 1f00 0000 7302 0000 0000 0572 0900 0000  ....s......r....
-00000370: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000380: 0003 0000 0043 0000 0073 0a00 0000 7400  .....C...s....t.
-00000390: a001 7c00 a101 5300 2901 7a22 0a20 2020  ..|...S.).z".   
-000003a0: 2046 6972 7374 2064 6174 6166 7261 6d65   First dataframe
-000003b0: 2066 6f72 2074 6573 740a 2020 2020 a902   for test.    ..
-000003c0: da02 7064 5a08 7265 6164 5f63 7376 2901  ..pdZ.read_csv).
-000003d0: 7207 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
-000003e0: 0600 0000 da0b 6461 7461 6672 616d 655f  ......dataframe_
-000003f0: 3127 0000 0073 0200 0000 0005 720c 0000  1'...s......r...
-00000400: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00000410: 0000 0300 0000 4300 0000 730a 0000 0074  ......C...s....t
-00000420: 00a0 017c 00a1 0153 0029 017a 230a 2020  ...|...S.).z#.  
-00000430: 2020 5365 636f 6e64 2064 6174 6166 7261    Second datafra
-00000440: 6d65 2066 6f72 2074 6573 740a 2020 2020  me for test.    
-00000450: 720a 0000 0029 0172 0800 0000 7205 0000  r....).r....r...
-00000460: 0072 0500 0000 7206 0000 00da 0b64 6174  .r....r......dat
-00000470: 6166 7261 6d65 5f32 2f00 0000 7302 0000  aframe_2/...s...
-00000480: 0000 0572 0d00 0000 6301 0000 0000 0000  ...r....c.......
-00000490: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-000004a0: 0073 0a00 0000 7400 a001 7c00 a101 5300  .s....t...|...S.
-000004b0: 2901 7a22 0a20 2020 2054 6869 7264 2064  ).z".    Third d
-000004c0: 6174 6166 7261 6d65 2066 6f72 2074 6573  ataframe for tes
-000004d0: 740a 2020 2020 720a 0000 0029 0172 0900  t.    r....).r..
-000004e0: 0000 7205 0000 0072 0500 0000 7206 0000  ..r....r....r...
-000004f0: 00da 0b64 6174 6166 7261 6d65 5f33 3700  ...dataframe_37.
-00000500: 0000 7302 0000 0000 0572 0e00 0000 6300  ..s......r....c.
-00000510: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-00000520: 0000 0043 0000 0073 1000 0000 7400 a001  ...C...s....t...
-00000530: 7402 6401 6402 8302 a101 5300 2903 7a1b  t.d.d.....S.).z.
-00000540: 0a20 2020 204c 6f61 6420 7069 636b 6c65  .    Load pickle
-00000550: 6420 6669 6c65 0a20 2020 207a 1674 6573  d file.    z.tes
-00000560: 7473 2f6d 7365 636c 6970 7365 2e70 6963  ts/mseclipse.pic
-00000570: 6b6c 65da 0272 6229 03da 0670 6963 6b6c  kle..rb)...pickl
-00000580: 65da 046c 6f61 64da 046f 7065 6e72 0500  e..load..openr..
-00000590: 0000 7205 0000 0072 0500 0000 7206 0000  ..r....r....r...
-000005a0: 00da 0a70 6963 6b6c 6564 5f6d 733f 0000  ...pickled_ms?..
-000005b0: 0073 0600 0000 0005 0401 08ff 7213 0000  .s..........r...
-000005c0: 0063 0400 0000 0000 0000 0000 0000 0b00  .c..............
-000005d0: 0000 0900 0000 4300 0000 73f8 0200 0074  ......C...s....t
-000005e0: 006a 017c 007c 0164 0164 0267 0264 038d  .j.|.|.d.d.g.d..
-000005f0: 0301 0074 006a 017c 027c 0364 0164 0267  ...t.j.|.|.d.d.g
-00000600: 0264 038d 0301 0074 02a0 0374 04a1 018f  .d.....t...t....
-00000610: 127d 0474 00a0 017c 027c 03a1 0201 0057  .}.t...|.|.....W
-00000620: 0035 0051 0052 0058 0064 047d 057c 046a  .5.Q.R.X.d.}.|.j
-00000630: 057d 0674 067c 0683 017d 077c 057c 076b  .}.t.|...}.|.|.k
-00000640: 067d 087c 0873 fa74 07a0 0864 057c 0866  .}.|.s.t...d.|.f
-00000650: 0164 067c 057c 0766 02a1 0474 07a0 097c  .d.|.|.f...t...|
-00000660: 05a1 0164 0774 0aa0 0ba1 006b 0673 9a74  ...d.t.....k.s.t
-00000670: 07a0 0c74 06a1 0172 a474 07a0 0974 06a1  ...t...r.t...t..
-00000680: 016e 0264 0764 0874 0aa0 0ba1 006b 0673  .n.d.d.t.....k.s
-00000690: bc74 07a0 0c7c 04a1 0172 c674 07a0 097c  .t...|...r.t...|
-000006a0: 04a1 016e 0264 0874 07a0 097c 06a1 0174  ...n.d.t...|...t
-000006b0: 07a0 097c 07a1 0164 099c 0516 007d 0964  ...|...d.....}.d
-000006c0: 0a64 0b7c 0969 0116 007d 0a74 0d74 07a0  .d.|.i...}.t.t..
-000006d0: 0e7c 0aa1 0183 0182 0164 0c04 007d 0504  .|.......d...}..
-000006e0: 007d 0804 007d 067d 0774 02a0 0374 04a1  .}...}.}.t...t..
-000006f0: 018f 1c7d 0474 006a 017c 007c 0164 0164  ...}.t.j.|.|.d.d
-00000700: 0264 0d67 0364 038d 0301 0057 0035 0051  .d.g.d.....W.5.Q
-00000710: 0052 0058 0064 0e7d 057c 046a 057d 0674  .R.X.d.}.|.j.}.t
-00000720: 067c 0683 017d 077c 057c 076b 067d 087c  .|...}.|.|.k.}.|
-00000730: 0890 0173 f074 07a0 0864 057c 0866 0164  ...s.t...d.|.f.d
-00000740: 067c 057c 0766 02a1 0474 07a0 097c 05a1  .|.|.f...t...|..
-00000750: 0164 0774 0aa0 0ba1 006b 0690 0173 8c74  .d.t.....k...s.t
-00000760: 07a0 0c74 06a1 0190 0172 9674 07a0 0974  ...t.....r.t...t
-00000770: 06a1 016e 0264 0764 0874 0aa0 0ba1 006b  ...n.d.d.t.....k
-00000780: 0690 0173 b274 07a0 0c7c 04a1 0190 0172  ...s.t...|.....r
-00000790: bc74 07a0 097c 04a1 016e 0264 0874 07a0  .t...|...n.d.t..
-000007a0: 097c 06a1 0174 07a0 097c 07a1 0164 099c  .|...t...|...d..
-000007b0: 0516 007d 0964 0a64 0b7c 0969 0116 007d  ...}.d.d.|.i...}
-000007c0: 0a74 0d74 07a0 0e7c 0aa1 0183 0182 0164  .t.t...|.......d
-000007d0: 0c04 007d 0504 007d 0804 007d 067d 0774  ...}...}...}.}.t
-000007e0: 02a0 0374 04a1 018f 1a7d 0474 006a 017c  ...t.....}.t.j.|
-000007f0: 007c 0164 0264 0267 0264 038d 0301 0057  .|.d.d.g.d.....W
-00000800: 0035 0051 0052 0058 0064 0f7d 057c 046a  .5.Q.R.X.d.}.|.j
-00000810: 057d 0674 067c 0683 017d 077c 057c 076b  .}.t.|...}.|.|.k
-00000820: 067d 087c 0890 0273 e474 07a0 0864 057c  .}.|...s.t...d.|
-00000830: 0866 0164 067c 057c 0766 02a1 0474 07a0  .f.d.|.|.f...t..
-00000840: 097c 05a1 0164 0774 0aa0 0ba1 006b 0690  .|...d.t.....k..
-00000850: 0273 8074 07a0 0c74 06a1 0190 0272 8a74  .s.t...t.....r.t
-00000860: 07a0 0974 06a1 016e 0264 0764 0874 0aa0  ...t...n.d.d.t..
-00000870: 0ba1 006b 0690 0273 a674 07a0 0c7c 04a1  ...k...s.t...|..
-00000880: 0190 0272 b074 07a0 097c 04a1 016e 0264  ...r.t...|...n.d
-00000890: 0874 07a0 097c 06a1 0174 07a0 097c 07a1  .t...|...t...|..
-000008a0: 0164 099c 0516 007d 0964 0a64 0b7c 0969  .d.....}.d.d.|.i
-000008b0: 0116 007d 0a74 0d74 07a0 0e7c 0aa1 0183  ...}.t.t...|....
-000008c0: 0182 0164 0c04 007d 0504 007d 0804 007d  ...d...}...}...}
-000008d0: 067d 0764 0c53 0029 107a 350a 2020 2020  .}.d.S.).z5.    
-000008e0: 5465 7374 204d 5341 6c69 676e 6572 2069  Test MSAligner i
-000008f0: 6e69 7469 616c 697a 6573 206f 7220 7468  nitializes or th
-00000900: 726f 7773 2065 7272 6f72 730a 2020 2020  rows errors.    
-00000910: da03 6870 31da 0368 7032 a901 da05 6e61  ..hp1..hp2....na
-00000920: 6d65 73fa 106d 7573 7420 6265 2070 726f  mes..must be pro
-00000930: 7669 6465 64a9 01da 0269 6ea9 017a 4b25  vided....in..zK%
-00000940: 2870 7931 2973 2069 6e20 2528 7079 3829  (py1)s in %(py8)
-00000950: 730a 7b25 2870 7938 2973 203d 2025 2870  s.{%(py8)s = %(p
-00000960: 7933 2973 2825 2870 7936 2973 0a7b 2528  y3)s(%(py6)s.{%(
-00000970: 7079 3629 7320 3d20 2528 7079 3429 732e  py6)s = %(py4)s.
-00000980: 7661 6c75 650a 7d29 0a7d da03 7374 72da  value.}).}..str.
-00000990: 0165 a905 da03 7079 31da 0370 7933 da03  .e....py1..py3..
-000009a0: 7079 34da 0370 7936 da03 7079 38fa 0f61  py4..py6..py8..a
-000009b0: 7373 6572 7420 2528 7079 3130 2973 da04  ssert %(py10)s..
-000009c0: 7079 3130 4eda 0368 7033 7a13 5468 6520  py10N..hp3z.The 
-000009d0: 6e75 6d62 6572 206f 6620 6e61 6d65 73da  number of names.
-000009e0: 0964 7570 6c69 6361 7465 290f da02 6d73  .duplicate)...ms
-000009f0: da09 4d53 416c 6967 6e65 72da 0670 7974  ..MSAligner..pyt
-00000a00: 6573 74da 0672 6169 7365 73da 0a56 616c  est..raises..Val
-00000a10: 7565 4572 726f 72da 0576 616c 7565 721c  ueError..valuer.
-00000a20: 0000 00da 0a40 7079 7465 7374 5f61 72da  .....@pytest_ar.
-00000a30: 115f 6361 6c6c 5f72 6570 7263 6f6d 7061  ._call_reprcompa
-00000a40: 7265 da09 5f73 6166 6572 6570 72da 0c40  re.._saferepr..@
-00000a50: 7079 5f62 7569 6c74 696e 73da 066c 6f63  py_builtins..loc
-00000a60: 616c 73da 185f 7368 6f75 6c64 5f72 6570  als.._should_rep
-00000a70: 725f 676c 6f62 616c 5f6e 616d 65da 0e41  r_global_name..A
-00000a80: 7373 6572 7469 6f6e 4572 726f 72da 135f  ssertionError.._
-00000a90: 666f 726d 6174 5f65 7870 6c61 6e61 7469  format_explanati
-00000aa0: 6f6e 290b 7207 0000 0072 0800 0000 720c  on).r....r....r.
-00000ab0: 0000 0072 0d00 0000 721d 0000 00da 0b40  ...r....r......@
-00000ac0: 7079 5f61 7373 6572 7430 da0b 4070 795f  py_assert0..@py_
-00000ad0: 6173 7365 7274 35da 0b40 7079 5f61 7373  assert5..@py_ass
-00000ae0: 6572 7437 da0b 4070 795f 6173 7365 7274  ert7..@py_assert
-00000af0: 32da 0b40 7079 5f66 6f72 6d61 7439 da0c  2..@py_format9..
-00000b00: 4070 795f 666f 726d 6174 3131 7205 0000  @py_format11r...
-00000b10: 0072 0500 0000 7206 0000 00da 1374 6573  .r....r......tes
-00000b20: 745f 696e 6974 6961 6c69 7a65 5f61 6464  t_initialize_add
-00000b30: 4900 0000 7346 0000 0000 0614 0314 030c  I...sF..........
-00000b40: 0116 0104 0006 0008 0008 0004 0078 000c  .............x..
-00000b50: 000e 0010 030c 0120 0104 0006 0008 0008  ....... ........
-00000b60: 0006 0080 000c 000e 0010 030c 011e 0104  ................
-00000b70: 0006 0008 0008 0006 0080 000c 000e 0072  ...............r
-00000b80: 3c00 0000 6304 0000 0000 0000 0000 0000  <...c...........
-00000b90: 000c 0000 0009 0000 0043 0000 0073 fc01  .........C...s..
-00000ba0: 0000 7400 a001 a100 7d04 7c04 a002 7c00  ..t.....}.|...|.
-00000bb0: 6401 a102 0100 7c04 a002 7c03 6402 a102  d.....|...|.d...
-00000bc0: 0100 7403 a004 7405 a101 8f12 7d05 7c04  ..t...t.....}.|.
-00000bd0: a002 7c01 6402 a102 0100 5700 3500 5100  ..|.d.....W.5.Q.
-00000be0: 5200 5800 6403 7d06 7c05 6a06 7d07 7407  R.X.d.}.|.j.}.t.
-00000bf0: 7c07 8301 7d08 7c06 7c08 6b06 7d09 7c09  |...}.|.|.k.}.|.
-00000c00: 73f2 7408 a009 6404 7c09 6601 6405 7c06  s.t...d.|.f.d.|.
-00000c10: 7c08 6602 a104 7408 a00a 7c06 a101 6406  |.f...t...|...d.
-00000c20: 740b a00c a100 6b06 7392 7408 a00d 7407  t.....k.s.t...t.
-00000c30: a101 729c 7408 a00a 7407 a101 6e02 6406  ..r.t...t...n.d.
-00000c40: 6407 740b a00c a100 6b06 73b4 7408 a00d  d.t.....k.s.t...
-00000c50: 7c05 a101 72be 7408 a00a 7c05 a101 6e02  |...r.t...|...n.
-00000c60: 6407 7408 a00a 7c07 a101 7408 a00a 7c08  d.t...|...t...|.
-00000c70: a101 6408 9c05 1600 7d0a 6409 640a 7c0a  ..d.....}.d.d.|.
-00000c80: 6901 1600 7d0b 740e 7408 a00f 7c0b a101  i...}.t.t...|...
-00000c90: 8301 8201 640b 0400 7d06 0400 7d09 0400  ....d...}...}...
-00000ca0: 7d07 7d08 7c04 a002 7c02 640c a102 0100  }.}.|...|.d.....
-00000cb0: 7403 a004 7405 a101 8f10 7d05 7c04 a002  t...t.....}.|...
-00000cc0: 7c03 a101 0100 5700 3500 5100 5200 5800  |.....W.5.Q.R.X.
-00000cd0: 640d 7d06 7c05 6a06 7d07 7407 7c07 8301  d.}.|.j.}.t.|...
-00000ce0: 7d08 7c06 7c08 6b06 7d09 7c09 9001 73e8  }.|.|.k.}.|...s.
-00000cf0: 7408 a009 6404 7c09 6601 6405 7c06 7c08  t...d.|.f.d.|.|.
-00000d00: 6602 a104 7408 a00a 7c06 a101 6406 740b  f...t...|...d.t.
-00000d10: a00c a100 6b06 9001 7384 7408 a00d 7407  ....k...s.t...t.
-00000d20: a101 9001 728e 7408 a00a 7407 a101 6e02  ....r.t...t...n.
-00000d30: 6406 6407 740b a00c a100 6b06 9001 73aa  d.d.t.....k...s.
-00000d40: 7408 a00d 7c05 a101 9001 72b4 7408 a00a  t...|.....r.t...
-00000d50: 7c05 a101 6e02 6407 7408 a00a 7c07 a101  |...n.d.t...|...
-00000d60: 7408 a00a 7c08 a101 6408 9c05 1600 7d0a  t...|...d.....}.
-00000d70: 6409 640a 7c0a 6901 1600 7d0b 740e 7408  d.d.|.i...}.t.t.
-00000d80: a00f 7c0b a101 8301 8201 640b 0400 7d06  ..|.......d...}.
-00000d90: 0400 7d09 0400 7d07 7d08 640b 5300 290e  ..}...}.}.d.S.).
-00000da0: 7a2b 0a20 2020 2054 6573 7420 4d53 416c  z+.    Test MSAl
-00000db0: 6967 6e65 7220 6164 645f 6461 7461 7365  igner add_datase
-00000dc0: 7420 6d65 7468 6f64 0a20 2020 2072 1400  t method.    r..
-00000dd0: 0000 7215 0000 0072 2700 0000 7219 0000  ..r....r'...r...
-00000de0: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00000df0: 721e 0000 0072 2400 0000 7225 0000 004e  r....r$...r%...N
-00000e00: 7226 0000 0072 1800 0000 2910 7228 0000  r&...r....).r(..
-00000e10: 0072 2900 0000 da0b 6164 645f 6461 7461  .r).....add_data
-00000e20: 7365 7472 2a00 0000 722b 0000 0072 2c00  setr*...r+...r,.
-00000e30: 0000 722d 0000 0072 1c00 0000 722e 0000  ..r-...r....r...
-00000e40: 0072 2f00 0000 7230 0000 0072 3100 0000  .r/...r0...r1...
-00000e50: 7232 0000 0072 3300 0000 7234 0000 0072  r2...r3...r4...r
-00000e60: 3500 0000 290c 7207 0000 0072 0800 0000  5...).r....r....
-00000e70: 720c 0000 0072 0d00 0000 da01 6172 1d00  r....r......ar..
-00000e80: 0000 7236 0000 0072 3700 0000 7238 0000  ..r6...r7...r8..
-00000e90: 0072 3900 0000 723a 0000 0072 3b00 0000  .r9...r:...r;...
-00000ea0: 7205 0000 0072 0500 0000 7206 0000 00da  r....r....r.....
-00000eb0: 1074 6573 745f 6164 645f 6461 7461 7365  .test_add_datase
-00000ec0: 7464 0000 0073 3400 0000 0004 0803 0c01  td...s4.........
-00000ed0: 0c03 0c01 1601 0400 0600 0800 0800 0400  ................
-00000ee0: 7800 0c00 0e00 1003 0c03 0c01 1401 0400  x...............
-00000ef0: 0600 0800 0800 0600 8000 0c00 0e00 723f  ..............r?
-00000f00: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00000f10: 2800 0000 0c00 0000 4300 0000 731e 1600  (.......C...s...
-00000f20: 0074 006a 017c 007c 0164 0164 0267 0264  .t.j.|.|.d.d.g.d
-00000f30: 038d 037d 037c 03a0 02a1 0001 007c 036a  ...}.|.......|.j
-00000f40: 0364 0119 007d 047c 026a 0364 0119 007d  .d...}.|.j.d...}
-00000f50: 057c 047c 056b 027d 067c 0673 8274 04a0  .|.|.k.}.|.s.t..
-00000f60: 0564 047c 0666 0164 057c 047c 0566 02a1  .d.|.f.d.|.|.f..
-00000f70: 0474 04a0 067c 04a1 0174 04a0 067c 05a1  .t...|...t...|..
-00000f80: 0164 069c 0216 007d 0764 0764 087c 0769  .d.....}.d.d.|.i
-00000f90: 0116 007d 0874 0774 04a0 087c 08a1 0183  ...}.t.t...|....
-00000fa0: 0182 0164 0904 007d 0404 007d 067d 057c  ...d...}...}.}.|
-00000fb0: 036a 0364 0219 007d 047c 026a 0364 0219  .j.d...}.|.j.d..
-00000fc0: 007d 057c 047c 056b 027d 067c 0673 f474  .}.|.|.k.}.|.s.t
-00000fd0: 04a0 0564 047c 0666 0164 057c 047c 0566  ...d.|.f.d.|.|.f
-00000fe0: 02a1 0474 04a0 067c 04a1 0174 04a0 067c  ...t...|...t...|
-00000ff0: 05a1 0164 069c 0216 007d 0764 0764 087c  ...d.....}.d.d.|
-00001000: 0769 0116 007d 0874 0774 04a0 087c 08a1  .i...}.t.t...|..
-00001010: 0183 0182 0164 0904 007d 0404 007d 067d  .....d...}...}.}
-00001020: 057c 03a0 09a1 0001 0074 0a6a 0b7d 097c  .|.......t.j.}.|
-00001030: 036a 0c64 0119 0064 0219 007d 057c 056a  .j.d...d...}.|.j
-00001040: 0d7d 0a7c 026a 0c64 0119 0064 0219 007d  .}.|.j.d...d...}
-00001050: 0b7c 0b6a 0d7d 0c7c 097c 0a7c 0c83 027d  .|.j.}.|.|.|...}
-00001060: 0d7c 0d6a 0e7d 0e7c 0e83 007d 0f7c 0f90  .|.j.}.|...}.|..
-00001070: 0173 d064 0a64 0b74 0fa0 10a1 006b 0690  .s.d.d.t.....k..
-00001080: 0173 6e74 04a0 1174 0aa1 0190 0172 7874  .snt...t.....rxt
-00001090: 04a0 0674 0aa1 016e 0264 0b74 04a0 067c  ...t...n.d.t...|
-000010a0: 09a1 0174 04a0 067c 05a1 0174 04a0 067c  ...t...|...t...|
-000010b0: 0aa1 0174 04a0 067c 0ba1 0174 04a0 067c  ...t...|...t...|
-000010c0: 0ca1 0174 04a0 067c 0da1 0174 04a0 067c  ...t...|...t...|
-000010d0: 0ea1 0174 04a0 067c 0fa1 0164 0c9c 0916  ...t...|...d....
-000010e0: 007d 1074 0774 04a0 087c 10a1 0183 0182  .}.t.t...|......
-000010f0: 0164 0904 007d 0904 007d 0504 007d 0a04  .d...}...}...}..
-00001100: 007d 0b04 007d 0c04 007d 0d04 007d 0e7d  .}...}...}...}.}
-00001110: 0f7c 03a0 12a1 0001 007c 036a 1364 0119  .|.......|.j.d..
-00001120: 0064 0219 007d 117c 026a 1364 0119 0064  .d...}.|.j.d...d
-00001130: 0219 007d 1274 0a6a 147d 097c 1164 0d19  ...}.t.j.}.|.d..
-00001140: 0064 0e19 007d 057c 1264 0d19 0064 0e19  .d...}.|.d...d..
-00001150: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b6a  .}.|.|.|...}.|.j
-00001160: 0e7d 0c7c 0c83 007d 0d7c 0d90 0273 bc64  .}.|...}.|...s.d
-00001170: 0f64 0b74 0fa0 10a1 006b 0690 0273 6a74  .d.t.....k...sjt
-00001180: 04a0 1174 0aa1 0190 0272 7474 04a0 0674  ...t.....rtt...t
-00001190: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
-000011a0: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
-000011b0: 04a0 067c 0ba1 0174 04a0 067c 0ca1 0174  ...|...t...|...t
-000011c0: 04a0 067c 0da1 0164 109c 0716 007d 1374  ...|...d.....}.t
-000011d0: 0774 04a0 087c 13a1 0183 0182 0164 0904  .t...|.......d..
-000011e0: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
-000011f0: 007d 0c7d 0d74 0a6a 147d 097c 1164 0d19  .}.}.t.j.}.|.d..
-00001200: 0064 1119 007d 057c 1264 0d19 0064 1119  .d...}.|.d...d..
-00001210: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b6a  .}.|.|.|...}.|.j
-00001220: 0e7d 0c7c 0c83 007d 0d7c 0d90 0373 7c64  .}.|...}.|...s|d
-00001230: 0f64 0b74 0fa0 10a1 006b 0690 0373 2a74  .d.t.....k...s*t
-00001240: 04a0 1174 0aa1 0190 0372 3474 04a0 0674  ...t.....r4t...t
-00001250: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
-00001260: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
-00001270: 04a0 067c 0ba1 0174 04a0 067c 0ca1 0174  ...|...t...|...t
-00001280: 04a0 067c 0da1 0164 109c 0716 007d 1374  ...|...d.....}.t
-00001290: 0774 04a0 087c 13a1 0183 0182 0164 0904  .t...|.......d..
-000012a0: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
-000012b0: 007d 0c7d 0d74 0a6a 147d 097c 1164 1219  .}.}.t.j.}.|.d..
-000012c0: 0064 0e19 007d 057c 1264 1219 0064 0e19  .d...}.|.d...d..
-000012d0: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b6a  .}.|.|.|...}.|.j
-000012e0: 0e7d 0c7c 0c83 007d 0d7c 0d90 0473 3c64  .}.|...}.|...s<d
-000012f0: 0f64 0b74 0fa0 10a1 006b 0690 0373 ea74  .d.t.....k...s.t
-00001300: 04a0 1174 0aa1 0190 0372 f474 04a0 0674  ...t.....r.t...t
-00001310: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
-00001320: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
-00001330: 04a0 067c 0ba1 0174 04a0 067c 0ca1 0174  ...|...t...|...t
-00001340: 04a0 067c 0da1 0164 109c 0716 007d 1374  ...|...d.....}.t
-00001350: 0774 04a0 087c 13a1 0183 0182 0164 0904  .t...|.......d..
-00001360: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
-00001370: 007d 0c7d 0d74 0a6a 147d 097c 1164 1219  .}.}.t.j.}.|.d..
-00001380: 0064 1119 007d 057c 1264 1219 0064 1119  .d...}.|.d...d..
-00001390: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b6a  .}.|.|.|...}.|.j
-000013a0: 0e7d 0c7c 0c83 007d 0d7c 0d90 0473 fc64  .}.|...}.|...s.d
-000013b0: 0f64 0b74 0fa0 10a1 006b 0690 0473 aa74  .d.t.....k...s.t
-000013c0: 04a0 1174 0aa1 0190 0472 b474 04a0 0674  ...t.....r.t...t
-000013d0: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
-000013e0: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
-000013f0: 04a0 067c 0ba1 0174 04a0 067c 0ca1 0174  ...|...t...|...t
-00001400: 04a0 067c 0da1 0164 109c 0716 007d 1374  ...|...d.....}.t
-00001410: 0774 04a0 087c 13a1 0183 0182 0164 0904  .t...|.......d..
-00001420: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
-00001430: 007d 0c7d 0d74 0a6a 147d 097c 1164 1319  .}.}.t.j.}.|.d..
-00001440: 0064 1119 007d 057c 1264 1319 0064 1119  .d...}.|.d...d..
-00001450: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b6a  .}.|.|.|...}.|.j
-00001460: 0e7d 0c7c 0c83 007d 0d7c 0d90 0573 bc64  .}.|...}.|...s.d
-00001470: 0f64 0b74 0fa0 10a1 006b 0690 0573 6a74  .d.t.....k...sjt
-00001480: 04a0 1174 0aa1 0190 0572 7474 04a0 0674  ...t.....rtt...t
-00001490: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
-000014a0: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
-000014b0: 04a0 067c 0ba1 0174 04a0 067c 0ca1 0174  ...|...t...|...t
-000014c0: 04a0 067c 0da1 0164 109c 0716 007d 1374  ...|...d.....}.t
-000014d0: 0774 04a0 087c 13a1 0183 0182 0164 0904  .t...|.......d..
-000014e0: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
-000014f0: 007d 0c7d 0d74 0a6a 147d 097c 1164 1319  .}.}.t.j.}.|.d..
-00001500: 0064 0e19 007d 057c 1264 1319 0064 0e19  .d...}.|.d...d..
-00001510: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b6a  .}.|.|.|...}.|.j
-00001520: 0e7d 0c7c 0c83 007d 0d7c 0d90 0673 7c64  .}.|...}.|...s|d
-00001530: 0f64 0b74 0fa0 10a1 006b 0690 0673 2a74  .d.t.....k...s*t
-00001540: 04a0 1174 0aa1 0190 0672 3474 04a0 0674  ...t.....r4t...t
-00001550: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
-00001560: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
-00001570: 04a0 067c 0ba1 0174 04a0 067c 0ca1 0174  ...|...t...|...t
-00001580: 04a0 067c 0da1 0164 109c 0716 007d 1374  ...|...d.....}.t
-00001590: 0774 04a0 087c 13a1 0183 0182 0164 0904  .t...|.......d..
-000015a0: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
-000015b0: 007d 0c7d 0d7c 03a0 15a1 0001 007c 036a  .}.}.|.......|.j
-000015c0: 1664 0119 0064 0219 007d 147c 026a 1664  .d...d...}.|.j.d
-000015d0: 0119 0064 0219 007d 1574 0a6a 147d 097c  ...d...}.t.j.}.|
-000015e0: 1464 0d19 007d 057c 1564 0d19 007d 0a7c  .d...}.|.d...}.|
-000015f0: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
-00001600: 0c83 007d 0d7c 0d90 0773 5864 0f64 0b74  ...}.|...sXd.d.t
-00001610: 0fa0 10a1 006b 0690 0773 0674 04a0 1174  .....k...s.t...t
-00001620: 0aa1 0190 0772 1074 04a0 0674 0aa1 016e  .....r.t...t...n
-00001630: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
-00001640: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
-00001650: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
-00001660: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
-00001670: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
-00001680: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
-00001690: 0d74 0a6a 147d 097c 1464 1219 007d 057c  .t.j.}.|.d...}.|
-000016a0: 1564 1219 007d 0a7c 097c 057c 0a83 027d  .d...}.|.|.|...}
-000016b0: 0b7c 0b6a 0e7d 0c7c 0c83 007d 0d7c 0d90  .|.j.}.|...}.|..
-000016c0: 0873 1064 0f64 0b74 0fa0 10a1 006b 0690  .s.d.d.t.....k..
-000016d0: 0773 be74 04a0 1174 0aa1 0190 0772 c874  .s.t...t.....r.t
-000016e0: 04a0 0674 0aa1 016e 0264 0b74 04a0 067c  ...t...n.d.t...|
-000016f0: 09a1 0174 04a0 067c 05a1 0174 04a0 067c  ...t...|...t...|
-00001700: 0aa1 0174 04a0 067c 0ba1 0174 04a0 067c  ...t...|...t...|
-00001710: 0ca1 0174 04a0 067c 0da1 0164 109c 0716  ...t...|...d....
-00001720: 007d 1374 0774 04a0 087c 13a1 0183 0182  .}.t.t...|......
-00001730: 0164 0904 007d 0904 007d 0504 007d 0a04  .d...}...}...}..
-00001740: 007d 0b04 007d 0c7d 0d74 0a6a 147d 097c  .}...}.}.t.j.}.|
-00001750: 1464 1319 007d 057c 1564 1319 007d 0a7c  .d...}.|.d...}.|
-00001760: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
-00001770: 0c83 007d 0d7c 0d90 0873 c864 0f64 0b74  ...}.|...s.d.d.t
-00001780: 0fa0 10a1 006b 0690 0873 7674 04a0 1174  .....k...svt...t
-00001790: 0aa1 0190 0872 8074 04a0 0674 0aa1 016e  .....r.t...t...n
-000017a0: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
-000017b0: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
-000017c0: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
-000017d0: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
-000017e0: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
-000017f0: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
-00001800: 0d7c 03a0 17a1 0001 0074 0a6a 147d 097c  .|.......t.j.}.|
-00001810: 036a 1864 0119 0064 0219 0064 0d19 007d  .j.d...d...d...}
-00001820: 057c 026a 1864 0119 0064 0219 0064 0d19  .|.j.d...d...d..
-00001830: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b90  .}.|.|.|...}.|..
-00001840: 0973 8064 1464 0b74 0fa0 10a1 006b 0690  .s.d.d.t.....k..
-00001850: 0973 3e74 04a0 1174 0aa1 0190 0972 4874  .s>t...t.....rHt
-00001860: 04a0 0674 0aa1 016e 0264 0b74 04a0 067c  ...t...n.d.t...|
-00001870: 09a1 0174 04a0 067c 05a1 0174 04a0 067c  ...t...|...t...|
-00001880: 0aa1 0174 04a0 067c 0ba1 0164 159c 0516  ...t...|...d....
-00001890: 007d 1674 0774 04a0 087c 16a1 0183 0182  .}.t.t...|......
-000018a0: 0164 0904 007d 0904 007d 0504 007d 0a7d  .d...}...}...}.}
-000018b0: 0b74 0a6a 147d 097c 036a 1864 0119 0064  .t.j.}.|.j.d...d
-000018c0: 0219 0064 1219 007d 057c 026a 1864 0119  ...d...}.|.j.d..
-000018d0: 0064 0219 0064 1219 007d 0a7c 097c 057c  .d...d...}.|.|.|
-000018e0: 0a83 027d 0b7c 0b90 0a73 2864 1464 0b74  ...}.|...s(d.d.t
-000018f0: 0fa0 10a1 006b 0690 0973 e674 04a0 1174  .....k...s.t...t
-00001900: 0aa1 0190 0972 f074 04a0 0674 0aa1 016e  .....r.t...t...n
-00001910: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
-00001920: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
-00001930: 0ba1 0164 159c 0516 007d 1674 0774 04a0  ...d.....}.t.t..
-00001940: 087c 16a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
-00001950: 007d 0504 007d 0a7d 0b74 0a6a 147d 097c  .}...}.}.t.j.}.|
-00001960: 036a 1864 0119 0064 0219 0064 1319 007d  .j.d...d...d...}
-00001970: 057c 026a 1864 0119 0064 0219 0064 1319  .|.j.d...d...d..
-00001980: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b90  .}.|.|.|...}.|..
-00001990: 0a73 d064 1464 0b74 0fa0 10a1 006b 0690  .s.d.d.t.....k..
-000019a0: 0a73 8e74 04a0 1174 0aa1 0190 0a72 9874  .s.t...t.....r.t
-000019b0: 04a0 0674 0aa1 016e 0264 0b74 04a0 067c  ...t...n.d.t...|
-000019c0: 09a1 0174 04a0 067c 05a1 0174 04a0 067c  ...t...|...t...|
-000019d0: 0aa1 0174 04a0 067c 0ba1 0164 159c 0516  ...t...|...d....
-000019e0: 007d 1674 0774 04a0 087c 16a1 0183 0182  .}.t.t...|......
-000019f0: 0164 0904 007d 0904 007d 0504 007d 0a7d  .d...}...}...}.}
-00001a00: 0b7c 03a0 19a1 0001 007c 036a 1a64 0119  .|.......|.j.d..
-00001a10: 0064 0219 007d 047c 046a 1b7d 067c 026a  .d...}.|.j.}.|.j
-00001a20: 1a64 0119 0064 0219 007d 177c 067c 1783  .d...d...}.|.|..
-00001a30: 017d 187c 1890 0b73 5064 1674 04a0 067c  .}.|...sPd.t...|
-00001a40: 04a1 0174 04a0 067c 06a1 0174 04a0 067c  ...t...|...t...|
-00001a50: 17a1 0174 04a0 067c 18a1 0164 179c 0416  ...t...|...d....
-00001a60: 007d 1974 0774 04a0 087c 19a1 0183 0182  .}.t.t...|......
-00001a70: 0164 0904 007d 0404 007d 0604 007d 177d  .d...}...}...}.}
-00001a80: 1874 006a 017c 007c 0164 0164 0267 0264  .t.j.|.|.d.d.g.d
-00001a90: 038d 037d 037c 03a0 1ca1 0001 0074 00a0  ...}.|.......t..
-00001aa0: 1d64 1864 1964 1a67 0364 1b64 1c64 1d67  .d.d.d.g.d.d.d.g
-00001ab0: 03a1 027d 1a74 00a0 1d64 1e64 1f64 2067  ...}.t...d.d.d g
-00001ac0: 0364 2164 2264 2367 03a1 027d 1b74 00a0  .d!d"d#g...}.t..
-00001ad0: 1d64 1964 1a64 2467 0364 1a64 2464 2567  .d.d.d$g.d.d$d%g
-00001ae0: 03a1 027d 1c74 006a 017c 007c 0164 0164  ...}.t.j.|.|.d.d
-00001af0: 0267 0264 038d 037d 037c 036a 1e64 0164  .g.d...}.|.j.d.d
-00001b00: 0274 1f7c 1a8e 0074 1f7c 1b8e 0074 1f7c  .t.|...t.|...t.|
-00001b10: 1c8e 0064 269c 0369 0169 0164 2764 288d  ...d&..i.i.d'd(.
-00001b20: 0201 007c 03a0 1ca1 0001 007c 036a 1364  ...|.......|.j.d
-00001b30: 0119 0064 0219 007d 1d74 0a6a 0b7d 097c  ...d...}.t.j.}.|
-00001b40: 1d64 0d19 0064 1119 007d 057c 1a64 2919  .d...d...}.|.d).
-00001b50: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b6a  .}.|.|.|...}.|.j
-00001b60: 0e7d 0c7c 0c83 007d 0d7c 0d90 0c73 bc64  .}.|...}.|...s.d
-00001b70: 2a64 0b74 0fa0 10a1 006b 0690 0c73 6a74  *d.t.....k...sjt
-00001b80: 04a0 1174 0aa1 0190 0c72 7474 04a0 0674  ...t.....rtt...t
-00001b90: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
-00001ba0: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
-00001bb0: 04a0 067c 0ba1 0174 04a0 067c 0ca1 0174  ...|...t...|...t
-00001bc0: 04a0 067c 0da1 0164 109c 0716 007d 1374  ...|...d.....}.t
-00001bd0: 0774 04a0 087c 13a1 0183 0182 0164 0904  .t...|.......d..
-00001be0: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
-00001bf0: 007d 0c7d 0d74 0a6a 0b7d 097c 1d64 0d19  .}.}.t.j.}.|.d..
-00001c00: 0064 0e19 007d 057c 1a64 1819 007d 0a7c  .d...}.|.d...}.|
-00001c10: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
-00001c20: 0c83 007d 0d7c 0d90 0d73 7864 2a64 0b74  ...}.|...sxd*d.t
-00001c30: 0fa0 10a1 006b 0690 0d73 2674 04a0 1174  .....k...s&t...t
-00001c40: 0aa1 0190 0d72 3074 04a0 0674 0aa1 016e  .....r0t...t...n
-00001c50: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
-00001c60: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
-00001c70: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
-00001c80: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
-00001c90: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
-00001ca0: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
-00001cb0: 0d74 0a6a 0b7d 097c 1d64 1219 0064 1119  .t.j.}.|.d...d..
-00001cc0: 007d 057c 1b64 2919 007d 0a7c 097c 057c  .}.|.d)..}.|.|.|
-00001cd0: 0a83 027d 0b7c 0b6a 0e7d 0c7c 0c83 007d  ...}.|.j.}.|...}
-00001ce0: 0d7c 0d90 0e73 3464 2a64 0b74 0fa0 10a1  .|...s4d*d.t....
-00001cf0: 006b 0690 0d73 e274 04a0 1174 0aa1 0190  .k...s.t...t....
-00001d00: 0d72 ec74 04a0 0674 0aa1 016e 0264 0b74  .r.t...t...n.d.t
-00001d10: 04a0 067c 09a1 0174 04a0 067c 05a1 0174  ...|...t...|...t
-00001d20: 04a0 067c 0aa1 0174 04a0 067c 0ba1 0174  ...|...t...|...t
-00001d30: 04a0 067c 0ca1 0174 04a0 067c 0da1 0164  ...|...t...|...d
-00001d40: 109c 0716 007d 1374 0774 04a0 087c 13a1  .....}.t.t...|..
-00001d50: 0183 0182 0164 0904 007d 0904 007d 0504  .....d...}...}..
-00001d60: 007d 0a04 007d 0b04 007d 0c7d 0d74 0a6a  .}...}...}.}.t.j
-00001d70: 0b7d 097c 1d64 1219 0064 0e19 007d 057c  .}.|.d...d...}.|
-00001d80: 1b64 1819 007d 0a7c 097c 057c 0a83 027d  .d...}.|.|.|...}
-00001d90: 0b7c 0b6a 0e7d 0c7c 0c83 007d 0d7c 0d90  .|.j.}.|...}.|..
-00001da0: 0e73 f064 2a64 0b74 0fa0 10a1 006b 0690  .s.d*d.t.....k..
-00001db0: 0e73 9e74 04a0 1174 0aa1 0190 0e72 a874  .s.t...t.....r.t
-00001dc0: 04a0 0674 0aa1 016e 0264 0b74 04a0 067c  ...t...n.d.t...|
-00001dd0: 09a1 0174 04a0 067c 05a1 0174 04a0 067c  ...t...|...t...|
-00001de0: 0aa1 0174 04a0 067c 0ba1 0174 04a0 067c  ...t...|...t...|
-00001df0: 0ca1 0174 04a0 067c 0da1 0164 109c 0716  ...t...|...d....
-00001e00: 007d 1374 0774 04a0 087c 13a1 0183 0182  .}.t.t...|......
-00001e10: 0164 0904 007d 0904 007d 0504 007d 0a04  .d...}...}...}..
-00001e20: 007d 0b04 007d 0c7d 0d74 0a6a 0b7d 097c  .}...}.}.t.j.}.|
-00001e30: 1d64 1319 0064 1119 007d 057c 1c64 2919  .d...d...}.|.d).
-00001e40: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b6a  .}.|.|.|...}.|.j
-00001e50: 0e7d 0c7c 0c83 007d 0d7c 0d90 0f73 ac64  .}.|...}.|...s.d
-00001e60: 2a64 0b74 0fa0 10a1 006b 0690 0f73 5a74  *d.t.....k...sZt
-00001e70: 04a0 1174 0aa1 0190 0f72 6474 04a0 0674  ...t.....rdt...t
-00001e80: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
-00001e90: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
-00001ea0: 04a0 067c 0ba1 0174 04a0 067c 0ca1 0174  ...|...t...|...t
-00001eb0: 04a0 067c 0da1 0164 109c 0716 007d 1374  ...|...d.....}.t
-00001ec0: 0774 04a0 087c 13a1 0183 0182 0164 0904  .t...|.......d..
-00001ed0: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
-00001ee0: 007d 0c7d 0d74 0a6a 0b7d 097c 1d64 1319  .}.}.t.j.}.|.d..
-00001ef0: 0064 0e19 007d 057c 1c64 1819 007d 0a7c  .d...}.|.d...}.|
-00001f00: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
-00001f10: 0c83 007d 0d7c 0d90 1073 6864 2a64 0b74  ...}.|...shd*d.t
-00001f20: 0fa0 10a1 006b 0690 1073 1674 04a0 1174  .....k...s.t...t
-00001f30: 0aa1 0190 1072 2074 04a0 0674 0aa1 016e  .....r t...t...n
-00001f40: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
-00001f50: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
-00001f60: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
-00001f70: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
-00001f80: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
-00001f90: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
-00001fa0: 0d74 006a 017c 007c 0164 0164 0267 0264  .t.j.|.|.d.d.g.d
-00001fb0: 038d 037d 037c 036a 1e64 0164 0274 1f7c  ...}.|.j.d.d.t.|
-00001fc0: 1a8e 0074 1f7c 1b8e 0074 1f7c 1c8e 0064  ...t.|...t.|...d
-00001fd0: 269c 0369 0169 0164 2b64 288d 0201 007c  &..i.i.d+d(....|
-00001fe0: 03a0 1ca1 0001 007c 036a 1364 0219 0064  .......|.j.d...d
-00001ff0: 0119 007d 1d74 0a6a 0b7d 097c 1d64 0d19  ...}.t.j.}.|.d..
-00002000: 0064 1119 007d 057c 1a64 2919 007d 0a7c  .d...}.|.d)..}.|
-00002010: 1a64 1819 007d 0b7c 0a7c 0b17 007d 0c7c  .d...}.|.|...}.|
-00002020: 097c 057c 0c83 027d 1e7c 1e6a 0e7d 1f7c  .|.|...}.|.j.}.|
-00002030: 1f83 007d 207c 2090 1173 9064 2c64 0b74  ...} | ..s.d,d.t
-00002040: 0fa0 10a1 006b 0690 1173 3674 04a0 1174  .....k...s6t...t
-00002050: 0aa1 0190 1172 4074 04a0 0674 0aa1 016e  .....r@t...t...n
-00002060: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
-00002070: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
-00002080: 0ba1 0174 04a0 067c 1ea1 0174 04a0 067c  ...t...|...t...|
-00002090: 1fa1 0174 04a0 067c 20a1 0164 2d9c 0816  ...t...| ..d-...
-000020a0: 007d 2174 0774 04a0 087c 21a1 0183 0182  .}!t.t...|!.....
-000020b0: 0164 0904 007d 0904 007d 0504 007d 0a04  .d...}...}...}..
-000020c0: 007d 0b04 007d 0c04 007d 1e04 007d 1f7d  .}...}...}...}.}
-000020d0: 2074 0a6a 0b7d 097c 1d64 0d19 0064 0e19   t.j.}.|.d...d..
-000020e0: 007d 057c 1a64 1819 007d 0a7c 0a0b 007d  .}.|.d...}.|...}
-000020f0: 0b7c 097c 057c 0b83 027d 227c 226a 0e7d  .|.|.|...}"|"j.}
-00002100: 1e7c 1e83 007d 1f7c 1f90 1273 5a64 2e64  .|...}.|...sZd.d
-00002110: 0b74 0fa0 10a1 006b 0690 1273 0874 04a0  .t.....k...s.t..
-00002120: 1174 0aa1 0190 1272 1274 04a0 0674 0aa1  .t.....r.t...t..
-00002130: 016e 0264 0b74 04a0 067c 09a1 0174 04a0  .n.d.t...|...t..
-00002140: 067c 05a1 0174 04a0 067c 0aa1 0174 04a0  .|...t...|...t..
-00002150: 067c 22a1 0174 04a0 067c 1ea1 0174 04a0  .|"..t...|...t..
-00002160: 067c 1fa1 0164 2f9c 0716 007d 2374 0774  .|...d/....}#t.t
-00002170: 04a0 087c 23a1 0183 0182 0164 0904 007d  ...|#......d...}
-00002180: 0904 007d 0504 007d 0a04 007d 0b04 007d  ...}...}...}...}
-00002190: 2204 007d 1e7d 1f7c 1b64 2919 007c 1b64  "..}.}.|.d)..|.d
-000021a0: 2919 007c 1b64 1819 0014 0064 301b 0017  )..|.d.....d0...
-000021b0: 007d 2474 0a6a 0b7d 097c 1d64 1219 0064  .}$t.j.}.|.d...d
-000021c0: 1119 007d 057c 097c 057c 2483 027d 187c  ...}.|.|.|$..}.|
-000021d0: 186a 0e7d 227c 2283 007d 1e7c 1e90 1373  .j.}"|"..}.|...s
-000021e0: 4c64 3164 0b74 0fa0 10a1 006b 0690 1273  Ld1d.t.....k...s
-000021f0: dc74 04a0 1174 0aa1 0190 1272 e674 04a0  .t...t.....r.t..
-00002200: 0674 0aa1 016e 0264 0b74 04a0 067c 09a1  .t...n.d.t...|..
-00002210: 0174 04a0 067c 05a1 0164 3274 0fa0 10a1  .t...|...d2t....
-00002220: 006b 0690 1373 1274 04a0 117c 24a1 0190  .k...s.t...|$...
-00002230: 1372 1c74 04a0 067c 24a1 016e 0264 3274  .r.t...|$..n.d2t
-00002240: 04a0 067c 18a1 0174 04a0 067c 22a1 0174  ...|...t...|"..t
-00002250: 04a0 067c 1ea1 0164 339c 0716 007d 2574  ...|...d3....}%t
-00002260: 0774 04a0 087c 25a1 0183 0182 0164 0904  .t...|%......d..
-00002270: 007d 0904 007d 0504 007d 1804 007d 227d  .}...}...}...}"}
-00002280: 1e74 0a6a 0b7d 097c 1d64 1219 0064 0e19  .t.j.}.|.d...d..
-00002290: 007d 057c 1b64 1819 007d 0a7c 0a0b 007d  .}.|.d...}.|...}
-000022a0: 0b7c 1b64 2919 007d 227c 0b7c 2214 007d  .|.d)..}"|.|"..}
-000022b0: 1e7c 1e7c 241b 007d 1f7c 097c 057c 1f83  .|.|$..}.|.|.|..
-000022c0: 027d 0e7c 0e6a 0e7d 0f7c 0f83 007d 267c  .}.|.j.}.|...}&|
-000022d0: 2690 1473 5064 3464 0b74 0fa0 10a1 006b  &..sPd4d.t.....k
-000022e0: 0690 1373 d074 04a0 1174 0aa1 0190 1372  ...s.t...t.....r
-000022f0: da74 04a0 0674 0aa1 016e 0264 0b74 04a0  .t...t...n.d.t..
-00002300: 067c 09a1 0174 04a0 067c 05a1 0174 04a0  .|...t...|...t..
-00002310: 067c 0aa1 0174 04a0 067c 22a1 0164 3274  .|...t...|"..d2t
-00002320: 0fa0 10a1 006b 0690 1473 1674 04a0 117c  .....k...s.t...|
-00002330: 24a1 0190 1472 2074 04a0 067c 24a1 016e  $....r t...|$..n
-00002340: 0264 3274 04a0 067c 0ea1 0174 04a0 067c  .d2t...|...t...|
-00002350: 0fa1 0174 04a0 067c 26a1 0164 359c 0916  ...t...|&..d5...
-00002360: 007d 2774 0774 04a0 087c 27a1 0183 0182  .}'t.t...|'.....
-00002370: 0164 0904 007d 0904 007d 0504 007d 0a04  .d...}...}...}..
-00002380: 007d 0b04 007d 2204 007d 1e04 007d 1f04  .}...}"..}...}..
-00002390: 007d 0e04 007d 0f7d 2674 0a6a 0b7d 097c  .}...}.}&t.j.}.|
-000023a0: 1d64 1319 0064 1119 007d 057c 1c64 2919  .d...d...}.|.d).
-000023b0: 007d 0a7c 1c64 1819 007d 0b7c 0a7c 0b17  .}.|.d...}.|.|..
-000023c0: 007d 0c7c 097c 057c 0c83 027d 1e7c 1e6a  .}.|.|.|...}.|.j
-000023d0: 0e7d 1f7c 1f83 007d 207c 2090 1573 3464  .}.|...} | ..s4d
-000023e0: 2c64 0b74 0fa0 10a1 006b 0690 1473 da74  ,d.t.....k...s.t
-000023f0: 04a0 1174 0aa1 0190 1472 e474 04a0 0674  ...t.....r.t...t
-00002400: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
-00002410: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
-00002420: 04a0 067c 0ba1 0174 04a0 067c 1ea1 0174  ...|...t...|...t
-00002430: 04a0 067c 1fa1 0174 04a0 067c 20a1 0164  ...|...t...| ..d
-00002440: 2d9c 0816 007d 2174 0774 04a0 087c 21a1  -....}!t.t...|!.
-00002450: 0183 0182 0164 0904 007d 0904 007d 0504  .....d...}...}..
-00002460: 007d 0a04 007d 0b04 007d 0c04 007d 1e04  .}...}...}...}..
-00002470: 007d 1f7d 2074 0a6a 0b7d 097c 1d64 1319  .}.} t.j.}.|.d..
-00002480: 0064 0e19 007d 057c 1c64 1819 007d 0a7c  .d...}.|.d...}.|
-00002490: 0a0b 007d 0b7c 097c 057c 0b83 027d 227c  ...}.|.|.|...}"|
-000024a0: 226a 0e7d 1e7c 1e83 007d 1f7c 1f90 1573  "j.}.|...}.|...s
-000024b0: fe64 2e64 0b74 0fa0 10a1 006b 0690 1573  .d.d.t.....k...s
-000024c0: ac74 04a0 1174 0aa1 0190 1572 b674 04a0  .t...t.....r.t..
-000024d0: 0674 0aa1 016e 0264 0b74 04a0 067c 09a1  .t...n.d.t...|..
-000024e0: 0174 04a0 067c 05a1 0174 04a0 067c 0aa1  .t...|...t...|..
-000024f0: 0174 04a0 067c 22a1 0174 04a0 067c 1ea1  .t...|"..t...|..
-00002500: 0174 04a0 067c 1fa1 0164 2f9c 0716 007d  .t...|...d/....}
-00002510: 2374 0774 04a0 087c 23a1 0183 0182 0164  #t.t...|#......d
-00002520: 0904 007d 0904 007d 0504 007d 0a04 007d  ...}...}...}...}
-00002530: 0b04 007d 2204 007d 1e7d 1f64 0953 0029  ...}"..}.}.d.S.)
-00002540: 367a 340a 2020 2020 5465 7374 2074 6865  6z4.    Test the
-00002550: 206d 6574 686f 6473 2061 7373 6f63 6961   methods associa
-00002560: 7465 6420 7769 7468 2061 6c69 676e 6d65  ted with alignme
-00002570: 6e74 0a20 2020 20da 0348 5031 da03 4850  nt.    ..HP1..HP
-00002580: 3272 1600 0000 a901 fa02 3d3d 2901 7a12  2r........==).z.
-00002590: 2528 7079 3129 7320 3d3d 2025 2870 7934  %(py1)s == %(py4
-000025a0: 2973 2902 721f 0000 0072 2100 0000 7a0e  )s).r....r!...z.
-000025b0: 6173 7365 7274 2025 2870 7936 2973 7222  assert %(py6)sr"
-000025c0: 0000 004e 7ac0 6173 7365 7274 2025 2870  ...Nz.assert %(p
-000025d0: 7931 3629 730a 7b25 2870 7931 3629 7320  y16)s.{%(py16)s 
-000025e0: 3d20 2528 7079 3134 2973 0a7b 2528 7079  = %(py14)s.{%(py
-000025f0: 3134 2973 203d 2025 2870 7931 3229 730a  14)s = %(py12)s.
-00002600: 7b25 2870 7931 3229 7320 3d20 2528 7079  {%(py12)s = %(py
-00002610: 3229 730a 7b25 2870 7932 2973 203d 2025  2)s.{%(py2)s = %
-00002620: 2870 7930 2973 2e65 7175 616c 0a7d 2825  (py0)s.equal.}(%
-00002630: 2870 7936 2973 0a7b 2528 7079 3629 7320  (py6)s.{%(py6)s 
-00002640: 3d20 2528 7079 3429 732e 7661 6c75 6573  = %(py4)s.values
-00002650: 0a7d 2c20 2528 7079 3130 2973 0a7b 2528  .}, %(py10)s.{%(
-00002660: 7079 3130 2973 203d 2025 2870 7938 2973  py10)s = %(py8)s
-00002670: 2e76 616c 7565 730a 7d29 0a7d 2e61 6c6c  .values.}).}.all
-00002680: 0a7d 2829 0a7d da02 6e70 2909 da03 7079  .}().}..np)...py
-00002690: 30da 0370 7932 7221 0000 0072 2200 0000  0..py2r!...r"...
-000026a0: 7223 0000 0072 2500 0000 da04 7079 3132  r#...r%.....py12
-000026b0: da04 7079 3134 da04 7079 3136 da02 5254  ..py14..py16..RT
-000026c0: da01 79fa 8661 7373 6572 7420 2528 7079  ..y..assert %(py
-000026d0: 3132 2973 0a7b 2528 7079 3132 2973 203d  12)s.{%(py12)s =
-000026e0: 2025 2870 7931 3029 730a 7b25 2870 7931   %(py10)s.{%(py1
-000026f0: 3029 7320 3d20 2528 7079 3829 730a 7b25  0)s = %(py8)s.{%
-00002700: 2870 7938 2973 203d 2025 2870 7932 2973  (py8)s = %(py2)s
-00002710: 0a7b 2528 7079 3229 7320 3d20 2528 7079  .{%(py2)s = %(py
-00002720: 3029 732e 6973 636c 6f73 650a 7d28 2528  0)s.isclose.}(%(
-00002730: 7079 3429 732c 2025 2870 7936 2973 290a  py4)s, %(py6)s).
-00002740: 7d2e 616c 6c0a 7d28 290a 7da9 0772 4500  }.all.}().}..rE.
-00002750: 0000 7246 0000 0072 2100 0000 7222 0000  ..rF...r!...r"..
-00002760: 0072 2300 0000 7225 0000 0072 4700 0000  .r#...r%...rG...
-00002770: da01 78da 024d 5ada 0949 6e74 656e 7369  ..x..MZ..Intensi
-00002780: 7479 7a52 6173 7365 7274 2025 2870 7938  tyzRassert %(py8
-00002790: 2973 0a7b 2528 7079 3829 7320 3d20 2528  )s.{%(py8)s = %(
-000027a0: 7079 3229 730a 7b25 2870 7932 2973 203d  py2)s.{%(py2)s =
-000027b0: 2025 2870 7930 2973 2e69 7363 6c6f 7365   %(py0)s.isclose
-000027c0: 0a7d 2825 2870 7934 2973 2c20 2528 7079  .}(%(py4)s, %(py
-000027d0: 3629 7329 0a7d 2905 7245 0000 0072 4600  6)s).}).rE...rF.
-000027e0: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
-000027f0: 007a 4861 7373 6572 7420 2528 7079 3729  .zHassert %(py7)
-00002800: 730a 7b25 2870 7937 2973 203d 2025 2870  s.{%(py7)s = %(p
-00002810: 7933 2973 0a7b 2528 7079 3329 7320 3d20  y3)s.{%(py3)s = 
-00002820: 2528 7079 3129 732e 6571 7561 6c73 0a7d  %(py1)s.equals.}
-00002830: 2825 2870 7935 2973 290a 7d29 0472 1f00  (%(py5)s).}).r..
-00002840: 0000 7220 0000 00da 0370 7935 da03 7079  ..r .....py5..py
-00002850: 37e9 0100 0000 e902 0000 00e9 0300 0000  7...............
-00002860: 679a 9999 9999 99f1 3f67 9a99 9999 9999  g.......?g......
-00002870: 0140 6766 6666 6666 660a 40e9 6400 0000  .@gffffff.@.d...
-00002880: e9c8 0000 0069 2c01 0000 6779 e926 3108  .....i,...gy.&1.
-00002890: 0059 4067 c7ba b88d 0600 6940 6710 e9b7  .Y@g......i@g...
-000028a0: af03 c072 40e9 0400 0000 e905 0000 00a9  ...r@...........
-000028b0: 0372 4a00 0000 724f 0000 0072 5000 0000  .rJ...rO...rP...
-000028c0: 4629 01da 0372 6563 7201 0000 007a 8461  F)...recr....z.a
-000028d0: 7373 6572 7420 2528 7079 3132 2973 0a7b  ssert %(py12)s.{
-000028e0: 2528 7079 3132 2973 203d 2025 2870 7931  %(py12)s = %(py1
-000028f0: 3029 730a 7b25 2870 7931 3029 7320 3d20  0)s.{%(py10)s = 
-00002900: 2528 7079 3829 730a 7b25 2870 7938 2973  %(py8)s.{%(py8)s
-00002910: 203d 2025 2870 7932 2973 0a7b 2528 7079   = %(py2)s.{%(py
-00002920: 3229 7320 3d20 2528 7079 3029 732e 6571  2)s = %(py0)s.eq
-00002930: 7561 6c0a 7d28 2528 7079 3429 732c 2025  ual.}(%(py4)s, %
-00002940: 2870 7936 2973 290a 7d2e 616c 6c0a 7d28  (py6)s).}.all.}(
-00002950: 290a 7d54 7a92 6173 7365 7274 2025 2870  ).}Tz.assert %(p
-00002960: 7931 3529 730a 7b25 2870 7931 3529 7320  y15)s.{%(py15)s 
-00002970: 3d20 2528 7079 3133 2973 0a7b 2528 7079  = %(py13)s.{%(py
-00002980: 3133 2973 203d 2025 2870 7931 3129 730a  13)s = %(py11)s.
-00002990: 7b25 2870 7931 3129 7320 3d20 2528 7079  {%(py11)s = %(py
-000029a0: 3229 730a 7b25 2870 7932 2973 203d 2025  2)s.{%(py2)s = %
-000029b0: 2870 7930 2973 2e65 7175 616c 0a7d 2825  (py0)s.equal.}(%
-000029c0: 2870 7934 2973 2c20 2825 2870 7936 2973  (py4)s, (%(py6)s
-000029d0: 202b 2025 2870 7938 2973 2929 0a7d 2e61   + %(py8)s)).}.a
-000029e0: 6c6c 0a7d 2829 0a7d 2908 7245 0000 0072  ll.}().}).rE...r
-000029f0: 4600 0000 7221 0000 0072 2200 0000 7223  F...r!...r"...r#
-00002a00: 0000 00da 0470 7931 31da 0470 7931 335a  .....py11..py13Z
-00002a10: 0470 7931 357a 8561 7373 6572 7420 2528  .py15z.assert %(
-00002a20: 7079 3133 2973 0a7b 2528 7079 3133 2973  py13)s.{%(py13)s
-00002a30: 203d 2025 2870 7931 3129 730a 7b25 2870   = %(py11)s.{%(p
-00002a40: 7931 3129 7320 3d20 2528 7079 3929 730a  y11)s = %(py9)s.
-00002a50: 7b25 2870 7939 2973 203d 2025 2870 7932  {%(py9)s = %(py2
-00002a60: 2973 0a7b 2528 7079 3229 7320 3d20 2528  )s.{%(py2)s = %(
-00002a70: 7079 3029 732e 6571 7561 6c0a 7d28 2528  py0)s.equal.}(%(
-00002a80: 7079 3429 732c 202d 2528 7079 3629 7329  py4)s, -%(py6)s)
-00002a90: 0a7d 2e61 6c6c 0a7d 2829 0a7d 2907 7245  .}.all.}().}).rE
-00002aa0: 0000 0072 4600 0000 7221 0000 0072 2200  ...rF...r!...r".
-00002ab0: 0000 da03 7079 3972 5c00 0000 725d 0000  ....py9r\...r]..
-00002ac0: 0069 4042 0f00 7a82 6173 7365 7274 2025  .i@B..z.assert %
-00002ad0: 2870 7931 3129 730a 7b25 2870 7931 3129  (py11)s.{%(py11)
-00002ae0: 7320 3d20 2528 7079 3929 730a 7b25 2870  s = %(py9)s.{%(p
-00002af0: 7939 2973 203d 2025 2870 7937 2973 0a7b  y9)s = %(py7)s.{
-00002b00: 2528 7079 3729 7320 3d20 2528 7079 3229  %(py7)s = %(py2)
-00002b10: 730a 7b25 2870 7932 2973 203d 2025 2870  s.{%(py2)s = %(p
-00002b20: 7930 2973 2e65 7175 616c 0a7d 2825 2870  y0)s.equal.}(%(p
-00002b30: 7934 2973 2c20 2528 7079 3529 7329 0a7d  y4)s, %(py5)s).}
-00002b40: 2e61 6c6c 0a7d 2829 0a7d da07 6e65 775f  .all.}().}..new_
-00002b50: 6d7a 7329 0772 4500 0000 7246 0000 0072  mzs).rE...rF...r
-00002b60: 2100 0000 7251 0000 0072 5200 0000 725e  !...rQ...rR...r^
-00002b70: 0000 0072 5c00 0000 7aa0 6173 7365 7274  ...r\...z.assert
-00002b80: 2025 2870 7931 3829 730a 7b25 2870 7931   %(py18)s.{%(py1
-00002b90: 3829 7320 3d20 2528 7079 3136 2973 0a7b  8)s = %(py16)s.{
-00002ba0: 2528 7079 3136 2973 203d 2025 2870 7931  %(py16)s = %(py1
-00002bb0: 3429 730a 7b25 2870 7931 3429 7320 3d20  4)s.{%(py14)s = 
-00002bc0: 2528 7079 3229 730a 7b25 2870 7932 2973  %(py2)s.{%(py2)s
-00002bd0: 203d 2025 2870 7930 2973 2e65 7175 616c   = %(py0)s.equal
-00002be0: 0a7d 2825 2870 7934 2973 2c20 2828 2d25  .}(%(py4)s, ((-%
-00002bf0: 2870 7936 2973 202a 2025 2870 7939 2973  (py6)s * %(py9)s
-00002c00: 2920 2f20 2528 7079 3131 2973 2929 0a7d  ) / %(py11)s)).}
-00002c10: 2e61 6c6c 0a7d 2829 0a7d 2909 7245 0000  .all.}().}).rE..
-00002c20: 0072 4600 0000 7221 0000 0072 2200 0000  .rF...r!...r"...
-00002c30: 725e 0000 0072 5c00 0000 7248 0000 0072  r^...r\...rH...r
-00002c40: 4900 0000 5a04 7079 3138 2920 7228 0000  I...Z.py18) r(..
-00002c50: 0072 2900 0000 5a0b 6765 6e5f 616e 6368  .r)...Z.gen_anch
-00002c60: 6f72 735a 0761 6e63 686f 7273 722e 0000  orsZ.anchorsr...
-00002c70: 0072 2f00 0000 7230 0000 0072 3400 0000  .r/...r0...r4...
-00002c80: 7235 0000 005a 0a67 656e 5f63 6f61 7273  r5...Z.gen_coars
-00002c90: 6572 4400 0000 da05 6571 7561 6c5a 0e63  erD.....equalZ.c
-00002ca0: 6f61 7273 655f 6d61 7463 6865 73da 0676  oarse_matches..v
-00002cb0: 616c 7565 73da 0361 6c6c 7231 0000 0072  alues..allr1...r
-00002cc0: 3200 0000 7233 0000 005a 0b67 656e 5f73  2...r3...Z.gen_s
-00002cd0: 6361 6c65 7273 5a07 7363 616c 6572 73da  calersZ.scalers.
-00002ce0: 0769 7363 6c6f 7365 5a11 6765 6e5f 7363  .iscloseZ.gen_sc
-00002cf0: 616c 6564 5f76 616c 7565 73da 0d73 6361  aled_values..sca
-00002d00: 6c65 645f 7661 6c75 6573 5a08 6765 6e5f  led_valuesZ.gen_
-00002d10: 7374 6473 5a04 7374 6473 5a0b 6765 6e5f  stdsZ.stdsZ.gen_
-00002d20: 6d61 7463 6865 73da 076d 6174 6368 6573  matches..matches
-00002d30: 5a06 6571 7561 6c73 da05 616c 6967 6eda  Z.equals..align.
-00002d40: 0c63 616c 635f 7363 616c 6572 735a 0b73  .calc_scalersZ.s
-00002d50: 6574 5f73 6361 6c65 7273 da03 7a69 7029  et_scalers..zip)
-00002d60: 2872 0c00 0000 720d 0000 0072 1300 0000  (r....r....r....
-00002d70: 723e 0000 0072 3600 0000 da0b 4070 795f  r>...r6.....@py_
-00002d80: 6173 7365 7274 3372 3900 0000 da0b 4070  assert3r9.....@p
-00002d90: 795f 666f 726d 6174 35da 0b40 7079 5f66  y_format5..@py_f
-00002da0: 6f72 6d61 7437 da0b 4070 795f 6173 7365  ormat7..@py_asse
-00002db0: 7274 3172 3700 0000 7238 0000 00da 0b40  rt1r7...r8.....@
-00002dc0: 7079 5f61 7373 6572 7439 da0c 4070 795f  py_assert9..@py_
-00002dd0: 6173 7365 7274 3131 5a0c 4070 795f 6173  assert11Z.@py_as
-00002de0: 7365 7274 3133 5a0c 4070 795f 6173 7365  sert13Z.@py_asse
-00002df0: 7274 3135 5a0c 4070 795f 666f 726d 6174  rt15Z.@py_format
-00002e00: 3137 5a0b 6870 315f 7363 616c 6572 735a  17Z.hp1_scalersZ
-00002e10: 0f70 6963 6b6c 6564 5f73 6361 6c65 7273  .pickled_scalers
-00002e20: da0c 4070 795f 666f 726d 6174 3133 7264  ..@py_format13rd
-00002e30: 0000 005a 0e70 6963 6b6c 6564 5f76 616c  ...Z.pickled_val
-00002e40: 7565 7372 3a00 0000 da0b 4070 795f 6173  uesr:.....@py_as
-00002e50: 7365 7274 34da 0b40 7079 5f61 7373 6572  sert4..@py_asser
-00002e60: 7436 da0b 4070 795f 666f 726d 6174 38da  t6..@py_format8.
-00002e70: 0272 745a 026d 7a5a 0969 6e74 656e 7369  .rtZ.mzZ.intensi
-00002e80: 7479 5a09 615f 7363 616c 6572 735a 0c40  tyZ.a_scalersZ.@
-00002e90: 7079 5f61 7373 6572 7431 305a 0c40 7079  py_assert10Z.@py
-00002ea0: 5f61 7373 6572 7431 325a 0c40 7079 5f61  _assert12Z.@py_a
-00002eb0: 7373 6572 7431 345a 0c40 7079 5f66 6f72  ssert14Z.@py_for
-00002ec0: 6d61 7431 365a 0b40 7079 5f61 7373 6572  mat16Z.@py_asser
-00002ed0: 7438 5a0c 4070 795f 666f 726d 6174 3134  t8Z.@py_format14
-00002ee0: 725f 0000 005a 0c40 7079 5f66 6f72 6d61  r_...Z.@py_forma
-00002ef0: 7431 325a 0c40 7079 5f61 7373 6572 7431  t12Z.@py_assert1
-00002f00: 375a 0c40 7079 5f66 6f72 6d61 7431 3972  7Z.@py_format19r
-00002f10: 0500 0000 7205 0000 0072 0600 0000 da16  ....r....r......
-00002f20: 7465 7374 5f61 6c69 676e 6d65 6e74 5f6d  test_alignment_m
-00002f30: 6574 686f 6473 7c00 0000 737c 0200 0000  ethods|...s|....
-00002f40: 0514 0308 010a 000a 0008 0004 002c 000c  .............,..
-00002f50: 000e 000c 010a 000a 0008 0004 002c 000c  .............,..
-00002f60: 000e 000c 0308 0106 000e 0006 000e 0006  ................
-00002f70: 000a 0006 0006 0006 0070 000e 0020 0608  .........p... ..
-00002f80: 010e 010e 0106 000c 000c 000a 0006 0006  ................
-00002f90: 0006 0060 000e 0018 0106 000c 000c 000a  ...`............
-00002fa0: 0006 0006 0006 0060 000e 0018 0106 000c  .......`........
-00002fb0: 000c 000a 0006 0006 0006 0060 000e 0018  ...........`....
-00002fc0: 0106 000c 000c 000a 0006 0006 0006 0060  ...............`
-00002fd0: 000e 0018 0106 000c 000c 000a 0006 0006  ................
-00002fe0: 0006 0060 000e 0018 0306 000c 000c 000a  ...`............
-00002ff0: 0006 0006 0006 0060 000e 0018 0508 010e  .......`........
-00003000: 010e 0106 0008 0008 000a 0006 0006 0006  ................
-00003010: 0060 000e 0018 0106 0008 0008 000a 0006  .`..............
-00003020: 0006 0006 0060 000e 0018 0106 0008 0008  .....`..........
-00003030: 000a 0006 0006 0006 0060 000e 0018 0308  .........`......
-00003040: 0106 0012 0012 000a 0006 0050 000e 0010  ...........P....
-00003050: 0106 0012 0012 000a 0006 0050 000e 0010  ...........P....
-00003060: 0106 0012 0012 000a 0006 0050 000e 0010  ...........P....
-00003070: 0508 010e 0006 000e 0008 0006 002a 000e  .............*..
-00003080: 0010 0314 0108 0318 0118 0118 0214 0104  ................
-00003090: 0202 0102 0016 ff02 ff02 0502 fa06 0808  ................
-000030a0: 010e 0106 000c 0008 000a 0006 0006 0006  ................
-000030b0: 0060 000e 0018 0106 000c 0008 000a 0006  .`..............
-000030c0: 0006 0006 0060 000e 0018 0106 000c 0008  .....`..........
-000030d0: 000a 0006 0006 0006 0060 000e 0018 0106  .........`......
-000030e0: 000c 0008 000a 0006 0006 0006 0060 000e  .............`..
-000030f0: 0018 0106 000c 0008 000a 0006 0006 0006  ................
-00003100: 0060 000e 0018 0106 000c 0008 000a 0006  .`..............
-00003110: 0006 0006 0060 000e 0018 0314 0104 0202  .....`..........
-00003120: 0102 0016 ff02 ff02 0502 fa06 0808 010e  ................
-00003130: 0106 000c 0008 0008 0008 000a 0006 0006  ................
-00003140: 0006 0068 000e 0020 0106 000c 0008 0006  ...h... ........
-00003150: 000a 0006 0006 0006 0060 000e 001c 011c  .........`......
-00003160: 0106 000c 000a 0006 0006 0006 007e 000e  .............~..
-00003170: 0014 0106 000c 0008 0006 0008 0008 0008  ................
-00003180: 000a 0006 0006 0006 008e 000e 0028 0106  .............(..
-00003190: 000c 0008 0008 0008 000a 0006 0006 0006  ................
-000031a0: 0068 000e 0020 0106 000c 0008 0006 000a  .h... ..........
-000031b0: 0006 0006 0006 0060 000e 0072 7400 0000  .......`...rt...
-000031c0: 6300 0000 0000 0000 0000 0000 0005 0000  c...............
-000031d0: 000a 0000 0043 0000 0073 d600 0000 7400  .....C...s....t.
-000031e0: a001 6401 6402 6403 6404 9c03 6405 6406  ..d.d.d.d...d.d.
-000031f0: 6407 6404 9c03 6408 6409 640a 6404 9c03  d.d...d.d.d.d...
-00003200: 6401 6401 6401 6404 9c03 6401 6401 6401  d.d.d.d...d.d.d.
-00003210: 6404 9c03 a105 7d00 7402 6a03 7d01 640b  d.....}.t.j.}.d.
-00003220: 7d02 7c01 7c00 7c02 8302 7d03 7c03 73c6  }.|.|.|...}.|.s.
-00003230: 640c 640d 7404 a005 a100 6b06 736a 7406  d.d.t.....k.sjt.
-00003240: a007 7402 a101 7274 7406 a008 7402 a101  ..t...rtt...t...
-00003250: 6e02 640d 7406 a008 7c01 a101 640e 7404  n.d.t...|...d.t.
-00003260: a005 a100 6b06 7394 7406 a007 7c00 a101  ....k.s.t...|...
-00003270: 729e 7406 a008 7c00 a101 6e02 640e 7406  r.t...|...n.d.t.
-00003280: a008 7c02 a101 7406 a008 7c03 a101 640f  ..|...t...|...d.
-00003290: 9c05 1600 7d04 7409 7406 a00a 7c04 a101  ....}.t.t...|...
-000032a0: 8301 8201 6410 0400 7d01 0400 7d02 7d03  ....d...}...}.}.
-000032b0: 6410 5300 2911 7a20 0a20 2020 2054 6573  d.S.).z .    Tes
-000032c0: 7420 7363 6f72 6520 6361 6c63 756c 6174  t score calculat
-000032d0: 696f 6e0a 2020 2020 7253 0000 0072 5700  ion.    rS...rW.
-000032e0: 0000 7256 0000 0072 5a00 0000 7254 0000  ..rV...rZ...rT..
-000032f0: 0067 b22e 6ea3 0100 6940 69e8 0300 00da  .g..n...i@i.....
-00003300: 066c 696e 6561 725a 0370 706d da05 6c6f  .linearZ.ppm..lo
-00003310: 6731 3072 5500 0000 7a52 6173 7365 7274  g10rU...zRassert
-00003320: 2025 2870 7937 2973 0a7b 2528 7079 3729   %(py7)s.{%(py7)
-00003330: 7320 3d20 2528 7079 3229 730a 7b25 2870  s = %(py2)s.{%(p
-00003340: 7932 2973 203d 2025 2870 7930 2973 2e69  y2)s = %(py0)s.i
-00003350: 7363 6c6f 7365 0a7d 2825 2870 7933 2973  sclose.}(%(py3)s
-00003360: 2c20 2528 7079 3529 7329 0a7d 7244 0000  , %(py5)s).}rD..
-00003370: 00da 0573 636f 7265 2905 7245 0000 0072  ...score).rE...r
-00003380: 4600 0000 7220 0000 0072 5100 0000 7252  F...r ...rQ...rR
-00003390: 0000 004e 290b 7228 0000 005a 0a63 616c  ...N).r(...Z.cal
-000033a0: 635f 7363 6f72 6572 4400 0000 7263 0000  c_scorerD...rc..
-000033b0: 0072 3100 0000 7232 0000 0072 2e00 0000  .r1...r2...r....
-000033c0: 7233 0000 0072 3000 0000 7234 0000 0072  r3...r0...r4...r
-000033d0: 3500 0000 2905 7277 0000 0072 6c00 0000  5...).rw...rl...
-000033e0: 7270 0000 0072 7100 0000 7272 0000 0072  rp...rq...rr...r
-000033f0: 0500 0000 7205 0000 0072 0600 0000 da0f  ....r....r......
-00003400: 7465 7374 5f63 616c 635f 7363 6f72 65e2  test_calc_score.
-00003410: 0000 0073 1c00 0000 0004 0401 0a01 0a01  ...s............
-00003420: 0a01 0a01 0afb 0407 0600 0400 0a00 0400  ................
-00003430: 6600 0e00 7278 0000 007a 1469 676e 6f72  f...rx...z.ignor
-00003440: 653a 696e 7661 6c69 6420 7661 6c75 6563  e:invalid valuec
-00003450: 0000 0000 0000 0000 0000 0000 0600 0000  ................
-00003460: 0900 0000 4300 0000 73c6 0000 0074 006a  ....C...s....t.j
-00003470: 017d 0074 026a 0374 00a0 0464 0164 0164  .}.t.j.t...d.d.d
-00003480: 0267 03a1 0174 00a0 0464 0264 0264 0367  .g...t...d.d.d.g
-00003490: 03a1 0164 0464 0564 068d 0464 0219 007d  ...d.d.d...d...}
-000034a0: 017c 007c 0183 017d 027c 026a 057d 037c  .|.|...}.|.j.}.|
-000034b0: 0383 007d 047c 0473 ae64 0764 0874 06a0  ...}.|.s.d.d.t..
-000034c0: 07a1 006b 0673 6474 08a0 0974 00a1 0172  ...k.sdt...t...r
-000034d0: 6e74 08a0 0a74 00a1 016e 0264 0874 08a0  nt...t...n.d.t..
-000034e0: 0a7c 00a1 0174 08a0 0a7c 01a1 0174 08a0  .|...t...|...t..
-000034f0: 0a7c 02a1 0174 08a0 0a7c 03a1 0174 08a0  .|...t...|...t..
-00003500: 0a7c 04a1 0164 099c 0616 007d 0574 0b74  .|...d.....}.t.t
-00003510: 08a0 0c7c 05a1 0183 0182 0164 0a04 007d  ...|.......d...}
-00003520: 0004 007d 0104 007d 0204 007d 037d 0464  ...}...}...}.}.d
-00003530: 0a53 0029 0b7a 330a 2020 2020 5375 7070  .S.).z3.    Supp
-00003540: 6c65 6d65 6e74 616c 2074 6573 7473 2074  lemental tests t
-00003550: 6f20 6361 6c63 756c 6174 696e 6720 7363  o calculating sc
-00003560: 616c 6572 730a 2020 2020 7201 0000 0072  alers.    r....r
-00003570: 5300 0000 7254 0000 005a 066c 6f77 6573  S...rT...Z.lowes
-00003580: 7372 7500 0000 2902 5a09 736d 6f6f 7468  sru...).Z.smooth
-00003590: 696e 67da 046d 6f64 657a 7961 7373 6572  ing..modezyasser
-000035a0: 7420 2528 7079 3130 2973 0a7b 2528 7079  t %(py10)s.{%(py
-000035b0: 3130 2973 203d 2025 2870 7938 2973 0a7b  10)s = %(py8)s.{
-000035c0: 2528 7079 3829 7320 3d20 2528 7079 3629  %(py8)s = %(py6)
-000035d0: 730a 7b25 2870 7936 2973 203d 2025 2870  s.{%(py6)s = %(p
-000035e0: 7932 2973 0a7b 2528 7079 3229 7320 3d20  y2)s.{%(py2)s = 
-000035f0: 2528 7079 3029 732e 6973 6e61 6e0a 7d28  %(py0)s.isnan.}(
-00003600: 2528 7079 3429 7329 0a7d 2e61 6c6c 0a7d  %(py4)s).}.all.}
-00003610: 2829 0a7d 7244 0000 0029 0672 4500 0000  ().}rD...).rE...
-00003620: 7246 0000 0072 2100 0000 7222 0000 0072  rF...r!...r"...r
-00003630: 2300 0000 7225 0000 004e 290d 7244 0000  #...r%...N).rD..
-00003640: 00da 0569 736e 616e 7228 0000 0072 6700  ...isnanr(...rg.
-00003650: 0000 da05 6172 7261 7972 6200 0000 7231  ....arrayrb...r1
-00003660: 0000 0072 3200 0000 722e 0000 0072 3300  ...r2...r....r3.
-00003670: 0000 7230 0000 0072 3400 0000 7235 0000  ..r0...r4...r5..
-00003680: 0029 0672 6c00 0000 7269 0000 0072 3700  .).rl...ri...r7.
-00003690: 0000 7238 0000 0072 6d00 0000 723b 0000  ..r8...rm...r;..
-000036a0: 0072 0500 0000 7205 0000 0072 0600 0000  .r....r....r....
-000036b0: da11 7465 7374 5f63 616c 635f 7363 616c  ..test_calc_scal
-000036c0: 6572 73f0 0000 0073 1200 0000 0007 0600  ers....s........
-000036d0: 2e00 0800 0600 0600 0400 5400 0e00 727c  ..........T...r|
-000036e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000036f0: 0a00 0000 0a00 0000 4300 0000 73dc 0000  ........C...s...
-00003700: 007c 006a 0064 0164 028d 017d 0174 01a0  .|.j.d.d...}.t..
-00003710: 02a1 007d 027c 02a0 037c 0164 03a1 0201  ...}.|...|.d....
-00003720: 0074 046a 057d 037c 026a 0664 0319 0064  .t.j.}.|.j.d...d
-00003730: 0119 007d 047c 0064 0119 007d 057c 037c  ...}.|.d...}.|.|
-00003740: 047c 0583 027d 067c 066a 077d 077c 0783  .|...}.|.j.}.|..
-00003750: 007d 087c 0873 c064 0464 0574 08a0 09a1  .}.|.s.d.d.t....
-00003760: 006b 0673 6e74 0aa0 0b74 04a1 0172 7874  .k.snt...t...rxt
-00003770: 0aa0 0c74 04a1 016e 0264 0574 0aa0 0c7c  ...t...n.d.t...|
-00003780: 03a1 0174 0aa0 0c7c 04a1 0174 0aa0 0c7c  ...t...|...t...|
-00003790: 05a1 0174 0aa0 0c7c 06a1 0174 0aa0 0c7c  ...t...|...t...|
-000037a0: 07a1 0174 0aa0 0c7c 08a1 0164 069c 0716  ...t...|...d....
-000037b0: 007d 0974 0d74 0aa0 0e7c 09a1 0183 0182  .}.t.t...|......
-000037c0: 0164 0704 007d 0304 007d 0404 007d 0504  .d...}...}...}..
-000037d0: 007d 0604 007d 077d 0864 0753 0029 087a  .}...}.}.d.S.).z
-000037e0: 420a 2020 2020 5465 7374 7320 746f 2073  B.    Tests to s
-000037f0: 6565 2069 6620 696e 7465 6e73 6974 7920  ee if intensity 
-00003800: 6973 2061 7574 6f63 616c 6375 6c61 7465  is autocalculate
-00003810: 6420 7768 656e 206d 6973 7369 6e67 0a20  d when missing. 
-00003820: 2020 2072 5000 0000 2901 da07 636f 6c75     rP...)...colu
-00003830: 6d6e 735a 0364 6633 724c 0000 0072 4400  mnsZ.df3rL...rD.
-00003840: 0000 724d 0000 004e 290f 5a04 6472 6f70  ..rM...N).Z.drop
-00003850: 7228 0000 0072 2900 0000 723d 0000 0072  r(...r)...r=...r
-00003860: 4400 0000 7263 0000 005a 0864 6174 6173  D...rc...Z.datas
-00003870: 6574 7372 6200 0000 7231 0000 0072 3200  etsrb...r1...r2.
-00003880: 0000 722e 0000 0072 3300 0000 7230 0000  ..r....r3...r0..
-00003890: 0072 3400 0000 7235 0000 0029 0a72 0e00  .r4...r5...).r..
-000038a0: 0000 5a11 6466 5f33 5f6e 6f5f 696e 7465  ..Z.df_3_no_inte
-000038b0: 6e73 6974 7972 3e00 0000 726c 0000 0072  nsityr>...rl...r
-000038c0: 6900 0000 7237 0000 0072 3800 0000 726d  i...r7...r8...rm
-000038d0: 0000 0072 6e00 0000 726f 0000 0072 0500  ...rn...ro...r..
-000038e0: 0000 7205 0000 0072 0600 0000 da1c 7465  ..r....r......te
-000038f0: 7374 5f61 6464 696e 675f 696e 7465 6e73  st_adding_intens
-00003900: 6974 795f 636f 6c75 6d6e fe00 0000 731a  ity_column....s.
-00003910: 0000 0000 050c 0208 010c 0206 000e 0008  ................
-00003920: 000a 0006 0006 0004 005c 000e 0072 7e00  .........\...r~.
-00003930: 0000 6303 0000 0000 0000 0000 0000 0010  ..c.............
-00003940: 0000 0008 0000 0043 0000 0073 1009 0000  .......C...s....
-00003950: 6401 6402 6403 6703 7d03 7400 6a01 7c00  d.d.d.g.}.t.j.|.
-00003960: 7c01 7c02 7c03 6404 8d04 7d04 7c04 a002  |.|.|.d...}.|...
-00003970: a100 0100 7c04 6a03 7d05 7404 7c05 8301  ....|.j.}.t.|...
-00003980: 7d06 6401 6402 6403 6703 7d07 7c06 7c07  }.d.d.d.g.}.|.|.
-00003990: 6b02 7d08 7c08 73da 7405 a006 6405 7c08  k.}.|.s.t...d.|.
-000039a0: 6601 6406 7c06 7c07 6602 a104 6407 7407  f.d.|.|.f...d.t.
-000039b0: a008 a100 6b06 7372 7405 a009 7404 a101  ....k.srt...t...
-000039c0: 727c 7405 a00a 7404 a101 6e02 6407 6408  r|t...t...n.d.d.
-000039d0: 7407 a008 a100 6b06 7394 7405 a009 7c04  t.....k.s.t...|.
-000039e0: a101 729e 7405 a00a 7c04 a101 6e02 6408  ..r.t...|...n.d.
-000039f0: 7405 a00a 7c05 a101 7405 a00a 7c06 a101  t...|...t...|...
-00003a00: 7405 a00a 7c07 a101 6409 9c05 1600 7d09  t...|...d.....}.
-00003a10: 640a 640b 7c09 6901 1600 7d0a 740b 7405  d.d.|.i...}.t.t.
-00003a20: a00c 7c0a a101 8301 8201 640c 0400 7d05  ..|.......d...}.
-00003a30: 0400 7d06 0400 7d08 7d07 7c04 6a03 6401  ..}...}.}.|.j.d.
-00003a40: 1900 7d0b 7404 7c0b 8301 7d0c 6402 6403  ..}.t.|...}.d.d.
-00003a50: 6702 7d08 7c0c 7c08 6b02 7d0d 7c0d 9001  g.}.|.|.k.}.|...
-00003a60: 7386 7405 a006 6405 7c0d 6601 640d 7c0c  s.t...d.|.f.d.|.
-00003a70: 7c08 6602 a104 6407 7407 a008 a100 6b06  |.f...d.t.....k.
-00003a80: 9001 7340 7405 a009 7404 a101 9001 724a  ..s@t...t.....rJ
-00003a90: 7405 a00a 7404 a101 6e02 6407 7405 a00a  t...t...n.d.t...
-00003aa0: 7c0b a101 7405 a00a 7c0c a101 7405 a00a  |...t...|...t...
-00003ab0: 7c08 a101 640e 9c04 1600 7d0e 640f 6410  |...d.....}.d.d.
-00003ac0: 7c0e 6901 1600 7d0f 740b 7405 a00c 7c0f  |.i...}.t.t...|.
-00003ad0: a101 8301 8201 640c 0400 7d0b 0400 7d0c  ......d...}...}.
-00003ae0: 0400 7d0d 7d08 7c04 6a03 6402 1900 7d0b  ..}.}.|.j.d...}.
-00003af0: 7404 7c0b 8301 7d0c 6401 6403 6702 7d08  t.|...}.d.d.g.}.
-00003b00: 7c0c 7c08 6b02 7d0d 7c0d 9002 7332 7405  |.|.k.}.|...s2t.
-00003b10: a006 6405 7c0d 6601 640d 7c0c 7c08 6602  ..d.|.f.d.|.|.f.
-00003b20: a104 6407 7407 a008 a100 6b06 9001 73ec  ..d.t.....k...s.
-00003b30: 7405 a009 7404 a101 9001 72f6 7405 a00a  t...t.....r.t...
-00003b40: 7404 a101 6e02 6407 7405 a00a 7c0b a101  t...n.d.t...|...
-00003b50: 7405 a00a 7c0c a101 7405 a00a 7c08 a101  t...|...t...|...
-00003b60: 640e 9c04 1600 7d0e 640f 6410 7c0e 6901  d.....}.d.d.|.i.
-00003b70: 1600 7d0f 740b 7405 a00c 7c0f a101 8301  ..}.t.t...|.....
-00003b80: 8201 640c 0400 7d0b 0400 7d0c 0400 7d0d  ..d...}...}...}.
-00003b90: 7d08 7c04 6a03 6403 1900 7d0b 7404 7c0b  }.|.j.d...}.t.|.
-00003ba0: 8301 7d0c 6401 6402 6702 7d08 7c0c 7c08  ..}.d.d.g.}.|.|.
-00003bb0: 6b02 7d0d 7c0d 9002 73de 7405 a006 6405  k.}.|...s.t...d.
-00003bc0: 7c0d 6601 640d 7c0c 7c08 6602 a104 6407  |.f.d.|.|.f...d.
-00003bd0: 7407 a008 a100 6b06 9002 7398 7405 a009  t.....k...s.t...
-00003be0: 7404 a101 9002 72a2 7405 a00a 7404 a101  t.....r.t...t...
-00003bf0: 6e02 6407 7405 a00a 7c0b a101 7405 a00a  n.d.t...|...t...
-00003c00: 7c0c a101 7405 a00a 7c08 a101 640e 9c04  |...t...|...d...
-00003c10: 1600 7d0e 640f 6410 7c0e 6901 1600 7d0f  ..}.d.d.|.i...}.
-00003c20: 740b 7405 a00c 7c0f a101 8301 8201 640c  t.t...|.......d.
-00003c30: 0400 7d0b 0400 7d0c 0400 7d0d 7d08 7400  ..}...}...}.}.t.
-00003c40: 6a01 7c00 7c01 7c02 7c03 6404 8d04 7d04  j.|.|.|.|.d...}.
-00003c50: 7c04 a002 6401 6402 6403 6703 a101 0100  |...d.d.d.g.....
-00003c60: 7c04 6a03 7d05 7404 7c05 8301 7d06 6401  |.j.}.t.|...}.d.
-00003c70: 6402 6403 6703 7d07 7c06 7c07 6b02 7d08  d.d.g.}.|.|.k.}.
-00003c80: 7c08 9003 73d0 7405 a006 6405 7c08 6601  |...s.t...d.|.f.
-00003c90: 6406 7c06 7c07 6602 a104 6407 7407 a008  d.|.|.f...d.t...
-00003ca0: a100 6b06 9003 7364 7405 a009 7404 a101  ..k...sdt...t...
-00003cb0: 9003 726e 7405 a00a 7404 a101 6e02 6407  ..rnt...t...n.d.
-00003cc0: 6408 7407 a008 a100 6b06 9003 738a 7405  d.t.....k...s.t.
-00003cd0: a009 7c04 a101 9003 7294 7405 a00a 7c04  ..|.....r.t...|.
-00003ce0: a101 6e02 6408 7405 a00a 7c05 a101 7405  ..n.d.t...|...t.
-00003cf0: a00a 7c06 a101 7405 a00a 7c07 a101 6409  ..|...t...|...d.
-00003d00: 9c05 1600 7d09 640a 640b 7c09 6901 1600  ....}.d.d.|.i...
-00003d10: 7d0a 740b 7405 a00c 7c0a a101 8301 8201  }.t.t...|.......
-00003d20: 640c 0400 7d05 0400 7d06 0400 7d08 7d07  d...}...}...}.}.
-00003d30: 7c04 6a03 6401 1900 7d0b 7404 7c0b 8301  |.j.d...}.t.|...
-00003d40: 7d0c 6402 6403 6702 7d08 7c0c 7c08 6b02  }.d.d.g.}.|.|.k.
-00003d50: 7d0d 7c0d 9004 737c 7405 a006 6405 7c0d  }.|...s|t...d.|.
-00003d60: 6601 640d 7c0c 7c08 6602 a104 6407 7407  f.d.|.|.f...d.t.
-00003d70: a008 a100 6b06 9004 7336 7405 a009 7404  ....k...s6t...t.
-00003d80: a101 9004 7240 7405 a00a 7404 a101 6e02  ....r@t...t...n.
-00003d90: 6407 7405 a00a 7c0b a101 7405 a00a 7c0c  d.t...|...t...|.
-00003da0: a101 7405 a00a 7c08 a101 640e 9c04 1600  ..t...|...d.....
-00003db0: 7d0e 640f 6410 7c0e 6901 1600 7d0f 740b  }.d.d.|.i...}.t.
-00003dc0: 7405 a00c 7c0f a101 8301 8201 640c 0400  t...|.......d...
-00003dd0: 7d0b 0400 7d0c 0400 7d0d 7d08 7c04 6a03  }...}...}.}.|.j.
-00003de0: 6402 1900 7d0b 7404 7c0b 8301 7d0c 6401  d...}.t.|...}.d.
-00003df0: 6403 6702 7d08 7c0c 7c08 6b02 7d0d 7c0d  d.g.}.|.|.k.}.|.
-00003e00: 9005 7328 7405 a006 6405 7c0d 6601 640d  ..s(t...d.|.f.d.
-00003e10: 7c0c 7c08 6602 a104 6407 7407 a008 a100  |.|.f...d.t.....
-00003e20: 6b06 9004 73e2 7405 a009 7404 a101 9004  k...s.t...t.....
-00003e30: 72ec 7405 a00a 7404 a101 6e02 6407 7405  r.t...t...n.d.t.
-00003e40: a00a 7c0b a101 7405 a00a 7c0c a101 7405  ..|...t...|...t.
-00003e50: a00a 7c08 a101 640e 9c04 1600 7d0e 640f  ..|...d.....}.d.
-00003e60: 6410 7c0e 6901 1600 7d0f 740b 7405 a00c  d.|.i...}.t.t...
-00003e70: 7c0f a101 8301 8201 640c 0400 7d0b 0400  |.......d...}...
-00003e80: 7d0c 0400 7d0d 7d08 7c04 6a03 6403 1900  }...}.}.|.j.d...
-00003e90: 7d0b 7404 7c0b 8301 7d0c 6401 6402 6702  }.t.|...}.d.d.g.
-00003ea0: 7d08 7c0c 7c08 6b02 7d0d 7c0d 9005 73d4  }.|.|.k.}.|...s.
-00003eb0: 7405 a006 6405 7c0d 6601 640d 7c0c 7c08  t...d.|.f.d.|.|.
-00003ec0: 6602 a104 6407 7407 a008 a100 6b06 9005  f...d.t.....k...
-00003ed0: 738e 7405 a009 7404 a101 9005 7298 7405  s.t...t.....r.t.
-00003ee0: a00a 7404 a101 6e02 6407 7405 a00a 7c0b  ..t...n.d.t...|.
-00003ef0: a101 7405 a00a 7c0c a101 7405 a00a 7c08  ..t...|...t...|.
-00003f00: a101 640e 9c04 1600 7d0e 640f 6410 7c0e  ..d.....}.d.d.|.
-00003f10: 6901 1600 7d0f 740b 7405 a00c 7c0f a101  i...}.t.t...|...
-00003f20: 8301 8201 640c 0400 7d0b 0400 7d0c 0400  ....d...}...}...
-00003f30: 7d0d 7d08 7400 6a01 7c00 7c01 7c02 7c03  }.}.t.j.|.|.|.|.
-00003f40: 6404 8d04 7d04 7c04 a002 6401 a101 0100  d...}.|...d.....
-00003f50: 7c04 6a03 7d05 7404 7c05 8301 7d06 6401  |.j.}.t.|...}.d.
-00003f60: 6701 7d07 7c06 7c07 6b02 7d08 7c08 9006  g.}.|.|.k.}.|...
-00003f70: 73bc 7405 a006 6405 7c08 6601 6406 7c06  s.t...d.|.f.d.|.
-00003f80: 7c07 6602 a104 6407 7407 a008 a100 6b06  |.f...d.t.....k.
-00003f90: 9006 7350 7405 a009 7404 a101 9006 725a  ..sPt...t.....rZ
-00003fa0: 7405 a00a 7404 a101 6e02 6407 6408 7407  t...t...n.d.d.t.
-00003fb0: a008 a100 6b06 9006 7376 7405 a009 7c04  ....k...svt...|.
-00003fc0: a101 9006 7280 7405 a00a 7c04 a101 6e02  ....r.t...|...n.
-00003fd0: 6408 7405 a00a 7c05 a101 7405 a00a 7c06  d.t...|...t...|.
-00003fe0: a101 7405 a00a 7c07 a101 6409 9c05 1600  ..t...|...d.....
-00003ff0: 7d09 640a 640b 7c09 6901 1600 7d0a 740b  }.d.d.|.i...}.t.
-00004000: 7405 a00c 7c0a a101 8301 8201 640c 0400  t...|.......d...
-00004010: 7d05 0400 7d06 0400 7d08 7d07 7c04 6a03  }...}...}.}.|.j.
-00004020: 6401 1900 7d0b 7404 7c0b 8301 7d0c 6402  d...}.t.|...}.d.
-00004030: 6403 6702 7d08 7c0c 7c08 6b02 7d0d 7c0d  d.g.}.|.|.k.}.|.
-00004040: 9007 7368 7405 a006 6405 7c0d 6601 640d  ..sht...d.|.f.d.
-00004050: 7c0c 7c08 6602 a104 6407 7407 a008 a100  |.|.f...d.t.....
-00004060: 6b06 9007 7322 7405 a009 7404 a101 9007  k...s"t...t.....
-00004070: 722c 7405 a00a 7404 a101 6e02 6407 7405  r,t...t...n.d.t.
-00004080: a00a 7c0b a101 7405 a00a 7c0c a101 7405  ..|...t...|...t.
-00004090: a00a 7c08 a101 640e 9c04 1600 7d0e 640f  ..|...d.....}.d.
-000040a0: 6410 7c0e 6901 1600 7d0f 740b 7405 a00c  d.|.i...}.t.t...
-000040b0: 7c0f a101 8301 8201 640c 0400 7d0b 0400  |.......d...}...
-000040c0: 7d0c 0400 7d0d 7d08 7400 6a01 7c00 7c01  }...}.}.t.j.|.|.
-000040d0: 7c02 7c03 6404 8d04 7d04 7c04 a002 6401  |.|.d...}.|...d.
-000040e0: 6402 a102 0100 7c04 6a03 7d05 7404 7c05  d.....|.j.}.t.|.
-000040f0: 8301 7d06 6401 6701 7d07 7c06 7c07 6b02  ..}.d.g.}.|.|.k.
-00004100: 7d08 7c08 9008 7352 7405 a006 6405 7c08  }.|...sRt...d.|.
-00004110: 6601 6406 7c06 7c07 6602 a104 6407 7407  f.d.|.|.f...d.t.
-00004120: a008 a100 6b06 9007 73e6 7405 a009 7404  ....k...s.t...t.
-00004130: a101 9007 72f0 7405 a00a 7404 a101 6e02  ....r.t...t...n.
-00004140: 6407 6408 7407 a008 a100 6b06 9008 730c  d.d.t.....k...s.
-00004150: 7405 a009 7c04 a101 9008 7216 7405 a00a  t...|.....r.t...
-00004160: 7c04 a101 6e02 6408 7405 a00a 7c05 a101  |...n.d.t...|...
-00004170: 7405 a00a 7c06 a101 7405 a00a 7c07 a101  t...|...t...|...
-00004180: 6409 9c05 1600 7d09 640a 640b 7c09 6901  d.....}.d.d.|.i.
-00004190: 1600 7d0a 740b 7405 a00c 7c0a a101 8301  ..}.t.t...|.....
-000041a0: 8201 640c 0400 7d05 0400 7d06 0400 7d08  ..d...}...}...}.
-000041b0: 7d07 7c04 6a03 6401 1900 7d0b 7404 7c0b  }.|.j.d...}.t.|.
-000041c0: 8301 7d0c 6402 6701 7d08 7c0c 7c08 6b02  ..}.d.g.}.|.|.k.
-000041d0: 7d0d 7c0d 9008 73fc 7405 a006 6405 7c0d  }.|...s.t...d.|.
-000041e0: 6601 640d 7c0c 7c08 6602 a104 6407 7407  f.d.|.|.f...d.t.
-000041f0: a008 a100 6b06 9008 73b6 7405 a009 7404  ....k...s.t...t.
-00004200: a101 9008 72c0 7405 a00a 7404 a101 6e02  ....r.t...t...n.
-00004210: 6407 7405 a00a 7c0b a101 7405 a00a 7c0c  d.t...|...t...|.
-00004220: a101 7405 a00a 7c08 a101 640e 9c04 1600  ..t...|...d.....
-00004230: 7d0e 640f 6410 7c0e 6901 1600 7d0f 740b  }.d.d.|.i...}.t.
-00004240: 7405 a00c 7c0f a101 8301 8201 640c 0400  t...|.......d...
-00004250: 7d0b 0400 7d0c 0400 7d0d 7d08 640c 5300  }...}...}.}.d.S.
-00004260: 2911 7a52 0a20 2020 2054 6573 7473 2074  ).zR.    Tests t
-00004270: 6865 2077 7261 7070 6572 7320 7768 6963  he wrappers whic
-00004280: 6820 636f 6e74 726f 6c20 7468 6520 696e  h control the in
-00004290: 6e65 7220 616e 6420 6f75 7465 7220 6461  ner and outer da
-000042a0: 7461 6672 616d 6520 666f 7220 6c6f 6f70  taframe for loop
-000042b0: 730a 2020 2020 7240 0000 0072 4100 0000  s.    r@...rA...
-000042c0: 5a03 4850 3372 1600 0000 7242 0000 0029  Z.HP3r....rB...)
-000042d0: 017a 4d25 2870 7935 2973 0a7b 2528 7079  .zM%(py5)s.{%(py
-000042e0: 3529 7320 3d20 2528 7079 3029 7328 2528  5)s = %(py0)s(%(
-000042f0: 7079 3329 730a 7b25 2870 7933 2973 203d  py3)s.{%(py3)s =
-00004300: 2025 2870 7931 2973 2e6d 6174 6368 6573   %(py1)s.matches
-00004310: 0a7d 290a 7d20 3d3d 2025 2870 7938 2973  .}).} == %(py8)s
-00004320: da04 6c69 7374 723e 0000 0029 0572 4500  ..listr>...).rE.
-00004330: 0000 721f 0000 0072 2000 0000 7251 0000  ..r....r ...rQ..
-00004340: 0072 2300 0000 7224 0000 0072 2500 0000  .r#...r$...r%...
-00004350: 4e29 017a 3025 2870 7934 2973 0a7b 2528  N).z0%(py4)s.{%(
-00004360: 7079 3429 7320 3d20 2528 7079 3029 7328  py4)s = %(py0)s(
-00004370: 2528 7079 3229 7329 0a7d 203d 3d20 2528  %(py2)s).} == %(
-00004380: 7079 3729 7329 0472 4500 0000 7246 0000  py7)s).rE...rF..
-00004390: 0072 2100 0000 7252 0000 007a 0e61 7373  .r!...rR...z.ass
-000043a0: 6572 7420 2528 7079 3929 7372 5e00 0000  ert %(py9)sr^...
-000043b0: 290d 7228 0000 0072 2900 0000 7266 0000  ).r(...r)...rf..
-000043c0: 0072 6500 0000 727f 0000 0072 2e00 0000  .re...r....r....
-000043d0: 722f 0000 0072 3100 0000 7232 0000 0072  r/...r1...r2...r
-000043e0: 3300 0000 7230 0000 0072 3400 0000 7235  3...r0...r4...r5
-000043f0: 0000 0029 1072 0c00 0000 720d 0000 0072  ...).r....r....r
-00004400: 0e00 0000 7217 0000 0072 3e00 0000 7239  ....r....r>...r9
-00004410: 0000 0072 7000 0000 7238 0000 0072 7100  ...rp...r8...rq.
-00004420: 0000 723a 0000 0072 3b00 0000 726c 0000  ..r:...r;...rl..
-00004430: 0072 6900 0000 7237 0000 0072 7200 0000  .ri...r7...rr...
-00004440: 5a0c 4070 795f 666f 726d 6174 3130 7205  Z.@py_format10r.
-00004450: 0000 0072 0500 0000 7206 0000 00da 1674  ...r....r......t
-00004460: 6573 745f 6461 7461 7365 745f 7365 6c65  est_dataset_sele
-00004470: 6374 696f 6e0b 0100 0073 ea00 0000 0005  ction....s......
-00004480: 0a01 1201 0801 0600 0800 0a00 0800 0400  ................
-00004490: 7800 0c00 0e00 1001 0a00 0800 0800 0800  x...............
-000044a0: 0600 5a00 0c00 0e00 1001 0a00 0800 0800  ..Z.............
-000044b0: 0800 0600 5a00 0c00 0e00 1001 0a00 0800  ....Z...........
-000044c0: 0800 0800 0600 5a00 0c00 0e00 1003 1201  ......Z.........
-000044d0: 1001 0600 0800 0a00 0800 0600 8000 0c00  ................
-000044e0: 0e00 1001 0a00 0800 0800 0800 0600 5a00  ..............Z.
-000044f0: 0c00 0e00 1001 0a00 0800 0800 0800 0600  ................
-00004500: 5a00 0c00 0e00 1001 0a00 0800 0800 0800  Z...............
-00004510: 0600 5a00 0c00 0e00 1003 1201 0a01 0600  ..Z.............
-00004520: 0800 0600 0800 0600 8000 0c00 0e00 1001  ................
-00004530: 0a00 0800 0800 0800 0600 5a00 0c00 0e00  ..........Z.....
-00004540: 1003 1201 0c01 0600 0800 0600 0800 0600  ................
-00004550: 8000 0c00 0e00 1001 0a00 0800 0600 0800  ................
-00004560: 0600 5a00 0c00 0e00 7280 0000 0029 23da  ..Z.....r....)#.
-00004570: 075f 5f64 6f63 5f5f da08 6275 696c 7469  .__doc__..builti
-00004580: 6e73 7231 0000 00da 195f 7079 7465 7374  nsr1....._pytest
-00004590: 2e61 7373 6572 7469 6f6e 2e72 6577 7269  .assertion.rewri
-000045a0: 7465 da09 6173 7365 7274 696f 6eda 0772  te..assertion..r
-000045b0: 6577 7269 7465 722e 0000 0072 0300 0000  ewriter....r....
-000045c0: da03 7379 7372 1000 0000 722a 0000 00da  ..sysr....r*....
-000045d0: 056e 756d 7079 7244 0000 005a 0670 616e  .numpyrD...Z.pan
-000045e0: 6461 7372 0b00 0000 5a0c 626d 7870 2e65  dasr....Z.bmxp.e
-000045f0: 636c 6970 7365 da07 6563 6c69 7073 6572  clipse..eclipser
-00004600: 2800 0000 da07 6669 7874 7572 6572 0700  (.....fixturer..
-00004610: 0000 7208 0000 0072 0900 0000 720c 0000  ..r....r....r...
-00004620: 0072 0d00 0000 720e 0000 0072 1300 0000  .r....r....r....
-00004630: 723c 0000 0072 3f00 0000 7274 0000 0072  r<...r?...rt...r
-00004640: 7800 0000 da04 6d61 726b da0e 6669 6c74  x.....mark..filt
-00004650: 6572 7761 726e 696e 6773 727c 0000 0072  erwarningsr|...r
-00004660: 7e00 0000 7280 0000 0072 0500 0000 7205  ~...r....r....r.
-00004670: 0000 0072 0500 0000 7206 0000 00da 083c  ...r....r......<
-00004680: 6d6f 6475 6c65 3e02 0000 0073 3e00 0000  module>....s>...
-00004690: 0403 0800 1200 0801 0801 0801 0801 0801  ................
-000046a0: 0801 0c03 0601 0a08 0601 0a07 0601 0a07  ................
-000046b0: 0601 0a07 0601 0a07 0601 0a07 0601 0a09  ................
-000046c0: 081b 0818 0866 080e 0a01 0a0d 080d       .....f........
+000001b0: 0a20 2020 207a 0974 6573 7431 2e63 7376  .    z.test1.csv
+000001c0: a903 7202 0000 00da 085f 5f66 696c 655f  ..r......__file_
+000001d0: 5fda 0670 6172 656e 74a9 0072 0600 0000  _..parent..r....
+000001e0: 7206 0000 00fa 3b43 3a5c 5573 6572 735c  r.....;C:\Users\
+000001f0: 6461 6e69 655c 5079 6368 6172 6d50 726f  danie\PycharmPro
+00000200: 6a65 6374 735c 626d 7870 5c74 6573 7473  jects\bmxp\tests
+00000210: 5c74 6573 745f 6d73 6563 6c69 7073 652e  \test_mseclipse.
+00000220: 7079 da0a 6669 6c65 7061 7468 5f31 0d00  py..filepath_1..
+00000230: 0000 7302 0000 0000 0572 0800 0000 6300  ..s......r....c.
+00000240: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00000250: 0000 0043 0000 0073 0e00 0000 7400 7401  ...C...s....t.t.
+00000260: 8301 6a02 6401 1b00 5300 2902 7a23 0a20  ..j.d...S.).z#. 
+00000270: 2020 2053 6563 6f6e 6420 6669 6c65 2070     Second file p
+00000280: 6174 6820 666f 7220 7465 7374 0a20 2020  ath for test.   
+00000290: 207a 0974 6573 7432 2e63 7376 7203 0000   z.test2.csvr...
+000002a0: 0072 0600 0000 7206 0000 0072 0600 0000  .r....r....r....
+000002b0: 7207 0000 00da 0a66 696c 6570 6174 685f  r......filepath_
+000002c0: 3215 0000 0073 0200 0000 0005 7209 0000  2....s......r...
+000002d0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000002e0: 0000 0200 0000 4300 0000 730e 0000 0074  ......C...s....t
+000002f0: 0074 0183 016a 0264 011b 0053 0029 027a  .t...j.d...S.).z
+00000300: 220a 2020 2020 5468 6972 6420 6669 6c65  ".    Third file
+00000310: 2070 6174 6820 666f 7220 7465 7374 0a20   path for test. 
+00000320: 2020 207a 0974 6573 7433 2e63 7376 7203     z.test3.csvr.
+00000330: 0000 0072 0600 0000 7206 0000 0072 0600  ...r....r....r..
+00000340: 0000 7207 0000 00da 0a66 696c 6570 6174  ..r......filepat
+00000350: 685f 331d 0000 0073 0200 0000 0005 720a  h_3....s......r.
+00000360: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000370: 0100 0000 0300 0000 4300 0000 730a 0000  ........C...s...
+00000380: 0074 00a0 017c 00a1 0153 0029 017a 220a  .t...|...S.).z".
+00000390: 2020 2020 4669 7273 7420 6461 7461 6672      First datafr
+000003a0: 616d 6520 666f 7220 7465 7374 0a20 2020  ame for test.   
+000003b0: 20a9 02da 0270 64da 0872 6561 645f 6373   ....pd..read_cs
+000003c0: 7629 0172 0800 0000 7206 0000 0072 0600  v).r....r....r..
+000003d0: 0000 7207 0000 00da 0b64 6174 6166 7261  ..r......datafra
+000003e0: 6d65 5f31 2500 0000 7302 0000 0000 0572  me_1%...s......r
+000003f0: 0e00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000400: 0001 0000 0003 0000 0043 0000 0073 0a00  .........C...s..
+00000410: 0000 7400 a001 7c00 a101 5300 2901 7a23  ..t...|...S.).z#
+00000420: 0a20 2020 2053 6563 6f6e 6420 6461 7461  .    Second data
+00000430: 6672 616d 6520 666f 7220 7465 7374 0a20  frame for test. 
+00000440: 2020 2072 0b00 0000 2901 7209 0000 0072     r....).r....r
+00000450: 0600 0000 7206 0000 0072 0700 0000 da0b  ....r....r......
+00000460: 6461 7461 6672 616d 655f 322d 0000 0073  dataframe_2-...s
+00000470: 0200 0000 0005 720f 0000 0063 0100 0000  ......r....c....
+00000480: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000490: 4300 0000 730a 0000 0074 00a0 017c 00a1  C...s....t...|..
+000004a0: 0153 0029 017a 220a 2020 2020 5468 6972  .S.).z".    Thir
+000004b0: 6420 6461 7461 6672 616d 6520 666f 7220  d dataframe for 
+000004c0: 7465 7374 0a20 2020 2072 0b00 0000 2901  test.    r....).
+000004d0: 720a 0000 0072 0600 0000 7206 0000 0072  r....r....r....r
+000004e0: 0700 0000 da0b 6461 7461 6672 616d 655f  ......dataframe_
+000004f0: 3335 0000 0073 0200 0000 0005 7210 0000  35...s......r...
+00000500: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000510: 0000 0500 0000 4300 0000 731a 0000 0074  ......C...s....t
+00000520: 00a0 0174 0274 0374 0483 016a 0564 011b  ...t.t.t...j.d..
+00000530: 0064 0283 02a1 0153 0029 037a 1b0a 2020  .d.....S.).z..  
+00000540: 2020 4c6f 6164 2070 6963 6b6c 6564 2066    Load pickled f
+00000550: 696c 650a 2020 2020 7a10 6d73 6563 6c69  ile.    z.msecli
+00000560: 7073 652e 7069 636b 6c65 da02 7262 2906  pse.pickle..rb).
+00000570: da06 7069 636b 6c65 da04 6c6f 6164 da04  ..pickle..load..
+00000580: 6f70 656e 7202 0000 0072 0400 0000 7205  openr....r....r.
+00000590: 0000 0072 0600 0000 7206 0000 0072 0600  ...r....r....r..
+000005a0: 0000 7207 0000 00da 0a70 6963 6b6c 6564  ..r......pickled
+000005b0: 5f6d 733d 0000 0073 0c00 0000 0005 0401  _ms=...s........
+000005c0: 0201 0c00 02ff 02ff 7215 0000 0063 0400  ........r....c..
+000005d0: 0000 0000 0000 0000 0000 0b00 0000 0900  ................
+000005e0: 0000 4300 0000 73f8 0200 0074 006a 017c  ..C...s....t.j.|
+000005f0: 007c 0164 0164 0267 0264 038d 0301 0074  .|.d.d.g.d.....t
+00000600: 006a 017c 027c 0364 0164 0267 0264 038d  .j.|.|.d.d.g.d..
+00000610: 0301 0074 02a0 0374 04a1 018f 127d 0474  ...t...t.....}.t
+00000620: 00a0 017c 027c 03a1 0201 0057 0035 0051  ...|.|.....W.5.Q
+00000630: 0052 0058 0064 047d 057c 046a 057d 0674  .R.X.d.}.|.j.}.t
+00000640: 067c 0683 017d 077c 057c 076b 067d 087c  .|...}.|.|.k.}.|
+00000650: 0873 fa74 07a0 0864 057c 0866 0164 067c  .s.t...d.|.f.d.|
+00000660: 057c 0766 02a1 0474 07a0 097c 05a1 0164  .|.f...t...|...d
+00000670: 0774 0aa0 0ba1 006b 0673 9a74 07a0 0c74  .t.....k.s.t...t
+00000680: 06a1 0172 a474 07a0 0974 06a1 016e 0264  ...r.t...t...n.d
+00000690: 0764 0874 0aa0 0ba1 006b 0673 bc74 07a0  .d.t.....k.s.t..
+000006a0: 0c7c 04a1 0172 c674 07a0 097c 04a1 016e  .|...r.t...|...n
+000006b0: 0264 0874 07a0 097c 06a1 0174 07a0 097c  .d.t...|...t...|
+000006c0: 07a1 0164 099c 0516 007d 0964 0a64 0b7c  ...d.....}.d.d.|
+000006d0: 0969 0116 007d 0a74 0d74 07a0 0e7c 0aa1  .i...}.t.t...|..
+000006e0: 0183 0182 0164 0c04 007d 0504 007d 0804  .....d...}...}..
+000006f0: 007d 067d 0774 02a0 0374 04a1 018f 1c7d  .}.}.t...t.....}
+00000700: 0474 006a 017c 007c 0164 0164 0264 0d67  .t.j.|.|.d.d.d.g
+00000710: 0364 038d 0301 0057 0035 0051 0052 0058  .d.....W.5.Q.R.X
+00000720: 0064 0e7d 057c 046a 057d 0674 067c 0683  .d.}.|.j.}.t.|..
+00000730: 017d 077c 057c 076b 067d 087c 0890 0173  .}.|.|.k.}.|...s
+00000740: f074 07a0 0864 057c 0866 0164 067c 057c  .t...d.|.f.d.|.|
+00000750: 0766 02a1 0474 07a0 097c 05a1 0164 0774  .f...t...|...d.t
+00000760: 0aa0 0ba1 006b 0690 0173 8c74 07a0 0c74  .....k...s.t...t
+00000770: 06a1 0190 0172 9674 07a0 0974 06a1 016e  .....r.t...t...n
+00000780: 0264 0764 0874 0aa0 0ba1 006b 0690 0173  .d.d.t.....k...s
+00000790: b274 07a0 0c7c 04a1 0190 0172 bc74 07a0  .t...|.....r.t..
+000007a0: 097c 04a1 016e 0264 0874 07a0 097c 06a1  .|...n.d.t...|..
+000007b0: 0174 07a0 097c 07a1 0164 099c 0516 007d  .t...|...d.....}
+000007c0: 0964 0a64 0b7c 0969 0116 007d 0a74 0d74  .d.d.|.i...}.t.t
+000007d0: 07a0 0e7c 0aa1 0183 0182 0164 0c04 007d  ...|.......d...}
+000007e0: 0504 007d 0804 007d 067d 0774 02a0 0374  ...}...}.}.t...t
+000007f0: 04a1 018f 1a7d 0474 006a 017c 007c 0164  .....}.t.j.|.|.d
+00000800: 0264 0267 0264 038d 0301 0057 0035 0051  .d.g.d.....W.5.Q
+00000810: 0052 0058 0064 0f7d 057c 046a 057d 0674  .R.X.d.}.|.j.}.t
+00000820: 067c 0683 017d 077c 057c 076b 067d 087c  .|...}.|.|.k.}.|
+00000830: 0890 0273 e474 07a0 0864 057c 0866 0164  ...s.t...d.|.f.d
+00000840: 067c 057c 0766 02a1 0474 07a0 097c 05a1  .|.|.f...t...|..
+00000850: 0164 0774 0aa0 0ba1 006b 0690 0273 8074  .d.t.....k...s.t
+00000860: 07a0 0c74 06a1 0190 0272 8a74 07a0 0974  ...t.....r.t...t
+00000870: 06a1 016e 0264 0764 0874 0aa0 0ba1 006b  ...n.d.d.t.....k
+00000880: 0690 0273 a674 07a0 0c7c 04a1 0190 0272  ...s.t...|.....r
+00000890: b074 07a0 097c 04a1 016e 0264 0874 07a0  .t...|...n.d.t..
+000008a0: 097c 06a1 0174 07a0 097c 07a1 0164 099c  .|...t...|...d..
+000008b0: 0516 007d 0964 0a64 0b7c 0969 0116 007d  ...}.d.d.|.i...}
+000008c0: 0a74 0d74 07a0 0e7c 0aa1 0183 0182 0164  .t.t...|.......d
+000008d0: 0c04 007d 0504 007d 0804 007d 067d 0764  ...}...}...}.}.d
+000008e0: 0c53 0029 107a 350a 2020 2020 5465 7374  .S.).z5.    Test
+000008f0: 204d 5341 6c69 676e 6572 2069 6e69 7469   MSAligner initi
+00000900: 616c 697a 6573 206f 7220 7468 726f 7773  alizes or throws
+00000910: 2065 7272 6f72 730a 2020 2020 da03 6870   errors.    ..hp
+00000920: 31da 0368 7032 a901 da05 6e61 6d65 73fa  1..hp2....names.
+00000930: 106d 7573 7420 6265 2070 726f 7669 6465  .must be provide
+00000940: 64a9 01da 0269 6ea9 017a 4b25 2870 7931  d....in..zK%(py1
+00000950: 2973 2069 6e20 2528 7079 3829 730a 7b25  )s in %(py8)s.{%
+00000960: 2870 7938 2973 203d 2025 2870 7933 2973  (py8)s = %(py3)s
+00000970: 2825 2870 7936 2973 0a7b 2528 7079 3629  (%(py6)s.{%(py6)
+00000980: 7320 3d20 2528 7079 3429 732e 7661 6c75  s = %(py4)s.valu
+00000990: 650a 7d29 0a7d da03 7374 72da 0165 a905  e.}).}..str..e..
+000009a0: da03 7079 31da 0370 7933 da03 7079 34da  ..py1..py3..py4.
+000009b0: 0370 7936 da03 7079 38fa 0f61 7373 6572  .py6..py8..asser
+000009c0: 7420 2528 7079 3130 2973 da04 7079 3130  t %(py10)s..py10
+000009d0: 4eda 0368 7033 7a13 5468 6520 6e75 6d62  N..hp3z.The numb
+000009e0: 6572 206f 6620 6e61 6d65 73da 0964 7570  er of names..dup
+000009f0: 6c69 6361 7465 290f da02 6d73 da09 4d53  licate)...ms..MS
+00000a00: 416c 6967 6e65 72da 0670 7974 6573 74da  Aligner..pytest.
+00000a10: 0672 6169 7365 73da 0a56 616c 7565 4572  .raises..ValueEr
+00000a20: 726f 72da 0576 616c 7565 721e 0000 00da  ror..valuer.....
+00000a30: 0a40 7079 7465 7374 5f61 72da 115f 6361  .@pytest_ar.._ca
+00000a40: 6c6c 5f72 6570 7263 6f6d 7061 7265 da09  ll_reprcompare..
+00000a50: 5f73 6166 6572 6570 72da 0c40 7079 5f62  _saferepr..@py_b
+00000a60: 7569 6c74 696e 73da 066c 6f63 616c 73da  uiltins..locals.
+00000a70: 185f 7368 6f75 6c64 5f72 6570 725f 676c  ._should_repr_gl
+00000a80: 6f62 616c 5f6e 616d 65da 0e41 7373 6572  obal_name..Asser
+00000a90: 7469 6f6e 4572 726f 72da 135f 666f 726d  tionError.._form
+00000aa0: 6174 5f65 7870 6c61 6e61 7469 6f6e 290b  at_explanation).
+00000ab0: 7208 0000 0072 0900 0000 720e 0000 0072  r....r....r....r
+00000ac0: 0f00 0000 721f 0000 00da 0b40 7079 5f61  ....r......@py_a
+00000ad0: 7373 6572 7430 da0b 4070 795f 6173 7365  ssert0..@py_asse
+00000ae0: 7274 35da 0b40 7079 5f61 7373 6572 7437  rt5..@py_assert7
+00000af0: da0b 4070 795f 6173 7365 7274 32da 0b40  ..@py_assert2..@
+00000b00: 7079 5f66 6f72 6d61 7439 da0c 4070 795f  py_format9..@py_
+00000b10: 666f 726d 6174 3131 7206 0000 0072 0600  format11r....r..
+00000b20: 0000 7207 0000 00da 1374 6573 745f 696e  ..r......test_in
+00000b30: 6974 6961 6c69 7a65 5f61 6464 4900 0000  itialize_addI...
+00000b40: 7346 0000 0000 0614 0314 030c 0116 0104  sF..............
+00000b50: 0006 0008 0008 0004 0078 000c 000e 0010  .........x......
+00000b60: 030c 0120 0104 0006 0008 0008 0006 0080  ... ............
+00000b70: 000c 000e 0010 030c 011e 0104 0006 0008  ................
+00000b80: 0008 0006 0080 000c 000e 0072 3e00 0000  ...........r>...
+00000b90: 6304 0000 0000 0000 0000 0000 000c 0000  c...............
+00000ba0: 0009 0000 0043 0000 0073 fc01 0000 7400  .....C...s....t.
+00000bb0: a001 a100 7d04 7c04 a002 7c00 6401 a102  ....}.|...|.d...
+00000bc0: 0100 7c04 a002 7c03 6402 a102 0100 7403  ..|...|.d.....t.
+00000bd0: a004 7405 a101 8f12 7d05 7c04 a002 7c01  ..t.....}.|...|.
+00000be0: 6402 a102 0100 5700 3500 5100 5200 5800  d.....W.5.Q.R.X.
+00000bf0: 6403 7d06 7c05 6a06 7d07 7407 7c07 8301  d.}.|.j.}.t.|...
+00000c00: 7d08 7c06 7c08 6b06 7d09 7c09 73f2 7408  }.|.|.k.}.|.s.t.
+00000c10: a009 6404 7c09 6601 6405 7c06 7c08 6602  ..d.|.f.d.|.|.f.
+00000c20: a104 7408 a00a 7c06 a101 6406 740b a00c  ..t...|...d.t...
+00000c30: a100 6b06 7392 7408 a00d 7407 a101 729c  ..k.s.t...t...r.
+00000c40: 7408 a00a 7407 a101 6e02 6406 6407 740b  t...t...n.d.d.t.
+00000c50: a00c a100 6b06 73b4 7408 a00d 7c05 a101  ....k.s.t...|...
+00000c60: 72be 7408 a00a 7c05 a101 6e02 6407 7408  r.t...|...n.d.t.
+00000c70: a00a 7c07 a101 7408 a00a 7c08 a101 6408  ..|...t...|...d.
+00000c80: 9c05 1600 7d0a 6409 640a 7c0a 6901 1600  ....}.d.d.|.i...
+00000c90: 7d0b 740e 7408 a00f 7c0b a101 8301 8201  }.t.t...|.......
+00000ca0: 640b 0400 7d06 0400 7d09 0400 7d07 7d08  d...}...}...}.}.
+00000cb0: 7c04 a002 7c02 640c a102 0100 7403 a004  |...|.d.....t...
+00000cc0: 7405 a101 8f10 7d05 7c04 a002 7c03 a101  t.....}.|...|...
+00000cd0: 0100 5700 3500 5100 5200 5800 640d 7d06  ..W.5.Q.R.X.d.}.
+00000ce0: 7c05 6a06 7d07 7407 7c07 8301 7d08 7c06  |.j.}.t.|...}.|.
+00000cf0: 7c08 6b06 7d09 7c09 9001 73e8 7408 a009  |.k.}.|...s.t...
+00000d00: 6404 7c09 6601 6405 7c06 7c08 6602 a104  d.|.f.d.|.|.f...
+00000d10: 7408 a00a 7c06 a101 6406 740b a00c a100  t...|...d.t.....
+00000d20: 6b06 9001 7384 7408 a00d 7407 a101 9001  k...s.t...t.....
+00000d30: 728e 7408 a00a 7407 a101 6e02 6406 6407  r.t...t...n.d.d.
+00000d40: 740b a00c a100 6b06 9001 73aa 7408 a00d  t.....k...s.t...
+00000d50: 7c05 a101 9001 72b4 7408 a00a 7c05 a101  |.....r.t...|...
+00000d60: 6e02 6407 7408 a00a 7c07 a101 7408 a00a  n.d.t...|...t...
+00000d70: 7c08 a101 6408 9c05 1600 7d0a 6409 640a  |...d.....}.d.d.
+00000d80: 7c0a 6901 1600 7d0b 740e 7408 a00f 7c0b  |.i...}.t.t...|.
+00000d90: a101 8301 8201 640b 0400 7d06 0400 7d09  ......d...}...}.
+00000da0: 0400 7d07 7d08 640b 5300 290e 7a2b 0a20  ..}.}.d.S.).z+. 
+00000db0: 2020 2054 6573 7420 4d53 416c 6967 6e65     Test MSAligne
+00000dc0: 7220 6164 645f 6461 7461 7365 7420 6d65  r add_dataset me
+00000dd0: 7468 6f64 0a20 2020 2072 1600 0000 7217  thod.    r....r.
+00000de0: 0000 0072 2900 0000 721b 0000 0072 1d00  ...r)...r....r..
+00000df0: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00000e00: 0072 2600 0000 7227 0000 004e 7228 0000  .r&...r'...Nr(..
+00000e10: 0072 1a00 0000 2910 722a 0000 0072 2b00  .r....).r*...r+.
+00000e20: 0000 da0b 6164 645f 6461 7461 7365 7472  ....add_datasetr
+00000e30: 2c00 0000 722d 0000 0072 2e00 0000 722f  ,...r-...r....r/
+00000e40: 0000 0072 1e00 0000 7230 0000 0072 3100  ...r....r0...r1.
+00000e50: 0000 7232 0000 0072 3300 0000 7234 0000  ..r2...r3...r4..
+00000e60: 0072 3500 0000 7236 0000 0072 3700 0000  .r5...r6...r7...
+00000e70: 290c 7208 0000 0072 0900 0000 720e 0000  ).r....r....r...
+00000e80: 0072 0f00 0000 da01 6172 1f00 0000 7238  .r......ar....r8
+00000e90: 0000 0072 3900 0000 723a 0000 0072 3b00  ...r9...r:...r;.
+00000ea0: 0000 723c 0000 0072 3d00 0000 7206 0000  ..r<...r=...r...
+00000eb0: 0072 0600 0000 7207 0000 00da 1074 6573  .r....r......tes
+00000ec0: 745f 6164 645f 6461 7461 7365 7464 0000  t_add_datasetd..
+00000ed0: 0073 3400 0000 0004 0803 0c01 0c03 0c01  .s4.............
+00000ee0: 1601 0400 0600 0800 0800 0400 7800 0c00  ............x...
+00000ef0: 0e00 1003 0c03 0c01 1401 0400 0600 0800  ................
+00000f00: 0800 0600 8000 0c00 0e00 7241 0000 0063  ..........rA...c
+00000f10: 0300 0000 0000 0000 0000 0000 2800 0000  ............(...
+00000f20: 0c00 0000 4300 0000 731e 1600 0074 006a  ....C...s....t.j
+00000f30: 017c 007c 0164 0164 0267 0264 038d 037d  .|.|.d.d.g.d...}
+00000f40: 037c 03a0 02a1 0001 007c 036a 0364 0119  .|.......|.j.d..
+00000f50: 007d 047c 026a 0364 0119 007d 057c 047c  .}.|.j.d...}.|.|
+00000f60: 056b 027d 067c 0673 8274 04a0 0564 047c  .k.}.|.s.t...d.|
+00000f70: 0666 0164 057c 047c 0566 02a1 0474 04a0  .f.d.|.|.f...t..
+00000f80: 067c 04a1 0174 04a0 067c 05a1 0164 069c  .|...t...|...d..
+00000f90: 0216 007d 0764 0764 087c 0769 0116 007d  ...}.d.d.|.i...}
+00000fa0: 0874 0774 04a0 087c 08a1 0183 0182 0164  .t.t...|.......d
+00000fb0: 0904 007d 0404 007d 067d 057c 036a 0364  ...}...}.}.|.j.d
+00000fc0: 0219 007d 047c 026a 0364 0219 007d 057c  ...}.|.j.d...}.|
+00000fd0: 047c 056b 027d 067c 0673 f474 04a0 0564  .|.k.}.|.s.t...d
+00000fe0: 047c 0666 0164 057c 047c 0566 02a1 0474  .|.f.d.|.|.f...t
+00000ff0: 04a0 067c 04a1 0174 04a0 067c 05a1 0164  ...|...t...|...d
+00001000: 069c 0216 007d 0764 0764 087c 0769 0116  .....}.d.d.|.i..
+00001010: 007d 0874 0774 04a0 087c 08a1 0183 0182  .}.t.t...|......
+00001020: 0164 0904 007d 0404 007d 067d 057c 03a0  .d...}...}.}.|..
+00001030: 09a1 0001 0074 0a6a 0b7d 097c 036a 0c64  .....t.j.}.|.j.d
+00001040: 0119 0064 0219 007d 057c 056a 0d7d 0a7c  ...d...}.|.j.}.|
+00001050: 026a 0c64 0119 0064 0219 007d 0b7c 0b6a  .j.d...d...}.|.j
+00001060: 0d7d 0c7c 097c 0a7c 0c83 027d 0d7c 0d6a  .}.|.|.|...}.|.j
+00001070: 0e7d 0e7c 0e83 007d 0f7c 0f90 0173 d064  .}.|...}.|...s.d
+00001080: 0a64 0b74 0fa0 10a1 006b 0690 0173 6e74  .d.t.....k...snt
+00001090: 04a0 1174 0aa1 0190 0172 7874 04a0 0674  ...t.....rxt...t
+000010a0: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
+000010b0: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
+000010c0: 04a0 067c 0ba1 0174 04a0 067c 0ca1 0174  ...|...t...|...t
+000010d0: 04a0 067c 0da1 0174 04a0 067c 0ea1 0174  ...|...t...|...t
+000010e0: 04a0 067c 0fa1 0164 0c9c 0916 007d 1074  ...|...d.....}.t
+000010f0: 0774 04a0 087c 10a1 0183 0182 0164 0904  .t...|.......d..
+00001100: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
+00001110: 007d 0c04 007d 0d04 007d 0e7d 0f7c 03a0  .}...}...}.}.|..
+00001120: 12a1 0001 007c 036a 1364 0119 0064 0219  .....|.j.d...d..
+00001130: 007d 117c 026a 1364 0119 0064 0219 007d  .}.|.j.d...d...}
+00001140: 1274 0a6a 147d 097c 1164 0d19 0064 0e19  .t.j.}.|.d...d..
+00001150: 007d 057c 1264 0d19 0064 0e19 007d 0a7c  .}.|.d...d...}.|
+00001160: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
+00001170: 0c83 007d 0d7c 0d90 0273 bc64 0f64 0b74  ...}.|...s.d.d.t
+00001180: 0fa0 10a1 006b 0690 0273 6a74 04a0 1174  .....k...sjt...t
+00001190: 0aa1 0190 0272 7474 04a0 0674 0aa1 016e  .....rtt...t...n
+000011a0: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
+000011b0: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
+000011c0: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
+000011d0: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
+000011e0: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
+000011f0: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
+00001200: 0d74 0a6a 147d 097c 1164 0d19 0064 1119  .t.j.}.|.d...d..
+00001210: 007d 057c 1264 0d19 0064 1119 007d 0a7c  .}.|.d...d...}.|
+00001220: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
+00001230: 0c83 007d 0d7c 0d90 0373 7c64 0f64 0b74  ...}.|...s|d.d.t
+00001240: 0fa0 10a1 006b 0690 0373 2a74 04a0 1174  .....k...s*t...t
+00001250: 0aa1 0190 0372 3474 04a0 0674 0aa1 016e  .....r4t...t...n
+00001260: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
+00001270: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
+00001280: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
+00001290: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
+000012a0: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
+000012b0: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
+000012c0: 0d74 0a6a 147d 097c 1164 1219 0064 0e19  .t.j.}.|.d...d..
+000012d0: 007d 057c 1264 1219 0064 0e19 007d 0a7c  .}.|.d...d...}.|
+000012e0: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
+000012f0: 0c83 007d 0d7c 0d90 0473 3c64 0f64 0b74  ...}.|...s<d.d.t
+00001300: 0fa0 10a1 006b 0690 0373 ea74 04a0 1174  .....k...s.t...t
+00001310: 0aa1 0190 0372 f474 04a0 0674 0aa1 016e  .....r.t...t...n
+00001320: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
+00001330: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
+00001340: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
+00001350: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
+00001360: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
+00001370: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
+00001380: 0d74 0a6a 147d 097c 1164 1219 0064 1119  .t.j.}.|.d...d..
+00001390: 007d 057c 1264 1219 0064 1119 007d 0a7c  .}.|.d...d...}.|
+000013a0: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
+000013b0: 0c83 007d 0d7c 0d90 0473 fc64 0f64 0b74  ...}.|...s.d.d.t
+000013c0: 0fa0 10a1 006b 0690 0473 aa74 04a0 1174  .....k...s.t...t
+000013d0: 0aa1 0190 0472 b474 04a0 0674 0aa1 016e  .....r.t...t...n
+000013e0: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
+000013f0: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
+00001400: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
+00001410: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
+00001420: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
+00001430: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
+00001440: 0d74 0a6a 147d 097c 1164 1319 0064 1119  .t.j.}.|.d...d..
+00001450: 007d 057c 1264 1319 0064 1119 007d 0a7c  .}.|.d...d...}.|
+00001460: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
+00001470: 0c83 007d 0d7c 0d90 0573 bc64 0f64 0b74  ...}.|...s.d.d.t
+00001480: 0fa0 10a1 006b 0690 0573 6a74 04a0 1174  .....k...sjt...t
+00001490: 0aa1 0190 0572 7474 04a0 0674 0aa1 016e  .....rtt...t...n
+000014a0: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
+000014b0: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
+000014c0: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
+000014d0: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
+000014e0: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
+000014f0: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
+00001500: 0d74 0a6a 147d 097c 1164 1319 0064 0e19  .t.j.}.|.d...d..
+00001510: 007d 057c 1264 1319 0064 0e19 007d 0a7c  .}.|.d...d...}.|
+00001520: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
+00001530: 0c83 007d 0d7c 0d90 0673 7c64 0f64 0b74  ...}.|...s|d.d.t
+00001540: 0fa0 10a1 006b 0690 0673 2a74 04a0 1174  .....k...s*t...t
+00001550: 0aa1 0190 0672 3474 04a0 0674 0aa1 016e  .....r4t...t...n
+00001560: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
+00001570: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
+00001580: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
+00001590: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
+000015a0: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
+000015b0: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
+000015c0: 0d7c 03a0 15a1 0001 007c 036a 1664 0119  .|.......|.j.d..
+000015d0: 0064 0219 007d 147c 026a 1664 0119 0064  .d...}.|.j.d...d
+000015e0: 0219 007d 1574 0a6a 147d 097c 1464 0d19  ...}.t.j.}.|.d..
+000015f0: 007d 057c 1564 0d19 007d 0a7c 097c 057c  .}.|.d...}.|.|.|
+00001600: 0a83 027d 0b7c 0b6a 0e7d 0c7c 0c83 007d  ...}.|.j.}.|...}
+00001610: 0d7c 0d90 0773 5864 0f64 0b74 0fa0 10a1  .|...sXd.d.t....
+00001620: 006b 0690 0773 0674 04a0 1174 0aa1 0190  .k...s.t...t....
+00001630: 0772 1074 04a0 0674 0aa1 016e 0264 0b74  .r.t...t...n.d.t
+00001640: 04a0 067c 09a1 0174 04a0 067c 05a1 0174  ...|...t...|...t
+00001650: 04a0 067c 0aa1 0174 04a0 067c 0ba1 0174  ...|...t...|...t
+00001660: 04a0 067c 0ca1 0174 04a0 067c 0da1 0164  ...|...t...|...d
+00001670: 109c 0716 007d 1374 0774 04a0 087c 13a1  .....}.t.t...|..
+00001680: 0183 0182 0164 0904 007d 0904 007d 0504  .....d...}...}..
+00001690: 007d 0a04 007d 0b04 007d 0c7d 0d74 0a6a  .}...}...}.}.t.j
+000016a0: 147d 097c 1464 1219 007d 057c 1564 1219  .}.|.d...}.|.d..
+000016b0: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b6a  .}.|.|.|...}.|.j
+000016c0: 0e7d 0c7c 0c83 007d 0d7c 0d90 0873 1064  .}.|...}.|...s.d
+000016d0: 0f64 0b74 0fa0 10a1 006b 0690 0773 be74  .d.t.....k...s.t
+000016e0: 04a0 1174 0aa1 0190 0772 c874 04a0 0674  ...t.....r.t...t
+000016f0: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
+00001700: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
+00001710: 04a0 067c 0ba1 0174 04a0 067c 0ca1 0174  ...|...t...|...t
+00001720: 04a0 067c 0da1 0164 109c 0716 007d 1374  ...|...d.....}.t
+00001730: 0774 04a0 087c 13a1 0183 0182 0164 0904  .t...|.......d..
+00001740: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
+00001750: 007d 0c7d 0d74 0a6a 147d 097c 1464 1319  .}.}.t.j.}.|.d..
+00001760: 007d 057c 1564 1319 007d 0a7c 097c 057c  .}.|.d...}.|.|.|
+00001770: 0a83 027d 0b7c 0b6a 0e7d 0c7c 0c83 007d  ...}.|.j.}.|...}
+00001780: 0d7c 0d90 0873 c864 0f64 0b74 0fa0 10a1  .|...s.d.d.t....
+00001790: 006b 0690 0873 7674 04a0 1174 0aa1 0190  .k...svt...t....
+000017a0: 0872 8074 04a0 0674 0aa1 016e 0264 0b74  .r.t...t...n.d.t
+000017b0: 04a0 067c 09a1 0174 04a0 067c 05a1 0174  ...|...t...|...t
+000017c0: 04a0 067c 0aa1 0174 04a0 067c 0ba1 0174  ...|...t...|...t
+000017d0: 04a0 067c 0ca1 0174 04a0 067c 0da1 0164  ...|...t...|...d
+000017e0: 109c 0716 007d 1374 0774 04a0 087c 13a1  .....}.t.t...|..
+000017f0: 0183 0182 0164 0904 007d 0904 007d 0504  .....d...}...}..
+00001800: 007d 0a04 007d 0b04 007d 0c7d 0d7c 03a0  .}...}...}.}.|..
+00001810: 17a1 0001 0074 0a6a 147d 097c 036a 1864  .....t.j.}.|.j.d
+00001820: 0119 0064 0219 0064 0d19 007d 057c 026a  ...d...d...}.|.j
+00001830: 1864 0119 0064 0219 0064 0d19 007d 0a7c  .d...d...d...}.|
+00001840: 097c 057c 0a83 027d 0b7c 0b90 0973 8064  .|.|...}.|...s.d
+00001850: 1464 0b74 0fa0 10a1 006b 0690 0973 3e74  .d.t.....k...s>t
+00001860: 04a0 1174 0aa1 0190 0972 4874 04a0 0674  ...t.....rHt...t
+00001870: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
+00001880: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
+00001890: 04a0 067c 0ba1 0164 159c 0516 007d 1674  ...|...d.....}.t
+000018a0: 0774 04a0 087c 16a1 0183 0182 0164 0904  .t...|.......d..
+000018b0: 007d 0904 007d 0504 007d 0a7d 0b74 0a6a  .}...}...}.}.t.j
+000018c0: 147d 097c 036a 1864 0119 0064 0219 0064  .}.|.j.d...d...d
+000018d0: 1219 007d 057c 026a 1864 0119 0064 0219  ...}.|.j.d...d..
+000018e0: 0064 1219 007d 0a7c 097c 057c 0a83 027d  .d...}.|.|.|...}
+000018f0: 0b7c 0b90 0a73 2864 1464 0b74 0fa0 10a1  .|...s(d.d.t....
+00001900: 006b 0690 0973 e674 04a0 1174 0aa1 0190  .k...s.t...t....
+00001910: 0972 f074 04a0 0674 0aa1 016e 0264 0b74  .r.t...t...n.d.t
+00001920: 04a0 067c 09a1 0174 04a0 067c 05a1 0174  ...|...t...|...t
+00001930: 04a0 067c 0aa1 0174 04a0 067c 0ba1 0164  ...|...t...|...d
+00001940: 159c 0516 007d 1674 0774 04a0 087c 16a1  .....}.t.t...|..
+00001950: 0183 0182 0164 0904 007d 0904 007d 0504  .....d...}...}..
+00001960: 007d 0a7d 0b74 0a6a 147d 097c 036a 1864  .}.}.t.j.}.|.j.d
+00001970: 0119 0064 0219 0064 1319 007d 057c 026a  ...d...d...}.|.j
+00001980: 1864 0119 0064 0219 0064 1319 007d 0a7c  .d...d...d...}.|
+00001990: 097c 057c 0a83 027d 0b7c 0b90 0a73 d064  .|.|...}.|...s.d
+000019a0: 1464 0b74 0fa0 10a1 006b 0690 0a73 8e74  .d.t.....k...s.t
+000019b0: 04a0 1174 0aa1 0190 0a72 9874 04a0 0674  ...t.....r.t...t
+000019c0: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
+000019d0: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
+000019e0: 04a0 067c 0ba1 0164 159c 0516 007d 1674  ...|...d.....}.t
+000019f0: 0774 04a0 087c 16a1 0183 0182 0164 0904  .t...|.......d..
+00001a00: 007d 0904 007d 0504 007d 0a7d 0b7c 03a0  .}...}...}.}.|..
+00001a10: 19a1 0001 007c 036a 1a64 0119 0064 0219  .....|.j.d...d..
+00001a20: 007d 047c 046a 1b7d 067c 026a 1a64 0119  .}.|.j.}.|.j.d..
+00001a30: 0064 0219 007d 177c 067c 1783 017d 187c  .d...}.|.|...}.|
+00001a40: 1890 0b73 5064 1674 04a0 067c 04a1 0174  ...sPd.t...|...t
+00001a50: 04a0 067c 06a1 0174 04a0 067c 17a1 0174  ...|...t...|...t
+00001a60: 04a0 067c 18a1 0164 179c 0416 007d 1974  ...|...d.....}.t
+00001a70: 0774 04a0 087c 19a1 0183 0182 0164 0904  .t...|.......d..
+00001a80: 007d 0404 007d 0604 007d 177d 1874 006a  .}...}...}.}.t.j
+00001a90: 017c 007c 0164 0164 0267 0264 038d 037d  .|.|.d.d.g.d...}
+00001aa0: 037c 03a0 1ca1 0001 0074 00a0 1d64 1864  .|.......t...d.d
+00001ab0: 1964 1a67 0364 1b64 1c64 1d67 03a1 027d  .d.g.d.d.d.g...}
+00001ac0: 1a74 00a0 1d64 1e64 1f64 2067 0364 2164  .t...d.d.d g.d!d
+00001ad0: 2264 2367 03a1 027d 1b74 00a0 1d64 1964  "d#g...}.t...d.d
+00001ae0: 1a64 2467 0364 1a64 2464 2567 03a1 027d  .d$g.d.d$d%g...}
+00001af0: 1c74 006a 017c 007c 0164 0164 0267 0264  .t.j.|.|.d.d.g.d
+00001b00: 038d 037d 037c 036a 1e64 0164 0274 1f7c  ...}.|.j.d.d.t.|
+00001b10: 1a8e 0074 1f7c 1b8e 0074 1f7c 1c8e 0064  ...t.|...t.|...d
+00001b20: 269c 0369 0169 0164 2764 288d 0201 007c  &..i.i.d'd(....|
+00001b30: 03a0 1ca1 0001 007c 036a 1364 0119 0064  .......|.j.d...d
+00001b40: 0219 007d 1d74 0a6a 0b7d 097c 1d64 0d19  ...}.t.j.}.|.d..
+00001b50: 0064 1119 007d 057c 1a64 2919 007d 0a7c  .d...}.|.d)..}.|
+00001b60: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
+00001b70: 0c83 007d 0d7c 0d90 0c73 bc64 2a64 0b74  ...}.|...s.d*d.t
+00001b80: 0fa0 10a1 006b 0690 0c73 6a74 04a0 1174  .....k...sjt...t
+00001b90: 0aa1 0190 0c72 7474 04a0 0674 0aa1 016e  .....rtt...t...n
+00001ba0: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
+00001bb0: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
+00001bc0: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
+00001bd0: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
+00001be0: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
+00001bf0: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
+00001c00: 0d74 0a6a 0b7d 097c 1d64 0d19 0064 0e19  .t.j.}.|.d...d..
+00001c10: 007d 057c 1a64 1819 007d 0a7c 097c 057c  .}.|.d...}.|.|.|
+00001c20: 0a83 027d 0b7c 0b6a 0e7d 0c7c 0c83 007d  ...}.|.j.}.|...}
+00001c30: 0d7c 0d90 0d73 7864 2a64 0b74 0fa0 10a1  .|...sxd*d.t....
+00001c40: 006b 0690 0d73 2674 04a0 1174 0aa1 0190  .k...s&t...t....
+00001c50: 0d72 3074 04a0 0674 0aa1 016e 0264 0b74  .r0t...t...n.d.t
+00001c60: 04a0 067c 09a1 0174 04a0 067c 05a1 0174  ...|...t...|...t
+00001c70: 04a0 067c 0aa1 0174 04a0 067c 0ba1 0174  ...|...t...|...t
+00001c80: 04a0 067c 0ca1 0174 04a0 067c 0da1 0164  ...|...t...|...d
+00001c90: 109c 0716 007d 1374 0774 04a0 087c 13a1  .....}.t.t...|..
+00001ca0: 0183 0182 0164 0904 007d 0904 007d 0504  .....d...}...}..
+00001cb0: 007d 0a04 007d 0b04 007d 0c7d 0d74 0a6a  .}...}...}.}.t.j
+00001cc0: 0b7d 097c 1d64 1219 0064 1119 007d 057c  .}.|.d...d...}.|
+00001cd0: 1b64 2919 007d 0a7c 097c 057c 0a83 027d  .d)..}.|.|.|...}
+00001ce0: 0b7c 0b6a 0e7d 0c7c 0c83 007d 0d7c 0d90  .|.j.}.|...}.|..
+00001cf0: 0e73 3464 2a64 0b74 0fa0 10a1 006b 0690  .s4d*d.t.....k..
+00001d00: 0d73 e274 04a0 1174 0aa1 0190 0d72 ec74  .s.t...t.....r.t
+00001d10: 04a0 0674 0aa1 016e 0264 0b74 04a0 067c  ...t...n.d.t...|
+00001d20: 09a1 0174 04a0 067c 05a1 0174 04a0 067c  ...t...|...t...|
+00001d30: 0aa1 0174 04a0 067c 0ba1 0174 04a0 067c  ...t...|...t...|
+00001d40: 0ca1 0174 04a0 067c 0da1 0164 109c 0716  ...t...|...d....
+00001d50: 007d 1374 0774 04a0 087c 13a1 0183 0182  .}.t.t...|......
+00001d60: 0164 0904 007d 0904 007d 0504 007d 0a04  .d...}...}...}..
+00001d70: 007d 0b04 007d 0c7d 0d74 0a6a 0b7d 097c  .}...}.}.t.j.}.|
+00001d80: 1d64 1219 0064 0e19 007d 057c 1b64 1819  .d...d...}.|.d..
+00001d90: 007d 0a7c 097c 057c 0a83 027d 0b7c 0b6a  .}.|.|.|...}.|.j
+00001da0: 0e7d 0c7c 0c83 007d 0d7c 0d90 0e73 f064  .}.|...}.|...s.d
+00001db0: 2a64 0b74 0fa0 10a1 006b 0690 0e73 9e74  *d.t.....k...s.t
+00001dc0: 04a0 1174 0aa1 0190 0e72 a874 04a0 0674  ...t.....r.t...t
+00001dd0: 0aa1 016e 0264 0b74 04a0 067c 09a1 0174  ...n.d.t...|...t
+00001de0: 04a0 067c 05a1 0174 04a0 067c 0aa1 0174  ...|...t...|...t
+00001df0: 04a0 067c 0ba1 0174 04a0 067c 0ca1 0174  ...|...t...|...t
+00001e00: 04a0 067c 0da1 0164 109c 0716 007d 1374  ...|...d.....}.t
+00001e10: 0774 04a0 087c 13a1 0183 0182 0164 0904  .t...|.......d..
+00001e20: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
+00001e30: 007d 0c7d 0d74 0a6a 0b7d 097c 1d64 1319  .}.}.t.j.}.|.d..
+00001e40: 0064 1119 007d 057c 1c64 2919 007d 0a7c  .d...}.|.d)..}.|
+00001e50: 097c 057c 0a83 027d 0b7c 0b6a 0e7d 0c7c  .|.|...}.|.j.}.|
+00001e60: 0c83 007d 0d7c 0d90 0f73 ac64 2a64 0b74  ...}.|...s.d*d.t
+00001e70: 0fa0 10a1 006b 0690 0f73 5a74 04a0 1174  .....k...sZt...t
+00001e80: 0aa1 0190 0f72 6474 04a0 0674 0aa1 016e  .....rdt...t...n
+00001e90: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
+00001ea0: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
+00001eb0: 0ba1 0174 04a0 067c 0ca1 0174 04a0 067c  ...t...|...t...|
+00001ec0: 0da1 0164 109c 0716 007d 1374 0774 04a0  ...d.....}.t.t..
+00001ed0: 087c 13a1 0183 0182 0164 0904 007d 0904  .|.......d...}..
+00001ee0: 007d 0504 007d 0a04 007d 0b04 007d 0c7d  .}...}...}...}.}
+00001ef0: 0d74 0a6a 0b7d 097c 1d64 1319 0064 0e19  .t.j.}.|.d...d..
+00001f00: 007d 057c 1c64 1819 007d 0a7c 097c 057c  .}.|.d...}.|.|.|
+00001f10: 0a83 027d 0b7c 0b6a 0e7d 0c7c 0c83 007d  ...}.|.j.}.|...}
+00001f20: 0d7c 0d90 1073 6864 2a64 0b74 0fa0 10a1  .|...shd*d.t....
+00001f30: 006b 0690 1073 1674 04a0 1174 0aa1 0190  .k...s.t...t....
+00001f40: 1072 2074 04a0 0674 0aa1 016e 0264 0b74  .r t...t...n.d.t
+00001f50: 04a0 067c 09a1 0174 04a0 067c 05a1 0174  ...|...t...|...t
+00001f60: 04a0 067c 0aa1 0174 04a0 067c 0ba1 0174  ...|...t...|...t
+00001f70: 04a0 067c 0ca1 0174 04a0 067c 0da1 0164  ...|...t...|...d
+00001f80: 109c 0716 007d 1374 0774 04a0 087c 13a1  .....}.t.t...|..
+00001f90: 0183 0182 0164 0904 007d 0904 007d 0504  .....d...}...}..
+00001fa0: 007d 0a04 007d 0b04 007d 0c7d 0d74 006a  .}...}...}.}.t.j
+00001fb0: 017c 007c 0164 0164 0267 0264 038d 037d  .|.|.d.d.g.d...}
+00001fc0: 037c 036a 1e64 0164 0274 1f7c 1a8e 0074  .|.j.d.d.t.|...t
+00001fd0: 1f7c 1b8e 0074 1f7c 1c8e 0064 269c 0369  .|...t.|...d&..i
+00001fe0: 0169 0164 2b64 288d 0201 007c 03a0 1ca1  .i.d+d(....|....
+00001ff0: 0001 007c 036a 1364 0219 0064 0119 007d  ...|.j.d...d...}
+00002000: 1d74 0a6a 0b7d 097c 1d64 0d19 0064 1119  .t.j.}.|.d...d..
+00002010: 007d 057c 1a64 2919 007d 0a7c 1a64 1819  .}.|.d)..}.|.d..
+00002020: 007d 0b7c 0a7c 0b17 007d 0c7c 097c 057c  .}.|.|...}.|.|.|
+00002030: 0c83 027d 1e7c 1e6a 0e7d 1f7c 1f83 007d  ...}.|.j.}.|...}
+00002040: 207c 2090 1173 9064 2c64 0b74 0fa0 10a1   | ..s.d,d.t....
+00002050: 006b 0690 1173 3674 04a0 1174 0aa1 0190  .k...s6t...t....
+00002060: 1172 4074 04a0 0674 0aa1 016e 0264 0b74  .r@t...t...n.d.t
+00002070: 04a0 067c 09a1 0174 04a0 067c 05a1 0174  ...|...t...|...t
+00002080: 04a0 067c 0aa1 0174 04a0 067c 0ba1 0174  ...|...t...|...t
+00002090: 04a0 067c 1ea1 0174 04a0 067c 1fa1 0174  ...|...t...|...t
+000020a0: 04a0 067c 20a1 0164 2d9c 0816 007d 2174  ...| ..d-....}!t
+000020b0: 0774 04a0 087c 21a1 0183 0182 0164 0904  .t...|!......d..
+000020c0: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
+000020d0: 007d 0c04 007d 1e04 007d 1f7d 2074 0a6a  .}...}...}.} t.j
+000020e0: 0b7d 097c 1d64 0d19 0064 0e19 007d 057c  .}.|.d...d...}.|
+000020f0: 1a64 1819 007d 0a7c 0a0b 007d 0b7c 097c  .d...}.|...}.|.|
+00002100: 057c 0b83 027d 227c 226a 0e7d 1e7c 1e83  .|...}"|"j.}.|..
+00002110: 007d 1f7c 1f90 1273 5a64 2e64 0b74 0fa0  .}.|...sZd.d.t..
+00002120: 10a1 006b 0690 1273 0874 04a0 1174 0aa1  ...k...s.t...t..
+00002130: 0190 1272 1274 04a0 0674 0aa1 016e 0264  ...r.t...t...n.d
+00002140: 0b74 04a0 067c 09a1 0174 04a0 067c 05a1  .t...|...t...|..
+00002150: 0174 04a0 067c 0aa1 0174 04a0 067c 22a1  .t...|...t...|".
+00002160: 0174 04a0 067c 1ea1 0174 04a0 067c 1fa1  .t...|...t...|..
+00002170: 0164 2f9c 0716 007d 2374 0774 04a0 087c  .d/....}#t.t...|
+00002180: 23a1 0183 0182 0164 0904 007d 0904 007d  #......d...}...}
+00002190: 0504 007d 0a04 007d 0b04 007d 2204 007d  ...}...}...}"..}
+000021a0: 1e7d 1f7c 1b64 2919 007c 1b64 2919 007c  .}.|.d)..|.d)..|
+000021b0: 1b64 1819 0014 0064 301b 0017 007d 2474  .d.....d0....}$t
+000021c0: 0a6a 0b7d 097c 1d64 1219 0064 1119 007d  .j.}.|.d...d...}
+000021d0: 057c 097c 057c 2483 027d 187c 186a 0e7d  .|.|.|$..}.|.j.}
+000021e0: 227c 2283 007d 1e7c 1e90 1373 4c64 3164  "|"..}.|...sLd1d
+000021f0: 0b74 0fa0 10a1 006b 0690 1273 dc74 04a0  .t.....k...s.t..
+00002200: 1174 0aa1 0190 1272 e674 04a0 0674 0aa1  .t.....r.t...t..
+00002210: 016e 0264 0b74 04a0 067c 09a1 0174 04a0  .n.d.t...|...t..
+00002220: 067c 05a1 0164 3274 0fa0 10a1 006b 0690  .|...d2t.....k..
+00002230: 1373 1274 04a0 117c 24a1 0190 1372 1c74  .s.t...|$....r.t
+00002240: 04a0 067c 24a1 016e 0264 3274 04a0 067c  ...|$..n.d2t...|
+00002250: 18a1 0174 04a0 067c 22a1 0174 04a0 067c  ...t...|"..t...|
+00002260: 1ea1 0164 339c 0716 007d 2574 0774 04a0  ...d3....}%t.t..
+00002270: 087c 25a1 0183 0182 0164 0904 007d 0904  .|%......d...}..
+00002280: 007d 0504 007d 1804 007d 227d 1e74 0a6a  .}...}...}"}.t.j
+00002290: 0b7d 097c 1d64 1219 0064 0e19 007d 057c  .}.|.d...d...}.|
+000022a0: 1b64 1819 007d 0a7c 0a0b 007d 0b7c 1b64  .d...}.|...}.|.d
+000022b0: 2919 007d 227c 0b7c 2214 007d 1e7c 1e7c  )..}"|.|"..}.|.|
+000022c0: 241b 007d 1f7c 097c 057c 1f83 027d 0e7c  $..}.|.|.|...}.|
+000022d0: 0e6a 0e7d 0f7c 0f83 007d 267c 2690 1473  .j.}.|...}&|&..s
+000022e0: 5064 3464 0b74 0fa0 10a1 006b 0690 1373  Pd4d.t.....k...s
+000022f0: d074 04a0 1174 0aa1 0190 1372 da74 04a0  .t...t.....r.t..
+00002300: 0674 0aa1 016e 0264 0b74 04a0 067c 09a1  .t...n.d.t...|..
+00002310: 0174 04a0 067c 05a1 0174 04a0 067c 0aa1  .t...|...t...|..
+00002320: 0174 04a0 067c 22a1 0164 3274 0fa0 10a1  .t...|"..d2t....
+00002330: 006b 0690 1473 1674 04a0 117c 24a1 0190  .k...s.t...|$...
+00002340: 1472 2074 04a0 067c 24a1 016e 0264 3274  .r t...|$..n.d2t
+00002350: 04a0 067c 0ea1 0174 04a0 067c 0fa1 0174  ...|...t...|...t
+00002360: 04a0 067c 26a1 0164 359c 0916 007d 2774  ...|&..d5....}'t
+00002370: 0774 04a0 087c 27a1 0183 0182 0164 0904  .t...|'......d..
+00002380: 007d 0904 007d 0504 007d 0a04 007d 0b04  .}...}...}...}..
+00002390: 007d 2204 007d 1e04 007d 1f04 007d 0e04  .}"..}...}...}..
+000023a0: 007d 0f7d 2674 0a6a 0b7d 097c 1d64 1319  .}.}&t.j.}.|.d..
+000023b0: 0064 1119 007d 057c 1c64 2919 007d 0a7c  .d...}.|.d)..}.|
+000023c0: 1c64 1819 007d 0b7c 0a7c 0b17 007d 0c7c  .d...}.|.|...}.|
+000023d0: 097c 057c 0c83 027d 1e7c 1e6a 0e7d 1f7c  .|.|...}.|.j.}.|
+000023e0: 1f83 007d 207c 2090 1573 3464 2c64 0b74  ...} | ..s4d,d.t
+000023f0: 0fa0 10a1 006b 0690 1473 da74 04a0 1174  .....k...s.t...t
+00002400: 0aa1 0190 1472 e474 04a0 0674 0aa1 016e  .....r.t...t...n
+00002410: 0264 0b74 04a0 067c 09a1 0174 04a0 067c  .d.t...|...t...|
+00002420: 05a1 0174 04a0 067c 0aa1 0174 04a0 067c  ...t...|...t...|
+00002430: 0ba1 0174 04a0 067c 1ea1 0174 04a0 067c  ...t...|...t...|
+00002440: 1fa1 0174 04a0 067c 20a1 0164 2d9c 0816  ...t...| ..d-...
+00002450: 007d 2174 0774 04a0 087c 21a1 0183 0182  .}!t.t...|!.....
+00002460: 0164 0904 007d 0904 007d 0504 007d 0a04  .d...}...}...}..
+00002470: 007d 0b04 007d 0c04 007d 1e04 007d 1f7d  .}...}...}...}.}
+00002480: 2074 0a6a 0b7d 097c 1d64 1319 0064 0e19   t.j.}.|.d...d..
+00002490: 007d 057c 1c64 1819 007d 0a7c 0a0b 007d  .}.|.d...}.|...}
+000024a0: 0b7c 097c 057c 0b83 027d 227c 226a 0e7d  .|.|.|...}"|"j.}
+000024b0: 1e7c 1e83 007d 1f7c 1f90 1573 fe64 2e64  .|...}.|...s.d.d
+000024c0: 0b74 0fa0 10a1 006b 0690 1573 ac74 04a0  .t.....k...s.t..
+000024d0: 1174 0aa1 0190 1572 b674 04a0 0674 0aa1  .t.....r.t...t..
+000024e0: 016e 0264 0b74 04a0 067c 09a1 0174 04a0  .n.d.t...|...t..
+000024f0: 067c 05a1 0174 04a0 067c 0aa1 0174 04a0  .|...t...|...t..
+00002500: 067c 22a1 0174 04a0 067c 1ea1 0174 04a0  .|"..t...|...t..
+00002510: 067c 1fa1 0164 2f9c 0716 007d 2374 0774  .|...d/....}#t.t
+00002520: 04a0 087c 23a1 0183 0182 0164 0904 007d  ...|#......d...}
+00002530: 0904 007d 0504 007d 0a04 007d 0b04 007d  ...}...}...}...}
+00002540: 2204 007d 1e7d 1f64 0953 0029 367a 340a  "..}.}.d.S.)6z4.
+00002550: 2020 2020 5465 7374 2074 6865 206d 6574      Test the met
+00002560: 686f 6473 2061 7373 6f63 6961 7465 6420  hods associated 
+00002570: 7769 7468 2061 6c69 676e 6d65 6e74 0a20  with alignment. 
+00002580: 2020 20da 0348 5031 da03 4850 3272 1800     ..HP1..HP2r..
+00002590: 0000 a901 fa02 3d3d 2901 7a12 2528 7079  ......==).z.%(py
+000025a0: 3129 7320 3d3d 2025 2870 7934 2973 2902  1)s == %(py4)s).
+000025b0: 7221 0000 0072 2300 0000 7a0e 6173 7365  r!...r#...z.asse
+000025c0: 7274 2025 2870 7936 2973 7224 0000 004e  rt %(py6)sr$...N
+000025d0: 7ac0 6173 7365 7274 2025 2870 7931 3629  z.assert %(py16)
+000025e0: 730a 7b25 2870 7931 3629 7320 3d20 2528  s.{%(py16)s = %(
+000025f0: 7079 3134 2973 0a7b 2528 7079 3134 2973  py14)s.{%(py14)s
+00002600: 203d 2025 2870 7931 3229 730a 7b25 2870   = %(py12)s.{%(p
+00002610: 7931 3229 7320 3d20 2528 7079 3229 730a  y12)s = %(py2)s.
+00002620: 7b25 2870 7932 2973 203d 2025 2870 7930  {%(py2)s = %(py0
+00002630: 2973 2e65 7175 616c 0a7d 2825 2870 7936  )s.equal.}(%(py6
+00002640: 2973 0a7b 2528 7079 3629 7320 3d20 2528  )s.{%(py6)s = %(
+00002650: 7079 3429 732e 7661 6c75 6573 0a7d 2c20  py4)s.values.}, 
+00002660: 2528 7079 3130 2973 0a7b 2528 7079 3130  %(py10)s.{%(py10
+00002670: 2973 203d 2025 2870 7938 2973 2e76 616c  )s = %(py8)s.val
+00002680: 7565 730a 7d29 0a7d 2e61 6c6c 0a7d 2829  ues.}).}.all.}()
+00002690: 0a7d da02 6e70 2909 da03 7079 30da 0370  .}..np)...py0..p
+000026a0: 7932 7223 0000 0072 2400 0000 7225 0000  y2r#...r$...r%..
+000026b0: 0072 2700 0000 da04 7079 3132 da04 7079  .r'.....py12..py
+000026c0: 3134 da04 7079 3136 da02 5254 da01 79fa  14..py16..RT..y.
+000026d0: 8661 7373 6572 7420 2528 7079 3132 2973  .assert %(py12)s
+000026e0: 0a7b 2528 7079 3132 2973 203d 2025 2870  .{%(py12)s = %(p
+000026f0: 7931 3029 730a 7b25 2870 7931 3029 7320  y10)s.{%(py10)s 
+00002700: 3d20 2528 7079 3829 730a 7b25 2870 7938  = %(py8)s.{%(py8
+00002710: 2973 203d 2025 2870 7932 2973 0a7b 2528  )s = %(py2)s.{%(
+00002720: 7079 3229 7320 3d20 2528 7079 3029 732e  py2)s = %(py0)s.
+00002730: 6973 636c 6f73 650a 7d28 2528 7079 3429  isclose.}(%(py4)
+00002740: 732c 2025 2870 7936 2973 290a 7d2e 616c  s, %(py6)s).}.al
+00002750: 6c0a 7d28 290a 7da9 0772 4700 0000 7248  l.}().}..rG...rH
+00002760: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
+00002770: 0000 7227 0000 0072 4900 0000 da01 78da  ..r'...rI.....x.
+00002780: 024d 5ada 0949 6e74 656e 7369 7479 7a52  .MZ..IntensityzR
+00002790: 6173 7365 7274 2025 2870 7938 2973 0a7b  assert %(py8)s.{
+000027a0: 2528 7079 3829 7320 3d20 2528 7079 3229  %(py8)s = %(py2)
+000027b0: 730a 7b25 2870 7932 2973 203d 2025 2870  s.{%(py2)s = %(p
+000027c0: 7930 2973 2e69 7363 6c6f 7365 0a7d 2825  y0)s.isclose.}(%
+000027d0: 2870 7934 2973 2c20 2528 7079 3629 7329  (py4)s, %(py6)s)
+000027e0: 0a7d 2905 7247 0000 0072 4800 0000 7223  .}).rG...rH...r#
+000027f0: 0000 0072 2400 0000 7225 0000 007a 4861  ...r$...r%...zHa
+00002800: 7373 6572 7420 2528 7079 3729 730a 7b25  ssert %(py7)s.{%
+00002810: 2870 7937 2973 203d 2025 2870 7933 2973  (py7)s = %(py3)s
+00002820: 0a7b 2528 7079 3329 7320 3d20 2528 7079  .{%(py3)s = %(py
+00002830: 3129 732e 6571 7561 6c73 0a7d 2825 2870  1)s.equals.}(%(p
+00002840: 7935 2973 290a 7d29 0472 2100 0000 7222  y5)s).}).r!...r"
+00002850: 0000 00da 0370 7935 da03 7079 37e9 0100  .....py5..py7...
+00002860: 0000 e902 0000 00e9 0300 0000 679a 9999  ............g...
+00002870: 9999 99f1 3f67 9a99 9999 9999 0140 6766  ....?g.......@gf
+00002880: 6666 6666 660a 40e9 6400 0000 e9c8 0000  fffff.@.d.......
+00002890: 0069 2c01 0000 6779 e926 3108 0059 4067  .i,...gy.&1..Y@g
+000028a0: c7ba b88d 0600 6940 6710 e9b7 af03 c072  ......i@g......r
+000028b0: 40e9 0400 0000 e905 0000 00a9 0372 4c00  @............rL.
+000028c0: 0000 7251 0000 0072 5200 0000 4629 01da  ..rQ...rR...F)..
+000028d0: 0372 6563 7201 0000 007a 8461 7373 6572  .recr....z.asser
+000028e0: 7420 2528 7079 3132 2973 0a7b 2528 7079  t %(py12)s.{%(py
+000028f0: 3132 2973 203d 2025 2870 7931 3029 730a  12)s = %(py10)s.
+00002900: 7b25 2870 7931 3029 7320 3d20 2528 7079  {%(py10)s = %(py
+00002910: 3829 730a 7b25 2870 7938 2973 203d 2025  8)s.{%(py8)s = %
+00002920: 2870 7932 2973 0a7b 2528 7079 3229 7320  (py2)s.{%(py2)s 
+00002930: 3d20 2528 7079 3029 732e 6571 7561 6c0a  = %(py0)s.equal.
+00002940: 7d28 2528 7079 3429 732c 2025 2870 7936  }(%(py4)s, %(py6
+00002950: 2973 290a 7d2e 616c 6c0a 7d28 290a 7d54  )s).}.all.}().}T
+00002960: 7a92 6173 7365 7274 2025 2870 7931 3529  z.assert %(py15)
+00002970: 730a 7b25 2870 7931 3529 7320 3d20 2528  s.{%(py15)s = %(
+00002980: 7079 3133 2973 0a7b 2528 7079 3133 2973  py13)s.{%(py13)s
+00002990: 203d 2025 2870 7931 3129 730a 7b25 2870   = %(py11)s.{%(p
+000029a0: 7931 3129 7320 3d20 2528 7079 3229 730a  y11)s = %(py2)s.
+000029b0: 7b25 2870 7932 2973 203d 2025 2870 7930  {%(py2)s = %(py0
+000029c0: 2973 2e65 7175 616c 0a7d 2825 2870 7934  )s.equal.}(%(py4
+000029d0: 2973 2c20 2825 2870 7936 2973 202b 2025  )s, (%(py6)s + %
+000029e0: 2870 7938 2973 2929 0a7d 2e61 6c6c 0a7d  (py8)s)).}.all.}
+000029f0: 2829 0a7d 2908 7247 0000 0072 4800 0000  ().}).rG...rH...
+00002a00: 7223 0000 0072 2400 0000 7225 0000 00da  r#...r$...r%....
+00002a10: 0470 7931 31da 0470 7931 33da 0470 7931  .py11..py13..py1
+00002a20: 357a 8561 7373 6572 7420 2528 7079 3133  5z.assert %(py13
+00002a30: 2973 0a7b 2528 7079 3133 2973 203d 2025  )s.{%(py13)s = %
+00002a40: 2870 7931 3129 730a 7b25 2870 7931 3129  (py11)s.{%(py11)
+00002a50: 7320 3d20 2528 7079 3929 730a 7b25 2870  s = %(py9)s.{%(p
+00002a60: 7939 2973 203d 2025 2870 7932 2973 0a7b  y9)s = %(py2)s.{
+00002a70: 2528 7079 3229 7320 3d20 2528 7079 3029  %(py2)s = %(py0)
+00002a80: 732e 6571 7561 6c0a 7d28 2528 7079 3429  s.equal.}(%(py4)
+00002a90: 732c 202d 2528 7079 3629 7329 0a7d 2e61  s, -%(py6)s).}.a
+00002aa0: 6c6c 0a7d 2829 0a7d 2907 7247 0000 0072  ll.}().}).rG...r
+00002ab0: 4800 0000 7223 0000 0072 2400 0000 da03  H...r#...r$.....
+00002ac0: 7079 3972 5e00 0000 725f 0000 0069 4042  py9r^...r_...i@B
+00002ad0: 0f00 7a82 6173 7365 7274 2025 2870 7931  ..z.assert %(py1
+00002ae0: 3129 730a 7b25 2870 7931 3129 7320 3d20  1)s.{%(py11)s = 
+00002af0: 2528 7079 3929 730a 7b25 2870 7939 2973  %(py9)s.{%(py9)s
+00002b00: 203d 2025 2870 7937 2973 0a7b 2528 7079   = %(py7)s.{%(py
+00002b10: 3729 7320 3d20 2528 7079 3229 730a 7b25  7)s = %(py2)s.{%
+00002b20: 2870 7932 2973 203d 2025 2870 7930 2973  (py2)s = %(py0)s
+00002b30: 2e65 7175 616c 0a7d 2825 2870 7934 2973  .equal.}(%(py4)s
+00002b40: 2c20 2528 7079 3529 7329 0a7d 2e61 6c6c  , %(py5)s).}.all
+00002b50: 0a7d 2829 0a7d da07 6e65 775f 6d7a 7329  .}().}..new_mzs)
+00002b60: 0772 4700 0000 7248 0000 0072 2300 0000  .rG...rH...r#...
+00002b70: 7253 0000 0072 5400 0000 7261 0000 0072  rS...rT...ra...r
+00002b80: 5e00 0000 7aa0 6173 7365 7274 2025 2870  ^...z.assert %(p
+00002b90: 7931 3829 730a 7b25 2870 7931 3829 7320  y18)s.{%(py18)s 
+00002ba0: 3d20 2528 7079 3136 2973 0a7b 2528 7079  = %(py16)s.{%(py
+00002bb0: 3136 2973 203d 2025 2870 7931 3429 730a  16)s = %(py14)s.
+00002bc0: 7b25 2870 7931 3429 7320 3d20 2528 7079  {%(py14)s = %(py
+00002bd0: 3229 730a 7b25 2870 7932 2973 203d 2025  2)s.{%(py2)s = %
+00002be0: 2870 7930 2973 2e65 7175 616c 0a7d 2825  (py0)s.equal.}(%
+00002bf0: 2870 7934 2973 2c20 2828 2d25 2870 7936  (py4)s, ((-%(py6
+00002c00: 2973 202a 2025 2870 7939 2973 2920 2f20  )s * %(py9)s) / 
+00002c10: 2528 7079 3131 2973 2929 0a7d 2e61 6c6c  %(py11)s)).}.all
+00002c20: 0a7d 2829 0a7d 2909 7247 0000 0072 4800  .}().}).rG...rH.
+00002c30: 0000 7223 0000 0072 2400 0000 7261 0000  ..r#...r$...ra..
+00002c40: 0072 5e00 0000 724a 0000 0072 4b00 0000  .r^...rJ...rK...
+00002c50: da04 7079 3138 2920 722a 0000 0072 2b00  ..py18) r*...r+.
+00002c60: 0000 5a0b 6765 6e5f 616e 6368 6f72 735a  ..Z.gen_anchorsZ
+00002c70: 0761 6e63 686f 7273 7230 0000 0072 3100  .anchorsr0...r1.
+00002c80: 0000 7232 0000 0072 3600 0000 7237 0000  ..r2...r6...r7..
+00002c90: 005a 0a67 656e 5f63 6f61 7273 6572 4600  .Z.gen_coarserF.
+00002ca0: 0000 da05 6571 7561 6c5a 0e63 6f61 7273  ....equalZ.coars
+00002cb0: 655f 6d61 7463 6865 73da 0676 616c 7565  e_matches..value
+00002cc0: 73da 0361 6c6c 7233 0000 0072 3400 0000  s..allr3...r4...
+00002cd0: 7235 0000 005a 0b67 656e 5f73 6361 6c65  r5...Z.gen_scale
+00002ce0: 7273 da07 7363 616c 6572 73da 0769 7363  rs..scalers..isc
+00002cf0: 6c6f 7365 5a11 6765 6e5f 7363 616c 6564  loseZ.gen_scaled
+00002d00: 5f76 616c 7565 73da 0d73 6361 6c65 645f  _values..scaled_
+00002d10: 7661 6c75 6573 5a08 6765 6e5f 7374 6473  valuesZ.gen_stds
+00002d20: 5a04 7374 6473 5a0b 6765 6e5f 6d61 7463  Z.stdsZ.gen_matc
+00002d30: 6865 73da 076d 6174 6368 6573 da06 6571  hes..matches..eq
+00002d40: 7561 6c73 da05 616c 6967 6eda 0c63 616c  uals..align..cal
+00002d50: 635f 7363 616c 6572 735a 0b73 6574 5f73  c_scalersZ.set_s
+00002d60: 6361 6c65 7273 da03 7a69 7029 2872 0e00  calers..zip)(r..
+00002d70: 0000 720f 0000 0072 1500 0000 7240 0000  ..r....r....r@..
+00002d80: 0072 3800 0000 da0b 4070 795f 6173 7365  .r8.....@py_asse
+00002d90: 7274 3372 3b00 0000 da0b 4070 795f 666f  rt3r;.....@py_fo
+00002da0: 726d 6174 35da 0b40 7079 5f66 6f72 6d61  rmat5..@py_forma
+00002db0: 7437 da0b 4070 795f 6173 7365 7274 3172  t7..@py_assert1r
+00002dc0: 3900 0000 723a 0000 00da 0b40 7079 5f61  9...r:.....@py_a
+00002dd0: 7373 6572 7439 da0c 4070 795f 6173 7365  ssert9..@py_asse
+00002de0: 7274 3131 da0c 4070 795f 6173 7365 7274  rt11..@py_assert
+00002df0: 3133 da0c 4070 795f 6173 7365 7274 3135  13..@py_assert15
+00002e00: 5a0c 4070 795f 666f 726d 6174 3137 5a0b  Z.@py_format17Z.
+00002e10: 6870 315f 7363 616c 6572 735a 0f70 6963  hp1_scalersZ.pic
+00002e20: 6b6c 6564 5f73 6361 6c65 7273 da0c 4070  kled_scalers..@p
+00002e30: 795f 666f 726d 6174 3133 7269 0000 005a  y_format13ri...Z
+00002e40: 0e70 6963 6b6c 6564 5f76 616c 7565 7372  .pickled_valuesr
+00002e50: 3c00 0000 da0b 4070 795f 6173 7365 7274  <.....@py_assert
+00002e60: 34da 0b40 7079 5f61 7373 6572 7436 da0b  4..@py_assert6..
+00002e70: 4070 795f 666f 726d 6174 38da 0272 745a  @py_format8..rtZ
+00002e80: 026d 7a5a 0969 6e74 656e 7369 7479 5a09  .mzZ.intensityZ.
+00002e90: 615f 7363 616c 6572 73da 0c40 7079 5f61  a_scalers..@py_a
+00002ea0: 7373 6572 7431 30da 0c40 7079 5f61 7373  ssert10..@py_ass
+00002eb0: 6572 7431 32da 0c40 7079 5f61 7373 6572  ert12..@py_asser
+00002ec0: 7431 345a 0c40 7079 5f66 6f72 6d61 7431  t14Z.@py_format1
+00002ed0: 36da 0b40 7079 5f61 7373 6572 7438 5a0c  6..@py_assert8Z.
+00002ee0: 4070 795f 666f 726d 6174 3134 7262 0000  @py_format14rb..
+00002ef0: 005a 0c40 7079 5f66 6f72 6d61 7431 32da  .Z.@py_format12.
+00002f00: 0c40 7079 5f61 7373 6572 7431 375a 0c40  .@py_assert17Z.@
+00002f10: 7079 5f66 6f72 6d61 7431 3972 0600 0000  py_format19r....
+00002f20: 7206 0000 0072 0700 0000 da16 7465 7374  r....r......test
+00002f30: 5f61 6c69 676e 6d65 6e74 5f6d 6574 686f  _alignment_metho
+00002f40: 6473 7c00 0000 7388 0200 0000 0514 0308  ds|...s.........
+00002f50: 010a 000a 0008 0004 002c 000c 000e 000c  .........,......
+00002f60: 010a 000a 0008 0004 002c 000c 000e 000c  .........,......
+00002f70: 0308 0106 000e 0006 000e 0006 000a 0006  ................
+00002f80: 0006 0006 0070 000e 0020 0608 010e 010e  .....p... ......
+00002f90: 0106 000c 000c 000a 0006 0006 0006 0060  ...............`
+00002fa0: 000e 0018 0106 000c 000c 000a 0006 0006  ................
+00002fb0: 0006 0060 000e 0018 0106 000c 000c 000a  ...`............
+00002fc0: 0006 0006 0006 0060 000e 0018 0106 000c  .......`........
+00002fd0: 000c 000a 0006 0006 0006 0060 000e 0018  ...........`....
+00002fe0: 0106 000c 000c 000a 0006 0006 0006 0060  ...............`
+00002ff0: 000e 0018 0306 000c 000c 000a 0006 0006  ................
+00003000: 0006 0060 000e 0018 0508 010e 010e 0106  ...`............
+00003010: 0008 0008 000a 0006 0006 0006 0060 000e  .............`..
+00003020: 0018 0106 0008 0008 000a 0006 0006 0006  ................
+00003030: 0060 000e 0018 0106 0008 0008 000a 0006  .`..............
+00003040: 0006 0006 0060 000e 0018 0308 0106 0012  .....`..........
+00003050: 0012 000a 0006 0050 000e 0010 0106 0012  .......P........
+00003060: 0012 000a 0006 0050 000e 0010 0106 0012  .......P........
+00003070: 0012 000a 0006 0050 000e 0010 0508 010e  .......P........
+00003080: 0006 000e 0008 0006 002a 000e 0010 0314  .........*......
+00003090: 0108 0318 0118 0118 0214 0104 0202 0102  ................
+000030a0: 0106 0106 0106 fd04 ff02 ff02 0902 f606  ................
+000030b0: 0c08 010e 0106 000c 0008 000a 0006 0006  ................
+000030c0: 0006 0060 000e 0018 0106 000c 0008 000a  ...`............
+000030d0: 0006 0006 0006 0060 000e 0018 0106 000c  .......`........
+000030e0: 0008 000a 0006 0006 0006 0060 000e 0018  ...........`....
+000030f0: 0106 000c 0008 000a 0006 0006 0006 0060  ...............`
+00003100: 000e 0018 0106 000c 0008 000a 0006 0006  ................
+00003110: 0006 0060 000e 0018 0106 000c 0008 000a  ...`............
+00003120: 0006 0006 0006 0060 000e 0018 0314 0104  .......`........
+00003130: 0202 0102 0106 0106 0106 fd04 ff02 ff02  ................
+00003140: 0902 f606 0c08 010e 0106 000c 0008 0008  ................
+00003150: 0008 000a 0006 0006 0006 0068 000e 0020  ...........h... 
+00003160: 0106 000c 0008 0006 000a 0006 0006 0006  ................
+00003170: 0060 000e 001c 011c 0106 000c 000a 0006  .`..............
+00003180: 0006 0006 007e 000e 0014 0106 000c 0008  .....~..........
+00003190: 0006 0008 0008 0008 000a 0006 0006 0006  ................
+000031a0: 008e 000e 0028 0106 000c 0008 0008 0008  .....(..........
+000031b0: 000a 0006 0006 0006 0068 000e 0020 0106  .........h... ..
+000031c0: 000c 0008 0006 000a 0006 0006 0006 0060  ...............`
+000031d0: 000e 0072 8100 0000 6300 0000 0000 0000  ...r....c.......
+000031e0: 0000 0000 0005 0000 000a 0000 0043 0000  .............C..
+000031f0: 0073 d600 0000 7400 a001 6401 6402 6403  .s....t...d.d.d.
+00003200: 6404 9c03 6405 6406 6407 6404 9c03 6408  d...d.d.d.d...d.
+00003210: 6409 640a 6404 9c03 6401 6401 6401 6404  d.d.d...d.d.d.d.
+00003220: 9c03 6401 6401 6401 6404 9c03 a105 7d00  ..d.d.d.d.....}.
+00003230: 7402 6a03 7d01 640b 7d02 7c01 7c00 7c02  t.j.}.d.}.|.|.|.
+00003240: 8302 7d03 7c03 73c6 640c 640d 7404 a005  ..}.|.s.d.d.t...
+00003250: a100 6b06 736a 7406 a007 7402 a101 7274  ..k.sjt...t...rt
+00003260: 7406 a008 7402 a101 6e02 640d 7406 a008  t...t...n.d.t...
+00003270: 7c01 a101 640e 7404 a005 a100 6b06 7394  |...d.t.....k.s.
+00003280: 7406 a007 7c00 a101 729e 7406 a008 7c00  t...|...r.t...|.
+00003290: a101 6e02 640e 7406 a008 7c02 a101 7406  ..n.d.t...|...t.
+000032a0: a008 7c03 a101 640f 9c05 1600 7d04 7409  ..|...d.....}.t.
+000032b0: 7406 a00a 7c04 a101 8301 8201 6410 0400  t...|.......d...
+000032c0: 7d01 0400 7d02 7d03 6410 5300 2911 7a20  }...}.}.d.S.).z 
+000032d0: 0a20 2020 2054 6573 7420 7363 6f72 6520  .    Test score 
+000032e0: 6361 6c63 756c 6174 696f 6e0a 2020 2020  calculation.    
+000032f0: 7255 0000 0072 5900 0000 7258 0000 0072  rU...rY...rX...r
+00003300: 5c00 0000 7256 0000 0067 b22e 6ea3 0100  \...rV...g..n...
+00003310: 6940 69e8 0300 00da 066c 696e 6561 72da  i@i......linear.
+00003320: 0370 706d da05 6c6f 6731 3072 5700 0000  .ppm..log10rW...
+00003330: 7a52 6173 7365 7274 2025 2870 7937 2973  zRassert %(py7)s
+00003340: 0a7b 2528 7079 3729 7320 3d20 2528 7079  .{%(py7)s = %(py
+00003350: 3229 730a 7b25 2870 7932 2973 203d 2025  2)s.{%(py2)s = %
+00003360: 2870 7930 2973 2e69 7363 6c6f 7365 0a7d  (py0)s.isclose.}
+00003370: 2825 2870 7933 2973 2c20 2528 7079 3529  (%(py3)s, %(py5)
+00003380: 7329 0a7d 7246 0000 00da 0573 636f 7265  s).}rF.....score
+00003390: 2905 7247 0000 0072 4800 0000 7222 0000  ).rG...rH...r"..
+000033a0: 0072 5300 0000 7254 0000 004e 290b 722a  .rS...rT...N).r*
+000033b0: 0000 005a 0a63 616c 635f 7363 6f72 6572  ...Z.calc_scorer
+000033c0: 4600 0000 7268 0000 0072 3300 0000 7234  F...rh...r3...r4
+000033d0: 0000 0072 3000 0000 7235 0000 0072 3200  ...r0...r5...r2.
+000033e0: 0000 7236 0000 0072 3700 0000 2905 7285  ..r6...r7...).r.
+000033f0: 0000 0072 7200 0000 7278 0000 0072 7900  ...rr...rx...ry.
+00003400: 0000 727a 0000 0072 0600 0000 7206 0000  ..rz...r....r...
+00003410: 0072 0700 0000 da0f 7465 7374 5f63 616c  .r......test_cal
+00003420: 635f 7363 6f72 65ea 0000 0073 1c00 0000  c_score....s....
+00003430: 0004 0401 0a01 0a01 0a01 0a01 0afb 0407  ................
+00003440: 0600 0400 0a00 0400 6600 0e00 7286 0000  ........f...r...
+00003450: 007a 1469 676e 6f72 653a 696e 7661 6c69  .z.ignore:invali
+00003460: 6420 7661 6c75 6563 0000 0000 0000 0000  d valuec........
+00003470: 0000 0000 0b00 0000 0700 0000 4300 0000  ............C...
+00003480: 731c 0100 0074 00a0 0164 0164 0164 0267  s....t...d.d.d.g
+00003490: 03a1 017d 0074 00a0 0164 0264 0264 0367  ...}.t...d.d.d.g
+000034a0: 03a1 017d 0174 026a 037c 007c 0164 0464  ...}.t.j.|.|.d.d
+000034b0: 0564 068d 0464 0219 007d 0274 00a0 047c  .d...d...}.t...|
+000034c0: 02a1 01a0 05a1 007d 0374 00a0 0674 00a0  .......}.t...t..
+000034d0: 0164 0264 0264 0267 03a1 017c 02a1 02a0  .d.d.d.g...|....
+000034e0: 05a1 007d 0467 007d 057c 037d 067c 0373  ...}.g.}.|.}.|.s
+000034f0: 707c 047d 067c 0690 0173 1064 0764 0864  p|.}.|...s.d.d.d
+00003500: 0974 07a0 08a1 006b 0673 9074 09a0 0a7c  .t.....k.s.t...|
+00003510: 03a1 0172 9a74 09a0 0b7c 03a1 016e 0264  ...r.t...|...n.d
+00003520: 0969 0116 007d 077c 05a0 0c7c 07a1 0101  .i...}.|...|....
+00003530: 007c 0373 e664 0a64 0b64 0c74 07a0 08a1  .|.s.d.d.d.t....
+00003540: 006b 0673 ca74 09a0 0a7c 04a1 0172 d474  .k.s.t...|...r.t
+00003550: 09a0 0b7c 04a1 016e 0264 0c69 0116 007d  ...|...n.d.i...}
+00003560: 087c 05a0 0c7c 08a1 0101 0074 09a0 0d7c  .|...|.....t...|
+00003570: 0564 02a1 0269 0016 007d 0964 0d64 0e7c  .d...i...}.d.d.|
+00003580: 0969 0116 007d 0a74 0e74 09a0 0f7c 0aa1  .i...}.t.t...|..
+00003590: 0183 0182 0164 0f04 007d 067d 0564 0f53  .....d...}.}.d.S
+000035a0: 0029 107a 330a 2020 2020 5375 7070 6c65  .).z3.    Supple
+000035b0: 6d65 6e74 616c 2074 6573 7473 2074 6f20  mental tests to 
+000035c0: 6361 6c63 756c 6174 696e 6720 7363 616c  calculating scal
+000035d0: 6572 730a 2020 2020 7201 0000 0072 5500  ers.    r....rU.
+000035e0: 0000 7256 0000 005a 066c 6f77 6573 7372  ..rV...Z.lowessr
+000035f0: 8200 0000 2902 da09 736d 6f6f 7468 696e  ....)...smoothin
+00003600: 67da 046d 6f64 657a 0725 2870 7932 2973  g..modez.%(py2)s
+00003610: 7248 0000 00da 0861 6c6c 5f6e 616e 737a  rH.....all_nansz
+00003620: 0725 2870 7934 2973 7223 0000 00da 0b69  .%(py4)sr#.....i
+00003630: 735f 6f72 6967 696e 616c 7a0e 6173 7365  s_originalz.asse
+00003640: 7274 2025 2870 7937 2973 7254 0000 004e  rt %(py7)srT...N
+00003650: 2910 7246 0000 00da 0561 7272 6179 722a  ).rF.....arrayr*
+00003660: 0000 0072 6d00 0000 da05 6973 6e61 6e72  ...rm.....isnanr
+00003670: 6600 0000 7268 0000 0072 3300 0000 7234  f...rh...r3...r4
+00003680: 0000 0072 3000 0000 7235 0000 0072 3200  ...r0...r5...r2.
+00003690: 0000 da06 6170 7065 6e64 da0e 5f66 6f72  ....append.._for
+000036a0: 6d61 745f 626f 6f6c 6f70 7236 0000 0072  mat_boolopr6...r
+000036b0: 3700 0000 290b 5a06 785f 7661 6c73 5a06  7...).Z.x_valsZ.
+000036c0: 795f 7661 6c73 da07 7265 7375 6c74 7372  y_vals..resultsr
+000036d0: 8900 0000 728a 0000 0072 7200 0000 7238  ....r....rr...r8
+000036e0: 0000 005a 0b40 7079 5f66 6f72 6d61 7433  ...Z.@py_format3
+000036f0: 7270 0000 00da 0b40 7079 5f66 6f72 6d61  rp.....@py_forma
+00003700: 7436 727a 0000 0072 0600 0000 7206 0000  t6rz...r....r...
+00003710: 0072 0700 0000 da11 7465 7374 5f63 616c  .r......test_cal
+00003720: 635f 7363 616c 6572 73f8 0000 0073 2600  c_scalers....s&.
+00003730: 0000 0008 1001 1001 1601 0e01 1c01 0400  ................
+00003740: 0400 0400 0400 0600 2c00 0a00 0400 2c00  ........,.....,.
+00003750: 0a00 1000 0c00 0e00 7291 0000 0063 0100  ........r....c..
+00003760: 0000 0000 0000 0000 0000 0a00 0000 0a00  ................
+00003770: 0000 4300 0000 73dc 0000 007c 006a 0064  ..C...s....|.j.d
+00003780: 0164 028d 017d 0174 01a0 02a1 007d 027c  .d...}.t.....}.|
+00003790: 02a0 037c 0164 03a1 0201 0074 046a 057d  ...|.d.....t.j.}
+000037a0: 037c 026a 0664 0319 0064 0119 007d 047c  .|.j.d...d...}.|
+000037b0: 0064 0119 007d 057c 037c 047c 0583 027d  .d...}.|.|.|...}
+000037c0: 067c 066a 077d 077c 0783 007d 087c 0873  .|.j.}.|...}.|.s
+000037d0: c064 0464 0574 08a0 09a1 006b 0673 6e74  .d.d.t.....k.snt
+000037e0: 0aa0 0b74 04a1 0172 7874 0aa0 0c74 04a1  ...t...rxt...t..
+000037f0: 016e 0264 0574 0aa0 0c7c 03a1 0174 0aa0  .n.d.t...|...t..
+00003800: 0c7c 04a1 0174 0aa0 0c7c 05a1 0174 0aa0  .|...t...|...t..
+00003810: 0c7c 06a1 0174 0aa0 0c7c 07a1 0174 0aa0  .|...t...|...t..
+00003820: 0c7c 08a1 0164 069c 0716 007d 0974 0d74  .|...d.....}.t.t
+00003830: 0aa0 0e7c 09a1 0183 0182 0164 0704 007d  ...|.......d...}
+00003840: 0304 007d 0404 007d 0504 007d 0604 007d  ...}...}...}...}
+00003850: 077d 0864 0753 0029 087a 420a 2020 2020  .}.d.S.).zB.    
+00003860: 5465 7374 7320 746f 2073 6565 2069 6620  Tests to see if 
+00003870: 696e 7465 6e73 6974 7920 6973 2061 7574  intensity is aut
+00003880: 6f63 616c 6375 6c61 7465 6420 7768 656e  ocalculated when
+00003890: 206d 6973 7369 6e67 0a20 2020 2072 5200   missing.    rR.
+000038a0: 0000 2901 da07 636f 6c75 6d6e 735a 0364  ..)...columnsZ.d
+000038b0: 6633 724e 0000 0072 4600 0000 724f 0000  f3rN...rF...rO..
+000038c0: 004e 290f da04 6472 6f70 722a 0000 0072  .N)...dropr*...r
+000038d0: 2b00 0000 723f 0000 0072 4600 0000 7268  +...r?...rF...rh
+000038e0: 0000 005a 0864 6174 6173 6574 7372 6600  ...Z.datasetsrf.
+000038f0: 0000 7233 0000 0072 3400 0000 7230 0000  ..r3...r4...r0..
+00003900: 0072 3500 0000 7232 0000 0072 3600 0000  .r5...r2...r6...
+00003910: 7237 0000 0029 0a72 1000 0000 5a11 6466  r7...).r....Z.df
+00003920: 5f33 5f6e 6f5f 696e 7465 6e73 6974 7972  _3_no_intensityr
+00003930: 4000 0000 7272 0000 0072 6f00 0000 7239  @...rr...ro...r9
+00003940: 0000 0072 3a00 0000 7273 0000 0072 7400  ...r:...rs...rt.
+00003950: 0000 7277 0000 0072 0600 0000 7206 0000  ..rw...r....r...
+00003960: 0072 0700 0000 da1c 7465 7374 5f61 6464  .r......test_add
+00003970: 696e 675f 696e 7465 6e73 6974 795f 636f  ing_intensity_co
+00003980: 6c75 6d6e 0801 0000 731a 0000 0000 050c  lumn....s.......
+00003990: 0208 010c 0206 000e 0008 000a 0006 0006  ................
+000039a0: 0004 005c 000e 0072 9400 0000 6303 0000  ...\...r....c...
+000039b0: 0000 0000 0000 0000 0010 0000 0008 0000  ................
+000039c0: 0043 0000 0073 1009 0000 6401 6402 6403  .C...s....d.d.d.
+000039d0: 6703 7d03 7400 6a01 7c00 7c01 7c02 7c03  g.}.t.j.|.|.|.|.
+000039e0: 6404 8d04 7d04 7c04 a002 a100 0100 7c04  d...}.|.......|.
+000039f0: 6a03 7d05 7404 7c05 8301 7d06 6401 6402  j.}.t.|...}.d.d.
+00003a00: 6403 6703 7d07 7c06 7c07 6b02 7d08 7c08  d.g.}.|.|.k.}.|.
+00003a10: 73da 7405 a006 6405 7c08 6601 6406 7c06  s.t...d.|.f.d.|.
+00003a20: 7c07 6602 a104 6407 7407 a008 a100 6b06  |.f...d.t.....k.
+00003a30: 7372 7405 a009 7404 a101 727c 7405 a00a  srt...t...r|t...
+00003a40: 7404 a101 6e02 6407 6408 7407 a008 a100  t...n.d.d.t.....
+00003a50: 6b06 7394 7405 a009 7c04 a101 729e 7405  k.s.t...|...r.t.
+00003a60: a00a 7c04 a101 6e02 6408 7405 a00a 7c05  ..|...n.d.t...|.
+00003a70: a101 7405 a00a 7c06 a101 7405 a00a 7c07  ..t...|...t...|.
+00003a80: a101 6409 9c05 1600 7d09 640a 640b 7c09  ..d.....}.d.d.|.
+00003a90: 6901 1600 7d0a 740b 7405 a00c 7c0a a101  i...}.t.t...|...
+00003aa0: 8301 8201 640c 0400 7d05 0400 7d06 0400  ....d...}...}...
+00003ab0: 7d08 7d07 7c04 6a03 6401 1900 7d0b 7404  }.}.|.j.d...}.t.
+00003ac0: 7c0b 8301 7d0c 6402 6403 6702 7d08 7c0c  |...}.d.d.g.}.|.
+00003ad0: 7c08 6b02 7d0d 7c0d 9001 7386 7405 a006  |.k.}.|...s.t...
+00003ae0: 6405 7c0d 6601 640d 7c0c 7c08 6602 a104  d.|.f.d.|.|.f...
+00003af0: 6407 7407 a008 a100 6b06 9001 7340 7405  d.t.....k...s@t.
+00003b00: a009 7404 a101 9001 724a 7405 a00a 7404  ..t.....rJt...t.
+00003b10: a101 6e02 6407 7405 a00a 7c0b a101 7405  ..n.d.t...|...t.
+00003b20: a00a 7c0c a101 7405 a00a 7c08 a101 640e  ..|...t...|...d.
+00003b30: 9c04 1600 7d0e 640f 6410 7c0e 6901 1600  ....}.d.d.|.i...
+00003b40: 7d0f 740b 7405 a00c 7c0f a101 8301 8201  }.t.t...|.......
+00003b50: 640c 0400 7d0b 0400 7d0c 0400 7d0d 7d08  d...}...}...}.}.
+00003b60: 7c04 6a03 6402 1900 7d0b 7404 7c0b 8301  |.j.d...}.t.|...
+00003b70: 7d0c 6401 6403 6702 7d08 7c0c 7c08 6b02  }.d.d.g.}.|.|.k.
+00003b80: 7d0d 7c0d 9002 7332 7405 a006 6405 7c0d  }.|...s2t...d.|.
+00003b90: 6601 640d 7c0c 7c08 6602 a104 6407 7407  f.d.|.|.f...d.t.
+00003ba0: a008 a100 6b06 9001 73ec 7405 a009 7404  ....k...s.t...t.
+00003bb0: a101 9001 72f6 7405 a00a 7404 a101 6e02  ....r.t...t...n.
+00003bc0: 6407 7405 a00a 7c0b a101 7405 a00a 7c0c  d.t...|...t...|.
+00003bd0: a101 7405 a00a 7c08 a101 640e 9c04 1600  ..t...|...d.....
+00003be0: 7d0e 640f 6410 7c0e 6901 1600 7d0f 740b  }.d.d.|.i...}.t.
+00003bf0: 7405 a00c 7c0f a101 8301 8201 640c 0400  t...|.......d...
+00003c00: 7d0b 0400 7d0c 0400 7d0d 7d08 7c04 6a03  }...}...}.}.|.j.
+00003c10: 6403 1900 7d0b 7404 7c0b 8301 7d0c 6401  d...}.t.|...}.d.
+00003c20: 6402 6702 7d08 7c0c 7c08 6b02 7d0d 7c0d  d.g.}.|.|.k.}.|.
+00003c30: 9002 73de 7405 a006 6405 7c0d 6601 640d  ..s.t...d.|.f.d.
+00003c40: 7c0c 7c08 6602 a104 6407 7407 a008 a100  |.|.f...d.t.....
+00003c50: 6b06 9002 7398 7405 a009 7404 a101 9002  k...s.t...t.....
+00003c60: 72a2 7405 a00a 7404 a101 6e02 6407 7405  r.t...t...n.d.t.
+00003c70: a00a 7c0b a101 7405 a00a 7c0c a101 7405  ..|...t...|...t.
+00003c80: a00a 7c08 a101 640e 9c04 1600 7d0e 640f  ..|...d.....}.d.
+00003c90: 6410 7c0e 6901 1600 7d0f 740b 7405 a00c  d.|.i...}.t.t...
+00003ca0: 7c0f a101 8301 8201 640c 0400 7d0b 0400  |.......d...}...
+00003cb0: 7d0c 0400 7d0d 7d08 7400 6a01 7c00 7c01  }...}.}.t.j.|.|.
+00003cc0: 7c02 7c03 6404 8d04 7d04 7c04 a002 6401  |.|.d...}.|...d.
+00003cd0: 6402 6403 6703 a101 0100 7c04 6a03 7d05  d.d.g.....|.j.}.
+00003ce0: 7404 7c05 8301 7d06 6401 6402 6403 6703  t.|...}.d.d.d.g.
+00003cf0: 7d07 7c06 7c07 6b02 7d08 7c08 9003 73d0  }.|.|.k.}.|...s.
+00003d00: 7405 a006 6405 7c08 6601 6406 7c06 7c07  t...d.|.f.d.|.|.
+00003d10: 6602 a104 6407 7407 a008 a100 6b06 9003  f...d.t.....k...
+00003d20: 7364 7405 a009 7404 a101 9003 726e 7405  sdt...t.....rnt.
+00003d30: a00a 7404 a101 6e02 6407 6408 7407 a008  ..t...n.d.d.t...
+00003d40: a100 6b06 9003 738a 7405 a009 7c04 a101  ..k...s.t...|...
+00003d50: 9003 7294 7405 a00a 7c04 a101 6e02 6408  ..r.t...|...n.d.
+00003d60: 7405 a00a 7c05 a101 7405 a00a 7c06 a101  t...|...t...|...
+00003d70: 7405 a00a 7c07 a101 6409 9c05 1600 7d09  t...|...d.....}.
+00003d80: 640a 640b 7c09 6901 1600 7d0a 740b 7405  d.d.|.i...}.t.t.
+00003d90: a00c 7c0a a101 8301 8201 640c 0400 7d05  ..|.......d...}.
+00003da0: 0400 7d06 0400 7d08 7d07 7c04 6a03 6401  ..}...}.}.|.j.d.
+00003db0: 1900 7d0b 7404 7c0b 8301 7d0c 6402 6403  ..}.t.|...}.d.d.
+00003dc0: 6702 7d08 7c0c 7c08 6b02 7d0d 7c0d 9004  g.}.|.|.k.}.|...
+00003dd0: 737c 7405 a006 6405 7c0d 6601 640d 7c0c  s|t...d.|.f.d.|.
+00003de0: 7c08 6602 a104 6407 7407 a008 a100 6b06  |.f...d.t.....k.
+00003df0: 9004 7336 7405 a009 7404 a101 9004 7240  ..s6t...t.....r@
+00003e00: 7405 a00a 7404 a101 6e02 6407 7405 a00a  t...t...n.d.t...
+00003e10: 7c0b a101 7405 a00a 7c0c a101 7405 a00a  |...t...|...t...
+00003e20: 7c08 a101 640e 9c04 1600 7d0e 640f 6410  |...d.....}.d.d.
+00003e30: 7c0e 6901 1600 7d0f 740b 7405 a00c 7c0f  |.i...}.t.t...|.
+00003e40: a101 8301 8201 640c 0400 7d0b 0400 7d0c  ......d...}...}.
+00003e50: 0400 7d0d 7d08 7c04 6a03 6402 1900 7d0b  ..}.}.|.j.d...}.
+00003e60: 7404 7c0b 8301 7d0c 6401 6403 6702 7d08  t.|...}.d.d.g.}.
+00003e70: 7c0c 7c08 6b02 7d0d 7c0d 9005 7328 7405  |.|.k.}.|...s(t.
+00003e80: a006 6405 7c0d 6601 640d 7c0c 7c08 6602  ..d.|.f.d.|.|.f.
+00003e90: a104 6407 7407 a008 a100 6b06 9004 73e2  ..d.t.....k...s.
+00003ea0: 7405 a009 7404 a101 9004 72ec 7405 a00a  t...t.....r.t...
+00003eb0: 7404 a101 6e02 6407 7405 a00a 7c0b a101  t...n.d.t...|...
+00003ec0: 7405 a00a 7c0c a101 7405 a00a 7c08 a101  t...|...t...|...
+00003ed0: 640e 9c04 1600 7d0e 640f 6410 7c0e 6901  d.....}.d.d.|.i.
+00003ee0: 1600 7d0f 740b 7405 a00c 7c0f a101 8301  ..}.t.t...|.....
+00003ef0: 8201 640c 0400 7d0b 0400 7d0c 0400 7d0d  ..d...}...}...}.
+00003f00: 7d08 7c04 6a03 6403 1900 7d0b 7404 7c0b  }.|.j.d...}.t.|.
+00003f10: 8301 7d0c 6401 6402 6702 7d08 7c0c 7c08  ..}.d.d.g.}.|.|.
+00003f20: 6b02 7d0d 7c0d 9005 73d4 7405 a006 6405  k.}.|...s.t...d.
+00003f30: 7c0d 6601 640d 7c0c 7c08 6602 a104 6407  |.f.d.|.|.f...d.
+00003f40: 7407 a008 a100 6b06 9005 738e 7405 a009  t.....k...s.t...
+00003f50: 7404 a101 9005 7298 7405 a00a 7404 a101  t.....r.t...t...
+00003f60: 6e02 6407 7405 a00a 7c0b a101 7405 a00a  n.d.t...|...t...
+00003f70: 7c0c a101 7405 a00a 7c08 a101 640e 9c04  |...t...|...d...
+00003f80: 1600 7d0e 640f 6410 7c0e 6901 1600 7d0f  ..}.d.d.|.i...}.
+00003f90: 740b 7405 a00c 7c0f a101 8301 8201 640c  t.t...|.......d.
+00003fa0: 0400 7d0b 0400 7d0c 0400 7d0d 7d08 7400  ..}...}...}.}.t.
+00003fb0: 6a01 7c00 7c01 7c02 7c03 6404 8d04 7d04  j.|.|.|.|.d...}.
+00003fc0: 7c04 a002 6401 a101 0100 7c04 6a03 7d05  |...d.....|.j.}.
+00003fd0: 7404 7c05 8301 7d06 6401 6701 7d07 7c06  t.|...}.d.g.}.|.
+00003fe0: 7c07 6b02 7d08 7c08 9006 73bc 7405 a006  |.k.}.|...s.t...
+00003ff0: 6405 7c08 6601 6406 7c06 7c07 6602 a104  d.|.f.d.|.|.f...
+00004000: 6407 7407 a008 a100 6b06 9006 7350 7405  d.t.....k...sPt.
+00004010: a009 7404 a101 9006 725a 7405 a00a 7404  ..t.....rZt...t.
+00004020: a101 6e02 6407 6408 7407 a008 a100 6b06  ..n.d.d.t.....k.
+00004030: 9006 7376 7405 a009 7c04 a101 9006 7280  ..svt...|.....r.
+00004040: 7405 a00a 7c04 a101 6e02 6408 7405 a00a  t...|...n.d.t...
+00004050: 7c05 a101 7405 a00a 7c06 a101 7405 a00a  |...t...|...t...
+00004060: 7c07 a101 6409 9c05 1600 7d09 640a 640b  |...d.....}.d.d.
+00004070: 7c09 6901 1600 7d0a 740b 7405 a00c 7c0a  |.i...}.t.t...|.
+00004080: a101 8301 8201 640c 0400 7d05 0400 7d06  ......d...}...}.
+00004090: 0400 7d08 7d07 7c04 6a03 6401 1900 7d0b  ..}.}.|.j.d...}.
+000040a0: 7404 7c0b 8301 7d0c 6402 6403 6702 7d08  t.|...}.d.d.g.}.
+000040b0: 7c0c 7c08 6b02 7d0d 7c0d 9007 7368 7405  |.|.k.}.|...sht.
+000040c0: a006 6405 7c0d 6601 640d 7c0c 7c08 6602  ..d.|.f.d.|.|.f.
+000040d0: a104 6407 7407 a008 a100 6b06 9007 7322  ..d.t.....k...s"
+000040e0: 7405 a009 7404 a101 9007 722c 7405 a00a  t...t.....r,t...
+000040f0: 7404 a101 6e02 6407 7405 a00a 7c0b a101  t...n.d.t...|...
+00004100: 7405 a00a 7c0c a101 7405 a00a 7c08 a101  t...|...t...|...
+00004110: 640e 9c04 1600 7d0e 640f 6410 7c0e 6901  d.....}.d.d.|.i.
+00004120: 1600 7d0f 740b 7405 a00c 7c0f a101 8301  ..}.t.t...|.....
+00004130: 8201 640c 0400 7d0b 0400 7d0c 0400 7d0d  ..d...}...}...}.
+00004140: 7d08 7400 6a01 7c00 7c01 7c02 7c03 6404  }.t.j.|.|.|.|.d.
+00004150: 8d04 7d04 7c04 a002 6401 6402 a102 0100  ..}.|...d.d.....
+00004160: 7c04 6a03 7d05 7404 7c05 8301 7d06 6401  |.j.}.t.|...}.d.
+00004170: 6701 7d07 7c06 7c07 6b02 7d08 7c08 9008  g.}.|.|.k.}.|...
+00004180: 7352 7405 a006 6405 7c08 6601 6406 7c06  sRt...d.|.f.d.|.
+00004190: 7c07 6602 a104 6407 7407 a008 a100 6b06  |.f...d.t.....k.
+000041a0: 9007 73e6 7405 a009 7404 a101 9007 72f0  ..s.t...t.....r.
+000041b0: 7405 a00a 7404 a101 6e02 6407 6408 7407  t...t...n.d.d.t.
+000041c0: a008 a100 6b06 9008 730c 7405 a009 7c04  ....k...s.t...|.
+000041d0: a101 9008 7216 7405 a00a 7c04 a101 6e02  ....r.t...|...n.
+000041e0: 6408 7405 a00a 7c05 a101 7405 a00a 7c06  d.t...|...t...|.
+000041f0: a101 7405 a00a 7c07 a101 6409 9c05 1600  ..t...|...d.....
+00004200: 7d09 640a 640b 7c09 6901 1600 7d0a 740b  }.d.d.|.i...}.t.
+00004210: 7405 a00c 7c0a a101 8301 8201 640c 0400  t...|.......d...
+00004220: 7d05 0400 7d06 0400 7d08 7d07 7c04 6a03  }...}...}.}.|.j.
+00004230: 6401 1900 7d0b 7404 7c0b 8301 7d0c 6402  d...}.t.|...}.d.
+00004240: 6701 7d08 7c0c 7c08 6b02 7d0d 7c0d 9008  g.}.|.|.k.}.|...
+00004250: 73fc 7405 a006 6405 7c0d 6601 640d 7c0c  s.t...d.|.f.d.|.
+00004260: 7c08 6602 a104 6407 7407 a008 a100 6b06  |.f...d.t.....k.
+00004270: 9008 73b6 7405 a009 7404 a101 9008 72c0  ..s.t...t.....r.
+00004280: 7405 a00a 7404 a101 6e02 6407 7405 a00a  t...t...n.d.t...
+00004290: 7c0b a101 7405 a00a 7c0c a101 7405 a00a  |...t...|...t...
+000042a0: 7c08 a101 640e 9c04 1600 7d0e 640f 6410  |...d.....}.d.d.
+000042b0: 7c0e 6901 1600 7d0f 740b 7405 a00c 7c0f  |.i...}.t.t...|.
+000042c0: a101 8301 8201 640c 0400 7d0b 0400 7d0c  ......d...}...}.
+000042d0: 0400 7d0d 7d08 640c 5300 2911 7a52 0a20  ..}.}.d.S.).zR. 
+000042e0: 2020 2054 6573 7473 2074 6865 2077 7261     Tests the wra
+000042f0: 7070 6572 7320 7768 6963 6820 636f 6e74  ppers which cont
+00004300: 726f 6c20 7468 6520 696e 6e65 7220 616e  rol the inner an
+00004310: 6420 6f75 7465 7220 6461 7461 6672 616d  d outer datafram
+00004320: 6520 666f 7220 6c6f 6f70 730a 2020 2020  e for loops.    
+00004330: 7242 0000 0072 4300 0000 5a03 4850 3372  rB...rC...Z.HP3r
+00004340: 1800 0000 7244 0000 0029 017a 4d25 2870  ....rD...).zM%(p
+00004350: 7935 2973 0a7b 2528 7079 3529 7320 3d20  y5)s.{%(py5)s = 
+00004360: 2528 7079 3029 7328 2528 7079 3329 730a  %(py0)s(%(py3)s.
+00004370: 7b25 2870 7933 2973 203d 2025 2870 7931  {%(py3)s = %(py1
+00004380: 2973 2e6d 6174 6368 6573 0a7d 290a 7d20  )s.matches.}).} 
+00004390: 3d3d 2025 2870 7938 2973 da04 6c69 7374  == %(py8)s..list
+000043a0: 7240 0000 0029 0572 4700 0000 7221 0000  r@...).rG...r!..
+000043b0: 0072 2200 0000 7253 0000 0072 2500 0000  .r"...rS...r%...
+000043c0: 7226 0000 0072 2700 0000 4e29 017a 3025  r&...r'...N).z0%
+000043d0: 2870 7934 2973 0a7b 2528 7079 3429 7320  (py4)s.{%(py4)s 
+000043e0: 3d20 2528 7079 3029 7328 2528 7079 3229  = %(py0)s(%(py2)
+000043f0: 7329 0a7d 203d 3d20 2528 7079 3729 7329  s).} == %(py7)s)
+00004400: 0472 4700 0000 7248 0000 0072 2300 0000  .rG...rH...r#...
+00004410: 7254 0000 007a 0e61 7373 6572 7420 2528  rT...z.assert %(
+00004420: 7079 3929 7372 6100 0000 290d 722a 0000  py9)sra...).r*..
+00004430: 0072 2b00 0000 726c 0000 0072 6a00 0000  .r+...rl...rj...
+00004440: 7295 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
+00004450: 3300 0000 7234 0000 0072 3500 0000 7232  3...r4...r5...r2
+00004460: 0000 0072 3600 0000 7237 0000 0029 1072  ...r6...r7...).r
+00004470: 0e00 0000 720f 0000 0072 1000 0000 7219  ....r....r....r.
+00004480: 0000 0072 4000 0000 723b 0000 0072 7800  ...r@...r;...rx.
+00004490: 0000 723a 0000 0072 7900 0000 723c 0000  ..r:...ry...r<..
+000044a0: 0072 3d00 0000 7272 0000 0072 6f00 0000  .r=...rr...ro...
+000044b0: 7239 0000 0072 7a00 0000 5a0c 4070 795f  r9...rz...Z.@py_
+000044c0: 666f 726d 6174 3130 7206 0000 0072 0600  format10r....r..
+000044d0: 0000 7207 0000 00da 1674 6573 745f 6461  ..r......test_da
+000044e0: 7461 7365 745f 7365 6c65 6374 696f 6e15  taset_selection.
+000044f0: 0100 0073 ea00 0000 0005 0a01 1201 0801  ...s............
+00004500: 0600 0800 0a00 0800 0400 7800 0c00 0e00  ..........x.....
+00004510: 1001 0a00 0800 0800 0800 0600 5a00 0c00  ............Z...
+00004520: 0e00 1001 0a00 0800 0800 0800 0600 5a00  ..............Z.
+00004530: 0c00 0e00 1001 0a00 0800 0800 0800 0600  ................
+00004540: 5a00 0c00 0e00 1003 1201 1001 0600 0800  Z...............
+00004550: 0a00 0800 0600 8000 0c00 0e00 1001 0a00  ................
+00004560: 0800 0800 0800 0600 5a00 0c00 0e00 1001  ........Z.......
+00004570: 0a00 0800 0800 0800 0600 5a00 0c00 0e00  ..........Z.....
+00004580: 1001 0a00 0800 0800 0800 0600 5a00 0c00  ............Z...
+00004590: 0e00 1003 1201 0a01 0600 0800 0600 0800  ................
+000045a0: 0600 8000 0c00 0e00 1001 0a00 0800 0800  ................
+000045b0: 0800 0600 5a00 0c00 0e00 1003 1201 0c01  ....Z...........
+000045c0: 0600 0800 0600 0800 0600 8000 0c00 0e00  ................
+000045d0: 1001 0a00 0800 0600 0800 0600 5a00 0c00  ............Z...
+000045e0: 0e00 7296 0000 0029 23da 075f 5f64 6f63  ..r....)#..__doc
+000045f0: 5f5f da08 6275 696c 7469 6e73 7233 0000  __..builtinsr3..
+00004600: 00da 195f 7079 7465 7374 2e61 7373 6572  ..._pytest.asser
+00004610: 7469 6f6e 2e72 6577 7269 7465 da09 6173  tion.rewrite..as
+00004620: 7365 7274 696f 6eda 0772 6577 7269 7465  sertion..rewrite
+00004630: 7230 0000 00da 0770 6174 686c 6962 7202  r0.....pathlibr.
+00004640: 0000 0072 1200 0000 722c 0000 00da 056e  ...r....r,.....n
+00004650: 756d 7079 7246 0000 00da 0670 616e 6461  umpyrF.....panda
+00004660: 7372 0c00 0000 5a0c 626d 7870 2e65 636c  sr....Z.bmxp.ecl
+00004670: 6970 7365 da07 6563 6c69 7073 6572 2a00  ipse..eclipser*.
+00004680: 0000 da07 6669 7874 7572 6572 0800 0000  ....fixturer....
+00004690: 7209 0000 0072 0a00 0000 720e 0000 0072  r....r....r....r
+000046a0: 0f00 0000 7210 0000 0072 1500 0000 723e  ....r....r....r>
+000046b0: 0000 0072 4100 0000 7281 0000 0072 8600  ...rA...r....r..
+000046c0: 0000 da04 6d61 726b da0e 6669 6c74 6572  ....mark..filter
+000046d0: 7761 726e 696e 6773 7291 0000 0072 9400  warningsr....r..
+000046e0: 0000 7296 0000 0072 0600 0000 7206 0000  ..r....r....r...
+000046f0: 0072 0600 0000 7207 0000 00da 083c 6d6f  .r....r......<mo
+00004700: 6475 6c65 3e02 0000 0073 3c00 0000 0403  dule>....s<.....
+00004710: 0800 1200 0c01 0801 0801 0801 0801 0c03  ................
+00004720: 0601 0a07 0601 0a07 0601 0a07 0601 0a07  ................
+00004730: 0601 0a07 0601 0a07 0601 0a0b 081b 0818  ................
+00004740: 086e 080e 0a01 0a0f 080d                 .n........
```

### Comparing `bmxp-0.0.9/tests/example1.csv` & `bmxp-0.1.0/tests/example1.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.9/tests/mseclipse.pickle` & `bmxp-0.1.0/tests/mseclipse.pickle`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.9/tests/test1.csv` & `bmxp-0.1.0/tests/test1.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.9/tests/test2.csv` & `bmxp-0.1.0/tests/test2.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.9/tests/test3.csv` & `bmxp-0.1.0/tests/test3.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.9/tests/test_gravity.csv` & `bmxp-0.1.0/tests/test_gravity.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.9/tests/test_gravity.py` & `bmxp-0.1.0/tests/test_gravity.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # pylint: disable=redefined-outer-name
 """
 Tests for Gravity
 """
+from pathlib import Path
 import pytest
 import pandas as pd
 from bmxp import gravity
 
 
 @pytest.fixture()
 def filepath():
     """
     First file path for test
     """
-    return "tests/test_gravity.csv"
+    return Path(__file__).parent / "test_gravity.csv"
 
 
 @pytest.fixture()
 def dataframe(filepath):
     """
     First dataframe for test
     """
```

### Comparing `bmxp-0.0.9/tests/test_mseclipse.py` & `bmxp-0.1.0/tests/test_mseclipse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # pylint: disable=redefined-outer-name
 """
 Tests for MSEclipse
 """
-import os
-import sys
+from pathlib import Path
 import pickle
 import pytest
 import numpy as np
 import pandas as pd
 import bmxp.eclipse as ms
 
 
 @pytest.fixture()
 def filepath_1():
     """
     First file path for test
     """
-    print("*****************", os.getcwd())
-    return "tests/test1.csv"
+    return Path(__file__).parent / "test1.csv"
 
 
 @pytest.fixture()
 def filepath_2():
     """
     Second file path for test
     """
-    return "tests/test2.csv"
+    return Path(__file__).parent / "test2.csv"
 
 
 @pytest.fixture()
 def filepath_3():
     """
     Third file path for test
     """
-    return "tests/test3.csv"
+    return Path(__file__).parent / "test3.csv"
 
 
 @pytest.fixture()
 def dataframe_1(filepath_1):
     """
     First dataframe for test
     """
@@ -62,15 +60,17 @@
 
 @pytest.fixture()
 def pickled_ms():
     """
     Load pickled file
     """
     return pickle.load(
-        open("tests/mseclipse.pickle", "rb")  # pylint: disable=consider-using-with
+        open(
+            Path(__file__).parent / "mseclipse.pickle", "rb"
+        )  # pylint: disable=consider-using-with
     )
 
 
 def test_initialize_add(filepath_1, filepath_2, dataframe_1, dataframe_2):
     """
     Test MSAligner initializes or throws errors
     """
@@ -184,15 +184,19 @@
     mz = ms.calc_scalers([100, 200, 300], [100.0005, 200.0008, 300.0009])
     intensity = ms.calc_scalers([2, 3, 4], [3, 4, 5])
 
     a = ms.MSAligner(dataframe_1, dataframe_2, names=["HP1", "HP2"])
     a.set_scalers(
         {
             "HP1": {
-                "HP2": {"RT": zip(*rt), "MZ": zip(*mz), "Intensity": zip(*intensity),}
+                "HP2": {
+                    "RT": zip(*rt),
+                    "MZ": zip(*mz),
+                    "Intensity": zip(*intensity),
+                }
             }
         },
         rec=False,
     )
     a.align()
     a_scalers = a.scalers["HP1"]["HP2"]
     assert np.equal(a_scalers["RT"]["x"], rt[0]).all()
@@ -203,15 +207,19 @@
     assert np.equal(a_scalers["Intensity"]["y"], intensity[1]).all()
 
     # check reciprocity for scaler generation works
     a = ms.MSAligner(dataframe_1, dataframe_2, names=["HP1", "HP2"])
     a.set_scalers(
         {
             "HP1": {
-                "HP2": {"RT": zip(*rt), "MZ": zip(*mz), "Intensity": zip(*intensity),}
+                "HP2": {
+                    "RT": zip(*rt),
+                    "MZ": zip(*mz),
+                    "Intensity": zip(*intensity),
+                }
             }
         },
         rec=True,
     )
     a.align()
     a_scalers = a.scalers["HP2"]["HP1"]
     assert np.equal(a_scalers["RT"]["x"], rt[0] + rt[1]).all()
@@ -239,20 +247,22 @@
 
 @pytest.mark.filterwarnings("ignore:invalid value")
 def test_calc_scalers():
     """
     Supplemental tests to calculating scalers
     """
 
-    # Will only return nans. Test it does not make an infinite loop
-    assert np.isnan(
-        ms.calc_scalers(
-            np.array([0, 0, 1]), np.array([1, 1, 2]), smoothing="lowess", mode="linear"
-        )[1]
-    ).all()
+    # Will return either nans, the original y_vals, or 1s.
+    # Test it does not make an infinite loop
+    x_vals = np.array([0, 0, 1])
+    y_vals = np.array([1, 1, 2])
+    results = ms.calc_scalers(x_vals, y_vals, smoothing="lowess", mode="linear")[1]
+    all_nans = np.isnan(results).all()
+    is_original = np.isclose(np.array([1, 1, 1]), results).all()
+    assert all_nans or is_original
 
 
 def test_adding_intensity_column(dataframe_3):
     """
     Tests to see if intensity is autocalculated when missing
     """
     # Create Dataframes without Intensity
@@ -292,7 +302,63 @@
     assert list(a.matches["HP1"]) == ["HP2", "HP3"]
 
     # test one to one
     a = ms.MSAligner(dataframe_1, dataframe_2, dataframe_3, names=names)
     a.align("HP1", "HP2")
     assert list(a.matches) == ["HP1"]
     assert list(a.matches["HP1"]) == ["HP2"]
+
+
+def test_schema(dataframe_1, dataframe_2):
+    dataframe_1 = dataframe_1.copy()
+    dataframe_2 = dataframe_2.copy()
+    schema_labels = {
+        "Compound_ID": "feature_id",
+        "RT": "rt (min)",
+        "MZ": "m/z",
+        "Intensity": "abundance",
+    }
+
+    a = ms.MSAligner(
+        dataframe_1.rename(columns=schema_labels),
+        dataframe_2.rename(columns=schema_labels),
+        names=["DS1", "DS2"],
+        schema_labels=schema_labels,
+    )
+    a.align()
+
+
+def test_instance_params(dataframe_1, dataframe_2, dataframe_3):
+    schema_labels = {"RT": "rt (min)"}
+    dataframe_1 = dataframe_1.copy().rename(columns=schema_labels)
+    dataframe_2 = dataframe_2.copy().rename(columns=schema_labels)
+    dataframe_3 = dataframe_3.copy().rename(columns=schema_labels)
+
+    a = ms.MSAligner(
+        dataframe_1,
+        dataframe_2,
+        dataframe_3,
+        names=["DS1", "DS2", "DS3"],
+        schema_labels=schema_labels,
+    )
+    a.descriptors = {"rt (min)": "linear", "MZ": "ppm"}
+    a.default_coarse_params["rt (min)"] = {"upper": 1.0, "lower": -1.0}
+    a.default_cutoff = 10
+    a.default_cutoffs = {"MZ": 6}
+    a.align()
+
+    a = ms.MSAligner(
+        dataframe_1,
+        dataframe_2,
+        dataframe_3,
+        names=["DS1", "DS2", "DS3"],
+        schema_labels=schema_labels,
+    )
+    a.descriptors = {"rt (min)": "linear", "MZ": "ppm"}
+    a.set_instance_defaults(
+        {
+            "coarse_params": {"rt (min)": {"upper": 1.0, "lower": -1.0}},
+            "cutoff": 10,
+            "cutoffs": {"MZ": 6},
+        }
+    )
+    a.align()
```


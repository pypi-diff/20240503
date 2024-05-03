# Comparing `tmp/pandorasat-0.5.6.tar.gz` & `tmp/pandorasat-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandorasat-0.5.6.tar", max compression
+gzip compressed data, was "pandorasat-0.5.7.tar", max compression
```

## Comparing `pandorasat-0.5.6.tar` & `pandorasat-0.5.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1073 2023-11-16 22:14:29.402553 pandorasat-0.5.6/LICENSE
--rw-r--r--   0        0        0     1276 2024-02-14 16:39:22.147171 pandorasat-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      814 2024-02-14 16:39:07.898357 pandorasat-0.5.6/src/pandorasat/__init__.py
--rw-r--r--   0        0        0     2143 2023-11-16 22:14:29.405491 pandorasat-0.5.6/src/pandorasat/citations.py
--rw-r--r--   0        0        0     3018 2023-11-16 22:14:29.405618 pandorasat-0.5.6/src/pandorasat/data/Pandora.Pandora.Visible.xml
--rw-r--r--   0        0        0    14687 2023-11-16 22:14:29.405752 pandorasat-0.5.6/src/pandorasat/data/dichroic-transmission.csv
--rw-r--r--   0        0        0     2777 2023-11-16 22:14:29.405832 pandorasat-0.5.6/src/pandorasat/data/pandora.mplstyle
--rw-r--r--   0        0        0    25577 2023-11-16 22:14:29.406002 pandorasat-0.5.6/src/pandorasat/data/pixel_vs_wavelength.csv
--rw-r--r--   0        0        0     4412 2023-11-16 22:14:29.406102 pandorasat-0.5.6/src/pandorasat/data/pixel_vs_wavelength_vis.csv
--rw-r--r--   0        0        0    26996 2023-11-16 22:45:54.629516 pandorasat-0.5.6/src/pandorasat/data/test-star.p
--rw-r--r--   0        0        0   202494 2023-11-16 22:14:29.406866 pandorasat-0.5.6/src/pandorasat/data/vega.csv
--rw-r--r--   0        0        0   202600 2023-11-16 22:14:29.407639 pandorasat-0.5.6/src/pandorasat/data/vega.dat
--rw-r--r--   0        0        0      484 2023-11-16 22:39:51.932871 pandorasat-0.5.6/src/pandorasat/hardware.py
--rw-r--r--   0        0        0     5836 2024-02-08 20:03:23.912765 pandorasat-0.5.6/src/pandorasat/irdetector.py
--rw-r--r--   0        0        0      311 2023-11-16 22:14:29.407897 pandorasat-0.5.6/src/pandorasat/orbit.py
--rw-r--r--   0        0        0      832 2023-11-16 22:39:51.200812 pandorasat-0.5.6/src/pandorasat/pandorasat.py
--rw-r--r--   0        0        0     5947 2024-02-09 18:25:59.010581 pandorasat-0.5.6/src/pandorasat/phoenix.py
--rw-r--r--   0        0        0     5394 2024-02-08 20:03:23.913123 pandorasat-0.5.6/src/pandorasat/utils.py
--rw-r--r--   0        0        0     5911 2024-02-08 20:03:23.913317 pandorasat-0.5.6/src/pandorasat/visibledetector.py
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 pandorasat-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-11-16 22:14:29.402553 pandorasat-0.5.7/LICENSE
+-rw-r--r--   0        0        0     1276 2024-05-03 17:37:47.065141 pandorasat-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      814 2024-05-03 17:37:40.383486 pandorasat-0.5.7/src/pandorasat/__init__.py
+-rw-r--r--   0        0        0     2143 2023-11-16 22:14:29.405491 pandorasat-0.5.7/src/pandorasat/citations.py
+-rw-r--r--   0        0        0     3018 2023-11-16 22:14:29.405618 pandorasat-0.5.7/src/pandorasat/data/Pandora.Pandora.Visible.xml
+-rw-r--r--   0        0        0    14687 2023-11-16 22:14:29.405752 pandorasat-0.5.7/src/pandorasat/data/dichroic-transmission.csv
+-rw-r--r--   0        0        0     2777 2023-11-16 22:14:29.405832 pandorasat-0.5.7/src/pandorasat/data/pandora.mplstyle
+-rw-r--r--   0        0        0    25577 2023-11-16 22:14:29.406002 pandorasat-0.5.7/src/pandorasat/data/pixel_vs_wavelength.csv
+-rw-r--r--   0        0        0     4412 2023-11-16 22:14:29.406102 pandorasat-0.5.7/src/pandorasat/data/pixel_vs_wavelength_vis.csv
+-rw-r--r--   0        0        0    26996 2023-11-16 22:45:54.629516 pandorasat-0.5.7/src/pandorasat/data/test-star.p
+-rw-r--r--   0        0        0   202494 2023-11-16 22:14:29.406866 pandorasat-0.5.7/src/pandorasat/data/vega.csv
+-rw-r--r--   0        0        0   202600 2023-11-16 22:14:29.407639 pandorasat-0.5.7/src/pandorasat/data/vega.dat
+-rw-r--r--   0        0        0      484 2023-11-16 22:39:51.932871 pandorasat-0.5.7/src/pandorasat/hardware.py
+-rw-r--r--   0        0        0     5976 2024-05-03 17:37:51.198955 pandorasat-0.5.7/src/pandorasat/irdetector.py
+-rw-r--r--   0        0        0      311 2023-11-16 22:14:29.407897 pandorasat-0.5.7/src/pandorasat/orbit.py
+-rw-r--r--   0        0        0      832 2023-11-16 22:39:51.200812 pandorasat-0.5.7/src/pandorasat/pandorasat.py
+-rw-r--r--   0        0        0     5947 2024-02-09 18:25:59.010581 pandorasat-0.5.7/src/pandorasat/phoenix.py
+-rw-r--r--   0        0        0     5394 2024-02-08 20:03:23.913123 pandorasat-0.5.7/src/pandorasat/utils.py
+-rw-r--r--   0        0        0     5911 2024-02-08 20:03:23.913317 pandorasat-0.5.7/src/pandorasat/visibledetector.py
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 pandorasat-0.5.7/PKG-INFO
```

### Comparing `pandorasat-0.5.6/LICENSE` & `pandorasat-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/pyproject.toml` & `pandorasat-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandorasat"
-version = "0.5.6"
+version = "0.5.7"
 description = ""
 authors = ["Christina Hedges <christina.l.hedges@nasa.gov>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 numpy = "^1.22.3"
 astropy = "^5.0.4"
```

### Comparing `pandorasat-0.5.6/src/pandorasat/__init__.py` & `pandorasat-0.5.7/src/pandorasat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.6"
+__version__ = "0.5.7"
 # Standard library
 import os  # noqa
 from glob import glob
 
 PACKAGEDIR = os.path.abspath(os.path.dirname(__file__))
 
 # Standard library
```

### Comparing `pandorasat-0.5.6/src/pandorasat/citations.py` & `pandorasat-0.5.7/src/pandorasat/citations.py`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/data/Pandora.Pandora.Visible.xml` & `pandorasat-0.5.7/src/pandorasat/data/Pandora.Pandora.Visible.xml`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/data/dichroic-transmission.csv` & `pandorasat-0.5.7/src/pandorasat/data/dichroic-transmission.csv`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/data/pandora.mplstyle` & `pandorasat-0.5.7/src/pandorasat/data/pandora.mplstyle`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/data/pixel_vs_wavelength.csv` & `pandorasat-0.5.7/src/pandorasat/data/pixel_vs_wavelength.csv`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/data/pixel_vs_wavelength_vis.csv` & `pandorasat-0.5.7/src/pandorasat/data/pixel_vs_wavelength_vis.csv`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/data/test-star.p` & `pandorasat-0.5.7/src/pandorasat/data/test-star.p`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/data/vega.csv` & `pandorasat-0.5.7/src/pandorasat/data/vega.csv`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/data/vega.dat` & `pandorasat-0.5.7/src/pandorasat/data/vega.dat`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/irdetector.py` & `pandorasat-0.5.7/src/pandorasat/irdetector.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def __repr__(self):
         return "NIRDetector"
 
     @property
     def shape(self):
         """Shape of the detector in pixels"""
-        return (2048, 512)
+        return (2048, 2048)
 
     @property
     def pixel_scale(self):
         """Pixel scale of the detector"""
         return 1.19 * u.arcsec / u.pixel
 
     @property
@@ -60,16 +60,21 @@
         return pd.read_csv(f"{PACKAGEDIR}/data/pixel_vs_wavelength.csv")
 
     @property
     def pixel_read_time(self):
         return 1e-5 * u.second / u.pixel
 
     @property
-    def frame_time(self):
-        return np.product(self.subarray_size) * u.pixel * self.pixel_read_time
+    def subarray_size(self):
+        return (400, 80)
+
+    def frame_time(self, array_size=None):
+        if array_size is None:
+            array_size = self.subarray_size
+        return np.product(array_size) * u.pixel * self.pixel_read_time
 
     @property
     def dark(self):
         return 1 * u.electron / u.second
 
     @property
     def read_noise(self):
```

### Comparing `pandorasat-0.5.6/src/pandorasat/pandorasat.py` & `pandorasat-0.5.7/src/pandorasat/pandorasat.py`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/phoenix.py` & `pandorasat-0.5.7/src/pandorasat/phoenix.py`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/utils.py` & `pandorasat-0.5.7/src/pandorasat/utils.py`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/src/pandorasat/visibledetector.py` & `pandorasat-0.5.7/src/pandorasat/visibledetector.py`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.6/PKG-INFO` & `pandorasat-0.5.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pandorasat
-Version: 0.5.6
+Version: 0.5.7
 Summary: 
 Author: Christina Hedges
 Author-email: christina.l.hedges@nasa.gov
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: astropy (>=5.0.4,<6.0.0)
 Requires-Dist: astroquery (>=0.4.6,<0.5.0)
 Requires-Dist: jupyter-contrib-nbextensions (>=0.7.0,<0.8.0)
 Requires-Dist: mkdocstrings-python (>=1.7.4,<2.0.0)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas[parquet] (>=2.2.0,<3.0.0)
```


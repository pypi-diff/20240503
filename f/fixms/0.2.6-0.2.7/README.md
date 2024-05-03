# Comparing `tmp/fixms-0.2.6.tar.gz` & `tmp/fixms-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixms-0.2.6.tar", max compression
+gzip compressed data, was "fixms-0.2.7.tar", max compression
```

## Comparing `fixms-0.2.6.tar` & `fixms-0.2.7.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     1069 2024-05-01 03:55:02.419385 fixms-0.2.6/LICENSE
--rw-r--r--   0        0        0     4935 2024-05-01 03:55:02.419385 fixms-0.2.6/README.md
--rw-r--r--   0        0        0        0 2024-05-01 03:55:02.419385 fixms-0.2.6/fixms/__init__.py
--rw-r--r--   0        0        0     1812 2024-05-01 03:55:02.419385 fixms-0.2.6/fixms/fix_ms.py
--rw-r--r--   0        0        0    20587 2024-05-01 03:55:02.419385 fixms-0.2.6/fixms/fix_ms_corrs.py
--rw-r--r--   0        0        0    14376 2024-05-01 03:55:02.419385 fixms-0.2.6/fixms/fix_ms_dir.py
--rw-r--r--   0        0        0     5105 2024-05-01 03:55:02.419385 fixms-0.2.6/fixms/logger.py
--rw-r--r--   0        0        0      886 2024-05-01 03:55:02.419385 fixms-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     5631 1970-01-01 00:00:00.000000 fixms-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-03 06:50:01.134498 fixms-0.2.7/LICENSE
+-rw-r--r--   0        0        0     4935 2024-05-03 06:50:01.134498 fixms-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 06:50:01.134498 fixms-0.2.7/fixms/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-03 06:50:01.202499 fixms-0.2.7/fixms/data/RACS_1313-72.SB57526.split.ms.zip
+-rw-r--r--   0        0        0      132 2024-05-03 06:50:01.202499 fixms-0.2.7/fixms/data/SB60933.RACS_1727+37.split.ms.zip
+-rw-r--r--   0        0        0        0 2024-05-03 06:50:01.202499 fixms-0.2.7/fixms/data/__init__.py
+-rw-r--r--   0        0        0     1812 2024-05-03 06:50:01.202499 fixms-0.2.7/fixms/fix_ms.py
+-rw-r--r--   0        0        0    20737 2024-05-03 06:50:01.202499 fixms-0.2.7/fixms/fix_ms_corrs.py
+-rw-r--r--   0        0        0    14376 2024-05-03 06:50:01.202499 fixms-0.2.7/fixms/fix_ms_dir.py
+-rw-r--r--   0        0        0     5105 2024-05-03 06:50:01.202499 fixms-0.2.7/fixms/logger.py
+-rw-r--r--   0        0        0      939 2024-05-03 06:50:01.202499 fixms-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     5691 1970-01-01 00:00:00.000000 fixms-0.2.7/PKG-INFO
```

### Comparing `fixms-0.2.6/LICENSE` & `fixms-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fixms-0.2.6/README.md` & `fixms-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `fixms-0.2.6/fixms/fix_ms.py` & `fixms-0.2.7/fixms/fix_ms.py`

 * *Files identical despite different names*

### Comparing `fixms-0.2.6/fixms/fix_ms_corrs.py` & `fixms-0.2.7/fixms/fix_ms_corrs.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,44 +59,50 @@
     # -> feed_angle = 45 - pol_angle
     new_ms_feed = -(pol_axes_cor - 45.0 * u.deg)
     with table((ms / "FEED").as_posix(), readonly=False, ack=False) as tf:
         tf.putcol("RECEPTOR_ANGLE", new_ms_feed.to(u.rad).value)
         tf.flush()
 
 
-def get_pol_axis(ms: Path, feed_idx: Optional[int] = None) -> u.Quantity:
+def get_pol_axis(
+    ms: Path, feed_idx: Optional[int] = None, col="RECEPTOR_ANGLE"
+) -> u.Quantity:
     """Get the polarization axis from the ASKAP MS. Checks are performed
     to ensure this polarisation axis angle is constant throughout the observation.
 
 
     Args:
         ms (Path): The path to the measurement set that will be inspected
         feed_idx (Optional[int], optional): Specify the entery in the FEED
         table of `ms` to return. This might be required when a subset of a
         measurement set has been extracted from an observation with a varying
         orientation.
 
     Returns:
         astropy.units.Quantity: The rotation of the PAF throughout the observing.
     """
+    _known_cols = ("RECEPTOR_ANGLE", "INSTRUMENT_RECEPTOR_ANGLE")
+    if col not in _known_cols:
+        raise ValueError(f"Unknown column {col=}, please use one of {_known_cols}")
+
     with table((ms / "FEED").as_posix(), readonly=True, ack=False) as tf:
-        ms_feed = tf.getcol("RECEPTOR_ANGLE") * u.rad
+        ms_feed = tf.getcol(col) * u.rad
         # PAF is at 45deg to feeds
         # 45 - feed_angle = pol_angle
         pol_axes = -(ms_feed - 45.0 * u.deg)
 
     if feed_idx is None:
         assert (ms_feed[:, 0] == ms_feed[0, 0]).all() & (
             ms_feed[:, 1] == ms_feed[0, 1]
-        ).all(), "The RECEPTOR_ANGLE changes with time, please check the MS"
+        ).all(), f"The {col} changes with time, please check the MS"
+
+        feed_idx = 0
 
-        pol_ang = pol_axes[0, 0].to(u.deg)
-    else:
-        logger.debug(f"Extracting the third-axis orientation for {feed_idx=}")
-        pol_ang = pol_axes[feed_idx, 0].to(u.deg)
+    logger.debug(f"Extracting the third-axis orientation for {feed_idx=}")
+    pol_ang = pol_axes[feed_idx, 0].to(u.deg)
 
     return pol_ang
 
 
 def convert_correlations(
     correlations: np.ndarray, pol_axis: u.Quantity, fix_stokes_factor: bool = True
 ) -> np.ndarray:
```

### Comparing `fixms-0.2.6/fixms/fix_ms_dir.py` & `fixms-0.2.7/fixms/fix_ms_dir.py`

 * *Files identical despite different names*

### Comparing `fixms-0.2.6/fixms/logger.py` & `fixms-0.2.7/fixms/logger.py`

 * *Files identical despite different names*

### Comparing `fixms-0.2.6/pyproject.toml` & `fixms-0.2.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "fixms"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["Alec Thomson (S&A, Kensington WA) <alec.thomson@csiro.au>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 numpy = "<1.26"
 astropy = ">=5"
 python-casacore = "*"
 tqdm = "*"
+importlib-resources = {version="*", python = "<3.9"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.group.dev.dependencies]
 isort = ">=5.12.0"
```

### Comparing `fixms-0.2.6/PKG-INFO` & `fixms-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: fixms
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 License: MIT
 Author: Alec Thomson (S&A, Kensington WA)
 Author-email: alec.thomson@csiro.au
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
 Requires-Dist: astropy (>=5)
+Requires-Dist: importlib-resources ; python_version < "3.9"
 Requires-Dist: numpy (<1.26)
 Requires-Dist: python-casacore
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 [![rtd](https://readthedocs.org/projects/fixms/badge/?version=latest)](https://fixms.readthedocs.io/) [![Tests](https://github.com/AlecThomson/FixMS/actions/workflows/test.yml/badge.svg)](https://github.com/AlecThomson/FixMS/actions/workflows/test.yml) [![PyPi](https://github.com/AlecThomson/FixMS/actions/workflows/publish.yml/badge.svg)](https://pypi.org/project/fixms/) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/AlecThomson/FixMS/main.svg)](https://results.pre-commit.ci/latest/github/AlecThomson/FixMS/main)
```


# Comparing `tmp/kelp_o_matic-0.9.1.tar.gz` & `tmp/kelp_o_matic-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kelp_o_matic-0.9.1.tar", max compression
+gzip compressed data, was "kelp_o_matic-0.9.2.tar", max compression
```

## Comparing `kelp_o_matic-0.9.1.tar` & `kelp_o_matic-0.9.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-01-16 18:54:06.032478 kelp_o_matic-0.9.1/LICENSE.txt
--rw-r--r--   0        0        0     1130 2024-01-16 18:54:06.032478 kelp_o_matic-0.9.1/README.md
--rw-r--r--   0        0        0      127 2024-01-16 18:56:08.044404 kelp_o_matic-0.9.1/kelp_o_matic/__init__.py
--rw-r--r--   0        0        0     2699 2024-01-16 18:54:06.260478 kelp_o_matic-0.9.1/kelp_o_matic/cli.py
--rw-r--r--   0        0        0      176 2024-01-16 18:54:06.260478 kelp_o_matic-0.9.1/kelp_o_matic/geotiff_io/__init__.py
--rw-r--r--   0        0        0     2819 2024-01-16 18:54:06.260478 kelp_o_matic-0.9.1/kelp_o_matic/geotiff_io/geotiff_reader.py
--rw-r--r--   0        0        0     2433 2024-01-16 18:54:06.260478 kelp_o_matic-0.9.1/kelp_o_matic/geotiff_io/geotiff_writer.py
--rw-r--r--   0        0        0     5146 2024-01-16 18:54:06.260478 kelp_o_matic-0.9.1/kelp_o_matic/hann.py
--rw-r--r--   0        0        0     4777 2024-01-16 18:54:06.260478 kelp_o_matic-0.9.1/kelp_o_matic/lib.py
--rw-r--r--   0        0        0     7441 2024-01-16 18:54:06.260478 kelp_o_matic-0.9.1/kelp_o_matic/managers.py
--rw-r--r--   0        0        0     4344 2024-01-16 18:54:06.260478 kelp_o_matic-0.9.1/kelp_o_matic/models.py
--rw-r--r--   0        0        0     1660 2024-01-16 18:54:06.260478 kelp_o_matic-0.9.1/kelp_o_matic/utils.py
--rw-r--r--   0        0        0      834 2024-01-16 18:56:07.996404 kelp_o_matic-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 kelp_o_matic-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-01-18 19:55:48.479675 kelp_o_matic-0.9.2/LICENSE.txt
+-rw-r--r--   0        0        0     1130 2024-01-18 19:55:48.479675 kelp_o_matic-0.9.2/README.md
+-rw-r--r--   0        0        0      127 2024-01-18 19:58:01.887311 kelp_o_matic-0.9.2/kelp_o_matic/__init__.py
+-rw-r--r--   0        0        0     2699 2024-01-18 19:55:48.711674 kelp_o_matic-0.9.2/kelp_o_matic/cli.py
+-rw-r--r--   0        0        0      176 2024-01-18 19:55:48.711674 kelp_o_matic-0.9.2/kelp_o_matic/geotiff_io/__init__.py
+-rw-r--r--   0        0        0     2819 2024-01-18 19:55:48.711674 kelp_o_matic-0.9.2/kelp_o_matic/geotiff_io/geotiff_reader.py
+-rw-r--r--   0        0        0     2433 2024-01-18 19:55:48.711674 kelp_o_matic-0.9.2/kelp_o_matic/geotiff_io/geotiff_writer.py
+-rw-r--r--   0        0        0     5146 2024-01-18 19:55:48.711674 kelp_o_matic-0.9.2/kelp_o_matic/hann.py
+-rw-r--r--   0        0        0     4777 2024-01-18 19:55:48.711674 kelp_o_matic-0.9.2/kelp_o_matic/lib.py
+-rw-r--r--   0        0        0     7442 2024-01-18 19:55:48.711674 kelp_o_matic-0.9.2/kelp_o_matic/managers.py
+-rw-r--r--   0        0        0     4421 2024-01-18 19:55:48.711674 kelp_o_matic-0.9.2/kelp_o_matic/models.py
+-rw-r--r--   0        0        0     1660 2024-01-18 19:55:48.711674 kelp_o_matic-0.9.2/kelp_o_matic/utils.py
+-rw-r--r--   0        0        0      834 2024-01-18 19:58:01.835311 kelp_o_matic-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 kelp_o_matic-0.9.2/PKG-INFO
```

### Comparing `kelp_o_matic-0.9.1/LICENSE.txt` & `kelp_o_matic-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kelp_o_matic-0.9.1/README.md` & `kelp_o_matic-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `kelp_o_matic-0.9.1/kelp_o_matic/cli.py` & `kelp_o_matic-0.9.2/kelp_o_matic/cli.py`

 * *Files identical despite different names*

### Comparing `kelp_o_matic-0.9.1/kelp_o_matic/geotiff_io/geotiff_reader.py` & `kelp_o_matic-0.9.2/kelp_o_matic/geotiff_io/geotiff_reader.py`

 * *Files identical despite different names*

### Comparing `kelp_o_matic-0.9.1/kelp_o_matic/geotiff_io/geotiff_writer.py` & `kelp_o_matic-0.9.2/kelp_o_matic/geotiff_io/geotiff_writer.py`

 * *Files identical despite different names*

### Comparing `kelp_o_matic-0.9.1/kelp_o_matic/hann.py` & `kelp_o_matic-0.9.2/kelp_o_matic/hann.py`

 * *Files identical despite different names*

### Comparing `kelp_o_matic-0.9.1/kelp_o_matic/lib.py` & `kelp_o_matic-0.9.2/kelp_o_matic/lib.py`

 * *Files identical despite different names*

### Comparing `kelp_o_matic-0.9.1/kelp_o_matic/managers.py` & `kelp_o_matic-0.9.2/kelp_o_matic/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,17 +146,17 @@
                 "significantly faster for tiled images.",
                 UserWarning,
             )
         elif crop_shape % y_shape != 0 or crop_shape % x_shape != 0:
             warnings.warn(
                 "Suboptimal crop_size and padding were specified. Performance "
                 "will be degraded. The detected block shape for this band is "
-                "({y_shape}, {x_shape}). Faster performance may be achieved by setting "
-                "the crop_size and the padding such that (crop_size + 2*padding) is a "
-                "multiple of {y_shape}.",
+                f"({y_shape}, {x_shape}). Faster performance may be achieved by "
+                "setting the crop_size and the padding such that "
+                f"(crop_size + 2*padding) is a multiple of {y_shape}.",
                 UserWarning,
             )
 
     def _run_checks(self):
         """Run image checks."""
         self._no_data_check()
         self._dtype_check()
@@ -184,15 +184,15 @@
 class RichSegmentationManager(GeotiffSegmentationManager):
     """Run the segmentation with Rich progress bars and logging."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.progress = Progress(
-            SpinnerColumn("earth"), *Progress.get_default_columns(), TimeElapsedColumn()
+            SpinnerColumn("dots"), *Progress.get_default_columns(), TimeElapsedColumn()
         )
         self.processing_task = self.progress.add_task(
             description="Processing", total=len(self.reader)
         )
 
     def __call__(self):
         with self.progress:
```

### Comparing `kelp_o_matic-0.9.1/kelp_o_matic/models.py` & `kelp_o_matic-0.9.2/kelp_o_matic/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,15 +100,18 @@
     torchscript_path = "LRASPP_MobileNetV3_mussel_presence_rgb_jit_miou=0.8745.pt"
 
 
 def _unet_efficientnet_b4_transform(x: Union[np.ndarray, Image]) -> torch.Tensor:
     # to float
     x = f.to_tensor(x)[:4, :, :].to(torch.float)
     # min-max scale
-    min_, _ = torch.kthvalue(x.flatten().unique(), 2)
+    x_unique = x.flatten().unique()
+    min_ = x_unique[0]
+    if len(x_unique) > 1:
+        min_, _ = torch.kthvalue(x_unique, 2)
     max_ = x.flatten().max()
     return torch.clamp((x - min_) / (max_ - min_ + 1e-8), 0, 1)
 
 
 class KelpRGBIPresenceSegmentationModel(_Model):
     torchscript_path = (
         "UNetPlusPlus_EfficientNetB4_kelp_presence_rgbi_jit_miou=0.8785.pt"
```

### Comparing `kelp_o_matic-0.9.1/kelp_o_matic/utils.py` & `kelp_o_matic-0.9.2/kelp_o_matic/utils.py`

 * *Files identical despite different names*

### Comparing `kelp_o_matic-0.9.1/pyproject.toml` & `kelp_o_matic-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kelp-o-matic"
-version = "0.9.1"
+version = "0.9.2"
 description = "Hakai Segment Tool for GeoTiff RPAS Imagery"
 authors = ["Taylor Denouden <taylor.denouden@hakai.org>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://kelp-o-matic.readthedocs.io"
 packages = [{ include = "kelp_o_matic" }]
```

### Comparing `kelp_o_matic-0.9.1/PKG-INFO` & `kelp_o_matic-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kelp-o-matic
-Version: 0.9.1
+Version: 0.9.2
 Summary: Hakai Segment Tool for GeoTiff RPAS Imagery
 License: MIT
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kelp-o-matic Version: 0.9.1 Summary: Hakai Segment
+Metadata-Version: 2.1 Name: kelp-o-matic Version: 0.9.2 Summary: Hakai Segment
 Tool for GeoTiff RPAS Imagery License: MIT Author: Taylor Denouden Author-
 email: taylor.denouden@hakai.org Requires-Python: >=3.9,<3.12 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: numpy (>=1.24.2,<2.0.0) Requires-Dist: rasterio
 (>=1.3.7,<2.0.0) Requires-Dist: rich (>=13.5,<14.0) Requires-Dist: torch
```


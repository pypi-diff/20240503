# Comparing `tmp/faim_ipa-0.3.0.tar.gz` & `tmp/faim_ipa-0.3.1.tar.gz`

## Comparing `faim_ipa-0.3.0.tar` & `faim_ipa-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/MetaSeriesUtils_dask.py
--rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/UIntHistogram.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/Zarr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/__init__.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/dask_utils.py
--rw-r--r--   0        0        0    11203 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/mobie.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/utils.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/alignment/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/alignment/alignment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/__init__.py
--rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/acquisition.py
--rw-r--r--   0        0        0    13108 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/converter.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/plate.py
--rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/cellvoyager/StackedTile.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/cellvoyager/__init__.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py
--rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/imagexpress/StackAcquisition.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/hcs/imagexpress/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/io/ChannelMetadata.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/io/MetaSeriesTiff.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/io/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/stitching/BoundingBox5D.py
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/stitching/DaskTileStitcher.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/stitching/Tile.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/stitching/__init__.py
--rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/stitching/stitching_utils.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/visiview/RegionAcquisition.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/visiview/StackedTile.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/visiview/__init__.py
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/src/faim_ipa/visiview/ome_companion_utils.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/.gitignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/LICENSE
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/README.md
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 faim_ipa-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/MetaSeriesUtils_dask.py
+-rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/UIntHistogram.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/Zarr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/__init__.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/dask_utils.py
+-rw-r--r--   0        0        0    11203 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/mobie.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/utils.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/alignment/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/alignment/alignment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/__init__.py
+-rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/acquisition.py
+-rw-r--r--   0        0        0    13424 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/converter.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/plate.py
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/cellvoyager/StackedTile.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/cellvoyager/__init__.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/imagexpress/StackAcquisition.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/hcs/imagexpress/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/io/ChannelMetadata.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/io/MetaSeriesTiff.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/io/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/stitching/BoundingBox5D.py
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/stitching/DaskTileStitcher.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/stitching/Tile.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/stitching/__init__.py
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/stitching/stitching_utils.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/visiview/RegionAcquisition.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/visiview/StackedTile.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/visiview/__init__.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/src/faim_ipa/visiview/ome_companion_utils.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/LICENSE
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/README.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 faim_ipa-0.3.1/PKG-INFO
```

### Comparing `faim_ipa-0.3.0/src/faim_ipa/MetaSeriesUtils_dask.py` & `faim_ipa-0.3.1/src/faim_ipa/MetaSeriesUtils_dask.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/UIntHistogram.py` & `faim_ipa-0.3.1/src/faim_ipa/UIntHistogram.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/Zarr.py` & `faim_ipa-0.3.1/src/faim_ipa/Zarr.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/dask_utils.py` & `faim_ipa-0.3.1/src/faim_ipa/dask_utils.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/mobie.py` & `faim_ipa-0.3.1/src/faim_ipa/mobie.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/utils.py` & `faim_ipa-0.3.1/src/faim_ipa/utils.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/alignment/alignment.py` & `faim_ipa-0.3.1/src/faim_ipa/alignment/alignment.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/acquisition.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/acquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/converter.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
     _ngff_plate: NGFFPlate
 
     def __init__(
         self,
         ngff_plate: NGFFPlate,
         yx_binning: int = 1,
-        stitching_yx_chunk_size_factor: int = 1,
         warp_func: Callable = stitching_utils.translate_tiles_2d,
         fuse_func: Callable = stitching_utils.fuse_mean,
         client: Client = None,
     ):
         """
         Parameters
         ----------
@@ -63,15 +62,14 @@
             Dask client used for the conversion.
         """
         assert (
             isinstance(yx_binning, int) and yx_binning >= 1
         ), "yx_binning must be an integer >= 1."
         self._ngff_plate = ngff_plate
         self._yx_binning = yx_binning
-        self._stitching_yx_chunk_size_factor = stitching_yx_chunk_size_factor
         self._warp_func = warp_func
         self._fuse_func = fuse_func
         self._client = client
 
     def create_zarr_plate(
         self, plate_acquisition: PlateAcquisition, wells: Optional[list[str]] = None
     ) -> zarr.Group:
@@ -155,14 +153,15 @@
         well_acquisitions = plate_acquisition.get_well_acquisitions(wells)
 
         for well_acquisition in well_acquisitions:
             well_group = self._create_well_group(
                 plate,
                 well_acquisition,
                 well_sub_group,
+                add_to_well_images=not build_acquisition_mask,
             )
             group = well_group[well_sub_group]
             self._write_stitched_image(
                 group,
                 chunks,
                 plate_acquisition,
                 storage_options,
@@ -361,19 +360,29 @@
             fuse_func=(
                 stitching_utils.fuse_sum if build_acquisition_mask else self._fuse_func
             ),
             build_acquisition_mask=build_acquisition_mask,
         )
         return image_da
 
-    def _create_well_group(self, plate, well_acquisition, well_sub_group):
+    def _create_well_group(
+        self, plate, well_acquisition, well_sub_group, add_to_well_images=True
+    ):
         row, col = well_acquisition.get_row_col()
         well_group = plate.require_group(row).require_group(col)
         well_group.require_group(well_sub_group)
-        write_well_metadata(well_group, [{"path": well_sub_group}])
+        if add_to_well_images:
+            zattrs = well_group.attrs.asdict()
+            if "well" in zattrs.keys() and "images" in zattrs["well"].keys():
+                existing_images = well_group.attrs.asdict()["well"]["images"]
+            else:
+                existing_images = []
+            write_well_metadata(
+                well_group, existing_images + [{"path": well_sub_group}]
+            )
         return well_group
 
     @staticmethod
     def _get_storage_options(
         storage_options: dict,
         output_shape: tuple[int, ...],
         chunks: tuple[int, ...],
```

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/plate.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/plate.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/cellvoyager/StackedTile.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/cellvoyager/StackedTile.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             illumination_correction_matrices=illumination_correction_matrices,
         )
 
     def _assemble_tiles(self) -> list[Tile]:
         tiles = []
         for i, row in self._files.iterrows():
             file = row["path"]
-            time_point = 0
+            time_point = row["t"] if "t" in row.index and row["t"] is not None else 0
             channel = row["channel"]
             metadata = load_metaseries_tiff_metadata(file)
             if self._z_spacing is None:
                 z = 1
             else:
                 z = row["z"] if row["z"] is not None else 1
 
@@ -73,16 +73,19 @@
         metadata = load_metaseries_tiff_metadata(self._files.iloc[0]["path"])
         return (metadata["spatial-calibration-y"], metadata["spatial-calibration-x"])
 
     def get_z_spacing(self) -> Optional[float]:
         return self._z_spacing
 
     def get_axes(self) -> list[str]:
+        axes = ["y", "x"]
+
         if "z" in self._files.columns:
-            axes = ["z", "y", "x"]
-        else:
-            axes = ["y", "x"]
+            axes = ["z"] + axes
 
         if self._files["channel"].nunique() > 1:
             axes = ["c"] + axes
 
+        if "t" in self._files.columns and self._files["t"].nunique() > 1:
+            axes = ["t"] + axes
+
         return axes
```

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,14 @@
                     _files[(_files["channel"] == ch) & (_files["z"].isna())].index,
                     inplace=True,
                 )
         return _files
 
     def _get_root_re(self) -> re.Pattern:
         return re.compile(
-            r".*[\/\\](?P<date>\d{4}-\d{2}-\d{2})[\/\\](?P<acq_id>\d+)(?:[\/\\]ZStep_(?P<z>\d+))?.*"
+            r".*[\/\\](?P<date>\d{4}-\d{2}-\d{2})[\/\\](?P<acq_id>\d+)(?:[\/\\]TimePoint_(?P<t>\d+))?(?:[\/\\]ZStep_(?P<z>\d+))?.*"
         )
 
     def _get_filename_re(self) -> re.Pattern:
         return re.compile(
             r"(?P<name>.*)_(?P<well>[A-Z]+\d{2})_?(?P<field>s\d+)?_?(?P<channel>w[1-9]{1})?(?!_thumb)(?P<md_id>[0-9A-F]{8}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{12})(?P<ext>.tif)"
         )
```

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,17 @@
             acquisition_dir=acquisition_dir,
             alignment=alignment,
             background_correction_matrices=background_correction_matrices,
             illumination_correction_matrices=illumination_correction_matrices,
         )
 
     def _get_root_re(self) -> re.Pattern:
-        return re.compile(r".*[\/\\](?P<date>\d{4}-\d{2}-\d{2})[\/\\](?P<acq_id>\d+)")
+        return re.compile(
+            r".*[\/\\](?P<date>\d{4}-\d{2}-\d{2})[\/\\](?P<acq_id>\d+)(?:[\/\\]TimePoint_(?P<t>\d+))?"
+        )
 
     def _get_filename_re(self) -> re.Pattern:
         return re.compile(
             r"(?P<name>.*)_(?P<well>[A-Z]+\d{2})_?(?P<field>s\d+)?_?(?P<channel>w[1-9]{1})?(?!_thumb)(?P<md_id>[0-9A-F]{8}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{12})(?P<ext>.tif)"
         )
 
     def _get_z_spacing(self) -> Optional[float]:
```

### Comparing `faim_ipa-0.3.0/src/faim_ipa/hcs/imagexpress/StackAcquisition.py` & `faim_ipa-0.3.1/src/faim_ipa/hcs/imagexpress/StackAcquisition.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def _parse_files(self) -> pd.DataFrame:
         files = super()._parse_files()
         self._z_spacing = self._compute_z_spacing(files)
         return files
 
     def _get_root_re(self) -> re.Pattern:
         return re.compile(
-            r".*[\/\\](?P<date>\d{4}-\d{2}-\d{2})[\/\\](?P<acq_id>\d+)(?:[\/\\]ZStep_(?P<z>\d+))"
+            r".*[\/\\](?P<date>\d{4}-\d{2}-\d{2})[\/\\](?P<acq_id>\d+)(?:[\/\\]TimePoint_(?P<t>\d+))?(?:[\/\\]ZStep_(?P<z>\d+))"
         )
 
     def _get_filename_re(self) -> re.Pattern:
         return re.compile(
             r"(?P<name>.*)_(?P<well>[A-Z]+\d{2})_?(?P<field>s\d+)?_?(?P<channel>w[1-9]{1})?(?!_thumb)(?P<md_id>[0-9A-F]{8}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{12})(?P<ext>.tif)"
         )
```

### Comparing `faim_ipa-0.3.0/src/faim_ipa/io/MetaSeriesTiff.py` & `faim_ipa-0.3.1/src/faim_ipa/io/MetaSeriesTiff.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/stitching/BoundingBox5D.py` & `faim_ipa-0.3.1/src/faim_ipa/stitching/BoundingBox5D.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/stitching/DaskTileStitcher.py` & `faim_ipa-0.3.1/src/faim_ipa/stitching/DaskTileStitcher.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/stitching/Tile.py` & `faim_ipa-0.3.1/src/faim_ipa/stitching/Tile.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/stitching/stitching_utils.py` & `faim_ipa-0.3.1/src/faim_ipa/stitching/stitching_utils.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/visiview/RegionAcquisition.py` & `faim_ipa-0.3.1/src/faim_ipa/visiview/RegionAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/visiview/StackedTile.py` & `faim_ipa-0.3.1/src/faim_ipa/visiview/StackedTile.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/src/faim_ipa/visiview/ome_companion_utils.py` & `faim_ipa-0.3.1/src/faim_ipa/visiview/ome_companion_utils.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/.gitignore` & `faim_ipa-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/LICENSE` & `faim_ipa-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.0/pyproject.toml` & `faim_ipa-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,19 @@
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
+cov-html = [
+  "test-cov",
+  "- coverage combine",
+  "coverage html",
+]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.9", "3.10", "3.11", "3.12"]
```

### Comparing `faim_ipa-0.3.0/PKG-INFO` & `faim_ipa-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faim-ipa
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tools used at FMI-FAIM for Image Processing and Analysis.
 Project-URL: Bug Tracker, https://github.com/fmi-faim/faim-ipa/issues
 Project-URL: Documentation, https://github.com/fmi-faim/faim-ipa#README.md
 Project-URL: Homepage, https://github.com/fmi-faim/faim-ipa.git
 Project-URL: Source Code, https://github.com/fmi-faim/faim-ipa
 Project-URL: User Support, https://github.com/fmi-faim/faim-ipa/issues
 Author-email: Tim-Oliver Buchholz <tim-oliver.buchholz@fmi.ch>, Jan Eglinger <jan.eglinger@fmi.ch>
```


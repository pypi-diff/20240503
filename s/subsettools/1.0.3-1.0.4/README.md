# Comparing `tmp/subsettools-1.0.3.tar.gz` & `tmp/subsettools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsettools-1.0.3.tar", max compression
+gzip compressed data, was "subsettools-1.0.4.tar", max compression
```

## Comparing `subsettools-1.0.3.tar` & `subsettools-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rwxr-xr-x   0        0        0     1092 2023-11-13 19:24:51.323232 subsettools-1.0.3/LICENSE
--rwxr-xr-x   0        0        0     2513 2023-12-19 18:35:23.614967 subsettools-1.0.3/README.md
--rw-r--r--   0        0        0      771 2024-02-05 17:43:06.301304 subsettools-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      444 2023-11-29 18:37:02.076146 subsettools-1.0.3/src/subsettools/__init__.py
--rw-r--r--   0        0        0     1956 2023-11-29 18:37:02.109147 subsettools-1.0.3/src/subsettools/_error_checking.py
--rw-r--r--   0        0        0     2110 2023-11-29 18:37:02.142147 subsettools-1.0.3/src/subsettools/datasets.py
--rw-r--r--   0        0        0      133 2023-11-29 18:37:02.142147 subsettools-1.0.3/src/subsettools/ref_yamls/__init__.py
--rw-r--r--   0        0        0    10637 2023-11-13 19:24:51.324232 subsettools-1.0.3/src/subsettools/ref_yamls/conus1_pf_spinup_box.yaml
--rw-r--r--   0        0        0    10190 2023-11-13 19:24:51.324232 subsettools-1.0.3/src/subsettools/ref_yamls/conus1_pf_spinup_solid.yaml
--rw-r--r--   0        0        0    10951 2023-11-13 19:24:51.324232 subsettools-1.0.3/src/subsettools/ref_yamls/conus1_pfclm_transient_box.yaml
--rw-r--r--   0        0        0    10482 2023-11-13 19:24:51.324232 subsettools-1.0.3/src/subsettools/ref_yamls/conus1_pfclm_transient_solid.yaml
--rw-r--r--   0        0        0    11495 2023-11-13 19:24:51.324232 subsettools-1.0.3/src/subsettools/ref_yamls/conus2_pf_spinup_box.yaml
--rw-r--r--   0        0        0    11047 2023-11-13 19:24:51.324232 subsettools-1.0.3/src/subsettools/ref_yamls/conus2_pf_spinup_solid.yaml
--rw-r--r--   0        0        0    11832 2023-11-13 19:24:51.324232 subsettools-1.0.3/src/subsettools/ref_yamls/conus2_pfclm_transient_box.yaml
--rw-r--r--   0        0        0    11384 2023-11-13 19:24:51.324232 subsettools-1.0.3/src/subsettools/ref_yamls/conus2_pfclm_transient_solid.yaml
--rw-r--r--   0        0        0     5886 2023-12-07 15:45:24.945374 subsettools-1.0.3/src/subsettools/subset_utils.py
--rw-r--r--   0        0        0    42667 2024-02-05 17:43:06.302304 subsettools-1.0.3/src/subsettools/subsettools.py
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 subsettools-1.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1092 2023-11-13 19:24:51.323232 subsettools-1.0.4/LICENSE
+-rwxr-xr-x   0        0        0     2690 2024-04-16 17:49:13.047816 subsettools-1.0.4/README.md
+-rw-r--r--   0        0        0      771 2024-05-03 17:17:58.029186 subsettools-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      511 2024-04-29 23:34:58.686225 subsettools-1.0.4/src/subsettools/__init__.py
+-rw-r--r--   0        0        0     2468 2024-04-29 23:34:58.686225 subsettools-1.0.4/src/subsettools/_error_checking.py
+-rw-r--r--   0        0        0     2110 2023-11-29 18:37:02.142147 subsettools-1.0.4/src/subsettools/datasets.py
+-rw-r--r--   0        0        0      133 2023-11-29 18:37:02.142147 subsettools-1.0.4/src/subsettools/ref_yamls/__init__.py
+-rw-r--r--   0        0        0    10637 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pf_spinup_box.yaml
+-rw-r--r--   0        0        0    10190 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pf_spinup_solid.yaml
+-rw-r--r--   0        0        0    10951 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pfclm_transient_box.yaml
+-rw-r--r--   0        0        0    10482 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pfclm_transient_solid.yaml
+-rw-r--r--   0        0        0    11495 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pf_spinup_box.yaml
+-rw-r--r--   0        0        0    11047 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pf_spinup_solid.yaml
+-rw-r--r--   0        0        0    11832 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pfclm_transient_box.yaml
+-rw-r--r--   0        0        0    11384 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pfclm_transient_solid.yaml
+-rw-r--r--   0        0        0     5886 2023-12-07 15:45:24.945374 subsettools-1.0.4/src/subsettools/subset_utils.py
+-rw-r--r--   0        0        0    41926 2024-04-29 23:34:58.692225 subsettools-1.0.4/src/subsettools/subsettools.py
+-rw-r--r--   0        0        0     3436 2024-05-03 17:17:58.029186 subsettools-1.0.4/src/subsettools/upstream_area.py
+-rw-r--r--   0        0        0     2604 2024-04-17 16:57:39.679663 subsettools-1.0.4/src/subsettools/upstream_area.py~
+-rw-r--r--   0        0        0     3344 1970-01-01 00:00:00.000000 subsettools-1.0.4/PKG-INFO
```

### Comparing `subsettools-1.0.3/LICENSE` & `subsettools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.3/README.md` & `subsettools-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,7 +18,9 @@
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines on the [SubsetTools GitHub repo](https://github.com/hydroframe/subsettools). Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
 `subsettools` is part of the [HydroFrame project](https://hydroframe.org/). It is licensed under the terms of the MIT license.
+
+Copyright 2024 The Trustees of Princeton University and The Arizona Board of Regents on behalf of the University of Arizona, College of Science Hydrology & Atmospheric Sciences
```

### Comparing `subsettools-1.0.3/pyproject.toml` & `subsettools-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subsettools"
-version = "1.0.3"
+version = "1.0.4"
 description = "Subsetting tools and utilities for ParFlow"
 authors = ["George Artavanis, Amanda Triplett"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
```

### Comparing `subsettools-1.0.3/src/subsettools/_error_checking.py` & `subsettools-1.0.4/src/subsettools/_error_checking.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,25 @@
     if not isinstance(grid, str):
         raise TypeError("grid must be a string")
     grid = grid.lower()
     if grid not in ["conus1", "conus2"]:
         raise ValueError("Supported grids are 'conus1' and 'conus2'")
 
 
+def _validate_latlon_list(latlon_pts):
+    """Check errors for a user-provided list of latlon points."""
+    if not isinstance(latlon_pts, list):
+        raise TypeError("latlon argument must be a list of points")
+    for point in latlon_pts:
+        if not (isinstance(point, list) and
+                len(point) == 2 and
+                all(isinstance(value, (int, float)) for value in point)):
+            raise ValueError("Each element of the list must be a list of two floats of the form [lat, lon]")
+
+    
 def _validate_dir(dir_name):
     """Check that dir_name is a valid directory."""
     if not os.path.isdir(dir_name):
         raise FileNotFoundError(f"{dir_name} is not a valid existing directory") 
 
 
 def _validate_grid_bounds(grid_bounds):
```

### Comparing `subsettools-1.0.3/src/subsettools/datasets.py` & `subsettools-1.0.4/src/subsettools/datasets.py`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.3/src/subsettools/ref_yamls/conus1_pf_spinup_box.yaml` & `subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pf_spinup_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.3/src/subsettools/ref_yamls/conus1_pf_spinup_solid.yaml` & `subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pf_spinup_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.3/src/subsettools/ref_yamls/conus1_pfclm_transient_box.yaml` & `subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pfclm_transient_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.3/src/subsettools/ref_yamls/conus1_pfclm_transient_solid.yaml` & `subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pfclm_transient_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.3/src/subsettools/ref_yamls/conus2_pf_spinup_box.yaml` & `subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pf_spinup_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.3/src/subsettools/ref_yamls/conus2_pf_spinup_solid.yaml` & `subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pf_spinup_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.3/src/subsettools/ref_yamls/conus2_pfclm_transient_box.yaml` & `subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pfclm_transient_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.3/src/subsettools/ref_yamls/conus2_pfclm_transient_solid.yaml` & `subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pfclm_transient_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.3/src/subsettools/subset_utils.py` & `subsettools-1.0.4/src/subsettools/subset_utils.py`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.3/src/subsettools/subsettools.py` & `subsettools-1.0.4/src/subsettools/subsettools.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     write_land_cover,
     edit_drvclmin,
     get_UTC_time,
 )
 from ._error_checking import (
     _validate_huc_list,
     _validate_grid,
+    _validate_latlon_list,
     _validate_dir,
     _validate_grid_bounds,
     _validate_date,
 )
 
 
 def huc_to_ij(huc_list, grid):
@@ -48,18 +49,18 @@
 
     .. code-block:: python
 
         grid_bounds = huc_to_ij(huc_list=["14080201", "14080202", "14080203"], grid="conus1")
     """
     _validate_huc_list(huc_list)
     _validate_grid(grid)
-    conus_hucs, _, indices_j, indices_i = _get_conus_hucs_indices(huc_list, grid.lower())
+    _, _, indices_j, indices_i = _get_conus_hucs_indices(huc_list, grid.lower())
     if indices_i.size == 0 or indices_j.size == 0:
         raise ValueError(f"The area defined by the provided HUCs is not part of the {grid} grid.")  
-    return _indices_to_ij(conus_hucs, indices_j, indices_i)
+    return _indices_to_ij(indices_j, indices_i)
 
 
 def _get_conus_hucs_indices(huc_list, grid):
     """Get the huc datafile as an ndarray and three mask arrays representing the selected hucs.
     
     Args:
         huc_list (list[str]): a list of huc IDs 
@@ -81,19 +82,18 @@
         raise ValueError(f"There is no HUC mapping entry for grid {grid}.")
     conus_hucs = hf_hydrodata.gridded.get_ndarray(entry, level=str(huc_len))
     sel_hucs = np.isin(conus_hucs, huc_list).squeeze()
     indices_j, indices_i = np.where(sel_hucs > 0)
     return conus_hucs, sel_hucs, indices_j, indices_i
 
 
-def _indices_to_ij(conus_hucs, indices_j, indices_i):
-    """Get the conus ij-bounds for the conus_hucs boundary defined by indices_j and indices_i.                                                  
+def _indices_to_ij(indices_j, indices_i):
+    """Get the conus ij-bounds for the boundary defined by indices_j and indices_i.                                                  
 
     Args:                                                                                                                           
-        conus_hucs (numpy.ndarray): conus huc data                                                                                             
         indices_j (numpy.ndarray): mask in the j direction for selected hucs                                                                    
         indices_i (numpy.ndarray): mask in the i direction for selected hucs                                                                   
  
     Returns:                                                                                                         
         A tuple of the form (imin, jmin, imax, jmax) representing the bounds                                                                    
         in conus_hucs defined by the two mask arrays indices_j and indices_i.                                                                   
     """
@@ -119,23 +119,18 @@
     Example:
 
     .. code-block:: python
 
         grid_bounds = latlon_to_ij(latlon_bounds=[[37.91, -91.43], [37.34, -90.63]], grid="conus2")
     """
     _validate_grid(grid)    
-    if not isinstance(latlon_bounds, list):
-        raise TypeError("latlon_bounds must be a list")
+    _validate_latlon_list(latlon_bounds)
     if len(latlon_bounds) != 2:
         raise ValueError("latlon_bounds must contain exactly two lat-lon points: [[lat1, lon1], [lat2, lon2]]")
-    for point in latlon_bounds:
-        if not (isinstance(point, list) and
-                len(point) == 2 and
-                all(isinstance(value, (int, float)) for value in point)):
-            raise ValueError("latlon_bounds must contain exactly two lat-lon points: [[lat1, lon1], [lat2, lon2]]")
+
     grid = grid.lower()
     point0 = hf_hydrodata.to_ij(grid, latlon_bounds[0][0], latlon_bounds[0][1])
     point1 = hf_hydrodata.to_ij(grid, latlon_bounds[1][0], latlon_bounds[1][1])
     imin, imax = [
         min(point0[0], point1[0]),
         max(point0[0], point1[0]),
     ]
@@ -176,43 +171,34 @@
             write_dir="/path/to/your/chosen/directory"
         )
     """
     _validate_huc_list(huc_list)
     _validate_grid(grid)
     _validate_dir(write_dir)
     grid = grid.lower()
-    conus_hucs, sel_hucs, indices_j, indices_i = _get_conus_hucs_indices(huc_list, grid)
+    _, sel_hucs, indices_j, indices_i = _get_conus_hucs_indices(huc_list, grid)
     if indices_i.size == 0 or indices_j.size == 0:
         raise ValueError(f"The area defined by the provided HUCs is not part of the {grid} grid.")      
-    arr_jmin = np.min(indices_j)
-    arr_jmax = np.max(indices_j) + 1  # right bound inclusive
-    ij_bounds = _indices_to_ij(conus_hucs, indices_j, indices_i)
-
-    nj = ij_bounds[3] - ij_bounds[1]
-    ni = ij_bounds[2] - ij_bounds[0]
+    imin, jmin, imax, jmax = _indices_to_ij(indices_j, indices_i)
+    nj = jmax - jmin
+    ni = imax - imin
 
     # checks conus1 / 2 grid and assigns appripriate dz and z_total for making the mask and solid file
     if grid  == "conus1":
         print("grid is conus1")
         layz = 100
         z_total = str(500)
     else:
         print("grid is conus2")
         layz = 200
         z_total = str(2000)
-    # could look this up in dC and get the information
 
     # create and write the pfb mask
     mask_clip = np.zeros((1, nj, ni))
-    mask_clip[0, :, :] = sel_hucs[
-        arr_jmin:arr_jmax, ij_bounds[0] : ij_bounds[2]
-    ]  # we need to use numpy iymin / iymax because we are subsetting the tif file
-#    mask_clip = np.flip(
-#        mask_clip, 1
-#    )  # This flip tooks the section we just subset and puts it in the appropriate parflow orientation
+    mask_clip[0, :, :] = sel_hucs[jmin:jmax, imin:imax]
     mask_clip = mask_clip.astype(float)
     mask_file_path = os.path.join(write_dir, "mask.pfb")
     write_pfb(mask_file_path, mask_clip, dx=1000, dy=1000, dz=layz, dist=False)
     print("Wrote mask.pfb")
     mask_vtk_path = os.path.join(write_dir, "mask_vtk.vtk")
     solid_file_path = os.path.join(write_dir, "solidfile.pfsol")
 
@@ -958,26 +944,29 @@
     run.Process.Topology.P = P
     run.Process.Topology.Q = Q
 
     if dist_clim_forcing:
         print("Distributing your climate forcing")
         forcing_dir = run.Solver.CLM.MetFilePath
         _validate_dir(forcing_dir)
-        for filename in pathlib.Path(forcing_dir).glob("*.pfb"):
-            run.dist(filename)
+        for file_name in os.listdir(forcing_dir):
+            if file_name.endswith(".pfb") and ".out." not in file_name:
+                file_path = os.path.join(forcing_dir, file_name)
+                run.dist(file_path)
     else:
-        print("no forcing directory provided, only distributing static inputs")
+        print("No forcing directory provided, only distributing static inputs")
 
-    static_input_paths = pathlib.Path(working_dir).glob("*.pfb")
     max_nz = 0
-    for path in static_input_paths:
-        input_array = read_pfb(path)
-        nz = input_array.shape[0]
-        if nz > max_nz:
-            max_nz = nz
-        run.dist(path)
-        print(f"Distributed {os.path.basename(path)} with NZ {nz}")
+    for file_name in os.listdir(working_dir):
+        if file_name.endswith(".pfb") and ".out." not in file_name:
+            file_path = os.path.join(working_dir, file_name)
+            input_array = read_pfb(file_path)
+            nz = input_array.shape[0]
+            if nz > max_nz:
+                max_nz = nz
+            run.dist(file_path)
+            print(f"Distributed {os.path.basename(file_path)} with NZ {nz}")
     run.ComputationalGrid.NZ = max_nz
 
     _, file_extension = os.path.splitext(runscript_path)
     file_path, _ = run.write(working_directory=working_dir, file_format=f"{file_extension[1:]}")
     return file_path
```

### Comparing `subsettools-1.0.3/PKG-INFO` & `subsettools-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subsettools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Subsetting tools and utilities for ParFlow
 License: MIT
 Author: George Artavanis, Amanda Triplett
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -38,7 +38,8 @@
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines on the [SubsetTools GitHub repo](https://github.com/hydroframe/subsettools). Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
 `subsettools` is part of the [HydroFrame project](https://hydroframe.org/). It is licensed under the terms of the MIT license.
 
+Copyright 2024 The Trustees of Princeton University and The Arizona Board of Regents on behalf of the University of Arizona, College of Science Hydrology & Atmospheric Sciences
```


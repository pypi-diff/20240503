# Comparing `tmp/metatensor-torch-0.4.0.tar.gz` & `tmp/metatensor_torch-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metatensor-torch-0.4.0.tar", last modified: Thu Apr 11 12:23:56 2024, max compression
+gzip compressed data, was "metatensor_torch-0.5.0.tar", last modified: Fri May  3 12:06:49 2024, max compression
```

## Comparing `metatensor-torch-0.4.0.tar` & `metatensor_torch-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.035126 metatensor-torch-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-11 12:23:56.035126 metatensor-torch-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.031126 metatensor-torch-0.4.0/build-backend/
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/build-backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.031126 metatensor-torch-0.4.0/metatensor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.031126 metatensor-torch-0.4.0/metatensor/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/_c_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.035126 metatensor-torch-0.4.0/metatensor/torch/atomistic/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17368 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/ase_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26835 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/systems_to_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    48268 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/learn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    59407 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor-torch-cxx-0.4.0.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.035126 metatensor-torch-0.4.0/metatensor_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:23:55.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:23:55.000000 metatensor-torch-0.4.0/n_commits_since_last_tag
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:23:56.035126 metatensor-torch-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.658967 metatensor_torch-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-03 12:06:49.658967 metatensor_torch-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.654967 metatensor_torch-0.5.0/build-backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/build-backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.650967 metatensor_torch-0.5.0/metatensor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.654967 metatensor_torch-0.5.0/metatensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/_c_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.654967 metatensor_torch-0.5.0/metatensor/torch/atomistic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18054 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/ase_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27073 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/atomistic/systems_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48268 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/metatensor/torch/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61377 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor-torch-cxx-0.5.0.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:49.658967 metatensor_torch-0.5.0/metatensor_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/metatensor_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:06:49.000000 metatensor_torch-0.5.0/n_commits_since_last_tag
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:06:49.658967 metatensor_torch-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12132 2024-05-03 12:06:24.000000 metatensor_torch-0.5.0/setup.py
```

### Comparing `metatensor-torch-0.4.0/LICENSE` & `metatensor_torch-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.4.0/PKG-INFO` & `metatensor_torch-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatensor-torch
-Version: 0.4.0
+Version: 0.5.0
 Summary: TorchScript bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
 Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
 Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/torch/CHANGELOG.html
```

### Comparing `metatensor-torch-0.4.0/build-backend/backend.py` & `metatensor_torch-0.5.0/build-backend/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 
 
 ROOT = os.path.realpath(os.path.dirname(__file__))
 METATENSOR_CORE = os.path.realpath(os.path.join(ROOT, "..", "..", "metatensor-core"))
 FORCED_METATENSOR_CORE_VERSION = os.environ.get(
     "METATENSOR_TORCH_BUILD_WITH_METATENSOR_CORE_VERSION"
 )
+METATENSOR_NO_LOCAL_DEPS = os.environ.get("METATENSOR_NO_LOCAL_DEPS", "0") == "1"
+
 
 if FORCED_METATENSOR_CORE_VERSION is not None:
     # force a specific version for metatensor-core, this is used when checking the build
     # from a sdist on a non-released version
     METATENSOR_CORE_DEP = f"metatensor-core =={FORCED_METATENSOR_CORE_VERSION}"
 
-elif os.path.exists(METATENSOR_CORE):
+elif not METATENSOR_NO_LOCAL_DEPS and os.path.exists(METATENSOR_CORE):
     # we are building from a git checkout
 
     # add a random uuid to the file url to prevent pip from using a cached
     # wheel for metatensor-core, and force it to re-build from scratch
     uuid = uuid.uuid4()
     METATENSOR_CORE_DEP = f"metatensor-core @ file://{METATENSOR_CORE}?{uuid}"
 else:
```

### Comparing `metatensor-torch-0.4.0/metatensor/torch/__init__.py` & `metatensor_torch-0.5.0/metatensor/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.4.0/metatensor/torch/_c_lib.py` & `metatensor_torch-0.5.0/metatensor/torch/_c_lib.py`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.4.0/metatensor/torch/atomistic/__init__.py` & `metatensor_torch-0.5.0/metatensor/torch/atomistic/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import os
 
 if os.environ.get("METATENSOR_IMPORT_FOR_SPHINX", "0") != "0":
-    from .documentation import System, NeighborsListOptions
+    from .documentation import System, NeighborListOptions
     from .documentation import (
         ModelOutput,
         ModelEvaluationOptions,
         ModelCapabilities,
         ModelMetadata,
     )
 
@@ -15,15 +15,15 @@
         load_model_extensions,
         register_autograd_neighbors,
         unit_conversion_factor,
     )
 
 else:
     System = torch.classes.metatensor.System
-    NeighborsListOptions = torch.classes.metatensor.NeighborsListOptions
+    NeighborListOptions = torch.classes.metatensor.NeighborListOptions
 
     ModelOutput = torch.classes.metatensor.ModelOutput
     ModelEvaluationOptions = torch.classes.metatensor.ModelEvaluationOptions
     ModelCapabilities = torch.classes.metatensor.ModelCapabilities
     ModelMetadata = torch.classes.metatensor.ModelMetadata
 
     load_model_extensions = torch.ops.metatensor.load_model_extensions
```

### Comparing `metatensor-torch-0.4.0/metatensor/torch/atomistic/_extensions.py` & `metatensor_torch-0.5.0/metatensor/torch/atomistic/_extensions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import hashlib
 import os
 import shutil
 import site
 
 import torch
 
+from .. import _c_lib
+
+
+METATENSOR_TORCH_LIB_PATH = _c_lib._lib_path()
+
 
 def _rascaline_lib_path():
     import rascaline
 
     return [rascaline._c_lib._lib_path()]
 
 
@@ -32,14 +37,17 @@
         # should we store the files directly inside the model file? This would makes
         # the model platform-specific but much more convenient (since the end user
         # does not have to move a model around)
 
     extensions = []
     extensions_deps = []
     for library in torch.ops.loaded_libraries:
+        if library == METATENSOR_TORCH_LIB_PATH:
+            continue
+
         path = _copy_extension(library, extensions_path)
         info = _extension_info(library)
         info["path"] = path
         extensions.append(info)
 
         for extra in EXTENSIONS_WITH_DEPENDENCIES.get(info["name"], lambda: [])():
             path = _copy_extension(extra, extensions_path)
```

### Comparing `metatensor-torch-0.4.0/metatensor/torch/atomistic/ase_calculator.py` & `metatensor_torch-0.5.0/metatensor/torch/atomistic/ase_calculator.py`

 * *Files 6% similar despite different names*

```diff
@@ -195,24 +195,24 @@
         """
         types, positions, cell = _ase_to_torch_data(
             atoms=atoms, dtype=self._dtype, device=self._device
         )
         system = System(types, positions, cell)
 
         # Compute the neighbors lists requested by the model using ASE NL
-        for options in self._model.requested_neighbors_lists():
+        for options in self._model.requested_neighbor_lists():
             neighbors = _compute_ase_neighbors(
                 atoms, options, dtype=self._dtype, device=self._device
             )
             register_autograd_neighbors(
                 system,
                 neighbors,
                 check_consistency=self.parameters["check_consistency"],
             )
-            system.add_neighbors_list(options, neighbors)
+            system.add_neighbor_list(options, neighbors)
 
         options = ModelEvaluationOptions(
             length_unit="angstrom",
             outputs=outputs,
             selected_atoms=selected_atoms,
         )
         return self._model(
@@ -270,24 +270,24 @@
             cell = cell @ scaling
 
         if "stresses" in properties:
             raise NotImplementedError("'stresses' are not implemented yet")
 
         # convert from ase.Atoms to metatensor.torch.atomistic.System
         system = System(types, positions, cell)
-        for options in self._model.requested_neighbors_lists():
+        for options in self._model.requested_neighbor_lists():
             neighbors = _compute_ase_neighbors(
                 atoms, options, dtype=self._dtype, device=self._device
             )
             register_autograd_neighbors(
                 system,
                 neighbors,
                 check_consistency=self.parameters["check_consistency"],
             )
-            system.add_neighbors_list(options, neighbors)
+            system.add_neighbor_list(options, neighbors)
 
         run_options = ModelEvaluationOptions(
             length_unit="angstrom",
             outputs=outputs,
             selected_atoms=None,
         )
 
@@ -407,63 +407,77 @@
     if "stresses" in properties:
         output.explicit_gradients = ["cell"]
 
     return {"energy": output}
 
 
 def _compute_ase_neighbors(atoms, options, dtype, device):
-    engine_cutoff = options.engine_cutoff(engine_length_unit="angstrom")
-    nl = ase.neighborlist.NeighborList(
-        cutoffs=[engine_cutoff] * len(atoms),
-        skin=0.0,
-        sorted=False,
-        self_interaction=False,
-        bothways=options.full_list,
-        primitive=ase.neighborlist.NewPrimitiveNeighborList,
+    nl_i, nl_j, nl_S, nl_D = ase.neighborlist.neighbor_list(
+        "ijSD",
+        atoms,
+        cutoff=options.engine_cutoff(engine_length_unit="angstrom"),
     )
-    nl.update(atoms)
 
-    cell = torch.from_numpy(atoms.cell[:])
-    positions = torch.from_numpy(atoms.positions)
+    selected = []
+    for pair_i, (i, j, S) in enumerate(zip(nl_i, nl_j, nl_S)):
+        # we want a half neighbor list, so drop all duplicated neighbors
+        if j < i:
+            continue
+        elif i == j:
+            if S[0] == 0 and S[1] == 0 and S[2] == 0:
+                # only create pairs with the same atom twice if the pair spans more
+                # than one unit cell
+                continue
+            elif S[0] + S[1] + S[2] < 0 or (
+                (S[0] + S[1] + S[2] == 0) and (S[2] < 0 or (S[2] == 0 and S[1] < 0))
+            ):
+                # When creating pairs between an atom and one of its periodic
+                # images, the code generate multiple redundant pairs (e.g. with
+                # shifts 0 1 1 and 0 -1 -1); and we want to only keep one of these.
+                # We keep the pair in the positive half plane of shifts.
+                continue
 
-    samples = []
-    distances = []
-    cutoff2 = engine_cutoff * engine_cutoff
-    for i in range(len(atoms)):
-        indices, offsets = nl.get_neighbors(i)
-        for j, offset in zip(indices, offsets):
-            distance = positions[j] - positions[i] + offset.dot(cell)
+        selected.append(pair_i)
 
-            distance2 = torch.dot(distance, distance).item()
+    selected = np.array(selected, dtype=np.int32)
+    n_pairs = len(selected)
 
-            if distance2 > cutoff2:
-                continue
+    if options.full_list:
+        distances = np.empty((2 * n_pairs, 3), dtype=np.float64)
+        samples = np.empty((2 * n_pairs, 5), dtype=np.int32)
+    else:
+        distances = np.empty((n_pairs, 3), dtype=np.float64)
+        samples = np.empty((n_pairs, 5), dtype=np.int32)
 
-            samples.append((i, j, offset[0], offset[1], offset[2]))
-            distances.append(distance.to(dtype=dtype, device=device))
+    samples[:n_pairs, 0] = nl_i[selected]
+    samples[:n_pairs, 1] = nl_j[selected]
+    samples[:n_pairs, 2:] = nl_S[selected]
 
-    if len(distances) == 0:
-        distances = torch.zeros((0, 3), dtype=dtype, device=device)
-        samples = torch.zeros((0, 5), dtype=torch.int32, device=device)
-    else:
-        samples = torch.tensor(samples, device=device)
-        distances = torch.vstack(distances)
+    distances[:n_pairs] = nl_D[selected]
+
+    if options.full_list:
+        samples[n_pairs:, 0] = nl_j[selected]
+        samples[n_pairs:, 1] = nl_i[selected]
+        samples[n_pairs:, 2:] = -nl_S[selected]
+
+        distances[n_pairs:] = -nl_D[selected]
 
+    distances = torch.from_numpy(distances).to(dtype=dtype).to(device=device)
     return TensorBlock(
         values=distances.reshape(-1, 3, 1),
         samples=Labels(
             names=[
                 "first_atom",
                 "second_atom",
                 "cell_shift_a",
                 "cell_shift_b",
                 "cell_shift_c",
             ],
-            values=samples,
-        ),
+            values=torch.from_numpy(samples),
+        ).to(device=device),
         components=[Labels.range("xyz", 3).to(device)],
         properties=Labels.range("distance", 1).to(device),
     )
 
 
 def _ase_to_torch_data(atoms, dtype, device):
     """Get the positions and cell from ASE atoms as torch tensors"""
```

### Comparing `metatensor-torch-0.4.0/metatensor/torch/atomistic/documentation.py` & `metatensor_torch-0.5.0/metatensor/torch/atomistic/documentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,17 +90,17 @@
 
         :param dtype: new dtype to use for all arrays. The dtype stays the same if this
             is set to ``None``.
         :param device: new device to use for all arrays. The device stays the same if
             this is set to ``None``.
         """
 
-    def add_neighbors_list(
+    def add_neighbor_list(
         self,
-        options: "NeighborsListOptions",
+        options: "NeighborListOptions",
         neighbors: TensorBlock,
     ):
         """
         Add a new neighbors list in this system corresponding to the given ``options``.
 
         The neighbors list should have the following samples: ``"first_atom"``,
         ``"second_atom"``, ``"cell_shift_a"``, ``"cell_shift_b"``, ``"cell_shift_c"``,
@@ -115,26 +115,26 @@
         second atom, i.e. ``positions[second_atom] - positions[first_atom] +
         cell_shift_a * cell_a + cell_shift_b * cell_b + cell_shift_c * cell_c``.
 
         :param options: options of the neighbors list
         :param neighbors: list of neighbors stored in a :py:class:`TensorBlock`
         """
 
-    def get_neighbors_list(
+    def get_neighbor_list(
         self,
-        options: "NeighborsListOptions",
+        options: "NeighborListOptions",
     ) -> TensorBlock:
         """
         Retrieve a previously stored neighbors list with the given ``options``, or throw
         an error if no such neighbors list exists.
 
         :param options: options of the neighbors list to retrieve
         """
 
-    def known_neighbors_lists(self) -> List["NeighborsListOptions"]:
+    def known_neighbor_lists(self) -> List["NeighborListOptions"]:
         """
         Get all the neighbors lists options registered with this :py:class:`System`
         """
 
     def add_data(self, name: str, data: TensorBlock, override: bool = False):
         """
         Add custom data to this system, stored as :py:class:`TensorBlock`.
@@ -158,15 +158,15 @@
 
     def known_data(self) -> List[str]:
         """
         Get the name of all the custom data registered with this :py:class:`System`
         """
 
 
-class NeighborsListOptions:
+class NeighborListOptions:
     """Options for the calculation of a neighbors list"""
 
     def __init__(self, cutoff: float, full_list: bool, requestor: str = ""):
         """
         :param cutoff: spherical cutoff radius for the neighbors list, in the
             model units
         :param full_list: should the list be a full or half neighbors list
@@ -214,18 +214,18 @@
 
     def __repr__(self) -> str:
         pass
 
     def __str__(self) -> str:
         pass
 
-    def __eq__(self, other: "NeighborsListOptions") -> bool:
+    def __eq__(self, other: "NeighborListOptions") -> bool:
         pass
 
-    def __ne__(self, other: "NeighborsListOptions") -> bool:
+    def __ne__(self, other: "NeighborListOptions") -> bool:
         pass
 
 
 class ModelOutput:
     """Description of one of the quantity a model can compute."""
 
     def __init__(
@@ -465,15 +465,15 @@
     ``neighbors.values`` was computed directly from ``system.positions`` and
     ``system.cell``, allowing downstream models to use it directly with full autograd
     integration.
 
     :param system: system containing the positions and cell used to compute the
         neighbors list
     :param system: neighbors list, following the same format as
-        :py:meth:`System.add_neighbors_list`
+        :py:meth:`System.add_neighbor_list`
     :param check_consistency: can be set to ``True`` to run a handful of additional
         checks in case the data in neighbors does not follow what's expected.
     """
 
 
 def unit_conversion_factor(quantity: str, from_unit: str, to_unit: str):
     """
```

### Comparing `metatensor-torch-0.4.0/metatensor/torch/atomistic/model.py` & `metatensor_torch-0.5.0/metatensor/torch/atomistic/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .. import __version__ as metatensor_version
 from .. import dtype_name
 from . import (
     ModelCapabilities,
     ModelEvaluationOptions,
     ModelMetadata,
     ModelOutput,
-    NeighborsListOptions,
+    NeighborListOptions,
     System,
     check_atomistic_model,
     load_model_extensions,
     unit_conversion_factor,
 )
 from ._extensions import _collect_extensions
 from .outputs import _check_outputs
@@ -34,34 +34,34 @@
     and :py:func:`metatensor.torch.atomistic.load_model_extensions()` before attempting
     to load the model.
 
     :param path: path to an exported metatensor model
     :param extensions_directory: path to a directory containing all extensions required
         by the exported model
     """
-    check_atomistic_model(path)
     load_model_extensions(path, extensions_directory)
+    check_atomistic_model(path)
     return torch.jit.load(path)
 
 
 class ModelInterface(torch.nn.Module):
     """
     Interface for models that can be used with :py:class:`MetatensorAtomisticModel`.
 
     There are several requirements that models must satisfy to be usable with
     :py:class:`MetatensorAtomisticModel`. The main one is concerns the
     :py:meth:`forward` function, which must have the signature defined in this
     interface.
 
     Additionally, the model can request neighbor lists to be computed by the simulation
     engine, and stored inside the input :py:class:`System`. This is done by defining the
-    optional :py:meth:`requested_neighbors_lists` method for the model or any of it's
+    optional :py:meth:`requested_neighbor_lists` method for the model or any of it's
     sub-module.
 
-    :py:class:`MetatensorAtomisticModel` will check if ``requested_neighbors_lists`` is
+    :py:class:`MetatensorAtomisticModel` will check if ``requested_neighbor_lists`` is
     defined for all the sub-modules of the model, then collect and unify identical
     requests for the simulation engine.
     """
 
     def __init__():
         """"""
         pass
@@ -101,32 +101,35 @@
         :param systems: atomistic systems on which to run the calculation
         :param outputs: set of outputs requested by the simulation engine
         :param selected_atoms: subset of atoms that should be included in the output,
             defaults to None
         :return: properties of the systems, as predicted by the machine learning model
         """
 
-    def requested_neighbors_lists(self) -> List[NeighborsListOptions]:
+    def requested_neighbor_lists(self) -> List[NeighborListOptions]:
         """
         Optional function declaring which neighbors list this model requires.
 
         This function can be defined on either the root model or any of it's
         sub-modules. A single module can request multiple neighbors list simultaneously
         if it needs them.
 
         It is then the responsibility of the code calling the model to:
 
         1. call this function (or more generally
-           :py:meth:`MetatensorAtomisticModel.requested_neighbors_lists`) to get the
+           :py:meth:`MetatensorAtomisticModel.requested_neighbor_lists`) to get the
            list of requests;
         2. compute all neighbor lists corresponding to these requests and add them to
            the systems before calling the model.
         """
 
 
+# This class name is prefixed with `Metatensor` because we are checking the class name
+# before loading a saved model `check_atomistic_model`, to try to prevent people from
+# loading arbitrary pytorch models inside the metatensor interface.
 class MetatensorAtomisticModel(torch.nn.Module):
     """
     :py:class:`MetatensorAtomisticModel` is the main entry point for atomistic machine
     learning based on metatensor. It is the interface between custom, user-defined
     models and simulation engines. Users should wrap their models with this class, and
     use :py:meth:`export()` to save and export the model to a file. The exported models
     can then be loaded by a simulation engine to compute properties of atomistic
@@ -228,15 +231,15 @@
     >>> # export the model
     >>> with tempfile.TemporaryDirectory() as directory:
     ...     wrapped.export(os.path.join(directory, "constant-energy-model.pt"))
     ...
     """
 
     # Some annotation to make the TorchScript compiler happy
-    _requested_neighbors_lists: List[NeighborsListOptions]
+    _requested_neighbor_lists: List[NeighborListOptions]
 
     def __init__(
         self,
         module: ModelInterface,
         metadata: ModelMetadata,
         capabilities: ModelCapabilities,
     ):
@@ -256,20 +259,20 @@
             raise ValueError("module should not be in training mode")
 
         _check_annotation(module)
         self._module = module
 
         # ============================================================================ #
 
-        # recursively explore `module` to get all the requested_neighbors_lists
-        self._requested_neighbors_lists = []
-        _get_requested_neighbors_lists(
+        # recursively explore `module` to get all the requested_neighbor_lists
+        self._requested_neighbor_lists = []
+        _get_requested_neighbor_lists(
             self._module,
             self._module.__class__.__name__,
-            self._requested_neighbors_lists,
+            self._requested_neighbor_lists,
             capabilities.length_unit,
         )
         # ============================================================================ #
 
         self._metadata = metadata
         self._capabilities = capabilities
 
@@ -316,20 +319,20 @@
 
     @torch.jit.export
     def metadata(self) -> ModelMetadata:
         """Get the metadata of the wrapped model"""
         return self._metadata
 
     @torch.jit.export
-    def requested_neighbors_lists(self) -> List[NeighborsListOptions]:
+    def requested_neighbor_lists(self) -> List[NeighborListOptions]:
         """
         Get the neighbors lists required by the wrapped model or any of the child
         module.
         """
-        return self._requested_neighbors_lists
+        return self._requested_neighbor_lists
 
     def forward(
         self,
         systems: List[System],
         options: ModelEvaluationOptions,
         check_consistency: bool,
     ) -> Dict[str, TensorMap]:
@@ -339,27 +342,27 @@
         unit to the model unit, including all neighbors lists distances.
 
         After running the model, this will convert all the outputs from the model units
         to the engine units.
 
         :param systems: input systems on which we should run the model. The systems
             should already contain all neighbors lists corresponding to the options in
-            :py:meth:`requested_neighbors_lists()`.
+            :py:meth:`requested_neighbor_lists()`.
         :param options: options for this run of the model
         :param check_consistency: Should we run additional check that everything is
             consistent? This should be set to ``True`` when verifying a model, and to
             ``False`` once you are sure everything is running fine.
 
         :return: A dictionary containing all the model outputs
         """
 
         if check_consistency:
             _check_inputs(
                 capabilities=self._capabilities,
-                requested_neighbors_lists=self._requested_neighbors_lists,
+                requested_neighbor_lists=self._requested_neighbor_lists,
                 systems=systems,
                 options=options,
                 expected_dtype=self._model_dtype,
             )
 
         # convert systems from engine to model units
         if self._capabilities.length_unit != options.length_unit:
@@ -463,22 +466,22 @@
                 "extensions": json.dumps(extensions),
                 "extensions-deps": json.dumps(deps),
                 "metadata": json.dumps(export_metadata),
             },
         )
 
 
-def _get_requested_neighbors_lists(
+def _get_requested_neighbor_lists(
     module: torch.nn.Module,
     module_name: str,
-    requested: List[NeighborsListOptions],
+    requested: List[NeighborListOptions],
     length_unit: str,
 ):
-    if hasattr(module, "requested_neighbors_lists"):
-        for new_options in module.requested_neighbors_lists():
+    if hasattr(module, "requested_neighbor_lists"):
+        for new_options in module.requested_neighbor_lists():
             new_options.add_requestor(module_name)
 
             already_requested = False
             for existing in requested:
                 if existing == new_options:
                     already_requested = True
                     for requestor in new_options.requestors():
@@ -492,15 +495,15 @@
                         f"match the model length units ('{length_unit}')"
                     )
 
                 new_options.length_unit = length_unit
                 requested.append(new_options)
 
     for child_name, child in module.named_children():
-        _get_requested_neighbors_lists(
+        _get_requested_neighbor_lists(
             module=child,
             module_name=module_name + "." + child_name,
             requested=requested,
             length_unit=length_unit,
         )
 
 
@@ -551,15 +554,15 @@
             "`forward()` must return a `Dict[str, TensorMap]`, "
             f"not {annotations['return']}"
         )
 
 
 def _check_inputs(
     capabilities: ModelCapabilities,
-    requested_neighbors_lists: List[NeighborsListOptions],
+    requested_neighbor_lists: List[NeighborListOptions],
     systems: List[System],
     options: ModelEvaluationOptions,
     expected_dtype: torch.dtype,
 ):
     if len(systems) == 0:
         return
 
@@ -611,15 +614,15 @@
         possible_atoms_values: List[List[int]] = []
         for s, system in enumerate(systems):
             for a in range(len(system)):
                 possible_atoms_values.append([s, a])
 
         possible_atoms = Labels(
             ["system", "atom"],
-            torch.tensor(possible_atoms_values),
+            torch.tensor(possible_atoms_values, device=global_device),
         )
 
         intersection = selected_atoms.intersection(possible_atoms)
         if len(intersection) != len(selected_atoms):
             raise ValueError(
                 "invalid selected_atoms: there are entries that are not "
                 "possible for the current systems"
@@ -639,22 +642,22 @@
             )
 
         # check that the atomic types of the system match the one the model supports
         all_types = torch.unique(system.types)
         for atom_type in all_types:
             if atom_type not in capabilities.atomic_types:
                 raise ValueError(
-                    f"this model can not run for the atomic type '{atom_type}'"
+                    f"this model can not run for the atomic type '{atom_type.item()}'"
                 )
 
         # Check neighbors lists
-        known_neighbors_lists = system.known_neighbors_lists()
-        for request in requested_neighbors_lists:
+        known_neighbor_lists = system.known_neighbor_lists()
+        for request in requested_neighbor_lists:
             found = False
-            for known in known_neighbors_lists:
+            for known in known_neighbor_lists:
                 if request == known:
                     found = True
 
             if not found:
                 raise ValueError(
                     "missing neighbors list in the system: the model requested "
                     f"a list for {request}, but it was not computed and stored "
@@ -676,17 +679,17 @@
         new_system = System(
             types=system.types,
             positions=conversion * system.positions,
             cell=conversion * system.cell,
         )
 
         # also update the neighbors list distances
-        for request in system.known_neighbors_lists():
-            neighbors = system.get_neighbors_list(request)
-            new_system.add_neighbors_list(
+        for request in system.known_neighbor_lists():
+            neighbors = system.get_neighbor_list(request)
+            new_system.add_neighbor_list(
                 request,
                 TensorBlock(
                     values=conversion * neighbors.values,
                     samples=neighbors.samples,
                     components=neighbors.components,
                     properties=neighbors.properties,
                 ),
```

### Comparing `metatensor-torch-0.4.0/metatensor/torch/atomistic/outputs.py` & `metatensor_torch-0.5.0/metatensor/torch/atomistic/outputs.py`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.4.0/metatensor/torch/atomistic/systems_to_torch.py` & `metatensor_torch-0.5.0/metatensor/torch/atomistic/systems_to_torch.py`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.4.0/metatensor/torch/documentation.py` & `metatensor_torch-0.5.0/metatensor/torch/documentation.py`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.4.0/metatensor/torch/learn.py` & `metatensor_torch-0.5.0/metatensor/torch/learn.py`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.4.0/metatensor/torch/operations.py` & `metatensor_torch-0.5.0/metatensor/torch/operations.py`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.4.0/metatensor/torch/utils.py` & `metatensor_torch-0.5.0/metatensor/torch/utils.py`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.4.0/metatensor_torch.egg-info/PKG-INFO` & `metatensor_torch-0.5.0/metatensor_torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatensor-torch
-Version: 0.4.0
+Version: 0.5.0
 Summary: TorchScript bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
 Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
 Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/torch/CHANGELOG.html
```

### Comparing `metatensor-torch-0.4.0/metatensor_torch.egg-info/SOURCES.txt` & `metatensor_torch-0.5.0/metatensor_torch.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.rst
-metatensor-torch-cxx-0.4.0.tar.gz
+metatensor-torch-cxx-0.5.0.tar.gz
 n_commits_since_last_tag
 pyproject.toml
 setup.py
 build-backend/backend.py
 metatensor/torch/__init__.py
 metatensor/torch/_c_lib.py
 metatensor/torch/documentation.py
```

### Comparing `metatensor-torch-0.4.0/pyproject.toml` & `metatensor_torch-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.4.0/setup.py` & `metatensor_torch-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,15 +287,26 @@
         authors = fd.read().splitlines()
 
     if authors[0].startswith(".."):
         # handle "raw" symlink files (on Windows or from full repo tarball)
         with open(os.path.join(ROOT, authors[0])) as fd:
             authors = fd.read().splitlines()
 
-    install_requires = ["torch >= 1.12"]
+    try:
+        import torch
+
+        # if we have torch, we are building a wheel, which will only be compatible with
+        # a single torch version
+        torch_v_major, torch_v_minor, *_ = torch.__version__.split(".")
+        torch_version = f"== {torch_v_major}.{torch_v_minor}.*"
+    except ImportError:
+        # otherwise we are building a sdist
+        torch_version = ">= 1.12"
+
+    install_requires = [f"torch {torch_version}"]
 
     # when packaging a sdist for release, we should never use local dependencies
     METATENSOR_NO_LOCAL_DEPS = os.environ.get("METATENSOR_NO_LOCAL_DEPS", "0") == "1"
 
     if not METATENSOR_NO_LOCAL_DEPS and os.path.exists(METATENSOR_CORE):
         # we are building from a git checkout
```


# Comparing `tmp/physics-tenpy-0.99.0.tar.gz` & `tmp/physics-tenpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physics-tenpy-0.99.0.tar", last modified: Tue Mar 19 14:03:44 2024, max compression
+gzip compressed data, was "physics-tenpy-1.0.0.tar", last modified: Tue Mar 19 16:52:46 2024, max compression
```

## Comparing `physics-tenpy-0.99.0.tar` & `physics-tenpy-1.0.0.tar`

### file list

```diff
@@ -1,167 +1,160 @@
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.678290 physics-tenpy-0.99.0/
--rw-r--r--   0 jakobunfried   (501) staff       (20)      699 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/AUTHORS.txt
--rw-r--r--   0 jakobunfried   (501) staff       (20)    35149 2023-10-17 09:32:41.000000 physics-tenpy-0.99.0/LICENSE
--rw-r--r--   0 jakobunfried   (501) staff       (20)      283 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/MANIFEST.in
--rw-r--r--   0 jakobunfried   (501) staff       (20)     9077 2024-03-19 14:03:44.678048 physics-tenpy-0.99.0/PKG-INFO
--rw-r--r--   0 jakobunfried   (501) staff       (20)     6538 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/README.rst
--rw-r--r--   0 jakobunfried   (501) staff       (20)      263 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/environment.yml
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.677108 physics-tenpy-0.99.0/physics_tenpy.egg-info/
--rw-r--r--   0 jakobunfried   (501) staff       (20)     9077 2024-03-19 14:03:44.000000 physics-tenpy-0.99.0/physics_tenpy.egg-info/PKG-INFO
--rw-r--r--   0 jakobunfried   (501) staff       (20)     4106 2024-03-19 14:03:44.000000 physics-tenpy-0.99.0/physics_tenpy.egg-info/SOURCES.txt
--rw-r--r--   0 jakobunfried   (501) staff       (20)        1 2024-03-19 14:03:44.000000 physics-tenpy-0.99.0/physics_tenpy.egg-info/dependency_links.txt
--rw-r--r--   0 jakobunfried   (501) staff       (20)       49 2024-03-19 14:03:44.000000 physics-tenpy-0.99.0/physics_tenpy.egg-info/entry_points.txt
--rw-r--r--   0 jakobunfried   (501) staff       (20)      293 2024-03-19 14:03:44.000000 physics-tenpy-0.99.0/physics_tenpy.egg-info/requires.txt
--rw-r--r--   0 jakobunfried   (501) staff       (20)        6 2024-03-19 14:03:44.000000 physics-tenpy-0.99.0/physics_tenpy.egg-info/top_level.txt
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2947 2024-03-19 12:04:25.000000 physics-tenpy-0.99.0/pyproject.toml
--rw-r--r--   0 jakobunfried   (501) staff       (20)       56 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/requirements.txt
--rw-r--r--   0 jakobunfried   (501) staff       (20)       38 2024-03-19 14:03:44.678332 physics-tenpy-0.99.0/setup.cfg
--rw-r--r--   0 jakobunfried   (501) staff       (20)     3040 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/setup.py
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.643806 physics-tenpy-0.99.0/tenpy/
--rw-r--r--   0 jakobunfried   (501) staff       (20)    14358 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/__init__.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      216 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/__main__.py
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.647860 physics-tenpy-0.99.0/tenpy/algorithms/
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1703 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/algorithms/__init__.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    24159 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/algorithms/algorithm.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    28960 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/algorithms/disentangler.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    67640 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/algorithms/dmrg.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     3086 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/algorithms/dmrg_parallel.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    14719 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/algorithms/exact_diag.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     5493 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/algorithms/mpo_evolution.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)   107611 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/algorithms/mps_common.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      482 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/algorithms/mps_sweeps.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    12572 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/algorithms/network_contractor.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    64167 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/algorithms/plane_wave_excitation.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    23027 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/algorithms/purification.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      686 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/algorithms/purification_tebd.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    36955 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/algorithms/tdvp.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    46093 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/algorithms/tebd.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    13928 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/algorithms/truncation.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    41030 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/algorithms/vumps.py
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.652763 physics-tenpy-0.99.0/tenpy/linalg/
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2237 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/linalg/__init__.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)  2481652 2024-03-19 14:03:39.000000 physics-tenpy-0.99.0/tenpy/linalg/_npc_helper.cpp
--rw-r--r--   0 jakobunfried   (501) staff       (20)    76923 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/linalg/_npc_helper.pyx
--rw-r--r--   0 jakobunfried   (501) staff       (20)    67009 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/linalg/charges.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    33138 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/linalg/krylov_based.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1306 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/linalg/lanczos.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)   205489 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/linalg/np_conserved.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     6556 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/linalg/random_matrix.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    34564 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/linalg/sparse.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    11721 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/linalg/svd_robust.py
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.657320 physics-tenpy-0.99.0/tenpy/models/
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1810 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/models/__init__.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     5126 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/aklt.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      834 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/bose_hubbard.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      896 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/bose_hubbard_chain.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2851 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/clock.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      511 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/fermion_chain.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      924 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/fermions_hubbard.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     3213 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/models/fermions_spinless.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     7140 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/models/haldane.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    11428 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/models/hofstadter.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    10378 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/models/hubbard.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)   159896 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/lattice.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    37428 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/models/mixed_xk.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)   100641 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/model.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     4281 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/spins.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     9449 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/spins_nnn.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2821 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/tf_ising.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2853 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/models/tj_model.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     6535 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/toric_code.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     5045 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/models/xxz_chain.py
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.659271 physics-tenpy-0.99.0/tenpy/networks/
--rw-r--r--   0 jakobunfried   (501) staff       (20)      971 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/networks/__init__.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     6151 2024-03-19 12:04:25.000000 physics-tenpy-0.99.0/tenpy/networks/momentum_mps.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)   123303 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/networks/mpo.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)   308901 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/networks/mps.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    26579 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/networks/purification_mps.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    92380 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/networks/site.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    65728 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/networks/terms.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    44825 2024-03-19 12:04:25.000000 physics-tenpy-0.99.0/tenpy/networks/uniform_mps.py
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.660621 physics-tenpy-0.99.0/tenpy/simulations/
--rw-r--r--   0 jakobunfried   (501) staff       (20)      929 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/simulations/__init__.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    59373 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/simulations/ground_state_search.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    18412 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/simulations/measurement.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    11500 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/simulations/post_processing.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    77255 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/simulations/simulation.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    24150 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/simulations/time_evolution.py
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.664610 physics-tenpy-0.99.0/tenpy/tools/
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1495 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/__init__.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    28801 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/cache.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     8840 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/events.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    12811 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/fit.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    49071 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/hdf5_io.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     8864 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/math.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    46408 2024-03-19 12:04:25.000000 physics-tenpy-0.99.0/tenpy/tools/misc.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    15377 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/optimization.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    20868 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tenpy/tools/params.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     6698 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/prediction.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     4986 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/process.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    10297 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/spectral_function_tools.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     3132 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/string.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     5268 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tenpy/tools/thread.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     3677 2024-03-19 13:59:37.000000 physics-tenpy-0.99.0/tenpy/version.py
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.674424 physics-tenpy-0.99.0/tests/
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.676323 physics-tenpy-0.99.0/tests/benchmark/
--rwxr-xr-x   0 jakobunfried   (501) staff       (20)    10574 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/benchmark/benchmark.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      564 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/benchmark/combine_npc.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      956 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/benchmark/combine_numpy.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2070 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/benchmark/dmrg_infinite.py
--rwxr-xr-x   0 jakobunfried   (501) staff       (20)     5765 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/benchmark/profiling.py
--rwxr-xr-x   0 jakobunfried   (501) staff       (20)     3047 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/benchmark/singlerun.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      563 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/benchmark/split_npc.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      824 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/benchmark/split_numpy.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1779 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/benchmark/tebd_infinite.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     3839 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/benchmark/tensordot_npc.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      473 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/benchmark/tensordot_numpy.py
-drwxr-xr-x   0 jakobunfried   (501) staff       (20)        0 2024-03-19 14:03:44.676939 physics-tenpy-0.99.0/tests/export_import_test/
--rw-r--r--   0 jakobunfried   (501) staff       (20)     5948 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/export_import_test/io_test.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2773 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/export_import_test/test_cache.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2361 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/export_import_test/test_hdf5.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     3368 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/export_import_test/test_pickle.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     3752 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/linting.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     4137 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/random_test.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    10599 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/tdvp_numpy.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     6116 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_charges.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    13061 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_dmrg.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2189 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_exact_diag.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1190 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_examples.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     7752 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_krylov_based.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    16676 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_lattice.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    24069 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2041 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_aklt.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      661 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_clock.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1652 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_fermions_spinless.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      677 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_haldane.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1327 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_hofstadter.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1134 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_hubbard.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     5420 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_mixed_xk.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      703 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_spins.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1454 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_spins_nnn.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      665 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_tf_ising.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      302 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_tj_model.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1366 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_toric_code.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2401 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_model_xxz_chain.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    17194 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_mpo.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    39600 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tests/test_mps.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     6653 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_network_contractor.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    35220 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tests/test_np_conserved.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      974 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_package_structure.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     1674 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_params.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     4141 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_post_processing.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2605 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_predict_ram.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     9981 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_purification.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     4860 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_random_matrix.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    15385 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_simulation.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     3886 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_simulation_exc.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    15992 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tests/test_site.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     3837 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_sparse.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2424 2024-03-19 12:04:23.000000 physics-tenpy-0.99.0/tests/test_svd_robust.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     3941 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_tdvp.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     5606 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_tebd.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    14068 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_terms.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    11862 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_time_evolution.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)    11352 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_tools.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2597 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_truncation.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)      781 2024-03-18 18:14:57.000000 physics-tenpy-0.99.0/tests/test_umps.py
--rw-r--r--   0 jakobunfried   (501) staff       (20)     2693 2024-03-19 12:04:25.000000 physics-tenpy-0.99.0/tests/test_vumps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.870699 physics-tenpy-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-03-19 16:52:46.870699 physics-tenpy-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.870699 physics-tenpy-1.0.0/physics_tenpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-03-19 16:52:46.000000 physics-tenpy-1.0.0/physics_tenpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-03-19 16:52:46.000000 physics-tenpy-1.0.0/physics_tenpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 16:52:46.000000 physics-tenpy-1.0.0/physics_tenpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-19 16:52:46.000000 physics-tenpy-1.0.0/physics_tenpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-19 16:52:46.000000 physics-tenpy-1.0.0/physics_tenpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-19 16:52:46.000000 physics-tenpy-1.0.0/physics_tenpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 16:52:46.870699 physics-tenpy-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.838699 physics-tenpy-1.0.0/tenpy/
+-rw-r--r--   0 runner    (1001) docker     (127)    14124 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.842699 physics-tenpy-1.0.0/tenpy/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28960 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/disentangler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62874 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/dmrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/dmrg_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/exact_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/mpo_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104585 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/mps_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/network_contractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64167 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/plane_wave_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22929 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/purification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/tdvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45401 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/tebd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/truncation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41030 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/algorithms/vumps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.846699 physics-tenpy-1.0.0/tenpy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2476405 2024-03-19 16:52:44.000000 physics-tenpy-1.0.0/tenpy/linalg/_npc_helper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    76923 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/linalg/_npc_helper.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    67009 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/linalg/charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31441 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/linalg/krylov_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)   204217 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/linalg/np_conserved.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/linalg/random_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32867 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/linalg/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/linalg/svd_robust.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.850699 physics-tenpy-1.0.0/tenpy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/aklt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/fermions_spinless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/haldane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/hofstadter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10378 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/hubbard.py
+-rw-r--r--   0 runner    (1001) docker     (127)   156227 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37428 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/mixed_xk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94458 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/spins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9391 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/spins_nnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/tf_ising.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/tj_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/toric_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/models/xxz_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.854699 physics-tenpy-1.0.0/tenpy/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/networks/momentum_mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121986 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/networks/mpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   306063 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/networks/mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26579 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/networks/purification_mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86818 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/networks/site.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65728 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/networks/terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44825 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/networks/uniform_mps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.854699 physics-tenpy-1.0.0/tenpy/simulations/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59373 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/simulations/ground_state_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/simulations/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/simulations/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75553 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/simulations/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24150 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/simulations/time_evolution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.858699 physics-tenpy-1.0.0/tenpy/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28801 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49071 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/hdf5_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35158 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/spectral_function_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/tools/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tenpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.866699 physics-tenpy-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.866699 physics-tenpy-1.0.0/tests/benchmark/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10574 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/benchmark/combine_npc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/benchmark/combine_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/benchmark/dmrg_infinite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5765 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/benchmark/profiling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3047 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/benchmark/singlerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/benchmark/split_npc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/benchmark/split_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/benchmark/tebd_infinite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/benchmark/tensordot_npc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/benchmark/tensordot_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:46.866699 physics-tenpy-1.0.0/tests/export_import_test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/export_import_test/io_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/export_import_test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/export_import_test/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/export_import_test/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/tdvp_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13061 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_dmrg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_exact_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_krylov_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16676 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24069 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_aklt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_fermions_spinless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_haldane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_hofstadter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_hubbard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_mixed_xk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_spins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_spins_nnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_tf_ising.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_tj_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_toric_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_model_xxz_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17194 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_mpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39438 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_network_contractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34968 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_np_conserved.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_package_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_predict_ram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_purification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_random_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_simulation_exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16011 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_svd_robust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_tdvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_tebd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14068 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_time_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_umps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-19 16:52:19.000000 physics-tenpy-1.0.0/tests/test_vumps.py
```

### Comparing `physics-tenpy-0.99.0/AUTHORS.txt` & `physics-tenpy-1.0.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/LICENSE` & `physics-tenpy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/PKG-INFO` & `physics-tenpy-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: physics-tenpy
-Version: 0.99.0
+Version: 1.0.0
 Summary: Simulation of quantum many-body systems with tensor networks in Python
 Author: TeNPy Developer Team
 Maintainer-email: Johannes Hauschild <tenpy@johannes-hauschild.de>, Jakob Unfried <jakob.unfried@tum.de>
 License: GPLv3
 Project-URL: Homepage, https://github.com/tenpy/tenpy
 Project-URL: Documentation, https://tenpy.readthedocs.io/
 Project-URL: Source, https://github.com/tenpy/tenpy
 Project-URL: User Forum, https://tenpy.johannes-hauschild.de
 Project-URL: Bug Tracker, https://github.com/tenpy/tenpy/issues
 Keywords: tensor networks,matrix product states
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -29,18 +29,18 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.txt
-Requires-Dist: numpy>=1.13
-Requires-Dist: scipy>=0.18
+Requires-Dist: numpy
+Requires-Dist: scipy
 Provides-Extra: plot
-Requires-Dist: matplotlib>=2.0; extra == "plot"
+Requires-Dist: matplotlib; extra == "plot"
 Provides-Extra: io
 Requires-Dist: h5py; extra == "io"
 Requires-Dist: pyyaml; extra == "io"
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 Provides-Extra: extra
 Requires-Dist: bottleneck; extra == "extra"
```

### Comparing `physics-tenpy-0.99.0/README.rst` & `physics-tenpy-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/physics_tenpy.egg-info/PKG-INFO` & `physics-tenpy-1.0.0/physics_tenpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: physics-tenpy
-Version: 0.99.0
+Version: 1.0.0
 Summary: Simulation of quantum many-body systems with tensor networks in Python
 Author: TeNPy Developer Team
 Maintainer-email: Johannes Hauschild <tenpy@johannes-hauschild.de>, Jakob Unfried <jakob.unfried@tum.de>
 License: GPLv3
 Project-URL: Homepage, https://github.com/tenpy/tenpy
 Project-URL: Documentation, https://tenpy.readthedocs.io/
 Project-URL: Source, https://github.com/tenpy/tenpy
 Project-URL: User Forum, https://tenpy.johannes-hauschild.de
 Project-URL: Bug Tracker, https://github.com/tenpy/tenpy/issues
 Keywords: tensor networks,matrix product states
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -29,18 +29,18 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.txt
-Requires-Dist: numpy>=1.13
-Requires-Dist: scipy>=0.18
+Requires-Dist: numpy
+Requires-Dist: scipy
 Provides-Extra: plot
-Requires-Dist: matplotlib>=2.0; extra == "plot"
+Requires-Dist: matplotlib; extra == "plot"
 Provides-Extra: io
 Requires-Dist: h5py; extra == "io"
 Requires-Dist: pyyaml; extra == "io"
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 Provides-Extra: extra
 Requires-Dist: bottleneck; extra == "extra"
```

### Comparing `physics-tenpy-0.99.0/physics_tenpy.egg-info/SOURCES.txt` & `physics-tenpy-1.0.0/physics_tenpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,40 +19,33 @@
 tenpy/algorithms/algorithm.py
 tenpy/algorithms/disentangler.py
 tenpy/algorithms/dmrg.py
 tenpy/algorithms/dmrg_parallel.py
 tenpy/algorithms/exact_diag.py
 tenpy/algorithms/mpo_evolution.py
 tenpy/algorithms/mps_common.py
-tenpy/algorithms/mps_sweeps.py
 tenpy/algorithms/network_contractor.py
 tenpy/algorithms/plane_wave_excitation.py
 tenpy/algorithms/purification.py
-tenpy/algorithms/purification_tebd.py
 tenpy/algorithms/tdvp.py
 tenpy/algorithms/tebd.py
 tenpy/algorithms/truncation.py
 tenpy/algorithms/vumps.py
 tenpy/linalg/__init__.py
 tenpy/linalg/_npc_helper.cpp
 tenpy/linalg/_npc_helper.pyx
 tenpy/linalg/charges.py
 tenpy/linalg/krylov_based.py
-tenpy/linalg/lanczos.py
 tenpy/linalg/np_conserved.py
 tenpy/linalg/random_matrix.py
 tenpy/linalg/sparse.py
 tenpy/linalg/svd_robust.py
 tenpy/models/__init__.py
 tenpy/models/aklt.py
-tenpy/models/bose_hubbard.py
-tenpy/models/bose_hubbard_chain.py
 tenpy/models/clock.py
-tenpy/models/fermion_chain.py
-tenpy/models/fermions_hubbard.py
 tenpy/models/fermions_spinless.py
 tenpy/models/haldane.py
 tenpy/models/hofstadter.py
 tenpy/models/hubbard.py
 tenpy/models/lattice.py
 tenpy/models/mixed_xk.py
 tenpy/models/model.py
```

### Comparing `physics-tenpy-0.99.0/pyproject.toml` & `physics-tenpy-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=68.0.0", "numpy>1.13", "scipy>=0.18", "Cython>0.29"]
+requires = ["setuptools>=68.0.0", "numpy", "scipy", "Cython>0.29"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "physics-tenpy"
 dynamic = ["version"]
 description = "Simulation of quantum many-body systems with tensor networks in Python"
 readme = {file = "README.rst", content-type = "text/x-rst"}
@@ -14,15 +14,15 @@
 ]
 maintainers = [
     {name = "Johannes Hauschild", email="tenpy@johannes-hauschild.de"},
     {name = "Jakob Unfried", email="jakob.unfried@tum.de"},
 ]
 keywords = ["tensor networks", "matrix product states"]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: C",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -34,20 +34,20 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 dependencies = [
-    "numpy>=1.13",
-    "scipy>=0.18",
+    "numpy",
+    "scipy",
 ]
 
 [project.optional-dependencies]
-plot = ["matplotlib>=2.0"]
+plot = ["matplotlib"]
 io = ["h5py", "pyyaml"]
 test = ["pytest>=6.0"]
 extra = ["bottleneck", "yapf==0.28.0", "docformatter==1.3.1"]
 docbuild = [
     "Sphinx", 
     "sphinx-rtd-theme", 
     "sphinxcontrib-bibtex",
```

### Comparing `physics-tenpy-0.99.0/setup.py` & `physics-tenpy-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/__init__.py` & `physics-tenpy-1.0.0/tenpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,18 +186,14 @@
             val = eval(val_string, context)
             tools.misc.set_recursive(options, key, val, insert_dicts=True)
     if len(options) == 0:
         raise ValueError("No options supplied! Check your command line arguments!")
     if 'output_filename' not in options and 'output_filename_params' not in options:
         raise ValueError("No output filename specified - refuse to run without saving anything!")
     if args.sim_class is not None:  # non-default
-        if 'simulation_class_name' in options:
-            warnings.warn('command line overrides deprecated `simulation_class_name` parameter',
-                          FutureWarning)
-            del options['simulation_class_name']
         options['simulation_class'] = args.sim_class
     if args.RAM:
         # exit immediately
         return estimate_simulation_RAM(suppress_non_RAM_output=True, unit='MB', **options)
     if 'sequential' not in options:
         return run_simulation(**options)
     else:
```

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/__init__.py` & `physics-tenpy-1.0.0/tenpy/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/algorithm.py` & `physics-tenpy-1.0.0/tenpy/algorithms/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """This module contains some base classes for algorithms."""
 # Copyright (C) TeNPy Developers, GNU GPLv3
 
-import warnings
 import time
 import numpy as np
 import logging
 logger = logging.getLogger(__name__)
 
 from .truncation import TruncationError
 from ..tools.misc import consistency_check
@@ -133,21 +132,14 @@
         if options is None:
             options = other_engine.options
         kwargs.setdefault('cache', other_engine.cache)
         obj = cls(other_engine.psi, other_engine.model, options, **kwargs)
         obj.checkpoint = other_engine.checkpoint  # TODO: do this?
         return obj
 
-    @property
-    def verbose(self):
-        warnings.warn(
-            "verbose is deprecated, we're using logging now! \n"
-            "See https://tenpy.readthedocs.io/en/latest/intro/logging.html", FutureWarning, 2)
-        return self.options.get('verbose', 1.)
-
     def run(self):
         """Actually run the algorithm.
 
         Needs to be implemented in subclasses.
         """
         raise NotImplementedError("Subclasses should implement this.")
```

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/disentangler.py` & `physics-tenpy-1.0.0/tenpy/algorithms/disentangler.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/dmrg.py` & `physics-tenpy-1.0.0/tenpy/algorithms/dmrg.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,21 +50,14 @@
 __all__ = [
     'run',
     'DMRGEngine',
     'SingleSiteDMRGEngine',
     'TwoSiteDMRGEngine',
     'chi_list',
     'full_diag_effH',
-    'Mixer',
-    'DensityMatrixMixer',
-    'SubspaceExpansion',
-    'SingleSiteMixer',
-    'TwoSiteMixer',
-    'EngineCombine',
-    'EngineFracture',
 ]
 
 
 def run(psi, model, options, **kwargs):
     r"""Run the DMRG algorithm to find the ground state of the given model.
 
     Parameters
@@ -109,94 +102,25 @@
         'E': E,
         'shelve': engine.shelve,
         'bond_statistics': engine.update_stats,
         'sweep_statistics': engine.sweep_stats
     }
 
 
-class Mixer(mps_common.Mixer):
-    """Deprecated.
-
-    .. deprecated :: 1.0.0
-        Use :class:`~tenpy.algorithms.mps_common.Mixer` instead.
-        Note the changed function names and signatures
-    """
-    deprecated = True # disable class in find_subclass()
-    update_sites = 2
-
-    def __init__(self, options, sweep_activated):
-        msg = ('The `Mixer`, `SubspaceExpansion` and `DensityMatrixMixer` have been moved '
-               'to tenpy.algorithms.mps_common. Note the changed function names and signatures.')
-        warnings.warn(msg, category=FutureWarning, stacklevel=2)
-        super().__init__(options, sweep_activated)
-
-
-class SubspaceExpansion(Mixer, mps_common.SubspaceExpansion):
-    """Deprecated.
-
-    .. deprecated :: 1.0.0
-        Use :class:`~tenpy.algorithms.mps_common.SubspaceExpansion` instead.
-        Note the changed function names and signatures
-    """
-    update_sites = 1
-
-    def perturb_svd(self, engine, theta, i0, move_right):
-        U, S, VH, err = self.mix_and_decompose_1site(engine, theta, i0, move_right)
-        return U, S, VH, err, S
-
-
-class SingleSiteMixer(SubspaceExpansion):
-    r"""Deprecated name for the :class:`SubspaceExpansion` class.
-
-    .. deprecated :: 0.5.0
-       Instead of `SingleSiteMixer` and `TwoSiteMixer`, directly use :class:`SubspaceExpansion`
-       which is compatible with both single-site and two-site DMRG.
-    """
-    def __init__(self, *args, **kwargs):
-        msg = ("The `SingleSiteMixer` and `TwoSiteMixer` have been replaced by the unified "
-               "`SubspaceExpansion` class, and\n"
-               "all mixers are compatible with both SingleSiteDMRGEngine and TwoSiteDMRGEngine.")
-        warnings.warn(msg, category=FutureWarning, stacklevel=2)
-        super().__init__(*args, **kwargs)
-
-
-class TwoSiteMixer(SingleSiteMixer):
-    # Both DMRG engines have code in mixed_svd to support both single-site and two-site mixers
-    pass
-
-
-class DensityMatrixMixer(Mixer, mps_common.DensityMatrixMixer):
-    """Deprecated.
-
-    .. deprecated :: 1.0.0
-        Use :class:`~tenpy.algorithms.mps_common.DensityMatrixMixer` instead.
-        Note the changed function names and signatures
-    """
-    update_sites = 2
-
-    def perturb_svd(self, engine, theta, i0, update_LP, update_RP):
-        qtotal_LR = [engine.psi.get_B(i0, form=None).qtotal,
-                     engine.psi.get_B(i0 + 1, form=None).qtotal]
-        return self.mixed_svd_2site(engine, theta, i0, update_LP, update_RP, qtotal_LR)
-
-
 class DMRGEngine(IterativeSweeps):
     """DMRG base class with common methods for the TwoSiteDMRG and SingleSiteDMRG.
 
     This engine is implemented as a subclass of :class:`~tenpy.algorithms.mps_common.Sweep`.
     It contains all methods that are generic between
     :class:`SingleSiteDMRGEngine` and :class:`TwoSiteDMRGEngine`.
     Use the latter two classes for actual DMRG runs.
 
     A generic protocol for approaching a physics question using DMRG is given in
     :doc:`/intro/dmrg-protocol`.
 
-    .. deprecated :: 0.5.0
-        Renamed parameter/attribute `DMRG_params` to :attr:`options`.
-
     Options
     -------
     .. cfg:config :: DMRGEngine
         :include: IterativeSweeps
 
     Attributes
     ----------
@@ -294,19 +218,14 @@
         disable_finite = 15
         disable_infinite = 50
         decay_finite = 2.
         decay_infinite = decay_finite ** (disable_finite / disable_infinite)
         mixer_options.setdefault('decay', decay_finite if self.finite else decay_infinite)
         mixer_options.setdefault('disable_after', disable_finite if self.finite else disable_infinite)
 
-    @property
-    def DMRG_params(self):
-        warnings.warn("renamed self.DMRG_params -> self.options", FutureWarning, stacklevel=2)
-        return self.options
-
     def pre_run_initialize(self):
         super().pre_run_initialize()
         E = np.nan
         return E, self.psi
 
     def run_iteration(self):
         """Perform a single iteration, consisting of ``N_sweeps_check`` sweeps.
@@ -1354,52 +1273,14 @@
         super().mixer_activate()
         if not self.mixer.can_decompose_1site:
             msg = (f'Using {self.mixer.__class__.__name__} with single-site DMRG is inefficient. '
                    f'The resulting algorithm has two-site costs!')
             warnings.warn(msg)
 
 
-class EngineCombine(TwoSiteDMRGEngine):
-    r"""Engine which combines legs into pipes as far as possible.
-
-    This engine combines the virtual and physical leg for the left site and right site into pipes.
-    This reduces the overhead of calculating charge combinations in the contractions,
-    but one :meth:`matvec` is formally more expensive, :math:`O(2 d^3 \chi^3 D)`.
-
-    .. deprecated :: 0.5.0
-       Directly use the :class:`TwoSiteDMRGEngine` with the DMRG parameter ``combine=True``.
-    """
-    def __init__(self, psi, model, DMRG_params):
-        msg = ("Old-style engines are deprecated in favor of `Sweep` subclasses.\n"
-               "Use `TwoSiteDMRGEngine` with parameter `combine=True` "
-               "instead of `EngineCombine`.")
-        warnings.warn(msg, category=FutureWarning, stacklevel=2)
-        DMRG_params['combine'] = True  # to reproduces old-style engine
-        super().__init__(psi, model, DMRG_params)
-
-
-class EngineFracture(TwoSiteDMRGEngine):
-    r"""Engine which keeps the legs separate.
-
-    Due to a different contraction order in :meth:`matvec`, this engine might be faster than
-    :class:`EngineCombine`, at least for large physical dimensions and if the MPO is sparse.
-    One :meth:`matvec` is :math:`O(2 \chi^3 d^2 W + 2 \chi^2 d^3 W^2 )`.
-
-    .. deprecated :: 0.5.0
-       Directly use the :class:`TwoSiteDMRGEngine` with the DMRG parameter ``combine=False``.
-    """
-    def __init__(self, psi, model, DMRG_params):
-        msg = ("Old-style engines are deprecated in favor of `Sweep` subclasses.\n"
-               "Use `TwoSiteDMRGEngine` with parameter `combine=False` "
-               "instead of `EngineFracture`.")
-        warnings.warn(msg, category=FutureWarning, stacklevel=2)
-        DMRG_params['combine'] = False  # to reproduces old-style engine
-        super().__init__(psi, model, DMRG_params)
-
-
 def chi_list(chi_max, dchi=20, nsweeps=20):
     """Compute a 'ramping-up' chi_list.
 
     The resulting chi_list allows to increases `chi` by `dchi` every `nsweeps` sweeps up to a given
     maximal `chi_max`.
 
     Parameters
```

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/dmrg_parallel.py` & `physics-tenpy-1.0.0/tenpy/algorithms/dmrg_parallel.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/exact_diag.py` & `physics-tenpy-1.0.0/tenpy/algorithms/exact_diag.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/mpo_evolution.py` & `physics-tenpy-1.0.0/tenpy/algorithms/mpo_evolution.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/mps_common.py` & `physics-tenpy-1.0.0/tenpy/algorithms/mps_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,19 +144,14 @@
         self.ortho_to_envs = []
         self.init_env(model, resume_data=self.resume_data, orthogonal_to=orthogonal_to)
         self.i0 = 0
         self.move_right = True
         self.update_LP_RP = (True, False)
 
     @property
-    def engine_params(self):
-        warnings.warn("renamed self.engine_params -> self.options", FutureWarning, stacklevel=2)
-        return self.options
-
-    @property
     def _all_envs(self):
         return [self.env] + self.ortho_to_envs
 
     @property
     def S_inv_cutoff(self):
         # high cutoff for regular inverse of S, higher cutoff if we need to (pseudo-) invert
         # a matrix (S can be 2D while the mixer is on)
@@ -215,64 +210,39 @@
             First, run DMRG to find the ground state,
             and then run DMRG again while orthogonalizing against the ground state,
             which yields the first excited state (in the same symmetry sector), and so on.
             Note that ``resume_data['orthogonal_to']`` takes precedence over the argument.
 
         Options
         -------
-        .. deprecated :: 0.6.0
-            Options `LP`, `LP_age`, `RP` and `RP_age` are now collected in a dictionary
-            `init_env_data` with different keys `init_LP`, `init_RP`, `age_LP`, `age_RP`
-
-        .. deprecated :: 0.8.0
-            Instead of passing the `init_env_data` as a option, it should be passed
-            as dict entry of `resume_data`.
 
         .. cfg:configoptions :: Sweep
-
-            init_env_data : dict
-                Dictionary as returned by ``self.env.get_initialization_data()`` from
-                :meth:`~tenpy.networks.mpo.MPOEnvironment.get_initialization_data`.
-                Deprecated, use the `resume_data` function/class argument instead.
-            orthogonal_to : list of :class:`~tenpy.networks.mps.MPS`
-                Deprecated in favor of the `orthogonal_to` function argument (forwarded from the
-                class argument) with the same effect.
+                
             start_env : int
                 Number of sweeps to be performed without optimization to update the environment.
 
         Raises
         ------
         ValueError
             If the engine is re-initialized with a new model, which legs are incompatible with
             those of hte old model.
         """
         H = model.H_MPO if model is not None else self.env.H
         # extract `init_env_data` from options or previous env
         if resume_data is None:
             resume_data = {}
-        if 'init_env_data' in self.options:
-            warnings.warn("put init_env_data in resume_data instead of options!", FutureWarning)
-            resume_data.setdefault('init_env_data', self.options['init_env_data'])
         init_env_data = {}
         if self.env is not None and self.psi.bc != 'finite':
             # reuse previous environments.
             # if legs are incompatible, MPOEnvironment.init_first_LP_last_RP will regenerate
             init_env_data = self.env.get_initialization_data()
         init_env_data = resume_data.get('init_env_data', init_env_data)
         if not self.psi.finite and init_env_data and \
                 self.options.get('chi_list', None) is not None:
             warnings.warn("Re-using environment with `chi_list` set! Do you want this?")
-        replaced = [('LP', 'init_LP'), ('LP_age', 'age_LP'), ('RP', 'init_RP'),
-                    ('RP_age', 'age_RP')]
-        if any([key_old in self.options for key_old, _ in replaced]):
-            warnings.warn("Deprecated options LP/RP/LP_age/RP_age: collected in `init_env_data`",
-                          FutureWarning)
-            for key_old, key_new in replaced:
-                if key_old in self.options:
-                    init_env_data[key_new] = self.options[key_old]
 
         # actually initialize the environment
         self._init_mpo_env(H, init_env_data)
         self._init_ortho_to_envs(orthogonal_to, resume_data)
 
         self.reset_stats(resume_data)
 
@@ -287,20 +257,14 @@
         else:
             cache = self.env.cache  # re-initialize and reuse the cache!
             cache.clear()  # remove old entries which might no longer be valid
         self.env = MPOEnvironment(self.psi, H, self.psi, cache=cache, **init_env_data)
 
     def _init_ortho_to_envs(self, orthogonal_to, resume_data):
         # (re)initialize ortho_to_envs
-        if 'orthogonal_to' in self.options:
-            warnings.warn(
-                "Deprecated `orthogonal_to` in dmrg options: instead give "
-                "`orthogonal_to` as keyword to the Algorithm class.", FutureWarning)
-            assert orthogonal_to is None
-            orthogonal_to = self.options['orthogonal_to']
         if 'orthogonal_to' in resume_data:
             orthogonal_to = resume_data['orthogonal_to']  # precedence for resume_data!
 
         if orthogonal_to:
             if not self.finite:
                 raise ValueError("Can't orthogonalize for infinite MPS: overlap not well defined.")
             logger.info("got %d states to orthogonalize against", len(orthogonal_to))
@@ -323,34 +287,26 @@
         ----------
         resume_data : dict
             Given when resuming a simulation, as returned by :meth:`get_resume_data`.
             Here, we read out the `sweeps`.
 
         Options
         -------
-        .. deprecated : 0.9
-            sweep_0 : int
-                Number of sweeps that have already been performed.
-                Pass as ``resume_data['sweeps']`` instead.
 
         .. cfg:configoptions :: Sweep
 
             chi_list : None | dict(int -> int)
                 By default (``None``) this feature is disabled.
                 A dict allows to gradually increase the `chi_max`.
                 An entry `at_sweep: chi` states that starting from sweep `at_sweep`,
                 the value `chi` is to be used for ``trunc_params['chi_max']``.
                 For example ``chi_list={0: 50, 20: 100}`` uses ``chi_max=50`` for the first
                 20 sweeps and ``chi_max=100`` afterwards.
         """
         self.sweeps = 0
-        if 'sweep_0' in self.options:
-            warnings.warn("Deprecated sweep_0 option: set as resume_data['sweep'] instead.",
-                          FutureWarning)
-            self.sweeps = self.options['sweep_0']
         if resume_data is not None and 'sweeps' in resume_data:
             self.sweeps = resume_data['sweeps']
         self.shelve = False
         self.chi_list = self.options.get('chi_list', None)
         if self.chi_list is not None:
             done = [k for k in self.chi_list.keys() if k < self.sweeps]
             if len(done) > 0:
@@ -690,20 +646,15 @@
         """
         Mixer_class = self.options.get('mixer', self.use_mixer_by_default)
         if not Mixer_class:
             return  # no mixer -> nothing to do
         if Mixer_class is True:
             Mixer_class = self.DefaultMixer
         if isinstance(Mixer_class, str):
-            if Mixer_class == "Mixer":
-                msg = 'Use `True` instead of "Mixer" for DMRG parameter "mixer"'
-                warnings.warn(msg, FutureWarning)
-                Mixer_class = self.DefaultMixer
-            else:
-                Mixer_class = find_subclass(Mixer, Mixer_class)
+            Mixer_class = find_subclass(Mixer, Mixer_class)
         mixer_params = self.options.subconfig('mixer_params')
         self.mixer = Mixer_class(mixer_params, self.sweeps)
         logger.info(f'activate {Mixer_class.__name__} with initial amplitude {self.mixer.amplitude}')
 
     def mixer_deactivate(self):
         """Deactivate the mixer.
 
@@ -2166,17 +2117,14 @@
     """Variational compression of an MPS (in place).
 
     To compress an MPS `psi`, use ``VariationalCompression(psi, options).run()``.
 
     The algorithm is the same as described in :class:`VariationalApplyMPO`,
     except that we don't have an MPO in the networks - one can think of the MPO being trivial.
 
-    .. deprecated :: 0.9.1
-        Renamed the option `N_sweeps` to `max_sweeps`.
-
     Parameters
     ----------
     psi : :class:`~tenpy.networks.mps.MPS`
         The state to be compressed.
     options : dict
         See :cfg:config:`VariationalCompression`.
     resume_data : None | dict
@@ -2210,17 +2158,14 @@
         super().__init__(psi, None, options, resume_data=resume_data)
         self.renormalize = []
         self._theta_diff = []
         self.options.setdefault('max_sweeps', 2)
 
     def pre_run_initialize(self):
         super().pre_run_initialize()
-        self.options.deprecated_alias("N_sweeps", "max_sweeps",
-                                      "Also check out the other new convergence parameters "
-                                      "min_N_sweeps and tol_theta_diff!")
         max_sweeps = self._max_sweeps = self.options.get("max_sweeps", 2)
         min_sweeps = self._min_sweeps = self.options.get("min_sweeps", 1)
         tol_diff = self._tol_theta_diff = self.options.get("tol_theta_diff", 1.e-8)
         if min_sweeps == max_sweeps and tol_diff is not None:
             warnings.warn("VariationalCompression with min_sweeps=max_sweeps: "
                           "we recommend to set tol_theta_diff=None to avoid overhead")
         return TruncationError()
```

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/network_contractor.py` & `physics-tenpy-1.0.0/tenpy/algorithms/network_contractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 """Network Contractor.
 
 A tool to contract a network of multiple tensors.
 
 This is an implementation of 'NCON: A tensor network contractor for MATLAB'
 by Robert N. C. Pfeifer, Glen Evenbly, Sukhwinder Singh, Guifre Vidal, see :arxiv:`1402.0939`
 
-.. autodata :: outer_product
-
 .. todo ::
     - implement or wrap netcon.m, a function to find optimal contraction sequences
         (:arxiv:`1304.6112`)
-    - implement or deprecate the outer_product in sequence behavior
 """
 # Copyright (C) TeNPy Developers, GNU GPLv3
 
 import numpy as np
 from ..linalg import np_conserved as npc
 
-__all__ = ['outer_product', 'contract', 'ncon']
-
-outer_product = -66666666  #: a constant that represents an outer product in the sequence of ncon
+__all__ = ['contract', 'ncon']
 
 
 def ncon(tensor_list, leg_links, sequence=None):
     """Implementation of ``ncon.m`` for TeNPy Arrays.
 
     This function is a python implementation of ``ncon.m`` (:arxiv:`1304.6112`) for tenpy
     :class:`~tenpy.linalg.np_conserved.Array`.
@@ -38,27 +33,23 @@
         `tensor_list`.
         Each entry is a sequence (e.g. a list) that has an integer value for each leg of the corresponding tensor.
         Positive values ``1,2,...`` are labels of contracted legs and should appear
         exactly twice in `leg_links`.
         Negative values ``-1,-2,-3,...`` are labels of uncontracted legs and indicate the final ordering
         (``-1`` is the first axis).
     sequence : list of int, optional
-        The order in which the contractions (indicated by positive values in `leg_links` are to be performed.
-        Ascending order is used by default
-        An entry of network_contractor.outer_product indicates performing an outer product.
-        This corresponds to the zero-in-sequence convention of :arxiv:`1304.6112`
+        The order in which the contractions (indicated by positive values in `leg_links`) are to be performed.
+        Ascending order is used by default.
 
     Returns
     -------
     result : :class:`Array` | complex
         The number or tensor resulting from the contraction.
     """
     tensor_list, leg_links, sequence = _ncon_input_checks(tensor_list, leg_links, sequence)
-    if outer_product in sequence:
-        raise NotImplementedError('Current implementation does not support outer product in sequence')
     tensor_list, leg_links, sequence = _ncon_do_traces(tensor_list, leg_links, sequence)
     tensor_list, leg_links, sequence = _ncon_do_binary_contractions(tensor_list, leg_links, sequence)
     tensor_list, leg_links = _ncon_do_outer_products(tensor_list, leg_links)
     result, = tensor_list
     if len(leg_links[0]) > 0:
         result.itranspose(np.argsort(-leg_links[0]))
     return result
@@ -86,16 +77,14 @@
         and is labelled ``l`` in the result.
     tensor_names : list of str
         A list of names for each tensor, to be used in `leg_contractions` and `open_legs`.
         The default value is list(range(len(tensor_list))), so that the tensor "names" are
         ``0, 1, 2, ...``.
     sequence : list of int
         The order in which the leg_contractions are to be performed.
-        An entry of network_contractor.outer_product indicates performing an outer product.
-        This corresponds to the zero-in-sequence convention of :arxiv:`1304.6112`
 
     Returns
     -------
     result : :class:`Array` | complex
         The number or tensor resulting from the contraction.
     """
 
@@ -121,17 +110,14 @@
     for tensor in tensor_list:
         leg_links.append([None] * len(tensor.legs))
 
     # fill in the contractions
     contraction_counter = 1
     new_sequence = []
     for n in sequence:
-        if n == outer_product:
-            new_sequence.append(outer_product)
-            continue
 
         con = leg_contractions[n - 1]
         leg_idx1 = tensor_list[con[0]].get_leg_index(con[1])
         leg_idx2 = tensor_list[con[2]].get_leg_index(con[3])
 
         if leg_links[con[0]][leg_idx1] is not None:
             raise RuntimeError('Multiple contradictory contractions for the leg ' + str(con[1]) +
@@ -184,16 +170,14 @@
     if sequence is None:
         sequence = np.arange(1, num_contractions + 1)
     else:
         sequence = np.asarray(sequence)
         if len(sequence) != num_contractions or set(sequence) != set(range(1, num_contractions + 1)):
             msg = f'Invalid sequence. Expected a permutation of [1, ..., {num_contractions}]. Got {sequence}.'
             raise ValueError(msg)
-        if outer_product in sequence:
-            raise ValueError('Outer product in sequence is deprecated.')
         
     return tensor_list, leg_links, sequence
 
 
 def _ncon_do_traces(tensor_list, leg_links, sequence):
     for n in range(len(leg_links)):
         if len(leg_links[n]) > len(np.unique(leg_links[n])):
```

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/plane_wave_excitation.py` & `physics-tenpy-1.0.0/tenpy/algorithms/plane_wave_excitation.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/purification.py` & `physics-tenpy-1.0.0/tenpy/algorithms/purification.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,17 +78,14 @@
         new_psi.set_SR(i0, S)
         return {'U': U, 'VH': VH, 'err': err}
 
 
 class PurificationTEBD(tebd.TEBDEngine):
     r"""Time evolving block decimation (TEBD) for purification MPS.
 
-    .. deprecated :: 0.6.0
-        Renamed parameter/attribute `TEBD_params` to :attr:`options`.
-
     Parameters are the same as for :class:`~tenpy.algorithms.algorithm.Algorithm`.
 
     Options
     -------
     .. cfg:config :: PurificationTEBD
         :include: TEBDEngine
```

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/tebd.py` & `physics-tenpy-1.0.0/tenpy/algorithms/tebd.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,25 +47,22 @@
 
 from .algorithm import TimeEvolutionAlgorithm, TimeDependentHAlgorithm
 from ..linalg import np_conserved as npc
 from .truncation import svd_theta, TruncationError, truncate
 from ..linalg import random_matrix
 from ..tools.misc import consistency_check
 
-__all__ = ['TEBDEngine', 'Engine', 'QRBasedTEBDEngine', 'RandomUnitaryEvolution', 'TimeDependentTEBD']
+__all__ = ['TEBDEngine', 'QRBasedTEBDEngine', 'RandomUnitaryEvolution', 'TimeDependentTEBD']
 
 
 class TEBDEngine(TimeEvolutionAlgorithm):
     """Time Evolving Block Decimation (TEBD) algorithm.
 
     Parameters are the same as for :class:`~tenpy.algorithms.algorithm.Algorithm`.
 
-    .. deprecated :: 0.6.0
-        Renamed parameter/attribute `TEBD_params` to :attr:`options`.
-
     Options
     -------
     .. cfg:config :: TEBDEngine
         :include: TimeEvolutionAlgorithm
 
         start_trunc_err : :class:`~tenpy.algorithms.truncation.TruncationError`
             Initial truncation error for :attr:`trunc_err`.
@@ -107,19 +104,14 @@
         TimeEvolutionAlgorithm.__init__(self, psi, model, options, **kwargs)
         self._trunc_err_bonds = [TruncationError() for i in range(psi.L + 1)]
         self._U = None
         self._U_param = {}
         self._update_index = None
 
     @property
-    def TEBD_params(self):
-        warnings.warn("renamed self.TEBD_params -> self.options", FutureWarning, stacklevel=2)
-        return self.options
-
-    @property
     def trunc_err_bonds(self):
         """truncation error introduced on each non-trivial bond."""
         return self._trunc_err_bonds[self.psi.nontrivial_bonds]
 
     # run() as defined in TimeEvolutionAlgorithm
 
     def run_GS(self):
@@ -583,26 +575,14 @@
         else:
             raise ValueError("Expect either 'real' or 'imag'inary time, got " + repr(type_evo))
         U = npc.expm(H2)
         assert (tuple(U.get_leg_labels()) == ('(p0.p1)', '(p0*.p1*)'))
         return U.split_legs()
 
 
-class Engine(TEBDEngine):
-    """Deprecated old name of :class:`TEBDEngine`.
-
-    .. deprecated : v0.8.0
-        Renamed the `Engine` to `TEBDEngine` to have unique algorithm class names.
-    """
-    def __init__(self, psi, model, options):
-        msg = "Renamed `Engine` class to `TEBDEngine`."
-        warnings.warn(msg, category=FutureWarning, stacklevel=2)
-        TEBDEngine.__init__(self, psi, model, options)
-
-
 class QRBasedTEBDEngine(TEBDEngine):
     r"""Version of TEBD that relies on QR decompositions rather than SVD.
 
     As introduced in :arxiv:`2212.09782`.
 
     .. todo ::
         To use `use_eig_based_svd == True`, which makes sense on GPU only, we need to implement
```

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/truncation.py` & `physics-tenpy-1.0.0/tenpy/algorithms/truncation.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,18 +139,14 @@
 
 
 def truncate(S, options):
     """Given a Schmidt spectrum `S`, determine which values to keep.
 
     Options
     -------
-    .. deprecated :: 0.5.1
-        Renamed `symmetry_tol` to `degeneracy_tol`,
-        and don't use log in the condition any more.
-
     .. cfg:config:: truncation
 
         chi_max : int
             Keep at most `chi_max` Schmidt values.
         chi_min : int
             Keep at least `chi_min` Schmidt values.
         degeneracy_tol: float
@@ -190,18 +186,14 @@
     """
     options = asConfig(options, "truncation")
     # by default, only truncate values which are much closer to zero than machine precision.
     # This is only to avoid problems with taking the inverse of `S`.
     chi_max = options.get('chi_max', 100)
     chi_min = options.get('chi_min', None)
     deg_tol = options.get('degeneracy_tol', None)
-    options.deprecated_alias('symmetry_tol', 'degeneracy_tol',
-                             "We don't use `log` in the condition anymore!")
-    if 'symmetry_tol' in options:  # deprecated!
-        deg_tol = np.log(options['symmetry_tol'])
     svd_min = options.get('svd_min', 1.e-14)
     trunc_cut = options.get('trunc_cut', 1.e-14)
 
     if trunc_cut is not None and trunc_cut >= 1.:
         raise ValueError("trunc_cut >=1.")
     if not np.any(S > 1.e-10):
         warnings.warn("no Schmidt value above 1.e-10", stacklevel=2)
```

### Comparing `physics-tenpy-0.99.0/tenpy/algorithms/vumps.py` & `physics-tenpy-1.0.0/tenpy/algorithms/vumps.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/linalg/__init__.py` & `physics-tenpy-1.0.0/tenpy/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/linalg/_npc_helper.cpp` & `physics-tenpy-1.0.0/tenpy/linalg/_npc_helper.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 /* Generated by Cython 3.0.9 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/core/include",
-            "/Users/jakobunfried/anaconda3/envs/tenpy099distribute/include"
+            "/tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/core/include"
         ],
         "language": "c++",
-        "library_dirs": [
-            "/Users/jakobunfried/anaconda3/envs/tenpy099distribute/lib"
-        ],
         "name": "tenpy.linalg._npc_helper",
         "sources": [
             "tenpy/linalg/_npc_helper.pyx"
         ]
     },
     "module_name": "tenpy.linalg._npc_helper"
 }
@@ -1660,177 +1656,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1909,42 +1905,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_5tenpy_6linalg_11_npc_helper_CblasGemmBatch;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -20185,261 +20181,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -20448,29 +20444,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -20481,15 +20477,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -20498,29 +20494,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -20531,15 +20527,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -20548,29 +20544,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -20581,15 +20577,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -20598,29 +20594,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -20631,15 +20627,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -20648,29 +20644,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -20681,217 +20677,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -20907,15 +20903,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -20923,68 +20919,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -20992,15 +20988,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -21015,15 +21011,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21039,15 +21035,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -21055,68 +21051,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -21124,15 +21120,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21147,15 +21143,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21171,15 +21167,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -21187,68 +21183,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -21256,15 +21252,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21279,170 +21275,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -46923,26 +46919,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../var/folders/v3/1dx96kyn4ms6yxbdt1wx831c0000gn/T/build-env-5u7bg62i/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-txkn3hd_/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `physics-tenpy-0.99.0/tenpy/linalg/_npc_helper.pyx` & `physics-tenpy-1.0.0/tenpy/linalg/_npc_helper.pyx`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/linalg/charges.py` & `physics-tenpy-1.0.0/tenpy/linalg/charges.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/linalg/krylov_based.py` & `physics-tenpy-1.0.0/tenpy/linalg/krylov_based.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Lanczos algorithm for np_conserved arrays."""
 # Copyright (C) TeNPy Developers, GNU GPLv3
 
-import warnings
 import numpy as np
 from .sparse import FlatHermitianOperator, OrthogonalNpcLinearOperator, ShiftNpcLinearOperator
 import logging
 logger = logging.getLogger(__name__)
 
 from . import np_conserved as npc
 from ..tools.params import asConfig
@@ -105,15 +104,15 @@
     Given the gap, the Ritz residual gives a bound on the error in the wavefunction,
     ``err < (RitzRes/gap)**2``. The gap is estimated from the full Lanczos spectrum.
     """
 
     _dtype_h_krylov = np.complex128
     _dtype_E = np.complex128
 
-    def __init__(self, H, psi0, options, orthogonal_to=[]):
+    def __init__(self, H, psi0, options):
         self.H = H
         self.psi0 = psi0.copy()
         self._psi0_norm = None
         self.options = options = asConfig(options, self.__class__.__name__)
         self.N_min = options.get('N_min', 2)
         self.N_max = options.get('N_max', 20)
         self.N_cache = self.N_max
@@ -430,24 +429,15 @@
         return P_err < self.P_tol and Delta_E0 < self.E_tol
 
 
 class LanczosGroundState(KrylovBased):
     """Lanczos algorithm to find the ground state.
 
     **Assumes** that `H` is hermitian.
-
-    .. deprecated :: 0.6.0
-        Renamed attribute `params` to :attr:`options`.
-
-    .. deprecated :: 0.6.0
-        Going to remove the `orthogonal_to` argument.
-        Instead, replace H with ``OrthogonalNpcLinearOperator(H, orthogonal_to)``
-        using the :class:`~tenpy.linalg.sparse.OrthogonalNpcLinearOperator`.
-
-
+    
     Options
     -------
     .. cfg:config :: LanczosGroundState
         :include: KrylovBased
 
         E_tol : float
             Stop if energy difference per step < `E_tol`
@@ -465,25 +455,20 @@
 
 
     """
 
     _dtype_h_krylov = np.float64
     _dtype_E = np.float64
 
-    def __init__(self, H, psi0, options, orthogonal_to=[]):
+    def __init__(self, H, psi0, options):
         super().__init__(H, psi0, options)
         self.E_tol = self.options.get('E_tol', np.inf)
         self.N_cache = self.options.get('N_cache', self.N_max)
         if self.N_cache < 2:
             raise ValueError("Need to cache at least two vectors.")
-        if len(orthogonal_to) > 0:
-            msg = ("Lanczos argument `orthogonal_to` is deprecated and will be removed.\n"
-                   "Instead, replace `H` with  `OrthogonalNpcLinearOperator(H, orthogonal_to)`.")
-            warnings.warn(msg, category=FutureWarning, stacklevel=2)
-            self.H = OrthogonalNpcLinearOperator(self.H, orthogonal_to)
 
     def run(self):
         """Find the ground state of H.
 
         Returns
         -------
         E0 : float
@@ -683,80 +668,63 @@
             self._result_norm = np.linalg.norm(exp_dH_e0)
             self._result_krylov = exp_dH_e0 / self._result_norm
 
     def _converged(self, k):
         return np.abs(self._result_krylov[k]) < self.P_tol
 
 
-def lanczos_arpack(H, psi, options={}, orthogonal_to=[]):
+def lanczos_arpack(H, psi, options={}):
     """Use :func:`scipy.sparse.linalg.eigsh` to find the ground state of `H`.
 
     This function has the same call/return structure as :func:`lanczos`, but uses
     the ARPACK package through the functions :func:`~tenpy.tools.math.speigsh` instead of the
     custom lanczos implementation in :class:`LanczosGroundState`.
     This function is mostly intended for debugging, since it requires to convert the vector
     from np_conserved :class:`~tenpy.linalg.np_conserved.Array` into a flat numpy array
     and back during *each* `matvec`-operation!
 
-    .. deprecated :: 0.6.0
-        Going to remove the `orthogonal_to` argument.
-        Instead, replace H with `OrthogonalNpcLinearOperator(H, orthogonal_to)`
-        using the :class:`~tenpy.linalg.sparse.OrthogonalNpcLinearOperator`.
-
     Parameters
     ----------
-    H, psi, options, orthogonal_to :
+    H, psi, options :
         See :class:`LanczosGroundState`.
         `H` and `psi` should have/use labels.
 
     Returns
     -------
     E0 : float
         Ground state energy.
     psi0 : :class:`~tenpy.linalg.np_conserved.Array`
         Ground state vector.
     """
-    if len(orthogonal_to) > 0:
-        msg = ("Lanczos argument `orthogonal_to` is deprecated and will be removed.\n"
-               "Instead, replace `H` with  `OrthogonalNpcLinearOperator(H, orthogonal_to)`.")
-        warnings.warn(msg, category=FutureWarning, stacklevel=2)
-        H = OrthogonalNpcLinearOperator(H, orthogonal_to)
     options = asConfig(options, "Lanczos")
     H_flat, psi_flat = FlatHermitianOperator.from_guess_with_pipe(H.matvec, psi, dtype=H.dtype)
     tol = options.get('P_tol', 1.e-14)
     N_min = options.get('N_min', None)
     Es, Vs = H_flat.eigenvectors(num_ev=1, which='SA', v0=psi_flat, tol=tol, ncv=N_min)
     psi0 = Vs[0].split_legs(0).itranspose(psi.get_leg_labels())
     return Es[0], psi0
 
 
-def gram_schmidt(vecs, rcond=1.e-14, verbose=None):
+def gram_schmidt(vecs, rcond=1.e-14):
     """In place Gram-Schmidt Orthogonalization and normalization for npc Arrays.
 
-    .. deprecated :: 0.9.1
-        Previously, this function return `vecs, ov` with `ov` being the overlaps
-        ``<vecs[i]|vecs[j]>``. The return value `ov` has been dropped now,
-        since it wasn't used anyways.
-
     Parameters
     ----------
     vecs : list of :class:`~tenpy.linalg.np_conserved.Array`
         The vectors which should be orthogonalized.
         All with the same *order* of the legs. Entries are modified *in place*.
         if a norm < rcond, the entry is set to `None`.
     rcond : float
         Vectors of ``norm < rcond`` (after projecting out previous vectors) are discarded.
 
     Returns
     -------
     vecs : list of Array
         The ortho-normalized vectors (without any ``None``).
     """
-    if verbose is not None:
-        warnings.warn("Dropped verbose argument", category=FutureWarning, stacklevel=2)
     res = []
     for vec in vecs:
         for other in res:
             ov = npc.inner(other, vec, 'range', do_conj=True)
             iadd_prefactor_other(vec, -ov, other)
         n = npc.norm(vec)
         if n > rcond:
```

### Comparing `physics-tenpy-0.99.0/tenpy/linalg/np_conserved.py` & `physics-tenpy-1.0.0/tenpy/linalg/np_conserved.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,37 +636,14 @@
         return len(self._data)
 
     @property
     def ndim(self):
         """Alias for :attr:`rank` or ``len(self.shape)``."""
         return self.rank
 
-    @property
-    def labels(self):
-        warnings.warn("Deprecated access of Array.labels as dictionary.",
-                      category=FutureWarning,
-                      stacklevel=2)
-        dict_lab = {}
-        for i, l in enumerate(self._labels):
-            if l is not None:
-                dict_lab[l] = i
-        return dict_lab
-
-    @labels.setter
-    def labels(self, dict_lab):
-        warnings.warn("Deprecated setting of Array.labels with dictionary.",
-                      category=FutureWarning,
-                      stacklevel=2)
-        list_lab = [None] * self.rank
-        for k, v in dict_lab.items():
-            if list_lab[v] is not None:
-                raise ValueError("Two labels point to the same index " + repr(dict_lab))
-            list_lab[v] = str(k)
-        self._labels = list_lab
-
     # labels ==================================================================
 
     def get_leg_index(self, label):
         """translate a leg-index or leg-label to a leg-index.
 
         Parameters
         ----------
@@ -1437,14 +1414,18 @@
         axes = self.get_leg_indices(axes)
         legs = [self.legs[a] for a in axes]
         return LegPipe(legs, **kwargs)
 
     def combine_legs(self, combine_legs, new_axes=None, pipes=None, qconj=None):
         """Reshape: combine multiple legs into multiple pipes. If necessary, transpose before.
 
+        .. versionchanged :: 1.0
+            Make `qconj` default to the `qconj` of the first leg to be combine rather than just +1.
+
+
         Parameters
         ----------
         combine_legs : (iterable of) iterable of {str|int}
             Bundles of leg indices or labels, which should be combined into a new output pipes.
             If multiple pipes should be created, use a list fore each new pipe.
         new_axes : None | (iterable of) int
             The leg-indices, at which the combined legs should appear in the resulting array.
@@ -1452,15 +1433,17 @@
             (taking into account that some axes are 'removed' by combining).
             Thus no transposition is performed if `combine_legs` contains only contiguous ranges.
         pipes : None | (iterable of) {:class:`LegPipes` | None}
             Optional: provide one or multiple of the resulting LegPipes to avoid overhead of
             computing new leg pipes for the same legs multiple times.
             The LegPipes are conjugated, if that is necessary for compatibility with the legs.
         qconj : (iterable of) {+1, -1}
-            Specify whether new created pipes point inward or outward. Defaults to +1.
+            Specify whether new created pipes point inward or outward.
+            Defaults to the same value as the first of the legs to be combined.
+            E.g. for a single combine, the default `qconj` is `self.get_leg(combine_legs[0]).qconj`.
             Ignored for given `pipes`, which are not newly calculated.
 
         Returns
         -------
         reshaped : :class:`Array`
             A copy of self, with some legs combined into pipes as specified by the arguments.
 
@@ -2669,20 +2652,15 @@
 
         pipes = list(pipes)
         # make pipes as necessary
         for i, pipe in enumerate(pipes):
             if pipe is None:
                 qconj_i = qconj[i]
                 if qconj_i is None:
-                    qconj_i = +1  # will change in future to
-                    qconj_i_new = self.get_leg(combine_legs[i][0]).qconj
-                    if qconj_i != qconj_i_new:
-                        warnings.warn(
-                            "combine_legs default value for `qconj` will change "
-                            "from +1 to `qconj` of the first leg, here `-1`", FutureWarning, 3)
+                    qconj_i = self.get_leg(combine_legs[i][0]).qconj
                 pipes[i] = self.make_pipe(axes=combine_legs[i], qconj=qconj_i)
             else:
                 # test for compatibility
                 legs = [self.get_leg(a) for a in combine_legs[i]]
                 if pipe.nlegs != len(legs):
                     raise ValueError("pipe has wrong number of legs")
                 if legs[0].qconj != pipe.legs[0].qconj:
@@ -2804,26 +2782,19 @@
         if self_labels == other_labels:
             return self  # fits
         if None in self_labels or None in other_labels:
             if set(self_labels) == set(other_labels) != set([None]):
                 warnings.warn("Not all legs labeled, so no transpose for Array addition. "
                               "Did you intend to transpose?")
             return self  # not all legs labeled
-        if set(self_labels) != set(other_labels):
-            return self  # different labels
-        # now: same labels, different order.
-        # TODO to keep backwards compatibility, just warn for now
-        warnings.warn(
-            "Arrays with same labels in different order. Transpose intended?"
-            " We will transpose in the future!",
-            category=FutureWarning,
-            stacklevel=2)
+        if set(self_labels) == set(other_labels):
+            # same labels, different order.
+            return self.transpose(other_labels)
+        # else: different labels
         return self
-        # TODO: do this for the next release
-        return self.transpose(other_labels)
 
 
 # ##################################
 # global functions
 # ##################################
 
 
@@ -3398,28 +3369,31 @@
     res._qdata = qdata_res
     res._qdata_sorted = a._qdata_sorted and b._qdata_sorted  # since grid is lex sorted
     # labels
     res._labels = _drop_duplicate_labels(a._labels, b._labels)
     return res
 
 
-def inner(a, b, axes=None, do_conj=False):
+def inner(a, b, axes='labels', do_conj=False):
     """Contract all legs in `a` and `b`, return scalar.
 
+    .. versionchanged :: 1.0
+        Change default behaviour of `axes` from ``'range'`` to ``'labels'``.
+
     Parameters
     ----------
     a, b : class:`Array`
         The arrays for which to calculate the product.
         Must have same rank, and compatible LegCharges.
     axes : ``(axes_a, axes_b)`` | ``'range'``, ``'labels'``
         `axes_a` and `axes_b` specify the legs of `a` and `b`, respectively,
         which should be contracted. Legs can be specified with leg labels or indices.
         We contract leg ``axes_a[i]`` of `a` with leg ``axes_b[i]`` of `b`.
-        The default ``axes='range'`` is equivalent to ``(range(rank), range(rank))``.
-        ``axes='labels'`` is equivalent to either ``(a.get_leg_labels(), a.get_leg_labels())``
+        ``axes='range'`` is equivalent to ``(range(rank), range(rank))``.
+        The default ``axes='labels'`` is equivalent to either ``(a.get_leg_labels(), a.get_leg_labels())``
         for ``do_conj=True``,
         or to ``(a.get_leg_labels(), conj_labels(a.get_leg_labels()))`` for ``do_conj=False``.
         In other words, ``axes='labels'`` requires `a` and `b` to have the same/conjugated labels
         up to a possible transposition, which is then reverted.
     do_conj : bool
         If ``False`` (Default), ignore it.
         If ``True``, conjugate `a` before, i.e., return ``inner(a.conj(), b, axes)``.
@@ -3429,18 +3403,15 @@
     inner_product : dtype
         A scalar (of common dtype of `a` and `b`) giving the full contraction of `a` and `b`.
     """
     if isinstance(a, list) and isinstance(b, list):
         return np.sum([inner(w, v, axes=axes, do_conj=do_conj) for w, v in zip(a, b)])
     if a.rank != b.rank:
         raise ValueError("different rank!")
-    if axes is None or axes == 'range':
-        if axes is None:
-            msg = "inner(): `axes` currently defaults to 'range', will change to 'labels'"
-            warnings.warn(msg, FutureWarning, stacklevel=2)
+    if axes == 'range':
         transp = False
     else:
         if axes == 'labels':
             a_labels = a.get_leg_labels()
             if do_conj:
                 axes = (a_labels, a_labels)
             else:
@@ -3656,15 +3627,15 @@
     if a.rank != 2:
         raise ValueError("Polar is only defined for a 2D matrix. Use LegPipes!")
     if cutoff < 0.:
         raise ValueError("invalid cutoff")
     # follow exactly the procedure lined out.
     # however, use inplace methods and don't construct the diagonal matrix explicitly.
     W, s, VH = svd(a, cutoff=cutoff, inner_labels=inner_labels) # w s vh
-    
+
     u = tensordot(W, VH, axes=([1, 0]))
     if not left:
         labels = VH.conj().get_leg_labels()[1], VH.get_leg_labels()[1]
         # a = up
         p = tensordot(VH.conj().itranspose().iscale_axis(s), VH, axes=([1, 0])).iset_leg_labels(labels)
         #p = (vh.T.conj() * s).dot(vh)
     else:
```

### Comparing `physics-tenpy-0.99.0/tenpy/linalg/random_matrix.py` & `physics-tenpy-1.0.0/tenpy/linalg/random_matrix.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/linalg/sparse.py` & `physics-tenpy-1.0.0/tenpy/linalg/sparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -549,38 +549,14 @@
             leg = self.leg
             for qinds, data in zip(npc_vec._qdata, npc_vec._data):
                 qi = qinds[0]
                 assert qi == qinds[1]
                 res[leg.get_slice(qi)] = data.reshape((-1, ))
             return res
 
-    def flat_to_npc_all_sectors(self, vec):
-        """Convert flat vector of *all* charge sectors into npc Array with extra "charge" leg.
-
-        .. deprecated :: 0.7.3
-            This is merged into :meth:`flat_to_npc` with ``self.charge_sector = None``.
-
-        Parameters
-        ----------
-        vec : 1D ndarray
-            Numpy vector to be converted.
-
-        Returns
-        -------
-        npc_vec : :class:`~tenpy.linalg.np_conserved.Array`
-            Same as `vec`, but converted into a npc array.
-        """
-        assert self._charge_sector is None
-        warnings.warn(
-            "Deprecated access of FlatLinearOperator.flat_to_npc_all_sectors.\n"
-            "directly use flat_to_npc instead!",
-            category=FutureWarning,
-            stacklevel=2)
-        return self.flat_to_npc(vec)
-
     def flat_to_npc_None_sector(self, vec, cutoff=1.e-10):
         """Convert flat vector of undetermined charge sectors into npc Array.
 
         The charge sector to be used is chosen as the block with the maximal norm,
         not by `self.charge_sector` (which might be `None`).
 
         Parameters
@@ -592,38 +568,14 @@
         -------
         npc_vec : :class:`~tenpy.linalg.np_conserved.Array`
             Same as `vec`, but converted into a npc array.
         """
         assert self._charge_sector is None
         return npc.Array.from_ndarray(vec, [self.leg], cutoff=cutoff, labels=[self.vec_label])
 
-    def npc_to_flat_all_sectors(self, npc_vec):
-        """Convert npc Array with qtotal = self.charge_sector into ndarray.
-
-        .. deprecated :: 0.7.3
-            This is merged into :meth:`npc_to_flat` with ``self.charge_sector = None``.
-
-        Parameters
-        ----------
-        npc_vec : :class:`~tenpy.linalg.np_conserved.Array`
-            Npc Array to be converted. Should only have entries in `self.charge_sector`.
-
-        Returns
-        -------
-        vec : 1D ndarray
-            Same as `npc_vec`, but converted into a flat Numpy array.
-        """
-        assert self._charge_sector is None
-        warnings.warn(
-            "Deprecated access of FlatLinearOperator.npc_to_flat_all_sectors.\n"
-            "directly use npc_to_flat instead!",
-            category=FutureWarning,
-            stacklevel=2)
-        return self.npc_to_flat(npc_vec)
-
     def _npc_matvec_wrapper(self, vec):
         """Wrapper around ``self._npc_matvec_multileg`` acting on a LegPipe.
 
         Used when the class was generated with :meth:`from_guess_with_pipe`.
 
         ``self._npc_matvec_multileg`` is a function which can act on a multi-dimensional npc Array
         and returns it with the same legs (with labels ``self._labels_split``).
```

### Comparing `physics-tenpy-0.99.0/tenpy/models/__init__.py` & `physics-tenpy-1.0.0/tenpy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/models/aklt.py` & `physics-tenpy-1.0.0/tenpy/models/aklt.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def __init__(self, model_params):
         model_params = asConfig(model_params, "AKLTModel")
         L = model_params.get('L', 2)
         conserve = model_params.get('conserve', 'Sz')
         if conserve == 'best':
             conserve = 'Sz'
             self.logger.info("%s: set conserve to %s", self.name, conserve)
-        sort_charge = model_params.get('sort_charge', None)
+        sort_charge = model_params.get('sort_charge', True)
         site = SpinSite(S=1., conserve=conserve, sort_charge=sort_charge)
 
         # lattice
         bc_MPS = model_params.get('bc_MPS', 'finite')
         bc = 'open' if bc_MPS == 'finite' else 'periodic'
         lat = Chain(L, site, bc=bc, bc_MPS=bc_MPS)
```

### Comparing `physics-tenpy-0.99.0/tenpy/models/clock.py` & `physics-tenpy-1.0.0/tenpy/models/clock.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,17 +37,16 @@
     Options
     -------
     .. cfg:config :: ClockModel
         :include: CouplingMPOModel
 
         conserve : None | 'Z'
             What should be conserved. See :class:`~tenpy.networks.Site.ClockSite`.
-        sort_charge : bool | None
-            Whether to sort by charges of physical legs.
-            See change comment in :class:`~tenpy.networks.site.Site`.
+        sort_charge : bool
+            Whether to sort by charges of physical legs. `True` by default.
         q : int
             The number of states per site.
         J, g : float | array
             Couplings as defined for the Hamiltonian above.
 
     """
 
@@ -55,15 +54,15 @@
         conserve = model_params.get('conserve', 'Z')
         if conserve == 'best':
             conserve = 'Z'
             self.logger.info("%s: set conserve to %s", self.name, conserve)
         q = model_params.get('q', None)
         if q is None:
             raise ValueError('Need to specify q.')
-        sort_charge = model_params.get('sort_charge', None)
+        sort_charge = model_params.get('sort_charge', True)
         return ClockSite(q=q, conserve=conserve, sort_charge=sort_charge)
 
     def init_terms(self, model_params):
         J = np.asarray(model_params.get('J', 1.))
         g = np.asarray(model_params.get('g', 1.))
         for u in range(len(self.lat.unit_cell)):
             self.add_onsite(-g, u, 'Z', plus_hc=True)
```

### Comparing `physics-tenpy-0.99.0/tenpy/models/fermions_spinless.py` & `physics-tenpy-1.0.0/tenpy/models/fermions_spinless.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/models/haldane.py` & `physics-tenpy-1.0.0/tenpy/models/haldane.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/models/hofstadter.py` & `physics-tenpy-1.0.0/tenpy/models/hofstadter.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/models/hubbard.py` & `physics-tenpy-1.0.0/tenpy/models/hubbard.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/models/lattice.py` & `physics-tenpy-1.0.0/tenpy/models/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 """
 # Copyright (C) TeNPy Developers, GNU GPLv3
 
 import numpy as np
 from scipy.spatial import ConvexHull, Voronoi
 import itertools
-import warnings
 import copy
 import logging
 logger = logging.getLogger(__name__)
 
 from ..networks.site import Site
 from ..tools.misc import to_iterable, to_array, inverse_permutation, get_close, find_subclass
 from ..networks.mps import MPS  # only to check boundary conditions
@@ -59,19 +58,14 @@
     Infinite boundary conditions of the MPS repeat in the first spatial direction of the lattice,
     i.e., if the site at ``(x_0, x_1, ..., x_{dim-1},u)`` has MPS index `i`, the site
     at ``(x_0 + Ls[0], x_1, ..., x_{dim-1}, u)`` corresponds to MPS index ``i + N_sites``.
     Use :meth:`mps2lat_idx` and :meth:`lat2mps_idx` for conversion of indices.
     The function :meth:`mps2lat_values` performs the necessary reshaping and re-ordering from
     arrays indexed in MPS form to arrays indexed in lattice form.
 
-    .. deprecated :: 0.5.0
-        The parameters and attributes `nearest_neighbors`, `next_nearest_neighbors` and
-        `next_next_nearest_neighbors` are deprecated. Instead, we use a dictionary `pairs`
-        with those names as keys and the corresponding values as specified before.
-
     Parameters
     ----------
     Ls : list of int
         the length in each direction
     unit_cell : list of :class:`~tenpy.networks.site.Site`
         The sites making up a unit cell of the lattice.
         If you want to specify it only after initialization, use ``None`` entries in the list.
@@ -89,20 +83,14 @@
         vector (justifying the definition of `N_rings` and `N_sites_per_ring`).
     basis : iterable of 1D arrays
         For each direction one translation vectors shifting the unit cell.
         Defaults to the standard ONB ``np.eye(dim)``.
     positions : iterable of 1D arrays
         For each site of the unit cell the position within the unit cell.
         Defaults to ``np.zeros((len(unit_cell), dim))``.
-    nearest_neighbors : ``None`` | list of ``(u1, u2, dx)``
-        Deprecated. Specify as ``pairs['nearest_neighbors']`` instead.
-    next_nearest_neighbors : ``None`` | list of ``(u1, u2, dx)``
-        Deprecated. Specify as ``pairs['next_nearest_neighbors']`` instead.
-    next_next_nearest_neighbors : ``None`` | list of ``(u1, u2, dx)``
-        Deprecated. Specify as ``pairs['next_next_nearest_neighbors']`` instead.
     pairs : dict
         Of the form ``{'nearest_neighbors': [(u1, u2, dx), ...], ...}``.
         Typical keys are ``'nearest_neighbors', 'next_nearest_neighbors'``.
         For each of them, it specifies a list of tuples ``(u1, u2, dx)`` which can
         be used as parameters for :meth:`~tenpy.models.model.CouplingModel.add_coupling`
         to generate couplings over each pair of ,e.g., ``'nearest_neighbors'``.
         Note that this adds couplings for each pair *only in one direction*!
@@ -171,17 +159,14 @@
                  Ls,
                  unit_cell,
                  order='default',
                  bc='open',
                  bc_MPS='finite',
                  basis=None,
                  positions=None,
-                 nearest_neighbors=None,
-                 next_nearest_neighbors=None,
-                 next_next_nearest_neighbors=None,
                  pairs=None):
         self.unit_cell = list(unit_cell)
         self._set_Ls(Ls)  # after setting unit_cell
         if positions is None:
             positions = np.zeros((len(self.unit_cell), self.dim))
         if basis is None:
             basis = np.eye(self.dim)
@@ -192,25 +177,14 @@
         self.boundary_conditions = bc  # property setter for self.bc and self.bc_shift
         self.bc_MPS = bc_MPS
         self.position_disorder = None  # no disorder by default
         # calculate order for MPS
         self.order = self.ordering(order)
         # uses attribute setter to calculate _mps2lat_vals_idx_fix_u etc and lat2mps
         self.pairs = pairs if pairs is not None else {}
-        for name, NN in [('nearest_neighbors', nearest_neighbors),
-                         ('next_nearest_neighbors', next_nearest_neighbors),
-                         ('next_next_nearest_neighbors', next_next_nearest_neighbors)]:
-            if NN is None:
-                continue  # no value set
-            msg = "Lattice.__init__() got argument `{0!s}`.\nSet as `neighbors['{0!s}'] instead!"
-            msg = msg.format(name)
-            warnings.warn(msg, FutureWarning)
-            if name in self.pairs:
-                raise ValueError("{0!s} specified twice!".format(name))
-            self.pairs[name] = NN
         self.test_sanity()  # check consistency
 
     def test_sanity(self):
         """Sanity check.
 
         Raises ValueErrors, if something is wrong.
         """
@@ -961,34 +935,14 @@
         for u1, u2, dx in pairs:
             if u1 == u:
                 count += 1
             if u2 == u:
                 count += 1
         return count
 
-    def number_nearest_neighbors(self, u=0):
-        """Deprecated.
-
-        .. deprecated :: 0.5.0
-            Use :meth:`count_neighbors` instead.
-        """
-        msg = "Use ``count_neighbors(u, 'nearest_neighbors')`` instead."
-        warnings.warn(msg, FutureWarning)
-        return self.count_neighbors(u, 'nearest_neighbors')
-
-    def number_next_nearest_neighbors(self, u=0):
-        """Deprecated.
-
-        .. deprecated :: 0.5.0
-            Use :meth:`count_neighbors` instead.
-        """
-        msg = "Use ``count_neighbors(u, 'next_nearest_neighbors')`` instead."
-        warnings.warn(msg, FutureWarning)
-        return self.count_neighbors(u, 'next_nearest_neighbors')
-
     def distance(self, u1, u2, dx):
         """Get the distance for a given coupling between two sites in the lattice.
 
         The `u1`, `u2`, `dx` parameters are defined in analogy with
         :meth:`~tenpy.models.model.CouplingModel.add_coupling`, i.e., this function
         calculates the distance between a pair of operators added with `add_coupling` (using the
         :attr:`basis` and :attr:`unit_cell_positions` of the lattice).
@@ -1595,35 +1549,14 @@
         self.N_rings = self.Ls[0]
         self.N_sites_per_ring = int(self.N_sites // self.N_rings)
         strides = [1]
         for L in self.Ls:
             strides.append(strides[-1] * L)
         self._strides = np.array(strides, np.intp)
 
-    @property
-    def nearest_neighbors(self):
-        msg = ("Deprecated access with ``lattice.nearest_neighbors``.\n"
-               "Use ``lattice.pairs['nearest_neighbors']`` instead.")
-        warnings.warn(msg, FutureWarning)
-        return self.pairs['nearest_neighbors']
-
-    @property
-    def next_nearest_neighbors(self):
-        msg = ("Deprecated access with ``lattice.next_nearest_neighbors``.\n"
-               "Use ``lattice.pairs['next_nearest_neighbors']`` instead.")
-        warnings.warn(msg, FutureWarning)
-        return self.pairs['next_nearest_neighbors']
-
-    @property
-    def next_next_nearest_neighbors(self):
-        msg = ("Deprecated access with ``lattice.next_next_nearest_neighbors``.\n"
-               "Use ``lattice.pairs['next_next_nearest_neighbors']`` instead.")
-        warnings.warn(msg, FutureWarning)
-        return self.pairs['next_next_nearest_neighbors']
-
 
 class TrivialLattice(Lattice):
     """Trivial lattice consisting of a single (possibly large) unit cell in 1D.
 
     This is useful if you need a valid :class:`Lattice` with given :meth:`mps_sites`
     and don't care about the actual geometry, e.g, because you don't intend to use the
     :class:`~tenpy.models.model.CouplingModel`.
@@ -1731,15 +1664,15 @@
     :func:`~tenpy.networks.site.set_common_charges` (see examples there!) to adjust the charges,
     especially if you have different sites. Consider a combination of Fermions and Spins:
 
     .. doctest :: MultiSpeciesLattice
 
         >>> simple_lat = Square(2, 3, None)
         >>> f = tenpy.networks.site.FermionSite(conserve='N')
-        >>> s = tenpy.networks.site.SpinHalfSite(conserve='Sz')
+        >>> s = tenpy.networks.site.SpinHalfSite(conserve='Sz', sort_charge=False)
         >>> tenpy.networks.site.set_common_charges([f, s], 'independent')
         [array([0, 1]), array([1, 0])]
         >>> fs_lat = MultiSpeciesLattice(simple_lat, [f, s], ['f', 's'])
 
     There are corresponding coupling pairs defined:
 
     .. doctest :: MultiSpeciesLattice
@@ -2991,28 +2924,14 @@
                 return get_order(self.shape, snake_winding, priority)
             elif order == "snake" or order == "snake_rings":
                 priority = (0, 2, 1)
                 snake_winding = (False, False, True)
                 return get_order(self.shape, snake_winding, priority)
         return super().ordering(order)
 
-    @property
-    def fourth_nearest_neighbors(self):
-        msg = ("Deprecated access with ``lattice.fourth_nearest_neighbors``.\n"
-               "Use ``lattice.pairs['fourth_nearest_neighbors']`` instead.")
-        warnings.warn(msg, FutureWarning)
-        return self.pairs['fourth_nearest_neighbors']
-
-    @property
-    def fifth_nearest_neighbors(self):
-        msg = ("Deprecated access with ``lattice.fifth_nearest_neighbors``.\n"
-               "Use ``lattice.pairs['fifth_nearest_neighbors']`` instead.")
-        warnings.warn(msg, FutureWarning)
-        return self.pairs['fifth_nearest_neighbors']
-
 
 class Kagome(Lattice):
     """A Kagome lattice.
 
     .. plot ::
 
         import matplotlib.pyplot as plt
```

### Comparing `physics-tenpy-0.99.0/tenpy/models/mixed_xk.py` & `physics-tenpy-1.0.0/tenpy/models/mixed_xk.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/models/model.py` & `physics-tenpy-1.0.0/tenpy/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,17 @@
 from ..networks import mpo  # used to construct the Hamiltonian as MPO
 from ..networks.terms import OnsiteTerms, CouplingTerms, MultiCouplingTerms
 from ..networks.terms import ExponentiallyDecayingTerms, order_combine_term
 from ..networks.site import Site, group_sites
 from ..tools.hdf5_io import Hdf5Exportable
 
 __all__ = [
-    'Model', 'NearestNeighborModel', 'MPOModel', 'CouplingModel', 'MultiCouplingModel',
-    'CouplingMPOModel'
+    'Model', 'NearestNeighborModel', 'MPOModel', 'CouplingModel', 'CouplingMPOModel'
 ]
 
-_DEPRECATED_ARG_NOT_SET = "DEPRECATED"
-
 
 class Model(Hdf5Exportable):
     """Base class for all models.
 
     The common base to all models is the underlying Hilbert space and geometry, specified by a
     :class:`~tenpy.model.lattice.Lattice`.
 
@@ -813,28 +810,18 @@
 
 class CouplingModel(Model):
     """Base class for a general model of a Hamiltonian consisting of two-site couplings.
 
     In this class, the terms of the Hamiltonian are specified explicitly as
     :class:`~tenpy.networks.terms.OnsiteTerms` or :class:`~tenpy.networks.terms.CouplingTerms`.
 
-    .. deprecated:: 0.4.0
-        `bc_coupling` will be removed in 1.0.0. To specify the full geometry in the lattice,
-        use the `bc` parameter of the :class:`~tenpy.model.lattice.Lattice`.
-
     Parameters
     ----------
     lattice : :class:`~tenpy.model.lattice.Lattice`
         The lattice defining the geometry and the local Hilbert space(s).
-    bc_coupling : (iterable of) {``'open'`` | ``'periodic'`` | ``int``}
-        Boundary conditions of the couplings in each direction of the lattice. Defines how the
-        couplings are added in :meth:`add_coupling`. A single string holds for all directions.
-        An integer `shift` means that we have periodic boundary conditions along this direction,
-        but shift/tilt by ``-shift*lattice.basis[0]`` (~cylinder axis for ``bc_MPS='infinite'``)
-        when going around the boundary along this direction.
     explicit_plus_hc : bool
         If True, the Hermitian conjugate of the MPO is computed at runtime,
         rather than saved in the MPO.
 
     Attributes
     ----------
     onsite_terms : {'category': :class:`~tenpy.networks.terms.OnsiteTerms`}
@@ -852,21 +839,16 @@
         and :attr:`exp_decaying_terms` *plus* their hermitian conjugate added.
         The flag will be carried on to the MPO, which will have a reduced bond dimension if
         ``self.add_coupling(..., plus_hc=True)`` was used.
         Note that :meth:`add_onsite`, :meth:`add_coupling`, :meth:`add_multi_coupling`
         and :meth:`add_exponentially_decaying_coupling` respect this flag, ensuring that the
         *represented* Hamiltonian is independent of the `explicit_plus_hc` flag.
     """
-    def __init__(self, lattice, bc_coupling=None, explicit_plus_hc=False):
+    def __init__(self, lattice, explicit_plus_hc=False):
         Model.__init__(self, lattice)
-        if bc_coupling is not None:
-            warnings.warn("`bc_coupling` in CouplingModel: use `bc` in Lattice instead",
-                          FutureWarning,
-                          stacklevel=2)
-            lattice._set_bc(bc_coupling)
         L = self.lat.N_sites
         self.onsite_terms = {}
         self.coupling_terms = {}
         self.exp_decaying_terms = ExponentiallyDecayingTerms(L)
         self.explicit_plus_hc = explicit_plus_hc
         CouplingModel.test_sanity(self)
         # like self.test_sanity(), but use the version defined below even for derived class
@@ -1036,16 +1018,14 @@
                      strength,
                      u1,
                      op1,
                      u2,
                      op2,
                      dx,
                      op_string=None,
-                     str_on_first=True,
-                     raise_op2_left=False,
                      category=None,
                      plus_hc=False):
         r"""Add two-site coupling terms to the Hamiltonian, summing over lattice sites.
 
         Represents couplings of the form
         :math:`\sum_{x_0, ..., x_{dim-1}} strength[shift(\vec{x})] * OP0 * OP1`, where
         ``OP0 := lat.unit_cell[u0].get_op(op0)`` acts on the site ``(x_0, ..., x_{dim-1}, u1)``,
@@ -1061,17 +1041,14 @@
         and is chosen such that the first entry ``strength[0, 0, ...]`` of `strength`
         is the prefactor for the first possible coupling
         fitting into the lattice if you imagine open boundary conditions.
 
         The necessary terms are just added to :attr:`coupling_terms`;
         this function does not rebuild the MPO.
 
-        .. deprecated:: 0.4.0
-            The arguments `str_on_first` and `raise_op2_left` will be removed in version 1.0.0.
-
         Parameters
         ----------
         strength : scalar | array
             Prefactor of the coupling. May vary spatially (see above). If an array of smaller size
             is provided, it gets tiled to the required shape.
             A single scalar number can be given to indicate a coupling which is uniform across
             the lattice.
@@ -1088,27 +1065,14 @@
             For a 1D lattice, a single int is also fine.
         op_string : str | None
             Name of an operator to be used between the OP1 and OP2 sites.
             Typical use case is the phase for a Jordan-Wigner transformation.
             The operator should be defined on all sites in the unit cell.
             If ``None``, auto-determine whether a Jordan-Wigner string is needed, using
             :meth:`~tenpy.networks.site.Site.op_needs_JW`.
-        str_on_first : bool
-            Whether the provided `op_string` should also act on the first site.
-            This option should be chosen as ``True`` for Jordan-Wigner strings.
-            When handling Jordan-Wigner strings we need to extend the `op_string` to also act on
-            the 'left', first site (in the sense of the MPS ordering of the sites given by the
-            lattice). In this case, there is a well-defined ordering of the operators in the
-            physical sense (i.e. which of `op1` or `op2` acts first on a given state).
-            We follow the convention that `op2` acts first (in the physical sense),
-            independent of the MPS ordering.
-            Deprecated.
-        raise_op2_left : bool
-            Raise an error when `op2` appears left of `op1`
-            (in the sense of the MPS ordering given by the lattice). Deprecated.
         category : str
             Descriptive name used as key for :attr:`coupling_terms`.
             Defaults to a string of the form ``"{op1}_i {op2}_j"``.
         plus_hc : bool
             If `True`, the hermitian conjugate of the terms is added automatically.
 
         Examples
@@ -1186,25 +1150,23 @@
         site1 = self.lat.unit_cell[u1]
         site2 = self.lat.unit_cell[u2]
         if op_string is None:
             need_JW1 = site1.op_needs_JW(op1)
             need_JW2 = site2.op_needs_JW(op2)
             if need_JW1 and need_JW2:
                 op_string = 'JW'
-                str_on_first = True
             elif need_JW1 or need_JW2:
                 raise ValueError("Only one of the operators needs a Jordan-Wigner string?!")
             else:
                 op_string = 'Id'
         for u in range(len(self.lat.unit_cell)):
             if not self.lat.unit_cell[u].valid_opname(op_string):
                 raise ValueError("unknown onsite operator {0!r} for u={1:d}\n"
                                  "{2!r}".format(op_string, u, self.lat.unit_cell[u]))
-        if op_string == "JW" and not str_on_first:
-            raise ValueError("Jordan Wigner string without `str_on_first`")
+        str_on_first = (op_string == 'JW')
         if np.all(dx == 0) and u1 == u2:
             raise ValueError("Coupling shouldn't be onsite!")
         mps_i, mps_j, strength_vals = self.lat.possible_couplings(u1, u2, dx, strength)
         if self.explicit_plus_hc:
             # we explicitly add the h.c. later ...
             if plus_hc:
                 plus_hc = False  # ... so there's no need to do it at the bottom of this function
@@ -1221,32 +1183,29 @@
             # and allows `str_on_first` being set explicitly
             if i < j:
                 o1, o2 = op1, op2
                 if str_on_first and op_string != 'Id':
                     o1 = site1.multiply_op_names([op1, op_string])  # op2 acts first!
             else:  # i > j
                 # swap operators to ensure i <= j
-                if raise_op2_left:
-                    raise ValueError("Op2 is left")
                 i, j = j, i
                 o1, o2 = op2, op1
                 if str_on_first and op_string != 'Id':
                     o1 = site2.multiply_op_names([op_string, op2])  # op2 acts first!
             # now we have always i < j and 0 <= i < N_sites
             # j >= N_sites indicates couplings between unit_cells of the infinite MPS.
             # o1 is the "left" operator; o2 is the "right" operator
             ct.add_coupling_term(current_strength, i, j, o1, o2, op_string)
 
         if plus_hc:
             hc_op1 = site1.get_hc_op_name(op1)
             hc_op2 = site2.get_hc_op_name(op2)
             hc_opstr = site2.get_hc_op_name(op_string)
             self.add_coupling(np.conj(strength), u2, hc_op2, u1, hc_op1, -dx,
-                              hc_opstr, str_on_first, raise_op2_left,
-                              category, plus_hc=False)  # yapf: disable
+                              hc_opstr, category, plus_hc=False)  # yapf: disable
         # done
 
     def add_coupling_term(self,
                           strength,
                           i,
                           j,
                           op_i,
@@ -1308,16 +1267,14 @@
         for t in self.coupling_terms.values():
             ct += t
         return ct
 
     def add_multi_coupling(self,
                            strength,
                            ops,
-                           _deprecate_1=_DEPRECATED_ARG_NOT_SET,
-                           _deprecate_2=_DEPRECATED_ARG_NOT_SET,
                            op_string=None,
                            category=None,
                            plus_hc=False,
                            switchLR='middle_i'):
         r"""Add multi-site coupling terms to the Hamiltonian, summing over lattice sites.
 
         Represents couplings of the form
@@ -1335,21 +1292,14 @@
         and is chosen such that the first entry ``strength[0, 0, ...]`` of `strength`
         is the prefactor for the first possible coupling
         fitting into the lattice if you imagine open boundary conditions.
 
         The necessary terms are just added to :attr:`coupling_terms`;
         this function does not rebuild the MPO.
 
-        .. deprecated:: 0.6.0
-            We switched from the three arguments `u0`, `op0` and `other_op` with
-            ``other_ops=[(u1, op1, dx1), (op2, u2, dx2), ...]``
-            to a single, equivalent argument `ops` which should now read
-            ``ops=[(op0, dx0, u0), (op1, dx1, u1), (op2, dx2, u2), ...]``, where
-            ``dx0 = [0]*self.lat.dim``. Note the changed order inside the tuples!
-
         Parameters
         ----------
         strength : scalar | array
             Prefactor of the coupling. May vary spatially, and is tiled to the required shape.
         ops : list of ``(opname, dx, u)``
             Each tuple determines one operator of the coupling, see the description above.
             `opname` (str) is the name of the operator,
@@ -1399,31 +1349,14 @@
 
         See also
         --------
         add_onsite : Add terms acting on one site only.
         add_coupling : Add terms acting on two sites.
         add_multi_coupling_term : Add a single term, not summing over the possible :math:`\vec{x}`.
         """
-        if _deprecate_1 is not _DEPRECATED_ARG_NOT_SET or \
-                _deprecate_2 is not _DEPRECATED_ARG_NOT_SET:
-            msg = ("Deprecated arguments of CouplingModel.add_multi_coupling:\n"
-                   "switch to using a single argument \n"
-                   "     ops=[(op0, [0]*self.lat.dim, u0), (op1, dx1, u1), (op2, dx2, u2), ...]\n"
-                   "instead of the three arguments \n"
-                   "     u0\n"
-                   "     op0\n"
-                   "     other_ops=[(u1, op1, dx1), (op2, u2, dx2), ...]\n"
-                   "Note the reordering ``(u, op, dx) -> (op, dx, u)`` in the tuples!")
-            warnings.warn(msg, FutureWarning, stacklevel=2)
-            u0 = ops
-            op0 = _deprecate_1
-            dx0 = [0] * self.lat.dim
-            other_ops = _deprecate_2
-            # new argument:
-            ops = [(op0, dx0, u0)] + [(op, dx, u) for (u, op, dx) in other_ops]
         # split `ops` into separate groups
         all_ops = [t[0] for t in ops]
         all_us = np.array([t[2] for t in ops], np.intp)
         all_dxs = np.array([t[1] for t in ops], np.intp).reshape([len(ops), self.lat.dim])
         if not np.any(np.asarray(strength) != 0.):
             return  # nothing to do: can even accept non-defined onsite operators
         need_JW = np.array([self.lat.unit_cell[u].op_needs_JW(op) for op, _, u in ops],
@@ -1641,44 +1574,14 @@
                                                                     subsites, op_string)
         if plus_hc:
             hc_op_i = site0.get_hc_op_name(op_i)
             hc_op_j = site0.get_hc_op_name(op_j)
             self.exp_decaying_terms.add_exponentially_decaying_coupling(
                 np.conj(strength), np.conj(lambda_), hc_op_i, hc_op_j, subsites, op_string)
 
-    def calc_H_onsite(self, tol_zero=1.e-15):
-        """Calculate `H_onsite` from `self.onsite_terms`.
-
-        .. deprecated:: 0.4.0
-            This function will be removed in 1.0.0.
-            Replace calls to this function by
-            ``self.all_onsite_terms().remove_zeros(tol_zero).to_Arrays(self.lat.mps_sites())``.
-            You might also want to take :attr:`explicit_plus_hc` into account.
-
-        Parameters
-        ----------
-        tol_zero : float
-            prefactors with ``abs(strength) < tol_zero`` are considered to be zero.
-
-        Returns
-        -------
-        H_onsite : list of npc.Array
-        onsite terms of the Hamiltonian. If :attr:`explicit_plus_hc` is True,
-            Hermitian conjugates of the onsite terms will be included.
-        """
-        warnings.warn("Deprecated `calc_H_onsite` in CouplingModel", FutureWarning, stacklevel=2)
-        ot = self.all_onsite_terms()
-        ot.remove_zeros(tol_zero)
-        ot_arrays = ot.to_Arrays(self.lat.mps_sites())
-        if self.explicit_plus_hc:
-            for i, op in enumerate(ot_arrays):
-                if op is not None:
-                    ot_arrays[i] = op + op.conj().itranspose(op.get_leg_labels())
-        return ot_arrays
-
     def calc_H_bond(self, tol_zero=1.e-15):
         """calculate `H_bond` from :attr:`coupling_terms` and :attr:`onsite_terms`.
 
         Parameters
         ----------
         tol_zero : float
             prefactors with ``abs(strength) < tol_zero`` are considered to be zero.
@@ -1832,30 +1735,14 @@
             if dx[ax] > 0:
                 strength[slices] *= np.exp(-1.j * phase[ax])  # hopping in *negative* y-direction
             else:
                 strength[slices] *= np.exp(1.j * phase[ax])  # hopping in *positive* y-direction
         return strength
 
 
-class MultiCouplingModel(CouplingModel):
-    """Deprecated class which was a generalization of the `CouplingModel`.
-
-    .. deprecated:: 0.7.2
-        In earlier versions of TeNPy, this class contained the methods
-        :meth:`add_multi_coupling` and :meth:`add_multi_coupling_term`.
-        However, since we introduced the :class:`~tenpy.networks.terms.MultiCouplingTerms`,
-        this separation within the Model class is no longer necessary.
-        We hence merged the `MultiCouplingModel` with the `CouplingModel`.
-    """
-    def __init_subclass__(cls):
-        msg = ("The `MultiCouplingModel` class is deprecated and has been merged into "
-               "the `CouplingModel`. No need to subclass the `MultiCouplingModel` anymore!")
-        warnings.warn(msg, DeprecationWarning, 2)
-
-
 def _warn_post_init_add(f):
     @wraps(f)
     def add_term_function(self, *args, **kwargs):
         res = f(self, *args, **kwargs)
         if hasattr(self, 'H_MPO') and not getattr(self, 'manually_call_init_H', False):
             warnings.warn(
                 "Adding terms to the CouplingMPOModel after initialization. "
@@ -1944,21 +1831,14 @@
         # 6) add terms of the Hamiltonian
         self.init_terms(model_params)
         # 7-8) initialize H_MPO, and H_bonds, if necessary
         self.init_H_from_terms()
         # finally checks for misspelled parameter names
         model_params.warn_unused()
 
-    @property
-    def verbose(self):
-        warnings.warn(
-            "verbose is deprecated, we're using logging now! \n"
-            "See https://tenpy.readthedocs.io/en/latest/intro/logging.html", FutureWarning, 2)
-        return self.options.get('verbose', 1.)
-
     def init_H_from_terms(self):
         """Initialize `H_MPO` (and `H_bond`) from the terms of the `CouplingModel`.
 
         This function is called automatically during `CouplingMPOModel.__init__`.
 
         If you use one of the `add_*` methods of the `CouplingModel` *after* initialization,
         you will need to call `init_H_from_terms` in the end by yourself,
```

### Comparing `physics-tenpy-0.99.0/tenpy/models/spins.py` & `physics-tenpy-1.0.0/tenpy/models/spins.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,17 +38,16 @@
         :include: CouplingMPOModel
 
         S : {0.5, 1, 1.5, 2, ...}
             The 2S+1 local states range from m = -S, -S+1, ... +S.
         conserve : 'best' | 'Sz' | 'parity' | None
             What should be conserved. See :class:`~tenpy.networks.Site.SpinSite`.
             For ``'best'``, we check the parameters what can be preserved.
-        sort_charge : bool | None
-            Whether to sort by charges of physical legs.
-            See change comment in :class:`~tenpy.networks.site.Site`.
+        sort_charge : bool
+            Whether to sort by charges of physical legs. `True` by default.
         Jx, Jy, Jz, hx, hy, hz, muJ, D, E  : float | array
             Coupling as defined for the Hamiltonian above.
 
     """
     def init_sites(self, model_params):
         S = model_params.get('S', 0.5)
         conserve = model_params.get('conserve', 'best')
@@ -58,15 +57,15 @@
                                             "check Sz conservation"):
                 conserve = 'Sz'
             elif not model_params.any_nonzero(['hx', 'hy'], "check parity conservation"):
                 conserve = 'parity'
             else:
                 conserve = None
             self.logger.info("%s: set conserve to %s", self.name, conserve)
-        sort_charge = model_params.get('sort_charge', None)
+        sort_charge = model_params.get('sort_charge', True)
         site = SpinSite(S, conserve, sort_charge)
         return site
 
     def init_terms(self, model_params):
         Jx = model_params.get('Jx', 1.)
         Jy = model_params.get('Jy', 1.)
         Jz = model_params.get('Jz', 1.)
```

### Comparing `physics-tenpy-0.99.0/tenpy/models/spins_nnn.py` & `physics-tenpy-1.0.0/tenpy/models/spins_nnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,17 +150,16 @@
         :include: CouplingMPOModel
 
         S : {0.5, 1, 1.5, 2, ...}
             The 2S+1 local states range from m = -S, -S+1, ... +S.
         conserve : 'best' | 'Sz' | 'parity' | None
             What should be conserved. See :class:`~tenpy.networks.Site.SpinSite`.
             For ``'best'``, we check the parameters what can be preserved.
-        sort_charge : bool | None
-            Whether to sort by charges of physical legs.
-            See change comment in :class:`~tenpy.networks.site.Site`.
+        sort_charge : bool
+            Whether to sort by charges of physical legs. `True` by default.
         Jx, Jy, Jz, Jxp, Jyp, Jzp, hx, hy, hz : float | array
             Coupling as defined for the Hamiltonian above.
     """
     def init_sites(self, model_params):
         S = model_params.get('S', 0.5)
         conserve = model_params.get('conserve', 'best')
         if conserve == 'best':
@@ -169,15 +168,15 @@
                                              ('Jxp', 'Jyp'), 'hx', 'hy'], "check Sz conservation"):
                 conserve = 'Sz'
             elif not model_params.any_nonzero(['hx', 'hy'], "check parity conservation"):
                 conserve = 'parity'
             else:
                 conserve = None
             self.logger.info("%s: set conserve to %s", self.name, conserve)
-        sort_charge = model_params.get('sort_charge', None)
+        sort_charge = model_params.get('sort_charge', True)
         site = SpinSite(S, conserve, sort_charge=sort_charge)
         return site
 
     def init_terms(self, model_params):
         # 0) read out/set default parameters
         Jx = model_params.get('Jx', 1.)
         Jy = model_params.get('Jy', 1.)
```

### Comparing `physics-tenpy-0.99.0/tenpy/models/tf_ising.py` & `physics-tenpy-1.0.0/tenpy/models/tf_ising.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,28 +39,27 @@
     Options
     -------
     .. cfg:config :: TFIModel
         :include: CouplingMPOModel
 
         conserve : None | 'parity'
             What should be conserved. See :class:`~tenpy.networks.Site.SpinHalfSite`.
-        sort_charge : bool | None
-            Whether to sort by charges of physical legs.
-            See change comment in :class:`~tenpy.networks.site.Site`.
+        sort_charge : bool
+            Whether to sort by charges of physical legs. `True` by default.
         J, g : float | array
             Coupling as defined for the Hamiltonian above.
 
     """
     def init_sites(self, model_params):
         conserve = model_params.get('conserve', 'parity')
         assert conserve != 'Sz'
         if conserve == 'best':
             conserve = 'parity'
             self.logger.info("%s: set conserve to %s", self.name, conserve)
-        sort_charge = model_params.get('sort_charge', None)
+        sort_charge = model_params.get('sort_charge', True)
         site = SpinHalfSite(conserve=conserve, sort_charge=sort_charge)
         return site
 
     def init_terms(self, model_params):
         J = np.asarray(model_params.get('J', 1.))
         g = np.asarray(model_params.get('g', 1.))
         for u in range(len(self.lat.unit_cell)):
```

### Comparing `physics-tenpy-0.99.0/tenpy/models/tj_model.py` & `physics-tenpy-1.0.0/tenpy/models/tj_model.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/models/toric_code.py` & `physics-tenpy-1.0.0/tenpy/models/toric_code.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,17 +113,16 @@
     .. cfg:config :: ToricCode
         :include: CouplingMPOModel
 
         Lx, Ly: int
             Dimension of the lattice, number of plaquettes around the cylinder.
         conserve : 'parity' | None
             What should be conserved. See :class:`~tenpy.networks.Site.SpinHalfSite`.
-        sort_charge : bool | None
-            Whether to sort by charges of physical legs.
-            See change comment in :class:`~tenpy.networks.site.Site`.
+        sort_charge : bool
+            Whether to sort by charges of physical legs. `True` by default.
         Jv, Jp : float | array
             Couplings as defined for the Hamiltonian above.
         order : str
             The order of the lattice sites in the lattice, see :class:`DualSquare`.
         bc_y : ``"open" | "periodic"``
             The boundary conditions in y-direction.
         bc_x : ``"open" | "periodic"``
@@ -137,15 +136,15 @@
             first and last sites of the MPS, and require **squared** MPS bond-dimensions.
     """
     default_lattice = DualSquare
     force_default_lattice = True
 
     def init_sites(self, model_params):
         conserve = model_params.get('conserve', 'parity')
-        sort_charge = model_params.get('sort_charge', None)
+        sort_charge = model_params.get('sort_charge', True)
         site = SpinHalfSite(conserve, sort_charge=sort_charge)
         return site
 
     def init_terms(self, model_params):
         Jv = np.asarray(model_params.get('Jv', 1.))
         Jp = np.asarray(model_params.get('Jp', 1.))
         # vertex/star term
```

### Comparing `physics-tenpy-0.99.0/tenpy/models/xxz_chain.py` & `physics-tenpy-1.0.0/tenpy/models/xxz_chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,28 +39,27 @@
 
         L : int
             Length of the chain.
         Jxx, Jz, hz : float | array
             Coupling as defined for the Hamiltonian above.
         bc_MPS : {'finite' | 'infinite'}
             MPS boundary conditions. Coupling boundary conditions are chosen appropriately.
-        sort_charge : bool | None
-            Whether to sort by charges of physical legs.
-            See change comment in :class:`~tenpy.networks.site.Site`.
+        sort_charge : bool
+            Whether to sort by charges of physical legs. `True` by default.
 
     """
     def __init__(self, model_params):
         # 0) read out/set default parameters
         model_params = asConfig(model_params, "XXZChain")
         L = model_params.get('L', 2)
         Jxx = model_params.get('Jxx', 1.)
         Jz = model_params.get('Jz', 1.)
         hz = model_params.get('hz', 0.)
         bc_MPS = model_params.get('bc_MPS', 'finite')
-        sort_charge = model_params.get('sort_charge', None)
+        sort_charge = model_params.get('sort_charge', True)
         # 1-3):
         USE_PREDEFINED_SITE = False
         if not USE_PREDEFINED_SITE:
             # 1) charges of the physical leg. The only time that we actually define charges!
             leg = npc.LegCharge.from_qflat(npc.ChargeInfo([1], ['2*Sz']), [1, -1])
             # 2) onsite operators
             Sp = [[0., 1.], [0., 0.]]
@@ -102,15 +101,15 @@
     model_params : dict | :class:`~tenpy.tools.params.Config`
         See :cfg:config:`XXZChain`
     """
     default_lattice = "Chain"
     force_default_lattice = True
 
     def init_sites(self, model_params):
-        sort_charge = model_params.get('sort_charge', None)
+        sort_charge = model_params.get('sort_charge', True)
         return SpinHalfSite(conserve='Sz', sort_charge=sort_charge)  # use predefined Site
 
     def init_terms(self, model_params):
         # read out parameters
         Jxx = model_params.get('Jxx', 1.)
         Jz = model_params.get('Jz', 1.)
         hz = model_params.get('hz', 0.)
```

### Comparing `physics-tenpy-0.99.0/tenpy/networks/__init__.py` & `physics-tenpy-1.0.0/tenpy/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/networks/momentum_mps.py` & `physics-tenpy-1.0.0/tenpy/networks/momentum_mps.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/networks/mpo.py` & `physics-tenpy-1.0.0/tenpy/networks/mpo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1358,43 +1358,14 @@
                 VH = VH.split_legs()
                 VH.iscale_axis(S, 'vL')
                 psi.set_SR(i, S)
                 psi.set_B(i, U, 'A')
 
         return trunc_err
 
-    def get_grouped_mpo(self, blocklen):
-        """group each `blocklen` subsequent tensors and  return result as a new MPO.
-
-        .. deprecated :: 0.5.0
-            Make a copy and use :meth:`group_sites` instead.
-        """
-        msg = "Use functions from `tenpy.algorithms.exact_diag.ExactDiag.from_H_mpo` instead"
-        warnings.warn(msg, FutureWarning, 2)
-        from copy import deepcopy
-        groupedMPO = deepcopy(self)
-        groupedMPO.group_sites(n=blocklen)
-        return (groupedMPO)
-
-    def get_full_hamiltonian(self, maxsize=1e6):
-        """extract the full Hamiltonian as a ``d**L``x``d**L`` matrix.
-
-        .. deprecated :: 0.5.0
-            Use :meth:`tenpy.algorithms.exact_diag.ExactDiag.from_H_mpo` instead.
-        """
-        msg = "Use functions from `tenpy.algorithms.exact_diag.ExactDiag.from_H_mpo` instead"
-        warnings.warn(msg, FutureWarning, 2)
-        if (self.dim[0]**(2 * self.L) > maxsize):
-            print('Matrix dimension exceeds maxsize')
-            return np.zeros(1)
-        singlesitempo = self.get_grouped_mpo(self.L)
-        # Note: the trace works only for 'finite' boundary conditions
-        # where the legs are trivial - otherwise it would give 0 or even raise an error!
-        return npc.trace(singlesitempo.get_W(0), axes=[['wL'], ['wR']])
-
     def _to_valid_index(self, i, bond=False):
         """Make sure `i` is a valid index (depending on `self.bc`)."""
         if not self.finite:
             return i % self.L
         if i < 0:
             i += self.L
         if i >= self.L + int(bond) or i < 0:
```

### Comparing `physics-tenpy-0.99.0/tenpy/networks/mps.py` & `physics-tenpy-1.0.0/tenpy/networks/mps.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 :attr:`~tenpy.networks.mps.MPS.nontrivial_bonds` depending on the boundary conditions.
 
 The matrices and singular values always represent a normalized state
 (i.e. ``np.linalg.norm(psi._S[ib]) == 1`` up to roundoff errors),
 but (for finite MPS) we keep track of the norm in :attr:`~tenpy.networks.mps.MPS.norm`
 (which is respected by :meth:`~tenpy.networks.mps.MPS.overlap`, ...).
 
-Valid MPS boundary conditions (not to confuse with `bc_coupling` of
-:class:`tenpy.models.model.CouplingModel`)  are the following:
+Valid MPS boundary conditions are the following:
 
 ==========  ===================================================================================
 `bc`        description
 ==========  ===================================================================================
 'finite'    Finite MPS, ``G0 s1 G1 ... s{L-1} G{l-1}``. This is achieved
             by using a trivial left and right bond ``s[0] = s[-1] = np.array([1.])``.
 'segment'   Generalization of 'finite', describes an MPS embedded in left and right
@@ -2457,39 +2456,14 @@
         ValueError : if trying to convert from a ``None`` form. Use :meth:`canonical_form` instead!
         """
         new_forms = self._parse_form(new_form)
         for i, new_form in enumerate(new_forms):
             new_B = self.get_B(i, form=new_form, copy=False)  # calculates the desired form.
             self.set_B(i, new_B, form=new_form)
 
-    def increase_L(self, new_L=None):
-        """Modify `self` inplace to enlarge the MPS unit cell.
-
-        .. deprecated :: 0.5.1
-            This method will be removed in version 1.0.0.
-            Use the equivalent ``psi.enlarge_mps_unit_cell(new_L//psi.L)`` instead of
-            ``psi.increase_L(new_L)``.
-
-        Parameters
-        ----------
-        new_L : int
-            New number of sites. Needs to be an integer multiple of :attr:`L`.
-            Defaults to ``2*self.L``.
-        """
-        old_L = self.L
-        if new_L is None:
-            new_L = 2 * old_L
-        if new_L % old_L:
-            raise ValueError("new_L = {0:d} not a multiple of old L={1:d}".format(new_L, old_L))
-        factor = new_L // old_L
-        warnings.warn(
-            "use `psi.enlarge_mps_unit_cell(factor=new_L//psi.L)` "
-            "instead of `psi.increase_L(new_L)`.", FutureWarning, 2)
-        self.enlarge_mps_unit_cell(factor)
-
     def enlarge_mps_unit_cell(self, factor=2):
         """Repeat the unit cell for infinite MPS boundary conditions; in place.
 
         Parameters
         ----------
         factor : int
             The new number of sites in the unit cell will be increased from `L` to ``factor*L``.
@@ -3585,36 +3559,28 @@
                               "thermodynamic limit! "
                               "See the warning in the docs of tenpy.networks.mps.")
             form = None if ignore_form else 'B'
             TM = TransferMatrix(self, other, charge_sector=charge_sector, form=form)
             ov, _ = TM.eigenvectors(**kwargs)
             return ov[0] * self.norm * other.norm
 
-    def expectation_value_terms_sum(self, term_list, prefactors=None):
+    def expectation_value_terms_sum(self, term_list):
         """Calculate expectation values for a bunch of terms and sum them up.
 
         This is equivalent to the following expression::
 
             sum([self.expectation_value_term(term)*strength for term, strength in term_list])
 
         However, for efficiency, the term_list is converted to an MPO and the expectation value
         of the MPO is evaluated.
 
-        .. deprecated:: 0.4.0
-            `prefactor` will be removed in version 1.0.0.
-            Instead, directly give just ``TermList(term_list, prefactors)`` as argument.
-
         Parameters
         ----------
         term_list : :class:`~tenpy.networks.terms.TermList`
             The terms and prefactors (`strength`) to be summed up.
-        prefactors :
-            Instead of specifying a :class:`~tenpy.networks.terms.TermList`,
-            one can also specify the term_list and strength separately.
-            This is deprecated.
 
         Returns
         -------
         terms_sum : list of (complex) float
             Equivalent to the expression
             ``sum([self.expectation_value_term(term)*strength for term, strength in term_list])``.
         _mpo :
@@ -3624,19 +3590,14 @@
 
         See also
         --------
         expectation_value_term : evaluates a single `term`.
         tenpy.networks.mpo.MPO.expectation_value : expectation value density of an MPO.
         """
         from . import mpo, terms
-        if prefactors is not None:
-            warnings.warn(
-                "Deprecated argument prefactors: replace arguments with "
-                "``TermList(term_list, prefactors)``.", FutureWarning, 2)
-            term_list = terms.TermList(term_list, prefactors)
         L = self.L
         if not self.finite:
             copy = None
             for a, term in enumerate(term_list.terms):
                 i_min = min([i for _, i in term])
                 if not 0 <= i_min < L:
                     if copy is None:
@@ -3919,23 +3880,14 @@
                 new_UL = npc.tensordot(old_UL, U, axes=['vR', 'vL'])
                 new_VR = npc.tensordot(VR_segment, old_VR, axes=['vR', 'vL'])
                 self.segment_boundaries = (new_UL, new_VR)
             else:
                 self.segment_boundaries = (U, VR_segment)
             return U, VR_segment
 
-    def canonical_form_infinite(self, **kwargs):
-        """Deprecated wrapper around :meth:`canonical_form_infinite1`."""
-        warnings.warn(
-            "There are different implementations of `canonical_form_infinite` now. "
-            "Select one explicitly!",
-            FutureWarning,
-            stacklevel=2)
-        self.canonical_form_infinite1(**kwargs)
-
     def canonical_form_infinite1(self, renormalize=True, tol_xi=1.e6):
         """Bring an infinite MPS into canonical form; in place.
 
         If any site is in :attr:`form` ``None``, it does *not* use any of the singular values `S`.
         If all sites have a `form`, it respects the `form` to ensure
         that one `S` is included per bond.
         The final state is always in right-canonical 'B' form.
@@ -4777,20 +4729,17 @@
         self.set_SR(i, S)
         self.set_B(i, B_L, 'B')
         self.set_B(i + 1, B_R, 'B')
         self.sites[self._to_valid_index(i)] = siteR  # swap 'sites' as well
         self.sites[self._to_valid_index(i + 1)] = siteL
         return err
 
-    def permute_sites(self, perm, swap_op='auto', trunc_par=None, verbose=None):
+    def permute_sites(self, perm, swap_op='auto', trunc_par=None):
         """Applies the permutation perm to the state; in place.
 
-        .. deprecated :: 0.8.0
-            Drop / ignore `verbose` argument, never print something.
-
         Parameters
         ----------
         perm : ndarray[ndim=1, int]
             The applied permutation, such that ``psi.permute_sites(perm)[i] = psi[perm[i]]``
             (where ``[i]`` indicates the `i`-th site).
         swap_op : ``None`` | ``'auto', 'autoInv'`` | :class:`~tenpy.linalg.np_conserved.Array`
             The operator used to swap the physical legs of a two-site wave function `theta`,
@@ -4799,16 +4748,14 @@
             Parameters for truncation, see :cfg:config:`truncation`.
 
         Returns
         -------
         trunc_err : :class:`~tenpy.algorithms.truncation.TruncationError`
             The error of the represented state introduced by the truncation after the swaps.
         """
-        if verbose is not None:
-            warnings.warn("Dropped verbose argument", category=FutureWarning, stacklevel=2)
         perm = list(perm)  # gets modified, so we should copy
         # In order to keep sites close together, we always scan from the left,
         # keeping everything up to `i` in strictly ascending order.
         # => more or less an 'insertion' sort algorithm.
         # Works nicely for permutations like [1,2,3,0,6,7,8,5] (swapping the 0 and 5 around).
         # For [ 2 3 4 5 6 7 0 1], it splits 0 and 1 apart (first swapping the 0 down, then the 1)
         if trunc_par is None:
@@ -4831,30 +4778,26 @@
         return trunc_err
 
     def compute_K(self,
                   perm,
                   swap_op='auto',
                   trunc_par=None,
                   canonicalize=1.e-6,
-                  verbose=None,
                   expected_mean_k=0.):
         r"""Compute the momentum quantum numbers of the entanglement spectrum for 2D states.
 
         Works for an infinite MPS living on a cylinder, infinitely long in `x` direction and with
         periodic boundary conditions in `y` directions.
         If the state is invariant under 'rotations' around the cylinder axis, one can find the
         momentum quantum numbers of it. (The rotation is nothing more than a translation in `y`.)
         This function permutes some sites (on a copy of `self`) to enact the rotation, and then
         finds the dominant eigenvector of the mixed transfer matrix to get the quantum numbers,
         along the lines of :cite:`pollmann2012`, see also (the appendix and Fig. 11 in the arXiv
         version of) :cite:`cincio2013`.
 
-        .. deprecated :: 0.8.0
-            Drop / ignore `verbose` argument, never print something.
-
         Parameters
         ----------
         perm : 1D ndarray | :class:`~tenpy.models.lattice.Lattice`
             Permutation to be applied to the physical indices, see :meth:`permute_sites`.
             If a lattice is given, we use it to read out the lattice structure and shift
             each site by one lattice-vector in y-direction (assuming periodic boundary conditions).
             (If you have a :class:`~tenpy.models.model.CouplingModel`,
@@ -5911,28 +5854,27 @@
     Here the `N` denotes the matrices of the bra and `M` the ones of the ket, respectively.
     To view it as a `matrix`, we combine the left and right indices to pipes::
 
         |  (vL.vL*) ->-TM->- (vR.vR*)   acting on  (vL.vL*) ->-RP
 
     Note that we keep all M and N as copies.
 
-    .. deprecated :: 0.6.0
-        The default for `shift_ket` was the value of `shift_bra`, this will be changed to 0.
+    .. versionchanged :: 1.0
+        shift_bra defaults to 0 rather than `shift_ket`.
 
     Parameters
     ----------
     bra : MPS
         The MPS which is to be (complex) conjugated.
     ket : MPS
         The MPS which is not (complex) conjugated.
     shift_bra : int
         We start the `N` of the bra at site `shift_bra` (i.e. the `j` in the above network).
-    shift_ket : int | None
+    shift_ket : int
         We start the `M` of the ket at site `shift_ket` (i.e. the `i` in the above network).
-        ``None`` is deprecated, default will be changed to 0 in the future.
     transpose : bool
         Whether `self.matvec` acts on `RP` (``False``) or `LP` (``True``).
     charge_sector : None | charges | ``0``
         Selects the charge sector of the vector onto which the Linear operator acts.
         ``None`` stands for *all* sectors, ``0`` stands for the zero-charge sector.
         Defaults to ``0``, i.e., **assumes** the dominant eigenvector is in charge sector 0.
         Note that you can update the `charge_sector` after initialization
@@ -5944,16 +5886,16 @@
     Attributes
     ----------
     L : int
         Number of physical sites involved in the transfer matrix, i.e. the least common multiple
         of `bra.L` and `ket.L`.
     shift_bra : int
         We start the `N` of the bra at site `shift_bra`.
-    shift_ket : int | None
-        We start the `M` of the ket at site `shift_ket`. ``None`` defaults to `shift_bra`.
+    shift_ket : int
+        We start the `M` of the ket at site `shift_ket`.
     transpose : bool
         Whether `self.matvec` acts on `RP` (``True``) or `LP` (``False``).
     qtotal : charges
         Total charge of the transfer matrix (which is gauged away in matvec).
     form : tuple(float, float) | None
         In which canonical form (all of) the `M` and `N` matrices are.
     flat_linop : :class:`~tenpy.linalg.sparse.FlatLinearOperator`
@@ -5969,26 +5911,21 @@
         The matrices of the ket, transposed for fast `matvec`.
     """
 
     def __init__(self,
                  bra,
                  ket,
                  shift_bra=0,
-                 shift_ket=None,
+                 shift_ket=0,
                  transpose=False,
                  charge_sector=0,
                  form='B'):
         L = lcm(bra.L, ket.L)
         if ket.chinfo != bra.chinfo:
             raise ValueError("incompatible charges")
-        if shift_ket is None:
-            if shift_bra != 0:
-                warnings.warn("default for shift_ket will change to 0. Specify both explicitly!",
-                              FutureWarning, 2)
-            shift_ket = shift_bra
         self.shift_bra = shift_bra
         self.shift_ket = shift_ket
         assert ket._p_label == bra._p_label
         form = ket._to_valid_form(form)
         ket_M = [ket.get_B(i, form=form) for i in range(shift_ket, shift_ket + L)]
         bra_N = [bra.get_B(i, form=form) for i in range(shift_bra, shift_bra + L)]
```

### Comparing `physics-tenpy-0.99.0/tenpy/networks/purification_mps.py` & `physics-tenpy-1.0.0/tenpy/networks/purification_mps.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/networks/site.py` & `physics-tenpy-1.0.0/tenpy/networks/site.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 
 """
 # Copyright (C) TeNPy Developers, GNU GPLv3
 
 import numpy as np
 import itertools
 import copy
-import warnings
 
 from ..linalg import np_conserved as npc
 from ..tools.misc import inverse_permutation, find_subclass
 from ..tools.hdf5_io import Hdf5Exportable
 
 __all__ = [
     'Site',
     'GroupedSite',
     'group_sites',
     'set_common_charges',
-    'multi_sites_combine_charges',
     'kron',
     'SpinHalfSite',
     'SpinSite',
     'FermionSite',
     'SpinHalfFermionSite',
     'SpinHalfHoleSite',
     'BosonSite',
@@ -44,44 +42,34 @@
 
     .. warning ::
         The order of the local basis can change depending on the charge conservation!
         This is a *necessary* feature since we need to sort the basis by charges for efficiency.
         We use the :attr:`state_labels` and :attr:`perm` to keep track of these permutations.
 
     .. versionchanged :: 0.10
+        Added `sort_charge` defaulting to `False`.
 
-        Add the option `sort_charge`. Right now the default behavior is ``False`` for
-        backwards compatibility, but we will change it for Version 1.0 to ``True``.
-        For now, we raise a warning in cases where it can lead to changes.
-        If you see this warning, just set the value explicitly to avoid breaking compatibility of
-        existing data with future releases.
-        Set it to `False`, if you already have data (for your particular model),
-        that you want to be able to load/compare to.
-        If you start a new project and don't have data yet, set it to `True`.
-        See also the `breaking changes` section in the release notes.
-
+    .. versionchanged :: 1.0
+        Make `sort_charge` default to `True`.
 
     Parameters
     ----------
     leg : :class:`~tenpy.linalg.charges.LegCharge`
         Charges of the physical states, to be used for the physical leg of MPS.
     state_labels : None | list of str
         Optionally a label for each local basis states. ``None`` entries are ignored / not set.
     **site_ops :
         Additional keyword arguments of the form ``name=op`` given to :meth:`add_op`.
         The identity operator ``'Id'`` is automatically included.
         If no ``'JW'`` for the Jordan-Wigner string is given,
         ``'JW'`` is set as an alias to ``'Id'``.
-    sort_charge : bool | None
+    sort_charge : bool
         Whether :meth:`sort_charge` should be called at the end of initialization.
         This is usually a good idea to reduce potential overhead when using charge conservation.
         Note that this might permute the order of the local basis states!
-        For backwards compatibility with existing data, it is not (yet) enabled by default,
-        but we started to warn about the behavior.
-        Explicitly set `sort_charge=False` to disable the warning.
 
     Attributes
     ----------
     leg : :class:`~tenpy.linalg.charges.LegCharge`
         Charges of the local basis states.
     state_labels : {str: int}
         (Optional) labels for the local basis states.
@@ -121,32 +109,70 @@
 
     Examples
     --------
     The following generates a site for spin-1/2 with Sz conservation.
     Note that ``Sx = (Sp + Sm)/2`` violates Sz conservation and is thus not a valid
     on-site operator.
 
-    >>> chinfo = npc.ChargeInfo([1], ['2*Sz'])
-    >>> ch = npc.LegCharge.from_qflat(chinfo, [1, -1])
-    >>> Sp = [[0, 1.], [0, 0]]
-    >>> Sm = [[0, 0], [1., 0]]
-    >>> Sz = [[0.5, 0], [0, -0.5]]
-    >>> site = tenpy.networks.site.Site(ch, ['up', 'down'], Splus=Sp, Sminus=Sm, Sz=Sz)
-    >>> print(site.Splus.to_ndarray())
-    [[0. 1.]
-     [0. 0.]]
-    >>> print(site.get_op('Sminus').to_ndarray())
-    [[0. 0.]
-     [1. 0.]]
-    >>> print(site.get_op('Splus Sminus').to_ndarray())
-    [[1. 0.]
-     [0. 0.]]
+    .. testsetup :: Site
+
+        from tenpy.linalg import np_conserved as npc
+        from tenpy.networks.site import Site
+
+    .. doctest :: Site
+    
+        >>> chinfo = npc.ChargeInfo([1], ['2 * Sz'])
+        >>> ch = npc.LegCharge.from_qflat(chinfo, [1, -1])
+        >>> Sp = [[0, 1.], [0, 0]]
+        >>> Sm = [[0, 0], [1., 0]]
+        >>> Sz = [[0.5, 0], [0, -0.5]]
+        >>> site = Site(ch, ['up', 'down'], Splus=Sp, Sminus=Sm, Sz=Sz)
+        >>> print(site.Splus.to_ndarray())
+        [[0. 0.]
+         [1. 0.]]
+        >>> print(site.get_op('Sminus').to_ndarray())
+        [[0. 1.]
+         [0. 0.]]
+        >>> print(site.get_op('Splus Sminus').to_ndarray())
+        [[0. 0.]
+         [0. 1.]]
+     
+    Note that sorting the charges (which happens by default!) may lead to unintuitive
+    matrix representations of the operators, because physicists are typically not used to
+    writing them in the sorted basis (in this case ``['down', 'up']``);
+
+    We get the unchanged order by setting ``sort_charges=False``. This is discouraged though,
+    as it can introduce overhead.
+
+    .. testsetup :: Site_sort_charge_False
+
+        from tenpy.linalg import np_conserved as npc
+        from tenpy.networks.site import Site
+        chinfo = npc.ChargeInfo([1], ['Sz'])
+        ch = npc.LegCharge.from_qflat(chinfo, [1, -1])
+        Sp = [[0, 1.], [0, 0]]
+        Sm = [[0, 0], [1., 0]]
+        Sz = [[0.5, 0], [0, -0.5]]
+
+    .. doctest :: Site_sort_charge_False
+
+        >>> site = Site(ch, ['up', 'down'], Splus=Sp, Sminus=Sm, Sz=Sz, sort_charge=False)
+        >>> print(site.Splus.to_ndarray())
+        [[0. 1.]
+         [0. 0.]]
+        >>> print(site.get_op('Sminus').to_ndarray())
+        [[0. 0.]
+         [1. 0.]]
+        >>> print(site.get_op('Splus Sminus').to_ndarray())
+        [[1. 0.]
+         [0. 0.]]
+
     """
 
-    def __init__(self, leg, state_labels=None, sort_charge=False, **site_ops):
+    def __init__(self, leg, state_labels=None, sort_charge=True, **site_ops):
         self.used_sort_charge = False
         self.leg = leg
         self.state_labels = dict()
         if state_labels is not None:
             for i, v in enumerate(state_labels):
                 if v is not None:
                     self.state_labels[str(v)] = i
@@ -160,25 +186,14 @@
             self.add_op(name, op)
         if 'JW' not in self.opnames:
             # include trivial `JW` to allow combinations
             # of bosonic and fermionic sites in an MPS
             self.add_op('JW', self.Id, hc='JW')
         if sort_charge:
             self.sort_charge()
-        elif sort_charge is None:
-            if not (leg.sorted and leg.bunched):
-                msg = (f"LegCharge of physical leg in site {self!s} is not sorted. "
-                       "You should explicitly set `sort_charge`. "
-                       "Set it to False, if you already have saved data for your model and want "
-                       "to be able to load it/keep backwards compatibility. "
-                       "For new projects, if you don't have data yet, set it to `True`. "
-                       "We will switch the default from False to True in version 1.0, "
-                       "which breaks compatibility of existing data with "
-                       "code/models that don't explicitly set sort_legcharge.")
-                warnings.warn(msg, FutureWarning, 2)
         self.test_sanity()
 
     def change_charge(self, new_leg_charge=None, permute=None):
         """Change the charges of the site (in place).
 
         Parameters
         ----------
@@ -805,16 +820,14 @@
     Before we can contract operators (and tensors) corresponding to different :class:`Site`
     instances, we first need to define the overall conserved charges, i.e., we need to merge the
     :class:`~tenpy.linalg.charges.ChargeInfo` of them to a single, global `chinfo` and adjust
     the charges of the physical legs. That's what this function does.
 
     A typical place to do this would be in :meth:`tenpy.models.model.CouplingMPOModel.init_sites`.
 
-    (This function replaces the now deprecated :func:`multi_sites_combine_charges`.)
-
     Parameters
     ----------
     sites : list of :class:`Site`
         The sites to be combined. The sites are modified **in place**.
     new_charges : ``'same'`` | ``'drop'`` | ``'independent'`` |  list of list of tuple
         Defines the new, common charges in terms of the old ones.
 
@@ -1127,131 +1140,14 @@
         need = need - new_charge_set
     if len(need) == 0:
         return np.array(charge_to_JW_parity, int)
     # else: couldn't partition at least with the greedy algorithm.
     return None
 
 
-def multi_sites_combine_charges(sites, same_charges=[]):
-    """Adjust the charges of the given sites (in place) such that they can be used together.
-
-    When we want to contract tensors corresponding to different :class:`Site` instances,
-    these sites need to share a single :class:`~tenpy.linalg.charges.ChargeInfo`.
-    This function adjusts the charges of these sites such that they can be used together.
-
-    .. deprecated :: 0.7.3
-        Deprecated in favor of the new, more powerful
-        :func:`~tenpy.networks.site.set_common_charges`.
-        Be aware of the slightly different argument structure though, namely that
-        this function keeps charges not included in `same_charges`, whereas you need
-        to include them explicitly into the `new_charges` argument of `set_common_charges`.
-
-
-    Parameters
-    ----------
-    sites : list of :class:`Site`
-        The sites to be combined. Modified **in place**.
-    same_charges : ``[[(int, int|str), (int, int|str), ...], ...]``
-        Defines which charges actually are the same, i.e. their quantum numbers are added up.
-        Each charge is specified by a tuple ``(s, i)= (int, int|str)``, where `s` gives the index
-        of the site within ``sites`` and `i` the index or name of the charge in the
-        :class:`~tenpy.linalg.charges.ChargeInfo` of this site.
-
-    Returns
-    -------
-    perms : list of ndarray
-        For each site the permutation performed on the physical leg to sort by charges.
-
-    Examples
-    --------
-    .. doctest :: multi_sites_combine_charges
-        :options: +NORMALIZE_WHITESPACE
-
-        >>> from tenpy.networks.site import *
-        >>> ferm = SpinHalfFermionSite(cons_N='N', cons_Sz='Sz')
-        >>> spin = SpinSite(1.0, 'Sz')
-        >>> ferm.leg.chinfo is spin.leg.chinfo
-        False
-        >>> print(spin.leg)
-         +1
-        0 [[-2]
-        1  [ 0]
-        2  [ 2]]
-        3
-        >>> multi_sites_combine_charges([ferm, spin], same_charges=[[(0, 1), (1, 0)]])
-        [array([0, 1, 2, 3]), array([0, 1, 2])]
-        >>> # no permutations where needed
-        >>> ferm.leg.chinfo is spin.leg.chinfo
-        True
-        >>> ferm.leg.chinfo.names
-        ['N', '2*Sz']
-        >>> print(spin.leg)
-         +1
-        0 [[ 0 -2]
-        1  [ 0  0]
-        2  [ 0  2]]
-        3
-    """
-    warnings.warn(
-        "multi_sites_combine_charges is deprecated! \n"
-        "Use `set_common_charges` instead, but watch out: "
-        "the argument structure is not equivalent!",
-        FutureWarning,
-        stacklevel=2)
-    # parse same_charges argument
-    same_charges = list(same_charges)  # need to modify elements...
-    same_charges_flat = []
-    for j in range(len(same_charges)):
-        same_charges_j = []
-        for s, i in same_charges[j]:
-            if isinstance(i, str):  # map string to ints
-                i = sites[s].leg.chinfo.names.index(i)
-            i = int(i)  # should be integer now...
-            same_charges_j.append((s, i))
-            same_charges_flat.append((s, i))
-        same_charges[j] = same_charges_j
-    if len(same_charges_flat) != len(set(same_charges_flat)):
-        raise ValueError("Can't have duplicates in same_charges!")
-    # find out which charges we keep
-    keep_charges = []  # list of (s, i) which appear in the new ChargeInfo
-    map_charges = {}  # dict (s, i)->(s,i): those not appearing in keep_charges to the one in it
-    for s, site in enumerate(sites):
-        for i in range(site.leg.chinfo.qnumber):
-            keep_charges.append((s, i))  # first all, remove some below
-    for same_charges_j in same_charges:
-        s0, i0 = same_charges_j[0]
-        for s, i in same_charges_j[1:]:
-            idx = keep_charges.index((s, i))
-            del keep_charges[idx]
-            map_charges[(s, i)] = (s0, i0)
-    # define common ChargeInfo class
-    qnumber = len(keep_charges)
-    names = [sites[s].leg.chinfo.names[i] for (s, i) in keep_charges]
-    mod = [sites[s].leg.chinfo.mod[i] for (s, i) in keep_charges]
-    chinfo = npc.ChargeInfo(mod, names)
-    # now define the new legs and update the charges of the sites
-    perms = []
-    for s, site in enumerate(sites):
-        old_qflat = site.leg.to_qflat()
-        new_qflat = np.zeros((site.leg.ind_len, qnumber), old_qflat.dtype)
-        for old_i in range(site.leg.chinfo.qnumber):
-            if (s, old_i) in map_charges:
-                new_i = keep_charges.index(map_charges[(s, old_i)])
-            else:
-                new_i = keep_charges.index((s, old_i))
-            new_qflat[:, new_i] = old_qflat[:, old_i]
-        # other charges are 0 = trivial
-        leg_unsorted = npc.LegCharge.from_qflat(chinfo, new_qflat, site.leg.qconj)
-        perm_qind, leg = leg_unsorted.sort()
-        perm_flat = leg_unsorted.perm_flat_from_perm_qind(perm_qind)
-        perms.append(perm_flat)
-        site.change_charge(leg, perm_flat)
-    return perms
-
-
 def kron(*ops, group=True):
     """Kronecker product of two or more local operators.
 
     Parameters
     ----------
     *ops : :class:`~tenpy.linalg.np_conserved.Array`
         Local operators with labels ``'p', 'p*'`` as defined in :class:`Site`.
@@ -1310,23 +1206,22 @@
     ----------
     conserve : str | None
         Defines what is conserved, see table above.
     sort_charge : bool
         Whether :meth:`sort_charge` should be called at the end of initialization.
         This is usually a good idea to reduce potential overhead when using charge conservation.
         Note that this permutes the order of the local basis states!
-        For backwards compatibility with existing data, it is not (yet) enabled by default.
 
     Attributes
     ----------
     conserve : str
         Defines what is conserved, see table above.
     """
 
-    def __init__(self, conserve='Sz', sort_charge=None):
+    def __init__(self, conserve='Sz', sort_charge=True):
         if not conserve:
             conserve = 'None'
         if conserve not in ['Sz', 'parity', 'None']:
             raise ValueError("invalid `conserve`: " + repr(conserve))
         Sx = [[0., 0.5], [0.5, 0.]]
         Sy = [[0., -0.5j], [+0.5j, 0.]]
         Sz = [[0.5, 0.], [0., -0.5]]
@@ -1391,25 +1286,24 @@
     ----------
     conserve : str
         Defines what is conserved, see table above.
     sort_charge : bool
         Whether :meth:`sort_charge` should be called at the end of initialization.
         This is usually a good idea to reduce potential overhead when using charge conservation.
         Note that this permutes the order of the local basis states for ``conserve='parity'``!
-        For backwards compatibility with existing data, it is not (yet) enabled by default.
 
     Attributes
     ----------
     S : {0.5, 1, 1.5, 2, ...}
         The 2S+1 states range from m = -S, -S+1, ... +S.
     conserve : str
         Defines what is conserved, see table above.
     """
 
-    def __init__(self, S=0.5, conserve='Sz', sort_charge=None):
+    def __init__(self, S=0.5, conserve='Sz', sort_charge=True):
         if not conserve:
             conserve = 'None'
         if conserve not in ['Sz', 'parity', 'None']:
             raise ValueError("invalid `conserve`: " + repr(conserve))
         self.S = S = float(S)
         d = 2 * S + 1
         if d <= 1:
@@ -2074,24 +1968,23 @@
         Number of states per site
     conserve : str | None
         Defines what is conserved, see table above.
     sort_charge : bool
         Whether :meth:`sort_charge` should be called at the end of initialization.
         This is usually a good idea to reduce potential overhead when using charge conservation.
         Note that this permutes the order of the local basis states!
-        For backwards compatibility with existing data, it is not (yet) enabled by default.
 
     Attributes
     ----------
     q : int
         Number of states per site
     conserve : str
         Defines what is conserved, see table above.
     """
-    def __init__(self, q, conserve='Z', sort_charge=None):
+    def __init__(self, q, conserve='Z', sort_charge=True):
         if not (isinstance(q, int) and q > 1):
             raise ValueError(f'invalid q: {q}')
         self.q = q
         if not conserve:
             conserve = 'None'
         if conserve not in ['Z', 'None']:
             raise ValueError("invalid `conserve`: " + repr(conserve))
```

### Comparing `physics-tenpy-0.99.0/tenpy/networks/terms.py` & `physics-tenpy-1.0.0/tenpy/networks/terms.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/networks/uniform_mps.py` & `physics-tenpy-1.0.0/tenpy/networks/uniform_mps.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/simulations/__init__.py` & `physics-tenpy-1.0.0/tenpy/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/simulations/ground_state_search.py` & `physics-tenpy-1.0.0/tenpy/simulations/ground_state_search.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/simulations/measurement.py` & `physics-tenpy-1.0.0/tenpy/simulations/measurement.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 from ..networks.mpo import MPOEnvironment
 from ..tools.misc import get_recursive
 
 __all__ = [
     'measurement_wrapper', 'm_measurement_index', 'm_bond_dimension', 'm_bond_energies',
     'm_simulation_parameter', 'm_energy_MPO', 'm_entropy', 'm_onsite_expectation_value',
     'm_correlation_length', 'm_evolved_time',
-    'measurement_index', 'bond_dimension', 'bond_energies', 'simulation_parameter', 'energy_MPO',
-    'entropy', 'onsite_expectation_value', 'correlation_length',  'evolved_time', 'psi_method',
 ]
 
 
 def measurement_wrapper(function, results_key, **kwargs):
     """Decorator to transform a function into a measurement function.
 
     As documented in :func:`m_measurement_index`, measurement functions need to take
@@ -267,73 +265,14 @@
     ----------
     results, psi, model, simulation, results_key:
         See :func:`~tenpy.simulation.measurement.measurement_index`.
     """
     results[results_key] = simulation.engine.evolved_time
 
 
-def psi_method(results, psi, model, simulation, method, key=None, **kwargs):
-    """Generic function to measure arbitrary method of psi with given additional kwargs.
-
-    .. deprecated :: 0.10.0
-
-        Instead of using this function :func:`tenpy.simulations.measurement.psi_method`
-        as a global measurement wrapper function, you can now directly use "psi_method"
-        as `module_name` and replace the `connect_measurements` simulation parameter
-        entries as follows::
-
-            An old python entry for connect_measurements
-                ['tenpy.simulations.measurement',
-                 'psi_method',
-                 {'method': 'correlation_function',
-                  'key': '<Sp_i Sm_j>',
-                  'ops1': 'Sp',
-                  'ops2': 'Sm'}]
-            can get replaced with new entry:
-                ['psi_method',
-                 'wrap correlation_function',
-                 {'results_key': '<Sp_i Sm_j>',
-                  'ops1': 'Sp',
-                  'ops2': 'Sm'}]
-            Similarly, an old yaml entry for connect_measurements
-                - - tenpy.simulations.measurement
-                  - psi_method
-                  - method: correlation_function
-                    key: '<Sp_i Sm_j>'
-                    ops1: Sp
-                    ops2: Sm
-            can get replaced with new yaml:
-                - - psi_method
-                  - wrap correlation_function
-                  - results_key: '<Sp_i Sm_j>'
-                    ops1: Sp
-                    ops2: Sm
-
-        The new way is now the preferred way of measuring psi methods, the old way is deprecated.
-        Note the additional "wrap " in the function name, which indicates that the specified
-        function just returns the results and does not take ``results, model, simulation`` as
-        arguments, hence we need a wrapper function for the measurement.
-        Also note the renaming of `key` to `results_key`.
-
-    Parameters
-    ----------
-    results, psi, model, simulation, key:
-        See :func:`~tenpy.simulation.measurement.measurement_index`.
-    method : str
-        Name of the method of `psi` to call. `key` defaults to this if not specified.
-    **kwargs :
-        further keyword arguments given to the method
-    """
-    # extract the deprecation comment from the doc string
-    _psi_method_deprecated_msg = '\n'.join([line[8:] for line in
-                                            psi_method.__doc__.splitlines()[4:42]])
-    warnings.warn(_psi_method_deprecated_msg, FutureWarning)
-    _m_psi_method_wrapped(results, psi, model, simulation, method, results_key=key, **kwargs)
-
-
 # the following wrapper functions _m_{psi,model}_method_[wrapped] are used
 # in simulation._connect_measurement_fct  for entries with 'psi_method' and 'model_method' in
 # :cfg:option:`Simulation.connect_measurement`
 
 def _m_psi_method(results, psi, model, simulation, func_name, **kwargs):
     psi_method = getattr(psi, func_name)
     psi_method(results, model, simulation, **kwargs)
@@ -358,68 +297,7 @@
     if results_key in results:
         raise ValueError(f"key {results_key!r} already exists in `results`, "
                          "measurement would overwrite data. "
                          "Probably a measurement function used multiple times!")
     model_method = getattr(model, func_name)
     res = model_method(**kwargs)
     results[results_key] = res
-
-
-# Deprecated functions
-_deprecated_msg = ("renamed function and argument {0:s}(..., key) to m_{0:s}(..., results_key), "
-                   "update corresponding entry in simulation parameter `connect_measurements`!")
-
-
-def measurement_index(results, psi, model, simulation, key='measurement_index'):
-    """Deprecated version of :func:`m_measurement_index`."""
-    warnings.warn(_deprecated_msg.format("measurement_index"), FutureWarning)
-    m_measurement_index(results, psi, model, simulation, key)
-
-
-def bond_dimension(results, psi, model, simulation, key='bond_dimension'):
-    """Deprecated version of :func:`m_bond_dimension`."""
-    warnings.warn(_deprecated_msg.format("bond_dimension"), FutureWarning)
-    m_bond_dimension(results, psi, model, simulation, key)
-
-
-def bond_energies(results, psi, model, simulation, key='bond_energies'):
-    """Deprecated version of :func:`m_bond_energies`."""
-    warnings.warn(_deprecated_msg.format("bond_energies"), FutureWarning)
-    m_bond_dimension(results, psi, model, simulation, key)
-
-
-def simulation_parameter(results, psi, model, simulation, recursive_key, key=None, **kwargs):
-    """Deprecated version of :func:`m_simulation_parameter`."""
-    warnings.warn(_deprecated_msg.format("simulation_parameter"), FutureWarning)
-    m_simulation_parameter(results, psi, model, simulation, recursive_key, key, **kwargs)
-
-
-def energy_MPO(results, psi, model, simulation, key='energy_MPO'):
-    """Deprecated version of :func:`m_energy_MPO`."""
-    warnings.warn(_deprecated_msg.format("energy_MPO"), FutureWarning)
-    m_energy_MPO(results, psi, model, simulation, key)
-
-
-def entropy(results, psi, model, simulation, key='entropy'):
-    """Deprecated version of :func:`m_entropy`."""
-    warnings.warn(_deprecated_msg.format("entropy"), FutureWarning)
-    m_entropy(results, psi, model, simulation, key)
-
-
-def onsite_expectation_value(results, psi, model, simulation, opname, key=None, fix_u=None,
-                             **kwargs):
-    """Deprecated version of :func:`m_onsite_expectation_value`."""
-    warnings.warn(_deprecated_msg.format("onsite_expectation_value"), FutureWarning)
-    m_onsite_expectation_value(results, psi, model, simulation, opname, key, fix_u, **kwargs)
-
-
-def correlation_length(results, psi, model, simulation, key='correlation_length', unit=None,
-                       **kwargs):
-    """Deprecated version of :func:`m_correlation_length`."""
-    warnings.warn(_deprecated_msg.format("correlation_length"), FutureWarning)
-    m_correlation_length(results, psi, model, simulation, key, unit, **kwargs)
-
-
-def evolved_time(results, psi, model, simulation, key='evolved_time'):
-    """Deprecated version of :func:`m_evolved_time`."""
-    warnings.warn(_deprecated_msg.format("evolved_time"), FutureWarning)
-    m_evolved_time(results, psi, model, simulation, key)
```

### Comparing `physics-tenpy-0.99.0/tenpy/simulations/post_processing.py` & `physics-tenpy-1.0.0/tenpy/simulations/post_processing.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/simulations/simulation.py` & `physics-tenpy-1.0.0/tenpy/simulations/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,27 +197,21 @@
         if cwd is not None:
             if not os.path.exists(cwd):
                 os.mkdir(cwd)
             os.chdir(cwd)
         self.fix_output_filenames()
         if setup_logging:
             log_params = self.options.setdefault('log_params', {})
-            if 'logging_params' in self.options:
-                # when you remove this if clause, also clean up the 'logging_params' from the
-                # self.options.touch(..., 'logging_params') below
-                warnings.warn("Renamed `logging_params` to `log_params` for simulation.",
-                              FutureWarning, 2)
-                log_params = self.options['logging_params']
             setup_logging_(**log_params, output_filename=self.output_filename)
         # now that we have logging running, catch up with log messages
         self.logger.info("new simulation\n%s\n%s\n%s", "=" * 80, self.__class__.__name__, "=" * 80)
         self.options = asConfig(self.options, self.__class__.__name__)
         self.options.touch('directory', 'output_filename', 'output_filename_params',
                            'overwrite_output', 'skip_if_output_exists', 'safe_write', 'log_params',
-                           'logging_params', 'estimate_RAM_const_offset')
+                           'estimate_RAM_const_offset')
         if cwd is not None:
             self.logger.info("change directory to %s", cwd)  # os.chdir(cwd) above
         self.logger.info("output filename: %s", self.output_filename)
 
         random_seed = self.options.get('random_seed', None)
         if random_seed is not None:
             if self.loaded_from_checkpoint:
@@ -254,21 +248,14 @@
     def __exit__(self, exc_type, exc_value, traceback):
         self.cache.__exit__(exc_type, exc_value, traceback)  # exit cache context
         if exc_type is not None:
             self.logger.exception("simulation abort with the following exception",
                                   exc_info=(exc_type, exc_value, traceback))
         self.options.warn_unused(True)
 
-    @property
-    def verbose(self):
-        warnings.warn(
-            "verbose is deprecated, we're using logging now! \n"
-            "See https://tenpy.readthedocs.io/en/latest/intro/logging.html", FutureWarning, 2)
-        return self.options.get('verbose', 1.)
-
     def estimate_RAM(self):
         """Estimates the RAM usage for the simulation, without running it.
 
         Returns
         -------
         RAM : int
             The expected RAM usage in kB.
@@ -1161,17 +1148,14 @@
     """
     def __init__(self, msg, filename):
         filename = str(filename)
         super().__init__(msg + '\n' + filename)
         self.filename = filename
 
 
-_deprecated_not_set = object()
-
-
 def init_simulation(simulation_class='GroundStateSearch',
                     simulation_class_kwargs=None,
                     **simulation_params):
     """Run the simulation with a simulation class.
 
     If you need to run the simulation, you can use a `with` statement for proper context
     management::
@@ -1201,22 +1185,17 @@
         simulation_class_kwargs = {}
     sim = SimClass(simulation_params, **simulation_class_kwargs)
     return sim
 
 
 def run_simulation(simulation_class='GroundStateSearch',
                    simulation_class_kwargs=None,
-                   *,
-                   simulation_class_name=_deprecated_not_set,
                    **simulation_params):
     """Run the simulation with a simulation class.
 
-    .. deprecated :: 0.9.0
-        The `simulation_class_name` argument has been renamed to just `simulation_class`.
-
     Parameters
     ----------
     simulation_class : str
         The name of a (sub)class of :class:`~tenpy.simulations.simulations.Simulation`
         to be used for running the simulation.
     simulation_class_kwargs : dict | None
         A dictionary of keyword-arguments to be used for the initializing the simulation.
@@ -1226,20 +1205,14 @@
 
     Returns
     -------
     results : dict
         The results of the Simulation, i.e., what
         :meth:`~tenpy.simulations.simulation.Simulation.run()` returned.
     """
-    if simulation_class_name is not _deprecated_not_set:
-        assert simulation_class == 'GroundStateSearch'
-        warnings.warn(
-            "The `simulation_class_name` argument has been renamed to `simulation_class`"
-            " for more consistency with remaining parameters.", FutureWarning)
-        simulation_class = simulation_class_name
     sim = init_simulation(simulation_class, simulation_class_kwargs, **simulation_params)
     with sim:
         results = sim.run()
     return results
 
 
 def init_simulation_from_checkpoint(*,
@@ -1374,15 +1347,14 @@
     return results
 
 
 def run_seq_simulations(sequential,
                         simulation_class='GroundStateSearch',
                         simulation_class_kwargs=None,
                         *,
-                        simulation_class_name=_deprecated_not_set,
                         resume_data=None,
                         collect_results_in_memory=False,
                         **simulation_params):
     """Sequentially run (variational) simulations.
 
     Uses the results (in particular the state) from one simulation to initialize another one.
     This allows to "adiabatically" or "smoothly" follow the evolution of the ground state as
@@ -1464,21 +1436,14 @@
         for k in recursive_keys:
             # goal of sequential simulation: keep the initial state from previous simulation!
             for check in ['initial_state', 'output_filename_params']:
                 assert not k.startswith(check), "really?!?"
     else:
         N_sims = 1
 
-    if simulation_class_name is not _deprecated_not_set:
-        assert simulation_class == 'GroundStateSearch'
-        warnings.warn(
-            "The `simulation_class_name` argument has been renamed to `simulation_class`"
-            " for more consistency with remaining parameters.", FutureWarning)
-        simulation_class = simulation_class_name
-
     SimClass = find_subclass(Simulation, simulation_class)
     if simulation_class_kwargs is None:
         simulation_class_kwargs = {}
 
     # try to create varying output filenames
     # do we save to file at all?
     if simulation_params.get('output_filename', None) is not None or \
```

### Comparing `physics-tenpy-0.99.0/tenpy/simulations/time_evolution.py` & `physics-tenpy-1.0.0/tenpy/simulations/time_evolution.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/__init__.py` & `physics-tenpy-1.0.0/tenpy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/cache.py` & `physics-tenpy-1.0.0/tenpy/tools/cache.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/events.py` & `physics-tenpy-1.0.0/tenpy/tools/events.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/fit.py` & `physics-tenpy-1.0.0/tenpy/tools/fit.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/hdf5_io.py` & `physics-tenpy-1.0.0/tenpy/tools/hdf5_io.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/math.py` & `physics-tenpy-1.0.0/tenpy/tools/math.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/misc.py` & `physics-tenpy-1.0.0/tenpy/tools/misc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """Miscellaneous tools, somewhat random mix yet often helpful."""
 # Copyright (C) TeNPy Developers, GNU GPLv3
 
 import operator
 import numpy as np
 from .optimization import bottleneck
-from .process import omp_set_nthreads
 from .params import Config
 from collections.abc import Mapping
 import os.path
-import argparse
 import warnings
 
 __all__ = [
     'to_iterable', 'to_iterable_of_len', 'to_array', 'anynan', 'argsort', 'lexsort',
     'inverse_permutation', 'list_to_dict_list', 'atleast_2d_pad', 'transpose_list_list',
-    'zero_if_close', 'pad', 'any_nonzero', 'add_with_None_0', 'chi_list', 'group_by_degeneracy',
-    'get_close', 'find_subclass', 'get_recursive', 'set_recursive', 'update_recursive',
-    'merge_recursive', 'flatten', 'setup_logging', 'build_initial_state', 'setup_executable',
-    'convert_memory_units', 'consistency_check', 'TenpyInconsistencyError',
-    'TenpyInconsistencyWarning', 'BetaWarning'
+    'zero_if_close', 'pad', 'add_with_None_0', 'group_by_degeneracy', 'get_close',
+    'find_subclass', 'get_recursive', 'set_recursive', 'update_recursive', 'merge_recursive',
+    'flatten', 'setup_logging', 'convert_memory_units', 'consistency_check',
+    'TenpyInconsistencyError', 'TenpyInconsistencyWarning', 'BetaWarning'
 ]
 
 _not_set = object()  # sentinel
 
 def to_iterable(a):
     """If `a` is a not iterable or a string, return ``[a]``, else return ``a``."""
     if type(a) == str:
@@ -361,65 +358,14 @@
     b[tuple(take)] = a
     # append
     take[axis] = slice(-w_r, None)
     b[tuple(take)] = v_r
     return b
 
 
-def any_nonzero(params, keys, verbose_msg=None):
-    """Check for any non-zero or non-equal entries in some parameters.
-
-    .. deprecated :: 0.8.0
-        This method will be removed in version 1.0.0.
-        Use :meth:`tenpy.tools.params.Config.any_nonzero` instead.
-
-    Parameters
-    ----------
-    params : dict | Config
-        A dictionary of parameters, or a :class:`~tenpy.tools.params.Config`
-        instance.
-    keys : list of {key | tuple of keys}
-        For a single key, check ``params[key]`` for non-zero entries.
-        For a tuple of keys, all the ``params[key]`` have to be equal (as numpy arrays).
-    verbose_msg : None | str
-        If params['verbose'] >= 1, we print `verbose_msg` before checking,
-        and a short notice with the `key`, if a non-zero entry is found.
-
-    Returns
-    -------
-    match : bool
-        False, if all params[key] are zero or `None` and
-        True, if any of the params[key] for single `key` in `keys`,
-        or if any of the entries for a tuple of `keys`
-    """
-    msg = ("tools.misc.any_nonzero() is deprecated in favor of "
-           "tools.params.Config.any_nonzero().")
-    warnings.warn(msg, category=FutureWarning, stacklevel=2)
-    if isinstance(params, Config):
-        return params.any_nonzero(keys, verbose_msg)
-    verbose = (params.get('verbose', 0) > 1.)
-    for k in keys:
-        if isinstance(k, tuple):
-            # check equality
-            val = params.get(k[0], None)
-            for k1 in k[1:]:
-                if not np.array_equal(val, params.get(k1, None)):
-                    if verbose:
-                        print("{k0!r} and {k1!r} have different entries.".format(k0=k[0], k1=k1))
-                    return True
-        else:
-            val = params.get(k, None)
-            if val is not None and np.any(np.array(val) != 0.):  # count `None` as zero
-                if verbose:
-                    print(verbose_msg)
-                    print(str(k) + " has nonzero entries")
-                return True
-    return False
-
-
 def add_with_None_0(a, b):
     """Return ``a + b``, treating `None` as zero.
 
     Parameters
     ----------
     a, b :
         The two things to be added, or ``None``.
@@ -432,27 +378,14 @@
     if a is None:
         return b
     if b is None:
         return a
     return a + b
 
 
-def chi_list(chi_max, dchi=20, nsweeps=20, verbose=0):
-    warnings.warn("Deprecated: moved `chi_list` to `tenpy.algorithms.dmrg.chi_list`.",
-                  category=FutureWarning,
-                  stacklevel=2)
-    from tenpy.algorithms import dmrg
-    chi_list = dmrg.chi_list(chi_max, dchi, nsweeps)
-    if verbose:
-        import pprint
-        print("chi_list = ")
-        pprint.pprint(chi_list)
-    return chi_list
-
-
 def group_by_degeneracy(E, *args, subset=None, cutoff=1.e-12):
     """Find groups of indices for which (energy) values are degenerate.
 
     Parameters
     ----------
     values : 1D array
         Values (e.g. energies) which need to be close to count as degenerate.
@@ -753,16 +686,15 @@
     return result
 
 
 #: default value for :cfg:option:`log.skip_setup`
 skip_logging_setup = False
 
 
-def setup_logging(options=None,
-                  output_filename=None,
+def setup_logging(output_filename=None,
                   *,
                   filename=_not_set,
                   to_stdout="INFO",
                   to_file="INFO",
                   format="%(levelname)-8s: %(message)s",
                   datefmt=None,
                   logger_levels={},
@@ -803,25 +735,21 @@
 
     .. note ::
         We **remove** any previously configured logging handlers.
         This is to handle the case when this function is called multiple times,
         e.g., because you run multiple :class:`~tenpy.simulations.simulation.Simulation`
         classes sequentially (e.g., :func:`~tenpy.simulations.simulation.run_seq_simulations`).
 
-    .. deprecated :: 0.9.0
-        The arguments were previously collected in a dictionary `options`.
-        Now they should be given directly as keyword arguments.
-
     Parameters
     ----------
-    **kwargs :
-        Keyword arguments as described in the options below.
     output_filename : None | str
         The filename for where results are saved. The :cfg:option:`log.filename` for the
         log-file defaults to this, but replacing the extension with ``.log``.
+    **kwargs :
+        Keyword arguments as described in the options below.
 
     Options
     -------
     .. cfg:config :: log
 
         skip_setup: bool
             If True, don't change anything in the logging setup; just return.
@@ -859,17 +787,14 @@
         dict_config : dict
             Alternatively, a full configuration dictionary for :func:`logging.config.dictConfig`.
             If used, all other options except `skip_setup` and `capture_warnings` are ignored.
         capture_warnings : bool
             Whether to call :func:`logging.captureWarnings` to include the warnings into the log.
     """
     import logging.config
-    if options is not None:
-        warnings.warn("Give logging parameters directly as keyword arguments!", FutureWarning, 2)
-        locals().update(**options)
     if filename is _not_set:
         if output_filename is not None:
             root, ext = os.path.splitext(output_filename)
             assert ext != '.log'
             filename = root + '.log'
         else:
             filename = None
@@ -932,198 +857,14 @@
         dict_config.setdefault('disable_existing_loggers', False)
     # note: dictConfig cleans up previously existing handlers etc
     logging.config.dictConfig(dict_config)
     if capture_warnings:
         logging.captureWarnings(True)
 
 
-def build_initial_state(size, states, filling, mode='random', seed=None):
-    warnings.warn(
-        "Deprecated `build_initial_state`: Use `tenpy.networks.mps.InitialStateBuilder` instead.",
-        category=FutureWarning,
-        stacklevel=2)
-    from tenpy.networks import mps
-    return mps.build_initial_state(size, states, filling, mode, seed)
-
-
-def setup_executable(mod, run_defaults, identifier_list=None):
-    """Read command line arguments and turn into useable dicts.
-
-    .. warning ::
-
-        this is a deprecated interface. Use the :class:`~tenpy.simulations.simulation.Simulation`
-        interface in combination with :func:`~tenpy.console_main` instead.
-        You can invoke that from the command line as ``python -m tenpy ...``.
-
-    Uses default values defined at:
-    - model class for model_par
-    - here for sim_par
-    - executable file for run_par
-    Alternatively, a model_defaults dictionary and identifier_list can be supplied without the model
-
-    NB: for setup_executable to work with a model class, the model class needs to define two things:
-            - defaults, a static (class level) dictionary with (key, value) pairs that have the name
-              of the parameter (as string) as key, and the default value as value.
-            - identifier, a static (class level) list or other iterable with the names of the parameters
-              to be used in filename identifiers.
-
-    Parameters
-    ----------
-    mod : model | dict
-        Model class (or instance) OR a dictionary containing model defaults
-    run_defaults : dict
-        default values for executable file parameters
-    identifier_list : iterable
-        Used only if mod is a dict. Contains the identifier variables
-
-    Returns
-    -------
-    model_par, sim_par, run_par : dict
-        containing all parameters.
-    args :
-        namespace with raw arguments for some backwards compatibility with executables.
-    """
-    warnings.warn("Deprecated: use `tenpy.run_simulation` and `tenpy.console_main` instead.",
-                  category=FutureWarning,
-                  stacklevel=2)
-    parser = argparse.ArgumentParser()
-
-    # These deal with backwards compatibility (supplying a model)
-    if type(mod) != dict and identifier_list == None:  # Assume we've been given a model class
-        try:
-            model_defaults = mod.defaults
-            identifier_list = mod.identifier
-        except AttributeError as err:
-            print("Cannot get model defaults and identifier list from mod. Is mod a class/instance?")
-            print(err)
-            raise AttributeError
-    elif type(mod) == dict and hasattr(identifier_list, '__iter__'):
-        model_defaults = mod
-    else:
-        raise ValueError("If model_par are supplied as dict, identifier_list should be provided.")
-
-    # The model_par bit (for all model parameters)
-    for label, value in model_defaults.items():
-        if type(value) == bool:  # For boolean defaults, we want a true/false flag
-            if value:
-                parser.add_argument('-' + label, action='store_false')
-            else:
-                parser.add_argument('-' + label, action='store_true')
-        else:  # For non-boolean defaults, take the type of the default as type for the cmdline var
-            parser.add_argument('-' + label, type=type(value), default=value)
-
-    # The run_par bit (for executable-level parameters). These are defined in the executable file
-    # but need to be included for argparse to work correctly.
-    for label, value in run_defaults.items():
-        if type(value) == bool:  # For boolean defaults, we want a true/false flag
-            if value:
-                parser.add_argument('-' + label, action='store_false')
-            else:
-                parser.add_argument('-' + label, action='store_true')
-        else:  # For non-boolean defaults, take the type of the default as type for the cmdline var
-            print('Adding argument', label)
-            parser.add_argument('-' + label, type=type(value), default=value)
-    # The following parameters are run-time but so general they're defined here
-    parser.add_argument('-ncores', type=int, default=1)
-    parser.add_argument('-dir', type=str, default=None)
-    parser.add_argument('-plots', action='store_true')  # Generic flag to activate plotting
-    parser.add_argument('-seed', default=None)  # For anything random
-
-    # The sim_par bit (for DMRG-related parameters). These don't vary, so we'll just define here.
-    parser.add_argument('-chi', type=int, default=100)
-    parser.add_argument('-dchi', type=int, default=20)  # Step size for chi ramp
-    parser.add_argument('-dsweeps', type=int, default=20)  # Number of sweeps for chi step
-    parser.add_argument('-min_sweeps', type=int, default=30)
-    parser.add_argument('-max_sweeps', type=int, default=1000)
-    #parser.add_argument('-n_steps', type=int, default=10)
-    #parser.add_argument('-max_steps', type=int, default=2400)
-    parser.add_argument('-mixer', action='store_true')  # To activate mixer
-    parser.add_argument('-mix_str', type=float, default=1.e-3)
-    parser.add_argument('-mix_dec', type=float, default=1.5)
-    parser.add_argument('-mix_len', type=int, default=80)
-    parser.add_argument('-start_env', type=int, default=0)
-    parser.add_argument('-update_env', type=int)
-
-    # Now parse and turn into manageable dicts.
-    args = parser.parse_args()
-    par_dict = vars(args)  # Turns args (='Namespace' object) into dict.
-
-    model_par = {}
-    for label in model_defaults.keys():  # Select the model-relevant parts of par_dict
-        model_par[label] = par_dict[label]
-
-    run_par = {}
-    for label in run_defaults.keys():  # Select the executable-relevant parts of par_dict
-        run_par[label] = par_dict[label]
-
-    try:
-        sim_par = {
-            'chi_list': chi_list(args.chi, args.dchi, args.dsweeps),
-            'N_sweeps_check': 10,
-            'min_sweeps': args.min_sweeps,
-            'max_sweeps': args.max_sweeps,
-            'verbose': args.verbose,  # Take this from the model
-            'lanczos_params': {
-                'N_min': 2,
-                'N_max': 40,
-                'E_tol': 10**(-12)
-            }
-        }
-    except AttributeError as err:
-        print(
-            'sim_par parsing has failed, most likely because model does not define verbose parameter.'
-        )
-        print(err)
-        raise AttributeError
-    if args.mixer:
-        sim_par['mixer'] = True
-        sim_par['mixer_params'] = {
-            'amplitude': args.mix_str,
-            'decay': args.mix_dec,
-            'disable_after': args.mix_len
-        }
-
-    # Having set up all dictionaries, we can now do some other setting up
-    omp_set_nthreads(args.ncores)
-    if not args.dir == None:
-        os.chdir(args.dir)
-    import matplotlib
-    matplotlib.rcParams["savefig.directory"] = os.chdir(os.getcwd())
-
-    # Build the identifier based on model-defined and general parameters
-    identifier = "chi_{}_seed_{}_".format(args.chi, args.seed)  # Only use seed if supplied?
-    for varname in identifier_list:
-        if 'conserve' in varname:
-            shortened = varname.replace('conserve',
-                                        'cons').replace('number',
-                                                        'num').replace('charge',
-                                                                       'ch').replace('spin', 'S')
-            identifier += shortened + "_"
-        elif model_par[varname] != 0:  # Parameters that are 0 are ignored. Only want supplied?
-            identifier += varname + "_" + str(model_par[varname]) + "_"
-    if args.mixer:
-        identifier += 'mix_({},{},{})'.format(args.mix_str, args.mix_dec, args.mix_len)
-    if identifier[-1] == "_":
-        identifier = identifier[:-1]
-    # Attempt to shorten the identifier
-    identifier = identifier.replace('periodic', 'inf').replace('finite', 'fin').replace('.0_', '_')
-    if len(identifier) >= 144:
-        print("Warning: identifier has a length longer than max filename on encrypted Ubuntu!")
-
-    run_par.update({
-        'ncores': args.ncores,
-        'dir': args.dir,
-        'plots': args.plots,
-        'identifier': identifier,
-        'seed': args.seed,
-    })
-
-    return model_par, sim_par, run_par, args
-
-
 def convert_memory_units(value, unit_from='bytes', unit_to=None):
     """Convert between different memory units.
 
     Parameters
     ----------
     value : float
         The value to convert.
```

### Comparing `physics-tenpy-0.99.0/tenpy/tools/optimization.py` & `physics-tenpy-1.0.0/tenpy/tools/optimization.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/prediction.py` & `physics-tenpy-1.0.0/tenpy/tools/prediction.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/process.py` & `physics-tenpy-1.0.0/tenpy/tools/process.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/spectral_function_tools.py` & `physics-tenpy-1.0.0/tenpy/tools/spectral_function_tools.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/string.py` & `physics-tenpy-1.0.0/tenpy/tools/string.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/tools/thread.py` & `physics-tenpy-1.0.0/tenpy/tools/thread.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tenpy/version.py` & `physics-tenpy-1.0.0/tenpy/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __all__ = [
     "version", "released", "short_version", "git_revision", "full_version", "version_summary"
 ]
 
 # hard-coded version for people without git...
 #: current release version as a string
-version = '0.99.0'
+version = '1.0.0'
 
 #: whether this is a released version or modified
 released = True
 
 #: same as version, but with 'v' in front
 short_version = 'v' + version
```

### Comparing `physics-tenpy-0.99.0/tests/benchmark/benchmark.py` & `physics-tenpy-1.0.0/tests/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/benchmark/combine_npc.py` & `physics-tenpy-1.0.0/tests/benchmark/combine_npc.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/benchmark/combine_numpy.py` & `physics-tenpy-1.0.0/tests/benchmark/combine_numpy.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/benchmark/dmrg_infinite.py` & `physics-tenpy-1.0.0/tests/benchmark/dmrg_infinite.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/benchmark/profiling.py` & `physics-tenpy-1.0.0/tests/benchmark/profiling.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/benchmark/singlerun.py` & `physics-tenpy-1.0.0/tests/benchmark/singlerun.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/benchmark/split_npc.py` & `physics-tenpy-1.0.0/tests/benchmark/split_npc.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/benchmark/split_numpy.py` & `physics-tenpy-1.0.0/tests/benchmark/split_numpy.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/benchmark/tebd_infinite.py` & `physics-tenpy-1.0.0/tests/benchmark/tebd_infinite.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/benchmark/tensordot_npc.py` & `physics-tenpy-1.0.0/tests/benchmark/tensordot_npc.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/export_import_test/io_test.py` & `physics-tenpy-1.0.0/tests/export_import_test/io_test.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/export_import_test/test_cache.py` & `physics-tenpy-1.0.0/tests/export_import_test/test_cache.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/export_import_test/test_hdf5.py` & `physics-tenpy-1.0.0/tests/export_import_test/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/export_import_test/test_pickle.py` & `physics-tenpy-1.0.0/tests/export_import_test/test_pickle.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/linting.py` & `physics-tenpy-1.0.0/tests/linting.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/random_test.py` & `physics-tenpy-1.0.0/tests/random_test.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/tdvp_numpy.py` & `physics-tenpy-1.0.0/tests/tdvp_numpy.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_charges.py` & `physics-tenpy-1.0.0/tests/test_charges.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_dmrg.py` & `physics-tenpy-1.0.0/tests/test_dmrg.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_exact_diag.py` & `physics-tenpy-1.0.0/tests/test_exact_diag.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_examples.py` & `physics-tenpy-1.0.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_krylov_based.py` & `physics-tenpy-1.0.0/tests/test_krylov_based.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_lattice.py` & `physics-tenpy-1.0.0/tests/test_lattice.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model.py` & `physics-tenpy-1.0.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_aklt.py` & `physics-tenpy-1.0.0/tests/test_model_aklt.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_clock.py` & `physics-tenpy-1.0.0/tests/test_model_clock.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_fermions_spinless.py` & `physics-tenpy-1.0.0/tests/test_model_fermions_spinless.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_haldane.py` & `physics-tenpy-1.0.0/tests/test_model_haldane.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_hofstadter.py` & `physics-tenpy-1.0.0/tests/test_model_hofstadter.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_hubbard.py` & `physics-tenpy-1.0.0/tests/test_model_hubbard.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_mixed_xk.py` & `physics-tenpy-1.0.0/tests/test_model_mixed_xk.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_spins.py` & `physics-tenpy-1.0.0/tests/test_model_spins.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_spins_nnn.py` & `physics-tenpy-1.0.0/tests/test_model_spins_nnn.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_tf_ising.py` & `physics-tenpy-1.0.0/tests/test_model_tf_ising.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_toric_code.py` & `physics-tenpy-1.0.0/tests/test_model_toric_code.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_model_xxz_chain.py` & `physics-tenpy-1.0.0/tests/test_model_xxz_chain.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_mpo.py` & `physics-tenpy-1.0.0/tests/test_mpo.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_mps.py` & `physics-tenpy-1.0.0/tests/test_mps.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,26 +378,21 @@
     s2 = 0.5**0.5
     assert np.linalg.norm(th - [0., s2, 0., 0., -s2, 0., 0, 0.]) < eps
     psi2.apply_product_op(['Sigmax', 'Sm', 'Sigmax'])
     th = psi2.get_theta(0, 3).to_ndarray().reshape((8, ))
     assert np.linalg.norm(th - [0., 0., 0., -s2, 0., 0., s2, 0.]) < eps
 
 
-@pytest.mark.filterwarnings('ignore::FutureWarning')
 def test_enlarge_mps_unit_cell():
     s = site.SpinHalfSite(conserve='Sz', sort_charge=True)
     psi = mps.MPS.from_product_state([s] * 3, ['up', 'down', 'up'], bc='infinite')
-    psi0 = psi.copy()
-    psi1 = psi.copy()
-    psi0.increase_L(9)
-    psi1.enlarge_mps_unit_cell(3)
-    for psi in [psi0, psi1]:
-        psi.test_sanity()
-        expval = psi.expectation_value('Sigmaz')
-        npt.assert_equal(expval, [1., -1., 1.] * 3)
+    psi.enlarge_mps_unit_cell(3)
+    psi.test_sanity()
+    expval = psi.expectation_value('Sigmaz')
+    npt.assert_equal(expval, [1., -1., 1.] * 3)
     # done
 
 
 def test_roll_mps_unit_cell():
     s = site.SpinHalfSite(conserve='Sz', sort_charge=True)
     psi = mps.MPS.from_product_state([s] * 4, ['down', 'up', 'up', 'up'], bc='infinite')
     psi1 = psi.copy()
```

### Comparing `physics-tenpy-0.99.0/tests/test_network_contractor.py` & `physics-tenpy-1.0.0/tests/test_network_contractor.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_np_conserved.py` & `physics-tenpy-1.0.0/tests/test_np_conserved.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Copyright (C) TeNPy Developers, GNU GPLv3
 
 import tenpy.linalg.np_conserved as npc
 import numpy as np
 import numpy.testing as npt
 import itertools as it
 from tenpy.tools.misc import inverse_permutation
-import pytest
 
 from random_test import gen_random_legcharge, random_Array
 
 chinfo = npc.ChargeInfo([1, 2], ['number', 'parity'])
 # parity can be derived from number. Yet, this should all work...
 qflat = np.array([[0, 0], [1, 1], [2, 0], [-2, 0], [1, 1]])
 lc = npc.LegCharge.from_qflat(chinfo, qflat)
@@ -268,16 +267,15 @@
 def test_npc_Array_reshape():
     a = random_Array((20, 15, 10), chinfo, sort=False)
     aflat = a.to_ndarray()
     for comb_legs, transpose in [([[1]], [0, 1, 2]), ([[1], [2]], [0, 1, 2]),
                                  ([[0], [1], [2]], [0, 1, 2]), ([[2, 0]], [1, 2, 0]),
                                  ([[2, 0, 1]], [2, 0, 1])]:
         print('combine legs', comb_legs)
-        with pytest.warns(FutureWarning):
-            acomb = a.combine_legs(comb_legs)  # just sorts second leg
+        acomb = a.combine_legs(comb_legs)  # just sorts second leg
         print("=> labels: ", acomb.get_leg_labels())
         acomb.test_sanity()
         asplit = acomb.split_legs()
         asplit.test_sanity()
         npt.assert_equal(asplit.to_ndarray(), aflat.transpose(transpose))
     print("test squeeze")
     b = random_Array((10, 1, 5, 1), chinfo3, sort=True)
@@ -320,16 +318,15 @@
 
 
 def test_npc_Array_reshape_2():
     # check that combine_leg is compatible with pipe.map_incoming_flat
     shape = (2, 5, 2)
     a = random_Array(shape, chinfo3, sort=True)
     aflat = a.to_ndarray()
-    with pytest.warns(FutureWarning):
-        acomb = a.combine_legs([[0, 1]])
+    acomb = a.combine_legs([[0, 1]])
     acombflat = acomb.to_ndarray()
     pipe = acomb.legs[0]
     print(a)
     print(acomb)
     print(pipe.q_map)
     print(pipe.slices)
     # expensive: compare all entries
@@ -500,20 +497,16 @@
 
 def test_npc_addition_transpose():
     # addition with labels and transposed axes
     a1 = np.random.random([3, 3, 4])
     a2 = np.swapaxes(a1, 0, 1)
     t1 = npc.Array.from_ndarray_trivial(a1, labels=['a', 'b', 'c'])
     t2 = npc.Array.from_ndarray_trivial(a2, labels=['b', 'a', 'c'])
-    # TODO: for now warning
-    with pytest.warns(FutureWarning):
-        diff = npc.norm(t1 - t2)
-    # TODO: when the behaviour is changed do
-    #  diff = npc.norm(t1 - t2)
-    #  assert diff < 1.e-10
+    diff = npc.norm(t1 - t2)
+    assert diff < 1.e-10
 
 
 def test_npc_tensordot():
     for sort in [True, False]:
         print("sort =", sort)
         a = random_Array((10, 12, 15), chinfo3, qtotal=[0], sort=sort)
         aflat = a.to_ndarray()
```

### Comparing `physics-tenpy-0.99.0/tests/test_package_structure.py` & `physics-tenpy-1.0.0/tests/test_package_structure.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_params.py` & `physics-tenpy-1.0.0/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_post_processing.py` & `physics-tenpy-1.0.0/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_predict_ram.py` & `physics-tenpy-1.0.0/tests/test_predict_ram.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_purification.py` & `physics-tenpy-1.0.0/tests/test_purification.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_random_matrix.py` & `physics-tenpy-1.0.0/tests/test_random_matrix.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_simulation.py` & `physics-tenpy-1.0.0/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_simulation_exc.py` & `physics-tenpy-1.0.0/tests/test_simulation_exc.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_site.py` & `physics-tenpy-1.0.0/tests/test_site.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 def test_site():
     chinfo = npc.ChargeInfo([1, 3])
     leg = gen_random_legcharge(chinfo, 8)
     op1 = npc.Array.from_func(np.random.random, [leg, leg.conj()], shape_kw='size')
     op2 = npc.Array.from_func(np.random.random, [leg, leg.conj()], shape_kw='size')
     op3_dense = np.diag(np.arange(10, 18))
     labels = [f'x{i:d}' for i in range(10, 18)]
-    s = site.Site(leg, labels, silly_op=op1)
+    s = site.Site(leg, labels, silly_op=op1, sort_charge=False)
     assert s.state_index('x10') == 0
     assert s.state_index('x17') == leg.ind_len - 1
     assert s.opnames == set(['silly_op', 'Id', 'JW'])
     assert s.silly_op is op1
     s.add_op('op2', op2)
     s.add_op('op3', op3_dense)
     assert s.op2 is op2
```

### Comparing `physics-tenpy-0.99.0/tests/test_sparse.py` & `physics-tenpy-1.0.0/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_svd_robust.py` & `physics-tenpy-1.0.0/tests/test_svd_robust.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,59 +6,34 @@
 from scipy.linalg import diagsvd
 
 from tenpy.linalg import svd_robust
 
 import random_test  # fix the random seed.  # noqa F401
 from tenpy.linalg.random_matrix import standard_normal_complex
 
-import pytest
 
-
-def test_CLAPACK_import():
-    """just try to import the lapack library on the local system."""
-    if not svd_robust._old_scipy:
-        return  # scipy test: no need to import that.
-    try:
-        svd_robust._load_lapack(warn=False)
-    except EnvironmentError as e:
-        print(str(e))
-        if str(e).startswith("Couldn't find LAPACK"):
-            print("(Not an issue if you have scipy >= 0.18.0)")
-        assert (False)
-
-
-def check_svd_function(svd_function):
+def test_svd():
     """check whether svd_function behaves as np.linalg.svd."""
     for dtype in [np.float32, np.float64, np.complex64, np.complex128]:
         print("dtype = ", dtype)
         for m, n in [(1, 1), (1, 10), (10, 1), (10, 10), (10, 20)]:
             print("m, n = ", m, n)
             tol_NULP = 200 * max(max(m, n)**3,
                                  100)  # quite large tolerance, but seems to be required...
             if np.dtype(dtype).kind == 'c':  # complex?
                 A = standard_normal_complex((m, n))
             else:
                 A = np.random.standard_normal(size=(m, n))
             A = np.asarray(A, dtype)
-            Sonly = svd_function(A, compute_uv=False)
+            Sonly = svd_robust.svd(A, compute_uv=False)
 
-            U_full, S_full, VTfull = svd_function(A, full_matrices=True, compute_uv=True)
+            U_full, S_full, VTfull = svd_robust.svd(A, full_matrices=True, compute_uv=True)
             npt.assert_array_almost_equal_nulp(Sonly, S_full, tol_NULP)
             recalc = U_full.dot(diagsvd(S_full, m, n)).dot(VTfull)
             npt.assert_array_almost_equal_nulp(recalc, A, tol_NULP)
 
-            U, S, VT = svd_function(A, full_matrices=False, compute_uv=True)
+            U, S, VT = svd_robust.svd(A, full_matrices=False, compute_uv=True)
             npt.assert_array_almost_equal_nulp(Sonly, S, tol_NULP)
             recalc = U.dot(np.diag(S)).dot(VT)
             npt.assert_array_almost_equal_nulp(recalc, A, tol_NULP)
         print("types of U, S, VT = ", U.dtype, S.dtype, VT.dtype)
         assert U.dtype == A.dtype
-
-
-def test_svd():
-    check_svd_function(svd_robust.svd)
-
-
-def test_svd_gesvd():
-    if not svd_robust._old_scipy:
-        pytest.skip("have scipy >0.18.0, no need to load LAPACK directly for robust svd")
-    check_svd_function(svd_robust.svd_gesvd)
```

### Comparing `physics-tenpy-0.99.0/tests/test_tdvp.py` & `physics-tenpy-1.0.0/tests/test_tdvp.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_tebd.py` & `physics-tenpy-1.0.0/tests/test_tebd.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_terms.py` & `physics-tenpy-1.0.0/tests/test_terms.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_time_evolution.py` & `physics-tenpy-1.0.0/tests/test_time_evolution.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_tools.py` & `physics-tenpy-1.0.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_truncation.py` & `physics-tenpy-1.0.0/tests/test_truncation.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_umps.py` & `physics-tenpy-1.0.0/tests/test_umps.py`

 * *Files identical despite different names*

### Comparing `physics-tenpy-0.99.0/tests/test_vumps.py` & `physics-tenpy-1.0.0/tests/test_vumps.py`

 * *Files identical despite different names*


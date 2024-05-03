# Comparing `tmp/parameter_sweep-0.1.dev0.tar.gz` & `tmp/parameter_sweep-0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parameter_sweep-0.1.dev0.tar", last modified: Fri May  3 13:19:23 2024, max compression
+gzip compressed data, was "parameter_sweep-0.1.dev1.tar", last modified: Fri May  3 03:57:38 2024, max compression
```

## Comparing `parameter_sweep-0.1.dev0.tar` & `parameter_sweep-0.1.dev1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.360278 parameter_sweep-0.1.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.340278 parameter_sweep-0.1.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.344278 parameter_sweep-0.1.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/.github/workflows/checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-03 13:19:23.360278 parameter_sweep-0.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.340278 parameter_sweep-0.1.dev0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.344278 parameter_sweep-0.1.dev0/docs/how_to_guides/
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/docs/how_to_guides/how_to_run_differential_parameter_sweep.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/docs/how_to_guides/how_to_use_parameter_sweep.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/docs/how_to_guides/how_to_use_parameter_sweep_monte_carlo.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.340278 parameter_sweep-0.1.dev0/docs/technical_reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.344278 parameter_sweep-0.1.dev0/docs/technical_reference/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/docs/technical_reference/tools/parallel_manager.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/docs/technical_reference/tools/parameter_sweep.rst
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 13:19:23.360278 parameter_sweep-0.1.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.344278 parameter_sweep-0.1.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.348279 parameter_sweep-0.1.dev0/src/parameter_sweep/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    21391 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/differential.py
--rw-r--r--   0 runner    (1001) docker     (127)    26810 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.348279 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/data_merging_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    29622 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/loop_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.352279 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/ro_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_all_options.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_bad_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_data_merging_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_diff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_expected_diff_directory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    55375 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_expected_option_directory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_expected_sweep_directory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_loop_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_missing_sweep_loop.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_sweep.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.352279 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/concurrent_futures_parallel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/mpi_parallel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/multiprocessing_parallel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/parallel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/parallel_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/ray_io_parallel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/single_process_parallel_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.352279 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/tests/test_concurrent_futures_parallel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/tests/test_multiprocessing_parallel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/tests/test_parallel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/tests/test_ray_io_parallel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parallel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    44170 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/parameter_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/sampling_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.356279 parameter_sweep-0.1.dev0/src/parameter_sweep/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59097 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/tests/test_differential_parameter_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)    90855 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/tests/test_parameter_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/tests/test_parameter_sweep_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/tests/test_parameter_sweep_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/tests/test_recursive_parameter_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/src/parameter_sweep/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.360278 parameter_sweep-0.1.dev0/src/parameter_sweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-03 13:19:23.000000 parameter_sweep-0.1.dev0/src/parameter_sweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-03 13:19:23.000000 parameter_sweep-0.1.dev0/src/parameter_sweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:19:23.000000 parameter_sweep-0.1.dev0/src/parameter_sweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 13:19:23.000000 parameter_sweep-0.1.dev0/src/parameter_sweep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 13:19:23.000000 parameter_sweep-0.1.dev0/src/parameter_sweep.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.356279 parameter_sweep-0.1.dev0/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:19:23.360278 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/
--rw-r--r--   0 runner    (1001) docker     (127)    42459 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/Differential_Parameter_Sweep_Flowchart.png
--rw-r--r--   0 runner    (1001) docker     (127)   107185 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/LSRRO_Eagle_strong_10K.png
--rw-r--r--   0 runner    (1001) docker     (127)   173606 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/Parameter_Sweep_Flowchart.png
--rw-r--r--   0 runner    (1001) docker     (127)    94575 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/RO-ERD_Eagle_Strong_Scaling_100K.png
--rw-r--r--   0 runner    (1001) docker     (127)   112695 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/RO-ERD_Mac_2500_speedup.png
--rw-r--r--   0 runner    (1001) docker     (127)    89575 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/RO-ERD_Mac_2500_time.png
--rw-r--r--   0 runner    (1001) docker     (127)    32730 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/RO_ERD_flowsheet.png
--rw-r--r--   0 runner    (1001) docker     (127)   301357 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/Recursive_Parameter_Sweep_flowchart.png
--rw-r--r--   0 runner    (1001) docker     (127)   123876 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/maps_LCOW_recovery_NaCl_loading.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/parameter_sweep_demo_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    49425 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/scatter_LCOW_vs_Acomp.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/watertap-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    25508 2024-05-03 13:18:13.000000 parameter_sweep-0.1.dev0/tutorials/parameter_sweep_demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.339689 parameter_sweep-0.1.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.319689 parameter_sweep-0.1.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.323689 parameter_sweep-0.1.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/.github/workflows/checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-03 03:57:38.339689 parameter_sweep-0.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.319689 parameter_sweep-0.1.dev1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.323689 parameter_sweep-0.1.dev1/docs/how_to_guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/docs/how_to_guides/how_to_run_differential_parameter_sweep.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/docs/how_to_guides/how_to_use_parameter_sweep.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/docs/how_to_guides/how_to_use_parameter_sweep_monte_carlo.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.319689 parameter_sweep-0.1.dev1/docs/technical_reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.323689 parameter_sweep-0.1.dev1/docs/technical_reference/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/docs/technical_reference/tools/parallel_manager.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/docs/technical_reference/tools/parameter_sweep.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 03:57:38.339689 parameter_sweep-0.1.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.319689 parameter_sweep-0.1.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.327689 parameter_sweep-0.1.dev1/src/parameter_sweep/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21391 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/differential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26810 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.327689 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/data_merging_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29622 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/loop_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.331689 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/ro_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_all_options.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_bad_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_data_merging_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_diff.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_expected_diff_directory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    55375 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_expected_option_directory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_expected_sweep_directory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_loop_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_missing_sweep_loop.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_sweep.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.331689 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/concurrent_futures_parallel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/mpi_parallel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/multiprocessing_parallel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/parallel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/parallel_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/ray_io_parallel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/single_process_parallel_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.331689 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/tests/test_concurrent_futures_parallel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/tests/test_multiprocessing_parallel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/tests/test_parallel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/tests/test_ray_io_parallel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parallel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44170 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/parameter_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/sampling_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.331689 parameter_sweep-0.1.dev1/src/parameter_sweep/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59097 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/tests/test_differential_parameter_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90855 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/tests/test_parameter_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/tests/test_parameter_sweep_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/tests/test_parameter_sweep_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/tests/test_recursive_parameter_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/src/parameter_sweep/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.335689 parameter_sweep-0.1.dev1/src/parameter_sweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-03 03:57:38.000000 parameter_sweep-0.1.dev1/src/parameter_sweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-03 03:57:38.000000 parameter_sweep-0.1.dev1/src/parameter_sweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 03:57:38.000000 parameter_sweep-0.1.dev1/src/parameter_sweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 03:57:38.000000 parameter_sweep-0.1.dev1/src/parameter_sweep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 03:57:38.000000 parameter_sweep-0.1.dev1/src/parameter_sweep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.331689 parameter_sweep-0.1.dev1/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:57:38.335689 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)    42459 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/Differential_Parameter_Sweep_Flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (127)   107185 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/LSRRO_Eagle_strong_10K.png
+-rw-r--r--   0 runner    (1001) docker     (127)   173606 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/Parameter_Sweep_Flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (127)    94575 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/RO-ERD_Eagle_Strong_Scaling_100K.png
+-rw-r--r--   0 runner    (1001) docker     (127)   112695 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/RO-ERD_Mac_2500_speedup.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89575 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/RO-ERD_Mac_2500_time.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32730 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/RO_ERD_flowsheet.png
+-rw-r--r--   0 runner    (1001) docker     (127)   301357 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/Recursive_Parameter_Sweep_flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123876 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/maps_LCOW_recovery_NaCl_loading.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/parameter_sweep_demo_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49425 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/scatter_LCOW_vs_Acomp.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/watertap-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25508 2024-05-03 03:56:20.000000 parameter_sweep-0.1.dev1/tutorials/parameter_sweep_demo.ipynb
```

### Comparing `parameter_sweep-0.1.dev0/.github/workflows/checks.yml` & `parameter_sweep-0.1.dev1/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/.gitignore` & `parameter_sweep-0.1.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/COPYRIGHT.md` & `parameter_sweep-0.1.dev1/COPYRIGHT.md`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/LICENSE.md` & `parameter_sweep-0.1.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/PKG-INFO` & `parameter_sweep-0.1.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameter-sweep
-Version: 0.1.dev0
+Version: 0.1.dev1
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pyomo
 Requires-Dist: numpy
 Requires-Dist: h5py
 Requires-Dist: pyyaml
 Requires-Dist: idaes-pse
```

### Comparing `parameter_sweep-0.1.dev0/README.md` & `parameter_sweep-0.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/docs/how_to_guides/how_to_run_differential_parameter_sweep.rst` & `parameter_sweep-0.1.dev1/docs/how_to_guides/how_to_run_differential_parameter_sweep.rst`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/docs/how_to_guides/how_to_use_parameter_sweep.rst` & `parameter_sweep-0.1.dev1/docs/how_to_guides/how_to_use_parameter_sweep.rst`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/docs/how_to_guides/how_to_use_parameter_sweep_monte_carlo.rst` & `parameter_sweep-0.1.dev1/docs/how_to_guides/how_to_use_parameter_sweep_monte_carlo.rst`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/docs/technical_reference/tools/parallel_manager.rst` & `parameter_sweep-0.1.dev1/docs/technical_reference/tools/parallel_manager.rst`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/docs/technical_reference/tools/parameter_sweep.rst` & `parameter_sweep-0.1.dev1/docs/technical_reference/tools/parameter_sweep.rst`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/pyproject.toml` & `parameter_sweep-0.1.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/__init__.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/__init__.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/differential.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/differential.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/functions.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/functions.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/data_merging_tool.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/data_merging_tool.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/loop_tool.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/loop_tool.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/ro_setup.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/ro_setup.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_all_options.yaml` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_all_options.yaml`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_bad_default.yaml` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_bad_default.yaml`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_data_merging_tool.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_data_merging_tool.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_diff.yaml` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_diff.yaml`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_expected_diff_directory.yaml` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_expected_diff_directory.yaml`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_expected_option_directory.yaml` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_expected_option_directory.yaml`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_expected_sweep_directory.yaml` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_expected_sweep_directory.yaml`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_loop_tool.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_loop_tool.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/loop_tool/tests/test_sweep.yaml` & `parameter_sweep-0.1.dev1/src/parameter_sweep/loop_tool/tests/test_sweep.yaml`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/model_manager.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/model_manager.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/concurrent_futures_parallel_manager.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/concurrent_futures_parallel_manager.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/mpi_parallel_manager.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/mpi_parallel_manager.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/multiprocessing_parallel_manager.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/multiprocessing_parallel_manager.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/parallel_manager.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/parallel_manager.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/parallel_manager_factory.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/parallel_manager_factory.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/ray_io_parallel_manager.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/ray_io_parallel_manager.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/results.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/results.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/single_process_parallel_manager.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/single_process_parallel_manager.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/tests/test_concurrent_futures_parallel_manager.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/tests/test_concurrent_futures_parallel_manager.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/tests/test_multiprocessing_parallel_manager.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/tests/test_multiprocessing_parallel_manager.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/tests/test_parallel_manager.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/tests/test_parallel_manager.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel/tests/test_ray_io_parallel_manager.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel/tests/test_ray_io_parallel_manager.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parallel_utils.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/parameter_sweep.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/parameter_sweep.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/reader.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/reader.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/sampling_types.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/sampling_types.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/tests/test_differential_parameter_sweep.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/tests/test_differential_parameter_sweep.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/tests/test_parameter_sweep.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/tests/test_parameter_sweep.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/tests/test_parameter_sweep_reader.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/tests/test_parameter_sweep_reader.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/tests/test_parameter_sweep_writer.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/tests/test_parameter_sweep_writer.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/tests/test_recursive_parameter_sweep.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/tests/test_recursive_parameter_sweep.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep/writer.py` & `parameter_sweep-0.1.dev1/src/parameter_sweep/writer.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep.egg-info/PKG-INFO` & `parameter_sweep-0.1.dev1/src/parameter_sweep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameter-sweep
-Version: 0.1.dev0
+Version: 0.1.dev1
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pyomo
 Requires-Dist: numpy
 Requires-Dist: h5py
 Requires-Dist: pyyaml
 Requires-Dist: idaes-pse
```

### Comparing `parameter_sweep-0.1.dev0/src/parameter_sweep.egg-info/SOURCES.txt` & `parameter_sweep-0.1.dev1/src/parameter_sweep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/Differential_Parameter_Sweep_Flowchart.png` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/Differential_Parameter_Sweep_Flowchart.png`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/LSRRO_Eagle_strong_10K.png` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/LSRRO_Eagle_strong_10K.png`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/Parameter_Sweep_Flowchart.png` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/Parameter_Sweep_Flowchart.png`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/RO-ERD_Eagle_Strong_Scaling_100K.png` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/RO-ERD_Eagle_Strong_Scaling_100K.png`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/RO-ERD_Mac_2500_speedup.png` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/RO-ERD_Mac_2500_speedup.png`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/RO-ERD_Mac_2500_time.png` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/RO-ERD_Mac_2500_time.png`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/RO_ERD_flowsheet.png` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/RO_ERD_flowsheet.png`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/Recursive_Parameter_Sweep_flowchart.png` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/Recursive_Parameter_Sweep_flowchart.png`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/maps_LCOW_recovery_NaCl_loading.jpg` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/maps_LCOW_recovery_NaCl_loading.jpg`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/parameter_sweep_demo_script.py` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/parameter_sweep_demo_script.py`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/scatter_LCOW_vs_Acomp.jpg` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/scatter_LCOW_vs_Acomp.jpg`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/assets_parameter_sweep_demo/watertap-logo.png` & `parameter_sweep-0.1.dev1/tutorials/assets_parameter_sweep_demo/watertap-logo.png`

 * *Files identical despite different names*

### Comparing `parameter_sweep-0.1.dev0/tutorials/parameter_sweep_demo.ipynb` & `parameter_sweep-0.1.dev1/tutorials/parameter_sweep_demo.ipynb`

 * *Files identical despite different names*


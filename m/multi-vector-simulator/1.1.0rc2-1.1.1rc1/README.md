# Comparing `tmp/multi-vector-simulator-1.1.0rc2.tar.gz` & `tmp/multi_vector_simulator-1.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi-vector-simulator-1.1.0rc2.tar", last modified: Sat Apr 27 21:21:57 2024, max compression
+gzip compressed data, was "multi_vector_simulator-1.1.1rc1.tar", last modified: Fri May  3 08:48:54 2024, max compression
```

## Comparing `multi-vector-simulator-1.1.0rc2.tar` & `multi_vector_simulator-1.1.1rc1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.241921 multi-vector-simulator-1.1.0rc2/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18092 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/LICENSE.md
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       45 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/MANIFEST.in
--rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13769 2024-04-27 21:21:57.241921 multi-vector-simulator-1.1.0rc2/PKG-INFO
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11547 2023-02-03 15:33:58.000000 multi-vector-simulator-1.1.0rc2/README.rst
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       38 2024-04-27 21:21:57.241921 multi-vector-simulator-1.1.0rc2/setup.cfg
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9653 2023-06-14 09:01:56.000000 multi-vector-simulator-1.1.0rc2/setup.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.221921 multi-vector-simulator-1.1.0rc2/src/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.229921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    16859 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/A0_initialization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    27452 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/A1_csv_to_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11661 2023-09-15 14:50:37.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/B0_data_input_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    72874 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C0_data_processing.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    40172 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C1_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18277 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C2_economic_functions.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14693 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D0_modelling_and_optimization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    54729 2024-04-27 21:06:46.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D1_model_components.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28866 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D2_model_constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12129 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E0_evaluation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44646 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E1_process_results.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18293 2023-11-01 09:47:08.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E2_economics.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44571 2024-03-27 00:09:52.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E3_indicator_calculation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9281 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E4_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9543 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F0_output.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    37196 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F1_plotting.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38813 2023-09-14 20:45:28.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F2_autoreport.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11757 2023-11-01 08:24:33.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F3_debug.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10258 2023-09-12 21:19:20.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/cli.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.229921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14353 2024-04-27 21:21:56.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/MVS_parameters_list.csv
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.229921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/assets/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)   168697 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6128 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/assets/styles.css
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.221921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      132 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/constraints.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       92 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/economic_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       22 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyBusses.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       81 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConsumption.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      332 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConversion.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      355 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProduction.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      312 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProviders.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/energyStorage.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      121 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/fixcost.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/project_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/simulation_settings.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      404 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/csv_elements/storage_01.csv
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/time_series/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       16 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/input_template/time_series/blank
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/constraints.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/economic_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      154 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyBusses.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      179 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConsumption.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1068 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      562 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      410 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProviders.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      221 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyStorage.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      200 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/fixcost.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      249 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/project_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      130 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/simulation_settings.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      491 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/storage_01.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    23516 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/mvs_config.json
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/time_series/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    78842 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    34217 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    13451 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/server.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.233921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25650 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3404 2022-03-30 10:59:56.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/analysis.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12078 2023-02-03 12:59:38.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8633 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants_json_strings.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1495 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants_output.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28826 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/data_parser.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1725 2023-02-03 13:29:18.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/exceptions.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5563 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/helpers.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      144 2024-04-27 21:21:50.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/version.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.237921 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/
--rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13769 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/PKG-INFO
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5026 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        1 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      192 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/entry_points.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      426 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/requires.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       23 2024-04-27 21:21:57.000000 multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/top_level.txt
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-27 21:21:57.237921 multi-vector-simulator-1.1.0rc2/tests/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/tests/test_A0_initialization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12999 2022-10-16 15:02:06.000000 multi-vector-simulator-1.1.0rc2/tests/test_A1_csv_to_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6610 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_B0_data_input_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    51979 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/tests/test_C0_data_processing.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    32932 2023-02-03 12:59:38.000000 multi-vector-simulator-1.1.0rc2/tests/test_C1_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10403 2024-04-27 21:08:22.000000 multi-vector-simulator-1.1.0rc2/tests/test_C2_economic_functions.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8840 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_D0_modelling_and_optimization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    47067 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_D1_model_components.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    19212 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_D2_model_constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     7318 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_E0_evaluation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    21776 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_E1_process_results.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11264 2022-09-23 09:34:10.000000 multi-vector-simulator-1.1.0rc2/tests/test_E2_economics.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    31598 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_E3_indicator_calculation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12189 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_E4_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14321 2022-11-02 09:00:04.000000 multi-vector-simulator-1.1.0rc2/tests/test_F0_output.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6212 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_F1_plotting.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    17082 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_KPI.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25033 2022-10-16 15:02:02.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    15959 2024-04-27 20:59:54.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_feedin.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    22774 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_scenarios.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9113 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_special_features.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38791 2024-04-27 21:03:48.000000 multi-vector-simulator-1.1.0rc2/tests/test_benchmark_stratified_thermal_storage.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3658 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/tests/test_input_folder_parameters.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      641 2022-01-27 11:19:42.000000 multi-vector-simulator-1.1.0rc2/tests/test_sensitivity.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5255 2022-09-23 09:43:57.000000 multi-vector-simulator-1.1.0rc2/tests/test_utils.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.116319 multi_vector_simulator-1.1.1rc1/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18092 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/LICENSE.md
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       45 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/MANIFEST.in
+-rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13768 2024-05-03 08:48:54.116319 multi_vector_simulator-1.1.1rc1/PKG-INFO
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11547 2024-04-28 21:08:27.000000 multi_vector_simulator-1.1.1rc1/README.rst
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       38 2024-05-03 08:48:54.116319 multi_vector_simulator-1.1.1rc1/setup.cfg
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9675 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/setup.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.104318 multi_vector_simulator-1.1.1rc1/src/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.108318 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    16867 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/A0_initialization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    27496 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/A1_csv_to_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11678 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/B0_data_input_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    73503 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/C0_data_processing.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    40172 2024-04-28 21:08:27.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/C1_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18281 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/C2_economic_functions.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14775 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/D0_modelling_and_optimization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    59778 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/D1_model_components.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    29059 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/D2_model_constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12151 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/E0_evaluation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    45315 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/E1_process_results.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18325 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/E2_economics.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44564 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/E3_indicator_calculation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9281 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/E4_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9542 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/F0_output.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    37324 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/F1_plotting.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    39409 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/F2_autoreport.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11757 2023-11-01 08:24:33.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/F3_debug.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10265 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/cli.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.108318 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14353 2024-05-03 08:48:53.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/MVS_parameters_list.csv
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.108318 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/assets/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)   168697 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6128 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/assets/styles.css
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.104318 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.108318 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      132 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/constraints.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       92 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/economic_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       22 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyBusses.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       81 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConsumption.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      332 2024-04-27 21:28:05.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConversion.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      355 2024-04-27 21:28:05.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProduction.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      312 2024-04-27 21:28:05.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProviders.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      150 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/energyStorage.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      121 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/fixcost.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/project_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/simulation_settings.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      404 2024-04-27 21:28:05.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/csv_elements/storage_01.csv
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.108318 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/time_series/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       16 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/input_template/time_series/blank
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.108318 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.108318 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/constraints.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/economic_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      154 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyBusses.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      179 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConsumption.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1068 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      562 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      410 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProviders.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      221 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyStorage.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      200 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/fixcost.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      249 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/project_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      130 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/simulation_settings.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      491 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/storage_01.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    23516 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/mvs_config.json
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.108318 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/time_series/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    78842 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    34217 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    13657 2024-04-28 21:08:27.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/server.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.112318 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25666 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3404 2022-03-30 10:59:56.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/analysis.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12525 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/constants.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8736 2024-04-28 21:08:27.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/constants_json_strings.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1495 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/constants_output.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28921 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/data_parser.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1725 2024-04-28 21:08:27.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/exceptions.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6460 2024-04-28 21:08:27.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/helpers.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      144 2024-05-03 08:47:41.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/version.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.112318 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator.egg-info/
+-rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)    13768 2024-05-03 08:48:54.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5026 2024-05-03 08:48:54.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        1 2024-05-03 08:48:54.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      192 2024-05-03 08:48:54.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator.egg-info/entry_points.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      425 2024-05-03 08:48:54.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator.egg-info/requires.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       23 2024-05-03 08:48:54.000000 multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator.egg-info/top_level.txt
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-05-03 08:48:54.112318 multi_vector_simulator-1.1.1rc1/tests/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12149 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_A0_initialization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    13021 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_A1_csv_to_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6955 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_B0_data_input_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    52255 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_C0_data_processing.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    32931 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_C1_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10403 2024-04-28 21:08:27.000000 multi_vector_simulator-1.1.1rc1/tests/test_C2_economic_functions.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8840 2024-04-28 21:08:27.000000 multi_vector_simulator-1.1.1rc1/tests/test_D0_modelling_and_optimization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    47224 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_D1_model_components.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    19386 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_D2_model_constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     7318 2022-10-16 15:02:02.000000 multi_vector_simulator-1.1.1rc1/tests/test_E0_evaluation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    21840 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_E1_process_results.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11296 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_E2_economics.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    31631 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_E3_indicator_calculation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12383 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_E4_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14412 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_F0_output.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6212 2022-10-16 15:02:02.000000 multi_vector_simulator-1.1.1rc1/tests/test_F1_plotting.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    17117 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_benchmark_KPI.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25034 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_benchmark_constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    15959 2024-04-28 21:08:27.000000 multi_vector_simulator-1.1.1rc1/tests/test_benchmark_feedin.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    22775 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_benchmark_scenarios.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9113 2024-04-28 21:08:27.000000 multi_vector_simulator-1.1.1rc1/tests/test_benchmark_special_features.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38791 2024-04-28 21:08:27.000000 multi_vector_simulator-1.1.1rc1/tests/test_benchmark_stratified_thermal_storage.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3658 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_input_folder_parameters.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      641 2022-01-27 11:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_sensitivity.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     5254 2024-04-30 19:19:42.000000 multi_vector_simulator-1.1.1rc1/tests/test_utils.py
```

### Comparing `multi-vector-simulator-1.1.0rc2/LICENSE.md` & `multi_vector_simulator-1.1.1rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/PKG-INFO` & `multi_vector_simulator-1.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-vector-simulator
-Version: 1.1.0rc2
+Version: 1.1.1rc1
 Summary: Multi-vector Simulation Tool assessing and optimizing Local Energy Systems (LES) for the E-LAND project
 Home-page: https://github.com/rl-institut/multi-vector-simulator
 Author: Reiner Lemoine Institut
 Author-email: pypi@rl-institut.de
 Project-URL: Bug Reports, https://github.com/rl-institut/multi-vector-simulator/issues
 Project-URL: Source, https://github.com/rl-institut/multi-vector-simulator
 Keywords: multi-vector local-energy-systems
@@ -39,15 +39,15 @@
 Requires-Dist: folium>=0.10.1; extra == "report"
 Requires-Dist: reverse_geocoder>=1.5.1; extra == "report"
 Requires-Dist: staticmap>=0.5.4; extra == "report"
 Requires-Dist: pyppeteer>=0.2.2; extra == "report"
 Requires-Dist: psutil>=5.7.0; extra == "report"
 Provides-Extra: test
 Requires-Dist: pytest>=5.3.1; extra == "test"
-Requires-Dist: black==19.10b0; extra == "test"
+Requires-Dist: black==24.3.0; extra == "test"
 Requires-Dist: coverage>=4.5; extra == "test"
 Requires-Dist: coveralls>=3.0.1; extra == "test"
 Requires-Dist: mock>=3.0.5; extra == "test"
 Requires-Dist: click==8.0.2; extra == "test"
 
 ##################################################
 MVS - Multi-Vector Simulator of the E-LAND toolbox
```

### Comparing `multi-vector-simulator-1.1.0rc2/README.rst` & `multi_vector_simulator-1.1.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/setup.py` & `multi_vector_simulator-1.1.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,18 @@
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
     #   py_modules=["my_module"],
-    packages=["multi_vector_simulator", "multi_vector_simulator.utils",],  # Required
+    packages=[
+        "multi_vector_simulator",
+        "multi_vector_simulator.utils",
+    ],  # Required
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. If you
     # do not support Python 2, you can simplify this to '>=3.5' or similar, see
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
     python_requires=">=3.6, <4",
     # This field lists other packages that your project depends on to run.
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/A0_initialization.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/A0_initialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,16 @@
       -o [REPORT_PATH]
         path to save the pdf report
 
 
     :return: parser
     """
     parser = argparse.ArgumentParser(
-        prog="mvs_report", description="Display the report of a MVS simulation",
+        prog="mvs_report",
+        description="Display the report of a MVS simulation",
     )
     parser.add_argument(
         "-pdf",
         dest=ARG_PDF,
         help="print the report as pdf (default: False)",
         nargs="?",
         const=True,
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/A1_csv_to_json.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/A1_csv_to_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,16 @@
     CsvParsingError,
     WrongStorageColumn,
     MissingCsvEndingError,
 )
 
 
 def create_input_json(
-    input_directory, pass_back=True,
+    input_directory,
+    pass_back=True,
 ):
     """Convert csv files to json file as input for the simulation.
 
     Looks at all csv-files in `input_directory` and compile the information they contain
     into a json file. The json file is then saved within the `input_directory`
     with the filename `CSV_FNAME`.
     While reading the csv files, it is checked, whether all required parameters
@@ -511,15 +512,17 @@
             single_dict.update({column: column_dict})
             # add exception for energyStorage
             if filename == ENERGY_STORAGE:
                 storage_file_name = check_storage_file_is_csv(
                     df.loc[STORAGE_FILENAME][column]
                 )
                 storage_dict = add_storage_components(
-                    storage_file_name, input_directory, single_dict[column][LABEL],
+                    storage_file_name,
+                    input_directory,
+                    single_dict[column][LABEL],
                 )
                 single_dict[column].update(storage_dict)
 
     logging.debug(
         "From file %s following assets are added to the energy system: %s",
         filename,
         asset_name_string[:-2],
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/B0_data_input_json.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/B0_data_input_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Module B0 - Data input json
 ===========================
 """
+
 import logging
 import copy
 import json
 import os
 
 import numpy as np
 import pandas as pd
@@ -317,15 +318,16 @@
         )
 
     # Move the json file created from csv to the copy of the input folder in the output folder
     if move_copy is True:
         os.replace(
             path_input_file,
             os.path.join(
-                dict_values[SIMULATION_SETTINGS][PATH_OUTPUT_FOLDER_INPUTS], CSV_FNAME,
+                dict_values[SIMULATION_SETTINGS][PATH_OUTPUT_FOLDER_INPUTS],
+                CSV_FNAME,
             ),
         )
 
     # add default value if the field PATHS_TO_PLOTS is not already present
     if PATHS_TO_PLOTS not in dict_values:
         dict_values.update(copy.deepcopy(DICT_PLOTS))
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C0_data_processing.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/C0_data_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,18 +286,20 @@
     -------
     Updates dict_values
     """
     auto_sinks = []
     for bus in dict_values[ENERGY_BUSSES]:
         excess_sink_name = bus + EXCESS_SINK
         energy_vector = dict_values[ENERGY_BUSSES][bus][ENERGY_VECTOR]
+        # TODO make this official if needed
+        excess_price = dict_values[ENERGY_BUSSES][bus].get("price", 0)
         define_sink(
             dict_values=dict_values,
             asset_key=excess_sink_name,
-            price={VALUE: 0, UNIT: CURR + "/" + UNIT},
+            price={VALUE: excess_price, UNIT: CURR + "/" + UNIT},
             inflow_direction=bus,
             energy_vector=energy_vector,
             asset_type="excess",
         )
         dict_values[ENERGY_BUSSES][bus].update({EXCESS_SINK: excess_sink_name})
         auto_sinks.append(excess_sink_name)
         logging.debug(
@@ -328,15 +330,17 @@
 
         # in case there is only one parameter provided (input bus and one output bus)
         if (
             FILENAME in dict_values[group][asset][EFFICIENCY]
             and HEADER in dict_values[group][asset][EFFICIENCY]
         ):
             receive_timeseries_from_csv(
-                dict_values[SIMULATION_SETTINGS], dict_values[group][asset], EFFICIENCY,
+                dict_values[SIMULATION_SETTINGS],
+                dict_values[group][asset],
+                EFFICIENCY,
             )
         # in case there is more than one parameter provided (either (A) n input busses and 1 output bus or (B) 1 input bus and n output busses)
         # dictionaries with filenames and headers will be replaced by timeseries, scalars will be mantained
         elif isinstance(dict_values[group][asset][EFFICIENCY][VALUE], list):
             treat_multiple_flows(dict_values[group][asset], dict_values, EFFICIENCY)
 
             # same distinction of values provided with dictionaries (one input and one output) or list (multiple).
@@ -392,15 +396,16 @@
     :param dict_values:
     :param group:
     :return:
     """
     for asset in dict_values[group]:
         for subasset in [STORAGE_CAPACITY, INPUT_POWER, OUTPUT_POWER]:
             define_missing_cost_data(
-                dict_values, dict_values[group][asset][subasset],
+                dict_values,
+                dict_values[group][asset][subasset],
             )
             evaluate_lifetime_costs(
                 dict_values[SIMULATION_SETTINGS],
                 dict_values[ECONOMIC_DATA],
                 dict_values[group][asset][subasset],
             )
 
@@ -498,31 +503,39 @@
 
     # read timeseries with filename provided for variable costs.
     # if multiple dispatch_price are given for multiple busses, it checks if any v
     # alue is a timeseries
     if DISPATCH_PRICE in dict_asset:
         if isinstance(dict_asset[DISPATCH_PRICE][VALUE], dict):
             receive_timeseries_from_csv(
-                dict_values[SIMULATION_SETTINGS], dict_asset, DISPATCH_PRICE,
+                dict_values[SIMULATION_SETTINGS],
+                dict_asset,
+                DISPATCH_PRICE,
             )
         elif isinstance(dict_asset[DISPATCH_PRICE][VALUE], list):
             treat_multiple_flows(dict_asset, dict_values, DISPATCH_PRICE)
 
     economic_data = dict_values[ECONOMIC_DATA]
 
     basic_costs = {
         OPTIMIZE_CAP: {VALUE: False, UNIT: TYPE_BOOL},
         UNIT: "?",
         INSTALLED_CAP: {VALUE: 0.0, UNIT: UNIT},
         DEVELOPMENT_COSTS: {VALUE: 0, UNIT: CURR},
         SPECIFIC_COSTS: {VALUE: 0, UNIT: CURR + "/" + UNIT},
         SPECIFIC_COSTS_OM: {VALUE: 0, UNIT: CURR + "/" + UNIT_YEAR},
         DISPATCH_PRICE: {VALUE: 0, UNIT: CURR + "/" + UNIT + "/" + UNIT_YEAR},
-        LIFETIME: {VALUE: economic_data[PROJECT_DURATION][VALUE], UNIT: UNIT_YEAR,},
-        AGE_INSTALLED: {VALUE: 0, UNIT: UNIT_YEAR,},
+        LIFETIME: {
+            VALUE: economic_data[PROJECT_DURATION][VALUE],
+            UNIT: UNIT_YEAR,
+        },
+        AGE_INSTALLED: {
+            VALUE: 0,
+            UNIT: UNIT_YEAR,
+        },
     }
 
     # checks that an asset has all cost parameters needed for evaluation.
     # Adds standard values.
     str = ""
     for cost in basic_costs:
         if cost not in dict_asset:
@@ -716,19 +729,25 @@
 
     months_in_a_period = determine_months_in_a_peak_demand_pricing_period(
         number_of_pricing_periods,
         dict_values[SIMULATION_SETTINGS][EVALUATED_PERIOD][VALUE],
     )
 
     dict_availability_timeseries = define_availability_of_peak_demand_pricing_assets(
-        dict_values, number_of_pricing_periods, months_in_a_period,
+        dict_values,
+        number_of_pricing_periods,
+        months_in_a_period,
     )
 
-    list_of_dso_energyConversion_assets = add_a_transformer_for_each_peak_demand_pricing_period(
-        dict_values, dso_dict, dict_availability_timeseries,
+    list_of_dso_energyConversion_assets = (
+        add_a_transformer_for_each_peak_demand_pricing_period(
+            dict_values,
+            dso_dict,
+            dict_availability_timeseries,
+        )
     )
 
     define_source(
         dict_values=dict_values,
         asset_key=dso_name + DSO_CONSUMPTION,
         outflow_direction=peak_demand_bus_name(dso_dict[OUTFLOW_DIRECTION]),
         price=dso_dict[ENERGY_PRICE],
@@ -1019,15 +1038,18 @@
         OPTIMIZE_CAP: {VALUE: True, UNIT: TYPE_BOOL},
         INSTALLED_CAP: {VALUE: 0, UNIT: dict_dso[UNIT]},
         INFLOW_DIRECTION: peak_demand_bus_name(dict_dso[INFLOW_DIRECTION]),
         OUTFLOW_DIRECTION: dict_dso[OUTFLOW_DIRECTION],
         AVAILABILITY_DISPATCH: timeseries_availability,
         EFFICIENCY: {VALUE: 1, UNIT: "factor"},
         DEVELOPMENT_COSTS: {VALUE: 0, UNIT: CURR},
-        SPECIFIC_COSTS: {VALUE: 0, UNIT: CURR + "/" + dict_dso[UNIT],},
+        SPECIFIC_COSTS: {
+            VALUE: 0,
+            UNIT: CURR + "/" + dict_dso[UNIT],
+        },
         # the demand pricing is only applied to consumption
         SPECIFIC_COSTS_OM: {
             VALUE: dict_dso[PEAK_DEMAND_PRICING][VALUE],
             UNIT: CURR + "/" + dict_dso[UNIT] + "/" + UNIT_YEAR,
         },
         DISPATCH_PRICE: {VALUE: 0, UNIT: CURR + "/" + dict_dso[UNIT] + "/" + UNIT_HOUR},
         OEMOF_ASSET_TYPE: OEMOF_TRANSFORMER,
@@ -1052,25 +1074,28 @@
         INFLOW_DIRECTION: dict_dso[INFLOW_DIRECTION],
         OUTFLOW_DIRECTION: peak_demand_bus_name(
             dict_dso[INFLOW_DIRECTION], feedin=True
         ),
         AVAILABILITY_DISPATCH: timeseries_availability,
         EFFICIENCY: {VALUE: 1, UNIT: "factor"},
         DEVELOPMENT_COSTS: {VALUE: 0, UNIT: CURR},
-        SPECIFIC_COSTS: {VALUE: 0, UNIT: CURR + "/" + dict_dso[UNIT],},
+        SPECIFIC_COSTS: {
+            VALUE: 0,
+            UNIT: CURR + "/" + dict_dso[UNIT],
+        },
         # the demand pricing is only applied to consumption
         SPECIFIC_COSTS_OM: {
             VALUE: 0,
             UNIT: CURR + "/" + dict_dso[UNIT] + "/" + UNIT_YEAR,
         },
         DISPATCH_PRICE: {VALUE: 0, UNIT: CURR + "/" + dict_dso[UNIT] + "/" + UNIT_HOUR},
         OEMOF_ASSET_TYPE: OEMOF_TRANSFORMER,
         ENERGY_VECTOR: dict_dso[ENERGY_VECTOR],
         AGE_INSTALLED: {VALUE: 0, UNIT: UNIT_YEAR},
-        TYPE_ASSET: dict_dso.get(TYPE_ASSET)
+        TYPE_ASSET: dict_dso.get(TYPE_ASSET),
         # LIFETIME: {VALUE: 100, UNIT: UNIT_YEAR},
     }
     if dict_dso.get(DSO_FEEDIN_CAP, None) is not None:
         dso_feedin_transformer[MAXIMUM_CAP] = {
             VALUE: dict_dso[DSO_FEEDIN_CAP][VALUE],
             UNIT: dict_dso[UNIT],
         }
@@ -1144,15 +1169,18 @@
         DISPATCHABILITY: True,
         LIFETIME: {
             VALUE: dict_values[ECONOMIC_DATA][PROJECT_DURATION][VALUE],
             UNIT: UNIT_YEAR,
         },
         OPTIMIZE_CAP: {VALUE: True, UNIT: TYPE_BOOL},
         MAXIMUM_CAP: {VALUE: None, UNIT: "?"},
-        AGE_INSTALLED: {VALUE: 0, UNIT: UNIT_YEAR,},
+        AGE_INSTALLED: {
+            VALUE: 0,
+            UNIT: UNIT_YEAR,
+        },
         ENERGY_VECTOR: energy_vector,
         EMISSION_FACTOR: emission_factor,
         TYPE_ASSET: asset_type,
     }
 
     if outflow_direction not in dict_values[ENERGY_BUSSES]:
         dict_values[ENERGY_BUSSES].update(
@@ -1328,15 +1356,18 @@
         LABEL: asset_key,
         INFLOW_DIRECTION: inflow_direction,
         # OPEX_VAR: {VALUE: price, UNIT: CURR + "/" + UNIT},
         LIFETIME: {
             VALUE: dict_values[ECONOMIC_DATA][PROJECT_DURATION][VALUE],
             UNIT: UNIT_YEAR,
         },
-        AGE_INSTALLED: {VALUE: 0, UNIT: UNIT_YEAR,},
+        AGE_INSTALLED: {
+            VALUE: 0,
+            UNIT: UNIT_YEAR,
+        },
         ENERGY_VECTOR: energy_vector,
         OPTIMIZE_CAP: {VALUE: True, UNIT: TYPE_BOOL},
         DISPATCHABILITY: {VALUE: True, UNIT: TYPE_BOOL},
         TYPE_ASSET: asset_type,
     }
 
     if inflow_direction not in dict_values[ENERGY_BUSSES]:
@@ -1402,15 +1433,17 @@
             )
     else:
         sink.update({DISPATCH_PRICE: {VALUE: price[VALUE], UNIT: price[UNIT]}})
 
     for item in [SPECIFIC_COSTS, SPECIFIC_COSTS_OM]:
         if item in kwargs:
             sink.update(
-                {item: kwargs[item],}
+                {
+                    item: kwargs[item],
+                }
             )
 
     # update dictionary
     dict_values[ENERGY_CONSUMPTION].update({asset_key: sink})
 
     # If multiple input busses exist
     apply_function_to_single_or_list(
@@ -1745,16 +1778,22 @@
 
     if TIMESERIES in dict_asset:
         timeseries = dict_asset[TIMESERIES]
         unit = dict_asset[UNIT]
 
         dict_asset.update(
             {
-                TIMESERIES_PEAK: {VALUE: max(timeseries), UNIT: unit,},
-                TIMESERIES_TOTAL: {VALUE: sum(timeseries), UNIT: unit,},
+                TIMESERIES_PEAK: {
+                    VALUE: max(timeseries),
+                    UNIT: unit,
+                },
+                TIMESERIES_TOTAL: {
+                    VALUE: sum(timeseries),
+                    UNIT: unit,
+                },
                 TIMESERIES_AVERAGE: {
                     VALUE: sum(timeseries) / len(timeseries),
                     UNIT: unit,
                 },
             }
         )
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C1_verification.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/C1_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/C2_economic_functions.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/C2_economic_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 - Calculate annuity factor
 - calculate crf depending on year
 - calculate specific lifetime capex, considering replacement costs and residual value of the asset
 - calculate annuity from present costs
 - calculate present costs based on annuity
 - calculate effective fuel price cost, in case there is a annual fuel price change (this functionality still has to be checked in this module)
 """
+
 import logging
 import pandas as pd
 
 from multi_vector_simulator.utils.constants import UNIT_HOUR
 
 from multi_vector_simulator.utils.constants_json_strings import (
     ANNUITY_FACTOR,
     DISPATCH_PRICE,
     VALUE,
     UNIT,
     LIFETIME_PRICE_DISPATCH,
 )
 
+
 # annuity factor to calculate present value of cash flows
 def annuity_factor(project_life, discount_factor):
     r"""
     Calculates the annuity factor, which in turn in used to calculate the present value of annuities (instalments)
 
     Parameters
     ----------
@@ -254,17 +256,17 @@
             linear_depreciation_last_investment
             * (year - project_lifetime)
             / (1 + discount_factor) ** (project_lifetime)
         )
         # Subtraction of component value at end of life with last replacement (= number_of_investments - 1)
         replacement_costs -= value_at_project_end
         # Update cash flow projection (specific)
-        present_value_of_capital_expenditures.loc[
-            project_lifetime
-        ] = -value_at_project_end
+        present_value_of_capital_expenditures.loc[project_lifetime] = (
+            -value_at_project_end
+        )
 
     return replacement_costs
 
 
 def annuity(present_value, crf):
     """
     Calculates the annuity which is a fixed stream of payments incurred by investments in assets
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D0_modelling_and_optimization.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/D0_modelling_and_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,16 @@
         """
         if dict_values[SIMULATION_SETTINGS][OUTPUT_LP_FILE][VALUE] is True:
             path_lp_file = os.path.join(
                 dict_values[SIMULATION_SETTINGS][PATH_OUTPUT_FOLDER], LP_FILE
             )
             logging.debug("Saving to lp-file.")
             local_energy_system.write(
-                path_lp_file, io_options={"symbolic_solver_labels": True},
+                path_lp_file,
+                io_options={"symbolic_solver_labels": True},
             )
 
     def simulating(dict_values, model, local_energy_system):
         """
         Initiates the oemof-solph simulation, accesses results and writes main results into dict
 
         If an error is encountered in the oemof solver, mvs should not be allowed to continue,
@@ -344,14 +345,15 @@
         -------
         Updated model with results, main results (flows, assets) and meta results (simulation)
         """
 
         logging.info("Starting simulation.")
         # turn warnings into errors
         warnings.filterwarnings("error")
+        warnings.filterwarnings("always", category=FutureWarning)
         try:
             local_energy_system.solve(
                 solver="cbc",
                 solve_kwargs={
                     "tee": False
                 },  # if tee_switch is true solver messages will be displayed
                 cmdline_options={"ratioGap": str(0.03)},
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D1_model_components.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/D1_model_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,26 +43,32 @@
     TIMESERIES_PEAK,
     INFLOW_DIRECTION,
     OUTFLOW_DIRECTION,
     SIMULATION_ANNUITY,
     MAXIMUM_ADD_CAP,
     MAXIMUM_ADD_CAP_NORMALIZED,
     DISPATCHABILITY,
+    TYPE_ASSET,
     OEMOF_ASSET_TYPE,
     OEMOF_GEN_STORAGE,
     OEMOF_SINK,
     OEMOF_SOURCE,
     OEMOF_TRANSFORMER,
     OEMOF_BUSSES,
     OEMOF_ExtractionTurbineCHP,
     EMISSION_FACTOR,
     BETA,
     INVESTMENT_BUS,
+    REDUCABLE_DEMAND,
+)
+from multi_vector_simulator.utils.helpers import (
+    get_item_if_list,
+    get_length_if_list,
+    reducable_demand_name,
 )
-from multi_vector_simulator.utils.helpers import get_item_if_list, get_length_if_list
 from multi_vector_simulator.utils.exceptions import (
     MissingParameterError,
     WrongParameterFormatError,
 )
 
 
 def check_list_parameters_transformers_single_input_single_output(
@@ -350,15 +356,18 @@
     - test_sink_non_dispatchable_single_input_bus()
     - test_sink_non_dispatchable_multiple_input_busses()
     - test_sink_dispatchable_single_input_bus()
     - test_sink_dispatchable_multiple_input_busses()
 
     """
     if TIMESERIES in dict_asset:
-        sink_non_dispatchable(model, dict_asset, **kwargs)
+        if dict_asset.get(TYPE_ASSET) == REDUCABLE_DEMAND:
+            sink_demand_reduction(model, dict_asset, **kwargs)
+        else:
+            sink_non_dispatchable(model, dict_asset, **kwargs)
 
     else:
         sink_dispatchable_optimize(model, dict_asset, **kwargs)
 
 
 def source(model, dict_asset, **kwargs):
     r"""
@@ -584,17 +593,17 @@
             outputs = {
                 kwargs[OEMOF_BUSSES][dict_asset[OUTFLOW_DIRECTION]]: solph.Flow(
                     nominal_value=dict_asset[INSTALLED_CAP][VALUE]
                 )
             }
             efficiencies = {}
             for i, efficiency in enumerate(dict_asset[EFFICIENCY][VALUE]):
-                efficiencies[
-                    kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION][i]]
-                ] = efficiency
+                efficiencies[kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION][i]]] = (
+                    efficiency
+                )
 
         elif isinstance(dict_asset[INFLOW_DIRECTION], str) and isinstance(
             dict_asset[OUTFLOW_DIRECTION], list
         ):
             # single input and multiple outputs
             num_outputs = len(dict_asset[OUTFLOW_DIRECTION])
             if get_length_if_list(dict_asset[EFFICIENCY][VALUE]) != num_outputs:
@@ -618,17 +627,17 @@
                     variable_costs=get_item_if_list(
                         dict_asset[DISPATCH_PRICE][VALUE], i
                     ),
                 )
 
             efficiencies = {}
             for i, efficiency in enumerate(dict_asset[EFFICIENCY][VALUE]):
-                efficiencies[
-                    kwargs[OEMOF_BUSSES][dict_asset[OUTFLOW_DIRECTION][i]]
-                ] = efficiency
+                efficiencies[kwargs[OEMOF_BUSSES][dict_asset[OUTFLOW_DIRECTION][i]]] = (
+                    efficiency
+                )
 
         else:
             # multiple inputs and multiple outputs
             inputs_names = ", ".join([f"'{n}'" for n in dict_asset[INFLOW_DIRECTION]])
             outputs_names = ", ".join([f"'{n}'" for n in dict_asset[OUTFLOW_DIRECTION]])
             missing_dispatch_prices_or_efficiencies = (
                 f"You defined multiple values for parameter '{INFLOW_DIRECTION}'"
@@ -637,23 +646,41 @@
                 f" at the moment."
             )
             logging.error(missing_dispatch_prices_or_efficiencies)
             raise ValueError(missing_dispatch_prices_or_efficiencies)
     else:
         # single input and single output
 
+        min_load_opts = {"min": 0, "max": 1}
+        min_load = dict_asset.get(SOC_MIN, None)
+        if min_load is not None:
+            if min_load[VALUE] != 0:
+                logging.warning(
+                    f"Minimal load of {min_load[VALUE]} was set to asset {dict_asset[LABEL]}"
+                )
+            min_load_opts["min"] = min_load[VALUE]
+        max_load = dict_asset.get(SOC_MAX, None)
+        if max_load is not None:
+            if max_load[VALUE] != 1:
+                logging.warning(
+                    f"Maximal load of {max_load[VALUE]} was set to asset {dict_asset[LABEL]}"
+                )
+
+            min_load_opts["max"] = max_load[VALUE]
+
         check_list_parameters_transformers_single_input_single_output(
             dict_asset, model.timeindex.size
         )
 
         inputs = {kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION]]: solph.Flow()}
         outputs = {
             kwargs[OEMOF_BUSSES][dict_asset[OUTFLOW_DIRECTION]]: solph.Flow(
                 nominal_value=dict_asset[INSTALLED_CAP][VALUE],
                 variable_costs=dict_asset[DISPATCH_PRICE][VALUE],
+                **min_load_opts,
             )
         }
         efficiencies = {
             kwargs[OEMOF_BUSSES][dict_asset[OUTFLOW_DIRECTION]]: dict_asset[EFFICIENCY][
                 VALUE
             ]
         }
@@ -687,18 +714,22 @@
     -------
     Indirectly updated `model` and dict of asset in `kwargs` with the transformer object.
 
     """
     missing_dispatch_prices_or_efficiencies = None
 
     investment_bus = dict_asset.get(INVESTMENT_BUS)
+    invest_opts = {}
+    if dict_asset[MAXIMUM_ADD_CAP][VALUE] is not None:
+        invest_opts["maximum"] = dict_asset[MAXIMUM_ADD_CAP][VALUE]
+
     investment = solph.Investment(
         ep_costs=dict_asset[SIMULATION_ANNUITY][VALUE],
-        maximum=dict_asset[MAXIMUM_ADD_CAP][VALUE],
         existing=dict_asset[INSTALLED_CAP][VALUE],
+        **invest_opts,
     )
 
     # check if the transformer has multiple input or multiple output busses
     # the investment object is always in the output bus
     if isinstance(dict_asset[INFLOW_DIRECTION], list) or isinstance(
         dict_asset[OUTFLOW_DIRECTION], list
     ):
@@ -737,17 +768,17 @@
                 kwargs[OEMOF_BUSSES][bus]: solph.Flow(
                     investment=investment if bus == investment_bus else None
                 )
             }
 
             efficiencies = {}
             for i, efficiency in enumerate(dict_asset[EFFICIENCY][VALUE]):
-                efficiencies[
-                    kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION][i]]
-                ] = efficiency
+                efficiencies[kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION][i]]] = (
+                    efficiency
+                )
 
         elif isinstance(dict_asset[INFLOW_DIRECTION], str) and isinstance(
             dict_asset[OUTFLOW_DIRECTION], list
         ):
             # single input and multiple outputs
             num_outputs = len(dict_asset[OUTFLOW_DIRECTION])
             if get_length_if_list(dict_asset[EFFICIENCY][VALUE]) != num_outputs:
@@ -797,14 +828,40 @@
     else:
         check_list_parameters_transformers_single_input_single_output(
             dict_asset, model.timeindex.size
         )
 
         # single input and single output
 
+        min_load_opts = {"min": 0, "max": 1}
+        min_load = dict_asset.get(SOC_MIN, None)
+        if min_load is not None:
+            if min_load[VALUE] != 0:
+                logging.warning(
+                    f"Minimal load of {min_load[VALUE]} was set to asset {dict_asset[LABEL]}"
+                )
+                min_load_opts["nonconvex"] = solph.NonConvex()
+            min_load_opts["min"] = min_load[VALUE]
+
+        max_load = dict_asset.get(SOC_MAX, None)
+        if max_load is not None:
+            if max_load[VALUE] != 1:
+                logging.warning(
+                    f"Maximal load of {max_load[VALUE]} was set to asset {dict_asset[LABEL]}"
+                )
+                min_load_opts["nonconvex"] = solph.NonConvex()
+
+            min_load_opts["max"] = max_load[VALUE]
+
+        if "nonconvex" in min_load_opts:
+            if invest_opts.get("maximum", None) is None:
+                raise ValueError(
+                    f"You need to provide a maximum_capacity to the asset {dict_asset[LABEL]}, if you set a minimal/maximal load different from 0/1"
+                )
+
         if investment_bus is None:
             investment_bus = dict_asset[OUTFLOW_DIRECTION]
 
         bus = dict_asset[INFLOW_DIRECTION]
         inputs = {
             kwargs[OEMOF_BUSSES][bus]: solph.Flow(
                 investment=investment if bus == investment_bus else None
@@ -822,14 +879,15 @@
                 )
             }
         else:
             outputs = {
                 kwargs[OEMOF_BUSSES][bus]: solph.Flow(
                     investment=investment if bus == investment_bus else None,
                     variable_costs=dict_asset[DISPATCH_PRICE][VALUE],
+                    **min_load_opts,
                 )
             }
 
         efficiencies = {
             kwargs[OEMOF_BUSSES][dict_asset[OUTFLOW_DIRECTION]]: dict_asset[EFFICIENCY][
                 VALUE
             ]
@@ -838,15 +896,14 @@
     if missing_dispatch_prices_or_efficiencies is None:
         t = solph.components.Converter(
             label=dict_asset[LABEL],
             inputs=inputs,
             outputs=outputs,
             conversion_factors=efficiencies,
         )
-
         model.add(t)
         kwargs[OEMOF_TRANSFORMER].update({dict_asset[LABEL]: t})
 
 
 def storage_fix(model, dict_asset, **kwargs):
     r"""
     Defines a storage with a fixed capacity.
@@ -992,15 +1049,15 @@
             VALUE
         ],  # storing efficiency
         outflow_conversion_factor=dict_asset[OUTPUT_POWER][EFFICIENCY][
             VALUE
         ],  # efficiency of discharge
         invest_relation_input_capacity=dict_asset[INPUT_POWER][C_RATE][VALUE],
         # storage can be charged with invest_relation_output_capacity*capacity in one timeperiod
-        invest_relation_output_capacity=dict_asset[OUTPUT_POWER][C_RATE][VALUE]
+        invest_relation_output_capacity=dict_asset[OUTPUT_POWER][C_RATE][VALUE],
         # storage can be emptied with invest_relation_output_capacity*capacity in one timeperiod
     )
     model.add(storage)
     kwargs[OEMOF_GEN_STORAGE].update({dict_asset[LABEL]: storage})
 
 
 def source_non_dispatchable_fix(model, dict_asset, **kwargs):
@@ -1124,15 +1181,16 @@
                 # add emission_factor for emission contraint
                 custom_attributes=dict(
                     emission_factor=dict_asset[EMISSION_FACTOR][VALUE]
                 ),
             )
         }
         source_dispatchable = solph.components.Source(
-            label=dict_asset[LABEL], outputs=outputs,
+            label=dict_asset[LABEL],
+            outputs=outputs,
         )
     else:
         if TIMESERIES in dict_asset:
             logging.info(
                 f"Asset {dict_asset[LABEL]} is introduced as a dispatchable source with an availability schedule."
             )
             logging.debug(
@@ -1191,15 +1249,16 @@
                 # add emission_factor for emission contraint
                 custom_attributes=dict(
                     emission_factor=dict_asset[EMISSION_FACTOR][VALUE]
                 ),
             )
         }
         source_dispatchable = solph.components.Source(
-            label=dict_asset[LABEL], outputs=outputs,
+            label=dict_asset[LABEL],
+            outputs=outputs,
         )
     else:
         if TIMESERIES in dict_asset:
             logging.info(
                 f"Asset {dict_asset[LABEL]} is introduced as a dispatchable source with an availability schedule."
             )
             logging.debug(
@@ -1210,15 +1269,16 @@
         outputs = {
             kwargs[OEMOF_BUSSES][dict_asset[OUTFLOW_DIRECTION]]: solph.Flow(
                 nominal_value=dict_asset[INSTALLED_CAP][VALUE],
                 variable_costs=dict_asset[DISPATCH_PRICE][VALUE],
             )
         }
         source_dispatchable = solph.components.Source(
-            label=dict_asset[LABEL], outputs=outputs,
+            label=dict_asset[LABEL],
+            outputs=outputs,
         )
     model.add(source_dispatchable)
     kwargs[OEMOF_SOURCE].update({dict_asset[LABEL]: source_dispatchable})
     logging.debug(
         f"Added: Dispatchable source {dict_asset[LABEL]} (fixed capacity) to bus {dict_asset[OUTFLOW_DIRECTION]}."
     )
 
@@ -1258,15 +1318,18 @@
             kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION]]: solph.Flow(
                 variable_costs=dict_asset[DISPATCH_PRICE][VALUE],
                 investment=solph.Investment(),
             )
         }
 
     # create and add excess electricity sink to micro_grid_system - variable
-    sink_dispatchable = solph.components.Sink(label=dict_asset[LABEL], inputs=inputs,)
+    sink_dispatchable = solph.components.Sink(
+        label=dict_asset[LABEL],
+        inputs=inputs,
+    )
     model.add(sink_dispatchable)
     kwargs[OEMOF_SINK].update({dict_asset[LABEL]: sink_dispatchable})
     logging.debug(
         f"Added: Dispatchable sink {dict_asset[LABEL]} (to be capacity optimized) to bus {dict_asset[INFLOW_DIRECTION]}.",
     )
 
 
@@ -1300,22 +1363,106 @@
         inputs = {
             kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION]]: solph.Flow(
                 fix=dict_asset[TIMESERIES], nominal_value=1
             )
         }
 
     # create and add demand sink to micro_grid_system - fixed
-    sink_demand = solph.components.Sink(label=dict_asset[LABEL], inputs=inputs,)
+    sink_demand = solph.components.Sink(
+        label=dict_asset[LABEL],
+        inputs=inputs,
+    )
     model.add(sink_demand)
     kwargs[OEMOF_SINK].update({dict_asset[LABEL]: sink_demand})
     logging.debug(
         f"Added: Non-dispatchable sink {dict_asset[LABEL]} to bus {dict_asset[INFLOW_DIRECTION]}"
     )
 
 
+def sink_demand_reduction(model, dict_asset, **kwargs):
+    r"""
+    Defines a non dispatchable sink to serve critical and non-critical demand.
+
+    See :py:func:`~.sink` for more information, including parameters.
+
+    Notes
+    -----
+    Tested with:
+    - test_sink_non_dispatchable_single_input_bus()
+    - test_sink_non_dispatchable_multiple_input_busses()
+
+    Returns
+    -------
+    Indirectly updated `model` and dict of asset in `kwargs` with the sink object.
+
+    """
+    demand_reduction_factor = 1 - dict_asset[EFFICIENCY][VALUE]
+    tot_demand = dict_asset[TIMESERIES]
+    non_critical_demand_ts = tot_demand * demand_reduction_factor
+    non_critical_demand_peak = non_critical_demand_ts.max()
+    if non_critical_demand_peak == 0:
+        max_non_critical = 1
+    else:
+        max_non_critical = non_critical_demand_ts / non_critical_demand_peak
+    critical_demand_ts = tot_demand * dict_asset[EFFICIENCY][VALUE]
+
+    # check if the sink has multiple input busses
+    if isinstance(dict_asset[INFLOW_DIRECTION], list):
+        raise (
+            ValueError(
+                f"The reducable demand {dict_asset[LABEL]} does not support multiple input busses"
+            )
+        )
+        # inputs_noncritical = {}
+        # inputs_critical = {}
+        # index = 0
+        # for bus in dict_asset[INFLOW_DIRECTION]:
+        #     inputs_critical[kwargs[OEMOF_BUSSES][bus]] = solph.Flow(
+        #         fix=dict_asset[TIMESERIES], nominal_value=1
+        #     )
+        #     index += 1
+    else:
+        inputs_noncritical = {
+            kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION]]: solph.Flow(
+                min=0,
+                max=max_non_critical,
+                nominal_value=non_critical_demand_peak,
+                variable_costs=-1e-15,
+            )
+        }
+        inputs_critical = {
+            kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION]]: solph.Flow(
+                fix=critical_demand_ts, nominal_value=1
+            )
+        }
+
+    non_critical_demand = solph.components.Sink(
+        label=reducable_demand_name(dict_asset[LABEL]),
+        inputs=inputs_noncritical,
+    )
+    critical_demand = solph.components.Sink(
+        label=reducable_demand_name(dict_asset[LABEL], critical=True),
+        inputs=inputs_critical,
+    )
+
+    # create and add demand sink and critical demand sink
+
+    model.add(critical_demand)
+    model.add(non_critical_demand)
+    kwargs[OEMOF_SINK].update(
+        {reducable_demand_name(dict_asset[LABEL]): non_critical_demand}
+    )
+    kwargs[OEMOF_SINK].update(
+        {reducable_demand_name(dict_asset[LABEL], critical=True): critical_demand}
+    )
+    logging.debug(
+        f"Added: Reducable Non-dispatchable sink {dict_asset[LABEL]} to bus {dict_asset[INFLOW_DIRECTION]}"
+    )
+
+
 def chp_fix(model, dict_asset, **kwargs):
     r"""
     Extraction turbine chp from Oemof solph. Extraction turbine must have one input and two outputs
     Notes
     -----
     Tested with:
     - test_to_be_written()
@@ -1374,15 +1521,15 @@
 def chp_optimize(model, dict_asset, **kwargs):
     r"""
     Extraction turbine chp from Oemof solph. Extraction turbine must have one input and two outputs
     Notes
     -----
     Tested with:
     - test_to_be_written()
-    
+
     Returns
     -------
     Indirectly updated `model` and dict of asset in `kwargs` with the extraction turbine component.
 
     """
 
     inputs = {kwargs[OEMOF_BUSSES][dict_asset[INFLOW_DIRECTION]]: solph.Flow()}
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/D2_model_constraints.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/D2_model_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 This module gathers all constraints that can be added to the MVS optimisation. 
 we will probably require another input CSV file or further parameters in simulation_settings.
 
 Future constraints are discussed in issue #133 (https://github.com/rl-institut/multi-vector-simulator/issues/133)
 
 constraints should be tested in-code (examples) and by comparing the lp file generated.
 """
+
 import logging
 import pyomo.environ as po
 from oemof.solph import constraints
 
 from multi_vector_simulator.utils.constants import DEFAULT_WEIGHTS_ENERGY_CARRIERS
 
 from multi_vector_simulator.utils.constants_json_strings import (
@@ -174,15 +175,18 @@
     """
 
     if dict_values[CONSTRAINTS][MINIMAL_RENEWABLE_FACTOR][VALUE] > 0:
 
         (
             renewable_assets,
             non_renewable_assets,
-        ) = prepare_constraint_minimal_renewable_share(dict_values, dict_model,)
+        ) = prepare_constraint_minimal_renewable_share(
+            dict_values,
+            dict_model,
+        )
 
         def renewable_share_rule(model):
             renewable_generation = 0
             total_generation = 0
 
             # Get the flows from all renewable assets
             for asset in renewable_assets:
@@ -233,15 +237,16 @@
     else:
         answer = None
 
     return answer
 
 
 def prepare_constraint_minimal_renewable_share(
-    dict_values, dict_model,
+    dict_values,
+    dict_model,
 ):
     r"""
     Prepare creating the minimal renewable factor constraint by processing dict_values
 
     Parameters
     ----------
     dict_values: dict
@@ -425,18 +430,24 @@
     - Test_Constraints.test_benchmark_minimal_degree_of_autonomy()
     """
 
     logging.debug(f"Data considered for the minimal degree of autonomy constraint:")
 
     if dict_values[CONSTRAINTS][MINIMAL_DEGREE_OF_AUTONOMY][VALUE] > 0:
 
-        demands = prepare_demand_assets(dict_values, dict_model,)
+        demands = prepare_demand_assets(
+            dict_values,
+            dict_model,
+        )
 
-        energy_provider_consumption_sources = prepare_energy_provider_consumption_sources(
-            dict_values, dict_model,
+        energy_provider_consumption_sources = (
+            prepare_energy_provider_consumption_sources(
+                dict_values,
+                dict_model,
+            )
         )
 
         def degree_of_autonomy_rule(model):
             total_demand = 0
             total_consumption_from_energy_provider = 0
 
             # Get the flows from demands and add weighing
@@ -490,15 +501,16 @@
     else:
         answer = None
 
     return answer
 
 
 def prepare_demand_assets(
-    dict_values, dict_model,
+    dict_values,
+    dict_model,
 ):
     r"""
     Perpare demand assets by processing `dict_values`
 
     Used for the following constraints:
     - minimal degree of autonomy
 
@@ -553,15 +565,16 @@
     demand_string = ", ".join(map(str, demand_list))
 
     logging.debug(f"Demands: {demand_string}")
     return demands
 
 
 def prepare_energy_provider_consumption_sources(
-    dict_values, dict_model,
+    dict_values,
+    dict_model,
 ):
     r"""
     Prepare energy provider consumption sources by processing `dict_values`.
 
     Used for the following constraints:
     - minimal degree of autonomy
     - net zero energy (NZE)
@@ -620,15 +633,16 @@
     logging.debug(
         f"Energy provider consumption sources: {dso_consumption_source_string}"
     )
     return energy_provider_consumption_sources
 
 
 def prepare_energy_provider_feedin_sinks(
-    dict_values, dict_model,
+    dict_values,
+    dict_model,
 ):
     r"""
     Prepare energy provider feedin sinks by processing `dict_values`.
 
     Used for the following constraints:
     - net zero energy (NZE)
 
@@ -715,19 +729,23 @@
     """
 
     logging.debug(f"Data considered for the net zero energy (NZE) constraint:")
 
     if dict_values[CONSTRAINTS][NET_ZERO_ENERGY][VALUE] == True:
 
         energy_provider_feedin_sinks = prepare_energy_provider_feedin_sinks(
-            dict_values, dict_model,
+            dict_values,
+            dict_model,
         )
 
-        energy_provider_consumption_sources = prepare_energy_provider_consumption_sources(
-            dict_values, dict_model,
+        energy_provider_consumption_sources = (
+            prepare_energy_provider_consumption_sources(
+                dict_values,
+                dict_model,
+            )
         )
 
         def net_zero_energy(model):
             total_feedin_to_energy_provider = 0
             total_consumption_from_energy_provider = 0
 
             # Get the flows from provider sources and add weighing
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E0_evaluation.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/E0_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,16 @@
     E1.get_timeseries_per_bus(dict_values, bus_data)
 
     # Store all information related to storages in bus_data, as storage capacity acts as a bus
     for storage in dict_values[ENERGY_STORAGE]:
         bus_data.update(
             {
                 dict_values[ENERGY_STORAGE][storage][LABEL]: solph.views.node(
-                    results_main, dict_values[ENERGY_STORAGE][storage][LABEL],
+                    results_main,
+                    dict_values[ENERGY_STORAGE][storage][LABEL],
                 )
             }
         )
         E1.get_storage_results(
             dict_values[SIMULATION_SETTINGS],
             bus_data[dict_values[ENERGY_STORAGE][storage][LABEL]],
             dict_values[ENERGY_STORAGE][storage],
@@ -156,17 +157,17 @@
                 )
                 + dict_values[ENERGY_STORAGE][storage][STORAGE_CAPACITY][
                     OPTIMIZED_ADD_CAP
                 ][UNIT]
                 + f") {SOC}"
             )
 
-            dict_values[OPTIMIZED_FLOWS][inflow_direction][
-                timeseries_name
-            ] = dict_values[ENERGY_STORAGE][storage][TIMESERIES_SOC]
+            dict_values[OPTIMIZED_FLOWS][inflow_direction][timeseries_name] = (
+                dict_values[ENERGY_STORAGE][storage][TIMESERIES_SOC]
+            )
 
     for group in [ENERGY_CONVERSION, ENERGY_PRODUCTION, ENERGY_CONSUMPTION]:
         for asset in dict_values[group]:
             E1.get_results(
                 settings=dict_values[SIMULATION_SETTINGS],
                 bus_data=bus_data,
                 dict_asset=dict_values[group][asset],
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E1_process_results.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/E1_process_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 Module E1 processes the oemof results.
 - receive time series per bus for all assets
 - write time series to dictionary
 - get optimal capacity of optimized assets
 - add the evaluation of time series
 
 """
+
 import logging
 import copy
 import pandas as pd
-
+from multi_vector_simulator.utils.helpers import reducable_demand_name
 from multi_vector_simulator.utils.constants import TYPE_NONE, TOTAL_FLOW
 from multi_vector_simulator.utils.constants_json_strings import (
     ECONOMIC_DATA,
     FLOW,
     INSTALLED_CAP,
     INPUT_POWER,
     OUTPUT_POWER,
@@ -66,14 +67,15 @@
     EMISSION_FACTOR,
     TOTAL_EMISSIONS,
     TIMESERIES_SOC,
     KPI_UNCOUPLED_DICT,
     FIX_COST,
     LIFETIME_PRICE_DISPATCH,
     AVERAGE_SOC,
+    TYPE_ASSET,
 )
 
 # Oemof.solph variables
 OEMOF_FLOW = "flow"
 OEMOF_SEQUENCES = "sequences"
 OEMOF_INVEST = "invest"
 OEMOF_SCALARS = "scalars"
@@ -730,16 +732,32 @@
     Returns
     -------
     Indirectly updates `dict_asset` with the flow of `bus`, the total flow, the annual
     total flow, the maximum of the flow ('peak_flow') and the average value of
     the flow ('average_flow').
 
     """
-    flow = bus[OEMOF_SEQUENCES][(flow_tuple, OEMOF_FLOW)]
-    flow = cut_below_micro(flow, dict_asset[LABEL] + FLOW)
+
+    if dict_asset.get(TYPE_ASSET) == "reducable_demand":
+        flow_tuple = (flow_tuple[0], reducable_demand_name(dict_asset[LABEL]))
+        flow = bus[OEMOF_SEQUENCES][(flow_tuple, OEMOF_FLOW)]
+        flow = cut_below_micro(flow, dict_asset[LABEL] + FLOW)
+        flow_tuple = (
+            flow_tuple[0],
+            reducable_demand_name(dict_asset[LABEL], critical=True),
+        )
+
+        flow_crit = bus[OEMOF_SEQUENCES][(flow_tuple, OEMOF_FLOW)]
+        flow_crit = cut_below_micro(flow_crit, dict_asset[LABEL] + FLOW)
+        flow = flow + flow_crit
+
+    else:
+        flow = bus[OEMOF_SEQUENCES][(flow_tuple, OEMOF_FLOW)]
+        flow = cut_below_micro(flow, dict_asset[LABEL] + FLOW)
+
     add_info_flows(
         evaluated_period=settings[EVALUATED_PERIOD][VALUE],
         dict_asset=dict_asset,
         flow=flow.dropna(),
         bus_name=multi_bus,
     )
     if multi_bus is None:
@@ -976,15 +994,15 @@
     # Energy production and conversion have the same tree structure, can be processed together:
 
     # Add the above dictionaries and lists of keys into new lists for iterating through, later
     comp_dict_list = [dict_energy_production, dict_energy_conversion]
     components_list = [keys_production, keys_conversion]
 
     # Defining the columns of the table and filling them up with the appropriate data
-    for (component_key, comp_dict) in zip(components_list, comp_dict_list):
+    for component_key, comp_dict in zip(components_list, comp_dict_list):
         for comps in component_key:
             # Define whether optimization takes place
             optimize = translate_optimizeCap_from_boolean_to_yes_no(
                 comp_dict[comps][OPTIMIZE_CAP][VALUE]
             )
             components.update(
                 {
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E2_economics.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/E2_economics.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,18 +165,20 @@
     )
 
     dict_asset.update(
         {COST_INVESTMENT: {VALUE: costs_investment_lifetime, UNIT: economic_data[CURR]}}
     )
 
     # Operation and management expenditures over the project lifetime
-    operation_and_management_expenditures = calculate_operation_and_management_expenditures(
-        specific_om_cost=dict_asset[LIFETIME_SPECIFIC_COST_OM][VALUE],
-        installed_capacity=dict_asset[INSTALLED_CAP][VALUE],
-        optimized_add_capacity=dict_asset[OPTIMIZED_ADD_CAP][VALUE],
+    operation_and_management_expenditures = (
+        calculate_operation_and_management_expenditures(
+            specific_om_cost=dict_asset[LIFETIME_SPECIFIC_COST_OM][VALUE],
+            installed_capacity=dict_asset[INSTALLED_CAP][VALUE],
+            optimized_add_capacity=dict_asset[OPTIMIZED_ADD_CAP][VALUE],
+        )
     )
     dict_asset.update(
         {
             COST_OM: {
                 VALUE: operation_and_management_expenditures,
                 UNIT: economic_data[CURR],
             }
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E3_indicator_calculation.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/E3_indicator_calculation.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 - calculate total generation of each asset and total_internal_generation
 - calculate total feedin electricity equivalent
 - calculate energy flows between sectors
 - calculate degree of sector coupling
 - calculate onsite energy fraction (OEF)
 - calculate onsite energy matching (OEM)
 """
+
 import logging
 
 from multi_vector_simulator.utils.constants import DEFAULT_WEIGHTS_ENERGY_CARRIERS
 from multi_vector_simulator.utils.constants import PROJECT_DATA
 from multi_vector_simulator.utils.constants_json_strings import (
     VALUE,
     LABEL,
@@ -857,15 +858,15 @@
     Determines onsite energy fraction (OEF), i.e. self-consumption, and adds KPI to dict_values
 
     Parameters
     ----------
     dict_values: dict
         dict with all project information and results
         after applying total_renewable_and_non_renewable_energy_origin
-    
+
     Returns
     -------
     None
         updated dict_values with onsite energy fraction KPI
 
     Tested with
     - test_add_onsite_energy_fraction()
@@ -938,15 +939,15 @@
     Parameters
     ----------
     dict_values: dict
         dict with all project information and results
         after applying total_renewable_and_non_renewable_energy_origin and
         total_demand_and_excess_each_sector and
         add_onsite_energy_fraction
-    
+
     Returns
     -------
     None
         updated dict_values with onsite energy matching KPI
 
     Tested with
     - test_add_onsite_energy_matching()
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/E4_verification.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/E4_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F0_output.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/F0_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 - Execute function: plot optimised capacities as a barchart (F1)
 - Execute function: plot all annuities as a barchart (F1)
 - Store scalars/KPI to excel
 - Process dictionary so that it can be stored to Json
 - Store dictionary to Json
 """
 
-
 import json
 import logging
 import os
 
 import pandas as pd
 
 from multi_vector_simulator.B0_data_input_json import convert_from_special_types_to_json
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F1_plotting.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/F1_plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -857,15 +857,16 @@
             scale=5,
         )
 
     return fig
 
 
 def plot_optimized_capacities(
-    dict_values, file_path=None,
+    dict_values,
+    file_path=None,
 ):
     """Plot capacities as a bar chart.
 
     Parameters
     ----------
     dict_values :
         dict Of all input and output parameters up to F0
@@ -878,15 +879,16 @@
     -------
     Dict with html DOM id for the figure as key and :class:`plotly.graph_objs.Figure` as value
     """
 
     # Add dataframe to hold all the KPIs and optimized additional capacities
     df_capacities = dict_values[KPI][KPI_SCALAR_MATRIX].copy(deep=True)
     df_capacities.drop(
-        columns=[TOTAL_FLOW, ANNUAL_TOTAL_FLOW, PEAK_FLOW, AVERAGE_FLOW], inplace=True,
+        columns=[TOTAL_FLOW, ANNUAL_TOTAL_FLOW, PEAK_FLOW, AVERAGE_FLOW],
+        inplace=True,
     )
     df_capacities.reset_index(drop=True, inplace=True)
 
     x_values = []
     y_values = []
     legends = []
 
@@ -996,15 +998,19 @@
             "text": plot_title,
             "y": 0.90,
             "x": 0.5,
             "font_size": 23,
             "xanchor": "center",
             "yanchor": "top",
         },
-        legend=dict(y=0.5, traceorder="normal", font=dict(color="black"),),
+        legend=dict(
+            y=0.5,
+            traceorder="normal",
+            font=dict(color="black"),
+        ),
     )
 
     if file_path is not None:
         # Function call to save the Plotly plot to the disk
         save_plots_to_disk(
             fig_obj=fig,
             file_path=file_path,
@@ -1164,15 +1170,21 @@
             "yanchor": "top",
             "pad": {"r": 5, "l": 5, "b": 5, "t": 5},
         },
         font_family="sans-serif",
         height=500,
         width=700,
         autosize=True,
-        legend=dict(orientation="v", y=0.5, yanchor="middle", x=0.95, xanchor="right",),
+        legend=dict(
+            orientation="v",
+            y=0.5,
+            yanchor="middle",
+            x=0.95,
+            xanchor="right",
+        ),
         margin=dict(l=10, r=10, b=50, pad=2),
         uniformtext_minsize=18,
     )
     fig.update_traces(hoverinfo="label+percent", textinfo="label", textfont_size=18)
 
     if file_path is not None:
         # Function call to save the Plotly plot to the disk
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F2_autoreport.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/F2_autoreport.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,18 @@
 
     browser = await launch()
     page = await browser.newPage()
     await page.goto(
         "http://127.0.0.1:8050", {"waitUntil": "domcontentloaded", "timeout": 120000}
     )
     await page.waitForSelector(
-        ".dash-cell", {"visible": "true",},
+        ".dash-cell",
+        {
+            "visible": "true",
+        },
     )
     await page.pdf({"path": path_pdf_report, "format": "A4", "printBackground": True})
     await browser.close()
     print("*" * 10)
     print("The report was saved under {}".format(path_pdf_report))
     print("You can now quit with ctlr+c")
     print("*" * 10)
@@ -355,15 +358,17 @@
                 children=html.Ul(children=[html.Li(v) for k, v in log_dict.items()]),
             ),
         ],
     )
 
 
 def insert_plotly_figure(
-    fig, id_plot=None, print_only=False,
+    fig,
+    id_plot=None,
+    print_only=False,
 ):
     r"""
     Insert a plotly figure in a dash app layout
 
     Parameters
     ----------
     fig: :class:`plotly.graph_objs.Figure`
@@ -402,15 +407,20 @@
             ),
         )
     ]
 
     # Dynamic plotly figure for the app
     if print_only is False:
         rendered_plots.append(
-            dcc.Graph(className="no-print", id=id_plot, figure=fig, responsive=True,)
+            dcc.Graph(
+                className="no-print",
+                id=id_plot,
+                figure=fig,
+                responsive=True,
+            )
         )
 
     return html.Div(children=rendered_plots)
 
 
 def ready_timeseries_plots(
     dict_values, data_type=DEMANDS, only_print=False, sector_demands=None
@@ -863,23 +873,25 @@
                                         style={"font-weight": "bold"},
                                     ),
                                     f"{scenarioName}",
                                 ],
                             ),
                             html.Div(
                                 className="cell imp_info2",
-                                children=[]
-                                if scenario_description == ""
-                                else [
-                                    html.Span(
-                                        "Scenario description  : ",
-                                        style={"font-weight": "bold"},
-                                    ),
-                                    f"{scenario_description}",
-                                ],
+                                children=(
+                                    []
+                                    if scenario_description == ""
+                                    else [
+                                        html.Span(
+                                            "Scenario description  : ",
+                                            style={"font-weight": "bold"},
+                                        ),
+                                        f"{scenario_description}",
+                                    ]
+                                ),
                             ),
                             html.Div(
                                 className="blockoftext",
                                 children=[
                                     "The energy system with the ",
                                     html.Span(
                                         f"{projectName}", style={"font-style": "italic"}
@@ -917,31 +929,34 @@
                                 children=[
                                     html.Div(
                                         className="cell small-6 location-map-column",
                                         children=[
                                             html.H4(["Project Location"]),
                                             html.Iframe(
                                                 srcDoc=open(
-                                                    leaflet_map_path, "r",
+                                                    leaflet_map_path,
+                                                    "r",
                                                 ).read(),
                                                 height="400",
                                             ),
                                             html.Div(
                                                 className="staticimagepdf print-only",
                                                 children=[
                                                     insert_body_text(
                                                         "The blue dot in the below map indicates "
                                                         "the location of the project."
                                                     ),
                                                     html.Img(
                                                         id="staticmapimage",
-                                                        src=""
-                                                        if MAP_STATIC is None
-                                                        else "data:image/png;base64,{}".format(
-                                                            MAP_STATIC.decode()
+                                                        src=(
+                                                            ""
+                                                            if MAP_STATIC is None
+                                                            else "data:image/png;base64,{}".format(
+                                                                MAP_STATIC.decode()
+                                                            )
                                                         ),
                                                         width="400px",
                                                         style={"marginLeft": "30px"},
                                                         alt="Map of the location",
                                                     ),
                                                 ],
                                             ),
@@ -1007,15 +1022,17 @@
                                 "The capacity optimization of components that were to be used resulted in:"
                             ),
                             make_dash_data_table(df_scalar_matrix),
                             insert_body_text(
                                 "With this, the demands are met with the following dispatch schedules:"
                             ),
                             html.Div(
-                                children=ready_flows_plots(dict_values=results_json,)
+                                children=ready_flows_plots(
+                                    dict_values=results_json,
+                                )
                             ),
                             html.Div(
                                 className="add-cap-plot",
                                 children=ready_capacities_plots(
                                     dict_values=results_json
                                 ),
                             ),
@@ -1024,29 +1041,31 @@
                             ),
                             make_dash_data_table(df_kpi_sectors),
                         ],
                     ),
                     insert_subsection(
                         title="Sankey diagram",
                         content=ready_sankey_diagram(
-                            dict_values=results_json, only_print=False,
+                            dict_values=results_json,
+                            only_print=False,
                         ),
                     ),
                     insert_subsection(
                         title="Economic Evaluation",
                         content=[
                             insert_body_text(
                                 "The following installation and operation costs "
                                 "result from capacity and dispatch optimization:"
                             ),
                             make_dash_data_table(df_cost_matrix),
                             html.Div(
                                 className="add-pie-plots",
                                 children=ready_costs_pie_plots(
-                                    dict_values=results_json, only_print=False,
+                                    dict_values=results_json,
+                                    only_print=False,
                                 ),
                             ),
                         ],
                     ),
                     insert_subsection(
                         title="Energy System: Key Performance Indicators (KPIs)",
                         content=[
@@ -1061,15 +1080,17 @@
                 ],
             ),
             html.Section(
                 className="cell small-10 small_offset-1 grid-x",
                 children=[
                     html.Div(
                         className="cell",
-                        children=[insert_headings(heading_text="Logging Messages"),],
+                        children=[
+                            insert_headings(heading_text="Logging Messages"),
+                        ],
                     ),
                     html.Div(
                         children=[
                             insert_subsection(
                                 title="Warning Messages",
                                 content=insert_log_messages(
                                     log_dict=results_json[SIMULATION_RESULTS][LOGS][
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/F3_debug.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/F3_debug.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/cli.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,16 @@
         save_energy_system_graph = True
     else:
         save_energy_system_graph = False
 
     print("")
     logging.debug("Accessing script: D0_modelling_and_optimization")
     results_meta, results_main = D0.run_oemof(
-        dict_values, save_energy_system_graph=save_energy_system_graph,
+        dict_values,
+        save_energy_system_graph=save_energy_system_graph,
     )
 
     print("")
     logging.debug("Accessing script: E0_evaluation")
     E0.evaluate_dict(dict_values, results_main, results_meta)
 
     logging.debug("Accessing script: F0_outputs")
@@ -185,15 +186,14 @@
         path_pdf_report=user_input.get("path_pdf_report", None),
         path_png_figs=user_input.get("path_png_figs", None),
     )
     return 1
 
 
 def report(pdf=None, path_simulation_output_json=None, path_pdf_report=None):
-
     """Display the report of a MVS simulation
 
     Command line use:
 
     .. code-block:: bash
 
         mvs_report [-h] [-i [PATH_SIM_OUTPUT]] [-o [REPORT_PATH]] [-pdf]
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/MVS_parameters_list.csv` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/MVS_parameters_list.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/assets/styles.css` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/assets/styles.css`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/mvs_config.json` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/mvs_config.json`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/server.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,17 @@
             )
             df = pd.DataFrame(data=js["data"], columns=mindex)
 
             ts_df = df.iloc[:-1]
             ts_index = pd.to_datetime(js["index"][:-1], unit="ms")
             investments = df.iloc[-1]
             ts_df.index = ts_index
-
+        for extra_var in ["status", "status_nominal"]:
+            if extra_var in ts_df:
+                ts_df.drop(extra_var, axis=1, inplace=True)
         super().__init__(
             data=ts_df.T.to_dict(orient="split")["data"],
             index=mindex,
             columns=ts_df.index,
         )
 
         self["investments"] = investments
@@ -185,15 +187,15 @@
             self.index.get_level_values("asset") == asset_name, "investments"
         ].dropna()
         if len(optimized_capacity) == 1:
             optimized_capacity = optimized_capacity[0]
         return optimized_capacity
 
 
-def run_simulation(json_dict, epa_format=True, **kwargs):
+def run_simulation(json_dict, epa_format=True, verbatim=False, **kwargs):
     r"""
      Starts MVS tool simulation from an input json file
 
      Parameters
     -----------
      json_dict: dict
          json from http request
@@ -305,15 +307,17 @@
                 ] = corrected_optimized_capacity
 
     dict_values["raw_results"] = br.to_json()  # to_dict(orient="split") #
 
     logging.debug("Convert results to json")
 
     if epa_format is True:
-        epa_dict_values = data_parser.convert_mvs_params_to_epa(dict_values)
+        epa_dict_values = data_parser.convert_mvs_params_to_epa(
+            dict_values, verbatim=verbatim
+        )
 
         json_values = F0.store_as_json(epa_dict_values)
         answer = json.loads(json_values)
     else:
         answer = dict_values
 
     return answer
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/__init__.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,17 @@
 from .exceptions import MissingParameterError
 
 
 class ParameterDocumentation:
     """Helper to access a parameter's information given its variable name"""
 
     def __init__(
-        self, param_info_file, label_header="label",
+        self,
+        param_info_file,
+        label_header="label",
     ):
         self.param_doc = pd.read_csv(param_info_file).set_index(label_header)
         self.label_hdr = label_header
         self.fname = param_info_file
         self.param_format = {"numeric": float, "str": str, "boolean": bool}
 
     @property
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/analysis.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 General Constants
 =================
 """
+
 import os
 from copy import deepcopy
 
 from multi_vector_simulator.utils.constants_json_strings import *
 
 # path to the root of this repository (assumes this file is in src/mvs_eland/utils folder)
 REPO_PATH = os.path.abspath(os.path.curdir)
@@ -159,26 +160,36 @@
     FIX_COST: [
         AGE_INSTALLED,
         DEVELOPMENT_COSTS,
         SPECIFIC_COSTS,
         LIFETIME,
         SPECIFIC_COSTS_OM,
     ],
-    SIMULATION_SETTINGS: [EVALUATED_PERIOD, OUTPUT_LP_FILE, START_DATE, TIMESTEP,],
+    SIMULATION_SETTINGS: [
+        EVALUATED_PERIOD,
+        OUTPUT_LP_FILE,
+        START_DATE,
+        TIMESTEP,
+    ],
     PROJECT_DATA: [
         COUNTRY,
         LATITUDE,
         LONGITUDE,
         PROJECT_ID,
         PROJECT_NAME,
         SCENARIO_ID,
         SCENARIO_NAME,
         SCENARIO_DESCRIPTION,
     ],
-    ECONOMIC_DATA: [CURR, DISCOUNTFACTOR, PROJECT_DURATION, TAX,],
+    ECONOMIC_DATA: [
+        CURR,
+        DISCOUNTFACTOR,
+        PROJECT_DURATION,
+        TAX,
+    ],
 }
 
 # list of csv filename which must be present within the CSV_ELEMENTS folder
 REQUIRED_CSV_FILES = tuple(REQUIRED_CSV_PARAMETERS.keys())
 # list of parameters which must be present within the JSON_FNAME file with the sub-parameters
 # note: if the value of a key is none, then the value is expected to be user-defined and thus cannot
 # be in a required parameters dict
@@ -257,63 +268,108 @@
         WARNING_TEXT: "allows defining the renewable share of the DSO supply (Values: Float). ",
         REQUIRED_IN_CSV_ELEMENTS: [ENERGY_PROVIDERS],
     },
     EMISSION_FACTOR: {
         DEFAULT_VALUE: 0,
         UNIT: TYPE_FLOAT,
         WARNING_TEXT: "allows calculating the total emissions of the energy system (Values: Float). ",
-        REQUIRED_IN_CSV_ELEMENTS: [ENERGY_PRODUCTION, ENERGY_PROVIDERS,],
+        REQUIRED_IN_CSV_ELEMENTS: [
+            ENERGY_PRODUCTION,
+            ENERGY_PROVIDERS,
+        ],
     },
     MAXIMUM_EMISSIONS: {
         DEFAULT_VALUE: DEFAULT_CONSTRAINT_VALUES[MAXIMUM_EMISSIONS][VALUE],
         UNIT: TYPE_NONE,
         WARNING_TEXT: "allows setting a maximum amount of emissions of the optimized energy system (Values: None/Float). ",
-        REQUIRED_IN_CSV_ELEMENTS: [CONSTRAINTS,],
+        REQUIRED_IN_CSV_ELEMENTS: [
+            CONSTRAINTS,
+        ],
     },
     MINIMAL_DEGREE_OF_AUTONOMY: {
         DEFAULT_VALUE: DEFAULT_CONSTRAINT_VALUES[MINIMAL_DEGREE_OF_AUTONOMY][VALUE],
         UNIT: TYPE_FLOAT,
         WARNING_TEXT: "allows setting a minimum degree of autonomy of the optimized energy system (Values: Float). ",
-        REQUIRED_IN_CSV_ELEMENTS: [CONSTRAINTS,],
+        REQUIRED_IN_CSV_ELEMENTS: [
+            CONSTRAINTS,
+        ],
     },
     SCENARIO_DESCRIPTION: {
         DEFAULT_VALUE: "",
         UNIT: TYPE_STR,
         WARNING_TEXT: "allows giving a description for the scenario being simulated",
         REQUIRED_IN_CSV_ELEMENTS: [PROJECT_DATA],
     },
     NET_ZERO_ENERGY: {
         DEFAULT_VALUE: DEFAULT_CONSTRAINT_VALUES[NET_ZERO_ENERGY][VALUE],
         UNIT: TYPE_BOOL,
         WARNING_TEXT: "allows to add a net zero energy constraint to optimization problem (activate by setting to `True`). ",
-        REQUIRED_IN_CSV_ELEMENTS: [CONSTRAINTS,],
+        REQUIRED_IN_CSV_ELEMENTS: [
+            CONSTRAINTS,
+        ],
     },
 }
 
 ENERGY_CARRIER_UNIT = "energy_carrier_unit"
 DEFAULT_WEIGHTS_ENERGY_CARRIERS = {
-    "LNG": {UNIT: "kWh_eleq/kg", VALUE: 12.69270292, ENERGY_CARRIER_UNIT: "kg",},
-    "Crude_oil": {UNIT: "kWh_eleq/kg", VALUE: 11.63042204, ENERGY_CARRIER_UNIT: "kg",},
+    "LNG": {
+        UNIT: "kWh_eleq/kg",
+        VALUE: 12.69270292,
+        ENERGY_CARRIER_UNIT: "kg",
+    },
+    "Crude_oil": {
+        UNIT: "kWh_eleq/kg",
+        VALUE: 11.63042204,
+        ENERGY_CARRIER_UNIT: "kg",
+    },
     "Diesel": {
         UNIT: "kWh_eleq/l",
         VALUE: 9.48030688,
         ENERGY_CARRIER_UNIT: "l",
     },  # https://epact.energy.gov/fuel-conversion-factors, conversion gallon->4.546092 l
-    "Kerosene": {UNIT: "kWh_eleq/l", VALUE: 8.908073954, ENERGY_CARRIER_UNIT: "l",},
-    "Gasoline": {UNIT: "kWh_eleq/l", VALUE: 8.735753974, ENERGY_CARRIER_UNIT: "l",},
-    "LPG": {UNIT: "kWh_eleq/l", VALUE: 6.472821609, ENERGY_CARRIER_UNIT: "l",},
-    "Ethane": {UNIT: "kWh_eleq/l", VALUE: 5.149767951, ENERGY_CARRIER_UNIT: "l",},
+    "Kerosene": {
+        UNIT: "kWh_eleq/l",
+        VALUE: 8.908073954,
+        ENERGY_CARRIER_UNIT: "l",
+    },
+    "Gasoline": {
+        UNIT: "kWh_eleq/l",
+        VALUE: 8.735753974,
+        ENERGY_CARRIER_UNIT: "l",
+    },
+    "LPG": {
+        UNIT: "kWh_eleq/l",
+        VALUE: 6.472821609,
+        ENERGY_CARRIER_UNIT: "l",
+    },
+    "Ethane": {
+        UNIT: "kWh_eleq/l",
+        VALUE: 5.149767951,
+        ENERGY_CARRIER_UNIT: "l",
+    },
     "H2": {
         UNIT: "kWh_eleq/kgH2",
         VALUE: 33.47281985,
         ENERGY_CARRIER_UNIT: "kgH2",
     },  # https://epact.energy.gov/fuel-conversion-factors
-    "Electricity": {UNIT: "kWh_eleq/kWh_el", VALUE: 1, ENERGY_CARRIER_UNIT: "kWh_el",},
-    "Biodiesel": {UNIT: "kWh_eleq/l", VALUE: 0.06290669, ENERGY_CARRIER_UNIT: "l",},
-    "Ethanol": {UNIT: "kWh_eleq/l", VALUE: 0.04242544, ENERGY_CARRIER_UNIT: "l",},
+    "Electricity": {
+        UNIT: "kWh_eleq/kWh_el",
+        VALUE: 1,
+        ENERGY_CARRIER_UNIT: "kWh_el",
+    },
+    "Biodiesel": {
+        UNIT: "kWh_eleq/l",
+        VALUE: 0.06290669,
+        ENERGY_CARRIER_UNIT: "l",
+    },
+    "Ethanol": {
+        UNIT: "kWh_eleq/l",
+        VALUE: 0.04242544,
+        ENERGY_CARRIER_UNIT: "l",
+    },
     "Natural_gas": {
         UNIT: "kWh_eleq/m3",
         VALUE: 0.00933273,
         ENERGY_CARRIER_UNIT: "l",
     },  # https://epact.energy.gov/fuel-conversion-factors, conversion gallon->4.546092 l
     "Gas": {
         UNIT: "kWh_eleq/m3",
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants_json_strings.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/constants_json_strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,18 @@
 DSO_PEAK_DEMAND_PERIOD = "_period"
 CONNECTED_CONSUMPTION_SOURCE = "connected_consumption_sources"
 CONNECTED_PEAK_DEMAND_PRICING_TRANSFORMERS = (
     "connected_peak_demand_pricing_transformers"
 )
 CONNECTED_FEEDIN_SINK = "connected_feedin_sink"
 
+SUFFIX_CRITICAL = "critical"
+SUFFIX_NONCRITICAL = "noncritical"
+REDUCABLE_DEMAND = "reducable_demand"
+
 # Autogenerated assets
 DISPATCHABILITY = "dispatchable"
 AVAILABILITY_DISPATCH = "availability_timeseries"
 ASSET_DICT = "asset_list"
 AUTO_CREATED_HIGHLIGHT = "(@)"
 #######################################
 # Parameters added in post-processing #
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/constants_output.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/constants_output.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/data_parser.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/data_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,20 @@
 
 MAP_MVS_EPA = {value: key for (key, value) in MAP_EPA_MVS.items()}
 
 # Fields expected for parameters of json returned to EPA, all assets will be returned
 EPA_PARAM_KEYS = {
     PROJECT_DATA: [PROJECT_ID, PROJECT_NAME, SCENARIO_ID, SCENARIO_NAME],
     SIMULATION_SETTINGS: [START_DATE, EVALUATED_PERIOD, TIMESTEP, OUTPUT_LP_FILE],
-    KPI: [KPI_SCALARS_DICT, KPI_UNCOUPLED_DICT, KPI_COST_MATRIX, KPI_SCALAR_MATRIX,],
+    KPI: [
+        KPI_SCALARS_DICT,
+        KPI_UNCOUPLED_DICT,
+        KPI_COST_MATRIX,
+        KPI_SCALAR_MATRIX,
+    ],
     "raw_results": ["index", "columns", "data"],
     "simulation_results": ["logs"],
 }
 
 # Fields expected for assets' parameters of json returned to EPA
 EPA_ASSET_KEYS = {
     ENERGY_PROVIDERS: [
@@ -300,15 +305,15 @@
         - Default value for `EMISSION_FACTOR` added
     - `ENERGY_CONSUMPTION`:
         - `DSM` is `False`
         - `DISPATCHABILITY` is FALSE
     - `ENERGY_PRODUCTION`:
         - Default value for `EMISSION_FACTOR` added
         - `DISPATCHABILITY` is always `False`, as no dispatchable fuel assets possible right now. Must be tackeld by EPA.
-     """
+    """
     epa_dict = deepcopy(epa_dict)
     dict_values = {}
 
     # Loop though one-dimensional energy system data (parameters directly in group)
     # Warnings for missing param_groups, will result in fatal error (except for fix_cost) as they can not be replaced with default values
     for param_group in [
         PROJECT_DATA,
@@ -409,17 +414,17 @@
                                 else:
                                     subasset[UNIT] = "kW"
                             # set the initial value of the state of charge to None
                             if k == MAP_MVS_EPA[STORAGE_CAPACITY]:
                                 subasset[SOC_INITIAL] = {VALUE: None, UNIT: TYPE_NONE}
                                 # move the optimize cap property from STORAGE_CAPACITY to the asset level
                                 if OPTIMIZE_CAP in subasset:
-                                    dict_asset[asset_label][
-                                        OPTIMIZE_CAP
-                                    ] = subasset.pop(OPTIMIZE_CAP)
+                                    dict_asset[asset_label][OPTIMIZE_CAP] = (
+                                        subasset.pop(OPTIMIZE_CAP)
+                                    )
 
                 # move the unit outside the timeseries dict
                 if TIMESERIES in dict_asset[asset_label]:
                     unit = dict_asset[asset_label][TIMESERIES].pop(UNIT)
                     data = dict_asset[asset_label][TIMESERIES].pop(VALUE)
                     dict_asset[asset_label][
                         UNIT
@@ -496,15 +501,17 @@
 
                 if asset_group == ENERGY_CONSUMPTION:
                     # DSM not used parameters, but to be sure it will be defined as False
                     if DSM not in dict_asset[asset_label]:
                         dict_asset[asset_label][DSM] = False
                     # Dispatchability of energy consumption assets always False
                     dict_asset[asset_label].update(
-                        {DISPATCHABILITY: {UNIT: TYPE_BOOL, VALUE: False},}
+                        {
+                            DISPATCHABILITY: {UNIT: TYPE_BOOL, VALUE: False},
+                        }
                     )
 
                 if asset_group == ENERGY_PRODUCTION or ENERGY_PROVIDERS:
                     # Emission factor only applicable for energy production assets and energy providers
                     if EMISSION_FACTOR not in dict_asset[asset_label]:
                         dict_asset[asset_label][EMISSION_FACTOR] = {
                             VALUE: KNOWN_EXTRA_PARAMETERS[EMISSION_FACTOR][
@@ -540,17 +547,17 @@
         missing_params = comparison[MISSING_PARAMETERS_KEY]
         if CONSTRAINTS in missing_params:
 
             if CONSTRAINTS not in dict_values:
                 dict_values[CONSTRAINTS] = {}
 
             for missing_constraint in missing_params[CONSTRAINTS]:
-                dict_values[CONSTRAINTS][
-                    missing_constraint
-                ] = DEFAULT_CONSTRAINT_VALUES[missing_constraint]
+                dict_values[CONSTRAINTS][missing_constraint] = (
+                    DEFAULT_CONSTRAINT_VALUES[missing_constraint]
+                )
 
             missing_params.pop(CONSTRAINTS)
 
         if SIMULATION_SETTINGS in missing_params:
             if (
                 OUTPUT_LP_FILE in missing_params[SIMULATION_SETTINGS]
                 and len(missing_params[SIMULATION_SETTINGS]) == 1
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/exceptions.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator/utils/helpers.py` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator/utils/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Util functions that are useful throughout the MVS
 
 Including:
 - find_valvue_by_key(): Finds value of a key in a nested dictionary.
 """
 
+from copy import deepcopy
 import os
 
 from multi_vector_simulator.utils.constants_json_strings import (
     DSO_FEEDIN_CAP,
     AUTO_CREATED_HIGHLIGHT,
     DSO_CONSUMPTION,
     DSO_FEEDIN,
@@ -24,14 +25,17 @@
     ENERGY_PROVIDERS,
     ENERGY_BUSSES,
     OEMOF_ASSET_TYPE,
     TYPE_ASSET,
     INFLOW_DIRECTION,
     OUTFLOW_DIRECTION,
     ENERGY_VECTOR,
+    SUFFIX_CRITICAL,
+    SUFFIX_NONCRITICAL,
+    REDUCABLE_DEMAND,
 )
 
 
 def find_value_by_key(data, target, result=None):
     """
     Finds value of a key in a nested dictionary.
 
@@ -116,14 +120,25 @@
     if isinstance(list_or_float, list):
         answer = len(list_or_float)
     else:
         answer = 0
     return answer
 
 
+def reducable_demand_name(demand_name: str, critical: bool = False):
+    """Name for auto created bus related to peak demand pricing period"""
+
+    if critical is False:
+        suffix = SUFFIX_NONCRITICAL
+    else:
+        suffix = SUFFIX_CRITICAL
+
+    return f"{demand_name}_{suffix} {AUTO_CREATED_HIGHLIGHT}"
+
+
 def peak_demand_bus_name(dso_name: str, feedin: bool = False):
     """Name for auto created bus related to peak demand pricing period"""
 
     if feedin is False:
         dso_direction = DSO_CONSUMPTION
     else:
         dso_direction = DSO_FEEDIN
@@ -178,9 +193,20 @@
                     output_bus = [output_bus]
             else:
                 output_bus = []
 
             for bus in input_bus + output_bus:
                 asset_busses[bus] = dict_values[ENERGY_BUSSES][bus].get(ENERGY_VECTOR)
             asset_type["busses"] = asset_busses
-            asset_types.append(asset_type)
+            if asset_type[TYPE_ASSET] == REDUCABLE_DEMAND:
+
+                asset_label = asset_type["label"]
+                asset_type["label"] = reducable_demand_name(asset_label)
+                asset_types.append(asset_type)
+                crit_asset_type = deepcopy(asset_type)
+                crit_asset_type["label"] = reducable_demand_name(
+                    asset_label, critical=True
+                )
+                asset_types.append(crit_asset_type)
+            else:
+                asset_types.append(asset_type)
     return asset_types
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/PKG-INFO` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-vector-simulator
-Version: 1.1.0rc2
+Version: 1.1.1rc1
 Summary: Multi-vector Simulation Tool assessing and optimizing Local Energy Systems (LES) for the E-LAND project
 Home-page: https://github.com/rl-institut/multi-vector-simulator
 Author: Reiner Lemoine Institut
 Author-email: pypi@rl-institut.de
 Project-URL: Bug Reports, https://github.com/rl-institut/multi-vector-simulator/issues
 Project-URL: Source, https://github.com/rl-institut/multi-vector-simulator
 Keywords: multi-vector local-energy-systems
@@ -39,15 +39,15 @@
 Requires-Dist: folium>=0.10.1; extra == "report"
 Requires-Dist: reverse_geocoder>=1.5.1; extra == "report"
 Requires-Dist: staticmap>=0.5.4; extra == "report"
 Requires-Dist: pyppeteer>=0.2.2; extra == "report"
 Requires-Dist: psutil>=5.7.0; extra == "report"
 Provides-Extra: test
 Requires-Dist: pytest>=5.3.1; extra == "test"
-Requires-Dist: black==19.10b0; extra == "test"
+Requires-Dist: black==24.3.0; extra == "test"
 Requires-Dist: coverage>=4.5; extra == "test"
 Requires-Dist: coveralls>=3.0.1; extra == "test"
 Requires-Dist: mock>=3.0.5; extra == "test"
 Requires-Dist: click==8.0.2; extra == "test"
 
 ##################################################
 MVS - Multi-Vector Simulator of the E-LAND toolbox
```

### Comparing `multi-vector-simulator-1.1.0rc2/src/multi_vector_simulator.egg-info/SOURCES.txt` & `multi_vector_simulator-1.1.1rc1/src/multi_vector_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_A0_initialization.py` & `multi_vector_simulator-1.1.1rc1/tests/test_A0_initialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                 test_out_path,
             ]
         ),
     )
     def test_if_csv_opt_path_input_file_set_to_path_input_folder_mvs_csv_config_dot_json(
         self, m_args, tmpdir
     ):
-        """Check that the path_input_file is <path_input_folder>/mvs_csv_config.json """
+        """Check that the path_input_file is <path_input_folder>/mvs_csv_config.json"""
         os.mkdir(self.fake_input_path)
         os.mkdir(os.path.join(self.fake_input_path, CSV_ELEMENTS))
         user_inputs = A0.process_user_arguments()
         assert user_inputs[PATH_INPUT_FILE] == os.path.join(
             self.fake_input_path, CSV_ELEMENTS, CSV_FNAME
         )
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_A1_csv_to_json.py` & `multi_vector_simulator-1.1.1rc1/tests/test_A1_csv_to_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,18 @@
     BENCHMARK_TEST_OUTPUT_FOLDER,
 )
 
 CSV_PARAMETERS = ["param1", "param2"]
 
 CSV_EXAMPLE = {"col1": {"param1": "val11", "param2": {VALUE: 21, UNIT: "factor"}}}
 CSV_TIMESERIES = {
-    "param1": {VALUE: {FILENAME: "test_time_series.csv", HEADER: "power"}, UNIT: "kW",}
+    "param1": {
+        VALUE: {FILENAME: "test_time_series.csv", HEADER: "power"},
+        UNIT: "kW",
+    }
 }
 
 CSV_LIST = {
     "param1": ["one", "two"],
     "param2": {UNIT: "factor", VALUE: [1.02, 3.04]},
     "param3": {UNIT: "currency/kWh", VALUE: [0.2, 0.7]},
     "param4": {UNIT: TYPE_BOOL, VALUE: [True, False, True]},
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_B0_data_input_json.py` & `multi_vector_simulator-1.1.1rc1/tests/test_B0_data_input_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,17 +103,34 @@
         A0.process_user_arguments()
 
         A1.create_input_json(input_directory=CSV_PATH, pass_back=True)
         dict_values = B0.load_json(
             JSON_CSV_PATH, path_output_folder=self.test_out_path, move_copy=True
         )
 
-        assert os.path.exists(os.path.join(CSV_PATH, CSV_ELEMENTS, CSV_FNAME,)) is False
+        assert (
+            os.path.exists(
+                os.path.join(
+                    CSV_PATH,
+                    CSV_ELEMENTS,
+                    CSV_FNAME,
+                )
+            )
+            is False
+        )
 
-        assert os.path.exists(os.path.join(CSV_PATH, CSV_FNAME,)) is False
+        assert (
+            os.path.exists(
+                os.path.join(
+                    CSV_PATH,
+                    CSV_FNAME,
+                )
+            )
+            is False
+        )
 
     @mock.patch(
         "argparse.ArgumentParser.parse_args",
         return_value=PARSER.parse_args(
             [
                 "-f",
                 "-log",
@@ -147,21 +164,27 @@
 
     def teardown_method(self):
         if os.path.exists(self.test_out_path):
             shutil.rmtree(self.test_out_path, ignore_errors=True)
 
 
 class TestConversionJsonToPythonTypes:
-    def setup(self):
+    def setup_method(self):
         self.n_days = 4
         self.start_date = pd.to_datetime("2018-01-01 00:00:00")
         self.end_date = self.start_date + pd.DateOffset(days=self.n_days - 1)
-        self.ti = pd.date_range(start=self.start_date, end=self.end_date, freq="1D",)
+        self.ti = pd.date_range(
+            start=self.start_date,
+            end=self.end_date,
+            freq="1D",
+        )
         self.ti_long = pd.date_range(
-            start=self.start_date, end=self.end_date, freq="1H",
+            start=self.start_date,
+            end=self.end_date,
+            freq="1H",
         )
         self.test_dict_series = {
             "series": {
                 DATA_TYPE_JSON_KEY: TYPE_SERIES,
                 VALUE: [d + 1 for d in range(self.n_days)],
             }
         }
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_C0_data_processing.py` & `multi_vector_simulator-1.1.1rc1/tests/test_C0_data_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,15 +629,15 @@
         C0.process_maximum_cap_constraint(dict_values, group, asset, subasset=None)
         assert (
             dict_values[group][asset][MAXIMUM_CAP][VALUE] is None
         ), f"The initial maximumCap defined by the end-user ({maxCap}) is overwritten by a different value ({dict_values[group][asset][MAXIMUM_CAP][VALUE]})."
 
 
 def test_process_maximum_cap_constraint_maximumCap_is_int_smaller_than_installed_cap():
-    """"The asset has a maximumCap < installedCap which is invalid and being ignored."""
+    """ "The asset has a maximumCap < installedCap which is invalid and being ignored."""
     maxCap = 10
     dict_values = {
         group: {
             asset: {
                 UNIT: unit,
                 INSTALLED_CAP: {VALUE: installed_cap},
                 MAXIMUM_CAP: {VALUE: maxCap},
@@ -668,15 +668,16 @@
         dict_values[group][asset][MAXIMUM_CAP][VALUE] == maxCap
     ), f"The initial maximumCap defined by the end-user ({maxCap}) is overwritten by a different value ({dict_values[group][asset][MAXIMUM_CAP][VALUE]})."
 
 
 def test_process_maximum_cap_constraint_group_is_ENERGY_PRODUCTION_non_dispatchable_asset():
     # ToDo: change assertion errors
     """The asset belongs to the energy production group, and is a non-dispatchable asset.
-    As the maximumCap is used to define the maximum capacity of an asset, but used in oemof-solph to limit a flow, the value has to be translated."""
+    As the maximumCap is used to define the maximum capacity of an asset, but used in oemof-solph to limit a flow, the value has to be translated.
+    """
     timeseries_peak = 0.8
     group = ENERGY_PRODUCTION
     maxCap = 100
     dict_values = {
         group: {
             asset: {
                 LABEL: asset,
@@ -699,15 +700,21 @@
     ), f"Message about the normalized value"
 
 
 def test_process_maximum_cap_constraint_subasset():
     """For storages, the subassets have to be processes. This tests the procedure examplary."""
     dict_values = {
         group: {
-            asset: {subasset: {LABEL: asset, UNIT: unit, MAXIMUM_CAP: {VALUE: None},}}
+            asset: {
+                subasset: {
+                    LABEL: asset,
+                    UNIT: unit,
+                    MAXIMUM_CAP: {VALUE: None},
+                }
+            }
         }
     }
 
     C0.process_maximum_cap_constraint(dict_values, group, asset, subasset=subasset)
     assert (
         dict_values[group][asset][subasset][MAXIMUM_CAP][VALUE] is None
     ), f"The function does not change the previously defined MAXIMUM_CAP."
@@ -763,18 +770,24 @@
     }
 )
 
 
 def test_add_a_transformer_for_each_peak_demand_pricing_period_1_period():
     dict_test_trafo = deepcopy(dict_test)
     dict_availability_timeseries = C0.define_availability_of_peak_demand_pricing_assets(
-        dict_test_trafo, 1, 12,
+        dict_test_trafo,
+        1,
+        12,
     )
-    list_of_dso_energyConversion_assets = C0.add_a_transformer_for_each_peak_demand_pricing_period(
-        dict_test_trafo, dict_test[ENERGY_PROVIDERS][DSO], dict_availability_timeseries,
+    list_of_dso_energyConversion_assets = (
+        C0.add_a_transformer_for_each_peak_demand_pricing_period(
+            dict_test_trafo,
+            dict_test[ENERGY_PROVIDERS][DSO],
+            dict_availability_timeseries,
+        )
     )
     assert (
         len(list_of_dso_energyConversion_assets) == 1
     ), f"The list of peak demand pricing transformers is not only one entry long."
     exp_list = [
         dict_test_trafo[ENERGY_PROVIDERS][DSO][LABEL]
         + DSO_CONSUMPTION
@@ -790,18 +803,24 @@
             transformer in dict_test_trafo[ENERGY_CONVERSION]
         ), f"Transformer {transformer} is not added as an energyConversion object."
 
 
 def test_add_a_transformer_for_each_peak_demand_pricing_period_2_periods():
     dict_test_trafo = deepcopy(dict_test)
     dict_availability_timeseries = C0.define_availability_of_peak_demand_pricing_assets(
-        dict_test_trafo, 2, 6,
+        dict_test_trafo,
+        2,
+        6,
     )
-    list_of_dso_energyConversion_assets = C0.add_a_transformer_for_each_peak_demand_pricing_period(
-        dict_test_trafo, dict_test[ENERGY_PROVIDERS][DSO], dict_availability_timeseries,
+    list_of_dso_energyConversion_assets = (
+        C0.add_a_transformer_for_each_peak_demand_pricing_period(
+            dict_test_trafo,
+            dict_test[ENERGY_PROVIDERS][DSO],
+            dict_availability_timeseries,
+        )
     )
     assert (
         len(list_of_dso_energyConversion_assets) == 2
     ), f"The list of peak demand pricing transformers is not only two entries long."
     exp_list = [
         dict_test[ENERGY_PROVIDERS][DSO][LABEL]
         + DSO_CONSUMPTION
@@ -1259,15 +1278,18 @@
     dict_asset = {
         ENERGY_VECTOR: "Electricity",
         FILENAME: "timeseries.csv",
         INFLOW_DIRECTION: "Electricity",
         LABEL: "Electricity demand",
         OEMOF_ASSET_TYPE: OEMOF_SINK,
         UNIT: "kW",
-        TIMESERIES: {VALUE: [4, 5, 6], DATA_TYPE_JSON_KEY: TYPE_SERIES,},
+        TIMESERIES: {
+            VALUE: [4, 5, 6],
+            DATA_TYPE_JSON_KEY: TYPE_SERIES,
+        },
     }
     C0.receive_timeseries_from_csv(settings_dict, dict_asset, input_type="input")
     assert (dict_asset[TIMESERIES].values == np.array([1, 2, 3])).all()
 
 
 def test_load_timeseries_from_TIMESERIES_if_file_under_FILENAME_not_exist():
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_C1_verification.py` & `multi_vector_simulator-1.1.1rc1/tests/test_C1_verification.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
     time_series = pd.Series([0, 0.22, 0.5, 0.99, 1, -0.01])
     result = C1.check_time_series_values_between_0_and_1(time_series=time_series)
     assert result is False
 
 
 @pytest.fixture()
 def get_dict_vals():
-    """ Reads input json file."""
+    """Reads input json file."""
     with open(os.path.join(JSON_PATH)) as json_file:
         dict_values = json.load(json_file)  # todo welches file???
     return dict_values
 
 
 def test_check_efficiency_of_storage_capacity_is_0(get_dict_vals):
     dict_values = get_dict_vals
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_C2_economic_functions.py` & `multi_vector_simulator-1.1.1rc1/tests/test_C2_economic_functions.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_D0_modelling_and_optimization.py` & `multi_vector_simulator-1.1.1rc1/tests/test_D0_modelling_and_optimization.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_D1_model_components.py` & `multi_vector_simulator-1.1.1rc1/tests/test_D1_model_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,37 +45,38 @@
 )
 from _constants import TEST_REPO_PATH, TEST_INPUT_DIRECTORY
 
 D1_JSON = os.path.join(
     TEST_REPO_PATH, TEST_INPUT_DIRECTORY, "inputs_for_D1", JSON_FNAME
 )
 
+
 # fixtures that help creating variables and data needed for the tests
 @pytest.fixture()
 def get_json():
-    """ Reads input json file. """
+    """Reads input json file."""
     with open(D1_JSON) as json_file:
         dict_values = json.load(json_file)
     yield dict_values
 
 
 @pytest.fixture()
 def get_model():
-    """ Creates solph.EnergySystem model. """
+    """Creates solph.EnergySystem model."""
     time_index = pd.date_range(
         start=pd.to_datetime("2018-01-01 00:00:00"),
         end=pd.to_datetime("2018-12-31 23:00:00"),
         freq="H",
     )
     yield solph.EnergySystem(timeindex=time_index)
 
 
 @pytest.fixture()
 def get_busses():
-    """ Creates busses (solph.Bus) dictionary. """
+    """Creates busses (solph.Bus) dictionary."""
     yield {
         "Fuel bus": solph.Bus(label="Fuel bus"),
         "Electricity bus": D1.CustomBus(
             label="Electricity bus", energy_vector="Electricity"
         ),
         "Electricity bus 2": D1.CustomBus(
             label="Electricity bus 2", energy_vector="Electricity"
@@ -86,15 +87,15 @@
         "Gas bus": solph.Bus(label="Gas bus"),
     }
 
 
 class TestTransformerComponent:
     @pytest.fixture(autouse=True)
     def setup_class(self, get_json, get_model, get_busses):
-        """ Sets up class attributes for the tests. """
+        """Sets up class attributes for the tests."""
         self.dict_values = get_json
         self.model = get_model
         self.transformers = {}
         self.busses = get_busses
 
     def helper_test_transformer_in_model_and_dict(
         self, optimize, dict_asset, multiple_outputs=False
@@ -298,28 +299,26 @@
             D1.transformer(
                 model=self.model,
                 dict_asset=dict_asset,
                 transformer=self.transformers,
                 bus=self.busses,
             )
 
-
     def test_transformer_fix_cap_single_busses(self):
         dict_asset = self.dict_values[ENERGY_CONVERSION][
             "transformer_fix_single_busses"
         ]
 
         D1.transformer(
             model=self.model,
             dict_asset=dict_asset,
             transformer=self.transformers,
             bus=self.busses,
         )
 
-
         # # only one output and one input bus
         # assert (
         #     len([str(i) for i in self.model.entities[-1].outputs]) == 1
         # ), f"Amount of output busses of transformer should be one but is {len([str(i) for i in self.model.entities[-1].outputs])}."
         # assert (
         #     len([str(i) for i in self.model.entities[-1].inputs]) == 1
         # ), f"Amount of input busses of transformer should be one but is {len([str(i) for i in self.model.entities[-1].inputs])}."
@@ -390,15 +389,17 @@
         ), f"Amount of input busses of transformer should be one but is {len([str(i) for i in self.model.nodes[-1].inputs])}."
 
         # checks done with helper function (see func for more information)
         self.helper_test_transformer_in_model_and_dict(
             optimize=False, dict_asset=dict_asset
         )
 
-    def test_transformer_fix_cap_multiple_input_busses(self,):
+    def test_transformer_fix_cap_multiple_input_busses(
+        self,
+    ):
         dict_asset = self.dict_values[ENERGY_CONVERSION][
             "transformer_fix_multiple_input_busses"
         ]
 
         D1.transformer(
             model=self.model,
             dict_asset=dict_asset,
@@ -574,15 +575,15 @@
                 bus=self.busses,
             )
 
 
 class TestSinkComponent:
     @pytest.fixture(autouse=True)
     def setup_class(self, get_json, get_model, get_busses):
-        """ Sets up class attributes for the tests. """
+        """Sets up class attributes for the tests."""
         self.dict_values = get_json
         self.model = get_model
         self.busses = get_busses
         self.sinks = {}
         self.time_series = pd.Series(data=[0.5, 0.4, 0.0])
 
     def helper_test_sink_in_model_and_dict(
@@ -635,60 +636,72 @@
                 )
 
     def test_sink_non_dispatchable_single_input_bus(self):
         dict_asset = self.dict_values[ENERGY_CONSUMPTION]["non_dispatchable_single"]
         dict_asset[TIMESERIES] = self.time_series
 
         D1.sink_non_dispatchable(
-            model=self.model, dict_asset=dict_asset, sink=self.sinks, bus=self.busses,
+            model=self.model,
+            dict_asset=dict_asset,
+            sink=self.sinks,
+            bus=self.busses,
         )
 
         self.helper_test_sink_in_model_and_dict(
             dispatchable=False, dict_asset=dict_asset, amount_inputs=1
         )
 
     def test_sink_non_dispatchable_multiple_input_busses(self):
         dict_asset = self.dict_values[ENERGY_CONSUMPTION]["non_dispatchable_multiple"]
         dict_asset[TIMESERIES] = self.time_series
 
         D1.sink_non_dispatchable(
-            model=self.model, dict_asset=dict_asset, sink=self.sinks, bus=self.busses,
+            model=self.model,
+            dict_asset=dict_asset,
+            sink=self.sinks,
+            bus=self.busses,
         )
 
         self.helper_test_sink_in_model_and_dict(
             dispatchable=False, dict_asset=dict_asset, amount_inputs=2
         )
 
     def test_sink_dispatchable_single_input_bus(self):
         dict_asset = self.dict_values[ENERGY_CONSUMPTION]["dispatchable_single"]
 
         D1.sink_dispatchable_optimize(
-            model=self.model, dict_asset=dict_asset, sink=self.sinks, bus=self.busses,
+            model=self.model,
+            dict_asset=dict_asset,
+            sink=self.sinks,
+            bus=self.busses,
         )
 
         self.helper_test_sink_in_model_and_dict(
             dispatchable=True, dict_asset=dict_asset, amount_inputs=1
         )
 
     def test_sink_dispatchable_multiple_input_busses(self):
         dict_asset = self.dict_values[ENERGY_CONSUMPTION]["dispatchable_multiple"]
 
         D1.sink_dispatchable_optimize(
-            model=self.model, dict_asset=dict_asset, sink=self.sinks, bus=self.busses,
+            model=self.model,
+            dict_asset=dict_asset,
+            sink=self.sinks,
+            bus=self.busses,
         )
 
         self.helper_test_sink_in_model_and_dict(
             dispatchable=True, dict_asset=dict_asset, amount_inputs=2
         )
 
 
 class TestSourceComponent:
     @pytest.fixture(autouse=True)
     def setup_class(self, get_json, get_model, get_busses):
-        """ Sets up class attributes for the tests. """
+        """Sets up class attributes for the tests."""
         self.dict_values = get_json
         self.model = get_model
         self.busses = get_busses
         self.sources = {}
         self.time_series = pd.Series(data=[10, 11, 12])
 
     def helper_test_source_in_model_and_dict(
@@ -824,15 +837,17 @@
         self.helper_test_source_in_model_and_dict(
             dict_asset=dict_asset,
             dispatchable=True,
             mode="optimize",
             timeseries="normalized",
         )
 
-    def test_source_dispatchable_optimize_timeseries_not_normalized_timeseries(self,):
+    def test_source_dispatchable_optimize_timeseries_not_normalized_timeseries(
+        self,
+    ):
         dict_asset = self.dict_values[ENERGY_PRODUCTION]["dispatchable_source_optimize"]
         dict_asset[TIMESERIES] = self.time_series
         dict_asset[TIMESERIES_PEAK] = {"unit": "kWp/H", "value": self.time_series.max()}
 
         D1.source(
             model=self.model,
             dict_asset=dict_asset,
@@ -885,15 +900,15 @@
             timeseries="not_normalized",
         )
 
 
 class TestStorageComponent:
     @pytest.fixture(autouse=True)
     def setup_class(self, get_json, get_model, get_busses):
-        """ Sets up class attributes for the tests. """
+        """Sets up class attributes for the tests."""
         self.dict_values = get_json
         self.model = get_model
         self.busses = get_busses
         self.storages = {}
 
     def test_storage_fix(self):
         dict_asset = self.dict_values[ENERGY_STORAGE]["storage_fix"]
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_D2_model_constraints.py` & `multi_vector_simulator-1.1.1rc1/tests/test_D2_model_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,16 @@
         OEMOF_BUSSES: {electricity: electricity, fuel: fuel},
     }
 
     (
         renewable_assets,
         non_renewable_assets,
     ) = D2.prepare_constraint_minimal_renewable_share(
-        dict_values=dict_values, dict_model=dict_model,
+        dict_values=dict_values,
+        dict_model=dict_model,
     )
 
     assert (
         pv_plant in renewable_assets
     ), f"The {pv_plant} is not added to the renewable assets."
     assert (
         pv_plant not in non_renewable_assets
@@ -180,15 +181,18 @@
         },
     }
     dict_model = {
         OEMOF_SINK: {demand_profiles: demand_profiles},
         OEMOF_BUSSES: {electricity: electricity},
     }
 
-    demands = D2.prepare_demand_assets(dict_values, dict_model,)
+    demands = D2.prepare_demand_assets(
+        dict_values,
+        dict_model,
+    )
 
     assert (
         demand_profiles in demands
     ), f"Demand asset {demand_profiles} should be in the demands taken into account for the constraints, but is not included in it ({demands.keys()})."
     exp = {
         D2.OEMOF_SOLPH_OBJECT_ASSET: dict_model[OEMOF_SINK][
             dict_values[ENERGY_CONSUMPTION][demand_profiles][LABEL]
@@ -210,31 +214,38 @@
         ), f"The expected value (exp[key]) of {key} for {demand_profiles} is not met, but is of value {demands[demand_profiles][key]}."
 
 
 def test_prepare_energy_provider_consumption_sources():
     electricity = "Electricity"
     dso = "DSO"
     dict_values = {
-        ENERGY_PROVIDERS: {dso: {LABEL: dso},},
+        ENERGY_PROVIDERS: {
+            dso: {LABEL: dso},
+        },
         ENERGY_PRODUCTION: {
             dso
             + DSO_CONSUMPTION: {
                 LABEL: dso + DSO_CONSUMPTION,
                 OUTFLOW_DIRECTION: electricity,
                 ENERGY_VECTOR: electricity,
             }
         },
     }
     dict_model = {
-        OEMOF_SOURCE: {dso + DSO_CONSUMPTION: dso + DSO_CONSUMPTION,},
+        OEMOF_SOURCE: {
+            dso + DSO_CONSUMPTION: dso + DSO_CONSUMPTION,
+        },
         OEMOF_BUSSES: {electricity: electricity},
     }
 
-    energy_provider_consumption_sources = D2.prepare_energy_provider_consumption_sources(
-        dict_values, dict_model,
+    energy_provider_consumption_sources = (
+        D2.prepare_energy_provider_consumption_sources(
+            dict_values,
+            dict_model,
+        )
     )
 
     DSO_source_name = dict_values[ENERGY_PROVIDERS][dso][LABEL] + DSO_CONSUMPTION
 
     assert (
         DSO_source_name in energy_provider_consumption_sources
     ), f"DSO source asset {DSO_source_name} should be in the energy provider source list taken into account for the constraints, but is not included in it ({energy_provider_consumption_sources.keys()})."
@@ -260,31 +271,36 @@
         ), f"The expected value (exp[key]) of {key} for {DSO_source_name} is not met, but is of value {energy_provider_consumption_sources[DSO_source_name][key]}."
 
 
 def test_prepare_energy_provider_feedin_sinks():
     electricity = "Electricity"
     dso = "DSO"
     dict_values = {
-        ENERGY_PROVIDERS: {dso: {LABEL: dso},},
+        ENERGY_PROVIDERS: {
+            dso: {LABEL: dso},
+        },
         ENERGY_CONSUMPTION: {
             dso
             + DSO_FEEDIN: {
                 LABEL: dso + DSO_FEEDIN,
                 INFLOW_DIRECTION: electricity,
                 ENERGY_VECTOR: electricity,
             }
         },
     }
     dict_model = {
-        OEMOF_SINK: {dso + DSO_FEEDIN: dso + DSO_FEEDIN,},
+        OEMOF_SINK: {
+            dso + DSO_FEEDIN: dso + DSO_FEEDIN,
+        },
         OEMOF_BUSSES: {electricity: electricity},
     }
 
     energy_provider_feedin_sinks = D2.prepare_energy_provider_feedin_sinks(
-        dict_values, dict_model,
+        dict_values,
+        dict_model,
     )
 
     DSO_sink_name = dict_values[ENERGY_PROVIDERS][dso][LABEL] + DSO_FEEDIN
 
     assert (
         DSO_sink_name in energy_provider_feedin_sinks
     ), f"DSO sink asset {DSO_sink_name} should be in the energy provider sink list taken into account for the constraints, but is not included in it ({energy_provider_feedin_sinks.keys()})."
@@ -362,15 +378,16 @@
         )
         return
 
     def test_constraint_maximum_emissions(self):
         """Checks if maximum emissions limit is properly added as a constraint"""
         # Create a solph model using the input values (especially the constraints setup as class variables above)
         model = D2.constraint_maximum_emissions(
-            model=solph.Model(self.model), dict_values=self.dict_values,
+            model=solph.Model(self.model),
+            dict_values=self.dict_values,
         )
         assert (
             model.integral_limit_emission_factor_constraint.upper.value
             == self.exp_emission_limit
         ), f"Either the maximum emission constraint has not been added or the wrong limit has been added; limit is {model.integral_limit_emission_factor_constraint.upper.value}."
 
     def test_add_constraints_maximum_emissions(self):
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_E0_evaluation.py` & `multi_vector_simulator-1.1.1rc1/tests/test_E0_evaluation.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_E1_process_results.py` & `multi_vector_simulator-1.1.1rc1/tests/test_E1_process_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,15 +318,17 @@
     )
     for parameter in [FLOW, TOTAL_FLOW, ANNUAL_TOTAL_FLOW, PEAK_FLOW, AVERAGE_FLOW]:
         assert (
             parameter in dict_test
         ), f"Parameter {parameter} should have been added to the dict_asset."
         if parameter == FLOW:
             assert_series_equal(
-                dict_test[FLOW].astype(np.int64), flow, check_names=False,
+                dict_test[FLOW].astype(np.int64),
+                flow,
+                check_names=False,
             )
         else:
             assert (
                 UNIT in dict_test[parameter]
             ), f"Parameter {parameter} should have been added to the dict_asset with an {VALUE}."
             assert (
                 VALUE in dict_test[parameter]
@@ -354,15 +356,17 @@
                 UNIT in dict_test[parameter]
             ), f"Parameter {parameter} should have been added to the dict_asset with an {VALUE}."
             assert (
                 VALUE in dict_test[parameter]
             ), f"Parameter {parameter} should have been added to the dict_asset with an {VALUE}."
 
     assert_series_equal(
-        dict_test[FLOW].astype(np.int64), flow, check_names=False,
+        dict_test[FLOW].astype(np.int64),
+        flow,
+        check_names=False,
     )
     assert dict_test[TOTAL_FLOW][VALUE] == sum(
         flow
     ), f"The {TOTAL_FLOW} should be {sum(flow)}, but is {dict_test[TOTAL_FLOW][VALUE]}"
     assert (
         dict_test[ANNUAL_TOTAL_FLOW][VALUE] == sum(flow) * 365
     ), f"The {ANNUAL_TOTAL_FLOW} should be {sum(flow)*365}, but is {dict_test[ANNUAL_TOTAL_FLOW][VALUE]}"
@@ -389,15 +393,17 @@
                 UNIT in dict_test[parameter]
             ), f"Parameter {parameter} should have been added to the dict_asset with an {VALUE}."
             assert (
                 VALUE in dict_test[parameter]
             ), f"Parameter {parameter} should have been added to the dict_asset with an {VALUE}."
 
     assert_series_equal(
-        dict_test[FLOW].astype(np.int64), flow, check_names=False,
+        dict_test[FLOW].astype(np.int64),
+        flow,
+        check_names=False,
     )
     assert dict_test[TOTAL_FLOW][VALUE] == sum(
         flow
     ), f"The {TOTAL_FLOW} should be {sum(flow)}, but is {dict_test[TOTAL_FLOW][VALUE]}"
     assert dict_test[ANNUAL_TOTAL_FLOW][VALUE] == sum(
         flow
     ), f"The {ANNUAL_TOTAL_FLOW} should be {sum(flow)}, but is {dict_test[ANNUAL_TOTAL_FLOW][VALUE]}"
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_E2_economics.py` & `multi_vector_simulator-1.1.1rc1/tests/test_E2_economics.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,18 +159,20 @@
     ), f"With {cost_replacement}, the total replacement costs are not equal to the sum of the replacement costs of each pre-installed ({specific_replacement_costs_of_installed_cap * installed_capacity}) and additional capacity ({specific_replacement_costs_of_optimized_cap * optimized_add_capacity})."
 
 
 def test_calculate_operation_and_management_expenditures():
     installed_capacity = 10
     optimized_add_capacity = 10
     specific_om_cost = 5
-    operation_and_management_expenditures = E2.calculate_operation_and_management_expenditures(
-        specific_om_cost=specific_om_cost,
-        installed_capacity=installed_capacity,
-        optimized_add_capacity=optimized_add_capacity,
+    operation_and_management_expenditures = (
+        E2.calculate_operation_and_management_expenditures(
+            specific_om_cost=specific_om_cost,
+            installed_capacity=installed_capacity,
+            optimized_add_capacity=optimized_add_capacity,
+        )
     )
     assert operation_and_management_expenditures == specific_om_cost * (
         installed_capacity + optimized_add_capacity
     ), f"With {operation_and_management_expenditures}, the OM costs are not equal to the sum of the capacities ({installed_capacity+optimized_add_capacity}) times the specific costs ({specific_om_cost})."
 
 
 def test_calculate_total_asset_costs_over_lifetime():
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_E3_indicator_calculation.py` & `multi_vector_simulator-1.1.1rc1/tests/test_E3_indicator_calculation.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,18 @@
 flow_dso = 50
 flow_pv_local = 100
 renewable_share_dso = 0.1
 
 dict_renewable_energy_use = {
     ENERGY_PRODUCTION: {
         dso
-        + DSO_CONSUMPTION: {ENERGY_VECTOR: electricity, TOTAL_FLOW: {VALUE: flow_dso},},
+        + DSO_CONSUMPTION: {
+            ENERGY_VECTOR: electricity,
+            TOTAL_FLOW: {VALUE: flow_dso},
+        },
         pv_plant: {
             ENERGY_VECTOR: electricity,
             TOTAL_FLOW: {VALUE: flow_pv_local},
             RENEWABLE_ASSET_BOOL: {VALUE: True},
         },
     },
     ENERGY_PROVIDERS: {
@@ -726,15 +729,15 @@
     ), f"The {DEGREE_OF_NZE} is not added to {KPI_SCALARS_DICT}"
     assert (
         dict_values_NZE[KPI][KPI_SCALARS_DICT][DEGREE_OF_NZE] == degree_of_nze
     ), f"The degree of NZE is not added successfully to the list of KPI's."
 
 
 def test_equation_degree_of_net_zero_energy():
-    """ Degree of NZE between 0 and 1."""
+    """Degree of NZE between 0 and 1."""
     total_feedin = 60
     total_grid_consumption = 80
     total_demand = 100
     degree_of_nze = E3.equation_degree_of_net_zero_energy(
         total_feedin, total_grid_consumption, total_demand
     )
     exp = 1 + (total_feedin - total_grid_consumption) / total_demand
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_E4_verification.py` & `multi_vector_simulator-1.1.1rc1/tests/test_E4_verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     return_value = E4.net_zero_energy_constraint_test(dict_values)
     assert (
         return_value == False
     ), f"When the net zero energy constraint is not met by a difference of >= e6 this test should fail."
 
 
 def test_detect_excessive_excess_generation_in_bus_warning_is_logged(caplog):
-    """A logging.warning is printed due to excessive excess generation. """
+    """A logging.warning is printed due to excessive excess generation."""
     bus_label = "Test_bus"
     dict_values = {
         "optimizedFlows": {
             bus_label: pd.DataFrame(
                 {"inflow": [1, 2, 3], "outflow": [-1, -1, -2], "excess": [0, 1, 1]}
             )
         }
@@ -158,15 +158,15 @@
     assert (
         f"Attention, on bus {bus_label} there is excessive excess generation"
         in caplog.text
     ), f"An intended warning is not logged although there is excessive excess generation."
 
 
 def test_detect_excessive_excess_generation_in_bus_no_excess(caplog):
-    """No excessive excess generation takes place. """
+    """No excessive excess generation takes place."""
     bus_label = "Test_bus"
     dict_values = {
         "optimizedFlows": {
             bus_label: pd.DataFrame(
                 {
                     "inflow": [1, 2, 3],
                     "outflow": [-1, -1.9, -2.5],
@@ -179,33 +179,41 @@
         E4.detect_excessive_excess_generation_in_bus(dict_values=dict_values)
     assert (
         caplog.text == ""
     ), f"A warning is logged although there is no excessive excess generation."
 
 
 def test_detect_excessive_excess_generation_in_bus_several_busses_two_warnings(caplog):
-    """Excessive excess generation takes place in two busses. """
+    """Excessive excess generation takes place in two busses."""
     excessive_excess_bus_1, excessive_excess_bus_2 = (
         "Bus_excessive_excess_1",
         "Bus_excessive_excess_2",
     )
     dict_values = {
         "optimizedFlows": {
             "Bus_no_excessive_excess": pd.DataFrame(
                 {
                     "inflow": [1, 2, 3],
                     "outflow": [-1, -1.9, -2.5],
                     "excess": [0, 0.1, 0.5],
                 }
             ),
             excessive_excess_bus_1: pd.DataFrame(
-                {"inflow": [1, 2, 3], "outflow": [-1, -1, -2], "excess": [0, 1, 1],}
+                {
+                    "inflow": [1, 2, 3],
+                    "outflow": [-1, -1, -2],
+                    "excess": [0, 1, 1],
+                }
             ),
             excessive_excess_bus_2: pd.DataFrame(
-                {"inflow": [1, 2, 3], "outflow": [-1, -1, -1], "excess": [0, 1, 2],}
+                {
+                    "inflow": [1, 2, 3],
+                    "outflow": [-1, -1, -1],
+                    "excess": [0, 1, 2],
+                }
             ),
         }
     }
     with caplog.at_level(logging.WARNING):
         E4.detect_excessive_excess_generation_in_bus(dict_values=dict_values)
     assert (
         f"Attention, on bus {excessive_excess_bus_1} there is excessive excess generation"
@@ -214,15 +222,16 @@
         in caplog.text
     ), f"One or two intended warnings are missing although there is excessive excess generation in two busses."
 
 
 def test_verify_state_of_charge_feasible(caplog):
     """Two cases are tested here
     Case 1 is no storage components in the energy system, hence no verification carried out
-    Case 2 is that all the SoC values are physically feasible, so no WARNING log messages"""
+    Case 2 is that all the SoC values are physically feasible, so no WARNING log messages
+    """
 
     # Test case: No storage components present in the system, so function is exited before any verification
     # Make an empty energyStorage dict signifying that there are no storage components in the energy system
     dict_values = {"energyStorage": {}}
     return_value = E4.verify_state_of_charge(dict_values=dict_values)
     assert (
         return_value is None
@@ -239,15 +248,19 @@
     index = pd.date_range(start="1/1/2018", periods=50, tz="Asia/Tokyo")
 
     # Create a SoC time series from above floats and date-time data
     soc_series = pd.Series(data=data, index=index)
 
     storage = "storage_01"
     # Add the SoC time series to the result JSON nested-dict
-    dict_values = {ENERGY_STORAGE: {storage: {TIMESERIES_SOC: soc_series},}}
+    dict_values = {
+        ENERGY_STORAGE: {
+            storage: {TIMESERIES_SOC: soc_series},
+        }
+    }
     # Test for the function's behavior with the current case
     with caplog.at_level(logging.WARNING):
         E4.verify_state_of_charge(dict_values=dict_values)
     assert (
         f"greater than 1. This is a physically impossible value!" not in caplog.text
     ), f"A WARNING message is logged even though the SoC values are all below 1."
     assert (
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_F0_output.py` & `multi_vector_simulator-1.1.1rc1/tests/test_F0_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,18 @@
 
         F0.store_scalars_to_excel(dict_scalars_two_tabs)
         assert os.path.exists(os.path.join(OUTPUT_PATH, "scalars.xlsx")) is True
 
     def test_store_each_bus_timeseries_to_excel_and_png_one_bus(self):
         """ """
         dict_timeseries_test_one_bus = {
-            PROJECT_DATA: {PROJECT_NAME: "a_project", SCENARIO_NAME: "a_scenario",},
+            PROJECT_DATA: {
+                PROJECT_NAME: "a_project",
+                SCENARIO_NAME: "a_scenario",
+            },
             SIMULATION_SETTINGS: {PATH_OUTPUT_FOLDER: OUTPUT_PATH},
             OPTIMIZED_FLOWS: {"a_bus": BUS},
         }
         dict_timeseries_test_one_bus.update(copy.deepcopy(DICT_PLOTS))
         F0.store_timeseries_all_busses_to_excel(dict_timeseries_test_one_bus)
         assert (
             os.path.exists(os.path.join(OUTPUT_PATH, "timeseries_all_busses.xlsx"))
@@ -150,15 +153,18 @@
         #     os.path.exists(os.path.join(OUTPUT_PATH, "a_bus_flows_365_days.png"))
         #     is True
         # )
 
     def test_store_each_bus_timeseries_to_excel_and_png_two_busses(self):
         """ """
         dict_timeseries_test_two_busses = {
-            PROJECT_DATA: {PROJECT_NAME: "a_project", SCENARIO_NAME: "a_scenario",},
+            PROJECT_DATA: {
+                PROJECT_NAME: "a_project",
+                SCENARIO_NAME: "a_scenario",
+            },
             SIMULATION_SETTINGS: {PATH_OUTPUT_FOLDER: OUTPUT_PATH},
             OPTIMIZED_FLOWS: {"a_bus": BUS, "b_bus": BUS},
         }
 
         dict_timeseries_test_two_busses.update(copy.deepcopy(DICT_PLOTS))
         F0.store_timeseries_all_busses_to_excel(dict_timeseries_test_two_busses)
         assert (
@@ -200,15 +206,15 @@
     @mock.patch(
         "argparse.ArgumentParser.parse_args",
         return_value=PARSER.parse_args(
             ["-f", "-log", "warning", "-o", OUTPUT_PATH, "-pdf"]
         ),
     )
     def test_generate_pdf_report(self, m_args):
-        """Run the simulation with -pdf option to make sure the pdf file is generated """
+        """Run the simulation with -pdf option to make sure the pdf file is generated"""
         main()
         assert os.path.exists(os.path.join(OUTPUT_PATH, PDF_REPORT)) is True
 
     def teardown_method(self):
         """ """
         if os.path.exists(OUTPUT_PATH):
             shutil.rmtree(OUTPUT_PATH, ignore_errors=True)
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_F1_plotting.py` & `multi_vector_simulator-1.1.1rc1/tests/test_F1_plotting.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_KPI.py` & `multi_vector_simulator-1.1.1rc1/tests/test_benchmark_KPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 In this module the tests run over whole simulation from main, not just single functions of modules
 
 What should differ between the different functions is the input file
 
 """
+
 import argparse
 import os
 import shutil
 import json
 
 import mock
 import pandas as pd
@@ -284,24 +285,27 @@
             else:
                 asset_data = data[asset_group][asset]
             # assertion
             for key in KEYS_TO_BE_EVALUATED_PER_ASSET:
                 assert (
                     key in asset_data
                 ), f"{key} is not in the asset data of {asset_group}, {asset}. It includes: {asset_data.keys()}."
-                if not pd.isna(expected_values.loc[asset, key]) and not pd.isna(asset_data[key][VALUE]):
+                if not pd.isna(expected_values.loc[asset, key]) and not pd.isna(
+                    asset_data[key][VALUE]
+                ):
                     assert float(expected_values.loc[asset, key]) == pytest.approx(
                         asset_data[key][VALUE], rel=1e-3
                     ), f"Parameter {key} of asset {asset} is not of expected value, expected {expected_values.loc[asset, key]}, got {asset_data[key][VALUE]}."
-                
+
         # Now we established that the externally calculated values are equal to the internally calculated values.
         # Therefore, we can now use the cost data from the assets to validate the cost data for the whole energy system.
 
         demand = pd.read_csv(
-            os.path.join(TEST_INPUT_PATH, USE_CASE, TIME_SERIES, "demand.csv"), sep=",",
+            os.path.join(TEST_INPUT_PATH, USE_CASE, TIME_SERIES, "demand.csv"),
+            sep=",",
         )
         aggregated_demand = demand.sum()[0]
 
         KEYS_TO_BE_EVALUATED_FOR_TOTAL_SYSTEM = {
             COST_INVESTMENT: 0,
             COST_UPFRONT: 0,
             COST_REPLACEMENT: 0,
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_constraints.py` & `multi_vector_simulator-1.1.1rc1/tests/test_benchmark_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 In this module the tests run over whole simulation from main, not just single functions of modules
 
 What should differ between the different functions is the input file
 
 """
+
 import argparse
 import os
 import shutil
 
 import pytest
 from pytest import approx
 import mock
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_feedin.py` & `multi_vector_simulator-1.1.1rc1/tests/test_benchmark_feedin.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_scenarios.py` & `multi_vector_simulator-1.1.1rc1/tests/test_benchmark_scenarios.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 In this module the tests run over whole simulation from main, not just single functions of modules
 
 What should differ between the different functions is the input file
 
 """
+
 import argparse
 import os
 import shutil
 import json
 
 import mock
 import pandas as pd
```

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_special_features.py` & `multi_vector_simulator-1.1.1rc1/tests/test_benchmark_special_features.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_benchmark_stratified_thermal_storage.py` & `multi_vector_simulator-1.1.1rc1/tests/test_benchmark_stratified_thermal_storage.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_input_folder_parameters.py` & `multi_vector_simulator-1.1.1rc1/tests/test_input_folder_parameters.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_sensitivity.py` & `multi_vector_simulator-1.1.1rc1/tests/test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.1.0rc2/tests/test_utils.py` & `multi_vector_simulator-1.1.1rc1/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
     def test_set_nested_value_with_unexisting_key_at_end_of_path(self):
         dct = dict(a=dict(a1=1, a2=2), b=dict(b1=dict(b11=11, b12=dict(b121=121))))
         with self.assertRaises(KeyError):
             set_nested_value(dct, 400, ("b", "b1", "b12", "b122"))
 
     def test_set_nested_value_with_unexisting_key_in_middle_of_path(self):
-        """because the path diverges """
+        """because the path diverges"""
         dct = dict(a=dict(a1=1, a2=2), b=dict(b1=dict(b11=11, b12=dict(b121=121))))
         with self.assertRaises(KeyError):
             set_nested_value(dct, 400, ("b", "d1", "b12", "b121"))
 
     def test_get_nested_value_with_unexisting_path(self):
         dct = dict(a=dict(a1=1, a2=2), b=dict(b1=dict(b11=11, b12=dict(b121=121))))
         with self.assertRaises(KeyError):
```


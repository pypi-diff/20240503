# Comparing `tmp/xenon_fuse-1.2.1.tar.gz` & `tmp/xenon_fuse-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenon_fuse-1.2.1.tar", max compression
+gzip compressed data, was "xenon_fuse-1.2.2.tar", max compression
```

## Comparing `xenon_fuse-1.2.1.tar` & `xenon_fuse-1.2.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1536 2024-04-24 11:35:16.193976 xenon_fuse-1.2.1/LICENSE
--rw-r--r--   0        0        0     1726 2024-04-24 11:35:16.193976 xenon_fuse-1.2.1/README.md
--rw-r--r--   0        0        0      204 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/__init__.py
--rw-r--r--   0        0        0     9142 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/common.py
--rw-r--r--   0        0        0     9697 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/context.py
--rw-r--r--   0        0        0     2785 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/dtypes.py
--rw-r--r--   0        0        0     2639 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugin.py
--rw-r--r--   0        0        0      241 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/__init__.py
--rw-r--r--   0        0        0      478 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/README.md
--rw-r--r--   0        0        0      593 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/__init__.py
--rw-r--r--   0        0        0     7963 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/csv_input.py
--rw-r--r--   0        0        0      615 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/__init__.py
--rw-r--r--   0        0        0     1055 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py
--rw-r--r--   0        0        0      803 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py
--rw-r--r--   0        0        0     2550 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py
--rw-r--r--   0        0        0      956 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py
--rw-r--r--   0        0        0     2017 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py
--rw-r--r--   0        0        0      837 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py
--rw-r--r--   0        0        0     8539 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py
--rw-r--r--   0        0        0    14728 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_drift.py
--rw-r--r--   0        0        0     4537 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_extraction.py
--rw-r--r--   0        0        0     3103 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_timing.py
--rw-r--r--   0        0        0     5453 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/s1_photon_hits.py
--rw-r--r--   0        0        0    13368 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/s1_photon_propagation.py
--rw-r--r--   0        0        0    34895 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/s2_photon_propagation.py
--rw-r--r--   0        0        0     9238 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/detector_physics/secondary_scintillation.py
--rw-r--r--   0        0        0      647 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/README.md
--rw-r--r--   0        0        0      459 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/__init__.py
--rw-r--r--   0        0        0     7280 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/detector_volumes.py
--rw-r--r--   0        0        0     2262 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/electric_field.py
--rw-r--r--   0        0        0     4556 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/find_cluster.py
--rw-r--r--   0        0        0    20236 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/input.py
--rw-r--r--   0        0        0     4424 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/merge_cluster.py
--rw-r--r--   0        0        0      456 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/microphysics_summary.py
--rw-r--r--   0        0        0     4305 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/wfsim_connection.py
--rw-r--r--   0        0        0    17364 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/micro_physics/yields.py
--rw-r--r--   0        0        0      152 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/README.md
--rw-r--r--   0        0        0      251 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/__init__.py
--rw-r--r--   0        0        0     9569 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/photon_pulses.py
--rw-r--r--   0        0        0      436 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/photon_summary.py
--rw-r--r--   0        0        0     8682 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/pmt_afterpulses.py
--rw-r--r--   0        0        0    20113 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py
--rw-r--r--   0        0        0      293 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/__init__.py
--rw-r--r--   0        0        0     2771 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/cluster_tagging.py
--rw-r--r--   0        0        0     2260 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/event_truth.py
--rw-r--r--   0        0        0     8331 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/peak_truth.py
--rw-r--r--   0        0        0     4784 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/records_truth.py
--rw-r--r--   0        0        0     1543 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/plugins/truth_information/surviving_clusters.py
--rw-r--r--   0        0        0      895 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/vertical_merger_plugin.py
--rw-r--r--   0        0        0     1041 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/fuse/volume_plugin.py
--rw-r--r--   0        0        0     1169 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      823 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/_utils.py
--rw-r--r--   0        0        0     1770 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_DetectorPhysics_csv.py
--rw-r--r--   0        0        0     3526 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_FullChain.py
--rw-r--r--   0        0        0     4900 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_FullChain_w_DelayedElectrons.py
--rw-r--r--   0        0        0     2490 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_MicroPhysics.py
--rw-r--r--   0        0        0     4560 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_deterministic_seed.py
--rw-r--r--   0        0        0     7134 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_input.py
--rw-r--r--   0        0        0     5000 2024-04-24 11:35:16.221976 xenon_fuse-1.2.1/tests/test_plugin_random_seed.py
--rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 xenon_fuse-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1536 2024-05-03 11:40:01.683310 xenon_fuse-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1823 2024-05-03 11:40:01.683310 xenon_fuse-1.2.2/README.md
+-rw-r--r--   0        0        0      204 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/__init__.py
+-rw-r--r--   0        0        0     9142 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/common.py
+-rw-r--r--   0        0        0     9697 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/context.py
+-rw-r--r--   0        0        0     2787 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/dtypes.py
+-rw-r--r--   0        0        0     2639 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugin.py
+-rw-r--r--   0        0        0      241 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/__init__.py
+-rw-r--r--   0        0        0      478 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/README.md
+-rw-r--r--   0        0        0      593 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/__init__.py
+-rw-r--r--   0        0        0     7963 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/csv_input.py
+-rw-r--r--   0        0        0      615 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/__init__.py
+-rw-r--r--   0        0        0     1055 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py
+-rw-r--r--   0        0        0      803 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py
+-rw-r--r--   0        0        0     2562 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py
+-rw-r--r--   0        0        0      960 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py
+-rw-r--r--   0        0        0     2017 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py
+-rw-r--r--   0        0        0      837 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py
+-rw-r--r--   0        0        0     8539 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py
+-rw-r--r--   0        0        0    14728 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_drift.py
+-rw-r--r--   0        0        0     4537 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_extraction.py
+-rw-r--r--   0        0        0     3103 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_timing.py
+-rw-r--r--   0        0        0     5457 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/s1_photon_hits.py
+-rw-r--r--   0        0        0    13372 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/s1_photon_propagation.py
+-rw-r--r--   0        0        0    35178 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/s2_photon_propagation.py
+-rw-r--r--   0        0        0     9238 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/secondary_scintillation.py
+-rw-r--r--   0        0        0      647 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/README.md
+-rw-r--r--   0        0        0      459 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/__init__.py
+-rw-r--r--   0        0        0     7280 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/detector_volumes.py
+-rw-r--r--   0        0        0     2262 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/electric_field.py
+-rw-r--r--   0        0        0     4556 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/find_cluster.py
+-rw-r--r--   0        0        0    20236 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/input.py
+-rw-r--r--   0        0        0     4424 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/merge_cluster.py
+-rw-r--r--   0        0        0      456 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/microphysics_summary.py
+-rw-r--r--   0        0        0     4305 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/wfsim_connection.py
+-rw-r--r--   0        0        0    17364 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/yields.py
+-rw-r--r--   0        0        0      152 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/README.md
+-rw-r--r--   0        0        0      251 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/__init__.py
+-rw-r--r--   0        0        0     9569 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/photon_pulses.py
+-rw-r--r--   0        0        0      436 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/photon_summary.py
+-rw-r--r--   0        0        0     8682 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/pmt_afterpulses.py
+-rw-r--r--   0        0        0    20113 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py
+-rw-r--r--   0        0        0      293 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/__init__.py
+-rw-r--r--   0        0        0     3892 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/cluster_tagging.py
+-rw-r--r--   0        0        0     2730 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/event_truth.py
+-rw-r--r--   0        0        0     8335 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/peak_truth.py
+-rw-r--r--   0        0        0     4784 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/records_truth.py
+-rw-r--r--   0        0        0     1543 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/surviving_clusters.py
+-rw-r--r--   0        0        0      895 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/vertical_merger_plugin.py
+-rw-r--r--   0        0        0     1041 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/volume_plugin.py
+-rw-r--r--   0        0        0     1169 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      823 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/_utils.py
+-rw-r--r--   0        0        0     1770 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_DetectorPhysics_csv.py
+-rw-r--r--   0        0        0     3530 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_FullChain.py
+-rw-r--r--   0        0        0     4908 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_FullChain_w_DelayedElectrons.py
+-rw-r--r--   0        0        0     2490 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_MicroPhysics.py
+-rw-r--r--   0        0        0     4560 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_deterministic_seed.py
+-rw-r--r--   0        0        0     7134 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_input.py
+-rw-r--r--   0        0        0     5000 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_plugin_random_seed.py
+-rw-r--r--   0        0        0     3347 1970-01-01 00:00:00.000000 xenon_fuse-1.2.2/PKG-INFO
```

### Comparing `xenon_fuse-1.2.1/LICENSE` & `xenon_fuse-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/README.md` & `xenon_fuse-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # XENON fuse
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/xenon-fuse.svg)](https://pypi.python.org/pypi/xenon-fuse/)
 [![Coverage Status](https://coveralls.io/repos/github/XENONnT/fuse/badge.svg)](https://coveralls.io/github/XENONnT/fuse)
 [![Test package](https://github.com/XENONnT/fuse/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/XENONnT/fuse/actions/workflows/pytest.yml)
 [![Readthedocs Badge](https://readthedocs.org/projects/fuse/badge/?version=latest)](https://xenon-fuse.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/XENONnT/fuse/main.svg)](https://results.pre-commit.ci/latest/github/XENONnT/fuse/main)
+[![DOI](https://zenodo.org/badge/622956443.svg)](https://zenodo.org/doi/10.5281/zenodo.11059395)
 
 **F**ramework for **U**nified **S**imulation of **E**vents
 
 fuse is the refactored version of the XENONnT simulation chain. The goal of this project is to unify [epix](https://github.com/XENONnT/epix) and [WFSim](https://github.com/XENONnT/WFSim) into a single program. fuse is based on the [strax framework](https://github.com/AxFoundation/strax), so that the simulation steps are encoded in plugins with defined inputs and outputs. This allows for a flexible and modular simulation chain.
 
 ## Installation
```

### Comparing `xenon_fuse-1.2.1/fuse/common.py` & `xenon_fuse-1.2.2/fuse/common.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/context.py` & `xenon_fuse-1.2.2/fuse/context.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/dtypes.py` & `xenon_fuse-1.2.2/fuse/dtypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 
 g4_fields = [
-    (("Time with respect to the start of the event [ns]", "t"), np.int64),
+    (("Time with respect to the start of the event [ns]", "t"), np.float64),
     (("Energy deposit [keV]", "ed"), np.float32),
     (("Particle type", "type"), "<U18"),
     (("Geant4 track ID", "trackid"), np.int16),
     (("Particle type of the parent particle", "parenttype"), "<U18"),
     (("Trackid of the parent particle", "parentid"), np.int16),
     (("Geant4 process creating the particle", "creaproc"), "<U25"),
     (("Geant4 process responsible for the energy deposit", "edproc"), "<U25"),
```

### Comparing `xenon_fuse-1.2.1/fuse/plugin.py` & `xenon_fuse-1.2.2/fuse/plugin.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/__init__.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/__init__.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/csv_input.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/csv_input.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/__init__.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/__init__.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,12 +78,12 @@
 
 
 @export
 class S1PhotonHitsMerger(VerticalMergerPlugin):
     """Plugin which concatenates the output of the regular and delayed s1
     photon hits plugins."""
 
-    depends_on = ("s1_photons", "delayed_s1_photons")
+    depends_on = ("s1_photon_hits", "delayed_s1_photon_hits")
 
-    provides = "merged_s1_photons"
+    provides = "merged_s1_photon_hits"
     data_kind = "interactions_in_roi"
-    __version__ = "0.0.1"
+    __version__ = "0.0.2"
```

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 log = logging.getLogger("fuse.detector_physics.delayed_electrons.delayed_electrons_s1photonhits")
 
 
 @export
 class S1PhotonHitsEmpty(FuseBasePlugin):
     """Plugin to return zeros for all S1 photon hits of delayed electrons."""
 
-    __version__ = "0.0.1"
+    __version__ = "0.0.2"
 
     depends_on = "photo_ionization_electrons"
-    provides = "delayed_s1_photons"
+    provides = "delayed_s1_photon_hits"
     data_kind = "delayed_interactions_in_roi"
 
     dtype = [
         (("Number detected S1 photons", "n_s1_photon_hits"), np.int32),
     ] + strax.time_fields
 
     def compute(self, delayed_interactions_in_roi):
```

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_drift.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_drift.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_extraction.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_extraction.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/electron_timing.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_timing.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/s1_photon_hits.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/s1_photon_hits.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 
 @export
 class S1PhotonHits(FuseBasePlugin):
     """Plugin to simulate the number of detected S1 photons using a S1 light
     collection efficiency map."""
 
-    __version__ = "0.2.0"
+    __version__ = "0.2.1"
 
     depends_on = "microphysics_summary"
-    provides = "s1_photons"
+    provides = "s1_photon_hits"
     data_kind = "interactions_in_roi"
 
     save_when = strax.SaveWhen.ALWAYS
 
     dtype = [
         (("Number detected S1 photons", "n_s1_photon_hits"), np.int32),
     ] + strax.time_fields
```

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/s1_photon_propagation.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/s1_photon_propagation.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     """Base plugin to simulate the propagation of S1 photons in the detector.
     Photons are randomly assigned to PMT channels based on their starting
     position and the timing of the photons is calculated.
 
     Note: The timing calculation is defined in the child plugin.
     """
 
-    __version__ = "0.3.1"
+    __version__ = "0.3.2"
 
-    depends_on = ("microphysics_summary", "s1_photons")
+    depends_on = ("microphysics_summary", "s1_photon_hits")
     provides = "propagated_s1_photons"
     data_kind = "s1_photons"
 
     save_when = strax.SaveWhen.TARGET
 
     dtype = propagated_photons_fields + strax.time_fields
```

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/s2_photon_propagation.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/s2_photon_propagation.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     """Base plugin to simulate the propagation of S2 photons in the detector.
     Photons are randomly assigned to PMT channels based on their starting
     position and the timing of the photons is calculated.
 
     Note: The timing calculation is defined in the child plugin.
     """
 
-    __version__ = "0.3.3"
+    __version__ = "0.3.4"
 
     depends_on = (
         "merged_electron_time",
         "merged_s2_photons",
         "merged_extracted_electrons",
         "merged_drifted_electrons",
         "merged_s2_photons_sum",
@@ -420,14 +420,17 @@
             _photon_channels=_photon_channels,
             _photon_gains=_photon_gains,
             _photon_is_dpe=_photon_is_dpe,
             _cluster_id=_cluster_id,
             photon_type=2,
         )
 
+        # Discard photons associated with negative channel numbers
+        result = result[result["channel"] >= 0]
+
         result = strax.sort_by_time(result)
 
         return result
 
     def photon_channels(self, n_electron, z_obs, positions, drift_time_mean, n_photons):
         channels = np.arange(self.n_tpc_pmts).astype(np.int64)
         top_index = np.arange(self.n_top_pmts)
@@ -462,15 +465,17 @@
                 _new_aft = _cur_aft * skewnorm.rvs(
                     loc=1.0, scale=self.s2_aft_sigma, a=self.s2_aft_skewness
                 )
                 _new_aft = np.clip(_new_aft, 0, 1)
                 pat[top_index] *= _new_aft / _cur_aft
                 pat[bottom_index] *= (1 - _new_aft) / (1 - _cur_aft)
 
-            # Pattern map return zeros
+            # If pattern map return zeros or has NAN values assign negative channel
+            # Photons with negative channel number will be rejected when
+            # building photon propagation output
             if np.isnan(pat).sum() > 0:
                 _photon_channels = np.array([-1] * n_ph)
 
             else:
                 _photon_channels = self.rng.choice(channels, size=n_ph, p=pat, replace=True)
 
             _buffer_photon_channels.append(_photon_channels)
```

### Comparing `xenon_fuse-1.2.1/fuse/plugins/detector_physics/secondary_scintillation.py` & `xenon_fuse-1.2.2/fuse/plugins/detector_physics/secondary_scintillation.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/micro_physics/README.md` & `xenon_fuse-1.2.2/fuse/plugins/micro_physics/README.md`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/micro_physics/detector_volumes.py` & `xenon_fuse-1.2.2/fuse/plugins/micro_physics/detector_volumes.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/micro_physics/electric_field.py` & `xenon_fuse-1.2.2/fuse/plugins/micro_physics/electric_field.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/micro_physics/find_cluster.py` & `xenon_fuse-1.2.2/fuse/plugins/micro_physics/find_cluster.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/micro_physics/input.py` & `xenon_fuse-1.2.2/fuse/plugins/micro_physics/input.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/micro_physics/merge_cluster.py` & `xenon_fuse-1.2.2/fuse/plugins/micro_physics/merge_cluster.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/micro_physics/wfsim_connection.py` & `xenon_fuse-1.2.2/fuse/plugins/micro_physics/wfsim_connection.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/micro_physics/yields.py` & `xenon_fuse-1.2.2/fuse/plugins/micro_physics/yields.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/photon_pulses.py` & `xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/photon_pulses.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/pmt_afterpulses.py` & `xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/pmt_afterpulses.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py` & `xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/truth_information/event_truth.py` & `xenon_fuse-1.2.2/fuse/plugins/truth_information/event_truth.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 import numpy as np
 
 export, __all__ = strax.exporter()
 
 
 @export
 class EventTruth(strax.Plugin):
-    __version__ = "0.0.3"
+    __version__ = "0.0.4"
 
     depends_on = ("microphysics_summary", "photon_summary", "peak_truth", "event_basics")
     provides = "event_truth"
     data_kind = "events"
 
     dtype = [
+        ("x_truth", np.float32),
+        ("y_truth", np.float32),
+        ("z_truth", np.float32),
         ("x_obs_truth", np.float32),
         ("y_obs_truth", np.float32),
         ("z_obs_truth", np.float32),
         ("energy_of_main_peaks_truth", np.float32),
         ("total_energy_in_event_truth", np.float32),
     ] + strax.time_fields
 
@@ -30,14 +33,23 @@
         result["time"] = events["time"]
         result["endtime"] = events["endtime"]
 
         for i, (pic, e) in enumerate(zip(peaks_in_event, events)):
             s1 = pic[e["s1_index"]]
             s2 = pic[e["s2_index"]]
 
+            result["x_truth"][i] = s2["average_x_of_contributing_clusters"]
+            result["y_truth"][i] = s2["average_y_of_contributing_clusters"]
+            result["z_truth"][i] = np.mean(
+                [
+                    s2["average_z_of_contributing_clusters"],
+                    s1["average_z_of_contributing_clusters"],
+                ]
+            )
+
             result["x_obs_truth"][i] = s2["average_x_obs_of_contributing_clusters"]
             result["y_obs_truth"][i] = s2["average_y_obs_of_contributing_clusters"]
             result["z_obs_truth"][i] = np.mean(
                 [
                     s2["average_z_obs_of_contributing_clusters"],
                     s1["average_z_obs_of_contributing_clusters"],
                 ]
```

### Comparing `xenon_fuse-1.2.1/fuse/plugins/truth_information/peak_truth.py` & `xenon_fuse-1.2.2/fuse/plugins/truth_information/peak_truth.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class PeakTruth(strax.OverlapWindowPlugin):
     __version__ = "0.0.5"
 
     depends_on = (
         "photon_summary",
         "peak_basics",
         "merged_microphysics_summary",
-        "merged_s1_photons",
+        "merged_s1_photon_hits",
         "merged_s2_photons_sum",
         "merged_drifted_electrons",
     )
     provides = "peak_truth"
     data_kind = "peaks"
 
     dtype = [
```

### Comparing `xenon_fuse-1.2.1/fuse/plugins/truth_information/records_truth.py` & `xenon_fuse-1.2.2/fuse/plugins/truth_information/records_truth.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/plugins/truth_information/surviving_clusters.py` & `xenon_fuse-1.2.2/fuse/plugins/truth_information/surviving_clusters.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/vertical_merger_plugin.py` & `xenon_fuse-1.2.2/fuse/vertical_merger_plugin.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/fuse/volume_plugin.py` & `xenon_fuse-1.2.2/fuse/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/pyproject.toml` & `xenon_fuse-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "xenon-fuse"
-version = "1.2.1"
+version = "1.2.2"
 description = "XENON Framework for Unified Simulations of Events"
 authors = [
   "Henning Schulze Eißing, <h_schu55@uni-muenster.de>",
   "Diego Ramírez García, <diego.ramirez@physik.uzh.ch>",
 ]
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `xenon_fuse-1.2.1/tests/_utils.py` & `xenon_fuse-1.2.2/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/tests/test_DetectorPhysics_csv.py` & `xenon_fuse-1.2.2/tests/test_DetectorPhysics_csv.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/tests/test_FullChain.py` & `xenon_fuse-1.2.2/tests/test_FullChain.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def tearDown(self):
         # self.temp_dir.cleanup()
         shutil.rmtree(self.temp_dir.name)
         os.makedirs(self.temp_dir.name)
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="S1PhotonHits timed out")
     def test_S1PhotonHits(self):
-        self.test_context.make(self.run_number, "s1_photons")
+        self.test_context.make(self.run_number, "s1_photon_hits")
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="S1PhotonPropagation timed out")
     def test_S1PhotonPropagation(self):
         self.test_context.make(self.run_number, "propagated_s1_photons")
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="ElectronDrift timed out")
     def test_ElectronDrift(self):
```

### Comparing `xenon_fuse-1.2.1/tests/test_FullChain_w_DelayedElectrons.py` & `xenon_fuse-1.2.2/tests/test_FullChain_w_DelayedElectrons.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         # self.temp_dir.cleanup()
         shutil.rmtree(self.temp_dir.name)
         os.makedirs(self.temp_dir.name)
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="S1PhotonHits timed out")
     def test_S1PhotonHits(self):
 
-        self.test_context.make(self.run_number, "s1_photons")
+        self.test_context.make(self.run_number, "s1_photon_hits")
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="S1PhotonPropagation timed out")
     def test_S1PhotonPropagation(self):
 
         self.test_context.make(self.run_number, "propagated_s1_photons")
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="ElectronDrift timed out")
@@ -110,15 +110,15 @@
         # self.test_context.make(self.run_number, "delayed_electrons_s2_photons_sum")
 
     @timeout_decorator.timeout(
         TIMEOUT, exception_message="DelayedElectronsS1PhotonHitsEmpty timed out"
     )
     def test_DelayedElectronsS1PhotonHitsEmpty(self):
 
-        self.test_context.make(self.run_number, "delayed_s1_photons")
+        self.test_context.make(self.run_number, "delayed_s1_photon_hits")
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="S2PhotonPropagation timed out")
     def test_S2PhotonPropagation(self):
 
         self.test_context.make(self.run_number, "propagated_s2_photons")
 
     @timeout_decorator.timeout(TIMEOUT, exception_message="PMTAfterPulses timed out")
```

### Comparing `xenon_fuse-1.2.1/tests/test_MicroPhysics.py` & `xenon_fuse-1.2.2/tests/test_MicroPhysics.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/tests/test_deterministic_seed.py` & `xenon_fuse-1.2.2/tests/test_deterministic_seed.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/tests/test_input.py` & `xenon_fuse-1.2.2/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/tests/test_plugin_random_seed.py` & `xenon_fuse-1.2.2/tests/test_plugin_random_seed.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.1/PKG-INFO` & `xenon_fuse-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenon-fuse
-Version: 1.2.1
+Version: 1.2.2
 Summary: XENON Framework for Unified Simulations of Events
 Home-page: https://github.com/XENONnT/fuse
 Author: Henning Schulze Eißing,
 Author-email: h_schu55@uni-muenster.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
@@ -40,14 +40,15 @@
 # XENON fuse
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/xenon-fuse.svg)](https://pypi.python.org/pypi/xenon-fuse/)
 [![Coverage Status](https://coveralls.io/repos/github/XENONnT/fuse/badge.svg)](https://coveralls.io/github/XENONnT/fuse)
 [![Test package](https://github.com/XENONnT/fuse/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/XENONnT/fuse/actions/workflows/pytest.yml)
 [![Readthedocs Badge](https://readthedocs.org/projects/fuse/badge/?version=latest)](https://xenon-fuse.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/XENONnT/fuse/main.svg)](https://results.pre-commit.ci/latest/github/XENONnT/fuse/main)
+[![DOI](https://zenodo.org/badge/622956443.svg)](https://zenodo.org/doi/10.5281/zenodo.11059395)
 
 **F**ramework for **U**nified **S**imulation of **E**vents
 
 fuse is the refactored version of the XENONnT simulation chain. The goal of this project is to unify [epix](https://github.com/XENONnT/epix) and [WFSim](https://github.com/XENONnT/WFSim) into a single program. fuse is based on the [strax framework](https://github.com/AxFoundation/strax), so that the simulation steps are encoded in plugins with defined inputs and outputs. This allows for a flexible and modular simulation chain.
 
 ## Installation
```


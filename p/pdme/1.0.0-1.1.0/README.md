# Comparing `tmp/pdme-1.0.0.tar.gz` & `tmp/pdme-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdme-1.0.0.tar", max compression
+gzip compressed data, was "pdme-1.1.0.tar", max compression
```

## Comparing `pdme-1.0.0.tar` & `pdme-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
--rw-r--r--   0        0        0     1229 2024-04-29 02:29:58.024469 pdme-1.0.0/README.md
--rw-r--r--   0        0        0      154 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/__init__.py
--rw-r--r--   0        0        0      184 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/inputs/__init__.py
--rw-r--r--   0        0        0      315 2024-04-29 02:30:19.109512 pdme-1.0.0/pdme/inputs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1471 2024-04-29 02:30:19.109512 pdme-1.0.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc
--rw-r--r--   0        0        0      688 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/inputs/dot_inputs.py
--rw-r--r--   0        0        0      536 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/measurement/__init__.py
--rw-r--r--   0        0        0      642 2024-04-29 02:30:20.821596 pdme-1.0.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1642 2024-04-29 02:30:20.825596 pdme-1.0.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc
--rw-r--r--   0        0        0     1864 2024-04-29 02:30:20.825596 pdme-1.0.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc
--rw-r--r--   0        0        0     1818 2024-04-29 02:30:20.833597 pdme-1.0.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc
--rw-r--r--   0        0        0     8295 2024-04-29 02:30:20.829597 pdme-1.0.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc
--rw-r--r--   0        0        0      984 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/measurement/dot_measure.py
--rw-r--r--   0        0        0     1224 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/measurement/dot_pair_measure.py
--rw-r--r--   0        0        0     1131 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/measurement/input_types.py
--rw-r--r--   0        0        0     5219 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/measurement/oscillating_dipole.py
--rw-r--r--   0        0        0       70 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/meta.py
--rw-r--r--   0        0        0     1066 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/model/__init__.py
--rw-r--r--   0        0        0      988 2024-04-29 02:30:20.861598 pdme-1.0.0/pdme/model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2740 2024-04-29 02:30:20.873599 pdme-1.0.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc
--rw-r--r--   0        0        0     5039 2024-04-29 02:30:20.885599 pdme-1.0.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc
--rw-r--r--   0        0        0     5083 2024-04-29 02:30:20.881599 pdme-1.0.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc
--rw-r--r--   0        0        0     4757 2024-04-29 02:30:20.885599 pdme-1.0.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc
--rw-r--r--   0        0        0     3850 2024-04-29 02:30:20.865599 pdme-1.0.0/pdme/model/__pycache__/model.cpython-39.pyc
--rw-r--r--   0        0        0     2928 2024-04-29 02:30:20.877599 pdme-1.0.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc
--rw-r--r--   0        0        0     3362 2024-04-29 02:30:20.877599 pdme-1.0.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc
--rw-r--r--   0        0        0     2367 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/model/fixed_magnitude_model.py
--rw-r--r--   0        0        0     5158 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
--rw-r--r--   0        0        0     5332 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/model/log_spaced_random_choice_model.py
--rw-r--r--   0        0        0     4699 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/model/log_spaced_random_choice_xy_model.py
--rw-r--r--   0        0        0     3594 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/model/model.py
--rw-r--r--   0        0        0     2560 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/model/multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0     3076 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0        0 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/py.typed
--rw-r--r--   0        0        0     1364 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/subspace_simulation/__init__.py
--rw-r--r--   0        0        0     2144 2024-04-29 02:30:20.865599 pdme-1.0.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      842 2024-04-29 02:30:20.869599 pdme-1.0.0/pdme/subspace_simulation/__pycache__/mcmc_costs.cpython-39.pyc
--rw-r--r--   0        0        0      575 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/subspace_simulation/mcmc_costs.py
--rw-r--r--   0        0        0        0 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/util/__init__.py
--rw-r--r--   0        0        0      167 2024-04-29 02:30:20.869599 pdme-1.0.0/pdme/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4177 2024-04-29 02:30:21.121611 pdme-1.0.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc
--rw-r--r--   0        0        0     3833 2024-04-29 02:30:20.869599 pdme-1.0.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc
--rw-r--r--   0        0        0     7925 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/util/fast_nonlocal_spectrum.py
--rw-r--r--   0        0        0     3604 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/util/fast_v_calc.py
--rw-r--r--   0        0        0      965 2024-04-29 02:29:58.028469 pdme-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 pdme-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1229 2024-05-02 23:07:06.298615 pdme-1.1.0/README.md
+-rw-r--r--   0        0        0      154 2024-05-02 23:07:06.302616 pdme-1.1.0/pdme/__init__.py
+-rw-r--r--   0        0        0     1578 2024-05-02 23:07:06.302616 pdme-1.1.0/pdme/calculations/__init__.py
+-rw-r--r--   0        0        0     1939 2024-05-02 23:07:43.852461 pdme-1.1.0/pdme/calculations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      184 2024-05-02 23:07:06.302616 pdme-1.1.0/pdme/inputs/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-02 23:07:44.144475 pdme-1.1.0/pdme/inputs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1471 2024-05-02 23:07:44.144475 pdme-1.1.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc
+-rw-r--r--   0        0        0      688 2024-05-02 23:07:06.302616 pdme-1.1.0/pdme/inputs/dot_inputs.py
+-rw-r--r--   0        0        0      536 2024-05-02 23:07:06.302616 pdme-1.1.0/pdme/measurement/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-02 23:07:44.184477 pdme-1.1.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1642 2024-05-02 23:07:44.188477 pdme-1.1.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc
+-rw-r--r--   0        0        0     1864 2024-05-02 23:07:44.188477 pdme-1.1.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc
+-rw-r--r--   0        0        0     1818 2024-05-02 23:07:44.196478 pdme-1.1.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc
+-rw-r--r--   0        0        0     9719 2024-05-02 23:07:44.196478 pdme-1.1.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc
+-rw-r--r--   0        0        0      984 2024-05-02 23:07:06.302616 pdme-1.1.0/pdme/measurement/dot_measure.py
+-rw-r--r--   0        0        0     1224 2024-05-02 23:07:06.302616 pdme-1.1.0/pdme/measurement/dot_pair_measure.py
+-rw-r--r--   0        0        0     1131 2024-05-02 23:07:06.302616 pdme-1.1.0/pdme/measurement/input_types.py
+-rw-r--r--   0        0        0     6903 2024-05-02 23:07:06.302616 pdme-1.1.0/pdme/measurement/oscillating_dipole.py
+-rw-r--r--   0        0        0       70 2024-05-02 23:07:06.302616 pdme-1.1.0/pdme/meta.py
+-rw-r--r--   0        0        0     1066 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/model/__init__.py
+-rw-r--r--   0        0        0      988 2024-05-02 23:07:44.240480 pdme-1.1.0/pdme/model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2740 2024-05-02 23:07:44.252481 pdme-1.1.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     5039 2024-05-02 23:07:44.268481 pdme-1.1.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc
+-rw-r--r--   0        0        0     5083 2024-05-02 23:07:44.260481 pdme-1.1.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc
+-rw-r--r--   0        0        0     4757 2024-05-02 23:07:44.264481 pdme-1.1.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc
+-rw-r--r--   0        0        0     3850 2024-05-02 23:07:44.244480 pdme-1.1.0/pdme/model/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0        0        0     2928 2024-05-02 23:07:44.256481 pdme-1.1.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     3362 2024-05-02 23:07:44.256481 pdme-1.1.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     2367 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/model/fixed_magnitude_model.py
+-rw-r--r--   0        0        0     5158 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
+-rw-r--r--   0        0        0     5332 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/model/log_spaced_random_choice_model.py
+-rw-r--r--   0        0        0     4699 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/model/log_spaced_random_choice_xy_model.py
+-rw-r--r--   0        0        0     3594 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/model/model.py
+-rw-r--r--   0        0        0     2560 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/model/multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0     3076 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0        0 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/py.typed
+-rw-r--r--   0        0        0     1364 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/subspace_simulation/__init__.py
+-rw-r--r--   0        0        0     2144 2024-05-02 23:07:44.244480 pdme-1.1.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      842 2024-05-02 23:07:44.248480 pdme-1.1.0/pdme/subspace_simulation/__pycache__/mcmc_costs.cpython-39.pyc
+-rw-r--r--   0        0        0      575 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/subspace_simulation/mcmc_costs.py
+-rw-r--r--   0        0        0        0 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/util/__init__.py
+-rw-r--r--   0        0        0      167 2024-05-02 23:07:44.248480 pdme-1.1.0/pdme/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4168 2024-05-02 23:07:44.528494 pdme-1.1.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc
+-rw-r--r--   0        0        0     3930 2024-05-02 23:07:44.252481 pdme-1.1.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc
+-rw-r--r--   0        0        0     9419 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/util/fast_nonlocal_spectrum.py
+-rw-r--r--   0        0        0     3707 2024-05-02 23:07:06.306616 pdme-1.1.0/pdme/util/fast_v_calc.py
+-rw-r--r--   0        0        0      965 2024-05-02 23:07:06.306616 pdme-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 pdme-1.1.0/PKG-INFO
```

### Comparing `pdme-1.0.0/README.md` & `pdme-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pdme - the python dipole model evaluator
 
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-green.svg?style=flat-square)](https://conventionalcommits.org)
 [![PyPI](https://img.shields.io/pypi/v/pdme?style=flat-square)](https://pypi.org/project/pdme/)
 [![Jenkins](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster&style=flat-square)](https://jenkins.deepak.science/job/gitea-physics/job/pdme/job/master/)
 ![Jenkins tests](https://img.shields.io/jenkins/tests?compact_message&jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)
 ![Jenkins Coverage](https://img.shields.io/jenkins/coverage/cobertura?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)
-![Maintenance](https://img.shields.io/maintenance/yes/2023?style=flat-square)
+![Maintenance](https://img.shields.io/maintenance/yes/2024?style=flat-square)
 
 This repo has library code for evaluating dipole models.
 
 ## Getting started
 
 `poetry install` to start locally
```

### Comparing `pdme-1.0.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc` & `pdme-1.1.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 688 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 b002 0000  a.......&./f....
+00000000: 610d 0d0a 0000 0000 9a1c 3466 b002 0000  a.........4f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6504 6500 6a03 6a06 1900  m.Z...e.e.j.j...
 00000060: 6504 6507 1900 6504 6505 6500 6a03 6a06  e.e...e.e.e.j.j.
 00000070: 6507 6602 1900 1900 6403 9c03 6404 6405  e.f.....d...d.d.
@@ -25,15 +25,15 @@
 00000180: 0200 0000 0400 0000 1300 0000 7314 0000  ............s...
 00000190: 0067 007c 005d 0c7d 0188 007c 0166 0291  .g.|.].}...|.f..
 000001a0: 0271 0453 00a9 0072 0700 0000 a902 da02  .q.S...r........
 000001b0: 2e30 da01 66a9 01da 0364 6f74 7207 0000  .0..f....dotr...
 000001c0: 00fa 502f 686f 6d65 2f6a 656e 6b69 6e73  ..P/home/jenkins
 000001d0: 2f61 6765 6e74 2f77 6f72 6b73 7061 6365  /agent/workspace
 000001e0: 2f67 6974 6561 2d70 6879 7369 6373 5f70  /gitea-physics_p
-000001f0: 646d 655f 312e 302e 302f 7064 6d65 2f69  dme_1.0.0/pdme/i
+000001f0: 646d 655f 312e 312e 302f 7064 6d65 2f69  dme_1.1.0/pdme/i
 00000200: 6e70 7574 732f 646f 745f 696e 7075 7473  nputs/dot_inputs
 00000210: 2e70 79da 0a3c 6c69 7374 636f 6d70 3e0a  .py..<listcomp>.
 00000220: 0000 00f3 0000 0000 7a3a 696e 7075 7473  ........z:inputs
 00000230: 5f77 6974 685f 6672 6571 7565 6e63 795f  _with_frequency_
 00000240: 7261 6e67 652e 3c6c 6f63 616c 733e 2e3c  range.<locals>.<
 00000250: 6c69 7374 636f 6d70 3e2e 3c6c 6973 7463  listcomp>.<listc
 00000260: 6f6d 703e 7207 0000 00a9 0172 0900 0000  omp>r......r....
```

### Comparing `pdme-1.0.0/pdme/inputs/dot_inputs.py` & `pdme-1.1.0/pdme/inputs/dot_inputs.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/measurement/__init__.py` & `pdme-1.1.0/pdme/measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc` & `pdme-1.1.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 536 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 1802 0000  a.......&./f....
+00000000: 610d 0d0a 0000 0000 9a1c 3466 1802 0000  a.........4f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 0100 6700  d.l.m.Z.m.Z...g.
 00000070: 6405 a201 5a0c 6406 5300 2907 e900 0000  d...Z.d.S.).....
@@ -30,12 +30,12 @@
 000001d0: 7207 0000 005a 1c70 646d 652e 6d65 6173  r....Z.pdme.meas
 000001e0: 7572 656d 656e 742e 696e 7075 745f 7479  urement.input_ty
 000001f0: 7065 7372 0800 0000 7209 0000 00da 075f  pesr....r......_
 00000200: 5f61 6c6c 5f5f a900 720b 0000 0072 0b00  _all__..r....r..
 00000210: 0000 fa53 2f68 6f6d 652f 6a65 6e6b 696e  ...S/home/jenkin
 00000220: 732f 6167 656e 742f 776f 726b 7370 6163  s/agent/workspac
 00000230: 652f 6769 7465 612d 7068 7973 6963 735f  e/gitea-physics_
-00000240: 7064 6d65 5f31 2e30 2e30 2f70 646d 652f  pdme_1.0.0/pdme/
+00000240: 7064 6d65 5f31 2e31 2e30 2f70 646d 652f  pdme_1.1.0/pdme/
 00000250: 6d65 6173 7572 656d 656e 742f 5f5f 696e  measurement/__in
 00000260: 6974 5f5f 2e70 79da 083c 6d6f 6475 6c65  it__.py..<module
 00000270: 3e01 0000 0073 0800 0000 1001 1004 1004  >....s..........
 00000280: 1003                                     ..
```

### Comparing `pdme-1.0.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc` & `pdme-1.1.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 984 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 d803 0000  a.......&./f....
+00000000: 610d 0d0a 0000 0000 9a1c 3466 d803 0000  a.........4f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a02 6501 4700 6403  Z.d.d.l.Z.e.G.d.
 00000050: 6404 8400 6404 8302 8301 5a04 6501 4700  d...d.....Z.e.G.
 00000060: 6405 6406 8400 6406 8302 8301 5a05 6402  d.d...d.....Z.d.
 00000070: 5300 2907 e900 0000 0029 01da 0964 6174  S.)......)...dat
@@ -32,15 +32,15 @@
 000001f0: 0000 4300 0000 7312 0000 0074 00a0 017c  ..C...s....t...|
 00000200: 006a 02a1 017c 005f 0264 0053 00a9 014e  .j...|._.d.S...N
 00000210: 2903 da05 6e75 6d70 79da 0561 7272 6179  )...numpy..array
 00000220: 7205 0000 00a9 01da 0473 656c 66a9 0072  r........self..r
 00000230: 0e00 0000 fa56 2f68 6f6d 652f 6a65 6e6b  .....V/home/jenk
 00000240: 696e 732f 6167 656e 742f 776f 726b 7370  ins/agent/worksp
 00000250: 6163 652f 6769 7465 612d 7068 7973 6963  ace/gitea-physic
-00000260: 735f 7064 6d65 5f31 2e30 2e30 2f70 646d  s_pdme_1.0.0/pdm
+00000260: 735f 7064 6d65 5f31 2e31 2e30 2f70 646d  s_pdme_1.1.0/pdm
 00000270: 652f 6d65 6173 7572 656d 656e 742f 646f  e/measurement/do
 00000280: 745f 6d65 6173 7572 652e 7079 da0d 5f5f  t_measure.py..__
 00000290: 706f 7374 5f69 6e69 745f 5f1b 0000 0073  post_init__....s
 000002a0: 0200 0000 0001 7a1c 446f 744d 6561 7375  ......z.DotMeasu
 000002b0: 7265 6d65 6e74 2e5f 5f70 6f73 745f 696e  rement.__post_in
 000002c0: 6974 5f5f a909 da08 5f5f 6e61 6d65 5f5f  it__....__name__
 000002d0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
```

### Comparing `pdme-1.0.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc` & `pdme-1.1.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 1224 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 c804 0000  a.......&./f....
+00000000: 610d 0d0a 0000 0000 9a1c 3466 c804 0000  a.........4f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a02 6501 4700 6403  Z.d.d.l.Z.e.G.d.
 00000050: 6404 8400 6404 8302 8301 5a04 6501 4700  d...d.....Z.e.G.
 00000060: 6405 6406 8400 6406 8302 8301 5a05 6402  d.d...d.....Z.d.
 00000070: 5300 2907 e900 0000 0029 01da 0964 6174  S.)......)...dat
@@ -38,15 +38,15 @@
 00000250: a001 7c00 6a02 a101 7c00 5f02 7400 a001  ..|.j...|._.t...
 00000260: 7c00 6a03 a101 7c00 5f03 6400 5300 a901  |.j...|._.d.S...
 00000270: 4e29 04da 056e 756d 7079 da05 6172 7261  N)...numpy..arra
 00000280: 7972 0500 0000 7206 0000 00a9 01da 0473  yr....r........s
 00000290: 656c 66a9 0072 0f00 0000 fa5b 2f68 6f6d  elf..r.....[/hom
 000002a0: 652f 6a65 6e6b 696e 732f 6167 656e 742f  e/jenkins/agent/
 000002b0: 776f 726b 7370 6163 652f 6769 7465 612d  workspace/gitea-
-000002c0: 7068 7973 6963 735f 7064 6d65 5f31 2e30  physics_pdme_1.0
+000002c0: 7068 7973 6963 735f 7064 6d65 5f31 2e31  physics_pdme_1.1
 000002d0: 2e30 2f70 646d 652f 6d65 6173 7572 656d  .0/pdme/measurem
 000002e0: 656e 742f 646f 745f 7061 6972 5f6d 6561  ent/dot_pair_mea
 000002f0: 7375 7265 2e70 79da 0d5f 5f70 6f73 745f  sure.py..__post_
 00000300: 696e 6974 5f5f 1f00 0000 7304 0000 0000  init__....s.....
 00000310: 010e 017a 2044 6f74 5061 6972 4d65 6173  ...z DotPairMeas
 00000320: 7572 656d 656e 742e 5f5f 706f 7374 5f69  urement.__post_i
 00000330: 6e69 745f 5fa9 09da 085f 5f6e 616d 655f  nit__....__name_
```

### Comparing `pdme-1.0.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc` & `pdme-1.1.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 1131 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 6b04 0000  a.......&./fk...
+00000000: 610d 0d0a 0000 0000 9a1c 3466 6b04 0000  a.........4fk...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6403 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6503 6501 6a02 6a0a 650b 6602 1900  ..e.e.j.j.e.f...
 00000070: 5a0c 6503 6501 6a02 6a0a 6501 6a02 6a0a  Z.e.e.j.j.e.j.j.
@@ -29,15 +29,15 @@
 000001c0: 0291 0271 0453 0029 0272 0100 0000 e901  ...q.S.).r......
 000001d0: 0000 00a9 03da 056e 756d 7079 da06 6170  .......numpy..ap
 000001e0: 7065 6e64 da05 6172 7261 79a9 02da 022e  pend..array.....
 000001f0: 30da 0569 6e70 7574 a900 7211 0000 00fa  0..input..r.....
 00000200: 562f 686f 6d65 2f6a 656e 6b69 6e73 2f61  V/home/jenkins/a
 00000210: 6765 6e74 2f77 6f72 6b73 7061 6365 2f67  gent/workspace/g
 00000220: 6974 6561 2d70 6879 7369 6373 5f70 646d  itea-physics_pdm
-00000230: 655f 312e 302e 302f 7064 6d65 2f6d 6561  e_1.0.0/pdme/mea
+00000230: 655f 312e 312e 302f 7064 6d65 2f6d 6561  e_1.1.0/pdme/mea
 00000240: 7375 7265 6d65 6e74 2f69 6e70 7574 5f74  surement/input_t
 00000250: 7970 6573 2e70 79da 0a3c 6c69 7374 636f  ypes.py..<listco
 00000260: 6d70 3e0d 0000 00f3 0000 0000 7a27 646f  mp>.........z'do
 00000270: 745f 696e 7075 7473 5f74 6f5f 6172 7261  t_inputs_to_arra
 00000280: 792e 3c6c 6f63 616c 733e 2e3c 6c69 7374  y.<locals>.<list
 00000290: 636f 6d70 3ea9 0272 0b00 0000 720d 0000  comp>..r....r...
 000002a0: 0029 0172 0700 0000 7211 0000 0072 1100  .).r....r....r..
```

### Comparing `pdme-1.0.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc` & `pdme-1.1.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 5219 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,519 +1,608 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 6314 0000  a.......&./fc...
+00000000: 610d 0d0a 0000 0000 9a1c 3466 f71a 0000  a.........4f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a02 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6404 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
-00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6406 6c0d  m.Z.m.Z...d.d.l.
-00000080: 6d0e 5a0e 6d0f 5a0f 0100 6501 4700 6407  m.Z.m.Z...e.G.d.
-00000090: 6408 8400 6408 8302 8301 5a10 4700 6409  d...d.....Z.G.d.
-000000a0: 640a 8400 640a 8302 5a11 6402 5300 290b  d...d...Z.d.S.).
-000000b0: e900 0000 0029 01da 0964 6174 6163 6c61  .....)...datacla
-000000c0: 7373 4e29 02da 0853 6571 7565 6e63 65da  ssN)...Sequence.
-000000d0: 044c 6973 7429 02da 0e44 6f74 4d65 6173  .List)...DotMeas
-000000e0: 7572 656d 656e 74da 1344 6f74 5261 6e67  urement..DotRang
-000000f0: 654d 6561 7375 7265 6d65 6e74 2902 da12  eMeasurement)...
-00000100: 446f 7450 6169 724d 6561 7375 7265 6d65  DotPairMeasureme
-00000110: 6e74 da17 446f 7450 6169 7252 616e 6765  nt..DotPairRange
-00000120: 4d65 6173 7572 656d 656e 7429 02da 0844  Measurement)...D
-00000130: 6f74 496e 7075 74da 0c44 6f74 5061 6972  otInput..DotPair
-00000140: 496e 7075 7463 0000 0000 0000 0000 0000  Inputc..........
-00000150: 0000 0000 0000 0500 0000 4000 0000 739a  ..........@...s.
-00000160: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-00000170: 0365 046a 0565 0664 023c 0065 046a 0565  .e.j.e.d.<.e.j.e
-00000180: 0664 033c 0065 0765 0664 043c 0064 0564  .d.<.e.e.d.<.d.d
-00000190: 069c 0164 0764 0884 045a 0865 046a 0565  ...d.d...Z.e.j.e
-000001a0: 0765 0764 099c 0364 0a64 0b84 045a 0965  .e.d...d.d...Z.e
-000001b0: 046a 0565 0764 0c9c 0264 0d64 0e84 045a  .j.e.d...d.d...Z
-000001c0: 0a65 0765 0764 0f9c 0264 1064 1184 045a  .e.e.d...d.d...Z
-000001d0: 0b65 046a 0565 046a 0565 0765 0764 129c  .e.j.e.j.e.e.d..
-000001e0: 0464 1364 1484 045a 0c65 046a 0564 069c  .d.d...Z.e.j.d..
-000001f0: 0164 1564 1684 045a 0d64 0553 0029 17da  .d.d...Z.d.S.)..
-00000200: 114f 7363 696c 6c61 7469 6e67 4469 706f  .OscillatingDipo
-00000210: 6c65 6107 0100 000a 0952 6570 7265 7365  lea......Represe
-00000220: 6e74 6174 696f 6e20 6f66 2061 6e20 6f73  ntation of an os
-00000230: 6369 6c6c 6174 696e 6720 6469 706f 6c65  cillating dipole
-00000240: 2c20 6569 7468 6572 206b 6e6f 776e 206f  , either known o
-00000250: 7220 6775 6573 7365 642e 0a0a 0950 6172  r guessed....Par
-00000260: 616d 6574 6572 730a 092d 2d2d 2d2d 2d2d  ameters..-------
-00000270: 2d2d 2d0a 0970 203a 206e 756d 7079 2e6e  ---..p : numpy.n
-00000280: 6461 7272 6179 0a09 5468 6520 6f73 6369  darray..The osci
-00000290: 6c6c 6174 696e 6720 6469 706f 6c65 206d  llating dipole m
-000002a0: 6f6d 656e 742c 2077 6974 6820 6f76 6572  oment, with over
-000002b0: 616c 6c20 7369 676e 2061 7262 6974 7261  all sign arbitra
-000002c0: 7279 2e0a 0a09 7320 3a20 6e75 6d70 792e  ry....s : numpy.
-000002d0: 6e64 6172 7261 790a 0954 6865 2070 6f73  ndarray..The pos
-000002e0: 6974 696f 6e20 6f66 2074 6865 2064 6970  ition of the dip
-000002f0: 6f6c 652e 0a0a 0977 203a 2066 6c6f 6174  ole....w : float
-00000300: 0a09 5468 6520 6f73 6369 6c6c 6174 696f  ..The oscillatio
-00000310: 6e20 6672 6571 7565 6e63 792e 0a09 da01  n frequency.....
-00000320: 70da 0173 da01 774e a901 da06 7265 7475  p..s..wN....retu
-00000330: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
-00000340: 0000 0003 0000 0043 0000 0073 2000 0000  .......C...s ...
-00000350: 7400 a001 7c00 6a02 a101 7c00 5f02 7400  t...|.j...|._.t.
-00000360: a001 7c00 6a03 a101 7c00 5f03 6401 5300  ..|.j...|._.d.S.
-00000370: 2902 7a2a 0a09 0943 6f65 7263 6520 7468  ).z*...Coerce th
-00000380: 6520 696e 7075 7473 2069 6e74 6f20 6e75  e inputs into nu
-00000390: 6d70 7920 6172 7261 7973 2e0a 0909 4e29  mpy arrays....N)
-000003a0: 04da 056e 756d 7079 da05 6172 7261 7972  ...numpy..arrayr
-000003b0: 0c00 0000 720d 0000 00a9 01da 0473 656c  ....r........sel
-000003c0: 66a9 0072 1500 0000 fa5d 2f68 6f6d 652f  f..r.....]/home/
-000003d0: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
-000003e0: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
-000003f0: 7973 6963 735f 7064 6d65 5f31 2e30 2e30  ysics_pdme_1.0.0
-00000400: 2f70 646d 652f 6d65 6173 7572 656d 656e  /pdme/measuremen
-00000410: 742f 6f73 6369 6c6c 6174 696e 675f 6469  t/oscillating_di
-00000420: 706f 6c65 2e70 79da 0d5f 5f70 6f73 745f  pole.py..__post_
-00000430: 696e 6974 5f5f 2200 0000 7304 0000 0000  init__"...s.....
-00000440: 040e 017a 1f4f 7363 696c 6c61 7469 6e67  ...z.Oscillating
-00000450: 4469 706f 6c65 2e5f 5f70 6f73 745f 696e  Dipole.__post_in
-00000460: 6974 5f5f 2903 da01 72da 0166 7210 0000  it__)...r..fr...
-00000470: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
-00000480: 0000 0400 0000 4300 0000 7318 0000 007c  ......C...s....|
-00000490: 00a0 007c 01a1 0164 0113 007c 00a0 017c  ...|...d...|...|
-000004a0: 02a1 0114 0053 0029 027a ba0a 0909 5265  .....S.).z....Re
-000004b0: 7475 726e 7320 7468 6520 6e6f 6973 6520  turns the noise 
-000004c0: 706f 7465 6e74 6961 6c20 6174 2061 2070  potential at a p
-000004d0: 6f69 6e74 2072 2c20 6174 2073 6f6d 6520  oint r, at some 
-000004e0: 6672 6571 7565 6e63 7920 662e 0a0a 0909  frequency f.....
-000004f0: 5061 7261 6d65 7465 7273 0a09 092d 2d2d  Parameters...---
-00000500: 2d2d 2d2d 2d2d 2d0a 0909 7220 3a20 6e75  -------...r : nu
-00000510: 6d70 792e 6e64 6172 7261 790a 0909 5468  mpy.ndarray...Th
-00000520: 6520 706f 7369 7469 6f6e 206f 6620 7468  e position of th
-00000530: 6520 646f 742e 0a0a 0909 6620 3a20 666c  e dot.....f : fl
-00000540: 6f61 740a 0909 5468 6520 646f 7420 6672  oat...The dot fr
-00000550: 6571 7565 6e63 7920 746f 2073 616d 706c  equency to sampl
-00000560: 652e 0a09 09e9 0200 0000 a902 da06 5f61  e............._a
-00000570: 6c70 6861 da02 5f62 2903 7214 0000 0072  lpha.._b).r....r
-00000580: 1800 0000 7219 0000 0072 1500 0000 7215  ....r....r....r.
-00000590: 0000 0072 1600 0000 da0d 735f 6174 5f70  ...r......s_at_p
-000005a0: 6f73 6974 696f 6e29 0000 0073 0200 0000  osition)...s....
-000005b0: 000c 7a1f 4f73 6369 6c6c 6174 696e 6744  ..z.OscillatingD
-000005c0: 6970 6f6c 652e 735f 6174 5f70 6f73 6974  ipole.s_at_posit
-000005d0: 696f 6e29 0272 1800 0000 7210 0000 0063  ion).r....r....c
-000005e0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-000005f0: 0400 0000 4300 0000 7326 0000 007c 017c  ....C...s&...|.|
-00000600: 006a 0018 007d 027c 006a 01a0 027c 02a1  .j...}.|.j...|..
-00000610: 0174 036a 04a0 057c 02a1 0164 0113 001b  .t.j...|...d....
-00000620: 0053 0029 024e e903 0000 0029 0672 0d00  .S.).N.....).r..
-00000630: 0000 720c 0000 00da 0364 6f74 7211 0000  ..r......dotr...
-00000640: 00da 066c 696e 616c 67da 046e 6f72 6d29  ...linalg..norm)
-00000650: 0372 1400 0000 7218 0000 00da 0464 6966  .r....r......dif
-00000660: 6672 1500 0000 7215 0000 0072 1600 0000  fr....r....r....
-00000670: 721c 0000 0037 0000 0073 0400 0000 0001  r....7...s......
-00000680: 0a01 7a18 4f73 6369 6c6c 6174 696e 6744  ..z.OscillatingD
-00000690: 6970 6f6c 652e 5f61 6c70 6861 2902 7219  ipole._alpha).r.
-000006a0: 0000 0072 1000 0000 6302 0000 0000 0000  ...r....c.......
-000006b0: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
-000006c0: 0073 2200 0000 6401 7400 6a01 1b00 7c00  .s"...d.t.j...|.
-000006d0: 6a02 7c01 6402 1300 7c00 6a02 6402 1300  j.|.d...|.j.d...
-000006e0: 1700 1b00 1400 5300 2903 4ee9 0100 0000  ......S.).N.....
-000006f0: 721a 0000 0029 0372 1100 0000 da02 7069  r....).r......pi
-00000700: 720e 0000 0029 0272 1400 0000 7219 0000  r....).r....r...
-00000710: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000720: 721d 0000 003b 0000 0073 0200 0000 0001  r....;...s......
-00000730: 7a14 4f73 6369 6c6c 6174 696e 6744 6970  z.OscillatingDip
-00000740: 6f6c 652e 5f62 2904 da02 7231 da02 7232  ole._b)...r1..r2
-00000750: 7219 0000 0072 1000 0000 6304 0000 0000  r....r....c.....
-00000760: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-00000770: 0000 0073 1e00 0000 7c00 a000 7c01 a101  ...s....|...|...
-00000780: 7c00 a000 7c02 a101 1400 7c00 a001 7c03  |...|.....|...|.
-00000790: a101 1400 5300 a901 4e72 1b00 0000 2904  ....S...Nr....).
-000007a0: 7214 0000 0072 2600 0000 7227 0000 0072  r....r&...r'...r
-000007b0: 1900 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-000007c0: 0000 00da 0e73 5f66 6f72 5f64 6f74 5f70  .....s_for_dot_p
-000007d0: 6169 723e 0000 0073 0200 0000 0001 7a20  air>...s......z 
-000007e0: 4f73 6369 6c6c 6174 696e 6744 6970 6f6c  OscillatingDipol
-000007f0: 652e 735f 666f 725f 646f 745f 7061 6972  e.s_for_dot_pair
-00000800: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000810: 0007 0000 0043 0000 0073 1e00 0000 7400  .....C...s....t.
-00000820: a001 7c00 6a02 7c00 6a03 7400 a004 7c00  ..|.j.|.j.t...|.
-00000830: 6a05 6701 a101 6703 a101 5300 7228 0000  j.g...g...S.r(..
-00000840: 0029 0672 1100 0000 da0b 636f 6e63 6174  .).r......concat
-00000850: 656e 6174 6572 0c00 0000 720d 0000 0072  enater....r....r
-00000860: 1200 0000 720e 0000 0072 1300 0000 7215  ....r....r....r.
-00000870: 0000 0072 1500 0000 7216 0000 00da 0d74  ...r....r......t
-00000880: 6f5f 666c 6174 5f61 7272 6179 4100 0000  o_flat_arrayA...
-00000890: 7302 0000 0000 017a 1f4f 7363 696c 6c61  s......z.Oscilla
-000008a0: 7469 6e67 4469 706f 6c65 2e74 6f5f 666c  tingDipole.to_fl
-000008b0: 6174 5f61 7272 6179 290e da08 5f5f 6e61  at_array)...__na
-000008c0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000008d0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-000008e0: 5f5f 646f 635f 5f72 1100 0000 da07 6e64  __doc__r......nd
-000008f0: 6172 7261 79da 0f5f 5f61 6e6e 6f74 6174  array..__annotat
-00000900: 696f 6e73 5f5f da05 666c 6f61 7472 1700  ions__..floatr..
-00000910: 0000 721e 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00000920: 0072 2900 0000 722b 0000 0072 1500 0000  .r)...r+...r....
-00000930: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000940: 0b00 0000 0d00 0000 7314 0000 000a 0204  ........s.......
-00000950: 0f0a 010a 0108 020e 0714 0e12 0410 0318  ................
-00000960: 0372 0b00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000970: 0000 0000 0000 0005 0000 0040 0000 0073  ...........@...s
-00000980: e200 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00000990: 6504 6505 1900 6402 9c01 6403 6404 8404  e.e...d...d.d...
-000009a0: 5a06 6507 6508 6405 9c02 6406 6407 8404  Z.e.e.d...d.d...
-000009b0: 5a09 650a 650b 6408 9c02 6409 640a 8404  Z.e.e.d...d.d...
-000009c0: 5a0c 6504 6507 1900 650d 6508 1900 640b  Z.e.e...e.e...d.
-000009d0: 9c02 640c 640d 8404 5a0e 6504 650a 1900  ..d.d...Z.e.e...
-000009e0: 650d 650b 1900 640e 9c02 640f 6410 8404  e.e...d...d.d...
-000009f0: 5a0f 6507 6510 6510 6511 6411 9c04 6412  Z.e.e.e.e.d...d.
-00000a00: 6413 8404 5a12 6504 6507 1900 6510 6510  d...Z.e.e...e.e.
-00000a10: 650d 6511 1900 6414 9c04 6415 6416 8404  e.e...d...d.d...
-00000a20: 5a13 650a 6510 6510 6514 6417 9c04 6418  Z.e.e.e.e.d...d.
-00000a30: 6419 8404 5a15 6504 650a 1900 6510 6510  d...Z.e.e...e.e.
-00000a40: 650d 6514 1900 641a 9c04 641b 641c 8404  e.e...d...d.d...
-00000a50: 5a16 6517 6a18 641d 9c01 641e 641f 8404  Z.e.j.d...d.d...
-00000a60: 5a19 6420 5300 2921 da1c 4f73 6369 6c6c  Z.d S.)!..Oscill
-00000a70: 6174 696e 6744 6970 6f6c 6541 7272 616e  atingDipoleArran
-00000a80: 6765 6d65 6e74 7a9d 0a09 4120 636f 6c6c  gementz...A coll
-00000a90: 6563 7469 6f6e 206f 6620 6f73 6369 6c6c  ection of oscill
-00000aa0: 6174 696e 6720 6469 706f 6c65 732c 2077  ating dipoles, w
-00000ab0: 6869 6368 2077 6520 6172 6520 696e 7465  hich we are inte
-00000ac0: 7265 7374 6564 2069 6e20 6265 696e 6720  rested in being 
-00000ad0: 6162 6c65 2074 6f20 6368 6172 6163 7465  able to characte
-00000ae0: 7269 7365 2e0a 0a09 5061 7261 6d65 7465  rise....Paramete
-00000af0: 7273 0a09 2d2d 2d2d 2d2d 2d2d 0a09 6469  rs..--------..di
-00000b00: 706f 6c65 7320 3a20 5365 7175 656e 6365  poles : Sequence
-00000b10: 5b4f 7363 696c 6c61 7469 6e67 4469 706f  [OscillatingDipo
-00000b20: 6c65 5d0a 09a9 01da 0764 6970 6f6c 6573  le]......dipoles
-00000b30: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000b40: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
-00000b50: 7c00 5f00 6400 5300 7228 0000 0072 3400  |._.d.S.r(...r4.
-00000b60: 0000 2902 7214 0000 0072 3500 0000 7215  ..).r....r5...r.
-00000b70: 0000 0072 1500 0000 7216 0000 00da 085f  ...r....r......_
-00000b80: 5f69 6e69 745f 5f4e 0000 0073 0200 0000  _init__N...s....
-00000b90: 0001 7a25 4f73 6369 6c6c 6174 696e 6744  ..z%OscillatingD
-00000ba0: 6970 6f6c 6541 7272 616e 6765 6d65 6e74  ipoleArrangement
-00000bb0: 2e5f 5f69 6e69 745f 5f29 02da 0964 6f74  .__init__)...dot
-00000bc0: 5f69 6e70 7574 7210 0000 0063 0200 0000  _inputr....c....
-00000bd0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000be0: 0300 0000 7338 0000 0074 00a0 017c 0164  ....s8...t...|.d
-00000bf0: 0119 00a1 0189 017c 0164 0219 0089 0074  .......|.d.....t
-00000c00: 0274 0387 0087 0166 0264 0364 0484 087c  .t.....f.d.d...|
-00000c10: 006a 0444 0083 0183 0188 0188 0083 0353  .j.D...........S
-00000c20: 0029 054e 7201 0000 0072 2400 0000 6301  .).Nr....r$...c.
-00000c30: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00000c40: 0000 0013 0000 0073 1800 0000 6700 7c00  .......s....g.|.
-00000c50: 5d10 7d01 7c01 a000 8801 8800 a102 9102  ].}.|...........
-00000c60: 7104 5300 7215 0000 00a9 0172 1e00 0000  q.S.r......r....
-00000c70: a902 da02 2e30 5a06 6469 706f 6c65 a902  .....0Z.dipole..
-00000c80: 7219 0000 0072 1800 0000 7215 0000 0072  r....r....r....r
-00000c90: 1600 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
-00000ca0: 5500 0000 f300 0000 007a 444f 7363 696c  U........zDOscil
-00000cb0: 6c61 7469 6e67 4469 706f 6c65 4172 7261  latingDipoleArra
-00000cc0: 6e67 656d 656e 742e 6765 745f 646f 745f  ngement.get_dot_
-00000cd0: 6d65 6173 7572 656d 656e 742e 3c6c 6f63  measurement.<loc
-00000ce0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e29  als>.<listcomp>)
-00000cf0: 0572 1100 0000 7212 0000 0072 0500 0000  .r....r....r....
-00000d00: da03 7375 6d72 3500 0000 2902 7214 0000  ..sumr5...).r...
-00000d10: 0072 3700 0000 7215 0000 0072 3b00 0000  .r7...r....r;...
-00000d20: 7216 0000 00da 1367 6574 5f64 6f74 5f6d  r......get_dot_m
-00000d30: 6561 7375 7265 6d65 6e74 5100 0000 730a  easurementQ...s.
-00000d40: 0000 0000 010e 0108 0102 011c ff7a 304f  .............z0O
-00000d50: 7363 696c 6c61 7469 6e67 4469 706f 6c65  scillatingDipole
-00000d60: 4172 7261 6e67 656d 656e 742e 6765 745f  Arrangement.get_
-00000d70: 646f 745f 6d65 6173 7572 656d 656e 7429  dot_measurement)
-00000d80: 02da 0e64 6f74 5f70 6169 725f 696e 7075  ...dot_pair_inpu
-00000d90: 7472 1000 0000 6302 0000 0000 0000 0000  tr....c.........
-00000da0: 0000 0002 0000 0005 0000 0003 0000 0073  ...............s
-00000db0: 4a00 0000 7400 a001 7c01 6401 1900 a101  J...t...|.d.....
-00000dc0: 8901 7400 a001 7c01 6402 1900 a101 8902  ..t...|.d.......
-00000dd0: 7c01 6403 1900 8900 7402 7403 8700 8701  |.d.....t.t.....
-00000de0: 8702 6603 6404 6405 8408 7c00 6a04 4400  ..f.d.d...|.j.D.
-00000df0: 8301 8301 8801 8802 8800 8304 5300 2906  ............S.).
-00000e00: 4e72 0100 0000 7224 0000 0072 1a00 0000  Nr....r$...r....
-00000e10: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000e20: 0007 0000 0013 0000 0073 1a00 0000 6700  .........s....g.
-00000e30: 7c00 5d12 7d01 7c01 a000 8801 8802 8800  |.].}.|.........
-00000e40: a103 9102 7104 5300 7215 0000 00a9 0172  ....q.S.r......r
-00000e50: 2900 0000 7239 0000 00a9 0372 1900 0000  )...r9.....r....
-00000e60: 7226 0000 0072 2700 0000 7215 0000 0072  r&...r'...r....r
-00000e70: 1600 0000 723c 0000 005f 0000 0072 3d00  ....r<..._...r=.
-00000e80: 0000 7a49 4f73 6369 6c6c 6174 696e 6744  ..zIOscillatingD
-00000e90: 6970 6f6c 6541 7272 616e 6765 6d65 6e74  ipoleArrangement
-00000ea0: 2e67 6574 5f64 6f74 5f70 6169 725f 6d65  .get_dot_pair_me
-00000eb0: 6173 7572 656d 656e 742e 3c6c 6f63 616c  asurement.<local
-00000ec0: 733e 2e3c 6c69 7374 636f 6d70 3e29 0572  s>.<listcomp>).r
-00000ed0: 1100 0000 7212 0000 0072 0700 0000 723e  ....r....r....r>
-00000ee0: 0000 0072 3500 0000 2902 7214 0000 0072  ...r5...).r....r
-00000ef0: 4000 0000 7215 0000 0072 4200 0000 7216  @...r....rB...r.
-00000f00: 0000 00da 1867 6574 5f64 6f74 5f70 6169  .....get_dot_pai
-00000f10: 725f 6d65 6173 7572 656d 656e 7458 0000  r_measurementX..
-00000f20: 0073 1200 0000 0003 0e01 0e01 0801 0201  .s..............
-00000f30: 1a01 0201 0201 02fc 7a35 4f73 6369 6c6c  ........z5Oscill
-00000f40: 6174 696e 6744 6970 6f6c 6541 7272 616e  atingDipoleArran
-00000f50: 6765 6d65 6e74 2e67 6574 5f64 6f74 5f70  gement.get_dot_p
-00000f60: 6169 725f 6d65 6173 7572 656d 656e 7429  air_measurement)
-00000f70: 02da 0a64 6f74 5f69 6e70 7574 7372 1000  ...dot_inputsr..
-00000f80: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00000f90: 0000 0003 0000 0003 0000 0073 1200 0000  ...........s....
-00000fa0: 8700 6601 6401 6402 8408 7c01 4400 8301  ..f.d.d...|.D...
-00000fb0: 5300 2903 7a7e 0a09 0946 6f72 2061 2073  S.).z~...For a s
-00000fc0: 6572 6965 7320 6f66 2070 6f69 6e74 732c  eries of points,
-00000fd0: 2065 6163 6820 7769 7468 2074 6872 6565   each with three
-00000fe0: 2063 6f6f 7264 696e 6174 6573 2061 6e64   coordinates and
-00000ff0: 2061 2066 7265 7175 656e 6379 2c20 7265   a frequency, re
-00001000: 7475 726e 2061 206c 6973 7420 6f66 2074  turn a list of t
-00001010: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
-00001020: 2044 6f74 4d65 6173 7572 656d 656e 7473   DotMeasurements
-00001030: 2e0a 0909 6301 0000 0000 0000 0000 0000  ....c...........
-00001040: 0002 0000 0005 0000 0013 0000 0073 1600  .............s..
-00001050: 0000 6700 7c00 5d0e 7d01 8800 a000 7c01  ..g.|.].}.....|.
-00001060: a101 9102 7104 5300 7215 0000 0029 0172  ....q.S.r....).r
-00001070: 3f00 0000 a902 723a 0000 0072 3700 0000  ?.....r:...r7...
-00001080: 7213 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00001090: 3c00 0000 6b00 0000 723d 0000 007a 454f  <...k...r=...zEO
-000010a0: 7363 696c 6c61 7469 6e67 4469 706f 6c65  scillatingDipole
-000010b0: 4172 7261 6e67 656d 656e 742e 6765 745f  Arrangement.get_
-000010c0: 646f 745f 6d65 6173 7572 656d 656e 7473  dot_measurements
-000010d0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000010e0: 6f6d 703e 7215 0000 0029 0272 1400 0000  omp>r....).r....
-000010f0: 7244 0000 0072 1500 0000 7213 0000 0072  rD...r....r....r
-00001100: 1600 0000 da14 6765 745f 646f 745f 6d65  ......get_dot_me
-00001110: 6173 7572 656d 656e 7473 6500 0000 7302  asurementse...s.
-00001120: 0000 0000 067a 314f 7363 696c 6c61 7469  .....z1Oscillati
-00001130: 6e67 4469 706f 6c65 4172 7261 6e67 656d  ngDipoleArrangem
-00001140: 656e 742e 6765 745f 646f 745f 6d65 6173  ent.get_dot_meas
-00001150: 7572 656d 656e 7473 2902 da0f 646f 745f  urements)...dot_
-00001160: 7061 6972 5f69 6e70 7574 7372 1000 0000  pair_inputsr....
-00001170: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001180: 0003 0000 0003 0000 0073 1200 0000 8700  .........s......
-00001190: 6601 6401 6402 8408 7c01 4400 8301 5300  f.d.d...|.D...S.
-000011a0: 2903 7a8b 0a09 0946 6f72 2061 2073 6572  ).z....For a ser
-000011b0: 6965 7320 6f66 2070 6169 7273 206f 6620  ies of pairs of 
-000011c0: 706f 696e 7473 2c20 6561 6368 2077 6974  points, each wit
-000011d0: 6820 7468 7265 6520 636f 6f72 6469 6e61  h three coordina
-000011e0: 7465 7320 616e 6420 6120 6672 6571 7565  tes and a freque
-000011f0: 6e63 792c 2072 6574 7572 6e20 6120 6c69  ncy, return a li
-00001200: 7374 206f 6620 7468 6520 636f 7272 6573  st of the corres
-00001210: 706f 6e64 696e 6720 446f 7450 6169 724d  ponding DotPairM
-00001220: 6561 7375 7265 6d65 6e74 732e 0a09 0963  easurements....c
-00001230: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001240: 0500 0000 1300 0000 7316 0000 0067 007c  ........s....g.|
-00001250: 005d 0e7d 0188 00a0 007c 01a1 0191 0271  .].}.....|.....q
-00001260: 0453 0072 1500 0000 2901 7243 0000 0029  .S.r....).rC...)
-00001270: 0272 3a00 0000 7240 0000 0072 1300 0000  .r:...r@...r....
-00001280: 7215 0000 0072 1600 0000 723c 0000 0073  r....r....r<...s
-00001290: 0000 0073 0400 0000 0602 02ff 7a4a 4f73  ...s........zJOs
-000012a0: 6369 6c6c 6174 696e 6744 6970 6f6c 6541  cillatingDipoleA
-000012b0: 7272 616e 6765 6d65 6e74 2e67 6574 5f64  rrangement.get_d
-000012c0: 6f74 5f70 6169 725f 6d65 6173 7572 656d  ot_pair_measurem
-000012d0: 656e 7473 2e3c 6c6f 6361 6c73 3e2e 3c6c  ents.<locals>.<l
-000012e0: 6973 7463 6f6d 703e 7215 0000 0029 0272  istcomp>r....).r
-000012f0: 1400 0000 7247 0000 0072 1500 0000 7213  ....rG...r....r.
-00001300: 0000 0072 1600 0000 da19 6765 745f 646f  ...r......get_do
-00001310: 745f 7061 6972 5f6d 6561 7375 7265 6d65  t_pair_measureme
-00001320: 6e74 736d 0000 0073 0600 0000 0006 0a02  ntsm...s........
-00001330: 02fe 7a36 4f73 6369 6c6c 6174 696e 6744  ..z6OscillatingD
-00001340: 6970 6f6c 6541 7272 616e 6765 6d65 6e74  ipoleArrangement
-00001350: 2e67 6574 5f64 6f74 5f70 6169 725f 6d65  .get_dot_pair_me
-00001360: 6173 7572 656d 656e 7473 2904 7237 0000  asurements).r7..
-00001370: 00da 0b6c 6f77 5f70 6572 6365 6e74 da0c  ...low_percent..
-00001380: 6869 6768 5f70 6572 6365 6e74 7210 0000  high_percentr...
-00001390: 0063 0400 0000 0000 0000 0000 0000 0400  .c..............
-000013a0: 0000 0700 0000 0300 0000 7358 0000 0074  ..........sX...t
-000013b0: 00a0 017c 0164 0119 00a1 0189 017c 0164  ...|.d.......|.d
-000013c0: 0219 0089 0074 027c 0274 0387 0087 0166  .....t.|.t.....f
-000013d0: 0264 0364 0484 087c 006a 0444 0083 0183  .d.d...|.j.D....
-000013e0: 0114 007c 0374 0387 0087 0166 0264 0564  ...|.t.....f.d.d
-000013f0: 0484 087c 006a 0444 0083 0183 0114 0088  ...|.j.D........
-00001400: 0188 0083 0453 0029 064e 7201 0000 0072  .....S.).Nr....r
-00001410: 2400 0000 6301 0000 0000 0000 0000 0000  $...c...........
-00001420: 0002 0000 0006 0000 0013 0000 0073 1800  .............s..
-00001430: 0000 6700 7c00 5d10 7d01 7c01 a000 8801  ..g.|.].}.|.....
-00001440: 8800 a102 9102 7104 5300 7215 0000 0072  ......q.S.r....r
-00001450: 3800 0000 7239 0000 0072 3b00 0000 7215  8...r9...r;...r.
-00001460: 0000 0072 1600 0000 723c 0000 007e 0000  ...r....r<...~..
-00001470: 0072 3d00 0000 7a52 4f73 6369 6c6c 6174  .r=...zROscillat
-00001480: 696e 6744 6970 6f6c 6541 7272 616e 6765  ingDipoleArrange
-00001490: 6d65 6e74 2e67 6574 5f70 6572 6365 6e74  ment.get_percent
-000014a0: 5f72 616e 6765 5f64 6f74 5f6d 6561 7375  _range_dot_measu
-000014b0: 7265 6d65 6e74 2e3c 6c6f 6361 6c73 3e2e  rement.<locals>.
-000014c0: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
-000014d0: 0000 0000 0000 0002 0000 0006 0000 0013  ................
-000014e0: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
-000014f0: 7c01 a000 8801 8800 a102 9102 7104 5300  |...........q.S.
-00001500: 7215 0000 0072 3800 0000 7239 0000 0072  r....r8...r9...r
-00001510: 3b00 0000 7215 0000 0072 1600 0000 723c  ;...r....r....r<
-00001520: 0000 007f 0000 0072 3d00 0000 2905 7211  .......r=...).r.
-00001530: 0000 0072 1200 0000 7206 0000 0072 3e00  ...r....r....r>.
-00001540: 0000 7235 0000 0029 0472 1400 0000 7237  ..r5...).r....r7
-00001550: 0000 0072 4900 0000 724a 0000 0072 1500  ...rI...rJ...r..
-00001560: 0000 723b 0000 0072 1600 0000 da21 6765  ..r;...r.....!ge
-00001570: 745f 7065 7263 656e 745f 7261 6e67 655f  t_percent_range_
-00001580: 646f 745f 6d65 6173 7572 656d 656e 7478  dot_measurementx
-00001590: 0000 0073 1000 0000 0003 0e01 0801 0201  ...s............
-000015a0: 1c01 1c01 0201 02fc 7a3e 4f73 6369 6c6c  ........z>Oscill
-000015b0: 6174 696e 6744 6970 6f6c 6541 7272 616e  atingDipoleArran
-000015c0: 6765 6d65 6e74 2e67 6574 5f70 6572 6365  gement.get_perce
-000015d0: 6e74 5f72 616e 6765 5f64 6f74 5f6d 6561  nt_range_dot_mea
-000015e0: 7375 7265 6d65 6e74 2904 7244 0000 0072  surement).rD...r
-000015f0: 4900 0000 724a 0000 0072 1000 0000 6304  I...rJ...r....c.
-00001600: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-00001610: 0000 0003 0000 0073 1600 0000 8700 8701  .......s........
-00001620: 8702 6603 6401 6402 8408 7c01 4400 8301  ..f.d.d...|.D...
-00001630: 5300 2903 fac4 0a09 0946 6f72 2061 2073  S.)......For a s
-00001640: 6572 6965 7320 6f66 2070 6169 7273 206f  eries of pairs o
-00001650: 6620 706f 696e 7473 2c20 6561 6368 2077  f points, each w
-00001660: 6974 6820 7468 7265 6520 636f 6f72 6469  ith three coordi
-00001670: 6e61 7465 7320 616e 6420 6120 6672 6571  nates and a freq
-00001680: 7565 6e63 792c 2061 6e64 2061 6c73 6f20  uency, and also 
-00001690: 6120 6c6f 7765 7220 6572 726f 7220 7261  a lower error ra
-000016a0: 6e67 6520 616e 6420 7570 7065 7220 6572  nge and upper er
-000016b0: 726f 7220 7261 6e67 652c 2072 6574 7572  ror range, retur
-000016c0: 6e20 6120 6c69 7374 206f 6620 7468 6520  n a list of the 
-000016d0: 636f 7272 6573 706f 6e64 696e 6720 446f  corresponding Do
-000016e0: 7450 6169 7252 616e 6765 4d65 6173 7572  tPairRangeMeasur
-000016f0: 656d 656e 7473 2e0a 0909 6301 0000 0000  ements....c.....
-00001700: 0000 0000 0000 0002 0000 0007 0000 0013  ................
-00001710: 0000 0073 1a00 0000 6700 7c00 5d12 7d01  ...s....g.|.].}.
-00001720: 8802 a000 7c01 8801 8800 a103 9102 7104  ....|.........q.
-00001730: 5300 7215 0000 0029 0172 4b00 0000 7245  S.r....).rK...rE
-00001740: 0000 00a9 0372 4a00 0000 7249 0000 0072  .....rJ...rI...r
-00001750: 1400 0000 7215 0000 0072 1600 0000 723c  ....r....r....r<
-00001760: 0000 008a 0000 0073 0400 0000 0602 02ff  .......s........
-00001770: 7a53 4f73 6369 6c6c 6174 696e 6744 6970  zSOscillatingDip
-00001780: 6f6c 6541 7272 616e 6765 6d65 6e74 2e67  oleArrangement.g
-00001790: 6574 5f70 6572 6365 6e74 5f72 616e 6765  et_percent_range
-000017a0: 5f64 6f74 5f6d 6561 7375 7265 6d65 6e74  _dot_measurement
-000017b0: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
-000017c0: 636f 6d70 3e72 1500 0000 2904 7214 0000  comp>r....).r...
-000017d0: 0072 4400 0000 7249 0000 0072 4a00 0000  .rD...rI...rJ...
-000017e0: 7215 0000 0072 4d00 0000 7216 0000 00da  r....rM...r.....
-000017f0: 2267 6574 5f70 6572 6365 6e74 5f72 616e  "get_percent_ran
-00001800: 6765 5f64 6f74 5f6d 6561 7375 7265 6d65  ge_dot_measureme
-00001810: 6e74 7384 0000 0073 0600 0000 0006 0e02  nts....s........
-00001820: 02fe 7a3f 4f73 6369 6c6c 6174 696e 6744  ..z?OscillatingD
-00001830: 6970 6f6c 6541 7272 616e 6765 6d65 6e74  ipoleArrangement
-00001840: 2e67 6574 5f70 6572 6365 6e74 5f72 616e  .get_percent_ran
-00001850: 6765 5f64 6f74 5f6d 6561 7375 7265 6d65  ge_dot_measureme
-00001860: 6e74 7329 04da 0a70 6169 725f 696e 7075  nts)...pair_inpu
-00001870: 7472 4900 0000 724a 0000 0072 1000 0000  trI...rJ...r....
-00001880: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
-00001890: 0007 0000 0003 0000 0073 6c00 0000 7400  .........sl...t.
-000018a0: a001 7c01 6401 1900 a101 8901 7400 a001  ..|.d.......t...
-000018b0: 7c01 6402 1900 a101 8902 7c01 6403 1900  |.d.......|.d...
-000018c0: 8900 7402 7c02 7403 8700 8701 8702 6603  ..t.|.t.......f.
-000018d0: 6404 6405 8408 7c00 6a04 4400 8301 8301  d.d...|.j.D.....
-000018e0: 1400 7c03 7403 8700 8701 8702 6603 6406  ..|.t.......f.d.
-000018f0: 6405 8408 7c00 6a04 4400 8301 8301 1400  d...|.j.D.......
-00001900: 8801 8802 8800 8305 5300 2907 4e72 0100  ........S.).Nr..
-00001910: 0000 7224 0000 0072 1a00 0000 6301 0000  ..r$...r....c...
-00001920: 0000 0000 0000 0000 0002 0000 0007 0000  ................
-00001930: 0013 0000 0073 1a00 0000 6700 7c00 5d12  .....s....g.|.].
-00001940: 7d01 7c01 a000 8801 8802 8800 a103 9102  }.|.............
-00001950: 7104 5300 7215 0000 0072 4100 0000 7239  q.S.r....rA...r9
-00001960: 0000 0072 4200 0000 7215 0000 0072 1600  ...rB...r....r..
-00001970: 0000 723c 0000 0097 0000 0072 3d00 0000  ..r<.......r=...
-00001980: 7a57 4f73 6369 6c6c 6174 696e 6744 6970  zWOscillatingDip
-00001990: 6f6c 6541 7272 616e 6765 6d65 6e74 2e67  oleArrangement.g
-000019a0: 6574 5f70 6572 6365 6e74 5f72 616e 6765  et_percent_range
-000019b0: 5f64 6f74 5f70 6169 725f 6d65 6173 7572  _dot_pair_measur
-000019c0: 656d 656e 742e 3c6c 6f63 616c 733e 2e3c  ement.<locals>.<
-000019d0: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
-000019e0: 0000 0000 0000 0200 0000 0700 0000 1300  ................
-000019f0: 0000 731a 0000 0067 007c 005d 127d 017c  ..s....g.|.].}.|
-00001a00: 01a0 0088 0188 0288 00a1 0391 0271 0453  .............q.S
-00001a10: 0072 1500 0000 7241 0000 0072 3900 0000  .r....rA...r9...
-00001a20: 7242 0000 0072 1500 0000 7216 0000 0072  rB...r....r....r
-00001a30: 3c00 0000 9900 0000 723d 0000 0029 0572  <.......r=...).r
-00001a40: 1100 0000 7212 0000 0072 0800 0000 723e  ....r....r....r>
-00001a50: 0000 0072 3500 0000 2904 7214 0000 0072  ...r5...).r....r
-00001a60: 4f00 0000 7249 0000 0072 4a00 0000 7215  O...rI...rJ...r.
-00001a70: 0000 0072 4200 0000 7216 0000 00da 2667  ...rB...r.....&g
-00001a80: 6574 5f70 6572 6365 6e74 5f72 616e 6765  et_percent_range
-00001a90: 5f64 6f74 5f70 6169 725f 6d65 6173 7572  _dot_pair_measur
-00001aa0: 656d 656e 748f 0000 0073 1c00 0000 0003  ement....s......
-00001ab0: 0e01 0e01 0801 0201 0201 1aff 0202 0201  ................
-00001ac0: 1aff 0202 0201 0201 02f9 7a43 4f73 6369  ..........zCOsci
-00001ad0: 6c6c 6174 696e 6744 6970 6f6c 6541 7272  llatingDipoleArr
-00001ae0: 616e 6765 6d65 6e74 2e67 6574 5f70 6572  angement.get_per
-00001af0: 6365 6e74 5f72 616e 6765 5f64 6f74 5f70  cent_range_dot_p
-00001b00: 6169 725f 6d65 6173 7572 656d 656e 7429  air_measurement)
-00001b10: 04da 0b70 6169 725f 696e 7075 7473 7249  ...pair_inputsrI
-00001b20: 0000 0072 4a00 0000 7210 0000 0063 0400  ...rJ...r....c..
-00001b30: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-00001b40: 0000 0300 0000 7316 0000 0087 0087 0187  ......s.........
-00001b50: 0266 0364 0164 0284 087c 0144 0083 0153  .f.d.d...|.D...S
-00001b60: 0029 0372 4c00 0000 6301 0000 0000 0000  .).rL...c.......
-00001b70: 0000 0000 0002 0000 0007 0000 0013 0000  ................
-00001b80: 0073 1a00 0000 6700 7c00 5d12 7d01 8802  .s....g.|.].}...
-00001b90: a000 7c01 8801 8800 a103 9102 7104 5300  ..|.........q.S.
-00001ba0: 7215 0000 0029 0172 5000 0000 2902 723a  r....).rP...).r:
-00001bb0: 0000 0072 4f00 0000 724d 0000 0072 1500  ...rO...rM...r..
-00001bc0: 0000 7216 0000 0072 3c00 0000 a800 0000  ..r....r<.......
-00001bd0: 7308 0000 0006 0402 fd04 0106 ff7a 584f  s............zXO
-00001be0: 7363 696c 6c61 7469 6e67 4469 706f 6c65  scillatingDipole
-00001bf0: 4172 7261 6e67 656d 656e 742e 6765 745f  Arrangement.get_
-00001c00: 7065 7263 656e 745f 7261 6e67 655f 646f  percent_range_do
-00001c10: 745f 7061 6972 5f6d 6561 7375 7265 6d65  t_pair_measureme
-00001c20: 6e74 732e 3c6c 6f63 616c 733e 2e3c 6c69  nts.<locals>.<li
-00001c30: 7374 636f 6d70 3e72 1500 0000 2904 7214  stcomp>r....).r.
-00001c40: 0000 0072 5100 0000 7249 0000 0072 4a00  ...rQ...rI...rJ.
-00001c50: 0000 7215 0000 0072 4d00 0000 7216 0000  ..r....rM...r...
-00001c60: 00da 2767 6574 5f70 6572 6365 6e74 5f72  ..'get_percent_r
-00001c70: 616e 6765 5f64 6f74 5f70 6169 725f 6d65  ange_dot_pair_me
-00001c80: 6173 7572 656d 656e 7473 9f00 0000 7306  asurements....s.
-00001c90: 0000 0000 090e 0402 fc7a 444f 7363 696c  .........zDOscil
-00001ca0: 6c61 7469 6e67 4469 706f 6c65 4172 7261  latingDipoleArra
-00001cb0: 6e67 656d 656e 742e 6765 745f 7065 7263  ngement.get_perc
-00001cc0: 656e 745f 7261 6e67 655f 646f 745f 7061  ent_range_dot_pa
-00001cd0: 6972 5f6d 6561 7375 7265 6d65 6e74 7372  ir_measurementsr
-00001ce0: 0f00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00001cf0: 0001 0000 0004 0000 0043 0000 0073 1600  .........C...s..
-00001d00: 0000 7400 a001 6401 6402 8400 7c00 6a02  ..t...d.d...|.j.
-00001d10: 4400 8301 a101 5300 2903 7a62 0a09 0952  D.....S.).zb...R
-00001d20: 6574 7572 6e73 2061 206e 756d 7079 2061  eturns a numpy a
-00001d30: 7272 6179 2077 6974 6820 7468 6520 6361  rray with the ca
-00001d40: 6e6f 6e69 6361 6c20 7265 7072 6573 656e  nonical represen
-00001d50: 7461 7469 6f6e 206f 6620 6561 6368 2064  tation of each d
-00001d60: 6970 6f6c 6520 696e 2061 206e 7837 206e  ipole in a nx7 n
-00001d70: 756d 7079 2061 7272 6179 2e0a 0909 6301  umpy array....c.
-00001d80: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001d90: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
-00001da0: 5d0c 7d01 7c01 a000 a100 9102 7104 5300  ].}.|.......q.S.
-00001db0: 7215 0000 0029 0172 2b00 0000 7239 0000  r....).r+...r9..
-00001dc0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00001dd0: 723c 0000 00b3 0000 0072 3d00 0000 7a3f  r<.......r=...z?
-00001de0: 4f73 6369 6c6c 6174 696e 6744 6970 6f6c  OscillatingDipol
-00001df0: 6541 7272 616e 6765 6d65 6e74 2e74 6f5f  eArrangement.to_
-00001e00: 6e75 6d70 795f 6172 7261 792e 3c6c 6f63  numpy_array.<loc
-00001e10: 616c 733e 2e3c 6c69 7374 636f 6d70 3e29  als>.<listcomp>)
-00001e20: 0372 1100 0000 7212 0000 0072 3500 0000  .r....r....r5...
-00001e30: 7213 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-00001e40: 1600 0000 da0e 746f 5f6e 756d 7079 5f61  ......to_numpy_a
-00001e50: 7272 6179 af00 0000 7302 0000 0000 047a  rray....s......z
-00001e60: 2b4f 7363 696c 6c61 7469 6e67 4469 706f  +OscillatingDipo
-00001e70: 6c65 4172 7261 6e67 656d 656e 742e 746f  leArrangement.to
-00001e80: 5f6e 756d 7079 5f61 7272 6179 4e29 1a72  _numpy_arrayN).r
-00001e90: 2c00 0000 722d 0000 0072 2e00 0000 722f  ,...r-...r....r/
-00001ea0: 0000 0072 0300 0000 720b 0000 0072 3600  ...r....r....r6.
-00001eb0: 0000 7209 0000 0072 0500 0000 723f 0000  ..r....r....r?..
-00001ec0: 0072 0a00 0000 7207 0000 0072 4300 0000  .r....r....rC...
-00001ed0: 7204 0000 0072 4600 0000 7248 0000 0072  r....rF...rH...r
-00001ee0: 3200 0000 7206 0000 0072 4b00 0000 724e  2...r....rK...rN
-00001ef0: 0000 0072 0800 0000 7250 0000 0072 5200  ...r....rP...rR.
-00001f00: 0000 7211 0000 0072 3000 0000 7253 0000  ..r....r0...rS..
-00001f10: 0072 1500 0000 7215 0000 0072 1500 0000  .r....r....r....
-00001f20: 7216 0000 0072 3300 0000 4500 0000 7336  r....r3...E...s6
-00001f30: 0000 0008 0104 0812 0310 0802 0102 fe0c  ................
-00001f40: 0e06 0106 fe0c 0906 0106 fe0c 0c06 0102  ................
-00001f50: fe0c 0d0a 0106 fe0c 0c06 0102 fe0c 1206  ................
-00001f60: 0102 0102 0106 fb0c 1072 3300 0000 2912  .........r3...).
-00001f70: da0b 6461 7461 636c 6173 7365 7372 0200  ..dataclassesr..
-00001f80: 0000 7211 0000 00da 0c6e 756d 7079 2e74  ..r......numpy.t
-00001f90: 7970 696e 67da 0674 7970 696e 6772 0300  yping..typingr..
-00001fa0: 0000 7204 0000 00da 1c70 646d 652e 6d65  ..r......pdme.me
-00001fb0: 6173 7572 656d 656e 742e 646f 745f 6d65  asurement.dot_me
-00001fc0: 6173 7572 6572 0500 0000 7206 0000 00da  asurer....r.....
-00001fd0: 2170 646d 652e 6d65 6173 7572 656d 656e  !pdme.measuremen
-00001fe0: 742e 646f 745f 7061 6972 5f6d 6561 7375  t.dot_pair_measu
-00001ff0: 7265 7207 0000 0072 0800 0000 da1c 7064  rer....r......pd
-00002000: 6d65 2e6d 6561 7375 7265 6d65 6e74 2e69  me.measurement.i
-00002010: 6e70 7574 5f74 7970 6573 7209 0000 0072  nput_typesr....r
-00002020: 0a00 0000 720b 0000 0072 3300 0000 7215  ....r....r3...r.
-00002030: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00002040: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00002050: 7312 0000 000c 0108 0108 0110 0110 0110  s...............
-00002060: 0410 0302 0110 37                        ......7
+00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6402 6c0d  m.Z.m.Z...d.d.l.
+00000080: 5a0e 6400 6406 6c0f 6d10 5a10 6d11 5a11  Z.d.d.l.m.Z.m.Z.
+00000090: 0100 6501 4700 6407 6408 8400 6408 8302  ..e.G.d.d...d...
+000000a0: 8301 5a12 4700 6409 640a 8400 640a 8302  ..Z.G.d.d...d...
+000000b0: 5a13 6402 5300 290b e900 0000 0029 01da  Z.d.S.)......)..
+000000c0: 0964 6174 6163 6c61 7373 4e29 02da 0853  .dataclassN)...S
+000000d0: 6571 7565 6e63 65da 044c 6973 7429 02da  equence..List)..
+000000e0: 0e44 6f74 4d65 6173 7572 656d 656e 74da  .DotMeasurement.
+000000f0: 1344 6f74 5261 6e67 654d 6561 7375 7265  .DotRangeMeasure
+00000100: 6d65 6e74 2902 da12 446f 7450 6169 724d  ment)...DotPairM
+00000110: 6561 7375 7265 6d65 6e74 da17 446f 7450  easurement..DotP
+00000120: 6169 7252 616e 6765 4d65 6173 7572 656d  airRangeMeasurem
+00000130: 656e 7429 02da 0844 6f74 496e 7075 74da  ent)...DotInput.
+00000140: 0c44 6f74 5061 6972 496e 7075 7463 0000  .DotPairInputc..
+00000150: 0000 0000 0000 0000 0000 0000 0000 0500  ................
+00000160: 0000 4000 0000 73da 0000 0065 005a 0164  ..@...s....e.Z.d
+00000170: 005a 0255 0064 015a 0365 046a 0565 0664  .Z.U.d.Z.e.j.e.d
+00000180: 023c 0065 046a 0565 0664 033c 0065 0765  .<.e.j.e.d.<.e.e
+00000190: 0664 043c 0064 0564 069c 0164 0764 0884  .d.<.d.d...d.d..
+000001a0: 045a 0865 046a 0565 0764 099c 0264 0a64  .Z.e.j.e.d...d.d
+000001b0: 0b84 045a 0965 046a 0565 046a 0564 099c  ...Z.e.j.e.j.d..
+000001c0: 0264 0c64 0d84 045a 0a65 0765 0764 0e9c  .d.d...Z.e.e.d..
+000001d0: 0264 0f64 1084 045a 0b65 046a 0565 0765  .d.d...Z.e.j.e.e
+000001e0: 0764 119c 0364 1264 1384 045a 0c65 046a  .d...d.d...Z.e.j
+000001f0: 0565 046a 0565 0765 0764 149c 0464 1564  .e.j.e.e.d...d.d
+00000200: 1684 045a 0d65 046a 0565 0765 0764 119c  ...Z.e.j.e.e.d..
+00000210: 0364 1764 1884 045a 0e65 046a 0565 046a  .d.d...Z.e.j.e.j
+00000220: 0565 0765 0764 149c 0464 1964 1a84 045a  .e.e.d...d.d...Z
+00000230: 0f65 046a 0564 069c 0164 1b64 1c84 045a  .e.j.d...d.d...Z
+00000240: 1064 0553 0029 1dda 114f 7363 696c 6c61  .d.S.)...Oscilla
+00000250: 7469 6e67 4469 706f 6c65 6107 0100 000a  tingDipolea.....
+00000260: 0952 6570 7265 7365 6e74 6174 696f 6e20  .Representation 
+00000270: 6f66 2061 6e20 6f73 6369 6c6c 6174 696e  of an oscillatin
+00000280: 6720 6469 706f 6c65 2c20 6569 7468 6572  g dipole, either
+00000290: 206b 6e6f 776e 206f 7220 6775 6573 7365   known or guesse
+000002a0: 642e 0a0a 0950 6172 616d 6574 6572 730a  d....Parameters.
+000002b0: 092d 2d2d 2d2d 2d2d 2d2d 2d0a 0970 203a  .----------..p :
+000002c0: 206e 756d 7079 2e6e 6461 7272 6179 0a09   numpy.ndarray..
+000002d0: 5468 6520 6f73 6369 6c6c 6174 696e 6720  The oscillating 
+000002e0: 6469 706f 6c65 206d 6f6d 656e 742c 2077  dipole moment, w
+000002f0: 6974 6820 6f76 6572 616c 6c20 7369 676e  ith overall sign
+00000300: 2061 7262 6974 7261 7279 2e0a 0a09 7320   arbitrary....s 
+00000310: 3a20 6e75 6d70 792e 6e64 6172 7261 790a  : numpy.ndarray.
+00000320: 0954 6865 2070 6f73 6974 696f 6e20 6f66  .The position of
+00000330: 2074 6865 2064 6970 6f6c 652e 0a0a 0977   the dipole....w
+00000340: 203a 2066 6c6f 6174 0a09 5468 6520 6f73   : float..The os
+00000350: 6369 6c6c 6174 696f 6e20 6672 6571 7565  cillation freque
+00000360: 6e63 792e 0a09 da01 70da 0173 da01 774e  ncy.....p..s..wN
+00000370: a901 da06 7265 7475 726e 6301 0000 0000  ....returnc.....
+00000380: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00000390: 0000 0073 2000 0000 7400 a001 7c00 6a02  ...s ...t...|.j.
+000003a0: a101 7c00 5f02 7400 a001 7c00 6a03 a101  ..|._.t...|.j...
+000003b0: 7c00 5f03 6401 5300 2902 7a2a 0a09 0943  |._.d.S.).z*...C
+000003c0: 6f65 7263 6520 7468 6520 696e 7075 7473  oerce the inputs
+000003d0: 2069 6e74 6f20 6e75 6d70 7920 6172 7261   into numpy arra
+000003e0: 7973 2e0a 0909 4e29 04da 056e 756d 7079  ys....N)...numpy
+000003f0: da05 6172 7261 7972 0c00 0000 720d 0000  ..arrayr....r...
+00000400: 00a9 01da 0473 656c 66a9 0072 1500 0000  .....self..r....
+00000410: fa5d 2f68 6f6d 652f 6a65 6e6b 696e 732f  .]/home/jenkins/
+00000420: 6167 656e 742f 776f 726b 7370 6163 652f  agent/workspace/
+00000430: 6769 7465 612d 7068 7973 6963 735f 7064  gitea-physics_pd
+00000440: 6d65 5f31 2e31 2e30 2f70 646d 652f 6d65  me_1.1.0/pdme/me
+00000450: 6173 7572 656d 656e 742f 6f73 6369 6c6c  asurement/oscill
+00000460: 6174 696e 675f 6469 706f 6c65 2e70 79da  ating_dipole.py.
+00000470: 0d5f 5f70 6f73 745f 696e 6974 5f5f 2300  .__post_init__#.
+00000480: 0000 7304 0000 0000 040e 017a 1f4f 7363  ..s........z.Osc
+00000490: 696c 6c61 7469 6e67 4469 706f 6c65 2e5f  illatingDipole._
+000004a0: 5f70 6f73 745f 696e 6974 5f5f 2902 da01  _post_init__)...
+000004b0: 7272 1000 0000 6302 0000 0000 0000 0000  rr....c.........
+000004c0: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
+000004d0: 1400 0000 7400 6a01 a002 7c00 6a03 7c00  ....t.j...|.j.|.
+000004e0: 6a04 7c01 a103 5300 2901 7a42 0a09 0952  j.|...S.).zB...R
+000004f0: 6574 7572 6e73 2074 6865 2065 6c65 6374  eturns the elect
+00000500: 7269 6320 706f 7465 6e74 6961 6c20 6f66  ric potential of
+00000510: 2074 6869 7320 6469 706f 6c65 2061 7420   this dipole at 
+00000520: 706f 7369 7469 6f6e 2072 2e0a 0909 2905  position r....).
+00000530: da04 7064 6d65 da0c 6361 6c63 756c 6174  ..pdme..calculat
+00000540: 696f 6e73 da12 656c 6563 7472 6963 5f70  ions..electric_p
+00000550: 6f74 656e 7469 616c 720c 0000 0072 0d00  otentialr....r..
+00000560: 0000 a902 7214 0000 0072 1800 0000 7215  ....r....r....r.
+00000570: 0000 0072 1500 0000 7216 0000 00da 195f  ...r....r......_
+00000580: 616c 7068 615f 656c 6563 7472 6963 5f70  alpha_electric_p
+00000590: 6f74 656e 7469 616c 2a00 0000 7302 0000  otential*...s...
+000005a0: 0000 047a 2b4f 7363 696c 6c61 7469 6e67  ...z+Oscillating
+000005b0: 4469 706f 6c65 2e5f 616c 7068 615f 656c  Dipole._alpha_el
+000005c0: 6563 7472 6963 5f70 6f74 656e 7469 616c  ectric_potential
+000005d0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000005e0: 0005 0000 0043 0000 0073 1400 0000 7400  .....C...s....t.
+000005f0: 6a01 a002 7c00 6a03 7c00 6a04 7c01 a103  j...|.j.|.j.|...
+00000600: 5300 2901 7a3e 0a09 0952 6574 7572 6e73  S.).z>...Returns
+00000610: 2074 6865 2065 6c65 6374 7269 6320 6669   the electric fi
+00000620: 656c 6420 6f66 2074 6869 7320 6469 706f  eld of this dipo
+00000630: 6c65 2061 7420 706f 7369 7469 6f6e 2072  le at position r
+00000640: 2e0a 0909 2905 7219 0000 0072 1a00 0000  ....).r....r....
+00000650: da0e 656c 6563 7472 6963 5f66 6965 6c64  ..electric_field
+00000660: 720c 0000 0072 0d00 0000 721c 0000 0072  r....r....r....r
+00000670: 1500 0000 7215 0000 0072 1600 0000 da15  ....r....r......
+00000680: 5f61 6c70 6861 5f65 6c65 6374 7269 635f  _alpha_electric_
+00000690: 6669 656c 6430 0000 0073 0200 0000 0004  field0...s......
+000006a0: 7a27 4f73 6369 6c6c 6174 696e 6744 6970  z'OscillatingDip
+000006b0: 6f6c 652e 5f61 6c70 6861 5f65 6c65 6374  ole._alpha_elect
+000006c0: 7269 635f 6669 656c 6429 02da 0166 7210  ric_field)...fr.
+000006d0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+000006e0: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+000006f0: 0074 006a 01a0 027c 017c 006a 03a1 0253  .t.j...|.|.j...S
+00000700: 00a9 014e 2904 7219 0000 0072 1a00 0000  ...N).r....r....
+00000710: da0e 7465 6c65 6772 6170 685f 6265 7461  ..telegraph_beta
+00000720: 720e 0000 0029 0272 1400 0000 7220 0000  r....).r....r ..
+00000730: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000740: da02 5f62 3600 0000 7302 0000 0000 017a  .._b6...s......z
+00000750: 144f 7363 696c 6c61 7469 6e67 4469 706f  .OscillatingDipo
+00000760: 6c65 2e5f 6229 0372 1800 0000 7220 0000  le._b).r....r ..
+00000770: 0072 1000 0000 6303 0000 0000 0000 0000  .r....c.........
+00000780: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+00000790: 1800 0000 7c00 a000 7c01 a101 6401 1300  ....|...|...d...
+000007a0: 7c00 a001 7c02 a101 1400 5300 2902 fae2  |...|.....S.)...
+000007b0: 0a09 0952 6574 7572 6e73 2074 6865 206e  ...Returns the n
+000007c0: 6f69 7365 2070 6f74 656e 7469 616c 2061  oise potential a
+000007d0: 7420 6120 706f 696e 7420 722c 2061 7420  t a point r, at 
+000007e0: 736f 6d65 2066 7265 7175 656e 6379 2066  some frequency f
+000007f0: 2e0a 0a09 0953 7065 6369 6669 6361 6c6c  .....Specificall
+00000800: 7920 666f 7220 656c 6563 7472 6963 2070  y for electric p
+00000810: 6f74 656e 7469 616c 210a 0a09 0950 6172  otential!....Par
+00000820: 616d 6574 6572 730a 0909 2d2d 2d2d 2d2d  ameters...------
+00000830: 2d2d 2d2d 0a09 0972 203a 206e 756d 7079  ----...r : numpy
+00000840: 2e6e 6461 7272 6179 0a09 0954 6865 2070  .ndarray...The p
+00000850: 6f73 6974 696f 6e20 6f66 2074 6865 2064  osition of the d
+00000860: 6f74 2e0a 0a09 0966 203a 2066 6c6f 6174  ot.....f : float
+00000870: 0a09 0954 6865 2064 6f74 2066 7265 7175  ...The dot frequ
+00000880: 656e 6379 2074 6f20 7361 6d70 6c65 2e0a  ency to sample..
+00000890: 0909 e902 0000 00a9 0272 1d00 0000 7223  .........r....r#
+000008a0: 0000 00a9 0372 1400 0000 7218 0000 0072  .....r....r....r
+000008b0: 2000 0000 7215 0000 0072 1500 0000 7216   ...r....r....r.
+000008c0: 0000 00da 2073 5f65 6c65 6374 7269 635f  .... s_electric_
+000008d0: 706f 7465 6e74 6961 6c5f 6174 5f70 6f73  potential_at_pos
+000008e0: 6974 696f 6e39 0000 0073 0200 0000 000e  ition9...s......
+000008f0: 7a32 4f73 6369 6c6c 6174 696e 6744 6970  z2OscillatingDip
+00000900: 6f6c 652e 735f 656c 6563 7472 6963 5f70  ole.s_electric_p
+00000910: 6f74 656e 7469 616c 5f61 745f 706f 7369  otential_at_posi
+00000920: 7469 6f6e 2904 da02 7231 da02 7232 7220  tion)...r1..r2r 
+00000930: 0000 0072 1000 0000 6304 0000 0000 0000  ...r....c.......
+00000940: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
+00000950: 0073 1e00 0000 7c00 a000 7c01 a101 7c00  .s....|...|...|.
+00000960: a000 7c02 a101 1400 7c00 a001 7c03 a101  ..|.....|...|...
+00000970: 1400 5300 2901 fa66 0a09 0954 6869 7320  ..S.)..f...This 
+00000980: 6973 2073 7065 6369 6669 6361 6c6c 7920  is specifically 
+00000990: 7468 6520 616e 616c 7974 6963 2063 7073  the analytic cps
+000009a0: 6420 666f 7220 656c 6563 7472 6963 2070  d for electric p
+000009b0: 6f74 656e 7469 616c 206e 6f69 7365 2e0a  otential noise..
+000009c0: 0909 5468 6973 2073 686f 756c 6420 6265  ..This should be
+000009d0: 2064 6570 7265 6361 7465 640a 0909 7226   deprecated...r&
+000009e0: 0000 00a9 0472 1400 0000 7229 0000 0072  .....r....r)...r
+000009f0: 2a00 0000 7220 0000 0072 1500 0000 7215  *...r ...r....r.
+00000a00: 0000 0072 1600 0000 da21 735f 656c 6563  ...r.....!s_elec
+00000a10: 7472 6963 5f70 6f74 656e 7469 616c 5f66  tric_potential_f
+00000a20: 6f72 5f64 6f74 5f70 6169 7249 0000 0073  or_dot_pairI...s
+00000a30: 0c00 0000 0008 0801 08ff 0202 08fe 02ff  ................
+00000a40: 7a33 4f73 6369 6c6c 6174 696e 6744 6970  z3OscillatingDip
+00000a50: 6f6c 652e 735f 656c 6563 7472 6963 5f70  ole.s_electric_p
+00000a60: 6f74 656e 7469 616c 5f66 6f72 5f64 6f74  otential_for_dot
+00000a70: 5f70 6169 7263 0300 0000 0000 0000 0000  _pairc..........
+00000a80: 0000 0300 0000 0400 0000 4300 0000 731c  ..........C...s.
+00000a90: 0000 007c 00a0 007c 01a1 0164 0119 0064  ...|...|...d...d
+00000aa0: 0213 007c 00a0 017c 02a1 0114 0053 0029  ...|...|.....S.)
+00000ab0: 0372 2400 0000 7201 0000 0072 2500 0000  .r$...r....r%...
+00000ac0: a902 721f 0000 0072 2300 0000 7227 0000  ..r....r#...r'..
+00000ad0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000ae0: da1d 735f 656c 6563 7472 6963 5f66 6965  ..s_electric_fie
+00000af0: 6c64 785f 6174 5f70 6f73 6974 696f 6e56  ldx_at_positionV
+00000b00: 0000 0073 0200 0000 000e 7a2f 4f73 6369  ...s......z/Osci
+00000b10: 6c6c 6174 696e 6744 6970 6f6c 652e 735f  llatingDipole.s_
+00000b20: 656c 6563 7472 6963 5f66 6965 6c64 785f  electric_fieldx_
+00000b30: 6174 5f70 6f73 6974 696f 6e63 0400 0000  at_positionc....
+00000b40: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00000b50: 4300 0000 7326 0000 007c 00a0 007c 01a1  C...s&...|...|..
+00000b60: 0164 0119 007c 00a0 007c 02a1 0164 0119  .d...|...|...d..
+00000b70: 0014 007c 00a0 017c 03a1 0114 0053 0029  ...|...|.....S.)
+00000b80: 0272 2b00 0000 7201 0000 0072 2e00 0000  .r+...r....r....
+00000b90: 722c 0000 0072 1500 0000 7215 0000 0072  r,...r....r....r
+00000ba0: 1600 0000 da1e 735f 656c 6563 7472 6963  ......s_electric
+00000bb0: 5f66 6965 6c64 785f 666f 725f 646f 745f  _fieldx_for_dot_
+00000bc0: 7061 6972 6600 0000 730c 0000 0000 080c  pairf...s.......
+00000bd0: 010c ff02 0208 fe02 ff7a 304f 7363 696c  .........z0Oscil
+00000be0: 6c61 7469 6e67 4469 706f 6c65 2e73 5f65  latingDipole.s_e
+00000bf0: 6c65 6374 7269 635f 6669 656c 6478 5f66  lectric_fieldx_f
+00000c00: 6f72 5f64 6f74 5f70 6169 7263 0100 0000  or_dot_pairc....
+00000c10: 0000 0000 0000 0000 0100 0000 0700 0000  ................
+00000c20: 4300 0000 731e 0000 0074 00a0 017c 006a  C...s....t...|.j
+00000c30: 027c 006a 0374 00a0 047c 006a 0567 01a1  .|.j.t...|.j.g..
+00000c40: 0167 03a1 0153 0072 2100 0000 2906 7211  .g...S.r!...).r.
+00000c50: 0000 00da 0b63 6f6e 6361 7465 6e61 7465  .....concatenate
+00000c60: 720c 0000 0072 0d00 0000 7212 0000 0072  r....r....r....r
+00000c70: 0e00 0000 7213 0000 0072 1500 0000 7215  ....r....r....r.
+00000c80: 0000 0072 1600 0000 da0d 746f 5f66 6c61  ...r......to_fla
+00000c90: 745f 6172 7261 7973 0000 0073 0200 0000  t_arrays...s....
+00000ca0: 0001 7a1f 4f73 6369 6c6c 6174 696e 6744  ..z.OscillatingD
+00000cb0: 6970 6f6c 652e 746f 5f66 6c61 745f 6172  ipole.to_flat_ar
+00000cc0: 7261 7929 11da 085f 5f6e 616d 655f 5fda  ray)...__name__.
+00000cd0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000ce0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+00000cf0: 5f5f 7211 0000 00da 076e 6461 7272 6179  __r......ndarray
+00000d00: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+00000d10: 5fda 0566 6c6f 6174 7217 0000 0072 1d00  _..floatr....r..
+00000d20: 0000 721f 0000 0072 2300 0000 7228 0000  ..r....r#...r(..
+00000d30: 0072 2d00 0000 722f 0000 0072 3000 0000  .r-...r/...r0...
+00000d40: 7232 0000 0072 1500 0000 7215 0000 0072  r2...r....r....r
+00000d50: 1500 0000 7216 0000 0072 0b00 0000 0e00  ....r....r......
+00000d60: 0000 7322 0000 000a 0204 0f0a 010a 0108  ..s"............
+00000d70: 020e 0712 0614 0610 0314 110a 0102 fe0c  ................
+00000d80: 0d14 110a 0102 fe0c 0d72 0b00 0000 6300  .........r....c.
+00000d90: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+00000da0: 0000 0040 0000 0073 e200 0000 6500 5a01  ...@...s....e.Z.
+00000db0: 6400 5a02 6401 5a03 6504 6505 1900 6402  d.Z.d.Z.e.e...d.
+00000dc0: 9c01 6403 6404 8404 5a06 6507 6508 6405  ..d.d...Z.e.e.d.
+00000dd0: 9c02 6406 6407 8404 5a09 650a 650b 6408  ..d.d...Z.e.e.d.
+00000de0: 9c02 6409 640a 8404 5a0c 6504 6507 1900  ..d.d...Z.e.e...
+00000df0: 650d 6508 1900 640b 9c02 640c 640d 8404  e.e...d...d.d...
+00000e00: 5a0e 6504 650a 1900 650d 650b 1900 640e  Z.e.e...e.e...d.
+00000e10: 9c02 640f 6410 8404 5a0f 6507 6510 6510  ..d.d...Z.e.e.e.
+00000e20: 6511 6411 9c04 6412 6413 8404 5a12 6504  e.d...d.d...Z.e.
+00000e30: 6507 1900 6510 6510 650d 6511 1900 6414  e...e.e.e.e...d.
+00000e40: 9c04 6415 6416 8404 5a13 650a 6510 6510  ..d.d...Z.e.e.e.
+00000e50: 6514 6417 9c04 6418 6419 8404 5a15 6504  e.d...d.d...Z.e.
+00000e60: 650a 1900 6510 6510 650d 6514 1900 641a  e...e.e.e.e...d.
+00000e70: 9c04 641b 641c 8404 5a16 6517 6a18 641d  ..d.d...Z.e.j.d.
+00000e80: 9c01 641e 641f 8404 5a19 6420 5300 2921  ..d.d...Z.d S.)!
+00000e90: da1c 4f73 6369 6c6c 6174 696e 6744 6970  ..OscillatingDip
+00000ea0: 6f6c 6541 7272 616e 6765 6d65 6e74 7a9d  oleArrangementz.
+00000eb0: 0a09 4120 636f 6c6c 6563 7469 6f6e 206f  ..A collection o
+00000ec0: 6620 6f73 6369 6c6c 6174 696e 6720 6469  f oscillating di
+00000ed0: 706f 6c65 732c 2077 6869 6368 2077 6520  poles, which we 
+00000ee0: 6172 6520 696e 7465 7265 7374 6564 2069  are interested i
+00000ef0: 6e20 6265 696e 6720 6162 6c65 2074 6f20  n being able to 
+00000f00: 6368 6172 6163 7465 7269 7365 2e0a 0a09  characterise....
+00000f10: 5061 7261 6d65 7465 7273 0a09 2d2d 2d2d  Parameters..----
+00000f20: 2d2d 2d2d 0a09 6469 706f 6c65 7320 3a20  ----..dipoles : 
+00000f30: 5365 7175 656e 6365 5b4f 7363 696c 6c61  Sequence[Oscilla
+00000f40: 7469 6e67 4469 706f 6c65 5d0a 09a9 01da  tingDipole].....
+00000f50: 0764 6970 6f6c 6573 6302 0000 0000 0000  .dipolesc.......
+00000f60: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00000f70: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
+00000f80: 7221 0000 0072 3b00 0000 2902 7214 0000  r!...r;...).r...
+00000f90: 0072 3c00 0000 7215 0000 0072 1500 0000  .r<...r....r....
+00000fa0: 7216 0000 00da 085f 5f69 6e69 745f 5f80  r......__init__.
+00000fb0: 0000 0073 0200 0000 0001 7a25 4f73 6369  ...s......z%Osci
+00000fc0: 6c6c 6174 696e 6744 6970 6f6c 6541 7272  llatingDipoleArr
+00000fd0: 616e 6765 6d65 6e74 2e5f 5f69 6e69 745f  angement.__init_
+00000fe0: 5f29 02da 0964 6f74 5f69 6e70 7574 7210  _)...dot_inputr.
+00000ff0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00001000: 0200 0000 0500 0000 0300 0000 7338 0000  ............s8..
+00001010: 0074 00a0 017c 0164 0119 00a1 0189 017c  .t...|.d.......|
+00001020: 0164 0219 0089 0074 0274 0387 0087 0166  .d.....t.t.....f
+00001030: 0264 0364 0484 087c 006a 0444 0083 0183  .d.d...|.j.D....
+00001040: 0188 0188 0083 0353 0029 054e 7201 0000  .......S.).Nr...
+00001050: 00e9 0100 0000 6301 0000 0000 0000 0000  ......c.........
+00001060: 0000 0002 0000 0006 0000 0013 0000 0073  ...............s
+00001070: 1800 0000 6700 7c00 5d10 7d01 7c01 a000  ....g.|.].}.|...
+00001080: 8801 8800 a102 9102 7104 5300 7215 0000  ........q.S.r...
+00001090: 00a9 0172 2800 0000 a902 da02 2e30 5a06  ...r(........0Z.
+000010a0: 6469 706f 6c65 a902 7220 0000 0072 1800  dipole..r ...r..
+000010b0: 0000 7215 0000 0072 1600 0000 da0a 3c6c  ..r....r......<l
+000010c0: 6973 7463 6f6d 703e 8800 0000 7304 0000  istcomp>....s...
+000010d0: 0006 0202 ff7a 4e4f 7363 696c 6c61 7469  .....zNOscillati
+000010e0: 6e67 4469 706f 6c65 4172 7261 6e67 656d  ngDipoleArrangem
+000010f0: 656e 742e 6765 745f 706f 7465 6e74 6961  ent.get_potentia
+00001100: 6c5f 646f 745f 6d65 6173 7572 656d 656e  l_dot_measuremen
+00001110: 742e 3c6c 6f63 616c 733e 2e3c 6c69 7374  t.<locals>.<list
+00001120: 636f 6d70 3e29 0572 1100 0000 7212 0000  comp>).r....r...
+00001130: 0072 0500 0000 da03 7375 6d72 3c00 0000  .r......sumr<...
+00001140: 2902 7214 0000 0072 3e00 0000 7215 0000  ).r....r>...r...
+00001150: 0072 4300 0000 7216 0000 00da 1d67 6574  .rC...r......get
+00001160: 5f70 6f74 656e 7469 616c 5f64 6f74 5f6d  _potential_dot_m
+00001170: 6561 7375 7265 6d65 6e74 8300 0000 7316  easurement....s.
+00001180: 0000 0000 010e 0108 0102 0102 010c 0204  ................
+00001190: fe04 ff02 0602 0102 f87a 3a4f 7363 696c  .........z:Oscil
+000011a0: 6c61 7469 6e67 4469 706f 6c65 4172 7261  latingDipoleArra
+000011b0: 6e67 656d 656e 742e 6765 745f 706f 7465  ngement.get_pote
+000011c0: 6e74 6961 6c5f 646f 745f 6d65 6173 7572  ntial_dot_measur
+000011d0: 656d 656e 7429 02da 0e64 6f74 5f70 6169  ement)...dot_pai
+000011e0: 725f 696e 7075 7472 1000 0000 6302 0000  r_inputr....c...
+000011f0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00001200: 0003 0000 0073 4a00 0000 7400 a001 7c01  .....sJ...t...|.
+00001210: 6401 1900 a101 8901 7400 a001 7c01 6402  d.......t...|.d.
+00001220: 1900 a101 8902 7c01 6403 1900 8900 7402  ......|.d.....t.
+00001230: 7403 8700 8701 8702 6603 6404 6405 8408  t.......f.d.d...
+00001240: 7c00 6a04 4400 8301 8301 8801 8802 8800  |.j.D...........
+00001250: 8304 5300 2906 4e72 0100 0000 723f 0000  ..S.).Nr....r?..
+00001260: 0072 2500 0000 6301 0000 0000 0000 0000  .r%...c.........
+00001270: 0000 0002 0000 0007 0000 0013 0000 0073  ...............s
+00001280: 1a00 0000 6700 7c00 5d12 7d01 7c01 a000  ....g.|.].}.|...
+00001290: 8801 8802 8800 a103 9102 7104 5300 7215  ..........q.S.r.
+000012a0: 0000 00a9 0172 2d00 0000 7241 0000 00a9  .....r-...rA....
+000012b0: 0372 2000 0000 7229 0000 0072 2a00 0000  .r ...r)...r*...
+000012c0: 7215 0000 0072 1600 0000 7244 0000 0099  r....r....rD....
+000012d0: 0000 0073 0400 0000 0602 02ff 7a53 4f73  ...s........zSOs
+000012e0: 6369 6c6c 6174 696e 6744 6970 6f6c 6541  cillatingDipoleA
+000012f0: 7272 616e 6765 6d65 6e74 2e67 6574 5f70  rrangement.get_p
+00001300: 6f74 656e 7469 616c 5f64 6f74 5f70 6169  otential_dot_pai
+00001310: 725f 6d65 6173 7572 656d 656e 742e 3c6c  r_measurement.<l
+00001320: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00001330: 3e29 0572 1100 0000 7212 0000 0072 0700  >).r....r....r..
+00001340: 0000 7245 0000 0072 3c00 0000 2902 7214  ..rE...r<...).r.
+00001350: 0000 0072 4700 0000 7215 0000 0072 4900  ...rG...r....rI.
+00001360: 0000 7216 0000 00da 2267 6574 5f70 6f74  ..r....."get_pot
+00001370: 656e 7469 616c 5f64 6f74 5f70 6169 725f  ential_dot_pair_
+00001380: 6d65 6173 7572 656d 656e 7491 0000 0073  measurement....s
+00001390: 1a00 0000 0003 0e01 0e01 0801 0201 0201  ................
+000013a0: 0e02 04fe 04ff 0206 0201 0201 02f7 7a3f  ..............z?
+000013b0: 4f73 6369 6c6c 6174 696e 6744 6970 6f6c  OscillatingDipol
+000013c0: 6541 7272 616e 6765 6d65 6e74 2e67 6574  eArrangement.get
+000013d0: 5f70 6f74 656e 7469 616c 5f64 6f74 5f70  _potential_dot_p
+000013e0: 6169 725f 6d65 6173 7572 656d 656e 7429  air_measurement)
+000013f0: 02da 0a64 6f74 5f69 6e70 7574 7372 1000  ...dot_inputsr..
+00001400: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
+00001410: 0000 0003 0000 0003 0000 0073 1200 0000  ...........s....
+00001420: 8700 6601 6401 6402 8408 7c01 4400 8301  ..f.d.d...|.D...
+00001430: 5300 2903 7a7e 0a09 0946 6f72 2061 2073  S.).z~...For a s
+00001440: 6572 6965 7320 6f66 2070 6f69 6e74 732c  eries of points,
+00001450: 2065 6163 6820 7769 7468 2074 6872 6565   each with three
+00001460: 2063 6f6f 7264 696e 6174 6573 2061 6e64   coordinates and
+00001470: 2061 2066 7265 7175 656e 6379 2c20 7265   a frequency, re
+00001480: 7475 726e 2061 206c 6973 7420 6f66 2074  turn a list of t
+00001490: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
+000014a0: 2044 6f74 4d65 6173 7572 656d 656e 7473   DotMeasurements
+000014b0: 2e0a 0909 6301 0000 0000 0000 0000 0000  ....c...........
+000014c0: 0002 0000 0005 0000 0013 0000 0073 1600  .............s..
+000014d0: 0000 6700 7c00 5d0e 7d01 8800 a000 7c01  ..g.|.].}.....|.
+000014e0: a101 9102 7104 5300 7215 0000 0029 0172  ....q.S.r....).r
+000014f0: 4600 0000 a902 7242 0000 0072 3e00 0000  F.....rB...r>...
+00001500: 7213 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00001510: 4400 0000 a900 0000 7302 0000 0006 017a  D.......s......z
+00001520: 4f4f 7363 696c 6c61 7469 6e67 4469 706f  OOscillatingDipo
+00001530: 6c65 4172 7261 6e67 656d 656e 742e 6765  leArrangement.ge
+00001540: 745f 706f 7465 6e74 6961 6c5f 646f 745f  t_potential_dot_
+00001550: 6d65 6173 7572 656d 656e 7473 2e3c 6c6f  measurements.<lo
+00001560: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00001570: 7215 0000 0029 0272 1400 0000 724b 0000  r....).r....rK..
+00001580: 0072 1500 0000 7213 0000 0072 1600 0000  .r....r....r....
+00001590: da1e 6765 745f 706f 7465 6e74 6961 6c5f  ..get_potential_
+000015a0: 646f 745f 6d65 6173 7572 656d 656e 7473  dot_measurements
+000015b0: a300 0000 7306 0000 0000 060a 0102 ff7a  ....s..........z
+000015c0: 3b4f 7363 696c 6c61 7469 6e67 4469 706f  ;OscillatingDipo
+000015d0: 6c65 4172 7261 6e67 656d 656e 742e 6765  leArrangement.ge
+000015e0: 745f 706f 7465 6e74 6961 6c5f 646f 745f  t_potential_dot_
+000015f0: 6d65 6173 7572 656d 656e 7473 2902 da0f  measurements)...
+00001600: 646f 745f 7061 6972 5f69 6e70 7574 7372  dot_pair_inputsr
+00001610: 1000 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00001620: 0002 0000 0003 0000 0003 0000 0073 1200  .............s..
+00001630: 0000 8700 6601 6401 6402 8408 7c01 4400  ....f.d.d...|.D.
+00001640: 8301 5300 2903 7a8b 0a09 0946 6f72 2061  ..S.).z....For a
+00001650: 2073 6572 6965 7320 6f66 2070 6169 7273   series of pairs
+00001660: 206f 6620 706f 696e 7473 2c20 6561 6368   of points, each
+00001670: 2077 6974 6820 7468 7265 6520 636f 6f72   with three coor
+00001680: 6469 6e61 7465 7320 616e 6420 6120 6672  dinates and a fr
+00001690: 6571 7565 6e63 792c 2072 6574 7572 6e20  equency, return 
+000016a0: 6120 6c69 7374 206f 6620 7468 6520 636f  a list of the co
+000016b0: 7272 6573 706f 6e64 696e 6720 446f 7450  rresponding DotP
+000016c0: 6169 724d 6561 7375 7265 6d65 6e74 732e  airMeasurements.
+000016d0: 0a09 0963 0100 0000 0000 0000 0000 0000  ...c............
+000016e0: 0200 0000 0500 0000 1300 0000 7316 0000  ............s...
+000016f0: 0067 007c 005d 0e7d 0188 00a0 007c 01a1  .g.|.].}.....|..
+00001700: 0191 0271 0453 0072 1500 0000 2901 724a  ...q.S.r....).rJ
+00001710: 0000 0029 0272 4200 0000 7247 0000 0072  ...).rB...rG...r
+00001720: 1300 0000 7215 0000 0072 1600 0000 7244  ....r....r....rD
+00001730: 0000 00b3 0000 0073 0400 0000 0602 02ff  .......s........
+00001740: 7a54 4f73 6369 6c6c 6174 696e 6744 6970  zTOscillatingDip
+00001750: 6f6c 6541 7272 616e 6765 6d65 6e74 2e67  oleArrangement.g
+00001760: 6574 5f70 6f74 656e 7469 616c 5f64 6f74  et_potential_dot
+00001770: 5f70 6169 725f 6d65 6173 7572 656d 656e  _pair_measuremen
+00001780: 7473 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ts.<locals>.<lis
+00001790: 7463 6f6d 703e 7215 0000 0029 0272 1400  tcomp>r....).r..
+000017a0: 0000 724e 0000 0072 1500 0000 7213 0000  ..rN...r....r...
+000017b0: 0072 1600 0000 da23 6765 745f 706f 7465  .r.....#get_pote
+000017c0: 6e74 6961 6c5f 646f 745f 7061 6972 5f6d  ntial_dot_pair_m
+000017d0: 6561 7375 7265 6d65 6e74 73ad 0000 0073  easurements....s
+000017e0: 0600 0000 0006 0a02 02fe 7a40 4f73 6369  ..........z@Osci
+000017f0: 6c6c 6174 696e 6744 6970 6f6c 6541 7272  llatingDipoleArr
+00001800: 616e 6765 6d65 6e74 2e67 6574 5f70 6f74  angement.get_pot
+00001810: 656e 7469 616c 5f64 6f74 5f70 6169 725f  ential_dot_pair_
+00001820: 6d65 6173 7572 656d 656e 7473 2904 723e  measurements).r>
+00001830: 0000 00da 0b6c 6f77 5f70 6572 6365 6e74  .....low_percent
+00001840: da0c 6869 6768 5f70 6572 6365 6e74 7210  ..high_percentr.
+00001850: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
+00001860: 0400 0000 0700 0000 0300 0000 7358 0000  ............sX..
+00001870: 0074 00a0 017c 0164 0119 00a1 0189 017c  .t...|.d.......|
+00001880: 0164 0219 0089 0074 027c 0274 0387 0087  .d.....t.|.t....
+00001890: 0166 0264 0364 0484 087c 006a 0444 0083  .f.d.d...|.j.D..
+000018a0: 0183 0114 007c 0374 0387 0087 0166 0264  .....|.t.....f.d
+000018b0: 0564 0484 087c 006a 0444 0083 0183 0114  .d...|.j.D......
+000018c0: 0088 0188 0083 0453 0029 064e 7201 0000  .......S.).Nr...
+000018d0: 0072 3f00 0000 6301 0000 0000 0000 0000  .r?...c.........
+000018e0: 0000 0002 0000 0006 0000 0013 0000 0073  ...............s
+000018f0: 1800 0000 6700 7c00 5d10 7d01 7c01 a000  ....g.|.].}.|...
+00001900: 8801 8800 a102 9102 7104 5300 7215 0000  ........q.S.r...
+00001910: 0072 4000 0000 7241 0000 0072 4300 0000  .r@...rA...rC...
+00001920: 7215 0000 0072 1600 0000 7244 0000 00c0  r....r....rD....
+00001930: 0000 0073 0400 0000 0602 02ff 7a5c 4f73  ...s........z\Os
+00001940: 6369 6c6c 6174 696e 6744 6970 6f6c 6541  cillatingDipoleA
+00001950: 7272 616e 6765 6d65 6e74 2e67 6574 5f70  rrangement.get_p
+00001960: 6572 6365 6e74 5f72 616e 6765 5f70 6f74  ercent_range_pot
+00001970: 656e 7469 616c 5f64 6f74 5f6d 6561 7375  ential_dot_measu
+00001980: 7265 6d65 6e74 2e3c 6c6f 6361 6c73 3e2e  rement.<locals>.
+00001990: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
+000019a0: 0000 0000 0000 0002 0000 0006 0000 0013  ................
+000019b0: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
+000019c0: 7c01 a000 8801 8800 a102 9102 7104 5300  |...........q.S.
+000019d0: 7215 0000 0072 4000 0000 7241 0000 0072  r....r@...rA...r
+000019e0: 4300 0000 7215 0000 0072 1600 0000 7244  C...r....r....rD
+000019f0: 0000 00c7 0000 0073 0400 0000 0602 02ff  .......s........
+00001a00: 2905 7211 0000 0072 1200 0000 7206 0000  ).r....r....r...
+00001a10: 0072 4500 0000 723c 0000 0029 0472 1400  .rE...r<...).r..
+00001a20: 0000 723e 0000 0072 5000 0000 7251 0000  ..r>...rP...rQ..
+00001a30: 0072 1500 0000 7243 0000 0072 1600 0000  .r....rC...r....
+00001a40: da2b 6765 745f 7065 7263 656e 745f 7261  .+get_percent_ra
+00001a50: 6e67 655f 706f 7465 6e74 6961 6c5f 646f  nge_potential_do
+00001a60: 745f 6d65 6173 7572 656d 656e 74b8 0000  t_measurement...
+00001a70: 0073 2800 0000 0003 0e01 0801 0201 0201  .s(.............
+00001a80: 0201 0c02 04fe 04ff 02ff 0207 0201 0201  ................
+00001a90: 0c02 04fe 04ff 02ff 0207 0201 02f0 7a48  ..............zH
+00001aa0: 4f73 6369 6c6c 6174 696e 6744 6970 6f6c  OscillatingDipol
+00001ab0: 6541 7272 616e 6765 6d65 6e74 2e67 6574  eArrangement.get
+00001ac0: 5f70 6572 6365 6e74 5f72 616e 6765 5f70  _percent_range_p
+00001ad0: 6f74 656e 7469 616c 5f64 6f74 5f6d 6561  otential_dot_mea
+00001ae0: 7375 7265 6d65 6e74 2904 724b 0000 0072  surement).rK...r
+00001af0: 5000 0000 7251 0000 0072 1000 0000 6304  P...rQ...r....c.
+00001b00: 0000 0000 0000 0000 0000 0004 0000 0003  ................
+00001b10: 0000 0003 0000 0073 1600 0000 8700 8701  .......s........
+00001b20: 8702 6603 6401 6402 8408 7c01 4400 8301  ..f.d.d...|.D...
+00001b30: 5300 2903 fac4 0a09 0946 6f72 2061 2073  S.)......For a s
+00001b40: 6572 6965 7320 6f66 2070 6169 7273 206f  eries of pairs o
+00001b50: 6620 706f 696e 7473 2c20 6561 6368 2077  f points, each w
+00001b60: 6974 6820 7468 7265 6520 636f 6f72 6469  ith three coordi
+00001b70: 6e61 7465 7320 616e 6420 6120 6672 6571  nates and a freq
+00001b80: 7565 6e63 792c 2061 6e64 2061 6c73 6f20  uency, and also 
+00001b90: 6120 6c6f 7765 7220 6572 726f 7220 7261  a lower error ra
+00001ba0: 6e67 6520 616e 6420 7570 7065 7220 6572  nge and upper er
+00001bb0: 726f 7220 7261 6e67 652c 2072 6574 7572  ror range, retur
+00001bc0: 6e20 6120 6c69 7374 206f 6620 7468 6520  n a list of the 
+00001bd0: 636f 7272 6573 706f 6e64 696e 6720 446f  corresponding Do
+00001be0: 7450 6169 7252 616e 6765 4d65 6173 7572  tPairRangeMeasur
+00001bf0: 656d 656e 7473 2e0a 0909 6301 0000 0000  ements....c.....
+00001c00: 0000 0000 0000 0002 0000 0007 0000 0013  ................
+00001c10: 0000 0073 1a00 0000 6700 7c00 5d12 7d01  ...s....g.|.].}.
+00001c20: 8802 a000 7c01 8801 8800 a103 9102 7104  ....|.........q.
+00001c30: 5300 7215 0000 0029 0172 5200 0000 724c  S.r....).rR...rL
+00001c40: 0000 00a9 0372 5100 0000 7250 0000 0072  .....rQ...rP...r
+00001c50: 1400 0000 7215 0000 0072 1600 0000 7244  ....r....r....rD
+00001c60: 0000 00d6 0000 0073 0800 0000 0604 02fd  .......s........
+00001c70: 0401 06ff 7a5d 4f73 6369 6c6c 6174 696e  ....z]Oscillatin
+00001c80: 6744 6970 6f6c 6541 7272 616e 6765 6d65  gDipoleArrangeme
+00001c90: 6e74 2e67 6574 5f70 6572 6365 6e74 5f72  nt.get_percent_r
+00001ca0: 616e 6765 5f70 6f74 656e 7469 616c 5f64  ange_potential_d
+00001cb0: 6f74 5f6d 6561 7375 7265 6d65 6e74 732e  ot_measurements.
+00001cc0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00001cd0: 6d70 3e72 1500 0000 2904 7214 0000 0072  mp>r....).r....r
+00001ce0: 4b00 0000 7250 0000 0072 5100 0000 7215  K...rP...rQ...r.
+00001cf0: 0000 0072 5400 0000 7216 0000 00da 2c67  ...rT...r.....,g
+00001d00: 6574 5f70 6572 6365 6e74 5f72 616e 6765  et_percent_range
+00001d10: 5f70 6f74 656e 7469 616c 5f64 6f74 5f6d  _potential_dot_m
+00001d20: 6561 7375 7265 6d65 6e74 73d0 0000 0073  easurements....s
+00001d30: 0600 0000 0006 0e04 02fc 7a49 4f73 6369  ..........zIOsci
+00001d40: 6c6c 6174 696e 6744 6970 6f6c 6541 7272  llatingDipoleArr
+00001d50: 616e 6765 6d65 6e74 2e67 6574 5f70 6572  angement.get_per
+00001d60: 6365 6e74 5f72 616e 6765 5f70 6f74 656e  cent_range_poten
+00001d70: 7469 616c 5f64 6f74 5f6d 6561 7375 7265  tial_dot_measure
+00001d80: 6d65 6e74 7329 04da 0a70 6169 725f 696e  ments)...pair_in
+00001d90: 7075 7472 5000 0000 7251 0000 0072 1000  putrP...rQ...r..
+00001da0: 0000 6304 0000 0000 0000 0000 0000 0004  ..c.............
+00001db0: 0000 0007 0000 0003 0000 0073 6c00 0000  ...........sl...
+00001dc0: 7400 a001 7c01 6401 1900 a101 8901 7400  t...|.d.......t.
+00001dd0: a001 7c01 6402 1900 a101 8902 7c01 6403  ..|.d.......|.d.
+00001de0: 1900 8900 7402 7c02 7403 8700 8701 8702  ....t.|.t.......
+00001df0: 6603 6404 6405 8408 7c00 6a04 4400 8301  f.d.d...|.j.D...
+00001e00: 8301 1400 7c03 7403 8700 8701 8702 6603  ....|.t.......f.
+00001e10: 6406 6405 8408 7c00 6a04 4400 8301 8301  d.d...|.j.D.....
+00001e20: 1400 8801 8802 8800 8305 5300 2907 4e72  ..........S.).Nr
+00001e30: 0100 0000 723f 0000 0072 2500 0000 6301  ....r?...r%...c.
+00001e40: 0000 0000 0000 0000 0000 0002 0000 0007  ................
+00001e50: 0000 0013 0000 0073 1a00 0000 6700 7c00  .......s....g.|.
+00001e60: 5d12 7d01 7c01 a000 8801 8802 8800 a103  ].}.|...........
+00001e70: 9102 7104 5300 7215 0000 0072 4800 0000  ..q.S.r....rH...
+00001e80: 7241 0000 0072 4900 0000 7215 0000 0072  rA...rI...r....r
+00001e90: 1600 0000 7244 0000 00e6 0000 0073 0400  ....rD.......s..
+00001ea0: 0000 0602 02ff 7a61 4f73 6369 6c6c 6174  ......zaOscillat
+00001eb0: 696e 6744 6970 6f6c 6541 7272 616e 6765  ingDipoleArrange
+00001ec0: 6d65 6e74 2e67 6574 5f70 6572 6365 6e74  ment.get_percent
+00001ed0: 5f72 616e 6765 5f70 6f74 656e 7469 616c  _range_potential
+00001ee0: 5f64 6f74 5f70 6169 725f 6d65 6173 7572  _dot_pair_measur
+00001ef0: 656d 656e 742e 3c6c 6f63 616c 733e 2e3c  ement.<locals>.<
+00001f00: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
+00001f10: 0000 0000 0000 0200 0000 0700 0000 1300  ................
+00001f20: 0000 731a 0000 0067 007c 005d 127d 017c  ..s....g.|.].}.|
+00001f30: 01a0 0088 0188 0288 00a1 0391 0271 0453  .............q.S
+00001f40: 0072 1500 0000 7248 0000 0072 4100 0000  .r....rH...rA...
+00001f50: 7249 0000 0072 1500 0000 7216 0000 0072  rI...r....r....r
+00001f60: 4400 0000 ed00 0000 7304 0000 0006 0202  D.......s.......
+00001f70: ff29 0572 1100 0000 7212 0000 0072 0800  .).r....r....r..
+00001f80: 0000 7245 0000 0072 3c00 0000 2904 7214  ..rE...r<...).r.
+00001f90: 0000 0072 5600 0000 7250 0000 0072 5100  ...rV...rP...rQ.
+00001fa0: 0000 7215 0000 0072 4900 0000 7216 0000  ..r....rI...r...
+00001fb0: 00da 3067 6574 5f70 6572 6365 6e74 5f72  ..0get_percent_r
+00001fc0: 616e 6765 5f70 6f74 656e 7469 616c 5f64  ange_potential_d
+00001fd0: 6f74 5f70 6169 725f 6d65 6173 7572 656d  ot_pair_measurem
+00001fe0: 656e 74dd 0000 0073 2c00 0000 0003 0e01  ent....s,.......
+00001ff0: 0e01 0801 0201 0201 0201 0e02 04fe 04ff  ................
+00002000: 02ff 0207 0201 0201 0e02 04fe 04ff 02ff  ................
+00002010: 0207 0201 0201 02ef 7a4d 4f73 6369 6c6c  ........zMOscill
+00002020: 6174 696e 6744 6970 6f6c 6541 7272 616e  atingDipoleArran
+00002030: 6765 6d65 6e74 2e67 6574 5f70 6572 6365  gement.get_perce
+00002040: 6e74 5f72 616e 6765 5f70 6f74 656e 7469  nt_range_potenti
+00002050: 616c 5f64 6f74 5f70 6169 725f 6d65 6173  al_dot_pair_meas
+00002060: 7572 656d 656e 7429 04da 0b70 6169 725f  urement)...pair_
+00002070: 696e 7075 7473 7250 0000 0072 5100 0000  inputsrP...rQ...
+00002080: 7210 0000 0063 0400 0000 0000 0000 0000  r....c..........
+00002090: 0000 0400 0000 0300 0000 0300 0000 7316  ..............s.
+000020a0: 0000 0087 0087 0187 0266 0364 0164 0284  .........f.d.d..
+000020b0: 087c 0144 0083 0153 0029 0372 5300 0000  .|.D...S.).rS...
+000020c0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000020d0: 0007 0000 0013 0000 0073 1a00 0000 6700  .........s....g.
+000020e0: 7c00 5d12 7d01 8802 a000 7c01 8801 8800  |.].}.....|.....
+000020f0: a103 9102 7104 5300 7215 0000 0029 0172  ....q.S.r....).r
+00002100: 5700 0000 2902 7242 0000 0072 5600 0000  W...).rB...rV...
+00002110: 7254 0000 0072 1500 0000 7216 0000 0072  rT...r....r....r
+00002120: 4400 0000 0001 0000 7308 0000 0006 0402  D.......s.......
+00002130: fd04 0106 ff7a 624f 7363 696c 6c61 7469  .....zbOscillati
+00002140: 6e67 4469 706f 6c65 4172 7261 6e67 656d  ngDipoleArrangem
+00002150: 656e 742e 6765 745f 7065 7263 656e 745f  ent.get_percent_
+00002160: 7261 6e67 655f 706f 7465 6e74 6961 6c5f  range_potential_
+00002170: 646f 745f 7061 6972 5f6d 6561 7375 7265  dot_pair_measure
+00002180: 6d65 6e74 732e 3c6c 6f63 616c 733e 2e3c  ments.<locals>.<
+00002190: 6c69 7374 636f 6d70 3e72 1500 0000 2904  listcomp>r....).
+000021a0: 7214 0000 0072 5800 0000 7250 0000 0072  r....rX...rP...r
+000021b0: 5100 0000 7215 0000 0072 5400 0000 7216  Q...r....rT...r.
+000021c0: 0000 00da 3167 6574 5f70 6572 6365 6e74  ....1get_percent
+000021d0: 5f72 616e 6765 5f70 6f74 656e 7469 616c  _range_potential
+000021e0: 5f64 6f74 5f70 6169 725f 6d65 6173 7572  _dot_pair_measur
+000021f0: 656d 656e 7473 f700 0000 7306 0000 0000  ements....s.....
+00002200: 090e 0402 fc7a 4e4f 7363 696c 6c61 7469  .....zNOscillati
+00002210: 6e67 4469 706f 6c65 4172 7261 6e67 656d  ngDipoleArrangem
+00002220: 656e 742e 6765 745f 7065 7263 656e 745f  ent.get_percent_
+00002230: 7261 6e67 655f 706f 7465 6e74 6961 6c5f  range_potential_
+00002240: 646f 745f 7061 6972 5f6d 6561 7375 7265  dot_pair_measure
+00002250: 6d65 6e74 7372 0f00 0000 6301 0000 0000  mentsr....c.....
+00002260: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+00002270: 0000 0073 1600 0000 7400 a001 6401 6402  ...s....t...d.d.
+00002280: 8400 7c00 6a02 4400 8301 a101 5300 2903  ..|.j.D.....S.).
+00002290: 7a62 0a09 0952 6574 7572 6e73 2061 206e  zb...Returns a n
+000022a0: 756d 7079 2061 7272 6179 2077 6974 6820  umpy array with 
+000022b0: 7468 6520 6361 6e6f 6e69 6361 6c20 7265  the canonical re
+000022c0: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
+000022d0: 6561 6368 2064 6970 6f6c 6520 696e 2061  each dipole in a
+000022e0: 206e 7837 206e 756d 7079 2061 7272 6179   nx7 numpy array
+000022f0: 2e0a 0909 6301 0000 0000 0000 0000 0000  ....c...........
+00002300: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
+00002310: 0000 6700 7c00 5d0c 7d01 7c01 a000 a100  ..g.|.].}.|.....
+00002320: 9102 7104 5300 7215 0000 0029 0172 3200  ..q.S.r....).r2.
+00002330: 0000 7241 0000 0072 1500 0000 7215 0000  ..rA...r....r...
+00002340: 0072 1600 0000 7244 0000 000b 0100 00f3  .r....rD........
+00002350: 0000 0000 7a3f 4f73 6369 6c6c 6174 696e  ....z?Oscillatin
+00002360: 6744 6970 6f6c 6541 7272 616e 6765 6d65  gDipoleArrangeme
+00002370: 6e74 2e74 6f5f 6e75 6d70 795f 6172 7261  nt.to_numpy_arra
+00002380: 792e 3c6c 6f63 616c 733e 2e3c 6c69 7374  y.<locals>.<list
+00002390: 636f 6d70 3e29 0372 1100 0000 7212 0000  comp>).r....r...
+000023a0: 0072 3c00 0000 7213 0000 0072 1500 0000  .r<...r....r....
+000023b0: 7215 0000 0072 1600 0000 da0e 746f 5f6e  r....r......to_n
+000023c0: 756d 7079 5f61 7272 6179 0701 0000 7302  umpy_array....s.
+000023d0: 0000 0000 047a 2b4f 7363 696c 6c61 7469  .....z+Oscillati
+000023e0: 6e67 4469 706f 6c65 4172 7261 6e67 656d  ngDipoleArrangem
+000023f0: 656e 742e 746f 5f6e 756d 7079 5f61 7272  ent.to_numpy_arr
+00002400: 6179 4e29 1a72 3300 0000 7234 0000 0072  ayN).r3...r4...r
+00002410: 3500 0000 7236 0000 0072 0300 0000 720b  5...r6...r....r.
+00002420: 0000 0072 3d00 0000 7209 0000 0072 0500  ...r=...r....r..
+00002430: 0000 7246 0000 0072 0a00 0000 7207 0000  ..rF...r....r...
+00002440: 0072 4a00 0000 7204 0000 0072 4d00 0000  .rJ...r....rM...
+00002450: 724f 0000 0072 3900 0000 7206 0000 0072  rO...r9...r....r
+00002460: 5200 0000 7255 0000 0072 0800 0000 7257  R...rU...r....rW
+00002470: 0000 0072 5900 0000 7211 0000 0072 3700  ...rY...r....r7.
+00002480: 0000 725b 0000 0072 1500 0000 7215 0000  ..r[...r....r...
+00002490: 0072 1500 0000 7216 0000 0072 3a00 0000  .r....r....r:...
+000024a0: 7700 0000 7336 0000 0008 0104 0812 0310  w...s6..........
+000024b0: 0f02 0102 fe0c 1306 0106 fe0c 0b06 0106  ................
+000024c0: fe0c 0c06 0102 fe0c 190a 0106 fe0c 0e06  ................
+000024d0: 0102 fe0c 1c06 0102 0102 0106 fb0c 1072  ...............r
+000024e0: 3a00 0000 2914 da0b 6461 7461 636c 6173  :...)...dataclas
+000024f0: 7365 7372 0200 0000 7211 0000 00da 0c6e  sesr....r......n
+00002500: 756d 7079 2e74 7970 696e 67da 0674 7970  umpy.typing..typ
+00002510: 696e 6772 0300 0000 7204 0000 00da 1c70  ingr....r......p
+00002520: 646d 652e 6d65 6173 7572 656d 656e 742e  dme.measurement.
+00002530: 646f 745f 6d65 6173 7572 6572 0500 0000  dot_measurer....
+00002540: 7206 0000 00da 2170 646d 652e 6d65 6173  r.....!pdme.meas
+00002550: 7572 656d 656e 742e 646f 745f 7061 6972  urement.dot_pair
+00002560: 5f6d 6561 7375 7265 7207 0000 0072 0800  _measurer....r..
+00002570: 0000 da11 7064 6d65 2e63 616c 6375 6c61  ....pdme.calcula
+00002580: 7469 6f6e 7372 1900 0000 da1c 7064 6d65  tionsr......pdme
+00002590: 2e6d 6561 7375 7265 6d65 6e74 2e69 6e70  .measurement.inp
+000025a0: 7574 5f74 7970 6573 7209 0000 0072 0a00  ut_typesr....r..
+000025b0: 0000 720b 0000 0072 3a00 0000 7215 0000  ..r....r:...r...
+000025c0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+000025d0: da08 3c6d 6f64 756c 653e 0100 0000 7314  ..<module>....s.
+000025e0: 0000 000c 0108 0108 0110 0110 0110 0408  ................
+000025f0: 0110 0302 0110 68                        ......h
```

### Comparing `pdme-1.0.0/pdme/measurement/dot_measure.py` & `pdme-1.1.0/pdme/measurement/dot_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/measurement/dot_pair_measure.py` & `pdme-1.1.0/pdme/measurement/dot_pair_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/measurement/input_types.py` & `pdme-1.1.0/pdme/measurement/input_types.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/measurement/oscillating_dipole.py` & `pdme-1.1.0/pdme/measurement/oscillating_dipole.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy.typing
 from typing import Sequence, List
 from pdme.measurement.dot_measure import DotMeasurement, DotRangeMeasurement
 from pdme.measurement.dot_pair_measure import (
 	DotPairMeasurement,
 	DotPairRangeMeasurement,
 )
+import pdme.calculations
 from pdme.measurement.input_types import DotInput, DotPairInput
 
 
 @dataclass
 class OscillatingDipole:
 	"""
 	Representation of an oscillating dipole, either known or guessed.
@@ -34,37 +35,86 @@
 	def __post_init__(self) -> None:
 		"""
 		Coerce the inputs into numpy arrays.
 		"""
 		self.p = numpy.array(self.p)
 		self.s = numpy.array(self.s)
 
-	def s_at_position(self, r: numpy.ndarray, f: float) -> float:
+	def _alpha_electric_potential(self, r: numpy.ndarray) -> float:
+		"""
+		Returns the electric potential of this dipole at position r.
+		"""
+		return pdme.calculations.electric_potential(self.p, self.s, r)
+
+	def _alpha_electric_field(self, r: numpy.ndarray) -> numpy.ndarray:
+		"""
+		Returns the electric field of this dipole at position r.
+		"""
+		return pdme.calculations.electric_field(self.p, self.s, r)
+
+	def _b(self, f: float) -> float:
+		return pdme.calculations.telegraph_beta(f, self.w)
+
+	def s_electric_potential_at_position(self, r: numpy.ndarray, f: float) -> float:
 		"""
 		Returns the noise potential at a point r, at some frequency f.
 
+		Specifically for electric potential!
+
 		Parameters
 		----------
 		r : numpy.ndarray
 		The position of the dot.
 
 		f : float
 		The dot frequency to sample.
 		"""
-		return (self._alpha(r)) ** 2 * self._b(f)
+		return (self._alpha_electric_potential(r)) ** 2 * self._b(f)
 
-	def _alpha(self, r: numpy.ndarray) -> float:
-		diff = r - self.s
-		return self.p.dot(diff) / (numpy.linalg.norm(diff) ** 3)
+	def s_electric_potential_for_dot_pair(
+		self, r1: numpy.ndarray, r2: numpy.ndarray, f: float
+	) -> float:
+		"""
+		This is specifically the analytic cpsd for electric potential noise.
+		This should be deprecated
+		"""
+		return (
+			self._alpha_electric_potential(r1)
+			* self._alpha_electric_potential(r2)
+			* self._b(f)
+		)
 
-	def _b(self, f: float) -> float:
-		return (1 / numpy.pi) * (self.w / (f**2 + self.w**2))
+	def s_electric_fieldx_at_position(self, r: numpy.ndarray, f: float) -> float:
+		"""
+		Returns the noise potential at a point r, at some frequency f.
 
-	def s_for_dot_pair(self, r1: numpy.ndarray, r2: numpy.ndarray, f: float) -> float:
-		return self._alpha(r1) * self._alpha(r2) * self._b(f)
+		Specifically for electric potential!
+
+		Parameters
+		----------
+		r : numpy.ndarray
+		The position of the dot.
+
+		f : float
+		The dot frequency to sample.
+		"""
+		return (self._alpha_electric_field(r)[0]) ** 2 * self._b(f)
+
+	def s_electric_fieldx_for_dot_pair(
+		self, r1: numpy.ndarray, r2: numpy.ndarray, f: float
+	) -> float:
+		"""
+		This is specifically the analytic cpsd for electric potential noise.
+		This should be deprecated
+		"""
+		return (
+			self._alpha_electric_field(r1)[0]
+			* self._alpha_electric_field(r2)[0]
+			* self._b(f)
+		)
 
 	def to_flat_array(self) -> numpy.ndarray:
 		return numpy.concatenate([self.p, self.s, numpy.array([self.w])])
 
 
 class OscillatingDipoleArrangement:
 	"""
@@ -74,103 +124,141 @@
 	--------
 	dipoles : Sequence[OscillatingDipole]
 	"""
 
 	def __init__(self, dipoles: Sequence[OscillatingDipole]):
 		self.dipoles = dipoles
 
-	def get_dot_measurement(self, dot_input: DotInput) -> DotMeasurement:
+	def get_potential_dot_measurement(self, dot_input: DotInput) -> DotMeasurement:
 		r = numpy.array(dot_input[0])
 		f = dot_input[1]
 		return DotMeasurement(
-			sum([dipole.s_at_position(r, f) for dipole in self.dipoles]), r, f
+			sum(
+				[
+					dipole.s_electric_potential_at_position(r, f)
+					for dipole in self.dipoles
+				]
+			),
+			r,
+			f,
 		)
 
-	def get_dot_pair_measurement(
+	def get_potential_dot_pair_measurement(
 		self, dot_pair_input: DotPairInput
 	) -> DotPairMeasurement:
 		r1 = numpy.array(dot_pair_input[0])
 		r2 = numpy.array(dot_pair_input[1])
 		f = dot_pair_input[2]
 		return DotPairMeasurement(
-			sum([dipole.s_for_dot_pair(r1, r2, f) for dipole in self.dipoles]),
+			sum(
+				[
+					dipole.s_electric_potential_for_dot_pair(r1, r2, f)
+					for dipole in self.dipoles
+				]
+			),
 			r1,
 			r2,
 			f,
 		)
 
-	def get_dot_measurements(
+	def get_potential_dot_measurements(
 		self, dot_inputs: Sequence[DotInput]
 	) -> List[DotMeasurement]:
 		"""
 		For a series of points, each with three coordinates and a frequency, return a list of the corresponding DotMeasurements.
 		"""
-		return [self.get_dot_measurement(dot_input) for dot_input in dot_inputs]
+		return [
+			self.get_potential_dot_measurement(dot_input) for dot_input in dot_inputs
+		]
 
-	def get_dot_pair_measurements(
+	def get_potential_dot_pair_measurements(
 		self, dot_pair_inputs: Sequence[DotPairInput]
 	) -> List[DotPairMeasurement]:
 		"""
 		For a series of pairs of points, each with three coordinates and a frequency, return a list of the corresponding DotPairMeasurements.
 		"""
 		return [
-			self.get_dot_pair_measurement(dot_pair_input)
+			self.get_potential_dot_pair_measurement(dot_pair_input)
 			for dot_pair_input in dot_pair_inputs
 		]
 
-	def get_percent_range_dot_measurement(
+	def get_percent_range_potential_dot_measurement(
 		self, dot_input: DotInput, low_percent: float, high_percent: float
 	) -> DotRangeMeasurement:
 		r = numpy.array(dot_input[0])
 		f = dot_input[1]
 		return DotRangeMeasurement(
-			low_percent * sum([dipole.s_at_position(r, f) for dipole in self.dipoles]),
-			high_percent * sum([dipole.s_at_position(r, f) for dipole in self.dipoles]),
+			low_percent
+			* sum(
+				[
+					dipole.s_electric_potential_at_position(r, f)
+					for dipole in self.dipoles
+				]
+			),
+			high_percent
+			* sum(
+				[
+					dipole.s_electric_potential_at_position(r, f)
+					for dipole in self.dipoles
+				]
+			),
 			r,
 			f,
 		)
 
-	def get_percent_range_dot_measurements(
+	def get_percent_range_potential_dot_measurements(
 		self, dot_inputs: Sequence[DotInput], low_percent: float, high_percent: float
 	) -> List[DotRangeMeasurement]:
 		"""
 		For a series of pairs of points, each with three coordinates and a frequency, and also a lower error range and upper error range, return a list of the corresponding DotPairRangeMeasurements.
 		"""
 		return [
-			self.get_percent_range_dot_measurement(dot_input, low_percent, high_percent)
+			self.get_percent_range_potential_dot_measurement(
+				dot_input, low_percent, high_percent
+			)
 			for dot_input in dot_inputs
 		]
 
-	def get_percent_range_dot_pair_measurement(
+	def get_percent_range_potential_dot_pair_measurement(
 		self, pair_input: DotPairInput, low_percent: float, high_percent: float
 	) -> DotPairRangeMeasurement:
 		r1 = numpy.array(pair_input[0])
 		r2 = numpy.array(pair_input[1])
 		f = pair_input[2]
 		return DotPairRangeMeasurement(
 			low_percent
-			* sum([dipole.s_for_dot_pair(r1, r2, f) for dipole in self.dipoles]),
+			* sum(
+				[
+					dipole.s_electric_potential_for_dot_pair(r1, r2, f)
+					for dipole in self.dipoles
+				]
+			),
 			high_percent
-			* sum([dipole.s_for_dot_pair(r1, r2, f) for dipole in self.dipoles]),
+			* sum(
+				[
+					dipole.s_electric_potential_for_dot_pair(r1, r2, f)
+					for dipole in self.dipoles
+				]
+			),
 			r1,
 			r2,
 			f,
 		)
 
-	def get_percent_range_dot_pair_measurements(
+	def get_percent_range_potential_dot_pair_measurements(
 		self,
 		pair_inputs: Sequence[DotPairInput],
 		low_percent: float,
 		high_percent: float,
 	) -> List[DotPairRangeMeasurement]:
 		"""
 		For a series of pairs of points, each with three coordinates and a frequency, and also a lower error range and upper error range, return a list of the corresponding DotPairRangeMeasurements.
 		"""
 		return [
-			self.get_percent_range_dot_pair_measurement(
+			self.get_percent_range_potential_dot_pair_measurement(
 				pair_input, low_percent, high_percent
 			)
 			for pair_input in pair_inputs
 		]
 
 	def to_numpy_array(self) -> numpy.ndarray:
 		"""
```

### Comparing `pdme-1.0.0/pdme/model/__init__.py` & `pdme-1.1.0/pdme/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/model/__pycache__/__init__.cpython-39.pyc` & `pdme-1.1.0/pdme/model/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 1066 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 2a04 0000  a.......&./f*...
+00000000: 610d 0d0a 0000 0000 9a1c 3466 2a04 0000  a.........4f*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -52,11 +52,11 @@
 00000330: 646f 6d5f 6368 6f69 6365 5f66 6978 6564  dom_choice_fixed
 00000340: 5f6f 7269 656e 7461 7469 6f6e 5f6d 6f64  _orientation_mod
 00000350: 656c 7208 0000 00da 075f 5f61 6c6c 5f5f  elr......__all__
 00000360: a900 720a 0000 0072 0a00 0000 fa4d 2f68  ..r....r.....M/h
 00000370: 6f6d 652f 6a65 6e6b 696e 732f 6167 656e  ome/jenkins/agen
 00000380: 742f 776f 726b 7370 6163 652f 6769 7465  t/workspace/gite
 00000390: 612d 7068 7973 6963 735f 7064 6d65 5f31  a-physics_pdme_1
-000003a0: 2e30 2e30 2f70 646d 652f 6d6f 6465 6c2f  .0.0/pdme/model/
+000003a0: 2e31 2e30 2f70 646d 652f 6d6f 6465 6c2f  .1.0/pdme/model/
 000003b0: 5f5f 696e 6974 5f5f 2e70 79da 083c 6d6f  __init__.py..<mo
 000003c0: 6475 6c65 3e01 0000 0073 0e00 0000 0c01  dule>....s......
 000003d0: 0c01 0c03 0c04 0c04 0c04 0c04            ............
```

### Comparing `pdme-1.0.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc` & `pdme-1.1.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 2367 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 3f09 0000  a.......&./f?...
+00000000: 610d 0d0a 0000 0000 9a1c 3466 3f09 0000  a.........4f?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6503 8303 5a07 6401 5300 2906  ..d.e...Z.d.S.).
 00000070: e900 0000 004e 2901 da0b 4469 706f 6c65  .....N)...Dipole
@@ -45,15 +45,15 @@
 000002c0: 7261 6e64 6f6d da0b 6465 6661 756c 745f  random..default_
 000002d0: 726e 67da 0372 6e67 2908 da04 7365 6c66  rng..rng)...self
 000002e0: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
 000002f0: 0900 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
 00000300: 0000 00a9 0072 1300 0000 fa5a 2f68 6f6d  .....r.....Z/hom
 00000310: 652f 6a65 6e6b 696e 732f 6167 656e 742f  e/jenkins/agent/
 00000320: 776f 726b 7370 6163 652f 6769 7465 612d  workspace/gitea-
-00000330: 7068 7973 6963 735f 7064 6d65 5f31 2e30  physics_pdme_1.0
+00000330: 7068 7973 6963 735f 7064 6d65 5f31 2e31  physics_pdme_1.1
 00000340: 2e30 2f70 646d 652f 6d6f 6465 6c2f 6669  .0/pdme/model/fi
 00000350: 7865 645f 6d61 676e 6974 7564 655f 6d6f  xed_magnitude_mo
 00000360: 6465 6c2e 7079 da08 5f5f 696e 6974 5f5f  del.py..__init__
 00000370: 1400 0000 7310 0000 0000 0a06 0106 0106  ....s...........
 00000380: 0106 0106 0106 0106 017a 2853 696e 676c  .........z(Singl
 00000390: 6544 6970 6f6c 6546 6978 6564 4d61 676e  eDipoleFixedMagn
 000003a0: 6974 7564 654d 6f64 656c 2e5f 5f69 6e69  itudeModel.__ini
```

### Comparing `pdme-1.0.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc` & `pdme-1.1.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 5158 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 2614 0000  a.......&./f&...
+00000000: 610d 0d0a 0000 0000 9a1c 3466 2614 0000  a.........4f&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6401 6c07  m.Z.m.Z...d.d.l.
 00000060: 5a07 6400 6404 6c08 6d09 5a09 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6401 6c0a 5a0b 6507 a00c 650d a101 5a0e  d.l.Z.e...e...Z.
@@ -107,15 +107,15 @@
 000006a0: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
 000006b0: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
 000006c0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
 000006d0: 0000 da02 7078 da02 7079 da02 707a a900  ....px..py..pz..
 000006e0: 7223 0000 00fa 752f 686f 6d65 2f6a 656e  r#....u/home/jen
 000006f0: 6b69 6e73 2f61 6765 6e74 2f77 6f72 6b73  kins/agent/works
 00000700: 7061 6365 2f67 6974 6561 2d70 6879 7369  pace/gitea-physi
-00000710: 6373 5f70 646d 655f 312e 302e 302f 7064  cs_pdme_1.0.0/pd
+00000710: 6373 5f70 646d 655f 312e 312e 302f 7064  cs_pdme_1.1.0/pd
 00000720: 6d65 2f6d 6f64 656c 2f6c 6f67 5f73 7061  me/model/log_spa
 00000730: 6365 645f 7261 6e64 6f6d 5f63 686f 6963  ced_random_choic
 00000740: 655f 6669 7865 645f 6f72 6965 6e74 6174  e_fixed_orientat
 00000750: 696f 6e5f 6d6f 6465 6c2e 7079 da08 5f5f  ion_model.py..__
 00000760: 696e 6974 5f5f 2d00 0000 732c 0000 0000  init__-...s,....
 00000770: 1006 0106 0106 0106 0106 0106 0106 0106  ................
 00000780: 0106 0106 0106 010c 0106 021e 011e 0112  ................
```

### Comparing `pdme-1.0.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc` & `pdme-1.1.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 5332 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 d414 0000  a.......&./f....
+00000000: 610d 0d0a 0000 0000 9a1c 3466 d414 0000  a.........4f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6401 6c07  m.Z.m.Z...d.d.l.
 00000060: 5a08 6400 6404 6c09 6d0a 5a0a 0100 4700  Z.d.d.l.m.Z...G.
 00000070: 6405 6406 8400 6406 6503 8303 5a0b 6401  d.d...d.e...Z.d.
@@ -81,15 +81,15 @@
 00000500: 0000 0029 0cda 0473 656c 6672 0700 0000  ...)...selfr....
 00000510: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
 00000520: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
 00000530: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
 00000540: 0000 a900 721a 0000 00fa 632f 686f 6d65  ....r.....c/home
 00000550: 2f6a 656e 6b69 6e73 2f61 6765 6e74 2f77  /jenkins/agent/w
 00000560: 6f72 6b73 7061 6365 2f67 6974 6561 2d70  orkspace/gitea-p
-00000570: 6879 7369 6373 5f70 646d 655f 312e 302e  hysics_pdme_1.0.
+00000570: 6879 7369 6373 5f70 646d 655f 312e 312e  hysics_pdme_1.1.
 00000580: 302f 7064 6d65 2f6d 6f64 656c 2f6c 6f67  0/pdme/model/log
 00000590: 5f73 7061 6365 645f 7261 6e64 6f6d 5f63  _spaced_random_c
 000005a0: 686f 6963 655f 6d6f 6465 6c2e 7079 da08  hoice_model.py..
 000005b0: 5f5f 696e 6974 5f5f 2000 0000 7320 0000  __init__ ...s ..
 000005c0: 0000 0e06 0106 0106 0106 0106 0106 0106  ................
 000005d0: 0106 0106 010c 0106 0110 0102 0108 ff04  ................
 000005e0: 037a 3e4c 6f67 5370 6163 6564 5261 6e64  .z>LogSpacedRand
@@ -262,15 +262,15 @@
 00001050: 0000 0072 3100 0000 5a09 6465 6c74 615f  ...r1...Z.delta_
 00001060: 7068 695a 0d74 656e 7461 7469 7665 5f70  phiZ.tentative_p
 00001070: 6869 5a0b 6465 6c74 615f 7468 6574 61da  hiZ.delta_theta.
 00001080: 0172 5a0f 7465 6e74 6174 6976 655f 7468  .rZ.tentative_th
 00001090: 6574 615a 0c74 656e 7461 7469 7665 5f70  etaZ.tentative_p
 000010a0: 785a 0c74 656e 7461 7469 7665 5f70 795a  xZ.tentative_pyZ
 000010b0: 0c74 656e 7461 7469 7665 5f70 7ada 0272  .tentative_pz..r
-000010c0: 785a 0272 795a 0272 7a5a 0c74 656e 7461  xZ.ryZ.rzZ.tenta
+000010c0: 78da 0272 795a 0272 7a5a 0c74 656e 7461  x..ryZ.rzZ.tenta
 000010d0: 7469 7665 5f72 785a 0c74 656e 7461 7469  tive_rxZ.tentati
 000010e0: 7665 5f72 795a 0c74 656e 7461 7469 7665  ve_ryZ.tentative
 000010f0: 5f72 7a72 4200 0000 5a0b 7465 6e74 6174  _rzrB...Z.tentat
 00001100: 6976 655f 77da 0d74 656e 7461 7469 7665  ive_w..tentative
 00001110: 5f64 6970 721a 0000 0072 1a00 0000 721b  _dipr....r....r.
 00001120: 0000 00da 216d 6172 6b6f 765f 6368 6169  ....!markov_chai
 00001130: 6e5f 6d6f 6e74 655f 6361 726c 6f5f 7072  n_monte_carlo_pr
@@ -294,25 +294,25 @@
 00001250: 0373 7472 721e 0000 0072 1400 0000 7215  .strr....r....r.
 00001260: 0000 00da 0947 656e 6572 6174 6f72 7204  .....Generatorr.
 00001270: 0000 0072 3700 0000 da07 6e64 6172 7261  ...r7.....ndarra
 00001280: 7972 4300 0000 da04 7064 6d65 da13 7375  yrC.....pdme..su
 00001290: 6273 7061 6365 5f73 696d 756c 6174 696f  bspace_simulatio
 000012a0: 6eda 1744 6970 6f6c 6553 7461 6e64 6172  n..DipoleStandar
 000012b0: 6444 6576 6961 7469 6f6e 7205 0000 0072  dDeviationr....r
-000012c0: 5700 0000 721a 0000 0072 1a00 0000 721a  W...r....r....r.
+000012c0: 5800 0000 721a 0000 0072 1a00 0000 721a  X...r....r....r.
 000012d0: 0000 0072 1b00 0000 7206 0000 000c 0000  ...r....r.......
 000012e0: 0073 4400 0000 0801 0415 0201 0201 0201  .sD.............
 000012f0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00001300: 02f3 0c1f 0e04 00ff 0201 0801 02fe 0c25  ...............%
 00001310: 00fc 0202 0201 0201 0601 04fb 0c24 00fc  .............$..
 00001320: 0202 0401 0601 0a01 04fb 7206 0000 0029  ..........r....)
 00001330: 0c72 1400 0000 da0c 6e75 6d70 792e 7261  .r......numpy.ra
 00001340: 6e64 6f6d da10 7064 6d65 2e6d 6f64 656c  ndom..pdme.model
 00001350: 2e6d 6f64 656c 7202 0000 00da 1070 646d  .modelr......pdm
 00001360: 652e 6d65 6173 7572 656d 656e 7472 0300  e.measurementr..
 00001370: 0000 7204 0000 00da 1870 646d 652e 7375  ..r......pdme.su
 00001380: 6273 7061 6365 5f73 696d 756c 6174 696f  bspace_simulatio
-00001390: 6e72 6100 0000 da06 7479 7069 6e67 7205  nra.....typingr.
+00001390: 6e72 6200 0000 da06 7479 7069 6e67 7205  nrb.....typingr.
 000013a0: 0000 0072 0600 0000 721a 0000 0072 1a00  ...r....r....r..
 000013b0: 0000 721a 0000 0072 1b00 0000 da08 3c6d  ..r....r......<m
 000013c0: 6f64 756c 653e 0100 0000 730c 0000 0008  odule>....s.....
 000013d0: 0108 010c 0110 0408 010c 03              ...........
```

### Comparing `pdme-1.0.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc` & `pdme-1.1.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 4699 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 5b12 0000  a.......&./f[...
+00000000: 610d 0d0a 0000 0000 9a1c 3466 5b12 0000  a.........4f[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6401 6c07  m.Z.m.Z...d.d.l.
 00000060: 5a08 6400 6404 6c09 6d0a 5a0a 0100 4700  Z.d.d.l.m.Z...G.
 00000070: 6405 6406 8400 6406 6503 8303 5a0b 6401  d.d...d.e...Z.d.
@@ -82,15 +82,15 @@
 00000510: 0029 0cda 0473 656c 6672 0700 0000 7208  .)...selfr....r.
 00000520: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
 00000530: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
 00000540: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
 00000550: a900 721a 0000 00fa 662f 686f 6d65 2f6a  ..r.....f/home/j
 00000560: 656e 6b69 6e73 2f61 6765 6e74 2f77 6f72  enkins/agent/wor
 00000570: 6b73 7061 6365 2f67 6974 6561 2d70 6879  kspace/gitea-phy
-00000580: 7369 6373 5f70 646d 655f 312e 302e 302f  sics_pdme_1.0.0/
+00000580: 7369 6373 5f70 646d 655f 312e 312e 302f  sics_pdme_1.1.0/
 00000590: 7064 6d65 2f6d 6f64 656c 2f6c 6f67 5f73  pdme/model/log_s
 000005a0: 7061 6365 645f 7261 6e64 6f6d 5f63 686f  paced_random_cho
 000005b0: 6963 655f 7879 5f6d 6f64 656c 2e70 79da  ice_xy_model.py.
 000005c0: 085f 5f69 6e69 745f 5f20 0000 0073 2000  .__init__ ...s .
 000005d0: 0000 000e 0601 0601 0601 0601 0601 0601  ................
 000005e0: 0601 0601 0601 0c01 0601 1001 0201 08ff  ................
 000005f0: 0403 7a40 4c6f 6753 7061 6365 6452 616e  ..z@LogSpacedRan
```

### Comparing `pdme-1.0.0/pdme/model/__pycache__/model.cpython-39.pyc` & `pdme-1.1.0/pdme/model/__pycache__/model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 3594 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 0a0e 0000  a.......&./f....
+00000000: 610d 0d0a 0000 0000 9a1c 3466 0a0e 0000  a.........4f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 6400 6401 6c05 5a06 6400 6403 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6504  m.Z.m.Z.m.Z...e.
 00000070: a00b 650c a101 5a0d 4700 6404 6405 8400  ..e...Z.G.d.d...
@@ -59,15 +59,15 @@
 000003a0: 6672 6571 7565 6e63 7929 2e0a 0909 4ea9  frequency)....N.
 000003b0: 01da 134e 6f74 496d 706c 656d 656e 7465  ...NotImplemente
 000003c0: 6445 7272 6f72 2903 da04 7365 6c66 7207  dError)...selfr.
 000003d0: 0000 0072 0800 0000 a900 720d 0000 00fa  ...r......r.....
 000003e0: 4a2f 686f 6d65 2f6a 656e 6b69 6e73 2f61  J/home/jenkins/a
 000003f0: 6765 6e74 2f77 6f72 6b73 7061 6365 2f67  gent/workspace/g
 00000400: 6974 6561 2d70 6879 7369 6373 5f70 646d  itea-physics_pdm
-00000410: 655f 312e 302e 302f 7064 6d65 2f6d 6f64  e_1.0.0/pdme/mod
+00000410: 655f 312e 312e 302f 7064 6d65 2f6d 6f64  e_1.1.0/pdme/mod
 00000420: 656c 2f6d 6f64 656c 2e70 79da 0b67 6574  el/model.py..get
 00000430: 5f64 6970 6f6c 6573 1300 0000 7302 0000  _dipoles....s...
 00000440: 0000 087a 1744 6970 6f6c 654d 6f64 656c  ...z.DipoleModel
 00000450: 2e67 6574 5f64 6970 6f6c 6573 2904 da01  .get_dipoles)...
 00000460: 6e72 0700 0000 7208 0000 0072 0900 0000  nr....r....r....
 00000470: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
 00000480: 0001 0000 0043 0000 0073 0800 0000 7400  .....C...s....t.
```

### Comparing `pdme-1.0.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc` & `pdme-1.1.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 2560 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 000a 0000  a.......&./f....
+00000000: 610d 0d0a 0000 0000 9a1c 3466 000a 0000  a.........4f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6503 8303 5a07 6401 5300 2906  ..d.e...Z.d.S.).
 00000070: e900 0000 004e 2901 da0b 4469 706f 6c65  .....N)...Dipole
@@ -49,15 +49,15 @@
 00000300: 745f 726e 67da 0372 6e67 720d 0000 0029  t_rng..rngr....)
 00000310: 09da 0473 656c 6672 0600 0000 7207 0000  ...selfr....r...
 00000320: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
 00000330: 720b 0000 0072 0c00 0000 720d 0000 00a9  r....r....r.....
 00000340: 0072 1400 0000 fa66 2f68 6f6d 652f 6a65  .r.....f/home/je
 00000350: 6e6b 696e 732f 6167 656e 742f 776f 726b  nkins/agent/work
 00000360: 7370 6163 652f 6769 7465 612d 7068 7973  space/gitea-phys
-00000370: 6963 735f 7064 6d65 5f31 2e30 2e30 2f70  ics_pdme_1.0.0/p
+00000370: 6963 735f 7064 6d65 5f31 2e31 2e30 2f70  ics_pdme_1.1.0/p
 00000380: 646d 652f 6d6f 6465 6c2f 6d75 6c74 6964  dme/model/multid
 00000390: 6970 6f6c 655f 6669 7865 645f 6d61 676e  ipole_fixed_magn
 000003a0: 6974 7564 655f 6d6f 6465 6c2e 7079 da08  itude_model.py..
 000003b0: 5f5f 696e 6974 5f5f 1700 0000 7312 0000  __init__....s...
 000003c0: 0000 0b06 0106 0106 0106 0106 0106 0106  ................
 000003d0: 010c 017a 2a4d 756c 7469 706c 6544 6970  ...z*MultipleDip
 000003e0: 6f6c 6546 6978 6564 4d61 676e 6974 7564  oleFixedMagnitud
```

### Comparing `pdme-1.0.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc` & `pdme-1.1.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 3076 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 040c 0000  a.......&./f....
+00000000: 610d 0d0a 0000 0000 9a1c 3466 040c 0000  a.........4f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6503 8303 5a07 6401 5300 2906  ..d.e...Z.d.S.).
 00000070: e900 0000 004e 2901 da0b 4469 706f 6c65  .....N)...Dipole
@@ -65,15 +65,15 @@
 00000400: 7272 0e00 0000 290a da04 7365 6c66 7206  rr....)...selfr.
 00000410: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
 00000420: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
 00000430: 0072 0d00 0000 720e 0000 00a9 0072 1700  .r....r......r..
 00000440: 0000 fa73 2f68 6f6d 652f 6a65 6e6b 696e  ...s/home/jenkin
 00000450: 732f 6167 656e 742f 776f 726b 7370 6163  s/agent/workspac
 00000460: 652f 6769 7465 612d 7068 7973 6963 735f  e/gitea-physics_
-00000470: 7064 6d65 5f31 2e30 2e30 2f70 646d 652f  pdme_1.0.0/pdme/
+00000470: 7064 6d65 5f31 2e31 2e30 2f70 646d 652f  pdme_1.1.0/pdme/
 00000480: 6d6f 6465 6c2f 7261 6e64 6f6d 5f63 6f75  model/random_cou
 00000490: 6e74 5f6d 756c 7469 6469 706f 6c65 5f66  nt_multidipole_f
 000004a0: 6978 6564 5f6d 6167 6e69 7475 6465 5f6d  ixed_magnitude_m
 000004b0: 6f64 656c 2e70 79da 085f 5f69 6e69 745f  odel.py..__init_
 000004c0: 5f1a 0000 0073 1c00 0000 000c 0601 0601  _....s..........
 000004d0: 0601 0601 0601 0601 0601 0c01 0601 1001  ................
 000004e0: 0201 08ff 0403 7a35 5261 6e64 6f6d 436f  ......z5RandomCo
```

### Comparing `pdme-1.0.0/pdme/model/fixed_magnitude_model.py` & `pdme-1.1.0/pdme/model/fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py` & `pdme-1.1.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/model/log_spaced_random_choice_model.py` & `pdme-1.1.0/pdme/model/log_spaced_random_choice_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/model/log_spaced_random_choice_xy_model.py` & `pdme-1.1.0/pdme/model/log_spaced_random_choice_xy_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/model/model.py` & `pdme-1.1.0/pdme/model/model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/model/multidipole_fixed_magnitude_model.py` & `pdme-1.1.0/pdme/model/multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py` & `pdme-1.1.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/subspace_simulation/__init__.py` & `pdme-1.1.0/pdme/subspace_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc` & `pdme-1.1.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 1364 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 5405 0000  a.......&./fT...
+00000000: 610d 0d0a 0000 0000 9a1c 3466 5405 0000  a.........4fT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6501  d.l.m.Z.m.Z...e.
 00000060: 4700 6405 6406 8400 6406 8302 8301 5a08  G.d.d...d.....Z.
 00000070: 4700 6407 6408 8400 6408 8302 5a09 6504  G.d.d...d...Z.e.
@@ -36,15 +36,15 @@
 00000230: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
 00000240: 5f5f 646f 635f 5fda 0566 6c6f 6174 da0f  __doc__..float..
 00000250: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fa9  __annotations__.
 00000260: 0072 0d00 0000 720d 0000 00fa 5b2f 686f  .r....r.....[/ho
 00000270: 6d65 2f6a 656e 6b69 6e73 2f61 6765 6e74  me/jenkins/agent
 00000280: 2f77 6f72 6b73 7061 6365 2f67 6974 6561  /workspace/gitea
 00000290: 2d70 6879 7369 6373 5f70 646d 655f 312e  -physics_pdme_1.
-000002a0: 302e 302f 7064 6d65 2f73 7562 7370 6163  0.0/pdme/subspac
+000002a0: 312e 302f 7064 6d65 2f73 7562 7370 6163  1.0/pdme/subspac
 000002b0: 655f 7369 6d75 6c61 7469 6f6e 2f5f 5f69  e_simulation/__i
 000002c0: 6e69 745f 5f2e 7079 7206 0000 000a 0000  nit__.pyr.......
 000002d0: 0073 0e00 0000 0a02 0404 0801 0801 0801  .s..............
 000002e0: 0801 0801 7206 0000 0063 0000 0000 0000  ....r....c......
 000002f0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
 00000300: 0000 732a 0000 0065 005a 0164 005a 0264  ..s*...e.Z.d.Z.d
 00000310: 015a 0365 0465 0519 0064 029c 0164 0364  .Z.e.e...d...d.d
```

### Comparing `pdme-1.0.0/pdme/subspace_simulation/__pycache__/mcmc_costs.cpython-39.pyc` & `pdme-1.1.0/pdme/subspace_simulation/__pycache__/mcmc_costs.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 575 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 3f02 0000  a.......&./f?...
+00000000: 610d 0d0a 0000 0000 9a1c 3466 3f02 0000  a.........4f?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6500 6a04 6500 6a04 6500  d.l.Z.e.j.e.j.e.
 00000050: 6a04 6402 9c03 6403 6404 8404 5a05 6500  j.d...d.d...Z.e.
 00000060: 6a04 6500 6a04 6500 6a04 6500 6a04 6405  j.e.j.e.j.e.j.d.
 00000070: 9c04 6406 6407 8404 5a06 6401 5300 2908  ..d.d...Z.d.S.).
@@ -16,15 +16,15 @@
 000000f0: 6178 6973 2903 da05 6e75 6d70 79da 036d  axis)...numpy..m
 00000100: 6178 da07 6d61 7869 6d75 6d29 0472 0200  ax..maximum).r..
 00000110: 0000 7203 0000 005a 0474 6f70 735a 0762  ..r....Z.topsZ.b
 00000120: 6f74 746f 6d73 a900 720a 0000 00fa 5d2f  ottoms..r.....]/
 00000130: 686f 6d65 2f6a 656e 6b69 6e73 2f61 6765  home/jenkins/age
 00000140: 6e74 2f77 6f72 6b73 7061 6365 2f67 6974  nt/workspace/git
 00000150: 6561 2d70 6879 7369 6373 5f70 646d 655f  ea-physics_pdme_
-00000160: 312e 302e 302f 7064 6d65 2f73 7562 7370  1.0.0/pdme/subsp
+00000160: 312e 312e 302f 7064 6d65 2f73 7562 7370  1.1.0/pdme/subsp
 00000170: 6163 655f 7369 6d75 6c61 7469 6f6e 2f6d  ace_simulation/m
 00000180: 636d 635f 636f 7374 732e 7079 da11 7072  cmc_costs.py..pr
 00000190: 6f70 6f72 7469 6f6e 616c 5f63 6f73 7406  oportional_cost.
 000001a0: 0000 0073 0600 0000 0001 1201 1201 720c  ...s..........r.
 000001b0: 0000 0029 04da 1064 6f74 5f69 6e70 7574  ...)...dot_input
 000001c0: 735f 6172 7261 79da 1861 6374 7561 6c5f  s_array..actual_
 000001d0: 6d65 6173 7572 656d 656e 745f 6172 7261  measurement_arra
```

### Comparing `pdme-1.0.0/pdme/subspace_simulation/mcmc_costs.py` & `pdme-1.1.0/pdme/subspace_simulation/mcmc_costs.py`

 * *Files identical despite different names*

### Comparing `pdme-1.0.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc` & `pdme-1.1.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 7925 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 f51e 0000  a.......&./f....
+00000000: 610d 0d0a 0000 0000 9a1c 3466 cb24 0000  a.........4f.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6501  d.l.Z.d.d.l.Z.e.
 00000040: a002 6503 a101 5a04 6500 6a05 6500 6a05  ..e...Z.e.j.e.j.
 00000050: 6500 6a05 6402 9c03 6403 6404 8404 5a06  e.j.d...d.d...Z.
 00000060: 6500 6a05 6500 6a05 6500 6a05 6405 9c03  e.j.e.j.e.j.d...
 00000070: 6406 6407 8404 5a07 6500 6a05 6500 6a05  d.d...Z.e.j.e.j.
 00000080: 6500 6a05 6405 9c03 6408 6409 8404 5a08  e.j.d...d.d...Z.
 00000090: 640a 640b 8400 5a09 6401 5300 290c e900  d.d...Z.d.S.)...
 000000a0: 0000 004e 2903 da0f 646f 745f 7061 6972  ...N)...dot_pair
 000000b0: 5f69 6e70 7574 73da 0764 6970 6f6c 6573  _inputs..dipoles
 000000c0: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
-000000d0: 0000 0000 0010 0000 0006 0000 0043 0000  .............C..
+000000d0: 0000 0000 0010 0000 0005 0000 0043 0000  .............C..
 000000e0: 0073 3002 0000 7c01 6401 6401 8502 6402  .s0...|.d.d...d.
 000000f0: 6403 8502 6602 1900 7d02 7c01 6401 6401  d...f...}.|.d.d.
 00000100: 8502 6403 6404 8502 6602 1900 7d03 7c01  ..d.d...f...}.|.
 00000110: 6401 6401 8502 6404 6602 1900 7d04 7400  d.d...d.f...}.t.
 00000120: a001 6405 7c02 9b00 9d02 a101 0100 7400  ..d.|.........t.
 00000130: a001 6406 7c03 9b00 9d02 a101 0100 7400  ..d.|.........t.
 00000140: a001 6407 7c04 9b00 9d02 a101 0100 7c00  ..d.|.........|.
@@ -37,18 +37,18 @@
 00000240: 9001 727e 7400 a001 640e 7c0b 9b00 9d02  ..r~t...d.|.....
 00000250: a101 0100 7400 a001 640f 7c0c 9b00 9d02  ....t...d.|.....
 00000260: a101 0100 7407 a00a 6410 7c09 7c02 a103  ....t...d.|.|...
 00000270: 7c0b 1b00 7d0d 7407 a00a 6410 7c0a 7c02  |...}.t...d.|.|.
 00000280: a103 7c0c 1b00 7d0e 7400 a004 7405 6a06  ..|...}.t...t.j.
 00000290: a101 9001 72d0 7400 a001 6411 7c0d 9b00  ....r.t...d.|...
 000002a0: 9d02 a101 0100 7400 a001 6412 7c0e 9b00  ......t...d.|...
-000002b0: 9d02 a101 0100 6408 7407 6a0b 1b00 7c04  ......d.t.j...|.
-000002c0: 6401 6401 8502 6401 6602 1900 7c07 640c  d.d...d.f...|.d.
-000002d0: 1300 7c04 6401 6401 8502 6401 6602 1900  ..|.d.d...d.f...
-000002e0: 640c 1300 1700 1b00 1400 7d0f 7400 a004  d.........}.t...
+000002b0: 9d02 a101 0100 640c 7c04 6401 6401 8502  ......d.|.d.d...
+000002c0: 6401 6602 1900 1400 7407 6a0b 7c07 1400  d.f.....t.j.|...
+000002d0: 640c 1300 7c04 6401 6401 8502 6401 6602  d...|.d.d...d.f.
+000002e0: 1900 640c 1300 1700 1b00 7d0f 7400 a004  ..d.......}.t...
 000002f0: 7405 6a06 a101 9002 7224 7400 a001 6413  t.j.....r$t...d.
 00000300: 7c0f 9b00 9d02 a101 0100 7c0d 7c0e 1400  |.........|.|...
 00000310: 7c0f 1400 5300 2914 fa22 0a09 4e6f 2065  |...S.).."..No e
 00000320: 7272 6f72 2063 6f72 7265 6374 696f 6e20  rror correction 
 00000330: 6865 7265 2062 6162 792e 0a09 4e72 0100  here baby...Nr..
 00000340: 0000 e903 0000 00e9 0600 0000 fa04 7073  ..............ps
 00000350: 3a20 fa04 7373 3a20 fa04 7773 3a20 e901  : ..ss: ..ws: ..
@@ -73,26 +73,26 @@
 00000480: da08 6469 6666 7365 7331 da08 6469 6666  ..diffses1..diff
 00000490: 7365 7332 da06 6e6f 726d 7331 da06 6e6f  ses2..norms1..no
 000004a0: 726d 7332 da08 616c 7068 7365 7331 da08  rms2..alphses1..
 000004b0: 616c 7068 7365 7332 da04 6273 6573 a900  alphses2..bses..
 000004c0: 7232 0000 00fa 5a2f 686f 6d65 2f6a 656e  r2....Z/home/jen
 000004d0: 6b69 6e73 2f61 6765 6e74 2f77 6f72 6b73  kins/agent/works
 000004e0: 7061 6365 2f67 6974 6561 2d70 6879 7369  pace/gitea-physi
-000004f0: 6373 5f70 646d 655f 312e 302e 302f 7064  cs_pdme_1.0.0/pd
+000004f0: 6373 5f70 646d 655f 312e 312e 302f 7064  cs_pdme_1.1.0/pd
 00000500: 6d65 2f75 7469 6c2f 6661 7374 5f6e 6f6e  me/util/fast_non
 00000510: 6c6f 6361 6c5f 7370 6563 7472 756d 2e70  local_spectrum.p
 00000520: 79da 0f66 6173 745f 735f 6e6f 6e6c 6f63  y..fast_s_nonloc
 00000530: 616c 0800 0000 733e 0000 0000 0614 0114  al....s>........
 00000540: 0110 0210 0110 0110 0216 0116 0112 0112  ................
 00000550: 020c 010e 0214 0114 010e 0110 0110 0214  ................
 00000560: 0114 010e 0110 0110 0212 0112 010e 0110  ................
 00000570: 0110 0236 010e 0110 0272 3400 0000 2903  ...6.....r4...).
 00000580: 7202 0000 00da 0964 6970 6f6c 6573 6573  r......dipoleses
 00000590: 7204 0000 0063 0200 0000 0000 0000 0000  r....c..........
-000005a0: 0000 1000 0000 0800 0000 4300 0000 73a0  ..........C...s.
+000005a0: 0000 1000 0000 0700 0000 4300 0000 73a0  ..........C...s.
 000005b0: 0200 007c 0164 0164 0185 0264 0164 0185  ...|.d.d...d.d..
 000005c0: 0264 0264 0385 0266 0319 007d 027c 0164  .d.d...f...}.|.d
 000005d0: 0164 0185 0264 0164 0185 0264 0364 0485  .d...d.d...d.d..
 000005e0: 0266 0319 007d 037c 0164 0164 0185 0264  .f...}.|.d.d...d
 000005f0: 0164 0185 0264 0466 0319 007d 0474 00a0  .d...d.f...}.t..
 00000600: 0164 057c 029b 009d 02a1 0101 0074 00a0  .d.|.........t..
 00000610: 0164 067c 039b 009d 02a1 0101 0074 00a0  .d.|.........t..
@@ -117,20 +117,20 @@
 00000740: 06a1 0190 0172 b474 00a0 0164 0d7c 0b9b  .....r.t...d.|..
 00000750: 009d 02a1 0101 0074 00a0 0164 0e7c 0c9b  .......t...d.|..
 00000760: 009d 02a1 0101 0074 07a0 0a64 0f7c 097c  .......t...d.|.|
 00000770: 02a1 037c 0b1b 007d 0d74 07a0 0a64 0f7c  ...|...}.t...d.|
 00000780: 0a7c 02a1 037c 0c1b 007d 0e74 00a0 0474  .|...|...}.t...t
 00000790: 056a 06a1 0190 0272 0674 00a0 0164 107c  .j.....r.t...d.|
 000007a0: 0d9b 009d 02a1 0101 0074 00a0 0164 117c  .........t...d.|
-000007b0: 0e9b 009d 02a1 0101 0064 0874 076a 0b1b  .........d.t.j..
-000007c0: 007c 0464 0164 0185 0264 0164 0164 0185  .|.d.d...d.d.d..
-000007d0: 0266 0319 007c 0764 0164 0185 0264 0166  .f...|.d.d...d.f
-000007e0: 0219 0064 1213 007c 0464 0164 0185 0264  ...d...|.d.d...d
-000007f0: 0164 0164 0185 0266 0319 0064 1213 0017  .d.d...f...d....
-00000800: 001b 0014 007d 0f74 00a0 0474 056a 06a1  .....}.t...t.j..
+000007b0: 0e9b 009d 02a1 0101 0064 127c 0464 0164  .........d.|.d.d
+000007c0: 0185 0264 0164 0164 0185 0266 0319 0014  ...d.d.d...f....
+000007d0: 0074 076a 0b7c 0764 0164 0185 0264 0166  .t.j.|.d.d...d.f
+000007e0: 0219 0014 0064 1213 007c 0464 0164 0185  .....d...|.d.d..
+000007f0: 0264 0164 0164 0185 0266 0319 0064 1213  .d.d.d...f...d..
+00000800: 0017 001b 007d 0f74 00a0 0474 056a 06a1  .....}.t...t.j..
 00000810: 0190 0272 7274 00a0 0164 137c 0f9b 009d  ...rrt...d.|....
 00000820: 02a1 0101 0074 00a0 0164 147c 0d7c 0e14  .....t...d.|.|..
 00000830: 007c 0f14 009b 0064 159d 03a1 0101 0074  .|.....d.......t
 00000840: 07a0 0a64 167c 0d7c 0e14 007c 0f14 00a1  ...d.|.|...|....
 00000850: 0253 0029 1772 0500 0000 4e72 0100 0000  .S.).r....Nr....
 00000860: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
 00000870: 0900 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
@@ -144,19 +144,19 @@
 000008f0: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
 00000900: 2700 0000 7228 0000 0072 2900 0000 722a  '...r(...r)...r*
 00000910: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
 00000920: 0000 722e 0000 0072 2f00 0000 7230 0000  ..r....r/...r0..
 00000930: 0072 3100 0000 7232 0000 0072 3200 0000  .r1...r2...r2...
 00000940: 7233 0000 00da 1966 6173 745f 735f 6e6f  r3.....fast_s_no
 00000950: 6e6c 6f63 616c 5f64 6970 6f6c 6573 6573  nlocal_dipoleses
-00000960: 3700 0000 7340 0000 0000 061a 011a 0116  7...s@..........
-00000970: 0210 0110 0110 0216 0116 0112 0112 020c  ................
-00000980: 010e 0226 0126 010e 0110 0110 0214 0114  ...&.&..........
-00000990: 010e 0110 0110 0212 0112 010e 0110 0110  ................
-000009a0: 024e 010e 0110 021a 0172 3b00 0000 6302  .N.......r;...c.
+00000960: 3700 0000 7340 0000 0000 111a 011a 0216  7...s@..........
+00000970: 0210 0110 0110 0416 0116 0212 0112 020c  ................
+00000980: 010e 0726 0126 010e 0110 0110 0414 0114  ...&.&..........
+00000990: 010e 0110 0110 0812 0112 010e 0110 0110  ................
+000009a0: 074e 010e 0110 031a 0172 3b00 0000 6302  .N.......r;...c.
 000009b0: 0000 0000 0000 0000 0000 0010 0000 000a  ................
 000009c0: 0000 0043 0000 0073 4803 0000 7c01 6401  ...C...sH...|.d.
 000009d0: 6401 8502 6401 6401 8502 6402 6403 8502  d...d.d...d.d...
 000009e0: 6603 1900 7d02 7c01 6401 6401 8502 6401  f...}.|.d.d...d.
 000009f0: 6401 8502 6403 6404 8502 6603 1900 7d03  d...d.d...f...}.
 00000a00: 7c01 6401 6401 8502 6401 6401 8502 6404  |.d.d...d.d...d.
 00000a10: 6603 1900 7d04 7400 a001 6405 7c02 9b00  f...}.t...d.|...
@@ -170,93 +170,92 @@
 00000a90: 6603 1900 7d08 7c07 7c08 6b03 a002 a100  f...}.|.|.k.....
 00000aa0: 72e4 7403 6409 7c00 9b00 9d02 8301 8201  r.t.d.|.........
 00000ab0: 7c05 6401 6401 8502 6401 6602 1900 7c03  |.d.d...d.f...|.
 00000ac0: 6401 6401 8502 6401 6401 6401 8502 6603  d.d...d.d.d...f.
 00000ad0: 1900 1800 7d09 7c06 6401 6401 8502 6401  ....}.|.d.d...d.
 00000ae0: 6602 1900 7c03 6401 6401 8502 6401 6401  f...|.d.d...d.d.
 00000af0: 6401 8502 6603 1900 1800 7d0a 7400 a004  d...f.....}.t...
-00000b00: 7405 6a06 a101 9001 725e 7400 a007 640a  t.j.....r^t...d.
-00000b10: 7c09 9b00 9d02 a101 0100 7400 a007 640b  |.........t...d.
-00000b20: 7c0a 9b00 9d02 a101 0100 7408 6a09 6a0a  |.........t.j.j.
-00000b30: 7c09 6403 640c 8d02 7d0b 7408 6a09 6a0a  |.d.d...}.t.j.j.
+00000b00: 7405 6a06 a101 9001 725e 7400 a001 640a  t.j.....r^t...d.
+00000b10: 7c09 9b00 9d02 a101 0100 7400 a001 640b  |.........t...d.
+00000b20: 7c0a 9b00 9d02 a101 0100 7407 6a08 6a09  |.........t.j.j.
+00000b30: 7c09 6403 640c 8d02 7d0b 7407 6a08 6a09  |.d.d...}.t.j.j.
 00000b40: 7c0a 6403 640c 8d02 7d0c 7400 a004 7405  |.d.d...}.t...t.
-00000b50: 6a06 a101 9001 72ac 7400 a007 640d 7c0b  j.....r.t...d.|.
-00000b60: 9b00 9d02 a101 0100 7400 a007 640e 7c0c  ........t...d.|.
-00000b70: 9b00 9d02 a101 0100 6403 7408 a00b 7408  ........d.t...t.
-00000b80: a00b 7408 a00c 640f 7c09 7c02 a103 7c0b  ..t...d.|.|...|.
-00000b90: 6410 1300 1b00 a101 7408 a00b 7c09 a101  d.......t...|...
+00000b50: 6a06 a101 9001 72ac 7400 a001 640d 7c0b  j.....r.t...d.|.
+00000b60: 9b00 9d02 a101 0100 7400 a001 640e 7c0c  ........t...d.|.
+00000b70: 9b00 9d02 a101 0100 6403 7407 a00a 7407  ........d.t...t.
+00000b80: a00a 7407 a00b 640f 7c09 7c02 a103 7c0b  ..t...d.|.|...|.
+00000b90: 6410 1300 1b00 a101 7407 a00a 7c09 a101  d.......t...|...
 00000ba0: 1400 a101 6401 6401 8502 6401 6401 8502  ....d.d...d.d...
 00000bb0: 6401 6401 8502 6402 6604 1900 1400 7c02  d.d...d.f.....|.
-00000bc0: 6401 6401 8502 7408 6a0d 6401 6401 8502  d.d...t.j.d.d...
+00000bc0: 6401 6401 8502 7407 6a0c 6401 6401 8502  d.d...t.j.d.d...
 00000bd0: 6402 6604 1900 1800 7c0b 6403 1300 1b00  d.f.....|.d.....
-00000be0: 7d0d 6403 7408 a00b 7408 a00b 7408 a00c  }.d.t...t...t...
+00000be0: 7d0d 6403 7407 a00a 7407 a00a 7407 a00b  }.d.t...t...t...
 00000bf0: 640f 7c0a 7c02 a103 7c0c 6410 1300 1b00  d.|.|...|.d.....
-00000c00: a101 7408 a00b 7c0a a101 1400 a101 6401  ..t...|.......d.
+00000c00: a101 7407 a00a 7c0a a101 1400 a101 6401  ..t...|.......d.
 00000c10: 6401 8502 6401 6401 8502 6401 6401 8502  d...d.d...d.d...
 00000c20: 6402 6604 1900 1400 7c02 6401 6401 8502  d.f.....|.d.d...
-00000c30: 7408 6a0d 6401 6401 8502 6402 6604 1900  t.j.d.d...d.f...
+00000c30: 7407 6a0c 6401 6401 8502 6402 6604 1900  t.j.d.d...d.f...
 00000c40: 1800 7c0c 6403 1300 1b00 7d0e 7400 a004  ..|.d.....}.t...
-00000c50: 7405 6a06 a101 9002 72ae 7400 a007 6411  t.j.....r.t...d.
-00000c60: 7c0d 9b00 9d02 a101 0100 7400 a007 6412  |.........t...d.
-00000c70: 7c0e 9b00 9d02 a101 0100 6408 7408 6a0e  |.........d.t.j.
-00000c80: 1b00 7c04 6401 6401 8502 6401 6401 6401  ..|.d.d...d.d.d.
-00000c90: 8502 6603 1900 7c07 6401 6401 8502 6401  ..f...|.d.d...d.
-00000ca0: 6602 1900 6410 1300 7c04 6401 6401 8502  f...d...|.d.d...
-00000cb0: 6401 6401 6401 8502 6603 1900 6410 1300  d.d.d...f...d...
-00000cc0: 1700 1b00 1400 7d0f 7400 a004 7405 6a06  ......}.t...t.j.
-00000cd0: a101 9003 721a 7400 a007 6413 7c0f 9b00  ....r.t...d.|...
-00000ce0: 9d02 a101 0100 7400 a007 6414 7c0d 7c0e  ......t...d.|.|.
+00000c50: 7405 6a06 a101 9002 72ae 7400 a001 6411  t.j.....r.t...d.
+00000c60: 7c0d 9b00 9d02 a101 0100 7400 a001 6412  |.........t...d.
+00000c70: 7c0e 9b00 9d02 a101 0100 6410 7c04 6401  |.........d.|.d.
+00000c80: 6401 8502 6401 6401 6401 8502 6603 1900  d...d.d.d...f...
+00000c90: 1400 7407 6a0d 7c07 6401 6401 8502 6401  ..t.j.|.d.d...d.
+00000ca0: 6602 1900 1400 6410 1300 7c04 6401 6401  f.....d...|.d.d.
+00000cb0: 8502 6401 6401 6401 8502 6603 1900 6410  ..d.d.d...f...d.
+00000cc0: 1300 1700 1b00 7d0f 7400 a004 7405 6a06  ......}.t...t.j.
+00000cd0: a101 9003 721a 7400 a001 6413 7c0f 9b00  ....r.t...d.|...
+00000ce0: 9d02 a101 0100 7400 a001 6414 7c0d 7c0e  ......t...d.|.|.
 00000cf0: 1400 7c0f 1400 9b00 6415 9d03 a101 0100  ..|.....d.......
-00000d00: 7408 a00c 6416 7c0d 7c0e 1400 7c0f 1400  t...d.|.|...|...
+00000d00: 7407 a00b 6416 7c0d 7c0e 1400 7c0f 1400  t...d.|.|...|...
 00000d10: a102 5300 2917 7205 0000 004e 7201 0000  ..S.).r....Nr...
 00000d20: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
 00000d30: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
 00000d40: 0c00 0000 720d 0000 0072 0e00 0000 7210  ....r....r....r.
 00000d50: 0000 0072 1200 0000 7213 0000 0072 3600  ...r....r....r6.
 00000d60: 0000 720f 0000 0072 1400 0000 7215 0000  ..r....r....r...
 00000d70: 0072 1600 0000 7237 0000 0072 3800 0000  .r....r7...r8...
-00000d80: 7239 0000 0029 0f72 1800 0000 7219 0000  r9...).r....r...
+00000d80: 7239 0000 0029 0e72 1800 0000 7219 0000  r9...).r....r...
 00000d90: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000da0: 721d 0000 0072 1e00 0000 da07 7761 726e  r....r......warn
-00000db0: 696e 6772 1f00 0000 7220 0000 0072 2100  ingr....r ...r!.
-00000dc0: 0000 da09 7472 616e 7370 6f73 6572 2200  ....transposer".
-00000dd0: 0000 da07 6e65 7761 7869 7372 2300 0000  ....newaxisr#...
-00000de0: 723a 0000 0072 3200 0000 7232 0000 0072  r:...r2...r2...r
-00000df0: 3300 0000 da2c 6661 7374 5f73 5f73 7069  3....,fast_s_spi
-00000e00: 6e5f 7175 6269 745f 7461 7275 6368 615f  n_qubit_tarucha_
-00000e10: 6e6f 6e6c 6f63 616c 5f64 6970 6f6c 6573  nonlocal_dipoles
-00000e20: 6573 6700 0000 7378 0000 0000 101a 021a  esg...sx........
-00000e30: 0216 0210 0110 0110 0616 0116 0212 0112  ................
-00000e40: 020c 010e 0c26 0126 010e 0110 0110 0310  .....&.&........
-00000e50: 0110 010e 0110 0110 2002 0104 0104 0114  ........ .......
-00000e60: ff02 0308 fd02 ff02 0516 fb02 ff02 0818  ................
-00000e70: f702 0a06 f504 0e02 0104 0104 0114 ff02  ................
-00000e80: 0308 fd02 ff02 0516 fb02 ff02 0818 f702  ................
-00000e90: 0a06 f504 0c0e 0110 0110 024e 010e 0110  ...........N....
-00000ea0: 021a 0172 3f00 0000 6301 0000 0000 0000  ...r?...c.......
-00000eb0: 0000 0000 0002 0000 0005 0000 004b 0000  .............K..
-00000ec0: 0073 2000 0000 7400 6a01 7400 6a02 7c00  .s ...t.j.t.j.|.
-00000ed0: 6601 6900 7c01 a401 8e01 6401 1800 1400  f.i.|.....d.....
-00000ee0: 6402 1b00 5300 2903 7a94 0a09 7573 6573  d...S.).z...uses
-00000ef0: 206e 756d 7079 2e73 6967 6e20 746f 2069   numpy.sign to i
-00000f00: 6d70 6c65 6d65 6e74 2041 7267 2066 6f72  mplement Arg for
-00000f10: 2072 6561 6c20 6e75 6d62 6572 7320 6f6e   real numbers on
-00000f20: 6c79 2e20 5368 6f75 6c64 2072 6574 7572  ly. Should retur
-00000f30: 6e20 7069 2066 6f72 206e 6567 6174 6976  n pi for negativ
-00000f40: 6520 696e 7075 7473 2c20 3020 666f 7220  e inputs, 0 for 
-00000f50: 706f 7369 7469 7665 2e0a 0950 6173 7365  positive...Passe
-00000f60: 7320 7468 726f 7567 6820 6172 6773 2074  s through args t
-00000f70: 6f20 6e75 6d70 792e 7369 676e 0a09 720b  o numpy.sign..r.
-00000f80: 0000 00e9 feff ffff 2903 721f 0000 0072  ........).r....r
-00000f90: 2300 0000 da04 7369 676e 2902 da01 78da  #.....sign)...x.
-00000fa0: 066b 7761 7267 7372 3200 0000 7232 0000  .kwargsr2...r2..
-00000fb0: 0072 3300 0000 da07 7369 676e 6172 67e5  .r3.....signarg.
-00000fc0: 0000 0073 0200 0000 0005 7244 0000 0029  ...s......rD...)
-00000fd0: 0a72 1f00 0000 721d 0000 00da 0967 6574  .r....r......get
-00000fe0: 4c6f 6767 6572 da08 5f5f 6e61 6d65 5f5f  Logger..__name__
-00000ff0: 7218 0000 00da 076e 6461 7272 6179 7234  r......ndarrayr4
-00001000: 0000 0072 3b00 0000 723f 0000 0072 4400  ...r;...r?...rD.
-00001010: 0000 7232 0000 0072 3200 0000 7232 0000  ..r2...r2...r2..
-00001020: 0072 3300 0000 da08 3c6d 6f64 756c 653e  .r3.....<module>
-00001030: 0100 0000 7318 0000 0008 0108 030a 0408  ....s...........
-00001040: 0104 fe0c 3008 0104 fe0c 3108 0104 fe0c  ....0.....1.....
-00001050: 7e                                       ~
+00000da0: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000db0: 2000 0000 7221 0000 00da 0974 7261 6e73   ...r!.....trans
+00000dc0: 706f 7365 7222 0000 00da 076e 6577 6178  poser".....newax
+00000dd0: 6973 7223 0000 0072 3a00 0000 7232 0000  isr#...r:...r2..
+00000de0: 0072 3200 0000 7233 0000 00da 2c66 6173  .r2...r3....,fas
+00000df0: 745f 735f 7370 696e 5f71 7562 6974 5f74  t_s_spin_qubit_t
+00000e00: 6172 7563 6861 5f6e 6f6e 6c6f 6361 6c5f  arucha_nonlocal_
+00000e10: 6469 706f 6c65 7365 7389 0000 0073 7800  dipoleses....sx.
+00000e20: 0000 0010 1a02 1a02 1602 1001 1001 1006  ................
+00000e30: 1601 1602 1201 1202 0c01 0e0c 2601 2601  ............&.&.
+00000e40: 0e01 1001 1003 1001 1001 0e01 1001 1020  ............... 
+00000e50: 0201 0401 0401 14ff 0203 08fd 02ff 0205  ................
+00000e60: 16fb 02ff 0208 18f7 020a 06f5 040e 0201  ................
+00000e70: 0401 0401 14ff 0203 08fd 02ff 0205 16fb  ................
+00000e80: 02ff 0208 18f7 020a 06f5 040c 0e01 1001  ................
+00000e90: 1002 4e01 0e01 1002 1a01 723e 0000 0063  ..N.......r>...c
+00000ea0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000eb0: 0500 0000 4b00 0000 7320 0000 0074 006a  ....K...s ...t.j
+00000ec0: 0174 006a 027c 0066 0169 007c 01a4 018e  .t.j.|.f.i.|....
+00000ed0: 0164 0118 0014 0064 021b 0053 0029 037a  .d.....d...S.).z
+00000ee0: 940a 0975 7365 7320 6e75 6d70 792e 7369  ...uses numpy.si
+00000ef0: 676e 2074 6f20 696d 706c 656d 656e 7420  gn to implement 
+00000f00: 4172 6720 666f 7220 7265 616c 206e 756d  Arg for real num
+00000f10: 6265 7273 206f 6e6c 792e 2053 686f 756c  bers only. Shoul
+00000f20: 6420 7265 7475 726e 2070 6920 666f 7220  d return pi for 
+00000f30: 6e65 6761 7469 7665 2069 6e70 7574 732c  negative inputs,
+00000f40: 2030 2066 6f72 2070 6f73 6974 6976 652e   0 for positive.
+00000f50: 0a09 5061 7373 6573 2074 6872 6f75 6768  ..Passes through
+00000f60: 2061 7267 7320 746f 206e 756d 7079 2e73   args to numpy.s
+00000f70: 6967 6e0a 0972 0b00 0000 e9fe ffff ff29  ign..r.........)
+00000f80: 0372 1f00 0000 7223 0000 00da 0473 6967  .r....r#.....sig
+00000f90: 6e29 02da 0178 da06 6b77 6172 6773 7232  n)...x..kwargsr2
+00000fa0: 0000 0072 3200 0000 7233 0000 00da 0773  ...r2...r3.....s
+00000fb0: 6967 6e61 7267 0701 0000 7302 0000 0000  ignarg....s.....
+00000fc0: 0572 4300 0000 290a 721f 0000 0072 1d00  .rC...).r....r..
+00000fd0: 0000 da09 6765 744c 6f67 6765 72da 085f  ....getLogger.._
+00000fe0: 5f6e 616d 655f 5f72 1800 0000 da07 6e64  _name__r......nd
+00000ff0: 6172 7261 7972 3400 0000 723b 0000 0072  arrayr4...r;...r
+00001000: 3e00 0000 7243 0000 0072 3200 0000 7232  >...rC...r2...r2
+00001010: 0000 0072 3200 0000 7233 0000 00da 083c  ...r2...r3.....<
+00001020: 6d6f 6475 6c65 3e01 0000 0073 1800 0000  module>....s....
+00001030: 0801 0803 0a04 0801 04fe 0c30 0801 04fe  ...........0....
+00001040: 0c53 0801 04fe 0c7e                      .S.....~
```

### Comparing `pdme-1.0.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc` & `pdme-1.1.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 29 02:29:58 2024 UTC, .py size: 3604 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 610d 0d0a 0000 0000 2606 2f66 140e 0000  a.......&./f....
+00000000: 610d 0d0a 0000 0000 9a1c 3466 7b0e 0000  a.........4f{...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6501  d.l.Z.d.d.l.Z.e.
 00000040: a002 6503 a101 5a04 6500 6a05 6500 6a05  ..e...Z.e.j.e.j.
 00000050: 6500 6a05 6402 9c03 6403 6404 8404 5a06  e.j.d...d.d...Z.
 00000060: 6500 6a05 6500 6a05 6500 6a05 6405 9c03  e.j.e.j.e.j.d...
 00000070: 6406 6407 8404 5a07 6500 6a05 6500 6a05  d.d...Z.e.j.e.j.
 00000080: 6500 6a05 6500 6a05 6408 9c04 6409 640a  e.j.e.j.d...d.d.
 00000090: 8404 5a08 6500 6a05 6500 6a05 6500 6a05  ..Z.e.j.e.j.e.j.
 000000a0: 6500 6a05 640b 9c04 640c 640d 8404 5a09  e.j.d...d.d...Z.
 000000b0: 6401 5300 290e e900 0000 004e 2903 da0a  d.S.)......N)...
 000000c0: 646f 745f 696e 7075 7473 da07 6469 706f  dot_inputs..dipo
 000000d0: 6c65 73da 0672 6574 7572 6e63 0200 0000  les..returnc....
-000000e0: 0000 0000 0000 0000 0b00 0000 0600 0000  ................
+000000e0: 0000 0000 0000 0000 0b00 0000 0500 0000  ................
 000000f0: 4300 0000 7348 0100 007c 0164 0164 0185  C...sH...|.d.d..
 00000100: 0264 0264 0385 0266 0219 007d 027c 0164  .d.d...f...}.|.d
 00000110: 0164 0185 0264 0364 0485 0266 0219 007d  .d...d.d...f...}
 00000120: 037c 0164 0164 0185 0264 0466 0219 007d  .|.d.d...d.f...}
 00000130: 0474 00a0 0164 057c 029b 009d 02a1 0101  .t...d.|........
 00000140: 0074 00a0 0164 067c 039b 009d 02a1 0101  .t...d.|........
 00000150: 0074 00a0 0164 077c 049b 009d 02a1 0101  .t...d.|........
@@ -25,216 +25,222 @@
 00000180: 0219 007d 067c 057c 0364 0164 0185 0264  ...}.|.|.d.d...d
 00000190: 0166 0219 0018 007d 0774 00a0 0164 087c  .f.....}.t...d.|
 000001a0: 079b 009d 02a1 0101 0074 026a 036a 047c  .........t.j.j.|
 000001b0: 0764 0964 0a8d 0264 0313 007d 0874 00a0  .d.d...d...}.t..
 000001c0: 0164 0b7c 089b 009d 02a1 0101 0074 02a0  .d.|.........t..
 000001d0: 0564 0c7c 077c 02a1 037c 081b 0064 0913  .d.|.|...|...d..
 000001e0: 007d 0974 00a0 0164 0d7c 099b 009d 02a1  .}.t...d.|......
-000001f0: 0101 0064 0e74 026a 061b 007c 0464 0164  ...d.t.j...|.d.d
-00000200: 0185 0264 0166 0219 007c 0664 0913 007c  ...d.f...|.d...|
-00000210: 0464 0164 0185 0264 0166 0219 0064 0913  .d.d...d.f...d..
-00000220: 0017 001b 0014 007d 0a74 00a0 0164 0f7c  .......}.t...d.|
+000001f0: 0101 0064 097c 0464 0164 0185 0264 0166  ...d.|.d.d...d.f
+00000200: 0219 0014 0074 026a 067c 0614 0064 0913  .....t.j.|...d..
+00000210: 007c 0464 0164 0185 0264 0166 0219 0064  .|.d.d...d.f...d
+00000220: 0913 0017 001b 007d 0a74 00a0 0164 0e7c  .......}.t...d.|
 00000230: 0a9b 009d 02a1 0101 007c 097c 0a14 0053  .........|.|...S
-00000240: 0029 107a 990a 094e 6f20 6572 726f 7220  .).z...No error 
+00000240: 0029 0f7a 990a 094e 6f20 6572 726f 7220  .).z...No error 
 00000250: 636f 7272 6563 7469 6f6e 2068 6572 6520  correction here 
 00000260: 6261 6279 2e0a 0945 7870 6563 7473 2064  baby...Expects d
 00000270: 6f74 5f69 6e70 7574 7320 746f 2062 6520  ot_inputs to be 
 00000280: 6e75 6d70 7920 6172 7261 7920 6f66 205b  numpy array of [
 00000290: 7278 2c20 7279 2c20 727a 2c20 665d 2065  rx, ry, rz, f] e
 000002a0: 6e74 7269 6573 2c20 736f 2061 206e 2062  ntries, so a n b
 000002b0: 7920 3420 7768 6572 6520 6e20 6973 206e  y 4 where n is n
 000002c0: 756d 6265 7220 6f66 206d 6561 7375 7265  umber of measure
 000002d0: 6d65 6e74 2070 6f69 6e74 732e 0a09 4e72  ment points...Nr
 000002e0: 0100 0000 e903 0000 00e9 0600 0000 fa04  ................
 000002f0: 7073 3a20 fa04 7373 3a20 fa04 7773 3a20  ps: ..ss: ..ws: 
 00000300: fa09 6469 6666 7365 733a 20e9 0200 0000  ..diffses: .....
 00000310: a901 da04 6178 6973 fa07 6e6f 726d 733a  ....axis..norms:
 00000320: 207a 0b2e 2e2e 6a69 2c20 2e2e 2e69 fa06   z....ji, ...i..
-00000330: 6173 6573 3a20 e901 0000 00fa 0662 7365  ases: .......bse
-00000340: 733a 20a9 07da 075f 6c6f 6767 6572 da05  s: ...._logger..
-00000350: 6465 6275 67da 056e 756d 7079 da06 6c69  debug..numpy..li
-00000360: 6e61 6c67 da04 6e6f 726d da06 6569 6e73  nalg..norm..eins
-00000370: 756d da02 7069 290b 7202 0000 0072 0300  um..pi).r....r..
-00000380: 0000 da02 7073 da02 7373 da02 7773 da02  ....ps..ss..ws..
-00000390: 7273 da02 6673 da07 6469 6666 7365 73da  rs..fs..diffses.
-000003a0: 056e 6f72 6d73 da04 6173 6573 da04 6273  .norms..ases..bs
-000003b0: 6573 a900 7223 0000 00fa 4f2f 686f 6d65  es..r#....O/home
-000003c0: 2f6a 656e 6b69 6e73 2f61 6765 6e74 2f77  /jenkins/agent/w
-000003d0: 6f72 6b73 7061 6365 2f67 6974 6561 2d70  orkspace/gitea-p
-000003e0: 6879 7369 6373 5f70 646d 655f 312e 302e  hysics_pdme_1.0.
-000003f0: 302f 7064 6d65 2f75 7469 6c2f 6661 7374  0/pdme/util/fast
-00000400: 5f76 5f63 616c 632e 7079 da13 6661 7374  _v_calc.py..fast
-00000410: 5f76 735f 666f 725f 6469 706f 6c65 7308  _vs_for_dipoles.
-00000420: 0000 0073 2200 0000 0007 1401 1401 1002  ...s"...........
-00000430: 1001 1001 1002 1401 1002 1402 1001 1401  ................
-00000440: 1001 1601 1002 3601 1001 7225 0000 0029  ......6...r%...)
-00000450: 0372 0200 0000 da09 6469 706f 6c65 7365  .r......dipolese
-00000460: 7372 0400 0000 6302 0000 0000 0000 0000  sr....c.........
-00000470: 0000 000b 0000 0008 0000 0043 0000 0073  ...........C...s
-00000480: 8c01 0000 7c01 6401 6401 8502 6401 6401  ....|.d.d...d.d.
-00000490: 8502 6402 6403 8502 6603 1900 7d02 7c01  ..d.d...f...}.|.
-000004a0: 6401 6401 8502 6401 6401 8502 6403 6404  d.d...d.d...d.d.
-000004b0: 8502 6603 1900 7d03 7c01 6401 6401 8502  ..f...}.|.d.d...
-000004c0: 6401 6401 8502 6404 6603 1900 7d04 7400  d.d...d.f...}.t.
-000004d0: a001 6405 7c02 9b00 9d02 a101 0100 7400  ..d.|.........t.
-000004e0: a001 6406 7c03 9b00 9d02 a101 0100 7400  ..d.|.........t.
-000004f0: a001 6407 7c04 9b00 9d02 a101 0100 7c00  ..d.|.........|.
-00000500: 6401 6401 8502 6402 6403 8502 6602 1900  d.d...d.d...f...
-00000510: 7d05 7c00 6401 6401 8502 6403 6602 1900  }.|.d.d...d.f...
-00000520: 7d06 7c05 6401 6401 8502 6401 6602 1900  }.|.d.d...d.f...
-00000530: 7c03 6401 6401 8502 6401 6401 6401 8502  |.d.d...d.d.d...
-00000540: 6603 1900 1800 7d07 7400 a001 6408 7c07  f.....}.t...d.|.
-00000550: 9b00 9d02 a101 0100 7402 6a03 6a04 7c07  ........t.j.j.|.
-00000560: 6403 6409 8d02 6403 1300 7d08 7400 a001  d.d...d...}.t...
-00000570: 640a 7c08 9b00 9d02 a101 0100 7402 a005  d.|.........t...
-00000580: 640b 7c07 7c02 a103 7c08 1b00 640c 1300  d.|.|...|...d...
-00000590: 7d09 7400 a001 640d 7c09 9b00 9d02 a101  }.t...d.|.......
-000005a0: 0100 640e 7402 6a06 1b00 7c04 6401 6401  ..d.t.j...|.d.d.
-000005b0: 8502 6401 6401 6401 8502 6603 1900 7c06  ..d.d.d...f...|.
-000005c0: 6401 6401 8502 6401 6602 1900 640c 1300  d.d...d.f...d...
-000005d0: 7c04 6401 6401 8502 6401 6401 6401 8502  |.d.d...d.d.d...
-000005e0: 6603 1900 640c 1300 1700 1b00 1400 7d0a  f...d.........}.
-000005f0: 7400 a001 640f 7c0a 9b00 9d02 a101 0100  t...d.|.........
-00000600: 7402 a005 6410 7c09 7c0a 1400 a102 5300  t...d.|.|.....S.
-00000610: 2911 6128 0100 000a 094e 6f20 6572 726f  ).a(.....No erro
-00000620: 7220 636f 7272 6563 7469 6f6e 2068 6572  r correction her
-00000630: 6520 6261 6279 2e0a 0945 7870 6563 7473  e baby...Expects
-00000640: 2064 6f74 5f69 6e70 7574 7320 746f 2062   dot_inputs to b
-00000650: 6520 6e75 6d70 7920 6172 7261 7920 6f66  e numpy array of
-00000660: 205b 7278 2c20 7279 2c20 727a 2c20 665d   [rx, ry, rz, f]
-00000670: 2065 6e74 7269 6573 2c20 736f 2061 206e   entries, so a n
-00000680: 2062 7920 3420 7768 6572 6520 6e20 6973   by 4 where n is
-00000690: 206e 756d 6265 7220 6f66 206d 6561 7375   number of measu
-000006a0: 7265 6d65 6e74 2070 6f69 6e74 732e 0a0a  rement points...
-000006b0: 0944 6970 6f6c 6573 6573 2061 7265 2065  .Dipoleses are e
-000006c0: 7870 6563 7465 6420 746f 2062 6520 6172  xpected to be ar
-000006d0: 7261 7920 6f66 2061 7272 6179 7320 6f66  ray of arrays of
-000006e0: 2061 7272 6179 733a 206c 6973 7420 6f66   arrays: list of
-000006f0: 2073 6574 7320 6f66 2064 6970 6f6c 6573   sets of dipoles
-00000700: 2077 6869 6368 2061 7265 2070 6172 7420   which are part 
-00000710: 6f66 2061 2073 696e 676c 6520 6172 7261  of a single arra
-00000720: 6e67 656d 656e 7420 746f 2062 6520 6164  ngement to be ad
-00000730: 6465 6420 746f 6765 7468 6572 2e0a 094e  ded together...N
-00000740: 7201 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
-00000750: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
-00000760: 0000 0072 0c00 0000 720e 0000 00fa 0d61  ...r....r......a
-00000770: 6263 642c 6163 642d 3e61 6263 720b 0000  bcd,acd->abcr...
-00000780: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000790: fa09 2e2e 2e6a 2d3e 2e2e 2e72 1200 0000  .....j->...r....
-000007a0: 290b 7202 0000 0072 2600 0000 721a 0000  ).r....r&...r...
-000007b0: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-000007c0: 721e 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-000007d0: 2100 0000 7222 0000 0072 2300 0000 7223  !...r"...r#...r#
-000007e0: 0000 0072 2400 0000 da15 6661 7374 5f76  ...r$.....fast_v
-000007f0: 735f 666f 725f 6469 706f 6c65 7365 7327  s_for_dipoleses'
-00000800: 0000 0073 2200 0000 0009 1a01 1a01 1602  ...s"...........
-00000810: 1001 1001 1002 1401 1002 2602 1001 1401  ..........&.....
-00000820: 1001 1601 1002 4e01 1001 7229 0000 0029  ......N...r)...)
-00000830: 0472 0200 0000 7226 0000 00da 0474 656d  .r....r&.....tem
-00000840: 7072 0400 0000 6303 0000 0000 0000 0000  pr....c.........
-00000850: 0000 0013 0000 0008 0000 0043 0000 0073  ...........C...s
-00000860: 9e01 0000 7c01 6401 6401 8502 6401 6401  ....|.d.d...d.d.
-00000870: 8502 6402 6403 8502 6603 1900 7d03 7c01  ..d.d...f...}.|.
-00000880: 6401 6401 8502 6401 6401 8502 6403 6404  d.d...d.d...d.d.
-00000890: 8502 6603 1900 7d04 7c01 6401 6401 8502  ..f...}.|.d.d...
-000008a0: 6401 6401 8502 6404 6603 1900 7d05 7c01  d.d...d.f...}.|.
-000008b0: 6401 6401 8502 6401 6401 8502 6405 6603  d.d...d.d...d.f.
-000008c0: 1900 7d06 7c01 6401 6401 8502 6401 6401  ..}.|.d.d...d.d.
-000008d0: 8502 6406 6603 1900 7d07 7c00 6401 6401  ..d.f...}.|.d.d.
-000008e0: 8502 6402 6403 8502 6602 1900 7d08 7c00  ..d.d...f...}.|.
-000008f0: 6401 6401 8502 6403 6602 1900 7d09 7c08  d.d...d.f...}.|.
-00000900: 6401 6401 8502 6401 6602 1900 7c04 6401  d.d...d.f...|.d.
-00000910: 6401 8502 6401 6401 6401 8502 6603 1900  d...d.d.d...f...
-00000920: 1800 7d0a 7400 a001 7c05 0b00 7c02 1b00  ..}.t...|...|...
-00000930: a101 7c07 1400 7d0b 7400 a001 7c06 0b00  ..|...}.t...|...
-00000940: 7c02 1b00 a101 7c07 1400 7d0c 6407 7c0b  |.....|...}.d.|.
-00000950: 7c0c 1400 7c0b 7c0c 1700 6408 1300 1b00  |...|.|...d.....
-00000960: 1400 7d0d 7c0b 7c0c 1700 7d0e 7c03 6a02  ..}.|.|...}.|.j.
-00000970: 7c0d 6a02 1400 6a02 7d0f 7400 6a03 6a04  |.j...j.}.t.j.j.
-00000980: 7c0a 6403 6409 8d02 6403 1300 7d10 7400  |.d.d...d...}.t.
-00000990: a005 640a 7c0a 7c0f a103 7c10 1b00 6408  ..d.|.|...|...d.
-000009a0: 1300 7d11 640b 7400 6a06 1b00 7c0e 6401  ..}.d.t.j...|.d.
-000009b0: 6401 8502 6401 6401 6401 8502 6603 1900  d...d.d.d...f...
-000009c0: 7c09 6401 6401 8502 6401 6602 1900 6408  |.d.d...d.f...d.
-000009d0: 1300 7c0e 6401 6401 8502 6401 6401 6401  ..|.d.d...d.d.d.
-000009e0: 8502 6603 1900 6408 1300 1700 1b00 1400  ..f...d.........
-000009f0: 7d12 7400 a005 640c 7c11 7c12 1400 a102  }.t...d.|.|.....
-00000a00: 5300 290d 61ef 0100 000a 094e 6f20 6572  S.).a......No er
-00000a10: 726f 7220 636f 7272 6563 7469 6f6e 2068  ror correction h
-00000a20: 6572 6520 6261 6279 2e0a 0945 7870 6563  ere baby...Expec
-00000a30: 7473 2064 6f74 5f69 6e70 7574 7320 746f  ts dot_inputs to
-00000a40: 2062 6520 6e75 6d70 7920 6172 7261 7920   be numpy array 
-00000a50: 6f66 205b 7278 2c20 7279 2c20 727a 2c20  of [rx, ry, rz, 
-00000a60: 665d 2065 6e74 7269 6573 2c20 736f 2061  f] entries, so a
-00000a70: 206e 2062 7920 3420 7768 6572 6520 6e20   n by 4 where n 
-00000a80: 6973 206e 756d 6265 7220 6f66 206d 6561  is number of mea
-00000a90: 7375 7265 6d65 6e74 2070 6f69 6e74 732e  surement points.
-00000aa0: 0a0a 0944 6970 6f6c 6573 6573 2061 7265  ...Dipoleses are
-00000ab0: 2065 7870 6563 7465 6420 746f 2062 6520   expected to be 
-00000ac0: 6172 7261 7920 6f66 2061 7272 6179 7320  array of arrays 
-00000ad0: 6f66 2061 7272 6179 733a 0a09 6c69 7374  of arrays:..list
-00000ae0: 206f 6620 7365 7473 206f 6620 6469 706f   of sets of dipo
-00000af0: 6c65 7320 7768 6963 6820 6172 6520 7061  les which are pa
-00000b00: 7274 206f 6620 6120 7369 6e67 6c65 2061  rt of a single a
-00000b10: 7272 616e 6765 6d65 6e74 2074 6f20 6265  rrangement to be
-00000b20: 2061 6464 6564 2074 6f67 6574 6865 722e   added together.
-00000b30: 0a09 5769 7468 696e 2065 6163 6820 6469  ..Within each di
-00000b40: 706f 6c65 2c20 7468 6520 6578 7065 6374  pole, the expect
-00000b50: 6564 2066 6f72 6d61 7420 6973 205b 7078  ed format is [px
-00000b60: 2c20 7079 2c20 707a 2c20 7378 2c20 7379  , py, pz, sx, sy
-00000b70: 2c20 737a 2c20 6531 2c20 6532 2c20 775d  , sz, e1, e2, w]
-00000b80: 0a09 5468 6520 7061 7373 6564 2069 6e20  ..The passed in 
-00000b90: 7720 6973 2065 7870 6563 7465 6420 746f  w is expected to
-00000ba0: 2062 6520 6861 6c66 2074 6865 2061 6374   be half the act
-00000bb0: 7561 6c2e 2054 6869 7320 6973 2062 6164  ual. This is bad
-00000bc0: 2c20 6275 7420 6865 7265 2066 6f72 2068  , but here for h
-00000bd0: 6973 746f 7269 6361 6c20 7265 6173 6f6e  istorical reason
-00000be0: 7320 746f 2062 6520 6368 616e 6765 6420  s to be changed 
-00000bf0: 6c61 7465 722e 0a09 4e72 0100 0000 7205  later...Nr....r.
-00000c00: 0000 0072 0600 0000 e907 0000 00e9 0800  ...r............
-00000c10: 0000 e904 0000 0072 0b00 0000 720c 0000  .......r....r...
-00000c20: 0072 2700 0000 7210 0000 0072 2800 0000  .r'...r....r(...
-00000c30: 2907 7215 0000 00da 0365 7870 da01 5472  ).r......exp..Tr
-00000c40: 1600 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
-00000c50: 0000 0029 1372 0200 0000 7226 0000 0072  ...).r....r&...r
-00000c60: 2a00 0000 5a06 7261 775f 7073 721b 0000  *...Z.raw_psr...
-00000c70: 005a 0365 3173 5a03 6532 735a 0672 6177  .Z.e1sZ.e2sZ.raw
-00000c80: 5f77 7372 1d00 0000 721e 0000 0072 1f00  _wsr....r....r..
-00000c90: 0000 5a03 7731 735a 0377 3273 5a0d 6d61  ..Z.w1sZ.w2sZ.ma
-00000ca0: 675f 7072 6566 6163 746f 7272 1c00 0000  g_prefactorr....
-00000cb0: 721a 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
-00000cc0: 2200 0000 7223 0000 0072 2300 0000 7224  "...r#...r#...r$
-00000cd0: 0000 00da 2066 6173 745f 7673 5f66 6f72  .... fast_vs_for
-00000ce0: 5f61 7379 6d6d 6574 7269 635f 6469 706f  _asymmetric_dipo
-00000cf0: 6c65 7365 7348 0000 0073 2200 0000 000c  lesesH...s".....
-00000d00: 1a01 1a01 1601 1601 1602 1401 1002 2602  ..............&.
-00000d10: 1401 1402 1801 0803 0e02 1402 1602 4e02  ..............N.
-00000d20: 7230 0000 0029 04da 0161 da03 6c6f 77da  r0...)...a..low.
-00000d30: 0468 6967 6872 0400 0000 6303 0000 0000  .highr....c.....
-00000d40: 0000 0000 0000 0003 0000 0006 0000 0043  ...............C
-00000d50: 0000 0073 1e00 0000 7400 6a01 7400 a002  ...s....t.j.t...
-00000d60: 7c01 7c00 6b00 7c02 7c00 6b04 a102 6401  |.|.k.|.|.k...d.
-00000d70: 6402 8d02 5300 2903 7a9d 0a09 496e 7465  d...S.).z...Inte
-00000d80: 6e64 6564 2073 7065 6369 6669 6361 6c6c  nded specificall
-00000d90: 7920 666f 7220 7468 6520 6361 7365 2077  y for the case w
-00000da0: 6865 7265 2061 2069 7320 6120 6c69 7374  here a is a list
-00000db0: 206f 6620 6172 7261 7973 2c20 616e 6420   of arrays, and 
-00000dc0: 6561 6368 2061 7272 6179 206d 7573 7420  each array must 
-00000dd0: 6265 2062 6574 7765 656e 2074 6865 2073  be between the s
-00000de0: 696e 676c 6520 6172 7261 7920 6c6f 7720  ingle array low 
-00000df0: 616e 6420 6869 6768 2c20 6275 7420 7769  and high, but wi
-00000e00: 7468 6f75 7420 6572 726f 7220 6368 6563  thout error chec
-00000e10: 6b69 6e67 2e0a 0972 1000 0000 720c 0000  king...r....r...
-00000e20: 0029 0372 1500 0000 da03 616c 6cda 0b6c  .).r......all..l
-00000e30: 6f67 6963 616c 5f61 6e64 2903 7231 0000  ogical_and).r1..
-00000e40: 0072 3200 0000 7233 0000 0072 2300 0000  .r2...r3...r#...
-00000e50: 7223 0000 0072 2400 0000 da07 6265 7477  r#...r$.....betw
-00000e60: 6565 6e71 0000 0073 0200 0000 0004 7236  eenq...s......r6
-00000e70: 0000 0029 0a72 1500 0000 da07 6c6f 6767  ...).r......logg
-00000e80: 696e 67da 0967 6574 4c6f 6767 6572 da08  ing..getLogger..
-00000e90: 5f5f 6e61 6d65 5f5f 7213 0000 00da 076e  __name__r......n
-00000ea0: 6461 7272 6179 7225 0000 0072 2900 0000  darrayr%...r)...
-00000eb0: 7230 0000 0072 3600 0000 7223 0000 0072  r0...r6...r#...r
-00000ec0: 2300 0000 7223 0000 0072 2400 0000 da08  #...r#...r$.....
-00000ed0: 3c6d 6f64 756c 653e 0100 0000 7318 0000  <module>....s...
-00000ee0: 0008 0108 030a 0408 0104 fe0c 2008 0104  ............ ...
-00000ef0: fe0c 220c 0104 fe0c 29                   ..".....)
+00000330: 6173 6573 3a20 fa06 6273 6573 3a20 a907  ases: ..bses: ..
+00000340: da07 5f6c 6f67 6765 72da 0564 6562 7567  .._logger..debug
+00000350: da05 6e75 6d70 79da 066c 696e 616c 67da  ..numpy..linalg.
+00000360: 046e 6f72 6dda 0665 696e 7375 6dda 0270  .norm..einsum..p
+00000370: 6929 0b72 0200 0000 7203 0000 00da 0270  i).r....r......p
+00000380: 73da 0273 73da 0277 73da 0272 73da 0266  s..ss..ws..rs..f
+00000390: 73da 0764 6966 6673 6573 da05 6e6f 726d  s..diffses..norm
+000003a0: 73da 0461 7365 73da 0462 7365 73a9 0072  s..ases..bses..r
+000003b0: 2200 0000 fa4f 2f68 6f6d 652f 6a65 6e6b  "....O/home/jenk
+000003c0: 696e 732f 6167 656e 742f 776f 726b 7370  ins/agent/worksp
+000003d0: 6163 652f 6769 7465 612d 7068 7973 6963  ace/gitea-physic
+000003e0: 735f 7064 6d65 5f31 2e31 2e30 2f70 646d  s_pdme_1.1.0/pdm
+000003f0: 652f 7574 696c 2f66 6173 745f 765f 6361  e/util/fast_v_ca
+00000400: 6c63 2e70 79da 1366 6173 745f 7673 5f66  lc.py..fast_vs_f
+00000410: 6f72 5f64 6970 6f6c 6573 0800 0000 7322  or_dipoles....s"
+00000420: 0000 0000 0714 0114 0110 0210 0110 0110  ................
+00000430: 0214 0110 0214 0210 0114 0110 0116 0110  ................
+00000440: 0236 0210 0172 2400 0000 2903 7202 0000  .6...r$...).r...
+00000450: 00da 0964 6970 6f6c 6573 6573 7204 0000  ...dipolesesr...
+00000460: 0063 0200 0000 0000 0000 0000 0000 0b00  .c..............
+00000470: 0000 0700 0000 4300 0000 738c 0100 007c  ......C...s....|
+00000480: 0164 0164 0185 0264 0164 0185 0264 0264  .d.d...d.d...d.d
+00000490: 0385 0266 0319 007d 027c 0164 0164 0185  ...f...}.|.d.d..
+000004a0: 0264 0164 0185 0264 0364 0485 0266 0319  .d.d...d.d...f..
+000004b0: 007d 037c 0164 0164 0185 0264 0164 0185  .}.|.d.d...d.d..
+000004c0: 0264 0466 0319 007d 0474 00a0 0164 057c  .d.f...}.t...d.|
+000004d0: 029b 009d 02a1 0101 0074 00a0 0164 067c  .........t...d.|
+000004e0: 039b 009d 02a1 0101 0074 00a0 0164 077c  .........t...d.|
+000004f0: 049b 009d 02a1 0101 007c 0064 0164 0185  .........|.d.d..
+00000500: 0264 0264 0385 0266 0219 007d 057c 0064  .d.d...f...}.|.d
+00000510: 0164 0185 0264 0366 0219 007d 067c 0564  .d...d.f...}.|.d
+00000520: 0164 0185 0264 0166 0219 007c 0364 0164  .d...d.f...|.d.d
+00000530: 0185 0264 0164 0164 0185 0266 0319 0018  ...d.d.d...f....
+00000540: 007d 0774 00a0 0164 087c 079b 009d 02a1  .}.t...d.|......
+00000550: 0101 0074 026a 036a 047c 0764 0364 098d  ...t.j.j.|.d.d..
+00000560: 0264 0313 007d 0874 00a0 0164 0a7c 089b  .d...}.t...d.|..
+00000570: 009d 02a1 0101 0074 02a0 0564 0b7c 077c  .......t...d.|.|
+00000580: 02a1 037c 081b 0064 0c13 007d 0974 00a0  ...|...d...}.t..
+00000590: 0164 0d7c 099b 009d 02a1 0101 0064 0c7c  .d.|.........d.|
+000005a0: 0464 0164 0185 0264 0164 0164 0185 0266  .d.d...d.d.d...f
+000005b0: 0319 0014 0074 026a 067c 0664 0164 0185  .....t.j.|.d.d..
+000005c0: 0264 0166 0219 0014 0064 0c13 007c 0464  .d.f.....d...|.d
+000005d0: 0164 0185 0264 0164 0164 0185 0266 0319  .d...d.d.d...f..
+000005e0: 0064 0c13 0017 001b 007d 0a74 00a0 0164  .d.......}.t...d
+000005f0: 0e7c 0a9b 009d 02a1 0101 0074 02a0 0564  .|.........t...d
+00000600: 0f7c 097c 0a14 00a1 0253 0029 1061 2801  .|.|.....S.).a(.
+00000610: 0000 0a09 4e6f 2065 7272 6f72 2063 6f72  ....No error cor
+00000620: 7265 6374 696f 6e20 6865 7265 2062 6162  rection here bab
+00000630: 792e 0a09 4578 7065 6374 7320 646f 745f  y...Expects dot_
+00000640: 696e 7075 7473 2074 6f20 6265 206e 756d  inputs to be num
+00000650: 7079 2061 7272 6179 206f 6620 5b72 782c  py array of [rx,
+00000660: 2072 792c 2072 7a2c 2066 5d20 656e 7472   ry, rz, f] entr
+00000670: 6965 732c 2073 6f20 6120 6e20 6279 2034  ies, so a n by 4
+00000680: 2077 6865 7265 206e 2069 7320 6e75 6d62   where n is numb
+00000690: 6572 206f 6620 6d65 6173 7572 656d 656e  er of measuremen
+000006a0: 7420 706f 696e 7473 2e0a 0a09 4469 706f  t points....Dipo
+000006b0: 6c65 7365 7320 6172 6520 6578 7065 6374  leses are expect
+000006c0: 6564 2074 6f20 6265 2061 7272 6179 206f  ed to be array o
+000006d0: 6620 6172 7261 7973 206f 6620 6172 7261  f arrays of arra
+000006e0: 7973 3a20 6c69 7374 206f 6620 7365 7473  ys: list of sets
+000006f0: 206f 6620 6469 706f 6c65 7320 7768 6963   of dipoles whic
+00000700: 6820 6172 6520 7061 7274 206f 6620 6120  h are part of a 
+00000710: 7369 6e67 6c65 2061 7272 616e 6765 6d65  single arrangeme
+00000720: 6e74 2074 6f20 6265 2061 6464 6564 2074  nt to be added t
+00000730: 6f67 6574 6865 722e 0a09 4e72 0100 0000  ogether...Nr....
+00000740: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
+00000750: 0800 0000 7209 0000 0072 0a00 0000 720c  ....r....r....r.
+00000760: 0000 0072 0e00 0000 fa0d 6162 6364 2c61  ...r......abcd,a
+00000770: 6364 2d3e 6162 6372 0b00 0000 720f 0000  cd->abcr....r...
+00000780: 0072 1000 0000 fa09 2e2e 2e6a 2d3e 2e2e  .r.........j->..
+00000790: 2e72 1100 0000 290b 7202 0000 0072 2500  .r....).r....r%.
+000007a0: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+000007b0: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+000007c0: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
+000007d0: 2200 0000 7222 0000 0072 2300 0000 da15  "...r"...r#.....
+000007e0: 6661 7374 5f76 735f 666f 725f 6469 706f  fast_vs_for_dipo
+000007f0: 6c65 7365 7328 0000 0073 2200 0000 0009  leses(...s".....
+00000800: 1a01 1a01 1602 1001 1001 1002 1401 1002  ................
+00000810: 2602 1001 1401 1001 1601 1002 4e01 1001  &...........N...
+00000820: 7228 0000 0029 0472 0200 0000 7225 0000  r(...).r....r%..
+00000830: 00da 0474 656d 7072 0400 0000 6303 0000  ...tempr....c...
+00000840: 0000 0000 0000 0000 0013 0000 0007 0000  ................
+00000850: 0043 0000 0073 a401 0000 7c01 6401 6401  .C...s....|.d.d.
+00000860: 8502 6401 6401 8502 6402 6403 8502 6603  ..d.d...d.d...f.
+00000870: 1900 7d03 7c01 6401 6401 8502 6401 6401  ..}.|.d.d...d.d.
+00000880: 8502 6403 6404 8502 6603 1900 7d04 7c01  ..d.d...f...}.|.
+00000890: 6401 6401 8502 6401 6401 8502 6404 6603  d.d...d.d...d.f.
+000008a0: 1900 7d05 7c01 6401 6401 8502 6401 6401  ..}.|.d.d...d.d.
+000008b0: 8502 6405 6603 1900 7d06 7c01 6401 6401  ..d.f...}.|.d.d.
+000008c0: 8502 6401 6401 8502 6406 6603 1900 7d07  ..d.d...d.f...}.
+000008d0: 7c00 6401 6401 8502 6402 6403 8502 6602  |.d.d...d.d...f.
+000008e0: 1900 7d08 7c00 6401 6401 8502 6403 6602  ..}.|.d.d...d.f.
+000008f0: 1900 7d09 7c08 6401 6401 8502 6401 6602  ..}.|.d.d...d.f.
+00000900: 1900 7c04 6401 6401 8502 6401 6401 6401  ..|.d.d...d.d.d.
+00000910: 8502 6603 1900 1800 7d0a 7400 a001 6407  ..f.....}.t...d.
+00000920: a101 0100 7402 a003 7c05 0b00 7c02 1b00  ....t...|...|...
+00000930: a101 7c07 1400 7d0b 7402 a003 7c06 0b00  ..|...}.t...|...
+00000940: 7c02 1b00 a101 7c07 1400 7d0c 6408 7c0b  |.....|...}.d.|.
+00000950: 7c0c 1400 7c0b 7c0c 1700 6409 1300 1b00  |...|.|...d.....
+00000960: 1400 7d0d 7c0b 7c0c 1700 7d0e 7c03 6a04  ..}.|.|...}.|.j.
+00000970: 7c0d 6a04 1400 6a04 7d0f 7402 6a05 6a06  |.j...j.}.t.j.j.
+00000980: 7c0a 6403 640a 8d02 6403 1300 7d10 7402  |.d.d...d...}.t.
+00000990: a007 640b 7c0a 7c0f a103 7c10 1b00 6409  ..d.|.|...|...d.
+000009a0: 1300 7d11 7c0e 6401 6401 8502 6401 6401  ..}.|.d.d...d.d.
+000009b0: 6401 8502 6603 1900 7402 6a08 7c09 6401  d...f...t.j.|.d.
+000009c0: 6401 8502 6401 6602 1900 1400 6409 1300  d...d.f.....d...
+000009d0: 7c0e 6401 6401 8502 6401 6401 6401 8502  |.d.d...d.d.d...
+000009e0: 6603 1900 6409 1300 1700 1b00 7d12 7402  f...d.......}.t.
+000009f0: a007 640c 7c11 7c12 1400 a102 5300 290d  ..d.|.|.....S.).
+00000a00: 61ef 0100 000a 094e 6f20 6572 726f 7220  a......No error 
+00000a10: 636f 7272 6563 7469 6f6e 2068 6572 6520  correction here 
+00000a20: 6261 6279 2e0a 0945 7870 6563 7473 2064  baby...Expects d
+00000a30: 6f74 5f69 6e70 7574 7320 746f 2062 6520  ot_inputs to be 
+00000a40: 6e75 6d70 7920 6172 7261 7920 6f66 205b  numpy array of [
+00000a50: 7278 2c20 7279 2c20 727a 2c20 665d 2065  rx, ry, rz, f] e
+00000a60: 6e74 7269 6573 2c20 736f 2061 206e 2062  ntries, so a n b
+00000a70: 7920 3420 7768 6572 6520 6e20 6973 206e  y 4 where n is n
+00000a80: 756d 6265 7220 6f66 206d 6561 7375 7265  umber of measure
+00000a90: 6d65 6e74 2070 6f69 6e74 732e 0a0a 0944  ment points....D
+00000aa0: 6970 6f6c 6573 6573 2061 7265 2065 7870  ipoleses are exp
+00000ab0: 6563 7465 6420 746f 2062 6520 6172 7261  ected to be arra
+00000ac0: 7920 6f66 2061 7272 6179 7320 6f66 2061  y of arrays of a
+00000ad0: 7272 6179 733a 0a09 6c69 7374 206f 6620  rrays:..list of 
+00000ae0: 7365 7473 206f 6620 6469 706f 6c65 7320  sets of dipoles 
+00000af0: 7768 6963 6820 6172 6520 7061 7274 206f  which are part o
+00000b00: 6620 6120 7369 6e67 6c65 2061 7272 616e  f a single arran
+00000b10: 6765 6d65 6e74 2074 6f20 6265 2061 6464  gement to be add
+00000b20: 6564 2074 6f67 6574 6865 722e 0a09 5769  ed together...Wi
+00000b30: 7468 696e 2065 6163 6820 6469 706f 6c65  thin each dipole
+00000b40: 2c20 7468 6520 6578 7065 6374 6564 2066  , the expected f
+00000b50: 6f72 6d61 7420 6973 205b 7078 2c20 7079  ormat is [px, py
+00000b60: 2c20 707a 2c20 7378 2c20 7379 2c20 737a  , pz, sx, sy, sz
+00000b70: 2c20 6531 2c20 6532 2c20 775d 0a09 5468  , e1, e2, w]..Th
+00000b80: 6520 7061 7373 6564 2069 6e20 7720 6973  e passed in w is
+00000b90: 2065 7870 6563 7465 6420 746f 2062 6520   expected to be 
+00000ba0: 6861 6c66 2074 6865 2061 6374 7561 6c2e  half the actual.
+00000bb0: 2054 6869 7320 6973 2062 6164 2c20 6275   This is bad, bu
+00000bc0: 7420 6865 7265 2066 6f72 2068 6973 746f  t here for histo
+00000bd0: 7269 6361 6c20 7265 6173 6f6e 7320 746f  rical reasons to
+00000be0: 2062 6520 6368 616e 6765 6420 6c61 7465   be changed late
+00000bf0: 722e 0a09 4e72 0100 0000 7205 0000 0072  r...Nr....r....r
+00000c00: 0600 0000 e907 0000 00e9 0800 0000 7a54  ..............zT
+00000c10: 5468 6973 206d 6574 686f 6420 6973 2076  This method is v
+00000c20: 6572 7920 6c69 6b65 6c79 2074 6f20 6265  ery likely to be
+00000c30: 2062 726f 6b65 6e2c 2061 6e64 2073 686f   broken, and sho
+00000c40: 756c 6420 6e6f 7420 6265 2075 7365 6420  uld not be used 
+00000c50: 7769 7468 6f75 7420 6d6f 7265 2074 686f  without more tho
+00000c60: 7567 6874 e904 0000 0072 0b00 0000 720c  ught.....r....r.
+00000c70: 0000 0072 2600 0000 7227 0000 0029 0972  ...r&...r'...).r
+00000c80: 1200 0000 da07 7761 726e 696e 6772 1400  ......warningr..
+00000c90: 0000 da03 6578 70da 0154 7215 0000 0072  ....exp..Tr....r
+00000ca0: 1600 0000 7217 0000 0072 1800 0000 2913  ....r....r....).
+00000cb0: 7202 0000 0072 2500 0000 7229 0000 005a  r....r%...r)...Z
+00000cc0: 0672 6177 5f70 7372 1a00 0000 5a03 6531  .raw_psr....Z.e1
+00000cd0: 735a 0365 3273 5a06 7261 775f 7773 721c  sZ.e2sZ.raw_wsr.
+00000ce0: 0000 0072 1d00 0000 721e 0000 005a 0377  ...r....r....Z.w
+00000cf0: 3173 5a03 7732 735a 0d6d 6167 5f70 7265  1sZ.w2sZ.mag_pre
+00000d00: 6661 6374 6f72 721b 0000 0072 1900 0000  factorr....r....
+00000d10: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
+00000d20: 2200 0000 7222 0000 0072 2300 0000 da20  "...r"...r#.... 
+00000d30: 6661 7374 5f76 735f 666f 725f 6173 796d  fast_vs_for_asym
+00000d40: 6d65 7472 6963 5f64 6970 6f6c 6573 6573  metric_dipoleses
+00000d50: 4900 0000 7328 0000 0000 0c1a 011a 0116  I...s(..........
+00000d60: 0116 0116 0214 0110 0226 0204 0102 ff04  .........&......
+00000d70: 0314 0114 0218 0108 030e 0214 0216 024a  ...............J
+00000d80: 0272 3000 0000 2904 da01 61da 036c 6f77  .r0...)...a..low
+00000d90: da04 6869 6768 7204 0000 0063 0300 0000  ..highr....c....
+00000da0: 0000 0000 0000 0000 0300 0000 0600 0000  ................
+00000db0: 4300 0000 731e 0000 0074 006a 0174 00a0  C...s....t.j.t..
+00000dc0: 027c 017c 006b 007c 027c 006b 04a1 0264  .|.|.k.|.|.k...d
+00000dd0: 0164 028d 0253 0029 037a 9d0a 0949 6e74  .d...S.).z...Int
+00000de0: 656e 6465 6420 7370 6563 6966 6963 616c  ended specifical
+00000df0: 6c79 2066 6f72 2074 6865 2063 6173 6520  ly for the case 
+00000e00: 7768 6572 6520 6120 6973 2061 206c 6973  where a is a lis
+00000e10: 7420 6f66 2061 7272 6179 732c 2061 6e64  t of arrays, and
+00000e20: 2065 6163 6820 6172 7261 7920 6d75 7374   each array must
+00000e30: 2062 6520 6265 7477 6565 6e20 7468 6520   be between the 
+00000e40: 7369 6e67 6c65 2061 7272 6179 206c 6f77  single array low
+00000e50: 2061 6e64 2068 6967 682c 2062 7574 2077   and high, but w
+00000e60: 6974 686f 7574 2065 7272 6f72 2063 6865  ithout error che
+00000e70: 636b 696e 672e 0a09 e901 0000 0072 0c00  cking........r..
+00000e80: 0000 2903 7214 0000 00da 0361 6c6c da0b  ..).r......all..
+00000e90: 6c6f 6769 6361 6c5f 616e 6429 0372 3100  logical_and).r1.
+00000ea0: 0000 7232 0000 0072 3300 0000 7222 0000  ..r2...r3...r"..
+00000eb0: 0072 2200 0000 7223 0000 00da 0762 6574  .r"...r#.....bet
+00000ec0: 7765 656e 7500 0000 7302 0000 0000 0472  weenu...s......r
+00000ed0: 3700 0000 290a 7214 0000 00da 076c 6f67  7...).r......log
+00000ee0: 6769 6e67 da09 6765 744c 6f67 6765 72da  ging..getLogger.
+00000ef0: 085f 5f6e 616d 655f 5f72 1200 0000 da07  .__name__r......
+00000f00: 6e64 6172 7261 7972 2400 0000 7228 0000  ndarrayr$...r(..
+00000f10: 0072 3000 0000 7237 0000 0072 2200 0000  .r0...r7...r"...
+00000f20: 7222 0000 0072 2200 0000 7223 0000 00da  r"...r"...r#....
+00000f30: 083c 6d6f 6475 6c65 3e01 0000 0073 1800  .<module>....s..
+00000f40: 0000 0801 0803 0a04 0801 04fe 0c21 0801  .............!..
+00000f50: 04fe 0c22 0c01 04fe 0c2c                 ...".....,
```

### Comparing `pdme-1.0.0/pdme/util/fast_nonlocal_spectrum.py` & `pdme-1.1.0/pdme/util/fast_nonlocal_spectrum.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,65 +41,99 @@
 
 	alphses1 = numpy.einsum("...ji, ...i", diffses1, ps) / norms1
 	alphses2 = numpy.einsum("...ji, ...i", diffses2, ps) / norms2
 	if _logger.isEnabledFor(logging.DEBUG):
 		_logger.debug(f"alphses1: {alphses1}")
 		_logger.debug(f"alphses2: {alphses2}")
 
-	bses = (1 / numpy.pi) * (ws[:, None] / (f1s**2 + ws[:, None] ** 2))
+	bses = 2 * ws[:, None] / ((numpy.pi * f1s) ** 2 + ws[:, None] ** 2)
 	if _logger.isEnabledFor(logging.DEBUG):
 		_logger.debug(f"bses: {bses}")
 
 	return alphses1 * alphses2 * bses
 
 
 def fast_s_nonlocal_dipoleses(
 	dot_pair_inputs: numpy.ndarray, dipoleses: numpy.ndarray
 ) -> numpy.ndarray:
 	"""
 	No error correction here baby.
 	"""
+
+	# We're going to annotate the indices on this class.
+	# Let's define some indices:
+	# A -> index of dipoleses configurations
+	# measurement_index -> if we have 100 frequencies for example, indexes which one of them it is
+	# j -> within a particular configuration, indexes dipole j
+	# If we need to use numbers, let's use A -> 2, j -> 10, measurement_index -> 9 for consistency with
+	# my other notes
+	# cart -> {x, y, z} is a cartesian axis
+
+	# ps, ss have shape [A, j, cart]
 	ps = dipoleses[:, :, 0:3]
 	ss = dipoleses[:, :, 3:6]
+	# ws shape [A, j]
 	ws = dipoleses[:, :, 6]
 
 	_logger.debug(f"ps: {ps}")
 	_logger.debug(f"ss: {ss}")
 	_logger.debug(f"ws: {ws}")
 
+	# rs have shape [meas_idx, {}, cart], where the inner index goes away leaving
+	# [meas, cart]
 	r1s = dot_pair_inputs[:, 0, 0:3]
 	r2s = dot_pair_inputs[:, 1, 0:3]
+	# fs have index [meas_idx], this makes sense
 	f1s = dot_pair_inputs[:, 0, 3]
 	f2s = dot_pair_inputs[:, 1, 3]
 
 	if (f1s != f2s).all():
 		raise ValueError(f"Dot pair frequencies are inconsistent: {dot_pair_inputs}")
 
+	# r1s have shape [meas, cart], adding the none makes it
+	# r1s[:, None].shape = [meas, 1, cart]
+	# ss[:, None, :].shape = [A, 1, j, cart]
+	# subtracting broadcasts by matching from the right to the left, giving a final shape of
+	# diffses.shape [A, meas, j, cart]
 	diffses1 = r1s[:, None] - ss[:, None, :]
 	diffses2 = r2s[:, None] - ss[:, None, :]
 	if _logger.isEnabledFor(logging.DEBUG):
 		_logger.debug(f"diffses1: {diffses1}")
 		_logger.debug(f"diffses2: {diffses2}")
 
+	# norming on the cartesian axis, which is axis 3 as seen above
+	# norms.shape [A, meas, j]
 	norms1 = numpy.linalg.norm(diffses1, axis=3) ** 3
 	norms2 = numpy.linalg.norm(diffses2, axis=3) ** 3
 	if _logger.isEnabledFor(logging.DEBUG):
 		_logger.debug(f"norms1: {norms1}")
 		_logger.debug(f"norms2: {norms2}")
 
+	# diffses shape [A, meas, j, cart]
+	# ps shape [A, j, cart]
+	# so we're summing over the d axis, the cartesian one.
+	# final shape of numerator is [A, meas, j]
+	# denom shape is [A, meas, j]
+	# final shape stayes [A, meas, j]
 	alphses1 = numpy.einsum("abcd,acd->abc", diffses1, ps) / norms1
 	alphses2 = numpy.einsum("abcd,acd->abc", diffses2, ps) / norms2
 	if _logger.isEnabledFor(logging.DEBUG):
 		_logger.debug(f"alphses1: {alphses1}")
 		_logger.debug(f"alphses2: {alphses2}")
 
-	bses = (1 / numpy.pi) * (ws[:, None, :] / (f1s[:, None] ** 2 + ws[:, None, :] ** 2))
+	# ws shape [A, j], so numerator has shape [A, 1, j]
+	# f1s shape is [meas], so first term of denom is [meas, 1]
+	# ws[:, None, :].shape [A, 1, j] so breadcasting the sum in denom gives
+	# denom.shape [A meas, j]
+	# so now overall shape is [A, meas, j]
+	bses = 2 * ws[:, None, :] / ((numpy.pi * f1s[:, None]) ** 2 + ws[:, None, :] ** 2)
 	if _logger.isEnabledFor(logging.DEBUG):
 		_logger.debug(f"bses: {bses}")
 
+	# so our output shape is [A, meas, j]
 	_logger.debug(f"Raw pair calc: [{alphses1 * alphses2 * bses}]")
 	return numpy.einsum("...j->...", alphses1 * alphses2 * bses)
 
 
 def fast_s_spin_qubit_tarucha_nonlocal_dipoleses(
 	dot_pair_inputs: numpy.ndarray, dipoleses: numpy.ndarray
 ) -> numpy.ndarray:
@@ -148,23 +182,23 @@
 	# these broadcast from right to left
 	# [	 measurement_idx, 1, rxs]
 	# [A,	  1,			   j, sxs]
 	# resulting in [A, measurement_idx, j, cart3] sxs rxs are both cart3
 	diffses1 = r1s[:, None] - ss[:, None, :]
 	diffses2 = r2s[:, None] - ss[:, None, :]
 	if _logger.isEnabledFor(logging.DEBUG):
-		_logger.warning(f"diffses1: {diffses1}")
-		_logger.warning(f"diffses2: {diffses2}")
+		_logger.debug(f"diffses1: {diffses1}")
+		_logger.debug(f"diffses2: {diffses2}")
 
 	# norms takes out axis 3, the last one, giving [A, measurement_idx, j]
 	norms1 = numpy.linalg.norm(diffses1, axis=3)
 	norms2 = numpy.linalg.norm(diffses2, axis=3)
 	if _logger.isEnabledFor(logging.DEBUG):
-		_logger.warning(f"norms1: {norms1}")
-		_logger.warning(f"norms2: {norms2}")
+		_logger.debug(f"norms1: {norms1}")
+		_logger.debug(f"norms2: {norms2}")
 
 	# _logger.info(f"norms1: {norms1}")
 	# _logger.info(f"norms1 shape: {norms1.shape}")
 	#
 	# diffses1 (A, measurement_idx, j, xs)
 	# ps:  (A, j, px)
 	# result is (A, measurement_idx, j)
@@ -211,22 +245,22 @@
 				)
 				* numpy.transpose(diffses2)
 			)[:, :, :, 0]
 		)
 		- ps[:, numpy.newaxis, :, 0]
 	) / (norms2**3)
 	if _logger.isEnabledFor(logging.DEBUG):
-		_logger.warning(f"alphses1: {alphses1}")
-		_logger.warning(f"alphses2: {alphses2}")
+		_logger.debug(f"alphses1: {alphses1}")
+		_logger.debug(f"alphses2: {alphses2}")
 
-	bses = (1 / numpy.pi) * (ws[:, None, :] / (f1s[:, None] ** 2 + ws[:, None, :] ** 2))
+	bses = 2 * ws[:, None, :] / ((numpy.pi * f1s[:, None]) ** 2 + ws[:, None, :] ** 2)
 	if _logger.isEnabledFor(logging.DEBUG):
-		_logger.warning(f"bses: {bses}")
+		_logger.debug(f"bses: {bses}")
 
-	_logger.warning(f"Raw pair calc: [{alphses1 * alphses2 * bses}]")
+	_logger.debug(f"Raw pair calc: [{alphses1 * alphses2 * bses}]")
 	return numpy.einsum("...j->...", alphses1 * alphses2 * bses)
 
 
 def signarg(x, **kwargs):
 	"""
 	uses numpy.sign to implement Arg for real numbers only. Should return pi for negative inputs, 0 for positive.
 	Passes through args to numpy.sign
```

### Comparing `pdme-1.0.0/pdme/util/fast_v_calc.py` & `pdme-1.1.0/pdme/util/fast_v_calc.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
 	_logger.debug(f"diffses: {diffses}")
 	norms = numpy.linalg.norm(diffses, axis=2) ** 3
 	_logger.debug(f"norms: {norms}")
 	ases = (numpy.einsum("...ji, ...i", diffses, ps) / norms) ** 2
 	_logger.debug(f"ases: {ases}")
 
-	bses = (1 / numpy.pi) * (ws[:, None] / (fs**2 + ws[:, None] ** 2))
+	bses = 2 * ws[:, None] / ((numpy.pi * fs) ** 2 + ws[:, None] ** 2)
+
 	_logger.debug(f"bses: {bses}")
 	return ases * bses
 
 
 def fast_vs_for_dipoleses(
 	dot_inputs: numpy.ndarray, dipoleses: numpy.ndarray
 ) -> numpy.ndarray:
@@ -60,15 +61,15 @@
 
 	_logger.debug(f"diffses: {diffses}")
 	norms = numpy.linalg.norm(diffses, axis=3) ** 3
 	_logger.debug(f"norms: {norms}")
 	ases = (numpy.einsum("abcd,acd->abc", diffses, ps) / norms) ** 2
 	_logger.debug(f"ases: {ases}")
 
-	bses = (1 / numpy.pi) * (ws[:, None, :] / (fs[:, None] ** 2 + ws[:, None, :] ** 2))
+	bses = 2 * ws[:, None, :] / ((numpy.pi * fs[:, None]) ** 2 + ws[:, None, :] ** 2)
 	_logger.debug(f"bses: {bses}")
 	return numpy.einsum("...j->...", ases * bses)
 
 
 def fast_vs_for_asymmetric_dipoleses(
 	dot_inputs: numpy.ndarray, dipoleses: numpy.ndarray, temp: numpy.ndarray
 ) -> numpy.ndarray:
@@ -88,28 +89,31 @@
 	raw_ws = dipoleses[:, :, 8]
 
 	rs = dot_inputs[:, 0:3]
 	fs = dot_inputs[:, 3]
 
 	diffses = rs[:, None] - ss[:, None, :]
 
+	_logger.warning(
+		"This method is very likely to be broken, and should not be used without more thought"
+	)
 	w1s = numpy.exp(-e1s / temp) * raw_ws
 	w2s = numpy.exp(-e2s / temp) * raw_ws
 
 	mag_prefactor = 4 * ((w1s * w2s) / ((w1s + w2s) ** 2))
 	ws = w1s + w2s
 
 	# some annoying broadcast thing here?
 	ps = (raw_ps.T * mag_prefactor.T).T
 
 	norms = numpy.linalg.norm(diffses, axis=3) ** 3
 
 	ases = (numpy.einsum("abcd,acd->abc", diffses, ps) / norms) ** 2
 
-	bses = (1 / numpy.pi) * (ws[:, None, :] / (fs[:, None] ** 2 + ws[:, None, :] ** 2))
+	bses = ws[:, None, :] / ((numpy.pi * fs[:, None]) ** 2 + ws[:, None, :] ** 2)
 
 	return numpy.einsum("...j->...", ases * bses)
 
 
 def between(a: numpy.ndarray, low: numpy.ndarray, high: numpy.ndarray) -> numpy.ndarray:
 	"""
 	Intended specifically for the case where a is a list of arrays, and each array must be between the single array low and high, but without error checking.
```

### Comparing `pdme-1.0.0/pyproject.toml` & `pdme-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdme"
-version = "1.0.0"
+version = "1.1.0"
 description = "Python dipole model evaluator"
 authors = ["Deepak <dmallubhotla+github@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
```

### Comparing `pdme-1.0.0/PKG-INFO` & `pdme-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdme
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python dipole model evaluator
 License: GPL-3.0-only
 Author: Deepak
 Author-email: dmallubhotla+github@gmail.com
 Requires-Python: >=3.8.1,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 # pdme - the python dipole model evaluator
 
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-green.svg?style=flat-square)](https://conventionalcommits.org)
 [![PyPI](https://img.shields.io/pypi/v/pdme?style=flat-square)](https://pypi.org/project/pdme/)
 [![Jenkins](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster&style=flat-square)](https://jenkins.deepak.science/job/gitea-physics/job/pdme/job/master/)
 ![Jenkins tests](https://img.shields.io/jenkins/tests?compact_message&jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)
 ![Jenkins Coverage](https://img.shields.io/jenkins/coverage/cobertura?jobUrl=https%3A%2F%2Fjenkins.deepak.science%2Fjob%2Fgitea-physics%2Fjob%2Fpdme%2Fjob%2Fmaster%2F&style=flat-square)
-![Maintenance](https://img.shields.io/maintenance/yes/2023?style=flat-square)
+![Maintenance](https://img.shields.io/maintenance/yes/2024?style=flat-square)
 
 This repo has library code for evaluating dipole models.
 
 ## Getting started
 
 `poetry install` to start locally
```


# Comparing `tmp/jsrm-0.0.6.tar.gz` & `tmp/jsrm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsrm-0.0.6.tar", last modified: Sat Oct 28 20:29:59 2023, max compression
+gzip compressed data, was "jsrm-0.0.7.tar", last modified: Fri May  3 09:40:00 2024, max compression
```

## Comparing `jsrm-0.0.6.tar` & `jsrm-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 20:29:59.553118 jsrm-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-10-28 20:29:41.000000 jsrm-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2023-10-28 20:29:59.553118 jsrm-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2023-10-28 20:29:41.000000 jsrm-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2023-10-28 20:29:41.000000 jsrm-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-28 20:29:59.553118 jsrm-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 20:29:59.545118 jsrm-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 20:29:59.545118 jsrm-0.0.6/src/jsrm/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 20:29:59.545118 jsrm-0.0.6/src/jsrm/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/parameters/hsa_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 20:29:59.545118 jsrm-0.0.6/src/jsrm/symbolic_derivation/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_derivation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_derivation/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)    25722 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_derivation/planar_hsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_derivation/planar_pcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_derivation/symbolic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 20:29:59.549118 jsrm-0.0.6/src/jsrm/symbolic_expressions/
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_expressions/pendulum_nl-1.dill
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_expressions/pendulum_nl-2.dill
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_expressions/pendulum_nl-3.dill
--rw-r--r--   0 runner    (1001) docker     (127)    52443 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-2.dill
--rw-r--r--   0 runner    (1001) docker     (127)    85783 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-4.dill
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_expressions/planar_pcs_ns-1.dill
--rw-r--r--   0 runner    (1001) docker     (127)    43433 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/symbolic_expressions/planar_pcs_ns-2.dill
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 20:29:59.549118 jsrm-0.0.6/src/jsrm/systems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/systems/euler_lagrangian.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/systems/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)    29179 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/systems/planar_hsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/systems/planar_pcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/systems/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-10-28 20:29:41.000000 jsrm-0.0.6/src/jsrm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 20:29:59.545118 jsrm-0.0.6/src/jsrm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2023-10-28 20:29:59.000000 jsrm-0.0.6/src/jsrm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2023-10-28 20:29:59.000000 jsrm-0.0.6/src/jsrm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-28 20:29:59.000000 jsrm-0.0.6/src/jsrm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-10-28 20:29:59.000000 jsrm-0.0.6/src/jsrm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-28 20:29:59.000000 jsrm-0.0.6/src/jsrm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 20:29:59.549118 jsrm-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2023-10-28 20:29:41.000000 jsrm-0.0.6/tests/test_planar_hsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2023-10-28 20:29:41.000000 jsrm-0.0.6/tests/test_planar_pcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.377231 jsrm-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-03 09:39:52.000000 jsrm-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-03 09:40:00.377231 jsrm-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-03 09:39:52.000000 jsrm-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-03 09:39:52.000000 jsrm-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:40:00.377231 jsrm-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.369231 jsrm-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.369231 jsrm-0.0.7/src/jsrm/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.373231 jsrm-0.0.7/src/jsrm/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15530 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/parameters/hsa_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.373231 jsrm-0.0.7/src/jsrm/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/rendering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.373231 jsrm-0.0.7/src/jsrm/rendering/planar_hsa/
+-rw-r--r--   0 runner    (1001) docker     (127)     9469 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/rendering/planar_hsa/opencv_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.373231 jsrm-0.0.7/src/jsrm/symbolic_derivation/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_derivation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_derivation/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26256 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_derivation/planar_hsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_derivation/planar_pcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_derivation/symbolic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.373231 jsrm-0.0.7/src/jsrm/symbolic_expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-1.dill
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-2.dill
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-3.dill
+-rw-r--r--   0 runner    (1001) docker     (127)    52619 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-2.dill
+-rw-r--r--   0 runner    (1001) docker     (127)    86067 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-4.dill
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_pcs_ns-1.dill
+-rw-r--r--   0 runner    (1001) docker     (127)    43433 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_pcs_ns-2.dill
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.377231 jsrm-0.0.7/src/jsrm/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/euler_lagrangian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31773 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/planar_hsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/planar_pcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/systems/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-03 09:39:52.000000 jsrm-0.0.7/src/jsrm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.377231 jsrm-0.0.7/src/jsrm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-03 09:40:00.000000 jsrm-0.0.7/src/jsrm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-03 09:40:00.000000 jsrm-0.0.7/src/jsrm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:40:00.000000 jsrm-0.0.7/src/jsrm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-03 09:40:00.000000 jsrm-0.0.7/src/jsrm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 09:40:00.000000 jsrm-0.0.7/src/jsrm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:40:00.377231 jsrm-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-03 09:39:52.000000 jsrm-0.0.7/tests/test_planar_hsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-03 09:39:52.000000 jsrm-0.0.7/tests/test_planar_pcs.py
```

### Comparing `jsrm-0.0.6/LICENSE.txt` & `jsrm-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/PKG-INFO` & `jsrm-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsrm
-Version: 0.0.6
+Version: 0.0.7
 Summary: Kinematic and dynamic models of continuum and articulated soft robots.
 Author-email: Maximilian Stölzle <maximilian@stoelzle.ch>
 Maintainer-email: Maximilian Stölzle <maximilian@stoelzle.ch>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -42,23 +42,23 @@
 License-File: LICENSE.txt
 Requires-Dist: dill
 Requires-Dist: jax
 Requires-Dist: numpy
 Requires-Dist: peppercorn
 Requires-Dist: sympy>=1.11
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: codecov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-html; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Provides-Extra: examples
 Requires-Dist: diffrax; extra == "examples"
 Requires-Dist: matplotlib; extra == "examples"
 Requires-Dist: opencv-python; extra == "examples"
 Provides-Extra: test
 Requires-Dist: codecov; extra == "test"
@@ -67,15 +67,15 @@
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-html; extra == "test"
 Requires-Dist: tox; extra == "test"
 
 # JAX Soft Robot Modelling
 
 This repository contains symbolic derivations of the kinematics and dynamics of various soft robots using Sympy.
-The symbolic expressions are then implemented in JAX used for fast, parallelizable, and differentiable simulations.
+The symbolic expressions are then implemented in JAX and can be used for fast, parallelizable, and differentiable simulations.
 So far, we have focused on planar settings and implemented the following soft robots:
 
 - [N-link pendulum](examples/simulate_pendulum.py)
 - [Planar Piecewise Constant Strain (PCS) continuum soft robot](examples/simulate_planar_pcs.py)
 - [Planar Handed Shearing Auxetics (HSA) robot](examples/simulate_planar_hsa.py)
 
 We are happy to receive contributions for other soft robots and/or other settings (e.g., 3D).
@@ -116,23 +116,34 @@
 
 ```bash
 pip install ".[examples]"
 ```
 
 ## Usage
 
-Always, first source all necessary environment variables when opening a new terminal:
+Always first source all necessary environment variables when opening a new terminal:
 
 ```bash
 source 01-configure-env-vars.sh
 ```
 
-Then, we can symbolically derive the pendulum kinematics and dynamics
+Then, we can symbolically derive the pendulum kinematics and dynamics:
 
 ```bash
 python examples/derive_pendulum.py
 ```
 
 Finally, we can simulate the pendulum
 ```bash
 python examples/simulate_pendulum.py
 ```
+
+## See also
+
+You might also be interested in the following repositories:
+ - The [`jax-spcs-kinematics`](https://github.com/tud-phi/jax-spcs-kinematics) repository contains an implementation
+ of the Selective Piecewise Constant Strain (SPCS) kinematics in JAX. We have shown in our paper that this kinematic 
+model is suitable for representing the shape of HSA rods.
+ - The [`HSA-PyElastica`](https://github.com/tud-phi/HSA-PyElastica) repository contains a plugin for PyElastica
+for the simulation of HSA robots.
+ - The [`hsa-planar-control`](https://github.com/tud-phi/hsa-planar-control) repository contains JAX and ROS2 implementations
+ of model-based control algorithms for planar HSA robots.
```

### Comparing `jsrm-0.0.6/README.md` & `jsrm-0.0.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # JAX Soft Robot Modelling
 
 This repository contains symbolic derivations of the kinematics and dynamics of various soft robots using Sympy.
-The symbolic expressions are then implemented in JAX used for fast, parallelizable, and differentiable simulations.
+The symbolic expressions are then implemented in JAX and can be used for fast, parallelizable, and differentiable simulations.
 So far, we have focused on planar settings and implemented the following soft robots:
 
 - [N-link pendulum](examples/simulate_pendulum.py)
 - [Planar Piecewise Constant Strain (PCS) continuum soft robot](examples/simulate_planar_pcs.py)
 - [Planar Handed Shearing Auxetics (HSA) robot](examples/simulate_planar_hsa.py)
 
 We are happy to receive contributions for other soft robots and/or other settings (e.g., 3D).
@@ -46,23 +46,34 @@
 
 ```bash
 pip install ".[examples]"
 ```
 
 ## Usage
 
-Always, first source all necessary environment variables when opening a new terminal:
+Always first source all necessary environment variables when opening a new terminal:
 
 ```bash
 source 01-configure-env-vars.sh
 ```
 
-Then, we can symbolically derive the pendulum kinematics and dynamics
+Then, we can symbolically derive the pendulum kinematics and dynamics:
 
 ```bash
 python examples/derive_pendulum.py
 ```
 
 Finally, we can simulate the pendulum
 ```bash
 python examples/simulate_pendulum.py
 ```
+
+## See also
+
+You might also be interested in the following repositories:
+ - The [`jax-spcs-kinematics`](https://github.com/tud-phi/jax-spcs-kinematics) repository contains an implementation
+ of the Selective Piecewise Constant Strain (SPCS) kinematics in JAX. We have shown in our paper that this kinematic 
+model is suitable for representing the shape of HSA rods.
+ - The [`HSA-PyElastica`](https://github.com/tud-phi/HSA-PyElastica) repository contains a plugin for PyElastica
+for the simulation of HSA robots.
+ - The [`hsa-planar-control`](https://github.com/tud-phi/hsa-planar-control) repository contains JAX and ROS2 implementations
+ of model-based control algorithms for planar HSA robots.
```

### Comparing `jsrm-0.0.6/pyproject.toml` & `jsrm-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "jsrm"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.6"  # Required
+version = "0.0.7"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Kinematic and dynamic models of continuum and articulated soft robots."  # Optional
 
 # This is an optional longer description of your project that represents
@@ -114,23 +114,23 @@
 #
 #   $ pip install sampleproject[dev]
 #
 # Similar to `dependencies` above, these must be valid existing
 # projects.
 [project.optional-dependencies] # Optional
 dev = [
-    "black",
     "bump2version",
     "check-manifest",
     "codecov",
     "coverage",
     "pre-commit",
     "pytest",
     "pytest-cov",
     "pytest-html",
+    "ruff",
     "tox",
 ]
 examples = [
     "diffrax",
     "matplotlib",
     "opencv-python",
 ]
```

### Comparing `jsrm-0.0.6/src/jsrm/integration.py` & `jsrm-0.0.7/src/jsrm/integration.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/math_utils.py` & `jsrm-0.0.7/src/jsrm/math_utils.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/parameters/hsa_params.py` & `jsrm-0.0.7/src/jsrm/parameters/hsa_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,25 @@
     "generate_base_params_for_epu",
     "PARAMS_FPU_CONTROL",
     "PARAMS_FPU_SYSTEM_ID",
     "PARAMS_EPU_CONTROL",
     "PARAMS_EPU_SYSTEM_ID",
 ]
 
+import jax
 from jax import Array
 import jax.numpy as jnp
 from typing import Dict
 
 
 def generate_common_base_params(
     num_segments: int = 1,
     num_rods_per_segment: int = 4,
     end_effector_attached: int = False,
+    consider_hysteresis: bool = False,
 ) -> Dict[str, Array]:
     assert num_rods_per_segment % 2 == 0, "num_rods_per_segment must be even"
 
     ones_rod = jnp.ones((num_segments, num_rods_per_segment))
 
     params = {
         "th0": jnp.array(0.0),  # initial orientation angle [rad]
@@ -58,14 +60,59 @@
         params["mpl"] = jnp.array(
             0.018
         )  # the end-effector attachment has a mass of 18g
         # the end-effector attachment has a center of gravity of 3.63mm in y-dir from its base.
         # as it has a thickness of 25mm, this is -21.37mm from the top surface (i.e., end-effector position)
         params["CoGpl"] = jnp.array([0.0, -0.02137])
 
+    params["hysteresis"] = {}
+    if consider_hysteresis:
+        """
+        Parameters for modeling Bouc-Wen hysteresis
+        https://en.wikipedia.org/wiki/Bouc%E2%80%93Wen_model_of_hysteresis
+
+        Notation of Bouc-Wen hysteresis model is based on the paper:
+        Song J. and Der Kiureghian A. (2006) 
+        Generalized Bouc–Wen model for highly asymmetric hysteresis. 
+        Journal of Engineering Mechanics. ASCE. Vol 132, No. 6 pp. 610–618
+
+        Important: we assume that each strain experiences independent hysteresis
+        """
+        # mapping hysteresis displacements to the strains
+        # per default, we only model the hysteresis on the axial strain
+        B_z = jax.scipy.linalg.block_diag(
+            *[
+                jnp.array([[0.0], [0.0], [1.0]]) for _ in range(num_segments)
+            ]  # assumes 3 strains per segment
+        )
+        params["hysteresis"]["basis"] = B_z
+        # number of hysteresis states
+        n_z = params["hysteresis"]["basis"].shape[1]
+        # ratio of post-yield and pre-yield stiffness
+        hys_alpha_val = 0.6
+        hys_alpha = jnp.array(
+            [
+                (hys_alpha_val if B_z[xi_idx, :].sum() > 0 else 1.0)
+                for xi_idx in range(3 * num_segments)
+            ]
+        )
+        params["hysteresis"]["alpha"] = hys_alpha
+        # params["hysteresis"]["alpha"] = 0.6 * jnp.ones((n_q, ))  # ratio of post-yield and pre-yield stiffness
+        params["hysteresis"]["beta"] = 30.0 * jnp.ones(
+            (n_z,)
+        )  # dimensionless parameter in the Bouc-Wen model
+        params["hysteresis"]["gamma"] = 1.0 * jnp.ones(
+            (n_z,)
+        )  # dimensionless parameter in the Bouc-Wen model
+        params["hysteresis"]["n"] = 1.0 * jnp.ones(
+            (n_z,)
+        )  # dimensionless parameter in the Bouc-Wen model
+        # to remove redundancy from Bouc-Wen model, choose A = 1
+        params["hysteresis"]["A"] = jnp.ones((n_z,))
+
     return params
 
 
 def generate_base_params_for_fpu(
     num_segments: int = 1,
     num_rods_per_segment: int = 4,
     rod_multiplier: int = 1,
@@ -261,21 +308,27 @@
         "h": jnp.array([[1.0, -1.0, 1.0, -1.0]]),
         "roff": 24e-3 * jnp.array([[1.0, 1.0, -1.0, -1.0]]),
     }
 )
 PARAMS_FPU_CONTROL = generate_base_params_for_fpu(
     num_segments=1, num_rods_per_segment=2, rod_multiplier=2
 )
+PARAMS_FPU_HYSTERESIS_CONTROL = generate_base_params_for_fpu(
+    num_segments=1, num_rods_per_segment=2, rod_multiplier=2, consider_hysteresis=True
+)
 
 PARAMS_EPU_SYSTEM_ID = generate_base_params_for_epu(
     num_segments=1, num_rods_per_segment=4
 )
 PARAMS_EPU_SYSTEM_ID.update(
     {
         "h": jnp.array([[1.0, -1.0, 1.0, -1.0]]),
         "roff": 24e-3 * jnp.array([[1.0, 1.0, -1.0, -1.0]]),
     }
 )
 
 PARAMS_EPU_CONTROL = generate_base_params_for_epu(
     num_segments=1, num_rods_per_segment=2, rod_multiplier=2
 )
+PARAMS_EPU_HYSTERESIS_CONTROL = generate_base_params_for_epu(
+    num_segments=1, num_rods_per_segment=2, rod_multiplier=2, consider_hysteresis=True
+)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jsrm-0.0.6/src/jsrm/symbolic_derivation/pendulum.py` & `jsrm-0.0.7/src/jsrm/symbolic_derivation/pendulum.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/symbolic_derivation/planar_hsa.py` & `jsrm-0.0.7/src/jsrm/symbolic_derivation/planar_hsa.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,16 @@
     Ar = sp.zeros(num_segments, num_rods_per_segment)
     # second area moment of inertia for bending of each rod
     Ir = sp.zeros(num_segments, num_rods_per_segment)
     # inertia matrix
     B = sp.zeros(num_dof, num_dof)
     # potential energy
     U = sp.Matrix([[0]])
+    # stiffness matrix
+    Shat = sp.zeros(3 * num_segments, 3 * num_segments)
     # elastic vector
     K = sp.zeros(3 * num_segments, 1)
     # damping matrix
     D = sp.zeros(3 * num_segments, 3 * num_segments)
     # actuation vector
     alpha = sp.zeros(3 * num_segments, 1)
 
@@ -334,14 +336,20 @@
                 S_b_deltar, S_sh_deltar, S_a_deltar
             )
             Sr = Shatr + Sdeltar
 
             # Jacobian of the strain of the physical HSA rods with respect to the configuration variables
             J_betar = sp.Matrix([[1, 0, 0], [0, 1, 0], [roff[i, j], 0, 1]])
 
+            # nominal stiffness matrix of the virtual backbone
+            Shat[3 * i : 3 * (i + 1), 3 * i : 3 * (i + 1)] += (
+                J_betar.T @ Shatr @ J_betar
+            )
+
+            # contribution of elastic forces of current rod to the virtual backbone
             vKr = J_betar.T @ Shatr @ (pxir - pxi_eqr)
             # add contribution of elasticity vector
             K[3 * i : 3 * (i + 1), 0] += vKr
 
             # damping coefficient of the current rod
             vDr = J_betar.T @ sp.diag(zetab[i, j], zetash[i, j], zetaa[i, j]) @ J_betar
             # add contribution of damping matrix
@@ -512,14 +520,16 @@
 
     # compute the gravity force vector
     G = -U.jacobian(xi).transpose()
     if simplify:
         G = sp.simplify(G)
     print("G =\n", G)
 
+    Shat = sp.simplify(Shat)
+    print("Shat =\n", Shat)
     K = sp.simplify(K)
     print("K =\n", K)
     D = sp.simplify(D)
     print("D =\n", D)
     alpha = sp.simplify(alpha)
     print("alpha =\n", alpha)
 
@@ -577,15 +587,16 @@
             "Jr_sms": Jr_sms,  # list of the Jacobians of the centerline of each rod
             "Jp_sms": Jp_sms,  # list of the platform Jacobians
             "Jee": Jee,  # Jacobian of the end-effector
             "Jee_d": Jee_d,  # time derivative of the Jacobian of the end-effector
             "B": B,
             "C": C,
             "G": G,
-            "K": K,
+            "Shat": Shat,  # nominal stiffness matrix of the virtual backbone
+            "K": K,  # nominal elastic forces on the virtual backbone
             "D": D,
             "alpha": alpha,
         },
     }
 
     if filepath is not None:
         if isinstance(filepath, str):
```

### Comparing `jsrm-0.0.6/src/jsrm/symbolic_derivation/planar_pcs.py` & `jsrm-0.0.7/src/jsrm/symbolic_derivation/planar_pcs.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/symbolic_derivation/symbolic_utils.py` & `jsrm-0.0.7/src/jsrm/symbolic_derivation/symbolic_utils.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/symbolic_expressions/pendulum_nl-1.dill` & `jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-1.dill`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/symbolic_expressions/pendulum_nl-2.dill` & `jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-2.dill`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/symbolic_expressions/pendulum_nl-3.dill` & `jsrm-0.0.7/src/jsrm/symbolic_expressions/pendulum_nl-3.dill`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-2.dill` & `jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-2.dill`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 95d0 cc00 0000 0000 007d 9428 8c0b  ...........}.(..
+00000000: 8004 9580 cd00 0000 0000 007d 9428 8c0b  ...........}.(..
 00000010: 7061 7261 6d73 5f73 796d 7394 7d94 288c  params_syms.}.(.
 00000020: 0374 6830 948c 1173 796d 7079 2e63 6f72  .th0...sympy.cor
 00000030: 652e 7379 6d62 6f6c 948c 0653 796d 626f  e.symbol...Symbo
 00000040: 6c94 9394 6803 8594 7d94 8c04 7265 616c  l...h...}...real
 00000050: 9488 7392 948c 016c 945d 9468 068c 026c  ..s....l.].h...l
 00000060: 3194 8594 7d94 288c 0b6e 6f6e 6e65 6761  1...}.(..nonnega
 00000070: 7469 7665 9488 8c07 6e6f 6e7a 6572 6f94  tive....nonzero.
@@ -3188,91 +3188,102 @@
 0000c730: 126a ca01 0000 8794 8194 8694 8194 8694  .j..............
 0000c740: 8194 6a55 0100 006a 6801 0000 688d 6a31  ..jU...jh...h.j1
 0000c750: 0200 0087 9481 946a 5501 0000 6a68 0100  .......jU...jh..
 0000c760: 0068 906a ce01 0000 8794 8194 7494 8194  .h.j........t...
 0000c770: 7494 8194 6a55 0100 0028 6a68 0100 006a  t...jU...(jh...j
 0000c780: 5901 0000 687c 6a8c 0200 006a 030f 0000  Y...h|j....j....
 0000c790: 6acd 0f00 0074 9481 9474 9481 9487 9481  j....t...t......
-0000c7a0: 9487 9481 948c 014b 946a 8302 0000 6a85  .......K.j....j.
-0000c7b0: 0200 006a f30d 0000 6a88 0200 006a 5c01  ...j....j....j\.
-0000c7c0: 0000 286a 5501 0000 6a68 0100 0068 966a  ..(jU...jh...h.j
-0000c7d0: 5c01 0000 6849 6a55 0100 006a 6801 0000  \...hIjU...jh...
-0000c7e0: 6a18 0100 0086 9481 9486 9481 9487 9481  j...............
-0000c7f0: 946a 5501 0000 6a68 0100 0068 9a6a 5c01  .jU...jh...h.j\.
-0000c800: 0000 684c 6ada 0f00 0086 9481 9487 9481  ..hLj...........
-0000c810: 946a 5501 0000 6a68 0100 0068 b46a 5c01  .jU...jh...h.j\.
-0000c820: 0000 6851 6a55 0100 006a 6801 0000 6a1c  ..hQjU...jh...j.
-0000c830: 0100 0086 9481 9486 9481 9487 9481 946a  ...............j
-0000c840: 5501 0000 6a68 0100 0068 b86a 5c01 0000  U...jh...h.j\...
-0000c850: 6854 6ae4 0f00 0086 9481 9487 9481 946a  hTj............j
-0000c860: 5501 0000 68aa 6840 6a5c 0100 006a 2001  U...h.h@j\...j .
-0000c870: 0000 6a55 0100 006a 6801 0000 6859 8694  ..jU...jh...hY..
-0000c880: 8194 6a55 0100 006a 1801 0000 6840 8694  ..jU...j....h@..
-0000c890: 8194 8794 8194 8794 8194 6a55 0100 0068  ..........jU...h
-0000c8a0: ae68 446a 5c01 0000 6a20 0100 006a 5501  .hDj\...j ...jU.
-0000c8b0: 0000 6a68 0100 0068 5c86 9481 946a 5501  ..jh...h\....jU.
-0000c8c0: 0000 6a18 0100 0068 4486 9481 9487 9481  ..j....hD.......
-0000c8d0: 9487 9481 9474 9481 946a 5c01 0000 286a  .....t...j\...(j
-0000c8e0: 5501 0000 6a68 0100 0068 b46a dc0f 0000  U...jh...h.j....
-0000c8f0: 8794 8194 6a55 0100 006a 6801 0000 68b8  ....jU...jh...h.
-0000c900: 6ae0 0f00 0087 9481 946a 5501 0000 6a68  j........jU...jh
-0000c910: 0100 0068 a06a e60f 0000 8794 8194 6a55  ...h.j........jU
-0000c920: 0100 006a 6801 0000 68a4 6aea 0f00 0087  ...jh...h.j.....
-0000c930: 9481 9474 9481 946a 5c01 0000 6a55 0100  ...t...j\...jU..
-0000c940: 0068 aa6a f20f 0000 8694 8194 6a55 0100  .h.j........jU..
-0000c950: 0068 ae6a fa0f 0000 8694 8194 8694 8194  .h.j............
-0000c960: 8794 8194 8794 8194 8c01 4494 6a83 0200  ..........D.j...
-0000c970: 006a 8502 0000 6a85 0200 006a 8802 0000  .j....j....j....
-0000c980: 286a 5c01 0000 2868 dc68 e06a 5501 0000  (j\...(h.h.jU...
-0000c990: 68f0 6a5f 0100 0068 406a 6301 0000 8694  h.j_...h@jc.....
-0000c9a0: 8194 8694 8194 6a55 0100 0068 f46a c704  ......jU...h.j..
-0000c9b0: 0000 8694 8194 7494 8194 6ac9 0200 006a  ......t...j....j
-0000c9c0: 5c01 0000 6a55 0100 0068 4068 f086 9481  \...jU...h@h....
-0000c9d0: 946a 5501 0000 6844 68f4 8694 8194 8694  .jU...hDh.......
-0000c9e0: 8194 6ac9 0200 006a 5c01 0000 68e6 68ea  ..j....j\...h.h.
-0000c9f0: 8694 8194 6ac9 0200 006a 2110 0000 6ac9  ....j....j!...j.
-0000ca00: 0200 006a 5c01 0000 68f0 68f4 8694 8194  ...j\...h.h.....
-0000ca10: 7494 8194 8794 8194 8c05 616c 7068 6194  t.........alpha.
-0000ca20: 6a83 0200 006a 8502 0000 6af3 0d00 006a  j....j....j....j
-0000ca30: 8802 0000 6a55 0100 006a 5f01 0000 6812  ....jU...j_...h.
-0000ca40: 6a8a 0200 0086 9481 946a 5c01 0000 6a55  j........j\...jU
-0000ca50: 0100 0068 126a 5c01 0000 6a55 0100 0028  ...h.j\...jU...(
-0000ca60: 6823 6a3b 0100 0068 be6a 5c01 0000 6849  h#j;...h.j\...hI
-0000ca70: 6ada 0f00 0086 9481 9474 9481 946a 5501  j........t...jU.
-0000ca80: 0000 2868 266a 3e01 0000 68c2 6a5c 0100  ..(h&j>...h.j\..
-0000ca90: 0068 4c6a da0f 0000 8694 8194 7494 8194  .hLj........t...
-0000caa0: 8694 8194 8694 8194 6a55 0100 0028 6a68  ........jU...(jh
-0000cab0: 0100 0068 236a 3b01 0000 6840 6a5c 0100  ...h#j;...h@j\..
-0000cac0: 006a 5501 0000 6a68 0100 0068 616a 5c01  .jU...jh...haj\.
-0000cad0: 0000 6a55 0100 0068 aa68 1286 9481 946a  ..jU...h.h.....j
-0000cae0: 5501 0000 6823 6a3b 0100 0068 d287 9481  U...h#j;...h....
-0000caf0: 9486 9481 9487 9481 946a 5501 0000 68d2  .........jU...h.
-0000cb00: 6812 6a5c 0100 006a 2001 0000 6a55 0100  h.j\...j ...jU..
-0000cb10: 006a 6801 0000 6859 8694 8194 6a55 0100  .jh...hY....jU..
-0000cb20: 006a 1801 0000 6840 8694 8194 8794 8194  .j....h@........
-0000cb30: 8794 8194 8694 8194 7494 8194 6a55 0100  ........t...jU..
-0000cb40: 0028 6a68 0100 0068 266a 3e01 0000 6844  .(jh...h&j>...hD
-0000cb50: 6a5c 0100 006a 5501 0000 6a68 0100 0068  j\...jU...jh...h
-0000cb60: 646a 5c01 0000 6a55 0100 0068 ae68 1286  dj\...jU...h.h..
-0000cb70: 9481 946a 5501 0000 6826 6a3e 0100 0068  ...jU...h&j>...h
-0000cb80: d687 9481 9486 9481 9487 9481 946a 5501  .............jU.
-0000cb90: 0000 68d6 6812 6a5c 0100 006a 2001 0000  ..h.h.j\...j ...
-0000cba0: 6a55 0100 006a 6801 0000 685c 8694 8194  jU...jh...h\....
-0000cbb0: 6a55 0100 006a 1801 0000 6844 8694 8194  jU...j....hD....
-0000cbc0: 8794 8194 8794 8194 8694 8194 7494 8194  ............t...
-0000cbd0: 8794 8194 8694 8194 6a55 0100 006a 5f01  ........jU...j_.
-0000cbe0: 0000 6812 6a68 0100 0086 9481 946a 5c01  ..h.jh.......j\.
-0000cbf0: 0000 6a55 0100 0028 6823 6a3b 0100 0068  ..jU...(h#j;...h
-0000cc00: c86a 5c01 0000 6851 6ae4 0f00 0086 9481  .j\...hQj.......
-0000cc10: 9474 9481 946a 5501 0000 2868 266a 3e01  .t...jU...(h&j>.
-0000cc20: 0000 68cc 6a5c 0100 0068 546a e40f 0000  ..h.j\...hTj....
-0000cc30: 8694 8194 7494 8194 8694 8194 8694 8194  ....t...........
-0000cc40: 6a55 0100 006a 2c10 0000 6a5c 0100 006a  jU...j,...j\...j
-0000cc50: 5501 0000 6a68 0100 0068 126a 5c01 0000  U...jh...h.j\...
-0000cc60: 6a55 0100 0028 6823 6a3b 0100 0068 d26a  jU...(h#j;...h.j
-0000cc70: 4610 0000 7494 8194 6a55 0100 0028 6826  F...t...jU...(h&
-0000cc80: 6a3e 0100 0068 d66a 5a10 0000 7494 8194  j>...h.jZ...t...
-0000cc90: 8694 8194 8794 8194 6a55 0100 0028 6861  ........jU...(ha
-0000cca0: 6823 6a3b 0100 006a 3e10 0000 7494 8194  h#j;...j>...t...
-0000ccb0: 6a55 0100 0028 6864 6826 6a3e 0100 006a  jU...(hdh&j>...j
-0000ccc0: 5210 0000 7494 8194 8794 8194 8694 8194  R...t...........
-0000ccd0: 8794 8194 8794 8194 7575 2e              ........uu.
+0000c7a0: 9487 9481 948c 0453 6861 7494 6a83 0200  .......Shat.j...
+0000c7b0: 006a 8502 0000 6a85 0200 006a 8802 0000  .j....j....j....
+0000c7c0: 286a 5c01 0000 2868 9668 9a6a 5501 0000  (j\...(h.h.jU...
+0000c7d0: 68aa 6a5f 0100 0068 406a 6301 0000 8694  h.j_...h@jc.....
+0000c7e0: 8194 8694 8194 6a55 0100 0068 ae6a c704  ......jU...h.j..
+0000c7f0: 0000 8694 8194 7494 8194 6a5c 0100 0068  ......t...j\...h
+0000c800: b468 b886 9481 946a 5c01 0000 6a55 0100  .h.....j\...jU..
+0000c810: 0068 aa68 4086 9481 946a 5501 0000 68ae  .h.h@....jU...h.
+0000c820: 6844 8694 8194 8694 8194 6ae2 0f00 006a  hD........j....j
+0000c830: 5c01 0000 68a0 68a4 8694 8194 6ac9 0200  \...h.h.....j...
+0000c840: 006a e80f 0000 6ac9 0200 006a 5c01 0000  .j....j....j\...
+0000c850: 68aa 68ae 8694 8194 7494 8194 8794 8194  h.h.....t.......
+0000c860: 8c01 4b94 6a83 0200 006a 8502 0000 6af3  ..K.j....j....j.
+0000c870: 0d00 006a 8802 0000 6a5c 0100 0028 6a55  ...j....j\...(jU
+0000c880: 0100 006a 6801 0000 6896 6a5c 0100 0068  ...jh...h.j\...h
+0000c890: 496a 5501 0000 6a68 0100 006a 1801 0000  IjU...jh...j....
+0000c8a0: 8694 8194 8694 8194 8794 8194 6a55 0100  ............jU..
+0000c8b0: 006a 6801 0000 689a 6a5c 0100 0068 4c6a  .jh...h.j\...hLj
+0000c8c0: f30f 0000 8694 8194 8794 8194 6a55 0100  ............jU..
+0000c8d0: 006a 6801 0000 68b4 6a5c 0100 0068 516a  .jh...h.j\...hQj
+0000c8e0: 5501 0000 6a68 0100 006a 1c01 0000 8694  U...jh...j......
+0000c8f0: 8194 8694 8194 8794 8194 6a55 0100 006a  ..........jU...j
+0000c900: 6801 0000 68b8 6a5c 0100 0068 546a fd0f  h...h.j\...hTj..
+0000c910: 0000 8694 8194 8794 8194 6a55 0100 0068  ..........jU...h
+0000c920: aa68 406a 5c01 0000 6a20 0100 006a 5501  .h@j\...j ...jU.
+0000c930: 0000 6a68 0100 0068 5986 9481 946a 5501  ..jh...hY....jU.
+0000c940: 0000 6a18 0100 0068 4086 9481 9487 9481  ..j....h@.......
+0000c950: 9487 9481 946a 5501 0000 68ae 6844 6a5c  .....jU...h.hDj\
+0000c960: 0100 006a 2001 0000 6a55 0100 006a 6801  ...j ...jU...jh.
+0000c970: 0000 685c 8694 8194 6a55 0100 006a 1801  ..h\....jU...j..
+0000c980: 0000 6844 8694 8194 8794 8194 8794 8194  ..hD............
+0000c990: 7494 8194 6a5c 0100 0028 6a55 0100 006a  t...j\...(jU...j
+0000c9a0: 6801 0000 68b4 6af5 0f00 0087 9481 946a  h...h.j........j
+0000c9b0: 5501 0000 6a68 0100 0068 b86a f90f 0000  U...jh...h.j....
+0000c9c0: 8794 8194 6a55 0100 006a 6801 0000 68a0  ....jU...jh...h.
+0000c9d0: 6aff 0f00 0087 9481 946a 5501 0000 6a68  j........jU...jh
+0000c9e0: 0100 0068 a46a 0310 0000 8794 8194 7494  ...h.j........t.
+0000c9f0: 8194 6a5c 0100 006a 5501 0000 68aa 6a0b  ..j\...jU...h.j.
+0000ca00: 1000 0086 9481 946a 5501 0000 68ae 6a13  .......jU...h.j.
+0000ca10: 1000 0086 9481 9486 9481 9487 9481 9487  ................
+0000ca20: 9481 948c 0144 946a 8302 0000 6a85 0200  .....D.j....j...
+0000ca30: 006a 8502 0000 6a88 0200 0028 6a5c 0100  .j....j....(j\..
+0000ca40: 0028 68dc 68e0 6a55 0100 0068 f06a da0f  .(h.h.jU...h.j..
+0000ca50: 0000 8694 8194 6a55 0100 0068 f46a c704  ......jU...h.j..
+0000ca60: 0000 8694 8194 7494 8194 6ac9 0200 006a  ......t...j....j
+0000ca70: 5c01 0000 6a55 0100 0068 4068 f086 9481  \...jU...h@h....
+0000ca80: 946a 5501 0000 6844 68f4 8694 8194 8694  .jU...hDh.......
+0000ca90: 8194 6ac9 0200 006a 5c01 0000 68e6 68ea  ..j....j\...h.h.
+0000caa0: 8694 8194 6ac9 0200 006a 3810 0000 6ac9  ....j....j8...j.
+0000cab0: 0200 006a 5c01 0000 68f0 68f4 8694 8194  ...j\...h.h.....
+0000cac0: 7494 8194 8794 8194 8c05 616c 7068 6194  t.........alpha.
+0000cad0: 6a83 0200 006a 8502 0000 6af3 0d00 006a  j....j....j....j
+0000cae0: 8802 0000 6a55 0100 006a 5f01 0000 6812  ....jU...j_...h.
+0000caf0: 6a8a 0200 0086 9481 946a 5c01 0000 6a55  j........j\...jU
+0000cb00: 0100 0068 126a 5c01 0000 6a55 0100 0028  ...h.j\...jU...(
+0000cb10: 6823 6a3b 0100 0068 be6a 5c01 0000 6849  h#j;...h.j\...hI
+0000cb20: 6af3 0f00 0086 9481 9474 9481 946a 5501  j........t...jU.
+0000cb30: 0000 2868 266a 3e01 0000 68c2 6a5c 0100  ..(h&j>...h.j\..
+0000cb40: 0068 4c6a f30f 0000 8694 8194 7494 8194  .hLj........t...
+0000cb50: 8694 8194 8694 8194 6a55 0100 0028 6a68  ........jU...(jh
+0000cb60: 0100 0068 236a 3b01 0000 6840 6a5c 0100  ...h#j;...h@j\..
+0000cb70: 006a 5501 0000 6a68 0100 0068 616a 5c01  .jU...jh...haj\.
+0000cb80: 0000 6a55 0100 0068 aa68 1286 9481 946a  ..jU...h.h.....j
+0000cb90: 5501 0000 6823 6a3b 0100 0068 d287 9481  U...h#j;...h....
+0000cba0: 9486 9481 9487 9481 946a 5501 0000 68d2  .........jU...h.
+0000cbb0: 6812 6a5c 0100 006a 2001 0000 6a55 0100  h.j\...j ...jU..
+0000cbc0: 006a 6801 0000 6859 8694 8194 6a55 0100  .jh...hY....jU..
+0000cbd0: 006a 1801 0000 6840 8694 8194 8794 8194  .j....h@........
+0000cbe0: 8794 8194 8694 8194 7494 8194 6a55 0100  ........t...jU..
+0000cbf0: 0028 6a68 0100 0068 266a 3e01 0000 6844  .(jh...h&j>...hD
+0000cc00: 6a5c 0100 006a 5501 0000 6a68 0100 0068  j\...jU...jh...h
+0000cc10: 646a 5c01 0000 6a55 0100 0068 ae68 1286  dj\...jU...h.h..
+0000cc20: 9481 946a 5501 0000 6826 6a3e 0100 0068  ...jU...h&j>...h
+0000cc30: d687 9481 9486 9481 9487 9481 946a 5501  .............jU.
+0000cc40: 0000 68d6 6812 6a5c 0100 006a 2001 0000  ..h.h.j\...j ...
+0000cc50: 6a55 0100 006a 6801 0000 685c 8694 8194  jU...jh...h\....
+0000cc60: 6a55 0100 006a 1801 0000 6844 8694 8194  jU...j....hD....
+0000cc70: 8794 8194 8794 8194 8694 8194 7494 8194  ............t...
+0000cc80: 8794 8194 8694 8194 6a55 0100 006a 5f01  ........jU...j_.
+0000cc90: 0000 6812 6a68 0100 0086 9481 946a 5c01  ..h.jh.......j\.
+0000cca0: 0000 6a55 0100 0028 6823 6a3b 0100 0068  ..jU...(h#j;...h
+0000ccb0: c86a 5c01 0000 6851 6afd 0f00 0086 9481  .j\...hQj.......
+0000ccc0: 9474 9481 946a 5501 0000 2868 266a 3e01  .t...jU...(h&j>.
+0000ccd0: 0000 68cc 6a5c 0100 0068 546a fd0f 0000  ..h.j\...hTj....
+0000cce0: 8694 8194 7494 8194 8694 8194 8694 8194  ....t...........
+0000ccf0: 6a55 0100 006a 4310 0000 6a5c 0100 006a  jU...jC...j\...j
+0000cd00: 5501 0000 6a68 0100 0068 126a 5c01 0000  U...jh...h.j\...
+0000cd10: 6a55 0100 0028 6823 6a3b 0100 0068 d26a  jU...(h#j;...h.j
+0000cd20: 5d10 0000 7494 8194 6a55 0100 0028 6826  ]...t...jU...(h&
+0000cd30: 6a3e 0100 0068 d66a 7110 0000 7494 8194  j>...h.jq...t...
+0000cd40: 8694 8194 8794 8194 6a55 0100 0028 6861  ........jU...(ha
+0000cd50: 6823 6a3b 0100 006a 5510 0000 7494 8194  h#j;...jU...t...
+0000cd60: 6a55 0100 0028 6864 6826 6a3e 0100 006a  jU...(hdh&j>...j
+0000cd70: 6910 0000 7494 8194 8794 8194 8694 8194  i...t...........
+0000cd80: 8794 8194 8794 8194 7575 2e              ........uu.
```

### Comparing `jsrm-0.0.6/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-4.dill` & `jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_hsa_ns-1_nrs-4.dill`

 * *Files 2% similar despite different names*

```diff
@@ -4090,15 +4090,15 @@
 0000ff90: 0100 006a 8003 0000 6a2b 0300 0087 9481  ...j....j+......
 0000ffa0: 946a e901 0000 286a fc01 0000 6812 6a73  .j....(j....h.js
 0000ffb0: 0200 006a 2503 0000 7494 8194 8794 8194  ...j%...t.......
 0000ffc0: 6a97 0700 0074 9481 946a e901 0000 286a  j....t...j....(j
 0000ffd0: 9e10 0000 6a61 0800 006a a210 0000 6a97  ....ja...j....j.
 0000ffe0: 0700 0074 9481 946a e901 0000 286a ca09  ...t...j....(j..
 0000fff0: 0000 284b 016a cb09 0000 4aff ffff ff4b  ..(K.j....J....K
-00010000: 0174 9485 947d 946a cf09 0000 9502 4f00  .t...}.j......O.
+00010000: 0174 9485 947d 946a cf09 0000 951e 5000  .t...}.j......P.
 00010010: 0000 0000 004b 3573 9294 6a86 0100 006a  .....K5s..j....j
 00010020: 0309 0000 6a1a 1000 0074 9481 946a e901  ....j....t...j..
 00010030: 0000 286a b610 0000 6a86 0100 006a 6108  ..(j....j....ja.
 00010040: 0000 6a28 1000 0074 9481 946a e901 0000  ..j(...t...j....
 00010050: 286a ca09 0000 284b 016a cb09 0000 4aff  (j....(K.j....J.
 00010060: ffff ff4b 0174 9485 947d 946a cf09 0000  ...K.t...}.j....
 00010070: 4b35 7392 946a 0309 0000 6a1a 1000 006a  K5s..j....j....j
@@ -5198,165 +5198,183 @@
 000144d0: 9481 946a e901 0000 286a fc01 0000 6aed  ...j....(j....j.
 000144e0: 0100 0068 b26a 8003 0000 6a6d 1600 006a  ...h.j....jm...j
 000144f0: d717 0000 7494 8194 6ae9 0100 0028 6afc  ....t...j....(j.
 00014500: 0100 006a ed01 0000 68b6 6a80 0300 006a  ...j....h.j....j
 00014510: 9b16 0000 6ad7 1700 0074 9481 946a e901  ....j....t...j..
 00014520: 0000 286a fc01 0000 6aed 0100 0068 ba6a  ..(j....j....h.j
 00014530: 8003 0000 6ac9 1600 006a d717 0000 7494  ....j....j....t.
-00014540: 8194 7494 8194 8794 8194 8794 8194 8c01  ..t.............
-00014550: 4b94 6a77 0300 006a 7903 0000 6a51 1500  K.jw...jy...jQ..
-00014560: 006a 7c03 0000 6af0 0100 0028 6ae9 0100  .j|...j....(j...
-00014570: 006a fc01 0000 68d4 6af0 0100 0068 676a  .j....h.j....hgj
-00014580: e901 0000 6afc 0100 006a a601 0000 8694  ....j....j......
-00014590: 8194 8694 8194 8794 8194 6ae9 0100 006a  ..........j....j
-000145a0: fc01 0000 68d8 6af0 0100 0068 6a6a e817  ....h.j....hjj..
-000145b0: 0000 8694 8194 8794 8194 6ae9 0100 006a  ..........j....j
-000145c0: fc01 0000 68dc 6af0 0100 0068 6d6a e817  ....h.j....hmj..
-000145d0: 0000 8694 8194 8794 8194 6ae9 0100 006a  ..........j....j
-000145e0: fc01 0000 68e0 6af0 0100 0068 706a e817  ....h.j....hpj..
-000145f0: 0000 8694 8194 8794 8194 6ae9 0100 006a  ..........j....j
-00014600: fc01 0000 6a0a 0100 006a f001 0000 6875  ....j....j....hu
-00014610: 6ae9 0100 006a fc01 0000 6aaa 0100 0086  j....j....j.....
-00014620: 9481 9486 9481 9487 9481 946a e901 0000  ...........j....
-00014630: 6afc 0100 006a 0e01 0000 6af0 0100 0068  j....j....j....h
-00014640: 786a fa17 0000 8694 8194 8794 8194 6ae9  xj............j.
-00014650: 0100 006a fc01 0000 6a12 0100 006a f001  ...j....j....j..
-00014660: 0000 687b 6afa 1700 0086 9481 9487 9481  ..h{j...........
-00014670: 946a e901 0000 6afc 0100 006a 1601 0000  .j....j....j....
-00014680: 6af0 0100 0068 7e6a fa17 0000 8694 8194  j....h~j........
-00014690: 8794 8194 6ae9 0100 0068 f868 566a f001  ....j....h.hVj..
-000146a0: 0000 6aae 0100 006a e901 0000 6afc 0100  ..j....j....j...
-000146b0: 0068 8386 9481 946a e901 0000 6aa6 0100  .h.....j....j...
-000146c0: 0068 5686 9481 9487 9481 9487 9481 946a  .hV............j
-000146d0: e901 0000 68fc 685a 6af0 0100 006a ae01  ....h.hZj....j..
-000146e0: 0000 6ae9 0100 006a fc01 0000 6886 8694  ..j....j....h...
-000146f0: 8194 6ae9 0100 006a a601 0000 685a 8694  ..j....j....hZ..
-00014700: 8194 8794 8194 8794 8194 6ae9 0100 006a  ..........j....j
-00014710: 0001 0000 685e 6af0 0100 006a ae01 0000  ....h^j....j....
-00014720: 6ae9 0100 006a fc01 0000 6889 8694 8194  j....j....h.....
-00014730: 6ae9 0100 006a a601 0000 685e 8694 8194  j....j....h^....
-00014740: 8794 8194 8794 8194 6ae9 0100 006a 0401  ........j....j..
-00014750: 0000 6862 6af0 0100 006a ae01 0000 6ae9  ..hbj....j....j.
-00014760: 0100 006a fc01 0000 688c 8694 8194 6ae9  ...j....h.....j.
-00014770: 0100 006a a601 0000 6862 8694 8194 8794  ...j....hb......
-00014780: 8194 8794 8194 7494 8194 6af0 0100 0028  ......t...j....(
-00014790: 6ae9 0100 006a fc01 0000 6a0a 0100 006a  j....j....j....j
-000147a0: ea17 0000 8794 8194 6ae9 0100 006a fc01  ........j....j..
-000147b0: 0000 6a0e 0100 006a ee17 0000 8794 8194  ..j....j........
-000147c0: 6ae9 0100 006a fc01 0000 6a12 0100 006a  j....j....j....j
-000147d0: f217 0000 8794 8194 6ae9 0100 006a fc01  ........j....j..
-000147e0: 0000 6a16 0100 006a f617 0000 8794 8194  ..j....j........
-000147f0: 6ae9 0100 006a fc01 0000 68e6 6afc 1700  j....j....h.j...
-00014800: 0087 9481 946a e901 0000 6afc 0100 0068  .....j....j....h
-00014810: ea6a 0018 0000 8794 8194 6ae9 0100 006a  .j........j....j
-00014820: fc01 0000 68ee 6a04 1800 0087 9481 946a  ....h.j........j
-00014830: e901 0000 6afc 0100 0068 f26a 0818 0000  ....j....h.j....
-00014840: 8794 8194 7494 8194 6af0 0100 0028 6ae9  ....t...j....(j.
-00014850: 0100 0068 f86a 1018 0000 8694 8194 6ae9  ...h.j........j.
-00014860: 0100 0068 fc6a 1818 0000 8694 8194 6ae9  ...h.j........j.
-00014870: 0100 006a 0001 0000 6a20 1800 0086 9481  ...j....j ......
-00014880: 946a e901 0000 6a04 0100 006a 2818 0000  .j....j....j(...
-00014890: 8694 8194 7494 8194 8794 8194 8794 8194  ....t...........
-000148a0: 8c01 4494 6a77 0300 006a 7903 0000 6a79  ..D.jw...jy...jy
-000148b0: 0300 006a 7c03 0000 286a f001 0000 286a  ...j|...(j....(j
-000148c0: 5201 0000 6a56 0100 006a 5a01 0000 6a5e  R...jV...jZ...j^
-000148d0: 0100 006a e901 0000 6a76 0100 006a f301  ...j....jv...j..
-000148e0: 0000 6856 6af7 0100 0086 9481 9486 9481  ..hVj...........
-000148f0: 946a e901 0000 6a7a 0100 006a f301 0000  .j....jz...j....
-00014900: 685a 6af7 0100 0086 9481 9486 9481 946a  hZj............j
-00014910: e901 0000 6a7e 0100 006a f301 0000 685e  ....j~...j....h^
-00014920: 6af7 0100 0086 9481 9486 9481 946a e901  j............j..
-00014930: 0000 6a82 0100 006a f706 0000 8694 8194  ..j....j........
-00014940: 7494 8194 6abd 0300 006a f001 0000 286a  t...j....j....(j
-00014950: e901 0000 6856 6a76 0100 0086 9481 946a  ....hVjv.......j
-00014960: e901 0000 685a 6a7a 0100 0086 9481 946a  ....hZjz.......j
-00014970: e901 0000 685e 6a7e 0100 0086 9481 946a  ....h^j~.......j
-00014980: e901 0000 6862 6a82 0100 0086 9481 9474  ....hbj........t
-00014990: 9481 946a bd03 0000 6af0 0100 0028 6a64  ...j....j....(jd
-000149a0: 0100 006a 6801 0000 6a6c 0100 006a 7001  ...jh...jl...jp.
-000149b0: 0000 7494 8194 6abd 0300 006a 6718 0000  ..t...j....jg...
-000149c0: 6abd 0300 006a f001 0000 286a 7601 0000  j....j....(jv...
-000149d0: 6a7a 0100 006a 7e01 0000 6a82 0100 0074  jz...j~...j....t
-000149e0: 9481 9474 9481 9487 9481 948c 0561 6c70  ...t.........alp
-000149f0: 6861 946a 7703 0000 6a79 0300 006a 5115  ha.jw...jy...jQ.
-00014a00: 0000 6a7c 0300 006a e901 0000 6af3 0100  ..j|...j....j...
-00014a10: 0068 126a 7e03 0000 8694 8194 6af0 0100  .h.j~.......j...
-00014a20: 0028 6ae9 0100 0068 126a f001 0000 286a  .(j....h.j....(j
-00014a30: e901 0000 2868 236a c901 0000 6a1c 0100  ....(h#j....j...
-00014a40: 006a f001 0000 6867 6ae8 1700 0086 9481  .j....hgj.......
-00014a50: 9474 9481 946a e901 0000 2868 266a cc01  .t...j....(h&j..
-00014a60: 0000 6a20 0100 006a f001 0000 686a 6ae8  ..j ...j....hjj.
-00014a70: 1700 0086 9481 9474 9481 946a e901 0000  .......t...j....
-00014a80: 2868 296a cf01 0000 6a24 0100 006a f001  (h)j....j$...j..
-00014a90: 0000 686d 6ae8 1700 0086 9481 9474 9481  ..hmj........t..
-00014aa0: 946a e901 0000 2868 2c6a d201 0000 6a28  .j....(h,j....j(
-00014ab0: 0100 006a f001 0000 6870 6ae8 1700 0086  ...j....hpj.....
-00014ac0: 9481 9474 9481 9474 9481 9486 9481 946a  ...t...t.......j
-00014ad0: e901 0000 286a fc01 0000 6823 6ac9 0100  ....(j....h#j...
-00014ae0: 0068 566a f001 0000 6ae9 0100 006a fc01  .hVj....j....j..
-00014af0: 0000 6891 6af0 0100 006a e901 0000 68f8  ..h.j....j....h.
-00014b00: 6812 8694 8194 6ae9 0100 0068 236a c901  h.....j....h#j..
-00014b10: 0000 6a40 0100 0087 9481 9486 9481 9487  ..j@............
-00014b20: 9481 946a e901 0000 6a40 0100 0068 126a  ...j....j@...h.j
-00014b30: f001 0000 6aae 0100 006a e901 0000 6afc  ....j....j....j.
-00014b40: 0100 0068 8386 9481 946a e901 0000 6aa6  ...h.....j....j.
-00014b50: 0100 0068 5686 9481 9487 9481 9487 9481  ...hV...........
-00014b60: 9486 9481 9474 9481 946a e901 0000 286a  .....t...j....(j
-00014b70: fc01 0000 6826 6acc 0100 0068 5a6a f001  ....h&j....hZj..
-00014b80: 0000 6ae9 0100 006a fc01 0000 6894 6af0  ..j....j....h.j.
-00014b90: 0100 006a e901 0000 68fc 6812 8694 8194  ...j....h.h.....
-00014ba0: 6ae9 0100 0068 266a cc01 0000 6a44 0100  j....h&j....jD..
-00014bb0: 0087 9481 9486 9481 9487 9481 946a e901  .............j..
-00014bc0: 0000 6a44 0100 0068 126a f001 0000 6aae  ..jD...h.j....j.
-00014bd0: 0100 006a e901 0000 6afc 0100 0068 8686  ...j....j....h..
-00014be0: 9481 946a e901 0000 6aa6 0100 0068 5a86  ...j....j....hZ.
-00014bf0: 9481 9487 9481 9487 9481 9486 9481 9474  ...............t
-00014c00: 9481 946a e901 0000 286a fc01 0000 6829  ...j....(j....h)
-00014c10: 6acf 0100 0068 5e6a f001 0000 6ae9 0100  j....h^j....j...
-00014c20: 006a fc01 0000 6897 6af0 0100 006a e901  .j....h.j....j..
-00014c30: 0000 6a00 0100 0068 1286 9481 946a e901  ..j....h.....j..
-00014c40: 0000 6829 6acf 0100 006a 4801 0000 8794  ..h)j....jH.....
-00014c50: 8194 8694 8194 8794 8194 6ae9 0100 006a  ..........j....j
-00014c60: 4801 0000 6812 6af0 0100 006a ae01 0000  H...h.j....j....
-00014c70: 6ae9 0100 006a fc01 0000 6889 8694 8194  j....j....h.....
-00014c80: 6ae9 0100 006a a601 0000 685e 8694 8194  j....j....h^....
-00014c90: 8794 8194 8794 8194 8694 8194 7494 8194  ............t...
-00014ca0: 6ae9 0100 0028 6afc 0100 0068 2c6a d201  j....(j....h,j..
-00014cb0: 0000 6862 6af0 0100 006a e901 0000 6afc  ..hbj....j....j.
-00014cc0: 0100 0068 9a6a f001 0000 6ae9 0100 006a  ...h.j....j....j
-00014cd0: 0401 0000 6812 8694 8194 6ae9 0100 0068  ....h.....j....h
-00014ce0: 2c6a d201 0000 6a4c 0100 0087 9481 9486  ,j....jL........
-00014cf0: 9481 9487 9481 946a e901 0000 6a4c 0100  .......j....jL..
-00014d00: 0068 126a f001 0000 6aae 0100 006a e901  .h.j....j....j..
-00014d10: 0000 6afc 0100 0068 8c86 9481 946a e901  ..j....h.....j..
-00014d20: 0000 6aa6 0100 0068 6286 9481 9487 9481  ..j....hb.......
-00014d30: 9487 9481 9486 9481 9474 9481 9474 9481  .........t...t..
-00014d40: 9486 9481 946a e901 0000 6af3 0100 0068  .....j....j....h
-00014d50: 126a fc01 0000 8694 8194 6af0 0100 0028  .j........j....(
-00014d60: 6ae9 0100 0028 6823 6ac9 0100 006a 2e01  j....(h#j....j..
-00014d70: 0000 6af0 0100 0068 756a e901 0000 6afc  ..j....huj....j.
-00014d80: 0100 006a aa01 0000 8694 8194 8694 8194  ...j............
-00014d90: 7494 8194 6ae9 0100 0028 6826 6acc 0100  t...j....(h&j...
-00014da0: 006a 3201 0000 6af0 0100 0068 786a de18  .j2...j....hxj..
-00014db0: 0000 8694 8194 7494 8194 6ae9 0100 0028  ......t...j....(
-00014dc0: 6829 6acf 0100 006a 3601 0000 6af0 0100  h)j....j6...j...
-00014dd0: 0068 7b6a de18 0000 8694 8194 7494 8194  .h{j........t...
-00014de0: 6ae9 0100 0028 682c 6ad2 0100 006a 3a01  j....(h,j....j:.
-00014df0: 0000 6af0 0100 0068 7e6a de18 0000 8694  ..j....h~j......
-00014e00: 8194 7494 8194 7494 8194 8694 8194 6ae9  ..t...t.......j.
-00014e10: 0100 006a 7218 0000 6af0 0100 0028 6ae9  ...jr...j....(j.
-00014e20: 0100 006a fc01 0000 6812 6af0 0100 0028  ...j....h.j....(
-00014e30: 6ae9 0100 0028 6823 6ac9 0100 006a 4001  j....(h#j....j@.
-00014e40: 0000 6a10 1800 0074 9481 946a e901 0000  ..j....t...j....
-00014e50: 2868 266a cc01 0000 6a44 0100 006a 1818  (h&j....jD...j..
-00014e60: 0000 7494 8194 6ae9 0100 0028 6829 6acf  ..t...j....(h)j.
-00014e70: 0100 006a 4801 0000 6a20 1800 0074 9481  ...jH...j ...t..
-00014e80: 946a e901 0000 2868 2c6a d201 0000 6a4c  .j....(h,j....jL
-00014e90: 0100 006a 2818 0000 7494 8194 7494 8194  ...j(...t...t...
-00014ea0: 8794 8194 6ae9 0100 0028 6891 6823 6ac9  ....j....(h.h#j.
-00014eb0: 0100 006a 8c18 0000 7494 8194 6ae9 0100  ...j....t...j...
-00014ec0: 0028 6894 6826 6acc 0100 006a a018 0000  .(h.h&j....j....
-00014ed0: 7494 8194 6ae9 0100 0028 6897 6829 6acf  t...j....(h.h)j.
-00014ee0: 0100 006a b418 0000 7494 8194 6ae9 0100  ...j....t...j...
-00014ef0: 0028 689a 682c 6ad2 0100 006a c818 0000  .(h.h,j....j....
-00014f00: 7494 8194 7494 8194 8694 8194 8794 8194  t...t...........
-00014f10: 8794 8194 7575 2e                        ....uu.
+00014540: 8194 7494 8194 8794 8194 8794 8194 8c04  ..t.............
+00014550: 5368 6174 946a 7703 0000 6a79 0300 006a  Shat.jw...jy...j
+00014560: 7903 0000 6a7c 0300 0028 6af0 0100 0028  y...j|...(j....(
+00014570: 68d4 68d8 68dc 68e0 6ae9 0100 0068 f86a  h.h.h.h.j....h.j
+00014580: f301 0000 6856 6af7 0100 0086 9481 9486  ....hVj.........
+00014590: 9481 946a e901 0000 68fc 6af3 0100 0068  ...j....h.j....h
+000145a0: 5a6a f701 0000 8694 8194 8694 8194 6ae9  Zj............j.
+000145b0: 0100 006a 0001 0000 6af3 0100 0068 5e6a  ...j....j....h^j
+000145c0: f701 0000 8694 8194 8694 8194 6ae9 0100  ............j...
+000145d0: 006a 0401 0000 6af7 0600 0086 9481 9474  .j....j........t
+000145e0: 9481 946a f001 0000 286a 0a01 0000 6a0e  ...j....(j....j.
+000145f0: 0100 006a 1201 0000 6a16 0100 0074 9481  ...j....j....t..
+00014600: 946a f001 0000 286a e901 0000 68f8 6856  .j....(j....h.hV
+00014610: 8694 8194 6ae9 0100 0068 fc68 5a86 9481  ....j....h.hZ...
+00014620: 946a e901 0000 6a00 0100 0068 5e86 9481  .j....j....h^...
+00014630: 946a e901 0000 6a04 0100 0068 6286 9481  .j....j....hb...
+00014640: 9474 9481 946a f817 0000 6af0 0100 0028  .t...j....j....(
+00014650: 68e6 68ea 68ee 68f2 7494 8194 6abd 0300  h.h.h.h.t...j...
+00014660: 006a 0218 0000 6abd 0300 006a f001 0000  .j....j....j....
+00014670: 2868 f868 fc6a 0001 0000 6a04 0100 0074  (h.h.j....j....t
+00014680: 9481 9474 9481 9487 9481 948c 014b 946a  ...t.........K.j
+00014690: 7703 0000 6a79 0300 006a 5115 0000 6a7c  w...jy...jQ...j|
+000146a0: 0300 006a f001 0000 286a e901 0000 6afc  ...j....(j....j.
+000146b0: 0100 0068 d46a f001 0000 6867 6ae9 0100  ...h.j....hgj...
+000146c0: 006a fc01 0000 6aa6 0100 0086 9481 9486  .j....j.........
+000146d0: 9481 9487 9481 946a e901 0000 6afc 0100  .......j....j...
+000146e0: 0068 d86a f001 0000 686a 6a0d 1800 0086  .h.j....hjj.....
+000146f0: 9481 9487 9481 946a e901 0000 6afc 0100  .......j....j...
+00014700: 0068 dc6a f001 0000 686d 6a0d 1800 0086  .h.j....hmj.....
+00014710: 9481 9487 9481 946a e901 0000 6afc 0100  .......j....j...
+00014720: 0068 e06a f001 0000 6870 6a0d 1800 0086  .h.j....hpj.....
+00014730: 9481 9487 9481 946a e901 0000 6afc 0100  .......j....j...
+00014740: 006a 0a01 0000 6af0 0100 0068 756a e901  .j....j....huj..
+00014750: 0000 6afc 0100 006a aa01 0000 8694 8194  ..j....j........
+00014760: 8694 8194 8794 8194 6ae9 0100 006a fc01  ........j....j..
+00014770: 0000 6a0e 0100 006a f001 0000 6878 6a1f  ..j....j....hxj.
+00014780: 1800 0086 9481 9487 9481 946a e901 0000  ...........j....
+00014790: 6afc 0100 006a 1201 0000 6af0 0100 0068  j....j....j....h
+000147a0: 7b6a 1f18 0000 8694 8194 8794 8194 6ae9  {j............j.
+000147b0: 0100 006a fc01 0000 6a16 0100 006a f001  ...j....j....j..
+000147c0: 0000 687e 6a1f 1800 0086 9481 9487 9481  ..h~j...........
+000147d0: 946a e901 0000 68f8 6856 6af0 0100 006a  .j....h.hVj....j
+000147e0: ae01 0000 6ae9 0100 006a fc01 0000 6883  ....j....j....h.
+000147f0: 8694 8194 6ae9 0100 006a a601 0000 6856  ....j....j....hV
+00014800: 8694 8194 8794 8194 8794 8194 6ae9 0100  ............j...
+00014810: 0068 fc68 5a6a f001 0000 6aae 0100 006a  .h.hZj....j....j
+00014820: e901 0000 6afc 0100 0068 8686 9481 946a  ....j....h.....j
+00014830: e901 0000 6aa6 0100 0068 5a86 9481 9487  ....j....hZ.....
+00014840: 9481 9487 9481 946a e901 0000 6a00 0100  .......j....j...
+00014850: 0068 5e6a f001 0000 6aae 0100 006a e901  .h^j....j....j..
+00014860: 0000 6afc 0100 0068 8986 9481 946a e901  ..j....h.....j..
+00014870: 0000 6aa6 0100 0068 5e86 9481 9487 9481  ..j....h^.......
+00014880: 9487 9481 946a e901 0000 6a04 0100 0068  .....j....j....h
+00014890: 626a f001 0000 6aae 0100 006a e901 0000  bj....j....j....
+000148a0: 6afc 0100 0068 8c86 9481 946a e901 0000  j....h.....j....
+000148b0: 6aa6 0100 0068 6286 9481 9487 9481 9487  j....hb.........
+000148c0: 9481 9474 9481 946a f001 0000 286a e901  ...t...j....(j..
+000148d0: 0000 6afc 0100 006a 0a01 0000 6a0f 1800  ..j....j....j...
+000148e0: 0087 9481 946a e901 0000 6afc 0100 006a  .....j....j....j
+000148f0: 0e01 0000 6a13 1800 0087 9481 946a e901  ....j........j..
+00014900: 0000 6afc 0100 006a 1201 0000 6a17 1800  ..j....j....j...
+00014910: 0087 9481 946a e901 0000 6afc 0100 006a  .....j....j....j
+00014920: 1601 0000 6a1b 1800 0087 9481 946a e901  ....j........j..
+00014930: 0000 6afc 0100 0068 e66a 2118 0000 8794  ..j....h.j!.....
+00014940: 8194 6ae9 0100 006a fc01 0000 68ea 6a25  ..j....j....h.j%
+00014950: 1800 0087 9481 946a e901 0000 6afc 0100  .......j....j...
+00014960: 0068 ee6a 2918 0000 8794 8194 6ae9 0100  .h.j).......j...
+00014970: 006a fc01 0000 68f2 6a2d 1800 0087 9481  .j....h.j-......
+00014980: 9474 9481 946a f001 0000 286a e901 0000  .t...j....(j....
+00014990: 68f8 6a35 1800 0086 9481 946a e901 0000  h.j5.......j....
+000149a0: 68fc 6a3d 1800 0086 9481 946a e901 0000  h.j=.......j....
+000149b0: 6a00 0100 006a 4518 0000 8694 8194 6ae9  j....jE.......j.
+000149c0: 0100 006a 0401 0000 6a4d 1800 0086 9481  ...j....jM......
+000149d0: 9474 9481 9487 9481 9487 9481 948c 0144  .t.............D
+000149e0: 946a 7703 0000 6a79 0300 006a 7903 0000  .jw...jy...jy...
+000149f0: 6a7c 0300 0028 6af0 0100 0028 6a52 0100  j|...(j....(jR..
+00014a00: 006a 5601 0000 6a5a 0100 006a 5e01 0000  .jV...jZ...j^...
+00014a10: 6ae9 0100 006a 7601 0000 6ae8 1700 0086  j....jv...j.....
+00014a20: 9481 946a e901 0000 6a7a 0100 006a ec17  ...j....jz...j..
+00014a30: 0000 8694 8194 6ae9 0100 006a 7e01 0000  ......j....j~...
+00014a40: 6af0 1700 0086 9481 946a e901 0000 6a82  j........j....j.
+00014a50: 0100 006a f706 0000 8694 8194 7494 8194  ...j........t...
+00014a60: 6abd 0300 006a f001 0000 286a e901 0000  j....j....(j....
+00014a70: 6856 6a76 0100 0086 9481 946a e901 0000  hVjv.......j....
+00014a80: 685a 6a7a 0100 0086 9481 946a e901 0000  hZjz.......j....
+00014a90: 685e 6a7e 0100 0086 9481 946a e901 0000  h^j~.......j....
+00014aa0: 6862 6a82 0100 0086 9481 9474 9481 946a  hbj........t...j
+00014ab0: bd03 0000 6af0 0100 0028 6a64 0100 006a  ....j....(jd...j
+00014ac0: 6801 0000 6a6c 0100 006a 7001 0000 7494  h...jl...jp...t.
+00014ad0: 8194 6abd 0300 006a 8618 0000 6abd 0300  ..j....j....j...
+00014ae0: 006a f001 0000 286a 7601 0000 6a7a 0100  .j....(jv...jz..
+00014af0: 006a 7e01 0000 6a82 0100 0074 9481 9474  .j~...j....t...t
+00014b00: 9481 9487 9481 948c 0561 6c70 6861 946a  .........alpha.j
+00014b10: 7703 0000 6a79 0300 006a 5115 0000 6a7c  w...jy...jQ...j|
+00014b20: 0300 006a e901 0000 6af3 0100 0068 126a  ...j....j....h.j
+00014b30: 7e03 0000 8694 8194 6af0 0100 0028 6ae9  ~.......j....(j.
+00014b40: 0100 0068 126a f001 0000 286a e901 0000  ...h.j....(j....
+00014b50: 2868 236a c901 0000 6a1c 0100 006a f001  (h#j....j....j..
+00014b60: 0000 6867 6a0d 1800 0086 9481 9474 9481  ..hgj........t..
+00014b70: 946a e901 0000 2868 266a cc01 0000 6a20  .j....(h&j....j 
+00014b80: 0100 006a f001 0000 686a 6a0d 1800 0086  ...j....hjj.....
+00014b90: 9481 9474 9481 946a e901 0000 2868 296a  ...t...j....(h)j
+00014ba0: cf01 0000 6a24 0100 006a f001 0000 686d  ....j$...j....hm
+00014bb0: 6a0d 1800 0086 9481 9474 9481 946a e901  j........t...j..
+00014bc0: 0000 2868 2c6a d201 0000 6a28 0100 006a  ..(h,j....j(...j
+00014bd0: f001 0000 6870 6a0d 1800 0086 9481 9474  ....hpj........t
+00014be0: 9481 9474 9481 9486 9481 946a e901 0000  ...t.......j....
+00014bf0: 286a fc01 0000 6823 6ac9 0100 0068 566a  (j....h#j....hVj
+00014c00: f001 0000 6ae9 0100 006a fc01 0000 6891  ....j....j....h.
+00014c10: 6af0 0100 006a e901 0000 68f8 6812 8694  j....j....h.h...
+00014c20: 8194 6ae9 0100 0068 236a c901 0000 6a40  ..j....h#j....j@
+00014c30: 0100 0087 9481 9486 9481 9487 9481 946a  ...............j
+00014c40: e901 0000 6a40 0100 0068 126a f001 0000  ....j@...h.j....
+00014c50: 6aae 0100 006a e901 0000 6afc 0100 0068  j....j....j....h
+00014c60: 8386 9481 946a e901 0000 6aa6 0100 0068  .....j....j....h
+00014c70: 5686 9481 9487 9481 9487 9481 9486 9481  V...............
+00014c80: 9474 9481 946a e901 0000 286a fc01 0000  .t...j....(j....
+00014c90: 6826 6acc 0100 0068 5a6a f001 0000 6ae9  h&j....hZj....j.
+00014ca0: 0100 006a fc01 0000 6894 6af0 0100 006a  ...j....h.j....j
+00014cb0: e901 0000 68fc 6812 8694 8194 6ae9 0100  ....h.h.....j...
+00014cc0: 0068 266a cc01 0000 6a44 0100 0087 9481  .h&j....jD......
+00014cd0: 9486 9481 9487 9481 946a e901 0000 6a44  .........j....jD
+00014ce0: 0100 0068 126a f001 0000 6aae 0100 006a  ...h.j....j....j
+00014cf0: e901 0000 6afc 0100 0068 8686 9481 946a  ....j....h.....j
+00014d00: e901 0000 6aa6 0100 0068 5a86 9481 9487  ....j....hZ.....
+00014d10: 9481 9487 9481 9486 9481 9474 9481 946a  ...........t...j
+00014d20: e901 0000 286a fc01 0000 6829 6acf 0100  ....(j....h)j...
+00014d30: 0068 5e6a f001 0000 6ae9 0100 006a fc01  .h^j....j....j..
+00014d40: 0000 6897 6af0 0100 006a e901 0000 6a00  ..h.j....j....j.
+00014d50: 0100 0068 1286 9481 946a e901 0000 6829  ...h.....j....h)
+00014d60: 6acf 0100 006a 4801 0000 8794 8194 8694  j....jH.........
+00014d70: 8194 8794 8194 6ae9 0100 006a 4801 0000  ......j....jH...
+00014d80: 6812 6af0 0100 006a ae01 0000 6ae9 0100  h.j....j....j...
+00014d90: 006a fc01 0000 6889 8694 8194 6ae9 0100  .j....h.....j...
+00014da0: 006a a601 0000 685e 8694 8194 8794 8194  .j....h^........
+00014db0: 8794 8194 8694 8194 7494 8194 6ae9 0100  ........t...j...
+00014dc0: 0028 6afc 0100 0068 2c6a d201 0000 6862  .(j....h,j....hb
+00014dd0: 6af0 0100 006a e901 0000 6afc 0100 0068  j....j....j....h
+00014de0: 9a6a f001 0000 6ae9 0100 006a 0401 0000  .j....j....j....
+00014df0: 6812 8694 8194 6ae9 0100 0068 2c6a d201  h.....j....h,j..
+00014e00: 0000 6a4c 0100 0087 9481 9486 9481 9487  ..jL............
+00014e10: 9481 946a e901 0000 6a4c 0100 0068 126a  ...j....jL...h.j
+00014e20: f001 0000 6aae 0100 006a e901 0000 6afc  ....j....j....j.
+00014e30: 0100 0068 8c86 9481 946a e901 0000 6aa6  ...h.....j....j.
+00014e40: 0100 0068 6286 9481 9487 9481 9487 9481  ...hb...........
+00014e50: 9486 9481 9474 9481 9474 9481 9486 9481  .....t...t......
+00014e60: 946a e901 0000 6af3 0100 0068 126a fc01  .j....j....h.j..
+00014e70: 0000 8694 8194 6af0 0100 0028 6ae9 0100  ......j....(j...
+00014e80: 0028 6823 6ac9 0100 006a 2e01 0000 6af0  .(h#j....j....j.
+00014e90: 0100 0068 756a e901 0000 6afc 0100 006a  ...huj....j....j
+00014ea0: aa01 0000 8694 8194 8694 8194 7494 8194  ............t...
+00014eb0: 6ae9 0100 0028 6826 6acc 0100 006a 3201  j....(h&j....j2.
+00014ec0: 0000 6af0 0100 0068 786a fd18 0000 8694  ..j....hxj......
+00014ed0: 8194 7494 8194 6ae9 0100 0028 6829 6acf  ..t...j....(h)j.
+00014ee0: 0100 006a 3601 0000 6af0 0100 0068 7b6a  ...j6...j....h{j
+00014ef0: fd18 0000 8694 8194 7494 8194 6ae9 0100  ........t...j...
+00014f00: 0028 682c 6ad2 0100 006a 3a01 0000 6af0  .(h,j....j:...j.
+00014f10: 0100 0068 7e6a fd18 0000 8694 8194 7494  ...h~j........t.
+00014f20: 8194 7494 8194 8694 8194 6ae9 0100 006a  ..t.......j....j
+00014f30: 9118 0000 6af0 0100 0028 6ae9 0100 006a  ....j....(j....j
+00014f40: fc01 0000 6812 6af0 0100 0028 6ae9 0100  ....h.j....(j...
+00014f50: 0028 6823 6ac9 0100 006a 4001 0000 6a35  .(h#j....j@...j5
+00014f60: 1800 0074 9481 946a e901 0000 2868 266a  ...t...j....(h&j
+00014f70: cc01 0000 6a44 0100 006a 3d18 0000 7494  ....jD...j=...t.
+00014f80: 8194 6ae9 0100 0028 6829 6acf 0100 006a  ..j....(h)j....j
+00014f90: 4801 0000 6a45 1800 0074 9481 946a e901  H...jE...t...j..
+00014fa0: 0000 2868 2c6a d201 0000 6a4c 0100 006a  ..(h,j....jL...j
+00014fb0: 4d18 0000 7494 8194 7494 8194 8794 8194  M...t...t.......
+00014fc0: 6ae9 0100 0028 6891 6823 6ac9 0100 006a  j....(h.h#j....j
+00014fd0: ab18 0000 7494 8194 6ae9 0100 0028 6894  ....t...j....(h.
+00014fe0: 6826 6acc 0100 006a bf18 0000 7494 8194  h&j....j....t...
+00014ff0: 6ae9 0100 0028 6897 6829 6acf 0100 006a  j....(h.h)j....j
+00015000: d318 0000 7494 8194 6ae9 0100 0028 689a  ....t...j....(h.
+00015010: 682c 6ad2 0100 006a e718 0000 7494 8194  h,j....j....t...
+00015020: 7494 8194 8694 8194 8794 8194 8794 8194  t...............
+00015030: 7575 2e                                  uu.
```

### Comparing `jsrm-0.0.6/src/jsrm/symbolic_expressions/planar_pcs_ns-1.dill` & `jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_pcs_ns-1.dill`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/symbolic_expressions/planar_pcs_ns-2.dill` & `jsrm-0.0.7/src/jsrm/symbolic_expressions/planar_pcs_ns-2.dill`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/systems/euler_lagrangian.py` & `jsrm-0.0.7/src/jsrm/systems/euler_lagrangian.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/systems/pendulum.py` & `jsrm-0.0.7/src/jsrm/systems/pendulum.py`

 * *Files identical despite different names*

### Comparing `jsrm-0.0.6/src/jsrm/systems/planar_hsa.py` & `jsrm-0.0.7/src/jsrm/systems/planar_hsa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import dill
 from jax import Array, jit, lax, vmap
 from jax import numpy as jnp
 import sympy as sp
 from pathlib import Path
-from typing import Callable, Dict, List, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
 from .utils import (
     concatenate_params_syms,
     compute_strain_basis,
 )
 
 
 def factory(
     sym_exp_filepath: Union[str, Path],
     strain_selector: Array = None,
     global_eps: float = 1e-6,
+    consider_hysteresis: bool = False,
 ) -> Tuple[
     Callable[[Dict[str, Array], Array, Array], Array],
     Callable[[Dict[str, Array], Array, Array], Array],
     Callable[[Dict[str, Array], Array], Array],
     Callable[[Dict[str, Array], Array], Array],
     Callable[[Dict[str, Array], Array], Array],
     Dict,
@@ -26,14 +27,15 @@
     """
     Create jax functions from file containing symbolic expressions.
     Args:
         sym_exp_filepath: path to file containing symbolic expressions
         strain_selector: array of shape (n_xi, ) with boolean values indicating which components of the
                 strain are active / non-zero
         global_eps: small number to avoid singularities (e.g., division by zero)
+        consider_hysteresis: If True, Bouc-Wen is used to model hysteresis. Otherwise, hysteresis will be neglected.
     Returns:
         forward_kinematics_virtual_backbone_fn: function that returns the chi vector of shape (3, n_q) with the
             positions and orientations of the virtual backbone
         forward_kinematics_end_effector_fn: function that returns the pose of the end effector of shape (3, )
         jacobian_end_effector_fn: function that returns the Jacobian of the end effector of shape (3, n_q)
         inverse_kinematics_end_effector_fn: function that returns the generalized coordinates for a given end-effector pose
         dynamical_matrices_fn: function that returns the B, C, G, K, D, and alpha matrices
@@ -144,14 +146,15 @@
     )
     C_lambda = sp.lambdify(
         params_syms_cat + state_syms_cat, sym_exps["exps"]["C"], "jax"
     )
     G_lambda = sp.lambdify(
         params_syms_cat + sym_exps["state_syms"]["xi"], sym_exps["exps"]["G"], "jax"
     )
+    Shat_lambda = sp.lambdify(params_syms_cat, sym_exps["exps"]["Shat"], "jax")
     K_lambda = sp.lambdify(
         params_syms_cat + sym_exps["state_syms"]["xi"], sym_exps["exps"]["K"], "jax"
     )
     D_lambda = sp.lambdify(params_syms_cat, sym_exps["exps"]["D"], "jax")
     alpha_lambda = sp.lambdify(
         params_syms_cat + sym_exps["state_syms"]["xi"] + sym_exps["state_syms"]["phi"],
         sym_exps["exps"]["alpha"],
@@ -248,19 +251,22 @@
         xi_bend_sign = jnp.where(xi_bend_sign == 0, 1, xi_bend_sign)
         # add eps to the bending strain (i.e. the first column)
         sigma_b_epsed = lax.select(
             jnp.abs(xi_reshaped[:, 0]) < _eps,
             xi_bend_sign * _eps,
             xi_reshaped[:, 0],
         )
-        xi_epsed = jnp.stack([
-            sigma_b_epsed,
-            xi_reshaped[:, 1],
-            xi_reshaped[:, 2],
-        ], axis=1)
+        xi_epsed = jnp.stack(
+            [
+                sigma_b_epsed,
+                xi_reshaped[:, 1],
+                xi_reshaped[:, 2],
+            ],
+            axis=1,
+        )
 
         # old implementation:
         # xi_epsed = xi_reshaped
         # xi_epsed = xi_epsed.at[:, 0].add(xi_bend_sign * _eps)
 
         # flatten the array
         xi_epsed = xi_epsed.flatten()
@@ -309,15 +315,19 @@
             segment_idx, chiv_lambda_sms, *params_for_lambdify, *xi_epsed, s_segment
         ).squeeze()
 
         return chi
 
     @jit
     def forward_kinematics_rod_fn(
-        params: Dict[str, Array], q: Array, s: Array, rod_idx: Array, eps: float = global_eps
+        params: Dict[str, Array],
+        q: Array,
+        s: Array,
+        rod_idx: Array,
+        eps: float = global_eps,
     ) -> Array:
         """
         Evaluate the forward kinematics of the physical rods
         Args:
             params: Dictionary of robot parameters
             q: generalized coordinates of shape (n_q, )
             s: point coordinate along the rod in the interval [0, L].
@@ -390,15 +400,17 @@
         chip = lax.switch(
             segment_idx, chip_lambda_sms, *params_for_lambdify, *xi_epsed
         ).squeeze()
 
         return chip
 
     @jit
-    def forward_kinematics_end_effector_fn(params: Dict[str, Array], q: Array, eps: float = global_eps) -> Array:
+    def forward_kinematics_end_effector_fn(
+        params: Dict[str, Array], q: Array, eps: float = global_eps
+    ) -> Array:
         """
         Evaluate the forward kinematics of the end-effector
         Args:
             params: Dictionary of robot parameters
             q: generalized coordinates of shape (n_q, )
             eps: small number to avoid singularities (e.g., division by zero)
         Returns:
@@ -416,15 +428,17 @@
         params_for_lambdify = select_params_for_lambdify_fn(params)
         # evaluate the symbolic expression
         chiee = chiee_lambda(*params_for_lambdify, *xi_epsed).squeeze()
 
         return chiee
 
     @jit
-    def jacobian_end_effector_fn(params: Dict[str, Array], q: Array, eps: float = global_eps) -> Array:
+    def jacobian_end_effector_fn(
+        params: Dict[str, Array], q: Array, eps: float = global_eps
+    ) -> Array:
         """
         Evaluate the Jacobian of the end-effector
         Args:
            params: Dictionary of robot parameters
            q: generalized coordinates of shape (n_q, )
            eps: small number to avoid singularities (e.g., division by zero)
         Returns:
@@ -539,23 +553,25 @@
         return q
 
     @jit
     def dynamical_matrices_fn(
         params: Dict[str, Array],
         q: Array,
         q_d: Array,
+        z: Optional[Array] = None,
         phi: Array = jnp.zeros((num_segments * num_rods_per_segment,)),
         eps: float = 1e4 * global_eps,
     ) -> Tuple[Array, Array, Array, Array, Array, Array]:
         """
         Compute the dynamical matrices of the system.
         Args:
             params: Dictionary of robot parameters
             q: generalized coordinates of shape (n_q, )
             q_d: generalized velocities of shape (n_q, )
+            z: state variables of the hysteresis model of shape (n_z, )
             phi: motor positions / twist angles of shape (num_segments * num_rods_per_segment, )
             eps: small number to avoid singularities (e.g., division by zero)
         Returns:
             B: mass / inertia matrix of shape (n_q, n_q)
             C: coriolis / centrifugal matrix of shape (n_q, n_q)
             G: gravity vector of shape (n_q, )
             K: elastic vector of shape (n_q, )
@@ -571,29 +587,44 @@
 
         # evaluate the symbolic expressions
         params_for_lambdify = select_params_for_lambdify_fn(params)
         B = B_lambda(*params_for_lambdify, *xi_epsed)
         C_xi = C_lambda(*params_for_lambdify, *xi_epsed, *xi_d)
         G = G_lambda(*params_for_lambdify, *xi_epsed).squeeze()
         K = K_lambda(*params_for_lambdify, *xi).squeeze()
+        Shat = Shat_lambda(*params_for_lambdify)
         D = D_lambda(*params_for_lambdify)
         alpha = alpha_lambda(*params_for_lambdify, *xi, *phi).squeeze()
 
+        if consider_hysteresis is True:
+            # hysteresis parameters
+            B_z = params["hysteresis"]["basis"]
+            hyst_alpha = params["hysteresis"]["alpha"]
+            # add the post-yield potential forces
+            K = hyst_alpha * K + (1 - hyst_alpha) * Shat @ (B_z @ z)
+
+            # TODO: add post-yield potential forces (i.e., hysteresis effects) to the actuation vector
+
         # apply the strain basis
         B = B_xi.T @ B @ B_xi
         C = B_xi.T @ C_xi @ B_xi
         G = B_xi.T @ G
         K = B_xi.T @ K
         D = B_xi.T @ D @ B_xi
         alpha = B_xi.T @ alpha
 
         return B, C, G, K, D, alpha
 
     def operational_space_dynamical_matrices_fn(
-        params: Dict[str, Array], q: Array, q_d: Array, B: Array, C: Array, eps: float = 1e4 * global_eps
+        params: Dict[str, Array],
+        q: Array,
+        q_d: Array,
+        B: Array,
+        C: Array,
+        eps: float = 1e4 * global_eps,
     ) -> Tuple[Array, Array, Array, Array, Array]:
         """
         Compute the dynamics in operational space.
         The implementation is based on Chapter 7.8 of "Modelling, Planning and Control of Robotics" by
         Siciliano, Sciavicco, Villani, Oriolo.
         Args:
             params: dictionary of parameters
@@ -623,18 +654,24 @@
         # end-effector Jacobian and its time-derivative
         Jee = Jee_lambda(*params_for_lambdify, *xi_epsed)
         Jee_d = Jee_d_lambda(*params_for_lambdify, *xi_epsed, *xi_d)
 
         # inverse of the inertia matrix in the configuration space
         B_inv = jnp.linalg.inv(B)
 
-        Lambda = jnp.linalg.inv(Jee @ B_inv @ Jee.T)  # inertia matrix in the operational space
-        mu = Lambda @ (Jee @ B_inv @ C - Jee_d)  # coriolis and centrifugal matrix in the operational space
-
-        JeeB_pinv = B_inv @ Jee.T @ Lambda  # dynamically-consistent pseudo-inverse of the Jacobian
+        Lambda = jnp.linalg.inv(
+            Jee @ B_inv @ Jee.T
+        )  # inertia matrix in the operational space
+        mu = Lambda @ (
+            Jee @ B_inv @ C - Jee_d
+        )  # coriolis and centrifugal matrix in the operational space
+
+        JeeB_pinv = (
+            B_inv @ Jee.T @ Lambda
+        )  # dynamically-consistent pseudo-inverse of the Jacobian
 
         return Lambda, mu, Jee, Jee_d, JeeB_pinv
 
     sys_helpers = {
         "eps": global_eps,
         "select_params_for_lambdify_fn": select_params_for_lambdify_fn,
         "beta_fn": beta_fn,
@@ -657,69 +694,100 @@
         sys_helpers,
     )
 
 
 def ode_factory(
     dynamical_matrices_fn: Callable,
     params: Dict[str, Array],
+    control_fn: Optional[Callable] = None,
     consider_underactuation_model: bool = True,
+    consider_hysteresis: bool = False,
 ) -> Callable[[float, Array], Array]:
     """
     Make an ODE function of the form ode_fn(t, x) -> x_dot.
     This function assumes a constant torque input (i.e. zero-order hold).
     Args:
         dynamical_matrices_fn: Callable that returns B, C, G, K, D, alpha_fn. Needs to conform to the signature:
-            dynamical_matrices_fn(params, q, q_d) -> Tuple[B, C, G, K, D, A]
+            dynamical_matrices_fn(params, q, q_d, z, phi) -> Tuple[B, C, G, K, D, A]
             where q and q_d are the configuration and velocity vectors, respectively,
             B is the inertia matrix of shape (n_q, n_q),
             C is the Coriolis matrix of shape (n_q, n_q),
             G is the gravity vector of shape (n_q, ),
             K is the stiffness vector of shape (n_q, ),
             D is the damping matrix of shape (n_q, n_q),
             alpha_fn is a function to compute the actuation vector of shape (n_q). It has the following signature:
                 alpha_fn(phi) -> tau_q where phi is the twist angle vector of shape (n_phi, )
         params: Dictionary with robot parameters
+        control_fn: Callable that returns the forcing function of the form control_fn(t, x) -> u. If consider_underactuation_model is True,
+            then u is an array of shape (n_q, ) with the configuration-space torques. If consider_underactuation_model is False,
+            then u is an array of shape (n_phi, ) with the motor positions / twist angles of the proximal end of the rods.
         consider_underactuation_model: If True, the underactuation model is considered. Otherwise, the fully-actuated
             model is considered with the identity matrix as the actuation matrix.
+        consider_hysteresis: If True, Bouc-Wen is used to model hysteresis. Otherwise, hysteresis will be neglected.
     Returns:
         ode_fn: ODE function of the form ode_fn(t, x) -> x_dot
     """
     num_rods = params["rout"].shape[0] * params["rout"].shape[1]
 
     @jit
     def ode_fn(t: float, x: Array, u: Array) -> Array:
         """
         ODE of the dynamical Lagrangian system.
         Args:
             t: time
-            x: state vector of shape (2 * n_q, )
+            x: state vector of shape (2 * n_q + n_z, ) where n_q is the number of configuration variables and n_z is the
+                number of state variables of the hysteresis model. The state vector is of the form [q, q_d, z]
             u: input to the system.
                 - if consider_underactuation_model is True, then this is an array of shape (n_phi) with
                     motor positions / twist angles of the proximal end of the rods
                 - if consider_underactuation_model is False, then this is an array of shape (n_q) with
                     the generalized torques
         Returns:
             x_d: time-derivative of the state vector of shape (2 * n_q, )
         """
-        n_q = x.shape[0] // 2
-        q, q_d = x[:n_q], x[n_q:]
+        if consider_hysteresis is True:
+            hys_params = params["hysteresis"]
+            B_z = hys_params["basis"]
+
+            n_z = B_z.shape[1]
+            n_q = (x.shape[0] - n_z) // 2
+            q, q_d, z = x[:n_q], x[n_q : 2 * n_q], x[2 * n_q :]
+
+            z_d = (B_z.T @ q_d) * (
+                hys_params["A"]
+                - jnp.abs(z) ** hys_params["n"]
+                * (
+                    hys_params["gamma"]
+                    + hys_params["beta"] * jnp.sign((B_z.T @ q_d) * z)
+                )
+            )
+        else:
+            n_q = x.shape[0] // 2
+            q, q_d = x[:n_q], x[n_q:]
+            z = None
+
+        if control_fn is not None:
+            u = u + control_fn(t, x)
 
         if consider_underactuation_model is True:
             phi = u
-            B, C, G, K, D, tau_q = dynamical_matrices_fn(params, q, q_d, phi)
+            B, C, G, K, D, tau_q = dynamical_matrices_fn(params, q, q_d, z=z, phi=phi)
         else:
             B, C, G, K, D, _ = dynamical_matrices_fn(
-                params, q, q_d, jnp.zeros((num_rods,))
+                params, q, q_d, z=z, phi=jnp.zeros((num_rods,))
             )
             tau_q = u
 
         # inverse of B
         B_inv = jnp.linalg.inv(B)
 
         # compute the acceleration
         q_dd = B_inv @ (tau_q - C @ q_d - G - K - D @ q_d)
 
-        x_d = jnp.concatenate([x[n_q:], q_dd])
+        if consider_hysteresis is True:
+            x_d = jnp.concatenate([q_d, q_dd, z_d])
+        else:
+            x_d = jnp.concatenate([x[n_q:], q_dd])
 
         return x_d
 
     return ode_fn
```

### Comparing `jsrm-0.0.6/src/jsrm/systems/planar_pcs.py` & `jsrm-0.0.7/src/jsrm/systems/planar_pcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,31 +126,36 @@
         xi_bend_sign = jnp.where(xi_bend_sign == 0, 1, xi_bend_sign)
         # add eps to the bending strain (i.e. the first column)
         sigma_b_epsed = lax.select(
             jnp.abs(xi_reshaped[:, 0]) < _eps,
             xi_bend_sign * _eps,
             xi_reshaped[:, 0],
         )
-        xi_epsed = jnp.stack([
-            sigma_b_epsed,
-            xi_reshaped[:, 1],
-            xi_reshaped[:, 2],
-        ], axis=1)
+        xi_epsed = jnp.stack(
+            [
+                sigma_b_epsed,
+                xi_reshaped[:, 1],
+                xi_reshaped[:, 2],
+            ],
+            axis=1,
+        )
 
         # old implementation:
         # xi_epsed = xi_reshaped
         # xi_epsed = xi_epsed.at[:, 0].add(xi_bend_sign * _eps)
 
         # flatten the array
         xi_epsed = xi_epsed.flatten()
 
         return xi_epsed
 
     @jit
-    def forward_kinematics_fn(params: Dict[str, Array], q: Array, s: Array, eps: float = global_eps) -> Array:
+    def forward_kinematics_fn(
+        params: Dict[str, Array], q: Array, s: Array, eps: float = global_eps
+    ) -> Array:
         """
         Evaluate the forward kinematics the tip of the links
         Args:
             params: Dictionary of robot parameters
             q: generalized coordinates of shape (n_q, )
             s: point coordinate along the rod in the interval [0, L].
             eps: small number to avoid singularities (e.g., division by zero)
```

### Comparing `jsrm-0.0.6/src/jsrm/systems/utils.py` & `jsrm-0.0.7/src/jsrm/systems/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     params_syms = sym_exps["params_syms"]
     # symbolic expressions
     exps = deepcopy(sym_exps["exps"])
 
     for exp_key, exp_val in exps.items():
         if issubclass(type(exp_val), list):
             for exp_item_idx, exp_item_val in enumerate(exp_val):
-                exps[exp_key][
-                    exp_item_idx
-                ] = substitute_params_into_single_symbolic_expression(
-                    exp_item_val, params_syms, params
+                exps[exp_key][exp_item_idx] = (
+                    substitute_params_into_single_symbolic_expression(
+                        exp_item_val, params_syms, params
+                    )
                 )
         else:
             exps[exp_key] = substitute_params_into_single_symbolic_expression(
                 exp_val, params_syms, params
             )
 
     return exps
@@ -70,15 +70,15 @@
             if param_sym in sym_exp.free_symbols:
                 sym_exp = sym_exp.subs(param_sym, params[param_key])
 
     return sym_exp
 
 
 def concatenate_params_syms(
-    params_syms: Dict[str, Union[sp.Symbol, List[sp.Symbol]]]
+    params_syms: Dict[str, Union[sp.Symbol, List[sp.Symbol]]],
 ) -> List[sp.Symbol]:
     # concatenate the robot params symbols
     params_syms_cat = []
     for params_key, params_sym in sorted(params_syms.items()):
         if type(params_sym) in [list, tuple]:
             params_syms_cat += params_sym
         else:
```

### Comparing `jsrm-0.0.6/src/jsrm.egg-info/PKG-INFO` & `jsrm-0.0.7/src/jsrm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsrm
-Version: 0.0.6
+Version: 0.0.7
 Summary: Kinematic and dynamic models of continuum and articulated soft robots.
 Author-email: Maximilian Stölzle <maximilian@stoelzle.ch>
 Maintainer-email: Maximilian Stölzle <maximilian@stoelzle.ch>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -42,23 +42,23 @@
 License-File: LICENSE.txt
 Requires-Dist: dill
 Requires-Dist: jax
 Requires-Dist: numpy
 Requires-Dist: peppercorn
 Requires-Dist: sympy>=1.11
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: codecov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-html; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Provides-Extra: examples
 Requires-Dist: diffrax; extra == "examples"
 Requires-Dist: matplotlib; extra == "examples"
 Requires-Dist: opencv-python; extra == "examples"
 Provides-Extra: test
 Requires-Dist: codecov; extra == "test"
@@ -67,15 +67,15 @@
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-html; extra == "test"
 Requires-Dist: tox; extra == "test"
 
 # JAX Soft Robot Modelling
 
 This repository contains symbolic derivations of the kinematics and dynamics of various soft robots using Sympy.
-The symbolic expressions are then implemented in JAX used for fast, parallelizable, and differentiable simulations.
+The symbolic expressions are then implemented in JAX and can be used for fast, parallelizable, and differentiable simulations.
 So far, we have focused on planar settings and implemented the following soft robots:
 
 - [N-link pendulum](examples/simulate_pendulum.py)
 - [Planar Piecewise Constant Strain (PCS) continuum soft robot](examples/simulate_planar_pcs.py)
 - [Planar Handed Shearing Auxetics (HSA) robot](examples/simulate_planar_hsa.py)
 
 We are happy to receive contributions for other soft robots and/or other settings (e.g., 3D).
@@ -116,23 +116,34 @@
 
 ```bash
 pip install ".[examples]"
 ```
 
 ## Usage
 
-Always, first source all necessary environment variables when opening a new terminal:
+Always first source all necessary environment variables when opening a new terminal:
 
 ```bash
 source 01-configure-env-vars.sh
 ```
 
-Then, we can symbolically derive the pendulum kinematics and dynamics
+Then, we can symbolically derive the pendulum kinematics and dynamics:
 
 ```bash
 python examples/derive_pendulum.py
 ```
 
 Finally, we can simulate the pendulum
 ```bash
 python examples/simulate_pendulum.py
 ```
+
+## See also
+
+You might also be interested in the following repositories:
+ - The [`jax-spcs-kinematics`](https://github.com/tud-phi/jax-spcs-kinematics) repository contains an implementation
+ of the Selective Piecewise Constant Strain (SPCS) kinematics in JAX. We have shown in our paper that this kinematic 
+model is suitable for representing the shape of HSA rods.
+ - The [`HSA-PyElastica`](https://github.com/tud-phi/HSA-PyElastica) repository contains a plugin for PyElastica
+for the simulation of HSA robots.
+ - The [`hsa-planar-control`](https://github.com/tud-phi/hsa-planar-control) repository contains JAX and ROS2 implementations
+ of model-based control algorithms for planar HSA robots.
```

### Comparing `jsrm-0.0.6/src/jsrm.egg-info/SOURCES.txt` & `jsrm-0.0.7/src/jsrm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 src/jsrm.egg-info/PKG-INFO
 src/jsrm.egg-info/SOURCES.txt
 src/jsrm.egg-info/dependency_links.txt
 src/jsrm.egg-info/requires.txt
 src/jsrm.egg-info/top_level.txt
 src/jsrm/parameters/__init__.py
 src/jsrm/parameters/hsa_params.py
+src/jsrm/rendering/__init__.py
+src/jsrm/rendering/planar_hsa/opencv_renderer.py
 src/jsrm/symbolic_derivation/__init__.py
 src/jsrm/symbolic_derivation/pendulum.py
 src/jsrm/symbolic_derivation/planar_hsa.py
 src/jsrm/symbolic_derivation/planar_pcs.py
 src/jsrm/symbolic_derivation/symbolic_utils.py
 src/jsrm/symbolic_expressions/pendulum_nl-1.dill
 src/jsrm/symbolic_expressions/pendulum_nl-2.dill
```

### Comparing `jsrm-0.0.6/tests/test_planar_hsa.py` & `jsrm-0.0.7/tests/test_planar_hsa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import dill
-from jax import config as jax_config
+import jax
 
-jax_config.update("jax_enable_x64", True)  # double precision
+jax.config.update("jax_enable_x64", True)  # double precision
 from jax import Array, jit, random
 from jax import numpy as jnp
 import jsrm
 from pathlib import Path
 import sympy as sp
 from typing import Tuple
```

### Comparing `jsrm-0.0.6/tests/test_planar_pcs.py` & `jsrm-0.0.7/tests/test_planar_pcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from jax import config as jax_config
+import jax
 
-jax_config.update("jax_enable_x64", True)  # double precision
+jax.config.update("jax_enable_x64", True)  # double precision
 from jax import numpy as jnp
 import jsrm
 from functools import partial
 from numpy.testing import assert_allclose
 from pathlib import Path
 
 from jsrm.systems import planar_pcs, euler_lagrangian
```


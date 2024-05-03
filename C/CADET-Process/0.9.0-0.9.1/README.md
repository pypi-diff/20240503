# Comparing `tmp/CADET-Process-0.9.0.tar.gz` & `tmp/cadet_process-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CADET-Process-0.9.0.tar", last modified: Fri Apr 12 13:00:53 2024, max compression
+gzip compressed data, was "cadet_process-0.9.1.tar", last modified: Fri May  3 11:47:14 2024, max compression
```

## Comparing `CADET-Process-0.9.0.tar` & `cadet_process-0.9.1.tar`

### file list

```diff
@@ -1,148 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.299767 CADET-Process-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.279767 CADET-Process-0.9.0/CADETProcess/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/CADETProcessError.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.279767 CADET-Process-0.9.0/CADETProcess/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11838 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/comparison/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29103 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/comparison/difference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/comparison/peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/comparison/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.283767 CADET-Process-0.9.0/CADETProcess/dataStructure/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/dataStructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/diskcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/nested_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    46781 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dataStructure/parameter_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.283767 CADET-Process-0.9.0/CADETProcess/dynamicEvents/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dynamicEvents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46703 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dynamicEvents/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    23338 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/dynamicEvents/section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.283767 CADET-Process-0.9.0/CADETProcess/equilibria/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/equilibria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11300 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/equilibria/buffer_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/equilibria/initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/equilibria/ptc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/equilibria/reaction_equilibria.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.283767 CADET-Process-0.9.0/CADETProcess/fractionation/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/fractionation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/fractionation/fractionationOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23970 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/fractionation/fractionator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/fractionation/fractions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.283767 CADET-Process-0.9.0/CADETProcess/modelBuilder/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/modelBuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46700 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/modelBuilder/carouselBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/modelBuilder/compartmentBuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.287767 CADET-Process-0.9.0/CADETProcess/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19931 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/axAdapater.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/individual.py
--rw-r--r--   0 runner    (1001) docker     (127)   123858 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/optimizationProblem.py
--rw-r--r--   0 runner    (1001) docker     (127)    22925 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/parallelizationBackend.py
--rw-r--r--   0 runner    (1001) docker     (127)    30874 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/population.py
--rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/pymooAdapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    20819 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/optimization/scipyAdapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11521 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.287767 CADET-Process-0.9.0/CADETProcess/processModel/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40576 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/componentSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    23039 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    30805 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/flowSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25841 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/process.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24710 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/solutionRecorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    33320 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/processModel/unitOperation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/simulationResults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.287767 CADET-Process-0.9.0/CADETProcess/simulator/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63873 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/simulator/cadetAdapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/simulator/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/smoothing2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51247 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/stationarity.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/sysinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/CADETProcess/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/tools/yamamoto.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/CADETProcess/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.299767 CADET-Process-0.9.0/CADET_Process.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-12 13:00:53.000000 CADET-Process-0.9.0/CADET_Process.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-12 13:00:53.000000 CADET-Process-0.9.0/CADET_Process.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:00:53.000000 CADET-Process-0.9.0/CADET_Process.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 13:00:53.000000 CADET-Process-0.9.0/CADET_Process.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 13:00:53.000000 CADET-Process-0.9.0/CADET_Process.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-12 13:00:53.299767 CADET-Process-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/examples/batch_elution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/batch_elution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/batch_elution/optimization_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/batch_elution/optimization_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/batch_elution/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/examples/characterize_chromatographic_system/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/Yamamoto_method.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/binding_model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/column_transport_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/particle_porosity.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/characterize_chromatographic_system/system_periphery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/examples/load_wash_elute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/load_wash_elute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/load_wash_elute/lwe_concentration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/load_wash_elute/lwe_flow_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/load_wash_elute/lwe_hic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.291767 CADET-Process-0.9.0/examples/recycling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/recycling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/recycling/clr_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/examples/recycling/mrssr_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-12 13:00:53.303767 CADET-Process-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:53.299767 CADET-Process-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22567 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/optimization_problem_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_buffer_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_cadet_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_cadet_reactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20831 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_carousel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_compartment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_difference.py
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (127)    34020 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    30279 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_flow_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_fractions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_individual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_optimization_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    46428 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_optimization_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_optimizer_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_parallelization_adapter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19841 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_population.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_pymoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    16395 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)    19464 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-12 13:00:49.000000 CADET-Process-0.9.0/tests/test_unit_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.764804 cadet_process-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.740803 cadet_process-0.9.1/CADETProcess/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/CADETProcessError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.740803 cadet_process-0.9.1/CADETProcess/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/comparison/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30202 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/comparison/difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/comparison/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/comparison/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.740803 cadet_process-0.9.1/CADETProcess/dataStructure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dataStructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dataStructure/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dataStructure/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dataStructure/dataStructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dataStructure/diskcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dataStructure/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dataStructure/nested_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46781 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dataStructure/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dataStructure/parameter_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.744803 cadet_process-0.9.1/CADETProcess/dynamicEvents/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dynamicEvents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46914 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dynamicEvents/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23623 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/dynamicEvents/section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.744803 cadet_process-0.9.1/CADETProcess/equilibria/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/equilibria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11300 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/equilibria/buffer_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/equilibria/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/equilibria/ptc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/equilibria/reaction_equilibria.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.744803 cadet_process-0.9.1/CADETProcess/fractionation/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/fractionation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/fractionation/fractionationOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24630 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/fractionation/fractionator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/fractionation/fractions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.744803 cadet_process-0.9.1/CADETProcess/modelBuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/modelBuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46700 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/modelBuilder/carouselBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/modelBuilder/compartmentBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.748803 cadet_process-0.9.1/CADETProcess/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/optimization/axAdapater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/optimization/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/optimization/individual.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127333 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/optimization/optimizationProblem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22925 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/optimization/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/optimization/parallelizationBackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32503 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/optimization/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/optimization/pymooAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29697 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/optimization/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20819 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/optimization/scipyAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11521 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.748803 cadet_process-0.9.1/CADETProcess/processModel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/processModel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40576 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/processModel/binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/processModel/componentSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23039 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/processModel/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30805 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/processModel/flowSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25841 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/processModel/process.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24710 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/processModel/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/processModel/solutionRecorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33320 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/processModel/unitOperation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/simulationResults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.752803 cadet_process-0.9.1/CADETProcess/simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63873 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/simulator/cadetAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/simulator/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/smoothing2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51247 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/stationarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/sysinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.752803 cadet_process-0.9.1/CADETProcess/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/tools/yamamoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-03 11:47:07.000000 cadet_process-0.9.1/CADETProcess/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.760804 cadet_process-0.9.1/CADET_Process.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-03 11:47:14.000000 cadet_process-0.9.1/CADET_Process.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-03 11:47:14.000000 cadet_process-0.9.1/CADET_Process.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:47:14.000000 cadet_process-0.9.1/CADET_Process.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-03 11:47:14.000000 cadet_process-0.9.1/CADET_Process.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 11:47:14.000000 cadet_process-0.9.1/CADET_Process.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-03 11:47:07.000000 cadet_process-0.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-03 11:47:14.764804 cadet_process-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-03 11:47:07.000000 cadet_process-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.752803 cadet_process-0.9.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.752803 cadet_process-0.9.1/examples/batch_elution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/batch_elution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/batch_elution/optimization_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/batch_elution/optimization_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/batch_elution/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.752803 cadet_process-0.9.1/examples/characterize_chromatographic_system/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/characterize_chromatographic_system/Yamamoto_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/characterize_chromatographic_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/characterize_chromatographic_system/binding_model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/characterize_chromatographic_system/column_transport_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/characterize_chromatographic_system/particle_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/characterize_chromatographic_system/system_periphery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.756803 cadet_process-0.9.1/examples/load_wash_elute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/load_wash_elute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/load_wash_elute/lwe_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/load_wash_elute/lwe_flow_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/load_wash_elute/lwe_hic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.756803 cadet_process-0.9.1/examples/recycling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/recycling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/recycling/clr_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-03 11:47:07.000000 cadet_process-0.9.1/examples/recycling/mrssr_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-03 11:47:07.000000 cadet_process-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-03 11:47:14.764804 cadet_process-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:14.760804 cadet_process-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22567 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/optimization_problem_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_buffer_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_cadet_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_cadet_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20831 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_carousel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_compartment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13226 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34020 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30279 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_flow_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_fractions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_individual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_optimization_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46428 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_optimization_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_optimizer_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_parallelization_adapter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19841 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_population.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_pymoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16395 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19464 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-03 11:47:07.000000 cadet_process-0.9.1/tests/test_unit_operation.py
```

### Comparing `CADET-Process-0.9.0/CADETProcess/__init__.py` & `cadet_process-0.9.1/CADETProcess/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 advanced chromatographic systems. It serves as an inteface for CADET, but also
 for other solvers.
 
 See https://cadet-process.readthedocs.io for complete documentation.
 """
 # Version information
 name = "CADET-Process"
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 # Imports
 from .CADETProcessError import *
 
 from . import log
 
 from .settings import Settings
```

### Comparing `CADET-Process-0.9.0/CADETProcess/comparison/__init__.py` & `cadet_process-0.9.1/CADETProcess/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/comparison/comparator.py` & `cadet_process-0.9.1/CADETProcess/comparison/comparator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import copy
 import importlib
 import functools
 
 import numpy as np
 import matplotlib.pyplot as plt
+from matplotlib.figure import Figure
+from matplotlib.axes import Axes
 
 from CADETProcess import CADETProcessError
-from CADETProcess import plotting
+from CADETProcess import plotting, SimulationResults
 from CADETProcess.dataStructure import Structure, String
 from CADETProcess.dataStructure import get_nested_value
 from CADETProcess.solution import SolutionBase
 from CADETProcess.comparison import DifferenceBase
 
 
 class Comparator(Structure):
@@ -219,15 +221,17 @@
 
         metrics = np.hstack(metrics).tolist()
 
         return metrics
 
     __call__ = evaluate
 
-    def setup_comparison_figure(self, plot_individual=False):
+    def setup_comparison_figure(
+        self, plot_individual: bool = False
+    ) -> tuple[list[Figure], list[Axes]]:
         """Set up a figure for comparing simulation results.
 
         Parameters
         ----------
         plot_individual : bool, optional
             If True, return figures for individual metrics.
             Otherwise, return a single figure for all metrics.
@@ -245,16 +249,16 @@
             n_rows=self.n_diffference_metrics,
             squeeze=False
         )
 
         plt.close(comparison_fig_all)
         comparison_axs_all = comparison_axs_all.reshape(-1)
 
-        comparison_fig_ind = []
-        comparison_axs_ind = []
+        comparison_fig_ind: list[Figure] = []
+        comparison_axs_ind: list[Axes] = []
         for i in range(self.n_diffference_metrics):
             fig, axs = plt.subplots()
             comparison_fig_ind.append(fig)
             comparison_axs_ind.append(axs)
             plt.close(fig)
 
         comparison_axs_ind = \
@@ -262,17 +266,25 @@
 
         if plot_individual:
             return comparison_fig_ind, comparison_axs_ind
         else:
             return comparison_fig_all, comparison_axs_all
 
     def plot_comparison(
-            self, simulation_results, axs=None, figs=None,
-            file_name=None, show=True, plot_individual=False):
-        """Plot the comparison of the simulation results with the reference data.
+            self,
+            simulation_results: list[SimulationResults],
+            axs: Axes | list[Axes] | None = None,
+            figs: Figure | list[Figure] | None = None,
+            file_name: str | None = None,
+            show: bool = True,
+            plot_individual: bool = False,
+            use_minutes: bool = True,
+            ) -> tuple[list[Figure], list[Axes]]:
+        """
+        Plot the comparison of the simulation results with the reference data.
 
         Parameters
         ----------
         simulation_results : list of SimulationResults
             List of simulation results to compare to reference data.
         axs : list of AxesSubplot, optional
             List of subplot axes to use for plotting the metrics.
@@ -280,14 +292,16 @@
             List of figures to use for plotting the metrics.
         file_name : str, optional
             Name of the file to save the figure to.
         show : bool, optional
             If True, displays the figure(s) on the screen.
         plot_individual : bool, optional
             If True, generates a separate figure for each metric.
+        use_minutes : bool, optional
+            Option to use x-aches (time) in minutes, default is set to True.
 
         Returns
         -------
         figs : list of Figure
             List of figures used for plotting the metrics.
         axs : list of AxesSubplot
             List of subplot axes used for plotting the metrics.
@@ -312,18 +326,19 @@
             )
 
             plot_args = {
                 'linestyle': 'dotted',
                 'color': 'k',
                 'label': 'reference',
             }
-            plotting.add_overlay(
-                ax, metric.reference.solution, metric.reference.time/60,
-                **plot_args
-            )
+            ref_time = metric.reference.time
+            if use_minutes:
+                ref_time = ref_time / 60
+
+            plotting.add_overlay(ax, metric.reference.solution, ref_time, **plot_args)
             ax.legend(loc=1)
 
             m = metric.evaluate(solution_sliced, slice=False)
             m = [
                 np.format_float_scientific(
                     n, precision=2,
                 )
```

### Comparing `CADET-Process-0.9.0/CADETProcess/comparison/difference.py` & `cadet_process-0.9.1/CADETProcess/comparison/difference.py`

 * *Files 6% similar despite different names*

```diff
@@ -462,14 +462,15 @@
 
     """
 
     @wraps(DifferenceBase.__init__)
     def __init__(
             self, *args,
             use_derivative=True, normalize_metrics=True, normalization_factor=None,
+            include_height=True,
             **kwargs):
         """Initialize Shape metric.
 
         Parameters
         ----------
         *args :
             Positional arguments for DifferenceBase.
@@ -479,31 +480,38 @@
         normalize_metrics : bool, optional
             If True, normalize the similarity metrics to a range of [0, 1] using a
             sigmoid function.
             Default is True.
         normalization_factor : float, optional
             Normalization factor used by the sigmoid function.
             Default is None, which sets it to 1/10 of the simulation time.
+        include_height : bool, optional
+            If True, also return a metric for the height difference.
+            If `use_derivative` is also true, also return height differences
+            for the derivatives.
         **kwargs : dict
             Keyword arguments passed to the base class constructor.
 
         """
         super().__init__(*args, **kwargs)
 
         if self.reference.n_comp > 1 and not self.use_total_concentration:
             if self.components is not None and len(self.components) == 1:
                 pass
             else:
                 raise CADETProcessError(
                     "Shape currently only supports single component."
                 )
 
-        self.peak_height = PeakHeight(
-            *args, normalize=False, normalize_metrics=normalize_metrics, **kwargs
-        )
+        self.include_height = include_height
+        if include_height:
+            warn("Peak height will be removed from the Shape difference metric.", DeprecationWarning)
+            self.peak_height = PeakHeight(
+                *args, normalize=False, normalize_metrics=normalize_metrics, **kwargs
+            )
 
         self.use_derivative = use_derivative
         if use_derivative:
             self.reference_der = self.reference.derivative
             self.reference_der.resample(
                 start=self._reference.time[0],
                 end=self._reference.time[-1],
@@ -531,27 +539,38 @@
         self.normalize_metrics = normalize_metrics
         if normalization_factor is None:
             normalization_factor = self.reference.time[-1]/10
         self.normalization_factor = normalization_factor
 
     @property
     def n_metrics(self):
+        n_metrics = 2
+
+        if self.include_height:
+            n_metrics += 1
+
         if self.use_derivative:
-            return 6
-        else:
-            return 3
+            n_metrics += 1
+
+            if self.include_height:
+                n_metrics += 2
+
+        return n_metrics
 
     @property
     def labels(self):
-        labels = ['Pearson Correleation', 'Time offset', 'Peak Height']
+        labels = ['Pearson Correleation', 'Time offset']
+        if self.include_height:
+            labels += ["Peak Height"]
         if self.use_derivative:
-            labels += [
-                'Pearson Correlation Derivative',
-                'Peak Minimum Derivative',
-                'Peak Maximum Derivative'
+            labels += ['Pearson Correlation Derivative']
+            if self.include_height:
+                labels += [
+                    'Peak Minimum Derivative',
+                    'Peak Maximum Derivative'
                 ]
         return labels
 
     def _evaluate(self, solution):
         """np.array: Shape similarity using pearson correlation.
 
         Parameters
@@ -562,45 +581,57 @@
         """
         corr, offset_original = pearson(
             self.reference.time,
             self.reference.solution_interpolated.solutions[0],
             solution.solution_interpolated.solutions[0],
         )
 
-        peak_height = self.peak_height(solution, slice=False)
+        if self.include_height:
+            peak_height = self.peak_height(solution, slice=False)
 
         if self.normalize_metrics:
             offset = sigmoid_distance(
                 offset_original, target=0, normalization=self.normalization_factor
             )
         else:
             offset = np.abs(offset_original)
 
         if not self.use_derivative:
-            return np.array([corr, offset, peak_height[0]])
+            if self.include_height:
+                return np.array([corr, offset, peak_height[0]])
+            elif not self.include_height:
+                return np.array([corr, offset])
 
         solution_der = solution.derivative
         solution_der_sliced = self.slice_and_transform(solution_der)
 
         corr_der = pearson_offset(
             self.reference_der_sliced.time,
             self.reference_der_sliced.solution_interpolated.solutions[0],
             solution_der_sliced.solution_interpolated.solutions[0],
             offset_original,
         )
 
         der_min = self.peak_der_min(solution_der_sliced, slice=False)
         der_max = self.peak_der_max(solution_der_sliced, slice=False)
 
-        return np.array(
-            [
-                corr, offset, peak_height[0],
-                corr_der, der_min[0], der_max[0]
-            ]
-        )
+        if self.include_height:
+            return np.array(
+                [
+                    corr, offset, peak_height[0],
+                    corr_der, der_min[0], der_max[0]
+                ]
+            )
+        elif not self.include_height:
+            return np.array(
+                [
+                    corr, offset,
+                    corr_der,
+                ]
+            )
 
 
 class PeakHeight(DifferenceBase):
     """Absolute difference in peak height difference metric.
 
     Attributes
     ----------
```

### Comparing `CADET-Process-0.9.0/CADETProcess/comparison/peaks.py` & `cadet_process-0.9.1/CADETProcess/comparison/peaks.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/comparison/shape.py` & `cadet_process-0.9.1/CADETProcess/comparison/shape.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/dataStructure/__init__.py` & `cadet_process-0.9.1/CADETProcess/dataStructure/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/dataStructure/aggregator.py` & `cadet_process-0.9.1/CADETProcess/dataStructure/aggregator.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/dataStructure/cache.py` & `cadet_process-0.9.1/CADETProcess/dataStructure/cache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/dataStructure/dataStructure.py` & `cadet_process-0.9.1/CADETProcess/dataStructure/dataStructure.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/dataStructure/diskcache.py` & `cadet_process-0.9.1/CADETProcess/dataStructure/diskcache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/dataStructure/nested_dict.py` & `cadet_process-0.9.1/CADETProcess/dataStructure/nested_dict.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/dataStructure/parameter.py` & `cadet_process-0.9.1/CADETProcess/dataStructure/parameter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/dataStructure/parameter_group.py` & `cadet_process-0.9.1/CADETProcess/dataStructure/parameter_group.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/dynamicEvents/__init__.py` & `cadet_process-0.9.1/CADETProcess/dynamicEvents/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/dynamicEvents/event.py` & `cadet_process-0.9.1/CADETProcess/dynamicEvents/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import defaultdict
 import copy
 import warnings
 
 from addict import Dict
 import numpy as np
+from matplotlib.axes import Axes
 
 from CADETProcess import CADETProcessError
 
 from CADETProcess.dataStructure import Structure, frozen_attributes
 from CADETProcess.dataStructure import (
     ParameterBase, Bool, Integer, Float, Sized, Typed, UnsignedFloat, NdPolynomial,
 )
@@ -767,52 +768,56 @@
 
             if np.any(np.isnan(current_value)):
                 warnings.warn(f"{evt_parameter} has entries which were not initialized")
                 flag = False
 
         return flag
 
-    def plot_events(self):
+    def plot_events(self, use_minutes: bool = True) -> list[Axes]:
         """
         Plot parameter state as a function of time.
 
         The method creates a plot for each parameter timeline and displays the state
         of the parameter against time. The time is represented on the x-axis, while
         the parameter state is shown on the y-axis.
 
         Parameters
         ----------
-        ax : matplotlib.Axes, optional
-            Axes to plot on. If not provided, new axes will be created.
+        use_minutes: bool, optional
+            Option to use x-aches (time) in minutes, default is set to True.
 
         Returns
         -------
         list of matplotlib.Axes
             List of axes objects, each containing a plot of the parameter state.
 
         Notes
         -----
         The time is divided into 1001 linearly spaced points between 0 and the cycle
         time for the evaluation of the parameter state.
         """
         time = np.linspace(0, self.cycle_time, 1001)
 
-        axs = []
+        if use_minutes:
+            time = time / 60
+        axs: list[Axes] = []
 
         for parameter, tl in self.parameter_timelines.items():
             fig, ax = plotting.setup_figure()
 
             y = tl.value(time)
 
             layout = plotting.Layout()
             layout.title = str(parameter)
-            layout.x_label = '$time~/~min$'
+            layout.x_label = "$time~/~s$"
+            if use_minutes:
+                layout.x_label = "$time~/~min$"
             layout.y_label = '$state$'
 
-            ax.plot(time/60, y)
+            ax.plot(time, y)
 
             plotting.set_layout(ax, layout)
 
             axs.append(ax)
 
         return axs
```

### Comparing `CADET-Process-0.9.0/CADETProcess/dynamicEvents/section.py` & `cadet_process-0.9.1/CADETProcess/dynamicEvents/section.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import itertools
 import warnings
 
 import numpy as np
 from numpy import VisibleDeprecationWarning
 import scipy
+from matplotlib.axes import Axes
+
 
 from CADETProcess import CADETProcessError
 from CADETProcess.dataStructure import Structure
 from CADETProcess.dataStructure import NdPolynomial
 from CADETProcess import plotting
 
 
@@ -401,38 +403,45 @@
 
     @property
     def end(self):
         """float: The end time of the timeline."""
         return self.section_times[-1]
 
     @plotting.create_and_save_figure
-    def plot(self, ax):
+    def plot(self, ax, use_minutes: bool = True) -> Axes:
         """Plot the state of the timeline over time.
 
         Parameters
         ----------
         ax : Axes
             The axes to plot on.
+        use_minutes : bool, optional
+            Option to use x-aches (time) in minutes, default is set to True.
 
         Returns
         -------
         ax : Axes
             The axes with the plot of the timeline state.
         """
         start = self.sections[0].start
         end = self.sections[-1].end
         time = np.linspace(start, end, 1001)
         y = self.value(time)
 
-        ax.plot(time/60, y)
+        if use_minutes:
+            time = time / 60
+            start = start / 60
+            end = end / 60
+
+        ax.plot(time, y)
 
         layout = plotting.Layout()
         layout.x_label = '$time~/~min$'
         layout.y_label = '$state$'
-        layout.x_lim = (start/60, end/60)
+        layout.x_lim = (start, end)
         layout.y_lim = (np.min(y), 1.1*np.max(y))
 
         plotting.set_layout(ax, layout)
 
         return ax
 
     @classmethod
```

### Comparing `CADET-Process-0.9.0/CADETProcess/equilibria/__init__.py` & `cadet_process-0.9.1/CADETProcess/equilibria/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/equilibria/buffer_capacity.py` & `cadet_process-0.9.1/CADETProcess/equilibria/buffer_capacity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/equilibria/initial_conditions.py` & `cadet_process-0.9.1/CADETProcess/equilibria/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/equilibria/ptc.py` & `cadet_process-0.9.1/CADETProcess/equilibria/ptc.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/equilibria/reaction_equilibria.py` & `cadet_process-0.9.1/CADETProcess/equilibria/reaction_equilibria.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/fractionation/fractionationOptimizer.py` & `cadet_process-0.9.1/CADETProcess/fractionation/fractionationOptimizer.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/fractionation/fractionator.py` & `cadet_process-0.9.1/CADETProcess/fractionation/fractionator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from collections import defaultdict
 from functools import wraps
 import os
 
 from addict import Dict
 import numpy as np
+from matplotlib.axes import Axes
 
 from CADETProcess import CADETProcessError
 from CADETProcess import settings
 from CADETProcess.dataStructure import String
 from CADETProcess.dynamicEvents import EventHandler
 from CADETProcess import plotting
 from CADETProcess.performance import Performance
-from CADETProcess.solution import slice_solution
+from CADETProcess.solution import slice_solution, SolutionIO
 from CADETProcess import SimulationResults
 
 from CADETProcess.fractionation.fractions import Fraction, FractionPool
 
 
 class Fractionator(EventHandler):
     """Class for Chromatogram Fractionation.
@@ -215,23 +216,31 @@
     @property
     def time(self):
         """np.ndarray: solution times of Chromatogram."""
         return self.chromatograms[0].time
 
     @plotting.create_and_save_figure
     def plot_fraction_signal(
-            self, chromatogram=None, ax=None, *args, **kwargs):
+            self,
+            chromatogram: SolutionIO | None = None,
+            use_minutes: bool = True,
+            ax: Axes = None,
+            *args,
+            **kwargs,
+            ) -> Axes:
         """Plot the signal without the waste fractions.
 
         Parameters
         ----------
         chromatogram : SolutionIO, optional
             Chromatogram to be plotted. If None, the first one is plotted.
         ax : Axes
             Axes to plot on.
+        use_minutes: bool, optional
+            Option to use x-aches (time) in minutes, default is set to True.
 
         Returns
         -------
         ax : Axes
             Axes with plot of parameter state.
 
         See Also
@@ -247,18 +256,22 @@
             chromatogram = self.chromatograms_dict[chromatogram]
 
         time_line = \
             self.performer_timelines['fractionation_states'][chromatogram.name]
 
         try:
             start = kwargs['start']
+            if use_minutes:
+                start = start / 60
         except KeyError:
             start = 0
         try:
             end = kwargs['end']
+            if use_minutes:
+                end = end / 60
         except KeyError:
             end = np.max(chromatogram.time)
 
         _,  ax = chromatogram.plot(show=False, ax=ax, *args, **kwargs)
 
         y_max = 1.1*np.max(chromatogram.solution)
 
@@ -268,31 +281,40 @@
             if comp_index == self.n_comp:
                 color_index = -1
                 text = 'W'
             else:
                 color_index = comp_index
                 text = str(comp_index + 1)
 
-            if sec.start != sec.end:
-                fill_regions.append(plotting.FillRegion(
-                    start=sec.start/60,
-                    end=sec.end/60,
-                    y_max=y_max,
-                    color_index=color_index,
-                    text=text
+            sec_start = sec.start
+            sec_end = sec.end
+
+            if use_minutes:
+                sec_start = sec_start / 60
+                sec_end = sec_end / 60
+
+            if sec_start != sec_end:
+                fill_regions.append(
+                    plotting.FillRegion(
+                        start=sec_start,
+                        end=sec_end,
+                        y_max=y_max,
+                        color_index=color_index,
+                        text=text,
                     )
                 )
 
         if len(time_line.sections) == 0:
-            fill_regions.append(plotting.FillRegion(
-                start=sec.start/60,
-                end=sec.end/60,
-                y_max=y_max,
-                color_index=-1,
-                text='W'
+            fill_regions.append(
+                plotting.FillRegion(
+                    start=sec_start,
+                    end=sec_end,
+                    y_max=y_max,
+                    color_index=-1,
+                    text="W"
                 )
             )
 
         plotting.add_fill_regions(ax, fill_regions, (start, end))
 
         return ax
```

### Comparing `CADET-Process-0.9.0/CADETProcess/fractionation/fractions.py` & `cadet_process-0.9.1/CADETProcess/fractionation/fractions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/log.py` & `cadet_process-0.9.1/CADETProcess/log.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/modelBuilder/__init__.py` & `cadet_process-0.9.1/CADETProcess/modelBuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/modelBuilder/carouselBuilder.py` & `cadet_process-0.9.1/CADETProcess/modelBuilder/carouselBuilder.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/modelBuilder/compartmentBuilder.py` & `cadet_process-0.9.1/CADETProcess/modelBuilder/compartmentBuilder.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/optimization/__init__.py` & `cadet_process-0.9.1/CADETProcess/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/optimization/axAdapater.py` & `cadet_process-0.9.1/CADETProcess/optimization/axAdapater.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
             self,
             optimization_problem: OptimizationProblem,
             parallelization_backend: ParallelizationBackendBase
     ) -> None:
         self.optimization_problem = optimization_problem
         self.parallelization_backend = parallelization_backend
 
+    @property
     def staging_required(self) -> bool:
         return False
 
     def run(self, trial: BaseTrial) -> Dict[str, Any]:
         # Get X from arms.
         X = []
         for arm in trial.arms:
@@ -270,15 +271,14 @@
             trial_data = {
                 "input": {var: x_i for var, x_i in zip(variables, x)},
             }
 
             arm_name = f"{trial.index}_{0}"
             trial.add_arm(Arm(parameters=trial_data["input"], name=arm_name))
             trial.run()
-            trial.mark_running()
             trial.mark_completed()
             self._post_processing(trial)
 
             # When returning to batch trials, the Arms can be initialized here
             # and then collectively returned. See commit history
 
     def _post_processing(self, trial):
@@ -303,15 +303,15 @@
         # Get objective values
         F_data = data[data['metric_name'].isin(objective_labels)]
         assert np.all(F_data["metric_name"].values == np.repeat(objective_labels, len(X)).astype(object))
         F = F_data["mean"].values.reshape((op.n_objectives, n_ind)).T
 
         # Get nonlinear constraint values
         if op.n_nonlinear_constraints > 0:
-            nonlincon_labels = op.nonlinear_constraint_labels
+            nonlincon_labels = [f"{name}_axidx_{i}" for i, name in enumerate(op.nonlinear_constraint_labels)]
             G_data = data[data['metric_name'].isin(nonlincon_labels)]
             assert np.all(G_data["metric_name"].values.tolist() == np.repeat(nonlincon_labels, len(X)))
             G = G_data["mean"].values.reshape((op.n_nonlinear_constraints, n_ind)).T
 
             nonlincon_cv_fun = op.evaluate_nonlinear_constraints_violation_population
             CV = nonlincon_cv_fun(X, untransform=True)
         else:
@@ -447,16 +447,14 @@
                 if stop_optimization:
                     print(global_stopping_message)
                     break
 
                 trial = self.ax_experiment.new_trial(generator_run=sample_generator)
                 trial.run()
 
-                trial.mark_running()
-
                 trial.mark_completed()
                 self._post_processing(trial)
 
                 n_iter += 1
                 n_evals += len(trial.arms)
 
         print(exp_to_df(self.ax_experiment))
```

### Comparing `CADET-Process-0.9.0/CADETProcess/optimization/cache.py` & `cadet_process-0.9.1/CADETProcess/optimization/cache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/optimization/individual.py` & `cadet_process-0.9.1/CADETProcess/optimization/individual.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,35 +28,36 @@
     '3dfc9d56e04dcd01590f48b1b57c9ed9fecb1e94e11d3c3f13cf0fd97b7a9f0f'
     """
     array = np.asarray(array)
     return hashlib.sha256(array.tobytes()).hexdigest()
 
 
 class Individual(Structure):
-    """Set of variables evaluated during Optimization.
+    """
+    Set of variables evaluated during Optimization.
 
     Attributes
     ----------
-    x : list
+    x : np.ndarray
         Variable values in untransformed space.
-    x_transformed : list
+    x_transformed : np.ndarray
         Independent variable values in transformed space.
-    f : list
+    f : np.ndarray
         Objective values.
-    f_min : list
+    f_min : np.ndarray
         Minimized objective values.
-    g : list
+    g : np.ndarray
         Nonlinear constraint values.
-    cv : list
+    cv : np.ndarray
         Nonlinear constraints violation.
     cv_tol : float
         Tolerance for constraints violation.
-    m : list
+    m : np.ndarray
         Meta score values.
-    m_min : list
+    m_min : np.ndarray
         Minimized meta score values.
 
     See Also
     --------
     CADETProcess.optimization.Population
     """
```

### Comparing `CADET-Process-0.9.0/CADETProcess/optimization/optimizationProblem.py` & `cadet_process-0.9.1/CADETProcess/optimization/optimizationProblem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1594,23 +1594,26 @@
             callbacks_dir=callbacks_dir,
             keep_progress=keep_progress,
             args=args,
             kwargs=kwargs
         )
         self._callbacks.append(callback)
 
-    def evaluate_callbacks(self, ind, current_iteration=1, force=False):
+    def evaluate_callbacks(self, ind, current_iteration=0, force=False):
         """Evaluate callback functions at point x.
 
         Parameters
         ----------
         ind : Individual
             Individual to be evalauted.
-        current_iteration : int
-            Current iteration to determine if callback should be evaluated.
+        current_iteration : int, optional
+            Current iteration step. This value is used to determine whether the
+            evaluation of callbacks should be skipped according to their evaluation
+            frequency. The default is 0, indicating the callbacks will be evaluated
+            regardless of the specified frequency.
         force : bool
             If True, do not use cached results. The default is False.
 
         See Also
         --------
         evaluate_callbacks_population
         _evaluate
@@ -1632,23 +1635,30 @@
                 self._evaluate(ind.x_transformed, callback, force, untransform=True)
             except CADETProcessError:
                 self.logger.warning(
                     f'Evaluation of {callback} failed at {ind.x}.'
                 )
 
     def evaluate_callbacks_population(
-            self, population, current_iteration, force=False, parallelization_backend=None):
+            self,
+            population,
+            current_iteration=0,
+            force=False,
+            parallelization_backend=None
+            ):
         """Evaluate callbacks for each individual ind in population.
 
         Parameters
         ----------
         population : list
             Population.
-        current_iteration : int
-            Current iteration step.
+        current_iteration : int, optional
+            Current iteration step. This value is used to determine whether the
+            evaluation of callbacks is skipped according to their evaluation frequency.
+            The default is 0, indicating it will definitely be evaluated.
         force : bool, optional
             If True, do not use cached values. The default is False.
         parallelization_backend : RunnerBase, optional
             Runner to use for the evaluation of the population in
             sequential or parallel mode.
 
         See Also
@@ -2935,38 +2945,142 @@
 
         return np.array(values, ndmin=2)
 
     @untransforms
     @gets_dependent_values
     def create_individual(
             self,
-            x,
-            f=None,
-            g=None,
-            m=None,
-            x_transformed=None,
-            f_min=None,
-            cv=None,
-            cv_tol=None,
-            m_min=None,
-            ):
+            x: np.ndarray,
+            f: np.ndarray = None,
+            g: np.ndarray | None = None,
+            m: np.ndarray | None = None,
+            f_min: np.ndarray | None = None,
+            cv: np.ndarray | None = None,
+            cv_tol: float = 0.,
+            m_min: np.ndarray | None = None,
+            ) -> Individual:
+        """
+        Create new individual from data.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            Variable values in untransformed space.
+        f : np.ndarray
+            Objective values.
+        g : np.ndarray
+            Nonlinear constraint values.
+        m : np.ndarray
+            Meta score values.
+        f_min : np.ndarray
+            Minimized objective values.
+        cv : np.ndarray
+            Nonlinear constraints violation.
+        cv_tol : float
+            Tolerance for constraints violation.
+        m_min : np.ndarray
+            Minimized meta score values.
+
+        Returns
+        -------
+        Individual
+            The newly created individual.
+        """
         x_indep = self.get_independent_values(x)
         x_transformed = self.transform(x_indep)
 
         ind = Individual(
             x, f, g, m, x_transformed, f_min, cv, cv_tol, m_min,
             self.independent_variable_names,
             self.objective_labels,
             self.nonlinear_constraint_labels,
             self.meta_score_labels,
             self.variable_names,
         )
 
         return ind
 
+    @ensures2d
+    @untransforms
+    @gets_dependent_values
+    def create_population(
+            self,
+            X: np.ndarray,
+            F: np.ndarray = None,
+            G: np.ndarray | None = None,
+            M: np.ndarray | None = None,
+            F_min: np.ndarray | None = None,
+            CV: np.ndarray | None = None,
+            cv_tol: float = 0.,
+            M_min: np.ndarray | None = None,
+            ) -> Population:
+        """
+        Create new population from data.
+
+        Parameters
+        ----------
+        X : np.ndarray
+            Variable values in untransformed space.
+        F : np.ndarray
+            Objective values.
+        G : np.ndarray
+            Nonlinear constraint values.
+        M : np.ndarray
+            Meta score values.
+        F_min : np.ndarray
+            Minimized objective values.
+        CV : np.ndarray
+            Nonlinear constraints violation.
+        cv_tol : float
+            Tolerance for constraints violation.
+        M_min : np.ndarray
+            Minimized meta score values.
+
+        Returns
+        -------
+        Population
+            The newly created population.
+        """
+        if F is None:
+            F = len(X) * [None]
+        else:
+            F = np.array(F, ndmin=2)
+
+        if G is None:
+            G = len(X) * [None]
+        else:
+            G = np.array(G, ndmin=2)
+
+        if M is None:
+            M = len(X) * [None]
+        else:
+            M = np.array(M, ndmin=2)
+
+        if F_min is None:
+            F_min = F
+        else:
+            F_min = np.array(F_min, ndmin=2)
+
+        if CV is None:
+            CV = G
+        else:
+            CV = np.array(CV, ndmin=2)
+
+        if M_min is None:
+            M_min = M
+        else:
+            M_min = np.array(M_min, ndmin=2)
+
+        pop = Population()
+        for x, f, g, m, f_min, cv, m_min in zip(X, F, G, M, F_min, CV, M_min):
+            ind = self.create_individual(x, f, g, m, f_min, cv, cv_tol, m_min)
+            pop.add_individual(ind)
+
+        return pop
+
     @property
     def parameters(self):
         parameters = Dict()
 
         parameters.variables = {
             opt.name: opt.parameters for opt in self.variables
         }
@@ -3811,14 +3925,15 @@
 
         self.frequency = frequency
 
         if callbacks_dir is not None:
             callbacks_dir = Path(callbacks_dir)
             callbacks_dir.mkdir(exist_ok=True, parents=True)
         self.callbacks_dir = callbacks_dir
+        self._callbacks_dir = callbacks_dir
 
         self.keep_progress = keep_progress
 
         self.args = args
         self.kwargs = kwargs
 
         self.id = uuid.uuid4()
@@ -3864,15 +3979,16 @@
         if 'evaluation_object' in signature:
             kwargs['evaluation_object'] = evaluation_object
         if 'callbacks_dir' in signature:
             if self.callbacks_dir is not None:
                 callbacks_dir = self.callbacks_dir
             else:
                 callbacks_dir = self._callbacks_dir
-            kwargs['callbacks_dir'] = callbacks_dir
+            if callbacks_dir is not None:
+                kwargs['callbacks_dir'] = callbacks_dir
 
         self.callback(request, *args, **kwargs)
 
     evaluate = __call__
 
     def __str__(self):
         return self.name
```

### Comparing `CADET-Process-0.9.0/CADETProcess/optimization/optimizer.py` & `cadet_process-0.9.1/CADETProcess/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/optimization/parallelizationBackend.py` & `cadet_process-0.9.1/CADETProcess/optimization/parallelizationBackend.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/optimization/population.py` & `cadet_process-0.9.1/CADETProcess/optimization/population.py`

 * *Files 4% similar despite different names*

```diff
@@ -562,59 +562,103 @@
             else:
                 figs[0].savefig(
                     f'{plot_directory / "objectives"}.png'
                 )
 
         return figs, axs
 
-    def setup_pareto(self):
+    def setup_pareto(self, include_meta: bool = False):
         """Set up base figure for plotting the Pareto front.
 
+        Parameters
+        ----------
+        include_meta : bool
+            If True, include meta scores in Pareto plot.
+
         Returns
         -------
         pymoo.visualization.scatter.Scatter
             The base figure object.
         """
-        n = self.dimensions[1]
+        if include_meta:
+            n = self.dimensions[1] + self.dimensions[3]
+            labels = self.objective_labels + self.meta_score_labels
+        else:
+            n = self.dimensions[1]
+            labels = self.objective_labels
         plot = Scatter(
             figsize=(6 * n, 5 * n),
             tight_layout=True,
             plot_3d=False,
-            labels=self.objective_labels,
+            labels=labels,
         )
         return plot
 
     def plot_pareto(
-            self, plot=None, color=None, show=True, plot_directory=None):
+            self,
+            plot=None,
+            include_meta=True,
+            plot_infeasible=True,
+            color_feas='blue',
+            color_infeas='red',
+            show=True,
+            plot_directory=None):
         """Plot pairwise Pareto fronts for each generation in the optimization.
 
         The Pareto front represents the optimal solutions that cannot be improved in one
         objective without sacrificing another. The method shows a pairwise Pareto plot,
         where each objective is plotted against every other objective in a scatter plot,
         allowing for a visualization of the trade-offs between the objectives.
 
         Parameters
         ----------
         plot : pymoo.visualization.scatter.Scatter, optional
             Base figure. If None is provided, a new one will be set up.
-        color : str, optional
-            Color for scatter points.
+        include_meta : bool, optional
+            If True, include meta scores in the plot. The default is True.
+        plot_infeasible : bool, optional
+            If True, plot infeasible points. The default is True.
+        color_feas : str, optional
+            The color for the feasible points. The default is 'blue'.
+        color_infeas : str, optional
+            The color for the infeasible points. The default is 'red'.
         show : bool, optional
             If True, display the plot. The default is True.
         plot_directory : str, optional
             The directory where the plot should be saved. The default is None.
 
         Returns
         -------
         pymoo.visualization.scatter.Scatter
             The scatter plot object.
         """
         if plot is None:
-            plot = self.setup_pareto()
-        plot.add(self.f, s=10, color=color)
+            plot = self.setup_pareto(include_meta)
+
+        feasible = self.feasible
+        infeasible = self.infeasible
+
+        if include_meta and self.m is not None:
+            if len(feasible) > 0:
+                values_feas = np.hstack((feasible.f, feasible.m))
+            else:
+                values_infeas = np.empty((0, self.n_f + self.n_m))
+            if len(infeasible) > 0:
+                values_infeas = np.hstack((infeasible.f, infeasible.m))
+            else:
+                values_infeas = np.empty((0, self.n_f + self.n_m))
+        else:
+            values_feas = feasible.f
+            values_infeas = infeasible.f
+
+        if len(feasible) > 0:
+            plot.add(values_feas, s=10, color=color_feas)
+
+        if plot_infeasible and len(infeasible) > 0:
+            plot.add(values_infeas, s=10, color=color_infeas)
 
         if plot_directory is not None:
             plot_directory = Path(plot_directory)
             plot.save(f'{plot_directory / "pareto.png"}')
 
         if not show:
             plt.close(plot.fig)
@@ -868,15 +912,15 @@
             dominates_one = False
             has_twin = False
             to_remove = []
 
             try:
                 # Do not add if invalid
                 if np.any(np.array(ind_new.cv) > self.cv_tol):
-                    break
+                    continue
             except TypeError:
                 pass
 
             for i, ind_pareto in enumerate(self):
                 # Do not add if is dominated
                 if not dominates_one and ind_pareto.dominates(ind_new):
                     is_dominated = True
```

### Comparing `CADET-Process-0.9.0/CADETProcess/optimization/pymooAdapter.py` & `cadet_process-0.9.1/CADETProcess/optimization/pymooAdapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,23 @@
     pop_size = UnsignedInteger()
 
     xtol = UnsignedFloat(default=1e-8)
     ftol = UnsignedFloat(default=0.0025)
     cvtol = UnsignedFloat(default=1e-6)
 
     n_max_gen = UnsignedInteger()
+    n_skip = UnsignedInteger(default=0)
 
     x_tol = xtol            # Alias for uniform interface
     f_tol = ftol            # Alias for uniform interface
     cv_tol = cvtol          # Alias for uniform interface
     n_max_iter = n_max_gen  # Alias for uniform interface
 
     _specific_options = [
-        'seed', 'pop_size', 'xtol', 'ftol', 'cvtol', 'n_max_gen'
+        'seed', 'pop_size', 'xtol', 'ftol', 'cvtol', 'n_max_gen', 'n_skip'
     ]
 
     def run(self, optimization_problem: OptimizationProblem, x0=None):
         """Solve optimization problem using functional pymoo implementation.
 
         Parameters
         ----------
@@ -116,15 +117,16 @@
         n_max_gen = self.get_max_number_of_generations(optimization_problem)
 
         termination = DefaultMultiObjectiveTermination(
             xtol=self.xtol,
             cvtol=self.cvtol,
             ftol=self.ftol,
             n_max_gen=n_max_gen,
-            n_max_evals=self.n_max_evals
+            n_max_evals=self.n_max_evals,
+            n_skip=self.n_skip,
         )
 
         algorithm.setup(
             problem, termination=termination,
             seed=self.seed, verbose=True, save_history=False,
             output=MultiObjectiveOutput(),
         )
```

### Comparing `CADET-Process-0.9.0/CADETProcess/optimization/results.py` & `cadet_process-0.9.1/CADETProcess/optimization/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,15 +513,16 @@
 
         """
         plot = None
         _show = False
         _plot_directory = None
 
         cNorm = colors.Normalize(vmin=0, vmax=self.n_gen)
-        scalarMap = cmx.ScalarMappable(norm=cNorm, cmap=cmap_feas)
+        scalarMap_feas = cmx.ScalarMappable(norm=cNorm, cmap=cmap_feas)
+        scalarMap_infeas = cmx.ScalarMappable(norm=cNorm, cmap=cmap_infeas)
 
         if plot_pareto:
             populations = self.pareto_fronts
             population_last = self.pareto_front
         else:
             populations = self.populations
             population_last = self.population_last
@@ -531,15 +532,16 @@
 
         for i, gen in enumerate(populations):
             if gen is population_last:
                 _plot_directory = plot_directory
                 _show = show
             plot = gen.plot_pareto(
                 plot,
-                color=scalarMap.to_rgba(i),
+                color_feas=scalarMap_feas.to_rgba(i),
+                color_infeas=scalarMap_infeas.to_rgba(i),
                 show=_show,
                 plot_directory=_plot_directory
             )
 
     def plot_corner(self, *args, **kwargs):
         """Create a corner plot of the independent variables.
```

### Comparing `CADET-Process-0.9.0/CADETProcess/optimization/scipyAdapter.py` & `cadet_process-0.9.1/CADETProcess/optimization/scipyAdapter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/performance.py` & `cadet_process-0.9.1/CADETProcess/performance.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/plotting.py` & `cadet_process-0.9.1/CADETProcess/plotting.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/processModel/__init__.py` & `cadet_process-0.9.1/CADETProcess/processModel/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/processModel/binding.py` & `cadet_process-0.9.1/CADETProcess/processModel/binding.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/processModel/componentSystem.py` & `cadet_process-0.9.1/CADETProcess/processModel/componentSystem.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/processModel/discretization.py` & `cadet_process-0.9.1/CADETProcess/processModel/discretization.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/processModel/flowSheet.py` & `cadet_process-0.9.1/CADETProcess/processModel/flowSheet.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/processModel/process.py` & `cadet_process-0.9.1/CADETProcess/processModel/process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/processModel/reaction.py` & `cadet_process-0.9.1/CADETProcess/processModel/reaction.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/processModel/solutionRecorder.py` & `cadet_process-0.9.1/CADETProcess/processModel/solutionRecorder.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/processModel/unitOperation.py` & `cadet_process-0.9.1/CADETProcess/processModel/unitOperation.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/reference.py` & `cadet_process-0.9.1/CADETProcess/reference.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/settings.py` & `cadet_process-0.9.1/CADETProcess/settings.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/simulationResults.py` & `cadet_process-0.9.1/CADETProcess/simulationResults.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/simulator/__init__.py` & `cadet_process-0.9.1/CADETProcess/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/simulator/cadetAdapter.py` & `cadet_process-0.9.1/CADETProcess/simulator/cadetAdapter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/simulator/simulator.py` & `cadet_process-0.9.1/CADETProcess/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/smoothing.py` & `cadet_process-0.9.1/CADETProcess/smoothing.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/smoothing2.py` & `cadet_process-0.9.1/CADETProcess/smoothing2.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/solution.py` & `cadet_process-0.9.1/CADETProcess/solution.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/stationarity.py` & `cadet_process-0.9.1/CADETProcess/stationarity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/sysinfo.py` & `cadet_process-0.9.1/CADETProcess/sysinfo.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/tools/yamamoto.py` & `cadet_process-0.9.1/CADETProcess/tools/yamamoto.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADETProcess/transform.py` & `cadet_process-0.9.1/CADETProcess/transform.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/CADET_Process.egg-info/PKG-INFO` & `cadet_process-0.9.1/CADET_Process.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 Metadata-Version: 2.1
 Name: CADET-Process
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Framework for Modelling and Optimizing Advanced Chromatographic Processes
 Home-page: https://github.com/fau-advanced-separations/CADET-Process
 Author: Johannes Schmölder
-Author-email: j.schmoelder@fz-juelich.de
+Author-email: Johannes Schmölder <j.schmoelder@fz-juelich.de>
+License: GPLv3
+Project-URL: homepage, https://github.com/fau-advanced-separations/CADET-Process
+Project-URL: documentation, https://cadet-process.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/fau-advanced-separations/CADET-Process/issues
+Keywords: process modeling,process optimization,chromatography
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: numpy>=1.21
-Requires-Dist: scipy>=1.11
-Requires-Dist: matplotlib>=3.4
-Requires-Dist: corner>=2.2.1
-Requires-Dist: sympy>=1.8
-Requires-Dist: pathos>=0.2.8
 Requires-Dist: addict==2.3
 Requires-Dist: cadet-python>=0.14
-Requires-Dist: hopsy>=1.4.0
-Requires-Dist: pymoo>=0.6
-Requires-Dist: numba>=0.55.1
+Requires-Dist: corner>=2.2.1
 Requires-Dist: diskcache>=5.4.0
+Requires-Dist: hopsy>=1.4.0
 Requires-Dist: joblib>=1.3.0
+Requires-Dist: numpy>=1.21
+Requires-Dist: matplotlib>=3.4
+Requires-Dist: numba>=0.55.1
+Requires-Dist: pathos>=0.2.8
 Requires-Dist: psutil>=5.9.8
+Requires-Dist: pymoo>=0.6
+Requires-Dist: scipy>=1.11
 Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: certifi; extra == "testing"
-Requires-Dist: pre-commit; extra == "testing"
-Requires-Dist: flake8; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pre-commit; extra == "testing"
 Requires-Dist: ax-platform>=0.3.5; extra == "testing"
 Provides-Extra: docs
+Requires-Dist: myst-nb>=0.17.1; extra == "docs"
+Requires-Dist: numpydoc>=1.5.0; extra == "docs"
 Requires-Dist: sphinx>=5.3.0; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex>=2.5.0; extra == "docs"
 Requires-Dist: sphinx_book_theme>=1.0.0; extra == "docs"
 Requires-Dist: sphinx_copybutton>=0.5.1; extra == "docs"
 Requires-Dist: sphinx-sitemap>=2.5.0; extra == "docs"
-Requires-Dist: numpydoc>=1.5.0; extra == "docs"
-Requires-Dist: myst-nb>=0.17.1; extra == "docs"
 Provides-Extra: ax
 Requires-Dist: ax-platform>=0.3.5; extra == "ax"
 
 # CADET-Process
 
 The [**CADET**](https://cadet.github.io) core simulator is a very powerful numerical engine that can simulate a large variety of physico-chemical models used in chromatography and other biochemical processes.
 However, the configuration files of **CADET** can be complex and difficult to work with.
```

### Comparing `CADET-Process-0.9.0/CADET_Process.egg-info/SOURCES.txt` & `cadet_process-0.9.1/CADET_Process.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE.md
 README.md
 pyproject.toml
 setup.cfg
-setup.py
 CADETProcess/CADETProcessError.py
 CADETProcess/__init__.py
 CADETProcess/log.py
 CADETProcess/metric.py
 CADETProcess/performance.py
 CADETProcess/plotting.py
 CADETProcess/reference.py
```

### Comparing `CADET-Process-0.9.0/LICENSE.md` & `cadet_process-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/PKG-INFO` & `cadet_process-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 Metadata-Version: 2.1
 Name: CADET-Process
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Framework for Modelling and Optimizing Advanced Chromatographic Processes
 Home-page: https://github.com/fau-advanced-separations/CADET-Process
 Author: Johannes Schmölder
-Author-email: j.schmoelder@fz-juelich.de
+Author-email: Johannes Schmölder <j.schmoelder@fz-juelich.de>
+License: GPLv3
+Project-URL: homepage, https://github.com/fau-advanced-separations/CADET-Process
+Project-URL: documentation, https://cadet-process.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/fau-advanced-separations/CADET-Process/issues
+Keywords: process modeling,process optimization,chromatography
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: numpy>=1.21
-Requires-Dist: scipy>=1.11
-Requires-Dist: matplotlib>=3.4
-Requires-Dist: corner>=2.2.1
-Requires-Dist: sympy>=1.8
-Requires-Dist: pathos>=0.2.8
 Requires-Dist: addict==2.3
 Requires-Dist: cadet-python>=0.14
-Requires-Dist: hopsy>=1.4.0
-Requires-Dist: pymoo>=0.6
-Requires-Dist: numba>=0.55.1
+Requires-Dist: corner>=2.2.1
 Requires-Dist: diskcache>=5.4.0
+Requires-Dist: hopsy>=1.4.0
 Requires-Dist: joblib>=1.3.0
+Requires-Dist: numpy>=1.21
+Requires-Dist: matplotlib>=3.4
+Requires-Dist: numba>=0.55.1
+Requires-Dist: pathos>=0.2.8
 Requires-Dist: psutil>=5.9.8
+Requires-Dist: pymoo>=0.6
+Requires-Dist: scipy>=1.11
 Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: certifi; extra == "testing"
-Requires-Dist: pre-commit; extra == "testing"
-Requires-Dist: flake8; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pre-commit; extra == "testing"
 Requires-Dist: ax-platform>=0.3.5; extra == "testing"
 Provides-Extra: docs
+Requires-Dist: myst-nb>=0.17.1; extra == "docs"
+Requires-Dist: numpydoc>=1.5.0; extra == "docs"
 Requires-Dist: sphinx>=5.3.0; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex>=2.5.0; extra == "docs"
 Requires-Dist: sphinx_book_theme>=1.0.0; extra == "docs"
 Requires-Dist: sphinx_copybutton>=0.5.1; extra == "docs"
 Requires-Dist: sphinx-sitemap>=2.5.0; extra == "docs"
-Requires-Dist: numpydoc>=1.5.0; extra == "docs"
-Requires-Dist: myst-nb>=0.17.1; extra == "docs"
 Provides-Extra: ax
 Requires-Dist: ax-platform>=0.3.5; extra == "ax"
 
 # CADET-Process
 
 The [**CADET**](https://cadet.github.io) core simulator is a very powerful numerical engine that can simulate a large variety of physico-chemical models used in chromatography and other biochemical processes.
 However, the configuration files of **CADET** can be complex and difficult to work with.
```

### Comparing `CADET-Process-0.9.0/README.md` & `cadet_process-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/examples/batch_elution/optimization_multi.py` & `cadet_process-0.9.1/examples/batch_elution/optimization_multi.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/examples/batch_elution/optimization_single.py` & `cadet_process-0.9.1/examples/batch_elution/optimization_single.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/examples/batch_elution/process.py` & `cadet_process-0.9.1/examples/batch_elution/process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/examples/characterize_chromatographic_system/Yamamoto_method.py` & `cadet_process-0.9.1/examples/characterize_chromatographic_system/Yamamoto_method.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/examples/characterize_chromatographic_system/binding_model_parameters.py` & `cadet_process-0.9.1/examples/characterize_chromatographic_system/binding_model_parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -245,33 +245,74 @@
         parameter_path='flow_sheet.column.binding_model.adsorption_rate',
         lb=1e-3, ub=1e3,
         transform='auto',
         indices=[1]  # modify only the protein (component index 1) parameter
     )
 
     optimization_problem.add_variable(
+        name='desorption_rate',
+        parameter_path='flow_sheet.column.binding_model.desorption_rate',
+        lb=1e-3, ub=1e3,
+        transform='auto',
+        indices=[1]  # modify only the protein (component index 1) parameter
+    )
+
+    optimization_problem.add_variable(
+        name='equilibrium_constant',
+        evaluation_objects=None,
+        lb=1e-4, ub=1e3,
+        transform='auto',
+        indices=[1]  # modify only the protein (component index 1) parameter
+    )
+
+    optimization_problem.add_variable(
+        name='kinetic_constant',
+        evaluation_objects=None,
+        lb=1e-4, ub=1e3,
+        transform='auto',
+        indices=[1]  # modify only the protein (component index 1) parameter
+    )
+
+    optimization_problem.add_variable(
         name='characteristic_charge',
         parameter_path='flow_sheet.column.binding_model.characteristic_charge',
         lb=1, ub=50,
         transform='auto',
         indices=[1]  # modify only the protein (component index 1) parameter
     )
 
+    optimization_problem.add_variable_dependency(
+        dependent_variable="desorption_rate",
+        independent_variables=["kinetic_constant", ],
+        transform=lambda k_kin: 1 / k_kin
+    )
+
+    optimization_problem.add_variable_dependency(
+        dependent_variable="adsorption_rate",
+        independent_variables=["kinetic_constant", "equilibrium_constant"],
+        transform=lambda k_kin, k_eq: k_eq / k_kin
+    )
+
 
     def callback(simulation_results, individual, evaluation_object, callbacks_dir='./'):
         comparator = comparators[evaluation_object.name]
         comparator.plot_comparison(
             simulation_results,
             file_name=f'{callbacks_dir}/{individual.id}_{evaluation_object}_comparison.png',
             show=False
         )
 
 
     optimization_problem.add_callback(callback, requires=[simulator])
 
+    print(optimization_problem.variable_names)
+    x0 = [1, 1, 1e-2, 1e-3, 10]
+    ind = optimization_problem.create_individual(x0)
+    optimization_problem.evaluate_callbacks(ind)
+
 # %% [markdown]
 # ```{note}
 # For performance reasons, the optimization is currently not run when building the documentation.
 # In future, we will try to sideload pre-computed results to also discuss them here.
 # ```
 
 # %%
```

### Comparing `CADET-Process-0.9.0/examples/characterize_chromatographic_system/column_transport_parameters.py` & `cadet_process-0.9.1/examples/characterize_chromatographic_system/column_transport_parameters.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/examples/characterize_chromatographic_system/particle_porosity.py` & `cadet_process-0.9.1/examples/characterize_chromatographic_system/particle_porosity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/examples/load_wash_elute/lwe_concentration.py` & `cadet_process-0.9.1/examples/load_wash_elute/lwe_concentration.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/examples/load_wash_elute/lwe_flow_rate.py` & `cadet_process-0.9.1/examples/load_wash_elute/lwe_flow_rate.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/examples/load_wash_elute/lwe_hic.py` & `cadet_process-0.9.1/examples/load_wash_elute/lwe_hic.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/examples/recycling/clr_process.py` & `cadet_process-0.9.1/examples/recycling/clr_process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/examples/recycling/mrssr_process.py` & `cadet_process-0.9.1/examples/recycling/mrssr_process.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/setup.cfg` & `cadet_process-0.9.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 
 [options]
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.10
 install_requires = 
 	numpy>=1.21
 	scipy>=1.11
 	matplotlib>=3.4
 	corner>=2.2.1
 	sympy>=1.8
 	pathos>=0.2.8
```

### Comparing `CADET-Process-0.9.0/tests/optimization_problem_fixtures.py` & `cadet_process-0.9.1/tests/optimization_problem_fixtures.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_binding.py` & `cadet_process-0.9.1/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_buffer_capacity.py` & `cadet_process-0.9.1/tests/test_buffer_capacity.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_cache.py` & `cadet_process-0.9.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_cadet_adapter.py` & `cadet_process-0.9.1/tests/test_cadet_adapter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_cadet_reactions.py` & `cadet_process-0.9.1/tests/test_cadet_reactions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_carousel.py` & `cadet_process-0.9.1/tests/test_carousel.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_compartment.py` & `cadet_process-0.9.1/tests/test_compartment.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_components.py` & `cadet_process-0.9.1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_difference.py` & `cadet_process-0.9.1/tests/test_difference.py`

 * *Files 3% similar despite different names*

```diff
@@ -294,68 +294,98 @@
         )
 
     def test_metric(self):
         # Compare with itself
         difference = Shape(
             self.reference,
             use_derivative=False,
-            components=['A']
+            components=['A'],
+            normalize_metrics=False,
+            include_height=False,
         )
-        metrics_expected = [0, 0, 0]
+        metrics_expected = [0, 0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak
         difference = Shape(
             self.reference_switched,
             use_derivative=False,
             components=['A'],
-            normalize_metrics=False
+            normalize_metrics=False,
+            include_height=False,
+        )
+        metrics_expected = [5.5511151e-16, 10]
+        metrics = difference.evaluate(self.reference)
+        np.testing.assert_almost_equal(metrics, metrics_expected)
+
+        # Compare with other Gauss Peak, include height
+        difference = Shape(
+            self.reference_switched,
+            use_derivative=False,
+            components=['A'],
+            normalize_metrics=False,
+            include_height=True,
         )
-        metrics_expected = [5.5511151e-16, 10, 0.0000000e+00]
+        metrics_expected = [5.5511151e-16, 10, 0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak, normalize_metrics
         difference = Shape(
             self.reference_switched,
             use_derivative=False,
             components=['A'],
-            normalize_metrics=True
+            normalize_metrics=True,
+            include_height=False,
         )
-        metrics_expected = [0, 4.6211716e-01, 0]
+        metrics_expected = [0, 4.6211716e-01]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak, include derivative
         difference = Shape(
             self.reference_switched,
             use_derivative=True,
             components=['A'],
-            normalize_metrics=False
+            normalize_metrics=False,
+            include_height=False,
+        )
+        metrics_expected = [0, 10, 0, ]
+        metrics = difference.evaluate(self.reference)
+        np.testing.assert_almost_equal(metrics, metrics_expected)
+
+        # Compare with other Gauss Peak, include derivative and height
+        difference = Shape(
+            self.reference_switched,
+            use_derivative=True,
+            components=['A'],
+            normalize_metrics=False,
+            include_height=True,
         )
         metrics_expected = [0, 10, 0, 0, 0, 0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Compare with other Gauss Peak, include derivative, normalize metrics
         difference = Shape(
             self.reference_switched,
             use_derivative=True,
             components=['A'],
-            normalize_metrics=True
+            normalize_metrics=True,
+            include_height=False,
         )
-        metrics_expected = [0, 4.6211716e-01, 0, 0, 0, 0]
+        metrics_expected = [0, 4.6211716e-01, 0]
         metrics = difference.evaluate(self.reference)
         np.testing.assert_almost_equal(metrics, metrics_expected)
 
         # Multi-component, currently not implemented
         with self.assertRaises(CADETProcessError):
             difference = Shape(self.reference, use_derivative=False)
-            metrics_expected = [0, 0, 0]
+            metrics_expected = [0, 0]
         with self.assertRaises(CADETProcessError):
             difference = Shape(self.reference_single)
             metrics = difference.evaluate(self.reference)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `CADET-Process-0.9.0/tests/test_equilibrium.py` & `cadet_process-0.9.1/tests/test_equilibrium.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_events.py` & `cadet_process-0.9.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_flow_sheet.py` & `cadet_process-0.9.1/tests/test_flow_sheet.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_fractions.py` & `cadet_process-0.9.1/tests/test_fractions.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_individual.py` & `cadet_process-0.9.1/tests/test_individual.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_optimization_integration.py` & `cadet_process-0.9.1/tests/test_optimization_integration.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_optimization_problem.py` & `cadet_process-0.9.1/tests/test_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_optimization_results.py` & `cadet_process-0.9.1/tests/test_optimization_results.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_optimizer_behavior.py` & `cadet_process-0.9.1/tests/test_optimizer_behavior.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 )
 
 # =========================
 #   Test-Optimizer Setup
 # =========================
 
 SOO_TEST_KWARGS = {
-    "atol": 0.05, # allows absolute 0.05 deviation (low values) of solution or
-    "rtol": 0.1,  # 0.1 alows 10% deviation of true solution
+    "atol": 0.05,   # allows absolute 0.05 deviation (low values) of solution or
+    "rtol": 0.1,    # 0.1 alows 10% deviation of true solution
 }
 
 MOO_TEST_KWARGS = {
     "atol": 0.01,
     "rtol": 0.1,
     "mismatch_tol": 0.33,  # 75 % of all solutions must lie on the pareto front
 }
@@ -55,19 +55,21 @@
 NON_DEFAULT_PARAMETERS = [
     (NEHVI, LinearConstraintsMooTestProblem,
         {"n_init_evals": 20, "n_max_evals": 40}),
     (U_NSGA3, NonlinearConstraintsMooTestProblem,
         {"pop_size": 300, "n_max_gen": 50}),
 ]
 
+
 def skip_if_combination_excluded(optimizer, problem):
     for o, p, r in EXCLUDE_COMBINATIONS:
         if isinstance(optimizer, o) and isinstance(problem, p):
             pytest.skip(reason=r)
 
+
 def set_non_default_parameters(optimizer, problem):
     for o, p, params in NON_DEFAULT_PARAMETERS:
         if isinstance(optimizer, o) and isinstance(problem, p):
             # override default parameters of the optimizer
             for pk, pv in params.items():
                 setattr(optimizer, pk, pv)
 
@@ -87,25 +89,26 @@
     xtol = XTOL
     cvtol = GTOL
     pop_size = 100
     n_max_gen = 20  # before used 100 generations --> this did not improve the fit
 
 
 class GPEI(GPEI):
-    n_init_evals=40
-    early_stopping_improvement_bar=1e-4
-    early_stopping_improvement_window=10
-    n_max_evals=50
+    n_init_evals = 40
+    early_stopping_improvement_bar = 1e-4
+    early_stopping_improvement_window = 10
+    n_max_evals = 50
 
 
 class NEHVI(NEHVI):
-    n_init_evals=50
-    early_stopping_improvement_bar=1e-4
-    early_stopping_improvement_window=10
-    n_max_evals=60
+    n_init_evals = 50
+    early_stopping_improvement_bar = 1e-4
+    early_stopping_improvement_window = 10
+    n_max_evals = 60
+
 
 # =========================
 #   Test problem factory
 # =========================
 
 @pytest.fixture(params=[
     # single objective problems
@@ -125,24 +128,26 @@
     partial(LinearConstraintsSooTestProblem, transform="linear"),
     partial(LinearEqualityConstraintsSooTestProblem, transform="linear"),
     partial(NonlinearLinearConstraintsSooTestProblem, transform="linear"),
 ])
 def optimization_problem(request):
     return request.param()
 
+
 @pytest.fixture(params=[
     SLSQP,
     TrustConstr,
     U_NSGA3,
     GPEI,
     NEHVI,
 ])
 def optimizer(request):
     return request.param()
 
+
 # =========================
 #          Tests
 # =========================
 
 def test_convergence(optimization_problem: TestProblem, optimizer: OptimizerBase):
     # only test problems that the optimizer can handle. The rest of the tests
     # will be marked as passed
@@ -171,14 +176,15 @@
             save_results=False,
         )
         if optimization_problem.n_objectives == 1:
             optimization_problem.test_if_solved(results, SOO_TEST_KWARGS)
         else:
             optimization_problem.test_if_solved(results, MOO_TEST_KWARGS)
 
+
 class AbortingCallback:
     """A callback that raises an exception after a specified number of calls."""
 
     def __init__(self, n_max_evals=2, abort=True):
         """Initialize callback with maximum number of evaluations and whether to abort."""
         self.n_calls = 0
         self.n_max_evals = n_max_evals
@@ -190,14 +196,15 @@
 
     def __call__(self, results):
         """Check the number of calls and raises an exception if the maximum has been reached."""
         if self.abort and self.n_calls >= self.n_max_evals:
             raise RuntimeError("Max number of evaluations reached. Aborting!")
         self.n_calls += 1
 
+
 def test_resume_from_checkpoint(
         optimization_problem: TestProblem, optimizer: OptimizerBase
     ):
     pytest.skip()
 
     # TODO: Do we need to run this for all problems?
     if optimizer.check_optimization_problem(optimization_problem):
```

### Comparing `CADET-Process-0.9.0/tests/test_parallelization_adapter.py` & `cadet_process-0.9.1/tests/test_parallelization_adapter.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_parameters.py` & `cadet_process-0.9.1/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_performance.py` & `cadet_process-0.9.1/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_population.py` & `cadet_process-0.9.1/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_pymoo.py` & `cadet_process-0.9.1/tests/test_pymoo.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_reaction.py` & `cadet_process-0.9.1/tests/test_reaction.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_sections.py` & `cadet_process-0.9.1/tests/test_sections.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_solution.py` & `cadet_process-0.9.1/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_transform.py` & `cadet_process-0.9.1/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `CADET-Process-0.9.0/tests/test_unit_operation.py` & `cadet_process-0.9.1/tests/test_unit_operation.py`

 * *Files identical despite different names*


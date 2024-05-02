# Comparing `tmp/analogvnn-1.0.7.tar.gz` & `tmp/analogvnn-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analogvnn-1.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "analogvnn-1.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `analogvnn-1.0.7.tar` & `analogvnn-1.0.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    17182 2023-11-22 06:26:23.971549 analogvnn-1.0.7/LICENSE
--rw-r--r--   0        0        0     3679 2023-11-22 06:36:48.581100 analogvnn-1.0.7/README.md
--rw-r--r--   0        0        0      728 2023-11-22 06:26:23.972550 analogvnn-1.0.7/analogvnn/__init__.py
--rw-r--r--   0        0        0     2873 2023-11-22 06:26:23.972550 analogvnn-1.0.7/analogvnn/backward/BackwardFunction.py
--rw-r--r--   0        0        0      930 2023-11-22 06:26:23.973549 analogvnn-1.0.7/analogvnn/backward/BackwardIdentity.py
--rw-r--r--   0        0        0    10140 2023-11-22 06:26:23.973549 analogvnn-1.0.7/analogvnn/backward/BackwardModule.py
--rw-r--r--   0        0        0      894 2023-11-22 06:26:23.974319 analogvnn-1.0.7/analogvnn/backward/BackwardUsingForward.py
--rw-r--r--   0        0        0        0 2023-11-22 06:26:23.974319 analogvnn-1.0.7/analogvnn/backward/__init__.py
--rw-r--r--   0        0        0       43 2023-11-22 06:26:23.974319 analogvnn-1.0.7/analogvnn/fn/__init__.py
--rw-r--r--   0        0        0      609 2023-11-22 06:26:23.975325 analogvnn-1.0.7/analogvnn/fn/dirac_delta.py
--rw-r--r--   0        0        0     1998 2023-11-22 06:26:23.975325 analogvnn-1.0.7/analogvnn/fn/reduce_precision.py
--rw-r--r--   0        0        0     1145 2023-11-22 06:26:23.975325 analogvnn-1.0.7/analogvnn/fn/test.py
--rw-r--r--   0        0        0      435 2023-11-22 06:26:23.976328 analogvnn-1.0.7/analogvnn/fn/to_matrix.py
--rw-r--r--   0        0        0     2154 2023-11-22 06:26:23.976328 analogvnn-1.0.7/analogvnn/fn/train.py
--rw-r--r--   0        0        0     6381 2023-11-22 06:27:56.452683 analogvnn-1.0.7/analogvnn/graph/AccumulateGrad.py
--rw-r--r--   0        0        0    16888 2023-11-22 06:26:23.977358 analogvnn-1.0.7/analogvnn/graph/AcyclicDirectedGraph.py
--rw-r--r--   0        0        0     3106 2023-11-22 06:26:23.977358 analogvnn-1.0.7/analogvnn/graph/ArgsKwargs.py
--rw-r--r--   0        0        0    12600 2023-11-22 06:26:23.978324 analogvnn-1.0.7/analogvnn/graph/BackwardGraph.py
--rw-r--r--   0        0        0     5066 2023-11-22 06:27:56.452683 analogvnn-1.0.7/analogvnn/graph/ForwardGraph.py
--rw-r--r--   0        0        0      503 2023-11-22 06:26:23.978324 analogvnn-1.0.7/analogvnn/graph/GraphEnum.py
--rw-r--r--   0        0        0     1655 2023-11-22 06:26:23.979324 analogvnn-1.0.7/analogvnn/graph/ModelGraph.py
--rw-r--r--   0        0        0     4036 2023-11-22 06:26:23.979324 analogvnn-1.0.7/analogvnn/graph/ModelGraphState.py
--rw-r--r--   0        0        0        0 2023-11-22 06:26:23.979324 analogvnn-1.0.7/analogvnn/graph/__init__.py
--rw-r--r--   0        0        0     2444 2023-11-22 06:26:23.980325 analogvnn-1.0.7/analogvnn/graph/to_graph_viz_digraph.py
--rw-r--r--   0        0        0     3326 2023-11-22 06:26:23.980325 analogvnn-1.0.7/analogvnn/nn/Linear.py
--rw-r--r--   0        0        0        0 2023-11-22 06:26:23.980325 analogvnn-1.0.7/analogvnn/nn/__init__.py
--rw-r--r--   0        0        0     1149 2023-11-22 06:26:23.981324 analogvnn-1.0.7/analogvnn/nn/activation/Activation.py
--rw-r--r--   0        0        0      944 2023-11-22 06:26:23.981324 analogvnn-1.0.7/analogvnn/nn/activation/BinaryStep.py
--rw-r--r--   0        0        0     3336 2023-11-22 06:26:23.981324 analogvnn-1.0.7/analogvnn/nn/activation/ELU.py
--rw-r--r--   0        0        0     2054 2023-11-22 06:29:34.173996 analogvnn-1.0.7/analogvnn/nn/activation/Gaussian.py
--rw-r--r--   0        0        0     1622 2023-11-22 06:26:23.982325 analogvnn-1.0.7/analogvnn/nn/activation/Identity.py
--rw-r--r--   0        0        0     4197 2023-11-22 06:26:23.983325 analogvnn-1.0.7/analogvnn/nn/activation/ReLU.py
--rw-r--r--   0        0        0      979 2023-11-22 06:26:23.983325 analogvnn-1.0.7/analogvnn/nn/activation/SiLU.py
--rw-r--r--   0        0        0     1953 2023-11-22 06:26:23.983325 analogvnn-1.0.7/analogvnn/nn/activation/Sigmoid.py
--rw-r--r--   0        0        0     1765 2023-11-22 06:26:23.984325 analogvnn-1.0.7/analogvnn/nn/activation/Tanh.py
--rw-r--r--   0        0        0        0 2023-11-22 06:26:23.984325 analogvnn-1.0.7/analogvnn/nn/activation/__init__.py
--rw-r--r--   0        0        0      895 2023-11-22 06:26:23.984325 analogvnn-1.0.7/analogvnn/nn/module/FullSequential.py
--rw-r--r--   0        0        0     9231 2023-11-22 06:26:23.985325 analogvnn-1.0.7/analogvnn/nn/module/Layer.py
--rw-r--r--   0        0        0    10932 2023-11-22 06:26:23.985325 analogvnn-1.0.7/analogvnn/nn/module/Model.py
--rw-r--r--   0        0        0     1470 2023-11-22 06:26:23.985325 analogvnn-1.0.7/analogvnn/nn/module/Sequential.py
--rw-r--r--   0        0        0        0 2023-11-22 06:26:23.986324 analogvnn-1.0.7/analogvnn/nn/module/__init__.py
--rw-r--r--   0        0        0     7169 2023-11-22 06:26:23.986324 analogvnn-1.0.7/analogvnn/nn/noise/GaussianNoise.py
--rw-r--r--   0        0        0     7025 2023-11-22 06:26:23.987325 analogvnn-1.0.7/analogvnn/nn/noise/LaplacianNoise.py
--rw-r--r--   0        0        0      154 2023-11-22 06:26:23.987325 analogvnn-1.0.7/analogvnn/nn/noise/Noise.py
--rw-r--r--   0        0        0    10404 2023-11-22 06:26:23.988324 analogvnn-1.0.7/analogvnn/nn/noise/PoissonNoise.py
--rw-r--r--   0        0        0     6860 2023-11-22 06:26:23.989326 analogvnn-1.0.7/analogvnn/nn/noise/UniformNoise.py
--rw-r--r--   0        0        0        0 2023-11-22 06:26:23.989326 analogvnn-1.0.7/analogvnn/nn/noise/__init__.py
--rw-r--r--   0        0        0     2044 2023-11-22 06:26:23.990325 analogvnn-1.0.7/analogvnn/nn/normalize/Clamp.py
--rw-r--r--   0        0        0     4469 2023-11-22 06:26:23.990325 analogvnn-1.0.7/analogvnn/nn/normalize/LPNorm.py
--rw-r--r--   0        0        0      170 2023-11-22 06:26:23.990325 analogvnn-1.0.7/analogvnn/nn/normalize/Normalize.py
--rw-r--r--   0        0        0        0 2023-11-22 06:26:23.990325 analogvnn-1.0.7/analogvnn/nn/normalize/__init__.py
--rw-r--r--   0        0        0      166 2023-11-22 06:26:23.991325 analogvnn-1.0.7/analogvnn/nn/precision/Precision.py
--rw-r--r--   0        0        0     3092 2023-11-22 06:26:23.991325 analogvnn-1.0.7/analogvnn/nn/precision/ReducePrecision.py
--rw-r--r--   0        0        0     2554 2023-11-22 06:26:23.992324 analogvnn-1.0.7/analogvnn/nn/precision/StochasticReducePrecision.py
--rw-r--r--   0        0        0        0 2023-11-22 06:26:23.992324 analogvnn-1.0.7/analogvnn/nn/precision/__init__.py
--rw-r--r--   0        0        0     7949 2023-11-22 06:26:23.993324 analogvnn-1.0.7/analogvnn/parameter/PseudoParameter.py
--rw-r--r--   0        0        0        0 2023-11-22 06:26:23.993324 analogvnn-1.0.7/analogvnn/parameter/__init__.py
--rw-r--r--   0        0        0        0 2023-11-22 06:26:23.993324 analogvnn-1.0.7/analogvnn/py.typed
--rw-r--r--   0        0        0     7979 2023-11-22 06:26:23.993324 analogvnn-1.0.7/analogvnn/utils/TensorboardModelLog.py
--rw-r--r--   0        0        0        0 2023-11-22 06:26:23.994325 analogvnn-1.0.7/analogvnn/utils/__init__.py
--rw-r--r--   0        0        0      591 2023-11-22 06:26:23.994325 analogvnn-1.0.7/analogvnn/utils/common_types.py
--rw-r--r--   0        0        0     2404 2023-11-22 06:26:23.994325 analogvnn-1.0.7/analogvnn/utils/get_model_summaries.py
--rw-r--r--   0        0        0     3016 2023-11-22 06:26:23.995324 analogvnn-1.0.7/analogvnn/utils/is_cpu_cuda.py
--rw-r--r--   0        0        0    35029 2023-11-22 06:26:23.995324 analogvnn-1.0.7/analogvnn/utils/render_autograd_graph.py
--rw-r--r--   0        0        0     1011 2023-11-22 06:26:23.996325 analogvnn-1.0.7/analogvnn/utils/to_tensor_parameter.py
--rw-r--r--   0        0        0     3418 2023-11-22 06:43:17.256979 analogvnn-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     6916 1970-01-01 00:00:00.000000 analogvnn-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    17182 2023-11-22 06:26:23.971549 analogvnn-1.0.8/LICENSE
+-rw-r--r--   0        0        0     3856 2024-05-02 23:21:47.451513 analogvnn-1.0.8/README.md
+-rw-r--r--   0        0        0      728 2023-11-22 06:26:23.972550 analogvnn-1.0.8/analogvnn/__init__.py
+-rw-r--r--   0        0        0     2873 2023-11-22 06:26:23.972550 analogvnn-1.0.8/analogvnn/backward/BackwardFunction.py
+-rw-r--r--   0        0        0      930 2023-11-22 06:26:23.973549 analogvnn-1.0.8/analogvnn/backward/BackwardIdentity.py
+-rw-r--r--   0        0        0    10140 2023-11-22 06:26:23.973549 analogvnn-1.0.8/analogvnn/backward/BackwardModule.py
+-rw-r--r--   0        0        0      894 2023-11-22 06:26:23.974319 analogvnn-1.0.8/analogvnn/backward/BackwardUsingForward.py
+-rw-r--r--   0        0        0        0 2023-11-22 06:26:23.974319 analogvnn-1.0.8/analogvnn/backward/__init__.py
+-rw-r--r--   0        0        0       43 2023-11-22 06:26:23.974319 analogvnn-1.0.8/analogvnn/fn/__init__.py
+-rw-r--r--   0        0        0      609 2023-11-22 06:26:23.975325 analogvnn-1.0.8/analogvnn/fn/dirac_delta.py
+-rw-r--r--   0        0        0     1998 2024-05-02 23:09:15.204222 analogvnn-1.0.8/analogvnn/fn/reduce_precision.py
+-rw-r--r--   0        0        0     1145 2023-11-22 06:26:23.975325 analogvnn-1.0.8/analogvnn/fn/test.py
+-rw-r--r--   0        0        0      435 2023-11-22 06:26:23.976328 analogvnn-1.0.8/analogvnn/fn/to_matrix.py
+-rw-r--r--   0        0        0     2154 2023-11-22 06:26:23.976328 analogvnn-1.0.8/analogvnn/fn/train.py
+-rw-r--r--   0        0        0     6381 2023-11-22 06:27:56.452683 analogvnn-1.0.8/analogvnn/graph/AccumulateGrad.py
+-rw-r--r--   0        0        0    16888 2023-11-22 06:26:23.977358 analogvnn-1.0.8/analogvnn/graph/AcyclicDirectedGraph.py
+-rw-r--r--   0        0        0     3106 2023-11-22 06:26:23.977358 analogvnn-1.0.8/analogvnn/graph/ArgsKwargs.py
+-rw-r--r--   0        0        0    12600 2023-11-22 06:26:23.978324 analogvnn-1.0.8/analogvnn/graph/BackwardGraph.py
+-rw-r--r--   0        0        0     5066 2023-11-22 06:27:56.452683 analogvnn-1.0.8/analogvnn/graph/ForwardGraph.py
+-rw-r--r--   0        0        0      503 2023-11-22 06:26:23.978324 analogvnn-1.0.8/analogvnn/graph/GraphEnum.py
+-rw-r--r--   0        0        0     1655 2023-11-22 06:26:23.979324 analogvnn-1.0.8/analogvnn/graph/ModelGraph.py
+-rw-r--r--   0        0        0     4036 2023-11-22 06:26:23.979324 analogvnn-1.0.8/analogvnn/graph/ModelGraphState.py
+-rw-r--r--   0        0        0        0 2023-11-22 06:26:23.979324 analogvnn-1.0.8/analogvnn/graph/__init__.py
+-rw-r--r--   0        0        0     2444 2023-11-22 06:26:23.980325 analogvnn-1.0.8/analogvnn/graph/to_graph_viz_digraph.py
+-rw-r--r--   0        0        0     3326 2023-11-22 06:26:23.980325 analogvnn-1.0.8/analogvnn/nn/Linear.py
+-rw-r--r--   0        0        0        0 2023-11-22 06:26:23.980325 analogvnn-1.0.8/analogvnn/nn/__init__.py
+-rw-r--r--   0        0        0     1149 2023-11-22 06:26:23.981324 analogvnn-1.0.8/analogvnn/nn/activation/Activation.py
+-rw-r--r--   0        0        0      944 2023-11-22 06:26:23.981324 analogvnn-1.0.8/analogvnn/nn/activation/BinaryStep.py
+-rw-r--r--   0        0        0     3336 2023-11-22 06:26:23.981324 analogvnn-1.0.8/analogvnn/nn/activation/ELU.py
+-rw-r--r--   0        0        0     2054 2023-11-22 06:29:34.173996 analogvnn-1.0.8/analogvnn/nn/activation/Gaussian.py
+-rw-r--r--   0        0        0     1622 2023-11-22 06:26:23.982325 analogvnn-1.0.8/analogvnn/nn/activation/Identity.py
+-rw-r--r--   0        0        0     4197 2023-11-22 06:26:23.983325 analogvnn-1.0.8/analogvnn/nn/activation/ReLU.py
+-rw-r--r--   0        0        0      979 2023-11-22 06:26:23.983325 analogvnn-1.0.8/analogvnn/nn/activation/SiLU.py
+-rw-r--r--   0        0        0     1953 2023-11-22 06:26:23.983325 analogvnn-1.0.8/analogvnn/nn/activation/Sigmoid.py
+-rw-r--r--   0        0        0     1765 2023-11-22 06:26:23.984325 analogvnn-1.0.8/analogvnn/nn/activation/Tanh.py
+-rw-r--r--   0        0        0        0 2023-11-22 06:26:23.984325 analogvnn-1.0.8/analogvnn/nn/activation/__init__.py
+-rw-r--r--   0        0        0      895 2023-11-22 06:26:23.984325 analogvnn-1.0.8/analogvnn/nn/module/FullSequential.py
+-rw-r--r--   0        0        0     9231 2023-11-22 06:26:23.985325 analogvnn-1.0.8/analogvnn/nn/module/Layer.py
+-rw-r--r--   0        0        0    10932 2023-11-22 06:26:23.985325 analogvnn-1.0.8/analogvnn/nn/module/Model.py
+-rw-r--r--   0        0        0     1470 2023-11-22 06:26:23.985325 analogvnn-1.0.8/analogvnn/nn/module/Sequential.py
+-rw-r--r--   0        0        0        0 2023-11-22 06:26:23.986324 analogvnn-1.0.8/analogvnn/nn/module/__init__.py
+-rw-r--r--   0        0        0     7169 2023-11-22 06:26:23.986324 analogvnn-1.0.8/analogvnn/nn/noise/GaussianNoise.py
+-rw-r--r--   0        0        0     7025 2023-11-22 06:26:23.987325 analogvnn-1.0.8/analogvnn/nn/noise/LaplacianNoise.py
+-rw-r--r--   0        0        0      154 2023-11-22 06:26:23.987325 analogvnn-1.0.8/analogvnn/nn/noise/Noise.py
+-rw-r--r--   0        0        0    10404 2023-11-22 06:26:23.988324 analogvnn-1.0.8/analogvnn/nn/noise/PoissonNoise.py
+-rw-r--r--   0        0        0     6860 2023-11-22 06:26:23.989326 analogvnn-1.0.8/analogvnn/nn/noise/UniformNoise.py
+-rw-r--r--   0        0        0        0 2023-11-22 06:26:23.989326 analogvnn-1.0.8/analogvnn/nn/noise/__init__.py
+-rw-r--r--   0        0        0     2044 2023-11-22 06:26:23.990325 analogvnn-1.0.8/analogvnn/nn/normalize/Clamp.py
+-rw-r--r--   0        0        0     4469 2023-11-22 06:26:23.990325 analogvnn-1.0.8/analogvnn/nn/normalize/LPNorm.py
+-rw-r--r--   0        0        0      170 2023-11-22 06:26:23.990325 analogvnn-1.0.8/analogvnn/nn/normalize/Normalize.py
+-rw-r--r--   0        0        0        0 2023-11-22 06:26:23.990325 analogvnn-1.0.8/analogvnn/nn/normalize/__init__.py
+-rw-r--r--   0        0        0      166 2023-11-22 06:26:23.991325 analogvnn-1.0.8/analogvnn/nn/precision/Precision.py
+-rw-r--r--   0        0        0     3092 2023-11-22 06:26:23.991325 analogvnn-1.0.8/analogvnn/nn/precision/ReducePrecision.py
+-rw-r--r--   0        0        0     2554 2023-11-22 06:26:23.992324 analogvnn-1.0.8/analogvnn/nn/precision/StochasticReducePrecision.py
+-rw-r--r--   0        0        0        0 2023-11-22 06:26:23.992324 analogvnn-1.0.8/analogvnn/nn/precision/__init__.py
+-rw-r--r--   0        0        0     8294 2024-05-02 23:09:21.704562 analogvnn-1.0.8/analogvnn/parameter/PseudoParameter.py
+-rw-r--r--   0        0        0        0 2023-11-22 06:26:23.993324 analogvnn-1.0.8/analogvnn/parameter/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-22 06:26:23.993324 analogvnn-1.0.8/analogvnn/py.typed
+-rw-r--r--   0        0        0     7979 2023-11-22 06:26:23.993324 analogvnn-1.0.8/analogvnn/utils/TensorboardModelLog.py
+-rw-r--r--   0        0        0        0 2023-11-22 06:26:23.994325 analogvnn-1.0.8/analogvnn/utils/__init__.py
+-rw-r--r--   0        0        0      591 2023-11-22 06:26:23.994325 analogvnn-1.0.8/analogvnn/utils/common_types.py
+-rw-r--r--   0        0        0     2404 2023-11-22 06:26:23.994325 analogvnn-1.0.8/analogvnn/utils/get_model_summaries.py
+-rw-r--r--   0        0        0     3016 2023-11-22 06:26:23.995324 analogvnn-1.0.8/analogvnn/utils/is_cpu_cuda.py
+-rw-r--r--   0        0        0    35029 2023-11-22 06:26:23.995324 analogvnn-1.0.8/analogvnn/utils/render_autograd_graph.py
+-rw-r--r--   0        0        0     1011 2023-11-22 06:26:23.996325 analogvnn-1.0.8/analogvnn/utils/to_tensor_parameter.py
+-rw-r--r--   0        0        0     3418 2024-05-02 23:28:43.532163 analogvnn-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7088 1970-01-01 00:00:00.000000 analogvnn-1.0.8/PKG-INFO
```

### Comparing `analogvnn-1.0.7/LICENSE` & `analogvnn-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/README.md` & `analogvnn-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # AnalogVNN
 
 [![arXiv](https://img.shields.io/badge/arXiv-2210.10048-orange.svg)](https://arxiv.org/abs/2210.10048)
+[![AML](https://img.shields.io/badge/AML-10.1063/5.0134156-orange.svg)](https://doi.org/10.1063/5.0134156)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Vivswan/AnalogVNN/blob/release/docs/_static/AnalogVNN_Demo.ipynb)
 
 [![PyPI version](https://badge.fury.io/py/analogvnn.svg)](https://badge.fury.io/py/analogvnn)
 [![Documentation Status](https://readthedocs.org/projects/analogvnn/badge/?version=stable)](https://analogvnn.readthedocs.io/en/stable/?badge=stable)
 [![Python](https://img.shields.io/badge/python-3.7--3.11-blue)](https://badge.fury.io/py/analogvnn)
 [![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-blue.svg)](https://opensource.org/licenses/MPL-2.0)
 
@@ -48,28 +49,32 @@
 gaining insights into how normalization, activation function, reduced precision, and
 noise influence accuracy in analog photonic neural networks. By following the same layer
 structure design present in PyTorch, the AnalogVNN framework allows users to convert most
 digital neural network models to their analog counterparts with just a few lines of code,
 taking full advantage of the open-source optimization, deep learning, and GPU acceleration
 libraries available through PyTorch.
 
-AnalogVNN Paper: [https://arxiv.org/abs/2210.10048](https://arxiv.org/abs/2210.10048)
+AnalogVNN Paper: [https://doi.org/10.1063/5.0134156](https://doi.org/10.1063/5.0134156)
 
 ## Citing AnalogVNN
 
 We would appreciate if you cite the following paper in your publications for which you used AnalogVNN:
 
 ```bibtex
-@article{shah2022analogvnn,
+@article{shah2023analogvnn,
   title={AnalogVNN: A fully modular framework for modeling and optimizing photonic neural networks},
   author={Shah, Vivswan and Youngblood, Nathan},
-  journal={arXiv preprint arXiv:2210.10048},
-  year={2022}
+  journal={APL Machine Learning},
+  volume={1},
+  number={2},
+  year={2023},
+  publisher={AIP Publishing}
 }
 ```
 
 Or in textual form:
 
 ```text
 Vivswan Shah, and Nathan Youngblood. "AnalogVNN: A fully modular framework for modeling 
-and optimizing photonic neural networks." arXiv preprint arXiv:2210.10048 (2022).
+and optimizing photonic neural networks." APL Machine Learning 1.2 (2023).
+DOI: 10.1063/5.0134156
 ```
```

### Comparing `analogvnn-1.0.7/analogvnn/__init__.py` & `analogvnn-1.0.8/analogvnn/__init__.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/backward/BackwardFunction.py` & `analogvnn-1.0.8/analogvnn/backward/BackwardFunction.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/backward/BackwardIdentity.py` & `analogvnn-1.0.8/analogvnn/backward/BackwardIdentity.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/backward/BackwardModule.py` & `analogvnn-1.0.8/analogvnn/backward/BackwardModule.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/backward/BackwardUsingForward.py` & `analogvnn-1.0.8/analogvnn/backward/BackwardUsingForward.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/fn/dirac_delta.py` & `analogvnn-1.0.8/analogvnn/fn/dirac_delta.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/fn/reduce_precision.py` & `analogvnn-1.0.8/analogvnn/fn/reduce_precision.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,27 +8,24 @@
 
 def reduce_precision(x: TENSOR_OPERABLE, precision: TENSOR_OPERABLE, divide: TENSOR_OPERABLE) -> TENSOR_OPERABLE:
     """Takes `x` and reduces its precision to `precision` by rounding to the nearest multiple of `precision`.
 
     Args:
       x (TENSOR_OPERABLE): Tensor
       precision (TENSOR_OPERABLE): the precision of the quantization.
-      divide (TENSOR_OPERABLE): the number of bits to be reduced
+      divide (TENSOR_OPERABLE): the rounding value that is if divide is 0.5,
+         then 0.6 will be rounded to 1.0 and 0.4 will be rounded to 0.0.
 
     Returns:
       TENSOR_OPERABLE: TENSOR_OPERABLE with the same shape as x, but with values rounded to the nearest
       multiple of precision.
     """
 
     x = x if isinstance(x, Tensor) else torch.tensor(x, requires_grad=False)
-    g: Tensor = x * precision
-    f = torch.sign(g) * torch.maximum(
-        torch.floor(torch.abs(g)),
-        torch.ceil(torch.abs(g) - divide)
-    ) * (1 / precision)
+    f = torch.sign(x) * torch.ceil(torch.abs(x * precision) - divide) * (1 / precision)
     return f
 
 
 def stochastic_reduce_precision(x: TENSOR_OPERABLE, precision: TENSOR_OPERABLE) -> TENSOR_OPERABLE:
     """Takes `x` and reduces its precision by rounding to the nearest multiple of `precision` with stochastic scheme.
 
     Args:
```

### Comparing `analogvnn-1.0.7/analogvnn/fn/test.py` & `analogvnn-1.0.8/analogvnn/fn/test.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/fn/train.py` & `analogvnn-1.0.8/analogvnn/fn/train.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/graph/AccumulateGrad.py` & `analogvnn-1.0.8/analogvnn/graph/AccumulateGrad.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/graph/AcyclicDirectedGraph.py` & `analogvnn-1.0.8/analogvnn/graph/AcyclicDirectedGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/graph/ArgsKwargs.py` & `analogvnn-1.0.8/analogvnn/graph/ArgsKwargs.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/graph/BackwardGraph.py` & `analogvnn-1.0.8/analogvnn/graph/BackwardGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/graph/ForwardGraph.py` & `analogvnn-1.0.8/analogvnn/graph/ForwardGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/graph/ModelGraph.py` & `analogvnn-1.0.8/analogvnn/graph/ModelGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/graph/ModelGraphState.py` & `analogvnn-1.0.8/analogvnn/graph/ModelGraphState.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/graph/to_graph_viz_digraph.py` & `analogvnn-1.0.8/analogvnn/graph/to_graph_viz_digraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/Linear.py` & `analogvnn-1.0.8/analogvnn/nn/Linear.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/activation/Activation.py` & `analogvnn-1.0.8/analogvnn/nn/activation/Activation.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/activation/BinaryStep.py` & `analogvnn-1.0.8/analogvnn/nn/activation/BinaryStep.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/activation/ELU.py` & `analogvnn-1.0.8/analogvnn/nn/activation/ELU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/activation/Gaussian.py` & `analogvnn-1.0.8/analogvnn/nn/activation/Gaussian.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/activation/Identity.py` & `analogvnn-1.0.8/analogvnn/nn/activation/Identity.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/activation/ReLU.py` & `analogvnn-1.0.8/analogvnn/nn/activation/ReLU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/activation/SiLU.py` & `analogvnn-1.0.8/analogvnn/nn/activation/SiLU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/activation/Sigmoid.py` & `analogvnn-1.0.8/analogvnn/nn/activation/Sigmoid.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/activation/Tanh.py` & `analogvnn-1.0.8/analogvnn/nn/activation/Tanh.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/module/FullSequential.py` & `analogvnn-1.0.8/analogvnn/nn/module/FullSequential.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/module/Layer.py` & `analogvnn-1.0.8/analogvnn/nn/module/Layer.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/module/Model.py` & `analogvnn-1.0.8/analogvnn/nn/module/Model.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/module/Sequential.py` & `analogvnn-1.0.8/analogvnn/nn/module/Sequential.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/noise/GaussianNoise.py` & `analogvnn-1.0.8/analogvnn/nn/noise/GaussianNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/noise/LaplacianNoise.py` & `analogvnn-1.0.8/analogvnn/nn/noise/LaplacianNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/noise/PoissonNoise.py` & `analogvnn-1.0.8/analogvnn/nn/noise/PoissonNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/noise/UniformNoise.py` & `analogvnn-1.0.8/analogvnn/nn/noise/UniformNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/normalize/Clamp.py` & `analogvnn-1.0.8/analogvnn/nn/normalize/Clamp.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/normalize/LPNorm.py` & `analogvnn-1.0.8/analogvnn/nn/normalize/LPNorm.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/precision/ReducePrecision.py` & `analogvnn-1.0.8/analogvnn/nn/precision/ReducePrecision.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/nn/precision/StochasticReducePrecision.py` & `analogvnn-1.0.8/analogvnn/nn/precision/StochasticReducePrecision.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/parameter/PseudoParameter.py` & `analogvnn-1.0.8/analogvnn/parameter/PseudoParameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Callable, Any
+from typing import Callable, Any, Optional, Union, Tuple
 
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.nn import ModuleDict
 from torch.nn.utils import parametrize
 
@@ -215,31 +215,41 @@
             module.parametrizations = ModuleDict()
 
         module.parametrizations[param_name] = new_param
         parametrize._inject_property(module, param_name)
         return new_param
 
     @classmethod
-    def parametrize_module(cls, module: nn.Module, transformation: Callable, requires_grad: bool = True):
+    def parametrize_module(
+            cls,
+            module: nn.Module,
+            transformation: Callable,
+            requires_grad: bool = True,
+            types: Optional[Union[type, Tuple[type]]] = None,
+    ):
         """Parametrize all parameters of a module.
 
         Args:
             module (nn.Module): the module parameters to parametrize.
             transformation (Callable): the transformation.
             requires_grad (bool): if True, only parametrized parameters that require gradients.
+            types (Union[type, Tuple[type]]): the type or tuple of types to parametrize.
         """
 
         with torch.no_grad():
             for name, parameter in list(module.named_parameters(recurse=False)):
                 if isinstance(parameter, cls):
                     continue
 
                 if requires_grad and not parameter.requires_grad:
                     continue
 
+                if types is not None and not isinstance(parameter, types):
+                    continue
+
                 cls.parameterize(module=module, param_name=name, transformation=transformation)
 
             for sub_module in module.children():
                 if sub_module == module:
                     continue
                 if hasattr(module, 'parametrizations') and (
                         sub_module is module.parametrizations or sub_module in module.parametrizations
```

### Comparing `analogvnn-1.0.7/analogvnn/utils/TensorboardModelLog.py` & `analogvnn-1.0.8/analogvnn/utils/TensorboardModelLog.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/utils/common_types.py` & `analogvnn-1.0.8/analogvnn/utils/common_types.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/utils/get_model_summaries.py` & `analogvnn-1.0.8/analogvnn/utils/get_model_summaries.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/utils/is_cpu_cuda.py` & `analogvnn-1.0.8/analogvnn/utils/is_cpu_cuda.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/utils/render_autograd_graph.py` & `analogvnn-1.0.8/analogvnn/utils/render_autograd_graph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/analogvnn/utils/to_tensor_parameter.py` & `analogvnn-1.0.8/analogvnn/utils/to_tensor_parameter.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.7/pyproject.toml` & `analogvnn-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [tool.setuptools.packages.find]
 where = ["analogvnn"]
 
 [project]
 # $ pip install analogvnn
 name = "analogvnn"
-version = "1.0.7"
+version = "1.0.8"
 description = "A fully modular framework for modeling and optimizing analog/photonic neural networks"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["deep-learning", "analog", "photonics", "neural-network", "framework", "pytorch"]
 authors = [
     { name = "Vivswan Shah", email = "vivswanshah@pitt.edu" }
```

### Comparing `analogvnn-1.0.7/PKG-INFO` & `analogvnn-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analogvnn
-Version: 1.0.7
+Version: 1.0.8
 Summary: A fully modular framework for modeling and optimizing analog/photonic neural networks
 Keywords: deep-learning,analog,photonics,neural-network,framework,pytorch
 Author-email: Vivswan Shah <vivswanshah@pitt.edu>
 Maintainer-email: Vivswan Shah <vivswanshah@pitt.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -69,14 +69,15 @@
 Provides-Extra: flake8
 Provides-Extra: full
 Provides-Extra: test
 
 # AnalogVNN
 
 [![arXiv](https://img.shields.io/badge/arXiv-2210.10048-orange.svg)](https://arxiv.org/abs/2210.10048)
+[![AML](https://img.shields.io/badge/AML-10.1063/5.0134156-orange.svg)](https://doi.org/10.1063/5.0134156)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Vivswan/AnalogVNN/blob/release/docs/_static/AnalogVNN_Demo.ipynb)
 
 [![PyPI version](https://badge.fury.io/py/analogvnn.svg)](https://badge.fury.io/py/analogvnn)
 [![Documentation Status](https://readthedocs.org/projects/analogvnn/badge/?version=stable)](https://analogvnn.readthedocs.io/en/stable/?badge=stable)
 [![Python](https://img.shields.io/badge/python-3.7--3.11-blue)](https://badge.fury.io/py/analogvnn)
 [![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-blue.svg)](https://opensource.org/licenses/MPL-2.0)
 
@@ -120,28 +121,32 @@
 gaining insights into how normalization, activation function, reduced precision, and
 noise influence accuracy in analog photonic neural networks. By following the same layer
 structure design present in PyTorch, the AnalogVNN framework allows users to convert most
 digital neural network models to their analog counterparts with just a few lines of code,
 taking full advantage of the open-source optimization, deep learning, and GPU acceleration
 libraries available through PyTorch.
 
-AnalogVNN Paper: [https://arxiv.org/abs/2210.10048](https://arxiv.org/abs/2210.10048)
+AnalogVNN Paper: [https://doi.org/10.1063/5.0134156](https://doi.org/10.1063/5.0134156)
 
 ## Citing AnalogVNN
 
 We would appreciate if you cite the following paper in your publications for which you used AnalogVNN:
 
 ```bibtex
-@article{shah2022analogvnn,
+@article{shah2023analogvnn,
   title={AnalogVNN: A fully modular framework for modeling and optimizing photonic neural networks},
   author={Shah, Vivswan and Youngblood, Nathan},
-  journal={arXiv preprint arXiv:2210.10048},
-  year={2022}
+  journal={APL Machine Learning},
+  volume={1},
+  number={2},
+  year={2023},
+  publisher={AIP Publishing}
 }
 ```
 
 Or in textual form:
 
 ```text
 Vivswan Shah, and Nathan Youngblood. "AnalogVNN: A fully modular framework for modeling 
-and optimizing photonic neural networks." arXiv preprint arXiv:2210.10048 (2022).
+and optimizing photonic neural networks." APL Machine Learning 1.2 (2023).
+DOI: 10.1063/5.0134156
 ```
```


# Comparing `tmp/ptflops-0.7.2.2.tar.gz` & `tmp/ptflops-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptflops-0.7.2.2.tar", last modified: Sun Jan 21 05:49:23 2024, max compression
+gzip compressed data, was "ptflops-0.7.3.tar", last modified: Sat May  4 03:20:37 2024, max compression
```

## Comparing `ptflops-0.7.2.2.tar` & `ptflops-0.7.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2024-01-21 05:49:23.317007 ptflops-0.7.2.2/
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     1075 2022-11-16 21:01:54.000000 ptflops-0.7.2.2/LICENSE
--rw-r--r--   0 vsovraso  (1002) vsovraso  (1002)     7232 2024-01-21 05:49:23.317007 ptflops-0.7.2.2/PKG-INFO
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     4731 2024-01-21 05:26:43.000000 ptflops-0.7.2.2/README.md
-drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2024-01-21 05:49:23.317007 ptflops-0.7.2.2/ptflops/
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)      482 2024-01-21 05:26:37.000000 ptflops-0.7.2.2/ptflops/__init__.py
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     4921 2024-01-21 05:26:37.000000 ptflops-0.7.2.2/ptflops/flops_counter.py
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)    17366 2024-01-03 23:19:38.000000 ptflops-0.7.2.2/ptflops/pytorch_engine.py
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)    14913 2023-12-25 01:16:29.000000 ptflops-0.7.2.2/ptflops/pytorch_ops.py
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     2481 2023-12-25 01:39:13.000000 ptflops-0.7.2.2/ptflops/utils.py
-drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2024-01-21 05:49:23.317007 ptflops-0.7.2.2/ptflops.egg-info/
--rw-r--r--   0 vsovraso  (1002) vsovraso  (1002)     7232 2024-01-21 05:49:23.000000 ptflops-0.7.2.2/ptflops.egg-info/PKG-INFO
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)      297 2024-01-21 05:49:23.000000 ptflops-0.7.2.2/ptflops.egg-info/SOURCES.txt
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        1 2024-01-21 05:49:23.000000 ptflops-0.7.2.2/ptflops.egg-info/dependency_links.txt
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)      112 2024-01-21 05:49:23.000000 ptflops-0.7.2.2/ptflops.egg-info/requires.txt
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        8 2024-01-21 05:49:23.000000 ptflops-0.7.2.2/ptflops.egg-info/top_level.txt
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     1293 2024-01-21 05:45:37.000000 ptflops-0.7.2.2/pyproject.toml
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)       38 2024-01-21 05:49:23.317007 ptflops-0.7.2.2/setup.cfg
+drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2024-05-04 03:20:37.235743 ptflops-0.7.3/
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     1075 2022-11-16 21:01:54.000000 ptflops-0.7.3/LICENSE
+-rw-r--r--   0 vsovraso  (1002) vsovraso  (1002)     8945 2024-05-04 03:20:37.235743 ptflops-0.7.3/PKG-INFO
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     6446 2024-05-04 02:21:29.000000 ptflops-0.7.3/README.md
+drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2024-05-04 03:20:37.235743 ptflops-0.7.3/ptflops/
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)      518 2024-05-04 02:21:29.000000 ptflops-0.7.3/ptflops/__init__.py
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     4952 2024-05-04 02:21:29.000000 ptflops-0.7.3/ptflops/aten_engine.py
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     3367 2024-05-04 02:21:29.000000 ptflops-0.7.3/ptflops/aten_ops.py
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     5878 2024-05-04 02:21:29.000000 ptflops-0.7.3/ptflops/flops_counter.py
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)    17367 2024-05-04 02:21:29.000000 ptflops-0.7.3/ptflops/pytorch_engine.py
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)    14913 2024-05-04 01:49:39.000000 ptflops-0.7.3/ptflops/pytorch_ops.py
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     2481 2023-12-25 01:39:13.000000 ptflops-0.7.3/ptflops/utils.py
+drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2024-05-04 03:20:37.235743 ptflops-0.7.3/ptflops.egg-info/
+-rw-r--r--   0 vsovraso  (1002) vsovraso  (1002)     8945 2024-05-04 03:20:37.000000 ptflops-0.7.3/ptflops.egg-info/PKG-INFO
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)      340 2024-05-04 03:20:37.000000 ptflops-0.7.3/ptflops.egg-info/SOURCES.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        1 2024-05-04 03:20:37.000000 ptflops-0.7.3/ptflops.egg-info/dependency_links.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)      112 2024-05-04 03:20:37.000000 ptflops-0.7.3/ptflops.egg-info/requires.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        8 2024-05-04 03:20:37.000000 ptflops-0.7.3/ptflops.egg-info/top_level.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     1291 2024-05-04 02:21:57.000000 ptflops-0.7.3/pyproject.toml
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)       38 2024-05-04 03:20:37.235743 ptflops-0.7.3/setup.cfg
```

### Comparing `ptflops-0.7.2.2/LICENSE` & `ptflops-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ptflops-0.7.2.2/PKG-INFO` & `ptflops-0.7.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptflops
-Version: 0.7.2.2
+Version: 0.7.3
 Summary: Flops counter for neural networks in pytorch framework
 Author-email: Vladislav Sovrasov <sovrasov.vlad@gmail.com>
 Maintainer-email: Vladislav Sovrasov <sovrasov.vlad@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Vladislav Sovrasov
         
@@ -46,19 +46,34 @@
 Requires-Dist: pytest==7.1.2; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 
 # Flops counting tool for neural networks in pytorch framework
 [![Pypi version](https://img.shields.io/pypi/v/ptflops.svg)](https://pypi.org/project/ptflops/)
 [![Build Status](https://travis-ci.com/sovrasov/flops-counter.pytorch.svg?branch=master)](https://travis-ci.com/sovrasov/flops-counter.pytorch)
 
-This script is designed to compute the theoretical amount of multiply-add operations
-in convolutional neural networks. It can also compute the number of parameters and
+This tool is designed to compute the theoretical amount of multiply-add operations
+in neural networks. It can also compute the number of parameters and
 print per-layer computational cost of a given network.
 
-Supported layers:
+`ptflops` has two backends, `pytorch` and `aten`. `pytorch` backend is a legacy one, it considers `nn.Modules` only. However,
+it's still useful, since it provides a better par-layer analytics for CNNs. In all other cases it's recommended to use
+`aten` backend, which considers aten operations, and therefore it covers more model architectures (including transformers).
+
+## `aten` backend
+### Operations considered:
+- aten.mm, aten.matmul, aten.addmm, aten.bmm
+- aten.convolution
+
+### Usage tips
+- Use `verbose=True` to see the operations which were not considered during complexity computation.
+- This backend prints per-module statistics only for modules directly nested into the root `nn.Module`.
+Deeper modules at the second level of nesting are not shown in the per-layer statistics.
+
+## `pytorch` backend
+### Supported layers:
 - Conv1d/2d/3d (including grouping)
 - ConvTranspose1d/2d/3d (including grouping)
 - BatchNorm1d/2d/3d, GroupNorm, InstanceNorm1d/2d/3d, LayerNorm
 - Activations (ReLU, PReLU, ELU, ReLU6, LeakyReLU, GELU)
 - Linear
 - Upsample
 - Poolings (AvgPool1d/2d/3d, MaxPool1d/2d/3d and adaptive ones)
@@ -66,28 +81,28 @@
 Experimental support:
 - RNN, LSTM, GRU (NLH layout is assumed)
 - RNNCell, LSTMCell, GRUCell
 - torch.nn.MultiheadAttention
 - torchvision.ops.DeformConv2d
 - visual transformers from [timm](https://github.com/huggingface/pytorch-image-models)
 
-Requirements: Pytorch >= 1.1, torchvision >= 0.3
-
-Thanks to @warmspringwinds for the initial version of script.
-
-## Usage tips
+### Usage tips
 
-- This tool doesn't take into account some of the `torch.nn.functional.*` and `tensor.*` operations. Therefore unsupported operations are
+- This backend doesn't take into account some of the `torch.nn.functional.*` and `tensor.*` operations. Therefore unsupported operations are
 not contributing to the final complexity estimation. See `ptflops/pytorch_ops.py:FUNCTIONAL_MAPPING,TENSOR_OPS_MAPPING` to check supported ops.
 - `ptflops` launches a given model on a random tensor and estimates amount of computations during inference. Complicated models can have several inputs, some of them could be optional. To construct non-trivial input one can use the `input_constructor` argument of the `get_model_complexity_info`. `input_constructor` is a function that takes the input spatial resolution as a tuple and returns a dict with named input arguments of the model. Next this dict would be passed to the model as a keyword arguments.
 - `verbose` parameter allows to get information about modules that don't contribute to the final numbers.
 - `ignore_modules` option forces `ptflops` to ignore the listed modules. This can be useful
 for research purposes. For instance, one can drop all convolutions from the counting process
 specifying `ignore_modules=[torch.nn.Conv2d]`.
 
+Requirements: Pytorch >= 1.1, torchvision >= 0.3
+
+Thanks to @warmspringwinds and Horace He for the initial version of the script.
+
 ## Install the latest version
 From PyPI:
 ```bash
 pip install ptflops
 ```
 
 From this repository:
@@ -99,50 +114,60 @@
 ```python
 import torchvision.models as models
 import torch
 from ptflops import get_model_complexity_info
 
 with torch.cuda.device(0):
   net = models.densenet161()
-  macs, params = get_model_complexity_info(net, (3, 224, 224), as_strings=True,
+  macs, params = get_model_complexity_info(net, (3, 224, 224), as_strings=True, backend='pytorch'
+                                           print_per_layer_stat=True, verbose=True)
+  print('{:<30}  {:<8}'.format('Computational complexity: ', macs))
+  print('{:<30}  {:<8}'.format('Number of parameters: ', params))
+
+  macs, params = get_model_complexity_info(net, (3, 224, 224), as_strings=True, backend='aten'
                                            print_per_layer_stat=True, verbose=True)
   print('{:<30}  {:<8}'.format('Computational complexity: ', macs))
   print('{:<30}  {:<8}'.format('Number of parameters: ', params))
 ```
 
 ## Citation
 If ptflops was useful for your paper or tech report, please cite me:
 ```
 @online{ptflops,
   author = {Vladislav Sovrasov},
   title = {ptflops: a flops counting tool for neural networks in pytorch framework},
-  year = 2018-2023,
+  year = 2018-2024,
   url = {https://github.com/sovrasov/flops-counter.pytorch},
 }
 ```
 
 ## Benchmark
 
 ### [torchvision](https://pytorch.org/vision/0.16/models.html)
 
+Model                  | Input Resolution | Params(M) | MACs(G) (`pytorch`) | MACs(G) (`aten`)
+---                    |---               |---        |---                  |---
+alexnet                | 224x224          | 61.10     | 0.72                | 0.71
+convnext_base          | 224x224          | 88.59     | 15.43               | 15.38
+densenet121            | 224x224          | 7.98      | 2.90                |
+efficientnet_b0        | 224x224          | 5.29      | 0.41                |
+efficientnet_v2_m      | 224x224          | 54.14     | 5.43                |
+googlenet              | 224x224          | 13.00     | 1.51                |
+inception_v3           | 224x224          | 27.16     | 5.75                | 5.71
+maxvit_t               | 224x224          | 30.92     | 5.48                |
+mnasnet1_0             | 224x224          | 4.38      | 0.33                |
+mobilenet_v2           | 224x224          | 3.50      | 0.32                |
+mobilenet_v3_large     | 224x224          | 5.48      | 0.23                |
+regnet_y_1_6gf         | 224x224          | 11.20     | 1.65                |
+resnet18               | 224x224          | 11.69     | 1.83                | 1.81
+resnet50               | 224x224          | 25.56     | 4.13                | 4.09
+resnext50_32x4d        | 224x224          | 25.03     | 4.29                |
+shufflenet_v2_x1_0     | 224x224          | 2.28      | 0.15                |
+squeezenet1_0          | 224x224          | 1.25      | 0.84                | 0.82
+vgg16                  | 224x224          | 138.36    | 15.52               | 15.48
+vit_b_16               | 224x224          | 86.57     | 17.61 (wrong)       | 16.86
+wide_resnet50_2        | 224x224          | 68.88     | 11.45               |
+
+
+### [timm](https://github.com/huggingface/pytorch-image-models)
+
 Model                  | Input Resolution | Params(M) | MACs(G)
----                    |---               |---        |---
-alexnet                | 224x224          | 61.10     | 0.72
-convnext_base          | 224x224          | 88.59     | 15.43
-densenet121            | 224x224          | 7.98      | 2.90
-efficientnet_b0        | 224x224          | 5.29      | 0.41
-efficientnet_v2_m      | 224x224          | 54.14     | 5.43
-googlenet              | 224x224          | 13.00     | 1.51
-inception_v3           | 224x224          | 27.16     | 2.86
-maxvit_t               | 224x224          | 30.92     | 5.48
-mnasnet1_0             | 224x224          | 4.38      | 0.33
-mobilenet_v2           | 224x224          | 3.50      | 0.32
-mobilenet_v3_large     | 224x224          | 5.48      | 0.23
-regnet_y_1_6gf         | 224x224          | 11.20     | 1.65
-resnet18               | 224x224          | 11.69     | 1.83
-resnet50               | 224x224          | 25.56     | 4.13
-resnext50_32x4d        | 224x224          | 25.03     | 4.29
-shufflenet_v2_x1_0     | 224x224          | 2.28      | 0.15
-squeezenet1_0          | 224x224          | 1.25      | 0.84
-vgg16                  | 224x224          | 138.36    | 15.52
-vit_b_16               | 224x224          | 86.57     | 17.60
-wide_resnet50_2        | 224x224          | 68.88     | 11.45
```

### Comparing `ptflops-0.7.2.2/ptflops/flops_counter.py` & `ptflops-0.7.3/ptflops/flops_counter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 '''
-Copyright (C) 2019-2023 Sovrasov V. - All Rights Reserved
+Copyright (C) 2019-2024 Sovrasov V. - All Rights Reserved
  * You may use, distribute and modify this code under the
  * terms of the MIT license.
  * You should have received a copy of the MIT license with
  * this file. If not visit https://opensource.org/licenses/MIT
 '''
 
 import sys
+from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, TextIO, Tuple, Union
 
 import torch.nn as nn
 
+from .aten_engine import get_flops_aten
 from .pytorch_engine import get_flops_pytorch
 from .utils import flops_to_string, params_to_string
 
 
+class FLOPS_BACKEND(Enum):
+    PYTORCH = 'pytorch'
+    ATEN = 'aten'
+
+
 def get_model_complexity_info(model: nn.Module,
                               input_res: Tuple[int, ...],
                               print_per_layer_stat: bool = True,
                               as_strings: bool = True,
                               input_constructor: Optional[Callable[[Tuple], Dict]] = None,
                               ost: TextIO = sys.stdout,
                               verbose: bool = False,
                               ignore_modules: List[nn.Module] = [],
                               custom_modules_hooks: Dict[nn.Module, Any] = {},
-                              backend: str = 'pytorch',
+                              backend: Union[str, FLOPS_BACKEND] = FLOPS_BACKEND.PYTORCH,
                               flops_units: Optional[str] = None,
                               param_units: Optional[str] = None,
                               output_precision: int = 2) -> Tuple[Union[str, int, None],
                                                                   Union[str, int, None]]:
     """
     Analyzes the input model and collects the amounts of parameters and MACs
     required to make a forward pass of the model.
@@ -54,14 +61,16 @@
     :type ost: TextIO
     :param verbose: Parameter to control printing of extra information and warnings.
     :type verbose: bool
     :param ignore_modules: A list of torch.nn.Module modules to ignore.
     :type ignore_modules: nn.Module
     :param custom_modules_hooks: A dict that contains custom hooks on torch modules.
     :type custom_modules_hooks: Dict[nn.Module, Any]
+    :param backend: Backend that used for evaluating model complexity.
+    :type backend: FLOPS_BACKEND
     :param flops_units: Units for string representation of MACs (GMac, MMac or KMac).
     :type flops_units: Optional[str]
     :param param_units: Units for string representation of params (M, K or B).
     :type param_units: Optional[str]
     :param output_precision: Floating point precision for representing MACs/params in
         given units.
     :type output_precision: int
@@ -71,23 +80,32 @@
             (macs, params): Nones in case of a failure during computations, or
             strings if :as_strings is true or integers otherwise.
     """
     assert type(input_res) is tuple
     assert len(input_res) >= 1
     assert isinstance(model, nn.Module)
 
-    if backend == 'pytorch':
+    if FLOPS_BACKEND(backend) == FLOPS_BACKEND.PYTORCH:
         flops_count, params_count = get_flops_pytorch(model, input_res,
                                                       print_per_layer_stat,
                                                       input_constructor, ost,
                                                       verbose, ignore_modules,
                                                       custom_modules_hooks,
                                                       output_precision=output_precision,
                                                       flops_units=flops_units,
                                                       param_units=param_units)
+    elif FLOPS_BACKEND(backend) == FLOPS_BACKEND.ATEN:
+        flops_count, params_count = get_flops_aten(model, input_res,
+                                                   print_per_layer_stat,
+                                                   input_constructor, ost,
+                                                   verbose, ignore_modules,
+                                                   custom_modules_hooks,
+                                                   output_precision=output_precision,
+                                                   flops_units=flops_units,
+                                                   param_units=param_units)
     else:
         raise ValueError('Wrong backend name')
 
     if as_strings and flops_count is not None and params_count is not None:
         flops_string = flops_to_string(
             flops_count,
             units=flops_units,
```

### Comparing `ptflops-0.7.2.2/ptflops/pytorch_engine.py` & `ptflops-0.7.3/ptflops/pytorch_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             _ = flops_model(batch)
         flops_count, params_count = flops_model.compute_average_flops_cost()
         flops_count += sum(torch_functional_flops)
         flops_count += sum(torch_tensor_ops_flops)
 
     except Exception as e:
         print("Flops estimation was not finished successfully because of"
-              f"the following exception:\n{type(e)} : {e}")
+              f" the following exception:\n{type(e)} : {e}")
         traceback.print_exc()
         reset_environment()
 
         return None, None
 
     if print_per_layer_stat:
         print_model_with_flops(
```

### Comparing `ptflops-0.7.2.2/ptflops/pytorch_ops.py` & `ptflops-0.7.3/ptflops/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `ptflops-0.7.2.2/ptflops/utils.py` & `ptflops-0.7.3/ptflops/utils.py`

 * *Files identical despite different names*

### Comparing `ptflops-0.7.2.2/ptflops.egg-info/PKG-INFO` & `ptflops-0.7.3/ptflops.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptflops
-Version: 0.7.2.2
+Version: 0.7.3
 Summary: Flops counter for neural networks in pytorch framework
 Author-email: Vladislav Sovrasov <sovrasov.vlad@gmail.com>
 Maintainer-email: Vladislav Sovrasov <sovrasov.vlad@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Vladislav Sovrasov
         
@@ -46,19 +46,34 @@
 Requires-Dist: pytest==7.1.2; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 
 # Flops counting tool for neural networks in pytorch framework
 [![Pypi version](https://img.shields.io/pypi/v/ptflops.svg)](https://pypi.org/project/ptflops/)
 [![Build Status](https://travis-ci.com/sovrasov/flops-counter.pytorch.svg?branch=master)](https://travis-ci.com/sovrasov/flops-counter.pytorch)
 
-This script is designed to compute the theoretical amount of multiply-add operations
-in convolutional neural networks. It can also compute the number of parameters and
+This tool is designed to compute the theoretical amount of multiply-add operations
+in neural networks. It can also compute the number of parameters and
 print per-layer computational cost of a given network.
 
-Supported layers:
+`ptflops` has two backends, `pytorch` and `aten`. `pytorch` backend is a legacy one, it considers `nn.Modules` only. However,
+it's still useful, since it provides a better par-layer analytics for CNNs. In all other cases it's recommended to use
+`aten` backend, which considers aten operations, and therefore it covers more model architectures (including transformers).
+
+## `aten` backend
+### Operations considered:
+- aten.mm, aten.matmul, aten.addmm, aten.bmm
+- aten.convolution
+
+### Usage tips
+- Use `verbose=True` to see the operations which were not considered during complexity computation.
+- This backend prints per-module statistics only for modules directly nested into the root `nn.Module`.
+Deeper modules at the second level of nesting are not shown in the per-layer statistics.
+
+## `pytorch` backend
+### Supported layers:
 - Conv1d/2d/3d (including grouping)
 - ConvTranspose1d/2d/3d (including grouping)
 - BatchNorm1d/2d/3d, GroupNorm, InstanceNorm1d/2d/3d, LayerNorm
 - Activations (ReLU, PReLU, ELU, ReLU6, LeakyReLU, GELU)
 - Linear
 - Upsample
 - Poolings (AvgPool1d/2d/3d, MaxPool1d/2d/3d and adaptive ones)
@@ -66,28 +81,28 @@
 Experimental support:
 - RNN, LSTM, GRU (NLH layout is assumed)
 - RNNCell, LSTMCell, GRUCell
 - torch.nn.MultiheadAttention
 - torchvision.ops.DeformConv2d
 - visual transformers from [timm](https://github.com/huggingface/pytorch-image-models)
 
-Requirements: Pytorch >= 1.1, torchvision >= 0.3
-
-Thanks to @warmspringwinds for the initial version of script.
-
-## Usage tips
+### Usage tips
 
-- This tool doesn't take into account some of the `torch.nn.functional.*` and `tensor.*` operations. Therefore unsupported operations are
+- This backend doesn't take into account some of the `torch.nn.functional.*` and `tensor.*` operations. Therefore unsupported operations are
 not contributing to the final complexity estimation. See `ptflops/pytorch_ops.py:FUNCTIONAL_MAPPING,TENSOR_OPS_MAPPING` to check supported ops.
 - `ptflops` launches a given model on a random tensor and estimates amount of computations during inference. Complicated models can have several inputs, some of them could be optional. To construct non-trivial input one can use the `input_constructor` argument of the `get_model_complexity_info`. `input_constructor` is a function that takes the input spatial resolution as a tuple and returns a dict with named input arguments of the model. Next this dict would be passed to the model as a keyword arguments.
 - `verbose` parameter allows to get information about modules that don't contribute to the final numbers.
 - `ignore_modules` option forces `ptflops` to ignore the listed modules. This can be useful
 for research purposes. For instance, one can drop all convolutions from the counting process
 specifying `ignore_modules=[torch.nn.Conv2d]`.
 
+Requirements: Pytorch >= 1.1, torchvision >= 0.3
+
+Thanks to @warmspringwinds and Horace He for the initial version of the script.
+
 ## Install the latest version
 From PyPI:
 ```bash
 pip install ptflops
 ```
 
 From this repository:
@@ -99,50 +114,60 @@
 ```python
 import torchvision.models as models
 import torch
 from ptflops import get_model_complexity_info
 
 with torch.cuda.device(0):
   net = models.densenet161()
-  macs, params = get_model_complexity_info(net, (3, 224, 224), as_strings=True,
+  macs, params = get_model_complexity_info(net, (3, 224, 224), as_strings=True, backend='pytorch'
+                                           print_per_layer_stat=True, verbose=True)
+  print('{:<30}  {:<8}'.format('Computational complexity: ', macs))
+  print('{:<30}  {:<8}'.format('Number of parameters: ', params))
+
+  macs, params = get_model_complexity_info(net, (3, 224, 224), as_strings=True, backend='aten'
                                            print_per_layer_stat=True, verbose=True)
   print('{:<30}  {:<8}'.format('Computational complexity: ', macs))
   print('{:<30}  {:<8}'.format('Number of parameters: ', params))
 ```
 
 ## Citation
 If ptflops was useful for your paper or tech report, please cite me:
 ```
 @online{ptflops,
   author = {Vladislav Sovrasov},
   title = {ptflops: a flops counting tool for neural networks in pytorch framework},
-  year = 2018-2023,
+  year = 2018-2024,
   url = {https://github.com/sovrasov/flops-counter.pytorch},
 }
 ```
 
 ## Benchmark
 
 ### [torchvision](https://pytorch.org/vision/0.16/models.html)
 
+Model                  | Input Resolution | Params(M) | MACs(G) (`pytorch`) | MACs(G) (`aten`)
+---                    |---               |---        |---                  |---
+alexnet                | 224x224          | 61.10     | 0.72                | 0.71
+convnext_base          | 224x224          | 88.59     | 15.43               | 15.38
+densenet121            | 224x224          | 7.98      | 2.90                |
+efficientnet_b0        | 224x224          | 5.29      | 0.41                |
+efficientnet_v2_m      | 224x224          | 54.14     | 5.43                |
+googlenet              | 224x224          | 13.00     | 1.51                |
+inception_v3           | 224x224          | 27.16     | 5.75                | 5.71
+maxvit_t               | 224x224          | 30.92     | 5.48                |
+mnasnet1_0             | 224x224          | 4.38      | 0.33                |
+mobilenet_v2           | 224x224          | 3.50      | 0.32                |
+mobilenet_v3_large     | 224x224          | 5.48      | 0.23                |
+regnet_y_1_6gf         | 224x224          | 11.20     | 1.65                |
+resnet18               | 224x224          | 11.69     | 1.83                | 1.81
+resnet50               | 224x224          | 25.56     | 4.13                | 4.09
+resnext50_32x4d        | 224x224          | 25.03     | 4.29                |
+shufflenet_v2_x1_0     | 224x224          | 2.28      | 0.15                |
+squeezenet1_0          | 224x224          | 1.25      | 0.84                | 0.82
+vgg16                  | 224x224          | 138.36    | 15.52               | 15.48
+vit_b_16               | 224x224          | 86.57     | 17.61 (wrong)       | 16.86
+wide_resnet50_2        | 224x224          | 68.88     | 11.45               |
+
+
+### [timm](https://github.com/huggingface/pytorch-image-models)
+
 Model                  | Input Resolution | Params(M) | MACs(G)
----                    |---               |---        |---
-alexnet                | 224x224          | 61.10     | 0.72
-convnext_base          | 224x224          | 88.59     | 15.43
-densenet121            | 224x224          | 7.98      | 2.90
-efficientnet_b0        | 224x224          | 5.29      | 0.41
-efficientnet_v2_m      | 224x224          | 54.14     | 5.43
-googlenet              | 224x224          | 13.00     | 1.51
-inception_v3           | 224x224          | 27.16     | 2.86
-maxvit_t               | 224x224          | 30.92     | 5.48
-mnasnet1_0             | 224x224          | 4.38      | 0.33
-mobilenet_v2           | 224x224          | 3.50      | 0.32
-mobilenet_v3_large     | 224x224          | 5.48      | 0.23
-regnet_y_1_6gf         | 224x224          | 11.20     | 1.65
-resnet18               | 224x224          | 11.69     | 1.83
-resnet50               | 224x224          | 25.56     | 4.13
-resnext50_32x4d        | 224x224          | 25.03     | 4.29
-shufflenet_v2_x1_0     | 224x224          | 2.28      | 0.15
-squeezenet1_0          | 224x224          | 1.25      | 0.84
-vgg16                  | 224x224          | 138.36    | 15.52
-vit_b_16               | 224x224          | 86.57     | 17.60
-wide_resnet50_2        | 224x224          | 68.88     | 11.45
```

### Comparing `ptflops-0.7.2.2/pyproject.toml` & `ptflops-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ptflops"
-version = "0.7.2.2"
+version = "0.7.3"
 dependencies = [
   "torch",
 ]
 requires-python = ">=3.7"
 authors = [
   {name = "Vladislav Sovrasov", email = "sovrasov.vlad@gmail.com"},
 ]
```


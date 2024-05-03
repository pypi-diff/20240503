# Comparing `tmp/denoising-diffusion-pytorch-1.9.6.tar.gz` & `tmp/denoising_diffusion_pytorch-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.9.6.tar", last modified: Mon Jan 22 15:11:57 2024, max compression
+gzip compressed data, was "denoising_diffusion_pytorch-2.0.0.tar", last modified: Fri May  3 16:35:25 2024, max compression
```

## Comparing `denoising-diffusion-pytorch-1.9.6.tar` & `denoising_diffusion_pytorch-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:11:57.731436 denoising-diffusion-pytorch-1.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-22 15:11:57.731436 denoising-diffusion-pytorch-1.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:11:57.727436 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)    28142 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    38313 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    30229 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    35848 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    21236 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:11:57.731436 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-22 15:11:57.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-22 15:11:57.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 15:11:57.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-22 15:11:57.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-22 15:11:57.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 15:11:57.731436 denoising-diffusion-pytorch-1.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:35:25.127220 denoising_diffusion_pytorch-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-03 16:35:25.127220 denoising_diffusion_pytorch-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:35:25.123220 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27964 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38426 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35678 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/karras_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/karras_unet_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23187 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/karras_unet_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21071 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:35:25.127220 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-03 16:35:25.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-03 16:35:25.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:35:25.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 16:35:25.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 16:35:25.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:35:25.127220 denoising_diffusion_pytorch-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.9.6/LICENSE` & `denoising_diffusion_pytorch-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.6/PKG-INFO` & `denoising_diffusion_pytorch-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.9.6
+Version: 2.0.0
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,14 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate
 Requires-Dist: einops
-Requires-Dist: ema-pytorch
+Requires-Dist: ema-pytorch>=0.4.2
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: pytorch-fid
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: tqdm
```

### Comparing `denoising-diffusion-pytorch-1.9.6/README.md` & `denoising_diffusion_pytorch-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <img src="./images/denoising-diffusion.png" width="500px"></img>
 
 ## Denoising Diffusion Probabilistic Model, in Pytorch
 
 Implementation of <a href="https://arxiv.org/abs/2006.11239">Denoising Diffusion Probabilistic Model</a> in Pytorch. It is a new approach to generative modeling that may <a href="https://ajolicoeur.wordpress.com/the-new-contender-to-gans-score-matching-with-langevin-sampling/">have the potential</a> to rival GANs. It uses denoising score matching to estimate the gradient of the data distribution, followed by Langevin sampling to sample from the true distribution.
 
-This implementation was transcribed from the official Tensorflow version <a href="https://github.com/hojonathanho/diffusion">here</a>
+This implementation was inspired by the official Tensorflow version <a href="https://github.com/hojonathanho/diffusion">here</a>
 
 Youtube AI Educators - <a href="https://www.youtube.com/watch?v=W-O7AZNzbzQ">Yannic Kilcher</a> | <a href="https://www.youtube.com/watch?v=344w5h24-h8">AI Coffeebreak with Letitia</a> | <a href="https://www.youtube.com/watch?v=HoKDTa5jHvg">Outlier</a>
 
 <a href="https://github.com/yiyixuxu/denoising-diffusion-flax">Flax implementation</a> from <a href="https://github.com/yiyixuxu">YiYi Xu</a>
 
 <a href="https://huggingface.co/blog/annotated-diffusion">Annotated code</a> by Research Scientists / Engineers from <a href="https://huggingface.co/">🤗 Huggingface</a>
 
@@ -123,21 +123,22 @@
     model,
     seq_length = 128,
     timesteps = 1000,
     objective = 'pred_v'
 )
 
 training_seq = torch.rand(64, 32, 128) # features are normalized from 0 to 1
-dataset = Dataset1D(training_seq)  # this is just an example, but you can formulate your own Dataset and pass it into the `Trainer1D` below
 
 loss = diffusion(training_seq)
 loss.backward()
 
 # Or using trainer
 
+dataset = Dataset1D(training_seq)  # this is just an example, but you can formulate your own Dataset and pass it into the `Trainer1D` below
+
 trainer = Trainer1D(
     diffusion,
     dataset = dataset,
     train_batch_size = 32,
     train_lr = 8e-5,
     train_num_steps = 700000,         # total training steps
     gradient_accumulate_every = 2,    # gradient accumulation steps
@@ -339,7 +340,18 @@
     author  = {Yelysei Bondarenko and Markus Nagel and Tijmen Blankevoort},
     journal = {ArXiv},
     year    = {2023},
     volume  = {abs/2306.12929},
     url     = {https://api.semanticscholar.org/CorpusID:259224568}
 }
 ```
+
+```bibtex
+@article{Karras2023AnalyzingAI,
+    title   = {Analyzing and Improving the Training Dynamics of Diffusion Models},
+    author  = {Tero Karras and Miika Aittala and Jaakko Lehtinen and Janne Hellsten and Timo Aila and Samuli Laine},
+    journal = {ArXiv},
+    year    = {2023},
+    volume  = {abs/2312.02696},
+    url     = {https://api.semanticscholar.org/CorpusID:265659032}
+}
+```
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 [./images/denoising-diffusion.png]## Denoising Diffusion Probabilistic Model,
 in Pytorch Implementation of _D_e_n_o_i_s_i_n_g_ _D_i_f_f_u_s_i_o_n_ _P_r_o_b_a_b_i_l_i_s_t_i_c_ _M_o_d_e_l in
 Pytorch. It is a new approach to generative modeling that may _h_a_v_e_ _t_h_e
 _p_o_t_e_n_t_i_a_l to rival GANs. It uses denoising score matching to estimate the
 gradient of the data distribution, followed by Langevin sampling to sample from
-the true distribution. This implementation was transcribed from the official
+the true distribution. This implementation was inspired by the official
 Tensorflow version _h_e_r_e Youtube AI Educators - _Y_a_n_n_i_c_ _K_i_l_c_h_e_r | _A_I_ _C_o_f_f_e_e_b_r_e_a_k
 _w_i_t_h_ _L_e_t_i_t_i_a | _O_u_t_l_i_e_r _F_l_a_x_ _i_m_p_l_e_m_e_n_t_a_t_i_o_n from _Y_i_Y_i_ _X_u _A_n_n_o_t_a_t_e_d_ _c_o_d_e by
 Research Scientists / Engineers from _ð__¤__ _H_u_g_g_i_n_g_f_a_c_e Update: Turns out none of
 the technicalities really matters at all | _"_C_o_l_d_ _D_i_f_f_u_s_i_o_n_"_ _p_a_p_e_r | _M_u_s_e [./
 images/sample.png][Image][![PyPI version](https://badge.fury.io/py/denoising-
 diffusion-pytorch.svg)](https://badge.fury.io/py/denoising-diffusion-pytorch)
 ## Install ```bash $ pip install denoising_diffusion_pytorch ``` ## Usage
@@ -36,19 +36,19 @@
 run ```python $ accelerate config ``` Then, in the same directory ```python $
 accelerate launch train.py ``` ## Miscellaneous ### 1D Sequence By popular
 request, a 1D Unet + Gaussian Diffusion implementation. ```python import torch
 from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D,
 Dataset1D model = Unet1D( dim = 64, dim_mults = (1, 2, 4, 8), channels = 32 )
 diffusion = GaussianDiffusion1D( model, seq_length = 128, timesteps = 1000,
 objective = 'pred_v' ) training_seq = torch.rand(64, 32, 128) # features are
-normalized from 0 to 1 dataset = Dataset1D(training_seq) # this is just an
-example, but you can formulate your own Dataset and pass it into the
-`Trainer1D` below loss = diffusion(training_seq) loss.backward() # Or using
-trainer trainer = Trainer1D( diffusion, dataset = dataset, train_batch_size =
-32, train_lr = 8e-5, train_num_steps = 700000, # total training steps
+normalized from 0 to 1 loss = diffusion(training_seq) loss.backward() # Or
+using trainer dataset = Dataset1D(training_seq) # this is just an example, but
+you can formulate your own Dataset and pass it into the `Trainer1D` below
+trainer = Trainer1D( diffusion, dataset = dataset, train_batch_size = 32,
+train_lr = 8e-5, train_num_steps = 700000, # total training steps
 gradient_accumulate_every = 2, # gradient accumulation steps ema_decay = 0.995,
 # exponential moving average decay amp = True, # turn on mixed precision )
 trainer.train() # after a lot of training sampled_seq = diffusion.sample
 (batch_size = 4) sampled_seq.shape # (4, 32, 128) ``` `Trainer1D` does not
 evaluate the generated samples in any way since the type of data is not known.
 You could consider adding a suitable metric to the training loop yourself after
 doing an editable install of this package `pip install -e .`. ## Citations
@@ -116,8 +116,12 @@
 Exact Attention with {IO}-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and
 Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher}, booktitle = {Advances
 in Neural Information Processing Systems}, year = {2022} } ``` ```bibtex
 @article{Bondarenko2023QuantizableTR, title = {Quantizable Transformers:
 Removing Outliers by Helping Attention Heads Do Nothing}, author = {Yelysei
 Bondarenko and Markus Nagel and Tijmen Blankevoort}, journal = {ArXiv}, year =
 {2023}, volume = {abs/2306.12929}, url = {https://api.semanticscholar.org/
-CorpusID:259224568} } ```
+CorpusID:259224568} } ``` ```bibtex @article{Karras2023AnalyzingAI, title =
+{Analyzing and Improving the Training Dynamics of Diffusion Models}, author =
+{Tero Karras and Miika Aittala and Jaakko Lehtinen and Janne Hellsten and Timo
+Aila and Samuli Laine}, journal = {ArXiv}, year = {2023}, volume = {abs/
+2312.02696}, url = {https://api.semanticscholar.org/CorpusID:265659032} } ```
```

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/__init__.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,7 +3,15 @@
 from denoising_diffusion_pytorch.learned_gaussian_diffusion import LearnedGaussianDiffusion
 from denoising_diffusion_pytorch.continuous_time_gaussian_diffusion import ContinuousTimeGaussianDiffusion
 from denoising_diffusion_pytorch.weighted_objective_gaussian_diffusion import WeightedObjectiveGaussianDiffusion
 from denoising_diffusion_pytorch.elucidated_diffusion import ElucidatedDiffusion
 from denoising_diffusion_pytorch.v_param_continuous_time_gaussian_diffusion import VParamContinuousTimeGaussianDiffusion
 
 from denoising_diffusion_pytorch.denoising_diffusion_pytorch_1d import GaussianDiffusion1D, Unet1D, Trainer1D, Dataset1D
+
+from denoising_diffusion_pytorch.karras_unet import (
+    KarrasUnet,
+    InvSqrtDecayLRSched
+)
+
+from denoising_diffusion_pytorch.karras_unet_1d import KarrasUnet1D
+from denoising_diffusion_pytorch.karras_unet_3d import KarrasUnet3D
```

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/attend.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/attend.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 AttentionConfig = namedtuple('AttentionConfig', ['enable_flash', 'enable_math', 'enable_mem_efficient'])
 
 # helpers
 
 def exists(val):
     return val is not None
 
+def default(val, d):
+    return val if exists(val) else d
+
 def once(fn):
     called = False
     @wraps(fn)
     def inner(x):
         nonlocal called
         if called:
             return
@@ -32,18 +35,20 @@
 
 # main class
 
 class Attend(nn.Module):
     def __init__(
         self,
         dropout = 0.,
-        flash = False
+        flash = False,
+        scale = None
     ):
         super().__init__()
         self.dropout = dropout
+        self.scale = scale
         self.attn_dropout = nn.Dropout(dropout)
 
         self.flash = flash
         assert not (flash and version.parse(torch.__version__) < version.parse('2.0.0')), 'in order to use flash attention, you must be using pytorch 2.0 or above'
 
         # determine efficient attention configs for cuda and cpu
 
@@ -61,14 +66,18 @@
         else:
             print_once('Non-A100 GPU detected, using math or mem efficient attention if input tensor is on cuda')
             self.cuda_config = AttentionConfig(False, True, True)
 
     def flash_attn(self, q, k, v):
         _, heads, q_len, _, k_len, is_cuda, device = *q.shape, k.shape[-2], q.is_cuda, q.device
 
+        if exists(self.scale):
+            default_scale = q.shape[-1]
+            q = q * (scale / default_scale)
+
         q, k, v = map(lambda t: t.contiguous(), (q, k, v))
 
         # Check if there is a compatible device for flash attention
 
         config = self.cuda_config if is_cuda else self.cpu_config
 
         # pytorch 2.0 flash attn: q, k, v, mask, dropout, causal, softmax_scale
@@ -91,15 +100,15 @@
         """
 
         q_len, k_len, device = q.shape[-2], k.shape[-2], q.device
 
         if self.flash:
             return self.flash_attn(q, k, v)
 
-        scale = q.shape[-1] ** -0.5
+        scale = default(self.scale, q.shape[-1] ** -0.5)
 
         # similarity
 
         sim = einsum(f"b h i d, b h j d -> b h i j", q, k) * scale
 
         # attention
```

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,41 +144,41 @@
         fouriered = torch.cat((freqs.sin(), freqs.cos()), dim = -1)
         fouriered = torch.cat((x, fouriered), dim = -1)
         return fouriered
 
 # building block modules
 
 class Block(nn.Module):
-    def __init__(self, dim, dim_out, groups = 8):
+    def __init__(self, dim, dim_out):
         super().__init__()
         self.proj = nn.Conv2d(dim, dim_out, 3, padding = 1)
-        self.norm = nn.GroupNorm(groups, dim_out)
+        self.norm = RMSNorm(dim_out)
         self.act = nn.SiLU()
 
     def forward(self, x, scale_shift = None):
         x = self.proj(x)
         x = self.norm(x)
 
         if exists(scale_shift):
             scale, shift = scale_shift
             x = x * (scale + 1) + shift
 
         x = self.act(x)
         return x
 
 class ResnetBlock(nn.Module):
-    def __init__(self, dim, dim_out, *, time_emb_dim = None, classes_emb_dim = None, groups = 8):
+    def __init__(self, dim, dim_out, *, time_emb_dim = None, classes_emb_dim = None):
         super().__init__()
         self.mlp = nn.Sequential(
             nn.SiLU(),
             nn.Linear(int(time_emb_dim) + int(classes_emb_dim), dim_out * 2)
         ) if exists(time_emb_dim) or exists(classes_emb_dim) else None
 
-        self.block1 = Block(dim, dim_out, groups = groups)
-        self.block2 = Block(dim_out, dim_out, groups = groups)
+        self.block1 = Block(dim, dim_out)
+        self.block2 = Block(dim_out, dim_out)
         self.res_conv = nn.Conv2d(dim, dim_out, 1) if dim != dim_out else nn.Identity()
 
     def forward(self, x, time_emb = None, class_emb = None):
 
         scale_shift = None
         if exists(self.mlp) and (exists(time_emb) or exists(class_emb)):
             cond_emb = tuple(filter(exists, (time_emb, class_emb)))
@@ -254,15 +254,14 @@
         dim,
         num_classes,
         cond_drop_prob = 0.5,
         init_dim = None,
         out_dim = None,
         dim_mults=(1, 2, 4, 8),
         channels = 3,
-        resnet_block_groups = 8,
         learned_variance = False,
         learned_sinusoidal_cond = False,
         random_fourier_features = False,
         learned_sinusoidal_dim = 16,
         attn_dim_head = 32,
         attn_heads = 4
     ):
@@ -279,16 +278,14 @@
 
         init_dim = default(init_dim, dim)
         self.init_conv = nn.Conv2d(input_channels, init_dim, 7, padding = 3)
 
         dims = [init_dim, *map(lambda m: dim * m, dim_mults)]
         in_out = list(zip(dims[:-1], dims[1:]))
 
-        block_klass = partial(ResnetBlock, groups = resnet_block_groups)
-
         # time embeddings
 
         time_dim = dim * 4
 
         self.random_or_learned_sinusoidal_cond = learned_sinusoidal_cond or random_fourier_features
 
         if self.random_or_learned_sinusoidal_cond:
@@ -324,39 +321,39 @@
         self.ups = nn.ModuleList([])
         num_resolutions = len(in_out)
 
         for ind, (dim_in, dim_out) in enumerate(in_out):
             is_last = ind >= (num_resolutions - 1)
 
             self.downs.append(nn.ModuleList([
-                block_klass(dim_in, dim_in, time_emb_dim = time_dim, classes_emb_dim = classes_dim),
-                block_klass(dim_in, dim_in, time_emb_dim = time_dim, classes_emb_dim = classes_dim),
+                ResnetBlock(dim_in, dim_in, time_emb_dim = time_dim, classes_emb_dim = classes_dim),
+                ResnetBlock(dim_in, dim_in, time_emb_dim = time_dim, classes_emb_dim = classes_dim),
                 Residual(PreNorm(dim_in, LinearAttention(dim_in))),
                 Downsample(dim_in, dim_out) if not is_last else nn.Conv2d(dim_in, dim_out, 3, padding = 1)
             ]))
 
         mid_dim = dims[-1]
-        self.mid_block1 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim, classes_emb_dim = classes_dim)
+        self.mid_block1 = ResnetBlock(mid_dim, mid_dim, time_emb_dim = time_dim, classes_emb_dim = classes_dim)
         self.mid_attn = Residual(PreNorm(mid_dim, Attention(mid_dim, dim_head = attn_dim_head, heads = attn_heads)))
-        self.mid_block2 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim, classes_emb_dim = classes_dim)
+        self.mid_block2 = ResnetBlock(mid_dim, mid_dim, time_emb_dim = time_dim, classes_emb_dim = classes_dim)
 
         for ind, (dim_in, dim_out) in enumerate(reversed(in_out)):
             is_last = ind == (len(in_out) - 1)
 
             self.ups.append(nn.ModuleList([
-                block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim, classes_emb_dim = classes_dim),
-                block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim, classes_emb_dim = classes_dim),
+                ResnetBlock(dim_out + dim_in, dim_out, time_emb_dim = time_dim, classes_emb_dim = classes_dim),
+                ResnetBlock(dim_out + dim_in, dim_out, time_emb_dim = time_dim, classes_emb_dim = classes_dim),
                 Residual(PreNorm(dim_out, LinearAttention(dim_out))),
                 Upsample(dim_out, dim_in) if not is_last else  nn.Conv2d(dim_out, dim_in, 3, padding = 1)
             ]))
 
         default_out_dim = channels * (1 if not learned_variance else 2)
         self.out_dim = default(out_dim, default_out_dim)
 
-        self.final_res_block = block_klass(dim * 2, dim, time_emb_dim = time_dim, classes_emb_dim = classes_dim)
+        self.final_res_block = ResnetBlock(dim * 2, dim, time_emb_dim = time_dim, classes_emb_dim = classes_dim)
         self.final_conv = nn.Conv2d(dim, self.out_dim, 1)
 
     def forward_with_cond_scale(
         self,
         *args,
         cond_scale = 1.,
         rescaled_phi = 0.,
```

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from random import random
 from functools import partial
 from collections import namedtuple
 from multiprocessing import cpu_count
 
 import torch
 from torch import nn, einsum
-from torch.cuda.amp import autocast
 import torch.nn.functional as F
+from torch.nn import Module, ModuleList
+from torch.cuda.amp import autocast
 from torch.utils.data import Dataset, DataLoader
 
 from torch.optim import Adam
 
 from torchvision import transforms as T, utils
 
 from einops import rearrange, reduce, repeat
@@ -94,40 +95,41 @@
 
 def Downsample(dim, dim_out = None):
     return nn.Sequential(
         Rearrange('b c (h p1) (w p2) -> b (c p1 p2) h w', p1 = 2, p2 = 2),
         nn.Conv2d(dim * 4, default(dim_out, dim), 1)
     )
 
-class RMSNorm(nn.Module):
+class RMSNorm(Module):
     def __init__(self, dim):
         super().__init__()
+        self.scale = dim ** 0.5
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
 
     def forward(self, x):
-        return F.normalize(x, dim = 1) * self.g * (x.shape[1] ** 0.5)
+        return F.normalize(x, dim = 1) * self.g * self.scale
 
 # sinusoidal positional embeds
 
-class SinusoidalPosEmb(nn.Module):
+class SinusoidalPosEmb(Module):
     def __init__(self, dim, theta = 10000):
         super().__init__()
         self.dim = dim
         self.theta = theta
 
     def forward(self, x):
         device = x.device
         half_dim = self.dim // 2
         emb = math.log(self.theta) / (half_dim - 1)
         emb = torch.exp(torch.arange(half_dim, device=device) * -emb)
         emb = x[:, None] * emb[None, :]
         emb = torch.cat((emb.sin(), emb.cos()), dim=-1)
         return emb
 
-class RandomOrLearnedSinusoidalPosEmb(nn.Module):
+class RandomOrLearnedSinusoidalPosEmb(Module):
     """ following @crowsonkb 's lead with random (learned optional) sinusoidal pos emb """
     """ https://github.com/crowsonkb/v-diffusion-jax/blob/master/diffusion/models/danbooru_128.py#L8 """
 
     def __init__(self, dim, is_random = False):
         super().__init__()
         assert divisible_by(dim, 2)
         half_dim = dim // 2
@@ -138,42 +140,42 @@
         freqs = x * rearrange(self.weights, 'd -> 1 d') * 2 * math.pi
         fouriered = torch.cat((freqs.sin(), freqs.cos()), dim = -1)
         fouriered = torch.cat((x, fouriered), dim = -1)
         return fouriered
 
 # building block modules
 
-class Block(nn.Module):
-    def __init__(self, dim, dim_out, groups = 8):
+class Block(Module):
+    def __init__(self, dim, dim_out):
         super().__init__()
         self.proj = nn.Conv2d(dim, dim_out, 3, padding = 1)
-        self.norm = nn.GroupNorm(groups, dim_out)
+        self.norm = RMSNorm(dim_out)
         self.act = nn.SiLU()
 
     def forward(self, x, scale_shift = None):
         x = self.proj(x)
         x = self.norm(x)
 
         if exists(scale_shift):
             scale, shift = scale_shift
             x = x * (scale + 1) + shift
 
         x = self.act(x)
         return x
 
-class ResnetBlock(nn.Module):
-    def __init__(self, dim, dim_out, *, time_emb_dim = None, groups = 8):
+class ResnetBlock(Module):
+    def __init__(self, dim, dim_out, *, time_emb_dim = None):
         super().__init__()
         self.mlp = nn.Sequential(
             nn.SiLU(),
             nn.Linear(time_emb_dim, dim_out * 2)
         ) if exists(time_emb_dim) else None
 
-        self.block1 = Block(dim, dim_out, groups = groups)
-        self.block2 = Block(dim_out, dim_out, groups = groups)
+        self.block1 = Block(dim, dim_out)
+        self.block2 = Block(dim_out, dim_out)
         self.res_conv = nn.Conv2d(dim, dim_out, 1) if dim != dim_out else nn.Identity()
 
     def forward(self, x, time_emb = None):
 
         scale_shift = None
         if exists(self.mlp) and exists(time_emb):
             time_emb = self.mlp(time_emb)
@@ -182,15 +184,15 @@
 
         h = self.block1(x, scale_shift = scale_shift)
 
         h = self.block2(h)
 
         return h + self.res_conv(x)
 
-class LinearAttention(nn.Module):
+class LinearAttention(Module):
     def __init__(
         self,
         dim,
         heads = 4,
         dim_head = 32,
         num_mem_kv = 4
     ):
@@ -227,15 +229,15 @@
 
         context = torch.einsum('b h d n, b h e n -> b h d e', k, v)
 
         out = torch.einsum('b h d e, b h d n -> b h e n', context, q)
         out = rearrange(out, 'b h c (x y) -> b (h c) x y', h = self.heads, x = h, y = w)
         return self.to_out(out)
 
-class Attention(nn.Module):
+class Attention(Module):
     def __init__(
         self,
         dim,
         heads = 4,
         dim_head = 32,
         num_mem_kv = 4,
         flash = False
@@ -265,24 +267,23 @@
         out = self.attend(q, k, v)
 
         out = rearrange(out, 'b h (x y) d -> b (h d) x y', x = h, y = w)
         return self.to_out(out)
 
 # model
 
-class Unet(nn.Module):
+class Unet(Module):
     def __init__(
         self,
         dim,
         init_dim = None,
         out_dim = None,
         dim_mults = (1, 2, 4, 8),
         channels = 3,
         self_condition = False,
-        resnet_block_groups = 8,
         learned_variance = False,
         learned_sinusoidal_cond = False,
         random_fourier_features = False,
         learned_sinusoidal_dim = 16,
         sinusoidal_pos_emb_theta = 10000,
         attn_dim_head = 32,
         attn_heads = 4,
@@ -299,16 +300,14 @@
 
         init_dim = default(init_dim, dim)
         self.init_conv = nn.Conv2d(input_channels, init_dim, 7, padding = 3)
 
         dims = [init_dim, *map(lambda m: dim * m, dim_mults)]
         in_out = list(zip(dims[:-1], dims[1:]))
 
-        block_klass = partial(ResnetBlock, groups = resnet_block_groups)
-
         # time embeddings
 
         time_dim = dim * 4
 
         self.random_or_learned_sinusoidal_cond = learned_sinusoidal_cond or random_fourier_features
 
         if self.random_or_learned_sinusoidal_cond:
@@ -337,51 +336,51 @@
 
         assert len(full_attn) == len(dim_mults)
 
         FullAttention = partial(Attention, flash = flash_attn)
 
         # layers
 
-        self.downs = nn.ModuleList([])
-        self.ups = nn.ModuleList([])
+        self.downs = ModuleList([])
+        self.ups = ModuleList([])
         num_resolutions = len(in_out)
 
         for ind, ((dim_in, dim_out), layer_full_attn, layer_attn_heads, layer_attn_dim_head) in enumerate(zip(in_out, full_attn, attn_heads, attn_dim_head)):
             is_last = ind >= (num_resolutions - 1)
 
             attn_klass = FullAttention if layer_full_attn else LinearAttention
 
-            self.downs.append(nn.ModuleList([
-                block_klass(dim_in, dim_in, time_emb_dim = time_dim),
-                block_klass(dim_in, dim_in, time_emb_dim = time_dim),
+            self.downs.append(ModuleList([
+                ResnetBlock(dim_in, dim_in, time_emb_dim = time_dim),
+                ResnetBlock(dim_in, dim_in, time_emb_dim = time_dim),
                 attn_klass(dim_in, dim_head = layer_attn_dim_head, heads = layer_attn_heads),
                 Downsample(dim_in, dim_out) if not is_last else nn.Conv2d(dim_in, dim_out, 3, padding = 1)
             ]))
 
         mid_dim = dims[-1]
-        self.mid_block1 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
+        self.mid_block1 = ResnetBlock(mid_dim, mid_dim, time_emb_dim = time_dim)
         self.mid_attn = FullAttention(mid_dim, heads = attn_heads[-1], dim_head = attn_dim_head[-1])
-        self.mid_block2 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
+        self.mid_block2 = ResnetBlock(mid_dim, mid_dim, time_emb_dim = time_dim)
 
         for ind, ((dim_in, dim_out), layer_full_attn, layer_attn_heads, layer_attn_dim_head) in enumerate(zip(*map(reversed, (in_out, full_attn, attn_heads, attn_dim_head)))):
             is_last = ind == (len(in_out) - 1)
 
             attn_klass = FullAttention if layer_full_attn else LinearAttention
 
-            self.ups.append(nn.ModuleList([
-                block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
-                block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
+            self.ups.append(ModuleList([
+                ResnetBlock(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
+                ResnetBlock(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
                 attn_klass(dim_out, dim_head = layer_attn_dim_head, heads = layer_attn_heads),
                 Upsample(dim_out, dim_in) if not is_last else  nn.Conv2d(dim_out, dim_in, 3, padding = 1)
             ]))
 
         default_out_dim = channels * (1 if not learned_variance else 2)
         self.out_dim = default(out_dim, default_out_dim)
 
-        self.final_res_block = block_klass(dim * 2, dim, time_emb_dim = time_dim)
+        self.final_res_block = ResnetBlock(dim * 2, dim, time_emb_dim = time_dim)
         self.final_conv = nn.Conv2d(dim, self.out_dim, 1)
 
     @property
     def downsample_factor(self):
         return 2 ** (len(self.downs) - 1)
 
     def forward(self, x, time, x_self_cond = None):
@@ -466,15 +465,15 @@
     v_start = torch.tensor(start / tau).sigmoid()
     v_end = torch.tensor(end / tau).sigmoid()
     alphas_cumprod = (-((t * (end - start) + start) / tau).sigmoid() + v_end) / (v_end - v_start)
     alphas_cumprod = alphas_cumprod / alphas_cumprod[0]
     betas = 1 - (alphas_cumprod[1:] / alphas_cumprod[:-1])
     return torch.clip(betas, 0, 0.999)
 
-class GaussianDiffusion(nn.Module):
+class GaussianDiffusion(Module):
     def __init__(
         self,
         model,
         *,
         image_size,
         timesteps = 1000,
         sampling_timesteps = None,
@@ -485,21 +484,24 @@
         auto_normalize = True,
         offset_noise_strength = 0.,  # https://www.crosslabs.org/blog/diffusion-with-offset-noise
         min_snr_loss_weight = False, # https://arxiv.org/abs/2303.09556
         min_snr_gamma = 5
     ):
         super().__init__()
         assert not (type(self) == GaussianDiffusion and model.channels != model.out_dim)
-        assert not model.random_or_learned_sinusoidal_cond
+        assert not hasattr(model, 'random_or_learned_sinusoidal_cond') or not model.random_or_learned_sinusoidal_cond
 
         self.model = model
 
         self.channels = self.model.channels
         self.self_condition = self.model.self_condition
 
+        if isinstance(image_size, int):
+            image_size = (image_size, image_size)
+        assert isinstance(image_size, (tuple, list)) and len(image_size) == 2, 'image size must be a integer or a tuple/list of two integers'
         self.image_size = image_size
 
         self.objective = objective
 
         assert objective in {'pred_noise', 'pred_x0', 'pred_v'}, 'objective must be either pred_noise (predict noise) or pred_x0 (predict image start) or pred_v (predict v [v-parameterization as defined in appendix D of progressive distillation paper, used in imagen-video successfully])'
 
         if beta_schedule == 'linear':
@@ -725,17 +727,17 @@
         ret = img if not return_all_timesteps else torch.stack(imgs, dim = 1)
 
         ret = self.unnormalize(ret)
         return ret
 
     @torch.inference_mode()
     def sample(self, batch_size = 16, return_all_timesteps = False):
-        image_size, channels = self.image_size, self.channels
+        (h, w), channels = self.image_size, self.channels
         sample_fn = self.p_sample_loop if not self.is_ddim_sampling else self.ddim_sample
-        return sample_fn((batch_size, channels, image_size, image_size), return_all_timesteps = return_all_timesteps)
+        return sample_fn((batch_size, channels, h, w), return_all_timesteps = return_all_timesteps)
 
     @torch.inference_mode()
     def interpolate(self, x1, x2, t = None, lam = 0.5):
         b, *_, device = *x1.shape, x1.device
         t = default(t, self.num_timesteps - 1)
 
         assert x1.shape == x2.shape
@@ -807,15 +809,15 @@
         loss = reduce(loss, 'b ... -> b', 'mean')
 
         loss = loss * extract(self.loss_weight, t, loss.shape)
         return loss.mean()
 
     def forward(self, img, *args, **kwargs):
         b, c, h, w, device, img_size, = *img.shape, img.device, self.image_size
-        assert h == img_size and w == img_size, f'height and width of image must be {img_size}'
+        assert h == img_size[0] and w == img_size[1], f'height and width of image must be {img_size}'
         t = torch.randint(0, self.num_timesteps, (b,), device=device).long()
 
         img = self.normalize(img)
         return self.p_losses(img, t, *args, **kwargs)
 
 # dataset classes
 
@@ -849,15 +851,15 @@
     def __getitem__(self, index):
         path = self.paths[index]
         img = Image.open(path)
         return self.transform(img)
 
 # trainer class
 
-class Trainer(object):
+class Trainer:
     def __init__(
         self,
         diffusion_model,
         folder,
         *,
         train_batch_size = 16,
         gradient_accumulate_every = 1,
```

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,41 +151,41 @@
         fouriered = torch.cat((freqs.sin(), freqs.cos()), dim = -1)
         fouriered = torch.cat((x, fouriered), dim = -1)
         return fouriered
 
 # building block modules
 
 class Block(nn.Module):
-    def __init__(self, dim, dim_out, groups = 8):
+    def __init__(self, dim, dim_out):
         super().__init__()
         self.proj = nn.Conv1d(dim, dim_out, 3, padding = 1)
-        self.norm = nn.GroupNorm(groups, dim_out)
+        self.norm = RMSNorm(dim_out)
         self.act = nn.SiLU()
 
     def forward(self, x, scale_shift = None):
         x = self.proj(x)
         x = self.norm(x)
 
         if exists(scale_shift):
             scale, shift = scale_shift
             x = x * (scale + 1) + shift
 
         x = self.act(x)
         return x
 
 class ResnetBlock(nn.Module):
-    def __init__(self, dim, dim_out, *, time_emb_dim = None, groups = 8):
+    def __init__(self, dim, dim_out, *, time_emb_dim = None):
         super().__init__()
         self.mlp = nn.Sequential(
             nn.SiLU(),
             nn.Linear(time_emb_dim, dim_out * 2)
         ) if exists(time_emb_dim) else None
 
-        self.block1 = Block(dim, dim_out, groups = groups)
-        self.block2 = Block(dim_out, dim_out, groups = groups)
+        self.block1 = Block(dim, dim_out)
+        self.block2 = Block(dim_out, dim_out)
         self.res_conv = nn.Conv1d(dim, dim_out, 1) if dim != dim_out else nn.Identity()
 
     def forward(self, x, time_emb = None):
 
         scale_shift = None
         if exists(self.mlp) and exists(time_emb):
             time_emb = self.mlp(time_emb)
@@ -258,15 +258,14 @@
         self,
         dim,
         init_dim = None,
         out_dim = None,
         dim_mults=(1, 2, 4, 8),
         channels = 3,
         self_condition = False,
-        resnet_block_groups = 8,
         learned_variance = False,
         learned_sinusoidal_cond = False,
         random_fourier_features = False,
         learned_sinusoidal_dim = 16,
         sinusoidal_pos_emb_theta = 10000,
         attn_dim_head = 32,
         attn_heads = 4
@@ -281,16 +280,14 @@
 
         init_dim = default(init_dim, dim)
         self.init_conv = nn.Conv1d(input_channels, init_dim, 7, padding = 3)
 
         dims = [init_dim, *map(lambda m: dim * m, dim_mults)]
         in_out = list(zip(dims[:-1], dims[1:]))
 
-        block_klass = partial(ResnetBlock, groups = resnet_block_groups)
-
         # time embeddings
 
         time_dim = dim * 4
 
         self.random_or_learned_sinusoidal_cond = learned_sinusoidal_cond or random_fourier_features
 
         if self.random_or_learned_sinusoidal_cond:
@@ -313,39 +310,39 @@
         self.ups = nn.ModuleList([])
         num_resolutions = len(in_out)
 
         for ind, (dim_in, dim_out) in enumerate(in_out):
             is_last = ind >= (num_resolutions - 1)
 
             self.downs.append(nn.ModuleList([
-                block_klass(dim_in, dim_in, time_emb_dim = time_dim),
-                block_klass(dim_in, dim_in, time_emb_dim = time_dim),
+                ResnetBlock(dim_in, dim_in, time_emb_dim = time_dim),
+                ResnetBlock(dim_in, dim_in, time_emb_dim = time_dim),
                 Residual(PreNorm(dim_in, LinearAttention(dim_in))),
                 Downsample(dim_in, dim_out) if not is_last else nn.Conv1d(dim_in, dim_out, 3, padding = 1)
             ]))
 
         mid_dim = dims[-1]
-        self.mid_block1 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
+        self.mid_block1 = ResnetBlock(mid_dim, mid_dim, time_emb_dim = time_dim)
         self.mid_attn = Residual(PreNorm(mid_dim, Attention(mid_dim, dim_head = attn_dim_head, heads = attn_heads)))
-        self.mid_block2 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
+        self.mid_block2 = ResnetBlock(mid_dim, mid_dim, time_emb_dim = time_dim)
 
         for ind, (dim_in, dim_out) in enumerate(reversed(in_out)):
             is_last = ind == (len(in_out) - 1)
 
             self.ups.append(nn.ModuleList([
-                block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
-                block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
+                ResnetBlock(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
+                ResnetBlock(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
                 Residual(PreNorm(dim_out, LinearAttention(dim_out))),
                 Upsample(dim_out, dim_in) if not is_last else  nn.Conv1d(dim_out, dim_in, 3, padding = 1)
             ]))
 
         default_out_dim = channels * (1 if not learned_variance else 2)
         self.out_dim = default(out_dim, default_out_dim)
 
-        self.final_res_block = block_klass(dim * 2, dim, time_emb_dim = time_dim)
+        self.final_res_block = ResnetBlock(dim * 2, dim, time_emb_dim = time_dim)
         self.final_conv = nn.Conv1d(dim, self.out_dim, 1)
 
     def forward(self, x, time, x_self_cond = None):
         if self.self_condition:
             x_self_cond = default(x_self_cond, lambda: torch.zeros_like(x))
             x = torch.cat((x_self_cond, x), dim = 1)
```

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,41 +144,41 @@
         fouriered = torch.cat((freqs.sin(), freqs.cos()), dim = -1)
         fouriered = torch.cat((x, fouriered), dim = -1)
         return fouriered
 
 # building block modules
 
 class Block(nn.Module):
-    def __init__(self, dim, dim_out, groups = 8):
+    def __init__(self, dim, dim_out):
         super().__init__()
         self.proj = nn.Conv2d(dim, dim_out, 3, padding = 1)
-        self.norm = nn.GroupNorm(groups, dim_out)
+        self.norm = RMSNorm(groups, dim_out)
         self.act = nn.SiLU()
 
     def forward(self, x, scale_shift = None):
         x = self.proj(x)
         x = self.norm(x)
 
         if exists(scale_shift):
             scale, shift = scale_shift
             x = x * (scale + 1) + shift
 
         x = self.act(x)
         return x
 
 class ResnetBlock(nn.Module):
-    def __init__(self, dim, dim_out, *, time_emb_dim = None, groups = 8):
+    def __init__(self, dim, dim_out, *, time_emb_dim = None):
         super().__init__()
         self.mlp = nn.Sequential(
             nn.SiLU(),
             nn.Linear(time_emb_dim, dim_out * 2)
         ) if exists(time_emb_dim) else None
 
-        self.block1 = Block(dim, dim_out, groups = groups)
-        self.block2 = Block(dim_out, dim_out, groups = groups)
+        self.block1 = Block(dim, dim_out)
+        self.block2 = Block(dim_out, dim_out)
         self.res_conv = nn.Conv2d(dim, dim_out, 1) if dim != dim_out else nn.Identity()
 
     def forward(self, x, time_emb = None):
 
         scale_shift = None
         if exists(self.mlp) and exists(time_emb):
             time_emb = self.mlp(time_emb)
@@ -251,15 +251,14 @@
         self,
         dim,
         init_dim = None,
         out_dim = None,
         dim_mults=(1, 2, 4, 8),
         channels = 3,
         self_condition = False,
-        resnet_block_groups = 8,
         learned_variance = False,
         learned_sinusoidal_cond = False,
         random_fourier_features = False,
         learned_sinusoidal_dim = 16
     ):
         super().__init__()
 
@@ -271,16 +270,14 @@
 
         init_dim = default(init_dim, dim)
         self.init_conv = nn.Conv2d(input_channels, init_dim, 7, padding = 3)
 
         dims = [init_dim, *map(lambda m: dim * m, dim_mults)]
         in_out = list(zip(dims[:-1], dims[1:]))
 
-        block_klass = partial(ResnetBlock, groups = resnet_block_groups)
-
         # time embeddings
 
         time_dim = dim * 4
 
         self.random_or_learned_sinusoidal_cond = learned_sinusoidal_cond or random_fourier_features
 
         if self.random_or_learned_sinusoidal_cond:
@@ -303,39 +300,39 @@
         self.ups = nn.ModuleList([])
         num_resolutions = len(in_out)
 
         for ind, (dim_in, dim_out) in enumerate(in_out):
             is_last = ind >= (num_resolutions - 1)
 
             self.downs.append(nn.ModuleList([
-                block_klass(dim_in, dim_in, time_emb_dim = time_dim),
-                block_klass(dim_in, dim_in, time_emb_dim = time_dim),
+                ResnetBlock(dim_in, dim_in, time_emb_dim = time_dim),
+                ResnetBlock(dim_in, dim_in, time_emb_dim = time_dim),
                 Residual(PreNorm(dim_in, LinearAttention(dim_in))),
                 Downsample(dim_in, dim_out) if not is_last else nn.Conv2d(dim_in, dim_out, 3, padding = 1)
             ]))
 
         mid_dim = dims[-1]
-        self.mid_block1 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
+        self.mid_block1 = ResnetBlock(mid_dim, mid_dim, time_emb_dim = time_dim)
         self.mid_attn = Residual(PreNorm(mid_dim, Attention(mid_dim)))
-        self.mid_block2 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
+        self.mid_block2 = ResnetBlock(mid_dim, mid_dim, time_emb_dim = time_dim)
 
         for ind, (dim_in, dim_out) in enumerate(reversed(in_out)):
             is_last = ind == (len(in_out) - 1)
 
             self.ups.append(nn.ModuleList([
-                block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
-                block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
+                ResnetBlock(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
+                ResnetBlock(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
                 Residual(PreNorm(dim_out, LinearAttention(dim_out))),
                 Upsample(dim_out, dim_in) if not is_last else  nn.Conv2d(dim_out, dim_in, 3, padding = 1)
             ]))
 
         default_out_dim = channels * (1 if not learned_variance else 2)
         self.out_dim = default(out_dim, default_out_dim)
 
-        self.final_res_block = block_klass(dim * 2, dim, time_emb_dim = time_dim)
+        self.final_res_block = ResnetBlock(dim * 2, dim, time_emb_dim = time_dim)
         self.final_conv = nn.Conv2d(dim, self.out_dim, 1)
 
     def forward(self, x, time, x_self_cond = None):
         if self.self_condition:
             x_self_cond = default(x_self_cond, lambda: torch.zeros_like(x))
             x = torch.cat((x_self_cond, x), dim = 1)
```

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     ):
         super().__init__(model, *args, **kwargs)
         assert model.out_dim == (model.channels * 2), 'dimension out of unet must be twice the number of channels for learned variance - you can also set the `learned_variance` keyword argument on the Unet to be `True`'
         assert not model.self_condition, 'not supported yet'
 
         self.vb_loss_weight = vb_loss_weight
 
-    def model_predictions(self, x, t, clip_x_start = False):
+    def model_predictions(self, x, t, x_self_cond = None, clip_x_start = False, rederive_pred_noise = False):
         model_output = self.model(x, t)
         model_output, pred_variance = model_output.chunk(2, dim = 1)
 
         maybe_clip = partial(torch.clamp, min = -1., max = 1.) if clip_x_start else identity
 
         if self.objective == 'pred_noise':
             pred_noise = model_output
```

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,41 +112,41 @@
         fouriered = torch.cat((freqs.sin(), freqs.cos()), dim = -1)
         fouriered = torch.cat((x, fouriered), dim = -1)
         return fouriered
 
 # building block modules
 
 class Block(nn.Module):
-    def __init__(self, dim, dim_out, groups = 8):
+    def __init__(self, dim, dim_out):
         super().__init__()
         self.proj = nn.Conv2d(dim, dim_out, 3, padding = 1)
-        self.norm = nn.GroupNorm(groups, dim_out)
+        self.norm = RMSNorm(dim_out, normalize_dim = 1)
         self.act = nn.SiLU()
 
     def forward(self, x, scale_shift = None):
         x = self.proj(x)
         x = self.norm(x)
 
         if exists(scale_shift):
             scale, shift = scale_shift
             x = x * (scale + 1) + shift
 
         x = self.act(x)
         return x
 
 class ResnetBlock(nn.Module):
-    def __init__(self, dim, dim_out, *, time_emb_dim = None, groups = 8):
+    def __init__(self, dim, dim_out, *, time_emb_dim = None):
         super().__init__()
         self.mlp = nn.Sequential(
             nn.SiLU(),
             nn.Linear(time_emb_dim, dim_out * 2)
         ) if exists(time_emb_dim) else None
 
-        self.block1 = Block(dim, dim_out, groups = groups)
-        self.block2 = Block(dim_out, dim_out, groups = groups)
+        self.block1 = Block(dim, dim_out)
+        self.block2 = Block(dim_out, dim_out)
         self.res_conv = nn.Conv2d(dim, dim_out, 1) if dim != dim_out else nn.Identity()
 
     def forward(self, x, time_emb = None):
 
         scale_shift = None
         if exists(self.mlp) and exists(time_emb):
             time_emb = self.mlp(time_emb)
@@ -315,15 +315,14 @@
         downsample_factor = 2,
         channels = 3,
         vit_depth = 6,
         vit_dropout = 0.2,
         attn_dim_head = 32,
         attn_heads = 4,
         ff_mult = 4,
-        resnet_block_groups = 8,
         learned_sinusoidal_dim = 16,
         init_img_transform: callable = None,
         final_img_itransform: callable = None,
         patch_size = 1,
         dual_patchnorm = False
     ):
         super().__init__()
@@ -365,16 +364,14 @@
             self.unpatchify = nn.ConvTranspose2d(input_channels, channels, patch_size, stride = patch_size)
 
         # determine dimensions
 
         dims = [init_dim, *map(lambda m: dim * m, dim_mults)]
         in_out = list(zip(dims[:-1], dims[1:]))
 
-        resnet_block = partial(ResnetBlock, groups = resnet_block_groups)
-
         # time embeddings
 
         time_dim = dim * 4
 
         sinu_pos_emb = LearnedSinusoidalPosEmb(learned_sinusoidal_dim)
         fourier_dim = learned_sinusoidal_dim + 1
 
@@ -396,16 +393,16 @@
         self.ups = nn.ModuleList([])
         num_resolutions = len(in_out)
 
         for ind, ((dim_in, dim_out), factor) in enumerate(zip(in_out, downsample_factor)):
             is_last = ind >= (num_resolutions - 1)
 
             self.downs.append(nn.ModuleList([
-                resnet_block(dim_in, dim_in, time_emb_dim = time_dim),
-                resnet_block(dim_in, dim_in, time_emb_dim = time_dim),
+                ResnetBlock(dim_in, dim_in, time_emb_dim = time_dim),
+                ResnetBlock(dim_in, dim_in, time_emb_dim = time_dim),
                 LinearAttention(dim_in),
                 Downsample(dim_in, dim_out, factor = factor)
             ]))
 
         mid_dim = dims[-1]
 
         self.vit = Transformer(
@@ -419,23 +416,23 @@
         )
 
         for ind, ((dim_in, dim_out), factor) in enumerate(zip(reversed(in_out), reversed(downsample_factor))):
             is_last = ind == (len(in_out) - 1)
 
             self.ups.append(nn.ModuleList([
                 Upsample(dim_out, dim_in, factor = factor),
-                resnet_block(dim_in * 2, dim_in, time_emb_dim = time_dim),
-                resnet_block(dim_in * 2, dim_in, time_emb_dim = time_dim),
+                ResnetBlock(dim_in * 2, dim_in, time_emb_dim = time_dim),
+                ResnetBlock(dim_in * 2, dim_in, time_emb_dim = time_dim),
                 LinearAttention(dim_in),
             ]))
 
         default_out_dim = input_channels
         self.out_dim = default(out_dim, default_out_dim)
 
-        self.final_res_block = resnet_block(dim * 2, dim, time_emb_dim = time_dim)
+        self.final_res_block = ResnetBlock(dim * 2, dim, time_emb_dim = time_dim)
         self.final_conv = nn.Conv2d(dim, self.out_dim, 1)
 
     def forward(self, x, time):
         x = self.init_img_transform(x)
 
         x = self.init_conv(x)
         r = x.clone()
```

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.9.6
+Version: 2.0.0
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,14 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate
 Requires-Dist: einops
-Requires-Dist: ema-pytorch
+Requires-Dist: ema-pytorch>=0.4.2
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: pytorch-fid
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: tqdm
```

### Comparing `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 denoising_diffusion_pytorch/classifier_free_guidance.py
 denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
 denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
 denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
 denoising_diffusion_pytorch/elucidated_diffusion.py
 denoising_diffusion_pytorch/fid_evaluation.py
 denoising_diffusion_pytorch/guided_diffusion.py
+denoising_diffusion_pytorch/karras_unet.py
+denoising_diffusion_pytorch/karras_unet_1d.py
+denoising_diffusion_pytorch/karras_unet_3d.py
 denoising_diffusion_pytorch/learned_gaussian_diffusion.py
 denoising_diffusion_pytorch/simple_diffusion.py
 denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
 denoising_diffusion_pytorch/version.py
 denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
 denoising_diffusion_pytorch.egg-info/PKG-INFO
 denoising_diffusion_pytorch.egg-info/SOURCES.txt
```

### Comparing `denoising-diffusion-pytorch-1.9.6/setup.py` & `denoising_diffusion_pytorch-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   keywords = [
     'artificial intelligence',
     'generative models'
   ],
   install_requires=[
     'accelerate',
     'einops',
-    'ema-pytorch',
+    'ema-pytorch>=0.4.2',
     'numpy',
     'pillow',
     'pytorch-fid',
     'torch',
     'torchvision',
     'tqdm'
   ],
```


# Comparing `tmp/hqq-0.1.7.tar.gz` & `tmp/hqq-0.1.7.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hqq-0.1.7.tar", last modified: Wed Apr 24 08:56:07 2024, max compression
+gzip compressed data, was "hqq-0.1.7.post1.tar", last modified: Fri May  3 14:45:11 2024, max compression
```

## Comparing `hqq-0.1.7.tar` & `hqq-0.1.7.post1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.294434 hqq-0.1.7/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11360 2023-12-02 17:25:57.000000 hqq-0.1.7/LICENSE
--rw-r--r--   0 hicham    (1009) hicham    (1009)      432 2024-04-24 08:56:07.294434 hqq-0.1.7/PKG-INFO
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.270433 hqq-0.1.7/hqq/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)       87 2024-04-16 08:24:14.000000 hqq-0.1.7/hqq/__init__.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.270433 hqq-0.1.7/hqq/backends/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2024-04-16 10:04:12.000000 hqq-0.1.7/hqq/backends/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3228 2024-04-19 12:02:43.000000 hqq-0.1.7/hqq/backends/marlin.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    10514 2024-04-24 08:49:06.000000 hqq-0.1.7/hqq/backends/torchao.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.274433 hqq-0.1.7/hqq/core/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:22.000000 hqq-0.1.7/hqq/core/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5195 2024-04-10 14:29:15.000000 hqq-0.1.7/hqq/core/bitpack.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    14118 2024-04-16 18:00:28.000000 hqq-0.1.7/hqq/core/optimize.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17172 2024-03-18 15:34:02.000000 hqq-0.1.7/hqq/core/peft.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    28563 2024-04-16 17:51:09.000000 hqq-0.1.7/hqq/core/quantize.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      639 2024-03-15 08:58:01.000000 hqq-0.1.7/hqq/core/utils.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.278433 hqq-0.1.7/hqq/engine/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7/hqq/engine/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3131 2024-03-25 11:05:14.000000 hqq-0.1.7/hqq/engine/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2568 2024-03-15 09:12:21.000000 hqq-0.1.7/hqq/engine/hf.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2458 2024-03-15 09:09:35.000000 hqq-0.1.7/hqq/engine/timm.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5287 2024-03-15 12:03:22.000000 hqq-0.1.7/hqq/engine/vllm.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.278433 hqq-0.1.7/hqq/kernels/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)       87 2024-03-15 10:04:14.000000 hqq-0.1.7/hqq/kernels/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2670 2024-03-25 10:15:39.000000 hqq-0.1.7/hqq/kernels/hqq_aten_cuda.cpp
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17933 2024-04-08 11:30:33.000000 hqq-0.1.7/hqq/kernels/hqq_aten_cuda_kernel.cu
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3412 2024-02-21 11:27:07.000000 hqq-0.1.7/hqq/kernels/hqq_aten_torch.cpp
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      494 2024-03-19 10:48:06.000000 hqq-0.1.7/hqq/kernels/setup_cuda.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      292 2024-03-14 16:26:18.000000 hqq-0.1.7/hqq/kernels/setup_torch.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.278433 hqq-0.1.7/hqq/models/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:32.000000 hqq-0.1.7/hqq/models/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17314 2024-04-22 18:40:37.000000 hqq-0.1.7/hqq/models/base.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.282434 hqq-0.1.7/hqq/models/hf/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7/hqq/models/hf/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1057 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/llama.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/mistral.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3464 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/mixtral.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2487 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/phi.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2361 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/phi_opt.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.282434 hqq-0.1.7/hqq/models/timm/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7/hqq/models/timm/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      750 2024-03-14 15:52:37.000000 hqq-0.1.7/hqq/models/timm/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2815 2024-03-14 15:53:15.000000 hqq-0.1.7/hqq/models/timm/vit_clip.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.290434 hqq-0.1.7/hqq/models/vllm/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7/hqq/models/vllm/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6114 2024-03-15 12:07:03.000000 hqq-0.1.7/hqq/models/vllm/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    16480 2024-03-14 15:55:27.000000 hqq-0.1.7/hqq/models/vllm/llama.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.290434 hqq-0.1.7/hqq/utils/
--rw-rw-r--   0 hicham    (1009) hicham    (1009)        0 2024-04-16 10:04:22.000000 hqq-0.1.7/hqq/utils/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    10844 2024-04-23 16:50:10.000000 hqq-0.1.7/hqq/utils/generation_hf.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6066 2024-04-22 17:00:27.000000 hqq-0.1.7/hqq/utils/patching.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.270433 hqq-0.1.7/hqq.egg-info/
--rw-r--r--   0 hicham    (1009) hicham    (1009)      432 2024-04-24 08:54:01.000000 hqq-0.1.7/hqq.egg-info/PKG-INFO
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1109 2024-04-24 08:54:01.000000 hqq-0.1.7/hqq.egg-info/SOURCES.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        1 2024-04-24 08:54:01.000000 hqq-0.1.7/hqq.egg-info/dependency_links.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)       92 2024-04-24 08:54:01.000000 hqq-0.1.7/hqq.egg-info/requires.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        4 2024-04-24 08:54:01.000000 hqq-0.1.7/hqq.egg-info/top_level.txt
--rw-rw-r--   0 hicham    (1009) hicham    (1009)       38 2024-04-24 08:56:07.294434 hqq-0.1.7/setup.cfg
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1700 2024-04-16 09:50:06.000000 hqq-0.1.7/setup.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.290434 hqq-0.1.7/tests/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3689 2024-03-25 10:44:50.000000 hqq-0.1.7/tests/test_bitpack.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11302 2024-03-01 10:40:44.000000 hqq-0.1.7/tests/test_quantize.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.800661 hqq-0.1.7.post1/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11360 2023-12-02 17:25:57.000000 hqq-0.1.7.post1/LICENSE
+-rw-r--r--   0 hicham    (1009) hicham    (1009)      438 2024-05-03 14:45:11.800661 hqq-0.1.7.post1/PKG-INFO
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.784661 hqq-0.1.7.post1/hqq/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)       93 2024-05-03 14:43:06.000000 hqq-0.1.7.post1/hqq/__init__.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.788661 hqq-0.1.7.post1/hqq/backends/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2024-04-16 10:04:12.000000 hqq-0.1.7.post1/hqq/backends/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3228 2024-04-19 12:02:43.000000 hqq-0.1.7.post1/hqq/backends/marlin.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    10514 2024-04-24 08:49:06.000000 hqq-0.1.7.post1/hqq/backends/torchao.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.788661 hqq-0.1.7.post1/hqq/core/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:22.000000 hqq-0.1.7.post1/hqq/core/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5195 2024-05-03 14:37:22.000000 hqq-0.1.7.post1/hqq/core/bitpack.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    14369 2024-05-03 14:37:54.000000 hqq-0.1.7.post1/hqq/core/optimize.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17172 2024-03-18 15:34:02.000000 hqq-0.1.7.post1/hqq/core/peft.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    28600 2024-05-03 14:41:05.000000 hqq-0.1.7.post1/hqq/core/quantize.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      670 2024-05-03 14:37:54.000000 hqq-0.1.7.post1/hqq/core/utils.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.792661 hqq-0.1.7.post1/hqq/engine/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post1/hqq/engine/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3131 2024-03-25 11:05:14.000000 hqq-0.1.7.post1/hqq/engine/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2568 2024-03-15 09:12:21.000000 hqq-0.1.7.post1/hqq/engine/hf.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2458 2024-03-15 09:09:35.000000 hqq-0.1.7.post1/hqq/engine/timm.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5287 2024-03-15 12:03:22.000000 hqq-0.1.7.post1/hqq/engine/vllm.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.792661 hqq-0.1.7.post1/hqq/kernels/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)       87 2024-03-15 10:04:14.000000 hqq-0.1.7.post1/hqq/kernels/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2670 2024-03-25 10:15:39.000000 hqq-0.1.7.post1/hqq/kernels/hqq_aten_cuda.cpp
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17933 2024-04-08 11:30:33.000000 hqq-0.1.7.post1/hqq/kernels/hqq_aten_cuda_kernel.cu
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3412 2024-02-21 11:27:07.000000 hqq-0.1.7.post1/hqq/kernels/hqq_aten_torch.cpp
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      494 2024-03-19 10:48:06.000000 hqq-0.1.7.post1/hqq/kernels/setup_cuda.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      292 2024-03-14 16:26:18.000000 hqq-0.1.7.post1/hqq/kernels/setup_torch.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.792661 hqq-0.1.7.post1/hqq/models/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:32.000000 hqq-0.1.7.post1/hqq/models/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17314 2024-04-22 18:40:37.000000 hqq-0.1.7.post1/hqq/models/base.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.796661 hqq-0.1.7.post1/hqq/models/hf/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post1/hqq/models/hf/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1057 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/llama.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/mistral.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3464 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/mixtral.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2487 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/phi.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2361 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/phi_opt.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.796661 hqq-0.1.7.post1/hqq/models/timm/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post1/hqq/models/timm/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      750 2024-03-14 15:52:37.000000 hqq-0.1.7.post1/hqq/models/timm/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2815 2024-03-14 15:53:15.000000 hqq-0.1.7.post1/hqq/models/timm/vit_clip.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.796661 hqq-0.1.7.post1/hqq/models/vllm/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post1/hqq/models/vllm/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6114 2024-03-15 12:07:03.000000 hqq-0.1.7.post1/hqq/models/vllm/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    16480 2024-03-14 15:55:27.000000 hqq-0.1.7.post1/hqq/models/vllm/llama.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.796661 hqq-0.1.7.post1/hqq/utils/
+-rw-rw-r--   0 hicham    (1009) hicham    (1009)        0 2024-04-16 10:04:22.000000 hqq-0.1.7.post1/hqq/utils/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    10844 2024-04-23 16:50:10.000000 hqq-0.1.7.post1/hqq/utils/generation_hf.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6066 2024-04-22 17:00:27.000000 hqq-0.1.7.post1/hqq/utils/patching.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.788661 hqq-0.1.7.post1/hqq.egg-info/
+-rw-r--r--   0 hicham    (1009) hicham    (1009)      438 2024-05-03 14:43:35.000000 hqq-0.1.7.post1/hqq.egg-info/PKG-INFO
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1109 2024-05-03 14:43:35.000000 hqq-0.1.7.post1/hqq.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        1 2024-05-03 14:43:35.000000 hqq-0.1.7.post1/hqq.egg-info/dependency_links.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)       92 2024-05-03 14:43:35.000000 hqq-0.1.7.post1/hqq.egg-info/requires.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        4 2024-05-03 14:43:35.000000 hqq-0.1.7.post1/hqq.egg-info/top_level.txt
+-rw-rw-r--   0 hicham    (1009) hicham    (1009)       38 2024-05-03 14:45:11.800661 hqq-0.1.7.post1/setup.cfg
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1706 2024-05-03 14:43:06.000000 hqq-0.1.7.post1/setup.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.800661 hqq-0.1.7.post1/tests/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3689 2024-03-25 10:44:50.000000 hqq-0.1.7.post1/tests/test_bitpack.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11302 2024-03-01 10:40:44.000000 hqq-0.1.7.post1/tests/test_quantize.py
```

### Comparing `hqq-0.1.7/LICENSE` & `hqq-0.1.7.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/backends/marlin.py` & `hqq-0.1.7.post1/hqq/backends/marlin.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/backends/torchao.py` & `hqq-0.1.7.post1/hqq/backends/torchao.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/core/bitpack.py` & `hqq-0.1.7.post1/hqq/core/bitpack.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/core/optimize.py` & `hqq-0.1.7.post1/hqq/core/optimize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Written by Dr. Hicham Badri @Mobius Labs GmbH - 2023
 #####################################################
 import torch
 import numpy as np
 from torch import float32, float16, Tensor
 from functools import partial
+from typing import Union
+
 
 # re-estimate the scale based on the inverse median: Only tested with axis==0
 def update_scale_inverse_median(
     W_f: Tensor, scale: Tensor, zero: Tensor, axis: int, min_max: list
 ) -> tuple:
     scale_rng = 2e4
     z_val = 1e-4
@@ -101,16 +103,16 @@
 @torch.inference_mode()
 def optimize_weights_proximal_v2(
     tensor: Tensor,
     scale: Tensor,
     zero: Tensor,
     min_max: list,
     axis: int = 0,
-    device: str | None = None,
-    dtype: torch.dtype | None = None,
+    device: Union[str, None] = None,
+    dtype: Union[torch.dtype, None] = None,
     opt_params: dict = {
         "lp_norm": 0.7,
         "beta": 1e1,
         "kappa": 1.01,
         "iters": 20,
         "tol": 0.0,
         "early_stop": True,
@@ -129,20 +131,20 @@
     # Check
     assert lp_norm <= 1.0, "lp_norm should be <=1"
     assert beta > 0.0, "beta should be > 0"
     assert kappa > 1.0, "kappa should be > 1"
     assert iters > 1, "iters should be > 1"
 
     # Cast/device
-    if(device is None):
+    if device is None:
         device = tensor.device
     else:
         device = torch.device(device)
 
-    if(dtype is None):
+    if dtype is None:
         dtype = float16 if (device.type == "cuda") else float32
 
     W_f = tensor.to(device=device, dtype=dtype)
     scale = scale.to(device=device, dtype=dtype)
     zero = zero.to(device=device, dtype=dtype)
 
     # Update scale: works slightly better. Tested on Llama2 only
@@ -189,30 +191,30 @@
 @torch.inference_mode()
 def optimize_weights_proximal_legacy(
     tensor: Tensor,
     scale: Tensor,
     zero: Tensor,
     min_max: list,
     axis: int = 0,
-    device: str | None = None,
+    device: Union[str, None] = None,
     opt_params: dict = {"lp_norm": 0.7, "beta": 1e1, "kappa": 1.01, "iters": 20},
     verbose: bool = False,
 ) -> tuple:
     lp_norm, beta, kappa, iters = (
         opt_params["lp_norm"],
         opt_params["beta"],
         opt_params["kappa"],
         opt_params["iters"],
     )
 
-    if(device is None):
+    if device is None:
         device = tensor.device
     else:
         device = torch.device(device)
-    
+
     dtype = float16 if (device.type == "cuda") else float32
     W_f = tensor.to(dtype=dtype, device=device)
     scale = scale.to(dtype=dtype, device=device)
     zero = zero.to(dtype=dtype, device=device)
 
     best_error = 1e4
     for i in range(iters):
@@ -235,181 +237,238 @@
     del W_f, W_q, W_r, W_e
     torch.cuda.empty_cache()
 
     W_q = torch.round(tensor * scale + zero).clamp(min_max[0], min_max[1])
     return W_q, scale, zero
 
 
-#Default: fast with early stopping
-optimize_weights_proximal      = optimize_weights_proximal_legacy
+# Default: fast with early stopping
+optimize_weights_proximal = optimize_weights_proximal_legacy
 
-#Slower, better quality: no early stoppping, more iterations
-optimize_weights_proximal_slow = partial(optimize_weights_proximal_v2, 
-    dtype=torch.float32, 
+# Slower, better quality: no early stoppping, more iterations
+optimize_weights_proximal_slow = partial(
+    optimize_weights_proximal_v2,
+    dtype=torch.float32,
     opt_params={
-    "lp_norm": 0.7,
-    "beta": 1e1,
-    "kappa": 1.01,
-    "iters": 100,
-    "tol": 0.0,
-    "early_stop": False,
-    "scale_gridsearch": False},)
+        "lp_norm": 0.7,
+        "beta": 1e1,
+        "kappa": 1.01,
+        "iters": 100,
+        "tol": 0.0,
+        "early_stop": False,
+        "scale_gridsearch": False,
+    },
+)
 
 ##############################################################################################################
-#L1 with SGD optimizer: supports scale and W_q updates. L{p<1} fails with SGD
+# L1 with SGD optimizer: supports scale and W_q updates. L{p<1} fails with SGD
+
 
 class LinearSchedulerWithWarmStart(torch.optim.lr_scheduler._LRScheduler):
     def __init__(self, optimizer, lr_start, lr_end, iters, warm_start=0, last_epoch=-1):
-        iters_wrm   = max(0, int(iters*warm_start))
-        self.lr_wrm = np.linspace(lr_end, lr_start, iters_wrm) if(iters_wrm>0) else np.array([])
+        iters_wrm = max(0, int(iters * warm_start))
+        self.lr_wrm = (
+            np.linspace(lr_end, lr_start, iters_wrm)
+            if (iters_wrm > 0)
+            else np.array([])
+        )
         self.lr_mid = np.linspace(lr_start, lr_end, iters - iters_wrm)
         self.lr_sch = np.concatenate([self.lr_wrm, self.lr_mid])
-        self.idx    = 0
+        self.idx = 0
         super(LinearSchedulerWithWarmStart, self).__init__(optimizer, last_epoch)
 
     def get_lr(self):
         self.idx = min(self.idx, len(self.lr_sch) - 1)
         out = [self.lr_sch[self.idx] for base_lr in self.base_lrs]
-        self.idx +=1 
+        self.idx += 1
         return out
 
+
 # SGD solver  || W - dequantize(quantize(W))||_1 (p=1 only, with additional fake inputs x)
 def optimize_weights_autograd(
     tensor: Tensor,
     scale: Tensor,
     zero: Tensor,
     min_max: list,
     axis: int = 0,
-    device: str | None = None,
-    dtype: torch.dtype = float32,
-    opt_params: dict = {"lr": 2e-3, "iters": 2500, "lr_schedule": False, "update_Wq":False, "use_fake_data": False},
-    data_params: dict = {"normalize": False, "data_rng": 10., "data_ctx": 32},
+    device: Union[str, None] = None,
+    dtype: Union[torch.dtype, None] = float32,
+    opt_params: dict = {
+        "lr": 2e-3,
+        "iters": 2500,
+        "lr_schedule": False,
+        "update_Wq": False,
+        "use_fake_data": False,
+    },
+    data_params: dict = {"normalize": False, "data_rng": 10.0, "data_ctx": 32},
     compile: bool = True,
     verbose: bool = False,
 ) -> tuple:
-    
     ref_device = scale.device
-    ref_dtype  = scale.dtype
+    ref_dtype = scale.dtype
 
-    if(device is None):
+    if device is None:
         device = tensor.device
     else:
         device = torch.device(device)
 
     W_f = tensor.to(dtype=dtype, device=device)
 
     params = {}
-    params["scale"]  = torch.nn.Parameter(scale.to(dtype=dtype, device=device), requires_grad=True)
-    params["zero"]   = torch.nn.Parameter(zero.to(dtype=dtype, device=device),  requires_grad=True)
+    params["scale"] = torch.nn.Parameter(
+        scale.to(dtype=dtype, device=device), requires_grad=True
+    )
+    params["zero"] = torch.nn.Parameter(
+        zero.to(dtype=dtype, device=device), requires_grad=True
+    )
 
-    if(opt_params["update_Wq"]):
+    if opt_params["update_Wq"]:
         with torch.no_grad():
-            params["W_q"] = torch.round(W_f * params["scale"] + params["zero"]).clamp(min_max[0], min_max[1])
+            params["W_q"] = torch.round(W_f * params["scale"] + params["zero"]).clamp(
+                min_max[0], min_max[1]
+            )
         params["W_q"] = torch.nn.Parameter(params["W_q"], requires_grad=True)
 
     optimizer = torch.optim.AdamW(
         [params[k] for k in params],
         lr=opt_params["lr"],
         betas=(0.9, 0.99),
         eps=1e-06,
         weight_decay=0.0,
     )
 
-    if(opt_params["lr_schedule"]):
-        scheduler = LinearSchedulerWithWarmStart(optimizer, lr_start=opt_params["lr"], lr_end=1e-6, iters=opt_params["iters"], warm_start=0)
+    if opt_params["lr_schedule"]:
+        scheduler = LinearSchedulerWithWarmStart(
+            optimizer,
+            lr_start=opt_params["lr"],
+            lr_end=1e-6,
+            iters=opt_params["iters"],
+            warm_start=0,
+        )
     else:
         scheduler = None
 
     with torch.no_grad():
-        if(data_params['normalize']):
-            scale_loss = 1./(tensor.abs().mean() + 1e-4)
+        if data_params["normalize"]:
+            scale_loss = 1.0 / (tensor.abs().mean() + 1e-4)
         else:
-            scale_loss = 1.
+            scale_loss = 1.0
 
     def _loss_fct(output, target):
-        return torch.mean(torch.abs(scale_loss*(target - output))) #L1
+        return torch.mean(torch.abs(scale_loss * (target - output)))  # L1
 
     def _fake_quant_fixed_Wq(W_f):
         # Quantize
-        W_q = torch.round(W_f * params["scale"] + params["zero"]).clamp(min_max[0], min_max[1])
+        W_q = torch.round(W_f * params["scale"] + params["zero"]).clamp(
+            min_max[0], min_max[1]
+        )
         # Dequantize
         W_r = (W_q - params["zero"]) / params["scale"]
         return W_r
 
     def _fake_quant_update_Wq(W_f):
         # Quantize
         W_q = torch.round(params["W_q"]).clamp(min_max[0], min_max[1])
         # Dequantize
         W_r = (W_q - params["zero"]) / params["scale"]
         return W_r
 
-    if(opt_params["update_Wq"]):
-        _fake_quant = _fake_quant_update_Wq 
+    if opt_params["update_Wq"]:
+        _fake_quant = _fake_quant_update_Wq
     else:
         _fake_quant = _fake_quant_fixed_Wq
 
     def _fake_quant_loss(W_f):
         return _loss_fct(_fake_quant(W_f), W_f)
 
     def _fake_quant_loss_with_fake_data(W_f):
-        x      = (torch.rand([data_params['data_ctx'], W_f.shape[1]], device=device, dtype=dtype) - 0.5)*2**data_params['data_rng']
-        y_ref  = torch.matmul(x, W_f.T)
+        x = (
+            torch.rand(
+                [data_params["data_ctx"], W_f.shape[1]], device=device, dtype=dtype
+            )
+            - 0.5
+        ) * 2 ** data_params["data_rng"]
+        y_ref = torch.matmul(x, W_f.T)
         y_pred = torch.matmul(x, _fake_quant(W_f).T)
         return _loss_fct(y_pred, y_ref)
 
-    if(opt_params['use_fake_data']):
-        _fake_quant_loss = _fake_quant_loss_with_fake_data 
+    if opt_params["use_fake_data"]:
+        _fake_quant_loss = _fake_quant_loss_with_fake_data
     else:
         _fake_quant_loss = _fake_quant_loss
 
-    if(compile):
+    if compile:
         _fake_quant_loss = torch.compile(_fake_quant_loss)
 
     def _step(W_f):
         optimizer.zero_grad()
         loss = _fake_quant_loss(W_f)
         loss.backward()
         optimizer.step()
-        if(scheduler is not None): 
+        if scheduler is not None:
             scheduler.step()
         return np.round(loss.item(), 10)
 
     with torch.no_grad():
         _init_loss = _fake_quant_loss(W_f).item()
 
     for i in range(opt_params["iters"]):
         loss_out = _step(W_f)
         if verbose and (i % 100) == 0:
             print(i, loss_out)
 
     with torch.no_grad():
         _final_loss = _fake_quant_loss(W_f).item()
 
-    if (_final_loss < _init_loss):
+    if _final_loss < _init_loss:
         for k in params:
             params[k] = params[k].data.detach()
     else:
         if verbose:
             print("optimization failed...")
         params = {"scale": scale, "zero": zero}
 
     scale = params["scale"].to(device=ref_device, dtype=ref_dtype)
-    zero  = params["zero"].to(device=ref_device, dtype=ref_dtype)
+    zero = params["zero"].to(device=ref_device, dtype=ref_dtype)
 
-    if("W_q" in params):
-        W_q   = params["W_q"].to(device=ref_device, dtype=ref_dtype)
+    if "W_q" in params:
+        W_q = params["W_q"].to(device=ref_device, dtype=ref_dtype)
     else:
-        W_q   = torch.round(tensor * scale + zero).clamp(min_max[0], min_max[1]).to(device=ref_device, dtype=ref_dtype)
+        W_q = (
+            torch.round(tensor * scale + zero)
+            .clamp(min_max[0], min_max[1])
+            .to(device=ref_device, dtype=ref_dtype)
+        )
 
     del W_f
     torch.cuda.empty_cache()
     return W_q, scale, zero
 
 
-optimize_weights_autograd_main     = partial(optimize_weights_autograd, dtype=torch.float32, 
-                                                                opt_params={"lr": 2e-3, "iters": 1000, "lr_schedule": True, "update_Wq": True, "use_fake_data": False}, 
-                                                                verbose=False, compile=True)
-
-optimize_weights_autograd_fakedata = partial(optimize_weights_autograd, dtype=torch.float32, 
-                                                                opt_params={"lr": 2e-3, "iters": 1000, "lr_schedule": True, "update_Wq": True, "use_fake_data": True}, 
-                                                                data_params={"normalize": False, "data_rng": 10., "data_ctx": 32},
-                                                                verbose=False, compile=True)
+optimize_weights_autograd_main = partial(
+    optimize_weights_autograd,
+    dtype=torch.float32,
+    opt_params={
+        "lr": 2e-3,
+        "iters": 1000,
+        "lr_schedule": True,
+        "update_Wq": True,
+        "use_fake_data": False,
+    },
+    verbose=False,
+    compile=True,
+)
+
+optimize_weights_autograd_fakedata = partial(
+    optimize_weights_autograd,
+    dtype=torch.float32,
+    opt_params={
+        "lr": 2e-3,
+        "iters": 1000,
+        "lr_schedule": True,
+        "update_Wq": True,
+        "use_fake_data": True,
+    },
+    data_params={"normalize": False, "data_rng": 10.0, "data_ctx": 32},
+    verbose=False,
+    compile=True,
+)
```

### Comparing `hqq-0.1.7/hqq/core/peft.py` & `hqq-0.1.7.post1/hqq/core/peft.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/core/quantize.py` & `hqq-0.1.7.post1/hqq/core/quantize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Written by Dr. Hicham Badri @Mobius Labs GmbH - 2023
 #####################################################
 import torch
 from torch import uint8, int32, float16, nn, Tensor
 import copy
 from enum import Enum
+from typing import Union
 
 from .utils import is_divisible
 from .optimize import optimize_weights_proximal
 from .bitpack import BitPack
 
 
 # Main HQQ Quantizer
@@ -54,15 +55,15 @@
         nbits: int = 4,
         channel_wise: bool = True,
         group_size: int = 64,
         optimize: bool = False,
         round_zero: bool = False,
         axis: int = 0,
         bitpack: bool = True,
-        compute_dtype: torch.dtype | None = None,
+        compute_dtype: Union[torch.dtype, None] = None,
         view_as_float: bool = False,
         device: str = "cuda",
     ) -> tuple:
         assert nbits in Quantizer.SUPPORTED_BITS, (
             "nbits=" + str(nbits) + " not supported."
         )
         assert axis in [0, 1], "axis should be either 0 or 1"
@@ -351,15 +352,15 @@
     if hqq_aten_is_available:
         backend = HQQBackend.ATEN
     else:
         backend = HQQBackend.PYTORCH
 
     def __init__(
         self,
-        linear_layer: nn.Module | None,
+        linear_layer: Union[nn.Module, None],
         quant_config: dict,
         del_orig: bool = True,
         compute_dtype: torch.dtype = float16,
         device: str = "cuda",
         initialize: bool = True,
     ):
         super().__init__()
```

### Comparing `hqq-0.1.7/hqq/engine/base.py` & `hqq-0.1.7.post1/hqq/engine/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/engine/hf.py` & `hqq-0.1.7.post1/hqq/engine/hf.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/engine/timm.py` & `hqq-0.1.7.post1/hqq/engine/timm.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/engine/vllm.py` & `hqq-0.1.7.post1/hqq/engine/vllm.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/kernels/hqq_aten_cuda.cpp` & `hqq-0.1.7.post1/hqq/kernels/hqq_aten_cuda.cpp`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/kernels/hqq_aten_cuda_kernel.cu` & `hqq-0.1.7.post1/hqq/kernels/hqq_aten_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/kernels/hqq_aten_torch.cpp` & `hqq-0.1.7.post1/hqq/kernels/hqq_aten_torch.cpp`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/models/base.py` & `hqq-0.1.7.post1/hqq/models/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/models/hf/base.py` & `hqq-0.1.7.post1/hqq/models/hf/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/models/hf/llama.py` & `hqq-0.1.7.post1/hqq/models/hf/llama.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/models/hf/mistral.py` & `hqq-0.1.7.post1/hqq/models/hf/mistral.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/models/hf/mixtral.py` & `hqq-0.1.7.post1/hqq/models/hf/mixtral.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/models/hf/phi.py` & `hqq-0.1.7.post1/hqq/models/hf/phi.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/models/hf/phi_opt.py` & `hqq-0.1.7.post1/hqq/models/hf/phi_opt.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/models/timm/base.py` & `hqq-0.1.7.post1/hqq/models/timm/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/models/timm/vit_clip.py` & `hqq-0.1.7.post1/hqq/models/timm/vit_clip.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/models/vllm/base.py` & `hqq-0.1.7.post1/hqq/models/vllm/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/models/vllm/llama.py` & `hqq-0.1.7.post1/hqq/models/vllm/llama.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/utils/generation_hf.py` & `hqq-0.1.7.post1/hqq/utils/generation_hf.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq/utils/patching.py` & `hqq-0.1.7.post1/hqq/utils/patching.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/hqq.egg-info/SOURCES.txt` & `hqq-0.1.7.post1/hqq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/setup.py` & `hqq-0.1.7.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def run(self):
         egg_info.run(self)
         run_setup_cuda()
 
 
 setup(
     name="hqq",
-    version="0.1.7",
+    version="0.1.7.post1",
     description="Half-Quadratic Quantization (HQQ)",
     url="https://github.com/mobiusml/hqq/",
     author="Dr. Hicham Badri",
     author_email="hicham@mobiuslabs.com",
     license="Apache 2",
     packages=find_packages(include=["hqq", "hqq.*"]),
     package_data={
```

### Comparing `hqq-0.1.7/tests/test_bitpack.py` & `hqq-0.1.7.post1/tests/test_bitpack.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7/tests/test_quantize.py` & `hqq-0.1.7.post1/tests/test_quantize.py`

 * *Files identical despite different names*


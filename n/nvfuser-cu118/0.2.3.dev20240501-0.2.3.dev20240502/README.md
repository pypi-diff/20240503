# Comparing `tmp/nvfuser_cu118-0.2.3.dev20240501.tar.gz` & `tmp/nvfuser_cu118-0.2.3.dev20240502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvfuser_cu118-0.2.3.dev20240501.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvfuser_cu118-0.2.3.dev20240502.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvfuser_cu118-0.2.3.dev20240501.tar` & `nvfuser_cu118-0.2.3.dev20240502.tar`

### PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvfuser_cu118
-Version: 0.2.3.dev20240501
+Version: 0.2.3.dev20240502
 Summary: A Fusion Code Generator for NVIDIA GPUs (commonly known as 'nvFuser')
 Home-page: https://github.com/NVIDIA/Fuser
 License: BSD-3-Clause
 License-File: LICENSE
 Provides-Extra: test
 Provides-Extra: torch
 Stub-Only: True
```


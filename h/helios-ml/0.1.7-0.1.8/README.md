# Comparing `tmp/helios_ml-0.1.7.tar.gz` & `tmp/helios_ml-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios_ml-0.1.7.tar", last modified: Wed May  1 19:54:10 2024, max compression
+gzip compressed data, was "helios_ml-0.1.8.tar", last modified: Fri May  3 20:20:58 2024, max compression
```

## Comparing `helios_ml-0.1.7.tar` & `helios_ml-0.1.8.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.419554 helios_ml-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.403554 helios_ml-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-01 19:53:38.000000 helios_ml-0.1.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-01 19:53:38.000000 helios_ml-0.1.7/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 19:53:38.000000 helios_ml-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-01 19:53:38.000000 helios_ml-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-01 19:53:38.000000 helios_ml-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-01 19:54:10.419554 helios_ml-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-01 19:53:38.000000 helios_ml-0.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.403554 helios_ml-0.1.7/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/data/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-05-01 19:53:38.000000 helios_ml-0.1.7/data/logo/logo-background.png
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-01 19:53:38.000000 helios_ml-0.1.7/data/logo/logo-transparent.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.403554 helios_ml-0.1.7/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/examples/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-05-01 19:53:38.000000 helios_ml-0.1.7/examples/cifar10/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-01 19:53:38.000000 helios_ml-0.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 19:53:38.000000 helios_ml-0.1.7/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-01 19:53:38.000000 helios_ml-0.1.7/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-01 19:53:38.000000 helios_ml-0.1.7/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:54:10.419554 helios_ml-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.403554 helios_ml-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/src/helios/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.407554 helios_ml-0.1.7/src/helios/core/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/rng.py
--rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/data/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/data/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/losses/weighted_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/metrics/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/model/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/nn/swa_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/optim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.411554 helios_ml-0.1.7/src/helios/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/scheduler/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35609 2024-05-01 19:53:38.000000 helios_ml-0.1.7/src/helios/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.415554 helios_ml-0.1.7/src/helios_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-01 19:54:10.000000 helios_ml-0.1.7/src/helios_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-01 19:54:10.000000 helios_ml-0.1.7/src/helios_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:54:10.000000 helios_ml-0.1.7/src/helios_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-01 19:54:10.000000 helios_ml-0.1.7/src/helios_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 19:54:10.000000 helios_ml-0.1.7/src/helios_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.415554 helios_ml-0.1.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.415554 helios_ml-0.1.7/test/registry_test/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/foo.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/func_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.415554 helios_ml-0.1.7/test/registry_test/nested/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/nested/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/nested/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/registry_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-01 19:53:38.000000 helios_ml-0.1.7/test/test_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:54:10.415554 helios_ml-0.1.7/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-01 19:53:38.000000 helios_ml-0.1.7/tools/generate_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.118081 helios_ml-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.102081 helios_ml-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.102081 helios_ml-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-03 20:20:12.000000 helios_ml-0.1.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-03 20:20:12.000000 helios_ml-0.1.8/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-03 20:20:12.000000 helios_ml-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-03 20:20:12.000000 helios_ml-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-03 20:20:12.000000 helios_ml-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-03 20:20:58.118081 helios_ml-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-03 20:20:12.000000 helios_ml-0.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.102081 helios_ml-0.1.8/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/data/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-05-03 20:20:12.000000 helios_ml-0.1.8/data/logo/logo-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-03 20:20:12.000000 helios_ml-0.1.8/data/logo/logo-transparent.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.102081 helios_ml-0.1.8/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/examples/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-05-03 20:20:12.000000 helios_ml-0.1.8/examples/cifar10/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-03 20:20:12.000000 helios_ml-0.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-03 20:20:12.000000 helios_ml-0.1.8/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-03 20:20:12.000000 helios_ml-0.1.8/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-03 20:20:12.000000 helios_ml-0.1.8/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:20:58.118081 helios_ml-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.102081 helios_ml-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/src/helios/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/src/helios/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/src/helios/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/data/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/losses/weighted_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/metrics/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/nn/swa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/optim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/scheduler/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35697 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.114081 helios_ml-0.1.8/src/helios_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-03 20:20:58.000000 helios_ml-0.1.8/src/helios_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-03 20:20:58.000000 helios_ml-0.1.8/src/helios_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:20:58.000000 helios_ml-0.1.8/src/helios_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-03 20:20:58.000000 helios_ml-0.1.8/src/helios_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 20:20:58.000000 helios_ml-0.1.8/src/helios_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.114081 helios_ml-0.1.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.114081 helios_ml-0.1.8/test/registry_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/foo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/func_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.114081 helios_ml-0.1.8/test/registry_test/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/nested/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/nested/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.114081 helios_ml-0.1.8/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-03 20:20:12.000000 helios_ml-0.1.8/tools/generate_requirements.py
```

### Comparing `helios_ml-0.1.7/.github/workflows/publish.yml` & `helios_ml-0.1.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/.github/workflows/tests.yml` & `helios_ml-0.1.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/.pre-commit-config.yaml` & `helios_ml-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/LICENSE` & `helios_ml-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/PKG-INFO` & `helios_ml-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.7
+Version: 0.1.8
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.7/README.rst` & `helios_ml-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/data/logo/logo-background.png` & `helios_ml-0.1.8/data/logo/logo-background.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/data/logo/logo-transparent.png` & `helios_ml-0.1.8/data/logo/logo-transparent.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/examples/cifar10/cifar10.py` & `helios_ml-0.1.8/examples/cifar10/cifar10.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/pyproject.toml` & `helios_ml-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/core/__init__.py` & `helios_ml-0.1.8/src/helios/core/__init__.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/core/cuda.py` & `helios_ml-0.1.8/src/helios/core/cuda.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/core/distributed.py` & `helios_ml-0.1.8/src/helios/core/distributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import dataclasses
+import dataclasses as dc
 import os
 import typing
 
 import torch
 import torch.distributed as dist
 
 
@@ -69,15 +69,15 @@
 
 
 def is_dist_active() -> bool:
     """Check if torch.distributed is active."""
     return dist.is_available() and dist.is_initialized()
 
 
-@dataclasses.dataclass
+@dc.dataclass
 class DistributedInfo:
     """
     Bundle information regarding distributed state.
 
     To understand what these mean, consider a run being performed over two nodes, each
     with 2 GPUs. Suppose we have a single process per GPU. Then the following values are
     assigned:
```

### Comparing `helios_ml-0.1.7/src/helios/core/logging.py` & `helios_ml-0.1.8/src/helios/core/logging.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/core/rng.py` & `helios_ml-0.1.8/src/helios/core/rng.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/core/utils.py` & `helios_ml-0.1.8/src/helios/core/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/data/__init__.py` & `helios_ml-0.1.8/src/helios/data/__init__.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/data/datamodule.py` & `helios_ml-0.1.8/src/helios/data/datamodule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import abc
 import copy
-import dataclasses
+import dataclasses as dc
 import enum
 import typing
 
 import torch
 import torch.utils.data as tud
 
 from helios import core
@@ -156,15 +156,15 @@
             sampler=sampler,
             worker_init_fn=_seed_worker,
         ),
         sampler,
     )
 
 
-@dataclasses.dataclass
+@dc.dataclass
 class DataLoaderParams:
     """
     Params used to create the dataloader object.
 
     Args:
         random_seed (int): value to use as seed for the worker processes.
         batch_size (int): number of samplers per batch.
@@ -185,33 +185,31 @@
     drop_last: bool = False
     debug_mode: bool = False
     is_distributed: bool | None = None
     sampler: ResumableSamplerType | None = None
 
     def to_dict(self) -> dict[str, typing.Any]:
         """Convert the params object to a dictionary using shallow copies."""
-        return {
-            field.name: getattr(self, field.name) for field in dataclasses.fields(self)
-        }
+        return {field.name: getattr(self, field.name) for field in dc.fields(self)}
 
     @classmethod
     def from_dict(cls, table: dict[str, typing.Any]):
         """Create a new params object from the given table."""
         params = cls()
-        keys = [field.name for field in dataclasses.fields(params)]
+        keys = [field.name for field in dc.fields(params)]
 
         # Skip the sampler key, since that one needs to be created differently.
         for key in keys:
             if key in table and key != "sampler":
                 setattr(params, key, table[key])
 
         return params
 
 
-@dataclasses.dataclass
+@dc.dataclass
 class Dataset:
     """
     The dataset and corresponding data loader params.
 
     Args:
         dataset (torch.utils.data.Dataset): the dataset.
         params (DataLoaderParams): the data loader params.
@@ -290,14 +288,35 @@
         """Reference to the trainer."""
         return core.get_from_optional(self._trainer)
 
     @trainer.setter
     def trainer(self, t) -> None:
         self._trainer = t
 
+    @property
+    def train_dataset(self) -> tud.Dataset | None:
+        """The training dataset (if available)."""
+        if self._train_dataset is not None:
+            return self._train_dataset.dataset
+        return None
+
+    @property
+    def valid_dataset(self) -> tud.Dataset | None:
+        """The validation dataset (if available)."""
+        if self._valid_dataset is not None:
+            return self._valid_dataset.dataset
+        return None
+
+    @property
+    def test_dataset(self) -> tud.Dataset | None:
+        """The testing dataset (if available)."""
+        if self._test_dataset is not None:
+            return self._test_dataset.dataset
+        return None
+
     def prepare_data(self) -> None:  # noqa: B027
         """
         Prepare data for training.
 
         This can include downloading datasets, or streaming them from external services.
         This function will be called on the primary process when using distributed
         training (will be called prior to initialization of the processes) so don't store
```

### Comparing `helios_ml-0.1.7/src/helios/data/functional.py` & `helios_ml-0.1.8/src/helios/data/functional.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/data/samplers.py` & `helios_ml-0.1.8/src/helios/data/samplers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/data/transforms.py` & `helios_ml-0.1.8/src/helios/data/transforms.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/losses/utils.py` & `helios_ml-0.1.8/src/helios/losses/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/losses/weighted_loss.py` & `helios_ml-0.1.8/src/helios/losses/weighted_loss.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/metrics/functional.py` & `helios_ml-0.1.8/src/helios/metrics/functional.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/metrics/metrics.py` & `helios_ml-0.1.8/src/helios/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/model/model.py` & `helios_ml-0.1.8/src/helios/model/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -314,21 +314,35 @@
         self._running_losses.clear()
 
     def have_metrics_improved(self) -> bool:
         """
         Determine whether the current validation results are an improvement or not.
 
         This is used when early stopping is enabled in the trainer to determine whether
-        the stop cycle count should increase or not.
+        the stop cycle count should increase or not. This is called immediately after the
+        validation cycle finishes.
 
         Returns:
             bool: false if no improvements were seen in the last validation cycle.
         """
         return True
 
+    def should_training_stop(self) -> bool:
+        """
+        Determine whether training should stop or continue.
+
+        This is used in the event that a validation metric crosses a certain threshold
+        after which training should stop. This is called after the validation cycle
+        finishes.
+
+        Returns:
+            bool: False if training should continue, true otherwise.
+        """
+        return False
+
     def on_testing_start(self) -> None:
         """
         Perform any necessary actions when testing starts.
 
         By default, this will clear out the table of testing values, but you may use it
         for any other tasks that should happen when testing begins.
         """
```

### Comparing `helios_ml-0.1.7/src/helios/model/utils.py` & `helios_ml-0.1.8/src/helios/model/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/nn/swa_utils.py` & `helios_ml-0.1.8/src/helios/nn/swa_utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/nn/utils.py` & `helios_ml-0.1.8/src/helios/nn/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/onnx.py` & `helios_ml-0.1.8/src/helios/onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/optim/utils.py` & `helios_ml-0.1.8/src/helios/optim/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/scheduler/schedulers.py` & `helios_ml-0.1.8/src/helios/scheduler/schedulers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/scheduler/utils.py` & `helios_ml-0.1.8/src/helios/scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/src/helios/trainer.py` & `helios_ml-0.1.8/src/helios/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-import dataclasses
+import dataclasses as dc
 import enum
 import itertools
 import os
 import pathlib
 import re
 import time
 import typing
@@ -59,15 +59,15 @@
     the distributed handler.
     """
 
     TRAIN = 0
     TEST = 1
 
 
-@dataclasses.dataclass
+@dc.dataclass
 class TrainingState:
     """
     The training state.
 
     Args:
         current_iteration (int): the current iteration number. Note that this refers to
         the iteration in which gradients are updated. This may or may not be equal to the
@@ -88,31 +88,34 @@
     global_epoch: int = 0
     validation_cycles: int = 0
     dataset_iter: int = 0
     early_stop_count: int = 0
     average_iter_time: float = 0
     running_iter: int = 0
 
-    dict = dataclasses.asdict
+    dict = dc.asdict
 
 
-def find_last_checkpoint(root: pathlib.Path) -> pathlib.Path | None:
+def find_last_checkpoint(root: pathlib.Path | None) -> pathlib.Path | None:
     """
     Find the last saved checkpoint (if available).
 
     The function assumes that checkpoint names contain 'epoch_<epoch>' and 'iter_<iter>'
     in the name, in which case it will return the path to the checkpoint with the highest
     epoch and/or iteration count.
 
     Args:
         root (pathlib.Path): the path where the checkpoints are stored.
 
     Returns:
         pathlib.Path | None: the path to the last checkpoint (if any).
     """
+    if root is None:
+        return None
+
     epoch = 0
     ite = 0
     last_chkpt = None
     regexp = re.compile(r"epoch_\d+_iter_\d+")
     for path in root.glob("*.pth"):
         if not regexp.search(path.stem):
             continue
@@ -390,22 +393,22 @@
         appropriate training loop for the given training unit.
         """
         self._configure_env()
         self._setup_datamodule()
         self._setup_model()
         self._prepare_roots()
 
-        chkpt_path = find_last_checkpoint(core.get_from_optional(self._chkpt_root))
-        training_state, resume_training = self._load_checkpoint(chkpt_path)
+        chkpt_path = find_last_checkpoint(self._chkpt_root)
+        training_state = self._load_checkpoint(chkpt_path)
 
         self._print_header(chkpt_path)
 
         self.model.on_training_start()
         if self._train_unit == TrainingUnit.ITERATION:
-            self._train_on_iteration(training_state, resume_training)
+            self._train_on_iteration(training_state)
         else:
             self._train_on_epoch(training_state)
 
         self.model.on_training_end()
 
         logging.flush_default_loggers()
         logging.close_default_loggers()
@@ -428,16 +431,17 @@
         self._setup_model(fast_init=True)
         self._prepare_roots(mkdir=False)
 
         chkpt_path: pathlib.Path | None = None
         loaded: bool = False
         if self._chkpt_root is not None:
             chkpt_path = find_last_checkpoint(core.get_from_optional(self._chkpt_root))
-            _, loaded = self._load_checkpoint(
-                chkpt_path, skip_rng=True, model_fast_init=True
+            loaded = (
+                self._load_checkpoint(chkpt_path, skip_rng=True, model_fast_init=True)
+                != TrainingState()
             )
 
         # We failed to load the last checkpoint, so tell the model to load its state.
         if self._chkpt_root is None or not loaded:
             self.model.load_for_testing()
 
         self._print_header(chkpt_path, for_training=False)
@@ -696,15 +700,15 @@
         torch.save(state_dict, chkpt_root / filename)
 
     def _load_checkpoint(
         self,
         chkpt_path: pathlib.Path | None,
         skip_rng: bool = False,
         model_fast_init: bool = False,
-    ) -> tuple[TrainingState, bool]:
+    ) -> TrainingState:
         """
         Load the given checkpoint.
 
         Args:
             chkpt_path (pathlib.Path): path to the checkpoint to load.
             skip_rng (bool): if True, skip the loading of the RNG states.
             model_fast_init (bool): whether the model should setup its full state or not.
@@ -712,32 +716,31 @@
         Returns:
             tuple[TrainingState, bool]: returns the loaded training state and True if the
             checkpoint was loaded successfully. Otherwise it returns an empty training
             state and False.
         """
         if chkpt_path is None:
             logging.setup_default_loggers(self._run_name, self._log_path, self._run_path)
-            return TrainingState(), False
+            return TrainingState()
 
         state_dict = torch.load(chkpt_path, map_location=self._map_loc)
         logging.restore_default_loggers(
             state_dict.get("log_path", None), state_dict.get("run_path", None)
         )
         if not skip_rng:
             rng.load_rng_state_dict(state_dict["rng"])
         self.model.load_state_dict(state_dict["model"], fast_init=model_fast_init)
-        return TrainingState(**state_dict["training_state"]), True
+        return TrainingState(**state_dict["training_state"])
 
-    def _train_on_iteration(self, state: TrainingState, resume_training: bool) -> None:
+    def _train_on_iteration(self, state: TrainingState) -> None:
         """
         Run the main loop for iteration-based training.
 
         Args:
             state (TrainingState): the training state.
-            resume_training (bool): if True, then training is resumed from the state.
         """
         total_steps = self._total_steps
         save_freq = self._chkpt_frequency
         val_freq = self._valid_frequency
         print_freq = self._print_frequency
         accumulation_steps = self._accumulation_steps
         enable_progress_bar = self._enable_progress_bar
@@ -830,14 +833,18 @@
                 if (
                     early_stop_cycles is not None
                     and state.early_stop_count >= early_stop_cycles
                 ):
                     training_done = True
                     break
 
+                if self.model.should_training_stop():
+                    training_done = True
+                    break
+
             state.dataset_iter = 0
             state.global_epoch += 1
 
             root_logger.info(
                 f"Epoch {epoch + 1} completed in {time.time() - epoch_start:.2f}s"
             )
 
@@ -945,14 +952,17 @@
             pbar.update()
             if (
                 early_stop_cycles is not None
                 and state.early_stop_count >= early_stop_cycles
             ):
                 training_done = True
 
+            if self.model.should_training_stop():
+                training_done = True
+
     def _validate(self, val_cycle: int) -> None:
         """
         Run the validation loop.
 
         Args:
             val_cycle (int): the current validation cycle number.
         """
```

### Comparing `helios_ml-0.1.7/src/helios_ml.egg-info/PKG-INFO` & `helios_ml-0.1.8/src/helios_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.7
+Version: 0.1.8
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.7/src/helios_ml.egg-info/SOURCES.txt` & `helios_ml-0.1.8/src/helios_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/test/conftest.py` & `helios_ml-0.1.8/test/conftest.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/test/test_core.py` & `helios_ml-0.1.8/test/test_core.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/test/test_data.py` & `helios_ml-0.1.8/test/test_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -227,11 +227,23 @@
         ]
         assert len(typing.cast(typing.Sized, hlds.SAMPLER_REGISTRY.keys())) == len(
             registered_names
         )
         for name in registered_names:
             assert name in hlds.SAMPLER_REGISTRY
 
+    def test_dataset_getters(self) -> None:
+        datamodule = SampleDataModule()
+        datamodule.setup()
+
+        assert datamodule.train_dataset is not None
+        assert datamodule.valid_dataset is not None
+        assert datamodule.test_dataset is not None
+
+        assert isinstance(datamodule.train_dataset, RandomDataset)
+        assert isinstance(datamodule.valid_dataset, SequentialDataset)
+        assert isinstance(datamodule.test_dataset, SequentialDataset)
+
 
 if __name__ == "__main__":
     t = TestDataModule()
     t.test_resume_sequential()
```

### Comparing `helios_ml-0.1.7/test/test_losses.py` & `helios_ml-0.1.8/test/test_losses.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/test/test_metrics.py` & `helios_ml-0.1.8/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/test/test_model.py` & `helios_ml-0.1.8/test/test_model.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/test/test_nn.py` & `helios_ml-0.1.8/test/test_nn.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/test/test_onnx.py` & `helios_ml-0.1.8/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.7/test/test_trainer.py` & `helios_ml-0.1.8/test/test_trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             "eval": False,
             "on_validation_start": False,
             "on_validation_batch_start": False,
             "valid_step": False,
             "on_validation_batch_end": False,
             "on_validation_end": False,
             "have_metrics_improved": False,
+            "should_training_stop": False,
         }
 
         self.called_test_funs: dict[str, bool] = {
             "load_for_testing": False,
             "eval": False,
             "on_testing_start": False,
             "on_testing_batch_start": False,
@@ -112,14 +113,18 @@
     def on_validation_end(self, cycle) -> None:
         self.called_train_funs["on_validation_end"] = True
 
     def have_metrics_improved(self) -> bool:
         self.called_train_funs["have_metrics_improved"] = True
         return True
 
+    def should_training_stop(self) -> bool:
+        self.called_train_funs["should_training_stop"] = True
+        return False
+
     def on_testing_start(self) -> None:
         self.called_test_funs["on_testing_start"] = True
 
     def on_testing_batch_start(self, step) -> None:
         self.called_test_funs["on_testing_batch_start"] = True
 
     def test_step(self, batch, step) -> None:
@@ -146,14 +151,33 @@
             raise RuntimeError("stop")
 
     def train_step(self, batch: torch.Tensor, state) -> None:
         as_np = F.tensor_to_numpy(batch)
         self.batches.append(as_np)
 
 
+class AccumulationModel(hlm.Model):
+    def __init__(self, accumulation_steps: int = 1) -> None:
+        super().__init__("test-accumulation")
+        self.accumulation_steps = accumulation_steps
+        self.global_steps: int = 0
+        self.accumulated_steps: int = 0
+
+    def setup(self, fast_init: bool = False) -> None:
+        pass
+
+    def train_step(self, batch: torch.Tensor, state: hlt.TrainingState) -> None:
+        self.global_steps += 1
+        if self.global_steps % self.accumulation_steps == 0:
+            self.accumulated_steps += 1
+
+        assert state.global_iteration == self.global_steps
+        assert state.current_iteration == self.accumulated_steps
+
+
 class TestTrainingUnit:
     def test_from_str(self) -> None:
         assert hlt.TrainingUnit.from_str("epoch") == hlt.TrainingUnit.EPOCH
         assert hlt.TrainingUnit.from_str("iteration") == hlt.TrainingUnit.ITERATION
 
         with pytest.raises(ValueError):
             hlt.TrainingUnit.from_str("foo")
@@ -344,7 +368,26 @@
         self.check_batches(batches, model.batches)
 
     def test_restart_iter(self, tmp_path: pathlib.Path) -> None:
         self.check_restart_trainer(hlt.TrainingUnit.ITERATION, tmp_path)
 
     def test_restart_epoch(self, tmp_path: pathlib.Path) -> None:
         self.check_restart_trainer(hlt.TrainingUnit.EPOCH, tmp_path)
+
+    def check_accumulation(self, num_steps: int) -> None:
+        datamodule = RandomDatamodule()
+        model = AccumulationModel(num_steps)
+        trainer = hlt.Trainer(
+            train_unit=hlt.TrainingUnit.ITERATION,
+            total_steps=20,
+            use_cpu=True,
+            accumulation_steps=num_steps,
+        )
+
+        trainer.fit(model, datamodule)
+
+    def test_accumulation(self) -> None:
+        self.check_accumulation(1)
+        self.check_accumulation(2)
+        self.check_accumulation(4)
+        self.check_accumulation(5)
+        self.check_accumulation(10)
```

### Comparing `helios_ml-0.1.7/tools/generate_requirements.py` & `helios_ml-0.1.8/tools/generate_requirements.py`

 * *Files identical despite different names*


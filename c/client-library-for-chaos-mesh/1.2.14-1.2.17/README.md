# Comparing `tmp/client-library-for-chaos-mesh-1.2.14.tar.gz` & `tmp/client_library_for_chaos_mesh-1.2.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/client-library-for-chaos-mesh-1.2.14.tar", last modified: Wed Aug 30 19:18:14 2023, max compression
+gzip compressed data, was "client_library_for_chaos_mesh-1.2.17.tar", last modified: Thu May  2 22:21:04 2024, max compression
```

## Comparing `client-library-for-chaos-mesh-1.2.14.tar` & `client_library_for_chaos_mesh-1.2.17.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.088182 client-library-for-chaos-mesh-1.2.14/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6684 2023-08-30 19:18:14.088182 client-library-for-chaos-mesh-1.2.14/PKG-INFO
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.080182 client-library-for-chaos-mesh-1.2.14/chaosmesh/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5488 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.080182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1709 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.080182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.080182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.080182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/disk/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2381 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/disk/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2399 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/disk/fill.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1473 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/disk/read_payload.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1612 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/disk/write_payload.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.080182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/networkattack/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/networkattack/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.080182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/stress/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2233 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/stress/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2855 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/stress/cpu.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1883 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/stress/memory.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.080182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.080182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/jvmfault/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3151 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/jvmfault/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2088 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/jvmfault/gc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3175 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/jvmfault/raise_exception.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.080182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/network/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2214 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/network/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3876 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/network/bandwidth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2193 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/network/partition.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.080182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/podfault/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2736 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/podfault/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2125 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/podfault/container_kill.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      914 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/podfault/pod_failure.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      893 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/podfault/pod_kill.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.084182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/stress/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      705 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/stress/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2549 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/stress/cpu.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2160 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/stress/memory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4438 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/factory.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.084182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.084182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.084182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/disk/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/disk/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      477 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/disk/fill.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      710 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/disk/read_payload.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      618 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/disk/write_payload.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.084182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/networkattack/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/networkattack/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.084182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/stress/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/stress/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      683 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/stress/cpu.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      806 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/stress/memory.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.084182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.084182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/jvmfault/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/jvmfault/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      684 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/jvmfault/gc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      832 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/jvmfault/raise_exception.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.084182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/network/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/network/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      750 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/network/bandwidth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      437 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/network/partition.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.084182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/podfault/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/podfault/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/podfault/container_kill.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      736 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_failure.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      934 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_kill.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.084182 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/stress/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/stress/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/stress/cpu.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/stress/memory.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.088182 client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2110 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/chaos_mesh.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4234 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/crd.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3861 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/experiment.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      536 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/k8s_resource.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      305 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/kubeclient.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      666 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/manifest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      534 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/selector.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.088182 client-library-for-chaos-mesh-1.2.14/chaosmesh/schedules/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4031 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/chaosmesh/schedules/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-30 19:18:14.088182 client-library-for-chaos-mesh-1.2.14/client_library_for_chaos_mesh.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6684 2023-08-30 19:18:14.000000 client-library-for-chaos-mesh-1.2.14/client_library_for_chaos_mesh.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3210 2023-08-30 19:18:14.000000 client-library-for-chaos-mesh-1.2.14/client_library_for_chaos_mesh.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-08-30 19:18:14.000000 client-library-for-chaos-mesh-1.2.14/client_library_for_chaos_mesh.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-08-30 19:18:14.000000 client-library-for-chaos-mesh-1.2.14/client_library_for_chaos_mesh.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       34 2023-08-30 19:18:14.000000 client-library-for-chaos-mesh-1.2.14/client_library_for_chaos_mesh.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-08-30 19:18:14.000000 client-library-for-chaos-mesh-1.2.14/client_library_for_chaos_mesh.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-08-30 19:18:14.088182 client-library-for-chaos-mesh-1.2.14/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1504 2023-08-30 19:17:55.000000 client-library-for-chaos-mesh-1.2.14/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-08-30 19:18:13.000000 client-library-for-chaos-mesh-1.2.14/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.617214 client_library_for_chaos_mesh-1.2.17/
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-02 22:21:04.613214 client_library_for_chaos_mesh-1.2.17/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.605214 client_library_for_chaos_mesh-1.2.17/chaosmesh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.605214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.605214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.605214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.605214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/disk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/disk/fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/disk/read_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/disk/write_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.605214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/networkattack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/networkattack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.605214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/stress/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/stress/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/stress/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.605214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.609214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/jvmfault/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/jvmfault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/jvmfault/gc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/jvmfault/raise_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.609214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/network/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/network/partition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.609214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/podfault/
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/podfault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/podfault/container_kill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/podfault/pod_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/podfault/pod_kill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.609214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/stress/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/stress/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/stress/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.609214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.609214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.609214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/disk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/disk/fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/disk/read_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/disk/write_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.609214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/networkattack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/networkattack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.609214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/stress/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/stress/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/stress/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.609214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.609214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/jvmfault/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/jvmfault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/jvmfault/gc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/jvmfault/raise_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.613214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/network/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/network/partition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.613214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/podfault/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/podfault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/podfault/container_kill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_kill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.613214 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/stress/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/stress/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/stress/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.613214 client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/chaos_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/crd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/k8s_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/kubeclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.613214 client_library_for_chaos_mesh-1.2.17/chaosmesh/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/chaosmesh/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:21:04.613214 client_library_for_chaos_mesh-1.2.17/client_library_for_chaos_mesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-02 22:21:04.000000 client_library_for_chaos_mesh-1.2.17/client_library_for_chaos_mesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-02 22:21:04.000000 client_library_for_chaos_mesh-1.2.17/client_library_for_chaos_mesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 22:21:04.000000 client_library_for_chaos_mesh-1.2.17/client_library_for_chaos_mesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 22:21:04.000000 client_library_for_chaos_mesh-1.2.17/client_library_for_chaos_mesh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 22:21:04.000000 client_library_for_chaos_mesh-1.2.17/client_library_for_chaos_mesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 22:21:04.000000 client_library_for_chaos_mesh-1.2.17/client_library_for_chaos_mesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 22:21:04.617214 client_library_for_chaos_mesh-1.2.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-02 22:20:46.000000 client_library_for_chaos_mesh-1.2.17/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 22:21:04.000000 client_library_for_chaos_mesh-1.2.17/version.txt
```

### Comparing `client-library-for-chaos-mesh-1.2.14/PKG-INFO` & `client_library_for_chaos_mesh-1.2.17/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: client-library-for-chaos-mesh
-Version: 1.2.14
+Version: 1.2.17
 Summary: A client to create experiments in ChaosMesh
 Home-page: https://github.com/vishrantgupta/client-library-for-chaos-mesh
 Author: Vishrant Gupta
 Author-email: vishrant.gupta@gmail.com
 Description-Content-Type: text/markdown
+Requires-Dist: kubernetes>=21.7.0
+Requires-Dist: polling>=0.3.2
+
+[![Upload Python Package](https://github.com/vmware-labs/client-library-for-chaos-mesh/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/vmware-labs/client-library-for-chaos-mesh/actions/workflows/python-publish.yml)
 
 # Client Library for Chaos Mesh
 
 ## Introduction
 
 Chaos Mesh is an open source cloud-native Chaos Engineering platform that allows you to simulate various faults and orchestrate fault scenarios in your kubernetes cluster. This client is written in Python and provides a single point of entry to
 create and manage experiments in Chaos Mesh.
```

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/client.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,11 +112,11 @@
         Arguments:
             experiment_type (Experiment): The type of chaos experiment to unschedule.
             namespace (str): The namespace in which the experiment is running.
             name (str): The name of the chaos experiment.
             **kwargs: The optional parameters for the experiment.
 
         Returns:
-            None
+            Schedule
         """
         log.info(f"deleting schedule for {experiment_type.value} experiment {name} in {namespace} namespace")
         return Schedule(self.factory.get_experiment(experiment_type, **kwargs)).delete(namespace=namespace, name=name)
```

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/__init__.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/disk/__init__.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/disk/fill.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/disk/fill.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/disk/read_payload.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/disk/read_payload.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/disk/write_payload.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/disk/write_payload.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/stress/__init__.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/stress/__init__.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/stress/cpu.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/stress/cpu.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/hosts/stress/memory.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/hosts/stress/memory.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/jvmfault/__init__.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/jvmfault/__init__.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/jvmfault/gc.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/jvmfault/gc.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/jvmfault/raise_exception.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/jvmfault/raise_exception.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/network/__init__.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/network/__init__.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/network/bandwidth.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/network/bandwidth.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/network/partition.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/network/partition.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/podfault/__init__.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/podfault/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         """
         return {
             "action": self.action(),
             "gracePeriod": 0,
             "mode": "all",
             "labels": {},
             "pods": {},
-            "value": ""
+            "value": "",
+            "duration": ""
         }
 
     @property
     def schedule(self) -> dict:
         return {
             "type": "PodChaos",
             "spec": "podChaos"
@@ -83,9 +84,10 @@
         :rtype: dict
         """
         return {
             "selector": asdict(self.kwargs['selector']),
             "mode": self.kwargs.get('mode'),
             "value": self.kwargs.get('value'),
             "action": self.kwargs.get('action'),
-            "gracePeriod": self.kwargs.get('gracePeriod')
+            "gracePeriod": self.kwargs.get('gracePeriod'),
+            "duration": self.kwargs.get('duration')
         }
```

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/podfault/container_kill.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/podfault/container_kill.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/podfault/pod_failure.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/podfault/pod_failure.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/podfault/pod_kill.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/podfault/pod_kill.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/stress/__init__.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/stress/__init__.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/stress/cpu.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/stress/cpu.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/base/k8s/stress/memory.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/base/k8s/stress/memory.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/factory.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/factory.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/disk/read_payload.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/disk/read_payload.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/disk/write_payload.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/disk/write_payload.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/stress/cpu.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/stress/cpu.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/hosts/stress/memory.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/hosts/stress/memory.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/jvmfault/gc.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/jvmfault/gc.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/jvmfault/raise_exception.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/jvmfault/raise_exception.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/network/bandwidth.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/network/bandwidth.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/podfault/container_kill.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/podfault/container_kill.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_failure.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_failure.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_kill.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/podfault/pod_kill.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/stress/cpu.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/stress/cpu.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/experiments/v1alpha1/k8s/stress/memory.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/experiments/v1alpha1/k8s/stress/memory.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/chaos_mesh.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/chaos_mesh.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/crd.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/crd.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/experiment.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/experiment.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/k8s_resource.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/k8s_resource.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/manifest.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/manifest.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/k8s/selector.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/k8s/selector.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/chaosmesh/schedules/__init__.py` & `client_library_for_chaos_mesh-1.2.17/chaosmesh/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/client_library_for_chaos_mesh.egg-info/PKG-INFO` & `client_library_for_chaos_mesh-1.2.17/client_library_for_chaos_mesh.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: client-library-for-chaos-mesh
-Version: 1.2.14
+Version: 1.2.17
 Summary: A client to create experiments in ChaosMesh
 Home-page: https://github.com/vishrantgupta/client-library-for-chaos-mesh
 Author: Vishrant Gupta
 Author-email: vishrant.gupta@gmail.com
 Description-Content-Type: text/markdown
+Requires-Dist: kubernetes>=21.7.0
+Requires-Dist: polling>=0.3.2
+
+[![Upload Python Package](https://github.com/vmware-labs/client-library-for-chaos-mesh/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/vmware-labs/client-library-for-chaos-mesh/actions/workflows/python-publish.yml)
 
 # Client Library for Chaos Mesh
 
 ## Introduction
 
 Chaos Mesh is an open source cloud-native Chaos Engineering platform that allows you to simulate various faults and orchestrate fault scenarios in your kubernetes cluster. This client is written in Python and provides a single point of entry to
 create and manage experiments in Chaos Mesh.
```

### Comparing `client-library-for-chaos-mesh-1.2.14/client_library_for_chaos_mesh.egg-info/SOURCES.txt` & `client_library_for_chaos_mesh-1.2.17/client_library_for_chaos_mesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `client-library-for-chaos-mesh-1.2.14/setup.py` & `client_library_for_chaos_mesh-1.2.17/setup.py`

 * *Files identical despite different names*


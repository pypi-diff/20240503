# Comparing `tmp/radiens-3.0.0b5.tar.gz` & `tmp/radiens-3.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radiens-3.0.0b5.tar", last modified: Wed Mar 27 16:33:48 2024, max compression
+gzip compressed data, was "radiens-3.0.0b6.tar", last modified: Mon Apr 22 06:20:08 2024, max compression
```

## Comparing `radiens-3.0.0b5.tar` & `radiens-3.0.0b6.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.108742 radiens-3.0.0b5/
--rw-r--r--   0 akelly     (502) staff       (20)     1068 2024-02-20 17:19:00.000000 radiens-3.0.0b5/LICENSE
--rw-r--r--   0 akelly     (502) staff       (20)     2518 2024-03-27 16:33:48.108474 radiens-3.0.0b5/PKG-INFO
--rw-r--r--   0 akelly     (502) staff       (20)      156 2024-02-20 17:19:00.000000 radiens-3.0.0b5/README.md
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.090028 radiens-3.0.0b5/radiens/
--rw-r--r--   0 akelly     (502) staff       (20)      404 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)    17445 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/allego_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.092019 radiens-3.0.0b5/radiens/api/
--rw-r--r--   0 akelly     (502) staff       (20)       10 2024-02-20 17:19:00.000000 radiens-3.0.0b5/radiens/api/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)    24457 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/api/api_allego.py
--rw-r--r--   0 akelly     (502) staff       (20)     4524 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/api/api_curate.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.092841 radiens-3.0.0b5/radiens/api/api_utils/
--rw-r--r--   0 akelly     (502) staff       (20)       19 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/api/api_utils/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)    12256 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/api/api_utils/protocols.py
--rw-r--r--   0 akelly     (502) staff       (20)    11102 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/api/api_utils/util.py
--rw-r--r--   0 akelly     (502) staff       (20)    10359 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/api/api_videre.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.093294 radiens-3.0.0b5/radiens/auth/
--rw-r--r--   0 akelly     (502) staff       (20)       83 2024-02-20 17:19:00.000000 radiens-3.0.0b5/radiens/auth/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     3278 2024-02-20 17:19:00.000000 radiens-3.0.0b5/radiens/auth/interceptors.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.095459 radiens-3.0.0b5/radiens/cli/
--rw-r--r--   0 akelly     (502) staff       (20)       13 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/cli/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     9387 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/allego.py
--rw-r--r--   0 akelly     (502) staff       (20)     7087 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/file_sys.py
--rw-r--r--   0 akelly     (502) staff       (20)     1813 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/main.py
--rw-r--r--   0 akelly     (502) staff       (20)    14132 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/signal_metrics.py
--rw-r--r--   0 akelly     (502) staff       (20)     6012 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/signals.py
--rw-r--r--   0 akelly     (502) staff       (20)     8216 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/spike_sorter.py
--rw-r--r--   0 akelly     (502) staff       (20)     1813 2024-02-28 21:59:51.000000 radiens-3.0.0b5/radiens/cli/sys.py
--rw-r--r--   0 akelly     (502) staff       (20)     5374 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/videre.py
--rw-r--r--   0 akelly     (502) staff       (20)    36686 2024-03-27 16:13:53.000000 radiens-3.0.0b5/radiens/curate_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.096248 radiens-3.0.0b5/radiens/exceptions/
--rw-r--r--   0 akelly     (502) staff       (20)      117 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/exceptions/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     1077 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/exceptions/grpc_error.py
--rw-r--r--   0 akelly     (502) staff       (20)      138 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/exceptions/scan_for_server_error.py
--rw-r--r--   0 akelly     (502) staff       (20)    14239 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/file_sys_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.102212 radiens-3.0.0b5/radiens/grpc_radiens/
--rw-r--r--   0 akelly     (502) staff       (20)       22 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/grpc_radiens/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)    33049 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/allegoserver_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)   159897 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/allegoserver_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    24570 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/biointerface_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/biointerface_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    76713 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/common_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/common_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)     7391 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/datasource_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/datasource_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    13824 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/pybridge_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)    27365 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/pybridge_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)     8740 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/radiens_dev_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/radiens_dev_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    16125 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/radiensserver_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)   174380 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/radiensserver_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    23177 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/spikesorter_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/spikesorter_pb2_grpc.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.104919 radiens-3.0.0b5/radiens/lib/
--rw-r--r--   0 akelly     (502) staff       (20)       13 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/lib/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     6207 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/allego_lib.py
--rw-r--r--   0 akelly     (502) staff       (20)    15292 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/channel_metadata.py
--rw-r--r--   0 akelly     (502) staff       (20)      166 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/corelib.py
--rw-r--r--   0 akelly     (502) staff       (20)    10754 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/dataset_metadata.py
--rw-r--r--   0 akelly     (502) staff       (20)     3660 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/fsys.py
--rw-r--r--   0 akelly     (502) staff       (20)    11891 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/sig_metrics.py
--rw-r--r--   0 akelly     (502) staff       (20)    11225 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/signals_snapshot.py
--rw-r--r--   0 akelly     (502) staff       (20)     7434 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/spike_sorter.py
--rw-r--r--   0 akelly     (502) staff       (20)    10914 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/spikes.py
--rw-r--r--   0 akelly     (502) staff       (20)     7087 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/summa.py
--rw-r--r--   0 akelly     (502) staff       (20)    26625 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/metrics_client.py
--rw-r--r--   0 akelly     (502) staff       (20)     8256 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/signals_client.py
--rw-r--r--   0 akelly     (502) staff       (20)    14790 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/spike_sorter_client.py
--rw-r--r--   0 akelly     (502) staff       (20)     7940 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/spikes_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.106144 radiens-3.0.0b5/radiens/utils/
--rw-r--r--   0 akelly     (502) staff       (20)       14 2024-02-20 17:19:00.000000 radiens-3.0.0b5/radiens/utils/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     6138 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/utils/config.py
--rw-r--r--   0 akelly     (502) staff       (20)     4232 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/utils/constants.py
--rw-r--r--   0 akelly     (502) staff       (20)    17298 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/utils/enums.py
--rw-r--r--   0 akelly     (502) staff       (20)    12166 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/utils/util.py
--rw-r--r--   0 akelly     (502) staff       (20)       24 2024-03-27 16:33:47.000000 radiens-3.0.0b5/radiens/version.py
--rw-r--r--   0 akelly     (502) staff       (20)    13003 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/videre_client.py
--rw-r--r--   0 akelly     (502) staff       (20)     2602 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/workspace_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.090941 radiens-3.0.0b5/radiens.egg-info/
--rw-r--r--   0 akelly     (502) staff       (20)     2518 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/PKG-INFO
--rw-r--r--   0 akelly     (502) staff       (20)     2328 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/SOURCES.txt
--rw-r--r--   0 akelly     (502) staff       (20)        1 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/dependency_links.txt
--rw-r--r--   0 akelly     (502) staff       (20)       49 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/entry_points.txt
--rw-r--r--   0 akelly     (502) staff       (20)       54 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/requires.txt
--rw-r--r--   0 akelly     (502) staff       (20)        8 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/top_level.txt
--rw-r--r--   0 akelly     (502) staff       (20)       38 2024-03-27 16:33:48.108799 radiens-3.0.0b5/setup.cfg
--rw-r--r--   0 akelly     (502) staff       (20)     1294 2024-03-27 15:53:37.000000 radiens-3.0.0b5/setup.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.108014 radiens-3.0.0b5/tests/
--rw-r--r--   0 akelly     (502) staff       (20)      221 2024-02-20 17:19:00.000000 radiens-3.0.0b5/tests/test_Auth.py
--rw-r--r--   0 akelly     (502) staff       (20)     5186 2024-03-27 15:53:37.000000 radiens-3.0.0b5/tests/test_allego_client.py
--rw-r--r--   0 akelly     (502) staff       (20)     3277 2024-02-28 17:36:10.000000 radiens-3.0.0b5/tests/test_base_client.py
--rw-r--r--   0 akelly     (502) staff       (20)      346 2024-02-20 17:19:00.000000 radiens-3.0.0b5/tests/test_config.py
--rw-r--r--   0 akelly     (502) staff       (20)     6114 2024-03-27 15:53:37.000000 radiens-3.0.0b5/tests/test_curate_client.py
--rw-r--r--   0 akelly     (502) staff       (20)     4116 2024-03-27 15:53:37.000000 radiens-3.0.0b5/tests/test_videre_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.686887 radiens-3.0.0b6/
+-rw-r--r--   0 akelly     (502) staff       (20)     1068 2024-04-08 14:50:48.000000 radiens-3.0.0b6/LICENSE
+-rw-r--r--   0 akelly     (502) staff       (20)     2705 2024-04-22 06:20:08.686536 radiens-3.0.0b6/PKG-INFO
+-rw-r--r--   0 akelly     (502) staff       (20)      156 2024-04-08 14:50:48.000000 radiens-3.0.0b6/README.md
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.673883 radiens-3.0.0b6/radiens/
+-rw-r--r--   0 akelly     (502) staff       (20)      404 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    17477 2024-04-22 06:17:45.000000 radiens-3.0.0b6/radiens/allego_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.675381 radiens-3.0.0b6/radiens/api/
+-rw-r--r--   0 akelly     (502) staff       (20)       10 2024-04-08 14:50:48.000000 radiens-3.0.0b6/radiens/api/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    24457 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/api/api_allego.py
+-rw-r--r--   0 akelly     (502) staff       (20)     4524 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/api/api_curate.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.675918 radiens-3.0.0b6/radiens/api/api_utils/
+-rw-r--r--   0 akelly     (502) staff       (20)       19 2024-04-22 04:21:48.000000 radiens-3.0.0b6/radiens/api/api_utils/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    12256 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/api/api_utils/protocols.py
+-rw-r--r--   0 akelly     (502) staff       (20)    11102 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/api/api_utils/util.py
+-rw-r--r--   0 akelly     (502) staff       (20)    10359 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/api/api_videre.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.676232 radiens-3.0.0b6/radiens/auth/
+-rw-r--r--   0 akelly     (502) staff       (20)       83 2024-04-08 14:50:48.000000 radiens-3.0.0b6/radiens/auth/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     3278 2024-04-08 14:50:48.000000 radiens-3.0.0b6/radiens/auth/interceptors.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.677712 radiens-3.0.0b6/radiens/cli/
+-rw-r--r--   0 akelly     (502) staff       (20)       13 2024-04-22 04:21:48.000000 radiens-3.0.0b6/radiens/cli/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     9387 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/cli/allego.py
+-rw-r--r--   0 akelly     (502) staff       (20)     7087 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/cli/file_sys.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1813 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/cli/main.py
+-rw-r--r--   0 akelly     (502) staff       (20)    14132 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/cli/signal_metrics.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6012 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/cli/signals.py
+-rw-r--r--   0 akelly     (502) staff       (20)     8216 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/cli/spike_sorter.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1813 2024-04-22 04:21:48.000000 radiens-3.0.0b6/radiens/cli/sys.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5374 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/cli/videre.py
+-rw-r--r--   0 akelly     (502) staff       (20)    36721 2024-04-22 06:16:55.000000 radiens-3.0.0b6/radiens/curate_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.678208 radiens-3.0.0b6/radiens/exceptions/
+-rw-r--r--   0 akelly     (502) staff       (20)      117 2024-04-22 04:21:48.000000 radiens-3.0.0b6/radiens/exceptions/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1077 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/exceptions/grpc_error.py
+-rw-r--r--   0 akelly     (502) staff       (20)      138 2024-04-22 04:21:48.000000 radiens-3.0.0b6/radiens/exceptions/scan_for_server_error.py
+-rw-r--r--   0 akelly     (502) staff       (20)    14239 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/file_sys_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.681693 radiens-3.0.0b6/radiens/grpc_radiens/
+-rw-r--r--   0 akelly     (502) staff       (20)       22 2024-04-22 04:21:48.000000 radiens-3.0.0b6/radiens/grpc_radiens/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    33177 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/allegoserver_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)   161611 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/allegoserver_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    24328 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/biointerface_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/biointerface_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    76753 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/common_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/common_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)     7391 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/datasource_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/datasource_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    13824 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/pybridge_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)    27365 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/pybridge_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)     8740 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/radiens_dev_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/radiens_dev_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    16355 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/radiensserver_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)   177728 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/radiensserver_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    24175 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/spikesorter_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2024-04-19 17:23:44.000000 radiens-3.0.0b6/radiens/grpc_radiens/spikesorter_pb2_grpc.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.683964 radiens-3.0.0b6/radiens/lib/
+-rw-r--r--   0 akelly     (502) staff       (20)       13 2024-04-22 04:21:48.000000 radiens-3.0.0b6/radiens/lib/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6207 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/lib/allego_lib.py
+-rw-r--r--   0 akelly     (502) staff       (20)    14944 2024-04-22 06:02:51.000000 radiens-3.0.0b6/radiens/lib/channel_metadata.py
+-rw-r--r--   0 akelly     (502) staff       (20)      166 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/lib/corelib.py
+-rw-r--r--   0 akelly     (502) staff       (20)    10802 2024-04-22 05:52:11.000000 radiens-3.0.0b6/radiens/lib/dataset_metadata.py
+-rw-r--r--   0 akelly     (502) staff       (20)     3660 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/lib/fsys.py
+-rw-r--r--   0 akelly     (502) staff       (20)    11891 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/lib/sig_metrics.py
+-rw-r--r--   0 akelly     (502) staff       (20)    11225 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/lib/signals_snapshot.py
+-rw-r--r--   0 akelly     (502) staff       (20)     7434 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/lib/spike_sorter.py
+-rw-r--r--   0 akelly     (502) staff       (20)    10914 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/lib/spikes.py
+-rw-r--r--   0 akelly     (502) staff       (20)     7087 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/lib/summa.py
+-rw-r--r--   0 akelly     (502) staff       (20)    26610 2024-04-22 04:50:16.000000 radiens-3.0.0b6/radiens/metrics_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     8256 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/signals_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)    14790 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/spike_sorter_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     7940 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/spikes_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.684968 radiens-3.0.0b6/radiens/utils/
+-rw-r--r--   0 akelly     (502) staff       (20)       14 2024-04-08 14:50:48.000000 radiens-3.0.0b6/radiens/utils/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6138 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/utils/config.py
+-rw-r--r--   0 akelly     (502) staff       (20)     4354 2024-04-22 06:02:08.000000 radiens-3.0.0b6/radiens/utils/constants.py
+-rw-r--r--   0 akelly     (502) staff       (20)    19075 2024-04-22 05:31:42.000000 radiens-3.0.0b6/radiens/utils/enums.py
+-rw-r--r--   0 akelly     (502) staff       (20)    12166 2024-04-22 06:02:04.000000 radiens-3.0.0b6/radiens/utils/util.py
+-rw-r--r--   0 akelly     (502) staff       (20)       24 2024-04-22 06:20:08.000000 radiens-3.0.0b6/radiens/version.py
+-rw-r--r--   0 akelly     (502) staff       (20)    13035 2024-04-22 06:18:46.000000 radiens-3.0.0b6/radiens/videre_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     2602 2024-04-22 04:24:24.000000 radiens-3.0.0b6/radiens/workspace_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.674750 radiens-3.0.0b6/radiens.egg-info/
+-rw-r--r--   0 akelly     (502) staff       (20)     2705 2024-04-22 06:20:08.000000 radiens-3.0.0b6/radiens.egg-info/PKG-INFO
+-rw-r--r--   0 akelly     (502) staff       (20)     2328 2024-04-22 06:20:08.000000 radiens-3.0.0b6/radiens.egg-info/SOURCES.txt
+-rw-r--r--   0 akelly     (502) staff       (20)        1 2024-04-22 06:20:08.000000 radiens-3.0.0b6/radiens.egg-info/dependency_links.txt
+-rw-r--r--   0 akelly     (502) staff       (20)       49 2024-04-22 06:20:08.000000 radiens-3.0.0b6/radiens.egg-info/entry_points.txt
+-rw-r--r--   0 akelly     (502) staff       (20)       54 2024-04-22 06:20:08.000000 radiens-3.0.0b6/radiens.egg-info/requires.txt
+-rw-r--r--   0 akelly     (502) staff       (20)        8 2024-04-22 06:20:08.000000 radiens-3.0.0b6/radiens.egg-info/top_level.txt
+-rw-r--r--   0 akelly     (502) staff       (20)       38 2024-04-22 06:20:08.686982 radiens-3.0.0b6/setup.cfg
+-rw-r--r--   0 akelly     (502) staff       (20)     1294 2024-04-22 04:24:24.000000 radiens-3.0.0b6/setup.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-04-22 06:20:08.686138 radiens-3.0.0b6/tests/
+-rw-r--r--   0 akelly     (502) staff       (20)      221 2024-04-08 14:50:48.000000 radiens-3.0.0b6/tests/test_Auth.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5186 2024-04-22 04:24:24.000000 radiens-3.0.0b6/tests/test_allego_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     3277 2024-04-22 04:21:48.000000 radiens-3.0.0b6/tests/test_base_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)      346 2024-04-08 14:50:48.000000 radiens-3.0.0b6/tests/test_config.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6114 2024-04-22 04:24:24.000000 radiens-3.0.0b6/tests/test_curate_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     4116 2024-04-22 04:24:24.000000 radiens-3.0.0b6/tests/test_videre_client.py
```

### Comparing `radiens-3.0.0b5/LICENSE` & `radiens-3.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/PKG-INFO` & `radiens-3.0.0b6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radiens
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: provides python API to RADIENS analytics platform
 Home-page: http://neuronexus.github.io
 Author: NeuroNexus
 Author-email: dkipke@neuronexus.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
@@ -29,14 +29,26 @@
 
 # Changelog
 
 All notable changes (for versions > `3.X.X`) to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [3.0.0b6] - 2024-04-22
+
+### Added
+
+- documentation updates
+
+## [3.0.0b5] - 2024-03-27
+
+### Added
+
+- `CurateClient.file_convert()` method for converting between supported file formats
+
 ## [3.0.0b4] - 2024-03-12
 
 ### Added
 
 - `units` attribute on `PSD` class that contains the units of the PSD (as a `string`) per `SignalType`
 - `SignalUnits` enum to represent units of signal data
```

### Comparing `radiens-3.0.0b5/radiens/allego_client.py` & `radiens-3.0.0b6/radiens/allego_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self._workspace = WorkspaceClient()
         self._spikes = SpikesClient(self)
         self._metrics = MetricsClient(self)
 
     @property
     def type(self) -> ClientType:
         """
-        Returns ClientType.ALLEGO
+        Returns :py:attr:`~radiens.utils.enums.ClientType.ALLEGO`
         """
         return ClientType.ALLEGO
 
     def workspace(self) -> WorkspaceClient:
         """
         Allego workspace API
         """
```

### Comparing `radiens-3.0.0b5/radiens/api/api_allego.py` & `radiens-3.0.0b6/radiens/api/api_allego.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/api/api_curate.py` & `radiens-3.0.0b6/radiens/api/api_curate.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/api/api_utils/protocols.py` & `radiens-3.0.0b6/radiens/api/api_utils/protocols.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/api/api_utils/util.py` & `radiens-3.0.0b6/radiens/api/api_utils/util.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/api/api_videre.py` & `radiens-3.0.0b6/radiens/api/api_videre.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/auth/interceptors.py` & `radiens-3.0.0b6/radiens/auth/interceptors.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/cli/allego.py` & `radiens-3.0.0b6/radiens/cli/allego.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/cli/file_sys.py` & `radiens-3.0.0b6/radiens/cli/file_sys.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/cli/main.py` & `radiens-3.0.0b6/radiens/cli/main.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/cli/signal_metrics.py` & `radiens-3.0.0b6/radiens/cli/signal_metrics.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/cli/signals.py` & `radiens-3.0.0b6/radiens/cli/signals.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/cli/spike_sorter.py` & `radiens-3.0.0b6/radiens/cli/spike_sorter.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/cli/sys.py` & `radiens-3.0.0b6/radiens/cli/sys.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/cli/videre.py` & `radiens-3.0.0b6/radiens/cli/videre.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/curate_client.py` & `radiens-3.0.0b6/radiens/curate_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         UID of this client session.
         """
         return self._id()
 
     @property
     def type(self) -> ClientType:
         """
-        Returns ClientType.CURATE
+        Returns :py:attr:`~radiens.utils.enums.ClientType.CURATE`
         """
         return ClientType.CURATE
 
     def signal_metrics(self) -> MetricsClient:
         """
         Signal metrics API
         """
@@ -309,17 +309,17 @@
             This is non-blocking. The requested DSP operation runs in the background.
 
         Example:
             >>> client.dsp_band_pass_filter(750,  2000, './my_source_file', './my_output_file')
             my_stream_id_e4c-jtyn4
 
         See Also:
-            py:meth:`dsp_progress`
-            py:meth:`dsp_progress_bar`
-            py:meth:`dsp_high_pass_filter`
+           :py:meth:`dsp_progress`
+           :py:meth:`dsp_progress_bar`
+           :py:meth:`dsp_high_pass_filter`
         """
         if force:
             rm_xdat_file(Path(target_path))
         protocol = ProtocolAPI('bp_filter')
         protocol.add_node(TransformNode(
             'src_0').datasource_source(Path(source_path)))
         protocol.add_node(TransformNode('filt_bp').bandpass(
@@ -367,17 +367,17 @@
             This is non-blocking. The requested DSP operation runs in the background.
 
         Example:
             >>> client.dsp_band_stop_filter(750,  2000, './my_source_file', './my_output_file')
             my_stream_id_e4c-jtyn4
 
         See Also:
-            py:meth:`dsp_progress`
-            py:meth:`dsp_progress_bar`
-            py:meth:`dsp_high_pass_filter`
+           :py:meth:`dsp_progress`
+           :py:meth:`dsp_progress_bar`
+           :py:meth:`dsp_high_pass_filter`
         """
         if force:
             rm_xdat_file(Path(target_path))
         protocol = ProtocolAPI('bs_filter')
         protocol.add_node(TransformNode(
             'src_0').datasource_source(Path(source_path)))
         protocol.add_node(TransformNode('filt_bs').bandstop(
@@ -424,17 +424,17 @@
             This is non-blocking. The requested DSP operation runs in the background.
 
         Example:
             >>> client.dsp_notch_filter(50,  2, './my_source_file', './my_output_file')
             my_stream_id_e4c-lkqw
 
         See Also:
-            py:meth:`dsp_progress`
-            py:meth:`dsp_progress_bar`
-            py:meth:`dsp_high_pass_filter`
+           :py:meth:`dsp_progress`
+           :py:meth:`dsp_progress_bar`
+           :py:meth:`dsp_high_pass_filter`
         """
         if force:
             rm_xdat_file(Path(target_path))
         protocol = ProtocolAPI('notch_filter')
         protocol.add_node(TransformNode(
             'src_0').datasource_source(Path(source_path)))
         protocol.add_node(TransformNode('filt_notch').notch(freq, bandwidth))
@@ -481,17 +481,17 @@
             This is non-blocking. The requested DSP operation runs in the background.
 
         Example:
             >>> client.dsp_paired_diff(1,  5, './my_source_file', './my_output_file')
             my_stream_id_e4c-rt4m
 
         See Also:
-            py:meth:`dsp_progress`
-            py:meth:`dsp_progress_bar`
-            py:meth:`dsp_high_pass_filter`
+           :py:meth:`dsp_progress`
+           :py:meth:`dsp_progress_bar`
+           :py:meth:`dsp_high_pass_filter`
         """
         if force:
             rm_xdat_file(Path(target_path))
         protocol = ProtocolAPI('paired_diff')
         protocol.add_node(TransformNode(
             'src_0').datasource_source(Path(source_path)))
         protocol.add_node(TransformNode(
@@ -537,17 +537,17 @@
             This is non-blocking. The requested DSP operation runs in the background.
 
         Example:
             >>> client.dsp_virtual_ref(5, './my_source_file', './my_output_file')
             my_stream_id_e4c-wq5c
 
         See Also:
-            py:meth:`dsp_progress`
-            py:meth:`dsp_progress_bar`
-            py:meth:`dsp_high_pass_filter`
+           :py:meth:`dsp_progress`
+           :py:meth:`dsp_progress_bar`
+           :py:meth:`dsp_high_pass_filter`
         """
         if force:
             rm_xdat_file(Path(target_path))
         protocol = ProtocolAPI('virtual_ref')
         protocol.add_node(TransformNode(
             'src_0').datasource_source(Path(source_path)))
         protocol.add_node(TransformNode('vref').virtual_ref(ref_chan))
@@ -585,17 +585,17 @@
             This is non-blocking. The requested DSP operation runs in the background.
 
         Example:
             >>> client.dsp_car('./my_source_file', './my_output_file')
             my_stream_id_e4c-wq5c
 
         See Also:
-            py:meth:`dsp_progress`
-            py:meth:`dsp_progress_bar`
-            py:meth:`dsp_high_pass_filter`
+           :py:meth:`dsp_progress`
+           :py:meth:`dsp_progress_bar`
+           :py:meth:`dsp_high_pass_filter`
         """
         if force:
             rm_xdat_file(Path(target_path))
         protocol = ProtocolAPI('CAR')
         protocol.add_node(TransformNode(
             'src_0').datasource_source(Path(source_path)))
         protocol.add_node(TransformNode('car').car())
@@ -642,17 +642,17 @@
             This is non-blocking. The requested DSP operation runs in the background.
 
         Example:
             >>> client.dsp_time_decimate(3, './my_source_file', './my_output_file')
             my_stream_id_e4c-wq5c
 
         See Also:
-            py:meth:`dsp_progress`
-            py:meth:`dsp_progress_bar`
-            py:meth:`dsp_high_pass_filter`
+           :py:meth:`dsp_progress`
+           :py:meth:`dsp_progress_bar`
+           :py:meth:`dsp_high_pass_filter`
         """
         if force:
             rm_xdat_file(Path(target_path))
         protocol = ProtocolAPI('decimate')
         protocol.add_node(TransformNode(
             'src_0').datasource_source(Path(source_path)))
         protocol.add_node(TransformNode('dec').time_decimate(decimate))
@@ -779,17 +779,17 @@
             This is non-blocking and the requested DSP operation runs in the background.
 
         Example:
             >>> client.dsp_slice_time(0.5, 10, './my_source_file', './my_output_file')
             None
 
         See Also:
-            py:meth:`dsp_progress`
-            py:meth:`dsp_progress_bar`
-            py:meth:`dsp_slice_channels`
+            :py:meth:`dsp_progress`
+            :py:meth:`dsp_progress_bar`
+            :py:meth:`dsp_slice_channels`
         """
         if force:
             rm_xdat_file(Path(target_path))
         protocol = ProtocolAPI('slice_time_0')
         protocol.add_node(TransformNode(
             'src_0').datasource_source(source_path))
         protocol.add_node(TransformNode(
@@ -832,17 +832,17 @@
             This is non-blocking and the requested DSP operation runs in the background.
 
         Example:
             >>> client.dsp_slice_channels([0,2,8,5], './my_source_file', './my_output_file')
             None
 
         See Also:
-            py:meth:`dsp_progress`
-            py:meth:`dsp_progress_bar`
-            py:meth:`dsp_slice_time`
+           :py:meth:`dsp_progress`
+           :py:meth:`dsp_progress_bar`
+           :py:meth:`dsp_slice_time`
         """
         if force:
             rm_xdat_file(Path(target_path))
         protocol = ProtocolAPI('slice_chan_0')
         protocol.add_node(TransformNode(
             'src_0').datasource_source(source_path))
         protocol.add_node(TransformNode(
```

### Comparing `radiens-3.0.0b5/radiens/exceptions/grpc_error.py` & `radiens-3.0.0b6/radiens/exceptions/grpc_error.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/file_sys_client.py` & `radiens-3.0.0b6/radiens/file_sys_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/grpc_radiens/allegoserver_pb2.py` & `radiens-3.0.0b6/radiens/grpc_radiens/allegoserver_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from . import common_pb2 as common__pb2
 from . import datasource_pb2 as datasource__pb2
 from . import biointerface_pb2 as biointerface__pb2
 from . import spikesorter_pb2 as spikesorter__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x61llegoserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\"4\n\x0eRestartRequest\x12\"\n\x04mode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\":\n\x11SetProfileRequest\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0c\n\x04type\x18\x02 \x02(\t\x12\x0b\n\x03\x64ur\x18\x03 \x02(\x02\"\xe9\x02\n\x10LogSystemRequest\x12\x34\n\x04mode\x18\x01 \x02(\x0e\x32&.allego.LogSystemRequest.LogSystemMode\x12=\n\x07outMode\x18\x02 \x01(\x0e\x32,.allego.LogSystemRequest.LogSystemOutputMode\x12\x16\n\x0eoutPathAndFile\x18\x03 \x01(\t\"|\n\rLogSystemMode\x12\n\n\x06\x63onfig\x10\x00\x12\n\n\x06status\x10\x01\x12\x0c\n\x08port_map\x10\x02\x12\n\n\x06pcache\x10\x03\x12\x0c\n\x08sigstats\x10\x04\x12\x11\n\rneurons_stats\x10\x06\x12\x18\n\x14\x62\x61se_signalgroup_map\x10\x07\"J\n\x13LogSystemOutputMode\x12\x12\n\x0eLOG_OUT_STDERR\x10\x00\x12\x0f\n\x0bLOG_OUT_CSV\x10\x01\x12\x0e\n\nLOG_OUT_MD\x10\x02\"4\n\x10SetStreamRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\"P\n\x10SetRecordRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x1a\n\x04port\x18\x02 \x01(\x0e\x32\x0c.allego.Port\"~\n\x14SetConfigCoreRequest\x12\x10\n\x08sampFreq\x18\x01 \x01(\x01\x12\x0f\n\x07loopDur\x18\x02 \x01(\x01\x12\x19\n\x11pcachePersistence\x18\x03 \x01(\x01\x12(\n\x0b\x63\x61\x62leLength\x18\x04 \x01(\x0b\x32\x13.allego.CableLength\">\n\x0b\x43\x61\x62leLength\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x13\n\x0b\x63\x61\x62leLength\x18\x02 \x02(\x01\"f\n\x0c\x43\x61\x62leLengths\x12\t\n\x01\x41\x18\x01 \x02(\x01\x12\t\n\x01\x42\x18\x02 \x02(\x01\x12\t\n\x01\x43\x18\x03 \x02(\x01\x12\t\n\x01\x44\x18\x04 \x02(\x01\x12\t\n\x01\x45\x18\x05 \x02(\x01\x12\t\n\x01\x46\x18\x06 \x02(\x01\x12\t\n\x01G\x18\x07 \x02(\x01\x12\t\n\x01H\x18\x08 \x02(\x01\"\xb1\x01\n\nConfigCore\x12\x1c\n\x14\x61llegoCoreServerPort\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seSampFreq\x18\x03 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x04 \x02(\x05\x12*\n\x0c\x63\x61\x62leLengths\x18\x05 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x06 \x02(\x0e\x32\x14.allego.BackboneMode\"\xda\x03\n\x0fRecordingStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x16\n\x0e\x61\x63tiveFileName\x18\x02 \x02(\t\x12\x10\n\x08\x64uration\x18\x03 \x02(\x01\x12\r\n\x05\x65rror\x18\x04 \x02(\t\x12+\n\x0frecordModePortA\x18\x05 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortB\x18\x06 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortC\x18\x07 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortD\x18\x08 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortE\x18\t \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortF\x18\n \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortG\x18\x0b \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortH\x18\x0c \x01(\x0e\x32\x12.allego.RecordMode\"r\n\x0fStreamingStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x1a\n\x12primaryCacheTRange\x18\x02 \x03(\x01\x12\x1b\n\x13hardwareMemoryLevel\x18\x03 \x02(\x01\"\xda\x01\n\x0e\x42\x61\x63kboneStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\"\xc9\x02\n\x0f\x43onfigAndStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\x12\x14\n\x0c\x62\x61seSampFreq\x18\x06 \x02(\x01\x12*\n\x0c\x63\x61\x62leLengths\x18\x07 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x08 \x02(\x0e\x32\x14.allego.BackboneMode\"\x9e\x01\n\x0f\x43onfigRecording\x12\x14\n\x0c\x62\x61seFileName\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seFilePath\x18\x02 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x03 \x01(\x05\x12\x11\n\ttimeStamp\x18\x04 \x01(\x08\x12\x18\n\x10splitFilesByPort\x18\x05 \x01(\x08\x12\x1b\n\x13\x66orceStartAtTStamp0\x18\x06 \x01(\x08\"V\n\x14\x44IOModeEventsRequest\x12\x0f\n\x07\x63hanIdx\x18\x02 \x02(\x05\x12\x16\n\x0e\x65ventThreshold\x18\x03 \x02(\x01\x12\x15\n\reventPolarity\x18\x04 \x02(\x08\"6\n\x14\x44IOModeManualRequest\x12\x0f\n\x07\x63hanIdx\x18\x01 \x02(\x05\x12\r\n\x05state\x18\x02 \x02(\x08\"s\n\x19\x44igitalOutChannelRegister\x12\x13\n\x0bmanualState\x18\x01 \x02(\x08\x12\x16\n\x0e\x65ventThreshold\x18\x02 \x02(\x01\x12\x15\n\reventPolarity\x18\x03 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x05\"q\n\x12\x44igitalOutRegister\x12\x1d\n\x04mode\x18\x01 \x02(\x0e\x32\x0f.allego.DIOMode\x12<\n\x11\x64outChanRegisters\x18\x02 \x03(\x0b\x32!.allego.DigitalOutChannelRegister\"\x1e\n\x0e\x44\x41\x43GainRequest\x12\x0c\n\x04gain\x18\x01 \x02(\x05\"9\n\x13\x44\x41\x43HighPassRegister\x12\x0e\n\x06\x65nable\x18\x01 \x02(\x08\x12\x12\n\ncutoffFreq\x18\x02 \x02(\x01\"w\n\x18\x41nalogOutChannelRegister\x12\x15\n\rPriNtvChanIdx\x18\x01 \x02(\x05\x12\x1b\n\x13\x41nalogOutNtvChanIdx\x18\x02 \x02(\x05\x12\x0e\n\x06Stream\x18\x03 \x02(\x05\x12\x17\n\x0fStreamOffsetIdx\x18\x04 \x02(\x05\"\x90\x01\n\x11\x41nalogOutRegister\x12;\n\x11\x61nalogOutChannels\x18\x01 \x03(\x0b\x32 .allego.AnalogOutChannelRegister\x12\x0c\n\x04gain\x18\x02 \x02(\x05\x12\x30\n\x0bhighpassReg\x18\x03 \x02(\x0b\x32\x1b.allego.DACHighPassRegister\"!\n\x0cSerialNumber\x12\x11\n\tserialNum\x18\x01 \x02(\t\"\x81\x01\n\x12SetSimPortsRequest\x12\x33\n\x07simPort\x18\x01 \x03(\x0b\x32\".allego.SetSimPortsRequest.SimPort\x1a\x36\n\x07SimPort\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07numChan\x18\x02 \x02(\x03\"4\n\x19SetHasGPIOExpanderRequest\x12\x17\n\x0fhasGPIOExpander\x18\x01 \x02(\x08\"\'\n\x14SetMuxChannelRequest\x12\x0f\n\x07\x63hannel\x18\x01 \x02(\x03\"\'\n\x14SetPotVoltageRequest\x12\x0f\n\x07voltage\x18\x01 \x02(\x02\"!\n\x10GetADCLevelReply\x12\r\n\x05level\x18\x01 \x02(\x02\"#\n\x12SetPotRangeRequest\x12\r\n\x05range\x18\x01 \x02(\x05\"!\n\x11SetPotModeRequest\x12\x0c\n\x04mode\x18\x01 \x02(\x08\")\n\x17SetPotCellEnableRequest\x12\x0e\n\x06\x65nable\x18\x01 \x02(\x08\",\n\x12ReadWireOutRequest\x12\x16\n\x0ewireOutAddress\x18\x01 \x02(\x03\"(\n\x10ReadWireOutReply\x12\x14\n\x0cwireOutValue\x18\x01 \x02(\x03\"\xc7\x02\n\x11LogsysConfigReply\x12(\n\nsystemMode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x03 \x02(\x05\x12\x1a\n\x12priCachePersistDur\x18\x04 \x02(\x01\x12!\n\x19priCacheStatsUpdatePeriod\x18\x05 \x02(\x01\x12\x12\n\nactiveSigs\x18\x06 \x02(\x05\x12\x10\n\x08priChans\x18\x07 \x02(\x05\x12\x10\n\x08\x61uxChans\x18\x08 \x02(\x05\x12\x10\n\x08\x64inChans\x18\t \x02(\x05\x12\x11\n\tdoutChans\x18\n \x02(\x05\x12\"\n\x08portSpec\x18\x0b \x03(\x0b\x32\x10.allego.PortInfo\x12\x19\n\x11numConnectedPorts\x18\x0c \x02(\x05\"Y\n\x08PortInfo\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\r\n\x05probe\x18\x02 \x02(\t\x12\x11\n\theadstage\x18\x03 \x02(\t\x12\x0f\n\x07numSigs\x18\x04 \x02(\x05\"c\n\x11LogsysStatusReply\x12\'\n\x07recStat\x18\x01 \x02(\x0b\x32\x16.allego.RecorderStatus\x12%\n\x07sysStat\x18\x02 \x02(\x0b\x32\x14.allego.SystemStatus\"\xba\x01\n\x0eRecorderStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x10\n\x08\x64uration\x18\x02 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\x03 \x02(\x01\x12\x11\n\tsizeBytes\x18\x04 \x02(\x05\x12\x0c\n\x04path\x18\x05 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x06 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x07 \x02(\x05\x12\x16\n\x0e\x61\x63tiveFileName\x18\x08 \x02(\t\"\x96\x03\n\x0cSystemStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x12\n\nnumPriSigs\x18\x03 \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x04 \x02(\x05\x12\x12\n\nnumDinSigs\x18\x05 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x06 \x02(\x05\x12\x13\n\x0btStampRange\x18\x07 \x03(\x03\x12\x0e\n\x06tRange\x18\x08 \x03(\x01\x12\x11\n\tstreamDur\x18\t \x02(\x01\x12\x14\n\x0cmeanChunkDur\x18\n \x02(\x01\x12\x1c\n\x14meanHardwareMemLevel\x18\x0b \x02(\x02\x12\x1b\n\x13maxHardwareMemLevel\x18\x0c \x02(\x02\x12\x1b\n\x13minHardwareMemLevel\x18\r \x02(\x02\x12\x1c\n\x14lastHardwareMemLevel\x18\x0e \x02(\x02\x12\x19\n\x11meanStreamLoopDur\x18\x0f \x02(\x01\x12\x18\n\x10streamEfficiency\x18\x10 \x02(\x01\"\xd8\x02\n\x11LogsysPcacheReply\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x18\n\x10minNumDatablocks\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x03\x12 \n\x18totalDatablocksProcessed\x18\x06 \x02(\x04\x12\x16\n\x0enumTimeSamples\x18\x07 \x02(\x03\x12\x1f\n\x17\x61llTimeMeanDatablockDur\x18\x08 \x02(\x01\x12\x15\n\rnumDataBlocks\x18\t \x02(\x05\x12\x0e\n\x06tRange\x18\n \x03(\x01\x12\x0f\n\x07tsRange\x18\x0b \x03(\x03\x12\x12\n\nnumPriSigs\x18\x0c \x02(\x05\x12\x12\n\nnumAuxSigs\x18\r \x02(\x05\x12\x12\n\nnumDinSigs\x18\x0e \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x0f \x02(\x05\"i\n\x11SetTriggerRequest\x12\'\n\x07\x63hannel\x18\x01 \x02(\x0e\x32\x16.allego.TriggerChannel\x12\x0f\n\x07\x65nabled\x18\x02 \x02(\x08\x12\x1a\n\x04port\x18\x03 \x01(\x0e\x32\x0c.allego.Port\"\\\n\x0cTriggerState\x12/\n\x0f\x65nabledChannels\x18\x01 \x03(\x0e\x32\x16.allego.TriggerChannel\x12\x1b\n\x05ports\x18\x02 \x03(\x0e\x32\x0c.allego.Port\"*\n\x12LoadAllMosiRequest\x12\x14\n\x0cregisterVals\x18\x01 \x03(\x05\"\x15\n\x13TransmitMosiRequest\"5\n\x0f\x44umpMisoRequest\x12\x10\n\x08nSamples\x18\x01 \x02(\x05\x12\x10\n\x08\x66ileName\x18\x02 \x02(\t\"\xc6\x03\n\x15SinapsStatusRegisters\x12\x18\n\x10\x63\x61librationState\x18\x01 \x02(\x08\x12\x1b\n\x13\x63\x61librationProgress\x18\x02 \x02(\x01\x12\x1d\n\x15numActivePixelsShank0\x18\x03 \x02(\x05\x12\x1d\n\x15numActivePixelsShank1\x18\x04 \x02(\x05\x12\x1d\n\x15numActivePixelsShank2\x18\x05 \x02(\x05\x12\x1d\n\x15numActivePixelsShank3\x18\x06 \x02(\x05\x12\x0f\n\x07vRefFFA\x18\x07 \x02(\x01\x12\x0f\n\x07vRefFFB\x18\x08 \x02(\x01\x12\x0f\n\x07vRefFFC\x18\t \x02(\x01\x12\x0f\n\x07vRefFFD\x18\n \x02(\x01\x12\x10\n\x08isError0\x18\x0b \x02(\x08\x12\x10\n\x08isError1\x18\x0c \x02(\x08\x12\x10\n\x08isError2\x18\r \x02(\x08\x12\x10\n\x08isError3\x18\x0e \x02(\x08\x12\x13\n\x0bhostCounter\x18\x0f \x02(\x05\x12\x13\n\x0b\x66pgaCounter\x18\x10 \x02(\x05\x12\x17\n\x0f\x66irmwareVersion\x18\x11 \x02(\t\x12\x17\n\x0fprobeGeneration\x18\x12 \x02(\x05\x12\x12\n\nprobeModel\x18\x13 \x02(\x05\"%\n\x12\x46lashSinapsRequest\x12\x0f\n\x07\x62itfile\x18\x01 \x02(\t\"3\n\x0cHALdashboard\x12#\n\x04mode\x18\x01 \x02(\x0e\x32\x15.allego.AllegoHALmode\"\xbc\x06\n\nStimParams\x12$\n\tstimShape\x18\x01 \x02(\x0e\x32\x11.allego.StimShape\x12*\n\x0cstimPolarity\x18\x02 \x02(\x0e\x32\x14.allego.StimPolarity\x12\x1a\n\x12\x66irstPhaseDuration\x18\x03 \x02(\x01\x12\x1b\n\x13secondPhaseDuration\x18\x04 \x02(\x01\x12\x17\n\x0finterphaseDelay\x18\x05 \x02(\x01\x12\x1b\n\x13\x66irstPhaseAmplitude\x18\x06 \x02(\x01\x12\x1c\n\x14secondPhaseAmplitude\x18\x07 \x02(\x01\x12\x17\n\x0f\x62\x61selineVoltage\x18\x08 \x02(\x01\x12:\n\x12triggerEdgeOrLevel\x18\n \x02(\x0e\x32\x1e.allego.StimTriggerEdgeOrLevel\x12\x36\n\x10triggerHighOrLow\x18\x0b \x02(\x0e\x32\x1c.allego.StimTriggerHighOrLow\x12\x0f\n\x07\x65nabled\x18\x0c \x02(\x08\x12\x18\n\x10postTriggerDelay\x18\r \x02(\x01\x12.\n\x0cpulseOrTrain\x18\x0e \x02(\x0e\x32\x18.allego.StimPulseOrTrain\x12\x1a\n\x12numberOfStimPulses\x18\x0f \x02(\x05\x12\x18\n\x10pulseTrainPeriod\x18\x10 \x02(\x01\x12\x18\n\x10refractoryPeriod\x18\x11 \x02(\x01\x12\x18\n\x10preStimAmpSettle\x18\x12 \x02(\x01\x12\x19\n\x11postStimAmpSettle\x18\x13 \x02(\x01\x12\x19\n\x11maintainAmpSettle\x18\x14 \x02(\x08\x12\x17\n\x0f\x65nableAmpSettle\x18\x15 \x02(\x08\x12\x1d\n\x15postStimChargeRecovOn\x18\x16 \x02(\x01\x12\x1e\n\x16postStimChargeRecovOff\x18\x17 \x02(\x01\x12\x1c\n\x14\x65nableChargeRecovery\x18\x18 \x02(\x08\x12\x1f\n\x17triggerSourceIsKeypress\x18\x19 \x02(\x08\x12\x18\n\x10triggerSourceIdx\x18\x1a \x02(\x05\x12\x16\n\x0estimSysChanIdx\x18\x1b \x02(\x05\"\x89\x01\n\x0fStimParamsReply\x12\x33\n\x06params\x18\x01 \x03(\x0b\x32#.allego.StimParamsReply.ParamsEntry\x1a\x41\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.allego.StimParams:\x02\x38\x01\">\n\x18ManualStimTriggerRequest\x12\x0f\n\x07trigger\x18\x01 \x02(\x05\x12\x11\n\ttriggerOn\x18\x02 \x02(\x08\"1\n\x1eManualStimTriggerToggleRequest\x12\x0f\n\x07trigger\x18\x01 \x02(\x05\"5\n\x0fStimStepMessage\x12\"\n\x08stimStep\x18\x01 \x02(\x0e\x32\x10.allego.StimStep*!\n\nStreamMode\x12\t\n\x05S_OFF\x10\x00\x12\x08\n\x04S_ON\x10\x01*!\n\nRecordMode\x12\t\n\x05R_OFF\x10\x00\x12\x08\n\x04R_ON\x10\x01*\x9f\x04\n\x0c\x42\x61\x63kboneMode\x12\x10\n\x0cSMARTBOX_PRO\x10\x00\x12\x19\n\x15SMARTBOX_SIM_GEN_SINE\x10\x01\x12\x1b\n\x17SMARTBOX_SIM_GEN_SPIKES\x10\x02\x12\x1b\n\x17SMARTBOX_SIM_DATASOURCE\x10\x03\x12\x13\n\x0fOPEN_EPHYS_USB3\x10\x04\x12#\n\x1fINTAN_RECORDING_CONTROLLER_1024\x10\x05\x12\x14\n\x10SMARTBOX_CLASSIC\x10\x06\x12\"\n\x1eINTAN_RECORDING_CONTROLLER_512\x10\x07\x12\x13\n\x0fOPEN_EPHYS_USB2\x10\x08\x12\x0e\n\nINTAN_USB2\x10\t\x12 \n\x1cSMARTBOX_SIM_GEN_SINE_MAPPED\x10\n\x12#\n\x1fSMARTBOX_SIM_GEN_SINE_HIGH_FREQ\x10\x0b\x12$\n SMARTBOX_SIM_GEN_SINE_MULTI_BAND\x10\x0c\x12\x1b\n\x17SMARTBOX_PRO_SINAPS_256\x10\r\x12\x1c\n\x18SMARTBOX_PRO_SINAPS_1024\x10\x0e\x12\x10\n\x0cXDAQ_ONE_REC\x10\x0f\x12\x11\n\rXDAQ_ONE_STIM\x10\x10\x12\x11\n\rXDAQ_CORE_REC\x10\x11\x12\x12\n\x0eXDAQ_CORE_STIM\x10\x12\x12\x1b\n\x17SMARTBOX_PRO_SINAPS_512\x10\x13*,\n\x07\x44IOMode\x12\n\n\x06manual\x10\x00\x12\n\n\x06\x65vents\x10\x01\x12\t\n\x05gated\x10\x02*\xf4\x01\n\x0eTriggerChannel\x12\x0b\n\x07T_DIN_0\x10\x00\x12\x0b\n\x07T_DIN_1\x10\x01\x12\x0b\n\x07T_DIN_2\x10\x02\x12\x0b\n\x07T_DIN_3\x10\x03\x12\x0b\n\x07T_DIN_4\x10\x04\x12\x0b\n\x07T_DIN_5\x10\x05\x12\x0b\n\x07T_DIN_6\x10\x06\x12\x0b\n\x07T_DIN_7\x10\x07\x12\x0c\n\x08T_DOUT_0\x10\x08\x12\x0c\n\x08T_DOUT_1\x10\t\x12\x0c\n\x08T_DOUT_2\x10\n\x12\x0c\n\x08T_DOUT_3\x10\x0b\x12\x0c\n\x08T_DOUT_4\x10\x0c\x12\x0c\n\x08T_DOUT_5\x10\r\x12\x0c\n\x08T_DOUT_6\x10\x0e\x12\x0c\n\x08T_DOUT_7\x10\x0f\x12\n\n\x06T_NONE\x10\x10*q\n\rAllegoHALmode\x12\x11\n\rA_HAL_GENERIC\x10\x00\x12\x13\n\x0f\x41_HAL_SPIKESORT\x10\x01\x12\x14\n\x10\x41_HAL_MULTISCALE\x10\x02\x12\"\n\x1e\x41_HAL_MULTISCALE_BIDIRECTIONAL\x10\x03*W\n\tStimShape\x12\x0c\n\x08\x42IPHASIC\x10\x00\x12\x1d\n\x19\x42IPHASIC_INTERPHASE_DELAY\x10\x01\x12\r\n\tTRIPHASIC\x10\x02\x12\x0e\n\nMONOPHASIC\x10\x03*4\n\x0cStimPolarity\x12\x12\n\x0e\x43\x41THODIC_FIRST\x10\x00\x12\x10\n\x0c\x41NODIC_FIRST\x10\x01*3\n\x16StimTriggerEdgeOrLevel\x12\x0b\n\x07ST_EDGE\x10\x00\x12\x0c\n\x08ST_LEVEL\x10\x01*/\n\x14StimTriggerHighOrLow\x12\x0b\n\x07ST_HIGH\x10\x00\x12\n\n\x06ST_LOW\x10\x01*5\n\x10StimPulseOrTrain\x12\x10\n\x0cSINGLE_PULSE\x10\x00\x12\x0f\n\x0bPULSE_TRAIN\x10\x01*\x90\x02\n\x08StimStep\x12\x13\n\x0fStimStepSizeMin\x10\x00\x12\x14\n\x10StimStepSize10nA\x10\x01\x12\x14\n\x10StimStepSize20nA\x10\x02\x12\x14\n\x10StimStepSize50nA\x10\x03\x12\x15\n\x11StimStepSize100nA\x10\x04\x12\x15\n\x11StimStepSize200nA\x10\x05\x12\x15\n\x11StimStepSize500nA\x10\x06\x12\x13\n\x0fStimStepSize1uA\x10\x07\x12\x13\n\x0fStimStepSize2uA\x10\x08\x12\x13\n\x0fStimStepSize5uA\x10\t\x12\x14\n\x10StimStepSize10uA\x10\n\x12\x13\n\x0fStimStepSizeMax\x10\x0b\x32\xbd*\n\nAllegoCore\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\x07Restart\x12\x16.allego.RestartRequest\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12j\n\x1bGetStatusPollFieldsToUpdate\x12\'.allego.StatusPollFieldsToUpdateRequest\x1a .allego.StatusPollFieldsToUpdate\"\x00\x12R\n\x17GetOfflineLicenseStatus\x12\x17.allego.StandardRequest\x1a\x1c.allego.OfflineLicenseStatus\"\x00\x12\x46\n\rSetConfigCore\x12\x1c.allego.SetConfigCoreRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0fSetProfileState\x12\x19.allego.SetProfileRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x12SetConfigRecording\x12\x17.allego.ConfigRecording\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetStreamState\x12\x18.allego.SetStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetRecordState\x12\x18.allego.SetRecordRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOEvents\x12\x1c.allego.DIOModeEventsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOManual\x12\x1c.allego.DIOModeManualRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bSetDIOGated\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nSetDACGain\x12\x16.allego.DACGainRequest\x1a\x15.allego.StandardReply\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x0eSetDACHighPass\x12\x1b.allego.DACHighPassRegister\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetSimPorts\x12\x1a.allego.SetSimPortsRequest\x1a\x15.allego.StandardReply\"\x00\x12P\n\x12SetHasGPIOExpander\x12!.allego.SetHasGPIOExpanderRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetMuxChannel\x12\x1c.allego.SetMuxChannelRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0fSetTriggerState\x12\x19.allego.SetTriggerRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetPotVoltage\x12\x1c.allego.SetPotVoltageRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetPotRange\x12\x1a.allego.SetPotRangeRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\nSetPotMode\x12\x19.allego.SetPotModeRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10SetPotCellEnable\x12\x1f.allego.SetPotCellEnableRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\rSetStimParams\x12\x12.allego.StimParams\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\rGetStimParams\x12\x17.allego.StandardRequest\x1a\x17.allego.StimParamsReply\"\x00\x12?\n\x0bSetStimStep\x12\x17.allego.StimStepMessage\x1a\x15.allego.StandardReply\"\x00\x12\x41\n\x0bGetStimStep\x12\x17.allego.StandardRequest\x1a\x17.allego.StimStepMessage\"\x00\x12N\n\x11ManualStimTrigger\x12 .allego.ManualStimTriggerRequest\x1a\x15.allego.StandardReply\"\x00\x12Z\n\x17ManualStimTriggerToggle\x12&.allego.ManualStimTriggerToggleRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\tGetConfig\x12\x17.allego.StandardRequest\x1a\x12.allego.ConfigCore\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12H\n\x12GetConfigRecording\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigRecording\"\x00\x12>\n\tGetStatus\x12\x17.allego.StandardRequest\x1a\x16.allego.BackboneStatus\"\x00\x12H\n\x12GetConfigAndStatus\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigAndStatus\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12\x42\n\x11GetIntanImpedance\x12\x18.allego.ImpedanceRequest\x1a\x11.allego.Impedance\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12\x42\n\tGetDIOReg\x12\x17.allego.StandardRequest\x1a\x1a.allego.DigitalOutRegister\"\x00\x12\x41\n\tGetDACReg\x12\x17.allego.StandardRequest\x1a\x19.allego.AnalogOutRegister\"\x00\x12<\n\tGetSerial\x12\x17.allego.StandardRequest\x1a\x14.allego.SerialNumber\"\x00\x12\x42\n\x0fGetTriggerState\x12\x17.allego.StandardRequest\x1a\x14.allego.TriggerState\"\x00\x12\x42\n\x0bGetADCLevel\x12\x17.allego.StandardRequest\x1a\x18.allego.GetADCLevelReply\"\x00\x12\x45\n\x0bReadWireOut\x12\x1a.allego.ReadWireOutRequest\x1a\x18.allego.ReadWireOutReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12H\n\x0eGetSorterIDMap\x12\x17.allego.StandardRequest\x1a\x1b.allego.GetSorterIDMapReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tScanPorts\x12\x17.allego.StandardRequest\x1a\x13.allego.SignalGroup\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12O\n\x13GetDataSourceStatus\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceStatus\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bLoadAllMosi\x12\x1a.allego.LoadAllMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x0cTransmitMosi\x12\x1b.allego.TransmitMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\x08\x44umpMiso\x12\x17.allego.DumpMisoRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x18GetSinapsStatusRegisters\x12\x17.allego.StandardRequest\x1a\x1d.allego.SinapsStatusRegisters\"\x00\x12\x42\n\x0b\x46lashSinaps\x12\x1a.allego.FlashSinapsRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x16GetOrCreateEventViewer\x12\x15.allego.EventViewerID\x1a\x19.allego.EventViewerConfig\"\x00\x12G\n\x11UpdateEventViewer\x12\x19.allego.EventViewerConfig\x1a\x15.allego.StandardReply\"\x00\x12T\n\x15ListEventViewerEvents\x12\x15.allego.EventViewerID\x1a\".allego.ListEventViewerEventsReply\"\x00\x12U\n\x13GetEventViewerEvent\x12\".allego.GetEventViewerEventRequest\x1a\x18.allego.EventViewerEvent\"\x00\x12L\n\x10ListEventViewers\x12\x17.allego.StandardRequest\x1a\x1d.allego.ListEventViewersReply\"\x00\x12\x42\n\x0fGetHALdashboard\x12\x17.allego.StandardRequest\x1a\x14.allego.HALdashboard\"\x00\x32\xe4\x02\n\x07Pcache1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12J\n\x15GetHDSnapshotFromHead\x12\x1a.allego.HDSnapshotRequest2\x1a\x13.allego.HDSnapshot2\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12K\n\x12SetTimeRangeToHead\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x32\x8d\x04\n\x04Kpi1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x12K\n\x0bSetKpiParam\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x0bGetKpiParam\x12\x19.allego.DataSourceRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12I\n\x12SetKpiUpdatePeriod\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x0fSetKpiPacketDur\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x32\xa3\n\n\x08Neurons1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SpikeSorterSetParams\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x63\n\x17SpikeSorterGetDashboard\x12#.allego.SpikeSorterDashboardRequest\x1a!.allego.SpikeSorterDashboardReply\"\x00\x12i\n\x18SpikeSorterGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12\x61\n\x1a\x42iointerfaceGetSpikesDense\x12\x1e.allego.SpikesGetSpikesRequest\x1a!.allego.SpikesSpikeDataDenseReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12l\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x11.allego.TimeRange\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x12q\n\x15GetSpikeTrainAnalytic\x12+.allego.SpikesGetSpikeTrainAnalyticsRequest\x1a).allego.SpikesGetSpikeTrainAnalyticsReply\"\x00\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x61llegoserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\"4\n\x0eRestartRequest\x12\"\n\x04mode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\":\n\x11SetProfileRequest\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0c\n\x04type\x18\x02 \x02(\t\x12\x0b\n\x03\x64ur\x18\x03 \x02(\x02\"\xe9\x02\n\x10LogSystemRequest\x12\x34\n\x04mode\x18\x01 \x02(\x0e\x32&.allego.LogSystemRequest.LogSystemMode\x12=\n\x07outMode\x18\x02 \x01(\x0e\x32,.allego.LogSystemRequest.LogSystemOutputMode\x12\x16\n\x0eoutPathAndFile\x18\x03 \x01(\t\"|\n\rLogSystemMode\x12\n\n\x06\x63onfig\x10\x00\x12\n\n\x06status\x10\x01\x12\x0c\n\x08port_map\x10\x02\x12\n\n\x06pcache\x10\x03\x12\x0c\n\x08sigstats\x10\x04\x12\x11\n\rneurons_stats\x10\x06\x12\x18\n\x14\x62\x61se_signalgroup_map\x10\x07\"J\n\x13LogSystemOutputMode\x12\x12\n\x0eLOG_OUT_STDERR\x10\x00\x12\x0f\n\x0bLOG_OUT_CSV\x10\x01\x12\x0e\n\nLOG_OUT_MD\x10\x02\"4\n\x10SetStreamRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\"P\n\x10SetRecordRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x1a\n\x04port\x18\x02 \x01(\x0e\x32\x0c.allego.Port\"~\n\x14SetConfigCoreRequest\x12\x10\n\x08sampFreq\x18\x01 \x01(\x01\x12\x0f\n\x07loopDur\x18\x02 \x01(\x01\x12\x19\n\x11pcachePersistence\x18\x03 \x01(\x01\x12(\n\x0b\x63\x61\x62leLength\x18\x04 \x01(\x0b\x32\x13.allego.CableLength\">\n\x0b\x43\x61\x62leLength\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x13\n\x0b\x63\x61\x62leLength\x18\x02 \x02(\x01\"f\n\x0c\x43\x61\x62leLengths\x12\t\n\x01\x41\x18\x01 \x02(\x01\x12\t\n\x01\x42\x18\x02 \x02(\x01\x12\t\n\x01\x43\x18\x03 \x02(\x01\x12\t\n\x01\x44\x18\x04 \x02(\x01\x12\t\n\x01\x45\x18\x05 \x02(\x01\x12\t\n\x01\x46\x18\x06 \x02(\x01\x12\t\n\x01G\x18\x07 \x02(\x01\x12\t\n\x01H\x18\x08 \x02(\x01\"\xb1\x01\n\nConfigCore\x12\x1c\n\x14\x61llegoCoreServerPort\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seSampFreq\x18\x03 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x04 \x02(\x05\x12*\n\x0c\x63\x61\x62leLengths\x18\x05 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x06 \x02(\x0e\x32\x14.allego.BackboneMode\"\xda\x03\n\x0fRecordingStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x16\n\x0e\x61\x63tiveFileName\x18\x02 \x02(\t\x12\x10\n\x08\x64uration\x18\x03 \x02(\x01\x12\r\n\x05\x65rror\x18\x04 \x02(\t\x12+\n\x0frecordModePortA\x18\x05 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortB\x18\x06 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortC\x18\x07 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortD\x18\x08 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortE\x18\t \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortF\x18\n \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortG\x18\x0b \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortH\x18\x0c \x01(\x0e\x32\x12.allego.RecordMode\"r\n\x0fStreamingStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x1a\n\x12primaryCacheTRange\x18\x02 \x03(\x01\x12\x1b\n\x13hardwareMemoryLevel\x18\x03 \x02(\x01\"\xda\x01\n\x0e\x42\x61\x63kboneStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\"\xc9\x02\n\x0f\x43onfigAndStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\x12\x14\n\x0c\x62\x61seSampFreq\x18\x06 \x02(\x01\x12*\n\x0c\x63\x61\x62leLengths\x18\x07 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x08 \x02(\x0e\x32\x14.allego.BackboneMode\"\x9e\x01\n\x0f\x43onfigRecording\x12\x14\n\x0c\x62\x61seFileName\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seFilePath\x18\x02 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x03 \x01(\x05\x12\x11\n\ttimeStamp\x18\x04 \x01(\x08\x12\x18\n\x10splitFilesByPort\x18\x05 \x01(\x08\x12\x1b\n\x13\x66orceStartAtTStamp0\x18\x06 \x01(\x08\"V\n\x14\x44IOModeEventsRequest\x12\x0f\n\x07\x63hanIdx\x18\x02 \x02(\x05\x12\x16\n\x0e\x65ventThreshold\x18\x03 \x02(\x01\x12\x15\n\reventPolarity\x18\x04 \x02(\x08\"6\n\x14\x44IOModeManualRequest\x12\x0f\n\x07\x63hanIdx\x18\x01 \x02(\x05\x12\r\n\x05state\x18\x02 \x02(\x08\"s\n\x19\x44igitalOutChannelRegister\x12\x13\n\x0bmanualState\x18\x01 \x02(\x08\x12\x16\n\x0e\x65ventThreshold\x18\x02 \x02(\x01\x12\x15\n\reventPolarity\x18\x03 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x05\"q\n\x12\x44igitalOutRegister\x12\x1d\n\x04mode\x18\x01 \x02(\x0e\x32\x0f.allego.DIOMode\x12<\n\x11\x64outChanRegisters\x18\x02 \x03(\x0b\x32!.allego.DigitalOutChannelRegister\"\x1e\n\x0e\x44\x41\x43GainRequest\x12\x0c\n\x04gain\x18\x01 \x02(\x05\"9\n\x13\x44\x41\x43HighPassRegister\x12\x0e\n\x06\x65nable\x18\x01 \x02(\x08\x12\x12\n\ncutoffFreq\x18\x02 \x02(\x01\"w\n\x18\x41nalogOutChannelRegister\x12\x15\n\rPriNtvChanIdx\x18\x01 \x02(\x05\x12\x1b\n\x13\x41nalogOutNtvChanIdx\x18\x02 \x02(\x05\x12\x0e\n\x06Stream\x18\x03 \x02(\x05\x12\x17\n\x0fStreamOffsetIdx\x18\x04 \x02(\x05\"\x90\x01\n\x11\x41nalogOutRegister\x12;\n\x11\x61nalogOutChannels\x18\x01 \x03(\x0b\x32 .allego.AnalogOutChannelRegister\x12\x0c\n\x04gain\x18\x02 \x02(\x05\x12\x30\n\x0bhighpassReg\x18\x03 \x02(\x0b\x32\x1b.allego.DACHighPassRegister\"!\n\x0cSerialNumber\x12\x11\n\tserialNum\x18\x01 \x02(\t\"\x81\x01\n\x12SetSimPortsRequest\x12\x33\n\x07simPort\x18\x01 \x03(\x0b\x32\".allego.SetSimPortsRequest.SimPort\x1a\x36\n\x07SimPort\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07numChan\x18\x02 \x02(\x03\"4\n\x19SetHasGPIOExpanderRequest\x12\x17\n\x0fhasGPIOExpander\x18\x01 \x02(\x08\"\'\n\x14SetMuxChannelRequest\x12\x0f\n\x07\x63hannel\x18\x01 \x02(\x03\"\'\n\x14SetPotVoltageRequest\x12\x0f\n\x07voltage\x18\x01 \x02(\x02\"!\n\x10GetADCLevelReply\x12\r\n\x05level\x18\x01 \x02(\x02\"#\n\x12SetPotRangeRequest\x12\r\n\x05range\x18\x01 \x02(\x05\"!\n\x11SetPotModeRequest\x12\x0c\n\x04mode\x18\x01 \x02(\x08\")\n\x17SetPotCellEnableRequest\x12\x0e\n\x06\x65nable\x18\x01 \x02(\x08\",\n\x12ReadWireOutRequest\x12\x16\n\x0ewireOutAddress\x18\x01 \x02(\x03\"(\n\x10ReadWireOutReply\x12\x14\n\x0cwireOutValue\x18\x01 \x02(\x03\"\xc7\x02\n\x11LogsysConfigReply\x12(\n\nsystemMode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x03 \x02(\x05\x12\x1a\n\x12priCachePersistDur\x18\x04 \x02(\x01\x12!\n\x19priCacheStatsUpdatePeriod\x18\x05 \x02(\x01\x12\x12\n\nactiveSigs\x18\x06 \x02(\x05\x12\x10\n\x08priChans\x18\x07 \x02(\x05\x12\x10\n\x08\x61uxChans\x18\x08 \x02(\x05\x12\x10\n\x08\x64inChans\x18\t \x02(\x05\x12\x11\n\tdoutChans\x18\n \x02(\x05\x12\"\n\x08portSpec\x18\x0b \x03(\x0b\x32\x10.allego.PortInfo\x12\x19\n\x11numConnectedPorts\x18\x0c \x02(\x05\"Y\n\x08PortInfo\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\r\n\x05probe\x18\x02 \x02(\t\x12\x11\n\theadstage\x18\x03 \x02(\t\x12\x0f\n\x07numSigs\x18\x04 \x02(\x05\"c\n\x11LogsysStatusReply\x12\'\n\x07recStat\x18\x01 \x02(\x0b\x32\x16.allego.RecorderStatus\x12%\n\x07sysStat\x18\x02 \x02(\x0b\x32\x14.allego.SystemStatus\"\xba\x01\n\x0eRecorderStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x10\n\x08\x64uration\x18\x02 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\x03 \x02(\x01\x12\x11\n\tsizeBytes\x18\x04 \x02(\x05\x12\x0c\n\x04path\x18\x05 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x06 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x07 \x02(\x05\x12\x16\n\x0e\x61\x63tiveFileName\x18\x08 \x02(\t\"\x96\x03\n\x0cSystemStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x12\n\nnumPriSigs\x18\x03 \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x04 \x02(\x05\x12\x12\n\nnumDinSigs\x18\x05 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x06 \x02(\x05\x12\x13\n\x0btStampRange\x18\x07 \x03(\x03\x12\x0e\n\x06tRange\x18\x08 \x03(\x01\x12\x11\n\tstreamDur\x18\t \x02(\x01\x12\x14\n\x0cmeanChunkDur\x18\n \x02(\x01\x12\x1c\n\x14meanHardwareMemLevel\x18\x0b \x02(\x02\x12\x1b\n\x13maxHardwareMemLevel\x18\x0c \x02(\x02\x12\x1b\n\x13minHardwareMemLevel\x18\r \x02(\x02\x12\x1c\n\x14lastHardwareMemLevel\x18\x0e \x02(\x02\x12\x19\n\x11meanStreamLoopDur\x18\x0f \x02(\x01\x12\x18\n\x10streamEfficiency\x18\x10 \x02(\x01\"\xd8\x02\n\x11LogsysPcacheReply\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x18\n\x10minNumDatablocks\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x03\x12 \n\x18totalDatablocksProcessed\x18\x06 \x02(\x04\x12\x16\n\x0enumTimeSamples\x18\x07 \x02(\x03\x12\x1f\n\x17\x61llTimeMeanDatablockDur\x18\x08 \x02(\x01\x12\x15\n\rnumDataBlocks\x18\t \x02(\x05\x12\x0e\n\x06tRange\x18\n \x03(\x01\x12\x0f\n\x07tsRange\x18\x0b \x03(\x03\x12\x12\n\nnumPriSigs\x18\x0c \x02(\x05\x12\x12\n\nnumAuxSigs\x18\r \x02(\x05\x12\x12\n\nnumDinSigs\x18\x0e \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x0f \x02(\x05\"i\n\x11SetTriggerRequest\x12\'\n\x07\x63hannel\x18\x01 \x02(\x0e\x32\x16.allego.TriggerChannel\x12\x0f\n\x07\x65nabled\x18\x02 \x02(\x08\x12\x1a\n\x04port\x18\x03 \x01(\x0e\x32\x0c.allego.Port\"\\\n\x0cTriggerState\x12/\n\x0f\x65nabledChannels\x18\x01 \x03(\x0e\x32\x16.allego.TriggerChannel\x12\x1b\n\x05ports\x18\x02 \x03(\x0e\x32\x0c.allego.Port\"*\n\x12LoadAllMosiRequest\x12\x14\n\x0cregisterVals\x18\x01 \x03(\x05\"\x15\n\x13TransmitMosiRequest\"5\n\x0f\x44umpMisoRequest\x12\x10\n\x08nSamples\x18\x01 \x02(\x05\x12\x10\n\x08\x66ileName\x18\x02 \x02(\t\"\xc6\x03\n\x15SinapsStatusRegisters\x12\x18\n\x10\x63\x61librationState\x18\x01 \x02(\x08\x12\x1b\n\x13\x63\x61librationProgress\x18\x02 \x02(\x01\x12\x1d\n\x15numActivePixelsShank0\x18\x03 \x02(\x05\x12\x1d\n\x15numActivePixelsShank1\x18\x04 \x02(\x05\x12\x1d\n\x15numActivePixelsShank2\x18\x05 \x02(\x05\x12\x1d\n\x15numActivePixelsShank3\x18\x06 \x02(\x05\x12\x0f\n\x07vRefFFA\x18\x07 \x02(\x01\x12\x0f\n\x07vRefFFB\x18\x08 \x02(\x01\x12\x0f\n\x07vRefFFC\x18\t \x02(\x01\x12\x0f\n\x07vRefFFD\x18\n \x02(\x01\x12\x10\n\x08isError0\x18\x0b \x02(\x08\x12\x10\n\x08isError1\x18\x0c \x02(\x08\x12\x10\n\x08isError2\x18\r \x02(\x08\x12\x10\n\x08isError3\x18\x0e \x02(\x08\x12\x13\n\x0bhostCounter\x18\x0f \x02(\x05\x12\x13\n\x0b\x66pgaCounter\x18\x10 \x02(\x05\x12\x17\n\x0f\x66irmwareVersion\x18\x11 \x02(\t\x12\x17\n\x0fprobeGeneration\x18\x12 \x02(\x05\x12\x12\n\nprobeModel\x18\x13 \x02(\x05\"%\n\x12\x46lashSinapsRequest\x12\x0f\n\x07\x62itfile\x18\x01 \x02(\t\"3\n\x0cHALdashboard\x12#\n\x04mode\x18\x01 \x02(\x0e\x32\x15.allego.AllegoHALmode\"\xbc\x06\n\nStimParams\x12$\n\tstimShape\x18\x01 \x02(\x0e\x32\x11.allego.StimShape\x12*\n\x0cstimPolarity\x18\x02 \x02(\x0e\x32\x14.allego.StimPolarity\x12\x1a\n\x12\x66irstPhaseDuration\x18\x03 \x02(\x01\x12\x1b\n\x13secondPhaseDuration\x18\x04 \x02(\x01\x12\x17\n\x0finterphaseDelay\x18\x05 \x02(\x01\x12\x1b\n\x13\x66irstPhaseAmplitude\x18\x06 \x02(\x01\x12\x1c\n\x14secondPhaseAmplitude\x18\x07 \x02(\x01\x12\x17\n\x0f\x62\x61selineVoltage\x18\x08 \x02(\x01\x12:\n\x12triggerEdgeOrLevel\x18\n \x02(\x0e\x32\x1e.allego.StimTriggerEdgeOrLevel\x12\x36\n\x10triggerHighOrLow\x18\x0b \x02(\x0e\x32\x1c.allego.StimTriggerHighOrLow\x12\x0f\n\x07\x65nabled\x18\x0c \x02(\x08\x12\x18\n\x10postTriggerDelay\x18\r \x02(\x01\x12.\n\x0cpulseOrTrain\x18\x0e \x02(\x0e\x32\x18.allego.StimPulseOrTrain\x12\x1a\n\x12numberOfStimPulses\x18\x0f \x02(\x05\x12\x18\n\x10pulseTrainPeriod\x18\x10 \x02(\x01\x12\x18\n\x10refractoryPeriod\x18\x11 \x02(\x01\x12\x18\n\x10preStimAmpSettle\x18\x12 \x02(\x01\x12\x19\n\x11postStimAmpSettle\x18\x13 \x02(\x01\x12\x19\n\x11maintainAmpSettle\x18\x14 \x02(\x08\x12\x17\n\x0f\x65nableAmpSettle\x18\x15 \x02(\x08\x12\x1d\n\x15postStimChargeRecovOn\x18\x16 \x02(\x01\x12\x1e\n\x16postStimChargeRecovOff\x18\x17 \x02(\x01\x12\x1c\n\x14\x65nableChargeRecovery\x18\x18 \x02(\x08\x12\x1f\n\x17triggerSourceIsKeypress\x18\x19 \x02(\x08\x12\x18\n\x10triggerSourceIdx\x18\x1a \x02(\x05\x12\x16\n\x0estimSysChanIdx\x18\x1b \x02(\x05\"\x89\x01\n\x0fStimParamsReply\x12\x33\n\x06params\x18\x01 \x03(\x0b\x32#.allego.StimParamsReply.ParamsEntry\x1a\x41\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.allego.StimParams:\x02\x38\x01\">\n\x18ManualStimTriggerRequest\x12\x0f\n\x07trigger\x18\x01 \x02(\x05\x12\x11\n\ttriggerOn\x18\x02 \x02(\x08\"1\n\x1eManualStimTriggerToggleRequest\x12\x0f\n\x07trigger\x18\x01 \x02(\x05\"5\n\x0fStimStepMessage\x12\"\n\x08stimStep\x18\x01 \x02(\x0e\x32\x10.allego.StimStep*!\n\nStreamMode\x12\t\n\x05S_OFF\x10\x00\x12\x08\n\x04S_ON\x10\x01*!\n\nRecordMode\x12\t\n\x05R_OFF\x10\x00\x12\x08\n\x04R_ON\x10\x01*\x9f\x04\n\x0c\x42\x61\x63kboneMode\x12\x10\n\x0cSMARTBOX_PRO\x10\x00\x12\x19\n\x15SMARTBOX_SIM_GEN_SINE\x10\x01\x12\x1b\n\x17SMARTBOX_SIM_GEN_SPIKES\x10\x02\x12\x1b\n\x17SMARTBOX_SIM_DATASOURCE\x10\x03\x12\x13\n\x0fOPEN_EPHYS_USB3\x10\x04\x12#\n\x1fINTAN_RECORDING_CONTROLLER_1024\x10\x05\x12\x14\n\x10SMARTBOX_CLASSIC\x10\x06\x12\"\n\x1eINTAN_RECORDING_CONTROLLER_512\x10\x07\x12\x13\n\x0fOPEN_EPHYS_USB2\x10\x08\x12\x0e\n\nINTAN_USB2\x10\t\x12 \n\x1cSMARTBOX_SIM_GEN_SINE_MAPPED\x10\n\x12#\n\x1fSMARTBOX_SIM_GEN_SINE_HIGH_FREQ\x10\x0b\x12$\n SMARTBOX_SIM_GEN_SINE_MULTI_BAND\x10\x0c\x12\x1b\n\x17SMARTBOX_PRO_SINAPS_256\x10\r\x12\x1c\n\x18SMARTBOX_PRO_SINAPS_1024\x10\x0e\x12\x10\n\x0cXDAQ_ONE_REC\x10\x0f\x12\x11\n\rXDAQ_ONE_STIM\x10\x10\x12\x11\n\rXDAQ_CORE_REC\x10\x11\x12\x12\n\x0eXDAQ_CORE_STIM\x10\x12\x12\x1b\n\x17SMARTBOX_PRO_SINAPS_512\x10\x13*,\n\x07\x44IOMode\x12\n\n\x06manual\x10\x00\x12\n\n\x06\x65vents\x10\x01\x12\t\n\x05gated\x10\x02*\xf4\x01\n\x0eTriggerChannel\x12\x0b\n\x07T_DIN_0\x10\x00\x12\x0b\n\x07T_DIN_1\x10\x01\x12\x0b\n\x07T_DIN_2\x10\x02\x12\x0b\n\x07T_DIN_3\x10\x03\x12\x0b\n\x07T_DIN_4\x10\x04\x12\x0b\n\x07T_DIN_5\x10\x05\x12\x0b\n\x07T_DIN_6\x10\x06\x12\x0b\n\x07T_DIN_7\x10\x07\x12\x0c\n\x08T_DOUT_0\x10\x08\x12\x0c\n\x08T_DOUT_1\x10\t\x12\x0c\n\x08T_DOUT_2\x10\n\x12\x0c\n\x08T_DOUT_3\x10\x0b\x12\x0c\n\x08T_DOUT_4\x10\x0c\x12\x0c\n\x08T_DOUT_5\x10\r\x12\x0c\n\x08T_DOUT_6\x10\x0e\x12\x0c\n\x08T_DOUT_7\x10\x0f\x12\n\n\x06T_NONE\x10\x10*q\n\rAllegoHALmode\x12\x11\n\rA_HAL_GENERIC\x10\x00\x12\x13\n\x0f\x41_HAL_SPIKESORT\x10\x01\x12\x14\n\x10\x41_HAL_MULTISCALE\x10\x02\x12\"\n\x1e\x41_HAL_MULTISCALE_BIDIRECTIONAL\x10\x03*W\n\tStimShape\x12\x0c\n\x08\x42IPHASIC\x10\x00\x12\x1d\n\x19\x42IPHASIC_INTERPHASE_DELAY\x10\x01\x12\r\n\tTRIPHASIC\x10\x02\x12\x0e\n\nMONOPHASIC\x10\x03*4\n\x0cStimPolarity\x12\x12\n\x0e\x43\x41THODIC_FIRST\x10\x00\x12\x10\n\x0c\x41NODIC_FIRST\x10\x01*3\n\x16StimTriggerEdgeOrLevel\x12\x0b\n\x07ST_EDGE\x10\x00\x12\x0c\n\x08ST_LEVEL\x10\x01*/\n\x14StimTriggerHighOrLow\x12\x0b\n\x07ST_HIGH\x10\x00\x12\n\n\x06ST_LOW\x10\x01*5\n\x10StimPulseOrTrain\x12\x10\n\x0cSINGLE_PULSE\x10\x00\x12\x0f\n\x0bPULSE_TRAIN\x10\x01*\x90\x02\n\x08StimStep\x12\x13\n\x0fStimStepSizeMin\x10\x00\x12\x14\n\x10StimStepSize10nA\x10\x01\x12\x14\n\x10StimStepSize20nA\x10\x02\x12\x14\n\x10StimStepSize50nA\x10\x03\x12\x15\n\x11StimStepSize100nA\x10\x04\x12\x15\n\x11StimStepSize200nA\x10\x05\x12\x15\n\x11StimStepSize500nA\x10\x06\x12\x13\n\x0fStimStepSize1uA\x10\x07\x12\x13\n\x0fStimStepSize2uA\x10\x08\x12\x13\n\x0fStimStepSize5uA\x10\t\x12\x14\n\x10StimStepSize10uA\x10\n\x12\x13\n\x0fStimStepSizeMax\x10\x0b\x32\xbd*\n\nAllegoCore\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\x07Restart\x12\x16.allego.RestartRequest\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12j\n\x1bGetStatusPollFieldsToUpdate\x12\'.allego.StatusPollFieldsToUpdateRequest\x1a .allego.StatusPollFieldsToUpdate\"\x00\x12R\n\x17GetOfflineLicenseStatus\x12\x17.allego.StandardRequest\x1a\x1c.allego.OfflineLicenseStatus\"\x00\x12\x46\n\rSetConfigCore\x12\x1c.allego.SetConfigCoreRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0fSetProfileState\x12\x19.allego.SetProfileRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x12SetConfigRecording\x12\x17.allego.ConfigRecording\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetStreamState\x12\x18.allego.SetStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetRecordState\x12\x18.allego.SetRecordRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOEvents\x12\x1c.allego.DIOModeEventsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOManual\x12\x1c.allego.DIOModeManualRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bSetDIOGated\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nSetDACGain\x12\x16.allego.DACGainRequest\x1a\x15.allego.StandardReply\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x0eSetDACHighPass\x12\x1b.allego.DACHighPassRegister\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetSimPorts\x12\x1a.allego.SetSimPortsRequest\x1a\x15.allego.StandardReply\"\x00\x12P\n\x12SetHasGPIOExpander\x12!.allego.SetHasGPIOExpanderRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetMuxChannel\x12\x1c.allego.SetMuxChannelRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0fSetTriggerState\x12\x19.allego.SetTriggerRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetPotVoltage\x12\x1c.allego.SetPotVoltageRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetPotRange\x12\x1a.allego.SetPotRangeRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\nSetPotMode\x12\x19.allego.SetPotModeRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10SetPotCellEnable\x12\x1f.allego.SetPotCellEnableRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\rSetStimParams\x12\x12.allego.StimParams\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\rGetStimParams\x12\x17.allego.StandardRequest\x1a\x17.allego.StimParamsReply\"\x00\x12?\n\x0bSetStimStep\x12\x17.allego.StimStepMessage\x1a\x15.allego.StandardReply\"\x00\x12\x41\n\x0bGetStimStep\x12\x17.allego.StandardRequest\x1a\x17.allego.StimStepMessage\"\x00\x12N\n\x11ManualStimTrigger\x12 .allego.ManualStimTriggerRequest\x1a\x15.allego.StandardReply\"\x00\x12Z\n\x17ManualStimTriggerToggle\x12&.allego.ManualStimTriggerToggleRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\tGetConfig\x12\x17.allego.StandardRequest\x1a\x12.allego.ConfigCore\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12H\n\x12GetConfigRecording\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigRecording\"\x00\x12>\n\tGetStatus\x12\x17.allego.StandardRequest\x1a\x16.allego.BackboneStatus\"\x00\x12H\n\x12GetConfigAndStatus\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigAndStatus\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12\x42\n\x11GetIntanImpedance\x12\x18.allego.ImpedanceRequest\x1a\x11.allego.Impedance\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12\x42\n\tGetDIOReg\x12\x17.allego.StandardRequest\x1a\x1a.allego.DigitalOutRegister\"\x00\x12\x41\n\tGetDACReg\x12\x17.allego.StandardRequest\x1a\x19.allego.AnalogOutRegister\"\x00\x12<\n\tGetSerial\x12\x17.allego.StandardRequest\x1a\x14.allego.SerialNumber\"\x00\x12\x42\n\x0fGetTriggerState\x12\x17.allego.StandardRequest\x1a\x14.allego.TriggerState\"\x00\x12\x42\n\x0bGetADCLevel\x12\x17.allego.StandardRequest\x1a\x18.allego.GetADCLevelReply\"\x00\x12\x45\n\x0bReadWireOut\x12\x1a.allego.ReadWireOutRequest\x1a\x18.allego.ReadWireOutReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12H\n\x0eGetSorterIDMap\x12\x17.allego.StandardRequest\x1a\x1b.allego.GetSorterIDMapReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tScanPorts\x12\x17.allego.StandardRequest\x1a\x13.allego.SignalGroup\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12O\n\x13GetDataSourceStatus\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceStatus\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bLoadAllMosi\x12\x1a.allego.LoadAllMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x0cTransmitMosi\x12\x1b.allego.TransmitMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\x08\x44umpMiso\x12\x17.allego.DumpMisoRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x18GetSinapsStatusRegisters\x12\x17.allego.StandardRequest\x1a\x1d.allego.SinapsStatusRegisters\"\x00\x12\x42\n\x0b\x46lashSinaps\x12\x1a.allego.FlashSinapsRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x16GetOrCreateEventViewer\x12\x15.allego.EventViewerID\x1a\x19.allego.EventViewerConfig\"\x00\x12G\n\x11UpdateEventViewer\x12\x19.allego.EventViewerConfig\x1a\x15.allego.StandardReply\"\x00\x12T\n\x15ListEventViewerEvents\x12\x15.allego.EventViewerID\x1a\".allego.ListEventViewerEventsReply\"\x00\x12U\n\x13GetEventViewerEvent\x12\".allego.GetEventViewerEventRequest\x1a\x18.allego.EventViewerEvent\"\x00\x12L\n\x10ListEventViewers\x12\x17.allego.StandardRequest\x1a\x1d.allego.ListEventViewersReply\"\x00\x12\x42\n\x0fGetHALdashboard\x12\x17.allego.StandardRequest\x1a\x14.allego.HALdashboard\"\x00\x32\xe4\x02\n\x07Pcache1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12J\n\x15GetHDSnapshotFromHead\x12\x1a.allego.HDSnapshotRequest2\x1a\x13.allego.HDSnapshot2\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12K\n\x12SetTimeRangeToHead\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x32\x8d\x04\n\x04Kpi1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x12K\n\x0bSetKpiParam\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x0bGetKpiParam\x12\x19.allego.DataSourceRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12I\n\x12SetKpiUpdatePeriod\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x0fSetKpiPacketDur\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x32\x8f\x0b\n\x08Neurons1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SpikeSorterSetParams\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x63\n\x17SpikeSorterGetDashboard\x12#.allego.SpikeSorterDashboardRequest\x1a!.allego.SpikeSorterDashboardReply\"\x00\x12i\n\x18SpikeSorterGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12j\n\x1bSpikeSorterGetFeatureParams\x12\".allego.SpikeSorterStandardRequest\x1a%.allego.SpikeSorterFeatureParamsReply\"\x00\x12\x61\n\x1a\x42iointerfaceGetSpikesDense\x12\x1e.allego.SpikesGetSpikesRequest\x1a!.allego.SpikesSpikeDataDenseReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12l\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x11.allego.TimeRange\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x12q\n\x15GetSpikeTrainAnalytic\x12+.allego.SpikesGetSpikeTrainAnalyticsRequest\x1a).allego.SpikesGetSpikeTrainAnalyticsReply\"\x00\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'allegoserver_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
@@ -166,9 +166,9 @@
   _ALLEGOCORE._serialized_start=8854
   _ALLEGOCORE._serialized_end=14291
   _PCACHE1._serialized_start=14294
   _PCACHE1._serialized_end=14650
   _KPI1._serialized_start=14653
   _KPI1._serialized_end=15178
   _NEURONS1._serialized_start=15181
-  _NEURONS1._serialized_end=16496
+  _NEURONS1._serialized_end=16604
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-3.0.0b5/radiens/grpc_radiens/allegoserver_pb2_grpc.py` & `radiens-3.0.0b6/radiens/grpc_radiens/allegoserver_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3031,14 +3031,19 @@
                 response_deserializer=spikesorter__pb2.SpikeSorterDashboardReply.FromString,
                 )
         self.SpikeSorterGetRasterData = channel.unary_unary(
                 '/allego.Neurons1/SpikeSorterGetRasterData',
                 request_serializer=spikesorter__pb2.SpikeSorterGetRasterDataRequest.SerializeToString,
                 response_deserializer=spikesorter__pb2.SpikeSorterRasterDataReply.FromString,
                 )
+        self.SpikeSorterGetFeatureParams = channel.unary_unary(
+                '/allego.Neurons1/SpikeSorterGetFeatureParams',
+                request_serializer=spikesorter__pb2.SpikeSorterStandardRequest.SerializeToString,
+                response_deserializer=spikesorter__pb2.SpikeSorterFeatureParamsReply.FromString,
+                )
         self.BiointerfaceGetSpikesDense = channel.unary_unary(
                 '/allego.Neurons1/BiointerfaceGetSpikesDense',
                 request_serializer=biointerface__pb2.SpikesGetSpikesRequest.SerializeToString,
                 response_deserializer=biointerface__pb2.SpikesSpikeDataDenseReply.FromString,
                 )
         self.BiointerfaceGetNeurons = channel.unary_unary(
                 '/allego.Neurons1/BiointerfaceGetNeurons',
@@ -3114,14 +3119,20 @@
 
     def SpikeSorterGetRasterData(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SpikeSorterGetFeatureParams(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def BiointerfaceGetSpikesDense(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def BiointerfaceGetNeurons(self, request, context):
@@ -3193,14 +3204,19 @@
                     response_serializer=spikesorter__pb2.SpikeSorterDashboardReply.SerializeToString,
             ),
             'SpikeSorterGetRasterData': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikeSorterGetRasterData,
                     request_deserializer=spikesorter__pb2.SpikeSorterGetRasterDataRequest.FromString,
                     response_serializer=spikesorter__pb2.SpikeSorterRasterDataReply.SerializeToString,
             ),
+            'SpikeSorterGetFeatureParams': grpc.unary_unary_rpc_method_handler(
+                    servicer.SpikeSorterGetFeatureParams,
+                    request_deserializer=spikesorter__pb2.SpikeSorterStandardRequest.FromString,
+                    response_serializer=spikesorter__pb2.SpikeSorterFeatureParamsReply.SerializeToString,
+            ),
             'BiointerfaceGetSpikesDense': grpc.unary_unary_rpc_method_handler(
                     servicer.BiointerfaceGetSpikesDense,
                     request_deserializer=biointerface__pb2.SpikesGetSpikesRequest.FromString,
                     response_serializer=biointerface__pb2.SpikesSpikeDataDenseReply.SerializeToString,
             ),
             'BiointerfaceGetNeurons': grpc.unary_unary_rpc_method_handler(
                     servicer.BiointerfaceGetNeurons,
@@ -3370,14 +3386,31 @@
         return grpc.experimental.unary_unary(request, target, '/allego.Neurons1/SpikeSorterGetRasterData',
             spikesorter__pb2.SpikeSorterGetRasterDataRequest.SerializeToString,
             spikesorter__pb2.SpikeSorterRasterDataReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def SpikeSorterGetFeatureParams(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.Neurons1/SpikeSorterGetFeatureParams',
+            spikesorter__pb2.SpikeSorterStandardRequest.SerializeToString,
+            spikesorter__pb2.SpikeSorterFeatureParamsReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def BiointerfaceGetSpikesDense(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `radiens-3.0.0b5/radiens/grpc_radiens/biointerface_pb2.py` & `radiens-3.0.0b6/radiens/grpc_radiens/biointerface_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,44 +10,44 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import common_pb2 as common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x62iointerface.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\"!\n\x0cSpikesStdReq\x12\x11\n\tdsourceID\x18\x01 \x02(\t\"\x14\n\x12SpikesNewLoadReply\"<\n\x0fSpikesRenameReq\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x16\n\x0eisForceReplace\x18\x02 \x01(\x08\"\x13\n\x11SpikesGetIDsReply\"\x80\x01\n\x14NeuronColorGroupData\x12\x1b\n\x13\x63olorGroupIdxNeuron\x18\x01 \x02(\x05\x12\x1c\n\x14\x63olorGroupIdxChannel\x18\x02 \x02(\x05\x12\x15\n\rposColorGroup\x18\x03 \x02(\x05\x12\x16\n\x0esizeColorGroup\x18\x04 \x02(\x05\"\xb8\x01\n\x17SpikeTrainAnalyticsData\x12\x12\n\nbinnedData\x18\x01 \x03(\x05\x12\x12\n\nbinCenters\x18\x02 \x03(\x01\x12\x0e\n\x06ntvIdx\x18\x03 \x02(\x05\x12\r\n\x05label\x18\x04 \x02(\t\x12\n\n\x02id\x18\x05 \x02(\t\x12\x0e\n\x06yRange\x18\x06 \x03(\x05\x12:\n\x14neuronColorGroupData\x18\x07 \x02(\x0b\x32\x1c.allego.NeuronColorGroupData\"y\n!SpikesGetSpikeTrainAnalyticsReply\x12@\n\x17spikeTrainAnalyticsData\x18\x01 \x03(\x0b\x32\x1f.allego.SpikeTrainAnalyticsData\x12\x12\n\nnumNeurons\x18\x02 \x02(\x05\"\xb2\x02\n#SpikesGetSpikeTrainAnalyticsRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x10\n\x08\x62inRange\x18\x03 \x03(\x01\x12\x0f\n\x07numBins\x18\x04 \x02(\x03\x12,\n\x08\x61nalytic\x18\x05 \x02(\x0e\x32\x1a.allego.SpikeTrainAnalytic\x12\x14\n\x0c\x63learHistory\x18\x06 \x01(\x08\x12\x16\n\x0eneuronStartIdx\x18\x07 \x01(\x03\x12$\n\x06sortBy\x18\x08 \x02(\x0e\x32\x14.allego.NeuronSortBy\x12(\n\x08sortMode\x18\t \x02(\x0e\x32\x16.allego.NeuronSortMode\x12\x12\n\nmaxNeurons\x18\n \x01(\x03\"\x87\x05\n\x0fSpikesSpecReply\x12\x16\n\x0e\x62iointerfaceID\x18\x01 \x02(\t\x12\x12\n\ndatasetUID\x18\x02 \x02(\t\x12\x10\n\x08\x63hecksum\x18\x03 \x02(\t\x12\x15\n\rprovenanceUID\x18\x04 \x03(\t\x12\x12\n\npersistDur\x18\x06 \x02(\x01\x12\x10\n\x08sampFreq\x18\x07 \x02(\x01\x12\x10\n\x08numSites\x18\x08 \x02(\x03\x12\x11\n\tsizeBytes\x18\t \x02(\x03\x12\x1d\n\x15\x65nabledSiteNtvChanIdx\x18\n \x03(\x05\x12\x11\n\ttimeRange\x18\x0b \x03(\x01\x12\x16\n\x0etimestampRange\x18\x0c \x03(\x03\x12\x15\n\rwallTimeStart\x18\r \x02(\t\x12$\n\x04site\x18\x0e \x03(\x0b\x32\x16.allego.SpikesSiteSpec\x12*\n\tsiteStats\x18\x11 \x01(\x0b\x32\x17.allego.SpikesSiteStats\x12\x31\n\tsensorExt\x18\x12 \x01(\x0b\x32\x1e.allego.SensorExtendedMetadata\x12(\n\x07project\x18\x13 \x01(\x0b\x32\x17.allego.ProjectMetadata\x12)\n\x07\x62ioType\x18\x14 \x02(\x0e\x32\x18.allego.BiointerfaceType\x12\x17\n\x0freqNumNeighbors\x18\x15 \x01(\x03\x12\x1c\n\x14neighborhoodRadiusUm\x18\x16 \x01(\x01\x12\x1d\n\x02tR\x18\x17 \x01(\x0b\x32\x11.allego.TimeRange\x12\x1f\n\x02sG\x18\x18 \x01(\x0b\x32\x13.allego.SignalGroup\x12\"\n\x07spikeTR\x18\x19 \x01(\x0b\x32\x11.allego.TimeRange\"\xf7\x04\n\x0eSpikesSiteSpec\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12,\n\x08neighbor\x18\x02 \x02(\x0b\x32\x1a.allego.NeighborDescriptor\x12\x11\n\tisEnabled\x18\x03 \x02(\x08\x12\x10\n\x08posProbe\x18\x04 \x03(\x01\x12\x11\n\tposTissue\x18\x05 \x03(\x01\x12\x10\n\x08sampFreq\x18\x06 \x02(\x01\x12\x15\n\rwallTimeStart\x18\x07 \x02(\t\x12\x11\n\ttimeRange\x18\x08 \x03(\x01\x12\x16\n\x0etimestampRange\x18\t \x03(\x03\x12\x16\n\x0espikeTimeRange\x18\n \x03(\x01\x12\x1b\n\x13spikeTimestampRange\x18\x0b \x03(\x03\x12\x1c\n\x14spikeTimeRangeMemory\x18\x0c \x03(\x01\x12!\n\x19spikeTimestampRangeMemory\x18\r \x03(\x03\x12\x1c\n\x14spikeCountSiteMemory\x18\x0e \x01(\x03\x12\x16\n\x0espikeCountSite\x18\x0f \x03(\x01\x12\x15\n\rspikeRateSite\x18\x10 \x03(\x01\x12\x14\n\x0cnoiseLevelSd\x18\x11 \x02(\x01\x12\x0f\n\x07snrSite\x18\x12 \x02(\x01\x12(\n\x06neuron\x18\x13 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12\x12\n\nnumNeurons\x18\x14 \x01(\x05\x12,\n\x07\x63ompLen\x18\x15 \x02(\x0b\x32\x1b.allego.SpikeComponentShape\x12\x1d\n\x02tR\x18\x16 \x01(\x0b\x32\x11.allego.TimeRange\x12\"\n\x07spikeTR\x18\x17 \x01(\x0b\x32\x11.allego.TimeRange\"!\n\x10SpikeLabelRecord\x12\r\n\x05label\x18\x01 \x03(\x05\"\x9a\x02\n\x0bSpikeMatrix\x12\x11\n\tnumSpikes\x18\x01 \x02(\x03\x12\x17\n\x0ftimestampsBytes\x18\x02 \x02(\x0c\x12\x0e\n\x06labels\x18\x03 \x03(\t\x12\x15\n\rwaveformBytes\x18\x04 \x01(\x0c\x12\x13\n\x0bwaveformLen\x18\x05 \x01(\x05\x12\x15\n\rfeaturesBytes\x18\x06 \x01(\x0c\x12\x13\n\x0b\x66\x65\x61turesLen\x18\x07 \x01(\x05\x12\x16\n\x0e\x66\x65\x61tures2Bytes\x18\x08 \x01(\x0c\x12\x14\n\x0c\x66\x65\x61tures2Len\x18\t \x01(\x05\x12\x13\n\x0bzscoreBytes\x18\n \x01(\x0c\x12\x11\n\tzscoreLen\x18\x0b \x01(\x05\x12\x0f\n\x07siteIdx\x18\x0c \x01(\x05\x12\x10\n\x08spikePos\x18\r \x03(\x05\"}\n\x0eSpikeMatrixSet\x12\x0b\n\x03uID\x18\x01 \x02(\t\x12\x0f\n\x07siteIdx\x18\x02 \x03(\x05\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12\x10\n\x08sampFreq\x18\x04 \x02(\x01\x12#\n\x06spkMtx\x18\x05 \x03(\x0b\x32\x13.allego.SpikeMatrix\"\x93\x01\n\x14NeuronSpikeMatrixSet\x12\x0e\n\x06labels\x18\x01 \x03(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x0f\n\x07siteIdx\x18\x03 \x03(\x05\x12#\n\x06spkMtx\x18\x04 \x03(\x0b\x32\x13.allego.SpikeMatrix\x12\x16\n\x0etimestampRange\x18\x05 \x03(\x03\x12\x0b\n\x03uID\x18\x06 \x02(\t\"\xa1\x02\n\x16SpikesGetSpikesRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\'\n\x04mode\x18\x02 \x02(\x0e\x32\x19.allego.NeuronsSignalMode\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12\x11\n\ttimeStart\x18\x04 \x02(\x01\x12\x10\n\x08timeStop\x18\x05 \x02(\x01\x12-\n\x0bspikeLabels\x18\x06 \x03(\x0b\x32\x18.allego.SpikeLabelRecord\x12\x1b\n\x13maxSpikesPerChannel\x18\x07 \x02(\x05\x12\x33\n\tspikeComp\x18\x08 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x11\n\tspkSortID\x18\t \x01(\t\"\x99\x01\n\x1a\x42iointerfaceGetHistRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12%\n\x04mode\x18\x02 \x02(\x0e\x32\x17.allego.HistScalingMode\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12-\n\x0bspikeLabels\x18\x04 \x03(\x0b\x32\x18.allego.SpikeLabelRecord\"\x90\x01\n%BiointerfaceGetSpikeTimestampsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12-\n\x0bspikeLabels\x18\x06 \x03(\x0b\x32\x18.allego.SpikeLabelRecord\"\x8b\x01\n BiointerfaceSpikeTimestampsReply\x12<\n\x18spikeTimestampsByChannel\x18\x02 \x03(\x0b\x32\x1a.allego.SpikeTimestampData\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimeStampRange\x18\x04 \x03(\x03\"S\n)BiointerfaceSeekEndSpikeTimestampsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x13\n\x0b\x63omponentID\x18\x02 \x02(\t\"Y\n\x1d\x42iointerfaceGetNeuronsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\"\xa1\x03\n\x1b\x42iointerfaceGetNeuronsReply\x12;\n\x04site\x18\x01 \x03(\x0b\x32-.allego.BiointerfaceGetNeuronsReply.SiteEntry\x1a\x36\n\x0eSpikeRateChunk\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x11\n\tspikeRate\x18\x02 \x03(\x01\x1a\xb2\x01\n\x07NeuronL\x12(\n\x06neuron\x18\x01 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12:\n\x14neuronColorGroupData\x18\x02 \x03(\x0b\x32\x1c.allego.NeuronColorGroupData\x12\x41\n\x05\x63hunk\x18\x03 \x01(\x0b\x32\x32.allego.BiointerfaceGetNeuronsReply.SpikeRateChunk\x1aX\n\tSiteEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.allego.BiointerfaceGetNeuronsReply.NeuronL:\x02\x38\x01\"\x87\x02\n\x0fSpikesSiteStats\x12\x17\n\x0fspikeCountStats\x18\t \x03(\x01\x12\x1e\n\x16labeledSpikeCountStats\x18\n \x03(\x01\x12 \n\x18unlabeledSpikeCountStats\x18\x0b \x03(\x01\x12\x16\n\x0espikeRateStats\x18\x0c \x03(\x01\x12\x1d\n\x15labeledSpikeRateStats\x18\r \x03(\x01\x12\x1f\n\x17unlabeledSpikeRateStats\x18\x0e \x03(\x01\x12\x16\n\x0esiteNoiseStats\x18\x0f \x03(\x01\x12\x14\n\x0csiteSnrStats\x18\x10 \x03(\x01\x12\x13\n\x0bneuronStats\x18\x11 \x03(\x01\"W\n\x13SpikeComponentShape\x12\x10\n\x08waveform\x18\x01 \x03(\x05\x12\x0f\n\x07\x66\x65\x61ture\x18\x02 \x03(\x05\x12\x10\n\x08\x66\x65\x61ture2\x18\x03 \x03(\x05\x12\x0b\n\x03pos\x18\x04 \x03(\x05\"\xa8\x01\n\x12NeighborDescriptor\x12\x0e\n\x06radius\x18\x01 \x02(\x01\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x10\n\x08\x64istance\x18\x03 \x03(\x01\x12\x10\n\x08thetaDeg\x18\x04 \x03(\x01\x12\x0e\n\x06phiDeg\x18\x05 \x03(\x01\x12\x0b\n\x03num\x18\x06 \x02(\x05\x12\x14\n\x0cSiteCenterUm\x18\x07 \x03(\x01\x12\x17\n\x0fSiteCenterTcsUm\x18\x08 \x03(\x01\"\xf3\x01\n\x10NeuronDescriptor\x12\x10\n\x08neuronID\x18\x01 \x02(\t\x12\x16\n\x0esiteNtvChanIdx\x18\x02 \x02(\x05\x12\x12\n\nspikeLabel\x18\x03 \x02(\t\x12\x10\n\x08posProbe\x18\x04 \x03(\x01\x12\x11\n\tposTissue\x18\x05 \x03(\x01\x12\x12\n\nspikeCount\x18\x06 \x02(\x03\x12\x11\n\tspikeRate\x18\x07 \x02(\x01\x12\x16\n\x0emeanAbsPeakWfm\x18\x08 \x01(\x01\x12\x0b\n\x03snr\x18\t \x01(\x01\x12\x30\n\x08metaData\x18\n \x01(\x0b\x32\x1e.allego.NeuronExtendedMetadata\"\x86\x01\n\x16NeuronExtendedMetadata\x12\x18\n\x10neuronCatalogUID\x18\x01 \x01(\t\x12\x13\n\x0b\x65nsembleUID\x18\x02 \x01(\t\x12\x17\n\x0f\x66uncAssemblyUID\x18\x03 \x03(\t\x12\x12\n\ndatasetUID\x18\x04 \x01(\t\x12\x10\n\x08probeUID\x18\x05 \x01(\t\"\x8b\x01\n\x10NeuronStatistics\x12\x1a\n\x12WaveformAvgAbsAmpl\x18\x01 \x02(\x01\x12\x0b\n\x03Snr\x18\x02 \x02(\x01\x12\x12\n\nspikeCount\x18\x03 \x02(\x03\x12\x14\n\x0c\x61vgSpikeRate\x18\x04 \x02(\x01\x12$\n\x04isih\x18\x05 \x01(\x0b\x32\x16.allego.NeuronHistData\"|\n\x0fSpikeDescriptor\x12\x11\n\ttimestamp\x18\x01 \x02(\x03\x12\r\n\x05label\x18\x02 \x02(\t\x12\x10\n\x08waveform\x18\x03 \x03(\x02\x12\x10\n\x08\x66\x65\x61tures\x18\x04 \x03(\x02\x12\x13\n\x0b\x64\x65\x63\x46\x65\x61tures\x18\x05 \x03(\x01\x12\x0e\n\x06zscore\x18\x06 \x03(\x02\"g\n\tSpikeData\x12&\n\x05spike\x18\x01 \x03(\x0b\x32\x17.allego.SpikeDescriptor\x12\x18\n\x10waveformMaxValue\x18\x02 \x02(\x02\x12\x18\n\x10waveformMinValue\x18\x03 \x02(\x02\"1\n\rSpikeTimeData\x12\x11\n\tspikeTime\x18\x01 \x03(\x01\x12\r\n\x05label\x18\x02 \x03(\x05\"V\n\x12SpikeTimestampData\x12\x17\n\x0fntvChanIdxArray\x18\x01 \x03(\x05\x12\x17\n\x0fspikeTimestamps\x18\x02 \x03(\x03\x12\x0e\n\x06labels\x18\x03 \x03(\x05\"\x85\x01\n\x0eSpikeTimestamp\x12\x16\n\x0espikeTimestamp\x18\x01 \x02(\x03\x12:\n\x14neuronColorGroupData\x18\x02 \x02(\x0b\x32\x1c.allego.NeuronColorGroupData\x12\r\n\x05label\x18\x03 \x02(\x05\x12\x10\n\x08\x64\x61taIdxs\x18\x04 \x03(\x05\"\xb6\x02\n\x17SpikeTemplateDescriptor\x12\x10\n\x08neuronID\x18\x01 \x02(\t\x12\r\n\x05label\x18\x02 \x02(\t\x12\x11\n\tnumSpikes\x18\x03 \x02(\x03\x12\x10\n\x08waveform\x18\x04 \x02(\x0c\x12\x12\n\nwaveformSd\x18\x05 \x02(\x0c\x12\x13\n\x0blenWaveform\x18\x06 \x02(\x03\x12\x10\n\x08\x66\x65\x61tures\x18\x07 \x02(\x0c\x12\x12\n\nfeaturesSd\x18\x08 \x02(\x0c\x12\x13\n\x0blenFeatures\x18\t \x02(\x03\x12\x11\n\tfeatures2\x18\n \x02(\x0c\x12\x13\n\x0b\x66\x65\x61tures2Sd\x18\x0b \x02(\x0c\x12\x14\n\x0clenFeatures2\x18\x0c \x02(\x03\x12\x0e\n\x06zscore\x18\r \x02(\x0c\x12\x10\n\x08zscoreSd\x18\x0e \x02(\x0c\x12\x11\n\tlenZscore\x18\x0f \x02(\x03\"[\n\x12SiteSpikeTemplates\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x31\n\x08template\x18\x02 \x03(\x0b\x32\x1f.allego.SpikeTemplateDescriptor\"\x97\x01\n\x1f\x42iointerfaceSpikeTemplatesReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12(\n\x04site\x18\x05 \x03(\x0b\x32\x1a.allego.SiteSpikeTemplates\"@\n\x14\x42iointerfaceMetaData\x12(\n\x0bsignalGroup\x18\x01 \x01(\x0b\x32\x13.allego.SignalGroup\"\xd6\x01\n\x1a\x42iointerfaceSpikeDataReply\x12\x16\n\x0e\x62iointerfaceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimestampRange\x18\x04 \x03(\x03\x12\x12\n\nntvChanIdx\x18\x05 \x03(\x05\x12\x1f\n\x04site\x18\x06 \x03(\x0b\x32\x11.allego.SpikeData\x12.\n\x08metaData\x18\x07 \x01(\x0b\x32\x1c.allego.BiointerfaceMetaData\"\xb5\x01\n\x1fSpikeDataDenseChannelDescriptor\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x0e\n\x06labels\x18\x02 \x03(\x05\x12:\n\x14neuronColorGroupData\x18\x03 \x03(\x0b\x32\x1c.allego.NeuronColorGroupData\x12\x18\n\x10waveformMaxValue\x18\x04 \x02(\x02\x12\x18\n\x10waveformMinValue\x18\x05 \x02(\x02\"\xb0\x01\n\x19SpikesSpikeDataDenseReply\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x17\n\x0fwaveformNPoints\x18\x02 \x02(\x05\x12\x14\n\x0ctotalNSpikes\x18\x03 \x02(\x05\x12\x43\n\x12\x63hannelDescriptors\x18\x04 \x03(\x0b\x32\'.allego.SpikeDataDenseChannelDescriptor\x12\x0c\n\x04\x64\x61ta\x18\x05 \x02(\x0c\"\x8a\x01\n\x17GroupSpikeTimeDataReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12#\n\x04site\x18\x05 \x03(\x0b\x32\x15.allego.SpikeTimeData\"v\n\x16\x42iointerfaceSpiketrain\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x10\n\x08sampFreq\x18\x03 \x02(\x01\x12$\n\x04site\x18\x04 \x03(\x0b\x32\x16.allego.SiteSpiketrain\"p\n\x0eSiteSpiketrain\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\"\n\x06neuron\x18\x02 \x03(\x0b\x32\x12.allego.Spiketrain\x12\x10\n\x08sampFreq\x18\x03 \x02(\x01\x12\x14\n\x0cnumNeighbors\x18\x04 \x02(\x05\"\x8b\x02\n\nSpiketrain\x12\x10\n\x08sampFreq\x18\x01 \x02(\x01\x12\r\n\x05label\x18\x02 \x02(\x05\x12\x17\n\x0fspikeTimestamps\x18\x03 \x03(\x03\x12\x14\n\x0cwaveformData\x18\x05 \x03(\x02\x12\x15\n\rwaveformShape\x18\x06 \x03(\x05\x12\x13\n\x0b\x66\x65\x61tureData\x18\x07 \x03(\x02\x12\x14\n\x0c\x66\x65\x61tureShape\x18\x08 \x03(\x05\x12\x12\n\nzscoreData\x18\t \x03(\x02\x12\x13\n\x0bzscoreShape\x18\n \x03(\x05\x12,\n\nneuronDesc\x18\x0f \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x14\n\x0cnumNeighbors\x18\x11 \x02(\x05\"\xb6\x01\n\x0eNeuronHistData\x12\x13\n\x0b\x62inWidthSec\x18\x01 \x02(\x01\x12\x15\n\rhistTimeRange\x18\x02 \x03(\x01\x12%\n\x04mode\x18\x03 \x02(\x0e\x32\x17.allego.HistScalingMode\x12\x14\n\x0cnumRefEvents\x18\x04 \x02(\x03\x12\x11\n\tnumSpikes\x18\x05 \x02(\x03\x12\x1a\n\x12numProcessedSpikes\x18\x06 \x02(\x03\x12\x0c\n\x04hist\x18\x07 \x03(\x01\"\x9d\x01\n\x0cSiteHistData\x12\x14\n\x0csitePosProbe\x18\x01 \x03(\x01\x12\x14\n\x0csitePosBrain\x18\x02 \x03(\x01\x12(\n\x06neuron\x18\x03 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12$\n\x04hist\x18\x04 \x03(\x0b\x32\x16.allego.NeuronHistData\x12\x11\n\ttimeRange\x18\x05 \x03(\x01\"\x8b\x01\n\x19\x42iointerfaceHistDataReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12\"\n\x04site\x18\x05 \x03(\x0b\x32\x14.allego.SiteHistData\"\xb4\x01\n\x17\x42iointerfaceSaveRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x11\n\ttimeRange\x18\x04 \x03(\x01\x12\x33\n\tspikeComp\x18\x05 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x1e\n\x16includeNeuronTemplates\x18\x06 \x02(\x08\"\xac\x01\n\x17\x42iointerfaceLoadRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x13\n\x0buidFragment\x18\x04 \x02(\t\x12\x33\n\tspikeComp\x18\x05 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x14\n\x0c\x66orceReplace\x18\x06 \x02(\x08\"\x95\x01\n\x19\x42iointerfaceSaveLoadReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x0b\n\x03uid\x18\x04 \x02(\t\x12\x1c\n\x14\x62iointerfaceMetaFile\x18\x05 \x02(\t\x12\x1a\n\x12neuronTemplateFile\x18\x06 \x02(\t\"2\n\x17\x42iointerfaceGetIDsReply\x12\x17\n\x0f\x62iointerfaceIDs\x18\x01 \x03(\t\"\xef\x01\n\x16\x42iointerfaceVizRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x35\n\x07vizType\x18\x02 \x02(\x0e\x32$.allego.BiointerfaceVizRequest.VType\x12\x12\n\nnumSamples\x18\x03 \x02(\x05\x12\x14\n\x0cisYAutoScale\x18\x04 \x02(\x08\x12\x0c\n\x04yLim\x18\x05 \x03(\x01\x12\x0e\n\x06\x66igDir\x18\x06 \x01(\t\x12\x12\n\nisAutoOpen\x18\x07 \x01(\x08\"/\n\x05VType\x12\x15\n\x11VIZ_BIO_TEMPLATES\x10\x00\x12\x0f\n\x0bVIZ_BIO_DEV\x10\x01\"2\n\x14\x42iointerfaceVizReply\x12\x1a\n\x12pngPathAndFileName\x18\x01 \x01(\t*T\n\x10\x42iointerfaceType\x12\x13\n\x0f\x42IO_SPIKETRAINS\x10\x00\x12\x14\n\x10\x42IO_SPIKES_CACHE\x10\x01\x12\x15\n\x11\x42IO_SPIKES_STREAM\x10\x02* \n\x12SpikesImportSchema\x12\n\n\x06NI_SIM\x10\x00*@\n\x13\x42iointerfaceCommand\x12\x13\n\x0f\x42IO_CMD_SAVE_ON\x10\x00\x12\x14\n\x10\x42IO_CMD_SAVE_OFF\x10\x01*J\n\x11\x42iointerfaceState\x12\x0f\n\x0b\x42IO_SAVE_ON\x10\x00\x12\x10\n\x0c\x42IO_SAVE_OFF\x10\x01\x12\x12\n\x0e\x42IO_CONFIGURED\x10\x02*\x1d\n\x12SpikeTrainAnalytic\x12\x07\n\x03ISI\x10\x00*C\n\x0cNeuronSortBy\x12\x14\n\x10SB_MONITOR_MATCH\x10\x00\x12\x11\n\rSB_SPIKE_RATE\x10\x01\x12\n\n\x06SB_SNR\x10\x02*5\n\x0eNeuronSortMode\x12\x10\n\x0cSM_ASCENDING\x10\x00\x12\x11\n\rSM_DESCENDING\x10\x01*X\n\x11NeuronsSignalMode\x12\n\n\x06Spikes\x10\x00\x12\x13\n\x0fSpikeTimestamps\x10\x01\x12\x0e\n\nSpikeTimes\x10\x02\x12\x12\n\x0eSpikeWaveforms\x10\x03*q\n\x18SpikeDescriptorComponent\x12\x0e\n\nCTimestamp\x10\x00\x12\n\n\x06\x43Label\x10\x01\x12\r\n\tCWaveform\x10\x02\x12\x0c\n\x08\x43\x46\x65\x61ture\x10\x03\x12\x0f\n\x0b\x43\x44\x65\x63\x46\x65\x61ture\x10\x04\x12\x0b\n\x07\x43Zscore\x10\x05*S\n\x0fHistScalingMode\x12\x0c\n\x08\x41sSpikes\x10\x00\x12\x0f\n\x0b\x41sSpikeRate\x10\x01\x12\n\n\x06\x41sNorm\x10\x02\x12\n\n\x06\x41sProb\x10\x03\x12\t\n\x05\x41sRaw\x10\x04\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x62iointerface.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\"!\n\x0cSpikesStdReq\x12\x11\n\tdsourceID\x18\x01 \x02(\t\"\x14\n\x12SpikesNewLoadReply\"<\n\x0fSpikesRenameReq\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x16\n\x0eisForceReplace\x18\x02 \x01(\x08\"\x13\n\x11SpikesGetIDsReply\"\x80\x01\n\x14NeuronColorGroupData\x12\x1b\n\x13\x63olorGroupIdxNeuron\x18\x01 \x02(\x05\x12\x1c\n\x14\x63olorGroupIdxChannel\x18\x02 \x02(\x05\x12\x15\n\rposColorGroup\x18\x03 \x02(\x05\x12\x16\n\x0esizeColorGroup\x18\x04 \x02(\x05\"\xb8\x01\n\x17SpikeTrainAnalyticsData\x12\x12\n\nbinnedData\x18\x01 \x03(\x05\x12\x12\n\nbinCenters\x18\x02 \x03(\x01\x12\x0e\n\x06ntvIdx\x18\x03 \x02(\x05\x12\r\n\x05label\x18\x04 \x02(\t\x12\n\n\x02id\x18\x05 \x02(\t\x12\x0e\n\x06yRange\x18\x06 \x03(\x05\x12:\n\x14neuronColorGroupData\x18\x07 \x02(\x0b\x32\x1c.allego.NeuronColorGroupData\"y\n!SpikesGetSpikeTrainAnalyticsReply\x12@\n\x17spikeTrainAnalyticsData\x18\x01 \x03(\x0b\x32\x1f.allego.SpikeTrainAnalyticsData\x12\x12\n\nnumNeurons\x18\x02 \x02(\x05\"\xb2\x02\n#SpikesGetSpikeTrainAnalyticsRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x10\n\x08\x62inRange\x18\x03 \x03(\x01\x12\x0f\n\x07numBins\x18\x04 \x02(\x03\x12,\n\x08\x61nalytic\x18\x05 \x02(\x0e\x32\x1a.allego.SpikeTrainAnalytic\x12\x14\n\x0c\x63learHistory\x18\x06 \x01(\x08\x12\x16\n\x0eneuronStartIdx\x18\x07 \x01(\x03\x12$\n\x06sortBy\x18\x08 \x02(\x0e\x32\x14.allego.NeuronSortBy\x12(\n\x08sortMode\x18\t \x02(\x0e\x32\x16.allego.NeuronSortMode\x12\x12\n\nmaxNeurons\x18\n \x01(\x03\"\x87\x05\n\x0fSpikesSpecReply\x12\x16\n\x0e\x62iointerfaceID\x18\x01 \x02(\t\x12\x12\n\ndatasetUID\x18\x02 \x02(\t\x12\x10\n\x08\x63hecksum\x18\x03 \x02(\t\x12\x15\n\rprovenanceUID\x18\x04 \x03(\t\x12\x12\n\npersistDur\x18\x06 \x02(\x01\x12\x10\n\x08sampFreq\x18\x07 \x02(\x01\x12\x10\n\x08numSites\x18\x08 \x02(\x03\x12\x11\n\tsizeBytes\x18\t \x02(\x03\x12\x1d\n\x15\x65nabledSiteNtvChanIdx\x18\n \x03(\x05\x12\x11\n\ttimeRange\x18\x0b \x03(\x01\x12\x16\n\x0etimestampRange\x18\x0c \x03(\x03\x12\x15\n\rwallTimeStart\x18\r \x02(\t\x12$\n\x04site\x18\x0e \x03(\x0b\x32\x16.allego.SpikesSiteSpec\x12*\n\tsiteStats\x18\x11 \x01(\x0b\x32\x17.allego.SpikesSiteStats\x12\x31\n\tsensorExt\x18\x12 \x01(\x0b\x32\x1e.allego.SensorExtendedMetadata\x12(\n\x07project\x18\x13 \x01(\x0b\x32\x17.allego.ProjectMetadata\x12)\n\x07\x62ioType\x18\x14 \x02(\x0e\x32\x18.allego.BiointerfaceType\x12\x17\n\x0freqNumNeighbors\x18\x15 \x01(\x03\x12\x1c\n\x14neighborhoodRadiusUm\x18\x16 \x01(\x01\x12\x1d\n\x02tR\x18\x17 \x01(\x0b\x32\x11.allego.TimeRange\x12\x1f\n\x02sG\x18\x18 \x01(\x0b\x32\x13.allego.SignalGroup\x12\"\n\x07spikeTR\x18\x19 \x01(\x0b\x32\x11.allego.TimeRange\"\xf7\x04\n\x0eSpikesSiteSpec\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12,\n\x08neighbor\x18\x02 \x02(\x0b\x32\x1a.allego.NeighborDescriptor\x12\x11\n\tisEnabled\x18\x03 \x02(\x08\x12\x10\n\x08posProbe\x18\x04 \x03(\x01\x12\x11\n\tposTissue\x18\x05 \x03(\x01\x12\x10\n\x08sampFreq\x18\x06 \x02(\x01\x12\x15\n\rwallTimeStart\x18\x07 \x02(\t\x12\x11\n\ttimeRange\x18\x08 \x03(\x01\x12\x16\n\x0etimestampRange\x18\t \x03(\x03\x12\x16\n\x0espikeTimeRange\x18\n \x03(\x01\x12\x1b\n\x13spikeTimestampRange\x18\x0b \x03(\x03\x12\x1c\n\x14spikeTimeRangeMemory\x18\x0c \x03(\x01\x12!\n\x19spikeTimestampRangeMemory\x18\r \x03(\x03\x12\x1c\n\x14spikeCountSiteMemory\x18\x0e \x01(\x03\x12\x16\n\x0espikeCountSite\x18\x0f \x03(\x01\x12\x15\n\rspikeRateSite\x18\x10 \x03(\x01\x12\x14\n\x0cnoiseLevelSd\x18\x11 \x02(\x01\x12\x0f\n\x07snrSite\x18\x12 \x02(\x01\x12(\n\x06neuron\x18\x13 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12\x12\n\nnumNeurons\x18\x14 \x01(\x05\x12,\n\x07\x63ompLen\x18\x15 \x02(\x0b\x32\x1b.allego.SpikeComponentShape\x12\x1d\n\x02tR\x18\x16 \x01(\x0b\x32\x11.allego.TimeRange\x12\"\n\x07spikeTR\x18\x17 \x01(\x0b\x32\x11.allego.TimeRange\"\x9a\x02\n\x0bSpikeMatrix\x12\x11\n\tnumSpikes\x18\x01 \x02(\x03\x12\x17\n\x0ftimestampsBytes\x18\x02 \x02(\x0c\x12\x0e\n\x06labels\x18\x03 \x03(\t\x12\x15\n\rwaveformBytes\x18\x04 \x01(\x0c\x12\x13\n\x0bwaveformLen\x18\x05 \x01(\x05\x12\x15\n\rfeaturesBytes\x18\x06 \x01(\x0c\x12\x13\n\x0b\x66\x65\x61turesLen\x18\x07 \x01(\x05\x12\x16\n\x0e\x66\x65\x61tures2Bytes\x18\x08 \x01(\x0c\x12\x14\n\x0c\x66\x65\x61tures2Len\x18\t \x01(\x05\x12\x13\n\x0bzscoreBytes\x18\n \x01(\x0c\x12\x11\n\tzscoreLen\x18\x0b \x01(\x05\x12\x0f\n\x07siteIdx\x18\x0c \x01(\x05\x12\x10\n\x08spikePos\x18\r \x03(\x05\"}\n\x0eSpikeMatrixSet\x12\x0b\n\x03uID\x18\x01 \x02(\t\x12\x0f\n\x07siteIdx\x18\x02 \x03(\x05\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12\x10\n\x08sampFreq\x18\x04 \x02(\x01\x12#\n\x06spkMtx\x18\x05 \x03(\x0b\x32\x13.allego.SpikeMatrix\"\x93\x01\n\x14NeuronSpikeMatrixSet\x12\x0e\n\x06labels\x18\x01 \x03(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x0f\n\x07siteIdx\x18\x03 \x03(\x05\x12#\n\x06spkMtx\x18\x04 \x03(\x0b\x32\x13.allego.SpikeMatrix\x12\x16\n\x0etimestampRange\x18\x05 \x03(\x03\x12\x0b\n\x03uID\x18\x06 \x02(\t\"\x87\x02\n\x16SpikesGetSpikesRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\'\n\x04mode\x18\x02 \x02(\x0e\x32\x19.allego.NeuronsSignalMode\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12\x11\n\ttimeStart\x18\x04 \x02(\x01\x12\x10\n\x08timeStop\x18\x05 \x02(\x01\x12\x13\n\x0bspikeLabels\x18\x06 \x03(\x05\x12\x1b\n\x13maxSpikesPerChannel\x18\x07 \x02(\x05\x12\x33\n\tspikeComp\x18\x08 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x11\n\tspkSortID\x18\t \x01(\t\"\x7f\n\x1a\x42iointerfaceGetHistRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12%\n\x04mode\x18\x02 \x02(\x0e\x32\x17.allego.HistScalingMode\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12\x13\n\x0bspikeLabels\x18\x04 \x03(\x05\"v\n%BiointerfaceGetSpikeTimestampsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x13\n\x0bspikeLabels\x18\x06 \x03(\x05\"\x8b\x01\n BiointerfaceSpikeTimestampsReply\x12<\n\x18spikeTimestampsByChannel\x18\x02 \x03(\x0b\x32\x1a.allego.SpikeTimestampData\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimeStampRange\x18\x04 \x03(\x03\"S\n)BiointerfaceSeekEndSpikeTimestampsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x13\n\x0b\x63omponentID\x18\x02 \x02(\t\"Y\n\x1d\x42iointerfaceGetNeuronsRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\"\xa1\x03\n\x1b\x42iointerfaceGetNeuronsReply\x12;\n\x04site\x18\x01 \x03(\x0b\x32-.allego.BiointerfaceGetNeuronsReply.SiteEntry\x1a\x36\n\x0eSpikeRateChunk\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x11\n\tspikeRate\x18\x02 \x03(\x01\x1a\xb2\x01\n\x07NeuronL\x12(\n\x06neuron\x18\x01 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12:\n\x14neuronColorGroupData\x18\x02 \x03(\x0b\x32\x1c.allego.NeuronColorGroupData\x12\x41\n\x05\x63hunk\x18\x03 \x01(\x0b\x32\x32.allego.BiointerfaceGetNeuronsReply.SpikeRateChunk\x1aX\n\tSiteEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.allego.BiointerfaceGetNeuronsReply.NeuronL:\x02\x38\x01\"\x87\x02\n\x0fSpikesSiteStats\x12\x17\n\x0fspikeCountStats\x18\t \x03(\x01\x12\x1e\n\x16labeledSpikeCountStats\x18\n \x03(\x01\x12 \n\x18unlabeledSpikeCountStats\x18\x0b \x03(\x01\x12\x16\n\x0espikeRateStats\x18\x0c \x03(\x01\x12\x1d\n\x15labeledSpikeRateStats\x18\r \x03(\x01\x12\x1f\n\x17unlabeledSpikeRateStats\x18\x0e \x03(\x01\x12\x16\n\x0esiteNoiseStats\x18\x0f \x03(\x01\x12\x14\n\x0csiteSnrStats\x18\x10 \x03(\x01\x12\x13\n\x0bneuronStats\x18\x11 \x03(\x01\"W\n\x13SpikeComponentShape\x12\x10\n\x08waveform\x18\x01 \x03(\x05\x12\x0f\n\x07\x66\x65\x61ture\x18\x02 \x03(\x05\x12\x10\n\x08\x66\x65\x61ture2\x18\x03 \x03(\x05\x12\x0b\n\x03pos\x18\x04 \x03(\x05\"\xa8\x01\n\x12NeighborDescriptor\x12\x0e\n\x06radius\x18\x01 \x02(\x01\x12\x12\n\nntvChanIdx\x18\x02 \x03(\x05\x12\x10\n\x08\x64istance\x18\x03 \x03(\x01\x12\x10\n\x08thetaDeg\x18\x04 \x03(\x01\x12\x0e\n\x06phiDeg\x18\x05 \x03(\x01\x12\x0b\n\x03num\x18\x06 \x02(\x05\x12\x14\n\x0cSiteCenterUm\x18\x07 \x03(\x01\x12\x17\n\x0fSiteCenterTcsUm\x18\x08 \x03(\x01\"\xf3\x01\n\x10NeuronDescriptor\x12\x10\n\x08neuronID\x18\x01 \x02(\t\x12\x16\n\x0esiteNtvChanIdx\x18\x02 \x02(\x05\x12\x12\n\nspikeLabel\x18\x03 \x02(\t\x12\x10\n\x08posProbe\x18\x04 \x03(\x01\x12\x11\n\tposTissue\x18\x05 \x03(\x01\x12\x12\n\nspikeCount\x18\x06 \x02(\x03\x12\x11\n\tspikeRate\x18\x07 \x02(\x01\x12\x16\n\x0emeanAbsPeakWfm\x18\x08 \x01(\x01\x12\x0b\n\x03snr\x18\t \x01(\x01\x12\x30\n\x08metaData\x18\n \x01(\x0b\x32\x1e.allego.NeuronExtendedMetadata\"\x86\x01\n\x16NeuronExtendedMetadata\x12\x18\n\x10neuronCatalogUID\x18\x01 \x01(\t\x12\x13\n\x0b\x65nsembleUID\x18\x02 \x01(\t\x12\x17\n\x0f\x66uncAssemblyUID\x18\x03 \x03(\t\x12\x12\n\ndatasetUID\x18\x04 \x01(\t\x12\x10\n\x08probeUID\x18\x05 \x01(\t\"\x8b\x01\n\x10NeuronStatistics\x12\x1a\n\x12WaveformAvgAbsAmpl\x18\x01 \x02(\x01\x12\x0b\n\x03Snr\x18\x02 \x02(\x01\x12\x12\n\nspikeCount\x18\x03 \x02(\x03\x12\x14\n\x0c\x61vgSpikeRate\x18\x04 \x02(\x01\x12$\n\x04isih\x18\x05 \x01(\x0b\x32\x16.allego.NeuronHistData\"|\n\x0fSpikeDescriptor\x12\x11\n\ttimestamp\x18\x01 \x02(\x03\x12\r\n\x05label\x18\x02 \x02(\t\x12\x10\n\x08waveform\x18\x03 \x03(\x02\x12\x10\n\x08\x66\x65\x61tures\x18\x04 \x03(\x02\x12\x13\n\x0b\x64\x65\x63\x46\x65\x61tures\x18\x05 \x03(\x01\x12\x0e\n\x06zscore\x18\x06 \x03(\x02\"g\n\tSpikeData\x12&\n\x05spike\x18\x01 \x03(\x0b\x32\x17.allego.SpikeDescriptor\x12\x18\n\x10waveformMaxValue\x18\x02 \x02(\x02\x12\x18\n\x10waveformMinValue\x18\x03 \x02(\x02\"1\n\rSpikeTimeData\x12\x11\n\tspikeTime\x18\x01 \x03(\x01\x12\r\n\x05label\x18\x02 \x03(\x05\"V\n\x12SpikeTimestampData\x12\x17\n\x0fntvChanIdxArray\x18\x01 \x03(\x05\x12\x17\n\x0fspikeTimestamps\x18\x02 \x03(\x03\x12\x0e\n\x06labels\x18\x03 \x03(\x05\"\x85\x01\n\x0eSpikeTimestamp\x12\x16\n\x0espikeTimestamp\x18\x01 \x02(\x03\x12:\n\x14neuronColorGroupData\x18\x02 \x02(\x0b\x32\x1c.allego.NeuronColorGroupData\x12\r\n\x05label\x18\x03 \x02(\x05\x12\x10\n\x08\x64\x61taIdxs\x18\x04 \x03(\x05\"\xb6\x02\n\x17SpikeTemplateDescriptor\x12\x10\n\x08neuronID\x18\x01 \x02(\t\x12\r\n\x05label\x18\x02 \x02(\t\x12\x11\n\tnumSpikes\x18\x03 \x02(\x03\x12\x10\n\x08waveform\x18\x04 \x02(\x0c\x12\x12\n\nwaveformSd\x18\x05 \x02(\x0c\x12\x13\n\x0blenWaveform\x18\x06 \x02(\x03\x12\x10\n\x08\x66\x65\x61tures\x18\x07 \x02(\x0c\x12\x12\n\nfeaturesSd\x18\x08 \x02(\x0c\x12\x13\n\x0blenFeatures\x18\t \x02(\x03\x12\x11\n\tfeatures2\x18\n \x02(\x0c\x12\x13\n\x0b\x66\x65\x61tures2Sd\x18\x0b \x02(\x0c\x12\x14\n\x0clenFeatures2\x18\x0c \x02(\x03\x12\x0e\n\x06zscore\x18\r \x02(\x0c\x12\x10\n\x08zscoreSd\x18\x0e \x02(\x0c\x12\x11\n\tlenZscore\x18\x0f \x02(\x03\"[\n\x12SiteSpikeTemplates\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x31\n\x08template\x18\x02 \x03(\x0b\x32\x1f.allego.SpikeTemplateDescriptor\"\x97\x01\n\x1f\x42iointerfaceSpikeTemplatesReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12(\n\x04site\x18\x05 \x03(\x0b\x32\x1a.allego.SiteSpikeTemplates\"@\n\x14\x42iointerfaceMetaData\x12(\n\x0bsignalGroup\x18\x01 \x01(\x0b\x32\x13.allego.SignalGroup\"\xd6\x01\n\x1a\x42iointerfaceSpikeDataReply\x12\x16\n\x0e\x62iointerfaceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimestampRange\x18\x04 \x03(\x03\x12\x12\n\nntvChanIdx\x18\x05 \x03(\x05\x12\x1f\n\x04site\x18\x06 \x03(\x0b\x32\x11.allego.SpikeData\x12.\n\x08metaData\x18\x07 \x01(\x0b\x32\x1c.allego.BiointerfaceMetaData\"\xb5\x01\n\x1fSpikeDataDenseChannelDescriptor\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x0e\n\x06labels\x18\x02 \x03(\x05\x12:\n\x14neuronColorGroupData\x18\x03 \x03(\x0b\x32\x1c.allego.NeuronColorGroupData\x12\x18\n\x10waveformMaxValue\x18\x04 \x02(\x02\x12\x18\n\x10waveformMinValue\x18\x05 \x02(\x02\"\xb0\x01\n\x19SpikesSpikeDataDenseReply\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x17\n\x0fwaveformNPoints\x18\x02 \x02(\x05\x12\x14\n\x0ctotalNSpikes\x18\x03 \x02(\x05\x12\x43\n\x12\x63hannelDescriptors\x18\x04 \x03(\x0b\x32\'.allego.SpikeDataDenseChannelDescriptor\x12\x0c\n\x04\x64\x61ta\x18\x05 \x02(\x0c\"\x8a\x01\n\x17GroupSpikeTimeDataReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12#\n\x04site\x18\x05 \x03(\x0b\x32\x15.allego.SpikeTimeData\"v\n\x16\x42iointerfaceSpiketrain\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x10\n\x08sampFreq\x18\x03 \x02(\x01\x12$\n\x04site\x18\x04 \x03(\x0b\x32\x16.allego.SiteSpiketrain\"p\n\x0eSiteSpiketrain\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\"\n\x06neuron\x18\x02 \x03(\x0b\x32\x12.allego.Spiketrain\x12\x10\n\x08sampFreq\x18\x03 \x02(\x01\x12\x14\n\x0cnumNeighbors\x18\x04 \x02(\x05\"\x8b\x02\n\nSpiketrain\x12\x10\n\x08sampFreq\x18\x01 \x02(\x01\x12\r\n\x05label\x18\x02 \x02(\x05\x12\x17\n\x0fspikeTimestamps\x18\x03 \x03(\x03\x12\x14\n\x0cwaveformData\x18\x05 \x03(\x02\x12\x15\n\rwaveformShape\x18\x06 \x03(\x05\x12\x13\n\x0b\x66\x65\x61tureData\x18\x07 \x03(\x02\x12\x14\n\x0c\x66\x65\x61tureShape\x18\x08 \x03(\x05\x12\x12\n\nzscoreData\x18\t \x03(\x02\x12\x13\n\x0bzscoreShape\x18\n \x03(\x05\x12,\n\nneuronDesc\x18\x0f \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x14\n\x0cnumNeighbors\x18\x11 \x02(\x05\"\xb6\x01\n\x0eNeuronHistData\x12\x13\n\x0b\x62inWidthSec\x18\x01 \x02(\x01\x12\x15\n\rhistTimeRange\x18\x02 \x03(\x01\x12%\n\x04mode\x18\x03 \x02(\x0e\x32\x17.allego.HistScalingMode\x12\x14\n\x0cnumRefEvents\x18\x04 \x02(\x03\x12\x11\n\tnumSpikes\x18\x05 \x02(\x03\x12\x1a\n\x12numProcessedSpikes\x18\x06 \x02(\x03\x12\x0c\n\x04hist\x18\x07 \x03(\x01\"\x9d\x01\n\x0cSiteHistData\x12\x14\n\x0csitePosProbe\x18\x01 \x03(\x01\x12\x14\n\x0csitePosBrain\x18\x02 \x03(\x01\x12(\n\x06neuron\x18\x03 \x03(\x0b\x32\x18.allego.NeuronDescriptor\x12$\n\x04hist\x18\x04 \x03(\x0b\x32\x16.allego.NeuronHistData\x12\x11\n\ttimeRange\x18\x05 \x03(\x01\"\x8b\x01\n\x19\x42iointerfaceHistDataReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x12\n\nntvChanIdx\x18\x04 \x03(\x05\x12\"\n\x04site\x18\x05 \x03(\x0b\x32\x14.allego.SiteHistData\"\xb4\x01\n\x17\x42iointerfaceSaveRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x11\n\ttimeRange\x18\x04 \x03(\x01\x12\x33\n\tspikeComp\x18\x05 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x1e\n\x16includeNeuronTemplates\x18\x06 \x02(\x08\"\xac\x01\n\x17\x42iointerfaceLoadRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x13\n\x0buidFragment\x18\x04 \x02(\t\x12\x33\n\tspikeComp\x18\x05 \x03(\x0e\x32 .allego.SpikeDescriptorComponent\x12\x14\n\x0c\x66orceReplace\x18\x06 \x02(\x08\"\x95\x01\n\x19\x42iointerfaceSaveLoadReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x03 \x02(\t\x12\x0b\n\x03uid\x18\x04 \x02(\t\x12\x1c\n\x14\x62iointerfaceMetaFile\x18\x05 \x02(\t\x12\x1a\n\x12neuronTemplateFile\x18\x06 \x02(\t\"2\n\x17\x42iointerfaceGetIDsReply\x12\x17\n\x0f\x62iointerfaceIDs\x18\x01 \x03(\t\"\xef\x01\n\x16\x42iointerfaceVizRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x35\n\x07vizType\x18\x02 \x02(\x0e\x32$.allego.BiointerfaceVizRequest.VType\x12\x12\n\nnumSamples\x18\x03 \x02(\x05\x12\x14\n\x0cisYAutoScale\x18\x04 \x02(\x08\x12\x0c\n\x04yLim\x18\x05 \x03(\x01\x12\x0e\n\x06\x66igDir\x18\x06 \x01(\t\x12\x12\n\nisAutoOpen\x18\x07 \x01(\x08\"/\n\x05VType\x12\x15\n\x11VIZ_BIO_TEMPLATES\x10\x00\x12\x0f\n\x0bVIZ_BIO_DEV\x10\x01\"2\n\x14\x42iointerfaceVizReply\x12\x1a\n\x12pngPathAndFileName\x18\x01 \x01(\t*T\n\x10\x42iointerfaceType\x12\x13\n\x0f\x42IO_SPIKETRAINS\x10\x00\x12\x14\n\x10\x42IO_SPIKES_CACHE\x10\x01\x12\x15\n\x11\x42IO_SPIKES_STREAM\x10\x02* \n\x12SpikesImportSchema\x12\n\n\x06NI_SIM\x10\x00*@\n\x13\x42iointerfaceCommand\x12\x13\n\x0f\x42IO_CMD_SAVE_ON\x10\x00\x12\x14\n\x10\x42IO_CMD_SAVE_OFF\x10\x01*J\n\x11\x42iointerfaceState\x12\x0f\n\x0b\x42IO_SAVE_ON\x10\x00\x12\x10\n\x0c\x42IO_SAVE_OFF\x10\x01\x12\x12\n\x0e\x42IO_CONFIGURED\x10\x02*\x1d\n\x12SpikeTrainAnalytic\x12\x07\n\x03ISI\x10\x00*C\n\x0cNeuronSortBy\x12\x14\n\x10SB_MONITOR_MATCH\x10\x00\x12\x11\n\rSB_SPIKE_RATE\x10\x01\x12\n\n\x06SB_SNR\x10\x02*5\n\x0eNeuronSortMode\x12\x10\n\x0cSM_ASCENDING\x10\x00\x12\x11\n\rSM_DESCENDING\x10\x01*X\n\x11NeuronsSignalMode\x12\n\n\x06Spikes\x10\x00\x12\x13\n\x0fSpikeTimestamps\x10\x01\x12\x0e\n\nSpikeTimes\x10\x02\x12\x12\n\x0eSpikeWaveforms\x10\x03*q\n\x18SpikeDescriptorComponent\x12\x0e\n\nCTimestamp\x10\x00\x12\n\n\x06\x43Label\x10\x01\x12\r\n\tCWaveform\x10\x02\x12\x0c\n\x08\x43\x46\x65\x61ture\x10\x03\x12\x0f\n\x0b\x43\x44\x65\x63\x46\x65\x61ture\x10\x04\x12\x0b\n\x07\x43Zscore\x10\x05*S\n\x0fHistScalingMode\x12\x0c\n\x08\x41sSpikes\x10\x00\x12\x0f\n\x0b\x41sSpikeRate\x10\x01\x12\n\n\x06\x41sNorm\x10\x02\x12\n\n\x06\x41sProb\x10\x03\x12\t\n\x05\x41sRaw\x10\x04\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'biointerface_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
   _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._options = None
   _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._serialized_options = b'8\001'
-  _BIOINTERFACETYPE._serialized_start=8899
-  _BIOINTERFACETYPE._serialized_end=8983
-  _SPIKESIMPORTSCHEMA._serialized_start=8985
-  _SPIKESIMPORTSCHEMA._serialized_end=9017
-  _BIOINTERFACECOMMAND._serialized_start=9019
-  _BIOINTERFACECOMMAND._serialized_end=9083
-  _BIOINTERFACESTATE._serialized_start=9085
-  _BIOINTERFACESTATE._serialized_end=9159
-  _SPIKETRAINANALYTIC._serialized_start=9161
-  _SPIKETRAINANALYTIC._serialized_end=9190
-  _NEURONSORTBY._serialized_start=9192
-  _NEURONSORTBY._serialized_end=9259
-  _NEURONSORTMODE._serialized_start=9261
-  _NEURONSORTMODE._serialized_end=9314
-  _NEURONSSIGNALMODE._serialized_start=9316
-  _NEURONSSIGNALMODE._serialized_end=9404
-  _SPIKEDESCRIPTORCOMPONENT._serialized_start=9406
-  _SPIKEDESCRIPTORCOMPONENT._serialized_end=9519
-  _HISTSCALINGMODE._serialized_start=9521
-  _HISTSCALINGMODE._serialized_end=9604
+  _BIOINTERFACETYPE._serialized_start=8784
+  _BIOINTERFACETYPE._serialized_end=8868
+  _SPIKESIMPORTSCHEMA._serialized_start=8870
+  _SPIKESIMPORTSCHEMA._serialized_end=8902
+  _BIOINTERFACECOMMAND._serialized_start=8904
+  _BIOINTERFACECOMMAND._serialized_end=8968
+  _BIOINTERFACESTATE._serialized_start=8970
+  _BIOINTERFACESTATE._serialized_end=9044
+  _SPIKETRAINANALYTIC._serialized_start=9046
+  _SPIKETRAINANALYTIC._serialized_end=9075
+  _NEURONSORTBY._serialized_start=9077
+  _NEURONSORTBY._serialized_end=9144
+  _NEURONSORTMODE._serialized_start=9146
+  _NEURONSORTMODE._serialized_end=9199
+  _NEURONSSIGNALMODE._serialized_start=9201
+  _NEURONSSIGNALMODE._serialized_end=9289
+  _SPIKEDESCRIPTORCOMPONENT._serialized_start=9291
+  _SPIKEDESCRIPTORCOMPONENT._serialized_end=9404
+  _HISTSCALINGMODE._serialized_start=9406
+  _HISTSCALINGMODE._serialized_end=9489
   _SPIKESSTDREQ._serialized_start=44
   _SPIKESSTDREQ._serialized_end=77
   _SPIKESNEWLOADREPLY._serialized_start=79
   _SPIKESNEWLOADREPLY._serialized_end=99
   _SPIKESRENAMEREQ._serialized_start=101
   _SPIKESRENAMEREQ._serialized_end=161
   _SPIKESGETIDSREPLY._serialized_start=163
@@ -60,100 +60,98 @@
   _SPIKESGETSPIKETRAINANALYTICSREPLY._serialized_end=623
   _SPIKESGETSPIKETRAINANALYTICSREQUEST._serialized_start=626
   _SPIKESGETSPIKETRAINANALYTICSREQUEST._serialized_end=932
   _SPIKESSPECREPLY._serialized_start=935
   _SPIKESSPECREPLY._serialized_end=1582
   _SPIKESSITESPEC._serialized_start=1585
   _SPIKESSITESPEC._serialized_end=2216
-  _SPIKELABELRECORD._serialized_start=2218
-  _SPIKELABELRECORD._serialized_end=2251
-  _SPIKEMATRIX._serialized_start=2254
-  _SPIKEMATRIX._serialized_end=2536
-  _SPIKEMATRIXSET._serialized_start=2538
-  _SPIKEMATRIXSET._serialized_end=2663
-  _NEURONSPIKEMATRIXSET._serialized_start=2666
-  _NEURONSPIKEMATRIXSET._serialized_end=2813
-  _SPIKESGETSPIKESREQUEST._serialized_start=2816
-  _SPIKESGETSPIKESREQUEST._serialized_end=3105
-  _BIOINTERFACEGETHISTREQUEST._serialized_start=3108
-  _BIOINTERFACEGETHISTREQUEST._serialized_end=3261
-  _BIOINTERFACEGETSPIKETIMESTAMPSREQUEST._serialized_start=3264
-  _BIOINTERFACEGETSPIKETIMESTAMPSREQUEST._serialized_end=3408
-  _BIOINTERFACESPIKETIMESTAMPSREPLY._serialized_start=3411
-  _BIOINTERFACESPIKETIMESTAMPSREPLY._serialized_end=3550
-  _BIOINTERFACESEEKENDSPIKETIMESTAMPSREQUEST._serialized_start=3552
-  _BIOINTERFACESEEKENDSPIKETIMESTAMPSREQUEST._serialized_end=3635
-  _BIOINTERFACEGETNEURONSREQUEST._serialized_start=3637
-  _BIOINTERFACEGETNEURONSREQUEST._serialized_end=3726
-  _BIOINTERFACEGETNEURONSREPLY._serialized_start=3729
-  _BIOINTERFACEGETNEURONSREPLY._serialized_end=4146
-  _BIOINTERFACEGETNEURONSREPLY_SPIKERATECHUNK._serialized_start=3821
-  _BIOINTERFACEGETNEURONSREPLY_SPIKERATECHUNK._serialized_end=3875
-  _BIOINTERFACEGETNEURONSREPLY_NEURONL._serialized_start=3878
-  _BIOINTERFACEGETNEURONSREPLY_NEURONL._serialized_end=4056
-  _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._serialized_start=4058
-  _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._serialized_end=4146
-  _SPIKESSITESTATS._serialized_start=4149
-  _SPIKESSITESTATS._serialized_end=4412
-  _SPIKECOMPONENTSHAPE._serialized_start=4414
-  _SPIKECOMPONENTSHAPE._serialized_end=4501
-  _NEIGHBORDESCRIPTOR._serialized_start=4504
-  _NEIGHBORDESCRIPTOR._serialized_end=4672
-  _NEURONDESCRIPTOR._serialized_start=4675
-  _NEURONDESCRIPTOR._serialized_end=4918
-  _NEURONEXTENDEDMETADATA._serialized_start=4921
-  _NEURONEXTENDEDMETADATA._serialized_end=5055
-  _NEURONSTATISTICS._serialized_start=5058
-  _NEURONSTATISTICS._serialized_end=5197
-  _SPIKEDESCRIPTOR._serialized_start=5199
-  _SPIKEDESCRIPTOR._serialized_end=5323
-  _SPIKEDATA._serialized_start=5325
-  _SPIKEDATA._serialized_end=5428
-  _SPIKETIMEDATA._serialized_start=5430
-  _SPIKETIMEDATA._serialized_end=5479
-  _SPIKETIMESTAMPDATA._serialized_start=5481
-  _SPIKETIMESTAMPDATA._serialized_end=5567
-  _SPIKETIMESTAMP._serialized_start=5570
-  _SPIKETIMESTAMP._serialized_end=5703
-  _SPIKETEMPLATEDESCRIPTOR._serialized_start=5706
-  _SPIKETEMPLATEDESCRIPTOR._serialized_end=6016
-  _SITESPIKETEMPLATES._serialized_start=6018
-  _SITESPIKETEMPLATES._serialized_end=6109
-  _BIOINTERFACESPIKETEMPLATESREPLY._serialized_start=6112
-  _BIOINTERFACESPIKETEMPLATESREPLY._serialized_end=6263
-  _BIOINTERFACEMETADATA._serialized_start=6265
-  _BIOINTERFACEMETADATA._serialized_end=6329
-  _BIOINTERFACESPIKEDATAREPLY._serialized_start=6332
-  _BIOINTERFACESPIKEDATAREPLY._serialized_end=6546
-  _SPIKEDATADENSECHANNELDESCRIPTOR._serialized_start=6549
-  _SPIKEDATADENSECHANNELDESCRIPTOR._serialized_end=6730
-  _SPIKESSPIKEDATADENSEREPLY._serialized_start=6733
-  _SPIKESSPIKEDATADENSEREPLY._serialized_end=6909
-  _GROUPSPIKETIMEDATAREPLY._serialized_start=6912
-  _GROUPSPIKETIMEDATAREPLY._serialized_end=7050
-  _BIOINTERFACESPIKETRAIN._serialized_start=7052
-  _BIOINTERFACESPIKETRAIN._serialized_end=7170
-  _SITESPIKETRAIN._serialized_start=7172
-  _SITESPIKETRAIN._serialized_end=7284
-  _SPIKETRAIN._serialized_start=7287
-  _SPIKETRAIN._serialized_end=7554
-  _NEURONHISTDATA._serialized_start=7557
-  _NEURONHISTDATA._serialized_end=7739
-  _SITEHISTDATA._serialized_start=7742
-  _SITEHISTDATA._serialized_end=7899
-  _BIOINTERFACEHISTDATAREPLY._serialized_start=7902
-  _BIOINTERFACEHISTDATAREPLY._serialized_end=8041
-  _BIOINTERFACESAVEREQUEST._serialized_start=8044
-  _BIOINTERFACESAVEREQUEST._serialized_end=8224
-  _BIOINTERFACELOADREQUEST._serialized_start=8227
-  _BIOINTERFACELOADREQUEST._serialized_end=8399
-  _BIOINTERFACESAVELOADREPLY._serialized_start=8402
-  _BIOINTERFACESAVELOADREPLY._serialized_end=8551
-  _BIOINTERFACEGETIDSREPLY._serialized_start=8553
-  _BIOINTERFACEGETIDSREPLY._serialized_end=8603
-  _BIOINTERFACEVIZREQUEST._serialized_start=8606
-  _BIOINTERFACEVIZREQUEST._serialized_end=8845
-  _BIOINTERFACEVIZREQUEST_VTYPE._serialized_start=8798
-  _BIOINTERFACEVIZREQUEST_VTYPE._serialized_end=8845
-  _BIOINTERFACEVIZREPLY._serialized_start=8847
-  _BIOINTERFACEVIZREPLY._serialized_end=8897
+  _SPIKEMATRIX._serialized_start=2219
+  _SPIKEMATRIX._serialized_end=2501
+  _SPIKEMATRIXSET._serialized_start=2503
+  _SPIKEMATRIXSET._serialized_end=2628
+  _NEURONSPIKEMATRIXSET._serialized_start=2631
+  _NEURONSPIKEMATRIXSET._serialized_end=2778
+  _SPIKESGETSPIKESREQUEST._serialized_start=2781
+  _SPIKESGETSPIKESREQUEST._serialized_end=3044
+  _BIOINTERFACEGETHISTREQUEST._serialized_start=3046
+  _BIOINTERFACEGETHISTREQUEST._serialized_end=3173
+  _BIOINTERFACEGETSPIKETIMESTAMPSREQUEST._serialized_start=3175
+  _BIOINTERFACEGETSPIKETIMESTAMPSREQUEST._serialized_end=3293
+  _BIOINTERFACESPIKETIMESTAMPSREPLY._serialized_start=3296
+  _BIOINTERFACESPIKETIMESTAMPSREPLY._serialized_end=3435
+  _BIOINTERFACESEEKENDSPIKETIMESTAMPSREQUEST._serialized_start=3437
+  _BIOINTERFACESEEKENDSPIKETIMESTAMPSREQUEST._serialized_end=3520
+  _BIOINTERFACEGETNEURONSREQUEST._serialized_start=3522
+  _BIOINTERFACEGETNEURONSREQUEST._serialized_end=3611
+  _BIOINTERFACEGETNEURONSREPLY._serialized_start=3614
+  _BIOINTERFACEGETNEURONSREPLY._serialized_end=4031
+  _BIOINTERFACEGETNEURONSREPLY_SPIKERATECHUNK._serialized_start=3706
+  _BIOINTERFACEGETNEURONSREPLY_SPIKERATECHUNK._serialized_end=3760
+  _BIOINTERFACEGETNEURONSREPLY_NEURONL._serialized_start=3763
+  _BIOINTERFACEGETNEURONSREPLY_NEURONL._serialized_end=3941
+  _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._serialized_start=3943
+  _BIOINTERFACEGETNEURONSREPLY_SITEENTRY._serialized_end=4031
+  _SPIKESSITESTATS._serialized_start=4034
+  _SPIKESSITESTATS._serialized_end=4297
+  _SPIKECOMPONENTSHAPE._serialized_start=4299
+  _SPIKECOMPONENTSHAPE._serialized_end=4386
+  _NEIGHBORDESCRIPTOR._serialized_start=4389
+  _NEIGHBORDESCRIPTOR._serialized_end=4557
+  _NEURONDESCRIPTOR._serialized_start=4560
+  _NEURONDESCRIPTOR._serialized_end=4803
+  _NEURONEXTENDEDMETADATA._serialized_start=4806
+  _NEURONEXTENDEDMETADATA._serialized_end=4940
+  _NEURONSTATISTICS._serialized_start=4943
+  _NEURONSTATISTICS._serialized_end=5082
+  _SPIKEDESCRIPTOR._serialized_start=5084
+  _SPIKEDESCRIPTOR._serialized_end=5208
+  _SPIKEDATA._serialized_start=5210
+  _SPIKEDATA._serialized_end=5313
+  _SPIKETIMEDATA._serialized_start=5315
+  _SPIKETIMEDATA._serialized_end=5364
+  _SPIKETIMESTAMPDATA._serialized_start=5366
+  _SPIKETIMESTAMPDATA._serialized_end=5452
+  _SPIKETIMESTAMP._serialized_start=5455
+  _SPIKETIMESTAMP._serialized_end=5588
+  _SPIKETEMPLATEDESCRIPTOR._serialized_start=5591
+  _SPIKETEMPLATEDESCRIPTOR._serialized_end=5901
+  _SITESPIKETEMPLATES._serialized_start=5903
+  _SITESPIKETEMPLATES._serialized_end=5994
+  _BIOINTERFACESPIKETEMPLATESREPLY._serialized_start=5997
+  _BIOINTERFACESPIKETEMPLATESREPLY._serialized_end=6148
+  _BIOINTERFACEMETADATA._serialized_start=6150
+  _BIOINTERFACEMETADATA._serialized_end=6214
+  _BIOINTERFACESPIKEDATAREPLY._serialized_start=6217
+  _BIOINTERFACESPIKEDATAREPLY._serialized_end=6431
+  _SPIKEDATADENSECHANNELDESCRIPTOR._serialized_start=6434
+  _SPIKEDATADENSECHANNELDESCRIPTOR._serialized_end=6615
+  _SPIKESSPIKEDATADENSEREPLY._serialized_start=6618
+  _SPIKESSPIKEDATADENSEREPLY._serialized_end=6794
+  _GROUPSPIKETIMEDATAREPLY._serialized_start=6797
+  _GROUPSPIKETIMEDATAREPLY._serialized_end=6935
+  _BIOINTERFACESPIKETRAIN._serialized_start=6937
+  _BIOINTERFACESPIKETRAIN._serialized_end=7055
+  _SITESPIKETRAIN._serialized_start=7057
+  _SITESPIKETRAIN._serialized_end=7169
+  _SPIKETRAIN._serialized_start=7172
+  _SPIKETRAIN._serialized_end=7439
+  _NEURONHISTDATA._serialized_start=7442
+  _NEURONHISTDATA._serialized_end=7624
+  _SITEHISTDATA._serialized_start=7627
+  _SITEHISTDATA._serialized_end=7784
+  _BIOINTERFACEHISTDATAREPLY._serialized_start=7787
+  _BIOINTERFACEHISTDATAREPLY._serialized_end=7926
+  _BIOINTERFACESAVEREQUEST._serialized_start=7929
+  _BIOINTERFACESAVEREQUEST._serialized_end=8109
+  _BIOINTERFACELOADREQUEST._serialized_start=8112
+  _BIOINTERFACELOADREQUEST._serialized_end=8284
+  _BIOINTERFACESAVELOADREPLY._serialized_start=8287
+  _BIOINTERFACESAVELOADREPLY._serialized_end=8436
+  _BIOINTERFACEGETIDSREPLY._serialized_start=8438
+  _BIOINTERFACEGETIDSREPLY._serialized_end=8488
+  _BIOINTERFACEVIZREQUEST._serialized_start=8491
+  _BIOINTERFACEVIZREQUEST._serialized_end=8730
+  _BIOINTERFACEVIZREQUEST_VTYPE._serialized_start=8683
+  _BIOINTERFACEVIZREQUEST_VTYPE._serialized_end=8730
+  _BIOINTERFACEVIZREPLY._serialized_start=8732
+  _BIOINTERFACEVIZREPLY._serialized_end=8782
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-3.0.0b5/radiens/grpc_radiens/common_pb2.py` & `radiens-3.0.0b6/radiens/grpc_radiens/common_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x06\x61llego\x1a\x1fgoogle/protobuf/timestamp.proto\"@\n\x14OfflineLicenseStatus\x12\x12\n\nisVerified\x18\x01 \x02(\x08\x12\x14\n\x0chardwareUUID\x18\x02 \x02(\t\"C\n\x0f\x46irmwareVersion\x12\x0c\n\x04\x64\x61te\x18\x01 \x02(\t\x12\x10\n\x08majorRev\x18\x02 \x02(\x05\x12\x10\n\x08minorRev\x18\x03 \x02(\x05\"k\n\x10RadixEnvironment\x12\x0f\n\x07version\x18\x01 \x02(\t\x12\x14\n\x0cuserDataPath\x18\x02 \x02(\t\x12\x30\n\x0f\x66irmwareVersion\x18\x03 \x02(\x0b\x32\x17.allego.FirmwareVersion\"!\n\x0fStandardRequest\x12\x0e\n\x06regStr\x18\x02 \x03(\t\"/\n\rStandardReply\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\x12\x0e\n\x06regStr\x18\x02 \x03(\t\"&\n\rDACOffRequest\x12\x15\n\rstreamGroupId\x18\x01 \x01(\t\"\xba\x01\n\x13WorkspaceDescriptor\x12\n\n\x02iD\x18\x01 \x02(\t\x12!\n\x03\x61pp\x18\x02 \x02(\x0e\x32\x14.allego.WorkspaceApp\x12\x12\n\nisModified\x18\x03 \x02(\x08\x12\x19\n\x11timestampLastUsed\x18\x04 \x02(\t\x12\x19\n\x11timestampModified\x18\x05 \x02(\t\x12*\n\nannotation\x18\x06 \x02(\x0b\x32\x16.allego.AnnotateBundle\"\xb8\x01\n\x17WorkspaceControlRequest\x12&\n\x03\x63md\x18\x01 \x02(\x0e\x32\x19.allego.WorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12*\n\nannotation\x18\x03 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x1a\n\x12targetFullFileName\x18\x04 \x01(\t\x12\x18\n\x10isForceOverwrite\x18\x05 \x01(\x08\"\xd3\x01\n\x13GetWorkspaceRequest\x12)\n\x03\x63md\x18\x01 \x02(\x0e\x32\x1c.allego.GetWorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12\x14\n\x0cworkspaceDir\x18\x03 \x01(\t\x12%\n\x07\x61ppMask\x18\x04 \x01(\x0e\x32\x14.allego.WorkspaceApp\x12,\n\x0c\x61nnotateMask\x18\x05 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x11\n\tisBrowser\x18\x06 \x01(\x08\"\xab\x01\n\x11GetWorkspaceReply\x12\x43\n\rworkspaceDesc\x18\x01 \x03(\x0b\x32,.allego.GetWorkspaceReply.WorkspaceDescEntry\x1aQ\n\x12WorkspaceDescEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x1b.allego.WorkspaceDescriptor:\x02\x38\x01\"`\n\x18GetRadiensServersRequest\x12\x15\n\rhostIPaddress\x18\x01 \x02(\t\x12-\n\nserverType\x18\x02 \x01(\x0e\x32\x19.allego.RadiensServerType\"\x97\x02\n\nServerSpec\x12\x0c\n\x04host\x18\x01 \x02(\t\x12\x0b\n\x03pid\x18\x02 \x02(\x05\x12\x30\n\x07service\x18\x03 \x03(\x0b\x32\x1f.allego.ServerSpec.ServiceEntry\x12\x30\n\x05spawn\x18\x04 \x01(\x0b\x32!.allego.ServerSpec.SpawnedProcess\x1a\x1b\n\x0bGrpcService\x12\x0c\n\x04port\x18\x01 \x02(\x05\x1a\x1d\n\x0eSpawnedProcess\x12\x0b\n\x03pid\x18\x01 \x03(\x05\x1aN\n\x0cServiceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.allego.ServerSpec.GrpcService:\x02\x38\x01\"j\n\x13RadiensServersReply\x12(\n\x0c\x61llegoserver\x18\x01 \x03(\x0b\x32\x12.allego.ServerSpec\x12)\n\rradiensserver\x18\x02 \x03(\x0b\x32\x12.allego.ServerSpec\"-\n\x14SignalGroupIDRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\"\xc4\x01\n\tSignalMap\x12\x0f\n\x07siteIdx\x18\x01 \x03(\x05\x12\x13\n\x0b\x63ompSiteNum\x18\x02 \x03(\t\x12\x13\n\x0bposProbeUmX\x18\x03 \x03(\x01\x12\x13\n\x0bposProbeUmY\x18\x04 \x03(\x01\x12\x13\n\x0bposProbeUmZ\x18\x05 \x03(\x01\x12\x14\n\x0cposTissueUmX\x18\x06 \x03(\x01\x12\x14\n\x0cposTissueUmY\x18\x07 \x03(\x01\x12\x14\n\x0cposTissueUmZ\x18\x08 \x03(\x01\x12\x10\n\x08sensorID\x18\t \x03(\t\"=\n\x10GPIOChannelCount\x12\x0c\n\x04nAux\x18\x01 \x02(\x05\x12\x0c\n\x04nDin\x18\x02 \x02(\x05\x12\r\n\x05nDout\x18\x03 \x02(\x05\"D\n\x10PortChannelCount\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"Q\n\x0eSetPortRequest\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x10\n\x08probeUID\x18\x02 \x02(\t\x12\x11\n\thstageUID\x18\x03 \x02(\t\"\xe2\x02\n\x11HDSnapshotRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12=\n\npriSignals\x18\x03 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\nauxSignals\x18\x04 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\ndinSignals\x18\x05 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12>\n\x0b\x64outSignals\x18\x06 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x1a&\n\x0fSelectedSignals\x12\x13\n\x0bntvChanIdxs\x18\x01 \x03(\x05\"\x96\x01\n\x12HDSnapshotRequest2\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12)\n\x07selMode\x18\x03 \x01(\x0e\x32\x18.allego.TimeRangeSelMode\x12#\n\x06sigSel\x18\x04 \x01(\x0b\x32\x13.allego.SigSelector\"L\n\x15RadiensPyGraphicsArgs\x12\x12\n\ngraphicsID\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0f\n\x07\x66igSize\x18\x03 \x03(\x03\"\xdd\x02\n\nPSDRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12)\n\x07selMode\x18\x03 \x02(\x0e\x32\x18.allego.TimeRangeSelMode\x12!\n\x05stype\x18\x04 \x02(\x0e\x32\x12.allego.SignalType\x12\x0f\n\x07ntvIdxs\x18\x05 \x03(\x03\x12\x12\n\nresampleFs\x18\x06 \x01(\x01\x12&\n\x07wdwType\x18\x07 \x01(\x0e\x32\x15.allego.PSDWindowType\x12#\n\x07scaling\x18\x08 \x01(\x0e\x32\x12.allego.PSDScaling\x12\x11\n\tfreqRange\x18\t \x03(\x01\x12\x14\n\x0c\x63ollapseFreq\x18\n \x01(\x08\x12\x11\n\tdeltaFreq\x18\x0b \x01(\x01\x12\x0c\n\x04path\x18\r \x01(\t\x12\x13\n\x0bisReturnPSD\x18\x0e \x01(\x08\"\xa1\x02\n\x03PSD\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12\x1f\n\x02sG\x18\x03 \x02(\x0b\x32\x13.allego.SignalGroup\x12!\n\x05stype\x18\x04 \x02(\x0e\x32\x12.allego.SignalType\x12\x1d\n\x02tR\x18\x05 \x02(\x0b\x32\x11.allego.TimeRange\x12 \n\x03psd\x18\x06 \x02(\x0b\x32\x13.allego.DenseMatrix\x12\x0c\n\x04\x66req\x18\x07 \x03(\x01\x12\x14\n\x0c\x66reqBinWidth\x18\x08 \x02(\x01\x12\x11\n\tfreqRange\x18\x0b \x03(\x01\x12&\n\x07wdwType\x18\t \x01(\x0e\x32\x15.allego.PSDWindowType\x12#\n\x07scaling\x18\n \x01(\x0e\x32\x12.allego.PSDScaling\"e\n\x18RadiensPyGraphicsRequest\x12\x1c\n\x07psdData\x18\x01 \x01(\x0b\x32\x0b.allego.PSD\x12+\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\x1d.allego.RadiensPyGraphicsArgs\"^\n\x0bSigSelector\x12\x12\n\nampNtvIdxs\x18\x01 \x03(\x03\x12\x12\n\nainNtvIdxs\x18\x02 \x03(\x03\x12\x12\n\ndinNtvIdxs\x18\x03 \x03(\x03\x12\x13\n\x0b\x64outNtvIdxs\x18\x04 \x03(\x03\"]\n\x0eHDSnapshotMeta\x12\x11\n\tglobalMin\x18\x04 \x02(\x01\x12\x11\n\tglobalMax\x18\x05 \x02(\x01\x12%\n\x08sigGroup\x18\x06 \x01(\x0b\x32\x13.allego.SignalGroup\"\x9f\x02\n\nHDSnapshot\x12$\n\x04meta\x18\x01 \x02(\x0b\x32\x16.allego.HDSnapshotMeta\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x13\n\x0btimeSamples\x18\x03 \x02(\x0c\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12&\n\npriSignals\x18\x05 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\nauxSignals\x18\x06 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\ndinSignals\x18\x07 \x01(\x0b\x32\x12.allego.RawSignals\x12\'\n\x0b\x64outSignals\x18\x08 \x01(\x0b\x32\x12.allego.RawSignals\"@\n\x0bHDSnapshot2\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12\x1e\n\x04sigs\x18\x02 \x02(\x0b\x32\x10.allego.Signals2\"\xb9\x03\n\x11GetSignalsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x37\n\x06params\x18\x02 \x02(\x0b\x32\'.allego.GetSignalsRequest.GetSigsParams\x1a\xd3\x02\n\rGetSigsParams\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x0e\n\x06wdwSec\x18\x02 \x02(\x01\x12\x14\n\x0c\x63hanHeightPx\x18\x03 \x02(\x01\x12\x10\n\x08\x61mpFsrUv\x18\x04 \x02(\x01\x12\x17\n\x0fplotWidthPoints\x18\x05 \x02(\x01\x12\x11\n\tgpioOnTop\x18\x06 \x02(\x08\x12\x0f\n\x07\x61inFsrV\x18\x07 \x02(\x01\x12\x13\n\x0b\x63omponentID\x18\x08 \x02(\t\x12-\n\x0cresampleType\x18\t \x02(\x0e\x32\x17.allego.ResampleRoutine\x12\x11\n\tisHeatmap\x18\n \x02(\x08\x12\x1b\n\x13isNotApplyDSPstage2\x18\x0b \x01(\x08\x12\x13\n\x0b\x63lipToRange\x18\x0c \x02(\x08\x12\x17\n\x0f\x62\x61ndpassLowFreq\x18\r \x01(\x01\x12\x18\n\x10\x62\x61ndpassHighFreq\x18\x0e \x01(\x01\"[\n\nRawSignals\x12\r\n\x05shape\x18\x01 \x03(\x05\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\x12\x1d\n\x02tR\x18\x04 \x01(\x0b\x32\x11.allego.TimeRange\"\xe7\x01\n\x08Signals2\x12\x1f\n\x02sG\x18\x01 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12%\n\x03\x61mp\x18\x03 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12%\n\x03\x61in\x18\x04 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12%\n\x03\x64in\x18\x05 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12&\n\x04\x64out\x18\x06 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\"\x85\x02\n\x14ListSensorSpecsReply\x12\x41\n\x06probes\x18\x01 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\x45\n\nheadstages\x18\x02 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x1a:\n\x14SpecWithChannelCount\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"d\n\x16ListDataSourcesRequest\x12\x11\n\tdirectory\x18\x01 \x02(\t\x12&\n\x06sortBy\x18\x02 \x01(\x0e\x32\x16.allego.DataSourceSort\x12\x0f\n\x07\x64irList\x18\x03 \x03(\t\"\x1c\n\x07SortMap\x12\x11\n\tsorterIds\x18\x01 \x03(\t\">\n\x16GetSignalGroupIDsReply\x12\x12\n\ncontinuous\x18\x01 \x03(\t\x12\x10\n\x08\x64iscrete\x18\x02 \x03(\t\"\xa0\x01\n\x13GetSorterIDMapReply\x12\x43\n\x0csigToSortMap\x18\x01 \x03(\x0b\x32-.allego.GetSorterIDMapReply.SigToSortMapEntry\x1a\x44\n\x11SigToSortMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.allego.SortMap:\x02\x38\x01\"\xaf\x01\n\nDataSource\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x02(\t\x12\x17\n\x0f\x64urationSeconds\x18\x03 \x02(\x01\x12\x17\n\x0f\x64urationMinutes\x18\x04 \x02(\x01\x12\x15\n\rdurationHours\x18\x05 \x02(\x01\x12(\n\x08\x66ileType\x18\x06 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x12\n\nnumSignals\x18\x07 \x02(\x05\"o\n\x0e\x46ileDescriptor\x12\x0c\n\x04path\x18\x01 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x13\n\x0b\x66ileNameUID\x18\x04 \x01(\t\"\xd0\x01\n\x08TimeSpec\x12\x30\n\ttimeRange\x18\x01 \x01(\x0b\x32\x1b.allego.TimeSpec.TimeRangeLH\x00\x12:\n\x0etimestampRange\x18\x02 \x01(\x0b\x32 .allego.TimeSpec.TimestampRangeLH\x00\x1a\x1f\n\nTimeRangeL\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x1a)\n\x0fTimestampRangeL\x12\x16\n\x0etimestampRange\x18\x01 \x03(\x03\x42\n\n\x08timeDesc\"\xbe\x01\n\nSignalSpec\x12.\n\x07siteNum\x18\x01 \x01(\x0b\x32\x1b.allego.SignalSpec.SiteNumLH\x00\x12\x34\n\nntvChanIdx\x18\x02 \x01(\x0b\x32\x1e.allego.SignalSpec.NtvChanIdxLH\x00\x1a\x1b\n\x08SiteNumL\x12\x0f\n\x07siteNum\x18\x01 \x03(\x05\x1a!\n\x0bNtvChanIdxL\x12\x12\n\nntvChanIdx\x18\x01 \x03(\x05\x42\n\n\x08siteDesc\"\x8c\x06\n\rChannelRecord\x12\x10\n\x08\x63hanName\x18\x01 \x02(\t\x12$\n\x08\x63hanType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\x12\n\nntvChanIdx\x18\x03 \x02(\x05\x12\x0f\n\x07siteNum\x18\x04 \x02(\x05\x12\x15\n\rcolorGroupIdx\x18\x05 \x02(\x05\x12\x12\n\nisSelected\x18\x06 \x02(\x08\x12\x13\n\x0bisAudioLeft\x18\x07 \x02(\x08\x12\x1a\n\x04port\x18\x08 \x02(\x0e\x32\x0c.allego.Port\x12\x11\n\tsiteShape\x18\t \x02(\t\x12\x10\n\x08siteCtrX\x18\n \x02(\x01\x12\x10\n\x08siteCtrY\x18\x0b \x02(\x01\x12\x10\n\x08siteCtrZ\x18\x0c \x02(\x01\x12\x13\n\x0bsiteLimXMin\x18\r \x02(\x01\x12\x13\n\x0bsiteLimXMax\x18\x0e \x02(\x01\x12\x13\n\x0bsiteLimYMin\x18\x0f \x02(\x01\x12\x13\n\x0bsiteLimYMax\x18\x10 \x02(\x01\x12\x13\n\x0bsiteLimZMin\x18\x11 \x02(\x01\x12\x13\n\x0bsiteLimZMax\x18\x12 \x02(\x01\x12\x13\n\x0bsiteCtrTcsX\x18\x13 \x02(\x01\x12\x13\n\x0bsiteCtrTcsY\x18\x14 \x02(\x01\x12\x13\n\x0bsiteCtrTcsZ\x18\x15 \x02(\x01\x12\x13\n\x0bsensorUnits\x18\x16 \x02(\t\x12\x0e\n\x06\x61\x62sIdx\x18\x17 \x02(\x05\x12\x14\n\x0cisAudioRight\x18\x18 \x02(\x08\x12\x12\n\nsysChanIdx\x18\x19 \x02(\x05\x12\x17\n\x0fsiteAreaMicron2\x18\x1a \x01(\x01\x12\x11\n\tscsToTcsX\x18\x1b \x01(\x01\x12\x11\n\tscsToTcsY\x18\x1c \x01(\x01\x12\x11\n\tscsToTcsZ\x18\x1d \x01(\x01\x12\x10\n\x08sensorID\x18\x1e \x01(\t\x12\x0f\n\x07probeID\x18\x1f \x01(\t\x12\x13\n\x0bheadstageID\x18  \x01(\t\x12\x13\n\x0b\x64\x61tasetRidx\x18! \x01(\x05\x12\x13\n\x0b\x64\x61tasetAidx\x18\" \x01(\x05\x12\x13\n\x0bntvChanName\x18# \x01(\t\x12\x11\n\tsensorUID\x18$ \x01(\t\x12\x11\n\tsensorIdx\x18% \x01(\x05\"\x1f\n\x07XYCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"+\n\x08XYZCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\x12\t\n\x01z\x18\x03 \x02(\x01\"\x81\x03\n\x06Sensor\x12\x0f\n\x07probeId\x18\x01 \x02(\t\x12\x13\n\x0bheadstageId\x18\x02 \x02(\t\x12+\n\twireframe\x18\x03 \x02(\x0b\x32\x18.allego.Sensor.WireFrame\x12\x0c\n\x04xMin\x18\x04 \x02(\x01\x12\x0c\n\x04xMax\x18\x05 \x02(\x01\x12\x0c\n\x04yMin\x18\x06 \x02(\x01\x12\x0c\n\x04yMax\x18\x07 \x02(\x01\x12+\n\x08position\x18\x08 \x02(\x0b\x32\x19.allego.SensorPositionTcs\x12\x11\n\tsensorUID\x18\t \x01(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\n \x01(\x05\x12\x10\n\x08numSites\x18\x0b \x02(\x05\x12\x11\n\tsensorIdx\x18\x0c \x01(\x05\x1am\n\tWireFrame\x12\x1c\n\x03vtx\x18\x01 \x03(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxXlim\x18\x02 \x02(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxYlim\x18\x03 \x02(\x0b\x32\x0f.allego.XYCoord\"\x98\x02\n\x0eSensorPortSpec\x12\x1f\n\x07sensorA\x18\x01 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorB\x18\x02 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorC\x18\x03 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorD\x18\x04 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorE\x18\x05 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorF\x18\x06 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorG\x18\x07 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorH\x18\x08 \x03(\x0b\x32\x0e.allego.Sensor\"t\n\x10SignalGroupUnits\x12\x32\n\x05units\x18\x01 \x03(\x0b\x32#.allego.SignalGroupUnits.UnitsEntry\x1a,\n\nUnitsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\x80\x02\n\x0bSignalGroup\x12\'\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x15.allego.ChannelRecord\x12.\n\x0esensorPortSpec\x18\x02 \x02(\x0b\x32\x16.allego.SensorPortSpec\x12\x12\n\ndatasetUID\x18\x03 \x01(\t\x12\x10\n\x08sampFreq\x18\x04 \x01(\x01\x12\x13\n\x0bsourceLabel\x18\x05 \x01(\t\x12\x19\n\x11neighborMaxRadius\x18\x06 \x01(\x01\x12-\n\x0bsignalUnits\x18\x07 \x01(\x0b\x32\x18.allego.SignalGroupUnits\x12\x13\n\x0bhasDiscrete\x18\x08 \x01(\x08\"\x87\x01\n\x18\x43reateSignalGroupRequest\x12\x16\n\x0e\x64\x61taSourceName\x18\x01 \x02(\t\x12\x16\n\x0e\x64\x61taSourcePath\x18\x02 \x02(\t\x12$\n\x04type\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x15\n\rstreamGroupId\x18\x04 \x02(\t\"s\n\tSubOpSort\x12)\n\x04sort\x18\x01 \x03(\x0e\x32\x1b.allego.SubOpSort.SortField\";\n\tSortField\x12\x0e\n\nSITE_CTR_X\x10\x00\x12\x0e\n\nSITE_CTR_Y\x10\x01\x12\x0e\n\nSITE_CTR_Z\x10\x02\"\xa5\x03\n\x18UpdateSignalGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12=\n\toperation\x18\x02 \x02(\x0e\x32*.allego.UpdateSignalGroupRequest.Operation\x12\x42\n\taddRemove\x18\x03 \x01(\x0e\x32-.allego.UpdateSignalGroupRequest.SubOperationH\x00\x12#\n\x06sortOp\x18\x04 \x01(\x0b\x32\x11.allego.SubOpSortH\x00\x12\x16\n\nntvChanIdx\x18\x05 \x03(\x05\x42\x02\x10\x01\x12&\n\nsignalType\x18\x06 \x02(\x0e\x32\x12.allego.SignalType\x12\x11\n\tpropagate\x18\x07 \x01(\x08\"B\n\tOperation\x12\t\n\x05\x43OLOR\x10\x00\x12\n\n\x06SELECT\x10\x01\x12\x14\n\x10\x44\x45PRECATED_AUDIO\x10\x02\x12\x08\n\x04SORT\x10\x03\"#\n\x0cSubOperation\x12\x07\n\x03\x41\x44\x44\x10\x00\x12\n\n\x06REMOVE\x10\x01\x42\x0e\n\x0csubOperation\"T\n\x14SliceSignalGroupSpec\x12\x0e\n\x06sortBy\x18\x01 \x02(\t\x12\r\n\x05\x64\x65lim\x18\x02 \x02(\t\x12\x1d\n\x02tR\x18\x03 \x01(\x0b\x32\x11.allego.TimeRange\"X\n\x17SliceSignalGroupRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12*\n\x04spec\x18\x02 \x02(\x0b\x32\x1c.allego.SliceSignalGroupSpec\"\x88\x01\n\x15SliceSignalGroupReply\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12*\n\x04spec\x18\x02 \x02(\x0b\x32\x1c.allego.SliceSignalGroupSpec\x12\x1f\n\x02sG\x18\x03 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x0f\n\x07outcome\x18\x04 \x02(\t\"\x0f\n\rLicenseStatus\"u\n\x12SetDSPGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12$\n\tdspParams\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"\xf2\x02\n\tDSPParams\x12\x1d\n\x04type\x18\x01 \x02(\x0e\x32\x0f.allego.DSPType\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12\x0e\n\x04\x66req\x18\x03 \x01(\x01H\x00\x12\x36\n\x0c\x66reqSpecBand\x18\x04 \x01(\x0b\x32\x1e.allego.DSPParams.FreqSpecBandH\x00\x12\x17\n\rrefNtvChanIdx\x18\x08 \x01(\x05H\x00\x12\x16\n\x0enotchBandwidth\x18\x05 \x01(\x01\x12\x11\n\tuserLabel\x18\x06 \x02(\t\x12\x1a\n\x04port\x18\x07 \x02(\x0e\x32\x0c.allego.Port\x12\x18\n\x10targetNtvChanIdx\x18\t \x01(\x01\x12\r\n\x05isAux\x18\n \x02(\x08\x12\x12\n\nauxChanIdx\x18\x0b \x01(\x05\x1a\x31\n\x0c\x46reqSpecBand\x12\x0f\n\x07lowFreq\x18\x01 \x02(\x01\x12\x10\n\x08highFreq\x18\x02 \x02(\x01\x42\n\n\x08\x66reqSpec\"\x85\x01\n\x08\x44SPGroup\x12#\n\x08hardware\x18\x01 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage1\x18\x02 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage2\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"\x9a\x01\n\x10SetSensorRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07probeId\x18\x03 \x01(\t\x12\x13\n\x0bheadstageId\x18\x04 \x01(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\x05 \x01(\x05\x12\x13\n\x0bnumChannels\x18\x06 \x01(\x05\"m\n\x11SensorPositionTcs\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\x12\x11\n\tRingAngle\x18\x05 \x02(\x01\x12\x12\n\nAxialAngle\x18\x06 \x02(\x01\x12\x10\n\x08\x41rcAngle\x18\x07 \x02(\x01\"\x90\x01\n\x1bSetSensorPositionTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12+\n\x08position\x18\x03 \x02(\x0b\x32\x19.allego.SensorPositionTcs\x12\x11\n\tsensorIdx\x18\x04 \x01(\x05\"F\n\x0fSitePositionTcs\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\"\x7f\n\x1aSetSitePositionsTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12.\n\rsitePositions\x18\x03 \x03(\x0b\x32\x17.allego.SitePositionTcs\"Y\n\x17\x46\x65\x61tureStartStopRequest\x12\x0e\n\x06nodeId\x18\x01 \x02(\t\x12.\n\x0e\x66\x65\x61tureLicense\x18\x02 \x02(\x0e\x32\x16.allego.FeatureLicense\"!\n\x0cPrivacyReply\x12\x11\n\tisPrivate\x18\x02 \x02(\x08\"&\n\x11SetPrivacyRequest\x12\x11\n\tisPrivate\x18\x01 \x02(\x08\"7\n\x0b\x44\x65nseMatrix\x12\x0c\n\x04rows\x18\x01 \x02(\x03\x12\x0c\n\x04\x63ols\x18\x02 \x02(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\"\\\n\tHistogram\x12\r\n\x05stats\x18\x01 \x03(\x01\x12\x0e\n\x06\x63ounts\x18\x02 \x03(\x01\x12\x10\n\x08\x64ividers\x18\x03 \x03(\x01\x12\x0f\n\x07numBins\x18\x04 \x02(\x03\x12\r\n\x05isPDF\x18\x05 \x02(\x08\"Y\n\x0bKpiMetricID\x12$\n\x04mode\x18\x01 \x02(\x0e\x32\x16.allego.KpiMetricsMode\x12$\n\x04name\x18\x02 \x02(\x0e\x32\x16.allego.KpiMetricsEnum\"\x85\x01\n\tTimeRange\x12\x14\n\x0ctimeRangeSec\x18\x01 \x03(\x01\x12\x11\n\ttimestamp\x18\x02 \x03(\x03\x12\n\n\x02\x66s\x18\x03 \x02(\x01\x12\x15\n\rwallTimeStart\x18\x04 \x01(\t\x12,\n\x08wallTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"q\n\tBundleReq\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12$\n\x07metrics\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0e\n\x06isTail\x18\x05 \x02(\x08\"\x9d\x01\n\rKpiMetricsReq\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x1e\n\x03\x61rg\x18\x03 \x02(\x0b\x32\x11.allego.BundleReq\x12\x0e\n\x06isPlot\x18\x04 \x01(\x08\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x14\n\x0cisReturnData\x18\x06 \x01(\x08\"\x83\x03\n\x0eKpiMetricsData\x12\x12\n\nnumPackets\x18\x01 \x02(\x03\x12\x0f\n\x07numSigs\x18\x02 \x02(\x03\x12\x12\n\nnumMetrics\x18\x03 \x02(\x03\x12#\n\x06metric\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0f\n\x07pktIdxs\x18\x05 \x03(\x03\x12 \n\x03val\x18\x06 \x02(\x0b\x32\x13.allego.DenseMatrix\x12\x35\n\tstatsPkts\x18\x07 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x31\n\x05stats\x18\x08 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x14\n\x0cpacketDurSec\x18\t \x02(\x01\x12\x1d\n\x02tR\x18\n \x02(\x0b\x32\x11.allego.TimeRange\x1a\x41\n\x0bMetricStats\x12\x0c\n\x04mean\x18\x01 \x03(\x01\x12\n\n\x02sD\x18\x02 \x03(\x01\x12\x0b\n\x03max\x18\x03 \x03(\x01\x12\x0b\n\x03min\x18\x04 \x03(\x01\"w\n\x16KpiBundlePacketMetrics\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12#\n\x07sigType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\'\n\x07metrics\x18\x04 \x02(\x0b\x32\x16.allego.KpiMetricsData\"S\n\nKpiMetrics\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12.\n\x06\x62undle\x18\x02 \x02(\x0b\x32\x1e.allego.KpiBundlePacketMetrics\"c\n\x11KpiControlRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x14\n\x0cisAllBundles\x18\x03 \x01(\x08\":\n\x12SetKpiParamRequest\x12\x15\n\rstreamGroupId\x18\x01 \x01(\t\x12\r\n\x05param\x18\x02 \x01(\x01\",\n\x13GetKpiStatusRequest\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\"K\n\x12KpiStandardRequest\x12\x11\n\tdsourceID\x18\x02 \x03(\t\x12\"\n\x03\x63md\x18\x03 \x01(\x0e\x32\x15.allego.KpiScannerCmd\"\xba\x01\n\rKpiFileStatus\x12,\n\x07\x64source\x18\x01 \x03(\x0b\x32\x1b.allego.KpiFileStatus.State\x1a{\n\x05State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\nisComplete\x18\x02 \x01(\x08\x12\x12\n\ndsourceUID\x18\x03 \x01(\t\x12 \n\x05kpiTR\x18\x04 \x01(\x0b\x32\x11.allego.TimeRange\x12\x17\n\x0f\x66ilePathAndName\x18\x05 \x01(\t\"\xc7\x04\n\x0eKpiFileStatus2\x12>\n\x07\x64source\x18\x01 \x03(\x0b\x32-.allego.KpiFileStatus2.KpiDatasourceStateSpec\x1a\xe9\x01\n\tKPI_State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\nisComplete\x18\x02 \x01(\x08\x12\x14\n\x0c\x66racComplete\x18\x03 \x01(\x01\x12\x17\n\x0f\x66ilePathAndName\x18\x04 \x01(\t\x12 \n\x05kpiTR\x18\x05 \x01(\x0b\x32\x11.allego.TimeRange\x12\x14\n\x0cpacketDurSec\x18\x06 \x01(\x01\x12\x0e\n\x06numAmp\x18\x07 \x01(\x03\x12\x18\n\x10\x62ytesInBundlePkt\x18\x08 \x01(\x03\x12\x12\n\nnumPackets\x18\t \x01(\x03\x12\x12\n\ndatasetUID\x18\n \x01(\t\x1aq\n\x10\x44\x61tasource_State\x12\x17\n\x0f\x66ilePathAndName\x18\x01 \x01(\t\x12\x1d\n\x02TR\x18\x02 \x01(\x0b\x32\x11.allego.TimeRange\x12\x12\n\ndatasetUID\x18\x03 \x01(\t\x12\x11\n\tdsourceID\x18\x04 \x01(\t\x1a\x95\x01\n\x16KpiDatasourceStateSpec\x12\x37\n\x06source\x18\x01 \x02(\x0b\x32\'.allego.KpiFileStatus2.Datasource_State\x12-\n\x03kpi\x18\x02 \x02(\x0b\x32 .allego.KpiFileStatus2.KPI_State\x12\x13\n\x0bisSprinting\x18\x03 \x02(\x08\"\xfd\x01\n\x0fKpiFileMetadata\x12.\n\x07\x64source\x18\x01 \x03(\x0b\x32\x1d.allego.KpiFileMetadata.State\x1a\xb9\x01\n\x05State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\ndsourceUID\x18\x02 \x01(\t\x12\x11\n\tpacketDur\x18\x03 \x01(\x01\x12\x0c\n\x04nAMP\x18\x04 \x01(\x03\x12\x1b\n\x13\x62ytesInBundlePacket\x18\x05 \x01(\x03\x12\x12\n\nnumPackets\x18\x06 \x01(\x03\x12 \n\x05kpiTR\x18\x07 \x01(\x0b\x32\x11.allego.TimeRange\x12\x17\n\x0f\x66ilePathAndName\x18\x08 \x01(\t\"\xd3\x02\n\x0eKpiStatusReply\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x11\n\ttimeRange\x18\x03 \x01(\x01\x12\x16\n\x0etimestampRange\x18\x04 \x01(\x03\x12\x18\n\x10numPacketsMemory\x18\x05 \x02(\x03\x12\x11\n\tpacketDur\x18\x06 \x02(\x01\x12\x14\n\x0cupdatePeriod\x18\x07 \x02(\x01\x12\x13\n\x0bpersistence\x18\x08 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\t \x02(\x01\x12\x1d\n\x15isTrackingSignalCache\x18\x0b \x02(\x08\x12\x12\n\nnumPackets\x18\x0c \x02(\x03\x12\x13\n\x0bmemoryBytes\x18\r \x02(\x01\x12\n\n\x02\x66s\x18\x0e \x01(\x01\x12\x15\n\rwallTimeStart\x18\x0f \x01(\t\x12\x1d\n\x02tR\x18\x10 \x01(\x0b\x32\x11.allego.TimeRange\x12\x0f\n\x07numSigs\x18\x11 \x01(\x03\"\xe6\x02\n\x11SigKpiParamRecord\x12\x15\n\risEventDetect\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x11\n\teventThr0\x18\x03 \x02(\x01\x12\x11\n\teventThr1\x18\x04 \x02(\x01\x12\x13\n\x0b\x65ventThrSd0\x18\x05 \x02(\x01\x12\x13\n\x0b\x65ventThrSd1\x18\x06 \x02(\x01\x12\x11\n\tpreThrPts\x18\x07 \x02(\x05\x12\x12\n\npostThrPts\x18\x08 \x02(\x05\x12\x11\n\tevtDurPts\x18\t \x02(\x05\x12\x11\n\tshadowPts\x18\n \x02(\x05\x12\x0e\n\x06preThr\x18\x0b \x02(\x01\x12\x0f\n\x07postThr\x18\x0c \x02(\x01\x12\x0e\n\x06\x65vtDur\x18\r \x02(\x01\x12\x0e\n\x06shadow\x18\x0e \x02(\x01\x12\x11\n\tisSetThr0\x18\x0f \x02(\x08\x12\x11\n\tisSetThr1\x18\x10 \x02(\x08\x12\x10\n\x08isSDThr0\x18\x11 \x02(\x08\x12\x10\n\x08isSDThr1\x18\x12 \x02(\x08\"J\n\x0e\x41nnotateBundle\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\r\n\x05notes\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x01(\t\"]\n\x0fProjectMetadata\x12\x12\n\nprojectUID\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61seUID\x18\x02 \x01(\t\x12\x10\n\x08trialUID\x18\x03 \x01(\t\x12\x13\n\x0b\x61nnotateUID\x18\x04 \x03(\t\"3\n\x16SensorExtendedMetadata\x12\x19\n\x11sensorInstanceUID\x18\x01 \x01(\t\"%\n\x0fGonumMatrixList\x12\x12\n\nmdataBytes\x18\x01 \x02(\x0c\"6\n\x0fRadixMatrixList\x12#\n\x06matrix\x18\x01 \x03(\x0b\x32\x13.allego.RadixMatrix\"*\n\x0bRadixMatrix\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\x12\r\n\x05shape\x18\x02 \x03(\x05\"/\n\x10RadixMatrixBytes\x12\x0c\n\x04\x64\x61ta\x18\x01 \x02(\x0c\x12\r\n\x05shape\x18\x02 \x03(\x05\"8\n\x10RadixSignalsList\x12$\n\x06matrix\x18\x01 \x03(\x0b\x32\x14.allego.RadixSignals\"\xa9\x01\n\x0cRadixSignals\x12\x10\n\x08sampFreq\x18\x01 \x02(\x01\x12 \n\x03pri\x18\x02 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x61ux\x18\x03 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x64in\x18\x04 \x02(\x0b\x32\x13.allego.RadixMatrix\x12!\n\x04\x64out\x18\x05 \x02(\x0b\x32\x13.allego.RadixMatrix\"\x19\n\x0cVectorString\x12\t\n\x01x\x18\x01 \x03(\t\"\x1a\n\rVectorFloat64\x12\t\n\x01x\x18\x01 \x03(\x01\"G\n\x12VectorSliceFloat64\x12\"\n\x03vec\x18\x01 \x03(\x0b\x32\x15.allego.VectorFloat64\x12\r\n\x05label\x18\x02 \x01(\t\"\xde\x02\n\x14LogsysKpiStatusReply\x12\x1f\n\x05portA\x18\x01 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portB\x18\x02 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portC\x18\x03 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portD\x18\x04 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portE\x18\x05 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portF\x18\x06 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portG\x18\x07 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portH\x18\x08 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux0\x18\t \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux1\x18\n \x02(\x0b\x32\x10.allego.KpiCache\"\xfc\x02\n\x08KpiCache\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x15\n\rminNumPackets\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x05\x12\x12\n\nnumPackets\x18\x06 \x02(\x05\x12\x0e\n\x06tRange\x18\x07 \x03(\x01\x12\x0f\n\x07tsRange\x18\x08 \x03(\x03\x12\x15\n\rmeanPacketDur\x18\t \x02(\x01\x12\x19\n\x11meanCalcPacketDur\x18\n \x02(\x01\x12\x11\n\tpacketDur\x18\x0b \x02(\x01\x12\x1d\n\x15totalPacketsProcessed\x18\x0c \x02(\r\x12\x12\n\nsignalType\x18\r \x02(\t\x12\x12\n\nnumPriSigs\x18\x0e \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x0f \x02(\x05\x12\x12\n\nnumDinSigs\x18\x10 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x11 \x02(\x05\x12\x14\n\x0cupdatePeriod\x18\x12 \x02(\x01\"\xfa\x02\n\x12LogsysKpiTailReply\x12\"\n\x05portA\x18\x01 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portB\x18\x02 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portC\x18\x03 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portD\x18\x04 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portE\x18\x05 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portF\x18\x06 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portG\x18\x07 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portH\x18\x08 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux0\x18\t \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux1\x18\n \x01(\x0b\x32\x13.allego.KpiPortInfo\"3\n\x0bKpiPortInfo\x12$\n\x07kpiTail\x18\x01 \x03(\x0b\x32\x13.allego.KpiTailRows\"\xf4\x02\n\x0bKpiTailRows\x12\x10\n\x08wallTime\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x02(\x01\x12\x14\n\x0clocalSigType\x18\x03 \x02(\t\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x03\x12\x0b\n\x03\x64ur\x18\x05 \x02(\x01\x12\x0e\n\x06stdDev\x18\x06 \x02(\x01\x12\x0f\n\x07\x63StdDev\x18\x07 \x02(\x01\x12\x11\n\tabsEvtAmp\x18\x08 \x02(\x01\x12\x12\n\ncabsEvtAmp\x18\t \x02(\x01\x12\x0b\n\x03SNR\x18\n \x02(\x01\x12\x0c\n\x04\x63SNR\x18\x0b \x02(\x01\x12\x0f\n\x07numEvts\x18\x0c \x02(\x05\x12\x10\n\x08\x63numEvts\x18\r \x02(\x05\x12\x0f\n\x07\x65vtRate\x18\x0e \x02(\x01\x12\x10\n\x08\x63\x45vtRate\x18\x0f \x02(\x01\x12\x0b\n\x03max\x18\x10 \x02(\x01\x12\x0c\n\x04\x63max\x18\x11 \x02(\x01\x12\x0b\n\x03min\x18\x12 \x02(\x01\x12\x0c\n\x04\x63min\x18\x13 \x02(\x01\x12\x14\n\x0cmeanPosPkAmp\x18\x14 \x02(\x01\x12\x14\n\x0cmeanNegPkAmp\x18\x15 \x02(\x01\"*\n\x18WarehouseHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\"(\n\x19OutfitterGetDeviceRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x9e\x01\n\x11SensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x16\n\x0eisIncludeModel\x18\x03 \x01(\x08\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"z\n\x19RegisterSensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x11\n\tprofileID\x18\x03 \x02(\t\"\x92\x01\n\x1dSaveSensorCompInstanceRequest\x12 \n\x05probe\x18\x01 \x01(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x01(\x0b\x32\x15.allego.HeadstageDesc\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"&\n\tProbeDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"*\n\rHeadstageDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"`\n\x12GetSensorCompReply\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeSpec\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageSpec\"x\n\tProbeSpec\x12\x1f\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x11.allego.ProbeDesc\x12!\n\x05model\x18\x02 \x01(\x0b\x32\x12.allego.ProbeModel\x12\'\n\x08metaData\x18\x03 \x01(\x0b\x32\x15.allego.ProbeMetaData\"\x88\x01\n\rHeadstageSpec\x12#\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x15.allego.HeadstageDesc\x12%\n\x05model\x18\x02 \x01(\x0b\x32\x16.allego.HeadstageModel\x12+\n\x08metaData\x18\x03 \x01(\x0b\x32\x19.allego.HeadstageMetaData\"\xce\x04\n\nProbeModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12.\n\x04site\x18\x02 \x03(\x0b\x32 .allego.ProbeModel.ProbeSiteDesc\x12\x34\n\twireframe\x18\x03 \x02(\x0b\x32!.allego.ProbeModel.ProbeWireFrame\x12\x34\n\x0esiteOverallMin\x18\x05 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x34\n\x0esiteOverallMax\x18\x06 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x1a\xde\x01\n\rProbeSiteDesc\x12\x0c\n\x04\x61rea\x18\x01 \x02(\x01\x12\x0f\n\x07\x63\x65nterX\x18\x02 \x02(\x01\x12\x0f\n\x07\x63\x65nterY\x18\x03 \x02(\x01\x12\x0f\n\x07\x63\x65nterZ\x18\x04 \x02(\x01\x12\x11\n\tlimitXMax\x18\x05 \x02(\x01\x12\x11\n\tlimitXMin\x18\x06 \x02(\x01\x12\x11\n\tlimitYMax\x18\x07 \x02(\x01\x12\x11\n\tlimitYMin\x18\x08 \x02(\x01\x12\x11\n\tlimitZMax\x18\t \x02(\x01\x12\x11\n\tlimitZMin\x18\n \x02(\x01\x12\x0b\n\x03num\x18\x0b \x02(\x03\x12\r\n\x05shape\x18\x0c \x02(\t\x1a^\n\x0eProbeWireFrame\x12,\n\x06vertex\x18\x01 \x03(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x0e\n\x06limitX\x18\x02 \x03(\x01\x12\x0e\n\x06limitY\x18\x03 \x03(\x01\x1a!\n\tProbePtXY\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"_\n\rProbeMetaData\x12\x11\n\tprobeName\x18\x01 \x02(\t\x12\x10\n\x08numSites\x18\x02 \x02(\x05\x12\x13\n\x0b\x63\x61talogTags\x18\x03 \x02(\t\x12\x14\n\x0cinstanceTags\x18\x04 \x02(\t\"\x84\x01\n\x0eHeadstageModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12\x31\n\x04rows\x18\x02 \x03(\x0b\x32#.allego.HeadstageModel.HeadstageRow\x1a\x33\n\x0cHeadstageRow\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x03\x12\x0f\n\x07siteNum\x18\x02 \x02(\x03\"\x13\n\x11HeadstageMetaData\"5\n\x0bUserProfile\x12\x11\n\tprofileID\x18\x01 \x02(\t\x12\x13\n\x0blicenseCode\x18\x02 \x02(\t\"B\n\x16GetCurrentProfileReply\x12(\n\x0buserProfile\x18\x01 \x02(\x0b\x32\x13.allego.UserProfile\"@\n\x13GetAllProfilesReply\x12)\n\x0cuserProfiles\x18\x01 \x03(\x0b\x32\x13.allego.UserProfile\"-\n\x18SetCurrentProfileRequest\x12\x11\n\tprofileID\x18\x01 \x02(\t\"\x88\x01\n\x14ManageNodeOrgPayload\x12\r\n\x05orgID\x18\x01 \x01(\t\x12\x0f\n\x07orgName\x18\x02 \x01(\t\x12\x14\n\x0corgShortName\x18\x03 \x01(\t\x12\x0c\n\x04\x63ity\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\r\n\x05state\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"i\n\x14ManageNodeOrgRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\"S\n\x12ManageNodeOrgReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\xa2\x01\n\x14ManageNodeLabPayload\x12\r\n\x05labID\x18\x01 \x01(\t\x12\x0f\n\x07labDesc\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65pt\x18\x03 \x01(\t\x12\x14\n\x0corganization\x18\x04 \x01(\t\x12\x0f\n\x07\x61\x64minID\x18\x05 \x01(\t\x12\x11\n\tlabHeadID\x18\x06 \x01(\t\x12\x14\n\x0clabManagerID\x18\x07 \x01(\t\x12\x0c\n\x04tags\x18\x08 \x01(\t\"i\n\x14ManageNodeLabRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\"S\n\x12ManageNodeLabReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\x99\x01\n\x15ManageNodeUserPayload\x12\x0e\n\x06userID\x18\x01 \x01(\t\x12\x0c\n\x04Name\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\x0c\x12\"\n\x04role\x18\x04 \x01(\x0e\x32\x14.allego.UserRoleType\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x0f\n\x07labName\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"k\n\x15ManageNodeUserRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12.\n\x07payload\x18\x02 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\"U\n\x13ManageNodeUserReply\x12.\n\x07payload\x18\x01 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"6\n\x13\x43\x61talogProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"]\n\x10ProbeNodeRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12%\n\x07payload\x18\x02 \x03(\x0b\x32\x14.allego.ProbePayload\"7\n\x0eProbeNodeReply\x12%\n\x07payload\x18\x01 \x03(\x0b\x32\x14.allego.ProbePayload\"/\n\x0cProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"\xa5\x02\n\x0b\x45\x64gePayload\x12/\n\x06source\x18\x01 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12/\n\x06target\x18\x02 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12)\n\tedgeLabel\x18\x03 \x02(\x0e\x32\x16.allego.WorldEdgeLabel\x12-\n\tdirection\x18\x04 \x02(\x0e\x32\x1a.allego.WorldEdgeDirection\x1aZ\n\x0bGenericNode\x12%\n\x05label\x18\x01 \x02(\x0e\x32\x16.allego.WorldNodeLabel\x12\x11\n\tidPropKey\x18\x02 \x02(\t\x12\x11\n\tidPropVal\x18\x03 \x02(\t\"8\n\x10WorldEdgeRequest\x12$\n\x07payload\x18\x01 \x03(\x0b\x32\x13.allego.EdgePayload\"\x10\n\x0eWorldEdgeReply\"E\n\x11QueryWorldRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.WorldQueryCmd\x12\x0c\n\x04\x61rgs\x18\x02 \x03(\t\"\xe6\x01\n\rQueryWorldRec\x12)\n\x03org\x18\x01 \x01(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12)\n\x03lab\x18\x02 \x01(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12+\n\x04user\x18\x03 \x01(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12-\n\x08\x63\x61tProbe\x18\x04 \x01(\x0b\x32\x1b.allego.CatalogProbePayload\x12#\n\x05probe\x18\x05 \x01(\x0b\x32\x14.allego.ProbePayload\"9\n\x0fQueryWorldReply\x12&\n\x07payload\x18\x01 \x03(\x0b\x32\x15.allego.QueryWorldRec\"/\n\x1aHighLowPassTransformParams\x12\x11\n\tfrequency\x18\x01 \x02(\x01\"B\n\x13\x42\x61ndTransformParams\x12\x14\n\x0clowFrequency\x18\x01 \x02(\x01\x12\x15\n\rhighFrequency\x18\x02 \x02(\x01\"F\n\x14NotchTransformParams\x12\x16\n\x0enotchFrequency\x18\x01 \x02(\x01\x12\x16\n\x0enotchBandwidth\x18\x02 \x02(\x01\"\x14\n\x12\x43\x41RTransformParams\"2\n\x19VirtualRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\"K\n\x18PairedRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\x12\x18\n\x10targetNtvChanIdx\x18\x02 \x02(\x05\"i\n\x1d\x44\x61taSourceSinkTransformParams\x12\x10\n\x08\x64srcName\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\">\n\x18SliceTimeTransformParams\x12\x11\n\ttimeStart\x18\x01 \x02(\x01\x12\x0f\n\x07timeEnd\x18\x02 \x02(\x01\"n\n\x1cSliceChannelsTransformParams\x12\x13\n\x0bsysChanIdxs\x18\x01 \x03(\x05\x12(\n\x0bsignalGroup\x18\x02 \x01(\x0b\x32\x13.allego.SignalGroup\x12\x0f\n\x07\x64srcUid\x18\x03 \x01(\t\"1\n\x19\x44ownsampleTransformParams\x12\x14\n\x0csampleFactor\x18\x01 \x02(\x05\"\xec\x01\n\x1aRemapSensorTransformParams\x12>\n\x07sensors\x18\x01 \x03(\x0b\x32-.allego.RemapSensorTransformParams.SensorSpec\x12\x0f\n\x07\x64srcUid\x18\x03 \x01(\t\x1a}\n\nSensorSpec\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07probeId\x18\x03 \x02(\t\x12\x13\n\x0bheadstageId\x18\x04 \x02(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\x05 \x01(\x05\x12\x13\n\x0bnumChannels\x18\x06 \x01(\x05\" \n\x08Position\x12\t\n\x01x\x18\x01 \x02(\x05\x12\t\n\x01y\x18\x02 \x02(\x05\"\x98\x06\n\rTransformNode\x12\n\n\x02id\x18\x01 \x02(\t\x12\'\n\x04type\x18\x02 \x02(\x0e\x32\x19.allego.TransformNodeType\x12\"\n\x08position\x18\x03 \x01(\x0b\x32\x10.allego.Position\x12\x0f\n\x07invalid\x18\x04 \x02(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x05 \x01(\t\x12=\n\x11highLowPassParams\x18\x06 \x01(\x0b\x32\".allego.HighLowPassTransformParams\x12/\n\nbandParams\x18\x07 \x01(\x0b\x32\x1b.allego.BandTransformParams\x12\x31\n\x0bnotchParams\x18\x08 \x01(\x0b\x32\x1c.allego.NotchTransformParams\x12-\n\tcarParams\x18\t \x01(\x0b\x32\x1a.allego.CARTransformParams\x12;\n\x10virtualRefParams\x18\n \x01(\x0b\x32!.allego.VirtualRefTransformParams\x12\x39\n\x0fpairedRefParams\x18\x0b \x01(\x0b\x32 .allego.PairedRefTransformParams\x12\x43\n\x14\x64\x61tasourceSinkParams\x18\x0c \x01(\x0b\x32%.allego.DataSourceSinkTransformParams\x12\x39\n\x0fsliceTimeParams\x18\r \x01(\x0b\x32 .allego.SliceTimeTransformParams\x12\x41\n\x13sliceChannelsParams\x18\x0e \x01(\x0b\x32$.allego.SliceChannelsTransformParams\x12;\n\x10\x64ownsampleParams\x18\x0f \x01(\x0b\x32!.allego.DownsampleTransformParams\x12=\n\x11remapSensorParams\x18\x10 \x01(\x0b\x32\".allego.RemapSensorTransformParams\";\n\rTransformEdge\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0e\n\x06source\x18\x02 \x02(\t\x12\x0e\n\x06target\x18\x03 \x02(\t\"t\n\x08Protocol\x12\n\n\x02id\x18\x01 \x02(\t\x12-\n\x0etransformNodes\x18\x02 \x03(\x0b\x32\x15.allego.TransformNode\x12-\n\x0etransformEdges\x18\x03 \x03(\x0b\x32\x15.allego.TransformEdge\"%\n\x0fProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\"B\n\x15RenameProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\x12\x15\n\rnewProtocolID\x18\x02 \x02(\t\";\n\x14GetAllProtocolsReply\x12#\n\tprotocols\x18\x01 \x03(\x0b\x32\x10.allego.Protocol\"{\n\x15\x41pplyProtocolProgress\x12\x1c\n\x14lastTimestampWritten\x18\x01 \x02(\x05\x12\x18\n\x10\x64srcTimestampEnd\x18\x02 \x02(\x05\x12\x14\n\x0c\x66racComplete\x18\x03 \x01(\x01\x12\x14\n\x0cincrementSec\x18\x04 \x01(\x01\"\x9a\x01\n\x1aSpikeSorterSetParamRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12,\n\x03\x63md\x18\x02 \x02(\x0e\x32\x1f.allego.SpikeSorterParamCommand\x12\x12\n\nregFloat64\x18\x03 \x03(\x01\x12\x0f\n\x07regBool\x18\x05 \x03(\x08\x12\x12\n\nntvChanIdx\x18\x06 \x03(\x05\"Q\n\x1bSpikeSorterSetParamsRequest\x12\x32\n\x06params\x18\x01 \x03(\x0b\x32\".allego.SpikeSorterSetParamRequest\"\xa7\x02\n\x1dSpikeSorterParamCommandRecord\x12\x11\n\tisEnabled\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x0b\n\x03thr\x18\x03 \x03(\x01\x12\r\n\x05thrSd\x18\x04 \x03(\x01\x12\x11\n\tthrWdwPts\x18\x05 \x03(\x05\x12\x0e\n\x06thrWdw\x18\x06 \x03(\x01\x12\x0e\n\x06shadow\x18\x07 \x02(\x01\x12\x11\n\tshadowPts\x18\x08 \x02(\x05\x12\x10\n\x08isSetThr\x18\t \x03(\x08\x12\x0f\n\x07weakThr\x18\n \x03(\x01\x12\x11\n\tweakThrSd\x18\x0b \x03(\x01\x12\x14\n\x0cisSetWeakThr\x18\x0c \x03(\x08\x12\x12\n\npeakWdwPts\x18\r \x03(\x05\x12\x0f\n\x07peakWdw\x18\x0e \x03(\x01\x12\x0c\n\x04isSD\x18\x0f \x02(\x08\"?\n\tKpiParams\x12\x32\n\x03rec\x18\x01 \x03(\x0b\x32%.allego.SpikeSorterParamCommandRecord\"J\n\x10\x44\x41\x43StreamRequest\x12\x0b\n\x03\x44\x41\x43\x18\x01 \x02(\x05\x12\x12\n\nNtvChanIdx\x18\x02 \x02(\x05\x12\x15\n\rstreamGroupId\x18\x03 \x01(\t\"\xde\x01\n\x11\x45ventViewerConfig\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x19\n\x11triggerSysChanIdx\x18\x03 \x01(\x05\x12\x1a\n\x12triggerThresholdUV\x18\x04 \x01(\x01\x12\x14\n\x0cpreTriggerMs\x18\x05 \x02(\x01\x12\x15\n\rpostTriggerMs\x18\x06 \x02(\x01\x12\'\n\x0btriggerType\x18\x07 \x01(\x0e\x32\x12.allego.SignalType\x12\x0e\n\x06ntvIdx\x18\x08 \x01(\x05\"=\n\rEventViewerID\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\"D\n\x1aGetEventViewerEventRequest\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x0f\n\x07\x65ventId\x18\x02 \x02(\t\"Y\n\x14\x45ventViewerEventDesc\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\"\x8f\x01\n\x10\x45ventViewerEvent\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12\x13\n\x0bsysChanIdxs\x18\x05 \x03(\x05\"a\n\x1aListEventViewerEventsReply\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12,\n\x06\x65vents\x18\x02 \x03(\x0b\x32\x1c.allego.EventViewerEventDesc\"D\n\x15ListEventViewersReply\x12+\n\x0c\x65ventViewers\x18\x01 \x03(\x0b\x32\x15.allego.EventViewerID\"3\n\x1fStatusPollFieldsToUpdateRequest\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\"^\n\x18StatusPollFieldsToUpdate\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\x12\x30\n\x0e\x66ieldsToUpdate\x18\x02 \x03(\x0e\x32\x18.allego.StatusPollFields\"\xa5\x01\n\x17\x44\x61shboardCommandRequest\x12\'\n\x08\x64\x61shType\x18\x01 \x01(\x0e\x32\x15.allego.DashboardType\x12\x32\n\x04\x61rgs\x18\x02 \x01(\x0b\x32$.allego.DashboardCommandRequest.Args\x1a-\n\x04\x41rgs\x12%\n\x03\x63md\x18\x01 \x02(\x0e\x32\x18.allego.DashboardCommand\"]\n\x13SelTableSignalGroup\x12\r\n\x05index\x18\x01 \x02(\t\x12\x15\n\rcriterionDesc\x18\x02 \x02(\t\x12\x0f\n\x07ntvIdxs\x18\x03 \x03(\x03\x12\x0f\n\x07numSigs\x18\x04 \x02(\x03\"?\n\x13SelectorTablesReply\x12(\n\x03sig\x18\x01 \x03(\x0b\x32\x1b.allego.SelTableSignalGroup\"\xfa\x02\n\x10\x44\x61taSourceStatus\x12%\n\x04type\x18\x01 \x02(\x0e\x32\x17.allego.SignalGroupType\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12\x10\n\x08\x64uration\x18\x04 \x02(\x01\x12(\n\x0bsignalGroup\x18\x06 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x17\n\x0fnumTotalSamples\x18\x07 \x02(\x03\x12\x12\n\nsampleFreq\x18\t \x01(\x01\x12\x0b\n\x03uid\x18\n \x02(\t\x12\x16\n\x0e\x64\x61taSourceType\x18\x0b \x02(\t\x12\x10\n\x08\x66ileType\x18\x0c \x02(\t\x12\x0c\n\x04mode\x18\r \x02(\t\x12\r\n\x05label\x18\x0e \x02(\t\x12\x0c\n\x04path\x18\x0f \x02(\t\x12\x14\n\x0c\x62\x61seFileName\x18\x10 \x02(\t\x12\x1d\n\x02tR\x18\x11 \x01(\x0b\x32\x11.allego.TimeRange\x12\x14\n\x0ckpiDsourceID\x18\x12 \x01(\t*\x96\x02\n\x0eRadixFileTypes\x12\x07\n\x03RHD\x10\x00\x12\x08\n\x04XDAT\x10\x01\x12\x07\n\x03\x43SV\x10\x02\x12\x08\n\x04HDF5\x10\x03\x12\x08\n\x04NEX5\x10\x04\x12\x07\n\x03NWB\x10\x05\x12\x10\n\x0c\x42IOINTERFACE\x10\x07\x12\r\n\tKILOSORT2\x10\x08\x12\x07\n\x03\x41NC\x10\t\x12\x0f\n\x0bSPKTRAIN_MU\x10\n\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_HDF5\x10\x0b\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_MAT5\x10\x0c\x12\x07\n\x03NSX\x10\r\x12\x07\n\x03PL2\x10\x0e\x12\x07\n\x03TDT\x10\x0f\x12\n\n\x06SPIKES\x10\x10\x12\x07\n\x03KPI\x10\x11\x12\x15\n\x11UNKNOWN_FILE_TYPE\x10\x12\x12\x0f\n\x0bMEAREC_HDF5\x10\x13*1\n\nSignalType\x12\x07\n\x03PRI\x10\x00\x12\x07\n\x03\x41UX\x10\x01\x12\x07\n\x03\x44IN\x10\x02\x12\x08\n\x04\x44OUT\x10\x03*:\n\x0fResampleRoutine\x12\t\n\x05NAIVE\x10\x00\x12\r\n\tRETENTIVE\x10\x01\x12\r\n\tANTIALIAS\x10\x03*>\n\x04Port\x12\x05\n\x01\x41\x10\x00\x12\x05\n\x01\x42\x10\x01\x12\x05\n\x01\x43\x10\x02\x12\x05\n\x01\x44\x10\x03\x12\x05\n\x01\x45\x10\x04\x12\x05\n\x01\x46\x10\x05\x12\x05\n\x01G\x10\x06\x12\x05\n\x01H\x10\x07*2\n\x0cWorkspaceApp\x12\n\n\x06\x41llego\x10\x00\x12\n\n\x06\x43urate\x10\x01\x12\n\n\x06Videre\x10\x02*\xa0\x01\n\x11WorkspaceCommands\x12\x0f\n\x0bWSPACE_Save\x10\x00\x12\x11\n\rWSPACE_SaveAs\x10\x01\x12\x11\n\rWSPACE_Export\x10\x02\x12\x11\n\rWSPACE_Import\x10\x03\x12\x11\n\rWSPACE_Delete\x10\x04\x12\x11\n\rWSPACE_Switch\x10\x07\x12\x1b\n\x17WSPACE_SwitchToLastUsed\x10\x08*C\n\x14GetWorkspaceCommands\x12\x13\n\x0fGET_WSPACE_List\x10\x01\x12\x16\n\x12GET_WSPACE_Current\x10\x02*8\n\x11RadiensServerType\x12\x10\n\x0c\x41llegoserver\x10\x00\x12\x11\n\rRadiensserver\x10\x01*\xae\x01\n\x0fGrpcServiceType\x12\x0f\n\x0b\x41LLEGO_CORE\x10\x00\x12\x11\n\rALLEGO_PCACHE\x10\x01\x12\x0e\n\nALLEGO_KPI\x10\x02\x12\x12\n\x0e\x41LLEGO_NEURONS\x10\x03\x12\x10\n\x0cRADIENS_CORE\x10\x04\x12\x18\n\x14RADIENS_SPIKE_SORTER\x10\x05\x12\x0f\n\x0bRADIENS_DEV\x10\x06\x12\x16\n\x12RADIENS_DASHBOARDS\x10\x07*?\n\x0e\x44\x65vDatasetType\x12\x08\n\x04\x42\x41SE\x10\x00\x12\t\n\x05TRAIN\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x08\n\x04TEST\x10\x03*C\n\rPSDWindowType\x12\x0f\n\x0bHAMMING_p01\x10\x00\x12\x0f\n\x0bHAMMING_p05\x10\x01\x12\x10\n\x0cPASS_THROUGH\x10\x02*\x1e\n\nPSDScaling\x12\x10\n\x0cPSD_ABSOLUTE\x10\x00*X\n\x0e\x44\x61taSourceSort\x12\x10\n\x0c\x44SOURCE_DATE\x10\x00\x12\x10\n\x0c\x44SOURCE_NAME\x10\x01\x12\x10\n\x0c\x44SOURCE_SIZE\x10\x02\x12\x10\n\x0c\x44SOURCE_TYPE\x10\x03*.\n\x0fSignalGroupType\x12\x11\n\rPRIMARY_CACHE\x10\x00\x12\x08\n\x04\x46ILE\x10\x03*\x81\x01\n\x07\x44SPType\x12\x0b\n\x07LOWPASS\x10\x00\x12\x0c\n\x08HIGHPASS\x10\x01\x12\x0c\n\x08\x42\x41NDPASS\x10\x02\x12\t\n\x05NOTCH\x10\x03\x12\x0c\n\x08\x42\x41NDSTOP\x10\x04\x12\x07\n\x03\x43\x41R\x10\x05\x12\x15\n\x11VIRTUAL_REFERENCE\x10\x06\x12\x14\n\x10PAIRED_REFERENCE\x10\x07*9\n\x0b\x46ilterStage\x12\x12\n\x0eSTAGE_HARDWARE\x10\x00\x12\n\n\x06STAGE1\x10\x01\x12\n\n\x06STAGE2\x10\x02*\xd3\x02\n\x0e\x46\x65\x61tureLicense\x12\x1a\n\x16\x46\x65\x61t_NoLicenseRequired\x10\x00\x12\x0c\n\x08\x46\x65\x61t_Any\x10\x01\x12\x0f\n\x0b\x46\x65\x61t_Power9\x10\x02\x12\x11\n\rFeat_RadixAPI\x10\x03\x12\x0e\n\nFeat_Scope\x10\x04\x12\x13\n\x0f\x46\x65\x61t_Electrodes\x10\x05\x12\x13\n\x0f\x46\x65\x61t_HDSnapshot\x10\x06\x12\x12\n\x0e\x46\x65\x61t_Impedance\x10\x07\x12\x10\n\x0c\x46\x65\x61t_Monitor\x10\x08\x12\x16\n\x12\x46\x65\x61t_SignalMetrics\x10\t\x12\x19\n\x15\x46\x65\x61t_SignalProcessing\x10\n\x12\x0f\n\x0b\x46\x65\x61t_System\x10\x0b\x12\x12\n\x0e\x46\x65\x61t_SpikeGrid\x10\x0c\x12\x14\n\x10\x46\x65\x61t_SpikeSorter\x10\r\x12\x0f\n\x0b\x46\x65\x61t_Raster\x10\x0e\x12\x14\n\x10\x46\x65\x61t_ThreeDModel\x10\x0f*\xed\x01\n\x10SummaryStatsEnum\x12\x10\n\x0cSS_STAT_MEAN\x10\x00\x12\x0e\n\nSS_STAT_SD\x10\x01\x12\x10\n\x0cSS_STAT_MODE\x10\x02\x12\x0f\n\x0bSS_STAT_MIN\x10\x03\x12\x0f\n\x0bSS_STAT_MAX\x10\x04\x12\x16\n\x12SS_STAT_MODE_COUNT\x10\x05\x12\x12\n\x0eSS_STAT_MEDIAN\x10\x06\x12\x0f\n\x0bSS_STAT_Q25\x10\x07\x12\x0f\n\x0bSS_STAT_Q75\x10\x08\x12\x10\n\x0cSS_STAT_SKEW\x10\t\x12\x14\n\x10SS_STAT_KURTOSIS\x10\n\x12\r\n\tSS_STAT_N\x10\x0b*_\n\x0eKpiMetricsMode\x12\x18\n\x14Kpi_MetricsMode_Base\x10\x00\x12\x17\n\x13Kpi_MetricsMode_Avg\x10\x01\x12\x1a\n\x16Kpi_MetricsMode_Stream\x10\x02*\xa1\x06\n\x0eKpiMetricsEnum\x12\x0f\n\x0bKPI_NUM_PTS\x10\x00\x12\x13\n\x0fKPI_NUM_PTS_ISI\x10\x01\x12\x0f\n\x0bKPI_DUR_SEC\x10\x02\x12\x0c\n\x08KPI_MEAN\x10\x03\x12\x0b\n\x07KPI_MIN\x10\x04\x12\x0f\n\x0bKPI_MIN_ISI\x10\x05\x12\x0b\n\x07KPI_MAX\x10\x06\x12\x0f\n\x0bKPI_MAX_ISI\x10\x07\x12\x0f\n\x0bKPI_MAX_ABS\x10\x08\x12\x13\n\x0fKPI_MAX_ABS_ISI\x10\t\x12\x15\n\x11KPI_TIMESTAMP_MIN\x10\n\x12\x15\n\x11KPI_TIMESTAMP_MAX\x10\x0b\x12\x18\n\x14KPI_MAX_MIN_DIFF_ABS\x10\x0c\x12\x1c\n\x18KPI_MAX_MIN_DIFF_ABS_ISI\x10\r\x12\n\n\x06KPI_SD\x10\x0e\x12\x0e\n\nKPI_SD_ISI\x10\x0f\x12\x0b\n\x07KPI_VAR\x10\x10\x12\x0f\n\x0bKPI_VAR_ISI\x10\x11\x12\x0b\n\x07KPI_RMS\x10\x12\x12\x0f\n\x0bKPI_RMS_ISI\x10\x13\x12\x10\n\x0cKPI_NOISE_UV\x10\x14\x12\x0b\n\x07KPI_SNR\x10\x15\x12\x12\n\x0eKPI_NUM_EVENTS\x10\x16\x12\x12\n\x0eKPI_EVENT_RATE\x10\x17\x12\x11\n\rKPI_EVENT_MAX\x10\x18\x12\x11\n\rKPI_EVENT_MIN\x10\x19\x12\x15\n\x11KPI_EVENT_MAX_ABS\x10\x1a\x12\x1e\n\x1aKPI_EVENT_MAX_MIN_DIFF_ABS\x10\x1b\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MIN\x10\x1c\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MAX\x10\x1d\x12\x1f\n\x1bKPI_EVENT_TIMESTAMP_MAX_ABS\x10\x1e\x12(\n$KPI_EVENT_TIMESTAMP_MAX_MIN_DIFF_ABS\x10\x1f\x12\x10\n\x0cKPI_MEAN_MAX\x10 \x12\x10\n\x0cKPI_MEAN_MIN\x10!\x12\x14\n\x10KPI_MEAN_MAX_ABS\x10\"\x12#\n\x1fKPI_EVENT_MEAN_MAX_MIN_DIFF_ABS\x10#\x12\"\n\x1eKPI_MAX_MIN_DIFF_ABS_AMPLIFIED\x10$*\x8b\x01\n\x13KpiMetricsStatsEnum\x12\x1e\n\x1aKPI_BDL_METRICS_STATS_MEAN\x10\x00\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MAX\x10\x01\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MIN\x10\x02\x12\x16\n\x12KPI_BDL_METRICS_SD\x10\x03*\xc0\x02\n\x19KpiBundlePacketsStatsEnum\x12\x14\n\x10KPI_BDL_NUM_SIGS\x10\x00\x12\x13\n\x0fKPI_BDL_DUR_SEC\x10\x01\x12\x1d\n\x19KPI_BDL_NUM_SIGS_W_EVENTS\x10\x02\x12\x15\n\x11KPI_BDL_SIG_YIELD\x10\x03\x12\x13\n\x0fKPI_BDL_RMS_AVG\x10\x04\x12\x13\n\x0fKPI_BDL_SNR_AVG\x10\x05\x12\x13\n\x0fKPI_BDL_SIG_MAX\x10\x06\x12\x13\n\x0fKPI_BDL_SIG_MIN\x10\x07\x12\x18\n\x14KPI_BDL_NOISE_UV_AVG\x10\x08\x12\x1c\n\x18KPI_BDL_NUM_EVENTS_TOTAL\x10\t\x12\x1a\n\x16KPI_BDL_NUM_EVENTS_AVG\x10\n\x12\x1a\n\x16KPI_BDL_EVENT_RATE_AVG\x10\x0b*F\n\x10TimeRangeSelMode\x12\x0e\n\nTRS_SUBSET\x10\x00\x12\x0f\n\x0bTRS_TO_HEAD\x10\x01\x12\x11\n\rTRS_FROM_HEAD\x10\x02*e\n\rKpiScannerCmd\x12\x13\n\x0fKPI_SCANNER_OFF\x10\x00\x12\x1e\n\x1aKPI_SCANNER_BESPOKE_SPRINT\x10\x01\x12\x1f\n\x1bKPI_SCANNER_STANDARD_SPRINT\x10\x02*N\n\x16OutfitterComponentType\x12\x16\n\x12OUTFIT_COMP_SENSOR\x10\x00\x12\x1c\n\x18OUTFIT_COMP_SPIKE_SORTER\x10\x01*}\n\x0eWorldNodeLabel\x12\x12\n\x0eWORLD_NODE_ORG\x10\x01\x12\x12\n\x0eWORLD_NODE_LAB\x10\x02\x12\x13\n\x0fWORLD_NODE_USER\x10\x03\x12\x18\n\x14WORLD_NODE_CAT_PROBE\x10\x04\x12\x14\n\x10WORLD_NODE_PROBE\x10\x05*\'\n\x0eWorldEdgeLabel\x12\x15\n\x11WORLD_EDGE_MEMBER\x10\x01*`\n\x12WorldEdgeDirection\x12\x18\n\x14WORLD_EDGE_DIR_RIGHT\x10\x01\x12\x17\n\x13WORLD_EDGE_DIR_LEFT\x10\x02\x12\x17\n\x13WORLD_EDGE_DIR_BOTH\x10\x03*\x9f\x01\n\x0cUserRoleType\x12\x0b\n\x07USER_PI\x10\x01\x12\x12\n\x0eUSER_SCIENTIST\x10\x02\x12\x11\n\rUSER_POST_DOC\x10\x03\x12\x15\n\x11USER_GRAD_STUDENT\x10\x04\x12\x13\n\x0fUSER_UG_STUDENT\x10\x05\x12\x10\n\x0cUSER_MANAGER\x10\x06\x12\r\n\tUSER_TECH\x10\x07\x12\x0e\n\nUSER_OTHER\x10\x08*G\n\rManageNodeCmd\x12\x10\n\x0cNODE_CMD_NEW\x10\x01\x12\x12\n\x0eNODE_CMD_MERGE\x10\x02\x12\x10\n\x0cNODE_CMD_DEL\x10\x03*\xe8\x01\n\rWorldQueryCmd\x12\x15\n\x11WQ_LIST_ALL_USERS\x10\x01\x12\x14\n\x10WQ_LIST_ALL_LABS\x10\x02\x12\x14\n\x10WQ_LIST_ALL_ORGS\x10\x03\x12\x1a\n\x16WQ_LIST_ALL_CAT_PROBES\x10\x04\x12\x16\n\x12WQ_LIST_ALL_PROBES\x10\x05\x12\x18\n\x14WQ_CAT_PROBE_BY_NAME\x10\x06\x12\x11\n\rWQ_USER_BY_ID\x10\x07\x12\x19\n\x15WQ_USER_AND_LAB_BY_ID\x10\x08\x12\x18\n\x14WQ2_LIST_ALL_DEVICES\x10\x1e*\x82\x02\n\x11TransformNodeType\x12\x10\n\x0cNOTCH_FILTER\x10\x00\x12\x13\n\x0f\x42\x41NDPASS_FILTER\x10\x01\x12\x13\n\x0f\x42\x41NDSTOP_FILTER\x10\x02\x12\x13\n\x0fHIGHPASS_FILTER\x10\x03\x12\x12\n\x0eLOWPASS_FILTER\x10\x04\x12\x0e\n\nPAIRED_REF\x10\x05\x12\x0f\n\x0bVIRTUAL_REF\x10\x06\x12\x0b\n\x07\x43\x41R_REF\x10\x07\x12\x0e\n\nSLICE_TIME\x10\t\x12\x12\n\x0eSLICE_CHANNELS\x10\n\x12\n\n\x06SOURCE\x10\x0b\x12\x08\n\x04SINK\x10\x0c\x12\x0e\n\nDOWNSAMPLE\x10\r\x12\x10\n\x0cREMAP_SENSOR\x10\x0e*\xdf\x01\n\x17SpikeSorterParamCommand\x12\x14\n\x10SORTER_THR_LEVEL\x10\x01\x12\x17\n\x13SORTER_THR_LEVEL_SD\x10\x04\x12\x12\n\x0eSORTER_THR_WDW\x10\x08\x12\x19\n\x15SORTER_WEAK_THR_LEVEL\x10\n\x12\x1c\n\x18SORTER_WEAK_THR_LEVEL_SD\x10\r\x12\x11\n\rSORTER_SHADOW\x10\x11\x12\x17\n\x13SORTER_THR_ACTIVATE\x10\x13\x12\x1c\n\x18SORTER_WEAK_THR_ACTIVATE\x10\x15*\xee\x03\n\x10StatusPollFields\x12\x19\n\x15PORT_CONNECTION_STATE\x10\x00\x12\x14\n\x10RECORDING_ERRORS\x10\x01\x12\x15\n\x11STREAM_TIME_RANGE\x10\x02\x12\x11\n\rSTREAM_STATUS\x10\x03\x12\x11\n\rRECORD_STATUS\x10\x04\x12\x10\n\x0cIS_CONNECTED\x10\x06\x12\x0e\n\nRECORD_DUR\x10\x07\x12\x11\n\rBACKBONE_MODE\x10\t\x12\x10\n\x0cSIGNAL_GROUP\x10\n\x12\x14\n\x10SINAPS_REGISTERS\x10\x0b\x12\x14\n\x10RECORDING_CONFIG\x10\x0c\x12\x0b\n\x07\x46ILTERS\x10\r\x12\x17\n\x13\x45VENT_THRESH_PARAMS\x10\x0e\x12\x10\n\x0c\x44\x41\x43_REGISTER\x10\x0f\x12\x10\n\x0c\x44IO_REGISTER\x10\x10\x12\x10\n\x0cTRIGGER_MODE\x10\x11\x12\x11\n\rCABLE_LENGTHS\x10\x12\x12\x11\n\rEVENT_VIEWERS\x10\x13\x12\x0f\n\x0bSAMPLE_RATE\x10\x14\x12\x0e\n\nALL_FIELDS\x10\x15\x12\x16\n\x12SPIKE_SORTER_STATE\x10\x16\x12\x0f\n\x0bSTIM_PARAMS\x10\x17\x12\x19\n\x15SPIKE_SORTER_WARNINGS\x10\x18\x12\x12\n\x0eSTIM_STEP_SIZE\x10\x19*\x1b\n\rDashboardType\x12\n\n\x06\x44\x41SH_1\x10\x00*N\n\x10\x44\x61shboardCommand\x12\x11\n\rDASH_CMD_OPEN\x10\x00\x12\x12\n\x0e\x44\x41SH_CMD_CLOSE\x10\x01\x12\x13\n\x0f\x44\x41SH_CMD_UPDATE\x10\x02\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x06\x61llego\x1a\x1fgoogle/protobuf/timestamp.proto\"@\n\x14OfflineLicenseStatus\x12\x12\n\nisVerified\x18\x01 \x02(\x08\x12\x14\n\x0chardwareUUID\x18\x02 \x02(\t\"C\n\x0f\x46irmwareVersion\x12\x0c\n\x04\x64\x61te\x18\x01 \x02(\t\x12\x10\n\x08majorRev\x18\x02 \x02(\x05\x12\x10\n\x08minorRev\x18\x03 \x02(\x05\"k\n\x10RadixEnvironment\x12\x0f\n\x07version\x18\x01 \x02(\t\x12\x14\n\x0cuserDataPath\x18\x02 \x02(\t\x12\x30\n\x0f\x66irmwareVersion\x18\x03 \x02(\x0b\x32\x17.allego.FirmwareVersion\"!\n\x0fStandardRequest\x12\x0e\n\x06regStr\x18\x02 \x03(\t\"/\n\rStandardReply\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\x12\x0e\n\x06regStr\x18\x02 \x03(\t\"&\n\rDACOffRequest\x12\x15\n\rstreamGroupId\x18\x01 \x01(\t\"\xba\x01\n\x13WorkspaceDescriptor\x12\n\n\x02iD\x18\x01 \x02(\t\x12!\n\x03\x61pp\x18\x02 \x02(\x0e\x32\x14.allego.WorkspaceApp\x12\x12\n\nisModified\x18\x03 \x02(\x08\x12\x19\n\x11timestampLastUsed\x18\x04 \x02(\t\x12\x19\n\x11timestampModified\x18\x05 \x02(\t\x12*\n\nannotation\x18\x06 \x02(\x0b\x32\x16.allego.AnnotateBundle\"\xb8\x01\n\x17WorkspaceControlRequest\x12&\n\x03\x63md\x18\x01 \x02(\x0e\x32\x19.allego.WorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12*\n\nannotation\x18\x03 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x1a\n\x12targetFullFileName\x18\x04 \x01(\t\x12\x18\n\x10isForceOverwrite\x18\x05 \x01(\x08\"\xd3\x01\n\x13GetWorkspaceRequest\x12)\n\x03\x63md\x18\x01 \x02(\x0e\x32\x1c.allego.GetWorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12\x14\n\x0cworkspaceDir\x18\x03 \x01(\t\x12%\n\x07\x61ppMask\x18\x04 \x01(\x0e\x32\x14.allego.WorkspaceApp\x12,\n\x0c\x61nnotateMask\x18\x05 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x11\n\tisBrowser\x18\x06 \x01(\x08\"\xab\x01\n\x11GetWorkspaceReply\x12\x43\n\rworkspaceDesc\x18\x01 \x03(\x0b\x32,.allego.GetWorkspaceReply.WorkspaceDescEntry\x1aQ\n\x12WorkspaceDescEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x1b.allego.WorkspaceDescriptor:\x02\x38\x01\"`\n\x18GetRadiensServersRequest\x12\x15\n\rhostIPaddress\x18\x01 \x02(\t\x12-\n\nserverType\x18\x02 \x01(\x0e\x32\x19.allego.RadiensServerType\"\x97\x02\n\nServerSpec\x12\x0c\n\x04host\x18\x01 \x02(\t\x12\x0b\n\x03pid\x18\x02 \x02(\x05\x12\x30\n\x07service\x18\x03 \x03(\x0b\x32\x1f.allego.ServerSpec.ServiceEntry\x12\x30\n\x05spawn\x18\x04 \x01(\x0b\x32!.allego.ServerSpec.SpawnedProcess\x1a\x1b\n\x0bGrpcService\x12\x0c\n\x04port\x18\x01 \x02(\x05\x1a\x1d\n\x0eSpawnedProcess\x12\x0b\n\x03pid\x18\x01 \x03(\x05\x1aN\n\x0cServiceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.allego.ServerSpec.GrpcService:\x02\x38\x01\"j\n\x13RadiensServersReply\x12(\n\x0c\x61llegoserver\x18\x01 \x03(\x0b\x32\x12.allego.ServerSpec\x12)\n\rradiensserver\x18\x02 \x03(\x0b\x32\x12.allego.ServerSpec\"-\n\x14SignalGroupIDRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\"\xc4\x01\n\tSignalMap\x12\x0f\n\x07siteIdx\x18\x01 \x03(\x05\x12\x13\n\x0b\x63ompSiteNum\x18\x02 \x03(\t\x12\x13\n\x0bposProbeUmX\x18\x03 \x03(\x01\x12\x13\n\x0bposProbeUmY\x18\x04 \x03(\x01\x12\x13\n\x0bposProbeUmZ\x18\x05 \x03(\x01\x12\x14\n\x0cposTissueUmX\x18\x06 \x03(\x01\x12\x14\n\x0cposTissueUmY\x18\x07 \x03(\x01\x12\x14\n\x0cposTissueUmZ\x18\x08 \x03(\x01\x12\x10\n\x08sensorID\x18\t \x03(\t\"=\n\x10GPIOChannelCount\x12\x0c\n\x04nAux\x18\x01 \x02(\x05\x12\x0c\n\x04nDin\x18\x02 \x02(\x05\x12\r\n\x05nDout\x18\x03 \x02(\x05\"D\n\x10PortChannelCount\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"Q\n\x0eSetPortRequest\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x10\n\x08probeUID\x18\x02 \x02(\t\x12\x11\n\thstageUID\x18\x03 \x02(\t\"\xe2\x02\n\x11HDSnapshotRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12=\n\npriSignals\x18\x03 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\nauxSignals\x18\x04 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\ndinSignals\x18\x05 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12>\n\x0b\x64outSignals\x18\x06 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x1a&\n\x0fSelectedSignals\x12\x13\n\x0bntvChanIdxs\x18\x01 \x03(\x05\"\x96\x01\n\x12HDSnapshotRequest2\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12)\n\x07selMode\x18\x03 \x01(\x0e\x32\x18.allego.TimeRangeSelMode\x12#\n\x06sigSel\x18\x04 \x01(\x0b\x32\x13.allego.SigSelector\"L\n\x15RadiensPyGraphicsArgs\x12\x12\n\ngraphicsID\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0f\n\x07\x66igSize\x18\x03 \x03(\x03\"\xdd\x02\n\nPSDRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12)\n\x07selMode\x18\x03 \x02(\x0e\x32\x18.allego.TimeRangeSelMode\x12!\n\x05stype\x18\x04 \x02(\x0e\x32\x12.allego.SignalType\x12\x0f\n\x07ntvIdxs\x18\x05 \x03(\x03\x12\x12\n\nresampleFs\x18\x06 \x01(\x01\x12&\n\x07wdwType\x18\x07 \x01(\x0e\x32\x15.allego.PSDWindowType\x12#\n\x07scaling\x18\x08 \x01(\x0e\x32\x12.allego.PSDScaling\x12\x11\n\tfreqRange\x18\t \x03(\x01\x12\x14\n\x0c\x63ollapseFreq\x18\n \x01(\x08\x12\x11\n\tdeltaFreq\x18\x0b \x01(\x01\x12\x0c\n\x04path\x18\r \x01(\t\x12\x13\n\x0bisReturnPSD\x18\x0e \x01(\x08\"\xa1\x02\n\x03PSD\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12\x1f\n\x02sG\x18\x03 \x02(\x0b\x32\x13.allego.SignalGroup\x12!\n\x05stype\x18\x04 \x02(\x0e\x32\x12.allego.SignalType\x12\x1d\n\x02tR\x18\x05 \x02(\x0b\x32\x11.allego.TimeRange\x12 \n\x03psd\x18\x06 \x02(\x0b\x32\x13.allego.DenseMatrix\x12\x0c\n\x04\x66req\x18\x07 \x03(\x01\x12\x14\n\x0c\x66reqBinWidth\x18\x08 \x02(\x01\x12\x11\n\tfreqRange\x18\x0b \x03(\x01\x12&\n\x07wdwType\x18\t \x01(\x0e\x32\x15.allego.PSDWindowType\x12#\n\x07scaling\x18\n \x01(\x0e\x32\x12.allego.PSDScaling\"e\n\x18RadiensPyGraphicsRequest\x12\x1c\n\x07psdData\x18\x01 \x01(\x0b\x32\x0b.allego.PSD\x12+\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\x1d.allego.RadiensPyGraphicsArgs\"^\n\x0bSigSelector\x12\x12\n\nampNtvIdxs\x18\x01 \x03(\x03\x12\x12\n\nainNtvIdxs\x18\x02 \x03(\x03\x12\x12\n\ndinNtvIdxs\x18\x03 \x03(\x03\x12\x13\n\x0b\x64outNtvIdxs\x18\x04 \x03(\x03\"]\n\x0eHDSnapshotMeta\x12\x11\n\tglobalMin\x18\x04 \x02(\x01\x12\x11\n\tglobalMax\x18\x05 \x02(\x01\x12%\n\x08sigGroup\x18\x06 \x01(\x0b\x32\x13.allego.SignalGroup\"\x9f\x02\n\nHDSnapshot\x12$\n\x04meta\x18\x01 \x02(\x0b\x32\x16.allego.HDSnapshotMeta\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x13\n\x0btimeSamples\x18\x03 \x02(\x0c\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12&\n\npriSignals\x18\x05 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\nauxSignals\x18\x06 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\ndinSignals\x18\x07 \x01(\x0b\x32\x12.allego.RawSignals\x12\'\n\x0b\x64outSignals\x18\x08 \x01(\x0b\x32\x12.allego.RawSignals\"@\n\x0bHDSnapshot2\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12\x1e\n\x04sigs\x18\x02 \x02(\x0b\x32\x10.allego.Signals2\"\xcd\x03\n\x11GetSignalsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x37\n\x06params\x18\x02 \x02(\x0b\x32\'.allego.GetSignalsRequest.GetSigsParams\x1a\xe7\x02\n\rGetSigsParams\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x0e\n\x06wdwSec\x18\x02 \x02(\x01\x12\x14\n\x0c\x63hanHeightPx\x18\x03 \x02(\x01\x12\x10\n\x08\x61mpFsrUv\x18\x04 \x02(\x01\x12\x17\n\x0fplotWidthPoints\x18\x05 \x02(\x01\x12\x11\n\tgpioOnTop\x18\x06 \x02(\x08\x12\x0f\n\x07\x61inFsrV\x18\x07 \x02(\x01\x12\x13\n\x0b\x63omponentID\x18\x08 \x02(\t\x12-\n\x0cresampleType\x18\t \x02(\x0e\x32\x17.allego.ResampleRoutine\x12\x11\n\tisHeatmap\x18\n \x02(\x08\x12\x1b\n\x13isNotApplyDSPstage2\x18\x0b \x01(\x08\x12\x13\n\x0b\x63lipToRange\x18\x0c \x02(\x08\x12\x17\n\x0f\x62\x61ndpassLowFreq\x18\r \x01(\x01\x12\x18\n\x10\x62\x61ndpassHighFreq\x18\x0e \x01(\x01\x12\x12\n\nntvChanIdx\x18\x0f \x01(\x01\"[\n\nRawSignals\x12\r\n\x05shape\x18\x01 \x03(\x05\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\x12\x1d\n\x02tR\x18\x04 \x01(\x0b\x32\x11.allego.TimeRange\"\xe7\x01\n\x08Signals2\x12\x1f\n\x02sG\x18\x01 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12%\n\x03\x61mp\x18\x03 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12%\n\x03\x61in\x18\x04 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12%\n\x03\x64in\x18\x05 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12&\n\x04\x64out\x18\x06 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\"\x85\x02\n\x14ListSensorSpecsReply\x12\x41\n\x06probes\x18\x01 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\x45\n\nheadstages\x18\x02 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x1a:\n\x14SpecWithChannelCount\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"d\n\x16ListDataSourcesRequest\x12\x11\n\tdirectory\x18\x01 \x02(\t\x12&\n\x06sortBy\x18\x02 \x01(\x0e\x32\x16.allego.DataSourceSort\x12\x0f\n\x07\x64irList\x18\x03 \x03(\t\"\x1c\n\x07SortMap\x12\x11\n\tsorterIds\x18\x01 \x03(\t\">\n\x16GetSignalGroupIDsReply\x12\x12\n\ncontinuous\x18\x01 \x03(\t\x12\x10\n\x08\x64iscrete\x18\x02 \x03(\t\"\xa0\x01\n\x13GetSorterIDMapReply\x12\x43\n\x0csigToSortMap\x18\x01 \x03(\x0b\x32-.allego.GetSorterIDMapReply.SigToSortMapEntry\x1a\x44\n\x11SigToSortMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.allego.SortMap:\x02\x38\x01\"\xaf\x01\n\nDataSource\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x02(\t\x12\x17\n\x0f\x64urationSeconds\x18\x03 \x02(\x01\x12\x17\n\x0f\x64urationMinutes\x18\x04 \x02(\x01\x12\x15\n\rdurationHours\x18\x05 \x02(\x01\x12(\n\x08\x66ileType\x18\x06 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x12\n\nnumSignals\x18\x07 \x02(\x05\"o\n\x0e\x46ileDescriptor\x12\x0c\n\x04path\x18\x01 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x13\n\x0b\x66ileNameUID\x18\x04 \x01(\t\"\xd0\x01\n\x08TimeSpec\x12\x30\n\ttimeRange\x18\x01 \x01(\x0b\x32\x1b.allego.TimeSpec.TimeRangeLH\x00\x12:\n\x0etimestampRange\x18\x02 \x01(\x0b\x32 .allego.TimeSpec.TimestampRangeLH\x00\x1a\x1f\n\nTimeRangeL\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x1a)\n\x0fTimestampRangeL\x12\x16\n\x0etimestampRange\x18\x01 \x03(\x03\x42\n\n\x08timeDesc\"\xbe\x01\n\nSignalSpec\x12.\n\x07siteNum\x18\x01 \x01(\x0b\x32\x1b.allego.SignalSpec.SiteNumLH\x00\x12\x34\n\nntvChanIdx\x18\x02 \x01(\x0b\x32\x1e.allego.SignalSpec.NtvChanIdxLH\x00\x1a\x1b\n\x08SiteNumL\x12\x0f\n\x07siteNum\x18\x01 \x03(\x05\x1a!\n\x0bNtvChanIdxL\x12\x12\n\nntvChanIdx\x18\x01 \x03(\x05\x42\n\n\x08siteDesc\"\x8c\x06\n\rChannelRecord\x12\x10\n\x08\x63hanName\x18\x01 \x02(\t\x12$\n\x08\x63hanType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\x12\n\nntvChanIdx\x18\x03 \x02(\x05\x12\x0f\n\x07siteNum\x18\x04 \x02(\x05\x12\x15\n\rcolorGroupIdx\x18\x05 \x02(\x05\x12\x12\n\nisSelected\x18\x06 \x02(\x08\x12\x13\n\x0bisAudioLeft\x18\x07 \x02(\x08\x12\x1a\n\x04port\x18\x08 \x02(\x0e\x32\x0c.allego.Port\x12\x11\n\tsiteShape\x18\t \x02(\t\x12\x10\n\x08siteCtrX\x18\n \x02(\x01\x12\x10\n\x08siteCtrY\x18\x0b \x02(\x01\x12\x10\n\x08siteCtrZ\x18\x0c \x02(\x01\x12\x13\n\x0bsiteLimXMin\x18\r \x02(\x01\x12\x13\n\x0bsiteLimXMax\x18\x0e \x02(\x01\x12\x13\n\x0bsiteLimYMin\x18\x0f \x02(\x01\x12\x13\n\x0bsiteLimYMax\x18\x10 \x02(\x01\x12\x13\n\x0bsiteLimZMin\x18\x11 \x02(\x01\x12\x13\n\x0bsiteLimZMax\x18\x12 \x02(\x01\x12\x13\n\x0bsiteCtrTcsX\x18\x13 \x02(\x01\x12\x13\n\x0bsiteCtrTcsY\x18\x14 \x02(\x01\x12\x13\n\x0bsiteCtrTcsZ\x18\x15 \x02(\x01\x12\x13\n\x0bsensorUnits\x18\x16 \x02(\t\x12\x0e\n\x06\x61\x62sIdx\x18\x17 \x02(\x05\x12\x14\n\x0cisAudioRight\x18\x18 \x02(\x08\x12\x12\n\nsysChanIdx\x18\x19 \x02(\x05\x12\x17\n\x0fsiteAreaMicron2\x18\x1a \x01(\x01\x12\x11\n\tscsToTcsX\x18\x1b \x01(\x01\x12\x11\n\tscsToTcsY\x18\x1c \x01(\x01\x12\x11\n\tscsToTcsZ\x18\x1d \x01(\x01\x12\x10\n\x08sensorID\x18\x1e \x01(\t\x12\x0f\n\x07probeID\x18\x1f \x01(\t\x12\x13\n\x0bheadstageID\x18  \x01(\t\x12\x13\n\x0b\x64\x61tasetRidx\x18! \x01(\x05\x12\x13\n\x0b\x64\x61tasetAidx\x18\" \x01(\x05\x12\x13\n\x0bntvChanName\x18# \x01(\t\x12\x11\n\tsensorUID\x18$ \x01(\t\x12\x11\n\tsensorIdx\x18% \x01(\x05\"\x1f\n\x07XYCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"+\n\x08XYZCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\x12\t\n\x01z\x18\x03 \x02(\x01\"\x81\x03\n\x06Sensor\x12\x0f\n\x07probeId\x18\x01 \x02(\t\x12\x13\n\x0bheadstageId\x18\x02 \x02(\t\x12+\n\twireframe\x18\x03 \x02(\x0b\x32\x18.allego.Sensor.WireFrame\x12\x0c\n\x04xMin\x18\x04 \x02(\x01\x12\x0c\n\x04xMax\x18\x05 \x02(\x01\x12\x0c\n\x04yMin\x18\x06 \x02(\x01\x12\x0c\n\x04yMax\x18\x07 \x02(\x01\x12+\n\x08position\x18\x08 \x02(\x0b\x32\x19.allego.SensorPositionTcs\x12\x11\n\tsensorUID\x18\t \x01(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\n \x01(\x05\x12\x10\n\x08numSites\x18\x0b \x02(\x05\x12\x11\n\tsensorIdx\x18\x0c \x01(\x05\x1am\n\tWireFrame\x12\x1c\n\x03vtx\x18\x01 \x03(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxXlim\x18\x02 \x02(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxYlim\x18\x03 \x02(\x0b\x32\x0f.allego.XYCoord\"\x98\x02\n\x0eSensorPortSpec\x12\x1f\n\x07sensorA\x18\x01 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorB\x18\x02 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorC\x18\x03 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorD\x18\x04 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorE\x18\x05 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorF\x18\x06 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorG\x18\x07 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorH\x18\x08 \x03(\x0b\x32\x0e.allego.Sensor\"t\n\x10SignalGroupUnits\x12\x32\n\x05units\x18\x01 \x03(\x0b\x32#.allego.SignalGroupUnits.UnitsEntry\x1a,\n\nUnitsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\x80\x02\n\x0bSignalGroup\x12\'\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x15.allego.ChannelRecord\x12.\n\x0esensorPortSpec\x18\x02 \x02(\x0b\x32\x16.allego.SensorPortSpec\x12\x12\n\ndatasetUID\x18\x03 \x01(\t\x12\x10\n\x08sampFreq\x18\x04 \x01(\x01\x12\x13\n\x0bsourceLabel\x18\x05 \x01(\t\x12\x19\n\x11neighborMaxRadius\x18\x06 \x01(\x01\x12-\n\x0bsignalUnits\x18\x07 \x01(\x0b\x32\x18.allego.SignalGroupUnits\x12\x13\n\x0bhasDiscrete\x18\x08 \x01(\x08\"\x87\x01\n\x18\x43reateSignalGroupRequest\x12\x16\n\x0e\x64\x61taSourceName\x18\x01 \x02(\t\x12\x16\n\x0e\x64\x61taSourcePath\x18\x02 \x02(\t\x12$\n\x04type\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x15\n\rstreamGroupId\x18\x04 \x02(\t\"s\n\tSubOpSort\x12)\n\x04sort\x18\x01 \x03(\x0e\x32\x1b.allego.SubOpSort.SortField\";\n\tSortField\x12\x0e\n\nSITE_CTR_X\x10\x00\x12\x0e\n\nSITE_CTR_Y\x10\x01\x12\x0e\n\nSITE_CTR_Z\x10\x02\"\xa5\x03\n\x18UpdateSignalGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12=\n\toperation\x18\x02 \x02(\x0e\x32*.allego.UpdateSignalGroupRequest.Operation\x12\x42\n\taddRemove\x18\x03 \x01(\x0e\x32-.allego.UpdateSignalGroupRequest.SubOperationH\x00\x12#\n\x06sortOp\x18\x04 \x01(\x0b\x32\x11.allego.SubOpSortH\x00\x12\x16\n\nntvChanIdx\x18\x05 \x03(\x05\x42\x02\x10\x01\x12&\n\nsignalType\x18\x06 \x02(\x0e\x32\x12.allego.SignalType\x12\x11\n\tpropagate\x18\x07 \x01(\x08\"B\n\tOperation\x12\t\n\x05\x43OLOR\x10\x00\x12\n\n\x06SELECT\x10\x01\x12\x14\n\x10\x44\x45PRECATED_AUDIO\x10\x02\x12\x08\n\x04SORT\x10\x03\"#\n\x0cSubOperation\x12\x07\n\x03\x41\x44\x44\x10\x00\x12\n\n\x06REMOVE\x10\x01\x42\x0e\n\x0csubOperation\"T\n\x14SliceSignalGroupSpec\x12\x0e\n\x06sortBy\x18\x01 \x02(\t\x12\r\n\x05\x64\x65lim\x18\x02 \x02(\t\x12\x1d\n\x02tR\x18\x03 \x01(\x0b\x32\x11.allego.TimeRange\"X\n\x17SliceSignalGroupRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12*\n\x04spec\x18\x02 \x02(\x0b\x32\x1c.allego.SliceSignalGroupSpec\"\x88\x01\n\x15SliceSignalGroupReply\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12*\n\x04spec\x18\x02 \x02(\x0b\x32\x1c.allego.SliceSignalGroupSpec\x12\x1f\n\x02sG\x18\x03 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x0f\n\x07outcome\x18\x04 \x02(\t\"\x0f\n\rLicenseStatus\"u\n\x12SetDSPGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12$\n\tdspParams\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"\xf2\x02\n\tDSPParams\x12\x1d\n\x04type\x18\x01 \x02(\x0e\x32\x0f.allego.DSPType\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12\x0e\n\x04\x66req\x18\x03 \x01(\x01H\x00\x12\x36\n\x0c\x66reqSpecBand\x18\x04 \x01(\x0b\x32\x1e.allego.DSPParams.FreqSpecBandH\x00\x12\x17\n\rrefNtvChanIdx\x18\x08 \x01(\x05H\x00\x12\x16\n\x0enotchBandwidth\x18\x05 \x01(\x01\x12\x11\n\tuserLabel\x18\x06 \x02(\t\x12\x1a\n\x04port\x18\x07 \x02(\x0e\x32\x0c.allego.Port\x12\x18\n\x10targetNtvChanIdx\x18\t \x01(\x01\x12\r\n\x05isAux\x18\n \x02(\x08\x12\x12\n\nauxChanIdx\x18\x0b \x01(\x05\x1a\x31\n\x0c\x46reqSpecBand\x12\x0f\n\x07lowFreq\x18\x01 \x02(\x01\x12\x10\n\x08highFreq\x18\x02 \x02(\x01\x42\n\n\x08\x66reqSpec\"\x85\x01\n\x08\x44SPGroup\x12#\n\x08hardware\x18\x01 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage1\x18\x02 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage2\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"\x9a\x01\n\x10SetSensorRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07probeId\x18\x03 \x01(\t\x12\x13\n\x0bheadstageId\x18\x04 \x01(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\x05 \x01(\x05\x12\x13\n\x0bnumChannels\x18\x06 \x01(\x05\"m\n\x11SensorPositionTcs\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\x12\x11\n\tRingAngle\x18\x05 \x02(\x01\x12\x12\n\nAxialAngle\x18\x06 \x02(\x01\x12\x10\n\x08\x41rcAngle\x18\x07 \x02(\x01\"\x90\x01\n\x1bSetSensorPositionTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12+\n\x08position\x18\x03 \x02(\x0b\x32\x19.allego.SensorPositionTcs\x12\x11\n\tsensorIdx\x18\x04 \x01(\x05\"F\n\x0fSitePositionTcs\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\"\x7f\n\x1aSetSitePositionsTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12.\n\rsitePositions\x18\x03 \x03(\x0b\x32\x17.allego.SitePositionTcs\"Y\n\x17\x46\x65\x61tureStartStopRequest\x12\x0e\n\x06nodeId\x18\x01 \x02(\t\x12.\n\x0e\x66\x65\x61tureLicense\x18\x02 \x02(\x0e\x32\x16.allego.FeatureLicense\"!\n\x0cPrivacyReply\x12\x11\n\tisPrivate\x18\x02 \x02(\x08\"&\n\x11SetPrivacyRequest\x12\x11\n\tisPrivate\x18\x01 \x02(\x08\"7\n\x0b\x44\x65nseMatrix\x12\x0c\n\x04rows\x18\x01 \x02(\x03\x12\x0c\n\x04\x63ols\x18\x02 \x02(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\"\\\n\tHistogram\x12\r\n\x05stats\x18\x01 \x03(\x01\x12\x0e\n\x06\x63ounts\x18\x02 \x03(\x01\x12\x10\n\x08\x64ividers\x18\x03 \x03(\x01\x12\x0f\n\x07numBins\x18\x04 \x02(\x03\x12\r\n\x05isPDF\x18\x05 \x02(\x08\"Y\n\x0bKpiMetricID\x12$\n\x04mode\x18\x01 \x02(\x0e\x32\x16.allego.KpiMetricsMode\x12$\n\x04name\x18\x02 \x02(\x0e\x32\x16.allego.KpiMetricsEnum\"\x85\x01\n\tTimeRange\x12\x14\n\x0ctimeRangeSec\x18\x01 \x03(\x01\x12\x11\n\ttimestamp\x18\x02 \x03(\x03\x12\n\n\x02\x66s\x18\x03 \x02(\x01\x12\x15\n\rwallTimeStart\x18\x04 \x01(\t\x12,\n\x08wallTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"q\n\tBundleReq\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12$\n\x07metrics\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0e\n\x06isTail\x18\x05 \x02(\x08\"\x9d\x01\n\rKpiMetricsReq\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x1e\n\x03\x61rg\x18\x03 \x02(\x0b\x32\x11.allego.BundleReq\x12\x0e\n\x06isPlot\x18\x04 \x01(\x08\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x14\n\x0cisReturnData\x18\x06 \x01(\x08\"\x83\x03\n\x0eKpiMetricsData\x12\x12\n\nnumPackets\x18\x01 \x02(\x03\x12\x0f\n\x07numSigs\x18\x02 \x02(\x03\x12\x12\n\nnumMetrics\x18\x03 \x02(\x03\x12#\n\x06metric\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0f\n\x07pktIdxs\x18\x05 \x03(\x03\x12 \n\x03val\x18\x06 \x02(\x0b\x32\x13.allego.DenseMatrix\x12\x35\n\tstatsPkts\x18\x07 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x31\n\x05stats\x18\x08 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x14\n\x0cpacketDurSec\x18\t \x02(\x01\x12\x1d\n\x02tR\x18\n \x02(\x0b\x32\x11.allego.TimeRange\x1a\x41\n\x0bMetricStats\x12\x0c\n\x04mean\x18\x01 \x03(\x01\x12\n\n\x02sD\x18\x02 \x03(\x01\x12\x0b\n\x03max\x18\x03 \x03(\x01\x12\x0b\n\x03min\x18\x04 \x03(\x01\"w\n\x16KpiBundlePacketMetrics\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12#\n\x07sigType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\'\n\x07metrics\x18\x04 \x02(\x0b\x32\x16.allego.KpiMetricsData\"S\n\nKpiMetrics\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12.\n\x06\x62undle\x18\x02 \x02(\x0b\x32\x1e.allego.KpiBundlePacketMetrics\"c\n\x11KpiControlRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x14\n\x0cisAllBundles\x18\x03 \x01(\x08\":\n\x12SetKpiParamRequest\x12\x15\n\rstreamGroupId\x18\x01 \x01(\t\x12\r\n\x05param\x18\x02 \x01(\x01\",\n\x13GetKpiStatusRequest\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\"K\n\x12KpiStandardRequest\x12\x11\n\tdsourceID\x18\x02 \x03(\t\x12\"\n\x03\x63md\x18\x03 \x01(\x0e\x32\x15.allego.KpiScannerCmd\"\xba\x01\n\rKpiFileStatus\x12,\n\x07\x64source\x18\x01 \x03(\x0b\x32\x1b.allego.KpiFileStatus.State\x1a{\n\x05State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\nisComplete\x18\x02 \x01(\x08\x12\x12\n\ndsourceUID\x18\x03 \x01(\t\x12 \n\x05kpiTR\x18\x04 \x01(\x0b\x32\x11.allego.TimeRange\x12\x17\n\x0f\x66ilePathAndName\x18\x05 \x01(\t\"\xc7\x04\n\x0eKpiFileStatus2\x12>\n\x07\x64source\x18\x01 \x03(\x0b\x32-.allego.KpiFileStatus2.KpiDatasourceStateSpec\x1a\xe9\x01\n\tKPI_State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\nisComplete\x18\x02 \x01(\x08\x12\x14\n\x0c\x66racComplete\x18\x03 \x01(\x01\x12\x17\n\x0f\x66ilePathAndName\x18\x04 \x01(\t\x12 \n\x05kpiTR\x18\x05 \x01(\x0b\x32\x11.allego.TimeRange\x12\x14\n\x0cpacketDurSec\x18\x06 \x01(\x01\x12\x0e\n\x06numAmp\x18\x07 \x01(\x03\x12\x18\n\x10\x62ytesInBundlePkt\x18\x08 \x01(\x03\x12\x12\n\nnumPackets\x18\t \x01(\x03\x12\x12\n\ndatasetUID\x18\n \x01(\t\x1aq\n\x10\x44\x61tasource_State\x12\x17\n\x0f\x66ilePathAndName\x18\x01 \x01(\t\x12\x1d\n\x02TR\x18\x02 \x01(\x0b\x32\x11.allego.TimeRange\x12\x12\n\ndatasetUID\x18\x03 \x01(\t\x12\x11\n\tdsourceID\x18\x04 \x01(\t\x1a\x95\x01\n\x16KpiDatasourceStateSpec\x12\x37\n\x06source\x18\x01 \x02(\x0b\x32\'.allego.KpiFileStatus2.Datasource_State\x12-\n\x03kpi\x18\x02 \x02(\x0b\x32 .allego.KpiFileStatus2.KPI_State\x12\x13\n\x0bisSprinting\x18\x03 \x02(\x08\"\xfd\x01\n\x0fKpiFileMetadata\x12.\n\x07\x64source\x18\x01 \x03(\x0b\x32\x1d.allego.KpiFileMetadata.State\x1a\xb9\x01\n\x05State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\ndsourceUID\x18\x02 \x01(\t\x12\x11\n\tpacketDur\x18\x03 \x01(\x01\x12\x0c\n\x04nAMP\x18\x04 \x01(\x03\x12\x1b\n\x13\x62ytesInBundlePacket\x18\x05 \x01(\x03\x12\x12\n\nnumPackets\x18\x06 \x01(\x03\x12 \n\x05kpiTR\x18\x07 \x01(\x0b\x32\x11.allego.TimeRange\x12\x17\n\x0f\x66ilePathAndName\x18\x08 \x01(\t\"\xd3\x02\n\x0eKpiStatusReply\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x11\n\ttimeRange\x18\x03 \x01(\x01\x12\x16\n\x0etimestampRange\x18\x04 \x01(\x03\x12\x18\n\x10numPacketsMemory\x18\x05 \x02(\x03\x12\x11\n\tpacketDur\x18\x06 \x02(\x01\x12\x14\n\x0cupdatePeriod\x18\x07 \x02(\x01\x12\x13\n\x0bpersistence\x18\x08 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\t \x02(\x01\x12\x1d\n\x15isTrackingSignalCache\x18\x0b \x02(\x08\x12\x12\n\nnumPackets\x18\x0c \x02(\x03\x12\x13\n\x0bmemoryBytes\x18\r \x02(\x01\x12\n\n\x02\x66s\x18\x0e \x01(\x01\x12\x15\n\rwallTimeStart\x18\x0f \x01(\t\x12\x1d\n\x02tR\x18\x10 \x01(\x0b\x32\x11.allego.TimeRange\x12\x0f\n\x07numSigs\x18\x11 \x01(\x03\"\xe6\x02\n\x11SigKpiParamRecord\x12\x15\n\risEventDetect\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x11\n\teventThr0\x18\x03 \x02(\x01\x12\x11\n\teventThr1\x18\x04 \x02(\x01\x12\x13\n\x0b\x65ventThrSd0\x18\x05 \x02(\x01\x12\x13\n\x0b\x65ventThrSd1\x18\x06 \x02(\x01\x12\x11\n\tpreThrPts\x18\x07 \x02(\x05\x12\x12\n\npostThrPts\x18\x08 \x02(\x05\x12\x11\n\tevtDurPts\x18\t \x02(\x05\x12\x11\n\tshadowPts\x18\n \x02(\x05\x12\x0e\n\x06preThr\x18\x0b \x02(\x01\x12\x0f\n\x07postThr\x18\x0c \x02(\x01\x12\x0e\n\x06\x65vtDur\x18\r \x02(\x01\x12\x0e\n\x06shadow\x18\x0e \x02(\x01\x12\x11\n\tisSetThr0\x18\x0f \x02(\x08\x12\x11\n\tisSetThr1\x18\x10 \x02(\x08\x12\x10\n\x08isSDThr0\x18\x11 \x02(\x08\x12\x10\n\x08isSDThr1\x18\x12 \x02(\x08\"J\n\x0e\x41nnotateBundle\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\r\n\x05notes\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x01(\t\"]\n\x0fProjectMetadata\x12\x12\n\nprojectUID\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61seUID\x18\x02 \x01(\t\x12\x10\n\x08trialUID\x18\x03 \x01(\t\x12\x13\n\x0b\x61nnotateUID\x18\x04 \x03(\t\"3\n\x16SensorExtendedMetadata\x12\x19\n\x11sensorInstanceUID\x18\x01 \x01(\t\"%\n\x0fGonumMatrixList\x12\x12\n\nmdataBytes\x18\x01 \x02(\x0c\"6\n\x0fRadixMatrixList\x12#\n\x06matrix\x18\x01 \x03(\x0b\x32\x13.allego.RadixMatrix\"*\n\x0bRadixMatrix\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\x12\r\n\x05shape\x18\x02 \x03(\x05\"/\n\x10RadixMatrixBytes\x12\x0c\n\x04\x64\x61ta\x18\x01 \x02(\x0c\x12\r\n\x05shape\x18\x02 \x03(\x05\"8\n\x10RadixSignalsList\x12$\n\x06matrix\x18\x01 \x03(\x0b\x32\x14.allego.RadixSignals\"\xa9\x01\n\x0cRadixSignals\x12\x10\n\x08sampFreq\x18\x01 \x02(\x01\x12 \n\x03pri\x18\x02 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x61ux\x18\x03 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x64in\x18\x04 \x02(\x0b\x32\x13.allego.RadixMatrix\x12!\n\x04\x64out\x18\x05 \x02(\x0b\x32\x13.allego.RadixMatrix\"\x19\n\x0cVectorString\x12\t\n\x01x\x18\x01 \x03(\t\"\x1a\n\rVectorFloat64\x12\t\n\x01x\x18\x01 \x03(\x01\"G\n\x12VectorSliceFloat64\x12\"\n\x03vec\x18\x01 \x03(\x0b\x32\x15.allego.VectorFloat64\x12\r\n\x05label\x18\x02 \x01(\t\"\xde\x02\n\x14LogsysKpiStatusReply\x12\x1f\n\x05portA\x18\x01 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portB\x18\x02 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portC\x18\x03 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portD\x18\x04 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portE\x18\x05 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portF\x18\x06 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portG\x18\x07 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portH\x18\x08 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux0\x18\t \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux1\x18\n \x02(\x0b\x32\x10.allego.KpiCache\"\xfc\x02\n\x08KpiCache\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x15\n\rminNumPackets\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x05\x12\x12\n\nnumPackets\x18\x06 \x02(\x05\x12\x0e\n\x06tRange\x18\x07 \x03(\x01\x12\x0f\n\x07tsRange\x18\x08 \x03(\x03\x12\x15\n\rmeanPacketDur\x18\t \x02(\x01\x12\x19\n\x11meanCalcPacketDur\x18\n \x02(\x01\x12\x11\n\tpacketDur\x18\x0b \x02(\x01\x12\x1d\n\x15totalPacketsProcessed\x18\x0c \x02(\r\x12\x12\n\nsignalType\x18\r \x02(\t\x12\x12\n\nnumPriSigs\x18\x0e \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x0f \x02(\x05\x12\x12\n\nnumDinSigs\x18\x10 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x11 \x02(\x05\x12\x14\n\x0cupdatePeriod\x18\x12 \x02(\x01\"\xfa\x02\n\x12LogsysKpiTailReply\x12\"\n\x05portA\x18\x01 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portB\x18\x02 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portC\x18\x03 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portD\x18\x04 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portE\x18\x05 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portF\x18\x06 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portG\x18\x07 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portH\x18\x08 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux0\x18\t \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux1\x18\n \x01(\x0b\x32\x13.allego.KpiPortInfo\"3\n\x0bKpiPortInfo\x12$\n\x07kpiTail\x18\x01 \x03(\x0b\x32\x13.allego.KpiTailRows\"\xf4\x02\n\x0bKpiTailRows\x12\x10\n\x08wallTime\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x02(\x01\x12\x14\n\x0clocalSigType\x18\x03 \x02(\t\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x03\x12\x0b\n\x03\x64ur\x18\x05 \x02(\x01\x12\x0e\n\x06stdDev\x18\x06 \x02(\x01\x12\x0f\n\x07\x63StdDev\x18\x07 \x02(\x01\x12\x11\n\tabsEvtAmp\x18\x08 \x02(\x01\x12\x12\n\ncabsEvtAmp\x18\t \x02(\x01\x12\x0b\n\x03SNR\x18\n \x02(\x01\x12\x0c\n\x04\x63SNR\x18\x0b \x02(\x01\x12\x0f\n\x07numEvts\x18\x0c \x02(\x05\x12\x10\n\x08\x63numEvts\x18\r \x02(\x05\x12\x0f\n\x07\x65vtRate\x18\x0e \x02(\x01\x12\x10\n\x08\x63\x45vtRate\x18\x0f \x02(\x01\x12\x0b\n\x03max\x18\x10 \x02(\x01\x12\x0c\n\x04\x63max\x18\x11 \x02(\x01\x12\x0b\n\x03min\x18\x12 \x02(\x01\x12\x0c\n\x04\x63min\x18\x13 \x02(\x01\x12\x14\n\x0cmeanPosPkAmp\x18\x14 \x02(\x01\x12\x14\n\x0cmeanNegPkAmp\x18\x15 \x02(\x01\"*\n\x18WarehouseHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\"(\n\x19OutfitterGetDeviceRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x9e\x01\n\x11SensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x16\n\x0eisIncludeModel\x18\x03 \x01(\x08\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"z\n\x19RegisterSensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x11\n\tprofileID\x18\x03 \x02(\t\"\x92\x01\n\x1dSaveSensorCompInstanceRequest\x12 \n\x05probe\x18\x01 \x01(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x01(\x0b\x32\x15.allego.HeadstageDesc\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"&\n\tProbeDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"*\n\rHeadstageDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"`\n\x12GetSensorCompReply\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeSpec\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageSpec\"x\n\tProbeSpec\x12\x1f\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x11.allego.ProbeDesc\x12!\n\x05model\x18\x02 \x01(\x0b\x32\x12.allego.ProbeModel\x12\'\n\x08metaData\x18\x03 \x01(\x0b\x32\x15.allego.ProbeMetaData\"\x88\x01\n\rHeadstageSpec\x12#\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x15.allego.HeadstageDesc\x12%\n\x05model\x18\x02 \x01(\x0b\x32\x16.allego.HeadstageModel\x12+\n\x08metaData\x18\x03 \x01(\x0b\x32\x19.allego.HeadstageMetaData\"\xce\x04\n\nProbeModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12.\n\x04site\x18\x02 \x03(\x0b\x32 .allego.ProbeModel.ProbeSiteDesc\x12\x34\n\twireframe\x18\x03 \x02(\x0b\x32!.allego.ProbeModel.ProbeWireFrame\x12\x34\n\x0esiteOverallMin\x18\x05 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x34\n\x0esiteOverallMax\x18\x06 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x1a\xde\x01\n\rProbeSiteDesc\x12\x0c\n\x04\x61rea\x18\x01 \x02(\x01\x12\x0f\n\x07\x63\x65nterX\x18\x02 \x02(\x01\x12\x0f\n\x07\x63\x65nterY\x18\x03 \x02(\x01\x12\x0f\n\x07\x63\x65nterZ\x18\x04 \x02(\x01\x12\x11\n\tlimitXMax\x18\x05 \x02(\x01\x12\x11\n\tlimitXMin\x18\x06 \x02(\x01\x12\x11\n\tlimitYMax\x18\x07 \x02(\x01\x12\x11\n\tlimitYMin\x18\x08 \x02(\x01\x12\x11\n\tlimitZMax\x18\t \x02(\x01\x12\x11\n\tlimitZMin\x18\n \x02(\x01\x12\x0b\n\x03num\x18\x0b \x02(\x03\x12\r\n\x05shape\x18\x0c \x02(\t\x1a^\n\x0eProbeWireFrame\x12,\n\x06vertex\x18\x01 \x03(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x0e\n\x06limitX\x18\x02 \x03(\x01\x12\x0e\n\x06limitY\x18\x03 \x03(\x01\x1a!\n\tProbePtXY\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"_\n\rProbeMetaData\x12\x11\n\tprobeName\x18\x01 \x02(\t\x12\x10\n\x08numSites\x18\x02 \x02(\x05\x12\x13\n\x0b\x63\x61talogTags\x18\x03 \x02(\t\x12\x14\n\x0cinstanceTags\x18\x04 \x02(\t\"\x84\x01\n\x0eHeadstageModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12\x31\n\x04rows\x18\x02 \x03(\x0b\x32#.allego.HeadstageModel.HeadstageRow\x1a\x33\n\x0cHeadstageRow\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x03\x12\x0f\n\x07siteNum\x18\x02 \x02(\x03\"\x13\n\x11HeadstageMetaData\"5\n\x0bUserProfile\x12\x11\n\tprofileID\x18\x01 \x02(\t\x12\x13\n\x0blicenseCode\x18\x02 \x02(\t\"B\n\x16GetCurrentProfileReply\x12(\n\x0buserProfile\x18\x01 \x02(\x0b\x32\x13.allego.UserProfile\"@\n\x13GetAllProfilesReply\x12)\n\x0cuserProfiles\x18\x01 \x03(\x0b\x32\x13.allego.UserProfile\"-\n\x18SetCurrentProfileRequest\x12\x11\n\tprofileID\x18\x01 \x02(\t\"\x88\x01\n\x14ManageNodeOrgPayload\x12\r\n\x05orgID\x18\x01 \x01(\t\x12\x0f\n\x07orgName\x18\x02 \x01(\t\x12\x14\n\x0corgShortName\x18\x03 \x01(\t\x12\x0c\n\x04\x63ity\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\r\n\x05state\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"i\n\x14ManageNodeOrgRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\"S\n\x12ManageNodeOrgReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\xa2\x01\n\x14ManageNodeLabPayload\x12\r\n\x05labID\x18\x01 \x01(\t\x12\x0f\n\x07labDesc\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65pt\x18\x03 \x01(\t\x12\x14\n\x0corganization\x18\x04 \x01(\t\x12\x0f\n\x07\x61\x64minID\x18\x05 \x01(\t\x12\x11\n\tlabHeadID\x18\x06 \x01(\t\x12\x14\n\x0clabManagerID\x18\x07 \x01(\t\x12\x0c\n\x04tags\x18\x08 \x01(\t\"i\n\x14ManageNodeLabRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\"S\n\x12ManageNodeLabReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\x99\x01\n\x15ManageNodeUserPayload\x12\x0e\n\x06userID\x18\x01 \x01(\t\x12\x0c\n\x04Name\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\x0c\x12\"\n\x04role\x18\x04 \x01(\x0e\x32\x14.allego.UserRoleType\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x0f\n\x07labName\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"k\n\x15ManageNodeUserRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12.\n\x07payload\x18\x02 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\"U\n\x13ManageNodeUserReply\x12.\n\x07payload\x18\x01 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"6\n\x13\x43\x61talogProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"]\n\x10ProbeNodeRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12%\n\x07payload\x18\x02 \x03(\x0b\x32\x14.allego.ProbePayload\"7\n\x0eProbeNodeReply\x12%\n\x07payload\x18\x01 \x03(\x0b\x32\x14.allego.ProbePayload\"/\n\x0cProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"\xa5\x02\n\x0b\x45\x64gePayload\x12/\n\x06source\x18\x01 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12/\n\x06target\x18\x02 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12)\n\tedgeLabel\x18\x03 \x02(\x0e\x32\x16.allego.WorldEdgeLabel\x12-\n\tdirection\x18\x04 \x02(\x0e\x32\x1a.allego.WorldEdgeDirection\x1aZ\n\x0bGenericNode\x12%\n\x05label\x18\x01 \x02(\x0e\x32\x16.allego.WorldNodeLabel\x12\x11\n\tidPropKey\x18\x02 \x02(\t\x12\x11\n\tidPropVal\x18\x03 \x02(\t\"8\n\x10WorldEdgeRequest\x12$\n\x07payload\x18\x01 \x03(\x0b\x32\x13.allego.EdgePayload\"\x10\n\x0eWorldEdgeReply\"E\n\x11QueryWorldRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.WorldQueryCmd\x12\x0c\n\x04\x61rgs\x18\x02 \x03(\t\"\xe6\x01\n\rQueryWorldRec\x12)\n\x03org\x18\x01 \x01(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12)\n\x03lab\x18\x02 \x01(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12+\n\x04user\x18\x03 \x01(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12-\n\x08\x63\x61tProbe\x18\x04 \x01(\x0b\x32\x1b.allego.CatalogProbePayload\x12#\n\x05probe\x18\x05 \x01(\x0b\x32\x14.allego.ProbePayload\"9\n\x0fQueryWorldReply\x12&\n\x07payload\x18\x01 \x03(\x0b\x32\x15.allego.QueryWorldRec\"/\n\x1aHighLowPassTransformParams\x12\x11\n\tfrequency\x18\x01 \x02(\x01\"B\n\x13\x42\x61ndTransformParams\x12\x14\n\x0clowFrequency\x18\x01 \x02(\x01\x12\x15\n\rhighFrequency\x18\x02 \x02(\x01\"F\n\x14NotchTransformParams\x12\x16\n\x0enotchFrequency\x18\x01 \x02(\x01\x12\x16\n\x0enotchBandwidth\x18\x02 \x02(\x01\"\x14\n\x12\x43\x41RTransformParams\"2\n\x19VirtualRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\"K\n\x18PairedRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\x12\x18\n\x10targetNtvChanIdx\x18\x02 \x02(\x05\"i\n\x1d\x44\x61taSourceSinkTransformParams\x12\x10\n\x08\x64srcName\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\">\n\x18SliceTimeTransformParams\x12\x11\n\ttimeStart\x18\x01 \x02(\x01\x12\x0f\n\x07timeEnd\x18\x02 \x02(\x01\"n\n\x1cSliceChannelsTransformParams\x12\x13\n\x0bsysChanIdxs\x18\x01 \x03(\x05\x12(\n\x0bsignalGroup\x18\x02 \x01(\x0b\x32\x13.allego.SignalGroup\x12\x0f\n\x07\x64srcUid\x18\x03 \x01(\t\"1\n\x19\x44ownsampleTransformParams\x12\x14\n\x0csampleFactor\x18\x01 \x02(\x05\"\xec\x01\n\x1aRemapSensorTransformParams\x12>\n\x07sensors\x18\x01 \x03(\x0b\x32-.allego.RemapSensorTransformParams.SensorSpec\x12\x0f\n\x07\x64srcUid\x18\x03 \x01(\t\x1a}\n\nSensorSpec\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07probeId\x18\x03 \x02(\t\x12\x13\n\x0bheadstageId\x18\x04 \x02(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\x05 \x01(\x05\x12\x13\n\x0bnumChannels\x18\x06 \x01(\x05\" \n\x08Position\x12\t\n\x01x\x18\x01 \x02(\x05\x12\t\n\x01y\x18\x02 \x02(\x05\"\x98\x06\n\rTransformNode\x12\n\n\x02id\x18\x01 \x02(\t\x12\'\n\x04type\x18\x02 \x02(\x0e\x32\x19.allego.TransformNodeType\x12\"\n\x08position\x18\x03 \x01(\x0b\x32\x10.allego.Position\x12\x0f\n\x07invalid\x18\x04 \x02(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x05 \x01(\t\x12=\n\x11highLowPassParams\x18\x06 \x01(\x0b\x32\".allego.HighLowPassTransformParams\x12/\n\nbandParams\x18\x07 \x01(\x0b\x32\x1b.allego.BandTransformParams\x12\x31\n\x0bnotchParams\x18\x08 \x01(\x0b\x32\x1c.allego.NotchTransformParams\x12-\n\tcarParams\x18\t \x01(\x0b\x32\x1a.allego.CARTransformParams\x12;\n\x10virtualRefParams\x18\n \x01(\x0b\x32!.allego.VirtualRefTransformParams\x12\x39\n\x0fpairedRefParams\x18\x0b \x01(\x0b\x32 .allego.PairedRefTransformParams\x12\x43\n\x14\x64\x61tasourceSinkParams\x18\x0c \x01(\x0b\x32%.allego.DataSourceSinkTransformParams\x12\x39\n\x0fsliceTimeParams\x18\r \x01(\x0b\x32 .allego.SliceTimeTransformParams\x12\x41\n\x13sliceChannelsParams\x18\x0e \x01(\x0b\x32$.allego.SliceChannelsTransformParams\x12;\n\x10\x64ownsampleParams\x18\x0f \x01(\x0b\x32!.allego.DownsampleTransformParams\x12=\n\x11remapSensorParams\x18\x10 \x01(\x0b\x32\".allego.RemapSensorTransformParams\";\n\rTransformEdge\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0e\n\x06source\x18\x02 \x02(\t\x12\x0e\n\x06target\x18\x03 \x02(\t\"t\n\x08Protocol\x12\n\n\x02id\x18\x01 \x02(\t\x12-\n\x0etransformNodes\x18\x02 \x03(\x0b\x32\x15.allego.TransformNode\x12-\n\x0etransformEdges\x18\x03 \x03(\x0b\x32\x15.allego.TransformEdge\"%\n\x0fProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\"B\n\x15RenameProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\x12\x15\n\rnewProtocolID\x18\x02 \x02(\t\";\n\x14GetAllProtocolsReply\x12#\n\tprotocols\x18\x01 \x03(\x0b\x32\x10.allego.Protocol\"{\n\x15\x41pplyProtocolProgress\x12\x1c\n\x14lastTimestampWritten\x18\x01 \x02(\x05\x12\x18\n\x10\x64srcTimestampEnd\x18\x02 \x02(\x05\x12\x14\n\x0c\x66racComplete\x18\x03 \x01(\x01\x12\x14\n\x0cincrementSec\x18\x04 \x01(\x01\"\x9a\x01\n\x1aSpikeSorterSetParamRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12,\n\x03\x63md\x18\x02 \x02(\x0e\x32\x1f.allego.SpikeSorterParamCommand\x12\x12\n\nregFloat64\x18\x03 \x03(\x01\x12\x0f\n\x07regBool\x18\x05 \x03(\x08\x12\x12\n\nntvChanIdx\x18\x06 \x03(\x05\"Q\n\x1bSpikeSorterSetParamsRequest\x12\x32\n\x06params\x18\x01 \x03(\x0b\x32\".allego.SpikeSorterSetParamRequest\"\xa7\x02\n\x1dSpikeSorterParamCommandRecord\x12\x11\n\tisEnabled\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x0b\n\x03thr\x18\x03 \x03(\x01\x12\r\n\x05thrSd\x18\x04 \x03(\x01\x12\x11\n\tthrWdwPts\x18\x05 \x03(\x05\x12\x0e\n\x06thrWdw\x18\x06 \x03(\x01\x12\x0e\n\x06shadow\x18\x07 \x02(\x01\x12\x11\n\tshadowPts\x18\x08 \x02(\x05\x12\x10\n\x08isSetThr\x18\t \x03(\x08\x12\x0f\n\x07weakThr\x18\n \x03(\x01\x12\x11\n\tweakThrSd\x18\x0b \x03(\x01\x12\x14\n\x0cisSetWeakThr\x18\x0c \x03(\x08\x12\x12\n\npeakWdwPts\x18\r \x03(\x05\x12\x0f\n\x07peakWdw\x18\x0e \x03(\x01\x12\x0c\n\x04isSD\x18\x0f \x02(\x08\"?\n\tKpiParams\x12\x32\n\x03rec\x18\x01 \x03(\x0b\x32%.allego.SpikeSorterParamCommandRecord\"J\n\x10\x44\x41\x43StreamRequest\x12\x0b\n\x03\x44\x41\x43\x18\x01 \x02(\x05\x12\x12\n\nNtvChanIdx\x18\x02 \x02(\x05\x12\x15\n\rstreamGroupId\x18\x03 \x01(\t\"\xde\x01\n\x11\x45ventViewerConfig\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x19\n\x11triggerSysChanIdx\x18\x03 \x01(\x05\x12\x1a\n\x12triggerThresholdUV\x18\x04 \x01(\x01\x12\x14\n\x0cpreTriggerMs\x18\x05 \x02(\x01\x12\x15\n\rpostTriggerMs\x18\x06 \x02(\x01\x12\'\n\x0btriggerType\x18\x07 \x01(\x0e\x32\x12.allego.SignalType\x12\x0e\n\x06ntvIdx\x18\x08 \x01(\x05\"=\n\rEventViewerID\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\"D\n\x1aGetEventViewerEventRequest\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x0f\n\x07\x65ventId\x18\x02 \x02(\t\"Y\n\x14\x45ventViewerEventDesc\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\"\x8f\x01\n\x10\x45ventViewerEvent\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12\x13\n\x0bsysChanIdxs\x18\x05 \x03(\x05\"a\n\x1aListEventViewerEventsReply\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12,\n\x06\x65vents\x18\x02 \x03(\x0b\x32\x1c.allego.EventViewerEventDesc\"D\n\x15ListEventViewersReply\x12+\n\x0c\x65ventViewers\x18\x01 \x03(\x0b\x32\x15.allego.EventViewerID\"3\n\x1fStatusPollFieldsToUpdateRequest\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\"^\n\x18StatusPollFieldsToUpdate\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\x12\x30\n\x0e\x66ieldsToUpdate\x18\x02 \x03(\x0e\x32\x18.allego.StatusPollFields\"\xa5\x01\n\x17\x44\x61shboardCommandRequest\x12\'\n\x08\x64\x61shType\x18\x01 \x01(\x0e\x32\x15.allego.DashboardType\x12\x32\n\x04\x61rgs\x18\x02 \x01(\x0b\x32$.allego.DashboardCommandRequest.Args\x1a-\n\x04\x41rgs\x12%\n\x03\x63md\x18\x01 \x02(\x0e\x32\x18.allego.DashboardCommand\"]\n\x13SelTableSignalGroup\x12\r\n\x05index\x18\x01 \x02(\t\x12\x15\n\rcriterionDesc\x18\x02 \x02(\t\x12\x0f\n\x07ntvIdxs\x18\x03 \x03(\x03\x12\x0f\n\x07numSigs\x18\x04 \x02(\x03\"?\n\x13SelectorTablesReply\x12(\n\x03sig\x18\x01 \x03(\x0b\x32\x1b.allego.SelTableSignalGroup\"\xfa\x02\n\x10\x44\x61taSourceStatus\x12%\n\x04type\x18\x01 \x02(\x0e\x32\x17.allego.SignalGroupType\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12\x10\n\x08\x64uration\x18\x04 \x02(\x01\x12(\n\x0bsignalGroup\x18\x06 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x17\n\x0fnumTotalSamples\x18\x07 \x02(\x03\x12\x12\n\nsampleFreq\x18\t \x01(\x01\x12\x0b\n\x03uid\x18\n \x02(\t\x12\x16\n\x0e\x64\x61taSourceType\x18\x0b \x02(\t\x12\x10\n\x08\x66ileType\x18\x0c \x02(\t\x12\x0c\n\x04mode\x18\r \x02(\t\x12\r\n\x05label\x18\x0e \x02(\t\x12\x0c\n\x04path\x18\x0f \x02(\t\x12\x14\n\x0c\x62\x61seFileName\x18\x10 \x02(\t\x12\x1d\n\x02tR\x18\x11 \x01(\x0b\x32\x11.allego.TimeRange\x12\x14\n\x0ckpiDsourceID\x18\x12 \x01(\t*\x96\x02\n\x0eRadixFileTypes\x12\x07\n\x03RHD\x10\x00\x12\x08\n\x04XDAT\x10\x01\x12\x07\n\x03\x43SV\x10\x02\x12\x08\n\x04HDF5\x10\x03\x12\x08\n\x04NEX5\x10\x04\x12\x07\n\x03NWB\x10\x05\x12\x10\n\x0c\x42IOINTERFACE\x10\x07\x12\r\n\tKILOSORT2\x10\x08\x12\x07\n\x03\x41NC\x10\t\x12\x0f\n\x0bSPKTRAIN_MU\x10\n\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_HDF5\x10\x0b\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_MAT5\x10\x0c\x12\x07\n\x03NSX\x10\r\x12\x07\n\x03PL2\x10\x0e\x12\x07\n\x03TDT\x10\x0f\x12\n\n\x06SPIKES\x10\x10\x12\x07\n\x03KPI\x10\x11\x12\x15\n\x11UNKNOWN_FILE_TYPE\x10\x12\x12\x0f\n\x0bMEAREC_HDF5\x10\x13*1\n\nSignalType\x12\x07\n\x03PRI\x10\x00\x12\x07\n\x03\x41UX\x10\x01\x12\x07\n\x03\x44IN\x10\x02\x12\x08\n\x04\x44OUT\x10\x03*:\n\x0fResampleRoutine\x12\t\n\x05NAIVE\x10\x00\x12\r\n\tRETENTIVE\x10\x01\x12\r\n\tANTIALIAS\x10\x03*>\n\x04Port\x12\x05\n\x01\x41\x10\x00\x12\x05\n\x01\x42\x10\x01\x12\x05\n\x01\x43\x10\x02\x12\x05\n\x01\x44\x10\x03\x12\x05\n\x01\x45\x10\x04\x12\x05\n\x01\x46\x10\x05\x12\x05\n\x01G\x10\x06\x12\x05\n\x01H\x10\x07*2\n\x0cWorkspaceApp\x12\n\n\x06\x41llego\x10\x00\x12\n\n\x06\x43urate\x10\x01\x12\n\n\x06Videre\x10\x02*\xa0\x01\n\x11WorkspaceCommands\x12\x0f\n\x0bWSPACE_Save\x10\x00\x12\x11\n\rWSPACE_SaveAs\x10\x01\x12\x11\n\rWSPACE_Export\x10\x02\x12\x11\n\rWSPACE_Import\x10\x03\x12\x11\n\rWSPACE_Delete\x10\x04\x12\x11\n\rWSPACE_Switch\x10\x07\x12\x1b\n\x17WSPACE_SwitchToLastUsed\x10\x08*C\n\x14GetWorkspaceCommands\x12\x13\n\x0fGET_WSPACE_List\x10\x01\x12\x16\n\x12GET_WSPACE_Current\x10\x02*8\n\x11RadiensServerType\x12\x10\n\x0c\x41llegoserver\x10\x00\x12\x11\n\rRadiensserver\x10\x01*\xae\x01\n\x0fGrpcServiceType\x12\x0f\n\x0b\x41LLEGO_CORE\x10\x00\x12\x11\n\rALLEGO_PCACHE\x10\x01\x12\x0e\n\nALLEGO_KPI\x10\x02\x12\x12\n\x0e\x41LLEGO_NEURONS\x10\x03\x12\x10\n\x0cRADIENS_CORE\x10\x04\x12\x18\n\x14RADIENS_SPIKE_SORTER\x10\x05\x12\x0f\n\x0bRADIENS_DEV\x10\x06\x12\x16\n\x12RADIENS_DASHBOARDS\x10\x07*?\n\x0e\x44\x65vDatasetType\x12\x08\n\x04\x42\x41SE\x10\x00\x12\t\n\x05TRAIN\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x08\n\x04TEST\x10\x03*C\n\rPSDWindowType\x12\x0f\n\x0bHAMMING_p01\x10\x00\x12\x0f\n\x0bHAMMING_p05\x10\x01\x12\x10\n\x0cPASS_THROUGH\x10\x02*\x1e\n\nPSDScaling\x12\x10\n\x0cPSD_ABSOLUTE\x10\x00*X\n\x0e\x44\x61taSourceSort\x12\x10\n\x0c\x44SOURCE_DATE\x10\x00\x12\x10\n\x0c\x44SOURCE_NAME\x10\x01\x12\x10\n\x0c\x44SOURCE_SIZE\x10\x02\x12\x10\n\x0c\x44SOURCE_TYPE\x10\x03*.\n\x0fSignalGroupType\x12\x11\n\rPRIMARY_CACHE\x10\x00\x12\x08\n\x04\x46ILE\x10\x03*\x81\x01\n\x07\x44SPType\x12\x0b\n\x07LOWPASS\x10\x00\x12\x0c\n\x08HIGHPASS\x10\x01\x12\x0c\n\x08\x42\x41NDPASS\x10\x02\x12\t\n\x05NOTCH\x10\x03\x12\x0c\n\x08\x42\x41NDSTOP\x10\x04\x12\x07\n\x03\x43\x41R\x10\x05\x12\x15\n\x11VIRTUAL_REFERENCE\x10\x06\x12\x14\n\x10PAIRED_REFERENCE\x10\x07*9\n\x0b\x46ilterStage\x12\x12\n\x0eSTAGE_HARDWARE\x10\x00\x12\n\n\x06STAGE1\x10\x01\x12\n\n\x06STAGE2\x10\x02*\xd3\x02\n\x0e\x46\x65\x61tureLicense\x12\x1a\n\x16\x46\x65\x61t_NoLicenseRequired\x10\x00\x12\x0c\n\x08\x46\x65\x61t_Any\x10\x01\x12\x0f\n\x0b\x46\x65\x61t_Power9\x10\x02\x12\x11\n\rFeat_RadixAPI\x10\x03\x12\x0e\n\nFeat_Scope\x10\x04\x12\x13\n\x0f\x46\x65\x61t_Electrodes\x10\x05\x12\x13\n\x0f\x46\x65\x61t_HDSnapshot\x10\x06\x12\x12\n\x0e\x46\x65\x61t_Impedance\x10\x07\x12\x10\n\x0c\x46\x65\x61t_Monitor\x10\x08\x12\x16\n\x12\x46\x65\x61t_SignalMetrics\x10\t\x12\x19\n\x15\x46\x65\x61t_SignalProcessing\x10\n\x12\x0f\n\x0b\x46\x65\x61t_System\x10\x0b\x12\x12\n\x0e\x46\x65\x61t_SpikeGrid\x10\x0c\x12\x14\n\x10\x46\x65\x61t_SpikeSorter\x10\r\x12\x0f\n\x0b\x46\x65\x61t_Raster\x10\x0e\x12\x14\n\x10\x46\x65\x61t_ThreeDModel\x10\x0f*\xed\x01\n\x10SummaryStatsEnum\x12\x10\n\x0cSS_STAT_MEAN\x10\x00\x12\x0e\n\nSS_STAT_SD\x10\x01\x12\x10\n\x0cSS_STAT_MODE\x10\x02\x12\x0f\n\x0bSS_STAT_MIN\x10\x03\x12\x0f\n\x0bSS_STAT_MAX\x10\x04\x12\x16\n\x12SS_STAT_MODE_COUNT\x10\x05\x12\x12\n\x0eSS_STAT_MEDIAN\x10\x06\x12\x0f\n\x0bSS_STAT_Q25\x10\x07\x12\x0f\n\x0bSS_STAT_Q75\x10\x08\x12\x10\n\x0cSS_STAT_SKEW\x10\t\x12\x14\n\x10SS_STAT_KURTOSIS\x10\n\x12\r\n\tSS_STAT_N\x10\x0b*_\n\x0eKpiMetricsMode\x12\x18\n\x14Kpi_MetricsMode_Base\x10\x00\x12\x17\n\x13Kpi_MetricsMode_Avg\x10\x01\x12\x1a\n\x16Kpi_MetricsMode_Stream\x10\x02*\xa1\x06\n\x0eKpiMetricsEnum\x12\x0f\n\x0bKPI_NUM_PTS\x10\x00\x12\x13\n\x0fKPI_NUM_PTS_ISI\x10\x01\x12\x0f\n\x0bKPI_DUR_SEC\x10\x02\x12\x0c\n\x08KPI_MEAN\x10\x03\x12\x0b\n\x07KPI_MIN\x10\x04\x12\x0f\n\x0bKPI_MIN_ISI\x10\x05\x12\x0b\n\x07KPI_MAX\x10\x06\x12\x0f\n\x0bKPI_MAX_ISI\x10\x07\x12\x0f\n\x0bKPI_MAX_ABS\x10\x08\x12\x13\n\x0fKPI_MAX_ABS_ISI\x10\t\x12\x15\n\x11KPI_TIMESTAMP_MIN\x10\n\x12\x15\n\x11KPI_TIMESTAMP_MAX\x10\x0b\x12\x18\n\x14KPI_MAX_MIN_DIFF_ABS\x10\x0c\x12\x1c\n\x18KPI_MAX_MIN_DIFF_ABS_ISI\x10\r\x12\n\n\x06KPI_SD\x10\x0e\x12\x0e\n\nKPI_SD_ISI\x10\x0f\x12\x0b\n\x07KPI_VAR\x10\x10\x12\x0f\n\x0bKPI_VAR_ISI\x10\x11\x12\x0b\n\x07KPI_RMS\x10\x12\x12\x0f\n\x0bKPI_RMS_ISI\x10\x13\x12\x10\n\x0cKPI_NOISE_UV\x10\x14\x12\x0b\n\x07KPI_SNR\x10\x15\x12\x12\n\x0eKPI_NUM_EVENTS\x10\x16\x12\x12\n\x0eKPI_EVENT_RATE\x10\x17\x12\x11\n\rKPI_EVENT_MAX\x10\x18\x12\x11\n\rKPI_EVENT_MIN\x10\x19\x12\x15\n\x11KPI_EVENT_MAX_ABS\x10\x1a\x12\x1e\n\x1aKPI_EVENT_MAX_MIN_DIFF_ABS\x10\x1b\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MIN\x10\x1c\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MAX\x10\x1d\x12\x1f\n\x1bKPI_EVENT_TIMESTAMP_MAX_ABS\x10\x1e\x12(\n$KPI_EVENT_TIMESTAMP_MAX_MIN_DIFF_ABS\x10\x1f\x12\x10\n\x0cKPI_MEAN_MAX\x10 \x12\x10\n\x0cKPI_MEAN_MIN\x10!\x12\x14\n\x10KPI_MEAN_MAX_ABS\x10\"\x12#\n\x1fKPI_EVENT_MEAN_MAX_MIN_DIFF_ABS\x10#\x12\"\n\x1eKPI_MAX_MIN_DIFF_ABS_AMPLIFIED\x10$*\x8b\x01\n\x13KpiMetricsStatsEnum\x12\x1e\n\x1aKPI_BDL_METRICS_STATS_MEAN\x10\x00\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MAX\x10\x01\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MIN\x10\x02\x12\x16\n\x12KPI_BDL_METRICS_SD\x10\x03*\xc0\x02\n\x19KpiBundlePacketsStatsEnum\x12\x14\n\x10KPI_BDL_NUM_SIGS\x10\x00\x12\x13\n\x0fKPI_BDL_DUR_SEC\x10\x01\x12\x1d\n\x19KPI_BDL_NUM_SIGS_W_EVENTS\x10\x02\x12\x15\n\x11KPI_BDL_SIG_YIELD\x10\x03\x12\x13\n\x0fKPI_BDL_RMS_AVG\x10\x04\x12\x13\n\x0fKPI_BDL_SNR_AVG\x10\x05\x12\x13\n\x0fKPI_BDL_SIG_MAX\x10\x06\x12\x13\n\x0fKPI_BDL_SIG_MIN\x10\x07\x12\x18\n\x14KPI_BDL_NOISE_UV_AVG\x10\x08\x12\x1c\n\x18KPI_BDL_NUM_EVENTS_TOTAL\x10\t\x12\x1a\n\x16KPI_BDL_NUM_EVENTS_AVG\x10\n\x12\x1a\n\x16KPI_BDL_EVENT_RATE_AVG\x10\x0b*F\n\x10TimeRangeSelMode\x12\x0e\n\nTRS_SUBSET\x10\x00\x12\x0f\n\x0bTRS_TO_HEAD\x10\x01\x12\x11\n\rTRS_FROM_HEAD\x10\x02*e\n\rKpiScannerCmd\x12\x13\n\x0fKPI_SCANNER_OFF\x10\x00\x12\x1e\n\x1aKPI_SCANNER_BESPOKE_SPRINT\x10\x01\x12\x1f\n\x1bKPI_SCANNER_STANDARD_SPRINT\x10\x02*N\n\x16OutfitterComponentType\x12\x16\n\x12OUTFIT_COMP_SENSOR\x10\x00\x12\x1c\n\x18OUTFIT_COMP_SPIKE_SORTER\x10\x01*}\n\x0eWorldNodeLabel\x12\x12\n\x0eWORLD_NODE_ORG\x10\x01\x12\x12\n\x0eWORLD_NODE_LAB\x10\x02\x12\x13\n\x0fWORLD_NODE_USER\x10\x03\x12\x18\n\x14WORLD_NODE_CAT_PROBE\x10\x04\x12\x14\n\x10WORLD_NODE_PROBE\x10\x05*\'\n\x0eWorldEdgeLabel\x12\x15\n\x11WORLD_EDGE_MEMBER\x10\x01*`\n\x12WorldEdgeDirection\x12\x18\n\x14WORLD_EDGE_DIR_RIGHT\x10\x01\x12\x17\n\x13WORLD_EDGE_DIR_LEFT\x10\x02\x12\x17\n\x13WORLD_EDGE_DIR_BOTH\x10\x03*\x9f\x01\n\x0cUserRoleType\x12\x0b\n\x07USER_PI\x10\x01\x12\x12\n\x0eUSER_SCIENTIST\x10\x02\x12\x11\n\rUSER_POST_DOC\x10\x03\x12\x15\n\x11USER_GRAD_STUDENT\x10\x04\x12\x13\n\x0fUSER_UG_STUDENT\x10\x05\x12\x10\n\x0cUSER_MANAGER\x10\x06\x12\r\n\tUSER_TECH\x10\x07\x12\x0e\n\nUSER_OTHER\x10\x08*G\n\rManageNodeCmd\x12\x10\n\x0cNODE_CMD_NEW\x10\x01\x12\x12\n\x0eNODE_CMD_MERGE\x10\x02\x12\x10\n\x0cNODE_CMD_DEL\x10\x03*\xe8\x01\n\rWorldQueryCmd\x12\x15\n\x11WQ_LIST_ALL_USERS\x10\x01\x12\x14\n\x10WQ_LIST_ALL_LABS\x10\x02\x12\x14\n\x10WQ_LIST_ALL_ORGS\x10\x03\x12\x1a\n\x16WQ_LIST_ALL_CAT_PROBES\x10\x04\x12\x16\n\x12WQ_LIST_ALL_PROBES\x10\x05\x12\x18\n\x14WQ_CAT_PROBE_BY_NAME\x10\x06\x12\x11\n\rWQ_USER_BY_ID\x10\x07\x12\x19\n\x15WQ_USER_AND_LAB_BY_ID\x10\x08\x12\x18\n\x14WQ2_LIST_ALL_DEVICES\x10\x1e*\x82\x02\n\x11TransformNodeType\x12\x10\n\x0cNOTCH_FILTER\x10\x00\x12\x13\n\x0f\x42\x41NDPASS_FILTER\x10\x01\x12\x13\n\x0f\x42\x41NDSTOP_FILTER\x10\x02\x12\x13\n\x0fHIGHPASS_FILTER\x10\x03\x12\x12\n\x0eLOWPASS_FILTER\x10\x04\x12\x0e\n\nPAIRED_REF\x10\x05\x12\x0f\n\x0bVIRTUAL_REF\x10\x06\x12\x0b\n\x07\x43\x41R_REF\x10\x07\x12\x0e\n\nSLICE_TIME\x10\t\x12\x12\n\x0eSLICE_CHANNELS\x10\n\x12\n\n\x06SOURCE\x10\x0b\x12\x08\n\x04SINK\x10\x0c\x12\x0e\n\nDOWNSAMPLE\x10\r\x12\x10\n\x0cREMAP_SENSOR\x10\x0e*\xdf\x01\n\x17SpikeSorterParamCommand\x12\x14\n\x10SORTER_THR_LEVEL\x10\x01\x12\x17\n\x13SORTER_THR_LEVEL_SD\x10\x04\x12\x12\n\x0eSORTER_THR_WDW\x10\x08\x12\x19\n\x15SORTER_WEAK_THR_LEVEL\x10\n\x12\x1c\n\x18SORTER_WEAK_THR_LEVEL_SD\x10\r\x12\x11\n\rSORTER_SHADOW\x10\x11\x12\x17\n\x13SORTER_THR_ACTIVATE\x10\x13\x12\x1c\n\x18SORTER_WEAK_THR_ACTIVATE\x10\x15*\xee\x03\n\x10StatusPollFields\x12\x19\n\x15PORT_CONNECTION_STATE\x10\x00\x12\x14\n\x10RECORDING_ERRORS\x10\x01\x12\x15\n\x11STREAM_TIME_RANGE\x10\x02\x12\x11\n\rSTREAM_STATUS\x10\x03\x12\x11\n\rRECORD_STATUS\x10\x04\x12\x10\n\x0cIS_CONNECTED\x10\x06\x12\x0e\n\nRECORD_DUR\x10\x07\x12\x11\n\rBACKBONE_MODE\x10\t\x12\x10\n\x0cSIGNAL_GROUP\x10\n\x12\x14\n\x10SINAPS_REGISTERS\x10\x0b\x12\x14\n\x10RECORDING_CONFIG\x10\x0c\x12\x0b\n\x07\x46ILTERS\x10\r\x12\x17\n\x13\x45VENT_THRESH_PARAMS\x10\x0e\x12\x10\n\x0c\x44\x41\x43_REGISTER\x10\x0f\x12\x10\n\x0c\x44IO_REGISTER\x10\x10\x12\x10\n\x0cTRIGGER_MODE\x10\x11\x12\x11\n\rCABLE_LENGTHS\x10\x12\x12\x11\n\rEVENT_VIEWERS\x10\x13\x12\x0f\n\x0bSAMPLE_RATE\x10\x14\x12\x0e\n\nALL_FIELDS\x10\x15\x12\x16\n\x12SPIKE_SORTER_STATE\x10\x16\x12\x0f\n\x0bSTIM_PARAMS\x10\x17\x12\x19\n\x15SPIKE_SORTER_WARNINGS\x10\x18\x12\x12\n\x0eSTIM_STEP_SIZE\x10\x19*\x1b\n\rDashboardType\x12\n\n\x06\x44\x41SH_1\x10\x00*N\n\x10\x44\x61shboardCommand\x12\x11\n\rDASH_CMD_OPEN\x10\x00\x12\x12\n\x0e\x44\x41SH_CMD_CLOSE\x10\x01\x12\x13\n\x0f\x44\x41SH_CMD_UPDATE\x10\x02\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
@@ -28,86 +28,86 @@
   _SERVERSPEC_SERVICEENTRY._serialized_options = b'8\001'
   _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._options = None
   _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._serialized_options = b'8\001'
   _SIGNALGROUPUNITS_UNITSENTRY._options = None
   _SIGNALGROUPUNITS_UNITSENTRY._serialized_options = b'8\001'
   _UPDATESIGNALGROUPREQUEST.fields_by_name['ntvChanIdx']._options = None
   _UPDATESIGNALGROUPREQUEST.fields_by_name['ntvChanIdx']._serialized_options = b'\020\001'
-  _RADIXFILETYPES._serialized_start=24615
-  _RADIXFILETYPES._serialized_end=24893
-  _SIGNALTYPE._serialized_start=24895
-  _SIGNALTYPE._serialized_end=24944
-  _RESAMPLEROUTINE._serialized_start=24946
-  _RESAMPLEROUTINE._serialized_end=25004
-  _PORT._serialized_start=25006
-  _PORT._serialized_end=25068
-  _WORKSPACEAPP._serialized_start=25070
-  _WORKSPACEAPP._serialized_end=25120
-  _WORKSPACECOMMANDS._serialized_start=25123
-  _WORKSPACECOMMANDS._serialized_end=25283
-  _GETWORKSPACECOMMANDS._serialized_start=25285
-  _GETWORKSPACECOMMANDS._serialized_end=25352
-  _RADIENSSERVERTYPE._serialized_start=25354
-  _RADIENSSERVERTYPE._serialized_end=25410
-  _GRPCSERVICETYPE._serialized_start=25413
-  _GRPCSERVICETYPE._serialized_end=25587
-  _DEVDATASETTYPE._serialized_start=25589
-  _DEVDATASETTYPE._serialized_end=25652
-  _PSDWINDOWTYPE._serialized_start=25654
-  _PSDWINDOWTYPE._serialized_end=25721
-  _PSDSCALING._serialized_start=25723
-  _PSDSCALING._serialized_end=25753
-  _DATASOURCESORT._serialized_start=25755
-  _DATASOURCESORT._serialized_end=25843
-  _SIGNALGROUPTYPE._serialized_start=25845
-  _SIGNALGROUPTYPE._serialized_end=25891
-  _DSPTYPE._serialized_start=25894
-  _DSPTYPE._serialized_end=26023
-  _FILTERSTAGE._serialized_start=26025
-  _FILTERSTAGE._serialized_end=26082
-  _FEATURELICENSE._serialized_start=26085
-  _FEATURELICENSE._serialized_end=26424
-  _SUMMARYSTATSENUM._serialized_start=26427
-  _SUMMARYSTATSENUM._serialized_end=26664
-  _KPIMETRICSMODE._serialized_start=26666
-  _KPIMETRICSMODE._serialized_end=26761
-  _KPIMETRICSENUM._serialized_start=26764
-  _KPIMETRICSENUM._serialized_end=27565
-  _KPIMETRICSSTATSENUM._serialized_start=27568
-  _KPIMETRICSSTATSENUM._serialized_end=27707
-  _KPIBUNDLEPACKETSSTATSENUM._serialized_start=27710
-  _KPIBUNDLEPACKETSSTATSENUM._serialized_end=28030
-  _TIMERANGESELMODE._serialized_start=28032
-  _TIMERANGESELMODE._serialized_end=28102
-  _KPISCANNERCMD._serialized_start=28104
-  _KPISCANNERCMD._serialized_end=28205
-  _OUTFITTERCOMPONENTTYPE._serialized_start=28207
-  _OUTFITTERCOMPONENTTYPE._serialized_end=28285
-  _WORLDNODELABEL._serialized_start=28287
-  _WORLDNODELABEL._serialized_end=28412
-  _WORLDEDGELABEL._serialized_start=28414
-  _WORLDEDGELABEL._serialized_end=28453
-  _WORLDEDGEDIRECTION._serialized_start=28455
-  _WORLDEDGEDIRECTION._serialized_end=28551
-  _USERROLETYPE._serialized_start=28554
-  _USERROLETYPE._serialized_end=28713
-  _MANAGENODECMD._serialized_start=28715
-  _MANAGENODECMD._serialized_end=28786
-  _WORLDQUERYCMD._serialized_start=28789
-  _WORLDQUERYCMD._serialized_end=29021
-  _TRANSFORMNODETYPE._serialized_start=29024
-  _TRANSFORMNODETYPE._serialized_end=29282
-  _SPIKESORTERPARAMCOMMAND._serialized_start=29285
-  _SPIKESORTERPARAMCOMMAND._serialized_end=29508
-  _STATUSPOLLFIELDS._serialized_start=29511
-  _STATUSPOLLFIELDS._serialized_end=30005
-  _DASHBOARDTYPE._serialized_start=30007
-  _DASHBOARDTYPE._serialized_end=30034
-  _DASHBOARDCOMMAND._serialized_start=30036
-  _DASHBOARDCOMMAND._serialized_end=30114
+  _RADIXFILETYPES._serialized_start=24635
+  _RADIXFILETYPES._serialized_end=24913
+  _SIGNALTYPE._serialized_start=24915
+  _SIGNALTYPE._serialized_end=24964
+  _RESAMPLEROUTINE._serialized_start=24966
+  _RESAMPLEROUTINE._serialized_end=25024
+  _PORT._serialized_start=25026
+  _PORT._serialized_end=25088
+  _WORKSPACEAPP._serialized_start=25090
+  _WORKSPACEAPP._serialized_end=25140
+  _WORKSPACECOMMANDS._serialized_start=25143
+  _WORKSPACECOMMANDS._serialized_end=25303
+  _GETWORKSPACECOMMANDS._serialized_start=25305
+  _GETWORKSPACECOMMANDS._serialized_end=25372
+  _RADIENSSERVERTYPE._serialized_start=25374
+  _RADIENSSERVERTYPE._serialized_end=25430
+  _GRPCSERVICETYPE._serialized_start=25433
+  _GRPCSERVICETYPE._serialized_end=25607
+  _DEVDATASETTYPE._serialized_start=25609
+  _DEVDATASETTYPE._serialized_end=25672
+  _PSDWINDOWTYPE._serialized_start=25674
+  _PSDWINDOWTYPE._serialized_end=25741
+  _PSDSCALING._serialized_start=25743
+  _PSDSCALING._serialized_end=25773
+  _DATASOURCESORT._serialized_start=25775
+  _DATASOURCESORT._serialized_end=25863
+  _SIGNALGROUPTYPE._serialized_start=25865
+  _SIGNALGROUPTYPE._serialized_end=25911
+  _DSPTYPE._serialized_start=25914
+  _DSPTYPE._serialized_end=26043
+  _FILTERSTAGE._serialized_start=26045
+  _FILTERSTAGE._serialized_end=26102
+  _FEATURELICENSE._serialized_start=26105
+  _FEATURELICENSE._serialized_end=26444
+  _SUMMARYSTATSENUM._serialized_start=26447
+  _SUMMARYSTATSENUM._serialized_end=26684
+  _KPIMETRICSMODE._serialized_start=26686
+  _KPIMETRICSMODE._serialized_end=26781
+  _KPIMETRICSENUM._serialized_start=26784
+  _KPIMETRICSENUM._serialized_end=27585
+  _KPIMETRICSSTATSENUM._serialized_start=27588
+  _KPIMETRICSSTATSENUM._serialized_end=27727
+  _KPIBUNDLEPACKETSSTATSENUM._serialized_start=27730
+  _KPIBUNDLEPACKETSSTATSENUM._serialized_end=28050
+  _TIMERANGESELMODE._serialized_start=28052
+  _TIMERANGESELMODE._serialized_end=28122
+  _KPISCANNERCMD._serialized_start=28124
+  _KPISCANNERCMD._serialized_end=28225
+  _OUTFITTERCOMPONENTTYPE._serialized_start=28227
+  _OUTFITTERCOMPONENTTYPE._serialized_end=28305
+  _WORLDNODELABEL._serialized_start=28307
+  _WORLDNODELABEL._serialized_end=28432
+  _WORLDEDGELABEL._serialized_start=28434
+  _WORLDEDGELABEL._serialized_end=28473
+  _WORLDEDGEDIRECTION._serialized_start=28475
+  _WORLDEDGEDIRECTION._serialized_end=28571
+  _USERROLETYPE._serialized_start=28574
+  _USERROLETYPE._serialized_end=28733
+  _MANAGENODECMD._serialized_start=28735
+  _MANAGENODECMD._serialized_end=28806
+  _WORLDQUERYCMD._serialized_start=28809
+  _WORLDQUERYCMD._serialized_end=29041
+  _TRANSFORMNODETYPE._serialized_start=29044
+  _TRANSFORMNODETYPE._serialized_end=29302
+  _SPIKESORTERPARAMCOMMAND._serialized_start=29305
+  _SPIKESORTERPARAMCOMMAND._serialized_end=29528
+  _STATUSPOLLFIELDS._serialized_start=29531
+  _STATUSPOLLFIELDS._serialized_end=30025
+  _DASHBOARDTYPE._serialized_start=30027
+  _DASHBOARDTYPE._serialized_end=30054
+  _DASHBOARDCOMMAND._serialized_start=30056
+  _DASHBOARDCOMMAND._serialized_end=30134
   _OFFLINELICENSESTATUS._serialized_start=57
   _OFFLINELICENSESTATUS._serialized_end=121
   _FIRMWAREVERSION._serialized_start=123
   _FIRMWAREVERSION._serialized_end=190
   _RADIXENVIRONMENT._serialized_start=192
   _RADIXENVIRONMENT._serialized_end=299
   _STANDARDREQUEST._serialized_start=301
@@ -167,351 +167,351 @@
   _HDSNAPSHOTMETA._serialized_start=3570
   _HDSNAPSHOTMETA._serialized_end=3663
   _HDSNAPSHOT._serialized_start=3666
   _HDSNAPSHOT._serialized_end=3953
   _HDSNAPSHOT2._serialized_start=3955
   _HDSNAPSHOT2._serialized_end=4019
   _GETSIGNALSREQUEST._serialized_start=4022
-  _GETSIGNALSREQUEST._serialized_end=4463
+  _GETSIGNALSREQUEST._serialized_end=4483
   _GETSIGNALSREQUEST_GETSIGSPARAMS._serialized_start=4124
-  _GETSIGNALSREQUEST_GETSIGSPARAMS._serialized_end=4463
-  _RAWSIGNALS._serialized_start=4465
-  _RAWSIGNALS._serialized_end=4556
-  _SIGNALS2._serialized_start=4559
-  _SIGNALS2._serialized_end=4790
-  _LISTSENSORSPECSREPLY._serialized_start=4793
-  _LISTSENSORSPECSREPLY._serialized_end=5054
-  _LISTSENSORSPECSREPLY_SPECWITHCHANNELCOUNT._serialized_start=4996
-  _LISTSENSORSPECSREPLY_SPECWITHCHANNELCOUNT._serialized_end=5054
-  _LISTDATASOURCESREQUEST._serialized_start=5056
-  _LISTDATASOURCESREQUEST._serialized_end=5156
-  _SORTMAP._serialized_start=5158
-  _SORTMAP._serialized_end=5186
-  _GETSIGNALGROUPIDSREPLY._serialized_start=5188
-  _GETSIGNALGROUPIDSREPLY._serialized_end=5250
-  _GETSORTERIDMAPREPLY._serialized_start=5253
-  _GETSORTERIDMAPREPLY._serialized_end=5413
-  _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._serialized_start=5345
-  _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._serialized_end=5413
-  _DATASOURCE._serialized_start=5416
-  _DATASOURCE._serialized_end=5591
-  _FILEDESCRIPTOR._serialized_start=5593
-  _FILEDESCRIPTOR._serialized_end=5704
-  _TIMESPEC._serialized_start=5707
-  _TIMESPEC._serialized_end=5915
-  _TIMESPEC_TIMERANGEL._serialized_start=5829
-  _TIMESPEC_TIMERANGEL._serialized_end=5860
-  _TIMESPEC_TIMESTAMPRANGEL._serialized_start=5862
-  _TIMESPEC_TIMESTAMPRANGEL._serialized_end=5903
-  _SIGNALSPEC._serialized_start=5918
-  _SIGNALSPEC._serialized_end=6108
-  _SIGNALSPEC_SITENUML._serialized_start=6034
-  _SIGNALSPEC_SITENUML._serialized_end=6061
-  _SIGNALSPEC_NTVCHANIDXL._serialized_start=6063
-  _SIGNALSPEC_NTVCHANIDXL._serialized_end=6096
-  _CHANNELRECORD._serialized_start=6111
-  _CHANNELRECORD._serialized_end=6891
-  _XYCOORD._serialized_start=6893
-  _XYCOORD._serialized_end=6924
-  _XYZCOORD._serialized_start=6926
-  _XYZCOORD._serialized_end=6969
-  _SENSOR._serialized_start=6972
-  _SENSOR._serialized_end=7357
-  _SENSOR_WIREFRAME._serialized_start=7248
-  _SENSOR_WIREFRAME._serialized_end=7357
-  _SENSORPORTSPEC._serialized_start=7360
-  _SENSORPORTSPEC._serialized_end=7640
-  _SIGNALGROUPUNITS._serialized_start=7642
-  _SIGNALGROUPUNITS._serialized_end=7758
-  _SIGNALGROUPUNITS_UNITSENTRY._serialized_start=7714
-  _SIGNALGROUPUNITS_UNITSENTRY._serialized_end=7758
-  _SIGNALGROUP._serialized_start=7761
-  _SIGNALGROUP._serialized_end=8017
-  _CREATESIGNALGROUPREQUEST._serialized_start=8020
-  _CREATESIGNALGROUPREQUEST._serialized_end=8155
-  _SUBOPSORT._serialized_start=8157
-  _SUBOPSORT._serialized_end=8272
-  _SUBOPSORT_SORTFIELD._serialized_start=8213
-  _SUBOPSORT_SORTFIELD._serialized_end=8272
-  _UPDATESIGNALGROUPREQUEST._serialized_start=8275
-  _UPDATESIGNALGROUPREQUEST._serialized_end=8696
-  _UPDATESIGNALGROUPREQUEST_OPERATION._serialized_start=8577
-  _UPDATESIGNALGROUPREQUEST_OPERATION._serialized_end=8643
-  _UPDATESIGNALGROUPREQUEST_SUBOPERATION._serialized_start=8645
-  _UPDATESIGNALGROUPREQUEST_SUBOPERATION._serialized_end=8680
-  _SLICESIGNALGROUPSPEC._serialized_start=8698
-  _SLICESIGNALGROUPSPEC._serialized_end=8782
-  _SLICESIGNALGROUPREQUEST._serialized_start=8784
-  _SLICESIGNALGROUPREQUEST._serialized_end=8872
-  _SLICESIGNALGROUPREPLY._serialized_start=8875
-  _SLICESIGNALGROUPREPLY._serialized_end=9011
-  _LICENSESTATUS._serialized_start=9013
-  _LICENSESTATUS._serialized_end=9028
-  _SETDSPGROUPREQUEST._serialized_start=9030
-  _SETDSPGROUPREQUEST._serialized_end=9147
-  _DSPPARAMS._serialized_start=9150
-  _DSPPARAMS._serialized_end=9520
-  _DSPPARAMS_FREQSPECBAND._serialized_start=9459
-  _DSPPARAMS_FREQSPECBAND._serialized_end=9508
-  _DSPGROUP._serialized_start=9523
-  _DSPGROUP._serialized_end=9656
-  _SETSENSORREQUEST._serialized_start=9659
-  _SETSENSORREQUEST._serialized_end=9813
-  _SENSORPOSITIONTCS._serialized_start=9815
-  _SENSORPOSITIONTCS._serialized_end=9924
-  _SETSENSORPOSITIONTCSREQUEST._serialized_start=9927
-  _SETSENSORPOSITIONTCSREQUEST._serialized_end=10071
-  _SITEPOSITIONTCS._serialized_start=10073
-  _SITEPOSITIONTCS._serialized_end=10143
-  _SETSITEPOSITIONSTCSREQUEST._serialized_start=10145
-  _SETSITEPOSITIONSTCSREQUEST._serialized_end=10272
-  _FEATURESTARTSTOPREQUEST._serialized_start=10274
-  _FEATURESTARTSTOPREQUEST._serialized_end=10363
-  _PRIVACYREPLY._serialized_start=10365
-  _PRIVACYREPLY._serialized_end=10398
-  _SETPRIVACYREQUEST._serialized_start=10400
-  _SETPRIVACYREQUEST._serialized_end=10438
-  _DENSEMATRIX._serialized_start=10440
-  _DENSEMATRIX._serialized_end=10495
-  _HISTOGRAM._serialized_start=10497
-  _HISTOGRAM._serialized_end=10589
-  _KPIMETRICID._serialized_start=10591
-  _KPIMETRICID._serialized_end=10680
-  _TIMERANGE._serialized_start=10683
-  _TIMERANGE._serialized_end=10816
-  _BUNDLEREQ._serialized_start=10818
-  _BUNDLEREQ._serialized_end=10931
-  _KPIMETRICSREQ._serialized_start=10934
-  _KPIMETRICSREQ._serialized_end=11091
-  _KPIMETRICSDATA._serialized_start=11094
-  _KPIMETRICSDATA._serialized_end=11481
-  _KPIMETRICSDATA_METRICSTATS._serialized_start=11416
-  _KPIMETRICSDATA_METRICSTATS._serialized_end=11481
-  _KPIBUNDLEPACKETMETRICS._serialized_start=11483
-  _KPIBUNDLEPACKETMETRICS._serialized_end=11602
-  _KPIMETRICS._serialized_start=11604
-  _KPIMETRICS._serialized_end=11687
-  _KPICONTROLREQUEST._serialized_start=11689
-  _KPICONTROLREQUEST._serialized_end=11788
-  _SETKPIPARAMREQUEST._serialized_start=11790
-  _SETKPIPARAMREQUEST._serialized_end=11848
-  _GETKPISTATUSREQUEST._serialized_start=11850
-  _GETKPISTATUSREQUEST._serialized_end=11894
-  _KPISTANDARDREQUEST._serialized_start=11896
-  _KPISTANDARDREQUEST._serialized_end=11971
-  _KPIFILESTATUS._serialized_start=11974
-  _KPIFILESTATUS._serialized_end=12160
-  _KPIFILESTATUS_STATE._serialized_start=12037
-  _KPIFILESTATUS_STATE._serialized_end=12160
-  _KPIFILESTATUS2._serialized_start=12163
-  _KPIFILESTATUS2._serialized_end=12746
-  _KPIFILESTATUS2_KPI_STATE._serialized_start=12246
-  _KPIFILESTATUS2_KPI_STATE._serialized_end=12479
-  _KPIFILESTATUS2_DATASOURCE_STATE._serialized_start=12481
-  _KPIFILESTATUS2_DATASOURCE_STATE._serialized_end=12594
-  _KPIFILESTATUS2_KPIDATASOURCESTATESPEC._serialized_start=12597
-  _KPIFILESTATUS2_KPIDATASOURCESTATESPEC._serialized_end=12746
-  _KPIFILEMETADATA._serialized_start=12749
-  _KPIFILEMETADATA._serialized_end=13002
-  _KPIFILEMETADATA_STATE._serialized_start=12817
-  _KPIFILEMETADATA_STATE._serialized_end=13002
-  _KPISTATUSREPLY._serialized_start=13005
-  _KPISTATUSREPLY._serialized_end=13344
-  _SIGKPIPARAMRECORD._serialized_start=13347
-  _SIGKPIPARAMRECORD._serialized_end=13705
-  _ANNOTATEBUNDLE._serialized_start=13707
-  _ANNOTATEBUNDLE._serialized_end=13781
-  _PROJECTMETADATA._serialized_start=13783
-  _PROJECTMETADATA._serialized_end=13876
-  _SENSOREXTENDEDMETADATA._serialized_start=13878
-  _SENSOREXTENDEDMETADATA._serialized_end=13929
-  _GONUMMATRIXLIST._serialized_start=13931
-  _GONUMMATRIXLIST._serialized_end=13968
-  _RADIXMATRIXLIST._serialized_start=13970
-  _RADIXMATRIXLIST._serialized_end=14024
-  _RADIXMATRIX._serialized_start=14026
-  _RADIXMATRIX._serialized_end=14068
-  _RADIXMATRIXBYTES._serialized_start=14070
-  _RADIXMATRIXBYTES._serialized_end=14117
-  _RADIXSIGNALSLIST._serialized_start=14119
-  _RADIXSIGNALSLIST._serialized_end=14175
-  _RADIXSIGNALS._serialized_start=14178
-  _RADIXSIGNALS._serialized_end=14347
-  _VECTORSTRING._serialized_start=14349
-  _VECTORSTRING._serialized_end=14374
-  _VECTORFLOAT64._serialized_start=14376
-  _VECTORFLOAT64._serialized_end=14402
-  _VECTORSLICEFLOAT64._serialized_start=14404
-  _VECTORSLICEFLOAT64._serialized_end=14475
-  _LOGSYSKPISTATUSREPLY._serialized_start=14478
-  _LOGSYSKPISTATUSREPLY._serialized_end=14828
-  _KPICACHE._serialized_start=14831
-  _KPICACHE._serialized_end=15211
-  _LOGSYSKPITAILREPLY._serialized_start=15214
-  _LOGSYSKPITAILREPLY._serialized_end=15592
-  _KPIPORTINFO._serialized_start=15594
-  _KPIPORTINFO._serialized_end=15645
-  _KPITAILROWS._serialized_start=15648
-  _KPITAILROWS._serialized_end=16020
-  _WAREHOUSEHEALTHCHECKSPEC._serialized_start=16022
-  _WAREHOUSEHEALTHCHECKSPEC._serialized_end=16064
-  _OUTFITTERGETDEVICEREQUEST._serialized_start=16066
-  _OUTFITTERGETDEVICEREQUEST._serialized_end=16106
-  _SENSORCOMPREQUEST._serialized_start=16109
-  _SENSORCOMPREQUEST._serialized_end=16267
-  _REGISTERSENSORCOMPREQUEST._serialized_start=16269
-  _REGISTERSENSORCOMPREQUEST._serialized_end=16391
-  _SAVESENSORCOMPINSTANCEREQUEST._serialized_start=16394
-  _SAVESENSORCOMPINSTANCEREQUEST._serialized_end=16540
-  _PROBEDESC._serialized_start=16542
-  _PROBEDESC._serialized_end=16580
-  _HEADSTAGEDESC._serialized_start=16582
-  _HEADSTAGEDESC._serialized_end=16624
-  _GETSENSORCOMPREPLY._serialized_start=16626
-  _GETSENSORCOMPREPLY._serialized_end=16722
-  _PROBESPEC._serialized_start=16724
-  _PROBESPEC._serialized_end=16844
-  _HEADSTAGESPEC._serialized_start=16847
-  _HEADSTAGESPEC._serialized_end=16983
-  _PROBEMODEL._serialized_start=16986
-  _PROBEMODEL._serialized_end=17576
-  _PROBEMODEL_PROBESITEDESC._serialized_start=17223
-  _PROBEMODEL_PROBESITEDESC._serialized_end=17445
-  _PROBEMODEL_PROBEWIREFRAME._serialized_start=17447
-  _PROBEMODEL_PROBEWIREFRAME._serialized_end=17541
-  _PROBEMODEL_PROBEPTXY._serialized_start=17543
-  _PROBEMODEL_PROBEPTXY._serialized_end=17576
-  _PROBEMETADATA._serialized_start=17578
-  _PROBEMETADATA._serialized_end=17673
-  _HEADSTAGEMODEL._serialized_start=17676
-  _HEADSTAGEMODEL._serialized_end=17808
-  _HEADSTAGEMODEL_HEADSTAGEROW._serialized_start=17757
-  _HEADSTAGEMODEL_HEADSTAGEROW._serialized_end=17808
-  _HEADSTAGEMETADATA._serialized_start=17810
-  _HEADSTAGEMETADATA._serialized_end=17829
-  _USERPROFILE._serialized_start=17831
-  _USERPROFILE._serialized_end=17884
-  _GETCURRENTPROFILEREPLY._serialized_start=17886
-  _GETCURRENTPROFILEREPLY._serialized_end=17952
-  _GETALLPROFILESREPLY._serialized_start=17954
-  _GETALLPROFILESREPLY._serialized_end=18018
-  _SETCURRENTPROFILEREQUEST._serialized_start=18020
-  _SETCURRENTPROFILEREQUEST._serialized_end=18065
-  _MANAGENODEORGPAYLOAD._serialized_start=18068
-  _MANAGENODEORGPAYLOAD._serialized_end=18204
-  _MANAGENODEORGREQUEST._serialized_start=18206
-  _MANAGENODEORGREQUEST._serialized_end=18311
-  _MANAGENODEORGREPLY._serialized_start=18313
-  _MANAGENODEORGREPLY._serialized_end=18396
-  _MANAGENODELABPAYLOAD._serialized_start=18399
-  _MANAGENODELABPAYLOAD._serialized_end=18561
-  _MANAGENODELABREQUEST._serialized_start=18563
-  _MANAGENODELABREQUEST._serialized_end=18668
-  _MANAGENODELABREPLY._serialized_start=18670
-  _MANAGENODELABREPLY._serialized_end=18753
-  _MANAGENODEUSERPAYLOAD._serialized_start=18756
-  _MANAGENODEUSERPAYLOAD._serialized_end=18909
-  _MANAGENODEUSERREQUEST._serialized_start=18911
-  _MANAGENODEUSERREQUEST._serialized_end=19018
-  _MANAGENODEUSERREPLY._serialized_start=19020
-  _MANAGENODEUSERREPLY._serialized_end=19105
-  _CATALOGPROBEPAYLOAD._serialized_start=19107
-  _CATALOGPROBEPAYLOAD._serialized_end=19161
-  _PROBENODEREQUEST._serialized_start=19163
-  _PROBENODEREQUEST._serialized_end=19256
-  _PROBENODEREPLY._serialized_start=19258
-  _PROBENODEREPLY._serialized_end=19313
-  _PROBEPAYLOAD._serialized_start=19315
-  _PROBEPAYLOAD._serialized_end=19362
-  _EDGEPAYLOAD._serialized_start=19365
-  _EDGEPAYLOAD._serialized_end=19658
-  _EDGEPAYLOAD_GENERICNODE._serialized_start=19568
-  _EDGEPAYLOAD_GENERICNODE._serialized_end=19658
-  _WORLDEDGEREQUEST._serialized_start=19660
-  _WORLDEDGEREQUEST._serialized_end=19716
-  _WORLDEDGEREPLY._serialized_start=19718
-  _WORLDEDGEREPLY._serialized_end=19734
-  _QUERYWORLDREQUEST._serialized_start=19736
-  _QUERYWORLDREQUEST._serialized_end=19805
-  _QUERYWORLDREC._serialized_start=19808
-  _QUERYWORLDREC._serialized_end=20038
-  _QUERYWORLDREPLY._serialized_start=20040
-  _QUERYWORLDREPLY._serialized_end=20097
-  _HIGHLOWPASSTRANSFORMPARAMS._serialized_start=20099
-  _HIGHLOWPASSTRANSFORMPARAMS._serialized_end=20146
-  _BANDTRANSFORMPARAMS._serialized_start=20148
-  _BANDTRANSFORMPARAMS._serialized_end=20214
-  _NOTCHTRANSFORMPARAMS._serialized_start=20216
-  _NOTCHTRANSFORMPARAMS._serialized_end=20286
-  _CARTRANSFORMPARAMS._serialized_start=20288
-  _CARTRANSFORMPARAMS._serialized_end=20308
-  _VIRTUALREFTRANSFORMPARAMS._serialized_start=20310
-  _VIRTUALREFTRANSFORMPARAMS._serialized_end=20360
-  _PAIREDREFTRANSFORMPARAMS._serialized_start=20362
-  _PAIREDREFTRANSFORMPARAMS._serialized_end=20437
-  _DATASOURCESINKTRANSFORMPARAMS._serialized_start=20439
-  _DATASOURCESINKTRANSFORMPARAMS._serialized_end=20544
-  _SLICETIMETRANSFORMPARAMS._serialized_start=20546
-  _SLICETIMETRANSFORMPARAMS._serialized_end=20608
-  _SLICECHANNELSTRANSFORMPARAMS._serialized_start=20610
-  _SLICECHANNELSTRANSFORMPARAMS._serialized_end=20720
-  _DOWNSAMPLETRANSFORMPARAMS._serialized_start=20722
-  _DOWNSAMPLETRANSFORMPARAMS._serialized_end=20771
-  _REMAPSENSORTRANSFORMPARAMS._serialized_start=20774
-  _REMAPSENSORTRANSFORMPARAMS._serialized_end=21010
-  _REMAPSENSORTRANSFORMPARAMS_SENSORSPEC._serialized_start=20885
-  _REMAPSENSORTRANSFORMPARAMS_SENSORSPEC._serialized_end=21010
-  _POSITION._serialized_start=21012
-  _POSITION._serialized_end=21044
-  _TRANSFORMNODE._serialized_start=21047
-  _TRANSFORMNODE._serialized_end=21839
-  _TRANSFORMEDGE._serialized_start=21841
-  _TRANSFORMEDGE._serialized_end=21900
-  _PROTOCOL._serialized_start=21902
-  _PROTOCOL._serialized_end=22018
-  _PROTOCOLREQUEST._serialized_start=22020
-  _PROTOCOLREQUEST._serialized_end=22057
-  _RENAMEPROTOCOLREQUEST._serialized_start=22059
-  _RENAMEPROTOCOLREQUEST._serialized_end=22125
-  _GETALLPROTOCOLSREPLY._serialized_start=22127
-  _GETALLPROTOCOLSREPLY._serialized_end=22186
-  _APPLYPROTOCOLPROGRESS._serialized_start=22188
-  _APPLYPROTOCOLPROGRESS._serialized_end=22311
-  _SPIKESORTERSETPARAMREQUEST._serialized_start=22314
-  _SPIKESORTERSETPARAMREQUEST._serialized_end=22468
-  _SPIKESORTERSETPARAMSREQUEST._serialized_start=22470
-  _SPIKESORTERSETPARAMSREQUEST._serialized_end=22551
-  _SPIKESORTERPARAMCOMMANDRECORD._serialized_start=22554
-  _SPIKESORTERPARAMCOMMANDRECORD._serialized_end=22849
-  _KPIPARAMS._serialized_start=22851
-  _KPIPARAMS._serialized_end=22914
-  _DACSTREAMREQUEST._serialized_start=22916
-  _DACSTREAMREQUEST._serialized_end=22990
-  _EVENTVIEWERCONFIG._serialized_start=22993
-  _EVENTVIEWERCONFIG._serialized_end=23215
-  _EVENTVIEWERID._serialized_start=23217
-  _EVENTVIEWERID._serialized_end=23278
-  _GETEVENTVIEWEREVENTREQUEST._serialized_start=23280
-  _GETEVENTVIEWEREVENTREQUEST._serialized_end=23348
-  _EVENTVIEWEREVENTDESC._serialized_start=23350
-  _EVENTVIEWEREVENTDESC._serialized_end=23439
-  _EVENTVIEWEREVENT._serialized_start=23442
-  _EVENTVIEWEREVENT._serialized_end=23585
-  _LISTEVENTVIEWEREVENTSREPLY._serialized_start=23587
-  _LISTEVENTVIEWEREVENTSREPLY._serialized_end=23684
-  _LISTEVENTVIEWERSREPLY._serialized_start=23686
-  _LISTEVENTVIEWERSREPLY._serialized_end=23754
-  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_start=23756
-  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_end=23807
-  _STATUSPOLLFIELDSTOUPDATE._serialized_start=23809
-  _STATUSPOLLFIELDSTOUPDATE._serialized_end=23903
-  _DASHBOARDCOMMANDREQUEST._serialized_start=23906
-  _DASHBOARDCOMMANDREQUEST._serialized_end=24071
-  _DASHBOARDCOMMANDREQUEST_ARGS._serialized_start=24026
-  _DASHBOARDCOMMANDREQUEST_ARGS._serialized_end=24071
-  _SELTABLESIGNALGROUP._serialized_start=24073
-  _SELTABLESIGNALGROUP._serialized_end=24166
-  _SELECTORTABLESREPLY._serialized_start=24168
-  _SELECTORTABLESREPLY._serialized_end=24231
-  _DATASOURCESTATUS._serialized_start=24234
-  _DATASOURCESTATUS._serialized_end=24612
+  _GETSIGNALSREQUEST_GETSIGSPARAMS._serialized_end=4483
+  _RAWSIGNALS._serialized_start=4485
+  _RAWSIGNALS._serialized_end=4576
+  _SIGNALS2._serialized_start=4579
+  _SIGNALS2._serialized_end=4810
+  _LISTSENSORSPECSREPLY._serialized_start=4813
+  _LISTSENSORSPECSREPLY._serialized_end=5074
+  _LISTSENSORSPECSREPLY_SPECWITHCHANNELCOUNT._serialized_start=5016
+  _LISTSENSORSPECSREPLY_SPECWITHCHANNELCOUNT._serialized_end=5074
+  _LISTDATASOURCESREQUEST._serialized_start=5076
+  _LISTDATASOURCESREQUEST._serialized_end=5176
+  _SORTMAP._serialized_start=5178
+  _SORTMAP._serialized_end=5206
+  _GETSIGNALGROUPIDSREPLY._serialized_start=5208
+  _GETSIGNALGROUPIDSREPLY._serialized_end=5270
+  _GETSORTERIDMAPREPLY._serialized_start=5273
+  _GETSORTERIDMAPREPLY._serialized_end=5433
+  _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._serialized_start=5365
+  _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._serialized_end=5433
+  _DATASOURCE._serialized_start=5436
+  _DATASOURCE._serialized_end=5611
+  _FILEDESCRIPTOR._serialized_start=5613
+  _FILEDESCRIPTOR._serialized_end=5724
+  _TIMESPEC._serialized_start=5727
+  _TIMESPEC._serialized_end=5935
+  _TIMESPEC_TIMERANGEL._serialized_start=5849
+  _TIMESPEC_TIMERANGEL._serialized_end=5880
+  _TIMESPEC_TIMESTAMPRANGEL._serialized_start=5882
+  _TIMESPEC_TIMESTAMPRANGEL._serialized_end=5923
+  _SIGNALSPEC._serialized_start=5938
+  _SIGNALSPEC._serialized_end=6128
+  _SIGNALSPEC_SITENUML._serialized_start=6054
+  _SIGNALSPEC_SITENUML._serialized_end=6081
+  _SIGNALSPEC_NTVCHANIDXL._serialized_start=6083
+  _SIGNALSPEC_NTVCHANIDXL._serialized_end=6116
+  _CHANNELRECORD._serialized_start=6131
+  _CHANNELRECORD._serialized_end=6911
+  _XYCOORD._serialized_start=6913
+  _XYCOORD._serialized_end=6944
+  _XYZCOORD._serialized_start=6946
+  _XYZCOORD._serialized_end=6989
+  _SENSOR._serialized_start=6992
+  _SENSOR._serialized_end=7377
+  _SENSOR_WIREFRAME._serialized_start=7268
+  _SENSOR_WIREFRAME._serialized_end=7377
+  _SENSORPORTSPEC._serialized_start=7380
+  _SENSORPORTSPEC._serialized_end=7660
+  _SIGNALGROUPUNITS._serialized_start=7662
+  _SIGNALGROUPUNITS._serialized_end=7778
+  _SIGNALGROUPUNITS_UNITSENTRY._serialized_start=7734
+  _SIGNALGROUPUNITS_UNITSENTRY._serialized_end=7778
+  _SIGNALGROUP._serialized_start=7781
+  _SIGNALGROUP._serialized_end=8037
+  _CREATESIGNALGROUPREQUEST._serialized_start=8040
+  _CREATESIGNALGROUPREQUEST._serialized_end=8175
+  _SUBOPSORT._serialized_start=8177
+  _SUBOPSORT._serialized_end=8292
+  _SUBOPSORT_SORTFIELD._serialized_start=8233
+  _SUBOPSORT_SORTFIELD._serialized_end=8292
+  _UPDATESIGNALGROUPREQUEST._serialized_start=8295
+  _UPDATESIGNALGROUPREQUEST._serialized_end=8716
+  _UPDATESIGNALGROUPREQUEST_OPERATION._serialized_start=8597
+  _UPDATESIGNALGROUPREQUEST_OPERATION._serialized_end=8663
+  _UPDATESIGNALGROUPREQUEST_SUBOPERATION._serialized_start=8665
+  _UPDATESIGNALGROUPREQUEST_SUBOPERATION._serialized_end=8700
+  _SLICESIGNALGROUPSPEC._serialized_start=8718
+  _SLICESIGNALGROUPSPEC._serialized_end=8802
+  _SLICESIGNALGROUPREQUEST._serialized_start=8804
+  _SLICESIGNALGROUPREQUEST._serialized_end=8892
+  _SLICESIGNALGROUPREPLY._serialized_start=8895
+  _SLICESIGNALGROUPREPLY._serialized_end=9031
+  _LICENSESTATUS._serialized_start=9033
+  _LICENSESTATUS._serialized_end=9048
+  _SETDSPGROUPREQUEST._serialized_start=9050
+  _SETDSPGROUPREQUEST._serialized_end=9167
+  _DSPPARAMS._serialized_start=9170
+  _DSPPARAMS._serialized_end=9540
+  _DSPPARAMS_FREQSPECBAND._serialized_start=9479
+  _DSPPARAMS_FREQSPECBAND._serialized_end=9528
+  _DSPGROUP._serialized_start=9543
+  _DSPGROUP._serialized_end=9676
+  _SETSENSORREQUEST._serialized_start=9679
+  _SETSENSORREQUEST._serialized_end=9833
+  _SENSORPOSITIONTCS._serialized_start=9835
+  _SENSORPOSITIONTCS._serialized_end=9944
+  _SETSENSORPOSITIONTCSREQUEST._serialized_start=9947
+  _SETSENSORPOSITIONTCSREQUEST._serialized_end=10091
+  _SITEPOSITIONTCS._serialized_start=10093
+  _SITEPOSITIONTCS._serialized_end=10163
+  _SETSITEPOSITIONSTCSREQUEST._serialized_start=10165
+  _SETSITEPOSITIONSTCSREQUEST._serialized_end=10292
+  _FEATURESTARTSTOPREQUEST._serialized_start=10294
+  _FEATURESTARTSTOPREQUEST._serialized_end=10383
+  _PRIVACYREPLY._serialized_start=10385
+  _PRIVACYREPLY._serialized_end=10418
+  _SETPRIVACYREQUEST._serialized_start=10420
+  _SETPRIVACYREQUEST._serialized_end=10458
+  _DENSEMATRIX._serialized_start=10460
+  _DENSEMATRIX._serialized_end=10515
+  _HISTOGRAM._serialized_start=10517
+  _HISTOGRAM._serialized_end=10609
+  _KPIMETRICID._serialized_start=10611
+  _KPIMETRICID._serialized_end=10700
+  _TIMERANGE._serialized_start=10703
+  _TIMERANGE._serialized_end=10836
+  _BUNDLEREQ._serialized_start=10838
+  _BUNDLEREQ._serialized_end=10951
+  _KPIMETRICSREQ._serialized_start=10954
+  _KPIMETRICSREQ._serialized_end=11111
+  _KPIMETRICSDATA._serialized_start=11114
+  _KPIMETRICSDATA._serialized_end=11501
+  _KPIMETRICSDATA_METRICSTATS._serialized_start=11436
+  _KPIMETRICSDATA_METRICSTATS._serialized_end=11501
+  _KPIBUNDLEPACKETMETRICS._serialized_start=11503
+  _KPIBUNDLEPACKETMETRICS._serialized_end=11622
+  _KPIMETRICS._serialized_start=11624
+  _KPIMETRICS._serialized_end=11707
+  _KPICONTROLREQUEST._serialized_start=11709
+  _KPICONTROLREQUEST._serialized_end=11808
+  _SETKPIPARAMREQUEST._serialized_start=11810
+  _SETKPIPARAMREQUEST._serialized_end=11868
+  _GETKPISTATUSREQUEST._serialized_start=11870
+  _GETKPISTATUSREQUEST._serialized_end=11914
+  _KPISTANDARDREQUEST._serialized_start=11916
+  _KPISTANDARDREQUEST._serialized_end=11991
+  _KPIFILESTATUS._serialized_start=11994
+  _KPIFILESTATUS._serialized_end=12180
+  _KPIFILESTATUS_STATE._serialized_start=12057
+  _KPIFILESTATUS_STATE._serialized_end=12180
+  _KPIFILESTATUS2._serialized_start=12183
+  _KPIFILESTATUS2._serialized_end=12766
+  _KPIFILESTATUS2_KPI_STATE._serialized_start=12266
+  _KPIFILESTATUS2_KPI_STATE._serialized_end=12499
+  _KPIFILESTATUS2_DATASOURCE_STATE._serialized_start=12501
+  _KPIFILESTATUS2_DATASOURCE_STATE._serialized_end=12614
+  _KPIFILESTATUS2_KPIDATASOURCESTATESPEC._serialized_start=12617
+  _KPIFILESTATUS2_KPIDATASOURCESTATESPEC._serialized_end=12766
+  _KPIFILEMETADATA._serialized_start=12769
+  _KPIFILEMETADATA._serialized_end=13022
+  _KPIFILEMETADATA_STATE._serialized_start=12837
+  _KPIFILEMETADATA_STATE._serialized_end=13022
+  _KPISTATUSREPLY._serialized_start=13025
+  _KPISTATUSREPLY._serialized_end=13364
+  _SIGKPIPARAMRECORD._serialized_start=13367
+  _SIGKPIPARAMRECORD._serialized_end=13725
+  _ANNOTATEBUNDLE._serialized_start=13727
+  _ANNOTATEBUNDLE._serialized_end=13801
+  _PROJECTMETADATA._serialized_start=13803
+  _PROJECTMETADATA._serialized_end=13896
+  _SENSOREXTENDEDMETADATA._serialized_start=13898
+  _SENSOREXTENDEDMETADATA._serialized_end=13949
+  _GONUMMATRIXLIST._serialized_start=13951
+  _GONUMMATRIXLIST._serialized_end=13988
+  _RADIXMATRIXLIST._serialized_start=13990
+  _RADIXMATRIXLIST._serialized_end=14044
+  _RADIXMATRIX._serialized_start=14046
+  _RADIXMATRIX._serialized_end=14088
+  _RADIXMATRIXBYTES._serialized_start=14090
+  _RADIXMATRIXBYTES._serialized_end=14137
+  _RADIXSIGNALSLIST._serialized_start=14139
+  _RADIXSIGNALSLIST._serialized_end=14195
+  _RADIXSIGNALS._serialized_start=14198
+  _RADIXSIGNALS._serialized_end=14367
+  _VECTORSTRING._serialized_start=14369
+  _VECTORSTRING._serialized_end=14394
+  _VECTORFLOAT64._serialized_start=14396
+  _VECTORFLOAT64._serialized_end=14422
+  _VECTORSLICEFLOAT64._serialized_start=14424
+  _VECTORSLICEFLOAT64._serialized_end=14495
+  _LOGSYSKPISTATUSREPLY._serialized_start=14498
+  _LOGSYSKPISTATUSREPLY._serialized_end=14848
+  _KPICACHE._serialized_start=14851
+  _KPICACHE._serialized_end=15231
+  _LOGSYSKPITAILREPLY._serialized_start=15234
+  _LOGSYSKPITAILREPLY._serialized_end=15612
+  _KPIPORTINFO._serialized_start=15614
+  _KPIPORTINFO._serialized_end=15665
+  _KPITAILROWS._serialized_start=15668
+  _KPITAILROWS._serialized_end=16040
+  _WAREHOUSEHEALTHCHECKSPEC._serialized_start=16042
+  _WAREHOUSEHEALTHCHECKSPEC._serialized_end=16084
+  _OUTFITTERGETDEVICEREQUEST._serialized_start=16086
+  _OUTFITTERGETDEVICEREQUEST._serialized_end=16126
+  _SENSORCOMPREQUEST._serialized_start=16129
+  _SENSORCOMPREQUEST._serialized_end=16287
+  _REGISTERSENSORCOMPREQUEST._serialized_start=16289
+  _REGISTERSENSORCOMPREQUEST._serialized_end=16411
+  _SAVESENSORCOMPINSTANCEREQUEST._serialized_start=16414
+  _SAVESENSORCOMPINSTANCEREQUEST._serialized_end=16560
+  _PROBEDESC._serialized_start=16562
+  _PROBEDESC._serialized_end=16600
+  _HEADSTAGEDESC._serialized_start=16602
+  _HEADSTAGEDESC._serialized_end=16644
+  _GETSENSORCOMPREPLY._serialized_start=16646
+  _GETSENSORCOMPREPLY._serialized_end=16742
+  _PROBESPEC._serialized_start=16744
+  _PROBESPEC._serialized_end=16864
+  _HEADSTAGESPEC._serialized_start=16867
+  _HEADSTAGESPEC._serialized_end=17003
+  _PROBEMODEL._serialized_start=17006
+  _PROBEMODEL._serialized_end=17596
+  _PROBEMODEL_PROBESITEDESC._serialized_start=17243
+  _PROBEMODEL_PROBESITEDESC._serialized_end=17465
+  _PROBEMODEL_PROBEWIREFRAME._serialized_start=17467
+  _PROBEMODEL_PROBEWIREFRAME._serialized_end=17561
+  _PROBEMODEL_PROBEPTXY._serialized_start=17563
+  _PROBEMODEL_PROBEPTXY._serialized_end=17596
+  _PROBEMETADATA._serialized_start=17598
+  _PROBEMETADATA._serialized_end=17693
+  _HEADSTAGEMODEL._serialized_start=17696
+  _HEADSTAGEMODEL._serialized_end=17828
+  _HEADSTAGEMODEL_HEADSTAGEROW._serialized_start=17777
+  _HEADSTAGEMODEL_HEADSTAGEROW._serialized_end=17828
+  _HEADSTAGEMETADATA._serialized_start=17830
+  _HEADSTAGEMETADATA._serialized_end=17849
+  _USERPROFILE._serialized_start=17851
+  _USERPROFILE._serialized_end=17904
+  _GETCURRENTPROFILEREPLY._serialized_start=17906
+  _GETCURRENTPROFILEREPLY._serialized_end=17972
+  _GETALLPROFILESREPLY._serialized_start=17974
+  _GETALLPROFILESREPLY._serialized_end=18038
+  _SETCURRENTPROFILEREQUEST._serialized_start=18040
+  _SETCURRENTPROFILEREQUEST._serialized_end=18085
+  _MANAGENODEORGPAYLOAD._serialized_start=18088
+  _MANAGENODEORGPAYLOAD._serialized_end=18224
+  _MANAGENODEORGREQUEST._serialized_start=18226
+  _MANAGENODEORGREQUEST._serialized_end=18331
+  _MANAGENODEORGREPLY._serialized_start=18333
+  _MANAGENODEORGREPLY._serialized_end=18416
+  _MANAGENODELABPAYLOAD._serialized_start=18419
+  _MANAGENODELABPAYLOAD._serialized_end=18581
+  _MANAGENODELABREQUEST._serialized_start=18583
+  _MANAGENODELABREQUEST._serialized_end=18688
+  _MANAGENODELABREPLY._serialized_start=18690
+  _MANAGENODELABREPLY._serialized_end=18773
+  _MANAGENODEUSERPAYLOAD._serialized_start=18776
+  _MANAGENODEUSERPAYLOAD._serialized_end=18929
+  _MANAGENODEUSERREQUEST._serialized_start=18931
+  _MANAGENODEUSERREQUEST._serialized_end=19038
+  _MANAGENODEUSERREPLY._serialized_start=19040
+  _MANAGENODEUSERREPLY._serialized_end=19125
+  _CATALOGPROBEPAYLOAD._serialized_start=19127
+  _CATALOGPROBEPAYLOAD._serialized_end=19181
+  _PROBENODEREQUEST._serialized_start=19183
+  _PROBENODEREQUEST._serialized_end=19276
+  _PROBENODEREPLY._serialized_start=19278
+  _PROBENODEREPLY._serialized_end=19333
+  _PROBEPAYLOAD._serialized_start=19335
+  _PROBEPAYLOAD._serialized_end=19382
+  _EDGEPAYLOAD._serialized_start=19385
+  _EDGEPAYLOAD._serialized_end=19678
+  _EDGEPAYLOAD_GENERICNODE._serialized_start=19588
+  _EDGEPAYLOAD_GENERICNODE._serialized_end=19678
+  _WORLDEDGEREQUEST._serialized_start=19680
+  _WORLDEDGEREQUEST._serialized_end=19736
+  _WORLDEDGEREPLY._serialized_start=19738
+  _WORLDEDGEREPLY._serialized_end=19754
+  _QUERYWORLDREQUEST._serialized_start=19756
+  _QUERYWORLDREQUEST._serialized_end=19825
+  _QUERYWORLDREC._serialized_start=19828
+  _QUERYWORLDREC._serialized_end=20058
+  _QUERYWORLDREPLY._serialized_start=20060
+  _QUERYWORLDREPLY._serialized_end=20117
+  _HIGHLOWPASSTRANSFORMPARAMS._serialized_start=20119
+  _HIGHLOWPASSTRANSFORMPARAMS._serialized_end=20166
+  _BANDTRANSFORMPARAMS._serialized_start=20168
+  _BANDTRANSFORMPARAMS._serialized_end=20234
+  _NOTCHTRANSFORMPARAMS._serialized_start=20236
+  _NOTCHTRANSFORMPARAMS._serialized_end=20306
+  _CARTRANSFORMPARAMS._serialized_start=20308
+  _CARTRANSFORMPARAMS._serialized_end=20328
+  _VIRTUALREFTRANSFORMPARAMS._serialized_start=20330
+  _VIRTUALREFTRANSFORMPARAMS._serialized_end=20380
+  _PAIREDREFTRANSFORMPARAMS._serialized_start=20382
+  _PAIREDREFTRANSFORMPARAMS._serialized_end=20457
+  _DATASOURCESINKTRANSFORMPARAMS._serialized_start=20459
+  _DATASOURCESINKTRANSFORMPARAMS._serialized_end=20564
+  _SLICETIMETRANSFORMPARAMS._serialized_start=20566
+  _SLICETIMETRANSFORMPARAMS._serialized_end=20628
+  _SLICECHANNELSTRANSFORMPARAMS._serialized_start=20630
+  _SLICECHANNELSTRANSFORMPARAMS._serialized_end=20740
+  _DOWNSAMPLETRANSFORMPARAMS._serialized_start=20742
+  _DOWNSAMPLETRANSFORMPARAMS._serialized_end=20791
+  _REMAPSENSORTRANSFORMPARAMS._serialized_start=20794
+  _REMAPSENSORTRANSFORMPARAMS._serialized_end=21030
+  _REMAPSENSORTRANSFORMPARAMS_SENSORSPEC._serialized_start=20905
+  _REMAPSENSORTRANSFORMPARAMS_SENSORSPEC._serialized_end=21030
+  _POSITION._serialized_start=21032
+  _POSITION._serialized_end=21064
+  _TRANSFORMNODE._serialized_start=21067
+  _TRANSFORMNODE._serialized_end=21859
+  _TRANSFORMEDGE._serialized_start=21861
+  _TRANSFORMEDGE._serialized_end=21920
+  _PROTOCOL._serialized_start=21922
+  _PROTOCOL._serialized_end=22038
+  _PROTOCOLREQUEST._serialized_start=22040
+  _PROTOCOLREQUEST._serialized_end=22077
+  _RENAMEPROTOCOLREQUEST._serialized_start=22079
+  _RENAMEPROTOCOLREQUEST._serialized_end=22145
+  _GETALLPROTOCOLSREPLY._serialized_start=22147
+  _GETALLPROTOCOLSREPLY._serialized_end=22206
+  _APPLYPROTOCOLPROGRESS._serialized_start=22208
+  _APPLYPROTOCOLPROGRESS._serialized_end=22331
+  _SPIKESORTERSETPARAMREQUEST._serialized_start=22334
+  _SPIKESORTERSETPARAMREQUEST._serialized_end=22488
+  _SPIKESORTERSETPARAMSREQUEST._serialized_start=22490
+  _SPIKESORTERSETPARAMSREQUEST._serialized_end=22571
+  _SPIKESORTERPARAMCOMMANDRECORD._serialized_start=22574
+  _SPIKESORTERPARAMCOMMANDRECORD._serialized_end=22869
+  _KPIPARAMS._serialized_start=22871
+  _KPIPARAMS._serialized_end=22934
+  _DACSTREAMREQUEST._serialized_start=22936
+  _DACSTREAMREQUEST._serialized_end=23010
+  _EVENTVIEWERCONFIG._serialized_start=23013
+  _EVENTVIEWERCONFIG._serialized_end=23235
+  _EVENTVIEWERID._serialized_start=23237
+  _EVENTVIEWERID._serialized_end=23298
+  _GETEVENTVIEWEREVENTREQUEST._serialized_start=23300
+  _GETEVENTVIEWEREVENTREQUEST._serialized_end=23368
+  _EVENTVIEWEREVENTDESC._serialized_start=23370
+  _EVENTVIEWEREVENTDESC._serialized_end=23459
+  _EVENTVIEWEREVENT._serialized_start=23462
+  _EVENTVIEWEREVENT._serialized_end=23605
+  _LISTEVENTVIEWEREVENTSREPLY._serialized_start=23607
+  _LISTEVENTVIEWEREVENTSREPLY._serialized_end=23704
+  _LISTEVENTVIEWERSREPLY._serialized_start=23706
+  _LISTEVENTVIEWERSREPLY._serialized_end=23774
+  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_start=23776
+  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_end=23827
+  _STATUSPOLLFIELDSTOUPDATE._serialized_start=23829
+  _STATUSPOLLFIELDSTOUPDATE._serialized_end=23923
+  _DASHBOARDCOMMANDREQUEST._serialized_start=23926
+  _DASHBOARDCOMMANDREQUEST._serialized_end=24091
+  _DASHBOARDCOMMANDREQUEST_ARGS._serialized_start=24046
+  _DASHBOARDCOMMANDREQUEST_ARGS._serialized_end=24091
+  _SELTABLESIGNALGROUP._serialized_start=24093
+  _SELTABLESIGNALGROUP._serialized_end=24186
+  _SELECTORTABLESREPLY._serialized_start=24188
+  _SELECTORTABLESREPLY._serialized_end=24251
+  _DATASOURCESTATUS._serialized_start=24254
+  _DATASOURCESTATUS._serialized_end=24632
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-3.0.0b5/radiens/grpc_radiens/datasource_pb2.py` & `radiens-3.0.0b6/radiens/grpc_radiens/datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/grpc_radiens/pybridge_pb2.py` & `radiens-3.0.0b6/radiens/grpc_radiens/pybridge_pb2.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/grpc_radiens/pybridge_pb2_grpc.py` & `radiens-3.0.0b6/radiens/grpc_radiens/pybridge_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/grpc_radiens/radiens_dev_pb2.py` & `radiens-3.0.0b6/radiens/grpc_radiens/radiens_dev_pb2.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/grpc_radiens/radiensserver_pb2.py` & `radiens-3.0.0b6/radiens/grpc_radiens/radiensserver_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from . import common_pb2 as common__pb2
 from . import datasource_pb2 as datasource__pb2
 from . import biointerface_pb2 as biointerface__pb2
 from . import spikesorter_pb2 as spikesorter__pb2
 from . import radiens_dev_pb2 as radiens__dev__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13radiensserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\x1a\x11radiens_dev.proto\"K\n\x19RadiensHealthcheckRequest\x12\x1a\n\x12isIncludeWarehouse\x18\x01 \x01(\x08\x12\x12\n\nisDetailed\x18\x02 \x01(\x08\"]\n\x16RadiensHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\x12\x33\n\toutfitter\x18\x02 \x01(\x0b\x32 .allego.WarehouseHealthcheckSpec\"\x1e\n\x0fRadiensClientId\x12\x0b\n\x03pid\x18\x01 \x02(\x05\"\x91\x01\n\x12SummaSessionsReply\x12?\n\x07session\x18\x01 \x03(\x0b\x32..allego.SummaSessionsReply.SummaCurrentSession\x1a:\n\x13SummaCurrentSession\x12\x0f\n\x07summaID\x18\x01 \x02(\t\x12\x12\n\ndsourceIDs\x18\x02 \x03(\t\"_\n\x14SummaAnalysisRequest\x12\x0f\n\x07summaID\x18\x01 \x01(\t\x12\x12\n\ndsourceIDs\x18\x02 \x03(\t\x12\x11\n\tpktDurSec\x18\x03 \x01(\x01\x12\x0f\n\x07reqPart\x18\x04 \x01(\t\"\xa1\x02\n\x12SummaAnalysisReply\x12\x0f\n\x07summaID\x18\x01 \x01(\t\x12\x15\n\rallDsourceIDs\x18\x02 \x03(\t\x12!\n\x05state\x18\x03 \x01(\x0b\x32\x12.allego.SummaState\x12\x33\n\x0e\x61llDsourceSpec\x18\x04 \x03(\x0b\x32\x1b.allego.SummaDatasourceSpec\x12-\n\x08\x61ggStats\x18\x05 \x01(\x0b\x32\x1b.allego.SummaAggregateStats\x12@\n\x14reqAvailDsourceStats\x18\x06 \x03(\x0b\x32\".allego.SummaDatasourceAnalysisPkg\x12\x1a\n\x12reqAvailDsourceIDs\x18\x07 \x03(\t\"\xd9\x01\n\nSummaState\x12\x0f\n\x07summaID\x18\x01 \x02(\t\x12\x12\n\nisComplete\x18\x02 \x02(\x08\x12\x14\n\x0c\x66racComplete\x18\x03 \x02(\x01\x12\x0b\n\x03msg\x18\x04 \x02(\t\x12\x19\n\x11\x64srcWalltimeStart\x18\x05 \x02(\t\x12\x17\n\x0f\x64srcWalltimeEnd\x18\x06 \x02(\t\x12\x1d\n\x15\x61nalysisWallTimeStart\x18\x07 \x02(\t\x12\x1a\n\x12\x61nalysisElapsedSec\x18\x08 \x02(\x01\x12\x14\n\x0cpacketDurSec\x18\t \x02(\x01\"]\n\x13SummaAggregateStats\x12%\n\x08metricID\x18\x01 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x1f\n\x04hist\x18\x02 \x03(\x0b\x32\x11.allego.Histogram\"\xbd\x01\n\x1aSummaDatasourceAnalysisPkg\x12%\n\x08metricID\x18\x01 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x1f\n\x04hist\x18\x02 \x03(\x0b\x32\x11.allego.Histogram\x12!\n\x04recs\x18\x03 \x03(\x0b\x32\x13.allego.DenseMatrix\x12#\n\x08histRecs\x18\x04 \x03(\x0b\x32\x11.allego.Histogram\x12\x0f\n\x07ntvIdxs\x18\x05 \x03(\x03\"~\n\x13SummaDatasourceSpec\x12\x1f\n\x02sG\x18\x01 \x01(\x0b\x32\x13.allego.SignalGroup\x12\x1d\n\x02tR\x18\x02 \x01(\x0b\x32\x11.allego.TimeRange\x12\'\n\x06niSpec\x18\x03 \x01(\x0b\x32\x17.allego.SpikesSpecReply2\xfc\x32\n\x0bRadiensCore\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12\x41\n\rClientConnect\x12\x17.allego.RadiensClientId\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x10\x43lientDisconnect\x12\x17.allego.RadiensClientId\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12R\n\x17GetOfflineLicenseStatus\x12\x17.allego.StandardRequest\x1a\x1c.allego.OfflineLicenseStatus\"\x00\x12H\n\rListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12V\n\x12\x43opyDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12X\n\x14RemoveDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12P\n\x12MoveDataSourceFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12N\n\x13SpikesListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12R\n\x0eSpikesCopyFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x10SpikesRemoveFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12L\n\x0eSpikesMoveFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x16ManageNodeOrganization\x12\x1c.allego.ManageNodeOrgRequest\x1a\x1a.allego.ManageNodeOrgReply\"\x00\x12K\n\rManageNodeLab\x12\x1c.allego.ManageNodeLabRequest\x1a\x1a.allego.ManageNodeLabReply\"\x00\x12N\n\x0eManageNodeUser\x12\x1d.allego.ManageNodeUserRequest\x1a\x1b.allego.ManageNodeUserReply\"\x00\x12\x45\n\x0fManageNodeProbe\x12\x18.allego.ProbeNodeRequest\x1a\x16.allego.ProbeNodeReply\"\x00\x12\x41\n\x0bManageEdges\x12\x18.allego.WorldEdgeRequest\x1a\x16.allego.WorldEdgeReply\"\x00\x12\x42\n\nQueryWorld\x12\x19.allego.QueryWorldRequest\x1a\x17.allego.QueryWorldReply\"\x00\x12V\n\x1bGetWarehouseSensorComponent\x12\x19.allego.SensorCompRequest\x1a\x1a.allego.GetSensorCompReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12H\n\x0eGetSorterIDMap\x12\x17.allego.StandardRequest\x1a\x1b.allego.GetSorterIDMapReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x0fGetHDSnapshotPy\x12\x1a.allego.HDSnapshotRequest2\x1a\x13.allego.HDSnapshot2\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12+\n\x06GetPSD\x12\x12.allego.PSDRequest\x1a\x0b.allego.PSD\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12J\n\x0eListDataSource\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12K\n\x11ListDataSourceIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12[\n\x15SetDataSourceFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12I\n\x0f\x43learDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12J\n\x10RenameDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12P\n\x1aGetDataSourceKpiFileStatus\x12\x19.allego.DataSourceRequest\x1a\x15.allego.KpiFileStatus\"\x00\x12R\n\x1bGetDataSourceKpiFileStatus2\x12\x19.allego.DataSourceRequest\x1a\x16.allego.KpiFileStatus2\"\x00\x12\x46\n\x0eGetKpiMetadata\x12\x19.allego.DataSourceRequest\x1a\x17.allego.KpiFileMetadata\"\x00\x12?\n\x08KpiClear\x12\x1a.allego.KpiStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0cKpiCalculate\x12\x1a.allego.KpiStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12\x46\n\x0fSetKpiPacketDur\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x12K\n\x0bSetKpiParam\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x0bGetKpiParam\x12\x19.allego.DataSourceRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12W\n\x11SpikesSetFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12\x46\n\x0cSpikesGetIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12H\n\x0eSpikesRenameID\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12S\n\x17SpikesGetAllSummaryInfo\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12\x45\n\rSpikesGetSpec\x12\x19.allego.DataSourceRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12\x64\n\x13SpikesGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12[\n\x14SpikesGetSpikesDense\x12\x1e.allego.SpikesGetSpikesRequest\x1a!.allego.SpikesSpikeDataDenseReply\"\x00\x12q\n\x15GetSpikeTrainAnalytic\x12+.allego.SpikesGetSpikeTrainAnalyticsRequest\x1a).allego.SpikesGetSpikeTrainAnalyticsReply\"\x00\x12I\n\x0fSpikesDeleteIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12l\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x11.allego.TimeRange\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x12[\n\x1b\x42iointerfaceListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12J\n\x15\x42iointerfaceSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12`\n BiointerfaceSetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12^\n\x1f\x42iointerfaceSetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x11\x44\x65leteSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x12K\n\x14SpikesGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12\x33\n\x0bSetProtocol\x12\x10.allego.Protocol\x1a\x10.allego.Protocol\"\x00\x12:\n\x0bGetProtocol\x12\x17.allego.ProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12\x43\n\x0eRenameProtocol\x12\x1d.allego.RenameProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12J\n\x0fGetAllProtocols\x12\x17.allego.StandardRequest\x1a\x1c.allego.GetAllProtocolsReply\"\x00\x12K\n\rApplyProtocol\x12\x17.allego.ProtocolRequest\x1a\x1d.allego.ApplyProtocolProgress\"\x00\x30\x01\x32\xca\x07\n\x13RadiensSpikeSorter1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x63\n\x17SpikeSorterGetDashboard\x12#.allego.SpikeSorterDashboardRequest\x1a!.allego.SpikeSorterDashboardReply\"\x00\x12I\n\x16SpikeSorterWrangleData\x12\x16.allego.WrangleRequest\x1a\x15.allego.StandardReply\"\x00\x12W\n\x11SpikeSorterLaunch\x12 .allego.SpikeSorterLaunchRequest\x1a\x1e.allego.SpikeSorterLaunchReply\"\x00\x12P\n\x11SpikeSorterDelete\x12\".allego.SpikeSorterStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12Q\n\x17SpikeSorterImportMearec\x12\x14.allego.RecgenImport\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x32\xe2\x03\n\nDashboards\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12L\n\x10\x43ommandDashboard\x12\x1f.allego.DashboardCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x15LaunchSessionAnalysis\x12\x1c.allego.SummaAnalysisRequest\x1a\x1a.allego.SummaAnalysisReply\"\x00\x12P\n\x12GetSessionAnalysis\x12\x1c.allego.SummaAnalysisRequest\x1a\x1a.allego.SummaAnalysisReply\"\x00\x12\x45\n\x0cListSessions\x12\x17.allego.StandardRequest\x1a\x1a.allego.SummaSessionsReply\"\x00\x12\x44\n\x10\x43learAllSessions\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x32\x90\x05\n\x0bRadiensDev1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12S\n\x1aSpkSortTrainerMakeNewModel\x12\x1c.allego.SpkSortTrainerNewReq\x1a\x15.allego.StandardReply\"\x00\x12W\n\x1aSpkSortTrainerProfileModel\x12 .allego.SpkSortTrainerProfileReq\x1a\x15.allego.StandardReply\"\x00\x12W\n#SpkSortTrainerMakeDefaultProdModels\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n$SpkSortTrainerListLocalNetworkModels\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x12g\n&SpkSortTrainerDeleteLocalNetworkModels\x12$.allego.SpkSortTrainerDeleteModelReq\x1a\x15.allego.StandardReply\"\x00\x12W\n\x17SpkSortTrainerGetStatus\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13radiensserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\x1a\x11radiens_dev.proto\"K\n\x19RadiensHealthcheckRequest\x12\x1a\n\x12isIncludeWarehouse\x18\x01 \x01(\x08\x12\x12\n\nisDetailed\x18\x02 \x01(\x08\"]\n\x16RadiensHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\x12\x33\n\toutfitter\x18\x02 \x01(\x0b\x32 .allego.WarehouseHealthcheckSpec\"\x1e\n\x0fRadiensClientId\x12\x0b\n\x03pid\x18\x01 \x02(\x05\"\x91\x01\n\x12SummaSessionsReply\x12?\n\x07session\x18\x01 \x03(\x0b\x32..allego.SummaSessionsReply.SummaCurrentSession\x1a:\n\x13SummaCurrentSession\x12\x0f\n\x07summaID\x18\x01 \x02(\t\x12\x12\n\ndsourceIDs\x18\x02 \x03(\t\"_\n\x14SummaAnalysisRequest\x12\x0f\n\x07summaID\x18\x01 \x01(\t\x12\x12\n\ndsourceIDs\x18\x02 \x03(\t\x12\x11\n\tpktDurSec\x18\x03 \x01(\x01\x12\x0f\n\x07reqPart\x18\x04 \x01(\t\"\xa1\x02\n\x12SummaAnalysisReply\x12\x0f\n\x07summaID\x18\x01 \x01(\t\x12\x15\n\rallDsourceIDs\x18\x02 \x03(\t\x12!\n\x05state\x18\x03 \x01(\x0b\x32\x12.allego.SummaState\x12\x33\n\x0e\x61llDsourceSpec\x18\x04 \x03(\x0b\x32\x1b.allego.SummaDatasourceSpec\x12-\n\x08\x61ggStats\x18\x05 \x01(\x0b\x32\x1b.allego.SummaAggregateStats\x12@\n\x14reqAvailDsourceStats\x18\x06 \x03(\x0b\x32\".allego.SummaDatasourceAnalysisPkg\x12\x1a\n\x12reqAvailDsourceIDs\x18\x07 \x03(\t\"\xd9\x01\n\nSummaState\x12\x0f\n\x07summaID\x18\x01 \x02(\t\x12\x12\n\nisComplete\x18\x02 \x02(\x08\x12\x14\n\x0c\x66racComplete\x18\x03 \x02(\x01\x12\x0b\n\x03msg\x18\x04 \x02(\t\x12\x19\n\x11\x64srcWalltimeStart\x18\x05 \x02(\t\x12\x17\n\x0f\x64srcWalltimeEnd\x18\x06 \x02(\t\x12\x1d\n\x15\x61nalysisWallTimeStart\x18\x07 \x02(\t\x12\x1a\n\x12\x61nalysisElapsedSec\x18\x08 \x02(\x01\x12\x14\n\x0cpacketDurSec\x18\t \x02(\x01\"]\n\x13SummaAggregateStats\x12%\n\x08metricID\x18\x01 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x1f\n\x04hist\x18\x02 \x03(\x0b\x32\x11.allego.Histogram\"\xbd\x01\n\x1aSummaDatasourceAnalysisPkg\x12%\n\x08metricID\x18\x01 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x1f\n\x04hist\x18\x02 \x03(\x0b\x32\x11.allego.Histogram\x12!\n\x04recs\x18\x03 \x03(\x0b\x32\x13.allego.DenseMatrix\x12#\n\x08histRecs\x18\x04 \x03(\x0b\x32\x11.allego.Histogram\x12\x0f\n\x07ntvIdxs\x18\x05 \x03(\x03\"~\n\x13SummaDatasourceSpec\x12\x1f\n\x02sG\x18\x01 \x01(\x0b\x32\x13.allego.SignalGroup\x12\x1d\n\x02tR\x18\x02 \x01(\x0b\x32\x11.allego.TimeRange\x12\'\n\x06niSpec\x18\x03 \x01(\x0b\x32\x17.allego.SpikesSpecReply2\xfc\x32\n\x0bRadiensCore\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12\x41\n\rClientConnect\x12\x17.allego.RadiensClientId\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x10\x43lientDisconnect\x12\x17.allego.RadiensClientId\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12R\n\x17GetOfflineLicenseStatus\x12\x17.allego.StandardRequest\x1a\x1c.allego.OfflineLicenseStatus\"\x00\x12H\n\rListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12V\n\x12\x43opyDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12X\n\x14RemoveDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12P\n\x12MoveDataSourceFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12N\n\x13SpikesListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12R\n\x0eSpikesCopyFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x10SpikesRemoveFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12L\n\x0eSpikesMoveFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x16ManageNodeOrganization\x12\x1c.allego.ManageNodeOrgRequest\x1a\x1a.allego.ManageNodeOrgReply\"\x00\x12K\n\rManageNodeLab\x12\x1c.allego.ManageNodeLabRequest\x1a\x1a.allego.ManageNodeLabReply\"\x00\x12N\n\x0eManageNodeUser\x12\x1d.allego.ManageNodeUserRequest\x1a\x1b.allego.ManageNodeUserReply\"\x00\x12\x45\n\x0fManageNodeProbe\x12\x18.allego.ProbeNodeRequest\x1a\x16.allego.ProbeNodeReply\"\x00\x12\x41\n\x0bManageEdges\x12\x18.allego.WorldEdgeRequest\x1a\x16.allego.WorldEdgeReply\"\x00\x12\x42\n\nQueryWorld\x12\x19.allego.QueryWorldRequest\x1a\x17.allego.QueryWorldReply\"\x00\x12V\n\x1bGetWarehouseSensorComponent\x12\x19.allego.SensorCompRequest\x1a\x1a.allego.GetSensorCompReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12H\n\x0eGetSorterIDMap\x12\x17.allego.StandardRequest\x1a\x1b.allego.GetSorterIDMapReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x0fGetHDSnapshotPy\x12\x1a.allego.HDSnapshotRequest2\x1a\x13.allego.HDSnapshot2\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12+\n\x06GetPSD\x12\x12.allego.PSDRequest\x1a\x0b.allego.PSD\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12J\n\x0eListDataSource\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12K\n\x11ListDataSourceIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12[\n\x15SetDataSourceFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12I\n\x0f\x43learDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12J\n\x10RenameDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12P\n\x1aGetDataSourceKpiFileStatus\x12\x19.allego.DataSourceRequest\x1a\x15.allego.KpiFileStatus\"\x00\x12R\n\x1bGetDataSourceKpiFileStatus2\x12\x19.allego.DataSourceRequest\x1a\x16.allego.KpiFileStatus2\"\x00\x12\x46\n\x0eGetKpiMetadata\x12\x19.allego.DataSourceRequest\x1a\x17.allego.KpiFileMetadata\"\x00\x12?\n\x08KpiClear\x12\x1a.allego.KpiStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0cKpiCalculate\x12\x1a.allego.KpiStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12\x46\n\x0fSetKpiPacketDur\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x12K\n\x0bSetKpiParam\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x0bGetKpiParam\x12\x19.allego.DataSourceRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12W\n\x11SpikesSetFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12\x46\n\x0cSpikesGetIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12H\n\x0eSpikesRenameID\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12S\n\x17SpikesGetAllSummaryInfo\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12\x45\n\rSpikesGetSpec\x12\x19.allego.DataSourceRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12\x64\n\x13SpikesGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12[\n\x14SpikesGetSpikesDense\x12\x1e.allego.SpikesGetSpikesRequest\x1a!.allego.SpikesSpikeDataDenseReply\"\x00\x12q\n\x15GetSpikeTrainAnalytic\x12+.allego.SpikesGetSpikeTrainAnalyticsRequest\x1a).allego.SpikesGetSpikeTrainAnalyticsReply\"\x00\x12I\n\x0fSpikesDeleteIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12l\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x11.allego.TimeRange\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x12[\n\x1b\x42iointerfaceListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12J\n\x15\x42iointerfaceSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12`\n BiointerfaceSetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12^\n\x1f\x42iointerfaceSetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x11\x44\x65leteSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x12K\n\x14SpikesGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12\x33\n\x0bSetProtocol\x12\x10.allego.Protocol\x1a\x10.allego.Protocol\"\x00\x12:\n\x0bGetProtocol\x12\x17.allego.ProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12\x43\n\x0eRenameProtocol\x12\x1d.allego.RenameProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12J\n\x0fGetAllProtocols\x12\x17.allego.StandardRequest\x1a\x1c.allego.GetAllProtocolsReply\"\x00\x12K\n\rApplyProtocol\x12\x17.allego.ProtocolRequest\x1a\x1d.allego.ApplyProtocolProgress\"\x00\x30\x01\x32\x8c\t\n\x13RadiensSpikeSorter1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SpikeSorterSetParams\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x63\n\x17SpikeSorterGetDashboard\x12#.allego.SpikeSorterDashboardRequest\x1a!.allego.SpikeSorterDashboardReply\"\x00\x12j\n\x1bSpikeSorterGetFeatureParams\x12\".allego.SpikeSorterStandardRequest\x1a%.allego.SpikeSorterFeatureParamsReply\"\x00\x12I\n\x16SpikeSorterWrangleData\x12\x16.allego.WrangleRequest\x1a\x15.allego.StandardReply\"\x00\x12W\n\x11SpikeSorterLaunch\x12 .allego.SpikeSorterLaunchRequest\x1a\x1e.allego.SpikeSorterLaunchReply\"\x00\x12P\n\x11SpikeSorterDelete\x12\".allego.SpikeSorterStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12Q\n\x17SpikeSorterImportMearec\x12\x14.allego.RecgenImport\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x32\xe2\x03\n\nDashboards\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12L\n\x10\x43ommandDashboard\x12\x1f.allego.DashboardCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x15LaunchSessionAnalysis\x12\x1c.allego.SummaAnalysisRequest\x1a\x1a.allego.SummaAnalysisReply\"\x00\x12P\n\x12GetSessionAnalysis\x12\x1c.allego.SummaAnalysisRequest\x1a\x1a.allego.SummaAnalysisReply\"\x00\x12\x45\n\x0cListSessions\x12\x17.allego.StandardRequest\x1a\x1a.allego.SummaSessionsReply\"\x00\x12\x44\n\x10\x43learAllSessions\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x32\x90\x05\n\x0bRadiensDev1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12S\n\x1aSpkSortTrainerMakeNewModel\x12\x1c.allego.SpkSortTrainerNewReq\x1a\x15.allego.StandardReply\"\x00\x12W\n\x1aSpkSortTrainerProfileModel\x12 .allego.SpkSortTrainerProfileReq\x1a\x15.allego.StandardReply\"\x00\x12W\n#SpkSortTrainerMakeDefaultProdModels\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n$SpkSortTrainerListLocalNetworkModels\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x12g\n&SpkSortTrainerDeleteLocalNetworkModels\x12$.allego.SpkSortTrainerDeleteModelReq\x1a\x15.allego.StandardReply\"\x00\x12W\n\x17SpkSortTrainerGetStatus\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'radiensserver_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
@@ -47,13 +47,13 @@
   _SUMMADATASOURCEANALYSISPKG._serialized_start=1178
   _SUMMADATASOURCEANALYSISPKG._serialized_end=1367
   _SUMMADATASOURCESPEC._serialized_start=1369
   _SUMMADATASOURCESPEC._serialized_end=1495
   _RADIENSCORE._serialized_start=1498
   _RADIENSCORE._serialized_end=8022
   _RADIENSSPIKESORTER1._serialized_start=8025
-  _RADIENSSPIKESORTER1._serialized_end=8995
-  _DASHBOARDS._serialized_start=8998
-  _DASHBOARDS._serialized_end=9480
-  _RADIENSDEV1._serialized_start=9483
-  _RADIENSDEV1._serialized_end=10139
+  _RADIENSSPIKESORTER1._serialized_end=9189
+  _DASHBOARDS._serialized_start=9192
+  _DASHBOARDS._serialized_end=9674
+  _RADIENSDEV1._serialized_start=9677
+  _RADIENSDEV1._serialized_end=10333
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-3.0.0b5/radiens/grpc_radiens/radiensserver_pb2_grpc.py` & `radiens-3.0.0b6/radiens/grpc_radiens/radiensserver_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -2865,14 +2865,19 @@
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.SpikeSorterSetParam = channel.unary_unary(
                 '/allego.RadiensSpikeSorter1/SpikeSorterSetParam',
                 request_serializer=common__pb2.SpikeSorterSetParamRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
+        self.SpikeSorterSetParams = channel.unary_unary(
+                '/allego.RadiensSpikeSorter1/SpikeSorterSetParams',
+                request_serializer=common__pb2.SpikeSorterSetParamsRequest.SerializeToString,
+                response_deserializer=common__pb2.StandardReply.FromString,
+                )
         self.SpikeSorterGetParam = channel.unary_unary(
                 '/allego.RadiensSpikeSorter1/SpikeSorterGetParam',
                 request_serializer=spikesorter__pb2.SpikeSorterStandardRequest.SerializeToString,
                 response_deserializer=spikesorter__pb2.GetSpikeSorterParamCommandReply.FromString,
                 )
         self.SpikeSorterGetState = channel.unary_unary(
                 '/allego.RadiensSpikeSorter1/SpikeSorterGetState',
@@ -2880,14 +2885,19 @@
                 response_deserializer=spikesorter__pb2.SpikeSorterState.FromString,
                 )
         self.SpikeSorterGetDashboard = channel.unary_unary(
                 '/allego.RadiensSpikeSorter1/SpikeSorterGetDashboard',
                 request_serializer=spikesorter__pb2.SpikeSorterDashboardRequest.SerializeToString,
                 response_deserializer=spikesorter__pb2.SpikeSorterDashboardReply.FromString,
                 )
+        self.SpikeSorterGetFeatureParams = channel.unary_unary(
+                '/allego.RadiensSpikeSorter1/SpikeSorterGetFeatureParams',
+                request_serializer=spikesorter__pb2.SpikeSorterStandardRequest.SerializeToString,
+                response_deserializer=spikesorter__pb2.SpikeSorterFeatureParamsReply.FromString,
+                )
         self.SpikeSorterWrangleData = channel.unary_unary(
                 '/allego.RadiensSpikeSorter1/SpikeSorterWrangleData',
                 request_serializer=radiens__dev__pb2.WrangleRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.SpikeSorterLaunch = channel.unary_unary(
                 '/allego.RadiensSpikeSorter1/SpikeSorterLaunch',
@@ -2930,14 +2940,20 @@
 
     def SpikeSorterSetParam(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SpikeSorterSetParams(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def SpikeSorterGetParam(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SpikeSorterGetState(self, request, context):
@@ -2948,14 +2964,20 @@
 
     def SpikeSorterGetDashboard(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SpikeSorterGetFeatureParams(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def SpikeSorterWrangleData(self, request, context):
         """specific to radiensserver
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -2997,14 +3019,19 @@
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'SpikeSorterSetParam': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikeSorterSetParam,
                     request_deserializer=common__pb2.SpikeSorterSetParamRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
+            'SpikeSorterSetParams': grpc.unary_unary_rpc_method_handler(
+                    servicer.SpikeSorterSetParams,
+                    request_deserializer=common__pb2.SpikeSorterSetParamsRequest.FromString,
+                    response_serializer=common__pb2.StandardReply.SerializeToString,
+            ),
             'SpikeSorterGetParam': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikeSorterGetParam,
                     request_deserializer=spikesorter__pb2.SpikeSorterStandardRequest.FromString,
                     response_serializer=spikesorter__pb2.GetSpikeSorterParamCommandReply.SerializeToString,
             ),
             'SpikeSorterGetState': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikeSorterGetState,
@@ -3012,14 +3039,19 @@
                     response_serializer=spikesorter__pb2.SpikeSorterState.SerializeToString,
             ),
             'SpikeSorterGetDashboard': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikeSorterGetDashboard,
                     request_deserializer=spikesorter__pb2.SpikeSorterDashboardRequest.FromString,
                     response_serializer=spikesorter__pb2.SpikeSorterDashboardReply.SerializeToString,
             ),
+            'SpikeSorterGetFeatureParams': grpc.unary_unary_rpc_method_handler(
+                    servicer.SpikeSorterGetFeatureParams,
+                    request_deserializer=spikesorter__pb2.SpikeSorterStandardRequest.FromString,
+                    response_serializer=spikesorter__pb2.SpikeSorterFeatureParamsReply.SerializeToString,
+            ),
             'SpikeSorterWrangleData': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikeSorterWrangleData,
                     request_deserializer=radiens__dev__pb2.WrangleRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'SpikeSorterLaunch': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikeSorterLaunch,
@@ -3099,14 +3131,31 @@
         return grpc.experimental.unary_unary(request, target, '/allego.RadiensSpikeSorter1/SpikeSorterSetParam',
             common__pb2.SpikeSorterSetParamRequest.SerializeToString,
             common__pb2.StandardReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def SpikeSorterSetParams(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensSpikeSorter1/SpikeSorterSetParams',
+            common__pb2.SpikeSorterSetParamsRequest.SerializeToString,
+            common__pb2.StandardReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def SpikeSorterGetParam(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -3150,14 +3199,31 @@
         return grpc.experimental.unary_unary(request, target, '/allego.RadiensSpikeSorter1/SpikeSorterGetDashboard',
             spikesorter__pb2.SpikeSorterDashboardRequest.SerializeToString,
             spikesorter__pb2.SpikeSorterDashboardReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def SpikeSorterGetFeatureParams(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensSpikeSorter1/SpikeSorterGetFeatureParams',
+            spikesorter__pb2.SpikeSorterStandardRequest.SerializeToString,
+            spikesorter__pb2.SpikeSorterFeatureParamsReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def SpikeSorterWrangleData(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `radiens-3.0.0b5/radiens/grpc_radiens/spikesorter_pb2.py` & `radiens-3.0.0b6/radiens/grpc_radiens/spikesorter_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import common_pb2 as common__pb2
 from . import biointerface_pb2 as biointerface__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11spikesorter.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x12\x62iointerface.proto\"\xa3\x01\n\x18SpikeSorterLaunchRequest\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12&\n\x06source\x18\x02 \x01(\x0b\x32\x16.allego.FileDescriptor\x12\x0c\n\x04seed\x18\x03 \x01(\x03\x12\x18\n\x10neighborRadiusUm\x18\x05 \x01(\x01\x12\x10\n\x08isAutoOn\x18\t \x01(\x08\x12\x12\n\nnbrPattern\x18\n \x01(\x05\"\x8a\x01\n\x19SpikeSorterCommandRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\'\n\x03\x63md\x18\x02 \x02(\x0e\x32\x1a.allego.SpikeSorterCommand\x12-\n\x06subCmd\x18\x03 \x02(\x0e\x32\x1d.allego.SpikeSorterSubCommand\"\x86\x02\n\x10SpikeSorterState\x12+\n\x03sys\x18\x01 \x02(\x0e\x32\x1e.allego.SpikeSorterStateSystem\x12\x14\n\x0c\x66racComplete\x18\x02 \x01(\x01\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\x12\n\nlaunchTime\x18\x04 \x01(\t\x12\x16\n\x0einitializeTime\x18\x05 \x01(\t\x12\x18\n\x10sessionStartTime\x18\x06 \x01(\t\x12\x17\n\x0fsessionStopTime\x18\x07 \x01(\t\x12\x0c\n\x04isOn\x18\x08 \x01(\x08\x12\x1a\n\x12kernelErrorMessage\x18\t \x01(\t\x12\x19\n\x11kernelWarnMessage\x18\n \x01(\t\"\x81\x01\n\x0cSpkSortIOreq\x12#\n\x04type\x18\x01 \x02(\x0e\x32\x15.allego.SpkSortIOtype\x12\'\n\x06target\x18\x02 \x02(\x0e\x32\x17.allego.SpkSortIOtarget\x12#\n\x04mode\x18\x03 \x02(\x0e\x32\x15.allego.SpkSortIOmode\"\x8f\x01\n\x16SpikeSorterLaunchReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12+\n\nsorterType\x18\x02 \x02(\x0e\x32\x17.allego.SpikeSorterType\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12$\n\x04\x64\x65sc\x18\x04 \x01(\x0b\x32\x16.allego.FileDescriptor\"0\n\x16GetSpikeSorterIDsReply\x12\x16\n\x0espikeSorterIDs\x18\x01 \x03(\t\"\xdd\x01\n\x1fSpikeSorterGetRasterDataRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x12\n\ntimeWindow\x18\x03 \x02(\x01\x12\x17\n\x0fplotWidthPoints\x18\x04 \x02(\x01\x12\x13\n\x0b\x63omponentID\x18\x05 \x02(\t\x12\x11\n\ttimeRange\x18\x06 \x03(\x01\x12 \n\x04mode\x18\x07 \x02(\x0e\x32\x12.allego.RasterMode\x12\x13\n\x0blabeledOnly\x18\x08 \x01(\x08\x12\x17\n\x0fprimarySiteOnly\x18\t \x01(\x08\"\x9d\x01\n\x1aSpikeSorterRasterDataReply\x12/\n\x0fspikeTimestamps\x18\x02 \x03(\x0b\x32\x16.allego.SpikeTimestamp\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimeStampRange\x18\x04 \x03(\x03\x12\x10\n\x08GPIOData\x18\x05 \x02(\x0c\x12\x11\n\tGPIOShape\x18\x06 \x03(\x05\"3\n\x1aSpikeSorterStandardRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\"_\n\x1bSpikeSorterDashboardRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12)\n\x0c\x64\x61shElements\x18\x02 \x03(\x0e\x32\x13.allego.DashElement\"\x86\x03\n\x12SpikeSorterDynamic\x12\x11\n\tisEnabled\x18\x01 \x01(\x08\x12\x43\n\x0fupdatePeriodSec\x18\x02 \x01(\x0b\x32*.allego.SpikeSorterDynamic.UpdatePeriodSec\x12\x35\n\x08\x63riteria\x18\x03 \x01(\x0b\x32#.allego.SpikeSorterDynamic.Criteria\x1a\xa0\x01\n\x08\x43riteria\x12\x31\n\x06\x64\x65tect\x18\x01 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x12\x30\n\x05train\x18\x02 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x12/\n\x04sort\x18\x03 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x1a>\n\x0fUpdatePeriodSec\x12\x0e\n\x06\x64\x65tect\x18\x01 \x01(\x01\x12\r\n\x05train\x18\x02 \x01(\x01\x12\x0c\n\x04sort\x18\x03 \x01(\x01\"\xc5\x01\n\x1cSpikeSorterSetDynamicRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x42\n\x07variant\x18\x02 \x03(\x0b\x32\x31.allego.SpikeSorterSetDynamicRequest.VariantEntry\x1aJ\n\x0cVariantEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.allego.SpikeSorterDynamic:\x02\x38\x01\"\xd8\x01\n\x1aSpikeSorterGetDynamicReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x15\n\rrootVariantID\x18\x02 \x02(\t\x12@\n\x07variant\x18\x03 \x03(\x0b\x32/.allego.SpikeSorterGetDynamicReply.VariantEntry\x1aJ\n\x0cVariantEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.allego.SpikeSorterDynamic:\x02\x38\x01\"l\n\x1fGetSpikeSorterParamCommandReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x32\n\x03rec\x18\x02 \x03(\x0b\x32%.allego.SpikeSorterParamCommandRecord\"3\n\x12\x43lusterMapOutliers\x12\x0c\n\x04mild\x18\x01 \x03(\x01\x12\x0f\n\x07\x65xtreme\x18\x02 \x03(\x01\"9\n\x13\x43lusterMapQuartiles\x12\n\n\x02q1\x18\x01 \x02(\x01\x12\n\n\x02q2\x18\x02 \x02(\x01\x12\n\n\x02q3\x18\x03 \x02(\x01\"\x83\x01\n\x0f\x43lusterMapStats\x12\x16\n\x0e\x63\x65ntroidCenter\x18\x01 \x03(\x01\x12\x12\n\ncentroidSd\x18\x02 \x03(\x01\x12\x16\n\x0e\x63\x65ntroidSdNorm\x18\x03 \x02(\x01\x12\x19\n\x11intraCentroidDist\x18\x04 \x03(\x01\x12\x11\n\tnumSpikes\x18\x05 \x02(\x03\"f\n\x10\x43lusterMapRecord\x12\r\n\x05label\x18\x01 \x02(\x05\x12&\n\x05stats\x18\x03 \x02(\x0b\x32\x17.allego.ClusterMapStats\x12\x1b\n\x13numSpikesTrainCache\x18\x04 \x02(\x03\"\xa8\x01\n\x13SpikeSortSiteStatus\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x15\n\rorderedLabels\x18\x02 \x03(\x05\x12)\n\x07\x63luster\x18\x03 \x03(\x0b\x32\x18.allego.ClusterMapRecord\x12\x11\n\tnumSpikes\x18\x04 \x03(\x03\x12\x0c\n\x04zeta\x18\x05 \x03(\x01\x12\x1a\n\x12\x61ggregateSpikeRate\x18\x06 \x02(\x01\"\x8f\x01\n\x14SpikeSortPhaseStatus\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x12\n\nchunkIndex\x18\x02 \x02(\x03\x12\x14\n\x0cupdatePeriod\x18\x03 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\x04 \x02(\x01\x12\x12\n\nisComplete\x18\x05 \x02(\x08\x12\x18\n\x10\x66ractionComplete\x18\x06 \x02(\x01\"*\n\x13SpikeSortNbrIdxList\x12\x13\n\x0bntvChanIdxs\x18\x01 \x03(\x05\"\xf2\x02\n\x16SpikeSorterStatusReply\x12\'\n\x05state\x18\x01 \x02(\x0b\x32\x18.allego.SpikeSorterState\x12\x16\n\x0e\x62iointerfaceID\x18\x03 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x04 \x02(\t\x12\x10\n\x08sampFreq\x18\x05 \x02(\x01\x12\x19\n\x11\x65nabledNtvChanIdx\x18\x06 \x03(\x05\x12+\n\x05phase\x18\x07 \x03(\x0b\x32\x1c.allego.SpikeSortPhaseStatus\x12\x30\n\x0b\x65nabledSite\x18\x08 \x03(\x0b\x32\x1b.allego.SpikeSortSiteStatus\x12\x12\n\nprobeYield\x18\t \x02(\x01\x12\x11\n\tsortStats\x18\n \x03(\x01\x12\x1b\n\x13\x64\x61tasourceTimeRange\x18\x0c \x03(\x01\x12\x1d\n\x15\x62iointerfaceTimeRange\x18\r \x03(\x01\x12\x12\n\nnumNeurons\x18\x0f \x02(\x03\"R\n\x1eSpikeSorterStatusVariantsReply\x12\x30\n\x08variants\x18\x01 \x03(\x0b\x32\x1e.allego.SpikeSorterStatusReply\"\xfd\x02\n\x19SpikeSorterClassifierSpec\x12\r\n\x05\x61lpha\x18\x01 \x02(\x01\x12\x11\n\talphaBias\x18\x02 \x02(\x01\x12\x16\n\x0e\x64imOutputLayer\x18\x03 \x02(\x05\x12\x16\n\x0e\x65rrorTolerance\x18\x04 \x02(\x01\x12\x19\n\x11hiddenLayerFactor\x18\x05 \x02(\x01\x12\n\n\x02iD\x18\x06 \x02(\t\x12\x16\n\x0einitBiasStdDev\x18\x07 \x02(\x01\x12\x18\n\x10initWeightStdDev\x18\x08 \x02(\x01\x12\x11\n\tisMasking\x18\t \x02(\x08\x12\x10\n\x08l1lambda\x18\n \x02(\x01\x12\x15\n\rminibatchSize\x18\x0b \x02(\x05\x12\x15\n\rmaxNumSamples\x18\x0c \x02(\x05\x12\x11\n\tnumEpochs\x18\r \x02(\x05\x12\x19\n\x11numSamplesTestMSE\x18\x0e \x02(\x05\x12\x1b\n\x13numConcurrentModels\x18\x0f \x02(\x05\x12\x17\n\x0flabelNoiseLevel\x18\x10 \x02(\x01\"u\n\x16SpikeSorterVariantSpec\x12\n\n\x02iD\x18\x01 \x02(\t\x12\x14\n\x0csiteConfigID\x18\x02 \x02(\t\x12\x39\n\x0e\x63lassifierSpec\x18\x03 \x02(\x0b\x32!.allego.SpikeSorterClassifierSpec\"\xcc\x01\n\x0fSpikeSorterSpec\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x02 \x02(\t\x12\x16\n\x0e\x62iointerfaceID\x18\x03 \x02(\t\x12\x1b\n\x13maxNumSiteNeighbors\x18\x04 \x02(\x05\x12\x18\n\x10neighborRadiusUm\x18\x05 \x02(\x01\x12/\n\x07variant\x18\x06 \x03(\x0b\x32\x1e.allego.SpikeSorterVariantSpec\x12\x0c\n\x04seed\x18\x08 \x02(\x03\"\xc2\x01\n\x19SpikeSorterGetConfigReply\x12%\n\x04spec\x18\x01 \x02(\x0b\x32\x17.allego.SpikeSorterSpec\x12\x16\n\x0e\x61IupdatePeriod\x18\x02 \x02(\x01\x12\x19\n\x11orderedVariantIDs\x18\x03 \x03(\t\x12\x15\n\rrootVariantID\x18\x04 \x02(\t\x12\x34\n\x0csorterStatus\x18\x06 \x03(\x0b\x32\x1e.allego.SpikeSorterStatusReply\"\x90\x02\n\x15SpikeSorterVizRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x11\n\tvariantID\x18\x02 \x02(\t\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12\x13\n\x0bspikeLabels\x18\x04 \x03(\x05\x12\x34\n\x07vizType\x18\x05 \x02(\x0e\x32#.allego.SpikeSorterVizRequest.VType\x12\x14\n\x0cisYAutoScale\x18\x06 \x02(\x08\x12\x0c\n\x04yLim\x18\x07 \x03(\x01\x12\x0e\n\x06\x66igDir\x18\x08 \x02(\t\x12\x11\n\tnumSpikes\x18\t \x02(\x05\"\'\n\x05VType\x12\x1e\n\x1aVIZ_SPIKESORT_TRAIN_SPIKES\x10\x00\"\xb6\x05\n\x19SpikeSorterDashboardReply\x12\"\n\x0c\x65nabledPorts\x18\x01 \x03(\x0e\x32\x0c.allego.Port\x12\x37\n\x07general\x18\x02 \x01(\x0b\x32&.allego.SpikeSorterDashboardGeneralRec\x12\x33\n\tsiteStats\x18\x03 \x01(\x0b\x32 .allego.IndicoDashboardSiteStats\x12\x43\n\tportStats\x18\x04 \x03(\x0b\x32\x30.allego.SpikeSorterDashboardReply.PortStatsEntry\x12\x43\n\tsitePanel\x18\x05 \x03(\x0b\x32\x30.allego.SpikeSorterDashboardReply.SitePanelEntry\x12G\n\x0bneuronPanel\x18\x06 \x03(\x0b\x32\x32.allego.SpikeSorterDashboardReply.NeuronPanelEntry\x12*\n\x02\x61I\x18\x07 \x01(\x0b\x32\x1e.allego.SpikeSorterDashboardAI\x1aR\n\x0ePortStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .allego.IndicoDashboardPortStats:\x02\x38\x01\x1aW\n\x0eSitePanelEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.allego.IndicoDashboardSiteIndicators:\x02\x38\x01\x1a[\n\x10NeuronPanelEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.allego.IndicoDashboardNeuronIndicators:\x02\x38\x01\"\xac\x03\n\x1eSpikeSorterDashboardGeneralRec\x12\'\n\x05state\x18\x01 \x02(\x0b\x32\x18.allego.SpikeSorterState\x12+\n\nsorterType\x18\x02 \x02(\x0e\x32\x17.allego.SpikeSorterType\x12\x10\n\x08sorterID\x18\x03 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x04 \x02(\t\x12\x11\n\ttimeRange\x18\x05 \x03(\x01\x12\x15\n\rnumTotalSites\x18\x06 \x02(\x03\x12\x17\n\x0fnumEnabledSites\x18\x07 \x02(\x03\x12\x16\n\x0enumActiveSites\x18\x08 \x02(\x03\x12\x12\n\nnumNeurons\x18\t \x02(\x03\x12\x12\n\nprobeYield\x18\n \x02(\x01\x12\x11\n\tsiteYield\x18\x0b \x02(\x01\x12\x1a\n\x12numSpikesProcessed\x18\x0c \x02(\x03\x12\x18\n\x10numSpikesLabeled\x18\r \x02(\x03\x12\x16\n\x0esortEfficiency\x18\x0e \x02(\x01\x12(\n\x08sinkDesc\x18\x0f \x02(\x0b\x32\x16.allego.FileDescriptor\"\xd5\x01\n\x16SpikeSorterDashboardAI\x12\x0c\n\x04\x62\x65ta\x18\x01 \x02(\x01\x12\"\n\x1a\x65stimatedReaderCompleteSec\x18\x02 \x02(\x01\x12\x1a\n\x12interSessionDurSec\x18\x03 \x02(\x01\x12\x19\n\x11interSessionStart\x18\x04 \x02(\t\x12\x15\n\rsessionDurSec\x18\x05 \x02(\x01\x12\x14\n\x0csessionStart\x18\x06 \x02(\t\x12\x12\n\nsessionIdx\x18\x07 \x02(\x03\x12\x11\n\tstartTime\x18\x08 \x02(\t\"_\n\x18IndicoDashboardSiteStats\x12\x0b\n\x03snr\x18\x01 \x03(\x01\x12\r\n\x05noise\x18\x02 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x03 \x03(\x01\x12\x12\n\nnumNeurons\x18\x04 \x02(\x03\"\x90\x01\n\x18IndicoDashboardPortStats\x12\x0b\n\x03snr\x18\x01 \x03(\x01\x12\r\n\x05noise\x18\x02 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x03 \x03(\x01\x12\x16\n\x0esortEfficiency\x18\x04 \x02(\x01\x12\x17\n\x0fnumEnabledSites\x18\x05 \x02(\x03\x12\x12\n\nnumNeurons\x18\x06 \x02(\x03\"\xd9\x01\n\x1dIndicoDashboardSiteIndicators\x12\x12\n\nntvChanIdx\x18\x01 \x03(\x05\x12\x0b\n\x03snr\x18\x02 \x03(\x01\x12\r\n\x05noise\x18\x03 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x04 \x03(\x01\x12\x16\n\x0esortEfficiency\x18\x05 \x03(\x01\x12\x11\n\tspikeRate\x18\x06 \x03(\x01\x12\x11\n\tposProbeX\x18\x07 \x03(\x01\x12\x11\n\tposProbeY\x18\x08 \x03(\x01\x12\x11\n\tposProbeZ\x18\t \x03(\x01\x12\x0f\n\x07siteNum\x18\n \x03(\x05\"\xb1\x01\n\x1fIndicoDashboardNeuronIndicators\x12\x10\n\x08neuronID\x18\x01 \x03(\t\x12\x0b\n\x03snr\x18\x02 \x03(\x01\x12\x11\n\tspikeRate\x18\x03 \x03(\x01\x12\x11\n\tposProbeX\x18\x04 \x03(\x01\x12\x11\n\tposProbeY\x18\x05 \x03(\x01\x12\x11\n\tposProbeZ\x18\x06 \x03(\x01\x12\x0f\n\x07siteNum\x18\x07 \x03(\x05\x12\x12\n\nspikeLabel\x18\x08 \x03(\x05\"\xa7\x02\n\x1cSpikeSorterDashboardSiteDesc\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x10\n\x08posProbe\x18\x03 \x03(\x01\x12\x10\n\x08posBrain\x18\x04 \x03(\x01\x12\x0e\n\x06snrMax\x18\x05 \x02(\x01\x12\x0e\n\x06snrMin\x18\x06 \x02(\x01\x12\x12\n\nnoiseLevel\x18\x07 \x02(\x01\x12\x12\n\nnumNeurons\x18\x08 \x02(\x03\x12/\n\rindicoCluster\x18\n \x03(\x0b\x32\x18.allego.ClusterMapRecord\x12\x1c\n\x14pileWaveformMinValue\x18\r \x02(\x02\x12\x1c\n\x14pileWaveformMaxValue\x18\x0e \x02(\x02\"\xd2\x01\n\x1eSpikeSorterDashboardNeuronDesc\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12&\n\x04\x64\x65sc\x18\x02 \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x0b\n\x03snr\x18\x05 \x02(\x01\x12\x0f\n\x07IsihMax\x18\x06 \x02(\x01\x12\x15\n\rIsihArgmaxSec\x18\x07 \x02(\x01\x12\x15\n\rIsihArgmaxIdx\x18\x08 \x02(\x03\x12\x10\n\x08IsihMean\x18\t \x02(\x01\x12\x0e\n\x06IsihSd\x18\n \x02(\x01\"\xfa\x01\n SpikeSorterDashboardNeuronDetail\x12&\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x18\n\x10templateWaveform\x18\x02 \x03(\x02\x12\x1a\n\x12templateSdWaveform\x18\x03 \x03(\x02\x12\x18\n\x10pileWaveformData\x18\x04 \x03(\x02\x12\x1e\n\x16numSamplesPileWaveform\x18\x05 \x02(\x05\x12\x18\n\x10numPileWaveforms\x18\x06 \x02(\x05\x12$\n\x04isih\x18\x0b \x02(\x0b\x32\x16.allego.NeuronHistData\"\xa9\x01\n\x1eSpikeSorterDashboardSiteDetail\x12\x32\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32$.allego.SpikeSorterDashboardSiteDesc\x12\x19\n\x11orderedSpikeLabel\x18\x02 \x03(\x05\x12\x38\n\x06neuron\x18\x03 \x03(\x0b\x32(.allego.SpikeSorterDashboardNeuronDetail*\x80\x01\n\x0fSpikeSorterType\x12\x0f\n\x0bSORTER_NULL\x10\x00\x12\x15\n\x11SORTER_VEX_STREAM\x10\x01\x12\x18\n\x14SORTER_SPIKES_STREAM\x10\x02\x12\x13\n\x0fSORTER_VEX_FILE\x10\x03\x12\x16\n\x12SORTER_SPIKES_FILE\x10\x04*\xb0\x01\n\x12SpikeSorterCommand\x12\x11\n\rSORTER_CMD_ON\x10\x00\x12\x12\n\x0eSORTER_CMD_OFF\x10\x01\x12\x19\n\x15SORTER_CMD_CLEAR_SORT\x10\x02\x12\x15\n\x11SORTER_CMD_REBASE\x10\x04\x12\x13\n\x0fSORTER_CMD_INIT\x10\x07\x12\x17\n\x13SORTER_CMD_LOCALIZE\x10\x08\x12\x13\n\x0fSORTER_CMD_SORT\x10\t*/\n\x15SpikeSorterSubCommand\x12\x16\n\x12SORTER_SUBCMD_NULL\x10\x00*@\n\x0fSpikeSorterMode\x12\x16\n\x12SORTER_MODE_STREAM\x10\x00\x12\x15\n\x11SORTER_MODE_BATCH\x10\x01*8\n\x10\x44\x65\x63InputFeatures\x12\x11\n\rALL_NEIGHBORS\x10\x00\x12\x11\n\rSVD_NEIGHBORS\x10\x01*I\n\x16SpikeSorterStateSystem\x12\n\n\x06SYS_ON\x10\x00\x12\x0b\n\x07SYS_OFF\x10\x01\x12\x16\n\x12SYS_NOT_CONFIGURED\x10\x02*f\n\rSpkSortIOtype\x12\x17\n\x13SPK_SORT_IO_NETWORK\x10\x00\x12\x17\n\x13SPK_SORT_IO_TRAINER\x10\x01\x12#\n\x1fSPK_SORT_IO_NETWORK_AND_TRAINER\x10\x02*>\n\x0fSpkSortIOtarget\x12\x14\n\x10SPK_SORT_IO_FSYS\x10\x00\x12\x15\n\x11SPK_SORT_IO_CLOUD\x10\x01*;\n\rSpkSortIOmode\x12\x14\n\x10SPK_SORT_IO_SAVE\x10\x00\x12\x14\n\x10SPK_SORT_IO_LOAD\x10\x01*\'\n\nRasterMode\x12\x0c\n\x08\x43HANNELS\x10\x00\x12\x0b\n\x07NEURONS\x10\x01*\x89\x01\n\x0b\x44\x61shElement\x12\x11\n\rENABLED_PORTS\x10\x01\x12\x0b\n\x07GENERAL\x10\x02\x12\x0e\n\nPORT_STATS\x10\x03\x12\x0e\n\nSITE_STATS\x10\x04\x12\x0e\n\nSITE_PANEL\x10\x05\x12\x10\n\x0cNEURON_STATS\x10\x06\x12\x10\n\x0cNEURON_PANEL\x10\x07\x12\x06\n\x02\x41I\x10\x08*u\n\x19SpikeSorterCriterionLevel\x12\x10\n\x0cSORTER_LEAST\x10\x00\x12\x0f\n\x0bSORTER_LESS\x10\x01\x12\x13\n\x0fSORTER_BALANCED\x10\x02\x12\x0f\n\x0bSORTER_MORE\x10\x03\x12\x0f\n\x0bSORTER_MOST\x10\x04*\x84\x01\n\x07SS_STAT\x12\x08\n\x04MEAN\x10\x00\x12\x06\n\x02SD\x10\x01\x12\x08\n\x04MODE\x10\x02\x12\x07\n\x03MIN\x10\x03\x12\x07\n\x03MAX\x10\x04\x12\x0e\n\nMODE_COUNT\x10\x05\x12\n\n\x06MEDIAN\x10\x06\x12\x07\n\x03Q25\x10\x07\x12\x07\n\x03Q75\x10\x08\x12\x08\n\x04SKEW\x10\t\x12\x0c\n\x08KURTOSIS\x10\n\x12\x05\n\x01N\x10\x0b\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11spikesorter.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x12\x62iointerface.proto\"\xe3\x01\n\x18SpikeSorterLaunchRequest\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12&\n\x06source\x18\x02 \x01(\x0b\x32\x16.allego.FileDescriptor\x12\x0c\n\x04seed\x18\x03 \x01(\x03\x12>\n\rfeatureParams\x18\x04 \x01(\x0b\x32\'.allego.SpikeSorterFeatureParamsRequest\x12\x18\n\x10neighborRadiusUm\x18\x05 \x01(\x01\x12\x10\n\x08isAutoOn\x18\t \x01(\x08\x12\x12\n\nnbrPattern\x18\n \x01(\x05\"\xca\x01\n\x19SpikeSorterCommandRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\'\n\x03\x63md\x18\x02 \x02(\x0e\x32\x1a.allego.SpikeSorterCommand\x12-\n\x06subCmd\x18\x03 \x02(\x0e\x32\x1d.allego.SpikeSorterSubCommand\x12>\n\rfeatureParams\x18\x04 \x01(\x0b\x32\'.allego.SpikeSorterFeatureParamsRequest\"\xa7\x01\n\x10SpikeSorterState\x12+\n\x03sys\x18\x01 \x02(\x0e\x32\x1e.allego.SpikeSorterStateSystem\x12\x14\n\x0c\x66racComplete\x18\x02 \x01(\x01\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\x0c\n\x04isOn\x18\x08 \x01(\x08\x12\x1a\n\x12kernelErrorMessage\x18\t \x01(\t\x12\x19\n\x11kernelWarnMessage\x18\n \x01(\t\"\x81\x01\n\x0cSpkSortIOreq\x12#\n\x04type\x18\x01 \x02(\x0e\x32\x15.allego.SpkSortIOtype\x12\'\n\x06target\x18\x02 \x02(\x0e\x32\x17.allego.SpkSortIOtarget\x12#\n\x04mode\x18\x03 \x02(\x0e\x32\x15.allego.SpkSortIOmode\"\x8f\x01\n\x16SpikeSorterLaunchReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12+\n\nsorterType\x18\x02 \x02(\x0e\x32\x17.allego.SpikeSorterType\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12$\n\x04\x64\x65sc\x18\x04 \x01(\x0b\x32\x16.allego.FileDescriptor\"0\n\x16GetSpikeSorterIDsReply\x12\x16\n\x0espikeSorterIDs\x18\x01 \x03(\t\"\xdd\x01\n\x1fSpikeSorterGetRasterDataRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x12\n\ntimeWindow\x18\x03 \x02(\x01\x12\x17\n\x0fplotWidthPoints\x18\x04 \x02(\x01\x12\x13\n\x0b\x63omponentID\x18\x05 \x02(\t\x12\x11\n\ttimeRange\x18\x06 \x03(\x01\x12 \n\x04mode\x18\x07 \x02(\x0e\x32\x12.allego.RasterMode\x12\x13\n\x0blabeledOnly\x18\x08 \x01(\x08\x12\x17\n\x0fprimarySiteOnly\x18\t \x01(\x08\"\x9d\x01\n\x1aSpikeSorterRasterDataReply\x12/\n\x0fspikeTimestamps\x18\x02 \x03(\x0b\x32\x16.allego.SpikeTimestamp\x12\x11\n\ttimeRange\x18\x03 \x03(\x01\x12\x16\n\x0etimeStampRange\x18\x04 \x03(\x03\x12\x10\n\x08GPIOData\x18\x05 \x02(\x0c\x12\x11\n\tGPIOShape\x18\x06 \x03(\x05\"3\n\x1aSpikeSorterStandardRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\"_\n\x1bSpikeSorterDashboardRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12)\n\x0c\x64\x61shElements\x18\x02 \x03(\x0e\x32\x13.allego.DashElement\"\x86\x03\n\x12SpikeSorterDynamic\x12\x11\n\tisEnabled\x18\x01 \x01(\x08\x12\x43\n\x0fupdatePeriodSec\x18\x02 \x01(\x0b\x32*.allego.SpikeSorterDynamic.UpdatePeriodSec\x12\x35\n\x08\x63riteria\x18\x03 \x01(\x0b\x32#.allego.SpikeSorterDynamic.Criteria\x1a\xa0\x01\n\x08\x43riteria\x12\x31\n\x06\x64\x65tect\x18\x01 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x12\x30\n\x05train\x18\x02 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x12/\n\x04sort\x18\x03 \x01(\x0e\x32!.allego.SpikeSorterCriterionLevel\x1a>\n\x0fUpdatePeriodSec\x12\x0e\n\x06\x64\x65tect\x18\x01 \x01(\x01\x12\r\n\x05train\x18\x02 \x01(\x01\x12\x0c\n\x04sort\x18\x03 \x01(\x01\"\xc5\x01\n\x1cSpikeSorterSetDynamicRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x42\n\x07variant\x18\x02 \x03(\x0b\x32\x31.allego.SpikeSorterSetDynamicRequest.VariantEntry\x1aJ\n\x0cVariantEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.allego.SpikeSorterDynamic:\x02\x38\x01\"\xd8\x01\n\x1aSpikeSorterGetDynamicReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x15\n\rrootVariantID\x18\x02 \x02(\t\x12@\n\x07variant\x18\x03 \x03(\x0b\x32/.allego.SpikeSorterGetDynamicReply.VariantEntry\x1aJ\n\x0cVariantEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.allego.SpikeSorterDynamic:\x02\x38\x01\"l\n\x1fGetSpikeSorterParamCommandReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x32\n\x03rec\x18\x02 \x03(\x0b\x32%.allego.SpikeSorterParamCommandRecord\"3\n\x12\x43lusterMapOutliers\x12\x0c\n\x04mild\x18\x01 \x03(\x01\x12\x0f\n\x07\x65xtreme\x18\x02 \x03(\x01\"9\n\x13\x43lusterMapQuartiles\x12\n\n\x02q1\x18\x01 \x02(\x01\x12\n\n\x02q2\x18\x02 \x02(\x01\x12\n\n\x02q3\x18\x03 \x02(\x01\"\x83\x01\n\x0f\x43lusterMapStats\x12\x16\n\x0e\x63\x65ntroidCenter\x18\x01 \x03(\x01\x12\x12\n\ncentroidSd\x18\x02 \x03(\x01\x12\x16\n\x0e\x63\x65ntroidSdNorm\x18\x03 \x02(\x01\x12\x19\n\x11intraCentroidDist\x18\x04 \x03(\x01\x12\x11\n\tnumSpikes\x18\x05 \x02(\x03\"f\n\x10\x43lusterMapRecord\x12\r\n\x05label\x18\x01 \x02(\x05\x12&\n\x05stats\x18\x03 \x02(\x0b\x32\x17.allego.ClusterMapStats\x12\x1b\n\x13numSpikesTrainCache\x18\x04 \x02(\x03\"\xa8\x01\n\x13SpikeSortSiteStatus\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x15\n\rorderedLabels\x18\x02 \x03(\x05\x12)\n\x07\x63luster\x18\x03 \x03(\x0b\x32\x18.allego.ClusterMapRecord\x12\x11\n\tnumSpikes\x18\x04 \x03(\x03\x12\x0c\n\x04zeta\x18\x05 \x03(\x01\x12\x1a\n\x12\x61ggregateSpikeRate\x18\x06 \x02(\x01\"\x8f\x01\n\x14SpikeSortPhaseStatus\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x12\n\nchunkIndex\x18\x02 \x02(\x03\x12\x14\n\x0cupdatePeriod\x18\x03 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\x04 \x02(\x01\x12\x12\n\nisComplete\x18\x05 \x02(\x08\x12\x18\n\x10\x66ractionComplete\x18\x06 \x02(\x01\"*\n\x13SpikeSortNbrIdxList\x12\x13\n\x0bntvChanIdxs\x18\x01 \x03(\x05\"\xf2\x02\n\x16SpikeSorterStatusReply\x12\'\n\x05state\x18\x01 \x02(\x0b\x32\x18.allego.SpikeSorterState\x12\x16\n\x0e\x62iointerfaceID\x18\x03 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x04 \x02(\t\x12\x10\n\x08sampFreq\x18\x05 \x02(\x01\x12\x19\n\x11\x65nabledNtvChanIdx\x18\x06 \x03(\x05\x12+\n\x05phase\x18\x07 \x03(\x0b\x32\x1c.allego.SpikeSortPhaseStatus\x12\x30\n\x0b\x65nabledSite\x18\x08 \x03(\x0b\x32\x1b.allego.SpikeSortSiteStatus\x12\x12\n\nprobeYield\x18\t \x02(\x01\x12\x11\n\tsortStats\x18\n \x03(\x01\x12\x1b\n\x13\x64\x61tasourceTimeRange\x18\x0c \x03(\x01\x12\x1d\n\x15\x62iointerfaceTimeRange\x18\r \x03(\x01\x12\x12\n\nnumNeurons\x18\x0f \x02(\x03\"R\n\x1eSpikeSorterStatusVariantsReply\x12\x30\n\x08variants\x18\x01 \x03(\x0b\x32\x1e.allego.SpikeSorterStatusReply\"\xfd\x02\n\x19SpikeSorterClassifierSpec\x12\r\n\x05\x61lpha\x18\x01 \x02(\x01\x12\x11\n\talphaBias\x18\x02 \x02(\x01\x12\x16\n\x0e\x64imOutputLayer\x18\x03 \x02(\x05\x12\x16\n\x0e\x65rrorTolerance\x18\x04 \x02(\x01\x12\x19\n\x11hiddenLayerFactor\x18\x05 \x02(\x01\x12\n\n\x02iD\x18\x06 \x02(\t\x12\x16\n\x0einitBiasStdDev\x18\x07 \x02(\x01\x12\x18\n\x10initWeightStdDev\x18\x08 \x02(\x01\x12\x11\n\tisMasking\x18\t \x02(\x08\x12\x10\n\x08l1lambda\x18\n \x02(\x01\x12\x15\n\rminibatchSize\x18\x0b \x02(\x05\x12\x15\n\rmaxNumSamples\x18\x0c \x02(\x05\x12\x11\n\tnumEpochs\x18\r \x02(\x05\x12\x19\n\x11numSamplesTestMSE\x18\x0e \x02(\x05\x12\x1b\n\x13numConcurrentModels\x18\x0f \x02(\x05\x12\x17\n\x0flabelNoiseLevel\x18\x10 \x02(\x01\"u\n\x16SpikeSorterVariantSpec\x12\n\n\x02iD\x18\x01 \x02(\t\x12\x14\n\x0csiteConfigID\x18\x02 \x02(\t\x12\x39\n\x0e\x63lassifierSpec\x18\x03 \x02(\x0b\x32!.allego.SpikeSorterClassifierSpec\"\xcc\x01\n\x0fSpikeSorterSpec\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x02 \x02(\t\x12\x16\n\x0e\x62iointerfaceID\x18\x03 \x02(\t\x12\x1b\n\x13maxNumSiteNeighbors\x18\x04 \x02(\x05\x12\x18\n\x10neighborRadiusUm\x18\x05 \x02(\x01\x12/\n\x07variant\x18\x06 \x03(\x0b\x32\x1e.allego.SpikeSorterVariantSpec\x12\x0c\n\x04seed\x18\x08 \x02(\x03\"\xc2\x01\n\x19SpikeSorterGetConfigReply\x12%\n\x04spec\x18\x01 \x02(\x0b\x32\x17.allego.SpikeSorterSpec\x12\x16\n\x0e\x61IupdatePeriod\x18\x02 \x02(\x01\x12\x19\n\x11orderedVariantIDs\x18\x03 \x03(\t\x12\x15\n\rrootVariantID\x18\x04 \x02(\t\x12\x34\n\x0csorterStatus\x18\x06 \x03(\x0b\x32\x1e.allego.SpikeSorterStatusReply\"\x90\x02\n\x15SpikeSorterVizRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12\x11\n\tvariantID\x18\x02 \x02(\t\x12\x12\n\nntvChanIdx\x18\x03 \x03(\x05\x12\x13\n\x0bspikeLabels\x18\x04 \x03(\x05\x12\x34\n\x07vizType\x18\x05 \x02(\x0e\x32#.allego.SpikeSorterVizRequest.VType\x12\x14\n\x0cisYAutoScale\x18\x06 \x02(\x08\x12\x0c\n\x04yLim\x18\x07 \x03(\x01\x12\x0e\n\x06\x66igDir\x18\x08 \x02(\t\x12\x11\n\tnumSpikes\x18\t \x02(\x05\"\'\n\x05VType\x12\x1e\n\x1aVIZ_SPIKESORT_TRAIN_SPIKES\x10\x00\"\xb5\x01\n\x1fSpikeSorterFeatureParamsRequest\x12\x13\n\x0bnumFeatures\x18\x01 \x02(\x05\x12\x18\n\x10posInfluenceFrac\x18\x02 \x02(\x01\x12\x1d\n\x15wfmShapeInfluenceFrac\x18\x03 \x02(\x01\x12-\n\x0b\x66\x65\x61tureType\x18\x04 \x01(\x0e\x32\x18.allego.InputFeatureType\x12\x15\n\rclusteringDim\x18\x05 \x01(\x05\"\xcb\x01\n\x1dSpikeSorterFeatureParamsReply\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12-\n\x0b\x66\x65\x61tureType\x18\x02 \x02(\x0e\x32\x18.allego.InputFeatureType\x12\x16\n\x0emaxNumFeatures\x18\x03 \x02(\x05\x12\x13\n\x0bnumFeatures\x18\x04 \x02(\x05\x12\x18\n\x10posInfluenceFrac\x18\x05 \x02(\x02\x12\x1d\n\x15wfmShapeInfluenceFrac\x18\x06 \x02(\x02\"\xb6\x05\n\x19SpikeSorterDashboardReply\x12\"\n\x0c\x65nabledPorts\x18\x01 \x03(\x0e\x32\x0c.allego.Port\x12\x37\n\x07general\x18\x02 \x01(\x0b\x32&.allego.SpikeSorterDashboardGeneralRec\x12\x33\n\tsiteStats\x18\x03 \x01(\x0b\x32 .allego.IndicoDashboardSiteStats\x12\x43\n\tportStats\x18\x04 \x03(\x0b\x32\x30.allego.SpikeSorterDashboardReply.PortStatsEntry\x12\x43\n\tsitePanel\x18\x05 \x03(\x0b\x32\x30.allego.SpikeSorterDashboardReply.SitePanelEntry\x12G\n\x0bneuronPanel\x18\x06 \x03(\x0b\x32\x32.allego.SpikeSorterDashboardReply.NeuronPanelEntry\x12*\n\x02\x61I\x18\x07 \x01(\x0b\x32\x1e.allego.SpikeSorterDashboardAI\x1aR\n\x0ePortStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .allego.IndicoDashboardPortStats:\x02\x38\x01\x1aW\n\x0eSitePanelEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.allego.IndicoDashboardSiteIndicators:\x02\x38\x01\x1a[\n\x10NeuronPanelEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.allego.IndicoDashboardNeuronIndicators:\x02\x38\x01\"\xac\x03\n\x1eSpikeSorterDashboardGeneralRec\x12\'\n\x05state\x18\x01 \x02(\x0b\x32\x18.allego.SpikeSorterState\x12+\n\nsorterType\x18\x02 \x02(\x0e\x32\x17.allego.SpikeSorterType\x12\x10\n\x08sorterID\x18\x03 \x02(\t\x12\x14\n\x0c\x64\x61tasourceID\x18\x04 \x02(\t\x12\x11\n\ttimeRange\x18\x05 \x03(\x01\x12\x15\n\rnumTotalSites\x18\x06 \x02(\x03\x12\x17\n\x0fnumEnabledSites\x18\x07 \x02(\x03\x12\x16\n\x0enumActiveSites\x18\x08 \x02(\x03\x12\x12\n\nnumNeurons\x18\t \x02(\x03\x12\x12\n\nprobeYield\x18\n \x02(\x01\x12\x11\n\tsiteYield\x18\x0b \x02(\x01\x12\x1a\n\x12numSpikesProcessed\x18\x0c \x02(\x03\x12\x18\n\x10numSpikesLabeled\x18\r \x02(\x03\x12\x16\n\x0esortEfficiency\x18\x0e \x02(\x01\x12(\n\x08sinkDesc\x18\x0f \x02(\x0b\x32\x16.allego.FileDescriptor\"\xd5\x01\n\x16SpikeSorterDashboardAI\x12\x0c\n\x04\x62\x65ta\x18\x01 \x02(\x01\x12\"\n\x1a\x65stimatedReaderCompleteSec\x18\x02 \x02(\x01\x12\x1a\n\x12interSessionDurSec\x18\x03 \x02(\x01\x12\x19\n\x11interSessionStart\x18\x04 \x02(\t\x12\x15\n\rsessionDurSec\x18\x05 \x02(\x01\x12\x14\n\x0csessionStart\x18\x06 \x02(\t\x12\x12\n\nsessionIdx\x18\x07 \x02(\x03\x12\x11\n\tstartTime\x18\x08 \x02(\t\"_\n\x18IndicoDashboardSiteStats\x12\x0b\n\x03snr\x18\x01 \x03(\x01\x12\r\n\x05noise\x18\x02 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x03 \x03(\x01\x12\x12\n\nnumNeurons\x18\x04 \x02(\x03\"\x90\x01\n\x18IndicoDashboardPortStats\x12\x0b\n\x03snr\x18\x01 \x03(\x01\x12\r\n\x05noise\x18\x02 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x03 \x03(\x01\x12\x16\n\x0esortEfficiency\x18\x04 \x02(\x01\x12\x17\n\x0fnumEnabledSites\x18\x05 \x02(\x03\x12\x12\n\nnumNeurons\x18\x06 \x02(\x03\"\xd9\x01\n\x1dIndicoDashboardSiteIndicators\x12\x12\n\nntvChanIdx\x18\x01 \x03(\x05\x12\x0b\n\x03snr\x18\x02 \x03(\x01\x12\r\n\x05noise\x18\x03 \x03(\x01\x12\x13\n\x0bneuronYield\x18\x04 \x03(\x01\x12\x16\n\x0esortEfficiency\x18\x05 \x03(\x01\x12\x11\n\tspikeRate\x18\x06 \x03(\x01\x12\x11\n\tposProbeX\x18\x07 \x03(\x01\x12\x11\n\tposProbeY\x18\x08 \x03(\x01\x12\x11\n\tposProbeZ\x18\t \x03(\x01\x12\x0f\n\x07siteNum\x18\n \x03(\x05\"\xb1\x01\n\x1fIndicoDashboardNeuronIndicators\x12\x10\n\x08neuronID\x18\x01 \x03(\t\x12\x0b\n\x03snr\x18\x02 \x03(\x01\x12\x11\n\tspikeRate\x18\x03 \x03(\x01\x12\x11\n\tposProbeX\x18\x04 \x03(\x01\x12\x11\n\tposProbeY\x18\x05 \x03(\x01\x12\x11\n\tposProbeZ\x18\x06 \x03(\x01\x12\x0f\n\x07siteNum\x18\x07 \x03(\x05\x12\x12\n\nspikeLabel\x18\x08 \x03(\x05\"\xa7\x02\n\x1cSpikeSorterDashboardSiteDesc\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x10\n\x08posProbe\x18\x03 \x03(\x01\x12\x10\n\x08posBrain\x18\x04 \x03(\x01\x12\x0e\n\x06snrMax\x18\x05 \x02(\x01\x12\x0e\n\x06snrMin\x18\x06 \x02(\x01\x12\x12\n\nnoiseLevel\x18\x07 \x02(\x01\x12\x12\n\nnumNeurons\x18\x08 \x02(\x03\x12/\n\rindicoCluster\x18\n \x03(\x0b\x32\x18.allego.ClusterMapRecord\x12\x1c\n\x14pileWaveformMinValue\x18\r \x02(\x02\x12\x1c\n\x14pileWaveformMaxValue\x18\x0e \x02(\x02\"\xd2\x01\n\x1eSpikeSorterDashboardNeuronDesc\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12&\n\x04\x64\x65sc\x18\x02 \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x0b\n\x03snr\x18\x05 \x02(\x01\x12\x0f\n\x07IsihMax\x18\x06 \x02(\x01\x12\x15\n\rIsihArgmaxSec\x18\x07 \x02(\x01\x12\x15\n\rIsihArgmaxIdx\x18\x08 \x02(\x03\x12\x10\n\x08IsihMean\x18\t \x02(\x01\x12\x0e\n\x06IsihSd\x18\n \x02(\x01\"\xfa\x01\n SpikeSorterDashboardNeuronDetail\x12&\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x18.allego.NeuronDescriptor\x12\x18\n\x10templateWaveform\x18\x02 \x03(\x02\x12\x1a\n\x12templateSdWaveform\x18\x03 \x03(\x02\x12\x18\n\x10pileWaveformData\x18\x04 \x03(\x02\x12\x1e\n\x16numSamplesPileWaveform\x18\x05 \x02(\x05\x12\x18\n\x10numPileWaveforms\x18\x06 \x02(\x05\x12$\n\x04isih\x18\x0b \x02(\x0b\x32\x16.allego.NeuronHistData\"\xa9\x01\n\x1eSpikeSorterDashboardSiteDetail\x12\x32\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32$.allego.SpikeSorterDashboardSiteDesc\x12\x19\n\x11orderedSpikeLabel\x18\x02 \x03(\x05\x12\x38\n\x06neuron\x18\x03 \x03(\x0b\x32(.allego.SpikeSorterDashboardNeuronDetail*\x80\x01\n\x0fSpikeSorterType\x12\x0f\n\x0bSORTER_NULL\x10\x00\x12\x15\n\x11SORTER_VEX_STREAM\x10\x01\x12\x18\n\x14SORTER_SPIKES_STREAM\x10\x02\x12\x13\n\x0fSORTER_VEX_FILE\x10\x03\x12\x16\n\x12SORTER_SPIKES_FILE\x10\x04*\x82\x01\n\x12SpikeSorterCommand\x12\x11\n\rSORTER_CMD_ON\x10\x00\x12\x12\n\x0eSORTER_CMD_OFF\x10\x01\x12\x19\n\x15SORTER_CMD_CLEAR_SORT\x10\x02\x12\x15\n\x11SORTER_CMD_REBASE\x10\x04\x12\x13\n\x0fSORTER_CMD_INIT\x10\x05*/\n\x15SpikeSorterSubCommand\x12\x16\n\x12SORTER_SUBCMD_NULL\x10\x00*@\n\x0fSpikeSorterMode\x12\x16\n\x12SORTER_MODE_STREAM\x10\x00\x12\x15\n\x11SORTER_MODE_BATCH\x10\x01*8\n\x10\x44\x65\x63InputFeatures\x12\x11\n\rALL_NEIGHBORS\x10\x00\x12\x11\n\rSVD_NEIGHBORS\x10\x01*I\n\x16SpikeSorterStateSystem\x12\n\n\x06SYS_ON\x10\x00\x12\x0b\n\x07SYS_OFF\x10\x01\x12\x16\n\x12SYS_NOT_CONFIGURED\x10\x02*f\n\rSpkSortIOtype\x12\x17\n\x13SPK_SORT_IO_NETWORK\x10\x00\x12\x17\n\x13SPK_SORT_IO_TRAINER\x10\x01\x12#\n\x1fSPK_SORT_IO_NETWORK_AND_TRAINER\x10\x02*>\n\x0fSpkSortIOtarget\x12\x14\n\x10SPK_SORT_IO_FSYS\x10\x00\x12\x15\n\x11SPK_SORT_IO_CLOUD\x10\x01*;\n\rSpkSortIOmode\x12\x14\n\x10SPK_SORT_IO_SAVE\x10\x00\x12\x14\n\x10SPK_SORT_IO_LOAD\x10\x01*\'\n\nRasterMode\x12\x0c\n\x08\x43HANNELS\x10\x00\x12\x0b\n\x07NEURONS\x10\x01*\x89\x01\n\x0b\x44\x61shElement\x12\x11\n\rENABLED_PORTS\x10\x01\x12\x0b\n\x07GENERAL\x10\x02\x12\x0e\n\nPORT_STATS\x10\x03\x12\x0e\n\nSITE_STATS\x10\x04\x12\x0e\n\nSITE_PANEL\x10\x05\x12\x10\n\x0cNEURON_STATS\x10\x06\x12\x10\n\x0cNEURON_PANEL\x10\x07\x12\x06\n\x02\x41I\x10\x08*u\n\x19SpikeSorterCriterionLevel\x12\x10\n\x0cSORTER_LEAST\x10\x00\x12\x0f\n\x0bSORTER_LESS\x10\x01\x12\x13\n\x0fSORTER_BALANCED\x10\x02\x12\x0f\n\x0bSORTER_MORE\x10\x03\x12\x0f\n\x0bSORTER_MOST\x10\x04*\x84\x01\n\x07SS_STAT\x12\x08\n\x04MEAN\x10\x00\x12\x06\n\x02SD\x10\x01\x12\x08\n\x04MODE\x10\x02\x12\x07\n\x03MIN\x10\x03\x12\x07\n\x03MAX\x10\x04\x12\x0e\n\nMODE_COUNT\x10\x05\x12\n\n\x06MEDIAN\x10\x06\x12\x07\n\x03Q25\x10\x07\x12\x07\n\x03Q75\x10\x08\x12\x08\n\x04SKEW\x10\t\x12\x0c\n\x08KURTOSIS\x10\n\x12\x05\n\x01N\x10\x0b*5\n\x10InputFeatureType\x12\x10\n\x0c\x46TR_TYPE_WFM\x10\x01\x12\x0f\n\x0b\x46TR_TYPE_SP\x10\x02\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spikesorter_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
@@ -29,128 +29,134 @@
   _SPIKESORTERGETDYNAMICREPLY_VARIANTENTRY._serialized_options = b'8\001'
   _SPIKESORTERDASHBOARDREPLY_PORTSTATSENTRY._options = None
   _SPIKESORTERDASHBOARDREPLY_PORTSTATSENTRY._serialized_options = b'8\001'
   _SPIKESORTERDASHBOARDREPLY_SITEPANELENTRY._options = None
   _SPIKESORTERDASHBOARDREPLY_SITEPANELENTRY._serialized_options = b'8\001'
   _SPIKESORTERDASHBOARDREPLY_NEURONPANELENTRY._options = None
   _SPIKESORTERDASHBOARDREPLY_NEURONPANELENTRY._serialized_options = b'8\001'
-  _SPIKESORTERTYPE._serialized_start=7694
-  _SPIKESORTERTYPE._serialized_end=7822
-  _SPIKESORTERCOMMAND._serialized_start=7825
-  _SPIKESORTERCOMMAND._serialized_end=8001
-  _SPIKESORTERSUBCOMMAND._serialized_start=8003
-  _SPIKESORTERSUBCOMMAND._serialized_end=8050
-  _SPIKESORTERMODE._serialized_start=8052
-  _SPIKESORTERMODE._serialized_end=8116
-  _DECINPUTFEATURES._serialized_start=8118
-  _DECINPUTFEATURES._serialized_end=8174
-  _SPIKESORTERSTATESYSTEM._serialized_start=8176
-  _SPIKESORTERSTATESYSTEM._serialized_end=8249
-  _SPKSORTIOTYPE._serialized_start=8251
-  _SPKSORTIOTYPE._serialized_end=8353
-  _SPKSORTIOTARGET._serialized_start=8355
-  _SPKSORTIOTARGET._serialized_end=8417
-  _SPKSORTIOMODE._serialized_start=8419
-  _SPKSORTIOMODE._serialized_end=8478
-  _RASTERMODE._serialized_start=8480
-  _RASTERMODE._serialized_end=8519
-  _DASHELEMENT._serialized_start=8522
-  _DASHELEMENT._serialized_end=8659
-  _SPIKESORTERCRITERIONLEVEL._serialized_start=8661
-  _SPIKESORTERCRITERIONLEVEL._serialized_end=8778
-  _SS_STAT._serialized_start=8781
-  _SS_STAT._serialized_end=8913
+  _SPIKESORTERTYPE._serialized_start=8117
+  _SPIKESORTERTYPE._serialized_end=8245
+  _SPIKESORTERCOMMAND._serialized_start=8248
+  _SPIKESORTERCOMMAND._serialized_end=8378
+  _SPIKESORTERSUBCOMMAND._serialized_start=8380
+  _SPIKESORTERSUBCOMMAND._serialized_end=8427
+  _SPIKESORTERMODE._serialized_start=8429
+  _SPIKESORTERMODE._serialized_end=8493
+  _DECINPUTFEATURES._serialized_start=8495
+  _DECINPUTFEATURES._serialized_end=8551
+  _SPIKESORTERSTATESYSTEM._serialized_start=8553
+  _SPIKESORTERSTATESYSTEM._serialized_end=8626
+  _SPKSORTIOTYPE._serialized_start=8628
+  _SPKSORTIOTYPE._serialized_end=8730
+  _SPKSORTIOTARGET._serialized_start=8732
+  _SPKSORTIOTARGET._serialized_end=8794
+  _SPKSORTIOMODE._serialized_start=8796
+  _SPKSORTIOMODE._serialized_end=8855
+  _RASTERMODE._serialized_start=8857
+  _RASTERMODE._serialized_end=8896
+  _DASHELEMENT._serialized_start=8899
+  _DASHELEMENT._serialized_end=9036
+  _SPIKESORTERCRITERIONLEVEL._serialized_start=9038
+  _SPIKESORTERCRITERIONLEVEL._serialized_end=9155
+  _SS_STAT._serialized_start=9158
+  _SS_STAT._serialized_end=9290
+  _INPUTFEATURETYPE._serialized_start=9292
+  _INPUTFEATURETYPE._serialized_end=9345
   _SPIKESORTERLAUNCHREQUEST._serialized_start=64
-  _SPIKESORTERLAUNCHREQUEST._serialized_end=227
-  _SPIKESORTERCOMMANDREQUEST._serialized_start=230
-  _SPIKESORTERCOMMANDREQUEST._serialized_end=368
-  _SPIKESORTERSTATE._serialized_start=371
-  _SPIKESORTERSTATE._serialized_end=633
-  _SPKSORTIOREQ._serialized_start=636
-  _SPKSORTIOREQ._serialized_end=765
-  _SPIKESORTERLAUNCHREPLY._serialized_start=768
-  _SPIKESORTERLAUNCHREPLY._serialized_end=911
-  _GETSPIKESORTERIDSREPLY._serialized_start=913
-  _GETSPIKESORTERIDSREPLY._serialized_end=961
-  _SPIKESORTERGETRASTERDATAREQUEST._serialized_start=964
-  _SPIKESORTERGETRASTERDATAREQUEST._serialized_end=1185
-  _SPIKESORTERRASTERDATAREPLY._serialized_start=1188
-  _SPIKESORTERRASTERDATAREPLY._serialized_end=1345
-  _SPIKESORTERSTANDARDREQUEST._serialized_start=1347
-  _SPIKESORTERSTANDARDREQUEST._serialized_end=1398
-  _SPIKESORTERDASHBOARDREQUEST._serialized_start=1400
-  _SPIKESORTERDASHBOARDREQUEST._serialized_end=1495
-  _SPIKESORTERDYNAMIC._serialized_start=1498
-  _SPIKESORTERDYNAMIC._serialized_end=1888
-  _SPIKESORTERDYNAMIC_CRITERIA._serialized_start=1664
-  _SPIKESORTERDYNAMIC_CRITERIA._serialized_end=1824
-  _SPIKESORTERDYNAMIC_UPDATEPERIODSEC._serialized_start=1826
-  _SPIKESORTERDYNAMIC_UPDATEPERIODSEC._serialized_end=1888
-  _SPIKESORTERSETDYNAMICREQUEST._serialized_start=1891
-  _SPIKESORTERSETDYNAMICREQUEST._serialized_end=2088
-  _SPIKESORTERSETDYNAMICREQUEST_VARIANTENTRY._serialized_start=2014
-  _SPIKESORTERSETDYNAMICREQUEST_VARIANTENTRY._serialized_end=2088
-  _SPIKESORTERGETDYNAMICREPLY._serialized_start=2091
-  _SPIKESORTERGETDYNAMICREPLY._serialized_end=2307
-  _SPIKESORTERGETDYNAMICREPLY_VARIANTENTRY._serialized_start=2014
-  _SPIKESORTERGETDYNAMICREPLY_VARIANTENTRY._serialized_end=2088
-  _GETSPIKESORTERPARAMCOMMANDREPLY._serialized_start=2309
-  _GETSPIKESORTERPARAMCOMMANDREPLY._serialized_end=2417
-  _CLUSTERMAPOUTLIERS._serialized_start=2419
-  _CLUSTERMAPOUTLIERS._serialized_end=2470
-  _CLUSTERMAPQUARTILES._serialized_start=2472
-  _CLUSTERMAPQUARTILES._serialized_end=2529
-  _CLUSTERMAPSTATS._serialized_start=2532
-  _CLUSTERMAPSTATS._serialized_end=2663
-  _CLUSTERMAPRECORD._serialized_start=2665
-  _CLUSTERMAPRECORD._serialized_end=2767
-  _SPIKESORTSITESTATUS._serialized_start=2770
-  _SPIKESORTSITESTATUS._serialized_end=2938
-  _SPIKESORTPHASESTATUS._serialized_start=2941
-  _SPIKESORTPHASESTATUS._serialized_end=3084
-  _SPIKESORTNBRIDXLIST._serialized_start=3086
-  _SPIKESORTNBRIDXLIST._serialized_end=3128
-  _SPIKESORTERSTATUSREPLY._serialized_start=3131
-  _SPIKESORTERSTATUSREPLY._serialized_end=3501
-  _SPIKESORTERSTATUSVARIANTSREPLY._serialized_start=3503
-  _SPIKESORTERSTATUSVARIANTSREPLY._serialized_end=3585
-  _SPIKESORTERCLASSIFIERSPEC._serialized_start=3588
-  _SPIKESORTERCLASSIFIERSPEC._serialized_end=3969
-  _SPIKESORTERVARIANTSPEC._serialized_start=3971
-  _SPIKESORTERVARIANTSPEC._serialized_end=4088
-  _SPIKESORTERSPEC._serialized_start=4091
-  _SPIKESORTERSPEC._serialized_end=4295
-  _SPIKESORTERGETCONFIGREPLY._serialized_start=4298
-  _SPIKESORTERGETCONFIGREPLY._serialized_end=4492
-  _SPIKESORTERVIZREQUEST._serialized_start=4495
-  _SPIKESORTERVIZREQUEST._serialized_end=4767
-  _SPIKESORTERVIZREQUEST_VTYPE._serialized_start=4728
-  _SPIKESORTERVIZREQUEST_VTYPE._serialized_end=4767
-  _SPIKESORTERDASHBOARDREPLY._serialized_start=4770
-  _SPIKESORTERDASHBOARDREPLY._serialized_end=5464
-  _SPIKESORTERDASHBOARDREPLY_PORTSTATSENTRY._serialized_start=5200
-  _SPIKESORTERDASHBOARDREPLY_PORTSTATSENTRY._serialized_end=5282
-  _SPIKESORTERDASHBOARDREPLY_SITEPANELENTRY._serialized_start=5284
-  _SPIKESORTERDASHBOARDREPLY_SITEPANELENTRY._serialized_end=5371
-  _SPIKESORTERDASHBOARDREPLY_NEURONPANELENTRY._serialized_start=5373
-  _SPIKESORTERDASHBOARDREPLY_NEURONPANELENTRY._serialized_end=5464
-  _SPIKESORTERDASHBOARDGENERALREC._serialized_start=5467
-  _SPIKESORTERDASHBOARDGENERALREC._serialized_end=5895
-  _SPIKESORTERDASHBOARDAI._serialized_start=5898
-  _SPIKESORTERDASHBOARDAI._serialized_end=6111
-  _INDICODASHBOARDSITESTATS._serialized_start=6113
-  _INDICODASHBOARDSITESTATS._serialized_end=6208
-  _INDICODASHBOARDPORTSTATS._serialized_start=6211
-  _INDICODASHBOARDPORTSTATS._serialized_end=6355
-  _INDICODASHBOARDSITEINDICATORS._serialized_start=6358
-  _INDICODASHBOARDSITEINDICATORS._serialized_end=6575
-  _INDICODASHBOARDNEURONINDICATORS._serialized_start=6578
-  _INDICODASHBOARDNEURONINDICATORS._serialized_end=6755
-  _SPIKESORTERDASHBOARDSITEDESC._serialized_start=6758
-  _SPIKESORTERDASHBOARDSITEDESC._serialized_end=7053
-  _SPIKESORTERDASHBOARDNEURONDESC._serialized_start=7056
-  _SPIKESORTERDASHBOARDNEURONDESC._serialized_end=7266
-  _SPIKESORTERDASHBOARDNEURONDETAIL._serialized_start=7269
-  _SPIKESORTERDASHBOARDNEURONDETAIL._serialized_end=7519
-  _SPIKESORTERDASHBOARDSITEDETAIL._serialized_start=7522
-  _SPIKESORTERDASHBOARDSITEDETAIL._serialized_end=7691
+  _SPIKESORTERLAUNCHREQUEST._serialized_end=291
+  _SPIKESORTERCOMMANDREQUEST._serialized_start=294
+  _SPIKESORTERCOMMANDREQUEST._serialized_end=496
+  _SPIKESORTERSTATE._serialized_start=499
+  _SPIKESORTERSTATE._serialized_end=666
+  _SPKSORTIOREQ._serialized_start=669
+  _SPKSORTIOREQ._serialized_end=798
+  _SPIKESORTERLAUNCHREPLY._serialized_start=801
+  _SPIKESORTERLAUNCHREPLY._serialized_end=944
+  _GETSPIKESORTERIDSREPLY._serialized_start=946
+  _GETSPIKESORTERIDSREPLY._serialized_end=994
+  _SPIKESORTERGETRASTERDATAREQUEST._serialized_start=997
+  _SPIKESORTERGETRASTERDATAREQUEST._serialized_end=1218
+  _SPIKESORTERRASTERDATAREPLY._serialized_start=1221
+  _SPIKESORTERRASTERDATAREPLY._serialized_end=1378
+  _SPIKESORTERSTANDARDREQUEST._serialized_start=1380
+  _SPIKESORTERSTANDARDREQUEST._serialized_end=1431
+  _SPIKESORTERDASHBOARDREQUEST._serialized_start=1433
+  _SPIKESORTERDASHBOARDREQUEST._serialized_end=1528
+  _SPIKESORTERDYNAMIC._serialized_start=1531
+  _SPIKESORTERDYNAMIC._serialized_end=1921
+  _SPIKESORTERDYNAMIC_CRITERIA._serialized_start=1697
+  _SPIKESORTERDYNAMIC_CRITERIA._serialized_end=1857
+  _SPIKESORTERDYNAMIC_UPDATEPERIODSEC._serialized_start=1859
+  _SPIKESORTERDYNAMIC_UPDATEPERIODSEC._serialized_end=1921
+  _SPIKESORTERSETDYNAMICREQUEST._serialized_start=1924
+  _SPIKESORTERSETDYNAMICREQUEST._serialized_end=2121
+  _SPIKESORTERSETDYNAMICREQUEST_VARIANTENTRY._serialized_start=2047
+  _SPIKESORTERSETDYNAMICREQUEST_VARIANTENTRY._serialized_end=2121
+  _SPIKESORTERGETDYNAMICREPLY._serialized_start=2124
+  _SPIKESORTERGETDYNAMICREPLY._serialized_end=2340
+  _SPIKESORTERGETDYNAMICREPLY_VARIANTENTRY._serialized_start=2047
+  _SPIKESORTERGETDYNAMICREPLY_VARIANTENTRY._serialized_end=2121
+  _GETSPIKESORTERPARAMCOMMANDREPLY._serialized_start=2342
+  _GETSPIKESORTERPARAMCOMMANDREPLY._serialized_end=2450
+  _CLUSTERMAPOUTLIERS._serialized_start=2452
+  _CLUSTERMAPOUTLIERS._serialized_end=2503
+  _CLUSTERMAPQUARTILES._serialized_start=2505
+  _CLUSTERMAPQUARTILES._serialized_end=2562
+  _CLUSTERMAPSTATS._serialized_start=2565
+  _CLUSTERMAPSTATS._serialized_end=2696
+  _CLUSTERMAPRECORD._serialized_start=2698
+  _CLUSTERMAPRECORD._serialized_end=2800
+  _SPIKESORTSITESTATUS._serialized_start=2803
+  _SPIKESORTSITESTATUS._serialized_end=2971
+  _SPIKESORTPHASESTATUS._serialized_start=2974
+  _SPIKESORTPHASESTATUS._serialized_end=3117
+  _SPIKESORTNBRIDXLIST._serialized_start=3119
+  _SPIKESORTNBRIDXLIST._serialized_end=3161
+  _SPIKESORTERSTATUSREPLY._serialized_start=3164
+  _SPIKESORTERSTATUSREPLY._serialized_end=3534
+  _SPIKESORTERSTATUSVARIANTSREPLY._serialized_start=3536
+  _SPIKESORTERSTATUSVARIANTSREPLY._serialized_end=3618
+  _SPIKESORTERCLASSIFIERSPEC._serialized_start=3621
+  _SPIKESORTERCLASSIFIERSPEC._serialized_end=4002
+  _SPIKESORTERVARIANTSPEC._serialized_start=4004
+  _SPIKESORTERVARIANTSPEC._serialized_end=4121
+  _SPIKESORTERSPEC._serialized_start=4124
+  _SPIKESORTERSPEC._serialized_end=4328
+  _SPIKESORTERGETCONFIGREPLY._serialized_start=4331
+  _SPIKESORTERGETCONFIGREPLY._serialized_end=4525
+  _SPIKESORTERVIZREQUEST._serialized_start=4528
+  _SPIKESORTERVIZREQUEST._serialized_end=4800
+  _SPIKESORTERVIZREQUEST_VTYPE._serialized_start=4761
+  _SPIKESORTERVIZREQUEST_VTYPE._serialized_end=4800
+  _SPIKESORTERFEATUREPARAMSREQUEST._serialized_start=4803
+  _SPIKESORTERFEATUREPARAMSREQUEST._serialized_end=4984
+  _SPIKESORTERFEATUREPARAMSREPLY._serialized_start=4987
+  _SPIKESORTERFEATUREPARAMSREPLY._serialized_end=5190
+  _SPIKESORTERDASHBOARDREPLY._serialized_start=5193
+  _SPIKESORTERDASHBOARDREPLY._serialized_end=5887
+  _SPIKESORTERDASHBOARDREPLY_PORTSTATSENTRY._serialized_start=5623
+  _SPIKESORTERDASHBOARDREPLY_PORTSTATSENTRY._serialized_end=5705
+  _SPIKESORTERDASHBOARDREPLY_SITEPANELENTRY._serialized_start=5707
+  _SPIKESORTERDASHBOARDREPLY_SITEPANELENTRY._serialized_end=5794
+  _SPIKESORTERDASHBOARDREPLY_NEURONPANELENTRY._serialized_start=5796
+  _SPIKESORTERDASHBOARDREPLY_NEURONPANELENTRY._serialized_end=5887
+  _SPIKESORTERDASHBOARDGENERALREC._serialized_start=5890
+  _SPIKESORTERDASHBOARDGENERALREC._serialized_end=6318
+  _SPIKESORTERDASHBOARDAI._serialized_start=6321
+  _SPIKESORTERDASHBOARDAI._serialized_end=6534
+  _INDICODASHBOARDSITESTATS._serialized_start=6536
+  _INDICODASHBOARDSITESTATS._serialized_end=6631
+  _INDICODASHBOARDPORTSTATS._serialized_start=6634
+  _INDICODASHBOARDPORTSTATS._serialized_end=6778
+  _INDICODASHBOARDSITEINDICATORS._serialized_start=6781
+  _INDICODASHBOARDSITEINDICATORS._serialized_end=6998
+  _INDICODASHBOARDNEURONINDICATORS._serialized_start=7001
+  _INDICODASHBOARDNEURONINDICATORS._serialized_end=7178
+  _SPIKESORTERDASHBOARDSITEDESC._serialized_start=7181
+  _SPIKESORTERDASHBOARDSITEDESC._serialized_end=7476
+  _SPIKESORTERDASHBOARDNEURONDESC._serialized_start=7479
+  _SPIKESORTERDASHBOARDNEURONDESC._serialized_end=7689
+  _SPIKESORTERDASHBOARDNEURONDETAIL._serialized_start=7692
+  _SPIKESORTERDASHBOARDNEURONDETAIL._serialized_end=7942
+  _SPIKESORTERDASHBOARDSITEDETAIL._serialized_start=7945
+  _SPIKESORTERDASHBOARDSITEDETAIL._serialized_end=8114
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-3.0.0b5/radiens/lib/allego_lib.py` & `radiens-3.0.0b6/radiens/lib/allego_lib.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/lib/channel_metadata.py` & `radiens-3.0.0b6/radiens/lib/channel_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,47 +89,55 @@
     @ property
     def attributes(self) -> dict:
         """
         Dictionary of attributes
         """
         return self._d
 
+    def site_positions(self, stype: SignalType) -> dict:
+        self._d['']
+
     def index(self, stype: SignalType) -> KeyIdxs:
         """
         Signal indices by signal type and index type. All indices are zero-indexed.
 
         Parameters:
-            stype (SignalType): requested signal type
-
-        Examples:
-            >>> meta.index[SignalType.AMP]
-            >>> KEY_IDXS(ntv=[5,1,23,46], dset=[0,1,2,3], sys=[5,1,23,46])
-            >>> meta.index[SignalType.AIN]
-            >>> KEY_IDXS(ntv=[3,2,0,1], dset=[0,1,2,3], sys=[35,34,32,33])  # signal has 32 AMP channels
+            stype (~radiens.utils.enums.SignalType): Signal type
 
-        Notes:
+        Returns:
+            KeyIdxs (~radiens.utils.constants.KeyIdxs): Key index object with keys `ntv`, `dset`, `sys`
 
-        Index definitions:
-          ``ntv`` is the position of the signal (channel) trace when the backing dataset
-          was created for each signal type.  For recording files, it is the position of the channels in the DAQ data stream or primary data file. The ``ntv`` index starts at zero for each signal type.
+        See Also:
+            :py:class:`~radiens.utils.enums.KeyIndex`
 
-          ``dset`` is the position of a signal trace in the backing dataset for each signal type.  Unless the signal traces in the dataset were re-ordered, ``dset`` will equal ``ntv``. The ``dset`` index starts at zero for each signal type.
 
-          ``sys`` is the position of the signal (channel) trace when the backing dataset was created.
-          The ``sys`` index starts at zero and increases in natural order over all signal types alway in the following order: 'amp', 'gpio_ain', 'gpio_din', 'gpio_dout'.
+        Examples:
+            >>> meta.index(SignalType.AMP)
+            >>> KeyIdxs(ntv=[5,1,23,46], dset=[0,1,2,3], sys=[5,1,23,46])
+            >>> meta.index(SignalType.AIN)
+            >>> KeyIdxs(ntv=[3,2,0,1], dset=[0,1,2,3], sys=[35,34,32,33])  # signal has 32 AMP channels
+
+        See Also:
+            :py:class:`~radiens.utils.enums.KeyIndex`
+            :py:class:`~radiens.utils.enums.SignalType`
         """
         if stype not in self._sig_map:
             raise ValueError('stype not in signal map')
         return self._sig_map[stype]
 
     def sel_index(self, stype: SignalType) -> KeyIdxs:
         """
         Selected signal indices by signal type and index type.
 
-        See :py:meth:`index` for more information on signal indices.
+        Parameters:
+            stype (~radiens.utils.enums.SignalType): Signal type
+
+
+       See Also:
+            :py:class:`~radiens.utils.enums.KeyIndex`
         """
         if stype not in self._sig_map:
             raise ValueError('stype not in signal map')
         return self._sel_sig_map[stype]
 
     def num_sigs(self, stype: SignalType) -> int:
         """
```

### Comparing `radiens-3.0.0b5/radiens/lib/dataset_metadata.py` & `radiens-3.0.0b6/radiens/lib/dataset_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,22 +252,22 @@
         Dataset ID of this DataSource the Radiens hub.  `None` indicates that it is not on a hub.
         """
         return self._d['dsource_id']
 
     @ property
     def time_range(self) -> TimeRange:
         """
-        Dataset time range
+        Dataset time range (:py:class:`~radiens.utils.constants.TimeRange`)
         """
         return self._d['TR']
 
     @ property
     def TR(self) -> TimeRange:
         """
-        Aliases `obj.time_range`
+        Alias for `time_range`.
         """
         return self._d['TR']
 
     @ property
     def channel_metadata(self) -> ChannelMetadata:
         """
         Dataset's ChannelMetadata, which describes the dataset's signals (aka channels), probes, positions, etc.
```

### Comparing `radiens-3.0.0b5/radiens/lib/fsys.py` & `radiens-3.0.0b6/radiens/lib/fsys.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/lib/sig_metrics.py` & `radiens-3.0.0b6/radiens/lib/sig_metrics.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/lib/signals_snapshot.py` & `radiens-3.0.0b6/radiens/lib/signals_snapshot.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/lib/spike_sorter.py` & `radiens-3.0.0b6/radiens/lib/spike_sorter.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/lib/spikes.py` & `radiens-3.0.0b6/radiens/lib/spikes.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/lib/summa.py` & `radiens-3.0.0b6/radiens/lib/summa.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/metrics_client.py` & `radiens-3.0.0b6/radiens/metrics_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,16 +65,15 @@
         return self.__parent.type.is_videre()
 
     def calculate(self,
                   dataset_metadata=None,
                   hub_name=DEFAULT_HUB_ID) -> None:
         """
         Calculates and saves signal metrics for a linked dataset.
-        If ``cmd=standard``, then signal metrics are calculated using the set of standard parameters:
-          thresholds:  2.0 * Vex_rms  (negative and positive)
+        If ``cmd=standard``, then signal metrics are calculated using the set of standard parameters: thresholds:  2.0 * Vex_rms  (negative and positive)
 
         If ``cmd=standard``, then signal metrics are calculated using the existing signal metrics parameters (thresholds, windows, etc.)
 
         This is only available for CurateClient and VidereClient
 
         Parameters:
             dataset_metadata (~radiens.lib.dataset_metadata.DatasetMetadata): dataset metadata object         
@@ -483,15 +482,15 @@
                     hub_name=DEFAULT_HUB_ID,
                     channel_metadata=None) -> SignalMetrics:
         """
         Gets the requested signal metrics from a linked dataset.
 
         Parameters:
             time_range (int, float, list, ndarray): if parent client is :py:class:`.AllegoClient`, then this parameter can be `float` or `int`; otherwise, it must be `list` or `~numpy.ndarray`
-            metrics (list): a list of :py:class:`~radiens.lib.sig_metrics.METRIC_ID`. It specified a default list is used.
+            metrics (list): a list of :py:class:`~radiens.utils.enums.MetricID`. It specified a default list is used.
             dataset_metadata (~radiens.lib.dataset_metadata.DatasetMetadata): dataset metadata object
             channel_metadata (~radiens.lib.channel_metadata.ChannelMetadata): Allego connected channels
 
 
         Returns:
             SignalMetrics (~radiens.lib.sig_metrics.SignalMetrics): Requested metrics
```

### Comparing `radiens-3.0.0b5/radiens/signals_client.py` & `radiens-3.0.0b6/radiens/signals_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/spike_sorter_client.py` & `radiens-3.0.0b6/radiens/spike_sorter_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/spikes_client.py` & `radiens-3.0.0b6/radiens/spikes_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/utils/config.py` & `radiens-3.0.0b6/radiens/utils/config.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/utils/constants.py` & `radiens-3.0.0b6/radiens/utils/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,17 @@
 NeuronDesc = namedtuple('NeuronDescriptor', ['id', 'ntv_idx', 'label', 'pos', 'spike_count',
                                              'spike_rate', 'mean_abs_peak_waveform', 'snr', 'metadata'])
 NeuronExtendedMetadata = namedtuple(
     'NeuronExtendedMetadata', ['neuron_uid', 'ensemble_uid', 'func_assembly_uid', 'dataset_uid', 'probe_uid'])
 
 SignalArrays = namedtuple(
     "SignalArrays", ['amp', 'gpio_ain', 'gpio_din', 'gpio_dout'])
-KeyIdxs = namedtuple("KEY_IDXS", ['ntv', 'dset', 'sys'])
+
+#: Python object with keys of type `ntv`, `dset`, `sys`. See :py:class:`~radiens.utils.enums.KeyIndex` for more details
+KeyIdxs = namedtuple("KeyIdxs", ['ntv', 'dset', 'sys', ])
 
 SigSelect = namedtuple(
     "SigSelect", ['amp', 'gpio_ain', 'gpio_din', 'gpio_dout', 'key_idx'])
 ''' SigSelect is used for selecting signals by the given key index type, `key_idx`. The elements are numpy arrays '''
 
 CONVERTIBLE_RADIENS_FILE_TYPES = [
     RadiensFileType.CSV,
```

### Comparing `radiens-3.0.0b5/radiens/utils/enums.py` & `radiens-3.0.0b6/radiens/utils/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 from typing import Any, Type, TypeVar
 
 from radiens.grpc_radiens import allegoserver_pb2, common_pb2, spikesorter_pb2
 
 MetricID = namedtuple("METRIC_ID", ['mode', 'name'])
 """
 Example:
-    >>> metric_id = METRIC_ID(mode=METRIC_MODE.BASE, name=METRIC.MEAN)
+    >>> metric_id = MetricID(mode=MetricMode.BASE, name=MetricName.MEAN)
 """
 
 
 MetricStats = namedtuple("METRIC_STATS", ['mean', 'sd', 'max', 'min'])
 
 # enums
 
 
 class ClientType(Enum):
     """TYPE is used to specify the type of client. 
     """
-    ALLEGO = 'AllegoClient'
-    VIDERE = 'VidereClient'
-    CURATE = 'CurateClient'
+
+    ALLEGO = 'AllegoClient'  #: Allego client
+    VIDERE = 'VidereClient'  #: Videre client
+    CURATE = 'CurateClient'  #: Curate client
 
     @classmethod
     def parse(cls, x: str | ClientType) -> ClientType:
         if isinstance(x, str):
             if x.lower() == 'allego' or x.lower() == 'allegoclient':
                 return cls.ALLEGO
             elif x.lower() == 'videre' or x.lower() == 'videreclient':
@@ -63,25 +64,32 @@
     SORTER = auto()
     DEV = auto()
     RADIENSPY = auto()
 
 
 class KeyIndex(Enum):
     """
-    An enumeration of key index types 
+    An enumeration of key index types.
+
+    See Also:
+        :py:meth:`~radiens.lib.channel_metadata.ChannelMetadata.index`
 
-    Example: 
-        >>> key_ind = KeyIndex.NTV 
+    Example:
+        >>> key_ind = KeyIndex.NTV
 
     Valid values are as follows:
     """
 
-    NTV = 0  #: native
-    DATA = 1  #: data
-    SYS = 2  #: system
+    #: The *native key index* is the position of the signal (channel) trace when the backing dataset was created for each signal type. For recording files, it is the position of the channels in the DAQ data stream or primary data file. The ``ntv`` index starts at zero for each signal type.
+    NTV = 0
+    #: The *dataset key index* is the position of a signal trace in the backing dataset for each signal type. Unless the signal traces in the dataset were re-ordered, ``dset`` will equal ``ntv``. The ``dset`` index starts at zero for each signal type.
+    DATA = 1
+    #: The *system key index* starts at zero and increases in natural order over all signal types, always in the following order:
+    #: ``'amp'``, ``'gpio_ain'``, ``'gpio_din'``, ``'gpio_dout'``.
+    SYS = 2
 
 
 # protobuf enums
 T = TypeVar('T', bound='GrpcEnum')
 
 
 class GrpcEnum(Enum):
@@ -254,22 +262,22 @@
     CURATE = common_pb2.WorkspaceApp.Curate
     VIDERE = common_pb2.WorkspaceApp.Videre
 
 
 class PsdScaling(GrpcEnum):
     '''PsdScaling is used to set the power spectral density (PSD) scale. 
     '''
-    ABSOLUTE = common_pb2.PSDScaling.PSD_ABSOLUTE
+    ABSOLUTE = common_pb2.PSDScaling.PSD_ABSOLUTE  #: absolute scale
 
 
 class SignalUnits(GrpcEnum):  # not defined in protos, but rather in corelib
-    UNKNOWN = 0
-    MICROVOLTS = 1
-    VOLTS = 2
-    BINARY = 3
+    UNKNOWN = 0  #: unknown units
+    MICROVOLTS = 1  #: microvolts
+    VOLTS = 2  #: volts
+    BINARY = 3  #: binary
 
     def __str__(self):
         if self.value == SignalUnits.MICROVOLTS.value:
             return "μV"
         elif self.value == SignalUnits.VOLTS.value:
             return "V"
         elif self.value == SignalUnits.BINARY.value:
@@ -280,16 +288,18 @@
             raise ValueError(
                 f"Invalid {self.__class__.__name__} value: {self.value}")
 
 
 class FftWindow(GrpcEnum):
     '''FftWindow is used to set the time-domain window function for power spectral density (PSD) analysis.  
     '''
-    HAMMING_p01 = common_pb2.PSDWindowType.HAMMING_p01
+    HAMMING_p01 = common_pb2.PSDWindowType.HAMMING_p01  #: Hamming window with 1% overlap
+    #: Hamming window with 5% overlap
     HAMMING_p05 = common_pb2.PSDWindowType.HAMMING_p05
+    #: pass-through (no windowing)
     PASS_THROUGH = common_pb2.PSDWindowType.PASS_THROUGH
 
 
 class StatsVector(GrpcEnum):
     '''Enum for summary statistic vectors'''
 
     STAT_MEAN = common_pb2.SummaryStatsEnum.SS_STAT_MEAN
@@ -323,24 +333,24 @@
     N = common_pb2.SummaryStatsEnum.SS_STAT_N
 
 
 class RadiensFileType(GrpcEnum):
     """
     An enumeration of Radiens file types
     """
-    RHD = common_pb2.RHD
-    XDAT = common_pb2.XDAT
-    CSV = common_pb2.CSV
-    HDF5 = common_pb2.HDF5
-    NEX5 = common_pb2.NEX5
-    NWB = common_pb2.NWB
-    KILOSORT2 = common_pb2.KILOSORT2
-    NSX = common_pb2.NSX
-    TDT = common_pb2.TDT
-    SPIKES = common_pb2.SPIKES
+    RHD = common_pb2.RHD  #: RHD file
+    XDAT = common_pb2.XDAT  #: XDAT file
+    CSV = common_pb2.CSV  #: CSV file
+    HDF5 = common_pb2.HDF5  #: HDF5 file
+    NEX5 = common_pb2.NEX5  #: NEX5 file
+    NWB = common_pb2.NWB  #: NWB file
+    KILOSORT2 = common_pb2.KILOSORT2  #: Kilosort2 (bin) file
+    NSX = common_pb2.NSX  #: NSX file
+    TDT = common_pb2.TDT  #: TDT file
+    SPIKES = common_pb2.SPIKES  #: Spikes file
 
 
 class TrsMode(GrpcEnum):
     """
     TrsMode is the time range selector (TRS) enum used to control time range selection in calls to get signals, spikes, power spectral density, or similar data sets.  
 
     Example:
@@ -353,15 +363,15 @@
     #: selects [start, head of stream/cache/file]
     TO_HEAD = common_pb2.TimeRangeSelMode.TRS_TO_HEAD
     #: selects [(head of stream/cache/file - start)
     FROM_HEAD = common_pb2.TimeRangeSelMode.TRS_FROM_HEAD
 
 
 class MetricMode(GrpcEnum):
-    BASE = common_pb2.KpiMetricsMode.Kpi_MetricsMode_Base  # : base packet
+    BASE = common_pb2.KpiMetricsMode.Kpi_MetricsMode_Base  #: base packet
     #: running average of all base packets in the stream
     AVG = common_pb2.KpiMetricsMode.Kpi_MetricsMode_Avg
     #: cumulative over all base packets in the stream
     STREAM = common_pb2.KpiMetricsMode.Kpi_MetricsMode_Stream
 
 
 class MetricName(GrpcEnum):
@@ -446,53 +456,63 @@
     An enumeration of port types
 
     Example:
         >>> port = Port.A
 
     Valid values are as follows:
     """
-    A = common_pb2.Port.A
-    B = common_pb2.Port.B
-    C = common_pb2.Port.C
-    D = common_pb2.Port.D
-    E = common_pb2.Port.E
-    F = common_pb2.Port.F
-    G = common_pb2.Port.G
-    H = common_pb2.Port.H
+    A = common_pb2.Port.A  #: port A
+    B = common_pb2.Port.B  #: port B
+    C = common_pb2.Port.C  #: port C
+    D = common_pb2.Port.D  #: port D
+    E = common_pb2.Port.E  #: port E
+    F = common_pb2.Port.F  #: port F
+    G = common_pb2.Port.G  #: port G
+    H = common_pb2.Port.H  #: port H
 
 
 class SystemMode(GrpcEnum):
     """
     An enumeration of system modes
 
     Example:
         >>> sys_mode = SystemMode.SMARTBOX_PRO
 
     Valid values are as follows:
     """
 
-    SMARTBOX_PRO = allegoserver_pb2.BackboneMode.SMARTBOX_PRO
+    SMARTBOX_PRO = allegoserver_pb2.BackboneMode.SMARTBOX_PRO  #: Smartbox Pro
+    #: Smartbox Pro Sinaps 256
     SMARTBOX_PRO_SINAPS_256 = allegoserver_pb2.BackboneMode.SMARTBOX_PRO_SINAPS_256
+    #: Smartbox Pro Sinaps 512
     SMARTBOX_PRO_SINAPS_512 = allegoserver_pb2.BackboneMode.SMARTBOX_PRO_SINAPS_512
+    #: Smartbox Pro Sinaps 1024
     SMARTBOX_PRO_SINAPS_1024 = allegoserver_pb2.BackboneMode.SMARTBOX_PRO_SINAPS_1024
-    SMARTBOX_CLASSIC = allegoserver_pb2.BackboneMode.SMARTBOX_CLASSIC
+    SMARTBOX_CLASSIC = allegoserver_pb2.BackboneMode.SMARTBOX_CLASSIC  #: Smartbox Classic
+    #: Smartbox Sim Gen Sine
     SMARTBOX_SIM_GEN_SINE = allegoserver_pb2.BackboneMode.SMARTBOX_SIM_GEN_SINE
+    #: Smartbox Sim Gen Sine Mapped
     SMARTBOX_SIM_GEN_SINE_MAPPED = allegoserver_pb2.BackboneMode.SMARTBOX_SIM_GEN_SINE_MAPPED
+    #: Smartbox Sim Gen Sine High Freq
     SMARTBOX_SIM_GEN_SINE_HIGH_FREQ = allegoserver_pb2.BackboneMode.SMARTBOX_SIM_GEN_SINE_HIGH_FREQ
+    #: Smartbox Sim Gen Sine Multi Band
     SMARTBOX_SIM_GEN_SINE_MULTI_BAND = allegoserver_pb2.BackboneMode.SMARTBOX_SIM_GEN_SINE_MULTI_BAND
+    #: Smartbox Sim Gen Spikes
     SMARTBOX_SIM_GEN_SPIKES = allegoserver_pb2.BackboneMode.SMARTBOX_SIM_GEN_SPIKES
-    OPEN_EPHYS_USB2 = allegoserver_pb2.BackboneMode.OPEN_EPHYS_USB2
-    OPEN_EPHYS_USB3 = allegoserver_pb2.BackboneMode.OPEN_EPHYS_USB3
-    INTAN_USB2 = allegoserver_pb2.BackboneMode.INTAN_USB2
+    OPEN_EPHYS_USB2 = allegoserver_pb2.BackboneMode.OPEN_EPHYS_USB2  #: Open Ephys USB2
+    OPEN_EPHYS_USB3 = allegoserver_pb2.BackboneMode.OPEN_EPHYS_USB3  #: Open Ephys USB3
+    INTAN_USB2 = allegoserver_pb2.BackboneMode.INTAN_USB2  #: Intan USB2
+    #: Intan Recording Controller 1024
     INTAN_RECORDING_CONTROLLER_1024 = allegoserver_pb2.BackboneMode.INTAN_RECORDING_CONTROLLER_1024
+    #: Intan Recording Controller 512
     INTAN_RECORDING_CONTROLLER_512 = allegoserver_pb2.BackboneMode.INTAN_RECORDING_CONTROLLER_512
-    XDAQ_ONE_REC = allegoserver_pb2.BackboneMode.XDAQ_ONE_REC
-    XDAQ_ONE_STIM = allegoserver_pb2.BackboneMode.XDAQ_ONE_STIM
-    XDAQ_CORE_REC = allegoserver_pb2.BackboneMode.XDAQ_CORE_REC
-    XDAQ_CORE_STIM = allegoserver_pb2.BackboneMode.XDAQ_CORE_STIM
+    XDAQ_ONE_REC = allegoserver_pb2.BackboneMode.XDAQ_ONE_REC  #: XDAQ One Rec
+    XDAQ_ONE_STIM = allegoserver_pb2.BackboneMode.XDAQ_ONE_STIM  #: XDAQ One Stim
+    XDAQ_CORE_REC = allegoserver_pb2.BackboneMode.XDAQ_CORE_REC  #: XDAQ Core Rec
+    XDAQ_CORE_STIM = allegoserver_pb2.BackboneMode.XDAQ_CORE_STIM  #: XDAQ Core Stim
 
 
 class SignalType(GrpcEnum):
     """
     An enumeration of signal types
 
     Example:
```

### Comparing `radiens-3.0.0b5/radiens/utils/util.py` & `radiens-3.0.0b6/radiens/utils/util.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens/videre_client.py` & `radiens-3.0.0b6/radiens/videre_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         UID of this client session.
         """
         return self._id()
 
     @property
     def type(self) -> ClientType:
         """
-        Returns ClientType.VIDERE
+        Returns :py:attr:`~radiens.utils.enums.ClientType.VIDERE`
         """
         return ClientType.VIDERE
 
     def signal_metrics(self) -> MetricsClient:
         """
         Videre signal metrics API
         """
```

### Comparing `radiens-3.0.0b5/radiens/workspace_client.py` & `radiens-3.0.0b6/radiens/workspace_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/radiens.egg-info/PKG-INFO` & `radiens-3.0.0b6/radiens.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radiens
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: provides python API to RADIENS analytics platform
 Home-page: http://neuronexus.github.io
 Author: NeuroNexus
 Author-email: dkipke@neuronexus.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
@@ -29,14 +29,26 @@
 
 # Changelog
 
 All notable changes (for versions > `3.X.X`) to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [3.0.0b6] - 2024-04-22
+
+### Added
+
+- documentation updates
+
+## [3.0.0b5] - 2024-03-27
+
+### Added
+
+- `CurateClient.file_convert()` method for converting between supported file formats
+
 ## [3.0.0b4] - 2024-03-12
 
 ### Added
 
 - `units` attribute on `PSD` class that contains the units of the PSD (as a `string`) per `SignalType`
 - `SignalUnits` enum to represent units of signal data
```

### Comparing `radiens-3.0.0b5/radiens.egg-info/SOURCES.txt` & `radiens-3.0.0b6/radiens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/setup.py` & `radiens-3.0.0b6/setup.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/tests/test_allego_client.py` & `radiens-3.0.0b6/tests/test_allego_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/tests/test_base_client.py` & `radiens-3.0.0b6/tests/test_base_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/tests/test_curate_client.py` & `radiens-3.0.0b6/tests/test_curate_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b5/tests/test_videre_client.py` & `radiens-3.0.0b6/tests/test_videre_client.py`

 * *Files identical despite different names*


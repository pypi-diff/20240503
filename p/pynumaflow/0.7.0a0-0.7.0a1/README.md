# Comparing `tmp/pynumaflow-0.7.0a0.tar.gz` & `tmp/pynumaflow-0.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumaflow-0.7.0a0.tar", max compression
+gzip compressed data, was "pynumaflow-0.7.0a1.tar", max compression
```

## Comparing `pynumaflow-0.7.0a0.tar` & `pynumaflow-0.7.0a1.tar`

### file list

```diff
@@ -1,94 +1,95 @@
--rw-r--r--   0        0        0    11357 2024-03-26 20:07:43.063086 pynumaflow-0.7.0a0/LICENSE
--rw-r--r--   0        0        0     6664 2024-03-26 20:07:43.063086 pynumaflow-0.7.0a0/README.md
--rw-r--r--   0        0        0      985 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/__init__.py
--rw-r--r--   0        0        0     2076 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/_constants.py
--rw-r--r--   0        0        0      332 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/info/__init__.py
--rw-r--r--   0        0        0     1594 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/info/server.py
--rw-r--r--   0        0        0     1193 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/info/types.py
--rw-r--r--   0        0        0      404 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapper/__init__.py
--rw-r--r--   0        0        0     5885 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapper/_dtypes.py
--rw-r--r--   0        0        0     3883 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapper/async_server.py
--rw-r--r--   0        0        0     4292 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapper/multiproc_server.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapper/servicer/__init__.py
--rw-r--r--   0        0        0     2652 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapper/servicer/async_servicer.py
--rw-r--r--   0        0        0     1351 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapper/servicer/sync_servicer.py
--rw-r--r--   0        0        0     1310 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapper/servicer/utils.py
--rw-r--r--   0        0        0     3912 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapper/sync_server.py
--rw-r--r--   0        0        0      308 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapstreamer/__init__.py
--rw-r--r--   0        0        0     5595 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapstreamer/_dtypes.py
--rw-r--r--   0        0        0     4654 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapstreamer/async_server.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapstreamer/servicer/__init__.py
--rw-r--r--   0        0        0     2404 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/mapstreamer/servicer/async_servicer.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/mapper/__init__.py
--rw-r--r--   0        0        0      908 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/mapper/map.proto
--rw-r--r--   0        0        0     2673 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/mapper/map_pb2.py
--rw-r--r--   0        0        0     3906 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/mapper/map_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/mapstreamer/__init__.py
--rw-r--r--   0        0        0      983 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/mapstreamer/mapstream.proto
--rw-r--r--   0        0        0     2855 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/mapstreamer/mapstream_pb2.py
--rw-r--r--   0        0        0     4174 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/mapstreamer/mapstream_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/reducer/__init__.py
--rw-r--r--   0        0        0     1823 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/reducer/reduce.proto
--rw-r--r--   0        0        0     4075 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/reducer/reduce_pb2.py
--rw-r--r--   0        0        0     4055 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/reducer/reduce_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sideinput/__init__.py
--rw-r--r--   0        0        0     1482 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sideinput/sideinput.proto
--rw-r--r--   0        0        0     1665 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sideinput/sideinput_pb2.py
--rw-r--r--   0        0        0     5798 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sideinput/sideinput_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sinker/__init__.py
--rw-r--r--   0        0        0     1232 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sinker/sink.proto
--rw-r--r--   0        0        0     2739 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sinker/sink_pb2.py
--rw-r--r--   0        0        0     3970 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sinker/sink_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sourcer/__init__.py
--rw-r--r--   0        0        0     6480 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sourcer/source.proto
--rw-r--r--   0        0        0     5017 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sourcer/source_pb2.py
--rw-r--r--   0        0        0     9375 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sourcer/source_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sourcetransformer/__init__.py
--rw-r--r--   0        0        0     1267 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sourcetransformer/transform.proto
--rw-r--r--   0        0        0     3093 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sourcetransformer/transform_pb2.py
--rw-r--r--   0        0        0     4534 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/proto/sourcetransformer/transform_pb2_grpc.py
--rw-r--r--   0        0        0      349 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducer/__init__.py
--rw-r--r--   0        0        0    10780 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducer/_dtypes.py
--rw-r--r--   0        0        0     6797 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducer/async_server.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducer/servicer/__init__.py
--rw-r--r--   0        0        0     5953 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducer/servicer/async_servicer.py
--rw-r--r--   0        0        0     6287 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducer/servicer/task_manager.py
--rw-r--r--   0        0        0      397 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducestreamer/__init__.py
--rw-r--r--   0        0        0     9558 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducestreamer/_dtypes.py
--rw-r--r--   0        0        0     7628 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducestreamer/async_server.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducestreamer/servicer/__init__.py
--rw-r--r--   0        0        0     5398 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducestreamer/servicer/async_servicer.py
--rw-r--r--   0        0        0    12042 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/reducestreamer/servicer/task_manager.py
--rw-r--r--   0        0        0       83 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/shared/__init__.py
--rw-r--r--   0        0        0      512 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/shared/asynciter.py
--rw-r--r--   0        0        0     8219 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/shared/server.py
--rw-r--r--   0        0        0      250 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/sideinput/__init__.py
--rw-r--r--   0        0        0     1826 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/sideinput/_dtypes.py
--rw-r--r--   0        0        0     3484 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/sideinput/server.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/sideinput/servicer/__init__.py
--rw-r--r--   0        0        0     1722 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/sideinput/servicer/servicer.py
--rw-r--r--   0        0        0      270 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/sinker/__init__.py
--rw-r--r--   0        0        0     6169 2024-03-26 20:07:43.075086 pynumaflow-0.7.0a0/pynumaflow/sinker/_dtypes.py
--rw-r--r--   0        0        0     4097 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sinker/async_server.py
--rw-r--r--   0        0        0     3800 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sinker/server.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sinker/servicer/__init__.py
--rw-r--r--   0        0        0     2835 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sinker/servicer/async_servicer.py
--rw-r--r--   0        0        0     2554 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sinker/servicer/sync_servicer.py
--rw-r--r--   0        0        0      520 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcer/__init__.py
--rw-r--r--   0        0        0     7957 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcer/_dtypes.py
--rw-r--r--   0        0        0     5712 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcer/async_server.py
--rw-r--r--   0        0        0     5375 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcer/server.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcer/servicer/__init__.py
--rw-r--r--   0        0        0     5138 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcer/servicer/async_servicer.py
--rw-r--r--   0        0        0     5591 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcer/servicer/sync_servicer.py
--rw-r--r--   0        0        0      446 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcetransformer/__init__.py
--rw-r--r--   0        0        0     6048 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcetransformer/_dtypes.py
--rw-r--r--   0        0        0     5208 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcetransformer/multiproc_server.py
--rw-r--r--   0        0        0     4845 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcetransformer/server.py
--rw-r--r--   0        0        0        0 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcetransformer/servicer/__init__.py
--rw-r--r--   0        0        0     2990 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/sourcetransformer/servicer/server.py
--rw-r--r--   0        0        0      170 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pynumaflow/types.py
--rw-r--r--   0        0        0     1706 2024-03-26 20:07:43.079086 pynumaflow-0.7.0a0/pyproject.toml
--rw-r--r--   0        0        0     7786 1970-01-01 00:00:00.000000 pynumaflow-0.7.0a0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-18 03:59:38.776839 pynumaflow-0.7.0a1/LICENSE
+-rw-r--r--   0        0        0     6678 2024-04-18 03:59:38.776839 pynumaflow-0.7.0a1/README.md
+-rw-r--r--   0        0        0      985 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/__init__.py
+-rw-r--r--   0        0        0     2310 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/_constants.py
+-rw-r--r--   0        0        0      332 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/info/__init__.py
+-rw-r--r--   0        0        0     1594 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/info/server.py
+-rw-r--r--   0        0        0     1422 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/info/types.py
+-rw-r--r--   0        0        0      404 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/__init__.py
+-rw-r--r--   0        0        0     5885 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/_dtypes.py
+-rw-r--r--   0        0        0     3883 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/async_server.py
+-rw-r--r--   0        0        0     4292 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/multiproc_server.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/__init__.py
+-rw-r--r--   0        0        0     2658 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/async_servicer.py
+-rw-r--r--   0        0        0     1351 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/sync_servicer.py
+-rw-r--r--   0        0        0     1310 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/utils.py
+-rw-r--r--   0        0        0     3912 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/sync_server.py
+-rw-r--r--   0        0        0      308 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapstreamer/__init__.py
+-rw-r--r--   0        0        0     5595 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapstreamer/_dtypes.py
+-rw-r--r--   0        0        0     4654 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapstreamer/async_server.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapstreamer/servicer/__init__.py
+-rw-r--r--   0        0        0     2410 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapstreamer/servicer/async_servicer.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapper/__init__.py
+-rw-r--r--   0        0        0      908 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map.proto
+-rw-r--r--   0        0        0     2731 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map_pb2.py
+-rw-r--r--   0        0        0     3906 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/__init__.py
+-rw-r--r--   0        0        0      983 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream.proto
+-rw-r--r--   0        0        0     2913 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream_pb2.py
+-rw-r--r--   0        0        0     4174 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/reducer/__init__.py
+-rw-r--r--   0        0        0     1823 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce.proto
+-rw-r--r--   0        0        0     4133 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce_pb2.py
+-rw-r--r--   0        0        0     4055 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/__init__.py
+-rw-r--r--   0        0        0     1482 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput.proto
+-rw-r--r--   0        0        0     1699 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput_pb2.py
+-rw-r--r--   0        0        0     5798 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sinker/__init__.py
+-rw-r--r--   0        0        0     1318 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink.proto
+-rw-r--r--   0        0        0     3037 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink_pb2.py
+-rw-r--r--   0        0        0     3970 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/__init__.py
+-rw-r--r--   0        0        0     6480 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source.proto
+-rw-r--r--   0        0        0     5075 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source_pb2.py
+-rw-r--r--   0        0        0     9375 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/__init__.py
+-rw-r--r--   0        0        0     1267 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform.proto
+-rw-r--r--   0        0        0     3151 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform_pb2.py
+-rw-r--r--   0        0        0     4534 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform_pb2_grpc.py
+-rw-r--r--   0        0        0      349 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/__init__.py
+-rw-r--r--   0        0        0    10780 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/_dtypes.py
+-rw-r--r--   0        0        0     6797 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/async_server.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/servicer/__init__.py
+-rw-r--r--   0        0        0     5959 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/servicer/async_servicer.py
+-rw-r--r--   0        0        0     6287 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/servicer/task_manager.py
+-rw-r--r--   0        0        0      397 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/__init__.py
+-rw-r--r--   0        0        0     9558 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/_dtypes.py
+-rw-r--r--   0        0        0     7628 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/async_server.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/servicer/__init__.py
+-rw-r--r--   0        0        0     5447 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/servicer/async_servicer.py
+-rw-r--r--   0        0        0    12042 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/servicer/task_manager.py
+-rw-r--r--   0        0        0       83 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/shared/__init__.py
+-rw-r--r--   0        0        0      512 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/shared/asynciter.py
+-rw-r--r--   0        0        0     8131 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/shared/server.py
+-rw-r--r--   0        0        0      250 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sideinput/__init__.py
+-rw-r--r--   0        0        0     1826 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sideinput/_dtypes.py
+-rw-r--r--   0        0        0     3484 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sideinput/server.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sideinput/servicer/__init__.py
+-rw-r--r--   0        0        0     1722 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sideinput/servicer/servicer.py
+-rw-r--r--   0        0        0      270 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/__init__.py
+-rw-r--r--   0        0        0     6886 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/_dtypes.py
+-rw-r--r--   0        0        0     4578 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/async_server.py
+-rw-r--r--   0        0        0     4266 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/server.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/__init__.py
+-rw-r--r--   0        0        0     2821 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/async_servicer.py
+-rw-r--r--   0        0        0     2540 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/sync_servicer.py
+-rw-r--r--   0        0        0      495 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/utils.py
+-rw-r--r--   0        0        0      520 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/__init__.py
+-rw-r--r--   0        0        0     7957 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/_dtypes.py
+-rw-r--r--   0        0        0     5712 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/async_server.py
+-rw-r--r--   0        0        0     5375 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/server.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/servicer/__init__.py
+-rw-r--r--   0        0        0     5138 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/servicer/async_servicer.py
+-rw-r--r--   0        0        0     5597 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/servicer/sync_servicer.py
+-rw-r--r--   0        0        0      446 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/__init__.py
+-rw-r--r--   0        0        0     6048 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/_dtypes.py
+-rw-r--r--   0        0        0     5208 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/multiproc_server.py
+-rw-r--r--   0        0        0     4845 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/server.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/servicer/__init__.py
+-rw-r--r--   0        0        0     2996 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/servicer/server.py
+-rw-r--r--   0        0        0      170 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/types.py
+-rw-r--r--   0        0        0     1706 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pyproject.toml
+-rw-r--r--   0        0        0     7800 1970-01-01 00:00:00.000000 pynumaflow-0.7.0a1/PKG-INFO
```

### Comparing `pynumaflow-0.7.0a0/LICENSE` & `pynumaflow-0.7.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/README.md` & `pynumaflow-0.7.0a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Python SDK for Numaflow
 
-[![Build](https://github.com/numaproj/numaflow-python/actions/workflows/ci.yml/badge.svg)](https://github.com/numaproj/numaflow-python/actions/workflows/ci.yml)
+[![Build](https://github.com/numaproj/numaflow-python/actions/workflows/run-tests.yml/badge.svg)](https://github.com/numaproj/numaflow-python/actions/workflows/run-tests.yml)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
 [![Release Version](https://img.shields.io/github/v/release/numaproj/numaflow-python?label=pynumaflow)](https://github.com/numaproj/numaflow-python/releases/latest)
 
 This is the Python SDK for [Numaflow](https://numaflow.numaproj.io/).
 
 This SDK provides the interface for writing different functionalities of Numaflow like [UDFs](https://numaflow.numaproj.io/user-guide/user-defined-functions/user-defined-functions/), [UDSinks](https://numaflow.numaproj.io/user-guide/sinks/user-defined-sinks/), [UDSources](https://numaflow.numaproj.io/user-guide/sources/user-defined-sources/) and [SideInput](https://numaflow.numaproj.io/specifications/side-inputs/) in Python.
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/__init__.py` & `pynumaflow-0.7.0a1/pynumaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/_constants.py` & `pynumaflow-0.7.0a1/pynumaflow/_constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,24 +13,29 @@
 REDUCE_STREAM_SOCK_PATH = "/var/run/numaflow/reducestream.sock"
 SOURCE_TRANSFORMER_SOCK_PATH = "/var/run/numaflow/sourcetransform.sock"
 SINK_SOCK_PATH = "/var/run/numaflow/sink.sock"
 SIDE_INPUT_SOCK_PATH = "/var/run/numaflow/sideinput.sock"
 SOURCE_SOCK_PATH = "/var/run/numaflow/source.sock"
 MULTIPROC_MAP_SOCK_PORT = 55551
 MULTIPROC_MAP_SOCK_ADDR = "0.0.0.0"
+FALLBACK_SINK_SOCK_PATH = "/var/run/numaflow/fb-sink.sock"
 
 # Server information file configs
 MAP_SERVER_INFO_FILE_PATH = "/var/run/numaflow/mapper-server-info"
 MAP_STREAM_SERVER_INFO_FILE_PATH = "/var/run/numaflow/mapstreamer-server-info"
 REDUCE_SERVER_INFO_FILE_PATH = "/var/run/numaflow/reducer-server-info"
 REDUCE_STREAM_SERVER_INFO_FILE_PATH = "/var/run/numaflow/reducestreamer-server-info"
 SOURCE_TRANSFORMER_SERVER_INFO_FILE_PATH = "/var/run/numaflow/sourcetransformer-server-info"
 SINK_SERVER_INFO_FILE_PATH = "/var/run/numaflow/sinker-server-info"
 SIDE_INPUT_SERVER_INFO_FILE_PATH = "/var/run/numaflow/sideinput-server-info"
 SOURCE_SERVER_INFO_FILE_PATH = "/var/run/numaflow/sourcer-server-info"
+FALLBACK_SINK_SERVER_INFO_FILE_PATH = "/var/run/numaflow/fb-sinker-server-info"
+
+ENV_UD_CONTAINER_TYPE = "NUMAFLOW_UD_CONTAINER_TYPE"
+UD_CONTAINER_FALLBACK_SINK = "fb-udsink"
 
 # TODO: need to make sure the DATUM_KEY value is the same as
 # https://github.com/numaproj/numaflow-go/blob/main/pkg/function/configs.go#L6
 WIN_START_TIME = "x-numaflow-win-start-time"
 WIN_END_TIME = "x-numaflow-win-end-time"
 MAX_MESSAGE_SIZE = 1024 * 1024 * 64
 # TODO: None instead of "EOF" ?
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/info/server.py` & `pynumaflow-0.7.0a1/pynumaflow/info/server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/info/types.py` & `pynumaflow-0.7.0a1/pynumaflow/info/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from dataclasses import dataclass, field
 from enum import Enum
 
 # Constants for using in the info-server
+# Specify the minimum Numaflow version required by the current SDK version
+MINIMUM_NUMAFLOW_VERSION = "1.2.0-rc4"
 # Need to keep consistent with all SDKs and client
 EOF = "U+005C__END__"
 
 # Env variables to be passed in the info server metadata.
 # These need to be accessed in the client using the same key.
 # Format - (key, env_var)
 METADATA_ENVS = [("CPU_LIMIT", "NUMAFLOW_CPU_LIMIT")]
@@ -34,15 +36,17 @@
 class ServerInfo:
     """
     ServerInfo is used for the gRPC server to provide the information such as protocol,
     sdk version, language, metadata to the client.
     Args:
         protocol: Protocol to use (UDS or TCP)
         language: Language used by the server(Python, Golang, Java)
+        minimum_numaflow_version: lower bound for the supported Numaflow version
         version: Numaflow sdk version used by the server
         metadata: Any additional information to be provided (env vars)
     """
 
     protocol: Protocol
     language: Language
+    minimum_numaflow_version: str
     version: str
     metadata: dict = field(default_factory=dict)
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/mapper/_dtypes.py` & `pynumaflow-0.7.0a1/pynumaflow/mapper/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/mapper/async_server.py` & `pynumaflow-0.7.0a1/pynumaflow/mapper/async_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/mapper/multiproc_server.py` & `pynumaflow-0.7.0a1/pynumaflow/mapper/multiproc_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/mapper/servicer/async_servicer.py` & `pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/async_servicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             res = await self.__invoke_map(
                 list(request.keys),
                 Datum(
                     keys=list(request.keys),
                     value=request.value,
                     event_time=request.event_time.ToDatetime(),
                     watermark=request.watermark.ToDatetime(),
-                    headers=request.headers,
+                    headers=dict(request.headers),
                 ),
             )
         except Exception as e:
             context.set_code(grpc.StatusCode.UNKNOWN)
             context.set_details(str(e))
             return map_pb2.MapResponse(results=[])
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/mapper/servicer/sync_servicer.py` & `pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/sync_servicer.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/mapper/servicer/utils.py` & `pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/utils.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/mapper/sync_server.py` & `pynumaflow-0.7.0a1/pynumaflow/mapper/sync_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/mapstreamer/_dtypes.py` & `pynumaflow-0.7.0a1/pynumaflow/mapstreamer/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/mapstreamer/async_server.py` & `pynumaflow-0.7.0a1/pynumaflow/mapstreamer/async_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/mapstreamer/servicer/async_servicer.py` & `pynumaflow-0.7.0a1/pynumaflow/mapstreamer/servicer/async_servicer.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         async for res in self.__invoke_map_stream(
             list(request.keys),
             Datum(
                 keys=list(request.keys),
                 value=request.value,
                 event_time=request.event_time.ToDatetime(),
                 watermark=request.watermark.ToDatetime(),
-                headers=request.headers,
+                headers=dict(request.headers),
             ),
         ):
             yield mapstream_pb2.MapStreamResponse(result=res)
 
     async def __invoke_map_stream(self, keys: list[str], req: Datum):
         try:
             async for msg in self.__map_stream_handler(keys, req):
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/mapper/map.proto` & `pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/mapper/map_pb2.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: map.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -21,16 +22,16 @@
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "map_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _MAPREQUEST_HEADERSENTRY._options = None
-    _MAPREQUEST_HEADERSENTRY._serialized_options = b"8\001"
+    _globals["_MAPREQUEST_HEADERSENTRY"]._options = None
+    _globals["_MAPREQUEST_HEADERSENTRY"]._serialized_options = b"8\001"
     _globals["_MAPREQUEST"]._serialized_start = 84
     _globals["_MAPREQUEST"]._serialized_end = 318
     _globals["_MAPREQUEST_HEADERSENTRY"]._serialized_start = 272
     _globals["_MAPREQUEST_HEADERSENTRY"]._serialized_end = 318
     _globals["_MAPRESPONSE"]._serialized_start = 320
     _globals["_MAPRESPONSE"]._serialized_end = 431
     _globals["_MAPRESPONSE_RESULT"]._serialized_start = 380
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/mapper/map_pb2_grpc.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/mapstreamer/mapstream.proto` & `pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/mapstreamer/mapstream_pb2.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: mapstream.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -21,16 +22,16 @@
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "mapstream_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _MAPSTREAMREQUEST_HEADERSENTRY._options = None
-    _MAPSTREAMREQUEST_HEADERSENTRY._serialized_options = b"8\001"
+    _globals["_MAPSTREAMREQUEST_HEADERSENTRY"]._options = None
+    _globals["_MAPSTREAMREQUEST_HEADERSENTRY"]._serialized_options = b"8\001"
     _globals["_MAPSTREAMREQUEST"]._serialized_start = 96
     _globals["_MAPSTREAMREQUEST"]._serialized_end = 348
     _globals["_MAPSTREAMREQUEST_HEADERSENTRY"]._serialized_start = 302
     _globals["_MAPSTREAMREQUEST_HEADERSENTRY"]._serialized_end = 348
     _globals["_MAPSTREAMRESPONSE"]._serialized_start = 351
     _globals["_MAPSTREAMRESPONSE"]._serialized_end = 479
     _globals["_MAPSTREAMRESPONSE_RESULT"]._serialized_start = 428
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/mapstreamer/mapstream_pb2_grpc.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/reducer/reduce.proto` & `pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/reducer/reduce_pb2.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: reduce.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -21,16 +22,16 @@
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "reduce_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _REDUCEREQUEST_PAYLOAD_HEADERSENTRY._options = None
-    _REDUCEREQUEST_PAYLOAD_HEADERSENTRY._serialized_options = b"8\001"
+    _globals["_REDUCEREQUEST_PAYLOAD_HEADERSENTRY"]._options = None
+    _globals["_REDUCEREQUEST_PAYLOAD_HEADERSENTRY"]._serialized_options = b"8\001"
     _globals["_REDUCEREQUEST"]._serialized_start = 90
     _globals["_REDUCEREQUEST"]._serialized_end = 626
     _globals["_REDUCEREQUEST_WINDOWOPERATION"]._serialized_start = 220
     _globals["_REDUCEREQUEST_WINDOWOPERATION"]._serialized_end = 378
     _globals["_REDUCEREQUEST_WINDOWOPERATION_EVENT"]._serialized_start = 338
     _globals["_REDUCEREQUEST_WINDOWOPERATION_EVENT"]._serialized_end = 378
     _globals["_REDUCEREQUEST_PAYLOAD"]._serialized_start = 381
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/reducer/reduce_pb2_grpc.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sideinput/sideinput.proto` & `pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sideinput/sideinput_pb2.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: sideinput.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sideinput/sideinput_pb2_grpc.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sinker/sink.proto` & `pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink.proto`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 syntax = "proto3";
-
 import "google/protobuf/empty.proto";
 import "google/protobuf/timestamp.proto";
 
 
 package sink.v1;
 
 service Sink {
@@ -29,21 +28,30 @@
 /**
  * ReadyResponse is the health check result.
  */
 message ReadyResponse {
   bool ready = 1;
 }
 
+/*
+  * Status is the status of the response.
+ */
+enum Status {
+  SUCCESS = 0;
+  FAILURE = 1;
+  FALLBACK = 2;
+}
+
 /**
  * SinkResponse is the individual response of each message written to the sink.
  */
 message SinkResponse {
   message Result {
     // id is the ID of the message, can be used to uniquely identify the message.
     string id = 1;
-    // success denotes the status of persisting to disk. if set to false, it means writing to sink for the message failed.
-    bool success = 2;
+    // status denotes the status of persisting to sink. It can be SUCCESS, FAILURE, or FALLBACK.
+    Status status = 2;
     // err_msg is the error message, set it if success is set to false.
     string err_msg = 3;
   }
   repeated Result results = 1;
 }
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sinker/sink_pb2.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: sink.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -13,30 +14,32 @@
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\nsink.proto\x12\x07sink.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xf9\x01\n\x0bSinkRequest\x12\x0c\n\x04keys\x18\x01 \x03(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12.\n\nevent_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\twatermark\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\n\n\x02id\x18\x05 \x01(\t\x12\x32\n\x07headers\x18\x06 \x03(\x0b\x32!.sink.v1.SinkRequest.HeadersEntry\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01"\x1e\n\rReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08"u\n\x0cSinkResponse\x12-\n\x07results\x18\x01 \x03(\x0b\x32\x1c.sink.v1.SinkResponse.Result\x1a\x36\n\x06Result\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x0f\n\x07\x65rr_msg\x18\x03 \x01(\t2z\n\x04Sink\x12\x37\n\x06SinkFn\x12\x14.sink.v1.SinkRequest\x1a\x15.sink.v1.SinkResponse(\x01\x12\x39\n\x07IsReady\x12\x16.google.protobuf.Empty\x1a\x16.sink.v1.ReadyResponseb\x06proto3'
+    b'\n\nsink.proto\x12\x07sink.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xf9\x01\n\x0bSinkRequest\x12\x0c\n\x04keys\x18\x01 \x03(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12.\n\nevent_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\twatermark\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\n\n\x02id\x18\x05 \x01(\t\x12\x32\n\x07headers\x18\x06 \x03(\x0b\x32!.sink.v1.SinkRequest.HeadersEntry\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01"\x1e\n\rReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08"\x85\x01\n\x0cSinkResponse\x12-\n\x07results\x18\x01 \x03(\x0b\x32\x1c.sink.v1.SinkResponse.Result\x1a\x46\n\x06Result\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1f\n\x06status\x18\x02 \x01(\x0e\x32\x0f.sink.v1.Status\x12\x0f\n\x07\x65rr_msg\x18\x03 \x01(\t*0\n\x06Status\x12\x0b\n\x07SUCCESS\x10\x00\x12\x0b\n\x07\x46\x41ILURE\x10\x01\x12\x0c\n\x08\x46\x41LLBACK\x10\x02\x32z\n\x04Sink\x12\x37\n\x06SinkFn\x12\x14.sink.v1.SinkRequest\x1a\x15.sink.v1.SinkResponse(\x01\x12\x39\n\x07IsReady\x12\x16.google.protobuf.Empty\x1a\x16.sink.v1.ReadyResponseb\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "sink_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _SINKREQUEST_HEADERSENTRY._options = None
-    _SINKREQUEST_HEADERSENTRY._serialized_options = b"8\001"
+    _globals["_SINKREQUEST_HEADERSENTRY"]._options = None
+    _globals["_SINKREQUEST_HEADERSENTRY"]._serialized_options = b"8\001"
+    _globals["_STATUS"]._serialized_start = 505
+    _globals["_STATUS"]._serialized_end = 553
     _globals["_SINKREQUEST"]._serialized_start = 86
     _globals["_SINKREQUEST"]._serialized_end = 335
     _globals["_SINKREQUEST_HEADERSENTRY"]._serialized_start = 289
     _globals["_SINKREQUEST_HEADERSENTRY"]._serialized_end = 335
     _globals["_READYRESPONSE"]._serialized_start = 337
     _globals["_READYRESPONSE"]._serialized_end = 367
-    _globals["_SINKRESPONSE"]._serialized_start = 369
-    _globals["_SINKRESPONSE"]._serialized_end = 486
-    _globals["_SINKRESPONSE_RESULT"]._serialized_start = 432
-    _globals["_SINKRESPONSE_RESULT"]._serialized_end = 486
-    _globals["_SINK"]._serialized_start = 488
-    _globals["_SINK"]._serialized_end = 610
+    _globals["_SINKRESPONSE"]._serialized_start = 370
+    _globals["_SINKRESPONSE"]._serialized_end = 503
+    _globals["_SINKRESPONSE_RESULT"]._serialized_start = 433
+    _globals["_SINKRESPONSE_RESULT"]._serialized_end = 503
+    _globals["_SINK"]._serialized_start = 555
+    _globals["_SINK"]._serialized_end = 677
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sinker/sink_pb2_grpc.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sourcer/source.proto` & `pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sourcer/source_pb2.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: source.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -21,16 +22,16 @@
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "source_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _READRESPONSE_RESULT_HEADERSENTRY._options = None
-    _READRESPONSE_RESULT_HEADERSENTRY._serialized_options = b"8\001"
+    _globals["_READRESPONSE_RESULT_HEADERSENTRY"]._options = None
+    _globals["_READRESPONSE_RESULT_HEADERSENTRY"]._serialized_options = b"8\001"
     _globals["_READREQUEST"]._serialized_start = 89
     _globals["_READREQUEST"]._serialized_end = 206
     _globals["_READREQUEST_REQUEST"]._serialized_start = 153
     _globals["_READREQUEST_REQUEST"]._serialized_end = 206
     _globals["_READRESPONSE"]._serialized_start = 209
     _globals["_READRESPONSE"]._serialized_end = 506
     _globals["_READRESPONSE_RESULT"]._serialized_start = 274
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sourcer/source_pb2_grpc.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sourcetransformer/transform.proto` & `pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sourcetransformer/transform_pb2.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: transform.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -21,16 +22,16 @@
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "transform_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _SOURCETRANSFORMREQUEST_HEADERSENTRY._options = None
-    _SOURCETRANSFORMREQUEST_HEADERSENTRY._serialized_options = b"8\001"
+    _globals["_SOURCETRANSFORMREQUEST_HEADERSENTRY"]._options = None
+    _globals["_SOURCETRANSFORMREQUEST_HEADERSENTRY"]._serialized_options = b"8\001"
     _globals["_SOURCETRANSFORMREQUEST"]._serialized_start = 104
     _globals["_SOURCETRANSFORMREQUEST"]._serialized_end = 376
     _globals["_SOURCETRANSFORMREQUEST_HEADERSENTRY"]._serialized_start = 330
     _globals["_SOURCETRANSFORMREQUEST_HEADERSENTRY"]._serialized_end = 376
     _globals["_SOURCETRANSFORMRESPONSE"]._serialized_start = 379
     _globals["_SOURCETRANSFORMRESPONSE"]._serialized_end = 576
     _globals["_SOURCETRANSFORMRESPONSE_RESULT"]._serialized_start = 477
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/proto/sourcetransformer/transform_pb2_grpc.py` & `pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/reducer/_dtypes.py` & `pynumaflow-0.7.0a1/pynumaflow/reducer/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/reducer/async_server.py` & `pynumaflow-0.7.0a1/pynumaflow/reducer/async_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/reducer/servicer/async_servicer.py` & `pynumaflow-0.7.0a1/pynumaflow/reducer/servicer/async_servicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             operation=d.operation.event,
             windows=d.operation.windows,
             payload=Datum(
                 keys=list(d.payload.keys),
                 value=d.payload.value,
                 event_time=d.payload.event_time.ToDatetime(),
                 watermark=d.payload.watermark.ToDatetime(),
-                headers=d.payload.headers,
+                headers=dict(d.payload.headers),
             ),
         )
         yield reduce_request
 
 
 class AsyncReduceServicer(reduce_pb2_grpc.ReduceServicer):
     """
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/reducer/servicer/task_manager.py` & `pynumaflow-0.7.0a1/pynumaflow/reducer/servicer/task_manager.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/reducestreamer/_dtypes.py` & `pynumaflow-0.7.0a1/pynumaflow/reducestreamer/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/reducestreamer/async_server.py` & `pynumaflow-0.7.0a1/pynumaflow/reducestreamer/async_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/reducestreamer/servicer/async_servicer.py` & `pynumaflow-0.7.0a1/pynumaflow/reducestreamer/servicer/async_servicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             operation=d.operation.event,
             windows=d.operation.windows,
             payload=Datum(
                 keys=list(d.payload.keys),
                 value=d.payload.value,
                 event_time=d.payload.event_time.ToDatetime(),
                 watermark=d.payload.watermark.ToDatetime(),
+                headers=dict(d.payload.headers),
             ),
         )
         yield reduce_request
 
 
 def get_exception_traceback_str(exc) -> str:
     file = io.StringIO()
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/reducestreamer/servicer/task_manager.py` & `pynumaflow-0.7.0a1/pynumaflow/reducestreamer/servicer/task_manager.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/shared/asynciter.py` & `pynumaflow-0.7.0a1/pynumaflow/shared/asynciter.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/shared/server.py` & `pynumaflow-0.7.0a1/pynumaflow/shared/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pynumaflow.exceptions import SocketError
 from pynumaflow.info.server import get_sdk_version, write as info_server_write, get_metadata_env
 from pynumaflow.info.types import (
     ServerInfo,
     Protocol,
     Language,
     METADATA_ENVS,
+    MINIMUM_NUMAFLOW_VERSION,
 )
 from pynumaflow.proto.mapper import map_pb2_grpc
 from pynumaflow.proto.sideinput import sideinput_pb2_grpc
 from pynumaflow.proto.sinker import sink_pb2_grpc
 from pynumaflow.proto.sourcer import source_pb2_grpc
 from pynumaflow.proto.sourcetransformer import transform_pb2_grpc
 
@@ -44,42 +45,40 @@
 def write_info_file(protocol: Protocol, info_file) -> None:
     """
     Write the server info file to the given path.
     """
     serv_info = ServerInfo(
         protocol=protocol,
         language=Language.PYTHON,
+        minimum_numaflow_version=MINIMUM_NUMAFLOW_VERSION,
         version=get_sdk_version(),
     )
     info_server_write(server_info=serv_info, info_file=info_file)
 
 
 def sync_server_start(
     servicer,
     bind_address: str,
     max_threads: int,
     server_info_file: str,
     server_options=None,
     udf_type: str = UDFType.Map,
-    add_info_server=True,
 ):
     """
     Utility function to start a sync grpc server instance.
     """
-    # Add the server information to the server info file,
-    # here we just write the protocol and language information
-    if add_info_server:
-        server_info = ServerInfo(
-            protocol=Protocol.UDS,
-            language=Language.PYTHON,
-            version=get_sdk_version(),
-        )
-    else:
-        server_info = None
-    # Run a sync server instances
+    # Add the server information to the server info file
+    server_info = ServerInfo(
+        protocol=Protocol.UDS,
+        language=Language.PYTHON,
+        minimum_numaflow_version=MINIMUM_NUMAFLOW_VERSION,
+        version=get_sdk_version(),
+    )
+
+    # Run a sync server instance
     _run_server(
         servicer=servicer,
         bind_address=bind_address,
         threads_per_proc=max_threads,
         server_options=server_options,
         udf_type=udf_type,
         server_info_file=server_info_file,
@@ -90,15 +89,15 @@
 def _run_server(
     servicer,
     bind_address: str,
     threads_per_proc,
     server_options,
     udf_type: str,
     server_info_file,
-    server_info=None,
+    server_info,
 ) -> None:
     """
     Starts the Synchronous server instance on the given UNIX socket
     with given max threads. Wait for the server to terminate.
     """
     server = grpc.server(
         ThreadPoolExecutor(
@@ -119,18 +118,15 @@
     elif udf_type == UDFType.SideInput:
         sideinput_pb2_grpc.add_SideInputServicer_to_server(servicer, server)
 
     # bind the server to the UDS/TCP socket
     server.add_insecure_port(bind_address)
     # start the gRPC server
     server.start()
-
-    # Add the server information to the server info file if provided
-    if server_info and server_info_file:
-        info_server_write(server_info=server_info, info_file=server_info_file)
+    info_server_write(server_info=server_info, info_file=server_info_file)
 
     _LOGGER.info("GRPC Server listening on: %s %d", bind_address, os.getpid())
     server.wait_for_termination()
 
 
 def start_multiproc_server(
     max_threads: int,
@@ -175,14 +171,15 @@
 
     # Convert the available ports to a comma separated string
     ports = ",".join(map(str, server_ports))
 
     serv_info = ServerInfo(
         protocol=Protocol.TCP,
         language=Language.PYTHON,
+        minimum_numaflow_version=MINIMUM_NUMAFLOW_VERSION,
         version=get_sdk_version(),
         metadata=get_metadata_env(envs=METADATA_ENVS),
     )
     # Add the PORTS metadata using the available ports
     serv_info.metadata["SERV_PORTS"] = ports
     info_server_write(server_info=serv_info, info_file=server_info_file)
 
@@ -201,18 +198,18 @@
     Starts the Async server instance on the given UNIX socket with given max threads.
     Add the server graceful shutdown coroutine to the cleanup_coroutines list.
     Wait for the server to terminate.
     """
     await server_async.start()
 
     # Add the server information to the server info file
-    # Here we just write the protocol and language information
     serv_info = ServerInfo(
         protocol=Protocol.UDS,
         language=Language.PYTHON,
+        minimum_numaflow_version=MINIMUM_NUMAFLOW_VERSION,
         version=get_sdk_version(),
     )
     info_server_write(server_info=serv_info, info_file=server_info_file)
 
     # Log the server start
     _LOGGER.info(
         "New Async GRPC Server listening on: %s with max threads: %s",
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sideinput/_dtypes.py` & `pynumaflow-0.7.0a1/pynumaflow/sideinput/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sideinput/server.py` & `pynumaflow-0.7.0a1/pynumaflow/sideinput/server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sideinput/servicer/servicer.py` & `pynumaflow-0.7.0a1/pynumaflow/sideinput/servicer/servicer.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sinker/_dtypes.py` & `pynumaflow-0.7.0a1/pynumaflow/sinker/_dtypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,29 +15,41 @@
     """
     Basic datatype for UDSink response.
 
     Args:
         id: the id of the event.
         success: boolean indicating whether the event was successfully processed.
         err: error message if the event was not successfully processed.
+        fallback: fallback is true if the message to be sent to the fallback sink.
     """
 
     id: str
     success: bool
     err: Optional[str]
+    fallback: bool
 
-    __slots__ = ("id", "success", "err")
+    __slots__ = ("id", "success", "err", "fallback")
 
+    # as_success creates a successful Response with the given id.
+    # The Success field is set to true.
     @classmethod
     def as_success(cls: type[R], id_: str) -> R:
-        return Response(id=id_, success=True, err=None)
+        return Response(id=id_, success=True, err=None, fallback=False)
 
+    # as_failure creates a failed Response with the given id and error message.
+    # The success field is set to false and the err field is set to the provided error message.
     @classmethod
     def as_failure(cls: type[R], id_: str, err_msg: str) -> R:
-        return Response(id=id_, success=False, err=err_msg)
+        return Response(id=id_, success=False, err=err_msg, fallback=False)
+
+    # as_fallback creates a Response with the fallback field set to true.
+    # This indicates that the message should be sent to the fallback sink.
+    @classmethod
+    def as_fallback(cls: type[R], id_: str) -> R:
+        return Response(id=id_, fallback=True, err=None, success=False)
 
 
 class Responses(Sequence[R]):
     """
     Container to hold a list of Response instances.
 
     Args:
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sinker/async_server.py` & `pynumaflow-0.7.0a1/pynumaflow/sinker/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,116 @@
 import os
 
-import aiorun
-import grpc
-
-from pynumaflow.sinker.servicer.async_servicer import AsyncSinkServicer
-from pynumaflow.proto.sinker import sink_pb2_grpc
 
+from pynumaflow.sinker.servicer.sync_servicer import SyncSinkServicer
 
 from pynumaflow._constants import (
     SINK_SOCK_PATH,
     MAX_MESSAGE_SIZE,
     MAX_THREADS,
+    _LOGGER,
+    UDFType,
     SINK_SERVER_INFO_FILE_PATH,
+    ENV_UD_CONTAINER_TYPE,
+    UD_CONTAINER_FALLBACK_SINK,
+    FALLBACK_SINK_SOCK_PATH,
+    FALLBACK_SINK_SERVER_INFO_FILE_PATH,
 )
 
-from pynumaflow.shared.server import NumaflowServer, start_async_server
-from pynumaflow.sinker._dtypes import AsyncSinkCallable
+from pynumaflow.shared.server import NumaflowServer, sync_server_start
+from pynumaflow.sinker._dtypes import SyncSinkCallable
 
 
-class SinkAsyncServer(NumaflowServer):
+class SinkServer(NumaflowServer):
     """
-    SinkAsyncServer is the main class to start a gRPC server for a sinker.
-    Create a new grpc Async Sink Server instance.
-    A new servicer instance is created and attached to the server.
-    The server instance is returned.
-    Args:
-        sinker_instance: The sinker instance to be used for Sink UDF
-        sock_path: The UNIX socket path to be used for the server
-        max_message_size: The max message size in bytes the server can receive and send
-        max_threads: The max number of threads to be spawned;
-                        defaults to number of processors x4
-
-    Example invocation:
-        import os
-        from collections.abc import AsyncIterable
-        from pynumaflow.sinker import Datum, Responses, Response, Sinker
-        from pynumaflow.sinker import SinkAsyncServer
-        from pynumaflow._constants import _LOGGER
-
-
-        class UserDefinedSink(Sinker):
-            async def handler(self, datums: AsyncIterable[Datum]) -> Responses:
-                responses = Responses()
-                async for msg in datums:
-                    _LOGGER.info("User Defined Sink %s", msg.value.decode("utf-8"))
-                    responses.append(Response.as_success(msg.id))
-                return responses
-
-
-        async def udsink_handler(datums: AsyncIterable[Datum]) -> Responses:
-            responses = Responses()
-            async for msg in datums:
-                _LOGGER.info("User Defined Sink %s", msg.value.decode("utf-8"))
-                responses.append(Response.as_success(msg.id))
-            return responses
-
-
-        if __name__ == "__main__":
-            invoke = os.getenv("INVOKE", "func_handler")
-            if invoke == "class":
-                sink_handler = UserDefinedSink()
-            else:
-                sink_handler = udsink_handler
-            grpc_server = SinkAsyncServer(sink_handler)
-            grpc_server.start()
+    SinkServer is the main class to start a gRPC server for a sinker.
     """
 
     def __init__(
         self,
-        sinker_instance: AsyncSinkCallable,
+        sinker_instance: SyncSinkCallable,
         sock_path=SINK_SOCK_PATH,
         max_message_size=MAX_MESSAGE_SIZE,
         max_threads=MAX_THREADS,
         server_info_file=SINK_SERVER_INFO_FILE_PATH,
     ):
+        """
+        Create a new grpc Sink Server instance.
+        A new servicer instance is created and attached to the server.
+        The server instance is returned.
+        Args:
+            sinker_instance: The sinker instance to be used for Sink UDF
+            sock_path: The UNIX socket path to be used for the server
+            max_message_size: The max message size in bytes the server can receive and send
+            max_threads: The max number of threads to be spawned;
+                            defaults to number of processors x4
+        Example invocation:
+            import os
+            from collections.abc import Iterator
+
+            from pynumaflow.sinker import Datum, Responses, Response, SinkServer
+            from pynumaflow.sinker import Sinker
+            from pynumaflow._constants import _LOGGER
+
+            class UserDefinedSink(Sinker):
+                def handler(self, datums: Iterator[Datum]) -> Responses:
+                    responses = Responses()
+                    for msg in datums:
+                        _LOGGER.info("User Defined Sink %s", msg.value.decode("utf-8"))
+                        responses.append(Response.as_success(msg.id))
+                    return responses
+
+            def udsink_handler(datums: Iterator[Datum]) -> Responses:
+                responses = Responses()
+                for msg in datums:
+                    _LOGGER.info("User Defined Sink %s", msg.value.decode("utf-8"))
+                    responses.append(Response.as_success(msg.id))
+                return responses
+
+            if __name__ == "__main__":
+                invoke = os.getenv("INVOKE", "func_handler")
+                if invoke == "class":
+                    sink_handler = UserDefinedSink()
+                else:
+                    sink_handler = udsink_handler
+                grpc_server = SinkServer(sink_handler)
+                grpc_server.start()
+
+        """
+        # If the container type is fallback sink, then use the fallback sink address and path.
+        if os.getenv(ENV_UD_CONTAINER_TYPE, "") == UD_CONTAINER_FALLBACK_SINK:
+            _LOGGER.info("Using Fallback Sink")
+            sock_path = FALLBACK_SINK_SOCK_PATH
+            server_info_file = FALLBACK_SINK_SERVER_INFO_FILE_PATH
+
         self.sock_path = f"unix://{sock_path}"
         self.max_threads = min(max_threads, int(os.getenv("MAX_THREADS", "4")))
         self.max_message_size = max_message_size
         self.server_info_file = server_info_file
 
         self.sinker_instance = sinker_instance
 
         self._server_options = [
             ("grpc.max_send_message_length", self.max_message_size),
             ("grpc.max_receive_message_length", self.max_message_size),
         ]
-        self.servicer = AsyncSinkServicer(sinker_instance)
+        self.servicer = SyncSinkServicer(sinker_instance)
 
     def start(self):
         """
-        Starter function for the Async server class, need a separate caller
-        so that all the async coroutines can be started from a single context
-        """
-        aiorun.run(self.aexec(), use_uvloop=True)
-
-    async def aexec(self):
+        Starts the Synchronous gRPC server on the
+        given UNIX socket with given max threads.
         """
-        Starts the Asynchronous gRPC server on the given UNIX socket with given max threads.
-        """
-        # As the server is async, we need to create a new server instance in the
-        # same thread as the event loop so that all the async calls are made in the
-        # same context
-        # Create a new server instance, add the servicer to it and start the server
-        server = grpc.aio.server()
-        server.add_insecure_port(self.sock_path)
-        sink_pb2_grpc.add_SinkServicer_to_server(self.servicer, server)
-        await start_async_server(
-            server, self.sock_path, self.max_threads, self._server_options, self.server_info_file
+        _LOGGER.info(
+            "Sync GRPC Sink listening on: %s with max threads: %s",
+            self.sock_path,
+            self.max_threads,
+        )
+        # Start the server
+        sync_server_start(
+            servicer=self.servicer,
+            bind_address=self.sock_path,
+            max_threads=self.max_threads,
+            server_info_file=self.server_info_file,
+            server_options=self._server_options,
+            udf_type=UDFType.Sink,
         )
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sinker/servicer/async_servicer.py` & `pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/async_servicer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from collections.abc import AsyncIterable
 
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow.sinker._dtypes import Responses, Datum, Response
 from pynumaflow.sinker._dtypes import SyncSinkCallable
 from pynumaflow.proto.sinker import sink_pb2_grpc, sink_pb2
+from pynumaflow.sinker.servicer.utils import build_sink_response
 from pynumaflow.types import NumaflowServicerContext
 from pynumaflow._constants import _LOGGER
 
 
 async def datum_generator(
     request_iterator: AsyncIterable[sink_pb2.SinkRequest],
 ) -> AsyncIterable[Datum]:
     async for d in request_iterator:
         datum = Datum(
             keys=list(d.keys),
             sink_msg_id=d.id,
             value=d.value,
             event_time=d.event_time.ToDatetime(),
             watermark=d.watermark.ToDatetime(),
-            headers=d.headers,
+            headers=dict(d.headers),
         )
         yield datum
 
 
 class AsyncSinkServicer(sink_pb2_grpc.SinkServicer):
     """
     This class is used to create a new grpc Sink servicer instance.
@@ -60,17 +61,15 @@
             err_msg = "UDSinkError: %r" % err
             _LOGGER.critical(err_msg, exc_info=True)
             rspns = Responses()
             async for _datum in datum_iterator:
                 rspns.append(Response.as_failure(_datum.id, err_msg))
         responses = []
         for rspn in rspns:
-            responses.append(
-                sink_pb2.SinkResponse.Result(id=rspn.id, success=rspn.success, err_msg=rspn.err)
-            )
+            responses.append(build_sink_response(rspn))
         return responses
 
     async def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> sink_pb2.ReadyResponse:
         """
         IsReady is the heartbeat endpoint for gRPC.
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sinker/servicer/sync_servicer.py` & `pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/sync_servicer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from collections.abc import Iterator, Iterable
 
 from google.protobuf import empty_pb2 as _empty_pb2
 from pynumaflow._constants import _LOGGER
 from pynumaflow.sinker._dtypes import Responses, Datum, Response
 from pynumaflow.sinker._dtypes import SyncSinkCallable
 from pynumaflow.proto.sinker import sink_pb2_grpc, sink_pb2
+from pynumaflow.sinker.servicer.utils import build_sink_response
 from pynumaflow.types import NumaflowServicerContext
 
 
 def datum_generator(request_iterator: Iterable[sink_pb2.SinkRequest]) -> Iterable[Datum]:
     for d in request_iterator:
         datum = Datum(
             keys=list(d.keys),
             sink_msg_id=d.id,
             value=d.value,
             event_time=d.event_time.ToDatetime(),
             watermark=d.watermark.ToDatetime(),
-            headers=d.headers,
+            headers=dict(d.headers),
         )
         yield datum
 
 
 class SyncSinkServicer(sink_pb2_grpc.SinkServicer):
     """
     This class is used to create a new grpc Sink servicer instance.
@@ -50,17 +51,15 @@
             _LOGGER.critical(err_msg, exc_info=True)
             rspns = Responses()
             for _datum in datum_iterator:
                 rspns.append(Response.as_failure(_datum.id, err_msg))
 
         responses = []
         for rspn in rspns:
-            responses.append(
-                sink_pb2.SinkResponse.Result(id=rspn.id, success=rspn.success, err_msg=rspn.err)
-            )
+            responses.append(build_sink_response(rspn))
 
         return sink_pb2.SinkResponse(results=responses)
 
     def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> sink_pb2.ReadyResponse:
         """
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sourcer/__init__.py` & `pynumaflow-0.7.0a1/pynumaflow/sourcer/__init__.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sourcer/_dtypes.py` & `pynumaflow-0.7.0a1/pynumaflow/sourcer/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sourcer/async_server.py` & `pynumaflow-0.7.0a1/pynumaflow/sourcer/async_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sourcer/server.py` & `pynumaflow-0.7.0a1/pynumaflow/sourcer/server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sourcer/servicer/async_servicer.py` & `pynumaflow-0.7.0a1/pynumaflow/sourcer/servicer/async_servicer.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sourcer/servicer/sync_servicer.py` & `pynumaflow-0.7.0a1/pynumaflow/sourcer/servicer/sync_servicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 event_time_timestamp = _timestamp_pb2.Timestamp()
                 event_time_timestamp.FromDatetime(dt=msg.event_time)
                 yield source_pb2.ReadResponse.Result(
                     payload=msg.payload,
                     keys=msg.keys,
                     offset=msg.offset.as_dict,
                     event_time=event_time_timestamp,
-                    headers=msg.headers,
+                    headers=dict(msg.headers),
                 )
         except Exception as err:
             _LOGGER.critical("User-Defined Source ReadError ", exc_info=True)
             raise err
 
     def AckFn(
         self, request: source_pb2.AckRequest, context: NumaflowServicerContext
```

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sourcetransformer/_dtypes.py` & `pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sourcetransformer/multiproc_server.py` & `pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/multiproc_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sourcetransformer/server.py` & `pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a0/pynumaflow/sourcetransformer/servicer/server.py` & `pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/servicer/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             msgts = self.__transform_handler(
                 list(request.keys),
                 Datum(
                     keys=list(request.keys),
                     value=request.value,
                     event_time=request.event_time.ToDatetime(),
                     watermark=request.watermark.ToDatetime(),
-                    headers=request.headers,
+                    headers=dict(request.headers),
                 ),
             )
         except Exception as err:
             _LOGGER.critical("UDFError, re-raising the error", exc_info=True)
             context.set_code(grpc.StatusCode.UNKNOWN)
             context.set_details(str(err))
             return transform_pb2.SourceTransformResponse(results=[])
```

### Comparing `pynumaflow-0.7.0a0/pyproject.toml` & `pynumaflow-0.7.0a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynumaflow"
-version = "0.7.0a0"
+version = "0.7.0a1"
 description = "Provides the interfaces of writing Python User Defined Functions and Sinks for NumaFlow."
 authors = ["NumaFlow Developers"]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Vigith Maurice <vigith@gmail.com>",
```

### Comparing `pynumaflow-0.7.0a0/PKG-INFO` & `pynumaflow-0.7.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumaflow
-Version: 0.7.0a0
+Version: 0.7.0a1
 Summary: Provides the interfaces of writing Python User Defined Functions and Sinks for NumaFlow.
 Home-page: https://github.com/numaproj/numaflow-python
 License: Apache-2.0
 Author: NumaFlow Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -23,15 +23,15 @@
 Requires-Dist: protobuf (>=3.20,<5.0)
 Requires-Dist: uvloop (>=0.19.0,<0.20.0)
 Project-URL: Repository, https://github.com/numaproj/numaflow-python
 Description-Content-Type: text/markdown
 
 # Python SDK for Numaflow
 
-[![Build](https://github.com/numaproj/numaflow-python/actions/workflows/ci.yml/badge.svg)](https://github.com/numaproj/numaflow-python/actions/workflows/ci.yml)
+[![Build](https://github.com/numaproj/numaflow-python/actions/workflows/run-tests.yml/badge.svg)](https://github.com/numaproj/numaflow-python/actions/workflows/run-tests.yml)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
 [![Release Version](https://img.shields.io/github/v/release/numaproj/numaflow-python?label=pynumaflow)](https://github.com/numaproj/numaflow-python/releases/latest)
 
 This is the Python SDK for [Numaflow](https://numaflow.numaproj.io/).
 
 This SDK provides the interface for writing different functionalities of Numaflow like [UDFs](https://numaflow.numaproj.io/user-guide/user-defined-functions/user-defined-functions/), [UDSinks](https://numaflow.numaproj.io/user-guide/sinks/user-defined-sinks/), [UDSources](https://numaflow.numaproj.io/user-guide/sources/user-defined-sources/) and [SideInput](https://numaflow.numaproj.io/specifications/side-inputs/) in Python.
```


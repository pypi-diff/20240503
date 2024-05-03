# Comparing `tmp/qdrant_client-1.9.0.tar.gz` & `tmp/qdrant_client-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_client-1.9.0.tar", max compression
+gzip compressed data, was "qdrant_client-1.9.1.tar", max compression
```

## Comparing `qdrant_client-1.9.0.tar` & `qdrant_client-1.9.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    11357 2024-04-22 13:35:21.717240 qdrant_client-1.9.0/LICENSE
--rw-r--r--   0        0        0     8203 2024-04-22 13:35:21.717240 qdrant_client-1.9.0/README.md
--rw-r--r--   0        0        0     2118 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      128 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/__init__.py
--rw-r--r--   0        0        0      891 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/_pydantic_compat.py
--rw-r--r--   0        0        0    13738 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/async_client_base.py
--rw-r--r--   0        0        0   104316 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/async_qdrant_client.py
--rw-r--r--   0        0        0    25772 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/async_qdrant_fastembed.py
--rw-r--r--   0        0        0   110852 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/async_qdrant_remote.py
--rw-r--r--   0        0        0       54 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/auth/__init__.py
--rw-r--r--   0        0        0     1567 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/auth/bearer_auth.py
--rw-r--r--   0        0        0    13555 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/client_base.py
--rw-r--r--   0        0        0    10047 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/connection.py
--rw-r--r--   0        0        0        0 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/conversions/__init__.py
--rw-r--r--   0        0        0     5014 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/conversions/common_types.py
--rw-r--r--   0        0        0   118493 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/conversions/conversion.py
--rw-r--r--   0        0        0      414 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/fastembed_common.py
--rw-r--r--   0        0        0      252 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/__init__.py
--rw-r--r--   0        0        0    55332 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/collections_pb2.py
--rw-r--r--   0        0        0      159 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/collections_pb2_grpc.py
--rw-r--r--   0        0        0     2501 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/collections_service_pb2.py
--rw-r--r--   0        0        0    21674 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/collections_service_pb2_grpc.py
--rw-r--r--   0        0        0     3499 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/json_with_int_pb2.py
--rw-r--r--   0        0        0      159 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/json_with_int_pb2_grpc.py
--rw-r--r--   0        0        0    79326 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/points_pb2.py
--rw-r--r--   0        0        0      159 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/points_pb2_grpc.py
--rw-r--r--   0        0        0     3185 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/points_service_pb2.py
--rw-r--r--   0        0        0    35635 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/points_service_pb2_grpc.py
--rw-r--r--   0        0        0     2433 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/qdrant_pb2.py
--rw-r--r--   0        0        0     2411 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/qdrant_pb2_grpc.py
--rw-r--r--   0        0        0     7842 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/snapshots_service_pb2.py
--rw-r--r--   0        0        0    10406 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/grpc/snapshots_service_pb2_grpc.py
--rw-r--r--   0        0        0      605 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/http/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/http/api/__init__.py
--rw-r--r--   0        0        0    10329 2024-04-22 13:35:21.725240 qdrant_client-1.9.0/qdrant_client/http/api/cluster_api.py
--rw-r--r--   0        0        0    44807 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/http/api/collections_api.py
--rw-r--r--   0        0        0    48992 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/http/api/points_api.py
--rw-r--r--   0        0        0     9003 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/http/api/service_api.py
--rw-r--r--   0        0        0    27690 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/http/api/snapshots_api.py
--rw-r--r--   0        0        0     7990 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/http/api_client.py
--rw-r--r--   0        0        0      233 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/http/configuration.py
--rw-r--r--   0        0        0     1616 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/http/exceptions.py
--rw-r--r--   0        0        0       22 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/http/models/__init__.py
--rw-r--r--   0        0        0   100408 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/http/models/models.py
--rw-r--r--   0        0        0        0 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/hybrid/__init__.py
--rw-r--r--   0        0        0     1083 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/hybrid/fusion.py
--rw-r--r--   0        0        0      799 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/hybrid/test_reranking.py
--rw-r--r--   0        0        0        0 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/__init__.py
--rw-r--r--   0        0        0    33972 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/async_qdrant_local.py
--rw-r--r--   0        0        0     1689 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/datetime_utils.py
--rw-r--r--   0        0        0     8771 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/distances.py
--rw-r--r--   0        0        0     2883 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/geo.py
--rw-r--r--   0        0        0     3911 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/json_path_parser.py
--rw-r--r--   0        0        0    62911 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/local_collection.py
--rw-r--r--   0        0        0      727 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/order_by.py
--rw-r--r--   0        0        0     9901 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/payload_filters.py
--rw-r--r--   0        0        0     2626 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/payload_value_extractor.py
--rw-r--r--   0        0        0     7156 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/payload_value_setter.py
--rw-r--r--   0        0        0     5587 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/persistence.py
--rw-r--r--   0        0        0    34399 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/qdrant_local.py
--rw-r--r--   0        0        0     1020 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/sparse.py
--rw-r--r--   0        0        0     7667 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/sparse_distances.py
--rw-r--r--   0        0        0        0 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/tests/__init__.py
--rw-r--r--   0        0        0     2451 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/tests/test_datetimes.py
--rw-r--r--   0        0        0     1953 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/tests/test_distances.py
--rw-r--r--   0        0        0     5387 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/tests/test_payload_filters.py
--rw-r--r--   0        0        0    18264 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/local/tests/test_payload_utils.py
--rw-r--r--   0        0        0       29 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/migrate/__init__.py
--rw-r--r--   0        0        0     6425 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/migrate/migrate.py
--rw-r--r--   0        0        0       85 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/models/__init__.py
--rw-r--r--   0        0        0     7034 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/parallel_processor.py
--rw-r--r--   0        0        0    20066 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/proto/collections.proto
--rw-r--r--   0        0        0     1894 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/proto/collections_service.proto
--rw-r--r--   0        0        0     1984 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/proto/json_with_int.proto
--rw-r--r--   0        0        0    31059 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/proto/points.proto
--rw-r--r--   0        0        0     4257 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/proto/points_service.proto
--rw-r--r--   0        0        0      408 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/proto/qdrant.proto
--rw-r--r--   0        0        0     1970 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/proto/snapshots_service.proto
--rw-r--r--   0        0        0        8 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/py.typed
--rw-r--r--   0        0        0   105934 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/qdrant_client.py
--rw-r--r--   0        0        0    26141 2024-04-22 13:35:21.729240 qdrant_client-1.9.0/qdrant_client/qdrant_fastembed.py
--rw-r--r--   0        0        0   111908 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_client/qdrant_remote.py
--rw-r--r--   0        0        0        0 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_client/uploader/__init__.py
--rw-r--r--   0        0        0     3660 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_client/uploader/grpc_uploader.py
--rw-r--r--   0        0        0     2874 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_client/uploader/rest_uploader.py
--rw-r--r--   0        0        0     3366 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_client/uploader/uploader.py
--rw-r--r--   0        0        0      267 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_openapi_client/__init__.py
--rw-r--r--   0        0        0       37 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_openapi_client/api/__init__.py
--rw-r--r--   0        0        0       53 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_openapi_client/api/collections_api.py
--rw-r--r--   0        0        0       48 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_openapi_client/api/points_api.py
--rw-r--r--   0        0        0       44 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_openapi_client/exceptions.py
--rw-r--r--   0        0        0       47 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_openapi_client/models/__init__.py
--rw-r--r--   0        0        0       47 2024-04-22 13:35:21.733240 qdrant_client-1.9.0/qdrant_openapi_client/models/models.py
--rw-r--r--   0        0        0     9529 1970-01-01 00:00:00.000000 qdrant_client-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-03 19:22:46.783005 qdrant_client-1.9.1/LICENSE
+-rw-r--r--   0        0        0     8203 2024-05-03 19:22:46.783005 qdrant_client-1.9.1/README.md
+-rw-r--r--   0        0        0     2118 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/__init__.py
+-rw-r--r--   0        0        0      891 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/_pydantic_compat.py
+-rw-r--r--   0        0        0    13738 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/async_client_base.py
+-rw-r--r--   0        0        0   104318 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/async_qdrant_client.py
+-rw-r--r--   0        0        0    25772 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/async_qdrant_fastembed.py
+-rw-r--r--   0        0        0   110852 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/async_qdrant_remote.py
+-rw-r--r--   0        0        0       54 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/auth/__init__.py
+-rw-r--r--   0        0        0     1567 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/auth/bearer_auth.py
+-rw-r--r--   0        0        0    13555 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/client_base.py
+-rw-r--r--   0        0        0    10047 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/connection.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/conversions/__init__.py
+-rw-r--r--   0        0        0     5014 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/conversions/common_types.py
+-rw-r--r--   0        0        0   118493 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/conversions/conversion.py
+-rw-r--r--   0        0        0      414 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/fastembed_common.py
+-rw-r--r--   0        0        0      252 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/__init__.py
+-rw-r--r--   0        0        0    55332 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/collections_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/collections_pb2_grpc.py
+-rw-r--r--   0        0        0     2501 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/collections_service_pb2.py
+-rw-r--r--   0        0        0    21674 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/collections_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3499 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/json_with_int_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/json_with_int_pb2_grpc.py
+-rw-r--r--   0        0        0    79326 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/points_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/points_pb2_grpc.py
+-rw-r--r--   0        0        0     3185 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/points_service_pb2.py
+-rw-r--r--   0        0        0    35635 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/points_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2433 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/qdrant_pb2.py
+-rw-r--r--   0        0        0     2411 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/qdrant_pb2_grpc.py
+-rw-r--r--   0        0        0     7842 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/snapshots_service_pb2.py
+-rw-r--r--   0        0        0    10406 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/grpc/snapshots_service_pb2_grpc.py
+-rw-r--r--   0        0        0      605 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/http/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/http/api/__init__.py
+-rw-r--r--   0        0        0    10329 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/http/api/cluster_api.py
+-rw-r--r--   0        0        0    44807 2024-05-03 19:22:46.787005 qdrant_client-1.9.1/qdrant_client/http/api/collections_api.py
+-rw-r--r--   0        0        0    48992 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/http/api/points_api.py
+-rw-r--r--   0        0        0     9003 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/http/api/service_api.py
+-rw-r--r--   0        0        0    27690 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/http/api/snapshots_api.py
+-rw-r--r--   0        0        0     7990 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/http/api_client.py
+-rw-r--r--   0        0        0      233 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/http/configuration.py
+-rw-r--r--   0        0        0     1616 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/http/exceptions.py
+-rw-r--r--   0        0        0       22 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/http/models/__init__.py
+-rw-r--r--   0        0        0   100408 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/http/models/models.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/hybrid/__init__.py
+-rw-r--r--   0        0        0     1083 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/hybrid/fusion.py
+-rw-r--r--   0        0        0      799 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/hybrid/test_reranking.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/__init__.py
+-rw-r--r--   0        0        0    33972 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/async_qdrant_local.py
+-rw-r--r--   0        0        0     1689 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/datetime_utils.py
+-rw-r--r--   0        0        0     8771 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/distances.py
+-rw-r--r--   0        0        0     2883 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/geo.py
+-rw-r--r--   0        0        0     3911 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/json_path_parser.py
+-rw-r--r--   0        0        0    62911 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/local_collection.py
+-rw-r--r--   0        0        0      727 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/order_by.py
+-rw-r--r--   0        0        0    10280 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/payload_filters.py
+-rw-r--r--   0        0        0     2626 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/payload_value_extractor.py
+-rw-r--r--   0        0        0     7156 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/payload_value_setter.py
+-rw-r--r--   0        0        0     5587 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/persistence.py
+-rw-r--r--   0        0        0    34399 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/qdrant_local.py
+-rw-r--r--   0        0        0     1020 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/sparse.py
+-rw-r--r--   0        0        0     7667 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/sparse_distances.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/tests/__init__.py
+-rw-r--r--   0        0        0     2451 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/tests/test_datetimes.py
+-rw-r--r--   0        0        0     1953 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/tests/test_distances.py
+-rw-r--r--   0        0        0     5387 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/tests/test_payload_filters.py
+-rw-r--r--   0        0        0    18264 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/local/tests/test_payload_utils.py
+-rw-r--r--   0        0        0       29 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/migrate/__init__.py
+-rw-r--r--   0        0        0     6425 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/migrate/migrate.py
+-rw-r--r--   0        0        0       85 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/models/__init__.py
+-rw-r--r--   0        0        0     7034 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/parallel_processor.py
+-rw-r--r--   0        0        0    20066 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/proto/collections.proto
+-rw-r--r--   0        0        0     1894 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/proto/collections_service.proto
+-rw-r--r--   0        0        0     1984 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/proto/json_with_int.proto
+-rw-r--r--   0        0        0    31059 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/proto/points.proto
+-rw-r--r--   0        0        0     4257 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/proto/points_service.proto
+-rw-r--r--   0        0        0      408 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/proto/qdrant.proto
+-rw-r--r--   0        0        0     1970 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/proto/snapshots_service.proto
+-rw-r--r--   0        0        0        8 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/py.typed
+-rw-r--r--   0        0        0   105936 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/qdrant_client.py
+-rw-r--r--   0        0        0    26141 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/qdrant_fastembed.py
+-rw-r--r--   0        0        0   111908 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/qdrant_remote.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/uploader/__init__.py
+-rw-r--r--   0        0        0     3660 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/uploader/grpc_uploader.py
+-rw-r--r--   0        0        0     2874 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/uploader/rest_uploader.py
+-rw-r--r--   0        0        0     3366 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_client/uploader/uploader.py
+-rw-r--r--   0        0        0      267 2024-05-03 19:22:46.791005 qdrant_client-1.9.1/qdrant_openapi_client/__init__.py
+-rw-r--r--   0        0        0       37 2024-05-03 19:22:46.795005 qdrant_client-1.9.1/qdrant_openapi_client/api/__init__.py
+-rw-r--r--   0        0        0       53 2024-05-03 19:22:46.795005 qdrant_client-1.9.1/qdrant_openapi_client/api/collections_api.py
+-rw-r--r--   0        0        0       48 2024-05-03 19:22:46.795005 qdrant_client-1.9.1/qdrant_openapi_client/api/points_api.py
+-rw-r--r--   0        0        0       44 2024-05-03 19:22:46.795005 qdrant_client-1.9.1/qdrant_openapi_client/exceptions.py
+-rw-r--r--   0        0        0       47 2024-05-03 19:22:46.795005 qdrant_client-1.9.1/qdrant_openapi_client/models/__init__.py
+-rw-r--r--   0        0        0       47 2024-05-03 19:22:46.795005 qdrant_client-1.9.1/qdrant_openapi_client/models/models.py
+-rw-r--r--   0        0        0     9529 1970-01-01 00:00:00.000000 qdrant_client-1.9.1/PKG-INFO
```

### Comparing `qdrant_client-1.9.0/LICENSE` & `qdrant_client-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/README.md` & `qdrant_client-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/pyproject.toml` & `qdrant_client-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qdrant-client"
-version = "1.9.0"
+version = "1.9.1"
 description = "Client library for the Qdrant vector search engine"
 authors = ["Andrey Vasnetsov <andrey@qdrant.tech>"]
 packages = [
     {include = "qdrant_client"},
     {include = "qdrant_openapi_client"}
 ]
 license = "Apache-2.0"
```

### Comparing `qdrant_client-1.9.0/qdrant_client/_pydantic_compat.py` & `qdrant_client-1.9.1/qdrant_client/_pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/async_client_base.py` & `qdrant_client-1.9.1/qdrant_client/async_client_base.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/async_qdrant_client.py` & `qdrant_client-1.9.1/qdrant_client/async_qdrant_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     .. note::
         If you need async, please consider using Async Implementations of QdrantClient.
 
         - :class:`qdrant_client.async_qdrant_client`
 
     Args:
         location:
-            If `:memory:` - use in-memory Qdrant instance.
+            If `":memory:"` - use in-memory Qdrant instance.
             If `str` - use it as a `url` parameter.
             If `None` - use default values for `host` and `port`.
         url: either host or str of "Optional[scheme], host, Optional[port], Optional[prefix]".
             Default: `None`
         port: Port of the REST API interface. Default: 6333
         grpc_port: Port of the gRPC interface. Default: 6334
         prefer_grpc: If `true` - use gPRC interface whenever possible in custom methods.
```

### Comparing `qdrant_client-1.9.0/qdrant_client/async_qdrant_fastembed.py` & `qdrant_client-1.9.1/qdrant_client/async_qdrant_fastembed.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/async_qdrant_remote.py` & `qdrant_client-1.9.1/qdrant_client/async_qdrant_remote.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/auth/bearer_auth.py` & `qdrant_client-1.9.1/qdrant_client/auth/bearer_auth.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/client_base.py` & `qdrant_client-1.9.1/qdrant_client/client_base.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/connection.py` & `qdrant_client-1.9.1/qdrant_client/connection.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/conversions/common_types.py` & `qdrant_client-1.9.1/qdrant_client/conversions/common_types.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/conversions/conversion.py` & `qdrant_client-1.9.1/qdrant_client/conversions/conversion.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/grpc/collections_pb2.py` & `qdrant_client-1.9.1/qdrant_client/grpc/collections_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/grpc/collections_service_pb2.py` & `qdrant_client-1.9.1/qdrant_client/grpc/collections_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/grpc/collections_service_pb2_grpc.py` & `qdrant_client-1.9.1/qdrant_client/grpc/collections_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/grpc/json_with_int_pb2.py` & `qdrant_client-1.9.1/qdrant_client/grpc/json_with_int_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/grpc/points_pb2.py` & `qdrant_client-1.9.1/qdrant_client/grpc/points_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/grpc/points_service_pb2.py` & `qdrant_client-1.9.1/qdrant_client/grpc/points_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/grpc/points_service_pb2_grpc.py` & `qdrant_client-1.9.1/qdrant_client/grpc/points_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/grpc/qdrant_pb2.py` & `qdrant_client-1.9.1/qdrant_client/grpc/qdrant_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/grpc/qdrant_pb2_grpc.py` & `qdrant_client-1.9.1/qdrant_client/grpc/qdrant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/grpc/snapshots_service_pb2.py` & `qdrant_client-1.9.1/qdrant_client/grpc/snapshots_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/grpc/snapshots_service_pb2_grpc.py` & `qdrant_client-1.9.1/qdrant_client/grpc/snapshots_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/http/__init__.py` & `qdrant_client-1.9.1/qdrant_client/http/__init__.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/http/api/cluster_api.py` & `qdrant_client-1.9.1/qdrant_client/http/api/cluster_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/http/api/collections_api.py` & `qdrant_client-1.9.1/qdrant_client/http/api/collections_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/http/api/points_api.py` & `qdrant_client-1.9.1/qdrant_client/http/api/points_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/http/api/service_api.py` & `qdrant_client-1.9.1/qdrant_client/http/api/service_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/http/api/snapshots_api.py` & `qdrant_client-1.9.1/qdrant_client/http/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/http/api_client.py` & `qdrant_client-1.9.1/qdrant_client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/http/exceptions.py` & `qdrant_client-1.9.1/qdrant_client/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/http/models/models.py` & `qdrant_client-1.9.1/qdrant_client/http/models/models.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/hybrid/fusion.py` & `qdrant_client-1.9.1/qdrant_client/hybrid/fusion.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/hybrid/test_reranking.py` & `qdrant_client-1.9.1/qdrant_client/hybrid/test_reranking.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/async_qdrant_local.py` & `qdrant_client-1.9.1/qdrant_client/local/async_qdrant_local.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/datetime_utils.py` & `qdrant_client-1.9.1/qdrant_client/local/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/distances.py` & `qdrant_client-1.9.1/qdrant_client/local/distances.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/geo.py` & `qdrant_client-1.9.1/qdrant_client/local/geo.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/json_path_parser.py` & `qdrant_client-1.9.1/qdrant_client/local/json_path_parser.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/local_collection.py` & `qdrant_client-1.9.1/qdrant_client/local/local_collection.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/order_by.py` & `qdrant_client-1.9.1/qdrant_client/local/order_by.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/payload_filters.py` & `qdrant_client-1.9.1/qdrant_client/local/payload_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,27 @@
 
 
 def check_geo_bounding_box(condition: models.GeoBoundingBox, values: Any) -> bool:
     if isinstance(values, dict) and "lat" in values and "lon" in values:
         lat = values["lat"]
         lon = values["lon"]
 
+        # handle anti-meridian crossing case
+        if condition.top_left.lon > condition.bottom_right.lon:
+            longitude_condition = (
+                (condition.top_left.lon <= lon <= 180 or -180 <= lon <= condition.bottom_right.lon)
+            )
+        else:
+            longitude_condition = (condition.top_left.lon <= lon <= condition.bottom_right.lon)
+
+        latitude_condition = condition.top_left.lat >= lat >= condition.bottom_right.lat
+
         return (
-            condition.top_left.lat >= lat >= condition.bottom_right.lat
-            and condition.top_left.lon <= lon <= condition.bottom_right.lon
+            longitude_condition
+            and latitude_condition
         )
 
     return False
 
 
 def check_geo_polygon(condition: models.GeoPolygon, values: Any) -> bool:
     if isinstance(values, dict) and "lat" in values and "lon" in values:
```

### Comparing `qdrant_client-1.9.0/qdrant_client/local/payload_value_extractor.py` & `qdrant_client-1.9.1/qdrant_client/local/payload_value_extractor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/payload_value_setter.py` & `qdrant_client-1.9.1/qdrant_client/local/payload_value_setter.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/persistence.py` & `qdrant_client-1.9.1/qdrant_client/local/persistence.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/qdrant_local.py` & `qdrant_client-1.9.1/qdrant_client/local/qdrant_local.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/sparse.py` & `qdrant_client-1.9.1/qdrant_client/local/sparse.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/sparse_distances.py` & `qdrant_client-1.9.1/qdrant_client/local/sparse_distances.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/tests/test_datetimes.py` & `qdrant_client-1.9.1/qdrant_client/local/tests/test_datetimes.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/tests/test_distances.py` & `qdrant_client-1.9.1/qdrant_client/local/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/tests/test_payload_filters.py` & `qdrant_client-1.9.1/qdrant_client/local/tests/test_payload_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/local/tests/test_payload_utils.py` & `qdrant_client-1.9.1/qdrant_client/local/tests/test_payload_utils.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/migrate/migrate.py` & `qdrant_client-1.9.1/qdrant_client/migrate/migrate.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/parallel_processor.py` & `qdrant_client-1.9.1/qdrant_client/parallel_processor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/proto/collections.proto` & `qdrant_client-1.9.1/qdrant_client/proto/collections.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/proto/collections_service.proto` & `qdrant_client-1.9.1/qdrant_client/proto/collections_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/proto/json_with_int.proto` & `qdrant_client-1.9.1/qdrant_client/proto/json_with_int.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/proto/points.proto` & `qdrant_client-1.9.1/qdrant_client/proto/points.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/proto/points_service.proto` & `qdrant_client-1.9.1/qdrant_client/proto/points_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/proto/snapshots_service.proto` & `qdrant_client-1.9.1/qdrant_client/proto/snapshots_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/qdrant_client.py` & `qdrant_client-1.9.1/qdrant_client/qdrant_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     .. note::
         If you need async, please consider using Async Implementations of QdrantClient.
 
         - :class:`qdrant_client.async_qdrant_client`
 
     Args:
         location:
-            If `:memory:` - use in-memory Qdrant instance.
+            If `":memory:"` - use in-memory Qdrant instance.
             If `str` - use it as a `url` parameter.
             If `None` - use default values for `host` and `port`.
         url: either host or str of "Optional[scheme], host, Optional[port], Optional[prefix]".
             Default: `None`
         port: Port of the REST API interface. Default: 6333
         grpc_port: Port of the gRPC interface. Default: 6334
         prefer_grpc: If `true` - use gPRC interface whenever possible in custom methods.
```

### Comparing `qdrant_client-1.9.0/qdrant_client/qdrant_fastembed.py` & `qdrant_client-1.9.1/qdrant_client/qdrant_fastembed.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/qdrant_remote.py` & `qdrant_client-1.9.1/qdrant_client/qdrant_remote.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/uploader/grpc_uploader.py` & `qdrant_client-1.9.1/qdrant_client/uploader/grpc_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/uploader/rest_uploader.py` & `qdrant_client-1.9.1/qdrant_client/uploader/rest_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/qdrant_client/uploader/uploader.py` & `qdrant_client-1.9.1/qdrant_client/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.9.0/PKG-INFO` & `qdrant_client-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-client
-Version: 1.9.0
+Version: 1.9.1
 Summary: Client library for the Qdrant vector search engine
 Home-page: https://github.com/qdrant/qdrant-client
 License: Apache-2.0
 Keywords: vector,search,neural,matching,client
 Author: Andrey Vasnetsov
 Author-email: andrey@qdrant.tech
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qdrant-client Version: 1.9.0 Summary: Client
+Metadata-Version: 2.1 Name: qdrant-client Version: 1.9.1 Summary: Client
 library for the Qdrant vector search engine Home-page: https://github.com/
 qdrant/qdrant-client License: Apache-2.0 Keywords:
 vector,search,neural,matching,client Author: Andrey Vasnetsov Author-email:
 andrey@qdrant.tech Requires-Python: >=3.8 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```


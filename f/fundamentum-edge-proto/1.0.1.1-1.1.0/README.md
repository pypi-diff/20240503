# Comparing `tmp/fundamentum_edge_proto-1.0.1.1.tar.gz` & `tmp/fundamentum_edge_proto-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundamentum_edge_proto-1.0.1.1.tar", last modified: Mon Mar 25 19:08:19 2024, max compression
+gzip compressed data, was "fundamentum_edge_proto-1.1.0.tar", last modified: Fri May  3 20:22:48 2024, max compression
```

## Comparing `fundamentum_edge_proto-1.0.1.1.tar` & `fundamentum_edge_proto-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-03-25 19:08:06.235083 fundamentum_edge_proto-1.0.1.1/LICENSE
--rw-r--r--   0        0        0      450 2024-03-25 19:08:06.235083 fundamentum_edge_proto-1.0.1.1/README.md
--rw-r--r--   0        0        0     1432 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/__init__.py
--rw-r--r--   0        0        0     1716 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/configuration_pb2.py
--rw-r--r--   0        0        0      648 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/configuration_pb2.pyi
--rw-r--r--   0        0        0     4348 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     2515 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/configuration_pb2_grpc.pyi
--rw-r--r--   0        0        0     1832 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/provisioning_pb2.py
--rw-r--r--   0        0        0     1352 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/provisioning_pb2.pyi
--rw-r--r--   0        0        0     2899 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/provisioning_pb2_grpc.py
--rw-r--r--   0        0        0     2337 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/provisioning_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/py.typed
--rw-r--r--   0        0        0     1808 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/telemetry_pb2.py
--rw-r--r--   0        0        0     1018 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/telemetry_pb2.pyi
--rw-r--r--   0        0        0     2747 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/telemetry_pb2_grpc.py
--rw-r--r--   0        0        0     1880 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/telemetry_pb2_grpc.pyi
--rw-r--r--   0        0        0     1917 2024-03-25 19:08:08.179090 fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/typed_stubs.py
--rw-r--r--   0        0        0     1735 2024-03-25 19:08:19.107125 fundamentum_edge_proto-1.0.1.1/pyproject.toml
--rw-r--r--   0        0        0    13796 1970-01-01 00:00:00.000000 fundamentum_edge_proto-1.0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-03 20:22:37.431906 fundamentum_edge_proto-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1161 2024-05-03 20:22:37.431906 fundamentum_edge_proto-1.1.0/README.md
+-rw-r--r--   0        0        0     1878 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/__init__.py
+-rw-r--r--   0        0        0     1430 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2.py
+-rw-r--r--   0        0        0      660 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2.pyi
+-rw-r--r--   0        0        0     3362 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     2139 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1539 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2.py
+-rw-r--r--   0        0        0     1352 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2.pyi
+-rw-r--r--   0        0        0     2223 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2_grpc.py
+-rw-r--r--   0        0        0     2078 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/py.typed
+-rw-r--r--   0        0        0      875 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/qos_pb2.py
+-rw-r--r--   0        0        0      471 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/qos_pb2.pyi
+-rw-r--r--   0        0        0       87 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/qos_pb2_grpc.py
+-rw-r--r--   0        0        0      382 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/qos_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1989 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2.py
+-rw-r--r--   0        0        0     1666 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2.pyi
+-rw-r--r--   0        0        0     2180 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2_grpc.py
+-rw-r--r--   0        0        0     1771 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/states_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1360 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2.py
+-rw-r--r--   0        0        0      726 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2.pyi
+-rw-r--r--   0        0        0     2158 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2_grpc.py
+-rw-r--r--   0        0        0     1703 2024-05-03 20:22:39.363914 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2429 2024-05-03 20:22:39.367915 fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/typed_stubs.py
+-rw-r--r--   0        0        0     2153 2024-05-03 20:22:48.047951 fundamentum_edge_proto-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    14505 1970-01-01 00:00:00.000000 fundamentum_edge_proto-1.1.0/PKG-INFO
```

### Comparing `fundamentum_edge_proto-1.0.1.1/LICENSE` & `fundamentum_edge_proto-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/configuration_pb2.pyi` & `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from google.protobuf import empty_pb2 as _empty_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
-
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ConfigData(_message.Message):
-    __slots__ = ("payload",)
+    __slots__ = ('payload',)
     PAYLOAD_FIELD_NUMBER: _ClassVar[int]
     payload: bytes
-    def __init__(self, payload: _Optional[bytes] = ...) -> None: ...
+
+    def __init__(self, payload: _Optional[bytes]=...) -> None:
+        ...
 
 class UpdateData(_message.Message):
-    __slots__ = ("payload",)
+    __slots__ = ('payload',)
     PAYLOAD_FIELD_NUMBER: _ClassVar[int]
     payload: bytes
-    def __init__(self, payload: _Optional[bytes] = ...) -> None: ...
+
+    def __init__(self, payload: _Optional[bytes]=...) -> None:
+        ...
```

### Comparing `fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/configuration_pb2_grpc.pyi` & `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/configuration_pb2_grpc.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,49 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import collections.abc
-import fundamentum_edge_proto.configuration_pb2
+from . import configuration_pb2
 import google.protobuf.empty_pb2
 import grpc
 import grpc.aio
 import typing
-
 _T = typing.TypeVar('_T')
 
 class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta):
     ...
 
-class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore
+class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):
     ...
 
 class ConfigurationStub:
     """Fundamentum Edge's configuration service."""
 
-    def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None: ...
-    Get: grpc.UnaryUnaryMultiCallable[
-        google.protobuf.empty_pb2.Empty,
-        fundamentum_edge_proto.configuration_pb2.ConfigData,
-    ]
-    """Get the device's current configuration."""
-    UpdateStream: grpc.UnaryStreamMultiCallable[
-        google.protobuf.empty_pb2.Empty,
-        fundamentum_edge_proto.configuration_pb2.UpdateData,
-    ]
-    """Subscribe to configuration updates."""
+    def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None:
+        ...
+    Get: grpc.UnaryUnaryMultiCallable[google.protobuf.empty_pb2.Empty, configuration_pb2.ConfigData]
+    "Get the device's current configuration."
+    UpdateStream: grpc.UnaryStreamMultiCallable[google.protobuf.empty_pb2.Empty, configuration_pb2.UpdateData]
+    'Subscribe to configuration updates.'
 
 class ConfigurationAsyncStub:
     """Fundamentum Edge's configuration service."""
-
-    Get: grpc.aio.UnaryUnaryMultiCallable[
-        google.protobuf.empty_pb2.Empty,
-        fundamentum_edge_proto.configuration_pb2.ConfigData,
-    ]
-    """Get the device's current configuration."""
-    UpdateStream: grpc.aio.UnaryStreamMultiCallable[
-        google.protobuf.empty_pb2.Empty,
-        fundamentum_edge_proto.configuration_pb2.UpdateData,
-    ]
-    """Subscribe to configuration updates."""
+    Get: grpc.aio.UnaryUnaryMultiCallable[google.protobuf.empty_pb2.Empty, configuration_pb2.ConfigData]
+    "Get the device's current configuration."
+    UpdateStream: grpc.aio.UnaryStreamMultiCallable[google.protobuf.empty_pb2.Empty, configuration_pb2.UpdateData]
+    'Subscribe to configuration updates.'
 
 class ConfigurationServicer(metaclass=abc.ABCMeta):
     """Fundamentum Edge's configuration service."""
 
     @abc.abstractmethod
-    def Get(
-        self,
-        request: google.protobuf.empty_pb2.Empty,
-        context: _ServicerContext,
-    ) -> typing.Union[fundamentum_edge_proto.configuration_pb2.ConfigData, collections.abc.Awaitable[fundamentum_edge_proto.configuration_pb2.ConfigData]]:
+    def Get(self, request: google.protobuf.empty_pb2.Empty, context: _ServicerContext) -> typing.Union[configuration_pb2.ConfigData, collections.abc.Awaitable[configuration_pb2.ConfigData]]:
         """Get the device's current configuration."""
+
     @abc.abstractmethod
-    def UpdateStream(
-        self,
-        request: google.protobuf.empty_pb2.Empty,
-        context: _ServicerContext,
-    ) -> typing.Union[collections.abc.Iterator[fundamentum_edge_proto.configuration_pb2.UpdateData], collections.abc.AsyncIterator[fundamentum_edge_proto.configuration_pb2.UpdateData]]:
+    def UpdateStream(self, request: google.protobuf.empty_pb2.Empty, context: _ServicerContext) -> typing.Union[collections.abc.Iterator[configuration_pb2.UpdateData], collections.abc.AsyncIterator[configuration_pb2.UpdateData]]:
         """Subscribe to configuration updates."""
 
-def add_ConfigurationServicer_to_server(servicer: ConfigurationServicer, server: typing.Union[grpc.Server, grpc.aio.Server]) -> None: ...
+def add_ConfigurationServicer_to_server(servicer: ConfigurationServicer, server: typing.Union[grpc.Server, grpc.aio.Server]) -> None:
+    ...
```

### Comparing `fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/provisioning_pb2.py` & `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,18 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: fundamentum_edge_proto/provisioning.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-# @@protoc_insertion_point(imports)
-
 _sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)fundamentum_edge_proto/provisioning.proto\x12\x17\x63om.fundamentum.edge.v1\"\xc2\x01\n\x10ProvisionRequest\x12\x14\n\x0c\x61pi_base_url\x18\x01 \x01(\t\x12\x12\n\nproject_id\x18\x02 \x01(\r\x12\x11\n\tregion_id\x18\x03 \x01(\r\x12\x13\n\x0bregistry_id\x18\x04 \x01(\r\x12\x15\n\rserial_number\x18\x05 \x01(\t\x12\x15\n\rasset_type_id\x18\x06 \x01(\x05\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x07 \x01(\t\x12\x18\n\x10replace_existing\x18\x08 \x01(\x08\"\x13\n\x11ProvisionResponse2r\n\x0cProvisioning\x12\x62\n\tProvision\x12).com.fundamentum.edge.v1.ProvisionRequest\x1a*.com.fundamentum.edge.v1.ProvisionResponseb\x06proto3')
-
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12provisioning.proto\x12\x17com.fundamentum.edge.v1"\xc2\x01\n\x10ProvisionRequest\x12\x14\n\x0capi_base_url\x18\x01 \x01(\t\x12\x12\n\nproject_id\x18\x02 \x01(\r\x12\x11\n\tregion_id\x18\x03 \x01(\r\x12\x13\n\x0bregistry_id\x18\x04 \x01(\r\x12\x15\n\rserial_number\x18\x05 \x01(\t\x12\x15\n\rasset_type_id\x18\x06 \x01(\x05\x12\x14\n\x0caccess_token\x18\x07 \x01(\t\x12\x18\n\x10replace_existing\x18\x08 \x01(\x08"\x13\n\x11ProvisionResponse2r\n\x0cProvisioning\x12b\n\tProvision\x12).com.fundamentum.edge.v1.ProvisionRequest\x1a*.com.fundamentum.edge.v1.ProvisionResponseb\x06proto3')
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fundamentum_edge_proto.provisioning_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'provisioning_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  _globals['_PROVISIONREQUEST']._serialized_start=71
-  _globals['_PROVISIONREQUEST']._serialized_end=265
-  _globals['_PROVISIONRESPONSE']._serialized_start=267
-  _globals['_PROVISIONRESPONSE']._serialized_end=286
-  _globals['_PROVISIONING']._serialized_start=288
-  _globals['_PROVISIONING']._serialized_end=402
-# @@protoc_insertion_point(module_scope)
+    DESCRIPTOR._options = None
+    _globals['_PROVISIONREQUEST']._serialized_start = 48
+    _globals['_PROVISIONREQUEST']._serialized_end = 242
+    _globals['_PROVISIONRESPONSE']._serialized_start = 244
+    _globals['_PROVISIONRESPONSE']._serialized_end = 263
+    _globals['_PROVISIONING']._serialized_start = 265
+    _globals['_PROVISIONING']._serialized_end = 379
```

### Comparing `fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/provisioning_pb2.pyi` & `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
-
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ProvisionRequest(_message.Message):
-    __slots__ = ("api_base_url", "project_id", "region_id", "registry_id", "serial_number", "asset_type_id", "access_token", "replace_existing")
+    __slots__ = ('api_base_url', 'project_id', 'region_id', 'registry_id', 'serial_number', 'asset_type_id', 'access_token', 'replace_existing')
     API_BASE_URL_FIELD_NUMBER: _ClassVar[int]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     REGION_ID_FIELD_NUMBER: _ClassVar[int]
     REGISTRY_ID_FIELD_NUMBER: _ClassVar[int]
     SERIAL_NUMBER_FIELD_NUMBER: _ClassVar[int]
     ASSET_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
     ACCESS_TOKEN_FIELD_NUMBER: _ClassVar[int]
@@ -18,12 +17,16 @@
     project_id: int
     region_id: int
     registry_id: int
     serial_number: str
     asset_type_id: int
     access_token: str
     replace_existing: bool
-    def __init__(self, api_base_url: _Optional[str] = ..., project_id: _Optional[int] = ..., region_id: _Optional[int] = ..., registry_id: _Optional[int] = ..., serial_number: _Optional[str] = ..., asset_type_id: _Optional[int] = ..., access_token: _Optional[str] = ..., replace_existing: bool = ...) -> None: ...
+
+    def __init__(self, api_base_url: _Optional[str]=..., project_id: _Optional[int]=..., region_id: _Optional[int]=..., registry_id: _Optional[int]=..., serial_number: _Optional[str]=..., asset_type_id: _Optional[int]=..., access_token: _Optional[str]=..., replace_existing: bool=...) -> None:
+        ...
 
 class ProvisionResponse(_message.Message):
     __slots__ = ()
-    def __init__(self) -> None: ...
+
+    def __init__(self) -> None:
+        ...
```

### Comparing `fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/provisioning_pb2_grpc.py` & `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2_grpc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,22 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-
-from fundamentum_edge_proto import provisioning_pb2 as fundamentum__edge__proto_dot_provisioning__pb2
-
+from . import provisioning_pb2 as provisioning__pb2
 
 class ProvisioningStub(object):
     """Fundamentum Edge's provisioning service.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.Provision = channel.unary_unary(
-                '/com.fundamentum.edge.v1.Provisioning/Provision',
-                request_serializer=fundamentum__edge__proto_dot_provisioning__pb2.ProvisionRequest.SerializeToString,
-                response_deserializer=fundamentum__edge__proto_dot_provisioning__pb2.ProvisionResponse.FromString,
-                )
-
+        self.Provision = channel.unary_unary('/com.fundamentum.edge.v1.Provisioning/Provision', request_serializer=provisioning__pb2.ProvisionRequest.SerializeToString, response_deserializer=provisioning__pb2.ProvisionResponse.FromString)
 
 class ProvisioningServicer(object):
     """Fundamentum Edge's provisioning service.
     """
 
     def Provision(self, request, context):
         """Provision this device against cloud-side.
@@ -33,42 +25,19 @@
         granted MQTT connectivity to the cloud-side broker thus enabling more
         features.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-
 def add_ProvisioningServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'Provision': grpc.unary_unary_rpc_method_handler(
-                    servicer.Provision,
-                    request_deserializer=fundamentum__edge__proto_dot_provisioning__pb2.ProvisionRequest.FromString,
-                    response_serializer=fundamentum__edge__proto_dot_provisioning__pb2.ProvisionResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'com.fundamentum.edge.v1.Provisioning', rpc_method_handlers)
+    rpc_method_handlers = {'Provision': grpc.unary_unary_rpc_method_handler(servicer.Provision, request_deserializer=provisioning__pb2.ProvisionRequest.FromString, response_serializer=provisioning__pb2.ProvisionResponse.SerializeToString)}
+    generic_handler = grpc.method_handlers_generic_handler('com.fundamentum.edge.v1.Provisioning', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
-
- # This class is part of an EXPERIMENTAL API.
 class Provisioning(object):
     """Fundamentum Edge's provisioning service.
     """
 
     @staticmethod
-    def Provision(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/com.fundamentum.edge.v1.Provisioning/Provision',
-            fundamentum__edge__proto_dot_provisioning__pb2.ProvisionRequest.SerializeToString,
-            fundamentum__edge__proto_dot_provisioning__pb2.ProvisionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+    def Provision(request, target, options=(), channel_credentials=None, call_credentials=None, insecure=False, compression=None, wait_for_ready=None, timeout=None, metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/com.fundamentum.edge.v1.Provisioning/Provision', provisioning__pb2.ProvisionRequest.SerializeToString, provisioning__pb2.ProvisionResponse.FromString, options, channel_credentials, insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/provisioning_pb2_grpc.pyi` & `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/provisioning_pb2_grpc.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,45 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import collections.abc
-import fundamentum_edge_proto.provisioning_pb2
 import grpc
 import grpc.aio
+from . import provisioning_pb2
 import typing
-
 _T = typing.TypeVar('_T')
 
 class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta):
     ...
 
-class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore
+class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):
     ...
 
 class ProvisioningStub:
     """Fundamentum Edge's provisioning service."""
 
-    def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None: ...
-    Provision: grpc.UnaryUnaryMultiCallable[
-        fundamentum_edge_proto.provisioning_pb2.ProvisionRequest,
-        fundamentum_edge_proto.provisioning_pb2.ProvisionResponse,
-    ]
-    """Provision this device against cloud-side.
-
-    On successful provisioning, amongst other things, the edge daemon will be
-    granted MQTT connectivity to the cloud-side broker thus enabling more
-    features.
-    """
+    def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None:
+        ...
+    Provision: grpc.UnaryUnaryMultiCallable[provisioning_pb2.ProvisionRequest, provisioning_pb2.ProvisionResponse]
+    'Provision this device against cloud-side.\n\n    On successful provisioning, amongst other things, the edge daemon will be\n    granted MQTT connectivity to the cloud-side broker thus enabling more\n    features.\n    '
 
 class ProvisioningAsyncStub:
     """Fundamentum Edge's provisioning service."""
-
-    Provision: grpc.aio.UnaryUnaryMultiCallable[
-        fundamentum_edge_proto.provisioning_pb2.ProvisionRequest,
-        fundamentum_edge_proto.provisioning_pb2.ProvisionResponse,
-    ]
-    """Provision this device against cloud-side.
-
-    On successful provisioning, amongst other things, the edge daemon will be
-    granted MQTT connectivity to the cloud-side broker thus enabling more
-    features.
-    """
+    Provision: grpc.aio.UnaryUnaryMultiCallable[provisioning_pb2.ProvisionRequest, provisioning_pb2.ProvisionResponse]
+    'Provision this device against cloud-side.\n\n    On successful provisioning, amongst other things, the edge daemon will be\n    granted MQTT connectivity to the cloud-side broker thus enabling more\n    features.\n    '
 
 class ProvisioningServicer(metaclass=abc.ABCMeta):
     """Fundamentum Edge's provisioning service."""
 
     @abc.abstractmethod
-    def Provision(
-        self,
-        request: fundamentum_edge_proto.provisioning_pb2.ProvisionRequest,
-        context: _ServicerContext,
-    ) -> typing.Union[fundamentum_edge_proto.provisioning_pb2.ProvisionResponse, collections.abc.Awaitable[fundamentum_edge_proto.provisioning_pb2.ProvisionResponse]]:
+    def Provision(self, request: provisioning_pb2.ProvisionRequest, context: _ServicerContext) -> typing.Union[provisioning_pb2.ProvisionResponse, collections.abc.Awaitable[provisioning_pb2.ProvisionResponse]]:
         """Provision this device against cloud-side.
 
         On successful provisioning, amongst other things, the edge daemon will be
         granted MQTT connectivity to the cloud-side broker thus enabling more
         features.
         """
 
-def add_ProvisioningServicer_to_server(servicer: ProvisioningServicer, server: typing.Union[grpc.Server, grpc.aio.Server]) -> None: ...
+def add_ProvisioningServicer_to_server(servicer: ProvisioningServicer, server: typing.Union[grpc.Server, grpc.aio.Server]) -> None:
+    ...
```

### Comparing `fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/telemetry_pb2.py` & `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,18 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: fundamentum_edge_proto/telemetry.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-# @@protoc_insertion_point(imports)
-
 _sym_db = _symbol_database.Default()
-
-
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&fundamentum_edge_proto/telemetry.proto\x12\x17\x63om.fundamentum.edge.v1\x1a\x1bgoogle/protobuf/empty.proto\"n\n\x10TelemetryRequest\x12\x0f\n\x07payload\x18\x01 \x01(\x0c\x12\x11\n\tsub_topic\x18\x02 \x01(\t\x12.\n\x03qos\x18\x03 \x01(\x0e\x32\x1c.com.fundamentum.edge.v1.QosH\x00\x88\x01\x01\x42\x06\n\x04_qos*H\n\x03Qos\x12\x14\n\x10QOS_AT_MOST_ONCE\x10\x00\x12\x15\n\x11QOS_AT_LEAST_ONCE\x10\x01\x12\x14\n\x10QOS_EXACTLY_ONCE\x10\x02\x32[\n\tTelemetry\x12N\n\x07Publish\x12).com.fundamentum.edge.v1.TelemetryRequest\x1a\x16.google.protobuf.Empty(\x01\x62\x06proto3')
-
+from . import qos_pb2 as qos__pb2
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0ftelemetry.proto\x12\x17com.fundamentum.edge.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\tqos.proto"n\n\x10TelemetryRequest\x12\x0f\n\x07payload\x18\x01 \x01(\x0c\x12\x11\n\tsub_topic\x18\x02 \x01(\t\x12.\n\x03qos\x18\x03 \x01(\x0e2\x1c.com.fundamentum.edge.v1.QosH\x00\x88\x01\x01B\x06\n\x04_qos2[\n\tTelemetry\x12N\n\x07Publish\x12).com.fundamentum.edge.v1.TelemetryRequest\x1a\x16.google.protobuf.Empty(\x01b\x06proto3')
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fundamentum_edge_proto.telemetry_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'telemetry_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  _globals['_QOS']._serialized_start=208
-  _globals['_QOS']._serialized_end=280
-  _globals['_TELEMETRYREQUEST']._serialized_start=96
-  _globals['_TELEMETRYREQUEST']._serialized_end=206
-  _globals['_TELEMETRY']._serialized_start=282
-  _globals['_TELEMETRY']._serialized_end=373
-# @@protoc_insertion_point(module_scope)
+    DESCRIPTOR._options = None
+    _globals['_TELEMETRYREQUEST']._serialized_start = 84
+    _globals['_TELEMETRYREQUEST']._serialized_end = 194
+    _globals['_TELEMETRY']._serialized_start = 196
+    _globals['_TELEMETRY']._serialized_end = 287
```

### Comparing `fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/telemetry_pb2.pyi` & `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 from google.protobuf import empty_pb2 as _empty_pb2
-from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
+import qos_pb2 as _qos_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional, Union as _Union
-
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Qos(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = ()
-    QOS_AT_MOST_ONCE: _ClassVar[Qos]
-    QOS_AT_LEAST_ONCE: _ClassVar[Qos]
-    QOS_EXACTLY_ONCE: _ClassVar[Qos]
-QOS_AT_MOST_ONCE: Qos
-QOS_AT_LEAST_ONCE: Qos
-QOS_EXACTLY_ONCE: Qos
-
 class TelemetryRequest(_message.Message):
-    __slots__ = ("payload", "sub_topic", "qos")
+    __slots__ = ('payload', 'sub_topic', 'qos')
     PAYLOAD_FIELD_NUMBER: _ClassVar[int]
     SUB_TOPIC_FIELD_NUMBER: _ClassVar[int]
     QOS_FIELD_NUMBER: _ClassVar[int]
     payload: bytes
     sub_topic: str
-    qos: Qos
-    def __init__(self, payload: _Optional[bytes] = ..., sub_topic: _Optional[str] = ..., qos: _Optional[_Union[Qos, str]] = ...) -> None: ...
+    qos: _qos_pb2.Qos
+
+    def __init__(self, payload: _Optional[bytes]=..., sub_topic: _Optional[str]=..., qos: _Optional[_Union[_qos_pb2.Qos, str]]=...) -> None:
+        ...
```

### Comparing `fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/telemetry_pb2_grpc.py` & `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2_grpc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,40 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-
-from fundamentum_edge_proto import telemetry_pb2 as fundamentum__edge__proto_dot_telemetry__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
+from . import telemetry_pb2 as telemetry__pb2
 
 class TelemetryStub(object):
     """Fundamentum Edge's telemetry service.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.Publish = channel.stream_unary(
-                '/com.fundamentum.edge.v1.Telemetry/Publish',
-                request_serializer=fundamentum__edge__proto_dot_telemetry__pb2.TelemetryRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
+        self.Publish = channel.stream_unary('/com.fundamentum.edge.v1.Telemetry/Publish', request_serializer=telemetry__pb2.TelemetryRequest.SerializeToString, response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString)
 
 class TelemetryServicer(object):
     """Fundamentum Edge's telemetry service.
     """
 
     def Publish(self, request_iterator, context):
         """Publishes device-specific data to the `event` topic or to one of its sub-topics if specified.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-
 def add_TelemetryServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'Publish': grpc.stream_unary_rpc_method_handler(
-                    servicer.Publish,
-                    request_deserializer=fundamentum__edge__proto_dot_telemetry__pb2.TelemetryRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'com.fundamentum.edge.v1.Telemetry', rpc_method_handlers)
+    rpc_method_handlers = {'Publish': grpc.stream_unary_rpc_method_handler(servicer.Publish, request_deserializer=telemetry__pb2.TelemetryRequest.FromString, response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString)}
+    generic_handler = grpc.method_handlers_generic_handler('com.fundamentum.edge.v1.Telemetry', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
-
- # This class is part of an EXPERIMENTAL API.
 class Telemetry(object):
     """Fundamentum Edge's telemetry service.
     """
 
     @staticmethod
-    def Publish(request_iterator,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.stream_unary(request_iterator, target, '/com.fundamentum.edge.v1.Telemetry/Publish',
-            fundamentum__edge__proto_dot_telemetry__pb2.TelemetryRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+    def Publish(request_iterator, target, options=(), channel_credentials=None, call_credentials=None, insecure=False, compression=None, wait_for_ready=None, timeout=None, metadata=None):
+        return grpc.experimental.stream_unary(request_iterator, target, '/com.fundamentum.edge.v1.Telemetry/Publish', telemetry__pb2.TelemetryRequest.SerializeToString, google_dot_protobuf_dot_empty__pb2.Empty.FromString, options, channel_credentials, insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/telemetry_pb2_grpc.pyi` & `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/telemetry_pb2_grpc.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,41 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import collections.abc
-import fundamentum_edge_proto.telemetry_pb2
 import google.protobuf.empty_pb2
 import grpc
 import grpc.aio
+from . import telemetry_pb2
 import typing
-
 _T = typing.TypeVar('_T')
 
 class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta):
     ...
 
-class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore
+class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):
     ...
 
 class TelemetryStub:
     """Fundamentum Edge's telemetry service."""
 
-    def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None: ...
-    Publish: grpc.StreamUnaryMultiCallable[
-        fundamentum_edge_proto.telemetry_pb2.TelemetryRequest,
-        google.protobuf.empty_pb2.Empty,
-    ]
-    """Publishes device-specific data to the `event` topic or to one of its sub-topics if specified."""
+    def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None:
+        ...
+    Publish: grpc.StreamUnaryMultiCallable[telemetry_pb2.TelemetryRequest, google.protobuf.empty_pb2.Empty]
+    'Publishes device-specific data to the `event` topic or to one of its sub-topics if specified.'
 
 class TelemetryAsyncStub:
     """Fundamentum Edge's telemetry service."""
-
-    Publish: grpc.aio.StreamUnaryMultiCallable[
-        fundamentum_edge_proto.telemetry_pb2.TelemetryRequest,
-        google.protobuf.empty_pb2.Empty,
-    ]
-    """Publishes device-specific data to the `event` topic or to one of its sub-topics if specified."""
+    Publish: grpc.aio.StreamUnaryMultiCallable[telemetry_pb2.TelemetryRequest, google.protobuf.empty_pb2.Empty]
+    'Publishes device-specific data to the `event` topic or to one of its sub-topics if specified.'
 
 class TelemetryServicer(metaclass=abc.ABCMeta):
     """Fundamentum Edge's telemetry service."""
 
     @abc.abstractmethod
-    def Publish(
-        self,
-        request_iterator: _MaybeAsyncIterator[fundamentum_edge_proto.telemetry_pb2.TelemetryRequest],
-        context: _ServicerContext,
-    ) -> typing.Union[google.protobuf.empty_pb2.Empty, collections.abc.Awaitable[google.protobuf.empty_pb2.Empty]]:
+    def Publish(self, request_iterator: _MaybeAsyncIterator[telemetry_pb2.TelemetryRequest], context: _ServicerContext) -> typing.Union[google.protobuf.empty_pb2.Empty, collections.abc.Awaitable[google.protobuf.empty_pb2.Empty]]:
         """Publishes device-specific data to the `event` topic or to one of its sub-topics if specified."""
 
-def add_TelemetryServicer_to_server(servicer: TelemetryServicer, server: typing.Union[grpc.Server, grpc.aio.Server]) -> None: ...
+def add_TelemetryServicer_to_server(servicer: TelemetryServicer, server: typing.Union[grpc.Server, grpc.aio.Server]) -> None:
+    ...
```

### Comparing `fundamentum_edge_proto-1.0.1.1/fundamentum_edge_proto/typed_stubs.py` & `fundamentum_edge_proto-1.1.0/fundamentum_edge_proto/typed_stubs.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 from typing import TYPE_CHECKING, cast, overload
 
 import grpc
 import grpc.aio
 
 from fundamentum_edge_proto.configuration_pb2_grpc import ConfigurationStub
 from fundamentum_edge_proto.provisioning_pb2_grpc import ProvisioningStub
+from fundamentum_edge_proto.states_pb2_grpc import StatesEventStub
 from fundamentum_edge_proto.telemetry_pb2_grpc import TelemetryStub
 
 if TYPE_CHECKING:
     from fundamentum_edge_proto.configuration_pb2_grpc import ConfigurationAsyncStub
     from fundamentum_edge_proto.provisioning_pb2_grpc import ProvisioningAsyncStub
+    from fundamentum_edge_proto.states_pb2_grpc import StatesEventAsyncStub
     from fundamentum_edge_proto.telemetry_pb2_grpc import TelemetryAsyncStub
 
 
 @overload
 def build_configuration_stub(channel: grpc.Channel) -> ConfigurationStub: ...
 @overload
 def build_configuration_stub(channel: grpc.aio.Channel) -> "ConfigurationAsyncStub": ...
@@ -36,14 +38,25 @@
     stub = ProvisioningStub(channel)
     if isinstance(channel, grpc.aio.Channel):
         return cast("ProvisioningAsyncStub", stub)
     return stub
 
 
 @overload
+def build_states_event_stub(channel: grpc.Channel) -> StatesEventStub: ...
+@overload
+def build_states_event_stub(channel: grpc.aio.Channel) -> "StatesEventAsyncStub": ...
+def build_states_event_stub(channel):
+    stub = StatesEventStub(channel)
+    if isinstance(channel, grpc.aio.Channel):
+        return cast("StatesEventAsyncStub", stub)
+    return stub
+
+
+@overload
 def build_telemetry_stub(channel: grpc.Channel) -> TelemetryStub: ...
 @overload
 def build_telemetry_stub(channel: grpc.aio.Channel) -> "TelemetryAsyncStub": ...
 def build_telemetry_stub(channel):
     stub = TelemetryStub(channel)
     if isinstance(channel, grpc.aio.Channel):
         return cast("TelemetryAsyncStub", stub)
```

### Comparing `fundamentum_edge_proto-1.0.1.1/pyproject.toml` & `fundamentum_edge_proto-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -7,42 +7,50 @@
 ]
 dynamic = []
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "protobuf>=3.20.3",
 ]
-version = "1.0.1.1"
+version = "1.1.0"
 
 [project.urls]
 repository = "https://bitbucket.org/amotus/fundamentum-edge-proto-python"
 
 [project.license]
 file = "LICENSE"
 
 [tool.pdm.dev-dependencies]
 build = [
     "grpcio-tools",
     "mypy-protobuf",
+    "protoletariat>=3.2.19",
 ]
 type-check = [
     "mypy>=1.9",
     "types-protobuf>=4.24",
     "grpc-stubs>=1.53",
 ]
 lint = [
     "ruff>=0.3",
 ]
 
 [tool.pdm.scripts]
-build-proto = "python -m grpc_tools.protoc\n  -I fundamentum_edge_proto=./proto\n  --python_out=.\n  --pyi_out=.\n  --grpc_python_out=.\n  --mypy_grpc_out=.\n  proto/configuration.proto\n  proto/provisioning.proto\n  proto/telemetry.proto\n"
+compile-proto = "python -m grpc_tools.protoc\n  --proto_path ./proto\n  --python_out ./fundamentum_edge_proto\n  --pyi_out ./fundamentum_edge_proto\n  --grpc_python_out ./fundamentum_edge_proto\n  --mypy_grpc_out ./fundamentum_edge_proto\n  configuration.proto\n  provisioning.proto\n  qos.proto\n  states.proto\n  telemetry.proto\n"
+patch-proto = "protol \n  --in-place \n  --python-out ./fundamentum_edge_proto\n  protoc \n  --proto-path ./proto \n  configuration.proto\n  provisioning.proto\n  qos.proto\n  states.proto\n  telemetry.proto\n"
 test-import = "python -c 'import fundamentum_edge_proto'"
 lint = "ruff check fundamentum_edge_proto"
 type-check = "mypy fundamentum_edge_proto/__init__.py fundamentum_edge_proto/typed_stubs.py"
 
+[tool.pdm.scripts.build-proto]
+composite = [
+    "compile-proto",
+    "patch-proto",
+]
+
 [tool.pdm.scripts.validate]
 composite = [
     "lint",
     "type-check",
     "test-import",
 ]
```

### Comparing `fundamentum_edge_proto-1.0.1.1/PKG-INFO` & `fundamentum_edge_proto-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundamentum-edge-proto
-Version: 1.0.1.1
+Version: 1.1.0
 Summary: fundamentum-edge protobufs
 Author-Email: Alex Sirois <asirois@dimonoff.com>, Jonathan Chouinard <jchouinard@dimonoff.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,15 +205,29 @@
            See the License for the specific language governing permissions and
            limitations under the License.
 Project-URL: Repository, https://bitbucket.org/amotus/fundamentum-edge-proto-python
 Requires-Python: >=3.10
 Requires-Dist: protobuf>=3.20.3
 Description-Content-Type: text/markdown
 
-# fundamentum-edge-proto-python
+# Fundamentum Edge Proto Python
+
+[![Crates.io][crate-badge]][crate-url]
+[![License][licence-badge]][licence-url]
+[![Build Status][build-badge]][build-url]
+
+[Website][website-url]
+
+[crate-badge]: https://img.shields.io/pypi/v/fundamentum-edge-proto.svg
+[crate-url]: https://pypi.org/project/fundamentum-edge-proto
+[licence-badge]: https://img.shields.io/badge/license-apache_2.0-blue.svg
+[licence-url]: https://bitbucket.org/amotus/fundamentum-edge-proto-python/src/master/LICENSE
+[build-badge]: https://img.shields.io/bitbucket/pipelines/amotus/fundamentum-edge-proto-python/master
+[build-url]: https://bitbucket.org/amotus/fundamentum-edge-proto-python/pipelines
+[website-url]: https://www.dimonoff.com/services/fundamentum-iot-platform-paas
 
 Python bindings to Fundamentum edge daemon's *gRPC* IDL files. A library that
 provides a Python representation of the basic types, interfaces and other
 components required to define and interact with the *gRPC* interface defined
 by [`fundamentum-edge-proto`][repo-proto].
 
 [repo-proto]: https://bitbucket.org/amotus/fundamentum-edge-proto
```


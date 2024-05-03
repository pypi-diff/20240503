# Comparing `tmp/openobd_protocol-0.0.40.tar.gz` & `tmp/openobd_protocol-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd_protocol-0.0.40.tar", last modified: Wed Apr 24 13:12:16 2024, max compression
+gzip compressed data, was "openobd_protocol-0.0.43.tar", last modified: Fri May  3 13:43:35 2024, max compression
```

## Comparing `openobd_protocol-0.0.40.tar` & `openobd_protocol-0.0.43.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.930296 openobd_protocol-0.0.40/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-24 13:12:16.929296 openobd_protocol-0.0.40/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/README.md
--rw-r--r--   0 root         (0) root         (0)     1895 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 13:12:16.930296 openobd_protocol-0.0.40/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.905295 openobd_protocol-0.0.40/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.916295 openobd_protocol-0.0.40/src/openobd_protocol/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/Authentication_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/Authentication_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1359 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/BasicResponse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/BasicResponse_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5065 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/BusConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/BusConfiguration_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.921296 openobd_protocol-0.0.40/src/openobd_protocol/CAN/
--rw-r--r--   0 root         (0) root         (0)     1978 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/CAN/CanServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      462 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/CAN/CanServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2751 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2565 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/CAN/Isotp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2400 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/CAN/Isotp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2349 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8395 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.924296 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/
--rw-r--r--   0 root         (0) root         (0)     2460 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/SessionServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    10370 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2492 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/Session_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2430 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/Session_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1712 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/Status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/Status_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.928296 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/
--rw-r--r--   0 root         (0) root         (0)     1748 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2973 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterface_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4208 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.929296 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-24 13:12:16.000000 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1610 2024-04-24 13:12:16.000000 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:12:16.000000 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-24 13:12:16.000000 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-24 13:12:16.000000 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 13:43:35.008488 openobd_protocol-0.0.43/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-03 13:43:35.008488 openobd_protocol-0.0.43/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/README.md
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 13:43:35.008488 openobd_protocol-0.0.43/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 13:43:34.975487 openobd_protocol-0.0.43/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 13:43:34.992488 openobd_protocol-0.0.43/src/openobd_protocol/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/Authentication_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/Authentication_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/BasicResponse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/BasicResponse_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/BusConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/BusConfiguration_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 13:43:34.998488 openobd_protocol-0.0.43/src/openobd_protocol/CAN/
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/CAN/CanServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      462 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/CAN/CanServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/CAN/Isotp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/CAN/Isotp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8395 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 13:43:35.004488 openobd_protocol-0.0.43/src/openobd_protocol/SessionController/
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/SessionController/SessionServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    10384 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/SessionController/Session_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/SessionController/Session_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/Status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/Status_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 13:43:35.007488 openobd_protocol-0.0.43/src/openobd_protocol/UserInterface/
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/UserInterface/UserInterface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-03 13:43:28.000000 openobd_protocol-0.0.43/src/openobd_protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 13:43:35.007488 openobd_protocol-0.0.43/src/openobd_protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-03 13:43:34.000000 openobd_protocol-0.0.43/src/openobd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-05-03 13:43:34.000000 openobd_protocol-0.0.43/src/openobd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 13:43:34.000000 openobd_protocol-0.0.43/src/openobd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-05-03 13:43:34.000000 openobd_protocol-0.0.43/src/openobd_protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-03 13:43:34.000000 openobd_protocol-0.0.43/src/openobd_protocol.egg-info/top_level.txt
```

### Comparing `openobd_protocol-0.0.40/LICENSE` & `openobd_protocol-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/PKG-INFO` & `openobd_protocol-0.0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.40
+Version: 0.0.43
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.0.40/pyproject.toml` & `openobd_protocol-0.0.43/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/Authentication_pb2.py` & `openobd_protocol-0.0.43/src/openobd_protocol/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/Authentication_pb2.pyi` & `openobd_protocol-0.0.43/src/openobd_protocol/Authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/BasicResponse_pb2.py` & `openobd_protocol-0.0.43/src/openobd_protocol/BasicResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/BasicResponse_pb2.pyi` & `openobd_protocol-0.0.43/src/openobd_protocol/BasicResponse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/BusConfiguration_pb2.py` & `openobd_protocol-0.0.43/src/openobd_protocol/BusConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/BusConfiguration_pb2.pyi` & `openobd_protocol-0.0.43/src/openobd_protocol/BusConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/CAN/CanServices_pb2.py` & `openobd_protocol-0.0.43/src/openobd_protocol/CAN/CanServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/CAN/CanServices_pb2_grpc.py` & `openobd_protocol-0.0.43/src/openobd_protocol/CAN/CanServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/CAN/Isotp_pb2.py` & `openobd_protocol-0.0.43/src/openobd_protocol/CAN/Isotp_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/CAN/Isotp_pb2.pyi` & `openobd_protocol-0.0.43/src/openobd_protocol/CAN/Isotp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/RemoteDiagnosticServices_pb2.py` & `openobd_protocol-0.0.43/src/openobd_protocol/RemoteDiagnosticServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py` & `openobd_protocol-0.0.43/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/SessionController/SessionServices_pb2.py` & `openobd_protocol-0.0.43/src/openobd_protocol/SessionController/SessionServices_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 from openobd_protocol.SessionController import Session_pb2 as openobd__protocol_dot_SessionController_dot_Session__pb2
 from openobd_protocol import BasicResponse_pb2 as openobd__protocol_dot_BasicResponse__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8openobd_protocol/SessionController/SessionServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\x1a\x30openobd_protocol/SessionController/Session.proto\x1a$openobd_protocol/BasicResponse.proto2\xb8\x05\n\x0fSessionServices\x12\x91\x01\n\x0fgetSessionToken\x12=.com.jifeline.OpenOBD.Protocol.SessionController.Authenticate\x1a=.com.jifeline.OpenOBD.Protocol.SessionController.SessionToken\"\x00\x12\x8e\x01\n\rcreateSession\x12=.com.jifeline.OpenOBD.Protocol.SessionController.StartSession\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x88\x01\n\ngetSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12t\n\rdeleteSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12\x7f\n\x0clistSessions\x12+.com.jifeline.OpenOBD.Protocol.EmptyRequest\x1a@.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfoList\"\x00\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8openobd_protocol/SessionController/SessionServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\x1a\x30openobd_protocol/SessionController/Session.proto\x1a$openobd_protocol/BasicResponse.proto2\xbb\x05\n\x0fSessionServices\x12\x91\x01\n\x0fgetSessionToken\x12=.com.jifeline.OpenOBD.Protocol.SessionController.Authenticate\x1a=.com.jifeline.OpenOBD.Protocol.SessionController.SessionToken\"\x00\x12\x8e\x01\n\rcreateSession\x12=.com.jifeline.OpenOBD.Protocol.SessionController.StartSession\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x88\x01\n\ngetSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12t\n\rdeleteSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12\x81\x01\n\x0egetSessionList\x12+.com.jifeline.OpenOBD.Protocol.EmptyRequest\x1a@.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfoList\"\x00\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.SessionController.SessionServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
   _globals['_SESSIONSERVICES']._serialized_start=229
-  _globals['_SESSIONSERVICES']._serialized_end=925
+  _globals['_SESSIONSERVICES']._serialized_end=928
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py` & `openobd_protocol-0.0.43/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
                 response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
                 )
         self.deleteSession = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/deleteSession',
                 request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.SerializeToString,
                 response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
                 )
-        self.listSessions = channel.unary_unary(
-                '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/listSessions',
+        self.getSessionList = channel.unary_unary(
+                '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSessionList',
                 request_serializer=openobd__protocol_dot_BasicResponse__pb2.EmptyRequest.SerializeToString,
                 response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfoList.FromString,
                 )
 
 
 class SessionServicesServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -66,15 +66,15 @@
 
     def deleteSession(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def listSessions(self, request, context):
+    def getSessionList(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_SessionServicesServicer_to_server(servicer, server):
@@ -95,16 +95,16 @@
                     response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.SerializeToString,
             ),
             'deleteSession': grpc.unary_unary_rpc_method_handler(
                     servicer.deleteSession,
                     request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.FromString,
                     response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
             ),
-            'listSessions': grpc.unary_unary_rpc_method_handler(
-                    servicer.listSessions,
+            'getSessionList': grpc.unary_unary_rpc_method_handler(
+                    servicer.getSessionList,
                     request_deserializer=openobd__protocol_dot_BasicResponse__pb2.EmptyRequest.FromString,
                     response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfoList.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'com.jifeline.OpenOBD.Protocol.SessionController.SessionServices', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
@@ -179,22 +179,22 @@
         return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/deleteSession',
             openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.SerializeToString,
             openobd__protocol_dot_Status__pb2.Status.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def listSessions(request,
+    def getSessionList(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/listSessions',
+        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSessionList',
             openobd__protocol_dot_BasicResponse__pb2.EmptyRequest.SerializeToString,
             openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfoList.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/SessionController/Session_pb2.py` & `openobd_protocol-0.0.43/src/openobd_protocol/SessionController/Session_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0openobd_protocol/SessionController/Session.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\"\'\n\x0cStartSession\x12\x17\n\x0f\x63onnection_uuid\x18\x01 \x01(\t\"}\n\x0bSessionInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x16\n\x0esession_status\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\t\x12\x18\n\x10session_endpoint\x18\x04 \x01(\t\x12\x1c\n\x14\x61uthentication_token\x18\x05 \x01(\t\"N\n\x0c\x41uthenticate\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x1a\n\x12\x63lient_credentials\x18\x02 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x03 \x01(\t\"\x1d\n\x0cSessionToken\x12\r\n\x05token\x18\x01 \x01(\t\"a\n\x0fSessionInfoList\x12N\n\x08sessions\x18\x01 \x03(\x0b\x32<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x1f\n\tSessionId\x12\x12\n\nsession_id\x18\x01 \x01(\tB\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0openobd_protocol/SessionController/Session.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\"\'\n\x0cStartSession\x12\x17\n\x0f\x63onnection_uuid\x18\x01 \x01(\t\"\x85\x01\n\x0bSessionInfo\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x16\n\x0esession_status\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\t\x12\x18\n\x10session_endpoint\x18\x04 \x01(\t\x12\x1c\n\x14\x61uthentication_token\x18\x05 \x01(\t\"N\n\x0c\x41uthenticate\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x1a\n\x12\x63lient_credentials\x18\x02 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x03 \x01(\t\"%\n\x0cSessionToken\x12\x15\n\rsession_token\x18\x01 \x01(\t\"a\n\x0fSessionInfoList\x12N\n\x08sessions\x18\x01 \x03(\x0b\x32<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x1f\n\tSessionId\x12\x12\n\nsession_id\x18\x01 \x01(\tB\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.SessionController.Session_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
   _globals['_STARTSESSION']._serialized_start=132
   _globals['_STARTSESSION']._serialized_end=171
-  _globals['_SESSIONINFO']._serialized_start=173
-  _globals['_SESSIONINFO']._serialized_end=298
-  _globals['_AUTHENTICATE']._serialized_start=300
-  _globals['_AUTHENTICATE']._serialized_end=378
-  _globals['_SESSIONTOKEN']._serialized_start=380
-  _globals['_SESSIONTOKEN']._serialized_end=409
-  _globals['_SESSIONINFOLIST']._serialized_start=411
-  _globals['_SESSIONINFOLIST']._serialized_end=508
-  _globals['_SESSIONID']._serialized_start=510
-  _globals['_SESSIONID']._serialized_end=541
+  _globals['_SESSIONINFO']._serialized_start=174
+  _globals['_SESSIONINFO']._serialized_end=307
+  _globals['_AUTHENTICATE']._serialized_start=309
+  _globals['_AUTHENTICATE']._serialized_end=387
+  _globals['_SESSIONTOKEN']._serialized_start=389
+  _globals['_SESSIONTOKEN']._serialized_end=426
+  _globals['_SESSIONINFOLIST']._serialized_start=428
+  _globals['_SESSIONINFOLIST']._serialized_end=525
+  _globals['_SESSIONID']._serialized_start=527
+  _globals['_SESSIONID']._serialized_end=558
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/SessionController/Session_pb2.pyi` & `openobd_protocol-0.0.43/src/openobd_protocol/SessionController/Session_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,42 +9,42 @@
 class StartSession(_message.Message):
     __slots__ = ("connection_uuid",)
     CONNECTION_UUID_FIELD_NUMBER: _ClassVar[int]
     connection_uuid: str
     def __init__(self, connection_uuid: _Optional[str] = ...) -> None: ...
 
 class SessionInfo(_message.Message):
-    __slots__ = ("id", "session_status", "created_at", "session_endpoint", "authentication_token")
-    ID_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ("session_id", "session_status", "created_at", "session_endpoint", "authentication_token")
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     SESSION_STATUS_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     SESSION_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
     AUTHENTICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    id: str
+    session_id: str
     session_status: str
     created_at: str
     session_endpoint: str
     authentication_token: str
-    def __init__(self, id: _Optional[str] = ..., session_status: _Optional[str] = ..., created_at: _Optional[str] = ..., session_endpoint: _Optional[str] = ..., authentication_token: _Optional[str] = ...) -> None: ...
+    def __init__(self, session_id: _Optional[str] = ..., session_status: _Optional[str] = ..., created_at: _Optional[str] = ..., session_endpoint: _Optional[str] = ..., authentication_token: _Optional[str] = ...) -> None: ...
 
 class Authenticate(_message.Message):
     __slots__ = ("client_id", "client_credentials", "api_key")
     CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
     CLIENT_CREDENTIALS_FIELD_NUMBER: _ClassVar[int]
     API_KEY_FIELD_NUMBER: _ClassVar[int]
     client_id: str
     client_credentials: str
     api_key: str
     def __init__(self, client_id: _Optional[str] = ..., client_credentials: _Optional[str] = ..., api_key: _Optional[str] = ...) -> None: ...
 
 class SessionToken(_message.Message):
-    __slots__ = ("token",)
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    token: str
-    def __init__(self, token: _Optional[str] = ...) -> None: ...
+    __slots__ = ("session_token",)
+    SESSION_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    session_token: str
+    def __init__(self, session_token: _Optional[str] = ...) -> None: ...
 
 class SessionInfoList(_message.Message):
     __slots__ = ("sessions",)
     SESSIONS_FIELD_NUMBER: _ClassVar[int]
     sessions: _containers.RepeatedCompositeFieldContainer[SessionInfo]
     def __init__(self, sessions: _Optional[_Iterable[_Union[SessionInfo, _Mapping]]] = ...) -> None: ...
```

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/Status_pb2.py` & `openobd_protocol-0.0.43/src/openobd_protocol/Status_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/Status_pb2.pyi` & `openobd_protocol-0.0.43/src/openobd_protocol/Status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py` & `openobd_protocol-0.0.43/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py` & `openobd_protocol-0.0.43/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterface_pb2.py` & `openobd_protocol-0.0.43/src/openobd_protocol/UserInterface/UserInterface_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi` & `openobd_protocol-0.0.43/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol.egg-info/PKG-INFO` & `openobd_protocol-0.0.43/src/openobd_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.40
+Version: 0.0.43
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.0.40/src/openobd_protocol.egg-info/SOURCES.txt` & `openobd_protocol-0.0.43/src/openobd_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/wirepas_networktool_messaging-4.4.0.tar.gz` & `tmp/wirepas_networktool_messaging-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wirepas_networktool_messaging-4.4.0.tar", last modified: Thu Dec 21 14:52:22 2023, max compression
+gzip compressed data, was "wirepas_networktool_messaging-4.4.1.tar", last modified: Fri May  3 09:06:45 2024, max compression
```

## Comparing `wirepas_networktool_messaging-4.4.0.tar` & `wirepas_networktool_messaging-4.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 14:52:22.968327 wirepas_networktool_messaging-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2023-12-21 14:51:58.000000 wirepas_networktool_messaging-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-21 14:52:22.968327 wirepas_networktool_messaging-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-12-21 14:51:58.000000 wirepas_networktool_messaging-4.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 14:52:22.968327 wirepas_networktool_messaging-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-12-21 14:51:58.000000 wirepas_networktool_messaging-4.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 14:52:22.964327 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-12-21 14:52:22.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-21 14:51:58.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-12-21 14:51:58.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 14:52:22.968327 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-21 14:51:58.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2023-12-21 14:52:07.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/commons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    94069 2023-12-21 14:52:07.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/internal_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)   180893 2023-12-21 14:52:07.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15037 2023-12-21 14:52:07.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/nanopb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26768 2023-12-21 14:52:07.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/otap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    42336 2023-12-21 14:52:07.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/positioning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    22618 2023-12-21 14:52:07.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/remote_api_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 14:52:22.968327 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-21 14:52:22.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-12-21 14:52:22.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 14:52:22.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-21 14:52:22.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-21 14:52:22.000000 wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:06:45.528368 wirepas_networktool_messaging-4.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-03 09:06:27.000000 wirepas_networktool_messaging-4.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-03 09:06:45.528368 wirepas_networktool_messaging-4.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-03 09:06:27.000000 wirepas_networktool_messaging-4.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:06:45.528368 wirepas_networktool_messaging-4.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-03 09:06:27.000000 wirepas_networktool_messaging-4.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:06:45.524368 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-03 09:06:45.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-03 09:06:27.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 09:06:27.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:06:45.528368 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 09:06:27.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16406 2024-05-03 09:06:31.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/commons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94674 2024-05-03 09:06:31.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/internal_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   177370 2024-05-03 09:06:31.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15037 2024-05-03 09:06:31.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/nanopb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26768 2024-05-03 09:06:31.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/otap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42336 2024-05-03 09:06:31.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/positioning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22618 2024-05-03 09:06:31.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/remote_api_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:06:45.524368 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-03 09:06:45.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-03 09:06:45.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:06:45.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 09:06:45.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 09:06:45.000000 wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging.egg-info/top_level.txt
```

### Comparing `wirepas_networktool_messaging-4.4.0/LICENSE` & `wirepas_networktool_messaging-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wirepas_networktool_messaging-4.4.0/PKG-INFO` & `wirepas_networktool_messaging-4.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wirepas_networktool_messaging
-Version: 4.4.0
+Version: 4.4.1
 Summary: WNT protocol buffers bindings.
 Home-page: https://github.com/wirepas/wirepas-networktool-messaging-python
 Author: Wirepas Ltd
 Author-email: opensource@wirepas.com
 License: Apache-2
 Keywords: wirepas WNT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wirepas_networktool_messaging-4.4.0/README.md` & `wirepas_networktool_messaging-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `wirepas_networktool_messaging-4.4.0/setup.py` & `wirepas_networktool_messaging-4.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/__about__.py` & `wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 __copyright__ = "2021 Wirepas Ltd"
 __description__ = "WNT protocol buffers bindings."
 __keywords__ = "wirepas WNT"
 __license__ = "Apache-2"
 __pkg_name__ = "wirepas_networktool_messaging"
 __title__ = "Wirepas Messaging For WNT"
 __url__ = "https://github.com/wirepas/wirepas-networktool-messaging-python"
-__version__ = "v4.4.0"
+__version__ = "v4.4.1"
```

### Comparing `wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/__init__.py` & `wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/commons_pb2.py` & `wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/nanopb_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,276 +1,277 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: commons.proto
+# source: nanopb.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='commons.proto',
-  package='com.wirepas.proto.wnt',
+  name='nanopb.proto',
+  package='',
   syntax='proto2',
-  serialized_options=None,
+  serialized_options=b'\n\030fi.kapsi.koti.jpa.nanopb',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\rcommons.proto\x12\x15\x63om.wirepas.proto.wnt\"c\n\x08\x46ullRole\x12\x32\n\tbase_role\x18\x01 \x01(\x0e\x32\x1f.com.wirepas.proto.wnt.BaseRole\x12\x0e\n\x06\x63\x62_mac\x18\x02 \x01(\x08\x12\x13\n\x0bis_autorole\x18\x04 \x01(\x08\"\xb1\x01\n\rAppConfigData\x12\x10\n\x08interval\x18\x01 \x01(\r\x12\x10\n\x08sequence\x18\x02 \x01(\r\x12\x12\n\napp_config\x18\x03 \x01(\x0c\x12\x12\n\nmax_length\x18\x04 \x01(\r\x12\x16\n\x0eis_override_on\x18\x05 \x01(\x08\x12<\n\x0eselection_type\x18\x06 \x01(\x0e\x32$.com.wirepas.proto.wnt.SelectionType*B\n\x08\x42\x61seRole\x12\x0b\n\x07SUBNODE\x10\x01\x12\x0c\n\x08HEADNODE\x10\x02\x12\x08\n\x04SINK\x10\x04\x12\x11\n\x0cROLE_UNKNOWN\x10\xff\x01*\\\n\x12MessageSendingType\x12 \n\x1cMESSAGE_SENDING_TYPE_INSTANT\x10\x01\x12$\n MESSAGE_SENDING_TYPE_DISTRIBUTED\x10\x02*D\n\rSelectionType\x12\x1a\n\x16SELECTION_TYPE_NETWORK\x10\x01\x12\x17\n\x13SELECTION_TYPE_SINK\x10\x02*\xf9\x01\n\x10ScratchpadAction\x12\x1d\n\x19SCRATCHPAD_ACTION_UNKNOWN\x10\x00\x12\x1d\n\x19SCRATCHPAD_ACTION_NO_OTAP\x10\x01\x12$\n SCRATCHPAD_ACTION_PROPAGATE_ONLY\x10\x02\x12+\n\'SCRATCHPAD_ACTION_PROPAGATE_AND_PROCESS\x10\x03\x12\x36\n2SCRATCHPAD_ACTION_PROPAGATE_AND_PROCESS_WITH_DELAY\x10\x04\x12\x1c\n\x18SCRATCHPAD_ACTION_LEGACY\x10\x05'
-)
-
-_BASEROLE = _descriptor.EnumDescriptor(
-  name='BaseRole',
-  full_name='com.wirepas.proto.wnt.BaseRole',
+  serialized_pb=b'\n\x0cnanopb.proto\x1a google/protobuf/descriptor.proto\"\xa3\x03\n\rNanoPBOptions\x12\x10\n\x08max_size\x18\x01 \x01(\x05\x12\x12\n\nmax_length\x18\x0e \x01(\x05\x12\x11\n\tmax_count\x18\x02 \x01(\x05\x12&\n\x08int_size\x18\x07 \x01(\x0e\x32\x08.IntSize:\nIS_DEFAULT\x12$\n\x04type\x18\x03 \x01(\x0e\x32\n.FieldType:\nFT_DEFAULT\x12\x18\n\nlong_names\x18\x04 \x01(\x08:\x04true\x12\x1c\n\rpacked_struct\x18\x05 \x01(\x08:\x05\x66\x61lse\x12\x1a\n\x0bpacked_enum\x18\n \x01(\x08:\x05\x66\x61lse\x12\x1b\n\x0cskip_message\x18\x06 \x01(\x08:\x05\x66\x61lse\x12\x18\n\tno_unions\x18\x08 \x01(\x08:\x05\x66\x61lse\x12\r\n\x05msgid\x18\t \x01(\r\x12\x1e\n\x0f\x61nonymous_oneof\x18\x0b \x01(\x08:\x05\x66\x61lse\x12\x15\n\x06proto3\x18\x0c \x01(\x08:\x05\x66\x61lse\x12\x1d\n\x0e\x65num_to_string\x18\r \x01(\x08:\x05\x66\x61lse\x12\x1b\n\x0c\x66ixed_length\x18\x0f \x01(\x08:\x05\x66\x61lse*i\n\tFieldType\x12\x0e\n\nFT_DEFAULT\x10\x00\x12\x0f\n\x0b\x46T_CALLBACK\x10\x01\x12\x0e\n\nFT_POINTER\x10\x04\x12\r\n\tFT_STATIC\x10\x02\x12\r\n\tFT_IGNORE\x10\x03\x12\r\n\tFT_INLINE\x10\x05*D\n\x07IntSize\x12\x0e\n\nIS_DEFAULT\x10\x00\x12\x08\n\x04IS_8\x10\x08\x12\t\n\x05IS_16\x10\x10\x12\t\n\x05IS_32\x10 \x12\t\n\x05IS_64\x10@:E\n\x0enanopb_fileopt\x12\x1c.google.protobuf.FileOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:G\n\rnanopb_msgopt\x12\x1f.google.protobuf.MessageOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:E\n\x0enanopb_enumopt\x12\x1c.google.protobuf.EnumOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:>\n\x06nanopb\x12\x1d.google.protobuf.FieldOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptionsB\x1a\n\x18\x66i.kapsi.koti.jpa.nanopb'
+  ,
+  dependencies=[google_dot_protobuf_dot_descriptor__pb2.DESCRIPTOR,])
+
+_FIELDTYPE = _descriptor.EnumDescriptor(
+  name='FieldType',
+  full_name='FieldType',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
-      name='SUBNODE', index=0, number=1,
+      name='FT_DEFAULT', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='HEADNODE', index=1, number=2,
+      name='FT_CALLBACK', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='SINK', index=2, number=4,
+      name='FT_POINTER', index=2, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='ROLE_UNKNOWN', index=3, number=255,
+      name='FT_STATIC', index=3, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=321,
-  serialized_end=387,
-)
-_sym_db.RegisterEnumDescriptor(_BASEROLE)
-
-BaseRole = enum_type_wrapper.EnumTypeWrapper(_BASEROLE)
-_MESSAGESENDINGTYPE = _descriptor.EnumDescriptor(
-  name='MessageSendingType',
-  full_name='com.wirepas.proto.wnt.MessageSendingType',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
     _descriptor.EnumValueDescriptor(
-      name='MESSAGE_SENDING_TYPE_INSTANT', index=0, number=1,
+      name='FT_IGNORE', index=4, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='MESSAGE_SENDING_TYPE_DISTRIBUTED', index=1, number=2,
+      name='FT_INLINE', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=389,
-  serialized_end=481,
+  serialized_start=472,
+  serialized_end=577,
 )
-_sym_db.RegisterEnumDescriptor(_MESSAGESENDINGTYPE)
+_sym_db.RegisterEnumDescriptor(_FIELDTYPE)
 
-MessageSendingType = enum_type_wrapper.EnumTypeWrapper(_MESSAGESENDINGTYPE)
-_SELECTIONTYPE = _descriptor.EnumDescriptor(
-  name='SelectionType',
-  full_name='com.wirepas.proto.wnt.SelectionType',
+FieldType = enum_type_wrapper.EnumTypeWrapper(_FIELDTYPE)
+_INTSIZE = _descriptor.EnumDescriptor(
+  name='IntSize',
+  full_name='IntSize',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
-      name='SELECTION_TYPE_NETWORK', index=0, number=1,
+      name='IS_DEFAULT', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='SELECTION_TYPE_SINK', index=1, number=2,
+      name='IS_8', index=1, number=8,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=483,
-  serialized_end=551,
-)
-_sym_db.RegisterEnumDescriptor(_SELECTIONTYPE)
-
-SelectionType = enum_type_wrapper.EnumTypeWrapper(_SELECTIONTYPE)
-_SCRATCHPADACTION = _descriptor.EnumDescriptor(
-  name='ScratchpadAction',
-  full_name='com.wirepas.proto.wnt.ScratchpadAction',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
     _descriptor.EnumValueDescriptor(
-      name='SCRATCHPAD_ACTION_UNKNOWN', index=0, number=0,
+      name='IS_16', index=2, number=16,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='SCRATCHPAD_ACTION_NO_OTAP', index=1, number=1,
+      name='IS_32', index=3, number=32,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='SCRATCHPAD_ACTION_PROPAGATE_ONLY', index=2, number=2,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='SCRATCHPAD_ACTION_PROPAGATE_AND_PROCESS', index=3, number=3,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='SCRATCHPAD_ACTION_PROPAGATE_AND_PROCESS_WITH_DELAY', index=4, number=4,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='SCRATCHPAD_ACTION_LEGACY', index=5, number=5,
+      name='IS_64', index=4, number=64,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=554,
-  serialized_end=803,
+  serialized_start=579,
+  serialized_end=647,
 )
-_sym_db.RegisterEnumDescriptor(_SCRATCHPADACTION)
-
-ScratchpadAction = enum_type_wrapper.EnumTypeWrapper(_SCRATCHPADACTION)
-SUBNODE = 1
-HEADNODE = 2
-SINK = 4
-ROLE_UNKNOWN = 255
-MESSAGE_SENDING_TYPE_INSTANT = 1
-MESSAGE_SENDING_TYPE_DISTRIBUTED = 2
-SELECTION_TYPE_NETWORK = 1
-SELECTION_TYPE_SINK = 2
-SCRATCHPAD_ACTION_UNKNOWN = 0
-SCRATCHPAD_ACTION_NO_OTAP = 1
-SCRATCHPAD_ACTION_PROPAGATE_ONLY = 2
-SCRATCHPAD_ACTION_PROPAGATE_AND_PROCESS = 3
-SCRATCHPAD_ACTION_PROPAGATE_AND_PROCESS_WITH_DELAY = 4
-SCRATCHPAD_ACTION_LEGACY = 5
+_sym_db.RegisterEnumDescriptor(_INTSIZE)
 
-
-
-_FULLROLE = _descriptor.Descriptor(
-  name='FullRole',
-  full_name='com.wirepas.proto.wnt.FullRole',
+IntSize = enum_type_wrapper.EnumTypeWrapper(_INTSIZE)
+FT_DEFAULT = 0
+FT_CALLBACK = 1
+FT_POINTER = 4
+FT_STATIC = 2
+FT_IGNORE = 3
+FT_INLINE = 5
+IS_DEFAULT = 0
+IS_8 = 8
+IS_16 = 16
+IS_32 = 32
+IS_64 = 64
+
+NANOPB_FILEOPT_FIELD_NUMBER = 1010
+nanopb_fileopt = _descriptor.FieldDescriptor(
+  name='nanopb_fileopt', full_name='nanopb_fileopt', index=0,
+  number=1010, type=11, cpp_type=10, label=1,
+  has_default_value=False, default_value=None,
+  message_type=None, enum_type=None, containing_type=None,
+  is_extension=True, extension_scope=None,
+  serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key)
+NANOPB_MSGOPT_FIELD_NUMBER = 1010
+nanopb_msgopt = _descriptor.FieldDescriptor(
+  name='nanopb_msgopt', full_name='nanopb_msgopt', index=1,
+  number=1010, type=11, cpp_type=10, label=1,
+  has_default_value=False, default_value=None,
+  message_type=None, enum_type=None, containing_type=None,
+  is_extension=True, extension_scope=None,
+  serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key)
+NANOPB_ENUMOPT_FIELD_NUMBER = 1010
+nanopb_enumopt = _descriptor.FieldDescriptor(
+  name='nanopb_enumopt', full_name='nanopb_enumopt', index=2,
+  number=1010, type=11, cpp_type=10, label=1,
+  has_default_value=False, default_value=None,
+  message_type=None, enum_type=None, containing_type=None,
+  is_extension=True, extension_scope=None,
+  serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key)
+NANOPB_FIELD_NUMBER = 1010
+nanopb = _descriptor.FieldDescriptor(
+  name='nanopb', full_name='nanopb', index=3,
+  number=1010, type=11, cpp_type=10, label=1,
+  has_default_value=False, default_value=None,
+  message_type=None, enum_type=None, containing_type=None,
+  is_extension=True, extension_scope=None,
+  serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key)
+
+
+_NANOPBOPTIONS = _descriptor.Descriptor(
+  name='NanoPBOptions',
+  full_name='NanoPBOptions',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='base_role', full_name='com.wirepas.proto.wnt.FullRole.base_role', index=0,
-      number=1, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=1,
+      name='max_size', full_name='NanoPBOptions.max_size', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='cb_mac', full_name='com.wirepas.proto.wnt.FullRole.cb_mac', index=1,
-      number=2, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
+      name='max_length', full_name='NanoPBOptions.max_length', index=1,
+      number=14, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='is_autorole', full_name='com.wirepas.proto.wnt.FullRole.is_autorole', index=2,
+      name='max_count', full_name='NanoPBOptions.max_count', index=2,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='int_size', full_name='NanoPBOptions.int_size', index=3,
+      number=7, type=14, cpp_type=8, label=1,
+      has_default_value=True, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='type', full_name='NanoPBOptions.type', index=4,
+      number=3, type=14, cpp_type=8, label=1,
+      has_default_value=True, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='long_names', full_name='NanoPBOptions.long_names', index=5,
       number=4, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
+      has_default_value=True, default_value=True,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=40,
-  serialized_end=139,
-)
-
-
-_APPCONFIGDATA = _descriptor.Descriptor(
-  name='AppConfigData',
-  full_name='com.wirepas.proto.wnt.AppConfigData',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
     _descriptor.FieldDescriptor(
-      name='interval', full_name='com.wirepas.proto.wnt.AppConfigData.interval', index=0,
-      number=1, type=13, cpp_type=3, label=1,
-      has_default_value=False, default_value=0,
+      name='packed_struct', full_name='NanoPBOptions.packed_struct', index=6,
+      number=5, type=8, cpp_type=7, label=1,
+      has_default_value=True, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='sequence', full_name='com.wirepas.proto.wnt.AppConfigData.sequence', index=1,
-      number=2, type=13, cpp_type=3, label=1,
-      has_default_value=False, default_value=0,
+      name='packed_enum', full_name='NanoPBOptions.packed_enum', index=7,
+      number=10, type=8, cpp_type=7, label=1,
+      has_default_value=True, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='skip_message', full_name='NanoPBOptions.skip_message', index=8,
+      number=6, type=8, cpp_type=7, label=1,
+      has_default_value=True, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='app_config', full_name='com.wirepas.proto.wnt.AppConfigData.app_config', index=2,
-      number=3, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
+      name='no_unions', full_name='NanoPBOptions.no_unions', index=9,
+      number=8, type=8, cpp_type=7, label=1,
+      has_default_value=True, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='max_length', full_name='com.wirepas.proto.wnt.AppConfigData.max_length', index=3,
-      number=4, type=13, cpp_type=3, label=1,
+      name='msgid', full_name='NanoPBOptions.msgid', index=10,
+      number=9, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='is_override_on', full_name='com.wirepas.proto.wnt.AppConfigData.is_override_on', index=4,
-      number=5, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
+      name='anonymous_oneof', full_name='NanoPBOptions.anonymous_oneof', index=11,
+      number=11, type=8, cpp_type=7, label=1,
+      has_default_value=True, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='proto3', full_name='NanoPBOptions.proto3', index=12,
+      number=12, type=8, cpp_type=7, label=1,
+      has_default_value=True, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='selection_type', full_name='com.wirepas.proto.wnt.AppConfigData.selection_type', index=5,
-      number=6, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=1,
+      name='enum_to_string', full_name='NanoPBOptions.enum_to_string', index=13,
+      number=13, type=8, cpp_type=7, label=1,
+      has_default_value=True, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='fixed_length', full_name='NanoPBOptions.fixed_length', index=14,
+      number=15, type=8, cpp_type=7, label=1,
+      has_default_value=True, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -278,37 +279,40 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=142,
-  serialized_end=319,
+  serialized_start=51,
+  serialized_end=470,
 )
 
-_FULLROLE.fields_by_name['base_role'].enum_type = _BASEROLE
-_APPCONFIGDATA.fields_by_name['selection_type'].enum_type = _SELECTIONTYPE
-DESCRIPTOR.message_types_by_name['FullRole'] = _FULLROLE
-DESCRIPTOR.message_types_by_name['AppConfigData'] = _APPCONFIGDATA
-DESCRIPTOR.enum_types_by_name['BaseRole'] = _BASEROLE
-DESCRIPTOR.enum_types_by_name['MessageSendingType'] = _MESSAGESENDINGTYPE
-DESCRIPTOR.enum_types_by_name['SelectionType'] = _SELECTIONTYPE
-DESCRIPTOR.enum_types_by_name['ScratchpadAction'] = _SCRATCHPADACTION
+_NANOPBOPTIONS.fields_by_name['int_size'].enum_type = _INTSIZE
+_NANOPBOPTIONS.fields_by_name['type'].enum_type = _FIELDTYPE
+DESCRIPTOR.message_types_by_name['NanoPBOptions'] = _NANOPBOPTIONS
+DESCRIPTOR.enum_types_by_name['FieldType'] = _FIELDTYPE
+DESCRIPTOR.enum_types_by_name['IntSize'] = _INTSIZE
+DESCRIPTOR.extensions_by_name['nanopb_fileopt'] = nanopb_fileopt
+DESCRIPTOR.extensions_by_name['nanopb_msgopt'] = nanopb_msgopt
+DESCRIPTOR.extensions_by_name['nanopb_enumopt'] = nanopb_enumopt
+DESCRIPTOR.extensions_by_name['nanopb'] = nanopb
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-FullRole = _reflection.GeneratedProtocolMessageType('FullRole', (_message.Message,), {
-  'DESCRIPTOR' : _FULLROLE,
-  '__module__' : 'commons_pb2'
-  # @@protoc_insertion_point(class_scope:com.wirepas.proto.wnt.FullRole)
-  })
-_sym_db.RegisterMessage(FullRole)
-
-AppConfigData = _reflection.GeneratedProtocolMessageType('AppConfigData', (_message.Message,), {
-  'DESCRIPTOR' : _APPCONFIGDATA,
-  '__module__' : 'commons_pb2'
-  # @@protoc_insertion_point(class_scope:com.wirepas.proto.wnt.AppConfigData)
+NanoPBOptions = _reflection.GeneratedProtocolMessageType('NanoPBOptions', (_message.Message,), {
+  'DESCRIPTOR' : _NANOPBOPTIONS,
+  '__module__' : 'nanopb_pb2'
+  # @@protoc_insertion_point(class_scope:NanoPBOptions)
   })
-_sym_db.RegisterMessage(AppConfigData)
+_sym_db.RegisterMessage(NanoPBOptions)
 
+nanopb_fileopt.message_type = _NANOPBOPTIONS
+google_dot_protobuf_dot_descriptor__pb2.FileOptions.RegisterExtension(nanopb_fileopt)
+nanopb_msgopt.message_type = _NANOPBOPTIONS
+google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(nanopb_msgopt)
+nanopb_enumopt.message_type = _NANOPBOPTIONS
+google_dot_protobuf_dot_descriptor__pb2.EnumOptions.RegisterExtension(nanopb_enumopt)
+nanopb.message_type = _NANOPBOPTIONS
+google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(nanopb)
 
+DESCRIPTOR._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/internal_pb2.py` & `wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/internal_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='internal.proto',
   package='com.wirepas.proto.wnt',
   syntax='proto2',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x0einternal.proto\x12\x15\x63om.wirepas.proto.wnt\x1a\rcommons.proto\"\xec\x04\n\x0cNodeMetadata\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x01\x12\x10\n\x08map_uuid\x18\n \x03(\t\x12\x11\n\tarea_uuid\x18\r \x03(\t\x12\x1a\n\x12is_area_uuid_empty\x18\x0e \x01(\x08\x12\x13\n\x0bis_approved\x18\x14 \x01(\x08\x12\x12\n\nis_deleted\x18\x15 \x01(\x08\x12\x19\n\x11is_map_uuid_empty\x18\x16 \x01(\x08\x12\x12\n\nis_virtual\x18\x17 \x01(\x08\x12M\n\x10positioning_role\x18\x1e \x01(\x0e\x32\x33.com.wirepas.proto.wnt.NodeMetadata.PositioningRole\x12\x13\n\x0brssi_offset\x18\x1f \x01(\x05\x12\x15\n\rwpe_scan_time\x18( \x01(\x04\x12\x1c\n\x14wpe_calculation_time\x18) \x01(\x04\x12\x0c\n\x04name\x18\x32 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x33 \x01(\t\x12\x13\n\x0bupdate_time\x18< \x01(\r\x12\"\n\x1a\x61nchor_calculated_latitude\x18\x46 \x01(\x01\x12#\n\x1b\x61nchor_calculated_longitude\x18G \x01(\x01\x12\"\n\x1a\x61nchor_calculated_altitude\x18H \x01(\x01\x12\x19\n\x10originator_token\x18\xff\x01 \x01(\t\"3\n\x0fPositioningRole\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x41NCHOR\x10\x01\x12\x07\n\x03TAG\x10\x02\"l\n\x13RTSituationMetadata\x12\x12\n\ncluster_no\x18\x01 \x01(\r\x12\x14\n\x0c\x63luster_size\x18\x02 \x01(\r\x12\x12\n\nnode_count\x18\x03 \x01(\r\x12\x17\n\x0f\x62\x61\x63kend_version\x18\n \x01(\t\"\xe4\x04\n\x0e\x42\x61\x63kendMessage\x12\x42\n\x07message\x18\x01 \x01(\x0e\x32\x31.com.wirepas.proto.wnt.BackendMessage.MessageType\x12\x11\n\tclient_id\x18\x02 \x01(\r\x12\x19\n\x10originator_token\x18\xff\x01 \x01(\t\"\xdf\x03\n\x0bMessageType\x12\t\n\x05\x44\x65lta\x10\x01\x12\x08\n\x04\x46ull\x10\x02\x12\x17\n\x13RTSituationMetadata\x10\x03\x12\x19\n\x15RTSituationDeleteNode\x10\x04\x12,\n(RTSituationRemoteApiConfigurationStarted\x10\x05\x12)\n%RTSituationRemoteApiActivationStarted\x10\x06\x12+\n\'RTSituationRemoteApiCancellationStarted\x10\x07\x12\x1d\n\x19RTSituationMetadataUpdate\x10\x08\x12\"\n\x1eRTSituationSendPositioningData\x10\t\x12#\n\x1fRTSituationComponentInformation\x10\n\x12 \n\x1cRTSituationQueryNodeMetadata\x10\x0b\x12#\n\x1fRTSituationQueryNetworkMetadata\x10\x0c\x12\x30\n,RTSituationQueryBuildingAndFloorPlanMetadata\x10\r\x12 \n\x1cRTSituationQueryAreaMetadata\x10\x0e\"\x99\x02\n\x0cOnlineStatus\x12:\n\x06status\x18\x01 \x01(\x0e\x32*.com.wirepas.proto.wnt.OnlineStatus.Status\x12\x13\n\x0bupdate_time\x18\x02 \x01(\r\x12\x1e\n\x16last_time_series_write\x18\x03 \x01(\r\x12\x43\n\x0fprevious_status\x18\x04 \x01(\x0e\x32*.com.wirepas.proto.wnt.OnlineStatus.Status\x12!\n\x19is_sink_online_in_gateway\x18\n \x01(\x08\"0\n\x06Status\x12\x0b\n\x07OFFLINE\x10\x00\x12\r\n\tUNCERTAIN\x10\x01\x12\n\n\x06ONLINE\x10\x02\"\xac\x01\n\rTraveltimeKPI\x12\x14\n\x0cqos0_minimum\x18\x01 \x01(\x02\x12\x14\n\x0cqos0_average\x18\x02 \x01(\x02\x12\x14\n\x0cqos0_maximum\x18\x03 \x01(\x02\x12\x14\n\x0cqos1_minimum\x18\x0b \x01(\x02\x12\x14\n\x0cqos1_average\x18\x0c \x01(\x02\x12\x14\n\x0cqos1_maximum\x18\r \x01(\x02\x12\x17\n\x0fwindow_duration\x18\x14 \x01(\x05\"w\n\x10\x42\x61\x63kendHeartbeat\x12\x37\n\x06sender\x18\x01 \x01(\x0e\x32\'.com.wirepas.proto.wnt.BackendComponent\x12\x12\n\ncluster_no\x18\x02 \x01(\r\x12\x16\n\ninterval_s\x18\x03 \x01(\r:\x02\x36\x30\"\x8a\x01\n\x16\x42\x61\x63kendComponentStatus\x12:\n\tcomponent\x18\x01 \x01(\x0e\x32\'.com.wirepas.proto.wnt.BackendComponent\x12\x34\n\x06status\x18\x02 \x01(\x0e\x32$.com.wirepas.proto.wnt.RunningStatus\"Q\n\x07Network\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0bupdate_time\x18\x03 \x01(\r\x12\x17\n\x0fis_delete_nodes\x18\x04 \x01(\x08\"y\n\x04User\x12.\n\x04role\x18\x01 \x01(\x0e\x32 .com.wirepas.proto.wnt.User.Role\x12\x11\n\tuser_name\x18\x02 \x01(\t\x12\x11\n\tfull_name\x18\x03 \x01(\t\"\x1b\n\x04Role\x12\t\n\x05\x41\x64min\x10\x01\x12\x08\n\x04User\x10\x02\"9\n\x08\x42uilding\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0bupdate_time\x18\x03 \x01(\r\"l\n\x0f\x46loorplanCorner\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x01\x12\x10\n\x08x_anchor\x18\x04 \x01(\x01\x12\x10\n\x08y_anchor\x18\x05 \x01(\x01\"\x1f\n\x07XYPoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"+\n\x08XYZPoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\x12\t\n\x01z\x18\x03 \x01(\x01\"}\n\x06Matrix\x12\x0b\n\x03m11\x18\x01 \x01(\x01\x12\x0b\n\x03m12\x18\x02 \x01(\x01\x12\x0b\n\x03m13\x18\x03 \x01(\x01\x12\x0b\n\x03m21\x18\x04 \x01(\x01\x12\x0b\n\x03m22\x18\x05 \x01(\x01\x12\x0b\n\x03m23\x18\x06 \x01(\x01\x12\x0b\n\x03m31\x18\x07 \x01(\x01\x12\x0b\n\x03m32\x18\x08 \x01(\x01\x12\x0b\n\x03m33\x18\t \x01(\x01\"\x9e\x06\n\tFloorPlan\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x62uilding_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\x05\x12\x10\n\x08image_id\x18\x0b \x01(\t\x12\x1a\n\x12image_thumbnail_id\x18\x0c \x01(\t\x12\x13\n\x0bimage_width\x18\r \x01(\r\x12\x14\n\x0cimage_height\x18\x0e \x01(\r\x12?\n\x0fleft_top_corner\x18\x15 \x01(\x0b\x32&.com.wirepas.proto.wnt.FloorplanCorner\x12@\n\x10right_top_corner\x18\x16 \x01(\x0b\x32&.com.wirepas.proto.wnt.FloorplanCorner\x12\x42\n\x12left_bottom_corner\x18\x17 \x01(\x0b\x32&.com.wirepas.proto.wnt.FloorplanCorner\x12\x43\n\x13right_bottom_corner\x18\x18 \x01(\x0b\x32&.com.wirepas.proto.wnt.FloorplanCorner\x12\x38\n\x10\x64istance_point_1\x18\x1f \x01(\x0b\x32\x1e.com.wirepas.proto.wnt.XYPoint\x12\x38\n\x10\x64istance_point_2\x18  \x01(\x0b\x32\x1e.com.wirepas.proto.wnt.XYPoint\x12\x15\n\rdistance_in_m\x18! \x01(\x01\x12\x36\n\x0frotation_matrix\x18( \x01(\x0b\x32\x1d.com.wirepas.proto.wnt.Matrix\x12=\n\x14offset_ecef_to_local\x18) \x01(\x0b\x32\x1f.com.wirepas.proto.wnt.XYZPoint\x12=\n\x14offset_local_to_ecef\x18* \x01(\x0b\x32\x1f.com.wirepas.proto.wnt.XYZPoint\x12\x18\n\x10pixels_per_meter\x18+ \x01(\x01\x12\x13\n\x0bupdate_time\x18\x32 \x01(\r\"2\n\x04\x41RGB\x12\t\n\x01\x41\x18\x01 \x01(\r\x12\t\n\x01R\x18\x02 \x01(\r\x12\t\n\x01G\x18\x03 \x01(\r\x12\t\n\x01\x42\x18\x04 \x01(\r\"<\n\x03LLA\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x01\"\xac\x01\n\x04\x41rea\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rfloor_plan_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12*\n\x05\x63olor\x18\x04 \x01(\x0b\x32\x1b.com.wirepas.proto.wnt.ARGB\x12\x32\n\x0epolygon_points\x18\n \x03(\x0b\x32\x1a.com.wirepas.proto.wnt.LLA\x12\x13\n\x0bupdate_time\x18\x14 \x01(\r\"\x99\x05\n\x15MetadataUpdateMessage\x12\x41\n\x19\x61\x64\x64\x65\x64_or_changed_networks\x18\x01 \x03(\x0b\x32\x1e.com.wirepas.proto.wnt.Network\x12\x38\n\x10\x64\x65leted_networks\x18\x02 \x03(\x0b\x32\x1e.com.wirepas.proto.wnt.Network\x12;\n\x16\x61\x64\x64\x65\x64_or_changed_users\x18\x0b \x03(\x0b\x32\x1b.com.wirepas.proto.wnt.User\x12\x32\n\rdeleted_users\x18\x0c \x03(\x0b\x32\x1b.com.wirepas.proto.wnt.User\x12\x43\n\x1a\x61\x64\x64\x65\x64_or_changed_buildings\x18\x15 \x03(\x0b\x32\x1f.com.wirepas.proto.wnt.Building\x12:\n\x11\x64\x65leted_buildings\x18\x16 \x03(\x0b\x32\x1f.com.wirepas.proto.wnt.Building\x12\x46\n\x1c\x61\x64\x64\x65\x64_or_changed_floor_plans\x18\x1f \x03(\x0b\x32 .com.wirepas.proto.wnt.FloorPlan\x12=\n\x13\x64\x65leted_floor_plans\x18  \x03(\x0b\x32 .com.wirepas.proto.wnt.FloorPlan\x12;\n\x16\x61\x64\x64\x65\x64_or_changed_areas\x18) \x03(\x0b\x32\x1b.com.wirepas.proto.wnt.Area\x12\x32\n\rdeleted_areas\x18* \x03(\x0b\x32\x1b.com.wirepas.proto.wnt.Area\x12\x19\n\x10originator_token\x18\xff\x01 \x01(\t\"\x9c\x03\n\x0fSinkPseudoIdMap\x12\x11\n\tpseudo_id\x18\x01 \x01(\t\x12\x12\n\nnetwork_id\x18\n \x01(\r\x12\x0f\n\x07\x61\x64\x64ress\x18\x0b \x01(\r\x12\x12\n\ngateway_id\x18\x0c \x01(\t\x12\x17\n\x0fgateway_sink_id\x18\r \x01(\t\x12\x38\n\napp_config\x18\x14 \x01(\x0b\x32$.com.wirepas.proto.wnt.AppConfigData\x12\"\n\x1astored_scratchpad_sequence\x18\x15 \x01(\r\x12\x37\n/stored_scratchpad_sequence_update_time_ms_epoch\x18\x16 \x01(\x04\x12\x42\n\x11scratchpad_action\x18\x17 \x01(\x0e\x32\'.com.wirepas.proto.wnt.ScratchpadAction\x12\x17\n\x0ftarget_sequence\x18\x18 \x01(\r\x12\x12\n\ntarget_crc\x18\x19 \x01(\r\x12\x1c\n\x14target_delay_minutes\x18\x1a \x01(\r*\xb1\x01\n\x10\x42\x61\x63kendComponent\x12\x10\n\x0c\x41UTH_MANAGER\x10\x01\x12\x18\n\x14\x44IAGNOSTICS_INJECTOR\x10\x02\x12\x0c\n\x08\x46\x45ROUTER\x10\x03\x12\x14\n\x10METADATA_MANAGER\x10\x04\x12\n\n\x06PARSER\x10\x05\x12\x0f\n\x0bRTSITUATION\x10\x06\x12\x16\n\x12TIMESERIES_MANAGER\x10\x07\x12\x18\n\x14GATEWAY_COMMUNICATOR\x10\x08*b\n\rRunningStatus\x12\x0c\n\x08STARTING\x10\x01\x12\x0b\n\x07RUNNING\x10\n\x12\x1c\n\x18RUNNING_AND_ACKNOWLEDGED\x10\x0b\x12\n\n\x06\x43LOSED\x10\x14\x12\x0c\n\x07UNKNOWN\x10\xff\x01'
+  serialized_pb=b'\n\x0einternal.proto\x12\x15\x63om.wirepas.proto.wnt\x1a\rcommons.proto\"\xec\x04\n\x0cNodeMetadata\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x01\x12\x10\n\x08map_uuid\x18\n \x03(\t\x12\x11\n\tarea_uuid\x18\r \x03(\t\x12\x1a\n\x12is_area_uuid_empty\x18\x0e \x01(\x08\x12\x13\n\x0bis_approved\x18\x14 \x01(\x08\x12\x12\n\nis_deleted\x18\x15 \x01(\x08\x12\x19\n\x11is_map_uuid_empty\x18\x16 \x01(\x08\x12\x12\n\nis_virtual\x18\x17 \x01(\x08\x12M\n\x10positioning_role\x18\x1e \x01(\x0e\x32\x33.com.wirepas.proto.wnt.NodeMetadata.PositioningRole\x12\x13\n\x0brssi_offset\x18\x1f \x01(\x05\x12\x15\n\rwpe_scan_time\x18( \x01(\x04\x12\x1c\n\x14wpe_calculation_time\x18) \x01(\x04\x12\x0c\n\x04name\x18\x32 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x33 \x01(\t\x12\x13\n\x0bupdate_time\x18< \x01(\r\x12\"\n\x1a\x61nchor_calculated_latitude\x18\x46 \x01(\x01\x12#\n\x1b\x61nchor_calculated_longitude\x18G \x01(\x01\x12\"\n\x1a\x61nchor_calculated_altitude\x18H \x01(\x01\x12\x19\n\x10originator_token\x18\xff\x01 \x01(\t\"3\n\x0fPositioningRole\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x41NCHOR\x10\x01\x12\x07\n\x03TAG\x10\x02\"l\n\x13RTSituationMetadata\x12\x12\n\ncluster_no\x18\x01 \x01(\r\x12\x14\n\x0c\x63luster_size\x18\x02 \x01(\r\x12\x12\n\nnode_count\x18\x03 \x01(\r\x12\x17\n\x0f\x62\x61\x63kend_version\x18\n \x01(\t\"\xe4\x04\n\x0e\x42\x61\x63kendMessage\x12\x42\n\x07message\x18\x01 \x01(\x0e\x32\x31.com.wirepas.proto.wnt.BackendMessage.MessageType\x12\x11\n\tclient_id\x18\x02 \x01(\r\x12\x19\n\x10originator_token\x18\xff\x01 \x01(\t\"\xdf\x03\n\x0bMessageType\x12\t\n\x05\x44\x65lta\x10\x01\x12\x08\n\x04\x46ull\x10\x02\x12\x17\n\x13RTSituationMetadata\x10\x03\x12\x19\n\x15RTSituationDeleteNode\x10\x04\x12,\n(RTSituationRemoteApiConfigurationStarted\x10\x05\x12)\n%RTSituationRemoteApiActivationStarted\x10\x06\x12+\n\'RTSituationRemoteApiCancellationStarted\x10\x07\x12\x1d\n\x19RTSituationMetadataUpdate\x10\x08\x12\"\n\x1eRTSituationSendPositioningData\x10\t\x12#\n\x1fRTSituationComponentInformation\x10\n\x12 \n\x1cRTSituationQueryNodeMetadata\x10\x0b\x12#\n\x1fRTSituationQueryNetworkMetadata\x10\x0c\x12\x30\n,RTSituationQueryBuildingAndFloorPlanMetadata\x10\r\x12 \n\x1cRTSituationQueryAreaMetadata\x10\x0e\"\x99\x02\n\x0cOnlineStatus\x12:\n\x06status\x18\x01 \x01(\x0e\x32*.com.wirepas.proto.wnt.OnlineStatus.Status\x12\x13\n\x0bupdate_time\x18\x02 \x01(\r\x12\x1e\n\x16last_time_series_write\x18\x03 \x01(\r\x12\x43\n\x0fprevious_status\x18\x04 \x01(\x0e\x32*.com.wirepas.proto.wnt.OnlineStatus.Status\x12!\n\x19is_sink_online_in_gateway\x18\n \x01(\x08\"0\n\x06Status\x12\x0b\n\x07OFFLINE\x10\x00\x12\r\n\tUNCERTAIN\x10\x01\x12\n\n\x06ONLINE\x10\x02\"\xac\x01\n\rTraveltimeKPI\x12\x14\n\x0cqos0_minimum\x18\x01 \x01(\x02\x12\x14\n\x0cqos0_average\x18\x02 \x01(\x02\x12\x14\n\x0cqos0_maximum\x18\x03 \x01(\x02\x12\x14\n\x0cqos1_minimum\x18\x0b \x01(\x02\x12\x14\n\x0cqos1_average\x18\x0c \x01(\x02\x12\x14\n\x0cqos1_maximum\x18\r \x01(\x02\x12\x17\n\x0fwindow_duration\x18\x14 \x01(\x05\"w\n\x10\x42\x61\x63kendHeartbeat\x12\x37\n\x06sender\x18\x01 \x01(\x0e\x32\'.com.wirepas.proto.wnt.BackendComponent\x12\x12\n\ncluster_no\x18\x02 \x01(\r\x12\x16\n\ninterval_s\x18\x03 \x01(\r:\x02\x36\x30\"\x8a\x01\n\x16\x42\x61\x63kendComponentStatus\x12:\n\tcomponent\x18\x01 \x01(\x0e\x32\'.com.wirepas.proto.wnt.BackendComponent\x12\x34\n\x06status\x18\x02 \x01(\x0e\x32$.com.wirepas.proto.wnt.RunningStatus\"Q\n\x07Network\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0bupdate_time\x18\x03 \x01(\r\x12\x17\n\x0fis_delete_nodes\x18\x04 \x01(\x08\"y\n\x04User\x12.\n\x04role\x18\x01 \x01(\x0e\x32 .com.wirepas.proto.wnt.User.Role\x12\x11\n\tuser_name\x18\x02 \x01(\t\x12\x11\n\tfull_name\x18\x03 \x01(\t\"\x1b\n\x04Role\x12\t\n\x05\x41\x64min\x10\x01\x12\x08\n\x04User\x10\x02\"9\n\x08\x42uilding\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0bupdate_time\x18\x03 \x01(\r\"l\n\x0f\x46loorplanCorner\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x01\x12\x10\n\x08x_anchor\x18\x04 \x01(\x01\x12\x10\n\x08y_anchor\x18\x05 \x01(\x01\"\x1f\n\x07XYPoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"+\n\x08XYZPoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\x12\t\n\x01z\x18\x03 \x01(\x01\"}\n\x06Matrix\x12\x0b\n\x03m11\x18\x01 \x01(\x01\x12\x0b\n\x03m12\x18\x02 \x01(\x01\x12\x0b\n\x03m13\x18\x03 \x01(\x01\x12\x0b\n\x03m21\x18\x04 \x01(\x01\x12\x0b\n\x03m22\x18\x05 \x01(\x01\x12\x0b\n\x03m23\x18\x06 \x01(\x01\x12\x0b\n\x03m31\x18\x07 \x01(\x01\x12\x0b\n\x03m32\x18\x08 \x01(\x01\x12\x0b\n\x03m33\x18\t \x01(\x01\"\x9e\x06\n\tFloorPlan\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x62uilding_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\x05\x12\x10\n\x08image_id\x18\x0b \x01(\t\x12\x1a\n\x12image_thumbnail_id\x18\x0c \x01(\t\x12\x13\n\x0bimage_width\x18\r \x01(\r\x12\x14\n\x0cimage_height\x18\x0e \x01(\r\x12?\n\x0fleft_top_corner\x18\x15 \x01(\x0b\x32&.com.wirepas.proto.wnt.FloorplanCorner\x12@\n\x10right_top_corner\x18\x16 \x01(\x0b\x32&.com.wirepas.proto.wnt.FloorplanCorner\x12\x42\n\x12left_bottom_corner\x18\x17 \x01(\x0b\x32&.com.wirepas.proto.wnt.FloorplanCorner\x12\x43\n\x13right_bottom_corner\x18\x18 \x01(\x0b\x32&.com.wirepas.proto.wnt.FloorplanCorner\x12\x38\n\x10\x64istance_point_1\x18\x1f \x01(\x0b\x32\x1e.com.wirepas.proto.wnt.XYPoint\x12\x38\n\x10\x64istance_point_2\x18  \x01(\x0b\x32\x1e.com.wirepas.proto.wnt.XYPoint\x12\x15\n\rdistance_in_m\x18! \x01(\x01\x12\x36\n\x0frotation_matrix\x18( \x01(\x0b\x32\x1d.com.wirepas.proto.wnt.Matrix\x12=\n\x14offset_ecef_to_local\x18) \x01(\x0b\x32\x1f.com.wirepas.proto.wnt.XYZPoint\x12=\n\x14offset_local_to_ecef\x18* \x01(\x0b\x32\x1f.com.wirepas.proto.wnt.XYZPoint\x12\x18\n\x10pixels_per_meter\x18+ \x01(\x01\x12\x13\n\x0bupdate_time\x18\x32 \x01(\r\"2\n\x04\x41RGB\x12\t\n\x01\x41\x18\x01 \x01(\r\x12\t\n\x01R\x18\x02 \x01(\r\x12\t\n\x01G\x18\x03 \x01(\r\x12\t\n\x01\x42\x18\x04 \x01(\r\"<\n\x03LLA\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x01\"\xac\x01\n\x04\x41rea\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rfloor_plan_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12*\n\x05\x63olor\x18\x04 \x01(\x0b\x32\x1b.com.wirepas.proto.wnt.ARGB\x12\x32\n\x0epolygon_points\x18\n \x03(\x0b\x32\x1a.com.wirepas.proto.wnt.LLA\x12\x13\n\x0bupdate_time\x18\x14 \x01(\r\"\x99\x05\n\x15MetadataUpdateMessage\x12\x41\n\x19\x61\x64\x64\x65\x64_or_changed_networks\x18\x01 \x03(\x0b\x32\x1e.com.wirepas.proto.wnt.Network\x12\x38\n\x10\x64\x65leted_networks\x18\x02 \x03(\x0b\x32\x1e.com.wirepas.proto.wnt.Network\x12;\n\x16\x61\x64\x64\x65\x64_or_changed_users\x18\x0b \x03(\x0b\x32\x1b.com.wirepas.proto.wnt.User\x12\x32\n\rdeleted_users\x18\x0c \x03(\x0b\x32\x1b.com.wirepas.proto.wnt.User\x12\x43\n\x1a\x61\x64\x64\x65\x64_or_changed_buildings\x18\x15 \x03(\x0b\x32\x1f.com.wirepas.proto.wnt.Building\x12:\n\x11\x64\x65leted_buildings\x18\x16 \x03(\x0b\x32\x1f.com.wirepas.proto.wnt.Building\x12\x46\n\x1c\x61\x64\x64\x65\x64_or_changed_floor_plans\x18\x1f \x03(\x0b\x32 .com.wirepas.proto.wnt.FloorPlan\x12=\n\x13\x64\x65leted_floor_plans\x18  \x03(\x0b\x32 .com.wirepas.proto.wnt.FloorPlan\x12;\n\x16\x61\x64\x64\x65\x64_or_changed_areas\x18) \x03(\x0b\x32\x1b.com.wirepas.proto.wnt.Area\x12\x32\n\rdeleted_areas\x18* \x03(\x0b\x32\x1b.com.wirepas.proto.wnt.Area\x12\x19\n\x10originator_token\x18\xff\x01 \x01(\t\"\xd8\x03\n\x0fSinkPseudoIdMap\x12\x11\n\tpseudo_id\x18\x01 \x01(\t\x12\x12\n\nnetwork_id\x18\n \x01(\r\x12\x0f\n\x07\x61\x64\x64ress\x18\x0b \x01(\r\x12\x12\n\ngateway_id\x18\x0c \x01(\t\x12\x17\n\x0fgateway_sink_id\x18\r \x01(\t\x12:\n\rstack_profile\x18\x0e \x01(\x0e\x32#.com.wirepas.proto.wnt.StackProfile\x12\x38\n\napp_config\x18\x14 \x01(\x0b\x32$.com.wirepas.proto.wnt.AppConfigData\x12\"\n\x1astored_scratchpad_sequence\x18\x15 \x01(\r\x12\x37\n/stored_scratchpad_sequence_update_time_ms_epoch\x18\x16 \x01(\x04\x12\x42\n\x11scratchpad_action\x18\x17 \x01(\x0e\x32\'.com.wirepas.proto.wnt.ScratchpadAction\x12\x17\n\x0ftarget_sequence\x18\x18 \x01(\r\x12\x12\n\ntarget_crc\x18\x19 \x01(\r\x12\x1c\n\x14target_delay_minutes\x18\x1a \x01(\r*\xb1\x01\n\x10\x42\x61\x63kendComponent\x12\x10\n\x0c\x41UTH_MANAGER\x10\x01\x12\x18\n\x14\x44IAGNOSTICS_INJECTOR\x10\x02\x12\x0c\n\x08\x46\x45ROUTER\x10\x03\x12\x14\n\x10METADATA_MANAGER\x10\x04\x12\n\n\x06PARSER\x10\x05\x12\x0f\n\x0bRTSITUATION\x10\x06\x12\x16\n\x12TIMESERIES_MANAGER\x10\x07\x12\x18\n\x14GATEWAY_COMMUNICATOR\x10\x08*b\n\rRunningStatus\x12\x0c\n\x08STARTING\x10\x01\x12\x0b\n\x07RUNNING\x10\n\x12\x1c\n\x18RUNNING_AND_ACKNOWLEDGED\x10\x0b\x12\n\n\x06\x43LOSED\x10\x14\x12\x0c\n\x07UNKNOWN\x10\xff\x01'
   ,
   dependencies=[commons__pb2.DESCRIPTOR,])
 
 _BACKENDCOMPONENT = _descriptor.EnumDescriptor(
   name='BackendComponent',
   full_name='com.wirepas.proto.wnt.BackendComponent',
   filename=None,
@@ -71,16 +71,16 @@
       name='GATEWAY_COMMUNICATOR', index=7, number=8,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=4879,
-  serialized_end=5056,
+  serialized_start=4939,
+  serialized_end=5116,
 )
 _sym_db.RegisterEnumDescriptor(_BACKENDCOMPONENT)
 
 BackendComponent = enum_type_wrapper.EnumTypeWrapper(_BACKENDCOMPONENT)
 _RUNNINGSTATUS = _descriptor.EnumDescriptor(
   name='RunningStatus',
   full_name='com.wirepas.proto.wnt.RunningStatus',
@@ -112,16 +112,16 @@
       name='UNKNOWN', index=4, number=255,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=5058,
-  serialized_end=5156,
+  serialized_start=5118,
+  serialized_end=5216,
 )
 _sym_db.RegisterEnumDescriptor(_RUNNINGSTATUS)
 
 RunningStatus = enum_type_wrapper.EnumTypeWrapper(_RUNNINGSTATUS)
 AUTH_MANAGER = 1
 DIAGNOSTICS_INJECTOR = 2
 FEROUTER = 3
@@ -1653,57 +1653,64 @@
       name='gateway_sink_id', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.gateway_sink_id', index=4,
       number=13, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='app_config', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.app_config', index=5,
+      name='stack_profile', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.stack_profile', index=5,
+      number=14, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=1,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='app_config', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.app_config', index=6,
       number=20, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='stored_scratchpad_sequence', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.stored_scratchpad_sequence', index=6,
+      name='stored_scratchpad_sequence', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.stored_scratchpad_sequence', index=7,
       number=21, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='stored_scratchpad_sequence_update_time_ms_epoch', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.stored_scratchpad_sequence_update_time_ms_epoch', index=7,
+      name='stored_scratchpad_sequence_update_time_ms_epoch', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.stored_scratchpad_sequence_update_time_ms_epoch', index=8,
       number=22, type=4, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='scratchpad_action', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.scratchpad_action', index=8,
+      name='scratchpad_action', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.scratchpad_action', index=9,
       number=23, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='target_sequence', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.target_sequence', index=9,
+      name='target_sequence', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.target_sequence', index=10,
       number=24, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='target_crc', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.target_crc', index=10,
+      name='target_crc', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.target_crc', index=11,
       number=25, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='target_delay_minutes', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.target_delay_minutes', index=11,
+      name='target_delay_minutes', full_name='com.wirepas.proto.wnt.SinkPseudoIdMap.target_delay_minutes', index=12,
       number=26, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -1714,15 +1721,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=4464,
-  serialized_end=4876,
+  serialized_end=4936,
 )
 
 _NODEMETADATA.fields_by_name['positioning_role'].enum_type = _NODEMETADATA_POSITIONINGROLE
 _NODEMETADATA_POSITIONINGROLE.containing_type = _NODEMETADATA
 _BACKENDMESSAGE.fields_by_name['message'].enum_type = _BACKENDMESSAGE_MESSAGETYPE
 _BACKENDMESSAGE_MESSAGETYPE.containing_type = _BACKENDMESSAGE
 _ONLINESTATUS.fields_by_name['status'].enum_type = _ONLINESTATUS_STATUS
@@ -1750,14 +1757,15 @@
 _METADATAUPDATEMESSAGE.fields_by_name['deleted_users'].message_type = _USER
 _METADATAUPDATEMESSAGE.fields_by_name['added_or_changed_buildings'].message_type = _BUILDING
 _METADATAUPDATEMESSAGE.fields_by_name['deleted_buildings'].message_type = _BUILDING
 _METADATAUPDATEMESSAGE.fields_by_name['added_or_changed_floor_plans'].message_type = _FLOORPLAN
 _METADATAUPDATEMESSAGE.fields_by_name['deleted_floor_plans'].message_type = _FLOORPLAN
 _METADATAUPDATEMESSAGE.fields_by_name['added_or_changed_areas'].message_type = _AREA
 _METADATAUPDATEMESSAGE.fields_by_name['deleted_areas'].message_type = _AREA
+_SINKPSEUDOIDMAP.fields_by_name['stack_profile'].enum_type = commons__pb2._STACKPROFILE
 _SINKPSEUDOIDMAP.fields_by_name['app_config'].message_type = commons__pb2._APPCONFIGDATA
 _SINKPSEUDOIDMAP.fields_by_name['scratchpad_action'].enum_type = commons__pb2._SCRATCHPADACTION
 DESCRIPTOR.message_types_by_name['NodeMetadata'] = _NODEMETADATA
 DESCRIPTOR.message_types_by_name['RTSituationMetadata'] = _RTSITUATIONMETADATA
 DESCRIPTOR.message_types_by_name['BackendMessage'] = _BACKENDMESSAGE
 DESCRIPTOR.message_types_by_name['OnlineStatus'] = _ONLINESTATUS
 DESCRIPTOR.message_types_by_name['TraveltimeKPI'] = _TRAVELTIMEKPI
```

### Comparing `wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/message_pb2.py` & `wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/message_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,114 +22,18 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='message.proto',
   package='com.wirepas.proto.wnt',
   syntax='proto2',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\rmessage.proto\x12\x15\x63om.wirepas.proto.wnt\x1a\x0cnanopb.proto\x1a\notap.proto\x1a\rcommons.proto\x1a\x0einternal.proto\x1a\x10remote_api.proto\x1a\x11positioning.proto\"\xb7\x03\n\x08Neighbor\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\r\x12\x1b\n\x13\x63luster_channel_MHz\x18\x02 \x01(\x02\x12\x16\n\x0eradio_power_dB\x18\x03 \x01(\x02\x12\x43\n\rneighbor_type\x18\x04 \x01(\x0e\x32,.com.wirepas.proto.wnt.Neighbor.NeighborType\x12\x10\n\x08rssi_dBm\x18\x05 \x01(\x02\x12\x14\n\x0cno_neighbors\x18\x06 \x01(\x08\x12\x17\n\x0f\x63luster_channel\x18\x07 \x01(\r\x12\x33\n+amount_of_cluster_beacon_reception_attempts\x18\x08 \x01(\r\x12:\n2amount_of_failed_cluster_beacon_reception_attempts\x18\t \x01(\r\"n\n\x0cNeighborType\x12\n\n\x06MEMBER\x10\x01\x12\x10\n\x0cSYNC_CLUSTER\x10\x02\x12\x16\n\x12\x41SSOCIATED_CLUSTER\x10\x03\x12\x0c\n\x08UNSYNCED\x10\x04\x12\x1a\n\x15NEIGHBOR_TYPE_UNKNOWN\x10\xff\x01\"C\n\x08\x43ostInfo\x12\x18\n\x10next_hop_address\x18\x02 \x01(\r\x12\x0c\n\x04\x63ost\x18\x03 \x01(\r\x12\x0f\n\x07quality\x18\x04 \x01(\x02\"R\n\x1f\x43\x61lculatedValuesFromDiagnostics\x12/\n\'low_energy_transmission_load_percentage\x18\x01 \x01(\x02\"\xc6\x30\n\x0f\x44iagnosticsData\x12\x39\n\tneighbors\x18\x01 \x03(\x0b\x32\x1f.com.wirepas.proto.wnt.NeighborB\x05\x92?\x02\x10 \x12\x17\n\x0f\x61\x63\x63\x65ss_cycle_ms\x18\x02 \x01(\x02\x12-\n\x04role\x18\x03 \x01(\x0e\x32\x1f.com.wirepas.proto.wnt.BaseRole\x12\x0e\n\x06\x63\x62_mac\x18\x04 \x01(\x08\x12\x13\n\x0bis_autorole\x18\x06 \x01(\x08\x12\x0f\n\x07voltage\x18\x07 \x01(\x02\x12\x18\n\x10max_buffer_usage\x18\x08 \x01(\x02\x12\x1c\n\x14\x61verage_buffer_usage\x18\t \x01(\x02\x12\x17\n\x0fmem_alloc_fails\x18\n \x01(\r\x12\r\n\x05scans\x18\x0c \x01(\r\x12\x18\n\x07\x64ropped\x18\x11 \x03(\rB\x07\x10\x01\x92?\x02\x10\x02\x12\x14\n\x0csink_address\x18\x31 \x01(\r\x12\x34\n\x04\x63ost\x18\x12 \x03(\x0b\x32\x1f.com.wirepas.proto.wnt.CostInfoB\x05\x92?\x02\x10\x02\x12\x46\n\x06\x65vents\x18\x13 \x03(\x0e\x32-.com.wirepas.proto.wnt.DiagnosticsData.EventsB\x07\x10\x01\x92?\x02\x10\x0f\x12\x12\n\nduty_cycle\x18\x14 \x01(\x02\x12\x0f\n\x07\x61ntenna\x18\x15 \x01(\r\x12\x1b\n\x13\x63luster_channel_MHz\x18\x17 \x01(\x02\x12\x1b\n\x13\x63hannel_reliability\x18\x18 \x01(\x02\x12\x16\n\x0e\x61loha_rx_ratio\x18\x1b \x01(\x02\x12\x1f\n\x17max_reserved_slot_usage\x18! \x01(\x02\x12\x1f\n\x17\x61vg_reserved_slot_usage\x18\x30 \x01(\x02\x12\x1c\n\x14max_aloha_slot_usage\x18\" \x01(\x02\x12\x12\n\nboot_count\x18# \x01(\r\x12\x18\n\x10sw_version_devel\x18$ \x01(\r\x12\x1e\n\x16sw_version_maintenance\x18% \x01(\r\x12\x18\n\x10sw_version_minor\x18& \x01(\r\x12\x18\n\x10sw_version_major\x18\' \x01(\r\x12\x1b\n\x13scratchpad_sequence\x18( \x01(\r\x12@\n\x08hw_magic\x18) \x01(\x0e\x32..com.wirepas.proto.wnt.DiagnosticsData.HWMagic\x12:\n\rstack_profile\x18* \x01(\x0e\x32#.com.wirepas.proto.wnt.StackProfile\x12\x14\n\x0cotap_enabled\x18+ \x01(\x08\x12\x18\n\x10\x62oot_line_number\x18, \x01(\r\x12\x11\n\tfile_hash\x18- \x01(\r\x12\x1c\n\x0bstack_trace\x18. \x03(\rB\x07\x10\x01\x92?\x02\x10\x03\x12\x1f\n\x17routers_in_neighborhood\x18\x32 \x01(\r\x12\x13\n\x0b\x63\x62_mac_load\x18\x33 \x01(\x02\x12\x1d\n\x15\x63luster_member_amount\x18\x34 \x01(\r\x12\"\n\x1a\x63luster_router_node_amount\x18\x35 \x01(\r\x12&\n\x1e\x62lacklisted_radio_channels_1_8\x18\x36 \x01(\r\x12\'\n\x1f\x62lacklisted_radio_channels_9_16\x18\x37 \x01(\r\x12(\n blacklisted_radio_channels_17_24\x18\x38 \x01(\r\x12(\n blacklisted_radio_channels_25_32\x18\x39 \x01(\r\x12(\n blacklisted_radio_channels_33_40\x18: \x01(\r\x12$\n\x1cscratchpad_firmware_sequence\x18; \x01(\r\x12$\n\x1c\x62roadcast_ll_members_pending\x18< \x01(\r\x12$\n\x1c\x62roadcast_le_members_pending\x18= \x01(\r\x12\"\n\x1a\x62roadcast_next_hop_pending\x18> \x01(\r\x12\x1f\n\x17\x62roadcast_unack_pending\x18? \x01(\r\x12\x1f\n\x17packets_expired_pending\x18@ \x01(\r\x12\x1f\n\x17packets_reroute_pending\x18\x41 \x01(\r\x12\x1f\n\x17unicast_cluster_pending\x18\x42 \x01(\r\x12\x1f\n\x17unicast_members_pending\x18\x43 \x01(\r\x12 \n\x18\x64ropped_packets_combined\x18\x44 \x01(\r\x12\x1d\n\x15\x63\x62mac_rx_messages_ack\x18\x45 \x01(\r\x12\x1f\n\x17\x63\x62mac_rx_messages_unack\x18\x46 \x01(\r\x12\"\n\x1a\x63\x62mac_rx_ack_other_reasons\x18G \x01(\r\x12\x1d\n\x15\x63\x62mac_tx_ack_cca_fail\x18H \x01(\r\x12!\n\x19\x63\x62mac_tx_ack_not_received\x18I \x01(\r\x12\x1d\n\x15\x63\x62mac_tx_messages_ack\x18J \x01(\r\x12\x1f\n\x17\x63\x62mac_tx_messages_unack\x18K \x01(\r\x12\x1f\n\x17\x63\x62mac_tx_cca_unack_fail\x18L \x01(\r\x12\x1a\n\x12\x63\x66mac_messages_ack\x18M \x01(\r\x12)\n!cfmac_pending_broadcast_le_member\x18N \x01(\r\x12\x1f\n\x17next_hop_radio_power_dB\x18O \x01(\x05\x12\x19\n\x11next_hop_rssi_dBm\x18P \x01(\x05\x12(\n blacklisted_radio_channels_count\x18Q \x01(\r\x12!\n\x19\x61pplication_version_major\x18R \x01(\r\x12!\n\x19\x61pplication_version_minor\x18S \x01(\r\x12\'\n\x1f\x61pplication_version_maintenance\x18T \x01(\r\x12!\n\x19\x61pplication_version_devel\x18U \x01(\r\x12\x44\n\ntrace_type\x18V \x01(\x0e\x32\x30.com.wirepas.proto.wnt.DiagnosticsData.TraceType\x12\x1e\n\x16packet_sequence_number\x18W \x01(\r\x12\x17\n\x0f\x63luster_channel\x18X \x01(\r\x12\x14\n\x0csleep_time_s\x18Y \x01(\r\x12\x46\n\x0b\x62oot_reason\x18Z \x01(\x0e\x32\x31.com.wirepas.proto.wnt.DiagnosticsData.BootReason\x12\x0f\n\x07rx_gain\x18[ \x01(\x05\x12\x1a\n\ttx_powers\x18\\ \x03(\x05\x42\x07\x10\x01\x92?\x02\x10\x10\x12\x1c\n\x14scratchpad_transfers\x18] \x01(\r\x12\x1c\n\x14installation_quality\x18^ \x01(\x02\x12m\n\x1binstallation_quality_errors\x18_ \x03(\x0e\x32?.com.wirepas.proto.wnt.DiagnosticsData.InstallationQualityErrorB\x07\x10\x01\x92?\x02\x10\x03\x12\'\n\x1f\x64ropped_unack_broadcast_packets\x18` \x01(\r\x12<\n4unacknowledged_broadcast_transmissions_channel_count\x18\x61 \x01(\r\x12+\n#wide_band_noise_rssi_correction_dBm\x18\x62 \x01(\x05\x12\x31\n)network_channel_packet_error_rate_percent\x18\x63 \x01(\x02\x12)\n!boot_diagnostics_tx_time_ms_epoch\x18\x64 \x01(\x04\x12\x15\n\rcca_limit_dBm\x18\x65 \x01(\x05\x12\x17\n\x0f\x61\x64\x64ress_clashes\x18\x66 \x01(\r\x12\x17\n\x0fll_device_count\x18g \x01(\r\x12\x1a\n\x12is_ble_scan_active\x18h \x01(\x08\x12$\n\x1c\x63ost_compensation_throughput\x18i \x01(\r\x12\"\n\x1a\x63ost_compensation_bad_link\x18j \x01(\r\x12%\n\x1d\x63ost_compensation_bad_channel\x18k \x01(\r\x12.\n&cost_compensation_price_of_association\x18l \x01(\r\x12+\n#cost_compensation_high_buffer_usage\x18m \x01(\r\x12\x31\n)cost_compensation_high_energy_consumption\x18n \x01(\r\x12 \n\x18is_joining_beacon_active\x18o \x01(\x08\x12#\n\x1b\x61mount_of_flooding_messages\x18p \x01(\r\x12-\n%amount_of_dropped_reassembled_packets\x18q \x01(\r\x12\x1b\n\x13modem_version_devel\x18r \x01(\r\x12!\n\x19modem_version_maintenance\x18s \x01(\r\x12\x1b\n\x13modem_version_minor\x18t \x01(\r\x12\x1b\n\x13modem_version_major\x18u \x01(\r\"\xc7\x0e\n\x06\x45vents\x12\x12\n\x0eROLE_NO_EVENTS\x10\x00\x12\x1c\n\x18SCAN_REASON_INITIAL_SCAN\x10\x01\x12\"\n\x1eSCAN_REASON_RESTRICTED_CHANNEL\x10\x02\x12\x1e\n\x1aSCAN_REASON_MAJOR_BOUNDARY\x10\x03\x12\x1a\n\x16SCAN_REASON_NO_CHANNEL\x10\x04\x12\x19\n\x15SCAN_REASON_BLACKLIST\x10\x05\x12\x1a\n\x16ROLE_CHANGE_TO_SUBNODE\x10\x08\x12\x1b\n\x17ROLE_CHANGE_TO_HEADNODE\x10\t\x12\x10\n\x0cROUTE_CHANGE\x10\x10\x12\x1d\n\x19SCAN_REASON_NEXT_HOP_LOST\x10\x14\x12\x1f\n\x1bSCAN_REASON_BOUNDARY_CHANGE\x10\x15\x12\x18\n\x14SCAN_REASON_HIGH_PER\x10\x16\x12\x1f\n\x1bSCANNING_REQ_BY_APPLICATION\x10\x17\x12 \n\x1cSCANNING_NO_CHANNEL_SELECTED\x10\x18\x12%\n!SCANNING_FTDMA_CONF_WITH_NEIGHBOR\x10\x19\x12(\n$SCANNING_FTDMA_CONF_WITH_NB_NEIGHBOR\x10\x1a\x12&\n\"SCANNING_TIMING_CONF_WITH_NEIGHBOR\x10\x1b\x12\x30\n,SCANNING_TIMING_CONF_WITH_MULTIPLE_NEIGHBORS\x10\x1c\x12 \n\x1cSCANNING_NEED_MORE_NEIGHBORS\x10\x1d\x12\x15\n\x11SCANNING_PERIODIC\x10\x1e\x12\x18\n\x14SCANNING_ROLE_CHANGE\x10\x1f\x12\x10\n\x0c\x42OOT_POWERON\x10 \x12\x14\n\x10\x42OOT_INTENTIONAL\x10!\x12\x13\n\x0f\x42OOT_SW_FAILURE\x10\"\x12\x1a\n\x16\x42OOT_PROCESSOR_FAILURE\x10#\x12\x18\n\x14\x42OOT_WATCHDOG_EXPIRE\x10$\x12\x1d\n\x19\x42OOT_UNINDENTIFIED_REASON\x10%\x12\x1e\n\x1aSYNCLOST_ALTERNATIVE_ROUTE\x10(\x12\x1a\n\x16SYNCLOST_PRIMARY_ROUTE\x10)\x12\x1c\n\x18\x46TDMA_ADJ_MINOR_BOUNDARY\x10\x30\x12\"\n\x1e\x46TDMA_ADJ_NOT_IN_SLOT_BOUNDARY\x10\x31\x12)\n%FTDMA_ADJ_CONFLICT_WITH_PRIMARY_ROUTE\x10\x32\x12-\n)FTDMA_ADJ_CONFLICT_WITH_ALTERNATIVE_ROUTE\x10\x33\x12$\n FTDMA_ADJ_CONFLICT_WITH_NEIGHBOR\x10\x34\x12!\n\x1d\x46TDMA_ADJ_NO_CHANNEL_SELECTED\x10\x35\x12!\n\x1d\x46TDMA_ADJ_CHANNEL_BLACKLISTED\x10\x36\x12\x1a\n\x16\x46TDMA_ADJ_OTHER_REASON\x10\x37\x12\x10\n\x0cSINK_CHANGED\x10\x38\x12\x0f\n\x0b\x46HMA_ADJUST\x10\x39\x12\x16\n\x12TDMA_ADJUST_CCSTAT\x10:\x12\x10\n\x0cROUTING_LOOP\x10@\x12\x18\n\x14\x44\x45NSE_REMOVE_SUBNODE\x10H\x12#\n\x1f\x44OWNLINK_TX_FAIL_COULD_NOT_SEND\x10I\x12,\n(DOWNLINK_TX_FAIL_NEXT_HOP_COULD_NOT_SEND\x10J\x12!\n\x1dUPLINK_TX_FAIL_COULD_NOT_SEND\x10K\x12 \n\x1cTOO_MANY_ROUTERS_DURING_SCAN\x10L\x12,\n(TIMING_LATE_FOR_SCHEDULING_MAC_OPERATION\x10M\x12\x1a\n\x16SCAN_REASON_ADVERTISER\x10N\x12\x13\n\x0fSCAN_REASON_APC\x10O\x12\x13\n\x0eRESET_NEW_BASE\x10\xc8\x01\x12\x10\n\x0bRESET_MODEM\x10\xce\x01\x12\x15\n\x10RESET_MODEM_INIT\x10\xcf\x01\x12\x13\n\x0eRESET_SOFT_WDT\x10\xd0\x01\x12\x0e\n\tRESET_NMI\x10\xd1\x01\x12\x15\n\x10RESET_HARD_FAULT\x10\xd2\x01\x12\x14\n\x0fRESET_BUS_FAULT\x10\xd3\x01\x12\x16\n\x11RESET_USAGE_FAULT\x10\xd4\x01\x12\x1b\n\x16RESET_MEM_MANAGE_FAULT\x10\xd5\x01\x12\x0e\n\tRESET_PIN\x10\xd6\x01\x12\x15\n\x10RESET_CPU_LOCKUP\x10\xd7\x01\x12\x1c\n\x17RESET_SYSTEM_OFF_WAKEUP\x10\xd8\x01\x12\x13\n\x0eRESET_BROWNOUT\x10\xd9\x01\x12\x13\n\x0eRESET_SECURITY\x10\xda\x01\x12\x12\n\rRESET_REQUEST\x10\xdb\x01\x12\x12\n\rEVENT_UNKNOWN\x10\xff\x01\"\xc2\x02\n\x07HWMagic\x12\t\n\x05NRF51\x10\x01\x12\t\n\x05\x45ZR32\x10\x02\x12\t\n\x05NRF52\x10\x03\x12\n\n\x06\x43\x43\x32\x36\x35\x30\x10\x04\x12\x1a\n\x16\x45\x46R32XG12_1024KB_128KB\x10\x05\x12\x19\n\x15NRF52840_1024KB_256KB\x10\x06\x12\x18\n\x14\x45\x46R32XG12_512KB_64KB\x10\x07\x12\x13\n\x0f\x45\x46R32XG13_512KB\x10\x08\x12\x0c\n\x08NRF52833\x10\t\x12\r\n\tEFR32XG21\x10\n\x12\r\n\tEFR32XG22\x10\x0b\x12\x11\n\rBGM210PA22JIA\x10\x0c\x12\x11\n\rBGM220PC22HNA\x10\r\x12\x11\n\rBGM220SC22HNA\x10\x0e\x12\x0b\n\x07NRF9160\x10\x0f\x12\r\n\tEFR32XG23\x10\x10\x12\r\n\tEFR32XG24\x10\x11\x12\x14\n\x0fHWMAGIC_UNKNOWN\x10\xff\x01\"\x87\x01\n\tTraceType\x12\x14\n\x10NODE_DIAGNOSTICS\x10\x01\x12\x18\n\x14NEIGHBOR_DIAGNOSTICS\x10\x02\x12\x14\n\x10SCAN_DIAGNOSTICS\x10\x03\x12\x14\n\x10\x42OOT_DIAGNOSTICS\x10\x04\x12\x1e\n\x1a\x42OOT_DIAGNOSTICS_WM_FW_5_0\x10\x07\"\xbb\x01\n\nBootReason\x12!\n\x1dNORMAL_POWER_ON_RESET_STARTUP\x10\x00\x12\x30\n,REBOOT_REQUESTED_AS_PART_OF_NORMAL_OPERATION\x10\x01\x12\x1b\n\x17SOFTWARE_ASSERT_FAILURE\x10\x02\x12\r\n\tMCU_FAULT\x10\x03\x12\x12\n\x0eWATCHDOG_RESET\x10\x04\x12\x18\n\x14UNKNOWN_RESET_REASON\x10\x05\"X\n\x18InstallationQualityError\x12\x14\n\x10NO_ROUTE_TO_SINK\x10\x00\x12\x18\n\x14NOT_ENOUGH_NEIGHBORS\x10\x01\x12\x0c\n\x08\x42\x41\x44_RSSI\x10\x02\"\x8d\x02\n\x06RxData\x12\x17\n\x0fsource_endpoint\x18\x02 \x01(\r\x12\x1c\n\x14\x64\x65stination_endpoint\x18\x04 \x01(\r\x12\x0e\n\x03qos\x18\x05 \x01(\r:\x01\x30\x12\x0f\n\x07payload\x18\x07 \x01(\x0c\x12\x14\n\x0cpayload_size\x18\x08 \x01(\r\x12\x14\n\x0csink_address\x18\t \x01(\r\x12\x11\n\thop_count\x18\n \x01(\r\x12 \n\x18gateway_rx_time_ms_epoch\x18\x0b \x01(\x04\x12 \n\x18\x62\x61\x63kend_rx_time_ms_epoch\x18\x0c \x01(\x04\x12(\n gateway_backend_rx_time_delta_ms\x18\r \x01(\x05\"\xc8\x06\n\x11\x41ppConfigResponse\x12H\n\x06result\x18\x01 \x01(\x0e\x32\x38.com.wirepas.proto.wnt.AppConfigResponse.AppConfigResult\"\xe8\x05\n\x0f\x41ppConfigResult\x12\x1f\n\x12UNKNOWN_ERROR_CODE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x06\n\x02OK\x10\x00\x12\x12\n\x0eINTERNAL_ERROR\x10\x01\x12\x13\n\x0fINVALID_SINK_ID\x10\x02\x12\x10\n\x0cINVALID_ROLE\x10\x03\x12\x1b\n\x17INVALID_NETWORK_ADDRESS\x10\x04\x12\x1b\n\x17INVALID_NETWORK_CHANNEL\x10\x05\x12\x17\n\x13INVALID_CHANNEL_MAP\x10\x06\x12\x18\n\x14INVALID_NETWORK_KEYS\x10\x07\x12\x14\n\x10INVALID_AC_RANGE\x10\x08\x12\x16\n\x12INVALID_SINK_STATE\x10\t\x12\x18\n\x14INVALID_DEST_ADDRESS\x10\n\x12\x19\n\x15INVALID_DEST_ENDPOINT\x10\x0b\x12\x18\n\x14INVALID_SRC_ENDPOINT\x10\x0c\x12\x0f\n\x0bINVALID_QOS\x10\r\x12\x18\n\x14INVALID_DATA_PAYLOAD\x10\x0e\x12\x16\n\x12INVALID_SCRATCHPAD\x10\x0f\x12\x1b\n\x17INVALID_SCRATCHPAD_SIZE\x10\x10\x12\x1b\n\x17INVALID_SEQUENCE_NUMBER\x10\x11\x12\x18\n\x14INVALID_REBOOT_DELAY\x10\x12\x12\x19\n\x15INVALID_DIAG_INTERVAL\x10\x13\x12\x16\n\x12INVALID_APP_CONFIG\x10\x14\x12\x11\n\rINVALID_PARAM\x10\x15\x12\x19\n\x15NO_SCRATCHPAD_PRESENT\x10\x16\x12\x11\n\rACCESS_DENIED\x10\x17\x12\x19\n\x15REQUEST_NEEDS_SINK_ID\x10\x18\x12\x19\n\x15INVALID_MAX_HOP_COUNT\x10\x19\x12\x16\n\x12SINK_OUT_OF_MEMORY\x10\x1a\x12\x10\n\x0cSINK_TIMEOUT\x10\x1b\x12\x1c\n\x18\x46IRST_INVALID_ENUM_VALUE\x10\x1c\"V\n\x0bMeasurement\x12\x11\n\tsensor_id\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04unit\x18\x04 \x01(\t\x12\x17\n\x0fno_measurements\x18\x05 \x01(\x08\"9\n\x10GatewayHeartbeat\x12\x13\n\x0bmac_address\x18\x01 \x01(\t\x12\x10\n\x08hostname\x18\x03 \x01(\t\"`\n\x0bGatewayInfo\x12\x1c\n\x14\x63urrent_time_s_epoch\x18\x01 \x01(\r\x12\r\n\x05model\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x13\n\x0b\x61pi_version\x18\x04 \x01(\r\"p\n\x14\x42\x61\x63kendComponentInfo\x12\x1c\n\x14\x63urrent_time_s_epoch\x18\x01 \x01(\r\x12:\n\tcomponent\x18\x02 \x01(\x0e\x32\'.com.wirepas.proto.wnt.BackendComponent\"2\n\x12\x43hannelIdToFreqMap\x12\n\n\x02id\x18\x01 \x01(\r\x12\x10\n\x08\x66req_MHz\x18\x02 \x01(\x02\"3\n\x11\x41\x63\x63\x65ssCycleLimits\x12\x0e\n\x06min_ms\x18\x01 \x01(\r\x12\x0e\n\x06max_ms\x18\x02 \x01(\r\"\x95\x01\n\x0bNodeMessage\x12\x1b\n\x13\x64\x65stination_address\x18\x01 \x01(\r\x12\x12\n\nnetwork_id\x18\x02 \x01(\r\x12\x18\n\x10source_end_point\x18\x03 \x01(\r\x12\x1d\n\x15\x64\x65stination_end_point\x18\x04 \x01(\r\x12\x0b\n\x03qos\x18\x05 \x01(\r\x12\x0f\n\x07payload\x18\x06 \x01(\x0c\"\xde\x01\n\x13GetScratchpadStatus\x12\x12\n\nnetwork_id\x18\x01 \x01(\r\x12\x19\n\x11resend_interval_s\x18\x02 \x01(\r\x12\x10\n\x08is_close\x18\x03 \x01(\x08\x12\x14\n\x0cis_sink_only\x18\x04 \x01(\x08\x12G\n\x14message_sending_type\x18\x05 \x01(\x0e\x32).com.wirepas.proto.wnt.MessageSendingType\x12\'\n\x1fmessage_distribution_interval_s\x18\x06 \x01(\r\"\x8f\t\n\x10ScratchpadStatus\x12\x1e\n\x16is_continuous_query_on\x18\x01 \x01(\x08\x12\x18\n\x10tx_time_ms_epoch\x18\x02 \x01(\x04\x12\x1e\n\x16stored_scratchpad_size\x18\n \x01(\r\x12\x1d\n\x15stored_scratchpad_crc\x18\x0b \x01(\r\x12\"\n\x1astored_scratchpad_sequence\x18\x0c \x01(\r\x12\x45\n\x16stored_scratchpad_type\x18\r \x01(\x0e\x32%.com.wirepas.proto.wnt.ScratchpadType\x12N\n\x18stored_scratchpad_status\x18\x0e \x01(\x0e\x32,.com.wirepas.proto.wnt.ScratchpadWriteStatus\x12$\n\x1cprocessed_fw_scratchpad_size\x18\x14 \x01(\r\x12#\n\x1bprocessed_fw_scratchpad_crc\x18\x15 \x01(\r\x12(\n processed_fw_scratchpad_sequence\x18\x16 \x01(\r\x12\x1c\n\x14processed_fw_area_id\x18\x17 \x01(\r\x12\"\n\x1aprocessed_fw_version_major\x18\x18 \x01(\r\x12\"\n\x1aprocessed_fw_version_minor\x18\x19 \x01(\r\x12(\n processed_fw_version_maintenance\x18\x1a \x01(\r\x12\"\n\x1aprocessed_fw_version_devel\x18\x1b \x01(\r\x12-\n%processed_application_scratchpad_size\x18( \x01(\r\x12,\n$processed_application_scratchpad_crc\x18) \x01(\r\x12\x31\n)processed_application_scratchpad_sequence\x18* \x01(\r\x12%\n\x1dprocessed_application_area_id\x18+ \x01(\r\x12+\n#processed_application_version_major\x18, \x01(\r\x12+\n#processed_application_version_minor\x18- \x01(\r\x12\x31\n)processed_application_version_maintenance\x18. \x01(\r\x12+\n#processed_application_version_devel\x18/ \x01(\r\x12\x42\n\x11scratchpad_action\x18< \x01(\x0e\x32\'.com.wirepas.proto.wnt.ScratchpadAction\x12\x17\n\x0ftarget_sequence\x18= \x01(\r\x12\x12\n\ntarget_crc\x18> \x01(\r\x12\x1c\n\x14target_delay_minutes\x18? \x01(\r\x12\x1e\n\x16remaining_time_minutes\x18@ \x01(\r\"m\n\x13SetScratchpadAction\x12\x12\n\nnetwork_id\x18\x01 \x01(\r\x12\x42\n\x11scratchpad_action\x18\x02 \x01(\x0e\x32\'.com.wirepas.proto.wnt.ScratchpadAction\"\xc8\x12\n\x07Message\x12\x0e\n\x02id\x18\x01 \x03(\rB\x02\x10\x01\x12\x12\n\nnetwork_id\x18\x02 \x01(\r\x12\x12\n\ngateway_id\x18\x03 \x01(\t\x12\x0f\n\x07tx_time\x18\x04 \x01(\x04\x12\x0f\n\x07rx_time\x18\x05 \x01(\x04\x12\x16\n\x0esource_address\x18\x07 \x01(\r\x12\x1b\n\x13\x64\x65stination_address\x18\x08 \x01(\r\x12\x16\n\x0etravel_time_ms\x18\t \x01(\x02\x12;\n\x0b\x64iagnostics\x18\x32 \x01(\x0b\x32&.com.wirepas.proto.wnt.DiagnosticsData\x12.\n\x07rx_data\x18\x33 \x01(\x0b\x32\x1d.com.wirepas.proto.wnt.RxData\x12\x38\n\napp_config\x18\x34 \x01(\x0b\x32$.com.wirepas.proto.wnt.AppConfigData\x12:\n\rstack_profile\x18\x35 \x01(\x0e\x32#.com.wirepas.proto.wnt.StackProfile\x12\x37\n\x0bmeasurement\x18\x36 \x03(\x0b\x32\".com.wirepas.proto.wnt.Measurement\x12=\n\x0cgw_heartbeat\x18\x37 \x01(\x0b\x32\'.com.wirepas.proto.wnt.GatewayHeartbeat\x12.\n\x07tx_data\x18\x38 \x01(\x0b\x32\x1d.com.wirepas.proto.wnt.RxData\x12\x17\n\x0fnetwork_channel\x18: \x01(\r\x12\x18\n\x10security_enabled\x18; \x01(\x08\x12?\n\x0c\x63hannel_info\x18< \x03(\x0b\x32).com.wirepas.proto.wnt.ChannelIdToFreqMap\x12\x45\n\x13\x61pp_config_response\x18= \x01(\x0b\x32(.com.wirepas.proto.wnt.AppConfigResponse\x12\x45\n\x13\x61\x63\x63\x65ss_cycle_limits\x18> \x01(\x0b\x32(.com.wirepas.proto.wnt.AccessCycleLimits\x12\x38\n\x0cgateway_info\x18? \x01(\x0b\x32\".com.wirepas.proto.wnt.GatewayInfo\x12K\n\x16\x62\x61\x63kend_component_info\x18@ \x01(\x0b\x32+.com.wirepas.proto.wnt.BackendComponentInfo\x12\x42\n\x11scratchpad_status\x18\x41 \x01(\x0b\x32\'.com.wirepas.proto.wnt.ScratchpadStatus\x12>\n\x0f\x62\x61\x63kend_message\x18\x46 \x01(\x0b\x32%.com.wirepas.proto.wnt.BackendMessage\x12:\n\ronline_status\x18G \x01(\x0b\x32#.com.wirepas.proto.wnt.OnlineStatus\x12<\n\x0etraveltime_kpi\x18H \x01(\x0b\x32$.com.wirepas.proto.wnt.TraveltimeKPI\x12:\n\rnode_metadata\x18I \x01(\x0b\x32#.com.wirepas.proto.wnt.NodeMetadata\x12H\n\x14rtsituation_metadata\x18J \x01(\x0b\x32*.com.wirepas.proto.wnt.RTSituationMetadata\x12\x42\n\x11\x62\x61\x63kend_heartbeat\x18K \x01(\x0b\x32\'.com.wirepas.proto.wnt.BackendHeartbeat\x12M\n\x17metadata_update_message\x18L \x01(\x0b\x32,.com.wirepas.proto.wnt.MetadataUpdateMessage\x12\x42\n\x12sink_pseudo_id_map\x18M \x03(\x0b\x32&.com.wirepas.proto.wnt.SinkPseudoIdMap\x12O\n\x18\x62\x61\x63kend_component_status\x18N \x01(\x0b\x32-.com.wirepas.proto.wnt.BackendComponentStatus\x12M\n\x12remoteapi_requests\x18P \x01(\x0b\x32\x31.com.wirepas.proto.wnt.RemoteApiRequestCollection\x12\x44\n\x12remoteapi_response\x18Q \x01(\x0b\x32(.com.wirepas.proto.wnt.RemoteApiResponse\x12\x39\n\rnode_messages\x18Z \x03(\x0b\x32\".com.wirepas.proto.wnt.NodeMessage\x12I\n\x15get_scratchpad_status\x18[ \x03(\x0b\x32*.com.wirepas.proto.wnt.GetScratchpadStatus\x12;\n\x0eset_otap_state\x18\x64 \x01(\x0b\x32#.com.wirepas.proto.wnt.SetOTAPState\x12L\n\x17set_otap_state_response\x18\x65 \x01(\x0b\x32+.com.wirepas.proto.wnt.SetOTAPStateResponse\x12I\n\x15set_scratchpad_action\x18\x66 \x01(\x0b\x32*.com.wirepas.proto.wnt.SetScratchpadAction\x12?\n\x15positioning_mesh_data\x18\x82\x01 \x01(\x0b\x32\x1f.com.wirepas.proto.wpe.MeshData\x12?\n\x17positioning_status_data\x18\x83\x01 \x01(\x0b\x32\x1d.com.wirepas.proto.wpe.Status\x12\x63\n\"calculated_values_from_diagnostics\x18\xa0\x01 \x01(\x0b\x32\x36.com.wirepas.proto.wnt.CalculatedValuesFromDiagnostics\"O\n\x11MessageCollection\x12:\n\x12message_collection\x18\x01 \x03(\x0b\x32\x1e.com.wirepas.proto.wnt.Message*\xee\x02\n\x0cStackProfile\x12\x0e\n\nPROFILE_24\x10\x01\x12\x0f\n\x0bPROFILE_868\x10\x02\x12\x0f\n\x0bPROFILE_915\x10\x03\x12\x0f\n\x0bPROFILE_870\x10\x04\x12\x0f\n\x0bPROFILE_917\x10\x05\x12\x16\n\x12PROFILE_RESERVED_1\x10\x06\x12\x16\n\x12PROFILE_RESERVED_2\x10\x07\x12\x0f\n\x0bPROFILE_865\x10\x08\x12\x14\n\x10PROFILE_EFR32_24\x10\t\x12\x16\n\x12PROFILE_RESERVED_3\x10\n\x12\x1f\n\x1bPROFILE_EFR32_915_AUSTRALIA\x10\x0b\x12\x13\n\x0fPROFILE_DECT_NR\x10\x0c\x12\x19\n\x15PROFILE_NRF52_24_4DBM\x10\r\x12\x19\n\x15PROFILE_NRF52_24_8DBM\x10\x0e\x12\x19\n\x15PROFILE_BLE_EFR32_DMP\x10\x0f\x12\x14\n\x0fPROFILE_UNKNOWN\x10\xff\x01*\x82\x01\n\x0eScratchpadType\x12\x19\n\x15SCRATCHPAD_TYPE_BLANK\x10\x00\x12\x1b\n\x17SCRATCHPAD_TYPE_PRESENT\x10\x01\x12\x1b\n\x17SCRATCHPAD_TYPE_PROCESS\x10\x02\x12\x1b\n\x17SCRATCHPAD_TYPE_UNKNOWN\x10\x03*\xbb\x03\n\x15ScratchpadWriteStatus\x12\x1e\n\x1aSCRATCHPAD_WRITE_STATUS_OK\x10\x00\x12(\n$SCRATCHPAD_WRITE_STATUS_COMPLETED_OK\x10\x01\x12+\n\'SCRATCHPAD_WRITE_STATUS_COMPLETED_ERROR\x10\x02\x12\'\n#SCRATCHPAD_WRITE_STATUS_NOT_ONGOING\x10\x03\x12)\n%SCRATCHPAD_WRITE_STATUS_INVALID_START\x10\x04\x12-\n)SCRATCHPAD_WRITE_STATUS_INVALID_NUM_BYTES\x10\x05\x12*\n&SCRATCHPAD_WRITE_STATUS_INVALID_HEADER\x10\x06\x12.\n*SCRATCHPAD_WRITE_STATUS_INVALID_NULL_BYTES\x10\x07\x12\'\n#SCRATCHPAD_WRITE_STATUS_FLASH_ERROR\x10\x08\x12#\n\x1fSCRATCHPAD_WRITE_STATUS_UNKNOWN\x10\t'
+  serialized_pb=b'\n\rmessage.proto\x12\x15\x63om.wirepas.proto.wnt\x1a\x0cnanopb.proto\x1a\notap.proto\x1a\rcommons.proto\x1a\x0einternal.proto\x1a\x10remote_api.proto\x1a\x11positioning.proto\"\xb7\x03\n\x08Neighbor\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\r\x12\x1b\n\x13\x63luster_channel_MHz\x18\x02 \x01(\x02\x12\x16\n\x0eradio_power_dB\x18\x03 \x01(\x02\x12\x43\n\rneighbor_type\x18\x04 \x01(\x0e\x32,.com.wirepas.proto.wnt.Neighbor.NeighborType\x12\x10\n\x08rssi_dBm\x18\x05 \x01(\x02\x12\x14\n\x0cno_neighbors\x18\x06 \x01(\x08\x12\x17\n\x0f\x63luster_channel\x18\x07 \x01(\r\x12\x33\n+amount_of_cluster_beacon_reception_attempts\x18\x08 \x01(\r\x12:\n2amount_of_failed_cluster_beacon_reception_attempts\x18\t \x01(\r\"n\n\x0cNeighborType\x12\n\n\x06MEMBER\x10\x01\x12\x10\n\x0cSYNC_CLUSTER\x10\x02\x12\x16\n\x12\x41SSOCIATED_CLUSTER\x10\x03\x12\x0c\n\x08UNSYNCED\x10\x04\x12\x1a\n\x15NEIGHBOR_TYPE_UNKNOWN\x10\xff\x01\"C\n\x08\x43ostInfo\x12\x18\n\x10next_hop_address\x18\x02 \x01(\r\x12\x0c\n\x04\x63ost\x18\x03 \x01(\r\x12\x0f\n\x07quality\x18\x04 \x01(\x02\"R\n\x1f\x43\x61lculatedValuesFromDiagnostics\x12/\n\'low_energy_transmission_load_percentage\x18\x01 \x01(\x02\"\xec\x30\n\x0f\x44iagnosticsData\x12\x39\n\tneighbors\x18\x01 \x03(\x0b\x32\x1f.com.wirepas.proto.wnt.NeighborB\x05\x92?\x02\x10 \x12\x17\n\x0f\x61\x63\x63\x65ss_cycle_ms\x18\x02 \x01(\x02\x12-\n\x04role\x18\x03 \x01(\x0e\x32\x1f.com.wirepas.proto.wnt.BaseRole\x12\x0e\n\x06\x63\x62_mac\x18\x04 \x01(\x08\x12\x13\n\x0bis_autorole\x18\x06 \x01(\x08\x12\x0f\n\x07voltage\x18\x07 \x01(\x02\x12\x18\n\x10max_buffer_usage\x18\x08 \x01(\x02\x12\x1c\n\x14\x61verage_buffer_usage\x18\t \x01(\x02\x12\x17\n\x0fmem_alloc_fails\x18\n \x01(\r\x12\r\n\x05scans\x18\x0c \x01(\r\x12\x18\n\x07\x64ropped\x18\x11 \x03(\rB\x07\x10\x01\x92?\x02\x10\x02\x12\x14\n\x0csink_address\x18\x31 \x01(\r\x12\x34\n\x04\x63ost\x18\x12 \x03(\x0b\x32\x1f.com.wirepas.proto.wnt.CostInfoB\x05\x92?\x02\x10\x02\x12\x46\n\x06\x65vents\x18\x13 \x03(\x0e\x32-.com.wirepas.proto.wnt.DiagnosticsData.EventsB\x07\x10\x01\x92?\x02\x10\x0f\x12\x12\n\nduty_cycle\x18\x14 \x01(\x02\x12\x0f\n\x07\x61ntenna\x18\x15 \x01(\r\x12\x1b\n\x13\x63luster_channel_MHz\x18\x17 \x01(\x02\x12\x1b\n\x13\x63hannel_reliability\x18\x18 \x01(\x02\x12\x16\n\x0e\x61loha_rx_ratio\x18\x1b \x01(\x02\x12\x1f\n\x17max_reserved_slot_usage\x18! \x01(\x02\x12\x1f\n\x17\x61vg_reserved_slot_usage\x18\x30 \x01(\x02\x12\x1c\n\x14max_aloha_slot_usage\x18\" \x01(\x02\x12\x12\n\nboot_count\x18# \x01(\r\x12\x18\n\x10sw_version_devel\x18$ \x01(\r\x12\x1e\n\x16sw_version_maintenance\x18% \x01(\r\x12\x18\n\x10sw_version_minor\x18& \x01(\r\x12\x18\n\x10sw_version_major\x18\' \x01(\r\x12\x1b\n\x13scratchpad_sequence\x18( \x01(\r\x12@\n\x08hw_magic\x18) \x01(\x0e\x32..com.wirepas.proto.wnt.DiagnosticsData.HWMagic\x12:\n\rstack_profile\x18* \x01(\x0e\x32#.com.wirepas.proto.wnt.StackProfile\x12\x14\n\x0cotap_enabled\x18+ \x01(\x08\x12\x18\n\x10\x62oot_line_number\x18, \x01(\r\x12\x11\n\tfile_hash\x18- \x01(\r\x12\x1c\n\x0bstack_trace\x18. \x03(\rB\x07\x10\x01\x92?\x02\x10\x03\x12\x1f\n\x17routers_in_neighborhood\x18\x32 \x01(\r\x12\x13\n\x0b\x63\x62_mac_load\x18\x33 \x01(\x02\x12\x1d\n\x15\x63luster_member_amount\x18\x34 \x01(\r\x12\"\n\x1a\x63luster_router_node_amount\x18\x35 \x01(\r\x12&\n\x1e\x62lacklisted_radio_channels_1_8\x18\x36 \x01(\r\x12\'\n\x1f\x62lacklisted_radio_channels_9_16\x18\x37 \x01(\r\x12(\n blacklisted_radio_channels_17_24\x18\x38 \x01(\r\x12(\n blacklisted_radio_channels_25_32\x18\x39 \x01(\r\x12(\n blacklisted_radio_channels_33_40\x18: \x01(\r\x12$\n\x1cscratchpad_firmware_sequence\x18; \x01(\r\x12$\n\x1c\x62roadcast_ll_members_pending\x18< \x01(\r\x12$\n\x1c\x62roadcast_le_members_pending\x18= \x01(\r\x12\"\n\x1a\x62roadcast_next_hop_pending\x18> \x01(\r\x12\x1f\n\x17\x62roadcast_unack_pending\x18? \x01(\r\x12\x1f\n\x17packets_expired_pending\x18@ \x01(\r\x12\x1f\n\x17packets_reroute_pending\x18\x41 \x01(\r\x12\x1f\n\x17unicast_cluster_pending\x18\x42 \x01(\r\x12\x1f\n\x17unicast_members_pending\x18\x43 \x01(\r\x12 \n\x18\x64ropped_packets_combined\x18\x44 \x01(\r\x12\x1d\n\x15\x63\x62mac_rx_messages_ack\x18\x45 \x01(\r\x12\x1f\n\x17\x63\x62mac_rx_messages_unack\x18\x46 \x01(\r\x12\"\n\x1a\x63\x62mac_rx_ack_other_reasons\x18G \x01(\r\x12\x1d\n\x15\x63\x62mac_tx_ack_cca_fail\x18H \x01(\r\x12!\n\x19\x63\x62mac_tx_ack_not_received\x18I \x01(\r\x12\x1d\n\x15\x63\x62mac_tx_messages_ack\x18J \x01(\r\x12\x1f\n\x17\x63\x62mac_tx_messages_unack\x18K \x01(\r\x12\x1f\n\x17\x63\x62mac_tx_cca_unack_fail\x18L \x01(\r\x12\x1a\n\x12\x63\x66mac_messages_ack\x18M \x01(\r\x12)\n!cfmac_pending_broadcast_le_member\x18N \x01(\r\x12\x1f\n\x17next_hop_radio_power_dB\x18O \x01(\x05\x12\x19\n\x11next_hop_rssi_dBm\x18P \x01(\x05\x12(\n blacklisted_radio_channels_count\x18Q \x01(\r\x12!\n\x19\x61pplication_version_major\x18R \x01(\r\x12!\n\x19\x61pplication_version_minor\x18S \x01(\r\x12\'\n\x1f\x61pplication_version_maintenance\x18T \x01(\r\x12!\n\x19\x61pplication_version_devel\x18U \x01(\r\x12\x44\n\ntrace_type\x18V \x01(\x0e\x32\x30.com.wirepas.proto.wnt.DiagnosticsData.TraceType\x12\x1e\n\x16packet_sequence_number\x18W \x01(\r\x12\x17\n\x0f\x63luster_channel\x18X \x01(\r\x12\x14\n\x0csleep_time_s\x18Y \x01(\r\x12\x46\n\x0b\x62oot_reason\x18Z \x01(\x0e\x32\x31.com.wirepas.proto.wnt.DiagnosticsData.BootReason\x12\x0f\n\x07rx_gain\x18[ \x01(\x05\x12\x1a\n\ttx_powers\x18\\ \x03(\x05\x42\x07\x10\x01\x92?\x02\x10\x10\x12\x1c\n\x14scratchpad_transfers\x18] \x01(\r\x12\x1c\n\x14installation_quality\x18^ \x01(\x02\x12m\n\x1binstallation_quality_errors\x18_ \x03(\x0e\x32?.com.wirepas.proto.wnt.DiagnosticsData.InstallationQualityErrorB\x07\x10\x01\x92?\x02\x10\x03\x12\'\n\x1f\x64ropped_unack_broadcast_packets\x18` \x01(\r\x12<\n4unacknowledged_broadcast_transmissions_channel_count\x18\x61 \x01(\r\x12+\n#wide_band_noise_rssi_correction_dBm\x18\x62 \x01(\x05\x12\x31\n)network_channel_packet_error_rate_percent\x18\x63 \x01(\x02\x12)\n!boot_diagnostics_tx_time_ms_epoch\x18\x64 \x01(\x04\x12\x15\n\rcca_limit_dBm\x18\x65 \x01(\x05\x12\x17\n\x0f\x61\x64\x64ress_clashes\x18\x66 \x01(\r\x12\x17\n\x0fll_device_count\x18g \x01(\r\x12\x1a\n\x12is_ble_scan_active\x18h \x01(\x08\x12$\n\x1c\x63ost_compensation_throughput\x18i \x01(\r\x12\"\n\x1a\x63ost_compensation_bad_link\x18j \x01(\r\x12%\n\x1d\x63ost_compensation_bad_channel\x18k \x01(\r\x12.\n&cost_compensation_price_of_association\x18l \x01(\r\x12+\n#cost_compensation_high_buffer_usage\x18m \x01(\r\x12\x31\n)cost_compensation_high_energy_consumption\x18n \x01(\r\x12 \n\x18is_joining_beacon_active\x18o \x01(\x08\x12#\n\x1b\x61mount_of_flooding_messages\x18p \x01(\r\x12-\n%amount_of_dropped_reassembled_packets\x18q \x01(\r\x12\x1b\n\x13modem_version_devel\x18r \x01(\r\x12!\n\x19modem_version_maintenance\x18s \x01(\r\x12\x1b\n\x13modem_version_minor\x18t \x01(\r\x12\x1b\n\x13modem_version_major\x18u \x01(\r\"\xe0\x0e\n\x06\x45vents\x12\x12\n\x0eROLE_NO_EVENTS\x10\x00\x12\x1c\n\x18SCAN_REASON_INITIAL_SCAN\x10\x01\x12\"\n\x1eSCAN_REASON_RESTRICTED_CHANNEL\x10\x02\x12\x1e\n\x1aSCAN_REASON_MAJOR_BOUNDARY\x10\x03\x12\x1a\n\x16SCAN_REASON_NO_CHANNEL\x10\x04\x12\x19\n\x15SCAN_REASON_BLACKLIST\x10\x05\x12\x1a\n\x16ROLE_CHANGE_TO_SUBNODE\x10\x08\x12\x1b\n\x17ROLE_CHANGE_TO_HEADNODE\x10\t\x12\x10\n\x0cROUTE_CHANGE\x10\x10\x12\x1d\n\x19SCAN_REASON_NEXT_HOP_LOST\x10\x14\x12\x1f\n\x1bSCAN_REASON_BOUNDARY_CHANGE\x10\x15\x12\x18\n\x14SCAN_REASON_HIGH_PER\x10\x16\x12\x1f\n\x1bSCANNING_REQ_BY_APPLICATION\x10\x17\x12 \n\x1cSCANNING_NO_CHANNEL_SELECTED\x10\x18\x12%\n!SCANNING_FTDMA_CONF_WITH_NEIGHBOR\x10\x19\x12(\n$SCANNING_FTDMA_CONF_WITH_NB_NEIGHBOR\x10\x1a\x12&\n\"SCANNING_TIMING_CONF_WITH_NEIGHBOR\x10\x1b\x12\x30\n,SCANNING_TIMING_CONF_WITH_MULTIPLE_NEIGHBORS\x10\x1c\x12 \n\x1cSCANNING_NEED_MORE_NEIGHBORS\x10\x1d\x12\x15\n\x11SCANNING_PERIODIC\x10\x1e\x12\x18\n\x14SCANNING_ROLE_CHANGE\x10\x1f\x12\x10\n\x0c\x42OOT_POWERON\x10 \x12\x14\n\x10\x42OOT_INTENTIONAL\x10!\x12\x13\n\x0f\x42OOT_SW_FAILURE\x10\"\x12\x1a\n\x16\x42OOT_PROCESSOR_FAILURE\x10#\x12\x18\n\x14\x42OOT_WATCHDOG_EXPIRE\x10$\x12\x1d\n\x19\x42OOT_UNINDENTIFIED_REASON\x10%\x12\x1e\n\x1aSYNCLOST_ALTERNATIVE_ROUTE\x10(\x12\x1a\n\x16SYNCLOST_PRIMARY_ROUTE\x10)\x12\x1c\n\x18\x46TDMA_ADJ_MINOR_BOUNDARY\x10\x30\x12\"\n\x1e\x46TDMA_ADJ_NOT_IN_SLOT_BOUNDARY\x10\x31\x12)\n%FTDMA_ADJ_CONFLICT_WITH_PRIMARY_ROUTE\x10\x32\x12-\n)FTDMA_ADJ_CONFLICT_WITH_ALTERNATIVE_ROUTE\x10\x33\x12$\n FTDMA_ADJ_CONFLICT_WITH_NEIGHBOR\x10\x34\x12!\n\x1d\x46TDMA_ADJ_NO_CHANNEL_SELECTED\x10\x35\x12!\n\x1d\x46TDMA_ADJ_CHANNEL_BLACKLISTED\x10\x36\x12\x1a\n\x16\x46TDMA_ADJ_OTHER_REASON\x10\x37\x12\x10\n\x0cSINK_CHANGED\x10\x38\x12\x0f\n\x0b\x46HMA_ADJUST\x10\x39\x12\x16\n\x12TDMA_ADJUST_CCSTAT\x10:\x12\x10\n\x0cROUTING_LOOP\x10@\x12\x18\n\x14\x44\x45NSE_REMOVE_SUBNODE\x10H\x12#\n\x1f\x44OWNLINK_TX_FAIL_COULD_NOT_SEND\x10I\x12,\n(DOWNLINK_TX_FAIL_NEXT_HOP_COULD_NOT_SEND\x10J\x12!\n\x1dUPLINK_TX_FAIL_COULD_NOT_SEND\x10K\x12 \n\x1cTOO_MANY_ROUTERS_DURING_SCAN\x10L\x12,\n(TIMING_LATE_FOR_SCHEDULING_MAC_OPERATION\x10M\x12\x1a\n\x16SCAN_REASON_ADVERTISER\x10N\x12\x13\n\x0fSCAN_REASON_APC\x10O\x12\x17\n\x13SHORT_ADDRESS_RESET\x10P\x12\x13\n\x0eRESET_NEW_BASE\x10\xc8\x01\x12\x10\n\x0bRESET_MODEM\x10\xce\x01\x12\x15\n\x10RESET_MODEM_INIT\x10\xcf\x01\x12\x13\n\x0eRESET_SOFT_WDT\x10\xd0\x01\x12\x0e\n\tRESET_NMI\x10\xd1\x01\x12\x15\n\x10RESET_HARD_FAULT\x10\xd2\x01\x12\x14\n\x0fRESET_BUS_FAULT\x10\xd3\x01\x12\x16\n\x11RESET_USAGE_FAULT\x10\xd4\x01\x12\x1b\n\x16RESET_MEM_MANAGE_FAULT\x10\xd5\x01\x12\x0e\n\tRESET_PIN\x10\xd6\x01\x12\x15\n\x10RESET_CPU_LOCKUP\x10\xd7\x01\x12\x1c\n\x17RESET_SYSTEM_OFF_WAKEUP\x10\xd8\x01\x12\x13\n\x0eRESET_BROWNOUT\x10\xd9\x01\x12\x13\n\x0eRESET_SECURITY\x10\xda\x01\x12\x12\n\rRESET_REQUEST\x10\xdb\x01\x12\x12\n\rEVENT_UNKNOWN\x10\xff\x01\"\xcf\x02\n\x07HWMagic\x12\t\n\x05NRF51\x10\x01\x12\t\n\x05\x45ZR32\x10\x02\x12\t\n\x05NRF52\x10\x03\x12\n\n\x06\x43\x43\x32\x36\x35\x30\x10\x04\x12\x1a\n\x16\x45\x46R32XG12_1024KB_128KB\x10\x05\x12\x19\n\x15NRF52840_1024KB_256KB\x10\x06\x12\x18\n\x14\x45\x46R32XG12_512KB_64KB\x10\x07\x12\x13\n\x0f\x45\x46R32XG13_512KB\x10\x08\x12\x0c\n\x08NRF52833\x10\t\x12\r\n\tEFR32XG21\x10\n\x12\r\n\tEFR32XG22\x10\x0b\x12\x11\n\rBGM210PA22JIA\x10\x0c\x12\x11\n\rBGM220PC22HNA\x10\r\x12\x11\n\rBGM220SC22HNA\x10\x0e\x12\x0b\n\x07NRF9160\x10\x0f\x12\r\n\tEFR32XG23\x10\x10\x12\r\n\tEFR32XG24\x10\x11\x12\x0b\n\x07NRF9120\x10\x12\x12\x14\n\x0fHWMAGIC_UNKNOWN\x10\xff\x01\"\x87\x01\n\tTraceType\x12\x14\n\x10NODE_DIAGNOSTICS\x10\x01\x12\x18\n\x14NEIGHBOR_DIAGNOSTICS\x10\x02\x12\x14\n\x10SCAN_DIAGNOSTICS\x10\x03\x12\x14\n\x10\x42OOT_DIAGNOSTICS\x10\x04\x12\x1e\n\x1a\x42OOT_DIAGNOSTICS_WM_FW_5_0\x10\x07\"\xbb\x01\n\nBootReason\x12!\n\x1dNORMAL_POWER_ON_RESET_STARTUP\x10\x00\x12\x30\n,REBOOT_REQUESTED_AS_PART_OF_NORMAL_OPERATION\x10\x01\x12\x1b\n\x17SOFTWARE_ASSERT_FAILURE\x10\x02\x12\r\n\tMCU_FAULT\x10\x03\x12\x12\n\x0eWATCHDOG_RESET\x10\x04\x12\x18\n\x14UNKNOWN_RESET_REASON\x10\x05\"X\n\x18InstallationQualityError\x12\x14\n\x10NO_ROUTE_TO_SINK\x10\x00\x12\x18\n\x14NOT_ENOUGH_NEIGHBORS\x10\x01\x12\x0c\n\x08\x42\x41\x44_RSSI\x10\x02\"\xa6\x02\n\x06RxData\x12\x17\n\x0fsource_endpoint\x18\x02 \x01(\r\x12\x1c\n\x14\x64\x65stination_endpoint\x18\x04 \x01(\r\x12\x0e\n\x03qos\x18\x05 \x01(\r:\x01\x30\x12\x0f\n\x07payload\x18\x07 \x01(\x0c\x12\x14\n\x0cpayload_size\x18\x08 \x01(\r\x12\x14\n\x0csink_address\x18\t \x01(\r\x12\x11\n\thop_count\x18\n \x01(\r\x12 \n\x18gateway_rx_time_ms_epoch\x18\x0b \x01(\x04\x12 \n\x18\x62\x61\x63kend_rx_time_ms_epoch\x18\x0c \x01(\x04\x12(\n gateway_backend_rx_time_delta_ms\x18\r \x01(\x05\x12\x17\n\x0fis_dect_network\x18\x0e \x01(\x08\"\xc8\x06\n\x11\x41ppConfigResponse\x12H\n\x06result\x18\x01 \x01(\x0e\x32\x38.com.wirepas.proto.wnt.AppConfigResponse.AppConfigResult\"\xe8\x05\n\x0f\x41ppConfigResult\x12\x1f\n\x12UNKNOWN_ERROR_CODE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x06\n\x02OK\x10\x00\x12\x12\n\x0eINTERNAL_ERROR\x10\x01\x12\x13\n\x0fINVALID_SINK_ID\x10\x02\x12\x10\n\x0cINVALID_ROLE\x10\x03\x12\x1b\n\x17INVALID_NETWORK_ADDRESS\x10\x04\x12\x1b\n\x17INVALID_NETWORK_CHANNEL\x10\x05\x12\x17\n\x13INVALID_CHANNEL_MAP\x10\x06\x12\x18\n\x14INVALID_NETWORK_KEYS\x10\x07\x12\x14\n\x10INVALID_AC_RANGE\x10\x08\x12\x16\n\x12INVALID_SINK_STATE\x10\t\x12\x18\n\x14INVALID_DEST_ADDRESS\x10\n\x12\x19\n\x15INVALID_DEST_ENDPOINT\x10\x0b\x12\x18\n\x14INVALID_SRC_ENDPOINT\x10\x0c\x12\x0f\n\x0bINVALID_QOS\x10\r\x12\x18\n\x14INVALID_DATA_PAYLOAD\x10\x0e\x12\x16\n\x12INVALID_SCRATCHPAD\x10\x0f\x12\x1b\n\x17INVALID_SCRATCHPAD_SIZE\x10\x10\x12\x1b\n\x17INVALID_SEQUENCE_NUMBER\x10\x11\x12\x18\n\x14INVALID_REBOOT_DELAY\x10\x12\x12\x19\n\x15INVALID_DIAG_INTERVAL\x10\x13\x12\x16\n\x12INVALID_APP_CONFIG\x10\x14\x12\x11\n\rINVALID_PARAM\x10\x15\x12\x19\n\x15NO_SCRATCHPAD_PRESENT\x10\x16\x12\x11\n\rACCESS_DENIED\x10\x17\x12\x19\n\x15REQUEST_NEEDS_SINK_ID\x10\x18\x12\x19\n\x15INVALID_MAX_HOP_COUNT\x10\x19\x12\x16\n\x12SINK_OUT_OF_MEMORY\x10\x1a\x12\x10\n\x0cSINK_TIMEOUT\x10\x1b\x12\x1c\n\x18\x46IRST_INVALID_ENUM_VALUE\x10\x1c\"V\n\x0bMeasurement\x12\x11\n\tsensor_id\x18\x01 \x01(\r\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04unit\x18\x04 \x01(\t\x12\x17\n\x0fno_measurements\x18\x05 \x01(\x08\"9\n\x10GatewayHeartbeat\x12\x13\n\x0bmac_address\x18\x01 \x01(\t\x12\x10\n\x08hostname\x18\x03 \x01(\t\"`\n\x0bGatewayInfo\x12\x1c\n\x14\x63urrent_time_s_epoch\x18\x01 \x01(\r\x12\r\n\x05model\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x13\n\x0b\x61pi_version\x18\x04 \x01(\r\"p\n\x14\x42\x61\x63kendComponentInfo\x12\x1c\n\x14\x63urrent_time_s_epoch\x18\x01 \x01(\r\x12:\n\tcomponent\x18\x02 \x01(\x0e\x32\'.com.wirepas.proto.wnt.BackendComponent\"2\n\x12\x43hannelIdToFreqMap\x12\n\n\x02id\x18\x01 \x01(\r\x12\x10\n\x08\x66req_MHz\x18\x02 \x01(\x02\"3\n\x11\x41\x63\x63\x65ssCycleLimits\x12\x0e\n\x06min_ms\x18\x01 \x01(\r\x12\x0e\n\x06max_ms\x18\x02 \x01(\r\"\x95\x01\n\x0bNodeMessage\x12\x1b\n\x13\x64\x65stination_address\x18\x01 \x01(\r\x12\x12\n\nnetwork_id\x18\x02 \x01(\r\x12\x18\n\x10source_end_point\x18\x03 \x01(\r\x12\x1d\n\x15\x64\x65stination_end_point\x18\x04 \x01(\r\x12\x0b\n\x03qos\x18\x05 \x01(\r\x12\x0f\n\x07payload\x18\x06 \x01(\x0c\"\xde\x01\n\x13GetScratchpadStatus\x12\x12\n\nnetwork_id\x18\x01 \x01(\r\x12\x19\n\x11resend_interval_s\x18\x02 \x01(\r\x12\x10\n\x08is_close\x18\x03 \x01(\x08\x12\x14\n\x0cis_sink_only\x18\x04 \x01(\x08\x12G\n\x14message_sending_type\x18\x05 \x01(\x0e\x32).com.wirepas.proto.wnt.MessageSendingType\x12\'\n\x1fmessage_distribution_interval_s\x18\x06 \x01(\r\"\x8f\t\n\x10ScratchpadStatus\x12\x1e\n\x16is_continuous_query_on\x18\x01 \x01(\x08\x12\x18\n\x10tx_time_ms_epoch\x18\x02 \x01(\x04\x12\x1e\n\x16stored_scratchpad_size\x18\n \x01(\r\x12\x1d\n\x15stored_scratchpad_crc\x18\x0b \x01(\r\x12\"\n\x1astored_scratchpad_sequence\x18\x0c \x01(\r\x12\x45\n\x16stored_scratchpad_type\x18\r \x01(\x0e\x32%.com.wirepas.proto.wnt.ScratchpadType\x12N\n\x18stored_scratchpad_status\x18\x0e \x01(\x0e\x32,.com.wirepas.proto.wnt.ScratchpadWriteStatus\x12$\n\x1cprocessed_fw_scratchpad_size\x18\x14 \x01(\r\x12#\n\x1bprocessed_fw_scratchpad_crc\x18\x15 \x01(\r\x12(\n processed_fw_scratchpad_sequence\x18\x16 \x01(\r\x12\x1c\n\x14processed_fw_area_id\x18\x17 \x01(\r\x12\"\n\x1aprocessed_fw_version_major\x18\x18 \x01(\r\x12\"\n\x1aprocessed_fw_version_minor\x18\x19 \x01(\r\x12(\n processed_fw_version_maintenance\x18\x1a \x01(\r\x12\"\n\x1aprocessed_fw_version_devel\x18\x1b \x01(\r\x12-\n%processed_application_scratchpad_size\x18( \x01(\r\x12,\n$processed_application_scratchpad_crc\x18) \x01(\r\x12\x31\n)processed_application_scratchpad_sequence\x18* \x01(\r\x12%\n\x1dprocessed_application_area_id\x18+ \x01(\r\x12+\n#processed_application_version_major\x18, \x01(\r\x12+\n#processed_application_version_minor\x18- \x01(\r\x12\x31\n)processed_application_version_maintenance\x18. \x01(\r\x12+\n#processed_application_version_devel\x18/ \x01(\r\x12\x42\n\x11scratchpad_action\x18< \x01(\x0e\x32\'.com.wirepas.proto.wnt.ScratchpadAction\x12\x17\n\x0ftarget_sequence\x18= \x01(\r\x12\x12\n\ntarget_crc\x18> \x01(\r\x12\x1c\n\x14target_delay_minutes\x18? \x01(\r\x12\x1e\n\x16remaining_time_minutes\x18@ \x01(\r\"m\n\x13SetScratchpadAction\x12\x12\n\nnetwork_id\x18\x01 \x01(\r\x12\x42\n\x11scratchpad_action\x18\x02 \x01(\x0e\x32\'.com.wirepas.proto.wnt.ScratchpadAction\"\xc8\x12\n\x07Message\x12\x0e\n\x02id\x18\x01 \x03(\rB\x02\x10\x01\x12\x12\n\nnetwork_id\x18\x02 \x01(\r\x12\x12\n\ngateway_id\x18\x03 \x01(\t\x12\x0f\n\x07tx_time\x18\x04 \x01(\x04\x12\x0f\n\x07rx_time\x18\x05 \x01(\x04\x12\x16\n\x0esource_address\x18\x07 \x01(\r\x12\x1b\n\x13\x64\x65stination_address\x18\x08 \x01(\r\x12\x16\n\x0etravel_time_ms\x18\t \x01(\x02\x12;\n\x0b\x64iagnostics\x18\x32 \x01(\x0b\x32&.com.wirepas.proto.wnt.DiagnosticsData\x12.\n\x07rx_data\x18\x33 \x01(\x0b\x32\x1d.com.wirepas.proto.wnt.RxData\x12\x38\n\napp_config\x18\x34 \x01(\x0b\x32$.com.wirepas.proto.wnt.AppConfigData\x12:\n\rstack_profile\x18\x35 \x01(\x0e\x32#.com.wirepas.proto.wnt.StackProfile\x12\x37\n\x0bmeasurement\x18\x36 \x03(\x0b\x32\".com.wirepas.proto.wnt.Measurement\x12=\n\x0cgw_heartbeat\x18\x37 \x01(\x0b\x32\'.com.wirepas.proto.wnt.GatewayHeartbeat\x12.\n\x07tx_data\x18\x38 \x01(\x0b\x32\x1d.com.wirepas.proto.wnt.RxData\x12\x17\n\x0fnetwork_channel\x18: \x01(\r\x12\x18\n\x10security_enabled\x18; \x01(\x08\x12?\n\x0c\x63hannel_info\x18< \x03(\x0b\x32).com.wirepas.proto.wnt.ChannelIdToFreqMap\x12\x45\n\x13\x61pp_config_response\x18= \x01(\x0b\x32(.com.wirepas.proto.wnt.AppConfigResponse\x12\x45\n\x13\x61\x63\x63\x65ss_cycle_limits\x18> \x01(\x0b\x32(.com.wirepas.proto.wnt.AccessCycleLimits\x12\x38\n\x0cgateway_info\x18? \x01(\x0b\x32\".com.wirepas.proto.wnt.GatewayInfo\x12K\n\x16\x62\x61\x63kend_component_info\x18@ \x01(\x0b\x32+.com.wirepas.proto.wnt.BackendComponentInfo\x12\x42\n\x11scratchpad_status\x18\x41 \x01(\x0b\x32\'.com.wirepas.proto.wnt.ScratchpadStatus\x12>\n\x0f\x62\x61\x63kend_message\x18\x46 \x01(\x0b\x32%.com.wirepas.proto.wnt.BackendMessage\x12:\n\ronline_status\x18G \x01(\x0b\x32#.com.wirepas.proto.wnt.OnlineStatus\x12<\n\x0etraveltime_kpi\x18H \x01(\x0b\x32$.com.wirepas.proto.wnt.TraveltimeKPI\x12:\n\rnode_metadata\x18I \x01(\x0b\x32#.com.wirepas.proto.wnt.NodeMetadata\x12H\n\x14rtsituation_metadata\x18J \x01(\x0b\x32*.com.wirepas.proto.wnt.RTSituationMetadata\x12\x42\n\x11\x62\x61\x63kend_heartbeat\x18K \x01(\x0b\x32\'.com.wirepas.proto.wnt.BackendHeartbeat\x12M\n\x17metadata_update_message\x18L \x01(\x0b\x32,.com.wirepas.proto.wnt.MetadataUpdateMessage\x12\x42\n\x12sink_pseudo_id_map\x18M \x03(\x0b\x32&.com.wirepas.proto.wnt.SinkPseudoIdMap\x12O\n\x18\x62\x61\x63kend_component_status\x18N \x01(\x0b\x32-.com.wirepas.proto.wnt.BackendComponentStatus\x12M\n\x12remoteapi_requests\x18P \x01(\x0b\x32\x31.com.wirepas.proto.wnt.RemoteApiRequestCollection\x12\x44\n\x12remoteapi_response\x18Q \x01(\x0b\x32(.com.wirepas.proto.wnt.RemoteApiResponse\x12\x39\n\rnode_messages\x18Z \x03(\x0b\x32\".com.wirepas.proto.wnt.NodeMessage\x12I\n\x15get_scratchpad_status\x18[ \x03(\x0b\x32*.com.wirepas.proto.wnt.GetScratchpadStatus\x12;\n\x0eset_otap_state\x18\x64 \x01(\x0b\x32#.com.wirepas.proto.wnt.SetOTAPState\x12L\n\x17set_otap_state_response\x18\x65 \x01(\x0b\x32+.com.wirepas.proto.wnt.SetOTAPStateResponse\x12I\n\x15set_scratchpad_action\x18\x66 \x01(\x0b\x32*.com.wirepas.proto.wnt.SetScratchpadAction\x12?\n\x15positioning_mesh_data\x18\x82\x01 \x01(\x0b\x32\x1f.com.wirepas.proto.wpe.MeshData\x12?\n\x17positioning_status_data\x18\x83\x01 \x01(\x0b\x32\x1d.com.wirepas.proto.wpe.Status\x12\x63\n\"calculated_values_from_diagnostics\x18\xa0\x01 \x01(\x0b\x32\x36.com.wirepas.proto.wnt.CalculatedValuesFromDiagnostics\"O\n\x11MessageCollection\x12:\n\x12message_collection\x18\x01 \x03(\x0b\x32\x1e.com.wirepas.proto.wnt.Message*\x82\x01\n\x0eScratchpadType\x12\x19\n\x15SCRATCHPAD_TYPE_BLANK\x10\x00\x12\x1b\n\x17SCRATCHPAD_TYPE_PRESENT\x10\x01\x12\x1b\n\x17SCRATCHPAD_TYPE_PROCESS\x10\x02\x12\x1b\n\x17SCRATCHPAD_TYPE_UNKNOWN\x10\x03*\xbb\x03\n\x15ScratchpadWriteStatus\x12\x1e\n\x1aSCRATCHPAD_WRITE_STATUS_OK\x10\x00\x12(\n$SCRATCHPAD_WRITE_STATUS_COMPLETED_OK\x10\x01\x12+\n\'SCRATCHPAD_WRITE_STATUS_COMPLETED_ERROR\x10\x02\x12\'\n#SCRATCHPAD_WRITE_STATUS_NOT_ONGOING\x10\x03\x12)\n%SCRATCHPAD_WRITE_STATUS_INVALID_START\x10\x04\x12-\n)SCRATCHPAD_WRITE_STATUS_INVALID_NUM_BYTES\x10\x05\x12*\n&SCRATCHPAD_WRITE_STATUS_INVALID_HEADER\x10\x06\x12.\n*SCRATCHPAD_WRITE_STATUS_INVALID_NULL_BYTES\x10\x07\x12\'\n#SCRATCHPAD_WRITE_STATUS_FLASH_ERROR\x10\x08\x12#\n\x1fSCRATCHPAD_WRITE_STATUS_UNKNOWN\x10\t'
   ,
   dependencies=[nanopb__pb2.DESCRIPTOR,otap__pb2.DESCRIPTOR,commons__pb2.DESCRIPTOR,internal__pb2.DESCRIPTOR,remote__api__pb2.DESCRIPTOR,positioning__pb2.DESCRIPTOR,])
 
-_STACKPROFILE = _descriptor.EnumDescriptor(
-  name='StackProfile',
-  full_name='com.wirepas.proto.wnt.StackProfile',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_24', index=0, number=1,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_868', index=1, number=2,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_915', index=2, number=3,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_870', index=3, number=4,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_917', index=4, number=5,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_RESERVED_1', index=5, number=6,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_RESERVED_2', index=6, number=7,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_865', index=7, number=8,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_EFR32_24', index=8, number=9,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_RESERVED_3', index=9, number=10,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_EFR32_915_AUSTRALIA', index=10, number=11,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_DECT_NR', index=11, number=12,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_NRF52_24_4DBM', index=12, number=13,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_NRF52_24_8DBM', index=13, number=14,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_BLE_EFR32_DMP', index=14, number=15,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PROFILE_UNKNOWN', index=15, number=255,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=12644,
-  serialized_end=13010,
-)
-_sym_db.RegisterEnumDescriptor(_STACKPROFILE)
-
-StackProfile = enum_type_wrapper.EnumTypeWrapper(_STACKPROFILE)
 _SCRATCHPADTYPE = _descriptor.EnumDescriptor(
   name='ScratchpadType',
   full_name='com.wirepas.proto.wnt.ScratchpadType',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
@@ -152,16 +56,16 @@
       name='SCRATCHPAD_TYPE_UNKNOWN', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=13013,
-  serialized_end=13143,
+  serialized_start=12707,
+  serialized_end=12837,
 )
 _sym_db.RegisterEnumDescriptor(_SCRATCHPADTYPE)
 
 ScratchpadType = enum_type_wrapper.EnumTypeWrapper(_SCRATCHPADTYPE)
 _SCRATCHPADWRITESTATUS = _descriptor.EnumDescriptor(
   name='ScratchpadWriteStatus',
   full_name='com.wirepas.proto.wnt.ScratchpadWriteStatus',
@@ -218,36 +122,20 @@
       name='SCRATCHPAD_WRITE_STATUS_UNKNOWN', index=9, number=9,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=13146,
-  serialized_end=13589,
+  serialized_start=12840,
+  serialized_end=13283,
 )
 _sym_db.RegisterEnumDescriptor(_SCRATCHPADWRITESTATUS)
 
 ScratchpadWriteStatus = enum_type_wrapper.EnumTypeWrapper(_SCRATCHPADWRITESTATUS)
-PROFILE_24 = 1
-PROFILE_868 = 2
-PROFILE_915 = 3
-PROFILE_870 = 4
-PROFILE_917 = 5
-PROFILE_RESERVED_1 = 6
-PROFILE_RESERVED_2 = 7
-PROFILE_865 = 8
-PROFILE_EFR32_24 = 9
-PROFILE_RESERVED_3 = 10
-PROFILE_EFR32_915_AUSTRALIA = 11
-PROFILE_DECT_NR = 12
-PROFILE_NRF52_24_4DBM = 13
-PROFILE_NRF52_24_8DBM = 14
-PROFILE_BLE_EFR32_DMP = 15
-PROFILE_UNKNOWN = 255
 SCRATCHPAD_TYPE_BLANK = 0
 SCRATCHPAD_TYPE_PRESENT = 1
 SCRATCHPAD_TYPE_PROCESS = 2
 SCRATCHPAD_TYPE_UNKNOWN = 3
 SCRATCHPAD_WRITE_STATUS_OK = 0
 SCRATCHPAD_WRITE_STATUS_COMPLETED_OK = 1
 SCRATCHPAD_WRITE_STATUS_COMPLETED_ERROR = 2
@@ -549,98 +437,103 @@
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='SCAN_REASON_APC', index=48, number=79,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_NEW_BASE', index=49, number=200,
+      name='SHORT_ADDRESS_RESET', index=49, number=80,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_MODEM', index=50, number=206,
+      name='RESET_NEW_BASE', index=50, number=200,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_MODEM_INIT', index=51, number=207,
+      name='RESET_MODEM', index=51, number=206,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_SOFT_WDT', index=52, number=208,
+      name='RESET_MODEM_INIT', index=52, number=207,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_NMI', index=53, number=209,
+      name='RESET_SOFT_WDT', index=53, number=208,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_HARD_FAULT', index=54, number=210,
+      name='RESET_NMI', index=54, number=209,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_BUS_FAULT', index=55, number=211,
+      name='RESET_HARD_FAULT', index=55, number=210,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_USAGE_FAULT', index=56, number=212,
+      name='RESET_BUS_FAULT', index=56, number=211,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_MEM_MANAGE_FAULT', index=57, number=213,
+      name='RESET_USAGE_FAULT', index=57, number=212,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_PIN', index=58, number=214,
+      name='RESET_MEM_MANAGE_FAULT', index=58, number=213,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_CPU_LOCKUP', index=59, number=215,
+      name='RESET_PIN', index=59, number=214,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_SYSTEM_OFF_WAKEUP', index=60, number=216,
+      name='RESET_CPU_LOCKUP', index=60, number=215,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_BROWNOUT', index=61, number=217,
+      name='RESET_SYSTEM_OFF_WAKEUP', index=61, number=216,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_SECURITY', index=62, number=218,
+      name='RESET_BROWNOUT', index=62, number=217,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RESET_REQUEST', index=63, number=219,
+      name='RESET_SECURITY', index=63, number=218,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='EVENT_UNKNOWN', index=64, number=255,
+      name='RESET_REQUEST', index=64, number=219,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='EVENT_UNKNOWN', index=65, number=255,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
   serialized_start=4338,
-  serialized_end=6201,
+  serialized_end=6226,
 )
 _sym_db.RegisterEnumDescriptor(_DIAGNOSTICSDATA_EVENTS)
 
 _DIAGNOSTICSDATA_HWMAGIC = _descriptor.EnumDescriptor(
   name='HWMagic',
   full_name='com.wirepas.proto.wnt.DiagnosticsData.HWMagic',
   filename=None,
@@ -729,23 +622,28 @@
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='EFR32XG24', index=16, number=17,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='HWMAGIC_UNKNOWN', index=17, number=255,
+      name='NRF9120', index=17, number=18,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='HWMAGIC_UNKNOWN', index=18, number=255,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=6204,
-  serialized_end=6526,
+  serialized_start=6229,
+  serialized_end=6564,
 )
 _sym_db.RegisterEnumDescriptor(_DIAGNOSTICSDATA_HWMAGIC)
 
 _DIAGNOSTICSDATA_TRACETYPE = _descriptor.EnumDescriptor(
   name='TraceType',
   full_name='com.wirepas.proto.wnt.DiagnosticsData.TraceType',
   filename=None,
@@ -776,16 +674,16 @@
       name='BOOT_DIAGNOSTICS_WM_FW_5_0', index=4, number=7,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=6529,
-  serialized_end=6664,
+  serialized_start=6567,
+  serialized_end=6702,
 )
 _sym_db.RegisterEnumDescriptor(_DIAGNOSTICSDATA_TRACETYPE)
 
 _DIAGNOSTICSDATA_BOOTREASON = _descriptor.EnumDescriptor(
   name='BootReason',
   full_name='com.wirepas.proto.wnt.DiagnosticsData.BootReason',
   filename=None,
@@ -821,16 +719,16 @@
       name='UNKNOWN_RESET_REASON', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=6667,
-  serialized_end=6854,
+  serialized_start=6705,
+  serialized_end=6892,
 )
 _sym_db.RegisterEnumDescriptor(_DIAGNOSTICSDATA_BOOTREASON)
 
 _DIAGNOSTICSDATA_INSTALLATIONQUALITYERROR = _descriptor.EnumDescriptor(
   name='InstallationQualityError',
   full_name='com.wirepas.proto.wnt.DiagnosticsData.InstallationQualityError',
   filename=None,
@@ -851,16 +749,16 @@
       name='BAD_RSSI', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=6856,
-  serialized_end=6944,
+  serialized_start=6894,
+  serialized_end=6982,
 )
 _sym_db.RegisterEnumDescriptor(_DIAGNOSTICSDATA_INSTALLATIONQUALITYERROR)
 
 _APPCONFIGRESPONSE_APPCONFIGRESULT = _descriptor.EnumDescriptor(
   name='AppConfigResult',
   full_name='com.wirepas.proto.wnt.AppConfigResponse.AppConfigResult',
   filename=None,
@@ -1016,16 +914,16 @@
       name='FIRST_INVALID_ENUM_VALUE', index=29, number=28,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=7315,
-  serialized_end=8059,
+  serialized_start=7378,
+  serialized_end=8122,
 )
 _sym_db.RegisterEnumDescriptor(_APPCONFIGRESPONSE_APPCONFIGRESULT)
 
 
 _NEIGHBOR = _descriptor.Descriptor(
   name='Neighbor',
   full_name='com.wirepas.proto.wnt.Neighbor',
@@ -1929,15 +1827,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=730,
-  serialized_end=6944,
+  serialized_end=6982,
 )
 
 
 _RXDATA = _descriptor.Descriptor(
   name='RxData',
   full_name='com.wirepas.proto.wnt.RxData',
   filename=None,
@@ -2011,28 +1909,35 @@
     _descriptor.FieldDescriptor(
       name='gateway_backend_rx_time_delta_ms', full_name='com.wirepas.proto.wnt.RxData.gateway_backend_rx_time_delta_ms', index=9,
       number=13, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='is_dect_network', full_name='com.wirepas.proto.wnt.RxData.is_dect_network', index=10,
+      number=14, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6947,
-  serialized_end=7216,
+  serialized_start=6985,
+  serialized_end=7279,
 )
 
 
 _APPCONFIGRESPONSE = _descriptor.Descriptor(
   name='AppConfigResponse',
   full_name='com.wirepas.proto.wnt.AppConfigResponse',
   filename=None,
@@ -2056,16 +1961,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7219,
-  serialized_end=8059,
+  serialized_start=7282,
+  serialized_end=8122,
 )
 
 
 _MEASUREMENT = _descriptor.Descriptor(
   name='Measurement',
   full_name='com.wirepas.proto.wnt.Measurement',
   filename=None,
@@ -2109,16 +2014,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8061,
-  serialized_end=8147,
+  serialized_start=8124,
+  serialized_end=8210,
 )
 
 
 _GATEWAYHEARTBEAT = _descriptor.Descriptor(
   name='GatewayHeartbeat',
   full_name='com.wirepas.proto.wnt.GatewayHeartbeat',
   filename=None,
@@ -2148,16 +2053,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8149,
-  serialized_end=8206,
+  serialized_start=8212,
+  serialized_end=8269,
 )
 
 
 _GATEWAYINFO = _descriptor.Descriptor(
   name='GatewayInfo',
   full_name='com.wirepas.proto.wnt.GatewayInfo',
   filename=None,
@@ -2201,16 +2106,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8208,
-  serialized_end=8304,
+  serialized_start=8271,
+  serialized_end=8367,
 )
 
 
 _BACKENDCOMPONENTINFO = _descriptor.Descriptor(
   name='BackendComponentInfo',
   full_name='com.wirepas.proto.wnt.BackendComponentInfo',
   filename=None,
@@ -2240,16 +2145,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8306,
-  serialized_end=8418,
+  serialized_start=8369,
+  serialized_end=8481,
 )
 
 
 _CHANNELIDTOFREQMAP = _descriptor.Descriptor(
   name='ChannelIdToFreqMap',
   full_name='com.wirepas.proto.wnt.ChannelIdToFreqMap',
   filename=None,
@@ -2279,16 +2184,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8420,
-  serialized_end=8470,
+  serialized_start=8483,
+  serialized_end=8533,
 )
 
 
 _ACCESSCYCLELIMITS = _descriptor.Descriptor(
   name='AccessCycleLimits',
   full_name='com.wirepas.proto.wnt.AccessCycleLimits',
   filename=None,
@@ -2318,16 +2223,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8472,
-  serialized_end=8523,
+  serialized_start=8535,
+  serialized_end=8586,
 )
 
 
 _NODEMESSAGE = _descriptor.Descriptor(
   name='NodeMessage',
   full_name='com.wirepas.proto.wnt.NodeMessage',
   filename=None,
@@ -2385,16 +2290,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8526,
-  serialized_end=8675,
+  serialized_start=8589,
+  serialized_end=8738,
 )
 
 
 _GETSCRATCHPADSTATUS = _descriptor.Descriptor(
   name='GetScratchpadStatus',
   full_name='com.wirepas.proto.wnt.GetScratchpadStatus',
   filename=None,
@@ -2452,16 +2357,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8678,
-  serialized_end=8900,
+  serialized_start=8741,
+  serialized_end=8963,
 )
 
 
 _SCRATCHPADSTATUS = _descriptor.Descriptor(
   name='ScratchpadStatus',
   full_name='com.wirepas.proto.wnt.ScratchpadStatus',
   filename=None,
@@ -2673,16 +2578,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8903,
-  serialized_end=10070,
+  serialized_start=8966,
+  serialized_end=10133,
 )
 
 
 _SETSCRATCHPADACTION = _descriptor.Descriptor(
   name='SetScratchpadAction',
   full_name='com.wirepas.proto.wnt.SetScratchpadAction',
   filename=None,
@@ -2712,16 +2617,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10072,
-  serialized_end=10181,
+  serialized_start=10135,
+  serialized_end=10244,
 )
 
 
 _MESSAGE = _descriptor.Descriptor(
   name='Message',
   full_name='com.wirepas.proto.wnt.Message',
   filename=None,
@@ -3031,16 +2936,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10184,
-  serialized_end=12560,
+  serialized_start=10247,
+  serialized_end=12623,
 )
 
 
 _MESSAGECOLLECTION = _descriptor.Descriptor(
   name='MessageCollection',
   full_name='com.wirepas.proto.wnt.MessageCollection',
   filename=None,
@@ -3063,26 +2968,26 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12562,
-  serialized_end=12641,
+  serialized_start=12625,
+  serialized_end=12704,
 )
 
 _NEIGHBOR.fields_by_name['neighbor_type'].enum_type = _NEIGHBOR_NEIGHBORTYPE
 _NEIGHBOR_NEIGHBORTYPE.containing_type = _NEIGHBOR
 _DIAGNOSTICSDATA.fields_by_name['neighbors'].message_type = _NEIGHBOR
 _DIAGNOSTICSDATA.fields_by_name['role'].enum_type = commons__pb2._BASEROLE
 _DIAGNOSTICSDATA.fields_by_name['cost'].message_type = _COSTINFO
 _DIAGNOSTICSDATA.fields_by_name['events'].enum_type = _DIAGNOSTICSDATA_EVENTS
 _DIAGNOSTICSDATA.fields_by_name['hw_magic'].enum_type = _DIAGNOSTICSDATA_HWMAGIC
-_DIAGNOSTICSDATA.fields_by_name['stack_profile'].enum_type = _STACKPROFILE
+_DIAGNOSTICSDATA.fields_by_name['stack_profile'].enum_type = commons__pb2._STACKPROFILE
 _DIAGNOSTICSDATA.fields_by_name['trace_type'].enum_type = _DIAGNOSTICSDATA_TRACETYPE
 _DIAGNOSTICSDATA.fields_by_name['boot_reason'].enum_type = _DIAGNOSTICSDATA_BOOTREASON
 _DIAGNOSTICSDATA.fields_by_name['installation_quality_errors'].enum_type = _DIAGNOSTICSDATA_INSTALLATIONQUALITYERROR
 _DIAGNOSTICSDATA_EVENTS.containing_type = _DIAGNOSTICSDATA
 _DIAGNOSTICSDATA_HWMAGIC.containing_type = _DIAGNOSTICSDATA
 _DIAGNOSTICSDATA_TRACETYPE.containing_type = _DIAGNOSTICSDATA
 _DIAGNOSTICSDATA_BOOTREASON.containing_type = _DIAGNOSTICSDATA
@@ -3094,15 +2999,15 @@
 _SCRATCHPADSTATUS.fields_by_name['stored_scratchpad_type'].enum_type = _SCRATCHPADTYPE
 _SCRATCHPADSTATUS.fields_by_name['stored_scratchpad_status'].enum_type = _SCRATCHPADWRITESTATUS
 _SCRATCHPADSTATUS.fields_by_name['scratchpad_action'].enum_type = commons__pb2._SCRATCHPADACTION
 _SETSCRATCHPADACTION.fields_by_name['scratchpad_action'].enum_type = commons__pb2._SCRATCHPADACTION
 _MESSAGE.fields_by_name['diagnostics'].message_type = _DIAGNOSTICSDATA
 _MESSAGE.fields_by_name['rx_data'].message_type = _RXDATA
 _MESSAGE.fields_by_name['app_config'].message_type = commons__pb2._APPCONFIGDATA
-_MESSAGE.fields_by_name['stack_profile'].enum_type = _STACKPROFILE
+_MESSAGE.fields_by_name['stack_profile'].enum_type = commons__pb2._STACKPROFILE
 _MESSAGE.fields_by_name['measurement'].message_type = _MEASUREMENT
 _MESSAGE.fields_by_name['gw_heartbeat'].message_type = _GATEWAYHEARTBEAT
 _MESSAGE.fields_by_name['tx_data'].message_type = _RXDATA
 _MESSAGE.fields_by_name['channel_info'].message_type = _CHANNELIDTOFREQMAP
 _MESSAGE.fields_by_name['app_config_response'].message_type = _APPCONFIGRESPONSE
 _MESSAGE.fields_by_name['access_cycle_limits'].message_type = _ACCESSCYCLELIMITS
 _MESSAGE.fields_by_name['gateway_info'].message_type = _GATEWAYINFO
@@ -3142,15 +3047,14 @@
 DESCRIPTOR.message_types_by_name['AccessCycleLimits'] = _ACCESSCYCLELIMITS
 DESCRIPTOR.message_types_by_name['NodeMessage'] = _NODEMESSAGE
 DESCRIPTOR.message_types_by_name['GetScratchpadStatus'] = _GETSCRATCHPADSTATUS
 DESCRIPTOR.message_types_by_name['ScratchpadStatus'] = _SCRATCHPADSTATUS
 DESCRIPTOR.message_types_by_name['SetScratchpadAction'] = _SETSCRATCHPADACTION
 DESCRIPTOR.message_types_by_name['Message'] = _MESSAGE
 DESCRIPTOR.message_types_by_name['MessageCollection'] = _MESSAGECOLLECTION
-DESCRIPTOR.enum_types_by_name['StackProfile'] = _STACKPROFILE
 DESCRIPTOR.enum_types_by_name['ScratchpadType'] = _SCRATCHPADTYPE
 DESCRIPTOR.enum_types_by_name['ScratchpadWriteStatus'] = _SCRATCHPADWRITESTATUS
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Neighbor = _reflection.GeneratedProtocolMessageType('Neighbor', (_message.Message,), {
   'DESCRIPTOR' : _NEIGHBOR,
   '__module__' : 'message_pb2'
```

### Comparing `wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/otap_pb2.py` & `wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/otap_pb2.py`

 * *Files identical despite different names*

### Comparing `wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/positioning_pb2.py` & `wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/positioning_pb2.py`

 * *Files identical despite different names*

### Comparing `wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging/proto/remote_api_pb2.py` & `wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging/proto/remote_api_pb2.py`

 * *Files identical despite different names*

### Comparing `wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging.egg-info/PKG-INFO` & `wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wirepas-networktool-messaging
-Version: 4.4.0
+Version: 4.4.1
 Summary: WNT protocol buffers bindings.
 Home-page: https://github.com/wirepas/wirepas-networktool-messaging-python
 Author: Wirepas Ltd
 Author-email: opensource@wirepas.com
 License: Apache-2
 Keywords: wirepas WNT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wirepas_networktool_messaging-4.4.0/wirepas_networktool_messaging.egg-info/SOURCES.txt` & `wirepas_networktool_messaging-4.4.1/wirepas_networktool_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*


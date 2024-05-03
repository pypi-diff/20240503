# Comparing `tmp/ovs-3.1.4.tar.gz` & `tmp/ovs-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovs-3.1.4.tar", last modified: Fri May  3 15:12:30 2024, max compression
+gzip compressed data, was "ovs-3.2.2.tar", last modified: Fri May  3 15:13:14 2024, max compression
```

## Comparing `ovs-3.1.4.tar` & `ovs-3.2.2.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:12:30.285089 ovs-3.1.4/
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)      837 2024-05-03 15:12:30.285089 ovs-3.1.4/PKG-INFO
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       45 2023-08-25 20:48:29.000000 ovs-3.1.4/README.rst
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:12:30.282089 ovs-3.1.4/ovs/
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       38 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/__init__.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     5226 2024-05-03 15:12:09.000000 ovs-3.1.4/ovs/_json.c
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:12:30.283089 ovs-3.1.4/ovs/compat/
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)        0 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/compat/__init__.py
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:12:30.283089 ovs-3.1.4/ovs/compat/sortedcontainers/
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     2131 2023-11-03 18:53:22.000000 ovs-3.1.4/ovs/compat/sortedcontainers/__init__.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    22712 2023-11-03 18:53:22.000000 ovs-3.1.4/ovs/compat/sortedcontainers/sorteddict.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    76293 2023-11-03 18:53:22.000000 ovs-3.1.4/ovs/compat/sortedcontainers/sortedlist.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    19825 2023-11-03 18:53:22.000000 ovs-3.1.4/ovs/compat/sortedcontainers/sortedset.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    20710 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/daemon.py
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:12:30.284089 ovs-3.1.4/ovs/db/
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       38 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/db/__init__.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     4856 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/db/custom_index.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    21659 2024-01-26 22:17:23.000000 ovs-3.1.4/ovs/db/data.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1156 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/db/error.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    98436 2024-05-03 15:12:09.000000 ovs-3.1.4/ovs/db/idl.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     3647 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/db/parser.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    11947 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/db/schema.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    23240 2024-01-26 22:17:23.000000 ovs-3.1.4/ovs/db/types.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     1371 2024-04-30 12:58:44.000000 ovs-3.1.4/ovs/dirs.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     4765 2024-05-03 14:58:55.000000 ovs-3.1.4/ovs/fatal_signal.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1330 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/fcntl_win.py
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:12:30.284089 ovs-3.1.4/ovs/flow/
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)      476 2024-05-03 15:09:39.000000 ovs-3.1.4/ovs/flow/__init__.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    14382 2024-05-03 15:09:39.000000 ovs-3.1.4/ovs/flow/decoders.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     7502 2024-05-03 15:09:39.000000 ovs-3.1.4/ovs/flow/filter.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     3772 2024-05-03 15:09:39.000000 ovs-3.1.4/ovs/flow/flow.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    11970 2024-05-03 15:09:39.000000 ovs-3.1.4/ovs/flow/kv.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     4005 2024-05-03 15:09:39.000000 ovs-3.1.4/ovs/flow/list.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    27938 2024-05-03 15:09:39.000000 ovs-3.1.4/ovs/flow/odp.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    14363 2024-05-03 15:12:09.000000 ovs-3.1.4/ovs/flow/ofp.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     9572 2024-05-03 15:12:09.000000 ovs-3.1.4/ovs/flow/ofp_act.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    15413 2024-05-03 15:10:22.000000 ovs-3.1.4/ovs/flow/ofp_fields.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    16843 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/json.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    21091 2024-05-03 12:23:34.000000 ovs-3.1.4/ovs/jsonrpc.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1869 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/ovsuuid.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    10282 2024-01-26 22:17:23.000000 ovs-3.1.4/ovs/poller.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1467 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/process.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    26007 2024-01-26 22:17:23.000000 ovs-3.1.4/ovs/reconnect.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    11976 2024-05-03 14:58:55.000000 ovs-3.1.4/ovs/socket_util.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    32175 2024-05-03 14:58:55.000000 ovs-3.1.4/ovs/stream.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     2432 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/timeval.py
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:12:30.285089 ovs-3.1.4/ovs/unixctl/
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     3032 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/unixctl/__init__.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1999 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/unixctl/client.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     8121 2024-05-03 14:58:55.000000 ovs-3.1.4/ovs/unixctl/server.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     3120 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/util.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)       93 2024-05-03 15:12:27.000000 ovs-3.1.4/ovs/version.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    16694 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/vlog.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     9226 2023-08-25 20:48:29.000000 ovs-3.1.4/ovs/winutils.py
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:12:30.285089 ovs-3.1.4/ovs.egg-info/
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)      837 2024-05-03 15:12:30.000000 ovs-3.1.4/ovs.egg-info/PKG-INFO
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1013 2024-05-03 15:12:30.000000 ovs-3.1.4/ovs.egg-info/SOURCES.txt
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)        1 2024-05-03 15:12:30.000000 ovs-3.1.4/ovs.egg-info/dependency_links.txt
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       84 2024-05-03 15:12:30.000000 ovs-3.1.4/ovs.egg-info/requires.txt
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)        4 2024-05-03 15:12:30.000000 ovs-3.1.4/ovs.egg-info/top_level.txt
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)       38 2024-05-03 15:12:30.285089 ovs-3.1.4/setup.cfg
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     4350 2024-05-03 15:09:39.000000 ovs-3.1.4/setup.py
+drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:13:14.094216 ovs-3.2.2/
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)      846 2024-05-03 15:13:14.093217 ovs-3.2.2/PKG-INFO
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       45 2023-08-25 20:48:29.000000 ovs-3.2.2/README.rst
+drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:13:14.090216 ovs-3.2.2/ovs/
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       38 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/__init__.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     5226 2024-05-03 15:12:09.000000 ovs-3.2.2/ovs/_json.c
+drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:13:14.090216 ovs-3.2.2/ovs/compat/
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)        0 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/compat/__init__.py
+drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:13:14.091216 ovs-3.2.2/ovs/compat/sortedcontainers/
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     2131 2023-11-03 18:53:22.000000 ovs-3.2.2/ovs/compat/sortedcontainers/__init__.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    22712 2023-11-03 18:53:22.000000 ovs-3.2.2/ovs/compat/sortedcontainers/sorteddict.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    76293 2023-11-03 18:53:22.000000 ovs-3.2.2/ovs/compat/sortedcontainers/sortedlist.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    19825 2023-11-03 18:53:22.000000 ovs-3.2.2/ovs/compat/sortedcontainers/sortedset.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    20710 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/daemon.py
+drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:13:14.092216 ovs-3.2.2/ovs/db/
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       38 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/db/__init__.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     4856 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/db/custom_index.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    21659 2024-01-26 22:17:23.000000 ovs-3.2.2/ovs/db/data.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1156 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/db/error.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    98436 2024-05-03 15:12:09.000000 ovs-3.2.2/ovs/db/idl.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     3647 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/db/parser.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    11947 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/db/schema.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    23240 2024-01-26 22:17:23.000000 ovs-3.2.2/ovs/db/types.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     1371 2024-04-30 12:58:44.000000 ovs-3.2.2/ovs/dirs.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     9740 2024-05-03 15:12:51.000000 ovs-3.2.2/ovs/dns_resolve.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     4765 2024-05-03 14:58:55.000000 ovs-3.2.2/ovs/fatal_signal.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1330 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/fcntl_win.py
+drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:13:14.093217 ovs-3.2.2/ovs/flow/
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)      476 2024-05-03 15:09:39.000000 ovs-3.2.2/ovs/flow/__init__.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    14382 2024-05-03 15:09:39.000000 ovs-3.2.2/ovs/flow/decoders.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     7502 2024-05-03 15:09:39.000000 ovs-3.2.2/ovs/flow/filter.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     3772 2024-05-03 15:09:39.000000 ovs-3.2.2/ovs/flow/flow.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    11970 2024-05-03 15:09:39.000000 ovs-3.2.2/ovs/flow/kv.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     4005 2024-05-03 15:09:39.000000 ovs-3.2.2/ovs/flow/list.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    28375 2024-05-03 15:12:51.000000 ovs-3.2.2/ovs/flow/odp.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    14363 2024-05-03 15:12:09.000000 ovs-3.2.2/ovs/flow/ofp.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     9572 2024-05-03 15:12:09.000000 ovs-3.2.2/ovs/flow/ofp_act.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    15413 2024-05-03 15:10:22.000000 ovs-3.2.2/ovs/flow/ofp_fields.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    16843 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/json.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    21091 2024-05-03 12:23:34.000000 ovs-3.2.2/ovs/jsonrpc.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1869 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/ovsuuid.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    10282 2024-01-26 22:17:23.000000 ovs-3.2.2/ovs/poller.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1467 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/process.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    26007 2024-01-26 22:17:23.000000 ovs-3.2.2/ovs/reconnect.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    12479 2024-05-03 15:12:51.000000 ovs-3.2.2/ovs/socket_util.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    32189 2024-05-03 15:12:51.000000 ovs-3.2.2/ovs/stream.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     2432 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/timeval.py
+drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:13:14.093217 ovs-3.2.2/ovs/unixctl/
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     3032 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/unixctl/__init__.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1999 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/unixctl/client.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     8121 2024-05-03 14:58:55.000000 ovs-3.2.2/ovs/unixctl/server.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     3120 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/util.py
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)       93 2024-05-03 15:13:11.000000 ovs-3.2.2/ovs/version.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    16694 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/vlog.py
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     9226 2023-08-25 20:48:29.000000 ovs-3.2.2/ovs/winutils.py
+drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:13:14.093217 ovs-3.2.2/ovs.egg-info/
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)      846 2024-05-03 15:13:14.000000 ovs-3.2.2/ovs.egg-info/PKG-INFO
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1032 2024-05-03 15:13:14.000000 ovs-3.2.2/ovs.egg-info/SOURCES.txt
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)        1 2024-05-03 15:13:14.000000 ovs-3.2.2/ovs.egg-info/dependency_links.txt
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       99 2024-05-03 15:13:14.000000 ovs-3.2.2/ovs.egg-info/requires.txt
+-rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)        4 2024-05-03 15:13:14.000000 ovs-3.2.2/ovs.egg-info/top_level.txt
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)       38 2024-05-03 15:13:14.094216 ovs-3.2.2/setup.cfg
+-rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     4341 2024-05-03 15:12:51.000000 ovs-3.2.2/setup.py
```

### Comparing `ovs-3.1.4/PKG-INFO` & `ovs-3.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ovs
-Version: 3.1.4
+Version: 3.2.2
 Summary: Open vSwitch library
 Home-page: http://www.openvswitch.org/
 Author: Open vSwitch
 Author-email: dev@openvswitch.org
 License: Apache 2.0
 Keywords: openvswitch,ovs,OVSDB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Requires-Dist: sortedcontainers
 Requires-Dist: pywin32>=1.0; sys_platform == "win32"
 Provides-Extra: flow
 Requires-Dist: netaddr; extra == "flow"
 Requires-Dist: pyparsing; extra == "flow"
+Provides-Extra: dns
+Requires-Dist: unbound; extra == "dns"
```

### Comparing `ovs-3.1.4/ovs/_json.c` & `ovs-3.2.2/ovs/_json.c`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/compat/sortedcontainers/__init__.py` & `ovs-3.2.2/ovs/compat/sortedcontainers/__init__.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/compat/sortedcontainers/sorteddict.py` & `ovs-3.2.2/ovs/compat/sortedcontainers/sorteddict.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/compat/sortedcontainers/sortedlist.py` & `ovs-3.2.2/ovs/compat/sortedcontainers/sortedlist.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/compat/sortedcontainers/sortedset.py` & `ovs-3.2.2/ovs/compat/sortedcontainers/sortedset.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/daemon.py` & `ovs-3.2.2/ovs/daemon.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/db/custom_index.py` & `ovs-3.2.2/ovs/db/custom_index.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/db/data.py` & `ovs-3.2.2/ovs/db/data.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/db/error.py` & `ovs-3.2.2/ovs/db/error.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/db/idl.py` & `ovs-3.2.2/ovs/db/idl.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/db/parser.py` & `ovs-3.2.2/ovs/db/parser.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/db/schema.py` & `ovs-3.2.2/ovs/db/schema.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/db/types.py` & `ovs-3.2.2/ovs/db/types.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/dirs.py` & `ovs-3.2.2/ovs/dirs.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/fatal_signal.py` & `ovs-3.2.2/ovs/fatal_signal.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/fcntl_win.py` & `ovs-3.2.2/ovs/fcntl_win.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/flow/decoders.py` & `ovs-3.2.2/ovs/flow/decoders.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/flow/filter.py` & `ovs-3.2.2/ovs/flow/filter.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/flow/flow.py` & `ovs-3.2.2/ovs/flow/flow.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/flow/kv.py` & `ovs-3.2.2/ovs/flow/kv.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/flow/list.py` & `ovs-3.2.2/ovs/flow/list.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/flow/odp.py` & `ovs-3.2.2/ovs/flow/odp.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,14 +482,22 @@
                                             {
                                                 "flags": decode_int,
                                                 "msgtype": decode_int,
                                                 "teid": decode_int,
                                             }
                                         )
                                     ),
+                                    "srv6": nested_kv_decoder(
+                                        KVDecoders(
+                                            {
+                                                "segments_left": decode_int,
+                                                "segs": decode_default,
+                                            }
+                                        )
+                                    ),
                                 }
                             )
                         ),
                         "out_port": decode_default,
                     }
                 )
             )
```

### Comparing `ovs-3.1.4/ovs/flow/ofp.py` & `ovs-3.2.2/ovs/flow/ofp.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/flow/ofp_act.py` & `ovs-3.2.2/ovs/flow/ofp_act.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/flow/ofp_fields.py` & `ovs-3.2.2/ovs/flow/ofp_fields.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/json.py` & `ovs-3.2.2/ovs/json.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/jsonrpc.py` & `ovs-3.2.2/ovs/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/ovsuuid.py` & `ovs-3.2.2/ovs/ovsuuid.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/poller.py` & `ovs-3.2.2/ovs/poller.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/process.py` & `ovs-3.2.2/ovs/process.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/reconnect.py` & `ovs-3.2.2/ovs/reconnect.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/socket_util.py` & `ovs-3.2.2/ovs/socket_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import errno
+import ipaddress
 import os
 import os.path
 import random
 import socket
 import sys
 
+from ovs import dns_resolve
 import ovs.fatal_signal
 import ovs.poller
 import ovs.vlog
 
 try:
     import ssl
 except ImportError:
@@ -212,30 +214,45 @@
             return False
     except socket.error:
         return False
 
     return True
 
 
-def inet_parse_active(target, default_port):
+def _inet_parse_active(target, default_port):
     address = target.split(":")
     if len(address) >= 2:
         host_name = ":".join(address[0:-1]).lstrip('[').rstrip(']')
         port = int(address[-1])
     else:
         if default_port:
             port = default_port
         else:
             raise ValueError("%s: port number must be specified" % target)
         host_name = address[0]
     if not host_name:
         raise ValueError("%s: bad peer name format" % target)
+    try:
+        host_name = str(ipaddress.ip_address(host_name))
+    except ValueError:
+        host_name = dns_resolve.resolve(host_name)
+    if not host_name:
+        raise ValueError("%s: bad peer name format" % target)
     return (host_name, port)
 
 
+def inet_parse_active(target, default_port, raises=True):
+    try:
+        return _inet_parse_active(target, default_port)
+    except ValueError:
+        if raises:
+            raise
+        return ("", default_port)
+
+
 def inet_create_socket_active(style, address):
     try:
         is_addr_inet = is_valid_ipv4_address(address[0])
         if is_addr_inet:
             sock = socket.socket(socket.AF_INET, style, 0)
             family = socket.AF_INET
         else:
@@ -258,15 +275,15 @@
         return 0
     except socket.error as e:
         sock.close()
         return get_exception_errno(e)
 
 
 def inet_open_active(style, target, default_port, dscp):
-    address = inet_parse_active(target, default_port)
+    address = inet_parse_active(target, default_port, raises=False)
     family, sock = inet_create_socket_active(style, address)
     if sock is None:
         return family, sock
     error = inet_connect_active(sock, address, family, dscp)
     if error:
         return error, None
     return 0, sock
```

### Comparing `ovs-3.1.4/ovs/stream.py` & `ovs-3.2.2/ovs/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -780,15 +780,15 @@
 
     @staticmethod
     def needs_probes():
         return True
 
     @staticmethod
     def _open(suffix, dscp):
-        address = ovs.socket_util.inet_parse_active(suffix, 0)
+        address = ovs.socket_util.inet_parse_active(suffix, 0, raises=False)
         family, sock = ovs.socket_util.inet_create_socket_active(
                 socket.SOCK_STREAM, address)
         if sock is None:
             return family, sock
 
         # Create an SSL context
         ctx = ssl.SSLContext(ssl.PROTOCOL_SSLv23)
```

### Comparing `ovs-3.1.4/ovs/timeval.py` & `ovs-3.2.2/ovs/timeval.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/unixctl/__init__.py` & `ovs-3.2.2/ovs/unixctl/__init__.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/unixctl/client.py` & `ovs-3.2.2/ovs/unixctl/client.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/unixctl/server.py` & `ovs-3.2.2/ovs/unixctl/server.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/util.py` & `ovs-3.2.2/ovs/util.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/vlog.py` & `ovs-3.2.2/ovs/vlog.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs/winutils.py` & `ovs-3.2.2/ovs/winutils.py`

 * *Files identical despite different names*

### Comparing `ovs-3.1.4/ovs.egg-info/PKG-INFO` & `ovs-3.2.2/ovs.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ovs
-Version: 3.1.4
+Version: 3.2.2
 Summary: Open vSwitch library
 Home-page: http://www.openvswitch.org/
 Author: Open vSwitch
 Author-email: dev@openvswitch.org
 License: Apache 2.0
 Keywords: openvswitch,ovs,OVSDB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Requires-Dist: sortedcontainers
 Requires-Dist: pywin32>=1.0; sys_platform == "win32"
 Provides-Extra: flow
 Requires-Dist: netaddr; extra == "flow"
 Requires-Dist: pyparsing; extra == "flow"
+Provides-Extra: dns
+Requires-Dist: unbound; extra == "dns"
```

### Comparing `ovs-3.1.4/ovs.egg-info/SOURCES.txt` & `ovs-3.2.2/ovs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.rst
 setup.py
 ovs/__init__.py
 ovs/_json.c
 ovs/daemon.py
 ovs/dirs.py
+ovs/dns_resolve.py
 ovs/fatal_signal.py
 ovs/fcntl_win.py
 ovs/json.py
 ovs/jsonrpc.py
 ovs/ovsuuid.py
 ovs/poller.py
 ovs/process.py
```

### Comparing `ovs-3.1.4/setup.py` & `ovs-3.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,26 +95,26 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Topic :: Database :: Front-Ends',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: System :: Networking',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
     ],
     ext_modules=[setuptools.Extension("ovs._json",
                                       sources=["ovs/_json.c"],
                                       libraries=libraries,
                                       extra_compile_args=extra_cflags,
                                       extra_link_args=extra_libs)],
     cmdclass={'build_ext': try_build_ext},
     install_requires=['sortedcontainers'],
     extras_require={':sys_platform == "win32"': ['pywin32 >= 1.0'],
-                    'flow': ['netaddr', 'pyparsing']},
+                    'flow': ['netaddr', 'pyparsing'],
+                    'dns': ['unbound']},
 )
 
 try:
     setuptools.setup(**setup_args)
 except BuildFailed:
     BUILD_EXT_WARNING = ("WARNING: The C extension could not be compiled, "
                          "speedups are not enabled.")
```


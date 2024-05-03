# Comparing `tmp/ovs-3.0.6.tar.gz` & `tmp/ovs-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovs-3.0.6.tar", last modified: Fri May  3 15:10:25 2024, max compression
+gzip compressed data, was "ovs-3.1.2.tar", last modified: Tue Aug  1 19:26:56 2023, max compression
```

## Comparing `ovs-3.0.6.tar` & `ovs-3.1.2.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:10:25.119723 ovs-3.0.6/
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)      837 2024-05-03 15:10:25.119723 ovs-3.0.6/PKG-INFO
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       45 2023-08-25 20:48:29.000000 ovs-3.0.6/README.rst
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:10:25.116723 ovs-3.0.6/ovs/
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       38 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/__init__.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     7038 2024-05-03 14:58:55.000000 ovs-3.0.6/ovs/_json.c
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:10:25.116723 ovs-3.0.6/ovs/compat/
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)        0 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/compat/__init__.py
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:10:25.117724 ovs-3.0.6/ovs/compat/sortedcontainers/
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     2131 2023-11-03 18:53:22.000000 ovs-3.0.6/ovs/compat/sortedcontainers/__init__.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    22712 2023-11-03 18:53:22.000000 ovs-3.0.6/ovs/compat/sortedcontainers/sorteddict.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    76293 2023-11-03 18:53:22.000000 ovs-3.0.6/ovs/compat/sortedcontainers/sortedlist.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    19825 2023-11-03 18:53:22.000000 ovs-3.0.6/ovs/compat/sortedcontainers/sortedset.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    20710 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/daemon.py
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:10:25.117724 ovs-3.0.6/ovs/db/
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       38 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/db/__init__.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     4856 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/db/custom_index.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    21659 2024-01-26 22:17:23.000000 ovs-3.0.6/ovs/db/data.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1156 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/db/error.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    97950 2024-05-03 14:58:55.000000 ovs-3.0.6/ovs/db/idl.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     3647 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/db/parser.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    11947 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/db/schema.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    23240 2024-01-26 22:17:23.000000 ovs-3.0.6/ovs/db/types.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     1371 2024-04-30 12:58:44.000000 ovs-3.0.6/ovs/dirs.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     4765 2024-05-03 14:58:55.000000 ovs-3.0.6/ovs/fatal_signal.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1330 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/fcntl_win.py
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:10:25.118723 ovs-3.0.6/ovs/flow/
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)      476 2024-05-03 15:09:39.000000 ovs-3.0.6/ovs/flow/__init__.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    14382 2024-05-03 15:09:39.000000 ovs-3.0.6/ovs/flow/decoders.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     7502 2024-05-03 15:09:39.000000 ovs-3.0.6/ovs/flow/filter.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     3772 2024-05-03 15:09:39.000000 ovs-3.0.6/ovs/flow/flow.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    11970 2024-05-03 15:09:39.000000 ovs-3.0.6/ovs/flow/kv.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     4005 2024-05-03 15:09:39.000000 ovs-3.0.6/ovs/flow/list.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    27938 2024-05-03 15:09:39.000000 ovs-3.0.6/ovs/flow/odp.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    14304 2024-05-03 15:09:39.000000 ovs-3.0.6/ovs/flow/ofp.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     9562 2024-05-03 15:09:39.000000 ovs-3.0.6/ovs/flow/ofp_act.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    15413 2024-05-03 15:10:22.000000 ovs-3.0.6/ovs/flow/ofp_fields.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    16843 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/json.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    21091 2024-05-03 12:23:34.000000 ovs-3.0.6/ovs/jsonrpc.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1869 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/ovsuuid.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    10282 2024-01-26 22:17:23.000000 ovs-3.0.6/ovs/poller.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1467 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/process.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    26007 2024-01-26 22:17:23.000000 ovs-3.0.6/ovs/reconnect.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    11976 2024-05-03 14:58:55.000000 ovs-3.0.6/ovs/socket_util.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)    32175 2024-05-03 14:58:55.000000 ovs-3.0.6/ovs/stream.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     2432 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/timeval.py
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:10:25.119723 ovs-3.0.6/ovs/unixctl/
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     3032 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/unixctl/__init__.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1999 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/unixctl/client.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     8121 2024-05-03 14:58:55.000000 ovs-3.0.6/ovs/unixctl/server.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     3120 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/util.py
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)       93 2024-05-03 15:10:22.000000 ovs-3.0.6/ovs/version.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)    16694 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/vlog.py
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     9226 2023-08-25 20:48:29.000000 ovs-3.0.6/ovs/winutils.py
-drwxr-xr-x   0 i.maximets  (1000) i.maximets  (1000)        0 2024-05-03 15:10:25.119723 ovs-3.0.6/ovs.egg-info/
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)      837 2024-05-03 15:10:25.000000 ovs-3.0.6/ovs.egg-info/PKG-INFO
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)     1013 2024-05-03 15:10:25.000000 ovs-3.0.6/ovs.egg-info/SOURCES.txt
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)        1 2024-05-03 15:10:25.000000 ovs-3.0.6/ovs.egg-info/dependency_links.txt
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)       84 2024-05-03 15:10:25.000000 ovs-3.0.6/ovs.egg-info/requires.txt
--rw-rw-r--   0 i.maximets  (1000) i.maximets  (1000)        4 2024-05-03 15:10:25.000000 ovs-3.0.6/ovs.egg-info/top_level.txt
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)       38 2024-05-03 15:10:25.119723 ovs-3.0.6/setup.cfg
--rw-r--r--   0 i.maximets  (1000) i.maximets  (1000)     4350 2024-05-03 15:09:39.000000 ovs-3.0.6/setup.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:26:56.066248 ovs-3.1.2/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)      670 2023-08-01 19:26:56.066248 ovs-3.1.2/PKG-INFO
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       45 2021-09-20 16:15:26.000000 ovs-3.1.2/README.rst
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:26:56.062248 ovs-3.1.2/ovs/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2021-09-20 16:15:26.000000 ovs-3.1.2/ovs/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     5226 2023-08-01 19:23:57.000000 ovs-3.1.2/ovs/_json.c
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:26:56.063248 ovs-3.1.2/ovs/compat/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)        0 2021-10-20 17:21:43.000000 ovs-3.1.2/ovs/compat/__init__.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:26:56.063248 ovs-3.1.2/ovs/compat/sortedcontainers/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     2131 2023-01-27 14:27:10.000000 ovs-3.1.2/ovs/compat/sortedcontainers/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    22712 2023-01-27 14:27:10.000000 ovs-3.1.2/ovs/compat/sortedcontainers/sorteddict.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    76293 2023-01-27 14:27:10.000000 ovs-3.1.2/ovs/compat/sortedcontainers/sortedlist.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    19825 2023-01-27 14:27:10.000000 ovs-3.1.2/ovs/compat/sortedcontainers/sortedset.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    20710 2021-09-20 16:15:26.000000 ovs-3.1.2/ovs/daemon.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:26:56.064247 ovs-3.1.2/ovs/db/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2021-09-20 16:15:26.000000 ovs-3.1.2/ovs/db/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     4856 2021-11-05 13:35:58.000000 ovs-3.1.2/ovs/db/custom_index.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    21659 2023-06-14 20:52:13.000000 ovs-3.1.2/ovs/db/data.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1156 2021-10-20 17:21:43.000000 ovs-3.1.2/ovs/db/error.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    97303 2023-08-01 19:23:57.000000 ovs-3.1.2/ovs/db/idl.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3647 2021-10-20 17:21:43.000000 ovs-3.1.2/ovs/db/parser.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    11947 2021-10-20 17:21:43.000000 ovs-3.1.2/ovs/db/schema.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    23240 2023-01-27 14:27:10.000000 ovs-3.1.2/ovs/db/types.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1329 2023-08-01 19:25:33.000000 ovs-3.1.2/ovs/dirs.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     4765 2021-10-20 17:21:43.000000 ovs-3.1.2/ovs/fatal_signal.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1330 2021-09-20 16:15:26.000000 ovs-3.1.2/ovs/fcntl_win.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:26:56.066248 ovs-3.1.2/ovs/flow/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)      476 2023-01-27 14:27:10.000000 ovs-3.1.2/ovs/flow/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    14382 2023-01-27 14:27:10.000000 ovs-3.1.2/ovs/flow/decoders.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     7502 2023-01-27 14:27:10.000000 ovs-3.1.2/ovs/flow/filter.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3772 2023-01-27 14:27:10.000000 ovs-3.1.2/ovs/flow/flow.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    11970 2023-08-01 19:23:57.000000 ovs-3.1.2/ovs/flow/kv.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     4005 2023-08-01 19:23:57.000000 ovs-3.1.2/ovs/flow/list.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    27631 2023-08-01 19:23:57.000000 ovs-3.1.2/ovs/flow/odp.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    14325 2023-08-01 19:23:57.000000 ovs-3.1.2/ovs/flow/ofp.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     9528 2023-08-01 19:23:57.000000 ovs-3.1.2/ovs/flow/ofp_act.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    15413 2023-08-01 19:25:48.000000 ovs-3.1.2/ovs/flow/ofp_fields.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    16843 2021-10-20 17:21:43.000000 ovs-3.1.2/ovs/json.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    21087 2023-04-18 01:01:46.000000 ovs-3.1.2/ovs/jsonrpc.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1869 2021-10-20 17:21:43.000000 ovs-3.1.2/ovs/ovsuuid.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    10282 2023-01-27 14:27:10.000000 ovs-3.1.2/ovs/poller.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1467 2021-09-20 16:15:26.000000 ovs-3.1.2/ovs/process.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    26007 2023-05-17 03:37:46.000000 ovs-3.1.2/ovs/reconnect.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    11976 2023-08-01 15:27:48.000000 ovs-3.1.2/ovs/socket_util.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    32175 2023-08-01 19:23:58.000000 ovs-3.1.2/ovs/stream.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     2432 2021-09-20 16:15:26.000000 ovs-3.1.2/ovs/timeval.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:26:56.066248 ovs-3.1.2/ovs/unixctl/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3032 2021-10-20 17:21:43.000000 ovs-3.1.2/ovs/unixctl/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1999 2021-10-20 17:21:43.000000 ovs-3.1.2/ovs/unixctl/client.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     8121 2021-10-20 17:21:43.000000 ovs-3.1.2/ovs/unixctl/server.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3120 2022-09-19 19:15:14.000000 ovs-3.1.2/ovs/util.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       93 2023-08-01 19:25:48.000000 ovs-3.1.2/ovs/version.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    16694 2021-10-20 17:21:43.000000 ovs-3.1.2/ovs/vlog.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     9226 2021-09-20 16:15:26.000000 ovs-3.1.2/ovs/winutils.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:26:56.063248 ovs-3.1.2/ovs.egg-info/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)      670 2023-08-01 19:26:56.000000 ovs-3.1.2/ovs.egg-info/PKG-INFO
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1028 2023-08-01 19:26:56.000000 ovs-3.1.2/ovs.egg-info/SOURCES.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)        1 2023-08-01 19:26:56.000000 ovs-3.1.2/ovs.egg-info/dependency_links.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       84 2023-08-01 19:26:56.000000 ovs-3.1.2/ovs.egg-info/requires.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)        4 2023-08-01 19:26:56.000000 ovs-3.1.2/ovs.egg-info/top_level.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       85 2022-04-28 18:38:11.000000 ovs-3.1.2/pyproject.toml
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2023-08-01 19:26:56.066248 ovs-3.1.2/setup.cfg
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     4350 2023-08-01 15:27:48.000000 ovs-3.1.2/setup.py
```

### Comparing `ovs-3.0.6/ovs/compat/sortedcontainers/__init__.py` & `ovs-3.1.2/ovs/compat/sortedcontainers/__init__.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/compat/sortedcontainers/sorteddict.py` & `ovs-3.1.2/ovs/compat/sortedcontainers/sorteddict.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/compat/sortedcontainers/sortedlist.py` & `ovs-3.1.2/ovs/compat/sortedcontainers/sortedlist.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/compat/sortedcontainers/sortedset.py` & `ovs-3.1.2/ovs/compat/sortedcontainers/sortedset.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/daemon.py` & `ovs-3.1.2/ovs/daemon.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/db/custom_index.py` & `ovs-3.1.2/ovs/db/custom_index.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/db/data.py` & `ovs-3.1.2/ovs/db/data.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/db/error.py` & `ovs-3.1.2/ovs/db/error.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/db/idl.py` & `ovs-3.1.2/ovs/db/idl.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,14 @@
         self.uuid = uuid.uuid1()
         self.last_id = str(uuid.UUID(int=0))
 
         # Server monitor.
         self._server_schema_request_id = None
         self._server_monitor_request_id = None
         self._db_change_aware_request_id = None
-        self._monitor_cancel_request_id = None
         self._server_db_name = '_Server'
         self._server_db_table = 'Database'
         self.server_tables = None
         self._server_db = None
         self.server_monitor_uuid = uuid.uuid1()
         self.leader_only = leader_only
         self.cluster_id = None
@@ -478,32 +477,27 @@
                                         tables=self.server_tables)
                     self.change_seqno = previous_change_seqno
                     if not self.__check_server_db():
                         self.force_reconnect()
                         break
                 else:
                     self.__parse_update(msg.params[1], OVSDB_UPDATE)
-            elif self.handle_monitor_canceled(msg):
-                break
-            elif self.handle_monitor_cancel_reply(msg):
-                break
             elif (msg.type == ovs.jsonrpc.Message.T_REPLY
                   and self._monitor_request_id is not None
                   and self._monitor_request_id == msg.id):
                 # Reply to our "monitor" request.
                 try:
                     self.change_seqno += 1
                     self._monitor_request_id = None
                     if (self.state ==
                             self.IDL_S_DATA_MONITOR_COND_SINCE_REQUESTED):
                         # If 'found' is false, clear table rows for new dump
                         if not msg.result[0]:
                             self.__clear()
                         self.__parse_update(msg.result[2], OVSDB_UPDATE3)
-                        self.last_id = msg.result[1]
                     elif self.state == self.IDL_S_DATA_MONITOR_COND_REQUESTED:
                         self.__clear()
                         self.__parse_update(msg.result, OVSDB_UPDATE2)
                     else:
                         assert self.state == self.IDL_S_DATA_MONITOR_REQUESTED
                         self.__clear()
                         self.__parse_update(msg.result, OVSDB_UPDATE)
@@ -617,41 +611,14 @@
                 # receive the reply, so keep the log level low.
                 vlog.dbg("%s: received unexpected %s message"
                          % (self._session.get_name(),
                              ovs.jsonrpc.Message.type_to_string(msg.type)))
 
         return initial_change_seqno != self.change_seqno
 
-    def handle_monitor_canceled(self, msg):
-        if msg.type != msg.T_NOTIFY:
-            return False
-        if msg.method != "monitor_canceled":
-            return False
-
-        if msg.params[0] == str(self.uuid):
-            params = [str(self.server_monitor_uuid)]
-        elif msg.params[0] == str(self.server_monitor_uuid):
-            params = [str(self.uuid)]
-        else:
-            return False
-
-        mc_msg = ovs.jsonrpc.Message.create_request("monitor_cancel", params)
-        self._monitor_cancel_request_id = mc_msg.id
-        self.send_request(mc_msg)
-        self.restart_fsm()
-        return True
-
-    def handle_monitor_cancel_reply(self, msg):
-        if msg.type != msg.T_REPLY:
-            return False
-        if msg.id != self._monitor_cancel_request_id:
-            return False
-        self._monitor_cancel_request_id = None
-        return True
-
     def compose_cond_change(self):
         if not self.cond_changed:
             return
 
         change_requests = {}
         for table in self.tables.values():
             # Always use the most recent conditions set by the IDL client when
@@ -1252,15 +1219,15 @@
         row.mycolumn["a"] = "b"              # don't do this
       will not change anything in the database, even after commit.  To modify
       the column, instead assign the modified column value back to the column:
         d = row.mycolumn
         d["a"] = "b"
         row.mycolumn = d
 """
-    def __init__(self, idl, table, uuid, data):
+    def __init__(self, idl, table, uuid, data, persist_uuid=False):
         # All of the explicit references to self.__dict__ below are required
         # to set real attributes with invoking self.__getattr__().
         self.__dict__["uuid"] = uuid
 
         self.__dict__["_idl"] = idl
         self.__dict__["_table"] = table
 
@@ -1307,14 +1274,18 @@
         self.__dict__["_mutations"] = {}
 
         # A dictionary whose keys are the names of columns that must be
         # verified as prerequisites when the transaction commits.  The values
         # in the dictionary are all None.
         self.__dict__["_prereqs"] = {}
 
+        # Indicates if the specified 'uuid' should be used as the row uuid
+        # or let the server generate it.
+        self.__dict__["_persist_uuid"] = persist_uuid
+
     def __lt__(self, other):
         if not isinstance(other, Row):
             return NotImplemented
         return bool(self.__dict__['uuid'] < other.__dict__['uuid'])
 
     def __eq__(self, other):
         if not isinstance(other, Row):
@@ -1845,15 +1816,19 @@
                 else:
                     # Let ovsdb-server decide whether to really delete it.
                     pass
             elif row._changes:
                 op = {"table": row._table.name}
                 if row._data is None:
                     op["op"] = "insert"
-                    op["uuid-name"] = _uuid_name_from_uuid(row.uuid)
+                    if row._persist_uuid:
+                        op["uuid"] = row.uuid
+                    else:
+                        op["uuid-name"] = _uuid_name_from_uuid(row.uuid)
+
                     any_updates = True
 
                     op_index = len(operations) - 1
                     self._inserted_rows[row.uuid] = _InsertedRow(op_index)
                 else:
                     op["op"] = "update"
                     op["where"] = _where_uuid_equals(row.uuid)
@@ -2085,28 +2060,30 @@
         txn._txn_rows[row.uuid] = row
         if '_inserts' in row._mutations:
             row._mutations['_inserts'].pop(column.name, None)
         if '_removes' in row._mutations:
             row._mutations['_removes'].pop(column.name, None)
         row._changes[column.name] = datum.copy()
 
-    def insert(self, table, new_uuid=None):
+    def insert(self, table, new_uuid=None, persist_uuid=False):
         """Inserts and returns a new row in 'table', which must be one of the
         ovs.db.schema.TableSchema objects in the Idl's 'tables' dict.
 
         The new row is assigned a provisional UUID.  If 'uuid' is None then one
         is randomly generated; otherwise 'uuid' should specify a randomly
-        generated uuid.UUID not otherwise in use.  ovsdb-server will assign a
-        different UUID when 'txn' is committed, but the IDL will replace any
-        uses of the provisional UUID in the data to be to be committed by the
-        UUID assigned by ovsdb-server."""
+        generated uuid.UUID not otherwise in use.  If 'persist_uuid' is true
+        and 'new_uuid' is specified, IDL requests the ovsdb-server to assign
+        the same UUID, otherwise ovsdb-server will assign a different UUID when
+        'txn' is committed and the IDL will replace any uses of the provisional
+        UUID in the data to be committed by the UUID assigned by
+        ovsdb-server."""
         assert self._status == Transaction.UNCOMMITTED
         if new_uuid is None:
             new_uuid = uuid.uuid4()
-        row = Row(self.idl, table, new_uuid, None)
+        row = Row(self.idl, table, new_uuid, None, persist_uuid=persist_uuid)
         table.rows[row.uuid] = row
         self._txn_rows[row.uuid] = row
         return row
 
     def _process_reply(self, msg):
         if msg.type == ovs.jsonrpc.Message.T_ERROR:
             self._status = Transaction.ERROR
```

### Comparing `ovs-3.0.6/ovs/db/parser.py` & `ovs-3.1.2/ovs/db/parser.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/db/schema.py` & `ovs-3.1.2/ovs/db/schema.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/db/types.py` & `ovs-3.1.2/ovs/db/types.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/dirs.py` & `ovs-3.1.2/ovs/dirs.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # The @variables@ in this file are replaced by default directories for
 # use in python/ovs/dirs.py in the source directory and replaced by the
 # configured directories for use in the installed python/ovs/dirs.py.
 #
 import os
 
 # Note that the use of """ is to aid in dealing with paths with quotes in them.
-PKGDATADIR = os.environ.get("OVS_PKGDATADIR", """/usr/local/share/openvswitch""")
-RUNDIR = os.environ.get("OVS_RUNDIR", """/usr/local/var/run/openvswitch""")
-LOGDIR = os.environ.get("OVS_LOGDIR", """/usr/local/var/log/openvswitch""")
-BINDIR = os.environ.get("OVS_BINDIR", """/usr/local/bin""")
+PKGDATADIR = os.environ.get("OVS_PKGDATADIR", """/usr/share/openvswitch""")
+RUNDIR = os.environ.get("OVS_RUNDIR", """/var/run/openvswitch""")
+LOGDIR = os.environ.get("OVS_LOGDIR", """/var/log/openvswitch""")
+BINDIR = os.environ.get("OVS_BINDIR", """/usr/bin""")
 
 DBDIR = os.environ.get("OVS_DBDIR")
 if not DBDIR:
     sysconfdir = os.environ.get("OVS_SYSCONFDIR")
     if sysconfdir:
         DBDIR = "%s/openvswitch" % sysconfdir
     else:
-        DBDIR = """/usr/local/etc/openvswitch"""
+        DBDIR = """/etc/openvswitch"""
```

### Comparing `ovs-3.0.6/ovs/fatal_signal.py` & `ovs-3.1.2/ovs/fatal_signal.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/fcntl_win.py` & `ovs-3.1.2/ovs/fcntl_win.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/flow/decoders.py` & `ovs-3.1.2/ovs/flow/decoders.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/flow/filter.py` & `ovs-3.1.2/ovs/flow/filter.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/flow/flow.py` & `ovs-3.1.2/ovs/flow/flow.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/flow/kv.py` & `ovs-3.1.2/ovs/flow/kv.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/flow/list.py` & `ovs-3.1.2/ovs/flow/list.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/flow/odp.py` & `ovs-3.1.2/ovs/flow/odp.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,14 @@
         )
 
     @staticmethod
     def _action_decoders_args():
         """Generate the arguments for the action KVDecoders."""
         _decoders = {
             "drop": decode_flag,
-            "meter": decode_int,
             "lb_output": decode_int,
             "trunc": decode_int,
             "recirc": decode_int,
             "userspace": nested_kv_decoder(
                 KVDecoders(
                     {
                         "pid": decode_int,
@@ -331,63 +330,52 @@
                         "helper": decode_default,
                         "timeout": decode_default,
                         "nat": decode_nat,
                     }
                 )
             ),
             **ODPFlow._tnl_action_decoder_args(),
-            "hash": nested_kv_decoder(
-                KVDecoders(
-                    {
-                        "l4": decode_int,
-                        "sym_l4": decode_int,
-                    }
-                )
-            ),
         }
 
-        _decoders["sample"] = nested_kv_decoder(
-            KVDecoders(
-                {
-                    "sample": (lambda x: float(x.strip("%"))),
-                    "actions": nested_kv_decoder(
-                        KVDecoders(
-                            decoders=_decoders,
-                            default_free=decode_free_output,
-                        ),
-                        is_list=True,
-                    ),
-                }
-            )
-        )
-
         _decoders["clone"] = nested_kv_decoder(
             KVDecoders(decoders=_decoders, default_free=decode_free_output),
             is_list=True,
         )
 
         return {
             **_decoders,
+            "sample": nested_kv_decoder(
+                KVDecoders(
+                    {
+                        "sample": (lambda x: float(x.strip("%"))),
+                        "actions": nested_kv_decoder(
+                            KVDecoders(
+                                decoders=_decoders,
+                                default_free=decode_free_output,
+                            ),
+                            is_list=True,
+                        ),
+                    }
+                )
+            ),
             "check_pkt_len": nested_kv_decoder(
                 KVDecoders(
                     {
                         "size": decode_int,
                         "gt": nested_kv_decoder(
                             KVDecoders(
                                 decoders=_decoders,
                                 default_free=decode_free_output,
-                            ),
-                            is_list=True,
+                            )
                         ),
                         "le": nested_kv_decoder(
                             KVDecoders(
                                 decoders=_decoders,
                                 default_free=decode_free_output,
-                            ),
-                            is_list=True,
+                            )
                         ),
                     }
                 )
             ),
         }
 
     @staticmethod
```

### Comparing `ovs-3.0.6/ovs/flow/ofp.py` & `ovs-3.1.2/ovs/flow/ofp.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,17 +100,14 @@
             no flow information but the string is expected to be found in a
             flow dump.
 
         Raises
             ValueError if the string is malformed.
             ParseError if an error in parsing occurs.
         """
-        if " reply " in ofp_string:
-            return None
-
         sections = list()
         parts = ofp_string.split("actions=")
         if len(parts) != 2:
             raise ValueError("malformed ofproto flow: %s" % ofp_string)
 
         actions = parts[1]
 
@@ -169,21 +166,20 @@
 
     @staticmethod
     def _gen_info_decoders():
         """Generate the info KVDecoders."""
         args = {
             "table": decode_int,
             "duration": decode_time,
-            "n_packets": decode_int,
+            "n_packet": decode_int,
             "n_bytes": decode_int,
             "cookie": decode_int,
             "idle_timeout": decode_time,
             "hard_timeout": decode_time,
             "hard_age": decode_time,
-            "idle_age": decode_time,
         }
         return KVDecoders(args)
 
     @staticmethod
     def _gen_match_decoders():
         """Generate the match KVDecoders."""
         args = {
@@ -399,18 +395,20 @@
         Args:
             action_decoders (dict): The decoders of the supported nested
             actions.
         """
         return {
             "learn": decode_learn(action_decoders),
             "clone": nested_kv_decoder(
-                KVDecoders(action_decoders, ignore_case=True), is_list=True
+                KVDecoders(action_decoders, default_free=decode_free_output,
+                           ignore_case=True), is_list=True
             ),
             "write_actions": nested_kv_decoder(
-                KVDecoders(action_decoders, ignore_case=True), is_list=True
+                KVDecoders(action_decoders, default_free=decode_free_output,
+                           ignore_case=True), is_list=True
             ),
         }
 
     @staticmethod
     def _other_action_decoders_args():
         """Generate the decoder arguments for other actions
         (see man(7) ovs-actions)."""
```

### Comparing `ovs-3.0.6/ovs/flow/ofp_act.py` & `ovs-3.1.2/ovs/flow/ofp_act.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     except ValueError:
         return {"port": value.strip('"')}
 
 
 def decode_controller(value):
     """Decodes the controller action."""
     if not value:
-        return KeyValue("output", "controller")
+        return KeyValue("output", {"port": "CONTROLLER"})
     else:
         # Try controller:max_len
         try:
             max_len = int(value)
             return {
                 "max_len": max_len,
             }
@@ -50,15 +50,14 @@
             KVDecoders(
                 {
                     "max_len": decode_int,
                     "reason": decode_default,
                     "id": decode_int,
                     "userdata": decode_default,
                     "pause": decode_flag,
-                    "meter_id": decode_int,
                 }
             )
         )(value)
 
 
 def decode_bundle_load(value):
     return decode_bundle(value, True)
```

### Comparing `ovs-3.0.6/ovs/flow/ofp_fields.py` & `ovs-3.1.2/ovs/flow/ofp_fields.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/json.py` & `ovs-3.1.2/ovs/json.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/jsonrpc.py` & `ovs-3.1.2/ovs/jsonrpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
 
     def __init__(self, reconnect, rpc, remotes):
         self.reconnect = reconnect
         self.rpc = rpc
         self.stream = None
         self.pstream = None
         self.seqno = 0
-        if type(remotes) is not list:
+        if type(remotes) != list:
             remotes = [remotes]
         self.remotes = remotes
         random.shuffle(self.remotes)
         self.next_remote = 0
 
     @staticmethod
     def open(name, probe_interval=None):
```

### Comparing `ovs-3.0.6/ovs/ovsuuid.py` & `ovs-3.1.2/ovs/ovsuuid.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/poller.py` & `ovs-3.1.2/ovs/poller.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/process.py` & `ovs-3.1.2/ovs/process.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/reconnect.py` & `ovs-3.1.2/ovs/reconnect.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/socket_util.py` & `ovs-3.1.2/ovs/socket_util.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/stream.py` & `ovs-3.1.2/ovs/stream.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/timeval.py` & `ovs-3.1.2/ovs/timeval.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/unixctl/__init__.py` & `ovs-3.1.2/ovs/unixctl/__init__.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/unixctl/client.py` & `ovs-3.1.2/ovs/unixctl/client.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/unixctl/server.py` & `ovs-3.1.2/ovs/unixctl/server.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/util.py` & `ovs-3.1.2/ovs/util.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/vlog.py` & `ovs-3.1.2/ovs/vlog.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs/winutils.py` & `ovs-3.1.2/ovs/winutils.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.6/ovs.egg-info/SOURCES.txt` & `ovs-3.1.2/ovs.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.rst
+pyproject.toml
 setup.py
 ovs/__init__.py
 ovs/_json.c
 ovs/daemon.py
 ovs/dirs.py
 ovs/fatal_signal.py
 ovs/fcntl_win.py
```

### Comparing `ovs-3.0.6/setup.py` & `ovs-3.1.2/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/ovs-3.0.4.tar.gz` & `tmp/ovs-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovs-3.0.4.tar", last modified: Tue Aug  1 19:22:37 2023, max compression
+gzip compressed data, was "ovs-3.1.2.tar", last modified: Tue Aug  1 19:26:56 2023, max compression
```

## Comparing `ovs-3.0.4.tar` & `ovs-3.1.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.230654 ovs-3.0.4/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)      670 2023-08-01 19:22:37.229654 ovs-3.0.4/PKG-INFO
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       45 2021-09-20 16:15:26.000000 ovs-3.0.4/README.rst
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.226654 ovs-3.0.4/ovs/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/__init__.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     7038 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/_json.c
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.226654 ovs-3.0.4/ovs/compat/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)        0 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/compat/__init__.py
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.227654 ovs-3.0.4/ovs/compat/sortedcontainers/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     2131 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/compat/sortedcontainers/__init__.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    22712 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/compat/sortedcontainers/sorteddict.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    76293 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/compat/sortedcontainers/sortedlist.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    19825 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/compat/sortedcontainers/sortedset.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    20710 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/daemon.py
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.228654 ovs-3.0.4/ovs/db/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/db/__init__.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     4856 2021-11-05 13:35:58.000000 ovs-3.0.4/ovs/db/custom_index.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    21659 2023-06-14 20:52:13.000000 ovs-3.0.4/ovs/db/data.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1156 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/db/error.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    96817 2023-08-01 18:54:03.000000 ovs-3.0.4/ovs/db/idl.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     3647 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/db/parser.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    11947 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/db/schema.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    23240 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/db/types.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1329 2023-08-01 18:44:12.000000 ovs-3.0.4/ovs/dirs.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     4765 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/fatal_signal.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1330 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/fcntl_win.py
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.229654 ovs-3.0.4/ovs/flow/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)      476 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/flow/__init__.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    14382 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/flow/decoders.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     7502 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/flow/filter.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     3772 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/flow/flow.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    10505 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/flow/kv.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     3819 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/flow/list.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    27561 2023-08-01 18:54:03.000000 ovs-3.0.4/ovs/flow/odp.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    13396 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/flow/ofp.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     8786 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/flow/ofp_act.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     7348 2023-08-01 18:55:30.000000 ovs-3.0.4/ovs/flow/ofp_fields.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    16843 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/json.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    21087 2023-04-18 01:01:46.000000 ovs-3.0.4/ovs/jsonrpc.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1869 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/ovsuuid.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    10282 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/poller.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1467 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/process.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    26007 2023-05-17 03:37:46.000000 ovs-3.0.4/ovs/reconnect.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    11976 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/socket_util.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    32107 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/stream.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     2432 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/timeval.py
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.229654 ovs-3.0.4/ovs/unixctl/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     3032 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/unixctl/__init__.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1999 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/unixctl/client.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     8121 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/unixctl/server.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     3120 2022-09-19 19:15:14.000000 ovs-3.0.4/ovs/util.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       93 2023-08-01 18:55:30.000000 ovs-3.0.4/ovs/version.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    16694 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/vlog.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     9226 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/winutils.py
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.226654 ovs-3.0.4/ovs.egg-info/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)      670 2023-08-01 19:22:37.000000 ovs-3.0.4/ovs.egg-info/PKG-INFO
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1028 2023-08-01 19:22:37.000000 ovs-3.0.4/ovs.egg-info/SOURCES.txt
--rw-rw-r--   0 twilson   (1000) twilson   (1000)        1 2023-08-01 19:22:37.000000 ovs-3.0.4/ovs.egg-info/dependency_links.txt
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       84 2023-08-01 19:22:37.000000 ovs-3.0.4/ovs.egg-info/requires.txt
--rw-rw-r--   0 twilson   (1000) twilson   (1000)        4 2023-08-01 19:22:37.000000 ovs-3.0.4/ovs.egg-info/top_level.txt
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       85 2022-04-28 18:38:11.000000 ovs-3.0.4/pyproject.toml
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2023-08-01 19:22:37.230654 ovs-3.0.4/setup.cfg
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     4350 2023-08-01 15:27:48.000000 ovs-3.0.4/setup.py
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

### Comparing `ovs-3.0.4/PKG-INFO` & `ovs-3.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovs
-Version: 3.0.4
+Version: 3.1.2
 Summary: Open vSwitch library
 Home-page: http://www.openvswitch.org/
 Author: Open vSwitch
 Author-email: dev@openvswitch.org
 License: Apache 2.0
 Keywords: openvswitch,ovs,OVSDB
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ovs-3.0.4/ovs/compat/sortedcontainers/__init__.py` & `ovs-3.1.2/ovs/compat/sortedcontainers/__init__.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/compat/sortedcontainers/sorteddict.py` & `ovs-3.1.2/ovs/compat/sortedcontainers/sorteddict.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/compat/sortedcontainers/sortedlist.py` & `ovs-3.1.2/ovs/compat/sortedcontainers/sortedlist.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/compat/sortedcontainers/sortedset.py` & `ovs-3.1.2/ovs/compat/sortedcontainers/sortedset.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/daemon.py` & `ovs-3.1.2/ovs/daemon.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/db/custom_index.py` & `ovs-3.1.2/ovs/db/custom_index.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/db/data.py` & `ovs-3.1.2/ovs/db/data.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/db/error.py` & `ovs-3.1.2/ovs/db/error.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/db/idl.py` & `ovs-3.1.2/ovs/db/idl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1219,15 +1219,15 @@
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
 
@@ -1274,14 +1274,18 @@
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
@@ -1812,15 +1816,19 @@
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
@@ -2052,28 +2060,30 @@
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

### Comparing `ovs-3.0.4/ovs/db/parser.py` & `ovs-3.1.2/ovs/db/parser.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/db/schema.py` & `ovs-3.1.2/ovs/db/schema.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/db/types.py` & `ovs-3.1.2/ovs/db/types.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/dirs.py` & `ovs-3.1.2/ovs/dirs.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/fatal_signal.py` & `ovs-3.1.2/ovs/fatal_signal.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/fcntl_win.py` & `ovs-3.1.2/ovs/fcntl_win.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/flow/decoders.py` & `ovs-3.1.2/ovs/flow/decoders.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/flow/filter.py` & `ovs-3.1.2/ovs/flow/filter.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/flow/flow.py` & `ovs-3.1.2/ovs/flow/flow.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/flow/kv.py` & `ovs-3.1.2/ovs/flow/kv.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,58 +81,81 @@
 
     The decoder to be used will be selected using the key as an index. If not
     found, the default decoder will be used. If free keys are found (i.e:
     keys without a value), the default_free decoder will be used. For that
     reason, the default_free decoder, must return both the key and value to be
     stored.
 
+    Globally defined "strict" variable controls what to do when decoders do not
+    contain a valid decoder for a key and a default function is not provided.
+    If set to True (default), a ParseError is raised.
+    If set to False, the value will be decoded as a string.
+
     Args:
         decoders (dict): Optional; A dictionary of decoders indexed by keyword.
-        default (callable): Optional; A decoder used if a match is not found in
-            configured decoders. If not provided, the default behavior is to
-            try to decode the value into an integer and, if that fails,
-            just return the string as-is.
+        default (callable): Optional; A function to use if a match is not
+            found in configured decoders. If not provided, the default behavior
+            depends on "strict". The function must accept a the key and a value
+            and return the decoded (key, value) tuple back.
         default_free (callable): Optional; The decoder used if a match is not
             found in configured decoders and it's a free value (e.g:
             a value without a key) Defaults to returning the free value as
             keyword and "True" as value.
             The callable must accept a string and return a key-value pair.
     """
 
-    def __init__(self, decoders=None, default=None, default_free=None):
-        self._decoders = decoders or dict()
-        self._default = default or decode_default
+    strict = True
+
+    def __init__(self, decoders=None, default=None, default_free=None,
+                 ignore_case=False):
+        if not decoders:
+            self._decoders = dict()
+        elif ignore_case:
+            self._decoders = {k.lower(): v for k, v in decoders.items()}
+        else:
+            self._decoders = decoders
+        self._default = default
         self._default_free = default_free or self._default_free_decoder
+        self._ignore_case = ignore_case
 
     def decode(self, keyword, value_str):
         """Decode a keyword and value.
 
         Args:
             keyword (str): The keyword whose value is to be decoded.
             value_str (str): The value string.
 
         Returns:
             The key (str) and value(any) to be stored.
         """
 
-        decoder = self._decoders.get(keyword)
+        decoder = None
+        if self._ignore_case:
+            decoder = self._decoders.get(keyword.lower())
+        else:
+            decoder = self._decoders.get(keyword)
         if decoder:
             result = decoder(value_str)
             if isinstance(result, KeyValue):
                 keyword = result.key
                 value = result.value
             else:
                 value = result
 
             return keyword, value
         else:
             if value_str:
-                return keyword, self._default(value_str)
-            else:
-                return self._default_free(keyword)
+                if self._default:
+                    return self._default(keyword, value_str)
+                if self.strict:
+                    raise ParseError(
+                        "Cannot parse key {}: No decoder found".format(keyword)
+                    )
+                return keyword, decode_default(value_str)
+            return self._default_free(keyword)
 
     @staticmethod
     def _default_free_decoder(key):
         """Default decoder for free keywords."""
         return key, True
 
 
@@ -304,11 +327,30 @@
         return True
 
     parser = KVParser(value, decoders)
     parser.parse()
     return {kv.key: kv.value for kv in parser.kv()}
 
 
-def nested_kv_decoder(decoders=None):
+def decode_nested_kv_list(decoders, value):
+    """A key-value decoder that extracts nested key-value pairs and returns
+    them in a list of dictionary.
+
+    Args:
+        decoders (KVDecoders): The KVDecoders to use.
+        value (str): The value string to decode.
+    """
+    if not value:
+        # Mark as flag
+        return True
+
+    parser = KVParser(value, decoders)
+    parser.parse()
+    return [{kv.key: kv.value} for kv in parser.kv()]
+
+
+def nested_kv_decoder(decoders=None, is_list=False):
     """Helper function that creates a nested kv decoder with given
     KVDecoders."""
+    if is_list:
+        return functools.partial(decode_nested_kv_list, decoders)
     return functools.partial(decode_nested_kv, decoders)
```

### Comparing `ovs-3.0.4/ovs/flow/list.py` & `ovs-3.1.2/ovs/flow/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,20 @@
         """Decode the index'th element of the list.
 
         Args:
             index (int): The position in the list of the element to decode.
             value_str (str): The value string to decode.
         """
         if index < 0 or index >= len(self._decoders):
-            return self._default_decoder(index, value_str)
+            if self._default_decoder:
+                return self._default_decoder(index, value_str)
+            else:
+                raise ParseError(
+                    f"Cannot decode element {index} in list: {value_str}"
+                )
 
         try:
             key = self._decoders[index][0]
             value = self._decoders[index][1](value_str)
             return key, value
         except Exception as e:
             raise ParseError(
```

### Comparing `ovs-3.0.4/ovs/flow/odp.py` & `ovs-3.1.2/ovs/flow/odp.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,28 +333,30 @@
                     }
                 )
             ),
             **ODPFlow._tnl_action_decoder_args(),
         }
 
         _decoders["clone"] = nested_kv_decoder(
-            KVDecoders(decoders=_decoders, default_free=decode_free_output)
+            KVDecoders(decoders=_decoders, default_free=decode_free_output),
+            is_list=True,
         )
 
         return {
             **_decoders,
             "sample": nested_kv_decoder(
                 KVDecoders(
                     {
                         "sample": (lambda x: float(x.strip("%"))),
                         "actions": nested_kv_decoder(
                             KVDecoders(
                                 decoders=_decoders,
                                 default_free=decode_free_output,
-                            )
+                            ),
+                            is_list=True,
                         ),
                     }
                 )
             ),
             "check_pkt_len": nested_kv_decoder(
                 KVDecoders(
                     {
```

### Comparing `ovs-3.0.4/ovs/flow/ofp.py` & `ovs-3.1.2/ovs/flow/ofp.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     decode_encap,
     decode_load_field,
     decode_set_field,
     decode_move_field,
     decode_dec_ttl,
     decode_chk_pkt_larger,
     decode_zone,
-    decode_exec,
     decode_learn,
 )
 
 
 class OFPFlow(Flow):
     """OFPFLow represents an OpenFlow Flow.
 
@@ -101,17 +100,14 @@
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
 
@@ -239,18 +235,20 @@
             **OFPFlow._output_actions_decoders_args(),
             **OFPFlow._encap_actions_decoders_args(),
             **OFPFlow._field_action_decoders_args(),
             **OFPFlow._meta_action_decoders_args(),
             **OFPFlow._fw_action_decoders_args(),
             **OFPFlow._control_action_decoders_args(),
             **OFPFlow._other_action_decoders_args(),
+            **OFPFlow._instruction_action_decoders_args(),
         }
         clone_actions = OFPFlow._clone_actions_decoders_args(actions)
         actions.update(clone_actions)
-        return KVDecoders(actions, default_free=decode_free_output)
+        return KVDecoders(actions, default_free=decode_free_output,
+                          ignore_case=True)
 
     @staticmethod
     def _output_actions_decoders_args():
         """Returns the decoder arguments for the output actions."""
         return {
             "output": decode_output,
             "drop": decode_flag,
@@ -268,44 +266,52 @@
     def _encap_actions_decoders_args():
         """Returns the decoders arguments for the encap actions."""
 
         return {
             "pop_vlan": decode_flag,
             "strip_vlan": decode_flag,
             "push_vlan": decode_default,
+            "pop_mpls": decode_int,
+            "push_mpls": decode_int,
             "decap": decode_flag,
             "encap": decode_encap,
         }
 
     @staticmethod
     def _field_action_decoders_args():
         """Returns the decoders arguments for field-modification actions."""
         # Field modification actions
         field_default_decoders = [
             "set_mpls_label",
             "set_mpls_tc",
             "set_mpls_ttl",
             "mod_nw_tos",
             "mod_nw_ecn",
-            "mod_tcp_src",
-            "mod_tcp_dst",
+            "mod_tp_src",
+            "mod_tp_dst",
         ]
         return {
             "load": decode_load_field,
             "set_field": functools.partial(
                 decode_set_field, KVDecoders(OFPFlow._field_decoder_args())
             ),
             "move": decode_move_field,
             "mod_dl_dst": EthMask,
             "mod_dl_src": EthMask,
             "mod_nw_dst": IPMask,
             "mod_nw_src": IPMask,
+            "mod_nw_ttl": decode_int,
+            "mod_vlan_vid": decode_int,
+            "set_vlan_vid": decode_int,
+            "mod_vlan_pcp": decode_int,
+            "set_vlan_pcp": decode_int,
             "dec_ttl": decode_dec_ttl,
             "dec_mpls_ttl": decode_flag,
             "dec_nsh_ttl": decode_flag,
+            "delete_field": decode_field,
             "check_pkt_larger": decode_chk_pkt_larger,
             **{field: decode_default for field in field_default_decoders},
         }
 
     @staticmethod
     def _meta_action_decoders_args():
         """Returns the decoders arguments for the metadata actions."""
@@ -323,29 +329,38 @@
                 KVDecoders(
                     {
                         "commit": decode_flag,
                         "zone": decode_zone,
                         "table": decode_int,
                         "nat": decode_nat,
                         "force": decode_flag,
-                        "exec": functools.partial(
-                            decode_exec,
+                        "exec": nested_kv_decoder(
                             KVDecoders(
                                 {
                                     **OFPFlow._encap_actions_decoders_args(),
                                     **OFPFlow._field_action_decoders_args(),
                                     **OFPFlow._meta_action_decoders_args(),
                                 }
                             ),
+                            is_list=True,
                         ),
                         "alg": decode_default,
                     }
                 )
             ),
             "ct_clear": decode_flag,
+            "fin_timeout": nested_kv_decoder(
+                KVDecoders(
+                    {
+                        "idle_timeout": decode_time,
+                        "hard_timeout": decode_time,
+                    }
+                )
+            ),
+            # learn moved to _clone actions.
         }
 
     @staticmethod
     def _control_action_decoders_args():
         return {
             "resubmit": nested_list_decoder(
                 ListDecoders(
@@ -378,29 +393,22 @@
         """Generate the decoder arguments for the clone actions.
 
         Args:
             action_decoders (dict): The decoders of the supported nested
             actions.
         """
         return {
-            "learn": decode_learn(
-                {
-                    **action_decoders,
-                    "fin_timeout": nested_kv_decoder(
-                        KVDecoders(
-                            {
-                                "idle_timeout": decode_time,
-                                "hard_timeout": decode_time,
-                            }
-                        )
-                    ),
-                }
+            "learn": decode_learn(action_decoders),
+            "clone": nested_kv_decoder(
+                KVDecoders(action_decoders, default_free=decode_free_output,
+                           ignore_case=True), is_list=True
             ),
-            "clone": functools.partial(
-                decode_exec, KVDecoders(action_decoders)
+            "write_actions": nested_kv_decoder(
+                KVDecoders(action_decoders, default_free=decode_free_output,
+                           ignore_case=True), is_list=True
             ),
         }
 
     @staticmethod
     def _other_action_decoders_args():
         """Generate the decoder arguments for other actions
         (see man(7) ovs-actions)."""
@@ -422,7 +430,19 @@
                         "sampling_port": decode_default,
                         "ingress": decode_flag,
                         "egress": decode_flag,
                     }
                 )
             ),
         }
+
+    @staticmethod
+    def _instruction_action_decoders_args():
+        """Generate the decoder arguments for instruction actions
+        (see man(7) ovs-actions)."""
+        return {
+            "meter": decode_int,
+            "clear_actions": decode_flag,
+            # write_actions moved to _clone actions
+            "write_metadata": decode_mask(64),
+            "goto_table": decode_int,
+        }
```

### Comparing `ovs-3.0.4/ovs/flow/ofp_act.py` & `ovs-3.1.2/ovs/flow/ofp_act.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,66 @@
 """Defines decoders for OpenFlow actions.
 """
-
-import functools
-
 from ovs.flow.decoders import (
     decode_default,
     decode_time,
     decode_flag,
     decode_int,
 )
-from ovs.flow.kv import nested_kv_decoder, KVDecoders, KeyValue, KVParser
+from ovs.flow.kv import (
+    nested_kv_decoder,
+    KVDecoders,
+    KeyValue,
+    KVParser,
+    ParseError,
+)
 from ovs.flow.list import nested_list_decoder, ListDecoders
-from ovs.flow.ofp_fields import field_decoders
+from ovs.flow.ofp_fields import field_decoders, field_aliases
 
 
 def decode_output(value):
     """Decodes the output value.
 
     Does not support field specification.
     """
     if len(value.split(",")) > 1:
-        return nested_kv_decoder()(value)
+        return nested_kv_decoder(
+            KVDecoders({"port": decode_default, "max_len": decode_int})
+        )(value)
     try:
         return {"port": int(value)}
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
         except ValueError:
             pass
         # controller(key[=val], ...)
-        return nested_kv_decoder()(value)
+        return nested_kv_decoder(
+            KVDecoders(
+                {
+                    "max_len": decode_int,
+                    "reason": decode_default,
+                    "id": decode_int,
+                    "userdata": decode_default,
+                    "pause": decode_flag,
+                }
+            )
+        )(value)
 
 
 def decode_bundle_load(value):
     return decode_bundle(value, True)
 
 
 def decode_bundle(value, load=False):
@@ -137,14 +152,20 @@
 
 
 def decode_field(value):
     """Decodes a field as defined in the 'Field Specification' of the actions
     man page:
     http://www.openvswitch.org/support/dist-docs/ovs-actions.7.txt."""
     parts = value.strip("]\n\r").split("[")
+    if (
+        parts[0] not in field_decoders.keys()
+        and parts[0] not in field_aliases.keys()
+    ):
+        raise ParseError("Field not supported: {}".format(parts[0]))
+
     result = {
         "field": parts[0],
     }
 
     if len(parts) > 1 and parts[1]:
         field_range = parts[1].split("..")
         start = field_range[0]
@@ -230,27 +251,14 @@
     try:
         return int(value, 0)
     except ValueError:
         pass
     return decode_field(value)
 
 
-def decode_exec(action_decoders, value):
-    """Decodes the value of the 'exec' keyword (part of the ct action).
-
-    Args:
-        decode_actions (KVDecoders): The decoders to be used to decode the
-            nested exec.
-        value (string): The string to be decoded.
-    """
-    exec_parser = KVParser(value, action_decoders)
-    exec_parser.parse()
-    return [{kv.key: kv.value} for kv in exec_parser.kv()]
-
-
 def decode_learn(action_decoders):
     """Create the decoder to be used to decode the 'learn' action.
 
     The learn action has two added complexities:
     1) It can hold any valid action key-value. Therefore we must take
     the precalculated action_decoders and use them. That's why we require
     them as argument.
@@ -265,42 +273,53 @@
     process.
 
     Args:
         action_decoders (dict): Dictionary of decoders to be used in nested
             action decoding.
     """
 
-    def decode_learn_field(decoder, value):
-        """Generates a decoder to be used for the 'field' argument of the
-        'learn' action.
-
-        The field can hold a value that should be decoded, either as a field,
-        or as a the value (see man(7) ovs-actions).
-
-        Args:
-            decoder (callable): The decoder.
+    def learn_field_decoding_kv(key, value):
+        """Decodes a key, value pair from the learn action.
+        The key must be a decodable field. The value can be either a value
+        in the format defined for the field or another field.
         """
-        if value in field_decoders.keys():
-            # It's a field
-            return value
-        else:
-            return decoder(value)
-
-    learn_field_decoders = {
-        field: functools.partial(decode_learn_field, decoder)
-        for field, decoder in field_decoders.items()
-    }
+        key_field = decode_field(key)
+        try:
+            return key, decode_field(value)
+        except ParseError:
+            return key, field_decoders.get(key_field.get("field"))(value)
+
+    def learn_field_decoding_free(key):
+        """Decodes the free fields found in the learn action.
+        Free fields indicate that the filed is to be copied from the original.
+        In order to express that in a dictionary, return the fieldspec as
+        value. So, the free fild NXM_OF_IP_SRC[], is encoded as:
+            "NXM_OF_IP_SRC[]": {
+                "field": "NXM_OF_IP_SRC"
+            }
+        That way we also ensure the actual free key is correct.
+        """
+        key_field = decode_field(key)
+        return key, key_field
+
     learn_decoders = {
         **action_decoders,
-        **learn_field_decoders,
         "idle_timeout": decode_time,
         "hard_timeout": decode_time,
+        "fin_idle_timeout": decode_time,
+        "fin_hard_timeout": decode_time,
         "priority": decode_int,
         "cookie": decode_int,
         "send_flow_rem": decode_flag,
         "table": decode_int,
         "delete_learned": decode_flag,
         "limit": decode_int,
         "result_dst": decode_field,
     }
 
-    return functools.partial(decode_exec, KVDecoders(learn_decoders))
+    learn_decoder = KVDecoders(
+        learn_decoders,
+        default=learn_field_decoding_kv,
+        default_free=learn_field_decoding_free,
+    )
+
+    return nested_kv_decoder(learn_decoder, is_list=True)
```

### Comparing `ovs-3.0.4/ovs/json.py` & `ovs-3.1.2/ovs/json.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/jsonrpc.py` & `ovs-3.1.2/ovs/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/ovsuuid.py` & `ovs-3.1.2/ovs/ovsuuid.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/poller.py` & `ovs-3.1.2/ovs/poller.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/process.py` & `ovs-3.1.2/ovs/process.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/reconnect.py` & `ovs-3.1.2/ovs/reconnect.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/socket_util.py` & `ovs-3.1.2/ovs/socket_util.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/stream.py` & `ovs-3.1.2/ovs/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -820,15 +820,16 @@
             return retval
 
         # TCP Connection is successful. Now do the SSL handshake
         try:
             self.socket.do_handshake()
         except ssl.SSLWantReadError:
             return errno.EAGAIN
-        except ssl.SSLSyscallError as e:
+        except (ssl.SSLSyscallError, ssl.SSLZeroReturnError,
+                ssl.SSLEOFError, OSError) as e:
             return ovs.socket_util.get_exception_errno(e)
 
         return 0
 
     def recv(self, n):
         try:
             return super(SSLStream, self)._recv(n)
```

### Comparing `ovs-3.0.4/ovs/timeval.py` & `ovs-3.1.2/ovs/timeval.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/unixctl/__init__.py` & `ovs-3.1.2/ovs/unixctl/__init__.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/unixctl/client.py` & `ovs-3.1.2/ovs/unixctl/client.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/unixctl/server.py` & `ovs-3.1.2/ovs/unixctl/server.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/util.py` & `ovs-3.1.2/ovs/util.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/vlog.py` & `ovs-3.1.2/ovs/vlog.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs/winutils.py` & `ovs-3.1.2/ovs/winutils.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/ovs.egg-info/PKG-INFO` & `ovs-3.1.2/ovs.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovs
-Version: 3.0.4
+Version: 3.1.2
 Summary: Open vSwitch library
 Home-page: http://www.openvswitch.org/
 Author: Open vSwitch
 Author-email: dev@openvswitch.org
 License: Apache 2.0
 Keywords: openvswitch,ovs,OVSDB
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ovs-3.0.4/ovs.egg-info/SOURCES.txt` & `ovs-3.1.2/ovs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovs-3.0.4/setup.py` & `ovs-3.1.2/setup.py`

 * *Files identical despite different names*


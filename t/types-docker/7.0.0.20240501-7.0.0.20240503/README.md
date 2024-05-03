# Comparing `tmp/types-docker-7.0.0.20240501.tar.gz` & `tmp/types-docker-7.0.0.20240503.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-docker-7.0.0.20240501.tar", last modified: Wed May  1 02:22:52 2024, max compression
+gzip compressed data, was "types-docker-7.0.0.20240503.tar", last modified: Fri May  3 02:20:42 2024, max compression
```

## Comparing `types-docker-7.0.0.20240501.tar` & `types-docker-7.0.0.20240503.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:52.983876 types-docker-7.0.0.20240501/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-01 02:22:52.000000 types-docker-7.0.0.20240501/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 02:22:52.000000 types-docker-7.0.0.20240501/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-01 02:22:52.983876 types-docker-7.0.0.20240501/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:52.975876 types-docker-7.0.0.20240501/docker-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-01 02:22:52.000000 types-docker-7.0.0.20240501/docker-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:52.975876 types-docker-7.0.0.20240501/docker-stubs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/container.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/exec_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/image.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/network.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/secret.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/api/volume.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:52.975876 types-docker-7.0.0.20240501/docker-stubs/context/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/context/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/context/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/context/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/context/context.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:52.979876 types-docker-7.0.0.20240501/docker-stubs/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/credentials/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/credentials/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/credentials/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/credentials/store.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/credentials/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/errors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:52.979876 types-docker-7.0.0.20240501/docker-stubs/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/configs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/images.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/secrets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/models/volumes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:52.000000 types-docker-7.0.0.20240501/docker-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/tls.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:52.979876 types-docker-7.0.0.20240501/docker-stubs/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/transport/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/transport/basehttpadapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/transport/npipeconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/transport/npipesocket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/transport/sshconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/transport/unixconn.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:52.983876 types-docker-7.0.0.20240501/docker-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/types/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/types/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/types/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/types/healthcheck.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/types/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/types/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/types/swarm.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:52.983876 types-docker-7.0.0.20240501/docker-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/utils/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/utils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/utils/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/utils/fnmatch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/utils/json_stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/utils/ports.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/utils/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/utils/socket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/utils/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 02:22:35.000000 types-docker-7.0.0.20240501/docker-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 02:22:52.983876 types-docker-7.0.0.20240501/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-01 02:22:52.000000 types-docker-7.0.0.20240501/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:22:52.983876 types-docker-7.0.0.20240501/types_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-01 02:22:52.000000 types-docker-7.0.0.20240501/types_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-01 02:22:52.000000 types-docker-7.0.0.20240501/types_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 02:22:52.000000 types-docker-7.0.0.20240501/types_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 02:22:52.000000 types-docker-7.0.0.20240501/types_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 02:22:52.000000 types-docker-7.0.0.20240501/types_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.558845 types-docker-7.0.0.20240503/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-03 02:20:40.000000 types-docker-7.0.0.20240503/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 02:20:40.000000 types-docker-7.0.0.20240503/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-03 02:20:42.558845 types-docker-7.0.0.20240503/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.546844 types-docker-7.0.0.20240503/docker-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 02:20:40.000000 types-docker-7.0.0.20240503/docker-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.550844 types-docker-7.0.0.20240503/docker-stubs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/container.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/exec_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/network.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/secret.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/volume.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.550844 types-docker-7.0.0.20240503/docker-stubs/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/context/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/context/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/context/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/context/context.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.550844 types-docker-7.0.0.20240503/docker-stubs/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/credentials/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/credentials/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/credentials/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/credentials/store.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/credentials/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/errors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.554844 types-docker-7.0.0.20240503/docker-stubs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/configs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/secrets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/volumes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:40.000000 types-docker-7.0.0.20240503/docker-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/tls.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.554844 types-docker-7.0.0.20240503/docker-stubs/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/basehttpadapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/npipeconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/npipesocket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/sshconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/unixconn.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.554844 types-docker-7.0.0.20240503/docker-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/healthcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/swarm.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.558845 types-docker-7.0.0.20240503/docker-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/fnmatch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/json_stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/ports.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/socket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:20:42.558845 types-docker-7.0.0.20240503/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-03 02:20:40.000000 types-docker-7.0.0.20240503/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.558845 types-docker-7.0.0.20240503/types_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-03 02:20:42.000000 types-docker-7.0.0.20240503/types_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-03 02:20:42.000000 types-docker-7.0.0.20240503/types_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:20:42.000000 types-docker-7.0.0.20240503/types_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 02:20:42.000000 types-docker-7.0.0.20240503/types_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 02:20:42.000000 types-docker-7.0.0.20240503/types_docker.egg-info/top_level.txt
```

### Comparing `types-docker-7.0.0.20240501/PKG-INFO` & `types-docker-7.0.0.20240503/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240501
+Version: 7.0.0.20240503
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2ac3ad9fcd788c28854a08ca895c8d713d6cc8be` and was tested
-with mypy 1.10.0, pyright 1.1.360, and
+This package was generated from typeshed commit `8c0fc298c53b7e74fe3aad431aa4cfe3772170b3` and was tested
+with mypy 1.10.0, pyright 1.1.361, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240501/docker-stubs/api/build.pyi` & `types-docker-7.0.0.20240503/docker-stubs/api/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/api/client.pyi` & `types-docker-7.0.0.20240503/docker-stubs/api/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/api/container.pyi` & `types-docker-7.0.0.20240503/docker-stubs/api/container.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/api/daemon.pyi` & `types-docker-7.0.0.20240503/docker-stubs/api/daemon.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/api/exec_api.pyi` & `types-docker-7.0.0.20240503/docker-stubs/api/exec_api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/api/image.pyi` & `types-docker-7.0.0.20240503/docker-stubs/api/image.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/api/network.pyi` & `types-docker-7.0.0.20240503/docker-stubs/api/network.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/api/plugin.pyi` & `types-docker-7.0.0.20240503/docker-stubs/api/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/api/service.pyi` & `types-docker-7.0.0.20240503/docker-stubs/api/service.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/api/swarm.pyi` & `types-docker-7.0.0.20240503/docker-stubs/api/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/api/volume.pyi` & `types-docker-7.0.0.20240503/docker-stubs/api/volume.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/auth.pyi` & `types-docker-7.0.0.20240503/docker-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/client.pyi` & `types-docker-7.0.0.20240503/docker-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/constants.pyi` & `types-docker-7.0.0.20240503/docker-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/context/api.pyi` & `types-docker-7.0.0.20240503/docker-stubs/context/api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/context/context.pyi` & `types-docker-7.0.0.20240503/docker-stubs/context/context.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/errors.pyi` & `types-docker-7.0.0.20240503/docker-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/models/containers.pyi` & `types-docker-7.0.0.20240503/docker-stubs/models/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/models/images.pyi` & `types-docker-7.0.0.20240503/docker-stubs/models/images.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from _typeshed import Incomplete
+from collections.abc import Generator
+from typing import Any
 
 from .resource import Collection, Model
 
 class Image(Model):
     @property
     def labels(self): ...
     @property
@@ -24,15 +26,15 @@
     def pull(self, platform: Incomplete | None = None): ...
     def has_platform(self, platform): ...
     attrs: Incomplete
     def reload(self) -> None: ...
 
 class ImageCollection(Collection):
     model: type[Image]
-    def build(self, **kwargs): ...
+    def build(self, **kwargs) -> tuple[Image, Generator[Any, None, None]]: ...
     def get(self, name): ...
     def get_registry_data(self, name, auth_config: Incomplete | None = None): ...
     def list(self, name: Incomplete | None = None, all: bool = False, filters: Incomplete | None = None): ...
     def load(self, data): ...
     def pull(self, repository, tag: str | None = None, all_tags: bool = False, **kwargs): ...
     def push(self, repository, tag: str | None = None, **kwargs): ...
     def remove(self, *args, **kwargs) -> None: ...
```

### Comparing `types-docker-7.0.0.20240501/docker-stubs/models/networks.pyi` & `types-docker-7.0.0.20240503/docker-stubs/models/networks.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/models/plugins.pyi` & `types-docker-7.0.0.20240503/docker-stubs/models/plugins.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/models/resource.pyi` & `types-docker-7.0.0.20240503/docker-stubs/models/resource.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/models/services.pyi` & `types-docker-7.0.0.20240503/docker-stubs/models/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/models/swarm.pyi` & `types-docker-7.0.0.20240503/docker-stubs/models/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/transport/npipeconn.pyi` & `types-docker-7.0.0.20240503/docker-stubs/transport/npipeconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/transport/npipesocket.pyi` & `types-docker-7.0.0.20240503/docker-stubs/transport/npipesocket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/transport/sshconn.pyi` & `types-docker-7.0.0.20240503/docker-stubs/transport/sshconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/transport/unixconn.pyi` & `types-docker-7.0.0.20240503/docker-stubs/transport/unixconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/types/__init__.pyi` & `types-docker-7.0.0.20240503/docker-stubs/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/types/containers.pyi` & `types-docker-7.0.0.20240503/docker-stubs/types/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/types/healthcheck.pyi` & `types-docker-7.0.0.20240503/docker-stubs/types/healthcheck.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/types/networks.pyi` & `types-docker-7.0.0.20240503/docker-stubs/types/networks.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/types/services.pyi` & `types-docker-7.0.0.20240503/docker-stubs/types/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/types/swarm.pyi` & `types-docker-7.0.0.20240503/docker-stubs/types/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/utils/__init__.pyi` & `types-docker-7.0.0.20240503/docker-stubs/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/utils/build.pyi` & `types-docker-7.0.0.20240503/docker-stubs/utils/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/utils/proxy.pyi` & `types-docker-7.0.0.20240503/docker-stubs/utils/proxy.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/utils/socket.pyi` & `types-docker-7.0.0.20240503/docker-stubs/utils/socket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/docker-stubs/utils/utils.pyi` & `types-docker-7.0.0.20240503/docker-stubs/utils/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240501/setup.py` & `types-docker-7.0.0.20240503/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2ac3ad9fcd788c28854a08ca895c8d713d6cc8be` and was tested
-with mypy 1.10.0, pyright 1.1.360, and
+This package was generated from typeshed commit `8c0fc298c53b7e74fe3aad431aa4cfe3772170b3` and was tested
+with mypy 1.10.0, pyright 1.1.361, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="7.0.0.20240501",
+      version="7.0.0.20240503",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md",
```

### Comparing `types-docker-7.0.0.20240501/types_docker.egg-info/PKG-INFO` & `types-docker-7.0.0.20240503/types_docker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240501
+Version: 7.0.0.20240503
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2ac3ad9fcd788c28854a08ca895c8d713d6cc8be` and was tested
-with mypy 1.10.0, pyright 1.1.360, and
+This package was generated from typeshed commit `8c0fc298c53b7e74fe3aad431aa4cfe3772170b3` and was tested
+with mypy 1.10.0, pyright 1.1.361, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240501/types_docker.egg-info/SOURCES.txt` & `types-docker-7.0.0.20240503/types_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*


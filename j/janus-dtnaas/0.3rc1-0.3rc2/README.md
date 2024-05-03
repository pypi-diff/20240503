# Comparing `tmp/janus-dtnaas-0.3rc1.tar.gz` & `tmp/janus_dtnaas-0.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus-dtnaas-0.3rc1.tar", last modified: Tue Mar 12 21:13:09 2024, max compression
+gzip compressed data, was "janus_dtnaas-0.3rc2.tar", last modified: Fri May  3 17:32:31 2024, max compression
```

## Comparing `janus-dtnaas-0.3rc1.tar` & `janus_dtnaas-0.3rc2.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.882915 janus-dtnaas-0.3rc1/
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1513 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/LICENSE
--rw-r--r--   0 ezra      (1000) ezra      (1000)       41 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/MANIFEST.in
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2641 2024-03-12 21:13:09.882915 janus-dtnaas-0.3rc1/PKG-INFO
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1514 2023-11-06 16:43:03.000000 janus-dtnaas-0.3rc1/README.md
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.878915 janus-dtnaas-0.3rc1/janus/
--rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2021-10-13 19:48:34.000000 janus-dtnaas-0.3rc1/janus/__init__.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)       24 2021-10-13 19:48:34.000000 janus-dtnaas-0.3rc1/janus/agent_settings.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.878915 janus-dtnaas-0.3rc1/janus/api/
--rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/janus/api/__init__.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)    10768 2024-03-12 18:21:06.000000 janus-dtnaas-0.3rc1/janus/api/agent.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     3795 2023-11-06 16:43:05.000000 janus-dtnaas-0.3rc1/janus/api/ansible_job.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      498 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/constants.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)    33884 2024-03-12 18:20:53.000000 janus-dtnaas-0.3rc1/janus/api/controller.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     5903 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/db.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.878915 janus-dtnaas-0.3rc1/janus/api/kubernetes/
--rw-r--r--   0 ezra      (1000) ezra      (1000)       32 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/kubernetes/__init__.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)    16739 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/kubernetes/kube.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     5023 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/manager.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     4276 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/models.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      204 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/models_ws.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.878915 janus-dtnaas-0.3rc1/janus/api/portainer/
--rw-r--r--   0 ezra      (1000) ezra      (1000)       50 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/portainer/__init__.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)    33445 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/portainer/endpoints_api.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)    29536 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/portainer/portainer_docker.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     6067 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/profile.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)        2 2023-11-06 16:43:05.000000 janus-dtnaas-0.3rc1/janus/api/query.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2086 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/service.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.878915 janus-dtnaas-0.3rc1/janus/api/slurm/
--rw-r--r--   0 ezra      (1000) ezra      (1000)       33 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/slurm/__init__.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     4344 2024-03-12 18:27:12.000000 janus-dtnaas-0.3rc1/janus/api/slurm/slurm.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1081 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/sockets.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.878915 janus-dtnaas-0.3rc1/janus/api/sys/
--rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2021-10-13 19:48:34.000000 janus-dtnaas-0.3rc1/janus/api/sys/__init__.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      206 2021-10-13 19:48:34.000000 janus-dtnaas-0.3rc1/janus/api/sys/cpu.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      599 2021-10-13 19:48:34.000000 janus-dtnaas-0.3rc1/janus/api/sys/disk.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      313 2021-10-13 19:48:34.000000 janus-dtnaas-0.3rc1/janus/api/sys/mem.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1668 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/janus/api/sys/net.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      373 2021-10-13 19:48:34.000000 janus-dtnaas-0.3rc1/janus/api/sys/numa.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2411 2021-10-13 19:48:34.000000 janus-dtnaas-0.3rc1/janus/api/sys/sysctl.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)    11595 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/janus/api/sys/tc.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     9953 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/api/utils.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     5774 2024-03-12 18:19:36.000000 janus-dtnaas-0.3rc1/janus/app.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.882915 janus-dtnaas-0.3rc1/janus/config/
--rw-r--r--   0 ezra      (1000) ezra      (1000)      122 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/janus/config/janus.conf.example
--rw-r--r--   0 ezra      (1000) ezra      (1000)      369 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/janus/config/logging.conf
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.882915 janus-dtnaas-0.3rc1/janus/config/profiles/
--rw-r--r--   0 ezra      (1000) ezra      (1000)      193 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/janus/config/profiles/ansible.yaml
--rw-r--r--   0 ezra      (1000) ezra      (1000)      217 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/janus/config/profiles/features.yaml
--rw-r--r--   0 ezra      (1000) ezra      (1000)      617 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/config/profiles/networks.yaml
--rw-r--r--   0 ezra      (1000) ezra      (1000)      177 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/janus/config/profiles/profiles.yaml
--rw-r--r--   0 ezra      (1000) ezra      (1000)      133 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/janus/config/profiles/qos.yaml
--rw-r--r--   0 ezra      (1000) ezra      (1000)      943 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/janus/config/profiles/test-profile.yaml
--rw-r--r--   0 ezra      (1000) ezra      (1000)      374 2023-07-10 18:28:11.000000 janus-dtnaas-0.3rc1/janus/config/profiles/volumes.yaml
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.882915 janus-dtnaas-0.3rc1/janus/lib/
--rw-r--r--   0 ezra      (1000) ezra      (1000)       40 2021-10-13 19:48:34.000000 janus-dtnaas-0.3rc1/janus/lib/__init__.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     3742 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/lib/agent_monitor.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     4390 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/janus/settings.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.882915 janus-dtnaas-0.3rc1/janus_dtnaas.egg-info/
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2641 2024-03-12 21:13:09.000000 janus-dtnaas-0.3rc1/janus_dtnaas.egg-info/PKG-INFO
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1448 2024-03-12 21:13:09.000000 janus-dtnaas-0.3rc1/janus_dtnaas.egg-info/SOURCES.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)        1 2024-03-12 21:13:09.000000 janus-dtnaas-0.3rc1/janus_dtnaas.egg-info/dependency_links.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)       46 2024-03-12 21:13:09.000000 janus-dtnaas-0.3rc1/janus_dtnaas.egg-info/entry_points.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)      292 2024-03-12 21:13:09.000000 janus-dtnaas-0.3rc1/janus_dtnaas.egg-info/requires.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)        6 2024-03-12 21:13:09.000000 janus-dtnaas-0.3rc1/janus_dtnaas.egg-info/top_level.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)      292 2024-03-12 21:11:58.000000 janus-dtnaas-0.3rc1/requirements.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)       38 2024-03-12 21:13:09.882915 janus-dtnaas-0.3rc1/setup.cfg
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2731 2024-03-12 21:11:32.000000 janus-dtnaas-0.3rc1/setup.py
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-03-12 21:13:09.882915 janus-dtnaas-0.3rc1/tests/
--rw-r--r--   0 ezra      (1000) ezra      (1000)      165 2022-03-01 15:51:48.000000 janus-dtnaas-0.3rc1/tests/test_api.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2912 2024-03-12 17:51:52.000000 janus-dtnaas-0.3rc1/tests/test_multithread_safety.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.745263 janus_dtnaas-0.3rc2/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1513 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/LICENSE
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       41 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/MANIFEST.in
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2641 2024-05-03 17:32:31.745263 janus_dtnaas-0.3rc2/PKG-INFO
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1514 2023-11-06 16:43:03.000000 janus_dtnaas-0.3rc2/README.md
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.741263 janus_dtnaas-0.3rc2/janus/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2021-10-13 19:48:34.000000 janus_dtnaas-0.3rc2/janus/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       24 2021-10-13 19:48:34.000000 janus_dtnaas-0.3rc2/janus/agent_settings.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.741263 janus_dtnaas-0.3rc2/janus/api/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/janus/api/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)    10768 2024-03-12 18:21:06.000000 janus_dtnaas-0.3rc2/janus/api/agent.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     3795 2023-11-06 16:43:05.000000 janus_dtnaas-0.3rc2/janus/api/ansible_job.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      738 2024-04-30 14:38:18.000000 janus_dtnaas-0.3rc2/janus/api/constants.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)    33781 2024-04-30 14:38:18.000000 janus_dtnaas-0.3rc2/janus/api/controller.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     5910 2024-04-04 16:23:48.000000 janus_dtnaas-0.3rc2/janus/api/db.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.741263 janus_dtnaas-0.3rc2/janus/api/edge/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       31 2024-04-30 14:38:18.000000 janus_dtnaas-0.3rc2/janus/api/edge/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     4396 2024-04-30 14:38:18.000000 janus_dtnaas-0.3rc2/janus/api/edge/edge.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.741263 janus_dtnaas-0.3rc2/janus/api/kubernetes/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       32 2024-03-12 17:51:52.000000 janus_dtnaas-0.3rc2/janus/api/kubernetes/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)    17040 2024-04-04 16:23:48.000000 janus_dtnaas-0.3rc2/janus/api/kubernetes/kube.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     5485 2024-04-30 14:38:18.000000 janus_dtnaas-0.3rc2/janus/api/manager.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     4550 2024-05-03 17:26:00.000000 janus_dtnaas-0.3rc2/janus/api/models.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      518 2024-04-30 14:38:18.000000 janus_dtnaas-0.3rc2/janus/api/models_ws.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.741263 janus_dtnaas-0.3rc2/janus/api/portainer/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       50 2024-03-12 17:51:52.000000 janus_dtnaas-0.3rc2/janus/api/portainer/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)    33445 2024-03-12 17:51:52.000000 janus_dtnaas-0.3rc2/janus/api/portainer/endpoints_api.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)    29487 2024-04-30 14:38:18.000000 janus_dtnaas-0.3rc2/janus/api/portainer/portainer_docker.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     6684 2024-05-03 17:26:00.000000 janus_dtnaas-0.3rc2/janus/api/profile.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      698 2024-04-30 14:38:18.000000 janus_dtnaas-0.3rc2/janus/api/pubsub.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        2 2023-11-06 16:43:05.000000 janus_dtnaas-0.3rc2/janus/api/query.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2117 2024-04-30 14:38:18.000000 janus_dtnaas-0.3rc2/janus/api/service.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.745263 janus_dtnaas-0.3rc2/janus/api/slurm/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       33 2024-03-12 17:51:52.000000 janus_dtnaas-0.3rc2/janus/api/slurm/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     8867 2024-04-30 14:38:18.000000 janus_dtnaas-0.3rc2/janus/api/slurm/slurm.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2258 2024-04-30 14:38:18.000000 janus_dtnaas-0.3rc2/janus/api/sockets.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.745263 janus_dtnaas-0.3rc2/janus/api/sys/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2021-10-13 19:48:34.000000 janus_dtnaas-0.3rc2/janus/api/sys/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      206 2021-10-13 19:48:34.000000 janus_dtnaas-0.3rc2/janus/api/sys/cpu.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      599 2021-10-13 19:48:34.000000 janus_dtnaas-0.3rc2/janus/api/sys/disk.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      313 2021-10-13 19:48:34.000000 janus_dtnaas-0.3rc2/janus/api/sys/mem.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1668 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/janus/api/sys/net.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      373 2021-10-13 19:48:34.000000 janus_dtnaas-0.3rc2/janus/api/sys/numa.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2411 2021-10-13 19:48:34.000000 janus_dtnaas-0.3rc2/janus/api/sys/sysctl.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)    11595 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/janus/api/sys/tc.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     9940 2024-04-04 16:23:48.000000 janus_dtnaas-0.3rc2/janus/api/utils.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     5774 2024-03-12 18:19:36.000000 janus_dtnaas-0.3rc2/janus/app.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.745263 janus_dtnaas-0.3rc2/janus/config/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      122 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/janus/config/janus.conf.example
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      369 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/janus/config/logging.conf
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.745263 janus_dtnaas-0.3rc2/janus/config/profiles/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      193 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/janus/config/profiles/ansible.yaml
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      217 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/janus/config/profiles/features.yaml
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      617 2024-03-12 17:51:52.000000 janus_dtnaas-0.3rc2/janus/config/profiles/networks.yaml
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      177 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/janus/config/profiles/profiles.yaml
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      133 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/janus/config/profiles/qos.yaml
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      943 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/janus/config/profiles/test-profile.yaml
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      374 2023-07-10 18:28:11.000000 janus_dtnaas-0.3rc2/janus/config/profiles/volumes.yaml
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.745263 janus_dtnaas-0.3rc2/janus/lib/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       40 2021-10-13 19:48:34.000000 janus_dtnaas-0.3rc2/janus/lib/__init__.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     3650 2024-04-04 16:23:48.000000 janus_dtnaas-0.3rc2/janus/lib/agent_monitor.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     4276 2024-05-03 17:26:00.000000 janus_dtnaas-0.3rc2/janus/settings.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.745263 janus_dtnaas-0.3rc2/janus_dtnaas.egg-info/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2641 2024-05-03 17:32:31.000000 janus_dtnaas-0.3rc2/janus_dtnaas.egg-info/PKG-INFO
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1518 2024-05-03 17:32:31.000000 janus_dtnaas-0.3rc2/janus_dtnaas.egg-info/SOURCES.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        1 2024-05-03 17:32:31.000000 janus_dtnaas-0.3rc2/janus_dtnaas.egg-info/dependency_links.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       46 2024-05-03 17:32:31.000000 janus_dtnaas-0.3rc2/janus_dtnaas.egg-info/entry_points.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      292 2024-05-03 17:32:31.000000 janus_dtnaas-0.3rc2/janus_dtnaas.egg-info/requires.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        6 2024-05-03 17:32:31.000000 janus_dtnaas-0.3rc2/janus_dtnaas.egg-info/top_level.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      292 2024-03-12 21:11:58.000000 janus_dtnaas-0.3rc2/requirements.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       38 2024-05-03 17:32:31.745263 janus_dtnaas-0.3rc2/setup.cfg
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2731 2024-05-03 17:32:05.000000 janus_dtnaas-0.3rc2/setup.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2024-05-03 17:32:31.745263 janus_dtnaas-0.3rc2/tests/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      165 2022-03-01 15:51:48.000000 janus_dtnaas-0.3rc2/tests/test_api.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2912 2024-03-12 17:51:52.000000 janus_dtnaas-0.3rc2/tests/test_multithread_safety.py
```

### Comparing `janus-dtnaas-0.3rc1/LICENSE` & `janus_dtnaas-0.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/PKG-INFO` & `janus_dtnaas-0.3rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus-dtnaas
-Version: 0.3rc1
+Version: 0.3rc2
 Summary: Janus DTNaaS Controller
 Home-page: https://github.com/esnet/janus
 Author: Ezra Kissel
 Author-email: kissel@es.net
 Keywords: Janus Controller
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `janus-dtnaas-0.3rc1/README.md` & `janus_dtnaas-0.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/janus/api/agent.py` & `janus_dtnaas-0.3rc2/janus/api/agent.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/janus/api/ansible_job.py` & `janus_dtnaas-0.3rc2/janus/api/ansible_job.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/janus/api/controller.py` & `janus_dtnaas-0.3rc2/janus/api/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 from janus.api.models import (
     Node,
     Network,
     ContainerProfile,
     NetworkProfile,
     VolumeProfile,
     SessionRequest,
-    SessionConstraints
+    SessionConstraints,
+    AddEndpointRequest
 )
 from janus.api.utils import (
     commit_db,
     cname_from_id,
     precommit_db,
     set_qos,
     error_svc,
@@ -238,29 +239,27 @@
             raise BadRequest("Body is empty")
         if type(req) is dict:
             req = [req]
         log.debug(req)
         eps = list()
         try:
             for r in req:
-                url_split = urlsplit(r['url'])
-                ep = {"name": r['name'],
-                      "url": r['url'],
-                      "public_url": url_split.hostname if not "public_url" in r else r['public_url'],
-                      "type": EPType(r['type'])}
+                ep = AddEndpointRequest(**r)
+                if not ep.public_url:
+                    url_split = urlsplit(r['url'])
+                    ep.public_url = url_split.hostname
                 eps.append(ep)
         except Exception as e:
             br = BadRequest()
             br.data = f"error decoding request: {e}"
             raise br
 
         try:
             for ep in eps:
-                kwargs = {}
-                ret = cfg.sm.add_node(ep, **kwargs)
+                ret = cfg.sm.add_node(ep)
         except Exception as e:
             return {"error": "{}".format(e)}, 500
 
         try:
             log.info("New Node added, refreshing endpoint DB...")
             init_db(refresh=True)
         except Exception as e:
```

### Comparing `janus-dtnaas-0.3rc1/janus/api/db.py` & `janus_dtnaas-0.3rc2/janus/api/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             subnet = w.get('subnet', [])
             # try to get subnet information from profile if not tracked in endpoint
             if not subnet:
                 pnet = cfg.pm.get_profile(Constants.NET, n)
                 try:
                     subnet = pnet.settings.ipam.get('config') if pnet else []
                 except Exception as e:
-                    pass
+                    subnet = []
             subnet = [keys_lower(x) for x in subnet]
             key = f"{k}-{n}"
             curr = dbase.get(net_table, key=key)
             if not curr:
                 net = {'name': n,
                        'key': key,
                        'subnet': list(subnet),
```

### Comparing `janus-dtnaas-0.3rc1/janus/api/kubernetes/kube.py` & `janus_dtnaas-0.3rc2/janus/api/kubernetes/kube.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,41 +59,48 @@
             ctx = [x for x in contexts if x.get('name') == ctx_name][0]
             return ctx.get('context').get('namespace', self.NS)
         except Exception as e:
             log.error(f"Could not get namespace for ctx={ctx_name}: {e}")
             return self.NS
 
     def _get_client(self, ctx_name):
-        if self.config:
-            return client.ApiClient(self.config)
-        return config.new_client_from_config(context=ctx_name)
+        try:
+            if self.config:
+                return client.ApiClient(self.config)
+            return config.new_client_from_config(context=ctx_name)
+        except Exception as e:
+            log.error(f"Could not get Kubernetes client for {ctx_name}: {e}")
+            return None
 
     def _get_contexts(self):
         if self.api_key and self.api_cluster_name and self.api_cluster_url:
             self.config = client.Configuration()
             self.config.host = self.api_cluster_url
             self.config.api_key['authorization'] = self.api_key
             self.config.api_key_prefix['authorization'] = 'Bearer'
             self.config.verify_ssl = False
             return [{'name': self.api_cluster_name,
                      'context': {
                          'host': self.api_cluster_url,
                          'namespace': self.api_namespace}
                      }], None
         else:
-            return config.list_kube_config_contexts()
+            try:
+                return config.list_kube_config_contexts()
+            except Exception:
+                return [], None
 
     def get_nodes(self, nname=None, cb=None, refresh=False):
         ret = list()
         if not refresh:
             return ret
         contexts, active_context = self._get_contexts()
         if not contexts:
             log.error("Cannot find any contexts in current configuration.")
-            return
+            return ret
 
         node_count = 0
         for ctx in contexts:
             ctx_name = ctx.get('name')
             if nname and nname != ctx_name:
                 continue
             host_info = {
@@ -104,14 +111,16 @@
                 "mem": {
                     "total": 0
                 }
             }
             cnodes = list()
             archs = set()
             api_client = self._get_client(ctx_name)
+            if not api_client:
+                continue
             v1 = client.CoreV1Api(api_client)
             try:
                 res = v1.list_node(watch=False)
             except Exception as e:
                 log.error(f"Could not list nodes on cluster {ctx_name}: {e}")
                 continue
             for i in res.items:
```

### Comparing `janus-dtnaas-0.3rc1/janus/api/manager.py` & `janus_dtnaas-0.3rc2/janus/api/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,106 +1,118 @@
 import re
 import logging
+import queue
 from janus.api.portainer import PortainerDockerApi
 from janus.api.kubernetes import KubernetesApi
 from janus.api.slurm import JanusSlurmApi
+from janus.api.edge import JanusEdgeApi
 from janus.api.constants import State, EPType
 from janus.lib import AgentMonitor
-from janus.api.models import Node
+from janus.api.models import Node, AddEndpointRequest
+from janus.api.pubsub import Publisher
 from janus.api.utils import error_svc, handle_image
 from janus.settings import cfg, AGENT_AUTO_TUNE
 
 
 log = logging.getLogger(__name__)
 
 
 class ServiceManager():
     def __init__(self, db):
         self._db = db
         self._am = AgentMonitor()
         self.service_map = {
             EPType.PORTAINER: PortainerDockerApi(),
             EPType.KUBERNETES: KubernetesApi(),
-            EPType.SLURM: JanusSlurmApi()
+            EPType.SLURM: JanusSlurmApi(),
+            EPType.EDGE: JanusEdgeApi()
         }
+        self._pubsub = Publisher()
 
-    def _add_node_cb(self, node, name, url):
+    @property
+    def pubsub(self):
+        return self._pubsub
+
+    def _add_node_cb(self, node: dict, name, url):
         try:
             table = self._db.get_table('images')
             for img in node.get('images'):
                 iname = re.split(':|@', img)[0]
                 self._db.upsert(table, {'image': img, 'name': iname}, 'name', iname)
         except Exception as e:
             log.error("Could not save images for {}: {}".format(url, e))
         try:
-            (n, ret) = self._am.check_agent(name, url)
+            ret = self._am.check_agent(Node(**node), url)
             node['host'] = ret.json()
-            (n, ret) = self._am.tune(name, url)
+            ret = self._am.tune(url)
             node['host']['tuning'] = ret.json()
         except Exception as e:
             log.error("Could not fetch agent info from {}: {}".format(url, e))
-            self._am.start_agent(node)
+            self._am.start_agent(Node(**node))
 
     def get_nodes(self, nname=None, refresh=False):
         nodes = list()
         for k, s in self.service_map.items():
             try:
                 ns = s.get_nodes(nname, cb=self._add_node_cb, refresh=refresh)
                 nodes.extend(ns)
             except Exception as e:
                 import traceback
                 traceback.print_exc()
                 log.error(f"Error retrieving nodes from {k}: {e}")
         return nodes
 
-    def add_node(self, ep, **kwargs):
-        eptype = ep.get('type')
+    def add_node(self, ep: AddEndpointRequest, **kwargs):
+        eptype = ep.type
         n = self.service_map[eptype].create_node(ep, **kwargs)
         # Tune remote endpoints after addition if requested
         if AGENT_AUTO_TUNE:
-            self._am.tune(ep, post=True)
+            try:
+                self._am.tune(ep.public_url, post=True)
+            except Exception as e:
+                log.error(f"Could not apply auto-tuning, agent not running?: {e}")
 
-    def remove_node(self, node=None, nname=None):
+    def remove_node(self, node: dict = None, nname=None):
         if nname:
             ntable = self._db.get_table('nodes')
             node = self._db.get(ntable, name=nname)
         eptype = node.get('endpoint_type')
         return self.service_map[eptype].remove_node(node.get('id'))
 
-    def get_handler(self, node=None, nname=None):
+    def get_handler(self, node: dict = None, nname=None):
         if nname:
             ntable = self._db.get_table('nodes')
             node = self._db.get(ntable, name=nname)
         if not node:
             log.error(f"Node does not exist (node={node}, nname={nname})")
             return None
         eptype = node.get('endpoint_type')
         return self.service_map[eptype]
 
-    def get_auth_token(self, node=None, ntype=EPType.PORTAINER):
+    def get_auth_token(self, node: dict = None, ntype=EPType.PORTAINER):
         return self.service_map[ntype].auth_token
 
 
     def init_service(self, s, errs=False):
         n = s.get('node')
         sname = s.get('sname')
         nname = n.get('name')
         img = s.get('image')
         handler = self.get_handler(n)
 
         if handler.type == EPType.PORTAINER:
             # Docker-specific v4 vs v6 image registry nonsense. Need to abstract this away.
             try:
-                handle_image(n, img, handler, s.get('pull_image'))
+                handle_image(Node(**n), img, handler, s.get('pull_image'))
             except Exception as e:
                 log.error(f"Could not pull image {img} on node {nname}: {e}")
                 errs = error_svc(s, e)
                 try:
                     v6img = f"registry.ipv6.docker.com/{img}"
-                    handle_image(n, v6img, handler, s.get('pull_image'))
+                    handle_image(Node(**n), v6img, handler, s.get('pull_image'))
                     s['image'] = v6img
                 except Exception as e:
                     log.error(f"Could not pull image {v6img} on node {nname}: {e}")
                     errs = error_svc(s, e)
                     return None, None
 
         # clear any errors if image resolved
```

### Comparing `janus-dtnaas-0.3rc1/janus/api/models.py` & `janus_dtnaas-0.3rc2/janus/api/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pydantic import BaseModel, root_validator, create_model
+from pydantic import BaseModel, SerializeAsAny, root_validator, create_model
 from typing import List, Optional, Union
 
 
 class QoSProfileSettings(BaseModel):
     delay: Optional[str] = None
     loss: Optional[str] = None
     rate: Optional[str] = None
@@ -77,15 +77,15 @@
     enable_ipv6: bool = False
     ipam: Optional[dict] = None
     options: Optional[dict] = None
 
 
 class NetworkProfile(BaseModel):
     name: str
-    settings: NetworkProfileSettings
+    settings: SerializeAsAny[NetworkProfileSettings]
 
 
 class VolumeProfileSettings(BaseModel):
     type: str
     driver: Optional[str] = None
     source: Optional[str] = None
     target: Optional[str] = None
@@ -97,37 +97,18 @@
         return values
 
 
 class VolumeProfile(BaseModel):
     name: str
     settings: VolumeProfileSettings
 
-
-class SessionConstraints(BaseModel):
-    cpu: Optional[float] = None
-    memory: Optional[int] = None
-    nodeName: Optional[str] = None
-    nodeCount: Optional[int] = None
-    time: Optional[int] = None
-
-
-class SessionRequest(BaseModel):
-    node: dict
-    image: str
-    profile: ContainerProfile
-    constraints: SessionConstraints
-    arguments: Optional[str]
-    remove_container: Optional[bool]
-    kwargs: Optional[dict]
-
-
 class Node(BaseModel):
     id: Union[int, str]
     name: str
-
+    images: Optional[list] = None
 
 class Network(object):
     def __init__(self, net, node=None):
         self.name = None
         self.ipv4 = None
         self.ipv6 = None
         self.node = node
@@ -148,7 +129,32 @@
             return True
         return False
 
 
 class ServiceRecord(object):
     def __init__(self, srec_dict):
         pass
+
+### API Request objects
+class SessionConstraints(BaseModel):
+    cpu: Optional[float] = None
+    memory: Optional[int] = None
+    nodeName: Optional[str] = None
+    nodeCount: Optional[int] = None
+    nodeQueue: Optional[str] = None
+    time: Optional[int] = None
+
+class SessionRequest(BaseModel):
+    node: dict
+    image: str
+    profile: ContainerProfile
+    constraints: SessionConstraints
+    arguments: Optional[str]
+    remove_container: Optional[bool]
+    kwargs: Optional[dict]
+
+class AddEndpointRequest(BaseModel):
+    type: int
+    name: str
+    url: str
+    edge_type: Optional[int] = None
+    public_url: Optional[str] = None
```

### Comparing `janus-dtnaas-0.3rc1/janus/api/portainer/endpoints_api.py` & `janus_dtnaas-0.3rc2/janus/api/portainer/endpoints_api.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/janus/api/portainer/portainer_docker.py` & `janus_dtnaas-0.3rc2/janus/api/portainer/portainer_docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import six
 import time
 import json
 import logging
 import queue
 import websocket
+import shlex
 from threading import Thread
 from concurrent.futures.thread import ThreadPoolExecutor
 
 from portainer_api.api_client import ApiClient
 from portainer_api.rest import ApiException
 from portainer_api.configuration import Configuration as Config
 from portainer_api.api import AuthApi
@@ -16,15 +17,16 @@
 
 from janus.api.service import Service
 from janus.api.constants import Constants, EPType
 from janus.api.models import (
     Node,
     Network,
     ContainerProfile,
-    SessionRequest
+    SessionRequest,
+    AddEndpointRequest
 )
 from janus.settings import REGISTRIES as iregs
 from janus.settings import cfg, IGNORE_EPS
 from janus.api.utils import (
     get_next_cport,
     get_next_sport,
     get_next_vf,
@@ -178,23 +180,23 @@
                 traceback.print_exc()
                 log.error("Backend error: {}".format(e))
                 return
 
         return list(nodes.values())
 
     @auth
-    def create_node(self, ep, **kwargs):
+    def create_node(self, ep: AddEndpointRequest, **kwargs):
         eapi = EndpointsApi(self.client)
         eptype = 2 # We use Portainer Agent registration method
-        kwargs = {"url": ep['url'],
-                  "public_url": ep['public_url'],
+        kwargs = {"url": ep.url,
+                  "public_url": ep.public_url,
                   "tls": "true",
                   "tls_skip_verify": "true",
                   "tls_skip_client_verify": "true"}
-        return eapi.endpoint_create(ep.get('name'), eptype, **kwargs)
+        return eapi.endpoint_create(ep.name, eptype, **kwargs)
 
     @auth
     def remove_node(self, nid):
         eapi = EndpointsApi(self.client)
         return eapi.endpoint_delete(nid)
 
     # Images
@@ -386,15 +388,14 @@
         res = self._call("/endpoints/{}/docker/exec/{}/start".format(node.id, eid),
                          "POST", body, **kwargs)
         string = res.read().decode('utf-8')
         return {"response": string}
 
     def exec_stream(self, node: Node, container, eid, **kwargs):
         ws_url = f"{cfg.PORTAINER_WS}/exec?token={self.client.jwt}&id={eid}&endpointId={node.id}"
-        print (ws_url)
         ws = websocket.create_connection(ws_url)
 
         def _get_stream(ws, q):
             while True:
                 try:
                     msg = ws.recv()
                     q.put({"msg": msg, "eof": False})
@@ -520,18 +521,18 @@
                 continue
             # Otherwise we need to either create or recreate the network
             if not ninfo:
                 log.info(f"Network {net.name} not found on {nname}, attempting to create")
             elif ninfo and not is_subset(kwargs, ninfo.get('_data')):
                 log.info(f"Network {net.name} found on {nname} but differs from profile, attempting to recreate")
                 try:
-                    self.remove_network(node.get('id'), net.name)
+                    self.remove_network(Node(**node), net.name)
                 except Exception as e:
                     log.warn(f"Removing network {net.name} on {nname} failed: {e}")
-            self.create_network(node.get('id'), net.name, **kwargs)
+            self.create_network(Node(**node), net.name, **kwargs)
             created = True
         return created
 
 
     def create_service_record(self, sname, sreq: SessionRequest, addrs_v4, addrs_v6, cports, sports):
         srec = dict()
         node = sreq.node
@@ -635,35 +636,35 @@
                     "IPAMConfig": {
                         "IPv4Address": mgmt_ipv4,
                         "IPv6Address": mgmt_ipv6
                     }
                 }
                 })
 
-            # Constrain container memory if requested
-            mem = get_mem(node, prof)
-            if mem:
-                docker_kwargs["HostConfig"].update({"Memory": mem})
-
-            for e in prof.settings.environment:
-                # XXX: do some sanity checking here
-                docker_kwargs['Env'].append(e)
-
-            for v in prof.settings.volumes:
-                vol = cfg.get_volume(v)
-                if vol:
-                    readonly = True if "ReadOnly" in vol and vol['ReadOnly'] else False
-                    mnt = {'Type': vol['type'],
-                           'Source': vol.get('source', None),
-                           'Target': vol.get('target', None),
-                           'ReadOnly': readonly
-                           }
-                    docker_kwargs['HostConfig']['Mounts'].append(mnt)
-                    if "driver" in vol:
-                        docker_kwargs['HostConfig']['VolumeDriver'] = vol['driver']
+        # Constrain container memory if requested
+        mem = get_mem(node, prof)
+        if mem:
+            docker_kwargs["HostConfig"].update({"Memory": mem})
+
+        for e in prof.settings.environment:
+            # XXX: do some sanity checking here
+            docker_kwargs['Env'].append(e)
+
+        for v in prof.settings.volumes:
+            vol = cfg.pm.get_profile(Constants.VOL, v)
+            if vol:
+                readonly = True if "ReadOnly" in vol and vol['ReadOnly'] else False
+                mnt = {'Type': vol.settings.type,
+                       'Source': vol.settings.source,
+                       'Target': vol.settings.target,
+                       'ReadOnly': readonly
+                }
+                docker_kwargs['HostConfig']['Mounts'].append(mnt)
+                if "driver" in vol:
+                    docker_kwargs['HostConfig']['VolumeDriver'] = vol['driver']
 
         if dnet.name and not mnet.is_host():
             try:
                 dinfo = node['networks'][dnet.name]
             except:
                 raise Exception("Network not found: {}".format(dnet.name))
             # Pin CPUs based on data net
```

### Comparing `janus-dtnaas-0.3rc1/janus/api/profile.py` & `janus_dtnaas-0.3rc2/janus/api/profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,47 @@
 import os
 import yaml
 import logging
 from .utils import Constants
 from janus import settings
 from janus.settings import cfg
 from janus.api.db import QueryUser
-from janus.api.models import QoS_Controller, ContainerProfile, NetworkProfile, VolumeProfile
+from janus.api.models import (
+    QoS_Controller,
+    ContainerProfile,
+    NetworkProfile,
+    NetworkProfileSettings,
+    VolumeProfile
+)
 
 
 log = logging.getLogger(__name__)
 
 class ProfileManager(QueryUser):
     CLSMAP = {
         Constants.HOST: ContainerProfile,
         Constants.NET: NetworkProfile,
         Constants.VOL: VolumeProfile,
         Constants.QOS: QoS_Controller
     }
 
+    def _create_defaults(self):
+        net_tbl = self._db.get_table(Constants.NET)
+        for nname in settings.DEFAULT_NET_PROFILES:
+            if self._db.get(net_tbl, name=nname):
+                continue
+            log.debug(f"Adding default network profile {nname}")
+            driver = "null" if nname == "none" else nname
+            nprof = NetworkProfile(name=nname,
+                                   settings=NetworkProfileSettings(driver=driver))
+            self._db.upsert(net_tbl, nprof.model_dump(), 'name', nname)
+
     def __init__(self, db, profile_path = None):
         self._db = db
+        self._create_defaults()
         self._profile_path = profile_path
 
     def get_profile_from_db(self, ptype=None, p=None, user=None, group=None):
         profile_tbl = self._db.get_table(ptype)
         query = self.query_builder(user, group, {"name": p})
         if query and p:
             ret = self._db.get(profile_tbl, query=query)
```

### Comparing `janus-dtnaas-0.3rc1/janus/api/service.py` & `janus_dtnaas-0.3rc2/janus/api/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
 from janus.api.models import Node, SessionRequest
+from janus.settings import cfg
 
 
 class Service(ABC):
     def __init__(self):
         pass
 
     @abstractmethod
```

### Comparing `janus-dtnaas-0.3rc1/janus/api/slurm/slurm.py` & `janus_dtnaas-0.3rc2/janus/lib/agent_monitor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,165 +1,100 @@
-import os
-import time
-import json
 import logging
-import queue
+import time
+import requests
 from threading import Thread
-
-import openapi_client
-from openapi_client.api.slurm_api import SlurmApi
-from openapi_client import ApiClient as Client
-from openapi_client import Configuration as Config
-from openapi_client.models.v0038_job_submission import V0038JobSubmission
-from openapi_client.models.v0038_job_properties import V0038JobProperties
-
-from janus.api.service import Service
-from janus.api.constants import EPType
-from janus.api.constants import Constants
+import concurrent
+from concurrent.futures.thread import ThreadPoolExecutor
+from tinydb import TinyDB, Query
+from janus import settings
 from janus.settings import cfg
-from janus.api.models import (
-    Node,
-    Network,
-    ContainerProfile,
-    SessionRequest
-)
-from janus.api.utils import (
-    get_next_cport,
-    get_next_sport,
-    get_next_vf,
-    get_next_ipv4,
-    get_next_ipv6,
-    get_numa,
-    get_cpu,
-    get_cpuset,
-    get_mem,
-    is_subset
-)
+from janus.api.utils import handle_image
+from janus.api.portainer import PortainerDockerApi
+from janus.api.models import Node
+from portainer_api.rest import ApiException
 
 
 log = logging.getLogger(__name__)
 
-class JanusSlurmApi(Service):
-    DEF_MEM = "4G"
-    DEF_CPU = "2"
-
-    def __init__(self):
-        self.api_name = os.getenv('SLURM_NAME')
-        self.api_jwt = os.getenv('SLURM_JWT')
-        self.api_url = os.getenv('SLURM_URL')
-        self.api_user = os.getenv('SLURM_USER')
-        if self.api_url:
-            c = Config()
-            c.host = self.api_url
-            self._config = c
-            self._headers = {"X-SLURM-USER-NAME": self.api_user,
-                             "X-SLURM-USER-TOKEN": self.api_jwt}
-        else:
-            self._config = None
-
-    def _get_client(self):
-        return SlurmApi(Client(self._config))
-
-    @property
-    def type(self):
-        return EPType.SLURM
-
-    def get_nodes(self, nname=None, cb=None, refresh=False):
-        ret = list()
-        if not self._config:
-            return ret
-        api_client = self._get_client()
-        res = api_client.slurm_v0038_get_nodes(_headers=self._headers)
-        host_info = {
-            "cpu": {
-                "brand_raw": str(),
-                "count": 0,
+class AgentMonitor(object):
+    def __init__(self, client=None):
+        self._th = None
+        self._stop = False
+        self._client = client
+        self._dapi = PortainerDockerApi(client)
+        log.debug("Initialized Janus Agent Monitor")
+
+    def start(self):
+        self._th = Thread(target=self._thr, args=())
+        self._th.start()
+
+    def stop(self):
+        self._stop = True
+        self._th.join()
+
+    def start_agent(self, n: Node):
+        log.info(f"Attempting to start agent {n.name}")
+        img = settings.AGENT_IMAGE
+        docker_kwargs = {
+            "HostConfig": {
+                "RestartPolicy": {"Name": "unless-stopped"},
+                "NetworkMode": "host",
+                "Privileged": True
             },
-            "mem": {
-                "total": 0
-            }
+            "Tty": True,
+            "Env": [f"AGENT_PORT={settings.AGENT_PORT}"]
         }
-        node_count = 0
-        cnodes = list()
-        archs = set()
-        for n in res.nodes:
-            cnode = {
-                "name": n.name,
-                "addresses": [ n.address ]
-            }
-            host_info['cpu']['count'] += int(n.cpus)
-            archs.add(n.architecture)
-            cnodes.append(cnode)
-            node_count += 1
-
-        host_info['cpu']['brand_raw'] = " ".join(archs)
-        ret.append({
-            "name": self.api_name,
-            "id": self.api_name,
-            "endpoint_type": EPType.SLURM,
-            "endpoint_status": 1,
-            "cluster_node_count": node_count,
-            "cluster_nodes": cnodes,
-            "networks": dict(),
-            "host": host_info,
-            "url": self.api_url,
-            "public_url": self.api_url
-        })
-        return ret
-
-    def get_images(self, node: Node):
-        pass
-
-    def get_networks(self, node: Node):
-        pass
-
-    def get_containers(self, node: Node):
-        pass
-
-    def get_logs(self, node: Node, container, since=0, stderr=1, stdout=1, tail=100, timestamps=0):
-        pass
-
-    def pull_image(self, node: Node, image, tag):
-        pass
-
-    def create_node(self, nname, eptype, **kwargs):
-        pass
-
-    def create_container(self, node: Node, image: str, name: str = None, **kwargs):
-        pass
-
-    def start_container(self, node: Node, container: str, service=None, **kwargs):
-        pass
-
-    def stop_container(self, node: Node, container, **kwargs):
-        pass
-
-    def create_network(self, node: Node, net_name, **kwargs):
-        pass
-
-    def inspect_container(self, node: Node, container):
-        pass
-
-    def remove_container(self, node: Node, container):
-        pass
-
-    def connect_network(self, node: Node, network, container):
-        pass
-
-    def exec_create(self, node: Node, container, **kwargs):
-        pass
-
-    def exec_start(self, node: Node, ectx, **kwargs):
-        pass
-
-    def exec_stream(self, node: Node, container, eid, **kwargs):
-        pass
-
-    def remove_network(self, node: Node, network, **kwargs):
-        pass
-
-    def resolve_networks(self, node: dict, prof):
-        pass
-
-    def create_service_record(self, sname, sreq: SessionRequest, addrs_v4, addrs_v6, cports, sports):
-        srec = dict()
-        return srec
+        try:
+            ret = self._dapi.get_containers(n)
+            for i in ret:
+                if i['Image'] == settings.AGENT_IMAGE:
+                    log.info(f"Agent container is already running on {n.name}, check firewall?")
+                    return
+            handle_image(n, img, self._dapi)
+            ret = self._dapi.create_container(n, img, **docker_kwargs)
+            self._dapi.start_container(n, ret['Id'])
+        except ApiException as e:
+            log.error(f"Could not start agent container on {n.name}: {e.reason}: {e.body}")
+
+    def check_agent(self, n: Node, url):
+        try:
+            ret = requests.get("{}://{}:{}/api/janus/agent/node".format(settings.AGENT_PROTO,
+                                                                        url,
+                                                                        settings.AGENT_PORT),
+                               verify=settings.AGENT_SSL_VERIFY,
+                               timeout=2)
+            return ret
+        except Exception as e:
+            raise e
+
+    def tune(self, url, post=False):
+        if post:
+            fn = requests.post
+            log.debug("Applying agent tuning at {}".format(url))
+        else:
+            fn = requests.get
+        try:
+            ret = fn("{}://{}:{}/api/janus/agent/tune".format(settings.AGENT_PROTO,
+                                                              url,
+                                                              settings.AGENT_PORT),
+                     verify=settings.AGENT_SSL_VERIFY,
+                     timeout=2,
+                     auth=(settings.AGENT_USERNAME, settings.AGENT_PASSWORD))
+            return ret
+        except Exception as e:
+            raise e
+
+    def _thr(self):
+        while not self._stop:
+            log.info("Checking on agent status")
+            DB = TinyDB(cfg.get_dbpath())
+            Node = Query()
+            nodes = DB.table('nodes').all()
+            futures = list()
+            with ThreadPoolExecutor(max_workers=8) as executor:
+                for n in nodes:
+                    futures.append(executor.submit(self.check_agent, n))
+            for future in concurrent.futures.as_completed(futures):
+                item,ret = future.result()
+                if not ret:
+                    self.start_agent(item)
+            time.sleep(10)
```

### Comparing `janus-dtnaas-0.3rc1/janus/api/sockets.py` & `janus_dtnaas-0.3rc2/janus/api/sockets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,63 @@
 import json
 import logging
 
 from janus.settings import cfg
 from janus.api.constants import WSType
-from janus.api.models_ws import WSExecStream
+from janus.api.models_ws import WSExecStream, EdgeAgentRegister
 from janus.api.models import Node
+from janus.api.pubsub import Subscriber, TOPIC
 
 
 log = logging.getLogger(__name__)
 
 def handle_websocket(sock):
     data = sock.receive()
-    print (data)
     try:
         js = json.loads(data)
     except Exception as e:
         log.error(f"Invalid websocket request: {e}")
         sock.send(json.dumps({"error": "Invalid request"}))
         return
-    if js.get("type") == WSType.EXEC_STREAM:
+
+    typ = js.get("type")
+    if not typ or typ not in [*WSType]:
+        sock.send(json.dumps({"error": f"Invalid websocket request type: {typ}"}))
+        return
+
+    if typ == WSType.AGENT_COMM:
+        while True:
+            msg = sock.receive()
+            if msg.strip() == "q" or msg.strip() == "quit":
+                return
+            sock.send(msg)
+
+    if typ == WSType.AGENT_REGISTER:
+        peer = sock.sock.getpeername()
+        try:
+            req = EdgeAgentRegister(**js)
+            cfg.sm.add_node(req)
+        except Exception as e:
+            log.error(f"Invalid request: {e}")
+            sock.send(json.dumps({"error": f"Invalid request: {e}"}))
+            return
+
+    if typ == WSType.EVENTS:
+        peer = sock.sock.getpeername()
+        log.debug(f"Got event stream request from {peer}")
+        sub = Subscriber(peer)
+        res = cfg.sm.pubsub.subscribe(sub, TOPIC.event_stream)
+        while True:
+            r = sub.read()
+            if r.get("eof"):
+                break
+            sock.send(json.dumps(r.get("msg")))
+
+    if typ == WSType.EXEC_STREAM:
+        log.debug(f"Got exec stream request from {sock.sock.getpeername()}")
         req = WSExecStream(**js)
         handler = cfg.sm.get_handler(nname=req.node)
         try:
             res = handler.exec_stream(Node(id=req.node_id, name=req.node), req.container, req.exec_id)
         except Exception as e:
             log.error(f"No exec stream found for node {req.node} and container {req.container}: {e}")
             sock.send(json.dumps({"error": "Exec stream not found"}))
```

### Comparing `janus-dtnaas-0.3rc1/janus/api/sys/disk.py` & `janus_dtnaas-0.3rc2/janus/api/sys/disk.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/janus/api/sys/net.py` & `janus_dtnaas-0.3rc2/janus/api/sys/net.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/janus/api/sys/sysctl.py` & `janus_dtnaas-0.3rc2/janus/api/sys/sysctl.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/janus/api/sys/tc.py` & `janus_dtnaas-0.3rc2/janus/api/sys/tc.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/janus/api/utils.py` & `janus_dtnaas-0.3rc2/janus/api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import logging
 from ipaddress import IPv4Network, IPv4Address
 from ipaddress import IPv6Network, IPv6Address
 
 from janus import settings
 from janus.api.constants import Constants
-from janus.api.models import Network
+from janus.api.models import Network,Node
 from janus.settings import cfg
 import requests
 import shlex
 
 log = logging.getLogger(__name__)
 
 def keys_lower(in_dict):
@@ -205,16 +205,16 @@
     named_nets = dbase.search(nets, name=net.name)
     alloced = list()
     for n in named_nets:
         alloced.extend(n['allocated_v6'])
     ipnet = None
     for sub in network['subnet']:
         try:
-            ipnet = IPv6Network(sub['Subnet'])
-            gw = IPv6Address(sub.get('Gateway'))
+            ipnet = IPv6Network(sub['subnet'])
+            gw = IPv6Address(sub.get('gateway'))
             if gw:
                 alloced.append(str(gw))
             break
         except:
             pass
 
     if net.ipv6 and not ipnet:
@@ -272,24 +272,24 @@
         reason = e.reason
     except:
         reason = str(e)
     s['errors'].append({'reason': reason,
                         'response': restxt})
     return True
 
-def handle_image(n, img, handler, pull=False):
-    if img not in n['images'] or pull:
+def handle_image(n: Node, img, handler, pull=False):
+    if img not in n.images or pull:
         parts = img.split(':')
         if len(parts) == 1:
-            if f"{img}:latest" not in n['images'] or pull:
-                log.info(f"Pulling image {img} for node {n['name']}")
-                handler.pull_image(n['id'], parts[0], 'latest')
+            if f"{img}:latest" not in n.images or pull:
+                log.info(f"Pulling image {img} for node {n.name}")
+                handler.pull_image(n, parts[0], 'latest')
         elif len(parts) > 1:
-            log.info(f"Pulling image {img} for node {n['name']}")
-            handler.pull_image(n['id'], parts[0], parts[1])
+            log.info(f"Pulling image {img} for node {n.name}")
+            handler.pull_image(n, parts[0], parts[1])
 
 def set_qos(url, qos):
         try:
             api_url = "{}://{}:{}/api/janus/agent/tc/netem".format(
                 settings.AGENT_PROTO,
                 url,
                 settings.AGENT_PORT
```

### Comparing `janus-dtnaas-0.3rc1/janus/app.py` & `janus_dtnaas-0.3rc2/janus/app.py`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/janus/config/profiles/networks.yaml` & `janus_dtnaas-0.3rc2/janus/config/profiles/networks.yaml`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/janus/config/profiles/test-profile.yaml` & `janus_dtnaas-0.3rc2/janus/config/profiles/test-profile.yaml`

 * *Files identical despite different names*

### Comparing `janus-dtnaas-0.3rc1/janus/settings.py` & `janus_dtnaas-0.3rc2/janus/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 try:
     FLASK_DEBUG = True #os.environ['DEBUG']
 except:
     FLASK_DEBUG = False
 
 DEFAULT_PROFILE = 'default'
+DEFAULT_NET_PROFILES = ['bridge', 'host', 'none']
 SUPPORTED_FEATURES = ['rdma']
 SUPPORTED_IMAGES = ['dtnaas/tools',
                     'dtnaas/ofed']
 
 REGISTRIES = {
     "wharf.es.net": {
         "auth": os.getenv("REGISTRY_AUTH")
@@ -153,23 +154,15 @@
 
     def get_dbpath(self):
         return self._dbpath
 
     def get_users(self):
         return self._users
 
-    def get_volume(self, v):
-        return self._volumes.get(v, {})
-
-    def get_qos(self, v):
-        return self._qos.get(v, {})
-
-    def get_qos_list(self):
-        return self._qos
-
+    # EK: XXX fix this
     def get_feature(self, f):
         return self._features.get(f, {})
 
     def get_poststart(self, key):
         return self._post_starts.get(key, {})
```

### Comparing `janus-dtnaas-0.3rc1/janus_dtnaas.egg-info/PKG-INFO` & `janus_dtnaas-0.3rc2/janus_dtnaas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus-dtnaas
-Version: 0.3rc1
+Version: 0.3rc2
 Summary: Janus DTNaaS Controller
 Home-page: https://github.com/esnet/janus
 Author: Ezra Kissel
 Author-email: kissel@es.net
 Keywords: Janus Controller
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `janus-dtnaas-0.3rc1/janus_dtnaas.egg-info/SOURCES.txt` & `janus_dtnaas-0.3rc2/janus_dtnaas.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 janus/api/constants.py
 janus/api/controller.py
 janus/api/db.py
 janus/api/manager.py
 janus/api/models.py
 janus/api/models_ws.py
 janus/api/profile.py
+janus/api/pubsub.py
 janus/api/query.py
 janus/api/service.py
 janus/api/sockets.py
 janus/api/utils.py
+janus/api/edge/__init__.py
+janus/api/edge/edge.py
 janus/api/kubernetes/__init__.py
 janus/api/kubernetes/kube.py
 janus/api/portainer/__init__.py
 janus/api/portainer/endpoints_api.py
 janus/api/portainer/portainer_docker.py
 janus/api/slurm/__init__.py
 janus/api/slurm/slurm.py
```

### Comparing `janus-dtnaas-0.3rc1/setup.py` & `janus_dtnaas-0.3rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.read()
 
 setup(
     name='janus-dtnaas',
-    version='0.3-rc1',
+    version='0.3-rc2',
     description='Janus DTNaaS Controller',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/esnet/janus',
     author='Ezra Kissel',
     author_email="kissel@es.net",
     include_package_data=True,
```

### Comparing `janus-dtnaas-0.3rc1/tests/test_multithread_safety.py` & `janus_dtnaas-0.3rc2/tests/test_multithread_safety.py`

 * *Files identical despite different names*


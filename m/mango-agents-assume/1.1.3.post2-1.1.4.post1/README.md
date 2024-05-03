# Comparing `tmp/mango_agents_assume-1.1.3.post2.tar.gz` & `tmp/mango_agents_assume-1.1.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango_agents_assume-1.1.3.post2.tar", max compression
+gzip compressed data, was "mango_agents_assume-1.1.4.post1.tar", last modified: Fri May  3 11:51:53 2024, max compression
```

## Comparing `mango_agents_assume-1.1.3.post2.tar` & `mango_agents_assume-1.1.4.post1.tar`

### file list

```diff
@@ -1,34 +1,150 @@
--rw-r--r--   0        0        0     1067 2022-11-03 13:22:16.556574 mango_agents_assume-1.1.3.post2/LICENSE
--rw-r--r--   0        0        0      141 2023-04-06 22:19:54.843999 mango_agents_assume-1.1.3.post2/mango/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 13:56:18.197719 mango_agents_assume-1.1.3.post2/mango/agent/__init__.py
--rw-r--r--   0        0        0    17623 2024-03-18 17:18:29.556656 mango_agents_assume-1.1.3.post2/mango/agent/core.py
--rw-r--r--   0        0        0    17574 2024-03-18 17:18:29.556656 mango_agents_assume-1.1.3.post2/mango/agent/role.py
--rw-r--r--   0        0        0        0 2023-01-10 13:56:18.197719 mango_agents_assume-1.1.3.post2/mango/container/__init__.py
--rw-r--r--   0        0        0    32729 2024-04-09 10:17:04.387085 mango_agents_assume-1.1.3.post2/mango/container/core.py
--rw-r--r--   0        0        0     6037 2024-04-09 08:54:16.173551 mango_agents_assume-1.1.3.post2/mango/container/external_coupling.py
--rw-r--r--   0        0        0     8927 2024-03-18 17:17:20.173174 mango_agents_assume-1.1.3.post2/mango/container/factory.py
--rw-r--r--   0        0        0    10859 2024-03-18 17:17:20.177174 mango_agents_assume-1.1.3.post2/mango/container/mqtt.py
--rw-r--r--   0        0        0     3946 2023-09-11 10:52:50.668639 mango_agents_assume-1.1.3.post2/mango/container/protocol.py
--rw-r--r--   0        0        0     9981 2024-03-18 17:18:29.556656 mango_agents_assume-1.1.3.post2/mango/container/tcp.py
--rw-r--r--   0        0        0        0 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.3.post2/mango/messages/__init__.py
--rw-r--r--   0        0        0      992 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.3.post2/mango/messages/acl_message.proto
--rw-r--r--   0        0        0     2416 2024-01-22 12:24:19.685957 mango_agents_assume-1.1.3.post2/mango/messages/acl_message_pb2.py
--rw-r--r--   0        0        0    11319 2023-11-06 23:31:59.293673 mango_agents_assume-1.1.3.post2/mango/messages/codecs.py
--rw-r--r--   0        0        0     6006 2023-11-07 11:08:26.783856 mango_agents_assume-1.1.3.post2/mango/messages/message.py
--rw-r--r--   0        0        0       88 2023-01-07 21:29:58.312170 mango_agents_assume-1.1.3.post2/mango/messages/other_proto_msgs.proto
--rw-r--r--   0        0        0     1051 2024-01-22 12:24:19.685957 mango_agents_assume-1.1.3.post2/mango/messages/other_proto_msgs_pb2.py
--rw-r--r--   0        0        0        0 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.3.post2/mango/modules/__init__.py
--rw-r--r--   0        0        0     2591 2023-09-11 10:52:43.728609 mango_agents_assume-1.1.3.post2/mango/modules/base_module.py
--rw-r--r--   0        0        0     4167 2023-04-06 22:19:54.847998 mango_agents_assume-1.1.3.post2/mango/modules/mqtt_module.py
--rw-r--r--   0        0        0     4179 2024-03-18 17:17:20.177174 mango_agents_assume-1.1.3.post2/mango/modules/rabbit_module.py
--rw-r--r--   0        0        0     2827 2023-04-06 22:19:54.847998 mango_agents_assume-1.1.3.post2/mango/modules/zero_module.py
--rw-r--r--   0        0        0        0 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.3.post2/mango/util/__init__.py
--rw-r--r--   0        0        0     2670 2023-04-06 22:19:54.847998 mango_agents_assume-1.1.3.post2/mango/util/clock.py
--rw-r--r--   0        0        0     4705 2024-04-09 08:56:29.145255 mango_agents_assume-1.1.3.post2/mango/util/distributed_clock.py
--rw-r--r--   0        0        0     9512 2024-03-18 17:17:20.181174 mango_agents_assume-1.1.3.post2/mango/util/distributed_termination.py
--rw-r--r--   0        0        0     9179 2023-09-11 10:52:50.672639 mango_agents_assume-1.1.3.post2/mango/util/multiprocessing.py
--rw-r--r--   0        0        0    30940 2024-03-18 17:18:29.556656 mango_agents_assume-1.1.3.post2/mango/util/scheduling.py
--rw-r--r--   0        0        0     2186 2024-04-09 10:22:38.865390 mango_agents_assume-1.1.3.post2/mango/util/termination_detection.py
--rw-r--r--   0        0        0     1325 2024-04-09 10:23:30.204505 mango_agents_assume-1.1.3.post2/pyproject.toml
--rw-r--r--   0        0        0     7488 2023-11-08 08:44:41.520711 mango_agents_assume-1.1.3.post2/readme.md
--rw-r--r--   0        0        0     8870 1970-01-01 00:00:00.000000 mango_agents_assume-1.1.3.post2/PKG-INFO
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.600746 mango_agents_assume-1.1.4.post1/
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.536746 mango_agents_assume-1.1.4.post1/.github/
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.540746 mango_agents_assume-1.1.4.post1/.github/workflows/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1114 2024-05-03 11:47:15.000000 mango_agents_assume-1.1.4.post1/.github/workflows/publish-mango.yml
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      763 2024-05-03 11:44:54.000000 mango_agents_assume-1.1.4.post1/.github/workflows/test-mango.yml
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1253 2023-04-06 09:00:23.000000 mango_agents_assume-1.1.4.post1/.gitignore
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      540 2024-05-03 11:47:15.000000 mango_agents_assume-1.1.4.post1/.readthedocs.yaml
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1067 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/LICENSE
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     9935 2024-05-03 11:51:53.600746 mango_agents_assume-1.1.4.post1/PKG-INFO
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.540746 mango_agents_assume-1.1.4.post1/docs/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      638 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/Makefile
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      799 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/make.bat
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      146 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/requirements.txt
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.548746 mango_agents_assume-1.1.4.post1/docs/source/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)        1 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/ACL messages.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4482 2024-05-03 11:44:54.000000 mango_agents_assume-1.1.4.post1/docs/source/agents-container.rst
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.552746 mango_agents_assume-1.1.4.post1/docs/source/api_ref/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      234 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/index.rst
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.552746 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.core/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      100 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.core/index.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       85 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.core/mango.core.agent.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       93 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.core/mango.core.container.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      113 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.core/mango.core.container_protocols.rst
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.556746 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.messages/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      108 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.messages/index.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       95 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.messages/mango.messages.codecs.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       97 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.messages/mango.messages.message.rst
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.560746 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.modules/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      106 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.modules/index.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      103 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.modules/mango.modules.base_module.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      103 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.modules/mango.modules.mqtt_module.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      107 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.modules/mango.modules.rabbit_module.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      103 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/api_ref/mango.modules/mango.modules.zero_module.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     9295 2023-09-11 10:52:50.000000 mango_agents_assume-1.1.4.post1/docs/source/codecs.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2316 2024-05-03 11:44:54.000000 mango_agents_assume-1.1.4.post1/docs/source/conf.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      184 2023-04-19 20:49:32.000000 mango_agents_assume-1.1.4.post1/docs/source/customizing-container.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     7032 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/datenschutz.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     3080 2024-05-03 11:44:54.000000 mango_agents_assume-1.1.4.post1/docs/source/development.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     6215 2023-04-19 20:49:32.000000 mango_agents_assume-1.1.4.post1/docs/source/getting_started.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      764 2024-05-03 11:44:54.000000 mango_agents_assume-1.1.4.post1/docs/source/impressum.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1510 2023-04-06 22:19:54.000000 mango_agents_assume-1.1.4.post1/docs/source/index.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1297 2023-04-19 20:49:32.000000 mango_agents_assume-1.1.4.post1/docs/source/installation.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1122 2024-05-03 11:44:54.000000 mango_agents_assume-1.1.4.post1/docs/source/legals.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     3085 2023-04-06 22:19:54.000000 mango_agents_assume-1.1.4.post1/docs/source/message exchange.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      957 2023-04-19 20:44:56.000000 mango_agents_assume-1.1.4.post1/docs/source/migration.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     5570 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/docs/source/privacy.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4946 2023-01-10 13:56:18.000000 mango_agents_assume-1.1.4.post1/docs/source/role-api.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     8381 2024-05-03 11:44:54.000000 mango_agents_assume-1.1.4.post1/docs/source/scheduling.rst
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    28653 2023-04-19 20:49:32.000000 mango_agents_assume-1.1.4.post1/docs/source/tutorial.rst
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.560746 mango_agents_assume-1.1.4.post1/examples/
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.564746 mango_agents_assume-1.1.4.post1/examples/distributed_clock/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1272 2023-04-06 09:00:23.000000 mango_agents_assume-1.1.4.post1/examples/distributed_clock/README.md
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     3232 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/examples/distributed_clock/clock_agent.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4250 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/examples/distributed_clock/clock_manager.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      223 2023-04-06 09:00:23.000000 mango_agents_assume-1.1.4.post1/examples/distributed_clock/docker-compose.yml
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      184 2023-04-06 09:00:23.000000 mango_agents_assume-1.1.4.post1/examples/distributed_clock/mqtt.conf
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1186 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/examples/distributed_clock/serializer.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1434 2023-09-11 10:52:50.000000 mango_agents_assume-1.1.4.post1/examples/external_clock.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.564746 mango_agents_assume-1.1.4.post1/examples/getting_started/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      457 2023-02-17 12:07:40.000000 mango_agents_assume-1.1.4.post1/examples/getting_started/v_1.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      768 2023-04-06 22:19:54.000000 mango_agents_assume-1.1.4.post1/examples/getting_started/v_2.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      431 2023-02-17 12:07:40.000000 mango_agents_assume-1.1.4.post1/examples/getting_started/v_3.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1576 2023-04-06 22:19:54.000000 mango_agents_assume-1.1.4.post1/examples/getting_started/v_4.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2331 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/examples/ping_pong_termination.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2960 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/examples/rrule_event.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4746 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/examples/simple_agent.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     6332 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/examples/simple_market.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1332 2023-04-25 16:29:39.000000 mango_agents_assume-1.1.4.post1/examples/tcp_container_example.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.568746 mango_agents_assume-1.1.4.post1/examples/tutorial/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1498 2023-04-06 22:19:54.000000 mango_agents_assume-1.1.4.post1/examples/tutorial/v1_basic_setup_and_message_passing.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     7094 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/examples/tutorial/v2_inter_container_messaging_and_basic_functionality.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     7369 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/examples/tutorial/v3_codecs_and_typing.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    10371 2023-04-19 20:32:58.000000 mango_agents_assume-1.1.4.post1/examples/tutorial/v4_scheduling_and_roles.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.568746 mango_agents_assume-1.1.4.post1/images/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    61566 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/images/mango_basics.jpg
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.568746 mango_agents_assume-1.1.4.post1/mango/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      226 2024-05-03 11:48:41.000000 mango_agents_assume-1.1.4.post1/mango/__init__.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.568746 mango_agents_assume-1.1.4.post1/mango/agent/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)        0 2023-01-10 13:56:18.000000 mango_agents_assume-1.1.4.post1/mango/agent/__init__.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    17623 2024-05-03 11:46:28.000000 mango_agents_assume-1.1.4.post1/mango/agent/core.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    17574 2024-05-03 11:46:28.000000 mango_agents_assume-1.1.4.post1/mango/agent/role.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.572746 mango_agents_assume-1.1.4.post1/mango/container/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)        0 2023-01-10 13:56:18.000000 mango_agents_assume-1.1.4.post1/mango/container/__init__.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    32729 2024-05-03 11:46:28.000000 mango_agents_assume-1.1.4.post1/mango/container/core.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     6037 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/mango/container/external_coupling.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     8927 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/mango/container/factory.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    10859 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/mango/container/mqtt.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     3946 2023-09-11 10:52:50.000000 mango_agents_assume-1.1.4.post1/mango/container/protocol.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     9981 2024-05-03 11:46:28.000000 mango_agents_assume-1.1.4.post1/mango/container/tcp.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.600746 mango_agents_assume-1.1.4.post1/mango/mango_agents_assume.egg-info/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     9935 2024-05-03 11:51:53.000000 mango_agents_assume-1.1.4.post1/mango/mango_agents_assume.egg-info/PKG-INFO
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4087 2024-05-03 11:51:53.000000 mango_agents_assume-1.1.4.post1/mango/mango_agents_assume.egg-info/SOURCES.txt
+-rw-r--r--   0 maurer    (1000) maurer    (1000)        1 2024-05-03 11:51:53.000000 mango_agents_assume-1.1.4.post1/mango/mango_agents_assume.egg-info/dependency_links.txt
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      130 2024-05-03 11:51:53.000000 mango_agents_assume-1.1.4.post1/mango/mango_agents_assume.egg-info/requires.txt
+-rw-r--r--   0 maurer    (1000) maurer    (1000)        1 2024-05-03 11:51:53.000000 mango_agents_assume-1.1.4.post1/mango/mango_agents_assume.egg-info/top_level.txt
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.576746 mango_agents_assume-1.1.4.post1/mango/messages/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)        0 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/mango/messages/__init__.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      992 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/mango/messages/acl_message.proto
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2416 2024-01-22 12:24:19.000000 mango_agents_assume-1.1.4.post1/mango/messages/acl_message_pb2.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    11319 2023-11-06 23:31:59.000000 mango_agents_assume-1.1.4.post1/mango/messages/codecs.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     6006 2023-11-07 11:08:26.000000 mango_agents_assume-1.1.4.post1/mango/messages/message.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       88 2023-01-07 21:29:58.000000 mango_agents_assume-1.1.4.post1/mango/messages/other_proto_msgs.proto
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1051 2024-01-22 12:24:19.000000 mango_agents_assume-1.1.4.post1/mango/messages/other_proto_msgs_pb2.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.580746 mango_agents_assume-1.1.4.post1/mango/modules/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)        0 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/mango/modules/__init__.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2591 2023-09-11 10:52:43.000000 mango_agents_assume-1.1.4.post1/mango/modules/base_module.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4167 2023-04-06 22:19:54.000000 mango_agents_assume-1.1.4.post1/mango/modules/mqtt_module.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4179 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/mango/modules/rabbit_module.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2827 2023-04-06 22:19:54.000000 mango_agents_assume-1.1.4.post1/mango/modules/zero_module.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.580746 mango_agents_assume-1.1.4.post1/mango/util/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)        0 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/mango/util/__init__.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2670 2023-04-06 22:19:54.000000 mango_agents_assume-1.1.4.post1/mango/util/clock.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4705 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/mango/util/distributed_clock.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     9512 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/mango/util/distributed_termination.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     9179 2023-09-11 10:52:50.000000 mango_agents_assume-1.1.4.post1/mango/util/multiprocessing.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    30940 2024-05-03 11:46:28.000000 mango_agents_assume-1.1.4.post1/mango/util/scheduling.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2186 2024-05-03 11:48:41.000000 mango_agents_assume-1.1.4.post1/mango/util/termination_detection.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1098 2023-09-25 10:36:02.000000 mango_agents_assume-1.1.4.post1/noxfile.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     1447 2024-05-03 11:48:41.000000 mango_agents_assume-1.1.4.post1/pyproject.toml
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     7488 2024-05-03 11:44:54.000000 mango_agents_assume-1.1.4.post1/readme.md
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      111 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/requirements.txt
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       38 2024-05-03 11:51:53.600746 mango_agents_assume-1.1.4.post1/setup.cfg
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.536746 mango_agents_assume-1.1.4.post1/tests/
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.584746 mango_agents_assume-1.1.4.post1/tests/integration_tests/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       60 2023-09-11 10:52:50.000000 mango_agents_assume-1.1.4.post1/tests/integration_tests/msg.proto
+-rw-r--r--   0 maurer    (1000) maurer    (1000)      961 2023-10-23 10:10:56.000000 mango_agents_assume-1.1.4.post1/tests/integration_tests/msg_pb2.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2184 2023-04-19 20:32:58.000000 mango_agents_assume-1.1.4.post1/tests/integration_tests/test_distributed_clock.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4795 2023-09-11 10:52:50.000000 mango_agents_assume-1.1.4.post1/tests/integration_tests/test_message_roundtrip.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2086 2023-09-11 10:52:43.000000 mango_agents_assume-1.1.4.post1/tests/integration_tests/test_message_roundtrip_mp.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2511 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/tests/integration_tests/test_single_container_termination.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.584746 mango_agents_assume-1.1.4.post1/tests/unit_tests/
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.584746 mango_agents_assume-1.1.4.post1/tests/unit_tests/clock/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     6653 2023-04-06 22:19:54.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/clock/test_external_clock.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.588746 mango_agents_assume-1.1.4.post1/tests/unit_tests/container/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     3933 2023-10-23 10:10:56.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/container/test_mp.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     5238 2023-10-23 10:10:56.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/container/test_tcp.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.592746 mango_agents_assume-1.1.4.post1/tests/unit_tests/core/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2584 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/core/test_agent.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     6066 2023-04-06 22:19:54.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/core/test_container.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     9361 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/core/test_external_scheduling_container.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.596747 mango_agents_assume-1.1.4.post1/tests/unit_tests/messages/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)       60 2022-11-03 13:22:16.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/messages/msg.proto
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     2019 2023-04-18 11:28:51.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/messages/msg_pb2.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     5020 2023-09-11 10:52:50.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/messages/test_codecs.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.596747 mango_agents_assume-1.1.4.post1/tests/unit_tests/role/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4128 2024-05-03 11:46:46.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/role/role_test.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     7520 2024-05-03 11:46:28.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/role_agent_test.py
+-rw-r--r--   0 maurer    (1000) maurer    (1000)     4861 2024-05-03 11:45:41.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/test_agents.py
+drwxr-xr-x   0 maurer    (1000) maurer    (1000)        0 2024-05-03 11:51:53.596747 mango_agents_assume-1.1.4.post1/tests/unit_tests/util/
+-rw-r--r--   0 maurer    (1000) maurer    (1000)    11324 2024-05-03 11:46:28.000000 mango_agents_assume-1.1.4.post1/tests/unit_tests/util/scheduling_test.py
```

### Comparing `mango_agents_assume-1.1.3.post2/LICENSE` & `mango_agents_assume-1.1.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/agent/core.py` & `mango_agents_assume-1.1.4.post1/mango/agent/core.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/agent/role.py` & `mango_agents_assume-1.1.4.post1/mango/agent/role.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/container/core.py` & `mango_agents_assume-1.1.4.post1/mango/container/core.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/container/external_coupling.py` & `mango_agents_assume-1.1.4.post1/mango/container/external_coupling.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/container/factory.py` & `mango_agents_assume-1.1.4.post1/mango/container/factory.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/container/mqtt.py` & `mango_agents_assume-1.1.4.post1/mango/container/mqtt.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/container/protocol.py` & `mango_agents_assume-1.1.4.post1/mango/container/protocol.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/container/tcp.py` & `mango_agents_assume-1.1.4.post1/mango/container/tcp.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/messages/acl_message.proto` & `mango_agents_assume-1.1.4.post1/mango/messages/acl_message.proto`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/messages/acl_message_pb2.py` & `mango_agents_assume-1.1.4.post1/mango/messages/acl_message_pb2.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/messages/codecs.py` & `mango_agents_assume-1.1.4.post1/mango/messages/codecs.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/messages/message.py` & `mango_agents_assume-1.1.4.post1/mango/messages/message.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/messages/other_proto_msgs_pb2.py` & `mango_agents_assume-1.1.4.post1/mango/messages/other_proto_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/modules/base_module.py` & `mango_agents_assume-1.1.4.post1/mango/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/modules/mqtt_module.py` & `mango_agents_assume-1.1.4.post1/mango/modules/mqtt_module.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/modules/rabbit_module.py` & `mango_agents_assume-1.1.4.post1/mango/modules/rabbit_module.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/modules/zero_module.py` & `mango_agents_assume-1.1.4.post1/mango/modules/zero_module.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/util/clock.py` & `mango_agents_assume-1.1.4.post1/mango/util/clock.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/util/distributed_clock.py` & `mango_agents_assume-1.1.4.post1/mango/util/distributed_clock.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/util/distributed_termination.py` & `mango_agents_assume-1.1.4.post1/mango/util/distributed_termination.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/util/multiprocessing.py` & `mango_agents_assume-1.1.4.post1/mango/util/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/util/scheduling.py` & `mango_agents_assume-1.1.4.post1/mango/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/mango/util/termination_detection.py` & `mango_agents_assume-1.1.4.post1/mango/util/termination_detection.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/pyproject.toml` & `mango_agents_assume-1.1.4.post1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,62 @@
-[tool.poetry]
+[build-system]
+requires = ["setuptools>=60", "setuptools-scm>=8.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
 name = "mango-agents-assume"
-version = "1.1.3-2"
+#version = "1.1.4-1"
+dynamic = ["version"]
 description = "Modular Python Agent Framework - Temporary Fork of mango for development purpose"
-authors = ["Mango Developers <mango@offis.de>", "Florian Maurer <fmaurer@disroot.org>"]
-license = "LICENSE"
+authors = [{name="Mango Developers", email="mango@offis.de"}, {name="Florian Maurer", email="fmaurer@disroot.org"}]
+license = {file="LICENSE"}
 readme = "readme.md"
-
-homepage = "https://mango-agents.readthedocs.io/"
-repository = "https://gitlab.com/maurerle/mango"
-
-keywords = ["agent based simulation", "simulation"]
+requires-python = ">=3.9"
 
 classifiers=[
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Framework :: AsyncIO",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
-packages = [
-    { include="mango", from="." },
+keywords = ["agent based simulation", "simulation"]
+
+dependencies = [
+    "paho-mqtt>=1.5.1",
+    "dill>=0.3.6",
+    "msgspec>=0.14.2",
+    "protobuf>=3.20.3",
+    "python-dateutil",
 ]
 
-[tool.poetry.dependencies]
-python = "^3.7"
-paho-mqtt = "^1.5.1"
-dill = ">=0.3.6"
-msgspec = ">=0.14.2"
-protobuf = "^3.20.3"
-python-dateutil = "^2.8.2"
-
-[tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-isort = "^5.12.0"
-pytest = "^7.2.2"
-pytest-cov = "^4.1.0"
-pytest-asyncio = "^0.21.1"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[project.urls]
+Homepage = "https://mango-agents.readthedocs.io/"
+Repository = "https://gitlab.com/maurerle/mango"
+
+[project.optional-dependencies]
+dev = [
+    "black",
+    "isort",
+    "pytest",
+    "pytest-cov",
+    "pytest-asyncio",
+]
+
+[tool.setuptools.packages.find]
+where = ["mango"]
+include = ["."]
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest]
 testpaths = "tests"
 
 [tool.coverage.report]
 exclude_lines = ["if __name__ == .__main__.:"]
+
+[tool.setuptools_scm]
```

### Comparing `mango_agents_assume-1.1.3.post2/readme.md` & `mango_agents_assume-1.1.4.post1/readme.md`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.3.post2/PKG-INFO` & `mango_agents_assume-1.1.4.post1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,58 @@
 Metadata-Version: 2.1
 Name: mango-agents-assume
-Version: 1.1.3.post2
+Version: 1.1.4.post1
 Summary: Modular Python Agent Framework - Temporary Fork of mango for development purpose
-Home-page: https://mango-agents.readthedocs.io/
-License: LICENSE
+Author-email: Mango Developers <mango@offis.de>, Florian Maurer <fmaurer@disroot.org>
+License: MIT License
+        
+        Copyright (c) 2020 OFFIS e.V.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://mango-agents.readthedocs.io/
+Project-URL: Repository, https://gitlab.com/maurerle/mango
 Keywords: agent based simulation,simulation
-Author: Mango Developers
-Author-email: mango@offis.de
-Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Framework :: AsyncIO
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: dill (>=0.3.6)
-Requires-Dist: msgspec (>=0.14.2)
-Requires-Dist: paho-mqtt (>=1.5.1,<2.0.0)
-Requires-Dist: protobuf (>=3.20.3,<4.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Project-URL: Repository, https://gitlab.com/maurerle/mango
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: paho-mqtt>=1.5.1
+Requires-Dist: dill>=0.3.6
+Requires-Dist: msgspec>=0.14.2
+Requires-Dist: protobuf>=3.20.3
+Requires-Dist: python-dateutil
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
 
 # mango
 
 [PyPi](https://pypi.org/project/mango-agents/) | [Read the Docs](https://mango-agents.readthedocs.io)
 | [Github](https://github.com/OFFIS-DAI/mango) | [mail](mailto:mango@offis.de)
 
 **Note:** _This project is still in an early development stage. 
@@ -232,8 +251,7 @@
 ## License
 
 Distributed under the MIT license. 
 
 [comment]: <> (##TODO  Release History * 0.0.1 First TCPContainer with json)
 [comment]: <> (* 0.0.2 * Added MQTTContainer and protobuf support  )
 
-
```


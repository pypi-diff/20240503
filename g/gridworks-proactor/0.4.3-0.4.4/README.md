# Comparing `tmp/gridworks_proactor-0.4.3.tar.gz` & `tmp/gridworks_proactor-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_proactor-0.4.3.tar", max compression
+gzip compressed data, was "gridworks_proactor-0.4.4.tar", max compression
```

## Comparing `gridworks_proactor-0.4.3.tar` & `gridworks_proactor-0.4.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1070 2024-04-23 18:16:37.007687 gridworks_proactor-0.4.3/LICENSE
--rw-r--r--   0        0        0     7405 2024-04-23 18:16:37.007687 gridworks_proactor-0.4.3/README.md
--rw-r--r--   0        0        0     2664 2024-04-23 18:16:49.083745 gridworks_proactor-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2767 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/__init__.py
--rw-r--r--   0        0        0      213 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/actors/__init__.py
--rw-r--r--   0        0        0     2523 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/actors/actor.py
--rw-r--r--   0        0        0     8347 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/actors/rest.py
--rw-r--r--   0        0        0     1611 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/config/__init__.py
--rw-r--r--   0        0        0     4112 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/config/logging.py
--rw-r--r--   0        0        0     1765 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/config/mqtt.py
--rw-r--r--   0        0        0     5583 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/config/paths.py
--rw-r--r--   0        0        0     2180 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/config/proactor_settings.py
--rw-r--r--   0        0        0     1592 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/external_watchdog.py
--rw-r--r--   0        0        0     6747 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/io_loop.py
--rw-r--r--   0        0        0     1841 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/links/__init__.py
--rw-r--r--   0        0        0     3105 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/links/acks.py
--rw-r--r--   0        0        0      514 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/links/asyncio_timer_manager.py
--rw-r--r--   0        0        0    19361 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/links/link_manager.py
--rw-r--r--   0        0        0    16224 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/links/link_state.py
--rw-r--r--   0        0        0     2220 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/links/message_times.py
--rw-r--r--   0        0        0    11742 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/links/mqtt.py
--rw-r--r--   0        0        0     2792 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/links/reuploads.py
--rw-r--r--   0        0        0     1487 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/links/timer_interface.py
--rw-r--r--   0        0        0     5899 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/logger.py
--rw-r--r--   0        0        0     5197 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/logging_setup.py
--rw-r--r--   0        0        0     7755 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/message.py
--rw-r--r--   0        0        0    13989 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/persister.py
--rw-r--r--   0        0        0    25498 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/proactor_implementation.py
--rw-r--r--   0        0        0     7554 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/proactor_interface.py
--rw-r--r--   0        0        0     2645 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/problems.py
--rw-r--r--   0        0        0        0 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/py.typed
--rw-r--r--   0        0        0     3714 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/stats.py
--rw-r--r--   0        0        0     1235 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/str_tasks.py
--rw-r--r--   0        0        0     9316 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/sync_thread.py
--rw-r--r--   0        0        0     5981 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/watchdog.py
--rw-r--r--   0        0        0     3723 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor/web_manager.py
--rw-r--r--   0        0        0     2215 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/__init__.py
--rw-r--r--   0        0        0     5947 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/certs.py
--rw-r--r--   0        0        0     6602 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/clean.py
--rw-r--r--   0        0        0     9416 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/comm_test_helper.py
--rw-r--r--   0        0        0    20073 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/config/hardware-layout.json
--rw-r--r--   0        0        0      807 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/dummies/__init__.py
--rw-r--r--   0        0        0      187 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/dummies/child/__init__.py
--rw-r--r--   0        0        0      658 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/dummies/child/config.py
--rw-r--r--   0        0        0     2739 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/dummies/child/dummy.py
--rw-r--r--   0        0        0      188 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/dummies/names.py
--rw-r--r--   0        0        0      193 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/dummies/parent/__init__.py
--rw-r--r--   0        0        0      750 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/dummies/parent/config.py
--rw-r--r--   0        0        0     2198 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/dummies/parent/dummy.py
--rw-r--r--   0        0        0     3349 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/logger_guard.py
--rw-r--r--   0        0        0    11463 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/proactor_recorder.py
--rw-r--r--   0        0        0    60714 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/proactor_test_collections.py
--rw-r--r--   0        0        0     4259 2024-04-23 18:16:37.011687 gridworks_proactor-0.4.3/src/gwproactor_test/wait.py
--rw-r--r--   0        0        0     8814 1970-01-01 00:00:00.000000 gridworks_proactor-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-03 14:43:01.081995 gridworks_proactor-0.4.4/LICENSE
+-rw-r--r--   0        0        0     7405 2024-05-03 14:43:01.081995 gridworks_proactor-0.4.4/README.md
+-rw-r--r--   0        0        0     2683 2024-05-03 14:43:09.305966 gridworks_proactor-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2767 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/__init__.py
+-rw-r--r--   0        0        0      213 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/actors/__init__.py
+-rw-r--r--   0        0        0     2523 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/actors/actor.py
+-rw-r--r--   0        0        0     8347 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/actors/rest.py
+-rw-r--r--   0        0        0     1611 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/config/__init__.py
+-rw-r--r--   0        0        0     4112 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/config/logging.py
+-rw-r--r--   0        0        0     1765 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/config/mqtt.py
+-rw-r--r--   0        0        0     5583 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/config/paths.py
+-rw-r--r--   0        0        0     2180 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/config/proactor_settings.py
+-rw-r--r--   0        0        0     1592 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/external_watchdog.py
+-rw-r--r--   0        0        0     6747 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/io_loop.py
+-rw-r--r--   0        0        0     1841 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/links/__init__.py
+-rw-r--r--   0        0        0     3105 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/links/acks.py
+-rw-r--r--   0        0        0      514 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/links/asyncio_timer_manager.py
+-rw-r--r--   0        0        0    23028 2024-05-03 14:43:09.305966 gridworks_proactor-0.4.4/src/gwproactor/links/link_manager.py
+-rw-r--r--   0        0        0    16224 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/links/link_state.py
+-rw-r--r--   0        0        0     2220 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/links/message_times.py
+-rw-r--r--   0        0        0    11742 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/links/mqtt.py
+-rw-r--r--   0        0        0     8703 2024-05-03 14:43:09.305966 gridworks_proactor-0.4.4/src/gwproactor/links/reuploads.py
+-rw-r--r--   0        0        0     1487 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/links/timer_interface.py
+-rw-r--r--   0        0        0     5899 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/logger.py
+-rw-r--r--   0        0        0     5197 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/logging_setup.py
+-rw-r--r--   0        0        0     7755 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/message.py
+-rw-r--r--   0        0        0    14158 2024-05-03 14:43:09.305966 gridworks_proactor-0.4.4/src/gwproactor/persister.py
+-rw-r--r--   0        0        0    25919 2024-05-03 14:43:09.305966 gridworks_proactor-0.4.4/src/gwproactor/proactor_implementation.py
+-rw-r--r--   0        0        0     7554 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/proactor_interface.py
+-rw-r--r--   0        0        0     2645 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/problems.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/py.typed
+-rw-r--r--   0        0        0     4492 2024-05-03 14:43:09.305966 gridworks_proactor-0.4.4/src/gwproactor/stats.py
+-rw-r--r--   0        0        0     1235 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/str_tasks.py
+-rw-r--r--   0        0        0     9316 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/sync_thread.py
+-rw-r--r--   0        0        0     5981 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/watchdog.py
+-rw-r--r--   0        0        0     3723 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor/web_manager.py
+-rw-r--r--   0        0        0     2215 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/__init__.py
+-rw-r--r--   0        0        0     5947 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/certs.py
+-rw-r--r--   0        0        0     6602 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/clean.py
+-rw-r--r--   0        0        0     9958 2024-05-03 14:43:09.305966 gridworks_proactor-0.4.4/src/gwproactor_test/comm_test_helper.py
+-rw-r--r--   0        0        0    20073 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/config/hardware-layout.json
+-rw-r--r--   0        0        0      807 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/dummies/__init__.py
+-rw-r--r--   0        0        0      187 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/dummies/child/__init__.py
+-rw-r--r--   0        0        0      658 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/dummies/child/config.py
+-rw-r--r--   0        0        0     2739 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/dummies/child/dummy.py
+-rw-r--r--   0        0        0      188 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/dummies/names.py
+-rw-r--r--   0        0        0      193 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/dummies/parent/__init__.py
+-rw-r--r--   0        0        0      750 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/dummies/parent/config.py
+-rw-r--r--   0        0        0     2198 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/dummies/parent/dummy.py
+-rw-r--r--   0        0        0     3349 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/logger_guard.py
+-rw-r--r--   0        0        0    11282 2024-05-03 14:43:09.305966 gridworks_proactor-0.4.4/src/gwproactor_test/proactor_recorder.py
+-rw-r--r--   0        0        0    65515 2024-05-03 14:43:09.305966 gridworks_proactor-0.4.4/src/gwproactor_test/proactor_test_collections.py
+-rw-r--r--   0        0        0     4259 2024-05-03 14:43:01.085995 gridworks_proactor-0.4.4/src/gwproactor_test/wait.py
+-rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 gridworks_proactor-0.4.4/PKG-INFO
```

### Comparing `gridworks_proactor-0.4.3/LICENSE` & `gridworks_proactor-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/README.md` & `gridworks_proactor-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/pyproject.toml` & `gridworks_proactor-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-proactor"
-version = "0.4.3"
+version = "0.4.4"
 description = "Gridworks Proactor"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-proactor"
 repository = "https://github.com/thegridelectric/gridworks-proactor"
 documentation = "https://gridworks-proactor.readthedocs.io"
@@ -31,14 +31,15 @@
 gridworks-protocol = "^0.7.4"
 #gridworks-protocol = {path="../gridworks-protocol", develop=true}
 #gridworks-protocol = {git = "https://github.com/thegridelectric/gridworks-protocol.git", branch="SOME_DEV_BRANCH"}
 gridworks-cert = {version = ">=0.4.2", optional = true}
 aiohttp = "^3.8.5"
 yarl = "^1.9.2"
 multidict = "^6.0.4"
+pendulum = "2.1.2"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
```

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/__init__.py` & `gridworks_proactor-0.4.4/src/gwproactor/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/actors/actor.py` & `gridworks_proactor-0.4.4/src/gwproactor/actors/actor.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/actors/rest.py` & `gridworks_proactor-0.4.4/src/gwproactor/actors/rest.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/config/__init__.py` & `gridworks_proactor-0.4.4/src/gwproactor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/config/logging.py` & `gridworks_proactor-0.4.4/src/gwproactor/config/logging.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/config/mqtt.py` & `gridworks_proactor-0.4.4/src/gwproactor/config/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/config/paths.py` & `gridworks_proactor-0.4.4/src/gwproactor/config/paths.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/config/proactor_settings.py` & `gridworks_proactor-0.4.4/src/gwproactor/config/proactor_settings.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/external_watchdog.py` & `gridworks_proactor-0.4.4/src/gwproactor/external_watchdog.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/io_loop.py` & `gridworks_proactor-0.4.4/src/gwproactor/io_loop.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/links/__init__.py` & `gridworks_proactor-0.4.4/src/gwproactor/links/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/links/acks.py` & `gridworks_proactor-0.4.4/src/gwproactor/links/acks.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/links/asyncio_timer_manager.py` & `gridworks_proactor-0.4.4/src/gwproactor/links/asyncio_timer_manager.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/links/link_manager.py` & `gridworks_proactor-0.4.4/src/gwproactor/links/link_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 from gwproactor.links.timer_interface import TimerManagerInterface
 from gwproactor.logger import ProactorLogger
 from gwproactor.message import MQTTConnectFailPayload
 from gwproactor.message import MQTTConnectPayload
 from gwproactor.message import MQTTDisconnectPayload
 from gwproactor.message import MQTTReceiptPayload
 from gwproactor.message import MQTTSubackPayload
+from gwproactor.persister import ByteDecodingError
+from gwproactor.persister import DecodingError
+from gwproactor.persister import FileEmptyWarning
 from gwproactor.persister import JSONDecodingError
 from gwproactor.persister import PersisterInterface
 from gwproactor.persister import UIDMissingWarning
 from gwproactor.problems import Problems
 from gwproactor.stats import ProactorStats
 
 
@@ -88,15 +91,14 @@
     ):
         self.publication_name = publication_name
         self._settings = settings
         self._logger = logger
         self._stats = stats
         self._event_persister = event_persister
         self._reuploads = Reuploads(
-            self._event_persister,
             self._logger,
             self._settings.num_initial_event_reuploads,
         )
         self._mqtt_clients = MQTTClients()
         self._mqtt_codecs = dict()
         self._states = LinkStates()
         self._message_times = MessageTimes()
@@ -204,14 +206,17 @@
                 s += f"\t{client}\n"
                 for subscription in self._mqtt_clients.client_wrapper(
                     client
                 ).subscription_items():
                     s += f"\t\t[{subscription}]\n"
             self._logger.lifecycle(s)
 
+    def get_reuploads_str(self, verbose: bool = True, num_events: int = 5) -> str:
+        return self._reuploads.get_str(verbose=verbose, num_events=num_events)
+
     def publish_message(
         self, client, message: Message, qos: int = 0, context: Any = None
     ) -> MQTTMessageInfo:
         topic = message.mqtt_topic()
         payload = self._mqtt_codecs[client].encode(message)
         self._logger.message_summary(
             "OUT mqtt    ",
@@ -249,69 +254,148 @@
             self.publish_upstream(event, AckRequired=True)
         return self._event_persister.persist(
             event.MessageId,
             event.json(sort_keys=True, indent=2).encode(self.PERSISTER_ENCODING),
         )
 
     def _start_reupload(self) -> None:
-        self._logger.path("++_start_reupload reuploading: %s", self.reuploading())
-        path_dbg = 0
         if not self._reuploads.reuploading():
+            self._continue_reupload(
+                self._reuploads.start_reupload(self._event_persister.pending())
+            )
+
+    def _continue_reupload(self, event_ids: list[str]) -> None:
+        self._logger.path("++_continue_reupload  %d", len(event_ids))
+        path_dbg = 0
+        tried_count_dbg = 0
+        sent_count_dbg = 0
+        continuation_count_dbg = -1
+
+        if event_ids:
             path_dbg |= 0x00000001
-            events_to_reupload = self._reuploads.start_reupload()
-            self._reupload_events(events_to_reupload)
-            if self._logger.isEnabledFor(logging.INFO):
-                path_dbg |= 0x00000002
-                if self._reuploads.reuploading():
-                    path_dbg |= 0x00000004
-                    state_str = f"{self._reuploads.num_reupload_pending} reupload events pending."
-                else:
-                    path_dbg |= 0x00000008
-                    state_str = "reupload complete."
-                self._logger.info(
-                    f"_start_reupload: reuploaded {len(events_to_reupload)} events. "
-                    f"{state_str} "
-                    f"Total pending events: {self._event_persister.num_pending}."
-                )
+            sent_one = False
+            # Try to send all requested events. At least send must succeed to
+            # continue the reupload, so if all sends fail, get more until
+            # one is sent or there are no more reuploads.
+            while not sent_one and self._reuploads.reuploading() and event_ids:
+                continuation_path_dbg = 0x00000002
+                continuation_count_dbg += 1
+                next_event_ids = []
+                for event_id in event_ids:
+                    event_path_dbg = 0x00000004
+                    tried_count_dbg += 1
+                    problems = Problems()
+                    ret = self._reupload_event(event_id)
+                    if ret.is_ok():
+                        event_path_dbg |= 0x00000008
+                        if ret.value:
+                            path_dbg |= 0x00000010
+                            sent_count_dbg += 1
+                            sent_one = True
+                        else:
+                            event_path_dbg |= 0x00000020
+                            problems.add_error(DecodingError(uid=event_id))
+                    else:
+                        event_path_dbg |= 0x00000040
+                        problems.add_problems(ret.err())
+                    if problems:
+                        event_path_dbg |= 0x00000080
+                        # There was some error decoding this event.
+                        # We generate a new event with information
+                        # about decoding failure and delete this event.
+                        self.generate_event(
+                            problems.problem_event(
+                                f"Event decoding error - uid:{event_id}"
+                            )
+                        )
+                        self._event_persister.clear(event_id)
+                        if sent_one:
+                            event_path_dbg |= 0x00000100
+                            self._reuploads.clear_unacked_event(event_id)
+                        else:
+                            event_path_dbg |= 0x00000200
+                            next_event_ids.extend(
+                                self._reuploads.process_ack_for_reupload(event_id)
+                            )
+                    self._logger.path("  1 event path:0x%08X", event_path_dbg)
+                    continuation_path_dbg |= event_path_dbg
+                self._logger.path("  1 continuation path:0x%08X", continuation_path_dbg)
+                event_ids = next_event_ids
+                path_dbg |= continuation_path_dbg
         self._logger.path(
-            "--_start_reupload reuploading: %s  path:0x%08X",
-            self.reuploading(),
+            "--_continue_reupload  path:0x%08X  sent:%d  tried:%d  continuations:%d",
             path_dbg,
+            sent_count_dbg,
+            tried_count_dbg,
+            continuation_count_dbg,
         )
 
-    def _reupload_events(self, event_ids: list[str]) -> Result[bool, BaseException]:
-        errors = []
-        for message_id in event_ids:
-            match self._event_persister.retrieve(message_id):
-                case Ok(event_bytes):
-                    if event_bytes is None:
-                        errors.append(
-                            UIDMissingWarning("reupload_events", uid=message_id)
+    def _reupload_event(self, event_id) -> Result[bool, Problems]:
+        """Load event for event_id from storage, decoded to JSON and send it.
+
+        Return either Ok(True) or Err(Problems(list of decoding errors)).
+
+        Send errors handled either by exception, which will propagate up, or
+        by ack timeout.
+        """
+        self._logger.path("++_reupload_event  %s", event_id)
+        path_dbg = 0
+        problems = Problems()
+        match self._event_persister.retrieve(event_id):
+            case Ok(event_bytes):
+                path_dbg |= 0x00000001
+                if event_bytes is None:
+                    path_dbg |= 0x00000002
+                    problems.add_error(
+                        UIDMissingWarning("reupload_events", uid=event_id)
+                    )
+                elif len(event_bytes) == 0:
+                    path_dbg |= 0x00000004
+                    problems.add_error(
+                        FileEmptyWarning("reupload_events", uid=event_id)
+                    )
+                else:
+                    path_dbg |= 0x00000008
+                    try:
+                        event_str = event_bytes.decode(encoding=self.PERSISTER_ENCODING)
+                    except BaseException as e:
+                        path_dbg |= 0x00000010
+                        problems.add_error(e).add_error(
+                            ByteDecodingError("reupload_events", uid=event_id)
                         )
                     else:
+                        path_dbg |= 0x00000020
                         try:
-                            event = json.loads(
-                                event_bytes.decode(encoding=self.PERSISTER_ENCODING)
-                            )
+                            event = json.loads(event_str)
                         except BaseException as e:
-                            errors.append(e)
-                            errors.append(
-                                JSONDecodingError("reupload_events", uid=message_id)
+                            path_dbg |= 0x00000040
+                            problems.add_error(e).add_error(
+                                JSONDecodingError(
+                                    f"reupload_events - raw json:\n<\n{event_str}\n>",
+                                    uid=event_id,
+                                )
                             )
                         else:
+                            path_dbg |= 0x00000080
                             self.publish_upstream(event, AckRequired=True)
-                case Err(error):
-                    errors.append(error)
-        if errors:
-            return Err(Problems(errors=errors))
-        return Ok()
+                            self._logger.path(
+                                "--_reupload_event:1  path:0x%08X", path_dbg
+                            )
+                            return Ok(True)
+            case Err(error):
+                path_dbg |= 0x00000100
+                problems.add_problems(error)
+        self._logger.path("--_reupload_event:0  path:0x%08X", path_dbg)
+        return Err(problems)
 
     def start(
         self, loop: asyncio.AbstractEventLoop, async_queue: asyncio.Queue
     ) -> None:
+        if self.upstream_client:
+            self._reuploads.stats = self._stats.link(self.upstream_client)
         self._mqtt_clients.start(loop, async_queue)
         self.generate_event(StartupEvent())
         self._states.start_all()
 
     def stop(self) -> Result[bool, Problems]:
         problems: Optional[Problems] = None
         for link_name in self._states.link_names():
@@ -406,25 +490,19 @@
         path_dbg = 0
         wait_info = self._acks.cancel_ack_timer(link_name, message_id)
         if wait_info is not None and message_id in self._event_persister:
             path_dbg |= 0x00000001
             self._event_persister.clear(message_id)
             if self._reuploads.reuploading() and link_name == self.upstream_client:
                 path_dbg |= 0x00000002
-                reupload_now = self._reuploads.process_ack_for_reupload(message_id)
-                if reupload_now:
-                    path_dbg |= 0x00000004
-                    self._reupload_events(reupload_now)
-                self._logger.path(
-                    "events pending: %d  reupload pending: %d",
-                    self._event_persister.num_pending,
-                    self._reuploads.num_reupload_pending,
+                self._continue_reupload(
+                    self._reuploads.process_ack_for_reupload(message_id)
                 )
                 if not self._reuploads.reuploading():
-                    path_dbg |= 0x00000008
+                    path_dbg |= 0x00000004
                     self._logger.info("reupload complete.")
         self._logger.path("--LinkManager.process_ack path:0x%08X", path_dbg)
 
     def send_ack(self, link_name: str, message: Message[Any]) -> None:
         if message.Header.MessageId:
             self.publish_message(
                 link_name,
```

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/links/link_state.py` & `gridworks_proactor-0.4.4/src/gwproactor/links/link_state.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/links/message_times.py` & `gridworks_proactor-0.4.4/src/gwproactor/links/message_times.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/links/mqtt.py` & `gridworks_proactor-0.4.4/src/gwproactor/links/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/links/timer_interface.py` & `gridworks_proactor-0.4.4/src/gwproactor/links/timer_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/logger.py` & `gridworks_proactor-0.4.4/src/gwproactor/logger.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/logging_setup.py` & `gridworks_proactor-0.4.4/src/gwproactor/logging_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/message.py` & `gridworks_proactor-0.4.4/src/gwproactor/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/persister.py` & `gridworks_proactor-0.4.4/src/gwproactor/persister.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,29 +55,38 @@
 
 class TrimFailed(PersisterError): ...
 
 
 class ReindexError(PersisterError): ...
 
 
-class JSONDecodingError(PersisterException): ...
+class DecodingError(PersisterError): ...
+
+
+class ByteDecodingError(DecodingError): ...
+
+
+class JSONDecodingError(DecodingError): ...
 
 
 class UIDExistedWarning(PersisterWarning): ...
 
 
 class FileExistedWarning(PersisterWarning): ...
 
 
 class FileMissingWarning(PersisterWarning): ...
 
 
 class UIDMissingWarning(PersisterWarning): ...
 
 
+class FileEmptyWarning(PersisterWarning): ...
+
+
 class PersisterInterface(abc.ABC):
     @abstractmethod
     def persist(self, uid: str, content: bytes) -> Result[bool, Problems]:
         """Persist content, indexed by uid"""
 
     @abstractmethod
     def clear(self, uid: str) -> Result[bool, Problems]:
@@ -193,17 +202,18 @@
         max_bytes: int = DEFAULT_MAX_BYTES,
         pat_watchdog_args: Optional[list[str]] = None,
         reindex_pat_seconds=REINDEX_PAT_SECONDS,
     ):
         self._base_dir = Path(base_dir).resolve()
         self._max_bytes = max_bytes
         self._curr_dir = self._today_dir()
+        self._curr_bytes = 0
         self._pat_watchdog_args = pat_watchdog_args
         self._reindex_pat_seconds = reindex_pat_seconds
-        self.reindex()
+        self._pending = dict()
 
     @property
     def max_bytes(self) -> int:
         return self._max_bytes
 
     @property
     def curr_bytes(self) -> int:
```

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/proactor_implementation.py` & `gridworks_proactor-0.4.4/src/gwproactor/proactor_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     _name: str
     _settings: ProactorSettings
     _node: ShNode
     _layout: HardwareLayout
     _logger: ProactorLogger
     _stats: ProactorStats
     _event_persister: PersisterInterface
+    _reindex_problems: Optional[Problems] = None
     _loop: Optional[asyncio.AbstractEventLoop] = None
     _receive_queue: Optional[asyncio.Queue] = None
     _links: LinkManager
     _communicators: Dict[str, CommunicatorInterface]
     _stop_requested: bool
     _tasks: List[asyncio.Task]
     _io_loop_manager: IOLoop
@@ -109,14 +110,17 @@
                 )
             )
         self._layout = hardware_layout
         self._node = self._layout.node(name)
         self._logger = ProactorLogger(**settings.logging.qualified_logger_names())
         self._stats = self.make_stats()
         self._event_persister = self.make_event_persister(settings)
+        reindex_result = self._event_persister.reindex()
+        if reindex_result.is_err():
+            self._reindex_problems = reindex_result.err()
         self._links = LinkManager(
             publication_name=self.publication_name,
             settings=settings,
             logger=self._logger,
             stats=self._stats,
             event_persister=self._event_persister,
             timer_manager=AsyncioTimerManager(),
@@ -617,14 +621,19 @@
             f"Shutting down due to ShutdownMessage, [{message.Payload.Reason}]"
         )
 
     async def run_forever(self):
         self._loop = asyncio.get_running_loop()
         self._receive_queue = asyncio.Queue()
         self._links.start(self._loop, self._receive_queue)
+        if self._reindex_problems is not None:
+            self.generate_event(
+                self._reindex_problems.problem_event("Startup event reindex() problems")
+            )
+        self._reindex_problems = None
         for communicator in self._communicators.values():
             if isinstance(communicator, Runnable):
                 communicator.start()
         self.start_tasks()
         await self.join()
 
     def start(self):
```

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/proactor_interface.py` & `gridworks_proactor-0.4.4/src/gwproactor/proactor_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/problems.py` & `gridworks_proactor-0.4.4/src/gwproactor/problems.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/stats.py` & `gridworks_proactor-0.4.4/src/gwproactor/stats.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,25 +6,44 @@
 
 from gwproto import Message
 
 from gwproactor.message import MQTTReceiptPayload
 
 
 @dataclass
+class ReuploadCounts:
+    started: int = 0
+    completed: int = 0
+
+    def start(self):
+        self.started += 1
+
+    def complete(self):
+        self.completed += 1
+
+
+@dataclass
 class LinkStats:
     name: str
     num_received_by_type: dict[str, int] = field(
         default_factory=lambda: defaultdict(int)
     )
     num_received_by_topic: dict[str, int] = field(
         default_factory=lambda: defaultdict(int)
     )
     comm_event_counts: dict[str, int] = field(default_factory=lambda: defaultdict(int))
+    reupload_counts: ReuploadCounts = field(default_factory=ReuploadCounts)
     timeouts: int = 0
 
+    def start_reupload(self):
+        self.reupload_counts.start()
+
+    def complete_reupload(self):
+        self.reupload_counts.complete()
+
     @property
     def num_received(self) -> int:
         return self.num_received_by_type[Message.type_name()]
 
     def __str__(self) -> str:
         s = f"LinkStats [{self.name}]  num_received: {self.num_received}  timeouts: {self.timeouts}"
         if self.num_received_by_type:
@@ -35,20 +54,23 @@
             s += "\n  Received by topic:"
             for topic in sorted(self.num_received_by_topic):
                 s += f"\n    {self.num_received_by_topic[topic]:3d}: [{topic}]"
         if self.comm_event_counts:
             s += "\n  Comm event counts:"
             for comm_event in self.comm_event_counts:
                 s += f"\n    {self.comm_event_counts[comm_event]:3d}: [{comm_event}]"
+            s += f"\n    {self.reupload_counts.started:3d}: [reuploads_started]"
+            s += f"\n    {self.reupload_counts.completed:3d}: [reuploads_completed]"
         return s
 
 
 class ProactorStats:
     num_received_by_type: dict[str, int]
     num_received_by_topic: dict[str, int]
+    num_events_received: int = 0
     links: dict[str, LinkStats]
 
     def __init__(self, link_names: Optional[Sequence[str]] = None):
         self.num_received_by_type = defaultdict(int)
         self.num_received_by_topic = defaultdict(int)
         if link_names is None:
             link_names = []
@@ -61,14 +83,16 @@
 
     def add_mqtt_message(self, message: Message[MQTTReceiptPayload]) -> None:
         self.num_received_by_topic[message.Payload.message.topic] += 1
         link_stats = self.link(message.Payload.client_name)
         link_stats.num_received_by_type[Message.type_name()] += 1
         link_stats.num_received_by_type[message.Header.MessageType] += 1
         link_stats.num_received_by_topic[message.Payload.message.topic] += 1
+        if "gridworks-event" in message.Payload.message.topic:
+            self.num_events_received += 1
 
     def total_received(self, message_type: str) -> int:
         return self.num_received_by_type.get(message_type, 0)
 
     @property
     def num_received(self) -> int:
         return self.num_received_by_type[Message.type_name()]
@@ -89,11 +113,12 @@
 
     def __str__(self) -> str:
         s = "ProactorStats Stats\n"
         if self.num_received_by_type:
             s += "\nGlobal received by message_type:"
             for message_type in sorted(self.num_received_by_type):
                 s += f"\n    {self.num_received_by_type[message_type]:3d}: [{message_type}]"
+            s += f"\n    {self.num_events_received:3d}: [gridworks.event*]"
         for link_name in sorted(self.links):
             s += "\n"
             s += str(self.links[link_name])
         return s
```

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/str_tasks.py` & `gridworks_proactor-0.4.4/src/gwproactor/str_tasks.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/sync_thread.py` & `gridworks_proactor-0.4.4/src/gwproactor/sync_thread.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/watchdog.py` & `gridworks_proactor-0.4.4/src/gwproactor/watchdog.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor/web_manager.py` & `gridworks_proactor-0.4.4/src/gwproactor/web_manager.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/__init__.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/certs.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/certs.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/clean.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/clean.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/comm_test_helper.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/comm_test_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 
 from gwproactor import Proactor
 from gwproactor import ProactorSettings
 from gwproactor import setup_logging
+from gwproactor.config import DEFAULT_BASE_NAME
+from gwproactor.config import LoggingSettings
 from gwproactor.config import MQTTClient
 from gwproactor.config import Paths
 from gwproactor_test import copy_keys
 from gwproactor_test.certs import uses_tls
 from gwproactor_test.logger_guard import LoggerGuards
 from gwproactor_test.proactor_recorder import ProactorT
 from gwproactor_test.proactor_recorder import RecorderInterface
@@ -45,14 +47,16 @@
 
     parent_recorder_t: Callable[..., RecorderInterface] = None
     child_recorder_t: Callable[..., RecorderInterface] = None
 
     parent_helper: ProactorTestHelper
     child_helper: ProactorTestHelper
     verbose: bool
+    child_verbose: bool
+    parent_verbose: bool
     parent_on_screen: bool
     lifecycle_logging: bool
     logger_guards: LoggerGuards
 
     warn_if_multi_subscription_tests_skipped: bool = True
 
     @classmethod
@@ -63,14 +67,16 @@
             cls.child_recorder_t = make_recorder_class(cls.child_t)
 
     def __init__(
         self,
         child_settings: Optional[ChildSettingsT] = None,
         parent_settings: Optional[ParentSettingsT] = None,
         verbose: bool = False,
+        child_verbose: bool = False,
+        parent_verbose: bool = False,
         lifecycle_logging: bool = False,
         add_child: bool = False,
         add_parent: bool = False,
         start_child: bool = False,
         start_parent: bool = False,
         parent_on_screen: bool = False,
         child_name: str = "",
@@ -91,21 +97,28 @@
             ),
             dict() if child_kwargs is None else child_kwargs,
         )
         self.parent_helper = ProactorTestHelper(
             parent_name,
             parent_path_name,
             (
-                self.parent_settings_t(paths=Paths(name=Path(parent_path_name)))
+                self.parent_settings_t(
+                    logging=LoggingSettings(
+                        base_log_name=f"parent_{DEFAULT_BASE_NAME}"
+                    ),
+                    paths=Paths(name=Path(parent_path_name)),
+                )
                 if parent_settings is None
                 else parent_settings
             ),
             dict() if parent_kwargs is None else parent_kwargs,
         )
         self.verbose = verbose
+        self.child_verbose = child_verbose
+        self.parent_verbose = parent_verbose
         self.parent_on_screen = parent_on_screen
         self.lifecycle_logging = lifecycle_logging
         self.setup_logging()
         if add_child or start_child:
             self.add_child()
             if start_child:
                 self.start_child()
@@ -203,31 +216,30 @@
     def setup_logging(self):
         self.child_helper.settings.paths.mkdirs(parents=True)
         self.parent_helper.settings.paths.mkdirs(parents=True)
         errors = []
         if not self.lifecycle_logging:
             self.child_helper.settings.logging.levels.lifecycle = logging.WARNING
             self.parent_helper.settings.logging.levels.lifecycle = logging.WARNING
-        args = argparse.Namespace(verbose=self.verbose)
         self.logger_guards = LoggerGuards(
             list(self.child_helper.settings.logging.qualified_logger_names().values())
             + list(
                 self.parent_helper.settings.logging.qualified_logger_names().values()
             )
         )
         setup_logging(
-            args,
+            argparse.Namespace(verbose=self.verbose or self.child_verbose),
             self.child_helper.settings,
             errors,
             add_screen_handler=True,
             root_gets_handlers=False,
         )
         assert not errors
         setup_logging(
-            args,
+            argparse.Namespace(verbose=self.verbose or self.parent_verbose),
             self.parent_helper.settings,
             errors,
             add_screen_handler=self.parent_on_screen,
             root_gets_handlers=False,
         )
         assert not errors
```

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/config/hardware-layout.json` & `gridworks_proactor-0.4.4/src/gwproactor_test/config/hardware-layout.json`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/dummies/__init__.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/dummies/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/dummies/child/config.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/dummies/child/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/dummies/child/dummy.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/dummies/child/dummy.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/dummies/parent/config.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/dummies/parent/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/dummies/parent/dummy.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/dummies/parent/dummy.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/logger_guard.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/logger_guard.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/proactor_recorder.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/proactor_recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,19 +244,15 @@
             s = str(self.stats)
             s += "\nLink states:\n"
             for link_name in self.stats.links:
                 s += f"  {link_name:10s}  {self._links.link_state(link_name).value}\n"
             s += "Pending acks:\n"
             for link_name in self.stats.links:
                 s += f"  {link_name:10s}  {self._links.num_acks(link_name):3d}\n"
-            s += (
-                f"pending events: {self._links.num_pending}  "
-                f"pending upload events: {self._links.num_reupload_pending}  "
-                f"reuploading: {self._links.reuploading()}\n"
-            )
+            s += self._links.get_reuploads_str() + "\n"
             s += f"subacks_paused: {self.subacks_paused}  pending_subacks: {len(self.pending_subacks)}\n"
             return s
 
         def summarize(self: ProactorT) -> None:
             self._logger.info(self.summary_str())
 
         def ping_peer(self) -> None:
```

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/proactor_test_collections.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/proactor_test_collections.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,107 @@
 import asyncio
 import logging
 import time
 import warnings
+from dataclasses import dataclass
+from pathlib import Path
 from typing import Type
 
 import pytest
 from gwproto import MQTTTopic
 from paho.mqtt.client import MQTT_ERR_CONN_LOST
 
+from gwproactor import ServicesInterface
 from gwproactor.links import StateName
 from gwproactor.message import DBGEvent
 from gwproactor.message import DBGPayload
+from gwproactor.persister import TimedRollingFilePersister
 from gwproactor_test.certs import uses_tls
 from gwproactor_test.comm_test_helper import CommTestHelper
 from gwproactor_test.wait import await_for
 
 
+@dataclass
+class _EventEntry:
+    uid: str
+    path: Path
+
+
+class _EventGen:
+    ok: list[_EventEntry]
+    corrupt: list[_EventEntry]
+    empty: list[_EventEntry]
+    missing: list[_EventEntry]
+
+    persister: TimedRollingFilePersister
+
+    def __len__(self) -> int:
+        return len(self.ok) + len(self.corrupt) + len(self.empty)
+
+    def __init__(self, proactor: ServicesInterface):
+        self.ok = []
+        self.corrupt = []
+        self.empty = []
+        self.missing = []
+        persister = proactor._event_persister  # noqa
+        assert isinstance(persister, TimedRollingFilePersister)
+        self.persister = persister
+
+    def _generate_event(self, member_name: str) -> _EventEntry:
+        event = DBGEvent(Command=DBGPayload(), Msg=f"event {len(self)} {member_name}")
+        ret = self.persister.persist(
+            event.MessageId, event.json(sort_keys=True, indent=2).encode()
+        )
+        if ret.is_err():
+            raise ret.err()
+        entry = _EventEntry(
+            event.MessageId, self.persister.get_path(event.MessageId)  # noqa
+        )
+        getattr(self, member_name).append(entry)
+        return entry
+
+    def _generate_ok(self) -> _EventEntry:
+        return self._generate_event("ok")
+
+    def _generate_corrupt(self) -> _EventEntry:
+        entry = self._generate_event("corrupt")
+        with entry.path.open() as f:
+            contents = f.read()
+        with entry.path.open("w") as f:
+            f.write(contents[:-6])
+        return entry
+
+    def _generate_empty(self) -> _EventEntry:
+        entry = self._generate_event("empty")
+        with entry.path.open("w") as f:
+            f.write("")
+        return entry
+
+    def _generate_missing(self) -> _EventEntry:
+        entry = self._generate_event("missing")
+        entry.path.unlink()
+        return entry
+
+    def generate(
+        self,
+        num_ok: int = 0,
+        num_corrupt: int = 0,
+        num_empty: int = 0,
+        num_missing: int = 0,
+    ):
+        for _ in range(num_ok):
+            self._generate_ok()
+        for _ in range(num_corrupt):
+            self._generate_corrupt()
+        for _ in range(num_empty):
+            self._generate_empty()
+        for _ in range(num_missing):
+            self._generate_missing()
+
+
 @pytest.mark.asyncio
 class ProactorCommTests:
     CTH: Type[CommTestHelper]
 
     async def test_no_parent(self):
         async with self.CTH(add_child=True) as h:
             child = h.child
@@ -1138,38 +1220,41 @@
             start_child=True,
             add_parent=True,
             verbose=False,
         ) as h:
             child = h.child
             child.disable_derived_events()
             upstream_link = h.child._links.link(child.upstream_client)
+            reupload_counts = h.child.stats.link(child.upstream_client).reupload_counts
             await await_for(
                 lambda: child.mqtt_quiescent(),
                 1,
                 "ERROR waiting for child to connect to mqtt",
                 err_str_f=h.summary_str,
             )
             # Some events should have been generated, and they should have all been sent
             assert child._links.num_pending > 0
             assert child._links.num_reupload_pending == 0
             assert child._links.num_reuploaded_unacked == 0
             assert not child._links.reuploading()
+            assert reupload_counts.started == 0
+            assert reupload_counts.completed == 0
 
             # Start parent, wait for reconnect.
             h.start_parent()
             await await_for(
                 lambda: upstream_link.active(),
                 1,
                 "ERROR waiting for parent",
                 err_str_f=h.summary_str,
             )
 
             # Wait for reuploading to complete
             await await_for(
-                lambda: not child._links.reuploading(),
+                lambda: reupload_counts.completed > 0,
                 1,
                 "ERROR waiting for re-upload to complete",
                 err_str_f=h.summary_str,
             )
 
             # All events should have been reuploaded.
             assert child._links.num_reupload_pending == 0
@@ -1187,14 +1272,15 @@
             add_parent=True,
             child_settings=self.CTH.child_settings_t(num_initial_event_reuploads=5),
             verbose=False,
         ) as h:
             child = h.child
             child.disable_derived_events()
             upstream_link = h.child._links.link(child.upstream_client)
+            reupload_counts = h.child.stats.link(child.upstream_client).reupload_counts
             await await_for(
                 lambda: child.mqtt_quiescent(),
                 1,
                 "ERROR waiting for child to connect to mqtt",
                 err_str_f=h.summary_str,
             )
             # Some events should have been generated, and they should have all been sent
@@ -1223,17 +1309,17 @@
                 1,
                 "ERROR waiting for parent",
                 err_str_f=h.summary_str,
             )
 
             # Wait for reupload to complete
             await await_for(
-                lambda: not child._links.reuploading(),
+                lambda: reupload_counts.completed > 0,
                 1,
-                "ERROR waiting for reupload",
+                "ERROR waiting for reupload to complete",
                 err_str_f=h.summary_str,
             )
 
     @pytest.mark.asyncio
     async def test_reupload_flow_control_detail(self):
         """
         Test:
@@ -1400,7 +1486,65 @@
                 #     f" loop_path_dbg: 0x{loop_path_dbg:08X}")
 
                 last_num_to_reupload = curr_num_to_reuplad
                 last_num_reuploaded_unacked = curr_num_reuploaded_unacked
                 last_num_repuload_pending = curr_num_repuload_pending
 
             assert not child_links.reuploading()
+
+    @pytest.mark.asyncio
+    async def test_reupload_errors(self):
+        async with self.CTH(
+            start_child=True,
+            add_parent=True,
+            child_verbose=False,
+        ) as h:
+            child = h.child
+            child.disable_derived_events()
+            reupload_counts = h.child.stats.link(child.upstream_client).reupload_counts
+            child_links = h.child._links
+            upstream_link = child_links.link(child.upstream_client)
+            parent = h.parent
+
+            def _err_str() -> str:
+                return (
+                    f"\nCHILD\n{child.summary_str()}\n"
+                    f"\nPARENT\n{parent.summary_str()}\n"
+                )
+
+            await await_for(
+                lambda: child.mqtt_quiescent(),
+                1,
+                "ERROR waiting for child to connect to mqtt",
+                err_str_f=_err_str,
+            )
+            base_num_pending = child_links.num_pending
+            assert base_num_pending > 0
+            assert child_links.num_reupload_pending == 0
+            assert child_links.num_reuploaded_unacked == 0
+            assert not child_links.reuploading()
+
+            generator = _EventGen(child)
+            generator.generate(num_corrupt=10)
+            generator.generate(num_ok=10)
+            generator.generate(num_empty=10)
+            generator.generate(num_ok=10)
+            generator.generate(num_missing=10)
+            generator.generate(num_ok=10)
+
+            h.start_parent()
+            await await_for(
+                lambda: upstream_link.active(),
+                1,
+                "ERROR waiting for active",
+                err_str_f=_err_str,
+            )
+
+            # Wait for reupload to complete
+            await await_for(
+                lambda: reupload_counts.completed > 0,
+                3,
+                "ERROR waiting for reupload to complete",
+                err_str_f=_err_str,
+            )
+            assert reupload_counts.started == reupload_counts.completed
+            assert parent.stats.num_events_received >= base_num_pending + 60
```

### Comparing `gridworks_proactor-0.4.3/src/gwproactor_test/wait.py` & `gridworks_proactor-0.4.4/src/gwproactor_test/wait.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.3/PKG-INFO` & `gridworks_proactor-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-proactor
-Version: 0.4.3
+Version: 0.4.4
 Summary: Gridworks Proactor
 Home-page: https://github.com/thegridelectric/gridworks-proactor
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: tests
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: gridworks-cert (>=0.4.2) ; extra == "tests"
 Requires-Dist: gridworks-protocol (>=0.7.4,<0.8.0)
 Requires-Dist: multidict (>=6.0.4,<7.0.0)
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
+Requires-Dist: pendulum (==2.1.2)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pytest (>=7.2.0) ; extra == "tests"
 Requires-Dist: pytest-asyncio (>=0.20.3) ; extra == "tests"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: result (>=0.9.0,<0.10.0)
 Requires-Dist: xdg (>=6.0.0,<7.0.0)
 Requires-Dist: yarl (>=1.9.2,<2.0.0)
```


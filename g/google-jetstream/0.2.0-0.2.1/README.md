# Comparing `tmp/google-jetstream-0.2.0.tar.gz` & `tmp/google_jetstream-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-jetstream-0.2.0.tar", last modified: Fri Apr  5 20:27:53 2024, max compression
+gzip compressed data, was "google_jetstream-0.2.1.tar", last modified: Fri May  3 21:42:43 2024, max compression
```

## Comparing `google-jetstream-0.2.0.tar` & `google_jetstream-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,61 @@
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.955054 google-jetstream-0.2.0/
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)       10 2024-02-25 02:26:58.000000 google-jetstream-0.2.0/AUTHORS
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)    11358 2024-02-25 01:51:15.000000 google-jetstream-0.2.0/LICENSE
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)       23 2024-04-05 20:24:22.000000 google-jetstream-0.2.0/MANIFEST.in
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)    12231 2024-04-05 20:27:53.955054 google-jetstream-0.2.0/PKG-INFO
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)    11508 2024-04-05 20:24:22.000000 google-jetstream-0.2.0/README.md
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.951054 google-jetstream-0.2.0/google_jetstream.egg-info/
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)    12231 2024-04-05 20:27:53.000000 google-jetstream-0.2.0/google_jetstream.egg-info/PKG-INFO
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1133 2024-04-05 20:27:53.000000 google-jetstream-0.2.0/google_jetstream.egg-info/SOURCES.txt
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)        1 2024-04-05 20:27:53.000000 google-jetstream-0.2.0/google_jetstream.egg-info/dependency_links.txt
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)       54 2024-04-05 20:27:53.000000 google-jetstream-0.2.0/google_jetstream.egg-info/requires.txt
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)       10 2024-04-05 20:27:53.000000 google-jetstream-0.2.0/google_jetstream.egg-info/top_level.txt
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.943053 google-jetstream-0.2.0/jetstream/
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/__init__.py
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.947053 google-jetstream-0.2.0/jetstream/core/
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/__init__.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     5185 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/config_lib.py
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.947053 google-jetstream-0.2.0/jetstream/core/implementations/
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/implementations/__init__.py
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.947053 google-jetstream-0.2.0/jetstream/core/implementations/mock/
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/implementations/mock/__init__.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)      993 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/implementations/mock/config.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1512 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/implementations/mock/server.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)    25986 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/orchestrator.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     3401 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/orchestrator_test.py
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.947053 google-jetstream-0.2.0/jetstream/core/proto/
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/proto/__init__.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2273 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/proto/jetstream_pb2.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     3182 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/proto/jetstream_pb2_grpc.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     4623 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/server_lib.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2857 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/server_test.py
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.951054 google-jetstream-0.2.0/jetstream/core/utils/
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/utils/__init__.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     3357 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/utils/async_multifuture.py
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.951054 google-jetstream-0.2.0/jetstream/engine/
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/__init__.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     7096 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/engine_api.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     9214 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/mock_engine.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     3896 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/mock_engine_test.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2792 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/mock_utils.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     6814 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/token_utils.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1840 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/tokenizer_pb2.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)      755 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/tokenizer_pb2_grpc.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2823 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/utils_test.py
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)       53 2024-04-05 19:41:14.000000 google-jetstream-0.2.0/requirements.in
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)       38 2024-04-05 20:27:53.955054 google-jetstream-0.2.0/setup.cfg
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1592 2024-04-05 20:24:22.000000 google-jetstream-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.068576 google_jetstream-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/google_jetstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-03 21:42:43.000000 google_jetstream-0.2.1/google_jetstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-03 21:42:43.000000 google_jetstream-0.2.1/google_jetstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:42:43.000000 google_jetstream-0.2.1/google_jetstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 21:42:43.000000 google_jetstream-0.2.1/google_jetstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 21:42:43.000000 google_jetstream-0.2.1/google_jetstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.060576 google_jetstream-0.2.1/jetstream/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.060576 google_jetstream-0.2.1/jetstream/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/config_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.060576 google_jetstream-0.2.1/jetstream/core/implementations/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/implementations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/core/implementations/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/implementations/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/implementations/mock/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/implementations/mock/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/core/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/proto/jetstream_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/proto/jetstream_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/server_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/utils/async_multifuture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/engine_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/mock_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12697 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/token_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/tokenizer_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/tokenizer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/tokenizer_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/core/test_config_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/core/test_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/core/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/engine/test_mock_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/engine/test_token_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/engine/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/third_party/llama3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/third_party/llama3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/third_party/llama3/llama3_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 21:42:43.068576 google_jetstream-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/setup.py
```

### Comparing `google-jetstream-0.2.0/LICENSE` & `google_jetstream-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/google_jetstream.egg-info/SOURCES.txt` & `google_jetstream-0.2.1/google_jetstream.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,28 +9,37 @@
 google_jetstream.egg-info/dependency_links.txt
 google_jetstream.egg-info/requires.txt
 google_jetstream.egg-info/top_level.txt
 jetstream/__init__.py
 jetstream/core/__init__.py
 jetstream/core/config_lib.py
 jetstream/core/orchestrator.py
-jetstream/core/orchestrator_test.py
 jetstream/core/server_lib.py
-jetstream/core/server_test.py
 jetstream/core/implementations/__init__.py
 jetstream/core/implementations/mock/__init__.py
 jetstream/core/implementations/mock/config.py
 jetstream/core/implementations/mock/server.py
 jetstream/core/proto/__init__.py
 jetstream/core/proto/jetstream_pb2.py
 jetstream/core/proto/jetstream_pb2_grpc.py
 jetstream/core/utils/__init__.py
 jetstream/core/utils/async_multifuture.py
 jetstream/engine/__init__.py
 jetstream/engine/engine_api.py
 jetstream/engine/mock_engine.py
-jetstream/engine/mock_engine_test.py
 jetstream/engine/mock_utils.py
 jetstream/engine/token_utils.py
+jetstream/engine/tokenizer_api.py
 jetstream/engine/tokenizer_pb2.py
 jetstream/engine/tokenizer_pb2_grpc.py
-jetstream/engine/utils_test.py
+jetstream/tests/__init__.py
+jetstream/tests/core/__init__.py
+jetstream/tests/core/test_config_lib.py
+jetstream/tests/core/test_orchestrator.py
+jetstream/tests/core/test_server.py
+jetstream/tests/engine/__init__.py
+jetstream/tests/engine/test_mock_engine.py
+jetstream/tests/engine/test_token_utils.py
+jetstream/tests/engine/test_utils.py
+jetstream/third_party/__init__.py
+jetstream/third_party/llama3/__init__.py
+jetstream/third_party/llama3/llama3_tokenizer.py
```

### Comparing `google-jetstream-0.2.0/jetstream/__init__.py` & `google_jetstream-0.2.1/jetstream/__init__.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/core/__init__.py` & `google_jetstream-0.2.1/jetstream/core/__init__.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/core/config_lib.py` & `google_jetstream-0.2.1/jetstream/core/config_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Configs of engines for the orchestrator to load."""
 
 import dataclasses
 import functools
-import math
 from typing import Any, Callable, List, Tuple, Type
 
 from jetstream.engine import engine_api
 from jetstream.engine import mock_engine
 
 
 Devices = Any
@@ -81,19 +80,20 @@
   )
 
 
 # ▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼#
 
 
 def slice_to_num_chips(s: str) -> int:
-  """Converts a TPU spec like v5e=4x2 to the number of chips, 8."""
-  # Account for the case where it is written 'v5e:4x2'.
-  delim = "=" if "=" in s else ":"
-  i = math.prod([int(c) for c in s.split(delim)[1].split("x")])
-  return i
+  """Converts a TPU spec like v5e-8 or v5e=8 to the number of chips, 8."""
+  # Account for the case where it is written 'tpu=8' for compatibility.
+  delim = "-" if "-" in s else "="
+  # TODO: Support more accelerator type check.
+  accelerator_type, num_devices = s.split(delim)
+  return int(num_devices) if accelerator_type != "v4" else int(num_devices) // 2
 
 
 def _split_devices_by_slices(
     devices: list[Devices], slices: list[int]
 ) -> List[List[Devices]]:
   """Converts an ordered list of devices into slices."""
   assert sum(slices) == len(devices), f"{sum(slices)} != {len(devices)}"
```

### Comparing `google-jetstream-0.2.0/jetstream/core/implementations/__init__.py` & `google_jetstream-0.2.1/jetstream/core/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/core/implementations/mock/__init__.py` & `google_jetstream-0.2.1/jetstream/core/implementations/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/core/implementations/mock/config.py` & `google_jetstream-0.2.1/jetstream/core/implementations/mock/config.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/core/implementations/mock/server.py` & `google_jetstream-0.2.1/jetstream/core/implementations/mock/server.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/core/orchestrator.py` & `google_jetstream-0.2.1/jetstream/core/orchestrator.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 
 import grpc
 import jax
 from jetstream.core.proto import jetstream_pb2
 from jetstream.core.proto import jetstream_pb2_grpc
 from jetstream.core.utils import async_multifuture
 from jetstream.engine import engine_api
-from jetstream.engine import token_utils
 import numpy as np
 
 
 root = logging.getLogger()
 root.setLevel(logging.DEBUG)
 
 handler = logging.StreamHandler(sys.stdout)
@@ -123,27 +122,27 @@
   """Current state of the driver."""
 
   #################### Information relevant for generation #####################
   max_tokens: int
   # We keep prefill and decode information together in the same object so that
   # there is less indirection about where this return channel is.
   # The return channel returns a list of strings, one per sample for that query.
-  return_channel: async_multifuture.AsyncMultifuture[list[str]]
+  return_channel: async_multifuture.AsyncMultifuture[list[list[int]]]
   # [num_samples,] which corresponds to whether each sample is complete for the
   # requests.
   complete: Optional[np.ndarray] = None
   prefill_result: Any = None
   #################### Information relevant for prefill ########################
   history_path: Optional[str] = None
   prefill_text: Optional[str] = None
   ################## Information relevant for detokenization ###################
   # Which generate step this was added at.
   generate_timestep_added: Optional[int] = None
 
-  def enqueue_tokens(self, generated_tokens: list[str]):
+  def enqueue_tokens(self, generated_tokens: list[list[int]]):
     """Records information about the step.
 
     Args:
       generated_tokens: One token to put into the return channel
 
     This should be called only from within the Drivers background thread.
     """
@@ -185,32 +184,43 @@
   # Allows us to pre-load the params, primarily so that we can iterate quickly
   # on the driver in colab without reloading weights.
   _prefill_params: list[Any]
   _generate_params: list[Any]
   # Stage 1
   _prefill_backlog: queue.Queue[ActiveRequest | None]
   # Stage 2
+  _transfer_backlogs: list[queue.Queue[ActiveRequest]] = []
+  # Stage 3
   # We keep this as a dict to avoid a possibly expensive object comparison
   # when logging the index of the generate engine we send a prefill result
   # to, it allows us to natively have the index from the min operation, rather
   # than have to call .index()
-  _generate_backlogs: dict[int, queue.Queue[ActiveRequest | None]] = {}
-  # Stage 3
+  _generate_backlogs: dict[int, queue.Queue[ActiveRequest]] = {}
+  # Stage 4
   # This can be a list because we can pass it as an arg to generate and
   # detokenize threads. It is a list of tokens to be detokenized.
   _detokenize_backlogs: list[queue.Queue[engine_api.ResultTokens]] = []
   _generate_slots: list[queue.Queue[int]] = []
-  _active_requests: list[queue.Queue[tuple[int, ActiveRequest | None]]] = []
+  _active_requests: list[queue.Queue[tuple[int, ActiveRequest]]] = []
+
+  # For interleaved_mode, only generate if all slots are full
+  # or corresponding prefill queue is empty.
+  _interleaved_mode: bool = False
+
+  # todo: remove jax_padding after all then engine migrate to np padding
+  _jax_padding = True
 
   def __init__(
       self,
       prefill_engines: Optional[list[engine_api.Engine]] = None,
       generate_engines: Optional[list[engine_api.Engine]] = None,
       prefill_params: Optional[list[Any]] = None,
       generate_params: Optional[list[Any]] = None,
+      interleaved_mode: bool = False,
+      jax_padding: bool = True,
   ):
     if prefill_engines is None:
       prefill_engines = []
     if generate_engines is None:
       generate_engines = []
     if prefill_params is None:
       prefill_params = []
@@ -222,30 +232,47 @@
         len(prefill_engines),
         len(generate_engines),
     )
     self._prefill_engines = prefill_engines
     self._generate_engines = generate_engines
     self._prefill_params = prefill_params
     self._generate_params = generate_params
+    self._interleaved_mode = interleaved_mode
+
     # Stages 1-4 represent the life cycle of a request.
     # Stage 1
     # At first, a request is placed here in order to get prefilled.
     self._prefill_backlog = queue.Queue()
-    # _ready_to_prefill event will block the prefill thread until there is
-    # available decode slot to insert the prefill result.
-    self._ready_to_prefill = threading.Event()
     # Stage 2
+    # After prefilling, it is placed here in order to get transferred to
+    # one of the generate backlogs.
+    # Interleaved Mode: Max size is 1 to increase the HBM utilization
+    # during generate.
+    # Disaggregated Mode: Max size is 4 to allow for 2 prefills to be enqueued
+    # while 1 transfer is enqueued while 1 is being transferred.
+    # TODO: Make queue size configurable.
+    self._transfer_backlogs = [
+        queue.Queue(1 if self._interleaved_mode else 4)
+        for i in range(len(self._prefill_engines))
+    ]
+    # Stage 3
     # Each generate engine accesses its own generate backlog.
+    # Interleaved Mode: Max size is 1 to increase the HBM utilization
+    # during generate.
+    # Disaggregated Mode: Set as 1/3 the number of concurrent decodes.
+    # TODO: Calculate the backlog to saturate the generate engine while
+    # minimizing the memory usage for disaggregated mode.
+    # TODO: Make queue size configurable.
     self._generate_backlogs = {
-        # Don't receive more than 1/3 the number of concurrent decodes to avoid
-        # OOM for single host.
-        idx: queue.Queue(engine.max_concurrent_decodes // 3)
+        idx: queue.Queue(
+            1 if self._interleaved_mode else engine.max_concurrent_decodes // 3
+        )
         for idx, engine in enumerate(self._generate_engines)
     }
-    # Stage 3
+    # Stage 4
     # After generation, ActiveRequests are placed on the detokenization backlog
     # for tokens to be sent into each ActiveRequest's return channel.
     # We have one of these per generate engine to simplify the logic keeping
     # track of which generation engine to replace slots on.
     # This is a queue of either - tuple[int, ActiveRequest] which represents our
     # active requests, or tuple[int, sample_tokens]. We combine these into one
     # queue because it allows us to be somewhat clever with how we do
@@ -279,29 +306,44 @@
         [
             self._generate_slots[idx].put(i)
             for i in range(engine.max_concurrent_decodes)
         ]
         for idx, engine in enumerate(self._generate_engines)
     ]
 
+    self._jax_padding = jax_padding
+
     # Create all threads
     self._prefill_threads = [
         JetThread(
             target=functools.partial(self._prefill_thread, idx),
             name=f"prefill-{idx}",
+            daemon=True,
+        )
+        for idx in range(len(self._prefill_engines))
+    ]
+    self._transfer_threads = [
+        JetThread(
+            target=functools.partial(
+                self._transfer_thread,
+                idx,
+            ),
+            name=f"transfer-{idx}",
+            daemon=True,
         )
         for idx in range(len(self._prefill_engines))
     ]
     self._generate_threads = [
         JetThread(
             target=functools.partial(
                 self._generate_thread,
                 idx,
             ),
             name=f"generate-{idx}",
+            daemon=True,
         )
         for idx in range(len(self._generate_engines))
     ]
     self.detokenize_threads = [
         JetThread(
             target=functools.partial(
                 self._detokenize_thread,
@@ -310,14 +352,15 @@
             name=f"detokenize-{idx}",
         )
         for idx in range(len(self._generate_engines))
     ]
     self._all_threads = list(
         itertools.chain(
             self._prefill_threads,
+            self._transfer_threads,
             self._generate_threads,
             self.detokenize_threads,
         )
     )
     self.live = True
     # Start all threads
     for t in self._all_threads:
@@ -327,14 +370,15 @@
     """Stops the driver and all background threads."""
     # Signal to all threads that they should stop.
     self.live = False
 
     all_backlogs = list(
         itertools.chain(
             [self._prefill_backlog],
+            self._transfer_backlogs,
             self._generate_backlogs.values(),
             self._detokenize_backlogs,
         )
     )
 
     while any(t.is_alive() for t in self._all_threads):
       # Empty all backlogs and mark any remaining requests as cancelled.
@@ -387,81 +431,108 @@
 
   def _prefill_thread(self, idx: int):
     """Thread which runs in the background performing prefills."""
     logging.info("---------Spinning up prefill thread %d.---------", idx)
     prefill_engine = self._prefill_engines[idx]
     prefill_params = self._prefill_params[idx]
     metadata = prefill_engine.get_tokenizer()
-    vocab = token_utils.load_vocab(metadata.path, metadata.extra_ids)
+    tokenizer = prefill_engine.build_tokenizer(metadata)
     logging.info("---------Prefill params %d loaded.---------", idx)
 
     while self.live:
-      # The prefill thread can wait until there is available decode slot to
-      # insert.
-      if self._generate_slots[idx].qsize() == 0:
-        logging.info(
-            "Prefill waits for available slot; prefill queue size %d",
-            self._prefill_backlog.qsize(),
-        )
-        self._ready_to_prefill.wait()
-        logging.info(
-            "Prefill continues; prefill queue size %d",
-            self._prefill_backlog.qsize(),
-        )
+      my_transfer_backlog = self._transfer_backlogs[idx]
       # The prefill thread can just sleep until it has work to do.
       request = self._prefill_backlog.get(block=True)
       if request is None:
         break
-      # TODO: Implement hot/cold cache for history.
-      history = self._load_cache_history(request.history_path)  # pylint: disable = assignment-from-none
       # Tokenize, and introduce a leading dimension
       is_bos = not bool(request.history_path)
       logging.info(
           "Prefilling on prefill engine %d : prefill queue size, %d,"
           " is_bos: %s, history: %s",
           idx,
           self._prefill_backlog.qsize(),
           is_bos,
           request.history_path,
       )
-      padded_tokens, true_length = token_utils.tokenize_and_pad(
+      padded_tokens, true_length = tokenizer.encode(
           request.prefill_text,
-          vocab,
           is_bos=is_bos,
           max_prefill_length=prefill_engine.max_prefill_length,
+          jax_padding=self._jax_padding,
       )
-      # Compute new kv cache for the prefill_text, conditional on
-      # history.
+      # Compute new kv cache for the prefill_text.
       prefill_result = prefill_engine.prefill(
           params=prefill_params,
-          existing_prefix=history,
           padded_tokens=padded_tokens,
           true_length=true_length,
       )
       request.prefill_result = prefill_result
       # Once prefill is complete, place it on the generation queue and block if
       # full.
-      self._generate_backlogs[idx].put(request, block=True)
+      my_transfer_backlog.put(request, block=True)
+      logging.info(
+          "Placed request on transfer queue %d, %d queued requests.",
+          idx,
+          my_transfer_backlog.qsize(),
+      )
+      del prefill_result
+      del request
+
+  def _transfer_thread(self, idx: int):
+    """Transfers the kv cache on an active request to the least full
+    generate backlog."""
+    transfer_backlog = self._transfer_backlogs[idx]
+
+    while self.live:
+      # The transfer thread can just sleep until it has work to do.
+      new_request = transfer_backlog.get(block=True)
+      target_idx = min(
+          self._generate_backlogs.items(), key=lambda q: q[1].qsize()
+      )[0]
+      # Only transfer the KVCache for the disaggregated serving.
+      # TODO: Remove the conditional after fixing the compatibility.
+      if not self._interleaved_mode:
+        logging.info(
+            "Transferring prefill from prefill engine %d "
+            "to generate engine %d.",
+            idx,
+            target_idx,
+        )
+        # Transfer the info to the relevant generate slice.
+        new_request.prefill_result = jax.device_put(
+            new_request.prefill_result,
+            self._generate_engines[
+                target_idx
+            ].get_prefix_destination_sharding(),
+        )
+        # Block here so we don't block on the generate thread that steps.
+        jax.block_until_ready(new_request.prefill_result)
+      # Place the request on the correct generate backlog and block if full.
+      self._generate_backlogs[target_idx].put(new_request, block=True)
       logging.info(
-          "Placed request on the generate queue, generate_backlogs=%d",
-          self._generate_backlogs[idx].qsize(),
+          "Successfully transferred prefill "
+          "from prefill engine %d to generate engine %d.",
+          idx,
+          target_idx,
       )
 
   def _generate_thread(self, idx: int):
     """Step token generation and insert prefills from backlog."""
     logging.info("---------Spinning up generate thread %d.---------", idx)
     generate_engine = self._generate_engines[idx]
     my_slots = self._generate_slots[idx]
     my_generate_backlog = self._generate_backlogs[idx]
     my_detokenize_backlog = self._detokenize_backlogs[idx]
 
     # Keep track of what step tokens were generated at.
     generate_timestep = 0
     # State to store things like running kv cache in.
     decode_state = generate_engine.init_decode_state()
+
     generate_params = self._generate_params[idx]
     logging.info("---------Generate params %d loaded.---------", idx)
     time_of_last_generate = time.time()
     time_of_last_print = time.time()
     while self.live:
       if (time.time() - time_of_last_print) > 1:
         logging.info(
@@ -471,15 +542,14 @@
             self._prefill_backlog.qsize(),
             my_slots.qsize(),
         )
         time_of_last_print = time.time()
 
       max_concurrent_decodes = generate_engine.max_concurrent_decodes
 
-      # TODO: Move insert to prefill thread.
       # Check if there are any free my_slots. We don't want to block here since
       # we can still generate if we can't insert. We do this in a while loop to
       # insert as many sequences as possible.
       while True:
         my_slots_size = my_slots.qsize()
 
         try:
@@ -490,14 +560,19 @@
           break
 
         # We block when the decode slots are all free since we need to get a
         # prefilled request to insert. We add timeout for the block to handle
         # the case when the prefill backlog is cancelled and we end up with no
         # more useful prefill work to do.
         block = my_slots_size == max_concurrent_decodes
+        if self._interleaved_mode:
+          # For interleaved mode, we also blocks when prefill backlog
+          # is not empty or there are transfer work to do.
+          block |= not self._prefill_backlog.empty()
+          block |= not self._transfer_backlogs[idx].empty()
         try:
           new_request = my_generate_backlog.get(block=block, timeout=1.0)
           # Got free slot and new request, use them.
         except queue.Empty:
           # No new requests, we can't insert, so put back slot.
           my_slots.put(slot, block=False)
           # If we were blocking and hit the timeout, then retry the loop.
@@ -557,16 +632,15 @@
     # For all filled my_slots, pop the sampled token onto the relevant
     # requests return channel. If it done, place it back onto free slots.
     my_detokenize_backlog = self._detokenize_backlogs[idx]
     my_generate_engine = self._generate_engines[idx]
     my_slots = self._generate_slots[idx]
 
     metadata = my_generate_engine.get_tokenizer()
-    vocab = token_utils.load_vocab(metadata.path, metadata.extra_ids)
-
+    tokenizer = my_generate_engine.build_tokenizer(metadata)
     my_live_requests = {
         i: None for i in range(my_generate_engine.max_concurrent_decodes)
     }
     while self.live:
       data = my_detokenize_backlog.get(block=True)
       if data is None:
         break
@@ -576,30 +650,28 @@
         generate_timestep_added, result_tokens = data
         # Disable attribute error because pytype doesn't know this
         # is a result tokens, and we can't annotate the tuple.
         result_tokens = result_tokens.convert_to_numpy()
 
         for slot, request in my_live_requests.items():
           if request is not None:
-            results, complete = token_utils.process_result_tokens(
+            results, complete = tokenizer.decode(
                 slot=slot,
                 slot_max_length=request.max_tokens,
                 result_tokens=result_tokens,
-                vocab=vocab,
                 complete=request.complete,
             )
             request.complete = complete
             # Return some tokens.
             request.enqueue_tokens(results)
             if request.complete.all():
               request.return_channel.close()
               # Place the slot back on the free queue.
               my_live_requests[slot] = None
               my_slots.put(slot, block=False)  # This should always have space.
-              self._ready_to_prefill.set()
         logging.info(
             "Detokenizing generate step %d took %.2fms",
             generate_timestep_added,
             (time.time() - start_detokenize_time) * 10**3,
         )
       else:
         # We want to update a slot with the new channel.
@@ -658,8 +730,13 @@
       # are placed there during the decoding loop, we pop from that queue by
       # using the .next method on the active request.
       # Yielding allows for the response to be a streaming grpc call - which
       # can be called via iterating over a for loop on the other side.
       # The DecodeResponse stream should consume all generated tokens in
       # return_channel when complete signal is received. It should check if
       # return_channel is empty to decide if it should exit the while loop.
-      yield jetstream_pb2.DecodeResponse(response=response)
+      repeated_token_ids = []
+      for token_ids in response:
+        repeated_token_ids.append(
+            jetstream_pb2.RepeatedTokenIds(token_ids=token_ids)
+        )
+      yield jetstream_pb2.DecodeResponse(response=repeated_token_ids)
```

### Comparing `google-jetstream-0.2.0/jetstream/core/orchestrator_test.py` & `google_jetstream-0.2.1/jetstream/tests/core/test_orchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 I.e. ['Ċ', 'Ō', 'Ɵ'] when converted back with chr().
 
 Therefore we should get back the character sequence '$lǔ' if we request 3 tokens
 decoded (these are the ascii chars at those indices which is what the test
 tokenizer returns).
 """
 
+import pytest
 from absl.testing import absltest
 from jetstream.core import orchestrator
 from jetstream.core.proto import jetstream_pb2
 from jetstream.engine import mock_engine
 
 
 class OrchestratorTest(absltest.TestCase):
@@ -62,14 +63,15 @@
         prefill_engines=[prefill_engine],
         generate_engines=[generate_engine],
         prefill_params=[prefill_engine.load_params()],
         generate_params=[generate_engine.load_params()],
     )
     return driver
 
+  @pytest.mark.asyncio
   async def test_orchestrator(self):
     """Test the multithreaded orchestration."""
     driver = self._setup_driver()
     client = orchestrator.LLMOrchestrator(driver=driver)
 
     # The string representation of np.array([[65, 66]]), [2] will be prepend
     # as BOS.
@@ -83,20 +85,18 @@
     )
     iterator = client.Decode(request)
     # chr of [266, 332, 415].
     expected_tokens = ["Ċ", "Ō", "Ɵ", ""]
     counter = 0
     async for token in iterator:
       # Tokens come through as bytes.
-      print(
-          "actual output: "
-          + bytes(token.response[0], encoding="utf-8").decode()
-      )
+      output_token = await token.response[0].token_id[0]
+      print("actual output: " + bytes(output_token, encoding="utf-8").decode())
       assert (
-          bytes(token.response[0], encoding="utf-8").decode()
+          bytes(output_token, encoding="utf-8").decode()
           == expected_tokens[counter]
       )
       counter += 1
     driver.stop()
 
 
 if __name__ == "__main__":
```

### Comparing `google-jetstream-0.2.0/jetstream/core/proto/__init__.py` & `google_jetstream-0.2.1/jetstream/core/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/core/proto/jetstream_pb2.py` & `google_jetstream-0.2.1/jetstream/core/proto/jetstream_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,24 +24,26 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n$jetstream/core/proto/jetstream.proto\x12\x0fjetstream_proto"e\n\rDecodeRequest\x12\x15\n\rsession_cache\x18\x01 \x01(\t\x12\x17\n\x0f\x61\x64\x64itional_text\x18\x02 \x01(\t\x12\x10\n\x08priority\x18\x03 \x01(\x05\x12\x12\n\nmax_tokens\x18\x04 \x01(\x05""\n\x0e\x44\x65\x63odeResponse\x12\x10\n\x08response\x18\x01 \x03(\t2]\n\x0cOrchestrator\x12M\n\x06\x44\x65\x63ode\x12\x1e.jetstream_proto.DecodeRequest\x1a\x1f.jetstream_proto.DecodeResponse"\x00\x30\x01\x62\x06proto3'
+    b'\n$jetstream/core/proto/jetstream.proto\x12\x0fjetstream_proto"e\n\rDecodeRequest\x12\x15\n\rsession_cache\x18\x01 \x01(\t\x12\x17\n\x0f\x61\x64\x64itional_text\x18\x02 \x01(\t\x12\x10\n\x08priority\x18\x03 \x01(\x05\x12\x12\n\nmax_tokens\x18\x04 \x01(\x05"E\n\x0e\x44\x65\x63odeResponse\x12\x33\n\x08response\x18\x01 \x03(\x0b\x32!.jetstream_proto.RepeatedTokenIds"%\n\x10RepeatedTokenIds\x12\x11\n\ttoken_ids\x18\x01 \x03(\x05\x32]\n\x0cOrchestrator\x12M\n\x06\x44\x65\x63ode\x12\x1e.jetstream_proto.DecodeRequest\x1a\x1f.jetstream_proto.DecodeResponse"\x00\x30\x01\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "jetstream.core.proto.jetstream_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals["_DECODEREQUEST"]._serialized_start = 57
   _globals["_DECODEREQUEST"]._serialized_end = 158
   _globals["_DECODERESPONSE"]._serialized_start = 160
-  _globals["_DECODERESPONSE"]._serialized_end = 194
-  _globals["_ORCHESTRATOR"]._serialized_start = 196
-  _globals["_ORCHESTRATOR"]._serialized_end = 289
+  _globals["_DECODERESPONSE"]._serialized_end = 229
+  _globals["_REPEATEDTOKENIDS"]._serialized_start = 231
+  _globals["_REPEATEDTOKENIDS"]._serialized_end = 268
+  _globals["_ORCHESTRATOR"]._serialized_start = 270
+  _globals["_ORCHESTRATOR"]._serialized_end = 363
 # @@protoc_insertion_point(module_scope)
```

### Comparing `google-jetstream-0.2.0/jetstream/core/proto/jetstream_pb2_grpc.py` & `google_jetstream-0.2.1/jetstream/core/proto/jetstream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/core/server_lib.py` & `google_jetstream-0.2.1/jetstream/core/server_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
 def run(
     port: int,
     config: Type[config_lib.ServerConfig],
     devices: Any,
     credentials: Any = grpc.insecure_server_credentials(),
     threads: int | None = None,
+    jax_padding: bool = True,
 ) -> JetStreamServer:
   """Runs a server with a specified config.
 
   Args:
     port: Port on which the server will be made available.
     config: A ServerConfig to config engine, model, device slices, etc.
     devices: Device objects, will be used to get engine with proper slicing.
@@ -107,29 +108,34 @@
   """
   logging.info("Kicking off gRPC server.")
   engines = config_lib.get_engines(config, devices=devices)
   prefill_params = [pe.load_params() for pe in engines.prefill_engines]
   generate_params = [ge.load_params() for ge in engines.generate_engines]
   shared_params = [ie.load_params() for ie in engines.interleaved_engines]
   logging.info("Loaded all weights.")
+  interleaved_mode = (
+      len(config.prefill_slices) + len(config.generate_slices) == 0
+  )
   driver = orchestrator.Driver(
       prefill_engines=engines.prefill_engines + engines.interleaved_engines,
       generate_engines=engines.generate_engines + engines.interleaved_engines,
       prefill_params=prefill_params + shared_params,
       generate_params=generate_params + shared_params,
+      interleaved_mode=interleaved_mode,
+      jax_padding=jax_padding,
   )
   # We default threads to the total number of concurrent allowed decodes,
   # to make sure we can fully saturate the model. Set default minimum to 64.
   threads = threads or max(driver.get_total_concurrent_requests(), 64)
   jetstream_server = JetStreamServer(driver, threads, port, credentials)
   logging.info("Starting server on port %d with %d threads", port, threads)
 
   jetstream_server.start()
   return jetstream_server
 
 
 def get_devices() -> Any:
-  """Gets devices locally."""
-  # Run interleaved engine on local device.
+  """Gets devices."""
+  # TODO: Add more logs for the devices.
   devices = jax.devices()
-  logging.info("Using local devices for interleaved serving: %d", len(devices))
+  logging.info("Using devices: %d", len(devices))
   return devices
```

### Comparing `google-jetstream-0.2.0/jetstream/core/server_test.py` & `google_jetstream-0.2.1/jetstream/tests/core/test_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 response.
 """
 
 from typing import Any, Type
 
 from absl.testing import absltest, parameterized
 import grpc
+import pytest
 from jetstream.core import config_lib
 from jetstream.core import server_lib
 from jetstream.core.proto import jetstream_pb2
 from jetstream.core.proto import jetstream_pb2_grpc
 import portpicker
 
 
@@ -41,15 +42,16 @@
       # Uses the same prefill / generate weights (2).
       (
           config_lib.InterleavedCPUTestServer,
           ["Ċ", "Ə", "ɖ", ""],
           [None],
       ),
   )
-  def test_server(
+  @pytest.mark.asyncio
+  async def test_server(
       self,
       config: Type[config_lib.ServerConfig],
       expected_tokens: list[str],
       devices: list[Any],
   ):
     """Sets up a server and requests token responses."""
     ######################### Server side ######################################
@@ -60,39 +62,39 @@
     server = server_lib.run(
         port=port,
         config=config,
         devices=devices,
         credentials=credentials,
     )
     ###################### Requester side ######################################
-    channel = grpc.secure_channel(
+    async with grpc.aio.secure_channel(
         f"localhost:{port}", grpc.local_channel_credentials()
-    )
-    stub = jetstream_pb2_grpc.OrchestratorStub(channel)
+    ) as channel:
+      stub = jetstream_pb2_grpc.OrchestratorStub(channel)
 
-    # The string representation of np.array([[65, 66]]), [2] will be prependd
-    # as BOS
-    text = "AB"
-    request = jetstream_pb2.DecodeRequest(
-        session_cache="",
-        additional_text=text,
-        priority=1,
-        max_tokens=3,
-    )
-    iterator = stub.Decode(request)
-    counter = 0
-    for token in iterator:
-      # Tokens come through as bytes
-      print(
-          "actual output: "
-          + bytes(token.response[0], encoding="utf-8").decode()
-      )
-      assert (
-          bytes(token.response[0], encoding="utf-8").decode()
-          == expected_tokens[counter]
+      # The string representation of np.array([[65, 66]]), [2] will be prependd
+      # as BOS
+      text = "AB"
+      request = jetstream_pb2.DecodeRequest(
+          session_cache="",
+          additional_text=text,
+          priority=1,
+          max_tokens=3,
       )
-      counter += 1
-    server.stop()
+      iterator = stub.Decode(request)
+      counter = 0
+      async for token in iterator:
+        # Tokens come through as bytes
+        output_token = await token.response[0].token_id[0]
+        print(
+            "actual output: " + bytes(output_token, encoding="utf-8").decode()
+        )
+        assert (
+            bytes(output_token, encoding="utf-8").decode()
+            == expected_tokens[counter]
+        )
+        counter += 1
+      server.stop()
 
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `google-jetstream-0.2.0/jetstream/core/utils/__init__.py` & `google_jetstream-0.2.1/jetstream/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/core/utils/async_multifuture.py` & `google_jetstream-0.2.1/jetstream/core/utils/async_multifuture.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/engine/__init__.py` & `google_jetstream-0.2.1/jetstream/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/engine/engine_api.py` & `google_jetstream-0.2.1/jetstream/engine/engine_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,27 +22,30 @@
 from typing import Any, Optional, Tuple, Union
 
 from flax import struct
 import jax
 import numpy as np
 
 from jetstream.engine import tokenizer_pb2
+from jetstream.engine import token_utils
 
 
 # The model parameters - their partitioning will be unique for different prefill
 # and decode topoologies.
 Params = Any
 # The result of a prefill operation, often a batch size 1 KVCache.
 Prefix = Any
 # The inputs into a generation step, often a prefill and generate cache tuple.
 DecodeState = Any
 # Accelerator representation of tokens.
 DeviceTokens = Any
 # Cpus asscociated with the mesh.
 CpuDevices = Any
+# Tokenkizer used by the engine
+Tokenizer = Any
 
 
 @struct.dataclass
 class SlotData:
   """Class to store slot data."""
 
   tokens: Union[jax.Array, np.ndarray]
@@ -78,14 +81,17 @@
   )
   samples_per_slot: int = struct.field(
       pytree_node=False,
   )
 
   def copy_to_host_async(self: "ResultTokens") -> None:
     """Copy to host asynchronously."""
+    # Do nothing for np array
+    if isinstance(self.data, np.ndarray):
+      return
     self.data.copy_to_host_async()
 
   def convert_to_numpy(self: "ResultTokens") -> "ResultTokens":
     """Converts to numpy."""
     return ResultTokens(
         np.array(self.data),
         self.tokens_idx,
@@ -193,15 +199,22 @@
   def get_prefix_destination_sharding(self) -> Any:
     """Returns the shardings necessary to transfer data between engines."""
 
   @abc.abstractmethod
   def get_tokenizer(
       self,
   ) -> tokenizer_pb2.TokenizerParameters:
-    """Returns the info to construct a sentencepiece tokenizer in py/c++."""
+    """Returns the info to construct a tokenizer in py/c++."""
+
+  def build_tokenizer(
+      self,
+      metadata: tokenizer_pb2.TokenizerParameters,
+  ) -> Tokenizer:
+    """Builds a new tokenizer object and returns it."""
+    return token_utils.SentencePieceTokenizer(metadata)
 
   @abc.abstractmethod
   def init_decode_state(self, *args, **kwargs) -> DecodeState:
     """Initialises any state which a generation step transforms."""
 
   @property
   @abc.abstractmethod
```

### Comparing `google-jetstream-0.2.0/jetstream/engine/mock_engine.py` & `google_jetstream-0.2.1/jetstream/engine/mock_engine.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/engine/mock_engine_test.py` & `google_jetstream-0.2.1/jetstream/tests/engine/test_mock_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,16 +48,29 @@
 
   def _prefill(self):
     """Performs prefill and returns a kv cache."""
     engine, params = self._setup()
     # A 2 will be pre-pended as 'bos' token from the vocab.
     text = "AB"
     metadata = engine.get_tokenizer()
-    vocab = token_utils.load_vocab(metadata.path, metadata.extra_ids)
-    tokens, true_length = token_utils.tokenize_and_pad(text, vocab, is_bos=True)
+    tokenizer = engine.build_tokenizer(metadata)
+    tokens, true_length = tokenizer.encode(text, is_bos=True)
+    prefill_result = engine.prefill(
+        params=params, padded_tokens=tokens, true_length=3
+    )
+    return engine, params, prefill_result, true_length
+
+  def _prefill_np(self):
+    """Performs prefill and returns a kv cache."""
+    engine, params = self._setup()
+    # A 2 will be pre-pended as 'bos' token from the vocab.
+    text = "AB"
+    metadata = engine.get_tokenizer()
+    tokenizer = engine.build_tokenizer(metadata)
+    tokens, true_length = tokenizer.encode(text, is_bos=True, jax_padding=False)
     prefill_result = engine.prefill(
         params=params, padded_tokens=tokens, true_length=3
     )
     return engine, params, prefill_result, true_length
 
   def _generate(self, slot=1):
     """Performs a single generation step."""
@@ -79,14 +92,21 @@
   def test_prefill(self):
     """Tests prefill with weight = 2."""
     _, _, prefill_result, true_length = self._prefill()
     np.testing.assert_array_equal(
         prefill_result[:, :true_length], np.array([[4.0, 130.0, 132.0]])
     )
 
+  def test_prefill_np(self):
+    """Tests prefill with weight = 2."""
+    _, _, prefill_result, true_length = self._prefill_np()
+    np.testing.assert_array_equal(
+        prefill_result[:, :true_length], np.array([[4.0, 130.0, 132.0]])
+    )
+
   def test_generate(self, slot=1):
     """Tests multiple generation steps."""
     engine, params, decode_state, sampled_tokens = self._generate(slot=slot)
     metadata = engine.get_tokenizer()
     tokenizer = token_utils.load_vocab(
         metadata.path, metadata.extra_ids
     ).tokenizer
```

### Comparing `google-jetstream-0.2.0/jetstream/engine/mock_utils.py` & `google_jetstream-0.2.1/jetstream/engine/mock_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -58,30 +58,32 @@
     """Converts a string into a integer sequenc."""
     # 'We use array methods, not python iterables so we don't
     # implement this method in the mock vocab.
     raise NotImplementedError
 
   def _decode(self, ids: np.ndarray):
     """Converts a numpy array into a string."""
-    # 'We use array methods, not python iterables so we don't
-    # implement this method in the mock vocab.
-    raise NotImplementedError
+    return "".join([chr(r) for r in list(ids)])
 
   def _encode_tf(self, s: str) -> np.ndarray:
     """Converts a string into a numpy array."""
     # We mock using numpy to avoid propagating tf dependencies.
     chars = np.array([ord(c) for c in s]).astype(np.int32)
     return chars
 
   def _decode_tf(self, ids: np.ndarray) -> List[str]:
     """Converts a numpy array into a string."""
     # We mock using numpy to avoid propagating tf dependencies.
     results = np.split(ids, ids.shape[0])
     return ["".join([chr(r) for r in list(line[0])]) for line in results]
 
+  def decode(self, ids: np.ndarray):
+    """Converts a numpy array into a string."""
+    return self._decode(ids)
+
   def encode_tf(self, s: str) -> np.ndarray:
     """Converts a string into a numpy array."""
     return self._encode_tf(s)
 
   def decode_tf(self, ids: np.ndarray) -> List[str]:
     """Converts a numpy array into a string."""
     return self._decode_tf(ids)
```

### Comparing `google-jetstream-0.2.0/jetstream/engine/tokenizer_pb2.py` & `google_jetstream-0.2.1/jetstream/engine/tokenizer_pb2.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/engine/tokenizer_pb2_grpc.py` & `google_jetstream-0.2.1/jetstream/engine/tokenizer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.2.0/jetstream/engine/utils_test.py` & `google_jetstream-0.2.1/jetstream/tests/engine/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,35 +51,40 @@
     result_tokens = engine_api.ResultTokens(
         data=data.astype(np.int32),
         tokens_idx=(0, speculations),
         valid_idx=(speculations, 2 * speculations),
         length_idx=(2 * speculations, 2 * speculations + 1),
         samples_per_slot=2,
     )
+    vocab = mock_utils.TestVocab()
     per_channel, complete = token_utils.process_result_tokens(
         slot=0,
         slot_max_length=4,
         result_tokens=result_tokens,
-        vocab=mock_utils.TestVocab(),
+        eos_id=vocab.eos_id,
+        pad_id=vocab.pad_id,
         complete=mock_complete,
     )
     np.testing.assert_equal(complete, np.array([1, 0]))
 
-    assert not per_channel[0]  # i.e. == '', because of the pad.
-    assert per_channel[1] == "AD"
+    text_output = [mock_utils.TestVocab().decode(row) for row in per_channel]
+    assert not text_output[0]  # i.e. == '', because of the pad.
+    assert text_output[1] == "AD"
     mock_complete = np.zeros(
         (mock_tokens.shape[0] // samples_per_slot), dtype=np.int32
     )
     per_channel, complete = token_utils.process_result_tokens(
         slot=1,
         slot_max_length=4,
         result_tokens=result_tokens,
-        vocab=mock_utils.TestVocab(),
+        eos_id=vocab.eos_id,
+        pad_id=vocab.pad_id,
         complete=mock_complete,
     )
-    assert per_channel[0] == "T3"
-    assert per_channel[1] == "A"  # second token is padded.
+    text_output = [mock_utils.TestVocab().decode(row) for row in per_channel]
+    assert text_output[0] == "T3"
+    assert text_output[1] == "A"  # second token is padded.
     np.testing.assert_equal(complete, np.array([0, 1]))
 
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `google-jetstream-0.2.0/setup.py` & `google_jetstream-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   with open(filename) as f:
     lineiter = (line.strip() for line in f)
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 setup(
     name="google-jetstream",
-    version="0.2.0",
+    version="0.2.1",
     description=(
         "JetStream is a throughput and memory optimized engine for LLM inference on XLA devices, starting with TPUs (and GPUs in future -- PRs welcome)."
     ),
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Google LLC",
     url="https://github.com/google/JetStream",
```


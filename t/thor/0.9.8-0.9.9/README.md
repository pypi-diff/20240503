# Comparing `tmp/thor-0.9.8.tar.gz` & `tmp/thor-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thor-0.9.8.tar", last modified: Wed Dec 13 04:11:44 2023, max compression
+gzip compressed data, was "thor-0.9.9.tar", last modified: Mon Jan 29 05:28:06 2024, max compression
```

## Comparing `thor-0.9.8.tar` & `thor-0.9.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 04:11:44.223946 thor-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-13 04:11:09.000000 thor-0.9.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-13 04:11:09.000000 thor-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2023-12-13 04:11:44.223946 thor-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-12-13 04:11:09.000000 thor-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 04:11:44.215946 thor-0.9.8/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-13 04:11:09.000000 thor-0.9.8/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-12-13 04:11:09.000000 thor-0.9.8/doc/events.md
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2023-12-13 04:11:09.000000 thor-0.9.8/doc/http.md
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-12-13 04:11:09.000000 thor-0.9.8/doc/loop.md
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2023-12-13 04:11:09.000000 thor-0.9.8/doc/tcp.md
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-12-13 04:11:09.000000 thor-0.9.8/doc/tls.md
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-12-13 04:11:09.000000 thor-0.9.8/doc/udp.md
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2023-12-13 04:11:09.000000 thor-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 04:11:44.223946 thor-0.9.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 04:11:44.219946 thor-0.9.8/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4498 2023-12-13 04:11:09.000000 thor-0.9.8/test/framework.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1800 2023-12-13 04:11:09.000000 thor-0.9.8/test/test_dns.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4264 2023-12-13 04:11:09.000000 thor-0.9.8/test/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28532 2023-12-13 04:11:09.000000 thor-0.9.8/test/test_http_client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14216 2023-12-13 04:11:09.000000 thor-0.9.8/test/test_http_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2023-12-13 04:11:09.000000 thor-0.9.8/test/test_http_server.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1338 2023-12-13 04:11:09.000000 thor-0.9.8/test/test_http_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5156 2023-12-13 04:11:09.000000 thor-0.9.8/test/test_loop.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4255 2023-12-13 04:11:09.000000 thor-0.9.8/test/test_tcp_client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1676 2023-12-13 04:11:09.000000 thor-0.9.8/test/test_tcp_server.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4398 2023-12-13 04:11:09.000000 thor-0.9.8/test/test_tls_client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1975 2023-12-13 04:11:09.000000 thor-0.9.8/test/test_udp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 04:11:44.219946 thor-0.9.8/thor/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1517 2023-12-13 04:11:09.000000 thor-0.9.8/thor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 04:11:44.219946 thor-0.9.8/thor/dns/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2023-12-13 04:11:09.000000 thor-0.9.8/thor/dns/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3181 2023-12-13 04:11:09.000000 thor-0.9.8/thor/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 04:11:44.223946 thor-0.9.8/thor/http/
--rwxr-xr-x   0 runner    (1001) docker     (127)      289 2023-12-13 04:11:09.000000 thor-0.9.8/thor/http/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24507 2023-12-13 04:11:09.000000 thor-0.9.8/thor/http/client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19321 2023-12-13 04:11:09.000000 thor-0.9.8/thor/http/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2777 2023-12-13 04:11:09.000000 thor-0.9.8/thor/http/error.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9932 2023-12-13 04:11:09.000000 thor-0.9.8/thor/http/server.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14938 2023-12-13 04:11:09.000000 thor-0.9.8/thor/loop.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 04:11:09.000000 thor-0.9.8/thor/py.typed
--rwxr-xr-x   0 runner    (1001) docker     (127)    13399 2023-12-13 04:11:09.000000 thor-0.9.8/thor/tcp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3197 2023-12-13 04:11:09.000000 thor-0.9.8/thor/tls.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3499 2023-12-13 04:11:09.000000 thor-0.9.8/thor/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 04:11:44.223946 thor-0.9.8/thor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2023-12-13 04:11:44.000000 thor-0.9.8/thor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-12-13 04:11:44.000000 thor-0.9.8/thor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 04:11:44.000000 thor-0.9.8/thor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-13 04:11:44.000000 thor-0.9.8/thor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-13 04:11:44.000000 thor-0.9.8/thor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 05:28:06.390753 thor-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-29 05:27:42.000000 thor-0.9.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-29 05:27:42.000000 thor-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-01-29 05:28:06.390753 thor-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-01-29 05:27:42.000000 thor-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 05:28:06.386752 thor-0.9.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-01-29 05:27:42.000000 thor-0.9.9/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-01-29 05:27:42.000000 thor-0.9.9/doc/events.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-01-29 05:27:42.000000 thor-0.9.9/doc/http.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-01-29 05:27:42.000000 thor-0.9.9/doc/loop.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-01-29 05:27:42.000000 thor-0.9.9/doc/tcp.md
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-29 05:27:42.000000 thor-0.9.9/doc/tls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-29 05:27:42.000000 thor-0.9.9/doc/udp.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-01-29 05:27:42.000000 thor-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 05:28:06.390753 thor-0.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 05:28:06.386752 thor-0.9.9/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4498 2024-01-29 05:27:42.000000 thor-0.9.9/test/framework.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1800 2024-01-29 05:27:42.000000 thor-0.9.9/test/test_dns.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4264 2024-01-29 05:27:42.000000 thor-0.9.9/test/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28532 2024-01-29 05:27:42.000000 thor-0.9.9/test/test_http_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14216 2024-01-29 05:27:42.000000 thor-0.9.9/test/test_http_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-01-29 05:27:42.000000 thor-0.9.9/test/test_http_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1338 2024-01-29 05:27:42.000000 thor-0.9.9/test/test_http_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5156 2024-01-29 05:27:42.000000 thor-0.9.9/test/test_loop.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4255 2024-01-29 05:27:42.000000 thor-0.9.9/test/test_tcp_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1676 2024-01-29 05:27:42.000000 thor-0.9.9/test/test_tcp_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4398 2024-01-29 05:27:42.000000 thor-0.9.9/test/test_tls_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1975 2024-01-29 05:27:42.000000 thor-0.9.9/test/test_udp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 05:28:06.390753 thor-0.9.9/thor/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1517 2024-01-29 05:27:42.000000 thor-0.9.9/thor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 05:28:06.390753 thor-0.9.9/thor/dns/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2024-01-29 05:27:42.000000 thor-0.9.9/thor/dns/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3240 2024-01-29 05:27:42.000000 thor-0.9.9/thor/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 05:28:06.390753 thor-0.9.9/thor/http/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      289 2024-01-29 05:27:42.000000 thor-0.9.9/thor/http/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24507 2024-01-29 05:27:42.000000 thor-0.9.9/thor/http/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19321 2024-01-29 05:27:42.000000 thor-0.9.9/thor/http/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2777 2024-01-29 05:27:42.000000 thor-0.9.9/thor/http/error.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9932 2024-01-29 05:27:42.000000 thor-0.9.9/thor/http/server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14938 2024-01-29 05:27:42.000000 thor-0.9.9/thor/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 05:27:42.000000 thor-0.9.9/thor/py.typed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13399 2024-01-29 05:27:42.000000 thor-0.9.9/thor/tcp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3197 2024-01-29 05:27:42.000000 thor-0.9.9/thor/tls.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3499 2024-01-29 05:27:42.000000 thor-0.9.9/thor/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 05:28:06.390753 thor-0.9.9/thor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-01-29 05:28:06.000000 thor-0.9.9/thor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-01-29 05:28:06.000000 thor-0.9.9/thor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 05:28:06.000000 thor-0.9.9/thor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-29 05:28:06.000000 thor-0.9.9/thor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-29 05:28:06.000000 thor-0.9.9/thor.egg-info/top_level.txt
```

### Comparing `thor-0.9.8/LICENSE.md` & `thor-0.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/PKG-INFO` & `thor-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thor
-Version: 0.9.8
+Version: 0.9.9
 Summary: Simple Event-Driven IO for Python
 Author-email: Mark Nottingham <mnot@mnot.net>
 License: # License
         
         
         Copyright (c) 2005– Mark Nottingham
```

### Comparing `thor-0.9.8/README.md` & `thor-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/doc/events.md` & `thor-0.9.9/doc/events.md`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/doc/http.md` & `thor-0.9.9/doc/http.md`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/doc/loop.md` & `thor-0.9.9/doc/loop.md`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/doc/tcp.md` & `thor-0.9.9/doc/tcp.md`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/doc/tls.md` & `thor-0.9.9/doc/tls.md`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/doc/udp.md` & `thor-0.9.9/doc/udp.md`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/pyproject.toml` & `thor-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/framework.py` & `thor-0.9.9/test/framework.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/test_dns.py` & `thor-0.9.9/test/test_dns.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/test_events.py` & `thor-0.9.9/test/test_events.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/test_http_client.py` & `thor-0.9.9/test/test_http_client.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/test_http_parser.py` & `thor-0.9.9/test/test_http_parser.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/test_http_server.py` & `thor-0.9.9/test/test_http_server.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/test_http_utils.py` & `thor-0.9.9/test/test_http_utils.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/test_loop.py` & `thor-0.9.9/test/test_loop.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/test_tcp_client.py` & `thor-0.9.9/test/test_tcp_client.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/test_tcp_server.py` & `thor-0.9.9/test/test_tcp_server.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/test_tls_client.py` & `thor-0.9.9/test/test_tls_client.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/test/test_udp.py` & `thor-0.9.9/test/test_udp.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/thor/__init__.py` & `thor-0.9.9/thor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,13 +28,13 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 from thor.loop import run, stop, time, schedule
 from thor.tcp import TcpClient, TcpServer
 from thor.udp import UdpEndpoint
 from thor.events import on
```

### Comparing `thor-0.9.8/thor/dns/__init__.py` & `thor-0.9.9/thor/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/thor/events.py` & `thor-0.9.9/thor/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 
     def __init__(self) -> None:
         self.__events: Dict[str, List[Callable]] = defaultdict(list)
         self.__sink: object = None
 
     def __getstate__(self) -> Dict[str, Any]:
         state = self.__dict__.copy()
-        del state["_EventEmitter__events"]
+        try:
+            del state["_EventEmitter__events"]
+        except KeyError:
+            pass
         return state
 
     def on(self, event: str, listener: Callable) -> None:
         """
         Call listener when event is emitted.
         """
         self.__events[event].append(listener)
```

### Comparing `thor-0.9.8/thor/http/client.py` & `thor-0.9.9/thor/http/client.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/thor/http/common.py` & `thor-0.9.9/thor/http/common.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/thor/http/error.py` & `thor-0.9.9/thor/http/error.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/thor/http/server.py` & `thor-0.9.9/thor/http/server.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/thor/loop.py` & `thor-0.9.9/thor/loop.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/thor/tcp.py` & `thor-0.9.9/thor/tcp.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/thor/tls.py` & `thor-0.9.9/thor/tls.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/thor/udp.py` & `thor-0.9.9/thor/udp.py`

 * *Files identical despite different names*

### Comparing `thor-0.9.8/thor.egg-info/PKG-INFO` & `thor-0.9.9/thor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thor
-Version: 0.9.8
+Version: 0.9.9
 Summary: Simple Event-Driven IO for Python
 Author-email: Mark Nottingham <mnot@mnot.net>
 License: # License
         
         
         Copyright (c) 2005– Mark Nottingham
```

### Comparing `thor-0.9.8/thor.egg-info/SOURCES.txt` & `thor-0.9.9/thor.egg-info/SOURCES.txt`

 * *Files identical despite different names*


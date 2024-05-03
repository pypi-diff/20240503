# Comparing `tmp/robotcode_core-0.80.0.tar.gz` & `tmp/robotcode_core-0.81.0.tar.gz`

## Comparing `robotcode_core-0.80.0.tar` & `robotcode_core-0.81.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/__version__.py
--rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/async_tools.py
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/concurrent.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/documents_manager.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/event.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/filewatcher.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/language.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/py.typed
--rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/text_document.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/types.py
--rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/uri.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/lsp/__init__.py
--rw-r--r--   0        0        0   233360 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/lsp/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/__init__.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/caching.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/cli.py
--rw-r--r--   0        0        0    21972 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/dataclasses.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/debugpy.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/glob_path.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/inspect.py
--rw-r--r--   0        0        0    16387 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/logging.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/net.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/path.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/process.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/safe_eval.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/src/robotcode/core/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/LICENSE.txt
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/README.md
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/pyproject.toml
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 robotcode_core-0.80.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/__version__.py
+-rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/async_tools.py
+-rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/concurrent.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/documents_manager.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/event.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/filewatcher.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/language.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/py.typed
+-rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/text_document.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/types.py
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/uri.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/lsp/__init__.py
+-rw-r--r--   0        0        0   233360 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/lsp/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/__init__.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/caching.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/cli.py
+-rw-r--r--   0        0        0    21972 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/dataclasses.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/debugpy.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/glob_path.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/inspect.py
+-rw-r--r--   0        0        0    16387 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/logging.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/net.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/path.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/process.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/safe_eval.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/src/robotcode/core/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/LICENSE.txt
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/README.md
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/pyproject.toml
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 robotcode_core-0.81.0/PKG-INFO
```

### Comparing `robotcode_core-0.80.0/src/robotcode/core/async_tools.py` & `robotcode_core-0.81.0/src/robotcode/core/async_tools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/concurrent.py` & `robotcode_core-0.81.0/src/robotcode/core/concurrent.py`

 * *Files 6% similar despite different names*

```diff
@@ -213,26 +213,46 @@
     with _running_tasks_lock:
         _running_tasks.pop(future, None)
 
 
 _P = ParamSpec("_P")
 
 
-def run_as_task(callable: Callable[_P, _TResult], *args: _P.args, **kwargs: _P.kwargs) -> Task[_TResult]:
+def _create_task_in_thread(
+    callable: Callable[_P, _TResult], *args: _P.args, **kwargs: _P.kwargs
+) -> Tuple[Task[_TResult], threading.Thread]:
     future: Task[_TResult] = Task()
     with _running_tasks_lock:
         thread = threading.Thread(
             target=_run_task_in_thread_handler,
             args=(future, callable, args, kwargs),
             name=str(callable),
         )
         _running_tasks[future] = thread
         future.add_done_callback(_remove_future_from_running_tasks)
+
     # TODO: don't set daemon=True because it can be deprecated in future pyhton versions
     thread.daemon = True
+    return future, thread
+
+
+def run_as_task(callable: Callable[_P, _TResult], *args: _P.args, **kwargs: _P.kwargs) -> Task[_TResult]:
+    future, thread = _create_task_in_thread(callable, *args, **kwargs)
+
+    thread.start()
+
+    return future
+
+
+def run_as_debugpy_hidden_task(callable: Callable[_P, _TResult], *args: _P.args, **kwargs: _P.kwargs) -> Task[_TResult]:
+    future, thread = _create_task_in_thread(callable, *args, **kwargs)
+
+    thread.pydev_do_not_trace = True  # type: ignore[attr-defined]
+    thread.is_pydev_daemon_thread = True  # type: ignore[attr-defined]
+
     thread.start()
 
     return future
 
 
 def _cancel_all_running_tasks(timeout: Optional[float] = None) -> None:
     threads: List[threading.Thread] = []
```

### Comparing `robotcode_core-0.80.0/src/robotcode/core/documents_manager.py` & `robotcode_core-0.81.0/src/robotcode/core/documents_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/event.py` & `robotcode_core-0.81.0/src/robotcode/core/event.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/filewatcher.py` & `robotcode_core-0.81.0/src/robotcode/core/filewatcher.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/language.py` & `robotcode_core-0.81.0/src/robotcode/core/language.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/text_document.py` & `robotcode_core-0.81.0/src/robotcode/core/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/uri.py` & `robotcode_core-0.81.0/src/robotcode/core/uri.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/workspace.py` & `robotcode_core-0.81.0/src/robotcode/core/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/lsp/types.py` & `robotcode_core-0.81.0/src/robotcode/core/lsp/types.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/utils/caching.py` & `robotcode_core-0.81.0/src/robotcode/core/utils/caching.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/utils/dataclasses.py` & `robotcode_core-0.81.0/src/robotcode/core/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/utils/debugpy.py` & `robotcode_core-0.81.0/src/robotcode/core/utils/debugpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import threading
 from typing import Optional, Sequence, Tuple, Union
 
+from robotcode.core.concurrent import run_as_debugpy_hidden_task
+
 from .logging import LoggingDescriptor
 from .net import find_free_port
 
 _logger = LoggingDescriptor(name=__name__)
 
 
 def is_debugpy_installed() -> bool:
@@ -11,22 +14,33 @@
         __import__("debugpy")
     except ImportError:
         _logger.warning("Module debugpy is not installed. If you want to debug python code, please install it.\n")
         return False
     return True
 
 
-def wait_for_debugpy_connected() -> bool:
+def wait_for_debugpy_connected(timeout: float = 30) -> bool:
     if is_debugpy_installed():
         import debugpy  # noqa: T100
 
+        connected = threading.Event()
         _logger.info("wait for debugpy client")
+
+        def _wait_for_client() -> bool:
+            if not connected.wait(timeout=timeout):
+                debugpy.wait_for_client.cancel()
+                return False
+
+            return True
+
+        wait_task = run_as_debugpy_hidden_task(_wait_for_client)
         debugpy.wait_for_client()  # noqa: T100
+        connected.set()
+        return wait_task.result()
 
-        return True
     return False
 
 
 def enable_debugpy(port: int, addresses: Union[Sequence[str], str, None] = None) -> bool:
     if is_debugpy_installed():
         import debugpy  # noqa: T100
```

### Comparing `robotcode_core-0.80.0/src/robotcode/core/utils/glob_path.py` & `robotcode_core-0.81.0/src/robotcode/core/utils/glob_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/utils/inspect.py` & `robotcode_core-0.81.0/src/robotcode/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/utils/logging.py` & `robotcode_core-0.81.0/src/robotcode/core/utils/logging.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/utils/net.py` & `robotcode_core-0.81.0/src/robotcode/core/utils/net.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/utils/path.py` & `robotcode_core-0.81.0/src/robotcode/core/utils/path.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/utils/process.py` & `robotcode_core-0.81.0/src/robotcode/core/utils/process.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/utils/safe_eval.py` & `robotcode_core-0.81.0/src/robotcode/core/utils/safe_eval.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/src/robotcode/core/utils/version.py` & `robotcode_core-0.81.0/src/robotcode/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/.gitignore` & `robotcode_core-0.81.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/LICENSE.txt` & `robotcode_core-0.81.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/README.md` & `robotcode_core-0.81.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.80.0/pyproject.toml` & `robotcode_core-0.81.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = ["typing-extensions>=4.4.0"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
-Donate = "https://github.com/sponsors/d-biehl"
+Donate = "https://opencollective.com/robotcode"
 Documentation = "https://github.com/robotcodedev/robotcode#readme"
 Changelog = "https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md"
 Issues = "https://github.com/robotcodedev/robotcode/issues"
 Source = "https://github.com/robotcodedev/robotcode"
 
 [tool.hatch.version]
 path = "src/robotcode/core/__version__.py"
```

### Comparing `robotcode_core-0.80.0/PKG-INFO` & `robotcode_core-0.81.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: robotcode-core
-Version: 0.80.0
+Version: 0.81.0
 Summary: Some core classes for RobotCode
 Project-URL: Homepage, https://robotcode.io
-Project-URL: Donate, https://github.com/sponsors/d-biehl
+Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
 Author-email: Daniel Biehl <dbiehl@live.de>
 License: Apache-2.0
 License-File: LICENSE.txt
```


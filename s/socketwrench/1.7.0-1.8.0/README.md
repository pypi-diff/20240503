# Comparing `tmp/socketwrench-1.7.0.tar.gz` & `tmp/socketwrench-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.7.0.tar", last modified: Mon Apr 15 17:50:38 2024, max compression
+gzip compressed data, was "socketwrench-1.8.0.tar", last modified: Fri May  3 02:49:14 2024, max compression
```

## Comparing `socketwrench-1.7.0.tar` & `socketwrench-1.8.0.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:38.192571 socketwrench-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-15 17:50:33.000000 socketwrench-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-15 17:50:38.192571 socketwrench-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-15 17:50:33.000000 socketwrench-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-15 17:50:33.000000 socketwrench-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:50:38.192571 socketwrench-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:38.188571 socketwrench-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:38.188571 socketwrench-1.7.0/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20979 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:38.188571 socketwrench-1.7.0/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    20017 2024-04-15 17:50:33.000000 socketwrench-1.7.0/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:38.188571 socketwrench-1.7.0/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-15 17:50:38.000000 socketwrench-1.7.0/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-15 17:50:38.000000 socketwrench-1.7.0/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:50:38.000000 socketwrench-1.7.0/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 17:50:38.000000 socketwrench-1.7.0/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.751569 socketwrench-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-03 02:49:08.000000 socketwrench-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 02:49:08.000000 socketwrench-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-03 02:49:14.751569 socketwrench-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-05-03 02:49:08.000000 socketwrench-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 02:49:08.000000 socketwrench-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:49:14.751569 socketwrench-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.743569 socketwrench-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.747569 socketwrench-1.8.0/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20975 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.747569 socketwrench-1.8.0/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.747569 socketwrench-1.8.0/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.751569 socketwrench-1.8.0/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21106 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.751569 socketwrench-1.8.0/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-03 02:49:14.000000 socketwrench-1.8.0/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-03 02:49:14.000000 socketwrench-1.8.0/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:49:14.000000 socketwrench-1.8.0/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 02:49:14.000000 socketwrench-1.8.0/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.7.0/LICENSE` & `socketwrench-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.7.0/PKG-INFO` & `socketwrench-1.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.7.0
+Version: 1.8.0
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -119,14 +119,21 @@
 
 ### Error Modes
 * `"hide"` or `ErrorModes.HIDE`: returns `b"Internal Server Error"` in the response body when an error occurs.
 * `type` or `ErrorModes.TYPE`: returns the error type only in the response body when an error occurs.
 * `"short"` or `ErrorModes.SHORT`: returns the python error message but no traceback in the response body when an error occurs.
 * `"traceback"` or `ErrorModes.TRACEBACK` or `ErrorModes.LONG` or `ErrorModes.TB`: returns the full traceback in the response body when an error occurs.
 
+To set the default error mode for all functions, use `set_default_error_mode`.
+```python
+from socketwrench import set_default_error_mode, ErrorModes
+
+set_default_error_mode(ErrorModes.TRACEBACK) # equivalent to ErrorModes=ErorModes.TRACEBACK
+```
+
 ### favicon.ico
 No need to use our favicon! pass a `str | Path` `.ico` filepath to `favicon` argument to use your own favicon. Alternatively, tag `@route('/favicon.ico')` on a function returning the path.
 
 ### fallback handler
 Add a custom function to handle any requests that don't match any other routes.
 
 # Planned Features
```

### Comparing `socketwrench-1.7.0/README.md` & `socketwrench-1.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,21 @@
 
 ### Error Modes
 * `"hide"` or `ErrorModes.HIDE`: returns `b"Internal Server Error"` in the response body when an error occurs.
 * `type` or `ErrorModes.TYPE`: returns the error type only in the response body when an error occurs.
 * `"short"` or `ErrorModes.SHORT`: returns the python error message but no traceback in the response body when an error occurs.
 * `"traceback"` or `ErrorModes.TRACEBACK` or `ErrorModes.LONG` or `ErrorModes.TB`: returns the full traceback in the response body when an error occurs.
 
+To set the default error mode for all functions, use `set_default_error_mode`.
+```python
+from socketwrench import set_default_error_mode, ErrorModes
+
+set_default_error_mode(ErrorModes.TRACEBACK) # equivalent to ErrorModes=ErorModes.TRACEBACK
+```
+
 ### favicon.ico
 No need to use our favicon! pass a `str | Path` `.ico` filepath to `favicon` argument to use your own favicon. Alternatively, tag `@route('/favicon.ico')` on a function returning the path.
 
 ### fallback handler
 Add a custom function to handle any requests that don't match any other routes.
 
 # Planned Features
```

### Comparing `socketwrench-1.7.0/pyproject.toml` & `socketwrench-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.7.0"
+version = "1.8.0"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.7.0/src/socketwrench/__init__.py` & `socketwrench-1.8.0/src/socketwrench/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     Query,
     Body,
     Route,
     FullPath,
     Method,
     File,
     ClientAddr,
-    Headers
+    Headers,
+    set_default_error_mode
 )
 from .tags import (
     tag,
     methods,
     get,
     post,
     put,
```

### Comparing `socketwrench-1.7.0/src/socketwrench/__main__.py` & `socketwrench-1.8.0/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.7.0/src/socketwrench/connection.py` & `socketwrench-1.8.0/src/socketwrench/connection.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.7.0/src/socketwrench/handlers.py` & `socketwrench-1.8.0/src/socketwrench/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,15 @@
             args = tuple(args)
         return args, kwargs, sig.return_annotation
 
     tag(parser, autofill=special_params, sig=sig)
     return parser
 
 @tag(accepts_route_params=True)
-def wrap_handler(_handler, error_mode: str = ErrorModes.HIDE):
+def wrap_handler(_handler, error_mode: str = None):
     """Converts any method into a method that takes a Request and returns a Response."""
     if getattr(_handler, "is_wrapped", False):
         return _handler
     parser = preprocess_args(_handler)
 
 
     # make a stub function that takes the same parameters as the handler but doesn't do anything
@@ -268,21 +268,22 @@
                             response = return_annotation(r)
                         else:
                             response = Response(r, version=request.version)
                     except:
                         response = Response(r, version=request.version)
         except Exception as e:
             logger.exception(e)
-            if error_mode == ErrorModes.HIDE:
+            _error_mode = error_mode if error_mode is not None else ErrorModes.DEFAULT
+            if _error_mode == ErrorModes.HIDE:
                 msg = b'Internal Server Error'
-            elif error_mode == ErrorModes.TYPE:
+            elif _error_mode == ErrorModes.TYPE:
                 msg = str(type(e)).encode()
-            elif error_mode == ErrorModes.SHORT:
+            elif _error_mode == ErrorModes.SHORT:
                 msg = str(e).encode()
-            elif error_mode == ErrorModes.LONG:
+            elif _error_mode == ErrorModes.LONG:
                 msg = traceback.format_exc().encode()
             response = ErrorResponse(msg, version=request.version)
         return response
 
     tag(wrapper,
         is_wrapped=True,
         sig=getattr(parser, "sig", inspect.signature(_handler)),
@@ -337,15 +338,17 @@
             contents = "<!DOCTYPE html><html><body><ul>" + "\n".join([f"<li><a href='{route}/{f.name}'>{f.name}</a></li>" for f in folder_contents]) + "</ul></body></html>"
             return Response(contents.encode(), version=request.version)
         r = FileResponse(p, version=request.version)
         print("content type", r.headers.get("Content-Type"))
         return r
 
 class RouteHandler:
-    default_favicon = Path(__file__).parent.parent / "resources" / "favicon.ico"
+    resources_folder = Path(__file__).parent / "resources"
+    playground_folder = resources_folder / "playground"
+    default_favicon = resources_folder / "favicon.ico"
 
     def __init__(self,
                  routes: dict | None = None,
                  fallback_handler=None,
                  base_path: str = "/",
                  require_tag: bool = False,
                  error_mode: str = ErrorModes.HIDE,
@@ -399,27 +402,27 @@
             r = FileResponse(self.favicon_path, version=request.version)
         except Exception as e:
             r = Response(b"Not Found", status_code=404, version=request.version)
         return r
 
     @get
     def swagger(self) -> FileResponse:
-        return FileResponse(Path(__file__).parent.parent / "resources" / "swagger.html")
+        return FileResponse(Path(__file__).parent / "resources" / "swagger.html")
 
     @get
     def playground(self) -> Path:
-        return Path(__file__).parent.parent / "resources" / "playground" / "playground.html"
+        return self.playground_folder / "playground.html"
 
     @get
     def playground_js(self) -> Path:
-        return Path(__file__).parent.parent / "resources" / "playground" /  "playground.js"
+        return self.playground_folder /  "playground.js"
 
     @get
     def playground_panels_js(self) -> Path:
-        return Path(__file__).parent.parent / "resources" / "playground" / "panels.js"
+        return self.playground_folder / "panels.js"
 
     def parse_routes_from_object(self, obj):
         for k in dir(obj):
             if not k.startswith("_"):
                 v = getattr(obj, k)
                 if callable(v):
                     if self.require_tag and not hasattr(v, "allowed_methods"):
@@ -432,15 +435,14 @@
                             self[route] = v
 
     def __call__(self, request: Request) -> Response:
         route = request.path.route()
         handler = self.routes.get(route, None)
         route_params = {}
         if handler is None:
-            print("matchable_routes", self.matchable_routes)
             for k, v in self.matchable_routes.items():
                 if v.match(route):
                     handler = v
                     break
             else:
                 if route in self.default_routes:
                     handler = self.default_routes[route]
```

### Comparing `socketwrench-1.7.0/src/socketwrench/openapi.py` & `socketwrench-1.8.0/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.7.0/src/socketwrench/samples/file_sample.py` & `socketwrench-1.8.0/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.7.0/src/socketwrench/samples/sample.py` & `socketwrench-1.8.0/src/socketwrench/samples/sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.7.0/src/socketwrench/server.py` & `socketwrench-1.8.0/src/socketwrench/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     default_host = ''
     default_backlog = 1
     default_chunk_size = Connection.default_chunk_size
     default_num_connection_threads = 1
     default_socket_options = None
     default_pause_sleep = 0.1
     default_accept_sleep = 0.1
-    default_favicon = Path(__file__).parent.parent / "resources" / "favicon.ico"
+    default_favicon = RouteHandler.default_favicon
 
     def __init__(self,
                  routes: dict | None = None,
                  port: int = default_port,
                  host: str = default_host,
                  backlog: int = default_backlog,
                  chunk_size: int = default_chunk_size,
```

### Comparing `socketwrench-1.7.0/src/socketwrench/tags.py` & `socketwrench-1.8.0/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.7.0/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.8.0/src/socketwrench.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.7.0
+Version: 1.8.0
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -119,14 +119,21 @@
 
 ### Error Modes
 * `"hide"` or `ErrorModes.HIDE`: returns `b"Internal Server Error"` in the response body when an error occurs.
 * `type` or `ErrorModes.TYPE`: returns the error type only in the response body when an error occurs.
 * `"short"` or `ErrorModes.SHORT`: returns the python error message but no traceback in the response body when an error occurs.
 * `"traceback"` or `ErrorModes.TRACEBACK` or `ErrorModes.LONG` or `ErrorModes.TB`: returns the full traceback in the response body when an error occurs.
 
+To set the default error mode for all functions, use `set_default_error_mode`.
+```python
+from socketwrench import set_default_error_mode, ErrorModes
+
+set_default_error_mode(ErrorModes.TRACEBACK) # equivalent to ErrorModes=ErorModes.TRACEBACK
+```
+
 ### favicon.ico
 No need to use our favicon! pass a `str | Path` `.ico` filepath to `favicon` argument to use your own favicon. Alternatively, tag `@route('/favicon.ico')` on a function returning the path.
 
 ### fallback handler
 Add a custom function to handle any requests that don't match any other routes.
 
 # Planned Features
```


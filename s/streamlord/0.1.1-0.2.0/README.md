# Comparing `tmp/streamlord-0.1.1.tar.gz` & `tmp/streamlord-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlord-0.1.1.tar", max compression
+gzip compressed data, was "streamlord-0.2.0.tar", max compression
```

## Comparing `streamlord-0.1.1.tar` & `streamlord-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       59 2024-04-15 11:50:57.981205 streamlord-0.1.1/README.md
--rw-r--r--   0        0        0      357 2024-04-15 11:51:23.283987 streamlord-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       81 2024-04-02 15:23:42.893017 streamlord-0.1.1/streamlord/__init__.py
--rw-r--r--   0        0        0       30 2024-04-02 15:23:42.893115 streamlord-0.1.1/streamlord/collectors/__init__.py
--rw-r--r--   0        0        0      144 2024-04-02 15:23:42.893228 streamlord-0.1.1/streamlord/collectors/navigation.py
--rw-r--r--   0        0        0       24 2024-04-02 15:23:42.893330 streamlord-0.1.1/streamlord/definitions/__init__.py
--rw-r--r--   0        0        0       90 2024-04-02 15:23:42.893418 streamlord-0.1.1/streamlord/definitions/contracts.py
--rw-r--r--   0        0        0      152 2024-04-02 15:23:42.893517 streamlord-0.1.1/streamlord/mappers/__init__.py
--rw-r--r--   0        0        0      832 2024-04-02 15:23:42.893612 streamlord-0.1.1/streamlord/mappers/destroyer.py
--rw-r--r--   0        0        0      729 2024-04-02 15:23:42.893704 streamlord-0.1.1/streamlord/mappers/digger.py
--rw-r--r--   0        0        0     1289 2024-04-02 15:23:42.893800 streamlord-0.1.1/streamlord/mappers/injector.py
--rw-r--r--   0        0        0     1622 2024-04-02 15:23:42.893901 streamlord-0.1.1/streamlord/mappers/squeezer.py
--rw-r--r--   0        0        0     1318 2024-04-05 08:07:40.295775 streamlord-0.1.1/streamlord/mappers/stamper.py
--rw-r--r--   0        0        0      809 2024-04-02 15:23:42.894091 streamlord-0.1.1/streamlord/pipeline.py
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 streamlord-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       59 2024-04-15 11:50:57.981205 streamlord-0.2.0/README.md
+-rw-r--r--   0        0        0      357 2024-05-03 12:00:02.891581 streamlord-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-02 15:23:42.893017 streamlord-0.2.0/streamlord/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-02 15:23:42.893115 streamlord-0.2.0/streamlord/collector/__init__.py
+-rw-r--r--   0        0        0      144 2024-04-02 15:23:42.893228 streamlord-0.2.0/streamlord/collector/navigation.py
+-rw-r--r--   0        0        0       24 2024-04-02 15:23:42.893330 streamlord-0.2.0/streamlord/definitions/__init__.py
+-rw-r--r--   0        0        0      156 2024-05-03 11:59:54.089348 streamlord-0.2.0/streamlord/definitions/contracts.py
+-rw-r--r--   0        0        0      922 2024-05-03 11:59:54.077897 streamlord-0.2.0/streamlord/pipeline.py
+-rw-r--r--   0        0        0      143 2024-05-03 11:59:54.106639 streamlord-0.2.0/streamlord/transformer/__init__.py
+-rw-r--r--   0        0        0      831 2024-05-03 11:59:54.085738 streamlord-0.2.0/streamlord/transformer/destroyer.py
+-rw-r--r--   0        0        0      726 2024-05-03 11:59:54.104177 streamlord-0.2.0/streamlord/transformer/digger.py
+-rw-r--r--   0        0        0     1287 2024-05-03 11:59:54.043206 streamlord-0.2.0/streamlord/transformer/injector.py
+-rw-r--r--   0        0        0     1621 2024-05-03 11:59:54.097556 streamlord-0.2.0/streamlord/transformer/squeezer.py
+-rw-r--r--   0        0        0     1316 2024-05-03 11:59:54.073387 streamlord-0.2.0/streamlord/transformer/stamper.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 streamlord-0.2.0/PKG-INFO
```

### Comparing `streamlord-0.1.1/streamlord/mappers/destroyer.py` & `streamlord-0.2.0/streamlord/transformer/destroyer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import collections
 
 
-class KeyRemover:
+class RemoveKey:
     def __init__(self, path: str):
         self._chain = path.split('.')
 
     def __call__(
         self,
         data: collections.abc.MutableMapping
     ) -> collections.abc.MutableMapping:
```

### Comparing `streamlord-0.1.1/streamlord/mappers/digger.py` & `streamlord-0.2.0/streamlord/transformer/digger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import collections.abc
 import typing
 
 
-class Digger:
+class Dig:
     def __init__(
         self,
         path: str
     ):
         self._chain = path.split('.')
 
     def __call__(
```

### Comparing `streamlord-0.1.1/streamlord/mappers/injector.py` & `streamlord-0.2.0/streamlord/transformer/injector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import collections.abc
 
 
-class Injector:
+class Inject:
     def __init__(
         self,
         reference: collections.abc.Mapping,
         search_path: str,
         injection_path: str,
         replace: bool = False
     ):
```

### Comparing `streamlord-0.1.1/streamlord/mappers/squeezer.py` & `streamlord-0.2.0/streamlord/transformer/squeezer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import collections.abc
 import typing
 
 
-class Squeezer:
+class Squeeze:
     def __init__(
         self,
         separator: str = '__',
         collapse_none: bool = True
     ):
         super().__init__()
         self._separator = separator
```

### Comparing `streamlord-0.1.1/streamlord/mappers/stamper.py` & `streamlord-0.2.0/streamlord/transformer/stamper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import collections.abc
 
 
-class Stamper:
+class Stamp:
     def __init__(self, parent_key: str, *nested_keys: str | tuple[str, str]):
         super().__init__()
         self._parent_chain = parent_key.split('.')
         self._nested_keys = [k if isinstance(k, tuple) else (k, k) for k in nested_keys]
 
     def __call__(self, data: collections.abc.MutableMapping):
         self._process(data)
```

### Comparing `streamlord-0.1.1/streamlord/pipeline.py` & `streamlord-0.2.0/streamlord/pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import collections.abc
 import typing
 
+from .definitions import contracts
 
-class Pipe:
-    def __init__(self, stream: collections.abc.Iterable[collections.abc.MutableMapping]):
+T = typing.TypeVar('T')
+
+
+class Pipe(typing.Generic[T]):
+    def __init__(self, stream: contracts.Stream[T]):
         self._stream = stream
         self._mappers = []
         self._filters = []
 
-    def map(self, *func: collections.abc.Callable) -> typing.Self:
+    def map(self, *func: collections.abc.Callable[[T], typing.Any]) -> typing.Self:
         self._mappers.extend(list(func))
         return self
 
-    def filter(self, func: collections.abc.Callable) -> typing.Self:
-        self._filters.append(func)
+    def filter(self, *func: collections.abc.Callable[[T], bool]) -> typing.Self:
+        self._filters.extend(list(func))
         return self
 
-    def collect(self, func: collections.abc.Callable = None) -> typing.Any:
+    def collect(self, func: collections.abc.Callable[[contracts.Stream[T]], typing.Any] = None) -> typing.Any:
         stream = self._stream
         for filter_func in self._filters:
             stream = filter(filter_func, stream)
 
         for map_func in self._mappers:
             stream = map(map_func, stream)
```

### Comparing `streamlord-0.1.1/PKG-INFO` & `streamlord-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlord
-Version: 0.1.1
+Version: 0.2.0
 Summary: Collection of tools to manipulate data streams
 Home-page: https://github.com/smairon/streamlord
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


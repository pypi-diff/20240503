# Comparing `tmp/toolfuse-0.1.19.tar.gz` & `tmp/toolfuse-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolfuse-0.1.19.tar", max compression
+gzip compressed data, was "toolfuse-0.1.20.tar", max compression
```

## Comparing `toolfuse-0.1.19.tar` & `toolfuse-0.1.20.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.19/LICENSE
--rw-r--r--   0        0        0     3333 2024-04-08 16:29:21.395807 toolfuse-0.1.19/README.md
--rw-r--r--   0        0        0      803 2024-04-27 21:02:12.438459 toolfuse-0.1.19/pyproject.toml
--rw-r--r--   0        0        0      341 2024-04-08 15:50:27.209682 toolfuse-0.1.19/toolfuse/__init__.py
--rw-r--r--   0        0        0    24639 2024-04-27 21:02:27.158378 toolfuse-0.1.19/toolfuse/base.py
--rw-r--r--   0        0        0      197 2024-04-27 21:02:03.126589 toolfuse-0.1.19/toolfuse/models.py
--rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 toolfuse-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.20/LICENSE
+-rw-r--r--   0        0        0     3333 2024-04-08 16:29:21.395807 toolfuse-0.1.20/README.md
+-rw-r--r--   0        0        0      803 2024-05-03 14:54:55.333238 toolfuse-0.1.20/pyproject.toml
+-rw-r--r--   0        0        0      341 2024-04-08 15:50:27.209682 toolfuse-0.1.20/toolfuse/__init__.py
+-rw-r--r--   0        0        0    24683 2024-05-03 14:54:29.536468 toolfuse-0.1.20/toolfuse/base.py
+-rw-r--r--   0        0        0      197 2024-04-27 21:02:03.126589 toolfuse-0.1.20/toolfuse/models.py
+-rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 toolfuse-0.1.20/PKG-INFO
```

### Comparing `toolfuse-0.1.19/LICENSE` & `toolfuse-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.19/README.md` & `toolfuse-0.1.20/README.md`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.19/pyproject.toml` & `toolfuse-0.1.20/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toolfuse"
-version = "0.1.19"
+version = "0.1.20"
 description = "Tools for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "toolfuse"}]
 
 [tool.poetry.dependencies]
```

### Comparing `toolfuse-0.1.19/toolfuse/base.py` & `toolfuse-0.1.20/toolfuse/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,16 @@
         return cls.__name__
 
     def ref(self) -> V1ToolRef:
         """Tool reference"""
         module = getmodule(self)
         if not module:
             raise ValueError("Tool not associated with a module")
-        version = pkgversion(module.__name__)
+        mod_parts = module.__name__.split(".")
+        version = pkgversion(mod_parts[0])
         return V1ToolRef(module=module.__name__, name=self.name(), version=version)
 
 
 def tool_from_cls(cls: Type[T]) -> Type[Tool]:
     """
     Dynamically creates a subclass of `Tool` that integrates methods from a given class `cls` as actions.
```

### Comparing `toolfuse-0.1.19/PKG-INFO` & `toolfuse-0.1.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolfuse
-Version: 0.1.19
+Version: 0.1.20
 Summary: Tools for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


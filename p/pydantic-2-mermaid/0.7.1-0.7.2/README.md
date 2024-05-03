# Comparing `tmp/pydantic_2_mermaid-0.7.1.tar.gz` & `tmp/pydantic_2_mermaid-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_2_mermaid-0.7.1.tar", max compression
+gzip compressed data, was "pydantic_2_mermaid-0.7.2.tar", max compression
```

## Comparing `pydantic_2_mermaid-0.7.1.tar` & `pydantic_2_mermaid-0.7.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1091 2023-11-26 11:38:53.460684 pydantic_2_mermaid-0.7.1/LICENSE
--rw-r--r--   0        0        0     4240 2023-12-10 11:46:34.128890 pydantic_2_mermaid-0.7.1/README.md
--rw-r--r--   0        0        0     1283 2024-02-28 13:17:14.241730 pydantic_2_mermaid-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      284 2024-02-20 14:38:46.415991 pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/__init__.py
--rw-r--r--   0        0        0     3231 2024-02-24 06:16:07.249079 pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/__main__.py
--rw-r--r--   0        0        0     4189 2024-02-24 06:28:10.759087 pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/mermaid_generator.py
--rw-r--r--   0        0        0     1738 2024-02-25 07:23:54.269783 pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/models.py
--rw-r--r--   0        0        0        0 2023-11-24 13:39:51.492967 pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/py.typed
--rw-r--r--   0        0        0     4917 2024-02-25 17:56:52.619782 pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/pydantic_parser.py
--rw-r--r--   0        0        0      551 2024-02-25 07:57:23.189783 pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/template.j2
--rw-r--r--   0        0        0     5099 1970-01-01 00:00:00.000000 pydantic_2_mermaid-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/LICENSE
+-rw-r--r--   0        0        0     4240 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/README.md
+-rw-r--r--   0        0        0     1354 2024-05-03 14:45:40.465070 pydantic_2_mermaid-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      284 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/__init__.py
+-rw-r--r--   0        0        0     3264 2024-05-03 14:38:55.094076 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/__main__.py
+-rw-r--r--   0        0        0     4189 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/mermaid_generator.py
+-rw-r--r--   0        0        0     1727 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/models.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/py.typed
+-rw-r--r--   0        0        0     5019 2024-05-03 14:38:55.094076 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/pydantic_parser.py
+-rw-r--r--   0        0        0      551 2024-05-02 13:49:34.267153 pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/template.j2
+-rw-r--r--   0        0        0     5099 1970-01-01 00:00:00.000000 pydantic_2_mermaid-0.7.2/PKG-INFO
```

### Comparing `pydantic_2_mermaid-0.7.1/LICENSE` & `pydantic_2_mermaid-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_2_mermaid-0.7.1/README.md` & `pydantic_2_mermaid-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_2_mermaid-0.7.1/pyproject.toml` & `pydantic_2_mermaid-0.7.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-2-mermaid"
-version = "0.7.1"
+version = "0.7.2"
 description = "Convert pydantic 2.0.3+ classes to markdown mermaid class charts"
 authors = ["Eric Websmith <eric.websmith@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pydantic_mermaid", from = "src" }]
 homepage = "https://github.com/EricWebsmith/pydantic-2-mermaid"
 
 # Specify the classifiers
@@ -17,18 +17,18 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 importlib-resources = "^6.1.1"
 jinja2 = "^3.1.3"
 pydantic = "^2.0.3"
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^1.8.0"
-pytest = "^7.4.0"
-pytest-cov = "^4.1.0"
-ruff = "^0.1.13"
+mypy = "^1.10.0"
+ruff = "^0.4.2"
+pytest = "^8.2.0"
+pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 pydantic-mermaid = 'pydantic_mermaid.__main__:main'
@@ -42,7 +42,11 @@
 line-length = 120
 
 [tool.ruff.lint]
 extend-select = ["T20", "I", "N", "C4", "PT", "RET", "SIM", "PTH", "PL", "RUF", "B"]
 
 [tool.ruff.lint.isort]
 known-first-party = ["pydantic_mermaid"]
+
+[tool.mypy]
+strict = true
+enable_error_code = ["ignore-without-code"]
```

### Comparing `pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/__main__.py` & `pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,17 @@
                     spec.loader.exec_module(module)
                     return module
 
             logger.error(f"Failed to import module from file {path}")  # pragma: no cover
             sys.exit(1)  # pragma: no cover
 
         return importlib.import_module(path)
-    except ModuleNotFoundError:  # pragma: no cover
+    except ModuleNotFoundError as e:  # pragma: no cover
         logger.error("The --module argument must be a module path separated by dots or a valid filepath")
+        logger.exception(e)
         sys.exit(1)
 
 
 def _parse_cli_args() -> argparse.Namespace:
     """
     Parses the command-line arguments passed to pydantic-mermaid.
     """
```

### Comparing `pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/mermaid_generator.py` & `pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/mermaid_generator.py`

 * *Files identical despite different names*

### Comparing `pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/models.py` & `pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Enum for representing the different types of relationships between classes."""
 
     Inheritance = auto()
     Dependency = auto()
     Both = Inheritance | Dependency
 
     def __str__(self) -> str:
-        return self.name.lower()  # type: ignore
+        return str(self.name).lower()
 
     def __repr__(self) -> str:  # pragma: no cover
         return str(self)
 
     @staticmethod
     def parse(s: str) -> "Relations":
         """Convert a string to a Relations enum"""
```

### Comparing `pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/pydantic_parser.py` & `pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/pydantic_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Parse pydantic 2.10 module to mermaid graph"""
+
 from enum import EnumMeta
 from types import ModuleType
 from typing import Any, Dict, List, Set, Type, get_args, get_origin
 
 from pydantic import BaseModel
 
 # ModelMetaclass is commonly used pydantic related packages, and we need to import it here
@@ -13,55 +14,63 @@
 
 from pydantic_mermaid.models import MermaidClass, MermaidGraph, Property
 
 NoneType = type(None)  # There is no NoneType in python 3.8
 base_types = [str, int, float, bool]
 
 
-def _get_name(v: Type[Any]) -> str:  # noqa: PLR0911
+def type_normalize(type_name: str) -> str:
+    if type_name == "NoneType":
+        return "None"
+
+    if type_name == "UnionType":
+        return "Union"
+
+    return type_name
+
+
+def _get_name(v: Type[Any]) -> str:
     """get name from type"""
     if v in base_types:
         return v.__name__
 
     # Support literal inner parts, like Literal[True, False]
     if type(v) in base_types:
         if isinstance(v, str):
             return f"'{v}'"
         return str(v)
 
     origin = get_origin(v)
     if origin is None:
-        if v == Ellipsis:  # type: ignore
-            return "..."
-
-        return v.__name__
+        return "..." if v == Ellipsis else type_normalize(v.__name__)  # type: ignore[comparison-overlap]
 
     # In python 3.8 Union has _name attribute
     if hasattr(origin, "_name"):
         origin_name = origin._name
     elif hasattr(origin, "__name__"):
         origin_name = origin.__name__
     sub_names = [_get_name(sub_type) for sub_type in get_args(v)]
 
-    if hasattr(v, "_name") and v._name == "Optional" and len(sub_names) == 2 and sub_names[-1] == "NoneType":  # noqa: PLR2004
-        return f"Optional[{sub_names[0]}]"
+    origin_name = type_normalize(origin_name)
+    if origin_name == "Union":
+        return " | ".join(sub_names)
 
     return f"{origin_name}[{', '.join(sub_names)}]"
 
 
 def _get_dependencies(v: Type[Any]) -> Set[str]:
     """get dependencies from property types"""
     ans: Set[str] = set()
 
     if v in base_types:
         return ans
 
     origin = get_origin(v)
 
-    if origin is None and hasattr(v, "__name__") and v != NoneType:  # type: ignore
+    if origin is None and hasattr(v, "__name__") and v != NoneType:
         ans.add(v.__name__)
 
     if origin is not None:
         for sub_v in get_args(v):
             ans |= _get_dependencies(sub_v)
 
     return ans
```

### Comparing `pydantic_2_mermaid-0.7.1/src/pydantic_mermaid/template.j2` & `pydantic_2_mermaid-0.7.2/src/pydantic_mermaid/template.j2`

 * *Files identical despite different names*

### Comparing `pydantic_2_mermaid-0.7.1/PKG-INFO` & `pydantic_2_mermaid-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-2-mermaid
-Version: 0.7.1
+Version: 0.7.2
 Summary: Convert pydantic 2.0.3+ classes to markdown mermaid class charts
 Home-page: https://github.com/EricWebsmith/pydantic-2-mermaid
 Author: Eric Websmith
 Author-email: eric.websmith@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


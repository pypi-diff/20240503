# Comparing `tmp/firebird_base-1.7.2.tar.gz` & `tmp/firebird_base-1.8.0.tar.gz`

## Comparing `firebird_base-1.7.2.tar` & `firebird_base-1.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/__init__.py
--rw-r--r--   0        0        0    13725 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/buffer.py
--rw-r--r--   0        0        0    23625 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/collections.py
--rw-r--r--   0        0        0   105343 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/config.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/config_pb2.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/config_pb2.pyi
--rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/hooks.py
--rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/logging.py
--rw-r--r--   0        0        0     9940 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/protobuf.py
--rw-r--r--   0        0        0    13088 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/signal.py
--rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/strconv.py
--rw-r--r--   0        0        0    23827 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/trace.py
--rw-r--r--   0        0        0    16483 2020-02-02 00:00:00.000000 firebird_base-1.7.2/src/firebird/base/types.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 firebird_base-1.7.2/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 firebird_base-1.7.2/LICENSE
--rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 firebird_base-1.7.2/README.md
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 firebird_base-1.7.2/pyproject.toml
--rw-r--r--   0        0        0    10202 2020-02-02 00:00:00.000000 firebird_base-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/__init__.py
+-rw-r--r--   0        0        0    13725 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/buffer.py
+-rw-r--r--   0        0        0    23625 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/collections.py
+-rw-r--r--   0        0        0   108416 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/config.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/config_pb2.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/config_pb2.pyi
+-rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/hooks.py
+-rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/logging.py
+-rw-r--r--   0        0        0     9940 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/protobuf.py
+-rw-r--r--   0        0        0    13088 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/signal.py
+-rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/strconv.py
+-rw-r--r--   0        0        0    23827 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/trace.py
+-rw-r--r--   0        0        0    16483 2020-02-02 00:00:00.000000 firebird_base-1.8.0/src/firebird/base/types.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 firebird_base-1.8.0/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 firebird_base-1.8.0/LICENSE
+-rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 firebird_base-1.8.0/README.md
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 firebird_base-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0    10202 2020-02-02 00:00:00.000000 firebird_base-1.8.0/PKG-INFO
```

### Comparing `firebird_base-1.7.2/src/firebird/base/buffer.py` & `firebird_base-1.8.0/src/firebird/base/buffer.py`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/src/firebird/base/collections.py` & `firebird_base-1.8.0/src/firebird/base/collections.py`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/src/firebird/base/config.py` & `firebird_base-1.8.0/src/firebird/base/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,18 @@
 from typing import Generic, Type, Any, List, Dict, Union, Sequence, Callable, Optional, \
      TypeVar, cast, get_type_hints
 from abc import ABC, abstractmethod
 import platform
 from pathlib import Path
 from uuid import UUID
 from decimal import Decimal, DecimalException
-from configparser import ConfigParser, DEFAULTSECT
+from configparser import (ConfigParser, DEFAULTSECT, ExtendedInterpolation,
+                          MAX_INTERPOLATION_DEPTH, InterpolationDepthError,
+                          InterpolationSyntaxError, NoSectionError, NoOptionError,
+                          InterpolationMissingOptionError)
 from inspect import signature, Signature, Parameter
 from enum import Enum, Flag
 import os
 from .config_pb2 import ConfigProto
 from .types import Error, MIME, ZMQAddress, PyExpr, PyCode, PyCallable
 from .strconv import get_convertor, convert_to_str, Convertor
 
@@ -136,14 +139,82 @@
     return members, not_covered
 
 def _power_of_two(value):
     if value < 1:
         return False
     return value == 2 ** (value.bit_length() - 1)
 
+class EnvExtendedInterpolation(ExtendedInterpolation):
+    """.. versionadded:: 1.8.0
+
+    Modified version of `configparser.ExtendedInterpolation` class that adds special
+    handling for "env" section that returns value of specified environment variable,
+    or empty string if such variable is not defined.
+
+    Example::
+
+       ${env:path} is reference to PATH environment variable.
+    """
+    def _interpolate_some(self, parser, option, accum, rest, section, map,
+                          depth):
+        rawval = parser.get(section, option, raw=True, fallback=rest)
+        if depth > MAX_INTERPOLATION_DEPTH:
+            raise InterpolationDepthError(option, section, rawval)
+        while rest:
+            p = rest.find("$")
+            if p < 0:
+                accum.append(rest)
+                return
+            if p > 0:
+                accum.append(rest[:p])
+                rest = rest[p:]
+            # p is no longer used
+            c = rest[1:2]
+            if c == "$":
+                accum.append("$")
+                rest = rest[2:]
+            elif c == "{":
+                m = self._KEYCRE.match(rest)
+                if m is None:
+                    raise InterpolationSyntaxError(option, section,
+                        "bad interpolation variable reference %r" % rest)
+                path = m.group(1).split(':')
+                rest = rest[m.end():]
+                sect = section
+                opt = option
+                try:
+                    if len(path) == 1:
+                        opt = parser.optionxform(path[0])
+                        v = map[opt]
+                    elif len(path) == 2:
+                        sect = path[0]
+                        opt = parser.optionxform(path[1])
+                        if sect == 'env':
+                            v = os.getenv(opt.upper(), '')
+                        else:
+                            v = parser.get(sect, opt, raw=True)
+                    else:
+                        raise InterpolationSyntaxError(
+                            option, section,
+                            "More than one ':' found: %r" % (rest,))
+                except (KeyError, NoSectionError, NoOptionError):
+                    raise InterpolationMissingOptionError(
+                        option, section, rawval, ":".join(path)) from None
+                if "$" in v:
+                    self._interpolate_some(parser, opt, accum, v, sect,
+                                           dict(parser.items(sect, raw=True)),
+                                           depth + 1)
+                else:
+                    accum.append(v)
+            else:
+                raise InterpolationSyntaxError(
+                    option, section,
+                    "'$' must be followed by '$' or '{', "
+                    "found: %r" % (rest,))
+
 class DirectoryScheme:
     """Class that provide paths to typically used application directories.
 
     Default scheme uses HOME directory as root for other directories. The HOME is
     determined as follows:
 
     1. If environment variable `<app_name>_HOME` exists, its value is used as HOME directory.
```

### Comparing `firebird_base-1.7.2/src/firebird/base/config_pb2.py` & `firebird_base-1.8.0/src/firebird/base/config_pb2.py`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/src/firebird/base/config_pb2.pyi` & `firebird_base-1.8.0/src/firebird/base/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/src/firebird/base/hooks.py` & `firebird_base-1.8.0/src/firebird/base/hooks.py`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/src/firebird/base/logging.py` & `firebird_base-1.8.0/src/firebird/base/logging.py`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/src/firebird/base/protobuf.py` & `firebird_base-1.8.0/src/firebird/base/protobuf.py`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/src/firebird/base/signal.py` & `firebird_base-1.8.0/src/firebird/base/signal.py`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/src/firebird/base/strconv.py` & `firebird_base-1.8.0/src/firebird/base/strconv.py`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/src/firebird/base/trace.py` & `firebird_base-1.8.0/src/firebird/base/trace.py`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/src/firebird/base/types.py` & `firebird_base-1.8.0/src/firebird/base/types.py`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/.gitignore` & `firebird_base-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/LICENSE` & `firebird_base-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/README.md` & `firebird_base-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `firebird_base-1.7.2/pyproject.toml` & `firebird_base-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.doc]
 detached = false
 platforms = ["linux"]
 dependencies = [
-  "Sphinx>=7.2.6",
+  "Sphinx==7.2.6",
   "sphinx-bootstrap-theme>=0.8.1",
   "sphinx-autodoc-typehints>=1.24.0",
   "doc2dash>=3.0.0"
 ]
 [tool.hatch.envs.doc.scripts]
 build = "cd docs ; make html"
 docset = [
```

### Comparing `firebird_base-1.7.2/PKG-INFO` & `firebird_base-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: firebird-base
-Version: 1.7.2
+Version: 1.8.0
 Summary: Firebird base modules for Python
 Project-URL: Home, https://github.com/FirebirdSQL/python3-base
 Project-URL: Documentation, https://firebird-base.rtfd.io
 Project-URL: Issues, https://github.com/FirebirdSQL/python3-base/issues
 Project-URL: Funding, https://github.com/sponsors/pcisar
 Project-URL: Source, https://github.com/FirebirdSQL/python3-base
 Author-email: Pavel Cisar <pcisar@users.sourceforge.net>
```


# Comparing `tmp/formol-0.7.0.tar.gz` & `tmp/formol-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formol-0.7.0.tar", max compression
+gzip compressed data, was "formol-0.8.0.tar", max compression
```

## Comparing `formol-0.7.0.tar` & `formol-0.8.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0    38303 2024-05-02 16:57:22.098929 formol-0.7.0/formol.py
--rw-r--r--   0        0        0     1786 2024-05-02 16:57:16.522217 formol-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 formol-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    38310 2024-05-03 17:33:50.048934 formol-0.8.0/formol.py
+-rw-r--r--   0        0        0     1786 2024-05-03 17:33:58.382276 formol-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 formol-0.8.0/PKG-INFO
```

### Comparing `formol-0.7.0/formol.py` & `formol-0.8.0/formol.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # pyright: strict
 
 __all__ = [
     'format',
     'format_c_block_comment',
     'format_prefixed_block_comment',
 ]
-__version__ = '0.7.0'
+__version__ = '0.8.0'
 __author__ = 'Philippe Proulx <eepp.ca>'
 
 
 from typing import Dict, Any, Type, TypeVar, Callable, List, Sequence, Union, Pattern, Match, Optional
 from dataclasses import dataclass
 import re
 
@@ -1055,15 +1055,15 @@
 
     # Returns the lines of the preformatted text block `pre`.
     def _pre_lines(self, pre: _Pre):
         return self._new_lines(pre.lines, lambda line: f'    {line}') + ['']
 
     # Returns the lines of the verbatim block `verbatim`.
     def _verbatim_lines(self, verbatim: _Verbatim):
-        return verbatim.lines.copy()
+        return verbatim.lines.copy() + ['']
 
     # Returns the lines of a break.
     def _hr_lines(self, _: _Hr):
         return ['┄' * (self._max_line_len), '']
 
     # Returns the lines of a blockquote.
     def _blockquote_lines(self, bq: _Blockquote):
```

### Comparing `formol-0.7.0/pyproject.toml` & `formol-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [build-system]
 requires = ['poetry-core']
 build-backend = 'poetry.core.masonry.api'
 
 [tool.poetry]
 name = 'formol'
-version = '0.7.0'
+version = '0.8.0'
 description = 'Plain text beautifier'
 license = 'MIT'
 authors = ['Philippe Proulx <eeppeliteloop@gmail.com>']
 repository = 'https://github.com/eepp/formol/'
 classifiers = [
 	'Development Status :: 4 - Beta',
 	'License :: OSI Approved :: MIT License',
```

### Comparing `formol-0.7.0/PKG-INFO` & `formol-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formol
-Version: 0.7.0
+Version: 0.8.0
 Summary: Plain text beautifier
 Home-page: https://github.com/eepp/formol/
 License: MIT
 Author: Philippe Proulx
 Author-email: eeppeliteloop@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```


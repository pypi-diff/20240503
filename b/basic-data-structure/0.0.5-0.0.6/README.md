# Comparing `tmp/basic_data_structure-0.0.5.tar.gz` & `tmp/basic_data_structure-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_data_structure-0.0.5.tar", max compression
+gzip compressed data, was "basic_data_structure-0.0.6.tar", max compression
```

## Comparing `basic_data_structure-0.0.5.tar` & `basic_data_structure-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1081 2024-04-28 08:59:59.054530 basic_data_structure-0.0.5/LICENSE
--rw-r--r--   0        0        0    10047 2024-04-30 22:14:31.641597 basic_data_structure-0.0.5/README.md
--rw-r--r--   0        0        0      226 2024-04-29 21:00:00.031231 basic_data_structure-0.0.5/basic_data_structure/__init__.py
--rw-r--r--   0        0        0      264 2024-04-30 13:24:11.669087 basic_data_structure-0.0.5/basic_data_structure/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-28 08:59:59.055304 basic_data_structure-0.0.5/basic_data_structure/list/__init__.py
--rw-r--r--   0        0        0     1810 2024-04-29 21:02:08.921475 basic_data_structure-0.0.5/basic_data_structure/list/iterators.py
--rw-r--r--   0        0        0     7537 2024-04-30 21:25:30.858355 basic_data_structure-0.0.5/basic_data_structure/list/linked_list.py
--rw-r--r--   0        0        0      462 2024-04-28 12:07:08.784934 basic_data_structure-0.0.5/basic_data_structure/list/list_node.py
--rw-r--r--   0        0        0        0 2024-04-28 10:54:44.865814 basic_data_structure-0.0.5/basic_data_structure/stack/__init__.py
--rw-r--r--   0        0        0     1888 2024-04-30 20:57:16.139682 basic_data_structure-0.0.5/basic_data_structure/stack/stack.py
--rw-r--r--   0        0        0        0 2024-04-28 08:59:59.055652 basic_data_structure-0.0.5/basic_data_structure/tree/__init__.py
--rw-r--r--   0        0        0      611 2024-04-28 11:41:56.300001 basic_data_structure-0.0.5/basic_data_structure/tree/tree_node.py
--rw-r--r--   0        0        0     3080 2024-04-30 22:05:08.355073 basic_data_structure-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    10901 1970-01-01 00:00:00.000000 basic_data_structure-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-28 08:59:59.054530 basic_data_structure-0.0.6/LICENSE
+-rw-r--r--   0        0        0      587 2024-05-03 16:48:03.707999 basic_data_structure-0.0.6/README.md
+-rw-r--r--   0        0        0     4021 2024-05-03 16:48:03.709589 basic_data_structure-0.0.6/basic_data_structure/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-03 11:33:12.350252 basic_data_structure-0.0.6/basic_data_structure/exceptions/__init__.py
+-rw-r--r--   0        0        0      432 2024-05-02 23:47:22.284102 basic_data_structure-0.0.6/basic_data_structure/exceptions/list_exceptions.py
+-rw-r--r--   0        0        0       94 2024-05-02 23:47:22.290260 basic_data_structure-0.0.6/basic_data_structure/exceptions/stack_exceptions.py
+-rw-r--r--   0        0        0       79 2024-05-03 11:33:12.354656 basic_data_structure-0.0.6/basic_data_structure/iterators/__init__.py
+-rw-r--r--   0        0        0      962 2024-05-02 23:47:22.292198 basic_data_structure-0.0.6/basic_data_structure/iterators/list_node_iterator.py
+-rw-r--r--   0        0        0      993 2024-05-02 23:47:22.278518 basic_data_structure-0.0.6/basic_data_structure/iterators/list_value_iterator.py
+-rw-r--r--   0        0        0    15052 2024-05-03 11:26:57.028979 basic_data_structure-0.0.6/basic_data_structure/linked_list.py
+-rw-r--r--   0        0        0       56 2024-05-03 11:32:24.104224 basic_data_structure-0.0.6/basic_data_structure/nodes/__init__.py
+-rw-r--r--   0        0        0      920 2024-05-03 11:26:57.034141 basic_data_structure-0.0.6/basic_data_structure/nodes/list_node.py
+-rw-r--r--   0        0        0     2794 2024-05-03 16:48:03.710129 basic_data_structure-0.0.6/basic_data_structure/nodes/tree_node.py
+-rw-r--r--   0        0        0     3903 2024-05-03 16:48:03.710795 basic_data_structure-0.0.6/basic_data_structure/stack.py
+-rw-r--r--   0        0        0     3775 2024-05-03 16:48:03.711444 basic_data_structure-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 basic_data_structure-0.0.6/PKG-INFO
```

### Comparing `basic_data_structure-0.0.5/LICENSE` & `basic_data_structure-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `basic_data_structure-0.0.5/basic_data_structure/list/iterators.py` & `basic_data_structure-0.0.6/basic_data_structure/iterators/list_value_iterator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,12 @@
-from typing import Any, Optional
-
-from basic_data_structure.list.list_node import ListNode
-
-
-class ListNodeIterator:
-    """Linked list node iterator.
-
-    Iterates through list and returns ListNode.
-    """
-
-    def __init__(self, head: Optional[ListNode]) -> None:
-        """Init iterator.
+"""# List value iterator"""
 
-        Parameters:
-            head: linked list head node
-        """
-        self.__pointer = head
-
-    def __iter__(self) -> 'ListNodeIterator':
-        """Return iterator.
-
-        Returns:
-            iterator (self)
-        """
-        return self
-
-    def __next__(self) -> ListNode:
-        """Retrieve next node from linked list.
-
-        Returns:
-            next ListNode
-
-        Raises:
-            StopIteration: when reached the end of the list
-        """
-        if self.__pointer is None:
-            raise StopIteration
+from typing import Any, Optional
 
-        response = self.__pointer
-        self.__pointer = self.__pointer.next
-        return response
+from basic_data_structure.nodes.list_node import ListNode
 
 
 class ListValueIterator:
     """Linked list value iterator.
 
     Iterates through list and returns value of a ListNode.
     """
```

### Comparing `basic_data_structure-0.0.5/pyproject.toml` & `basic_data_structure-0.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "basic-data-structure"
-version = "0.0.5"
+version = "0.0.6"
 description = "Implementation of basic sata structures in Python"
 authors = ["Mikhail Shagov <mishaga@me.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/mishaga/basic_data_structure"
 keywords = ["data structure", "data structures", "python data structures", "basic data structures"]
 
 [tool.poetry.urls]
 "Issues" = "https://github.com/mishaga/basic_data_structure/issues"
+"Documentation" = "https://mishaga.github.io/basic_data_structure/"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 wemake-python-styleguide = "^0.19.2"
 flake8-pyproject = "^1.2.3"
 pytest = "^8.2.0"
 isort = "^5.13.2"
+pdoc = "^14.4.0"
 
 
 [tool.isort]
 profile = "wemake"
 
 
 [tool.flake8]
@@ -43,30 +45,39 @@
     "magic_method",
     "property_method",
     "static_method",
     "class_method",
     "method",
     "private_method",
 ]
-ignore = ["D100", "D104", "WPS112"]
+ignore = ["D300", "D301", "D400", "RST214", "RST215", "RST201", "RST213", "RST301", "WPS112"]
 per-file-ignores = [
-    "*/__init__.py: F401, WPS300, WPS412",
+    "*/__init__.py: F401, WPS412",
 ]
 # B001   – Do not use bare except
 # B008   – Do not perform function calls in argument defaults
 # D100   – Missing docstring in public module
+# D103   – Missing docstring in public function
 # D104   – Missing docstring in public package
+# D300   – Use """triple double quotes"""
+# D301   – Use r""" if any backslashes in a docstring
+# D400   – First line should end with a period
 # DAR101 – Missing parameter(s) in Docstring
 # DAR201 – Missing "Returns" in Docstring
 # DAR301 – Missing "Yields" in Docstring
 # DAR401 – Missing exception in Raises section
 # E722   – Do not use bare except
 # F401   – Imported but unused
 # E711   – comparison to None
 # N805   – first argument of a method should be named 'self'
+# RST214 – Inline literal start-string without end-string
+# RST215 – Inline interpreted text or phrase reference start-string without end-string
+# RST201 – Block quote ends without a blank line; unexpected unindent
+# RST213 – Inline emphasis start-string without end-string
+# RST301 – Unexpected indentation
 # S101   – Use of assert detected
 # WPS110 – Found wrong variable name
 # WPS112 – Found private name pattern
 # WPS115 – Found upper-case constant in a class
 # WPS201 – Found module with too many imports
 # WPS202 – Found too many module members
 # WPS204 – Found overused expression
@@ -87,9 +98,10 @@
 # WPS323 – Found % string formatting
 # WPS404 – Found complex default value
 # WPS412 – Found `__init__.py` module with logic
 # WPS432 – Found magic number
 # WPS442 – Found outer scope names shadowing
 # WPS450 – Found protected object import
 # WPS451 – Found positional-only argument
+# WPS507 – Found useless `len()` compare
 # WPS520 – Found compare with falsy constant
 # Q001   – Single quote multiline found but double quotes preferred
```


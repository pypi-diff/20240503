# Comparing `tmp/gr1336_toolbox-0.0.2.tar.gz` & `tmp/gr1336_toolbox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gr1336_toolbox-0.0.2.tar", last modified: Thu May  2 16:00:12 2024, max compression
+gzip compressed data, was "gr1336_toolbox-0.0.3.tar", last modified: Fri May  3 03:03:42 2024, max compression
```

## Comparing `gr1336_toolbox-0.0.2.tar` & `gr1336_toolbox-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:00:12.856040 gr1336_toolbox-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 16:00:12.856040 gr1336_toolbox-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:00:12.856040 gr1336_toolbox-0.0.2/gr1336_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/misc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/test_even_odd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/text_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/types_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:00:12.856040 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 16:00:12.000000 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 16:00:12.000000 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:00:12.000000 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 16:00:12.000000 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 16:00:12.000000 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:00:12.856040 gr1336_toolbox-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:03:42.137633 gr1336_toolbox-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-03 03:03:42.137633 gr1336_toolbox-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:03:42.137633 gr1336_toolbox-0.0.3/gr1336_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/misc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/test_even_odd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/text_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/types_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:03:42.137633 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-03 03:03:42.000000 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-03 03:03:42.000000 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 03:03:42.000000 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 03:03:42.000000 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 03:03:42.000000 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 03:03:42.137633 gr1336_toolbox-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/setup.py
```

### Comparing `gr1336_toolbox-0.0.2/LICENSE` & `gr1336_toolbox-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.2/PKG-INFO` & `gr1336_toolbox-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.0.2
+Version: 0.0.3
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License:  Apache Software License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `gr1336_toolbox-0.0.2/gr1336_toolbox/__init__.py` & `gr1336_toolbox-0.0.3/gr1336_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.2/gr1336_toolbox/file_manager.py` & `gr1336_toolbox-0.0.3/gr1336_toolbox/file_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import pyarrow as pa
 from typing import Any
 from pathlib import Path
 import pyarrow.parquet as pq
 from .types_check import _path
 
 
-def get_dirs(path: str | Path) -> list[str]:
+def get_dirs(path: str | Path) -> list[Path]:
     if not _path(path):
         return []
-    return [str(x) for x in Path(path).glob("*") if x.is_dir()]
+    return [x for x in Path(path).glob("*") if x.is_dir()]
 
 
-def get_files(path: str | Path, extension: str | None = None) -> list[str]:
+def get_files(path: str | Path, extension: str | None = None) -> list[Path]:
     if not _path(path):
         return []
     if not extension:
-        return [str(x) for x in Path(path).glob("*") if x.is_file()]
+        return [x for x in Path(path).glob("*") if x.is_file()]
     return [x for x in Path(path).glob(f"*.{extension}") if x.is_file()]
 
 
 def _create(path: str | Path):
     Path(path).parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `gr1336_toolbox-0.0.2/gr1336_toolbox/misc_tools.py` & `gr1336_toolbox-0.0.3/gr1336_toolbox/misc_tools.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.2/gr1336_toolbox/test_even_odd.py` & `gr1336_toolbox-0.0.3/gr1336_toolbox/test_even_odd.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.2/gr1336_toolbox/text_tools.py` & `gr1336_toolbox-0.0.3/gr1336_toolbox/text_tools.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.2/gr1336_toolbox/types_check.py` & `gr1336_toolbox-0.0.3/gr1336_toolbox/types_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         return isinstance(entry, dict)
     return bool(entry)
 
 
 def _compare(arg1: Any | None, arg2: Any) -> Any:
     """
     arg1 if its not None or arg2.
-    It considers fasely values from the first arg.
+    It considers falsely values from the first arg.
     Falsely are usualy: (0, "", {}, False, [])
     """
     return arg1 if arg1 is not None else arg2
 
 
 def _path(entry) -> bool:
     if _str(entry):
```

### Comparing `gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/PKG-INFO` & `gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.0.2
+Version: 0.0.3
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License:  Apache Software License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `gr1336_toolbox-0.0.2/setup.py` & `gr1336_toolbox-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    version="0.0.2",
+    version="0.0.3",
     name="gr1336_toolbox",
     description="Personal collection of reusable tools in python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gr1336/gr1336_toolbox/",
     install_requires=["numpy", "pyperclip", "textblob", "pyyaml", "pyarrow"],
     author="gr1336",
```


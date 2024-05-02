# Comparing `tmp/daffodil-0.4.2.tar.gz` & `tmp/daffodil-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daffodil-0.4.2.tar", last modified: Thu May  2 03:52:56 2024, max compression
+gzip compressed data, was "daffodil-0.4.3.tar", last modified: Thu May  2 16:51:43 2024, max compression
```

## Comparing `daffodil-0.4.2.tar` & `daffodil-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 03:52:56.530249 daffodil-0.4.2/
--rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.4.2/LICENSE
--rw-rw-rw-   0        0        0    54014 2024-05-02 03:52:56.527255 daffodil-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0    53364 2024-05-01 01:35:13.000000 daffodil-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 03:52:56.524249 daffodil-0.4.2/daffodil.egg-info/
--rw-rw-rw-   0        0        0    54014 2024-05-02 03:52:56.000000 daffodil-0.4.2/daffodil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-02 03:52:56.000000 daffodil-0.4.2/daffodil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 03:52:56.000000 daffodil-0.4.2/daffodil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-02 03:52:56.000000 daffodil-0.4.2/daffodil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 03:52:56.000000 daffodil-0.4.2/daffodil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      766 2024-05-02 03:32:58.000000 daffodil-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-02 03:52:56.530249 daffodil-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      903 2024-05-02 03:32:58.000000 daffodil-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 03:52:56.521252 daffodil-0.4.2/tests/
--rw-rw-rw-   0        0        0   164640 2024-05-02 03:32:58.000000 daffodil-0.4.2/tests/test_daf.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:51:43.175856 daffodil-0.4.3/
+-rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0    54019 2024-05-02 16:51:43.172860 daffodil-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0    53364 2024-05-01 01:35:13.000000 daffodil-0.4.3/README.md
+-rw-rw-rw-   0        0        0      819 2024-05-02 16:49:22.000000 daffodil-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 16:51:43.175856 daffodil-0.4.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 16:51:43.115857 daffodil-0.4.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 16:51:43.130864 daffodil-0.4.3/src/daffodil/
+-rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.4.3/src/daffodil/__init__.py
+-rw-rw-rw-   0        0        0   200471 2024-05-02 16:49:22.000000 daffodil-0.4.3/src/daffodil/daf.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:51:43.163855 daffodil-0.4.3/src/daffodil/lib/
+-rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.4.3/src/daffodil/lib/__init__.py
+-rw-rw-rw-   0        0        0    43220 2024-05-02 16:49:22.000000 daffodil-0.4.3/src/daffodil/lib/daf_indexing.py
+-rw-rw-rw-   0        0        0    31645 2024-05-02 16:49:22.000000 daffodil-0.4.3/src/daffodil/lib/daf_md.py
+-rw-rw-rw-   0        0        0     7708 2024-05-02 16:49:22.000000 daffodil-0.4.3/src/daffodil/lib/daf_pandas.py
+-rw-rw-rw-   0        0        0     5174 2024-05-02 03:32:58.000000 daffodil-0.4.3/src/daffodil/lib/daf_types.py
+-rw-rw-rw-   0        0        0    51145 2024-05-02 03:32:58.000000 daffodil-0.4.3/src/daffodil/lib/daf_utils.py
+-rw-rw-rw-   0        0        0     5796 2024-05-02 03:32:58.000000 daffodil-0.4.3/src/daffodil/lib/md_demo.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:51:43.170852 daffodil-0.4.3/src/daffodil.egg-info/
+-rw-rw-rw-   0        0        0    54019 2024-05-02 16:51:43.000000 daffodil-0.4.3/src/daffodil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2024-05-02 16:51:43.000000 daffodil-0.4.3/src/daffodil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 16:51:43.000000 daffodil-0.4.3/src/daffodil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-02 16:51:43.000000 daffodil-0.4.3/src/daffodil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 16:51:43.000000 daffodil-0.4.3/src/daffodil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 16:51:43.166855 daffodil-0.4.3/tests/
+-rw-rw-rw-   0        0        0   164684 2024-05-02 16:49:22.000000 daffodil-0.4.3/tests/test_daf.py
```

### Comparing `daffodil-0.4.2/LICENSE` & `daffodil-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `daffodil-0.4.2/PKG-INFO` & `daffodil-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: daffodil
-Version: 0.4.2
+Version: 0.4.3
 Summary: Daffodil provides lightweight and fast 2-D dataframes
-Home-page: https://github.com/raylutz/daffodil
-Author: Ray Lutz
-Author-email: raylutz@cognisys.com
+Author-email: Ray Lutz <raylutz@cognisys.com>
 License: MIT
+Project-URL: Homepage, https://github.com/raylutz/daffodil
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `daffodil-0.4.2/README.md` & `daffodil-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `daffodil-0.4.2/daffodil.egg-info/PKG-INFO` & `daffodil-0.4.3/src/daffodil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: daffodil
-Version: 0.4.2
+Version: 0.4.3
 Summary: Daffodil provides lightweight and fast 2-D dataframes
-Home-page: https://github.com/raylutz/daffodil
-Author: Ray Lutz
-Author-email: raylutz@cognisys.com
+Author-email: Ray Lutz <raylutz@cognisys.com>
 License: MIT
+Project-URL: Homepage, https://github.com/raylutz/daffodil
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `daffodil-0.4.2/tests/test_daf.py` & `daffodil-0.4.3/tests/test_daf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # test_daf
 # copyright (c) 2024 Ray Lutz
 
-#import os
+import os
 import sys
 import unittest
 import numpy as np
 import pandas as pd
 #from io import BytesIO
 from pathlib import Path
-sys.path.append('..')
+sys.path.append(os.path.join(os.path.dirname(sys.path[0]), 'src'))
 
 from daffodil.daf import Daf
 from daffodil.lib import daf_utils as utils
 
 class TestDaf(unittest.TestCase):
 
     maxDiff = None
```


# Comparing `tmp/cli-nb2py-0.7.0.tar.gz` & `tmp/cli-nb2py-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-nb2py-0.7.0.tar", last modified: Fri May  3 14:16:09 2024, max compression
+gzip compressed data, was "cli-nb2py-0.7.1.tar", last modified: Fri May  3 14:34:31 2024, max compression
```

## Comparing `cli-nb2py-0.7.0.tar` & `cli-nb2py-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:16:09.630922 cli-nb2py-0.7.0/
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     1072 2024-05-03 14:09:37.000000 cli-nb2py-0.7.0/LICENSE
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 14:16:09.630731 cli-nb2py-0.7.0/PKG-INFO
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     2892 2024-05-03 14:12:12.000000 cli-nb2py-0.7.0/README.md
-drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:16:09.629746 cli-nb2py-0.7.0/cli_nb2py/
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:09:37.000000 cli-nb2py-0.7.0/cli_nb2py/__init__.py
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     4560 2024-05-03 14:10:01.000000 cli-nb2py-0.7.0/cli_nb2py/main.py
-drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:16:09.630490 cli-nb2py-0.7.0/cli_nb2py.egg-info/
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/PKG-INFO
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)      266 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/SOURCES.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)        1 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/dependency_links.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)       46 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/entry_points.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)        9 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/requires.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)       10 2024-05-03 14:16:09.000000 cli-nb2py-0.7.0/cli_nb2py.egg-info/top_level.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)       38 2024-05-03 14:16:09.630957 cli-nb2py-0.7.0/setup.cfg
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)      834 2024-05-03 14:10:13.000000 cli-nb2py-0.7.0/setup.py
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:34:31.021706 cli-nb2py-0.7.1/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     1072 2024-05-03 14:09:37.000000 cli-nb2py-0.7.1/LICENSE
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 14:34:31.021464 cli-nb2py-0.7.1/PKG-INFO
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     2892 2024-05-03 14:12:12.000000 cli-nb2py-0.7.1/README.md
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:34:31.020492 cli-nb2py-0.7.1/cli_nb2py/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:09:37.000000 cli-nb2py-0.7.1/cli_nb2py/__init__.py
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     4713 2024-05-03 14:33:03.000000 cli-nb2py-0.7.1/cli_nb2py/main.py
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:34:31.021231 cli-nb2py-0.7.1/cli_nb2py.egg-info/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 14:34:30.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/PKG-INFO
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)      266 2024-05-03 14:34:31.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/SOURCES.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        1 2024-05-03 14:34:30.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/dependency_links.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       46 2024-05-03 14:34:30.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/entry_points.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        9 2024-05-03 14:34:30.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/requires.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       10 2024-05-03 14:34:30.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/top_level.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       38 2024-05-03 14:34:31.021744 cli-nb2py-0.7.1/setup.cfg
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)      834 2024-05-03 14:33:50.000000 cli-nb2py-0.7.1/setup.py
```

### Comparing `cli-nb2py-0.7.0/LICENSE` & `cli-nb2py-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-nb2py-0.7.0/PKG-INFO` & `cli-nb2py-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-nb2py
-Version: 0.7.0
+Version: 0.7.1
 Summary: Reliable Notebook to Python converter
 Home-page: https://github.com/BardiaKh/nb2py
 Author: Bardia Khosravi
 Author-email: bardiakhosravi95@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cli-nb2py-0.7.0/README.md` & `cli-nb2py-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cli-nb2py-0.7.0/cli_nb2py/main.py` & `cli-nb2py-0.7.1/cli_nb2py/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import argparse
 import json
 import os
+import re
 
 header_comment = '# %%\n'
 
 def is_import_line(line):
     return line.startswith('import ') or line.startswith('from ')
 
+def escape_double_quotes(line):
+    return re.sub(r'(?<!\\)"', '\\"', line)
+
 def nb2py(notebook):
     imports = []
     os_modifications = []
     sys_modifications = []
     main_code = []
     cell_separator = '\n\n#---\n\n'  # Separator for cell contents
 
@@ -39,25 +43,25 @@
                 if line.strip().startswith("!") or line.strip().startswith("%"):
                     line = f"##{line}"
 
                 # Check for triple quotes
                 if '"""' in line:
                     if in_multiline_string:
                         # End of multiline string
-                        multiline_string_content.append(line.replace('"""', ''))
+                        multiline_string_content.append(escape_double_quotes(line.replace('"""', '')))
                         cell_content.append('"' + '\\n" +\\\n"'.join(multiline_string_content) + '\\n"')
                         in_multiline_string = False
                         multiline_string_content = []
                     else:
                         # Start of multiline string
                         in_multiline_string = True
-                        multiline_string_content.append(line.replace('"""', ''))
+                        multiline_string_content.append(escape_double_quotes(line.replace('"""', '')))
                 else:
                     if in_multiline_string:
-                        multiline_string_content.append(line)
+                        multiline_string_content.append(escape_double_quotes(line))
                     else:
                         cell_content.append(line)
 
             if in_multiline_string:
                 cell_content.append('"' + '\\n" +\\\n"'.join(multiline_string_content) + '\\n"')
 
         if cell_content:
```

### Comparing `cli-nb2py-0.7.0/cli_nb2py.egg-info/PKG-INFO` & `cli-nb2py-0.7.1/cli_nb2py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-nb2py
-Version: 0.7.0
+Version: 0.7.1
 Summary: Reliable Notebook to Python converter
 Home-page: https://github.com/BardiaKh/nb2py
 Author: Bardia Khosravi
 Author-email: bardiakhosravi95@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cli-nb2py-0.7.0/setup.py` & `cli-nb2py-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cli-nb2py",
-    version="0.7.0",
+    version="0.7.1",
     author="Bardia Khosravi",
     author_email="bardiakhosravi95@gmail.com",
     description="Reliable Notebook to Python converter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BardiaKh/nb2py",
     packages = setuptools.find_packages(),
```


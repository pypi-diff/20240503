# Comparing `tmp/cli-nb2py-0.7.1.tar.gz` & `tmp/cli-nb2py-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-nb2py-0.7.1.tar", last modified: Fri May  3 14:34:31 2024, max compression
+gzip compressed data, was "cli-nb2py-0.7.2.tar", last modified: Fri May  3 16:27:14 2024, max compression
```

## Comparing `cli-nb2py-0.7.1.tar` & `cli-nb2py-0.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:34:31.021706 cli-nb2py-0.7.1/
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     1072 2024-05-03 14:09:37.000000 cli-nb2py-0.7.1/LICENSE
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 14:34:31.021464 cli-nb2py-0.7.1/PKG-INFO
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     2892 2024-05-03 14:12:12.000000 cli-nb2py-0.7.1/README.md
-drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:34:31.020492 cli-nb2py-0.7.1/cli_nb2py/
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:09:37.000000 cli-nb2py-0.7.1/cli_nb2py/__init__.py
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     4713 2024-05-03 14:33:03.000000 cli-nb2py-0.7.1/cli_nb2py/main.py
-drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:34:31.021231 cli-nb2py-0.7.1/cli_nb2py.egg-info/
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 14:34:30.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/PKG-INFO
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)      266 2024-05-03 14:34:31.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/SOURCES.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)        1 2024-05-03 14:34:30.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/dependency_links.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)       46 2024-05-03 14:34:30.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/entry_points.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)        9 2024-05-03 14:34:30.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/requires.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)       10 2024-05-03 14:34:30.000000 cli-nb2py-0.7.1/cli_nb2py.egg-info/top_level.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)       38 2024-05-03 14:34:31.021744 cli-nb2py-0.7.1/setup.cfg
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)      834 2024-05-03 14:33:50.000000 cli-nb2py-0.7.1/setup.py
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 16:27:14.216766 cli-nb2py-0.7.2/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     1072 2024-05-03 14:09:37.000000 cli-nb2py-0.7.2/LICENSE
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 16:27:14.216573 cli-nb2py-0.7.2/PKG-INFO
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     2892 2024-05-03 14:12:12.000000 cli-nb2py-0.7.2/README.md
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 16:27:14.215584 cli-nb2py-0.7.2/cli_nb2py/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:09:37.000000 cli-nb2py-0.7.2/cli_nb2py/__init__.py
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     4572 2024-05-03 16:26:40.000000 cli-nb2py-0.7.2/cli_nb2py/main.py
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 16:27:14.216343 cli-nb2py-0.7.2/cli_nb2py.egg-info/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/PKG-INFO
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)      266 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/SOURCES.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        1 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/dependency_links.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       46 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/entry_points.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        9 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/requires.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       10 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/top_level.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       38 2024-05-03 16:27:14.216805 cli-nb2py-0.7.2/setup.cfg
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)      834 2024-05-03 15:49:24.000000 cli-nb2py-0.7.2/setup.py
```

### Comparing `cli-nb2py-0.7.1/LICENSE` & `cli-nb2py-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-nb2py-0.7.1/PKG-INFO` & `cli-nb2py-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-nb2py
-Version: 0.7.1
+Version: 0.7.2
 Summary: Reliable Notebook to Python converter
 Home-page: https://github.com/BardiaKh/nb2py
 Author: Bardia Khosravi
 Author-email: bardiakhosravi95@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cli-nb2py-0.7.1/README.md` & `cli-nb2py-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cli-nb2py-0.7.1/cli_nb2py/main.py` & `cli-nb2py-0.7.2/cli_nb2py/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,31 +43,28 @@
                 if line.strip().startswith("!") or line.strip().startswith("%"):
                     line = f"##{line}"
 
                 # Check for triple quotes
                 if '"""' in line:
                     if in_multiline_string:
                         # End of multiline string
-                        multiline_string_content.append(escape_double_quotes(line.replace('"""', '')))
-                        cell_content.append('"' + '\\n" +\\\n"'.join(multiline_string_content) + '\\n"')
+                        multiline_string_content.append(escape_double_quotes(line.replace('"""', '"')))
+                        cell_content.append('"' + '\\n" +\\\n"'.join(multiline_string_content))
                         in_multiline_string = False
                         multiline_string_content = []
                     else:
                         # Start of multiline string
                         in_multiline_string = True
-                        multiline_string_content.append(escape_double_quotes(line.replace('"""', '')))
+                        multiline_string_content.append(escape_double_quotes(line.replace('"""', '"')))
                 else:
                     if in_multiline_string:
                         multiline_string_content.append(escape_double_quotes(line))
                     else:
                         cell_content.append(line)
 
-            if in_multiline_string:
-                cell_content.append('"' + '\\n" +\\\n"'.join(multiline_string_content) + '\\n"')
-
         if cell_content:
             main_code.append('\n'.join(cell_content))
 
     # Insert os.environ and sys.path modifications after their imports
     for i, line in enumerate(imports):
         if 'import os' in line or 'from os import' in line:
             for mod in sorted(os_modifications, reverse=True):
```

### Comparing `cli-nb2py-0.7.1/cli_nb2py.egg-info/PKG-INFO` & `cli-nb2py-0.7.2/cli_nb2py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-nb2py
-Version: 0.7.1
+Version: 0.7.2
 Summary: Reliable Notebook to Python converter
 Home-page: https://github.com/BardiaKh/nb2py
 Author: Bardia Khosravi
 Author-email: bardiakhosravi95@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cli-nb2py-0.7.1/setup.py` & `cli-nb2py-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cli-nb2py",
-    version="0.7.1",
+    version="0.7.2",
     author="Bardia Khosravi",
     author_email="bardiakhosravi95@gmail.com",
     description="Reliable Notebook to Python converter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BardiaKh/nb2py",
     packages = setuptools.find_packages(),
```


# Comparing `tmp/cli-nb2py-0.7.2.tar.gz` & `tmp/cli_nb2py-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-nb2py-0.7.2.tar", last modified: Fri May  3 16:27:14 2024, max compression
+gzip compressed data, was "cli_nb2py-0.7.3.tar", last modified: Fri May  3 18:45:08 2024, max compression
```

## Comparing `cli-nb2py-0.7.2.tar` & `cli_nb2py-0.7.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 16:27:14.216766 cli-nb2py-0.7.2/
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     1072 2024-05-03 14:09:37.000000 cli-nb2py-0.7.2/LICENSE
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 16:27:14.216573 cli-nb2py-0.7.2/PKG-INFO
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     2892 2024-05-03 14:12:12.000000 cli-nb2py-0.7.2/README.md
-drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 16:27:14.215584 cli-nb2py-0.7.2/cli_nb2py/
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:09:37.000000 cli-nb2py-0.7.2/cli_nb2py/__init__.py
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     4572 2024-05-03 16:26:40.000000 cli-nb2py-0.7.2/cli_nb2py/main.py
-drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 16:27:14.216343 cli-nb2py-0.7.2/cli_nb2py.egg-info/
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/PKG-INFO
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)      266 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/SOURCES.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)        1 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/dependency_links.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)       46 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/entry_points.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)        9 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/requires.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)       10 2024-05-03 16:27:14.000000 cli-nb2py-0.7.2/cli_nb2py.egg-info/top_level.txt
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)       38 2024-05-03 16:27:14.216805 cli-nb2py-0.7.2/setup.cfg
--rw-r--r--   0 bardiakhosravi   (501) staff       (20)      834 2024-05-03 15:49:24.000000 cli-nb2py-0.7.2/setup.py
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 18:45:08.531717 cli_nb2py-0.7.3/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     1072 2024-05-03 14:09:37.000000 cli_nb2py-0.7.3/LICENSE
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 18:45:08.531534 cli_nb2py-0.7.3/PKG-INFO
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     2892 2024-05-03 14:12:12.000000 cli_nb2py-0.7.3/README.md
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 18:45:08.530371 cli_nb2py-0.7.3/cli_nb2py/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 14:09:37.000000 cli_nb2py-0.7.3/cli_nb2py/__init__.py
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     4976 2024-05-03 18:40:04.000000 cli_nb2py-0.7.3/cli_nb2py/main.py
+drwxr-xr-x   0 bardiakhosravi   (501) staff       (20)        0 2024-05-03 18:45:08.531357 cli_nb2py-0.7.3/cli_nb2py.egg-info/
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)     3358 2024-05-03 18:45:08.000000 cli_nb2py-0.7.3/cli_nb2py.egg-info/PKG-INFO
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)      266 2024-05-03 18:45:08.000000 cli_nb2py-0.7.3/cli_nb2py.egg-info/SOURCES.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        1 2024-05-03 18:45:08.000000 cli_nb2py-0.7.3/cli_nb2py.egg-info/dependency_links.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       46 2024-05-03 18:45:08.000000 cli_nb2py-0.7.3/cli_nb2py.egg-info/entry_points.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)        9 2024-05-03 18:45:08.000000 cli_nb2py-0.7.3/cli_nb2py.egg-info/requires.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       10 2024-05-03 18:45:08.000000 cli_nb2py-0.7.3/cli_nb2py.egg-info/top_level.txt
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)       38 2024-05-03 18:45:08.531758 cli_nb2py-0.7.3/setup.cfg
+-rw-r--r--   0 bardiakhosravi   (501) staff       (20)      834 2024-05-03 18:43:03.000000 cli_nb2py-0.7.3/setup.py
```

### Comparing `cli-nb2py-0.7.2/LICENSE` & `cli_nb2py-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-nb2py-0.7.2/PKG-INFO` & `cli_nb2py-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-nb2py
-Version: 0.7.2
+Version: 0.7.3
 Summary: Reliable Notebook to Python converter
 Home-page: https://github.com/BardiaKh/nb2py
 Author: Bardia Khosravi
 Author-email: bardiakhosravi95@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cli-nb2py-0.7.2/README.md` & `cli_nb2py-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `cli-nb2py-0.7.2/cli_nb2py/main.py` & `cli_nb2py-0.7.3/cli_nb2py/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 
 def is_import_line(line):
     return line.startswith('import ') or line.startswith('from ')
 
 def escape_double_quotes(line):
     return re.sub(r'(?<!\\)"', '\\"', line)
 
+def process_triple_quotes(line, mode="start"):
+    if mode == "start":
+        line_seg = line.partition('"""')
+        return escape_double_quotes(line_seg[0]) + '"' + escape_double_quotes(line_seg[2])
+    elif mode == "end":
+        line_seg = line.rpartition('"""')
+        return escape_double_quotes(line_seg[0])+ '"' + escape_double_quotes(line_seg[2])
+
 def nb2py(notebook):
     imports = []
     os_modifications = []
     sys_modifications = []
     main_code = []
     cell_separator = '\n\n#---\n\n'  # Separator for cell contents
 
@@ -40,25 +48,25 @@
                 if line.startswith('sys.path'):
                     sys_modifications.append(line)
                     continue
                 if line.strip().startswith("!") or line.strip().startswith("%"):
                     line = f"##{line}"
 
                 # Check for triple quotes
-                if '"""' in line:
+                if '"""' in line and not line.strip().startswith('#') and line.count('"""') % 2 == 1:
                     if in_multiline_string:
-                        # End of multiline string
-                        multiline_string_content.append(escape_double_quotes(line.replace('"""', '"')))
-                        cell_content.append('"' + '\\n" +\\\n"'.join(multiline_string_content))
+                        # Closing triple quotes
+                        multiline_string_content.append(process_triple_quotes(line, mode="end"))
+                        cell_content.append('\\n" +\\\n"'.join(multiline_string_content))
                         in_multiline_string = False
                         multiline_string_content = []
                     else:
-                        # Start of multiline string
+                        # Opening triple quotes
                         in_multiline_string = True
-                        multiline_string_content.append(escape_double_quotes(line.replace('"""', '"')))
+                        multiline_string_content.append(process_triple_quotes(line, mode="start"))
                 else:
                     if in_multiline_string:
                         multiline_string_content.append(escape_double_quotes(line))
                     else:
                         cell_content.append(line)
 
         if cell_content:
```

### Comparing `cli-nb2py-0.7.2/cli_nb2py.egg-info/PKG-INFO` & `cli_nb2py-0.7.3/cli_nb2py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-nb2py
-Version: 0.7.2
+Version: 0.7.3
 Summary: Reliable Notebook to Python converter
 Home-page: https://github.com/BardiaKh/nb2py
 Author: Bardia Khosravi
 Author-email: bardiakhosravi95@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cli-nb2py-0.7.2/setup.py` & `cli_nb2py-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cli-nb2py",
-    version="0.7.2",
+    version="0.7.3",
     author="Bardia Khosravi",
     author_email="bardiakhosravi95@gmail.com",
     description="Reliable Notebook to Python converter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BardiaKh/nb2py",
     packages = setuptools.find_packages(),
```


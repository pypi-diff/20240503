# Comparing `tmp/fico-0.1.0.tar.gz` & `tmp/fico-0.1.1.tar.gz`

## Comparing `fico-0.1.0.tar` & `fico-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 fico-0.1.0/requirements.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 fico-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fico-0.1.0/.vscode/tasks.json
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 fico-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 fico-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fico-0.1.0/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 fico-0.1.0/docs/make.bat
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fico-0.1.0/docs/source/cli.rst
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 fico-0.1.0/docs/source/figurelib.rst
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fico-0.1.0/docs/source/modules.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fico-0.1.0/src/cli/__init__.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 fico-0.1.0/src/cli/build.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 fico-0.1.0/src/fico/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fico-0.1.0/src/fico/__init__.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 fico-0.1.0/src/fico/building.py
--rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 fico-0.1.0/src/fico/figure.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 fico-0.1.0/src/fico/styling.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fico-0.1.0/src/fico/utils.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 fico-0.1.0/src/fico/styles/eit6_publication.mplstyle
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 fico-0.1.0/src/fico/templates/basic_table.tex
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fico-0.1.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fico-0.1.0/LICENSE
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 fico-0.1.0/README.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 fico-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 fico-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 fico-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 fico-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fico-0.1.1/.vscode/tasks.json
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 fico-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 fico-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fico-0.1.1/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 fico-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fico-0.1.1/docs/source/cli.rst
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 fico-0.1.1/docs/source/figurelib.rst
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fico-0.1.1/docs/source/modules.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fico-0.1.1/src/cli/__init__.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 fico-0.1.1/src/cli/build.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 fico-0.1.1/src/fico/__about__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fico-0.1.1/src/fico/__init__.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 fico-0.1.1/src/fico/building.py
+-rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 fico-0.1.1/src/fico/figure.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 fico-0.1.1/src/fico/styling.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fico-0.1.1/src/fico/utils.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 fico-0.1.1/src/fico/styles/eit6_publication.mplstyle
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 fico-0.1.1/src/fico/templates/basic_table.tex
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fico-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fico-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 fico-0.1.1/README.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 fico-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 fico-0.1.1/PKG-INFO
```

### Comparing `fico-0.1.0/.vscode/tasks.json` & `fico-0.1.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `fico-0.1.0/docs/Makefile` & `fico-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fico-0.1.0/docs/conf.py` & `fico-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fico-0.1.0/docs/make.bat` & `fico-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fico-0.1.0/src/cli/build.py` & `fico-0.1.1/src/cli/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 
 def import_container(container_module_path: str) -> FigureContainer:
     module_name, container_name = container_module_path.split(":")
 
     try:
         module = importlib.import_module(module_name)
     except ModuleNotFoundError:
-        error_msg = f"{red("Error")}: module {underlined(module_name)} not found in current directory."
+        error_msg = f"{red('Error')}: module {underlined(module_name)} not found in current directory."
         cprint(error_msg)
         sys.exit(1)
 
     try:
         container: FigureContainer = getattr(module, container_name)
     except AttributeError:
-        error_msg = f"{red("Error")}: module {underlined(module_name)} does not define an attribute named {underlined(container_name)}."
+        error_msg = f"{red('Error')}: module {underlined(module_name)} does not define an attribute named {underlined(container_name)}."
         cprint(error_msg)
         sys.exit(1)
 
     if not isinstance(container, FigureContainer):
-        error_msg = f"{red("Error")}: the attribute {module_name}.{container_name} is of type {type(container).__name__}, expected FigureContainer."
+        error_msg = f"{red('Error')}: the attribute {module_name}.{container_name} is of type {type(container).__name__}, expected FigureContainer."
         cprint(error_msg)
         sys.exit(1)
 
     return container
 
 
 def build_handler(args):
```

### Comparing `fico-0.1.0/src/fico/building.py` & `fico-0.1.1/src/fico/building.py`

 * *Files identical despite different names*

### Comparing `fico-0.1.0/src/fico/figure.py` & `fico-0.1.1/src/fico/figure.py`

 * *Files identical despite different names*

### Comparing `fico-0.1.0/LICENSE` & `fico-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fico-0.1.0/README.md` & `fico-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fico-0.1.0/pyproject.toml` & `fico-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fico-0.1.0/PKG-INFO` & `fico-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fico
-Version: 0.1.0
+Version: 0.1.1
 Summary: Build tool for creating Matplotlib figures with sensible defaults that look native in LaTeX-documents.
 Author: Markus Ellyton
 License: MIT License
         
         Copyright (c) 2024 MarkusEllyton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


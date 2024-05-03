# Comparing `tmp/expression-builder-0.0.7.tar.gz` & `tmp/expression-builder-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expression-builder-0.0.7.tar", last modified: Fri Mar  8 17:19:16 2024, max compression
+gzip compressed data, was "expression-builder-0.0.8.tar", last modified: Fri May  3 09:44:30 2024, max compression
```

## Comparing `expression-builder-0.0.7.tar` & `expression-builder-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-08 17:19:16.240427 expression-builder-0.0.7/
--rw-r--r--   0 tom        (501) staff       (20)     1077 2024-01-09 12:51:47.000000 expression-builder-0.0.7/LICENCE
--rw-r--r--   0 tom        (501) staff       (20)      643 2024-03-08 17:19:16.240284 expression-builder-0.0.7/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      206 2024-01-09 12:51:47.000000 expression-builder-0.0.7/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-08 17:19:16.239393 expression-builder-0.0.7/expression_builder/
--rw-r--r--   0 tom        (501) staff       (20)        1 2024-01-09 12:51:47.000000 expression-builder-0.0.7/expression_builder/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      402 2024-03-05 12:14:55.000000 expression-builder-0.0.7/expression_builder/exceptions.py
--rw-r--r--   0 tom        (501) staff       (20)    70960 2024-03-08 17:14:00.000000 expression-builder-0.0.7/expression_builder/expression_builder.py
--rw-r--r--   0 tom        (501) staff       (20)      186 2024-01-09 12:51:47.000000 expression-builder-0.0.7/expression_builder/globals.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-03-08 17:19:16.240090 expression-builder-0.0.7/expression_builder.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      643 2024-03-08 17:19:16.000000 expression-builder-0.0.7/expression_builder.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      329 2024-03-08 17:19:16.000000 expression-builder-0.0.7/expression_builder.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2024-03-08 17:19:16.000000 expression-builder-0.0.7/expression_builder.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       19 2024-03-08 17:19:16.000000 expression-builder-0.0.7/expression_builder.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2024-03-08 17:19:16.240478 expression-builder-0.0.7/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      674 2024-03-08 17:14:24.000000 expression-builder-0.0.7/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-05-03 09:44:30.962702 expression-builder-0.0.8/
+-rw-r--r--   0 tom        (501) staff       (20)     1077 2024-01-09 12:51:47.000000 expression-builder-0.0.8/LICENCE
+-rw-r--r--   0 tom        (501) staff       (20)      643 2024-05-03 09:44:30.962590 expression-builder-0.0.8/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      206 2024-01-09 12:51:47.000000 expression-builder-0.0.8/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-05-03 09:44:30.961864 expression-builder-0.0.8/expression_builder/
+-rw-r--r--   0 tom        (501) staff       (20)        1 2024-01-09 12:51:47.000000 expression-builder-0.0.8/expression_builder/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      402 2024-03-05 12:14:55.000000 expression-builder-0.0.8/expression_builder/exceptions.py
+-rw-r--r--   0 tom        (501) staff       (20)    71115 2024-05-03 09:42:29.000000 expression-builder-0.0.8/expression_builder/expression_builder.py
+-rw-r--r--   0 tom        (501) staff       (20)      186 2024-01-09 12:51:47.000000 expression-builder-0.0.8/expression_builder/globals.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-05-03 09:44:30.962393 expression-builder-0.0.8/expression_builder.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      643 2024-05-03 09:44:30.000000 expression-builder-0.0.8/expression_builder.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      329 2024-05-03 09:44:30.000000 expression-builder-0.0.8/expression_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2024-05-03 09:44:30.000000 expression-builder-0.0.8/expression_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       19 2024-05-03 09:44:30.000000 expression-builder-0.0.8/expression_builder.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2024-05-03 09:44:30.962757 expression-builder-0.0.8/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      674 2024-05-03 09:43:04.000000 expression-builder-0.0.8/setup.py
```

### Comparing `expression-builder-0.0.7/LICENCE` & `expression-builder-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `expression-builder-0.0.7/PKG-INFO` & `expression-builder-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expression-builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: Django app that does mathematical expression
 Home-page: https://github.com/django-advance-utils/expression-builder
 Author: Tom Turner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `expression-builder-0.0.7/expression_builder/expression_builder.py` & `expression-builder-0.0.8/expression_builder/expression_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,16 +207,18 @@
                                                                variables=variables,
                                                                statement_variables=statement_variables,
                                                                replace_values=replace_values,
                                                                statement_inheritance_level=self.get_inheritance_level(),
                                                                expression_log=expression_log)
                             arguments.append(arg_statement)
 
-                        function_data = self.convert_functions(function_name, arguments)
-
+                        try:
+                            function_data = self.convert_functions(function_name, arguments)
+                        except ValueError:
+                            raise ExpressionError(f'Value error ({statement})')
                         if function_data['routine']:
                             if function_name == "switch":
                                 function_value, skip_characters = self.process_switch_statement(
                                     switch_value=function_data['value'],
                                     statement=statement,
                                     current_character_index=current_character_index,
                                     variables=variables,
```

### Comparing `expression-builder-0.0.7/expression_builder.egg-info/PKG-INFO` & `expression-builder-0.0.8/expression_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expression-builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: Django app that does mathematical expression
 Home-page: https://github.com/django-advance-utils/expression-builder
 Author: Tom Turner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `expression-builder-0.0.7/setup.py` & `expression-builder-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="expression-builder",
-    version="0.0.7",
+    version="0.0.8",
     author="Tom Turner",
     description="Django app that does mathematical expression",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/expression-builder",
     include_package_data=True,
     packages=['expression_builder'],
```


# Comparing `tmp/milliman_sensi-1.1.0.tar.gz` & `tmp/milliman_sensi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milliman_sensi-1.1.0.tar", last modified: Fri Jan 19 13:46:17 2024, max compression
+gzip compressed data, was "milliman_sensi-1.1.1.tar", last modified: Mon Jan 29 13:14:16 2024, max compression
```

## Comparing `milliman_sensi-1.1.0.tar` & `milliman_sensi-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-19 13:46:17.776838 milliman_sensi-1.1.0/
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-01-19 13:46:14.000000 milliman_sensi-1.1.0/LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      822 2024-01-19 13:46:17.776838 milliman_sensi-1.1.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-01-19 13:46:14.000000 milliman_sensi-1.1.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-19 13:46:17.776838 milliman_sensi-1.1.0/milliman_sensi/
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-01-19 13:46:14.000000 milliman_sensi-1.1.0/milliman_sensi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-19 13:46:14.000000 milliman_sensi-1.1.0/milliman_sensi/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30945 2024-01-19 13:46:14.000000 milliman_sensi-1.1.0/milliman_sensi/io.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25958 2024-01-19 13:46:14.000000 milliman_sensi-1.1.0/milliman_sensi/syntax.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18064 2024-01-19 13:46:14.000000 milliman_sensi-1.1.0/milliman_sensi/table_diff.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12750 2024-01-19 13:46:14.000000 milliman_sensi-1.1.0/milliman_sensi/utility.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-19 13:46:17.776838 milliman_sensi-1.1.0/milliman_sensi.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      822 2024-01-19 13:46:17.000000 milliman_sensi-1.1.0/milliman_sensi.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      384 2024-01-19 13:46:17.000000 milliman_sensi-1.1.0/milliman_sensi.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-19 13:46:17.000000 milliman_sensi-1.1.0/milliman_sensi.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-01-19 13:46:17.000000 milliman_sensi-1.1.0/milliman_sensi.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-01-19 13:46:17.000000 milliman_sensi-1.1.0/milliman_sensi.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-01-19 13:46:17.776838 milliman_sensi-1.1.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1152 2024-01-19 13:46:15.000000 milliman_sensi-1.1.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:14:16.864031 milliman_sensi-1.1.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-01-29 13:14:13.000000 milliman_sensi-1.1.1/LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      822 2024-01-29 13:14:16.864031 milliman_sensi-1.1.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-01-29 13:14:13.000000 milliman_sensi-1.1.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:14:16.864031 milliman_sensi-1.1.1/milliman_sensi/
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-01-29 13:14:13.000000 milliman_sensi-1.1.1/milliman_sensi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-29 13:14:13.000000 milliman_sensi-1.1.1/milliman_sensi/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30945 2024-01-29 13:14:13.000000 milliman_sensi-1.1.1/milliman_sensi/io.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26358 2024-01-29 13:14:13.000000 milliman_sensi-1.1.1/milliman_sensi/syntax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18064 2024-01-29 13:14:13.000000 milliman_sensi-1.1.1/milliman_sensi/table_diff.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12750 2024-01-29 13:14:13.000000 milliman_sensi-1.1.1/milliman_sensi/utility.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:14:16.864031 milliman_sensi-1.1.1/milliman_sensi.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      822 2024-01-29 13:14:16.000000 milliman_sensi-1.1.1/milliman_sensi.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      384 2024-01-29 13:14:16.000000 milliman_sensi-1.1.1/milliman_sensi.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-29 13:14:16.000000 milliman_sensi-1.1.1/milliman_sensi.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-01-29 13:14:16.000000 milliman_sensi-1.1.1/milliman_sensi.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-01-29 13:14:16.000000 milliman_sensi-1.1.1/milliman_sensi.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-01-29 13:14:16.868031 milliman_sensi-1.1.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1152 2024-01-29 13:14:13.000000 milliman_sensi-1.1.1/setup.py
```

### Comparing `milliman_sensi-1.1.0/LICENSE.txt` & `milliman_sensi-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `milliman_sensi-1.1.0/PKG-INFO` & `milliman_sensi-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milliman_sensi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A parser and modifier of the configuration in Milliman-CHESS
 Home-page: https://dev.azure.com/millimanparis/CHESS-Sensitivity-Manager
 Author: Quincy HSIEH
 Author-email: quincy.hsieh@milliman.com
 License: MIT
 Keywords: Milliman CHESS,configuration,parsers,sensitibity
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `milliman_sensi-1.1.0/milliman_sensi/io.py` & `milliman_sensi-1.1.1/milliman_sensi/io.py`

 * *Files identical despite different names*

### Comparing `milliman_sensi-1.1.0/milliman_sensi/syntax.py` & `milliman_sensi-1.1.1/milliman_sensi/syntax.py`

 * *Files 2% similar despite different names*

```diff
@@ -587,16 +587,21 @@
         # convert all columns to string to avoid losing leading zeros
         # (uses converters because dtype=str does not work)
         # then, check if first cell is empty, if so, set index to first column
         input_df = pd.read_csv(input_path, sep=col_sep, header=None, converters={i: str for i in range(100)})
         first_cell = input_df.iloc[0, 0]
         input_df.columns = input_df.iloc[0]
         input_df.drop(0, inplace=True)
+        
         if first_cell == "":
-            input_df.set_index(input_df.columns[0], inplace=True)
+            # set index to first column and delete it
+            input_df.set_index(input_df.columns[0], inplace=True, drop=True)
+        else:
+            # reset index and don't insert it as a column
+            input_df.reset_index(inplace=True, drop=True)
 
         # Select from dataframe using conditions inside .where("...")
         df_selected_with_condition = input_df.copy()
         if syntax.condition:
             logger.debug(f"Selecting from dataframe: {syntax.condition}")
             condition = syntax.condition.strip("()")
             or_conditions = condition.split("||")
@@ -641,19 +646,25 @@
             raise err
 
         for column, indexes in dict_selected_with_col.items():
             for index in indexes:
                 logger.debug(f"Replacing value at [{index},{column}] with {indexes[index]}")
                 input_df.loc[index, column] = indexes[index]
 
-        logger.debug(f"Dataframe types are:\n {input_df.dtypes}")
-        os.remove(input_path)
         if first_cell == "":
             # reset index back to first column
             input_df.reset_index(inplace=True)
-        input_df.to_csv(input_path, sep=col_sep, index=False, float_format="%.18g")
+
+        logger.debug(f"Dataframe types are:\n {input_df.dtypes}")
+
+        input_df.to_csv(input_path + ".tmp", sep=col_sep, index=False, float_format="%.18g")
+        if os.path.exists(input_path):
+            os.remove(input_path)
+        os.rename(input_path + ".tmp", input_path)
         logger.debug(f"Saved to {input_path}:\n" + "\t" + input_df.to_string().replace("\n", "\n\t"))
         return True
 
     except Exception as exc:
         logger.error(f"Failed to apply syntax to file: {input_path}: {exc}")
+        if os.path.exists(input_path + ".tmp"):
+            os.remove(input_path + ".tmp")
         return False
```

### Comparing `milliman_sensi-1.1.0/milliman_sensi/table_diff.py` & `milliman_sensi-1.1.1/milliman_sensi/table_diff.py`

 * *Files identical despite different names*

### Comparing `milliman_sensi-1.1.0/milliman_sensi/utility.py` & `milliman_sensi-1.1.1/milliman_sensi/utility.py`

 * *Files identical despite different names*

### Comparing `milliman_sensi-1.1.0/milliman_sensi.egg-info/PKG-INFO` & `milliman_sensi-1.1.1/milliman_sensi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milliman-sensi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A parser and modifier of the configuration in Milliman-CHESS
 Home-page: https://dev.azure.com/millimanparis/CHESS-Sensitivity-Manager
 Author: Quincy HSIEH
 Author-email: quincy.hsieh@milliman.com
 License: MIT
 Keywords: Milliman CHESS,configuration,parsers,sensitibity
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `milliman_sensi-1.1.0/setup.py` & `milliman_sensi-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.6',
     ]
 
 # calling the setup function
 setup(name='milliman_sensi',
-      version="1.1.0",
+      version="1.1.1",
       description='A parser and modifier of the configuration in Milliman-CHESS',
       long_description="""A parser and modifier of CHESS's configuration
 To parse configuration files and apply them to create new sensitivity tables""",
       url='https://dev.azure.com/millimanparis/CHESS-Sensitivity-Manager',
       author='Quincy HSIEH',
       author_email='quincy.hsieh@milliman.com',
       license='MIT',
```


# Comparing `tmp/odk_tools-0.1.6.tar.gz` & `tmp/odk_tools-0.1.7.tar.gz`

## Comparing `odk_tools-0.1.6.tar` & `odk_tools-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.1.6/src/odk_tools/__init__.py
--rw-r--r--   0        0        0    20111 2020-02-02 00:00:00.000000 odk_tools-0.1.6/src/odk_tools/classes.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 odk_tools-0.1.6/src/odk_tools/functions.py
--rw-r--r--   0        0        0    21151 2020-02-02 00:00:00.000000 odk_tools-0.1.6/src/odk_tools/odk.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 odk_tools-0.1.6/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 odk_tools-0.1.6/LICENSE
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 odk_tools-0.1.6/README.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 odk_tools-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 odk_tools-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.1.7/src/odk_tools/__init__.py
+-rw-r--r--   0        0        0    20111 2020-02-02 00:00:00.000000 odk_tools-0.1.7/src/odk_tools/classes.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 odk_tools-0.1.7/src/odk_tools/functions.py
+-rw-r--r--   0        0        0    21124 2020-02-02 00:00:00.000000 odk_tools-0.1.7/src/odk_tools/odk.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 odk_tools-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 odk_tools-0.1.7/LICENSE
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 odk_tools-0.1.7/README.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 odk_tools-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 odk_tools-0.1.7/PKG-INFO
```

### Comparing `odk_tools-0.1.6/src/odk_tools/classes.py` & `odk_tools-0.1.7/src/odk_tools/classes.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.1.6/src/odk_tools/functions.py` & `odk_tools-0.1.7/src/odk_tools/functions.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.1.6/src/odk_tools/odk.py` & `odk_tools-0.1.7/src/odk_tools/odk.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
                     a.append(j)
             return a
 
 
         def select_one(select, value):
             x = survey["type"].loc[survey["name"] == select].iloc[0].split(" ")[1]
             y = choices["label::English (en)"].loc[choices["list_name"]
-                                                   == x].loc[choices["name"].map(lambda x: str(x)) == str(value)].iloc[0]
+                                                   == x].loc[choices["name"] == value].iloc[0]
             return y
 
 
         def select_multiple(select, value):
             x = survey["type"].loc[survey["name"] == select].iloc[0].split(" ")[1]
             y = choices.loc[choices["list_name"] == x]
             z = []
```

### Comparing `odk_tools-0.1.6/LICENSE` & `odk_tools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `odk_tools-0.1.6/pyproject.toml` & `odk_tools-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "odk_tools"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for interacting with an ODK server and uploading/downloading submissions"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `odk_tools-0.1.6/PKG-INFO` & `odk_tools-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: odk_tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of tools for interacting with an ODK server and uploading/downloading submissions
 Project-URL: Homepage, https://github.com/federlorenz/odk_tools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


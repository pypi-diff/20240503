# Comparing `tmp/odk_tools-0.1.7.tar.gz` & `tmp/odk_tools-0.1.8.tar.gz`

## Comparing `odk_tools-0.1.7.tar` & `odk_tools-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.1.7/src/odk_tools/__init__.py
--rw-r--r--   0        0        0    20111 2020-02-02 00:00:00.000000 odk_tools-0.1.7/src/odk_tools/classes.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 odk_tools-0.1.7/src/odk_tools/functions.py
--rw-r--r--   0        0        0    21124 2020-02-02 00:00:00.000000 odk_tools-0.1.7/src/odk_tools/odk.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 odk_tools-0.1.7/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 odk_tools-0.1.7/LICENSE
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 odk_tools-0.1.7/README.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 odk_tools-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 odk_tools-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.1.8/src/odk_tools/__init__.py
+-rw-r--r--   0        0        0    20111 2020-02-02 00:00:00.000000 odk_tools-0.1.8/src/odk_tools/classes.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 odk_tools-0.1.8/src/odk_tools/functions.py
+-rw-r--r--   0        0        0    21128 2020-02-02 00:00:00.000000 odk_tools-0.1.8/src/odk_tools/odk.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 odk_tools-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 odk_tools-0.1.8/LICENSE
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 odk_tools-0.1.8/README.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 odk_tools-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 odk_tools-0.1.8/PKG-INFO
```

### Comparing `odk_tools-0.1.7/src/odk_tools/classes.py` & `odk_tools-0.1.8/src/odk_tools/classes.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.1.7/src/odk_tools/functions.py` & `odk_tools-0.1.8/src/odk_tools/functions.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.1.7/src/odk_tools/odk.py` & `odk_tools-0.1.8/src/odk_tools/odk.py`

 * *Files 1% similar despite different names*

```diff
@@ -535,15 +535,15 @@
                 tree.find('meta').find('instanceID').text = 'uuid:'+str(uuid.uuid4())
                 root.find('meta').find('deprecatedID').text = old
         xml_out = BytesIO()
         tree.write(xml_out, encoding='utf-8')
         return xml_out.getvalue()
 
     def change_submission(self, variable: str | list[str], id, project=None, form=None, func: FunctionType = lambda x: x | list[FunctionType]):
-        if project != None | form != None:
+        if (project != None) | (form != None):
             self.set_target(project, form)
         if type(variable) == str:
             c = self.get_submission_xml(id)
             ff = self.modify_xml(c, variable, func)
             self.put_submission(id, self.update_xml(ff))
         else:
             c = self.get_submission_xml(id)
```

### Comparing `odk_tools-0.1.7/LICENSE` & `odk_tools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `odk_tools-0.1.7/pyproject.toml` & `odk_tools-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "odk_tools"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for interacting with an ODK server and uploading/downloading submissions"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `odk_tools-0.1.7/PKG-INFO` & `odk_tools-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: odk_tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of tools for interacting with an ODK server and uploading/downloading submissions
 Project-URL: Homepage, https://github.com/federlorenz/odk_tools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


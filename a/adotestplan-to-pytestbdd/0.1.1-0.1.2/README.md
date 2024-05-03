# Comparing `tmp/adotestplan_to_pytestbdd-0.1.1.tar.gz` & `tmp/adotestplan_to_pytestbdd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adotestplan_to_pytestbdd-0.1.1.tar", max compression
+gzip compressed data, was "adotestplan_to_pytestbdd-0.1.2.tar", max compression
```

## Comparing `adotestplan_to_pytestbdd-0.1.1.tar` & `adotestplan_to_pytestbdd-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1079 2024-04-24 14:23:35.016975 adotestplan_to_pytestbdd-0.1.1/LICENSE
--rw-r--r--   0        0        0     4515 2024-04-24 15:20:49.819219 adotestplan_to_pytestbdd-0.1.1/README.md
--rw-r--r--   0        0        0      399 2024-04-24 15:17:53.031059 adotestplan_to_pytestbdd-0.1.1/adotestplan_to_pytestbdd/__init__.py
--rw-r--r--   0        0        0    50506 2024-04-24 15:17:53.031059 adotestplan_to_pytestbdd-0.1.1/adotestplan_to_pytestbdd/ado_test_plan.py
--rw-r--r--   0        0        0     2040 2024-04-24 15:21:19.551244 adotestplan_to_pytestbdd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 adotestplan_to_pytestbdd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-03 14:05:10.785592 adotestplan_to_pytestbdd-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4515 2024-05-03 14:05:10.785592 adotestplan_to_pytestbdd-0.1.2/README.md
+-rw-r--r--   0        0        0      399 2024-05-03 14:05:10.785592 adotestplan_to_pytestbdd-0.1.2/adotestplan_to_pytestbdd/__init__.py
+-rw-r--r--   0        0        0    50743 2024-05-03 14:05:10.785592 adotestplan_to_pytestbdd-0.1.2/adotestplan_to_pytestbdd/ado_test_plan.py
+-rw-r--r--   0        0        0     2040 2024-05-03 14:05:10.785592 adotestplan_to_pytestbdd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 adotestplan_to_pytestbdd-0.1.2/PKG-INFO
```

### Comparing `adotestplan_to_pytestbdd-0.1.1/LICENSE` & `adotestplan_to_pytestbdd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adotestplan_to_pytestbdd-0.1.1/README.md` & `adotestplan_to_pytestbdd-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `adotestplan_to_pytestbdd-0.1.1/adotestplan_to_pytestbdd/ado_test_plan.py` & `adotestplan_to_pytestbdd-0.1.2/adotestplan_to_pytestbdd/ado_test_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -849,15 +849,18 @@
             # but lets handle it elsewhere.
             pass
 
     def _has_params(self, work_item: WorkItem):
         if 'Microsoft.VSTS.TCM.Parameters' in work_item.fields and \
                 len(work_item.fields['Microsoft.VSTS.TCM.Parameters']):
             parameter_table = work_item.fields['Microsoft.VSTS.TCM.Parameters']
-            table = ET.fromstring(parameter_table)
+            try:
+                table = ET.fromstring(parameter_table)
+            except ET.ParseError:
+                table = parameter_table
             if len(table):
                 return True
         if 'Microsoft.VSTS.TCM.LocalDataSource' in work_item.fields and \
                 len(work_item.fields['Microsoft.VSTS.TCM.LocalDataSource']):
             try:
                 params_fields = json.loads(
                     work_item.fields['Microsoft.VSTS.TCM.LocalDataSource'])
@@ -874,15 +877,19 @@
             # a shared param, likely. process elsewhere
             return
         try:
             parameter_data_source = work_item.fields['Microsoft.VSTS.TCM.LocalDataSource']
         except KeyError:
             raise ValueError(
                 f"Non-Shared parameter on {work_item.id} has no values")
-        params = ET.fromstring(nonshared_parameter_table).findall('param')
+        try:
+            params = ET.fromstring(nonshared_parameter_table).findall('param')
+        except ET.ParseError:
+            # its just a string ID, shared param likely. process elsewhere.
+            return
         try:
             tables = ET.fromstring(parameter_data_source).findall('Table1')
         except ET.ParseError:
             # a shared param, likely. process elsewhere
             return
         if not len(tables):
             raise ValueError(
```

### Comparing `adotestplan_to_pytestbdd-0.1.1/pyproject.toml` & `adotestplan_to_pytestbdd-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adotestplan-to-pytestbdd"
-version = "0.1.1"
+version = "0.1.2"
 description = "Utility for translating AzureDevOps Test Plans to Gherkin Feature file and Pytest-BDD runners"
 authors = [
     "David VanKampen <david.vankampen@bissell.com>",
     "Tristan VanFossen <tristan.vanfossen@bissell.com>"
 ]
 readme = "README.md"
 repository = 'https://github.com/bissell-homecare-inc/adotestplan-to-pytestbdd'
```

### Comparing `adotestplan_to_pytestbdd-0.1.1/PKG-INFO` & `adotestplan_to_pytestbdd-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adotestplan-to-pytestbdd
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utility for translating AzureDevOps Test Plans to Gherkin Feature file and Pytest-BDD runners
 Home-page: https://github.com/bissell-homecare-inc/adotestplan-to-pytestbdd
 Keywords: ADO,AzureDevOps,BDD
 Author: David VanKampen
 Author-email: david.vankampen@bissell.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```


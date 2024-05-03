# Comparing `tmp/salure_helpers_profit-3.3.3.tar.gz` & `tmp/salure_helpers_profit-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_profit-3.3.3.tar", last modified: Tue Apr  2 19:07:10 2024, max compression
+gzip compressed data, was "dist/salure_helpers_profit-3.3.4.tar", last modified: Fri May  3 16:53:08 2024, max compression
```

## Comparing `salure_helpers_profit-3.3.3.tar` & `salure_helpers_profit-3.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      262 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/profit_data_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    14742 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/profit_get.py
--rw-rw-rw-   0 root         (0) root         (0)    17456 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/profit_get_async.py
--rw-rw-rw-   0 root         (0) root         (0)   164848 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/salure_helpers/profit/profit_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      128 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/salure_helpers_profit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 19:07:10.000000 salure_helpers_profit-3.3.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-04-02 19:06:54.000000 salure_helpers_profit-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/salure_helpers/profit/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-05-03 16:52:47.000000 salure_helpers_profit-3.3.4/salure_helpers/profit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2024-05-03 16:52:47.000000 salure_helpers_profit-3.3.4/salure_helpers/profit/profit_data_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14742 2024-05-03 16:52:47.000000 salure_helpers_profit-3.3.4/salure_helpers/profit/profit_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    17456 2024-05-03 16:52:47.000000 salure_helpers_profit-3.3.4/salure_helpers/profit/profit_get_async.py
+-rw-rw-rw-   0 root         (0) root         (0)   164865 2024-05-03 16:52:47.000000 salure_helpers_profit-3.3.4/salure_helpers/profit/profit_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/salure_helpers_profit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/salure_helpers_profit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/salure_helpers_profit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/salure_helpers_profit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/salure_helpers_profit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      128 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/salure_helpers_profit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/salure_helpers_profit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 16:53:08.000000 salure_helpers_profit-3.3.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-05-03 16:52:47.000000 salure_helpers_profit-3.3.4/setup.py
```

### Comparing `salure_helpers_profit-3.3.3/salure_helpers/profit/profit_data_cleaner.py` & `salure_helpers_profit-3.3.4/salure_helpers/profit/profit_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-3.3.3/salure_helpers/profit/profit_get.py` & `salure_helpers_profit-3.3.4/salure_helpers/profit/profit_get.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-3.3.3/salure_helpers/profit/profit_get_async.py` & `salure_helpers_profit-3.3.4/salure_helpers/profit/profit_get_async.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-3.3.3/salure_helpers/profit/profit_update.py` & `salure_helpers_profit-3.3.4/salure_helpers/profit/profit_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1438,34 +1438,34 @@
         required_fields = ['employee_id', 'year', 'month', 'employer_id', 'wage_component_id', 'value', 'guid']
 
         self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
 
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, 'HrCompMutGUID')
 
         base_body = {
-            "HrCompMut": {
+            "HrCompMutGUID": {
                 "Element": {
                     "@GuLi": data['guid'],
-                    "@Year": data['year'],
-                    "@PeId": data['month'],
-                    "@EmId": data['employee_id'],
-                    "@ErId": data['employer_id'],
-                    "@Sc02": data['wage_component_id'],
                     "Fields": {
-                        "VaD1": data['value']
+                        "VaD1": data['value'],
+                        "Year": data['year'],
+                        "PeId": data['month'],
+                        "EmId": data['employee_id'],
+                        "ErId": data['employer_id'],
+                        "Sc02": data['wage_component_id'],
                     }
                 }
             }
         }
         fields_to_update = {}
         selector_to_update = {}
 
         # Add fields that you want to update a dict (adding to body itself is too much text)
-        selector_to_update.update({"@PtId": data['period_table']}) if 'period_table' in data else selector_to_update.update({"@PtId": 5})
-        selector_to_update.update({"@DaTi": data['date']}) if 'date' in data else ""
+        selector_to_update.update({"PtId": data['period_table']}) if 'period_table' in data else selector_to_update.update({"PtId": 5})
+        selector_to_update.update({"DaTi": data['date']}) if 'date' in data else ""
 
         fields_to_update.update(overload_fields) if overload_fields is not None else ''
 
         # Update the request body with update fields
         base_body['HrCompMut']['Element']['Fields'].update(fields_to_update)
         base_body['HrCompMut']['Element'].update(selector_to_update)
```

### Comparing `salure_helpers_profit-3.3.3/setup.py` & `salure_helpers_profit-3.3.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_profit',
-    version='3.3.3',
+    version='3.3.4',
     description='Profit wrapper from Salure',
     long_description='Profit wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.profit"],
     license='Salure License',
     install_requires=[
```


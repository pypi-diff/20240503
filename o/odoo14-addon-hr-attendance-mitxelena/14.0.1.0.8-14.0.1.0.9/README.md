# Comparing `tmp/odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8.tar.gz` & `tmp/odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8.tar", last modified: Fri Sep  1 17:17:38 2023, max compression
+gzip compressed data, was "odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9.tar", last modified: Fri Sep  1 17:37:40 2023, max compression
```

## Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8.tar` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:17:38.470070 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/
--rw-r--r--   0 root         (0) root         (0)      644 2023-09-01 17:17:38.470070 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:17:38.466070 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:17:38.466070 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:17:38.466070 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-09-01 15:55:34.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      871 2023-09-01 17:17:36.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:17:38.466070 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/models/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-09-01 15:55:34.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11710 2023-09-01 17:17:36.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/models/hr_attendance_mitxelena.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:17:38.466070 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/security/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-09-01 15:55:34.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/security/ir.model.access.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:17:38.466070 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/views/
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-09-01 16:00:26.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/views/hr_attendance_views.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:17:38.470070 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo14_addon_hr_attendance_mitxelena.egg-info/
--rw-r--r--   0 root         (0) root         (0)      644 2023-09-01 17:17:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo14_addon_hr_attendance_mitxelena.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      722 2023-09-01 17:17:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo14_addon_hr_attendance_mitxelena.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-01 17:17:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo14_addon_hr_attendance_mitxelena.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-01 17:17:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo14_addon_hr_attendance_mitxelena.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       53 2023-09-01 17:17:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo14_addon_hr_attendance_mitxelena.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-09-01 17:17:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo14_addon_hr_attendance_mitxelena.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-01 17:17:38.470070 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-09-01 17:17:36.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:37:40.124227 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      644 2023-09-01 17:37:40.124227 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:37:40.120227 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:37:40.120227 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:37:40.120227 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-09-01 15:55:34.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      871 2023-09-01 17:37:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:37:40.120227 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/models/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-09-01 15:55:34.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11827 2023-09-01 17:37:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/models/hr_attendance_mitxelena.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:37:40.120227 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/security/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-09-01 15:55:34.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:37:40.120227 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/views/
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-09-01 16:00:26.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/views/hr_attendance_views.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 17:37:40.124227 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo14_addon_hr_attendance_mitxelena.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      644 2023-09-01 17:37:39.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo14_addon_hr_attendance_mitxelena.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      722 2023-09-01 17:37:39.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo14_addon_hr_attendance_mitxelena.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-01 17:37:39.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo14_addon_hr_attendance_mitxelena.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-01 17:37:39.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo14_addon_hr_attendance_mitxelena.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       53 2023-09-01 17:37:39.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo14_addon_hr_attendance_mitxelena.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-09-01 17:37:39.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo14_addon_hr_attendance_mitxelena.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-01 17:37:40.124227 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-09-01 17:37:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/setup.py
```

### Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/PKG-INFO` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-hr_attendance_mitxelena
-Version: 14.0.1.0.8
+Version: 14.0.1.0.9
 Summary: Employee Attendances Customizations for Mitxelena
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

### Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/__manifest__.py` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/__manifest__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'HR Attendance Mitxelena',
-    'version': '14.0.1.0.8',
+    'version': '14.0.1.0.9',
     'category': 'Human Resources',
     'sequence': 20,
     'summary': 'Employee Attendances Customizations for Mitxelena',
     'description': """
 Customizations of Employee Attendances for Mitxelena
 ====================================================
 This module includes customizations for handling employee attendances at Mitxelena,
```

### Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/models/hr_attendance_mitxelena.py` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/models/hr_attendance_mitxelena.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,18 @@
         if self.is_holiday:
             return False
         # if check_in is in Sunday but shift_type is night, is not weekend
         if check_in.weekday() == 6 and self.shift_type == 'night':
             return False
         # if check_in is between Monday and Friday, is not weekend
         if check_in.weekday() < 5:
-            return False        
+            return False
+        # if consecutive_days is bigger than 5, is weekend
+        if check_in.consecutive_days > 5:
+            return True
         return True
 
     @api.depends('check_in', 'consecutive_days')
     def _compute_is_relevo(self):
         for record in self:           
             tz = timezone(record.env.user.tz or 'Europe/Madrid')
             check_in = record.check_in.replace(
```

### Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo/addons/hr_attendance_mitxelena/views/hr_attendance_views.xml` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo/addons/hr_attendance_mitxelena/views/hr_attendance_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo14_addon_hr_attendance_mitxelena.egg-info/PKG-INFO` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo14_addon_hr_attendance_mitxelena.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-hr-attendance-mitxelena
-Version: 14.0.1.0.8
+Version: 14.0.1.0.9
 Summary: Employee Attendances Customizations for Mitxelena
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

### Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.8/odoo14_addon_hr_attendance_mitxelena.egg-info/SOURCES.txt` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.9/odoo14_addon_hr_attendance_mitxelena.egg-info/SOURCES.txt`

 * *Files identical despite different names*


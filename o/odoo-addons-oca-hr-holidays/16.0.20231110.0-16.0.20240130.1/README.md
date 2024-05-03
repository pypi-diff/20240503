# Comparing `tmp/odoo_addons_oca_hr_holidays-16.0.20231110.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_hr_holidays-16.0.20240130.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1390 bytes, number of entries: 4
--rw-r--r--  2.0 unx      515 b- defN 23-Nov-11 04:00 odoo_addons_oca_hr_holidays-16.0.20231110.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Nov-11 04:00 odoo_addons_oca_hr_holidays-16.0.20231110.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Nov-11 04:00 odoo_addons_oca_hr_holidays-16.0.20231110.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      416 b- defN 23-Nov-11 04:00 odoo_addons_oca_hr_holidays-16.0.20231110.0.dist-info/RECORD
-4 files, 1024 bytes uncompressed, 568 bytes compressed:  44.5%
+Zip file size: 1414 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      655 b- defN 24-Jan-31 04:21 odoo_addons_oca_hr_holidays-16.0.20240130.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jan-31 04:21 odoo_addons_oca_hr_holidays-16.0.20240130.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Jan-31 04:21 odoo_addons_oca_hr_holidays-16.0.20240130.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      416 b- defN 24-Jan-31 04:21 odoo_addons_oca_hr_holidays-16.0.20240130.1.dist-info/RECORD
+4 files, 1164 bytes uncompressed, 592 bytes compressed:  49.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_hr_holidays-16.0.20231110.0.dist-info/METADATA
+Filename: odoo_addons_oca_hr_holidays-16.0.20240130.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_hr_holidays-16.0.20231110.0.dist-info/WHEEL
+Filename: odoo_addons_oca_hr_holidays-16.0.20240130.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_hr_holidays-16.0.20231110.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_hr_holidays-16.0.20240130.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_hr_holidays-16.0.20231110.0.dist-info/RECORD
+Filename: odoo_addons_oca_hr_holidays-16.0.20240130.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_hr_holidays-16.0.20231110.0.dist-info/METADATA` & `odoo_addons_oca_hr_holidays-16.0.20240130.1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-hr-holidays
-Version: 16.0.20231110.0
+Version: 16.0.20240130.1
 Summary: Meta package for oca-hr-holidays Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
+Requires-Dist: odoo-addon-hr-holidays-leave-auto-approve <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-holidays-natural-period <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-holidays-public <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-holidays-public-city <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-hr-leave-type-code <16.1dev,>=16.0dev
 
 UNKNOWN
```


# Comparing `tmp/odoo_addons_oca_wms-16.0.20240415.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_wms-16.0.20240502.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1604 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2805 b- defN 24-Apr-16 08:26 odoo_addons_oca_wms-16.0.20240415.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 08:26 odoo_addons_oca_wms-16.0.20240415.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-16 08:26 odoo_addons_oca_wms-16.0.20240415.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 24-Apr-16 08:26 odoo_addons_oca_wms-16.0.20240415.0.dist-info/RECORD
-4 files, 3283 bytes uncompressed, 846 bytes compressed:  74.2%
+Zip file size: 1625 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3001 b- defN 24-May-03 06:33 odoo_addons_oca_wms-16.0.20240502.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 06:33 odoo_addons_oca_wms-16.0.20240502.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-03 06:33 odoo_addons_oca_wms-16.0.20240502.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 24-May-03 06:33 odoo_addons_oca_wms-16.0.20240502.2.dist-info/RECORD
+4 files, 3479 bytes uncompressed, 867 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_wms-16.0.20240415.0.dist-info/METADATA
+Filename: odoo_addons_oca_wms-16.0.20240502.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240415.0.dist-info/WHEEL
+Filename: odoo_addons_oca_wms-16.0.20240502.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240415.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_wms-16.0.20240502.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240415.0.dist-info/RECORD
+Filename: odoo_addons_oca_wms-16.0.20240502.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_wms-16.0.20240415.0.dist-info/METADATA` & `odoo_addons_oca_wms-16.0.20240502.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-wms
-Version: 16.0.20240415.0
+Version: 16.0.20240502.2
 Summary: Meta package for oca-wms Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-delivery-carrier-warehouse <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-stock-available-to-promise-release <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-stock-available-to-promise-release-block <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-shopfloor <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-shopfloor-base <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-shopfloor-mobile-base <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-available-to-promise-release <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-available-to-promise-release-block <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-available-to-promise-release-exclude-location <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-dynamic-routing <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-stock-picking-batch-creation <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-completion-info <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-type-shipping-policy <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-auto-release <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-batch-mode-commercial-partner <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-cutoff <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-delivery <16.1dev,>=16.0dev
```


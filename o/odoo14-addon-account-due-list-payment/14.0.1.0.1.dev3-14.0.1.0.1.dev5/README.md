# Comparing `tmp/odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3-py3-none-any.whl.zip` & `tmp/odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 16289 bytes, number of entries: 14
--rw-r--r--  2.0 unx       21 b- defN 24-Jan-20 02:57 odoo/addons/account_due_list_payment/__init__.py
--rw-r--r--  2.0 unx      533 b- defN 24-Jan-20 02:57 odoo/addons/account_due_list_payment/__manifest__.py
--rw-r--r--  2.0 unx     1351 b- defN 24-Jan-20 02:57 odoo/addons/account_due_list_payment/i18n/account_due_list_payment.pot
--rw-r--r--  2.0 unx     1601 b- defN 24-Jan-20 02:57 odoo/addons/account_due_list_payment/i18n/es.po
--rw-r--r--  2.0 unx       32 b- defN 24-Jan-20 02:57 odoo/addons/account_due_list_payment/models/__init__.py
--rw-r--r--  2.0 unx      774 b- defN 24-Jan-20 02:57 odoo/addons/account_due_list_payment/models/account_move_line.py
--rw-r--r--  2.0 unx     9455 b- defN 24-Jan-20 02:57 odoo/addons/account_due_list_payment/static/description/icon.png
--rw-r--r--  2.0 unx       43 b- defN 24-Jan-20 02:57 odoo/addons/account_due_list_payment/tests/__init__.py
--rw-r--r--  2.0 unx      906 b- defN 24-Jan-20 02:57 odoo/addons/account_due_list_payment/tests/test_action_register_payment.py
--rw-r--r--  2.0 unx     2118 b- defN 24-Jan-20 02:57 odoo/addons/account_due_list_payment/views/account_move_line.xml
--rw-r--r--  2.0 unx      641 b- defN 24-Jan-20 02:58 odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-20 02:58 odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Jan-20 02:58 odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1609 b- defN 24-Jan-20 02:58 odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/RECORD
-14 files, 19181 bytes uncompressed, 13443 bytes compressed:  29.9%
+Zip file size: 17108 bytes, number of entries: 15
+-rw-r--r--  2.0 unx       21 b- defN 24-Feb-24 02:58 odoo/addons/account_due_list_payment/__init__.py
+-rw-r--r--  2.0 unx      533 b- defN 24-Feb-24 02:58 odoo/addons/account_due_list_payment/__manifest__.py
+-rw-r--r--  2.0 unx     1351 b- defN 24-Feb-24 02:58 odoo/addons/account_due_list_payment/i18n/account_due_list_payment.pot
+-rw-r--r--  2.0 unx     1601 b- defN 24-Feb-24 02:58 odoo/addons/account_due_list_payment/i18n/es.po
+-rw-r--r--  2.0 unx     1582 b- defN 24-Feb-24 02:58 odoo/addons/account_due_list_payment/i18n/it.po
+-rw-r--r--  2.0 unx       32 b- defN 24-Feb-24 02:58 odoo/addons/account_due_list_payment/models/__init__.py
+-rw-r--r--  2.0 unx      774 b- defN 24-Feb-24 02:58 odoo/addons/account_due_list_payment/models/account_move_line.py
+-rw-r--r--  2.0 unx     9455 b- defN 24-Feb-24 02:58 odoo/addons/account_due_list_payment/static/description/icon.png
+-rw-r--r--  2.0 unx       43 b- defN 24-Feb-24 02:58 odoo/addons/account_due_list_payment/tests/__init__.py
+-rw-r--r--  2.0 unx      906 b- defN 24-Feb-24 02:58 odoo/addons/account_due_list_payment/tests/test_action_register_payment.py
+-rw-r--r--  2.0 unx     2118 b- defN 24-Feb-24 02:58 odoo/addons/account_due_list_payment/views/account_move_line.xml
+-rw-r--r--  2.0 unx      641 b- defN 24-Feb-24 02:59 odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Feb-24 02:59 odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Feb-24 02:59 odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1713 b- defN 24-Feb-24 02:59 odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/RECORD
+15 files, 20867 bytes uncompressed, 14092 bytes compressed:  32.5%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: odoo/addons/account_due_list_payment/i18n/account_due_list_payment.pot
 Comment: 
 
 Filename: odoo/addons/account_due_list_payment/i18n/es.po
 Comment: 
 
+Filename: odoo/addons/account_due_list_payment/i18n/it.po
+Comment: 
+
 Filename: odoo/addons/account_due_list_payment/models/__init__.py
 Comment: 
 
 Filename: odoo/addons/account_due_list_payment/models/account_move_line.py
 Comment: 
 
 Filename: odoo/addons/account_due_list_payment/static/description/icon.png
@@ -24,20 +27,20 @@
 
 Filename: odoo/addons/account_due_list_payment/tests/test_action_register_payment.py
 Comment: 
 
 Filename: odoo/addons/account_due_list_payment/views/account_move_line.xml
 Comment: 
 
-Filename: odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/METADATA
+Filename: odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/WHEEL
+Filename: odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/top_level.txt
+Filename: odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/RECORD
+Filename: odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/METADATA` & `odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-account-due-list-payment
-Version: 14.0.1.0.1.dev3
+Version: 14.0.1.0.1.dev5
 Summary: Allows you to make payments directly from the due list view
 Home-page: https://github.com/OCA/account-payment
 Author: Engenere.one,Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/RECORD` & `odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 odoo/addons/account_due_list_payment/__init__.py,sha256=X9EJGOE2GtZbS0G82PtSXmWSZ_R8jEM0rlJTDliQjp4,21
 odoo/addons/account_due_list_payment/__manifest__.py,sha256=a73Tacr6dxJkt_DGS95I4NiuURrYt_aCEtLhdDRSrnk,533
 odoo/addons/account_due_list_payment/i18n/account_due_list_payment.pot,sha256=KyzLg5eNRUQrVrtRhtsay0QXCuyibsEyrqM31JVQUDU,1351
 odoo/addons/account_due_list_payment/i18n/es.po,sha256=rX4dUKXx5IFKy8slrO8X3CInRpgmV2zAVrTkUT3ICCs,1601
+odoo/addons/account_due_list_payment/i18n/it.po,sha256=m8FQkNSdUxJMn_p8RuPrg2X7W_42OEkh-VXlgyyWDfQ,1582
 odoo/addons/account_due_list_payment/models/__init__.py,sha256=mF9GDUr6-OiEO9ML3T5FLEFtNN01jg2OpdHPAqiCdKA,32
 odoo/addons/account_due_list_payment/models/account_move_line.py,sha256=2i6ov6_k6I01-oEuuqDqZAwm8GKePgPplFQmIzbWpWA,774
 odoo/addons/account_due_list_payment/static/description/icon.png,sha256=6xBPJauaFOF0KDHfHgQopSc28kKvxMaeoQFQWZtfZDo,9455
 odoo/addons/account_due_list_payment/tests/__init__.py,sha256=8H9RQIcFclbHrOlS6r1r0EQm272Yz2Ea2Ckzl5oezPw,43
 odoo/addons/account_due_list_payment/tests/test_action_register_payment.py,sha256=9W26LF1x3jpQdv9H21SphYAtTdpmHfEht2cGRTXfQdw,906
 odoo/addons/account_due_list_payment/views/account_move_line.xml,sha256=gsTMimZptZ5KMAzL_SlFnXNMJBaClcIwROL3ml1ELeM,2118
-odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/METADATA,sha256=keEmC749eJcPhYBPBfK0wStj4Grc2CkCAOvfTwgkBdw,641
-odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_account_due_list_payment-14.0.1.0.1.dev3.dist-info/RECORD,,
+odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/METADATA,sha256=ZRgzgVWE3S8bkh21Fx8WYajELK1uTa8zENv1vh53T2Y,641
+odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_account_due_list_payment-14.0.1.0.1.dev5.dist-info/RECORD,,
```


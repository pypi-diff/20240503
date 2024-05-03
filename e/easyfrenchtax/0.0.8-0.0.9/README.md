# Comparing `tmp/easyfrenchtax-0.0.8.tar.gz` & `tmp/easyfrenchtax-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfrenchtax-0.0.8.tar", last modified: Thu Jul 20 16:54:07 2023, max compression
+gzip compressed data, was "easyfrenchtax-0.0.9.tar", last modified: Fri May  3 18:10:49 2024, max compression
```

## Comparing `easyfrenchtax-0.0.8.tar` & `easyfrenchtax-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-20 16:54:07.354313 easyfrenchtax-0.0.8/
--rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.8/LICENSE
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-20 16:54:07.354391 easyfrenchtax-0.0.8/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.8/README.md
--rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.8/pyproject.toml
--rw-r--r--   0 hadrien    (501) staff       (20)      853 2023-07-20 16:54:07.354672 easyfrenchtax-0.0.8/setup.cfg
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-20 16:54:07.350046 easyfrenchtax-0.0.8/src/
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-20 16:54:07.351788 easyfrenchtax-0.0.8/src/easyfrenchtax/
--rw-r--r--   0 hadrien    (501) staff       (20)      114 2023-07-16 12:40:46.000000 easyfrenchtax-0.0.8/src/easyfrenchtax/__init__.py
--rw-r--r--   0 hadrien    (501) staff       (20)    22810 2023-07-20 14:14:29.000000 easyfrenchtax-0.0.8/src/easyfrenchtax/stock_helper.py
--rw-r--r--   0 hadrien    (501) staff       (20)    27735 2023-06-02 20:57:34.000000 easyfrenchtax-0.0.8/src/easyfrenchtax/tax_simulator.py
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-20 16:54:07.352835 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-20 16:54:07.000000 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)      480 2023-07-20 16:54:07.000000 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/SOURCES.txt
--rw-r--r--   0 hadrien    (501) staff       (20)        1 2023-07-20 16:54:07.000000 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/dependency_links.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       18 2023-07-20 16:54:07.000000 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/requires.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       14 2023-07-20 16:54:07.000000 easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/top_level.txt
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-20 16:54:07.354077 easyfrenchtax-0.0.8/tests/
--rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.8/tests/test_capital_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.8/tests/test_fiscal_advantages.py
--rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.8/tests/test_income_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.8/tests/test_rental_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    14179 2023-07-20 16:51:06.000000 easyfrenchtax-0.0.8/tests/test_stock_helper.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-03 18:10:49.782119 easyfrenchtax-0.0.9/
+-rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.9/LICENSE
+-rw-r--r--   0 hadrien    (501) staff       (20)     2587 2024-05-03 18:10:49.782036 easyfrenchtax-0.0.9/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)     1821 2024-05-03 18:10:18.000000 easyfrenchtax-0.0.9/README.md
+-rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.9/pyproject.toml
+-rw-r--r--   0 hadrien    (501) staff       (20)      853 2024-05-03 18:10:49.782460 easyfrenchtax-0.0.9/setup.cfg
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-03 18:10:49.774028 easyfrenchtax-0.0.9/src/
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-03 18:10:49.777001 easyfrenchtax-0.0.9/src/easyfrenchtax/
+-rw-r--r--   0 hadrien    (501) staff       (20)      125 2023-08-11 21:09:23.000000 easyfrenchtax-0.0.9/src/easyfrenchtax/__init__.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    22815 2023-08-11 21:09:23.000000 easyfrenchtax-0.0.9/src/easyfrenchtax/stock_helper.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    27996 2024-05-03 13:20:43.000000 easyfrenchtax-0.0.9/src/easyfrenchtax/tax_simulator.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-03 18:10:49.781718 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/
+-rw-r--r--   0 hadrien    (501) staff       (20)     2587 2024-05-03 18:10:49.000000 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)      480 2024-05-03 18:10:49.000000 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/SOURCES.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)        1 2024-05-03 18:10:49.000000 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/dependency_links.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       18 2024-05-03 18:10:49.000000 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/requires.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       14 2024-05-03 18:10:49.000000 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/top_level.txt
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-03 18:10:49.781170 easyfrenchtax-0.0.9/tests/
+-rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.9/tests/test_capital_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.9/tests/test_fiscal_advantages.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.9/tests/test_income_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.9/tests/test_rental_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    14179 2023-07-20 16:51:06.000000 easyfrenchtax-0.0.9/tests/test_stock_helper.py
```

### Comparing `easyfrenchtax-0.0.8/LICENSE` & `easyfrenchtax-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.8/PKG-INFO` & `easyfrenchtax-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
@@ -13,17 +13,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: currencyconverter
 
 # easyfrenchtax
-This project helps me understanding and projecting French taxes, especially wrt. stock, stock options, RSUs and other systems. It doesn't replace a tax advisor, I am not a lawyer, you should not rely blindly on this software for filling your tax return.
+This project helps me to understand and project French taxes, especially wrt. stock, stock options, RSUs and other systems. It doesn't replace a tax advisor, I am not a lawyer, you should not rely blindly on this software for filling your tax return.
 
 # Tax simulator
 The following are supported:
 - Progressive income tax
 - Rental income (unfurnished)
 - Family quotient (incl. capping, but excl. shared custody situations)
 - Some deductions/reductions (PER, child care, home services, charity donations)
@@ -32,15 +33,15 @@
 - Fixed interest income, incl. when tax has been partially withheld by a bank
 - Social taxes
 
 These elements of taxation have been tested against the tax simulator of the French government. I invite you to read and understand these tests, this will give you a feeling of whether you want to trust this project or not.
 
 # Stock helper
 
-This module helps filling the tax statement regarding stock acquisition or capital gain. It takes as input the stocks received (RSU, Stock Options) or bought (ESPP, direct buying) and what has been exercised/sold; it outputs the fields to fill a form 2074 and parts of 2042C. More precisely, it supports the following:
+This module helps to fill the tax statement regarding stock acquisition or capital gain. It takes as input the stocks received (RSU, Stock Options) or bought (ESPP, direct buying) and what has been exercised/sold; it outputs the fields to fill a form 2074 and parts of 2042C. More precisely, it supports the following:
 - Typical retention plans like RSU or Stock Options, direct stocks
 - Currency conversion at acquisition/exercise/buying/selling dates
 - Weighted average price ("Prix moyen pondéré" or PMP in French tax lingo)
 - Outputs fields 3VG/3VH for form 2042C, and frame 5 (512-524) + fields 903/913 for form 2074
 
 # Contact and contributions
 If you want to chat about this project, don't hesitate to shoot an email at hadrien.hamel@gmail.com. Contributions and bug reports are welcome!
```

### Comparing `easyfrenchtax-0.0.8/README.md` & `easyfrenchtax-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # easyfrenchtax
-This project helps me understanding and projecting French taxes, especially wrt. stock, stock options, RSUs and other systems. It doesn't replace a tax advisor, I am not a lawyer, you should not rely blindly on this software for filling your tax return.
+This project helps me to understand and project French taxes, especially wrt. stock, stock options, RSUs and other systems. It doesn't replace a tax advisor, I am not a lawyer, you should not rely blindly on this software for filling your tax return.
 
 # Tax simulator
 The following are supported:
 - Progressive income tax
 - Rental income (unfurnished)
 - Family quotient (incl. capping, but excl. shared custody situations)
 - Some deductions/reductions (PER, child care, home services, charity donations)
@@ -12,15 +12,15 @@
 - Fixed interest income, incl. when tax has been partially withheld by a bank
 - Social taxes
 
 These elements of taxation have been tested against the tax simulator of the French government. I invite you to read and understand these tests, this will give you a feeling of whether you want to trust this project or not.
 
 # Stock helper
 
-This module helps filling the tax statement regarding stock acquisition or capital gain. It takes as input the stocks received (RSU, Stock Options) or bought (ESPP, direct buying) and what has been exercised/sold; it outputs the fields to fill a form 2074 and parts of 2042C. More precisely, it supports the following:
+This module helps to fill the tax statement regarding stock acquisition or capital gain. It takes as input the stocks received (RSU, Stock Options) or bought (ESPP, direct buying) and what has been exercised/sold; it outputs the fields to fill a form 2074 and parts of 2042C. More precisely, it supports the following:
 - Typical retention plans like RSU or Stock Options, direct stocks
 - Currency conversion at acquisition/exercise/buying/selling dates
 - Weighted average price ("Prix moyen pondéré" or PMP in French tax lingo)
 - Outputs fields 3VG/3VH for form 2042C, and frame 5 (512-524) + fields 903/913 for form 2074
 
 # Contact and contributions
 If you want to chat about this project, don't hesitate to shoot an email at hadrien.hamel@gmail.com. Contributions and bug reports are welcome!
```

### Comparing `easyfrenchtax-0.0.8/setup.cfg` & `easyfrenchtax-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easyfrenchtax
-version = 0.0.8
+version = 0.0.9
 author = Hadrien Hamel
 author_email = hadrien.hamel@gmail.com
 license = MIT
 description = A simulator of French taxes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/had/easyfrenchtax
```

### Comparing `easyfrenchtax-0.0.8/src/easyfrenchtax/stock_helper.py` & `easyfrenchtax-0.0.9/src/easyfrenchtax/stock_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dateutil.relativedelta import relativedelta
 from currency_converter import CurrencyConverter
 from collections import defaultdict
 import csv
 import glob
 
-class RsuTaxScheme(Enum):
+class RsuTaxScheme(str, Enum):
     NONQUALIFIED_RSU = "Non-qualified RSU"
     QUALIFIED_RSU = "Qualified RSU"
     MACRON_1_RSU = "Macron I"
     MACRON_2_RSU = "Macron II"
     MACRON_3_RSU = "Macron III"
 
 class StockType(Enum):
```

### Comparing `easyfrenchtax-0.0.8/src/easyfrenchtax/tax_simulator.py` & `easyfrenchtax-0.0.9/src/easyfrenchtax/tax_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     NET_TAXES = "net_taxes"
     NET_SOCIAL_TAXES = "net_social_taxes"
 
 
 # Lots of parameters evolve year after year (inflation, political decisions, etc.)
 # This dictionary gathers all variable parameters.
 TaxParameters = namedtuple("TaxParameters", [
-    # Source: https://www.economie.gouv.fr/particuliers/quotient-familial
+    # Source: https://www.service-public.fr/particuliers/vosdroits/F2705
     "family_quotient_benefices_capping",
     # https://www.service-public.fr/particuliers/vosdroits/F1419
     "slices_thresholds", "slices_rates",
     # https://www.impots.gouv.fr/particulier/questions/comment-puis-je-beneficier-de-la-deduction-forfaitaire-de-10
     "fees_10p_deduction_ceiling", "fees_10p_deduction_floor"
 ])
 year_tax_parameters: dict[int, TaxParameters] = {
@@ -121,15 +121,21 @@
     2023: TaxParameters(
         family_quotient_benefices_capping=1678,
         slices_thresholds=[10777, 27478, 78570, 168994],
         slices_rates=[0.11, 0.30, 0.41, 0.45],
         fees_10p_deduction_ceiling=13522,
         fees_10p_deduction_floor=472
     ),
-
+    2024: TaxParameters(
+        family_quotient_benefices_capping=1759,
+        slices_thresholds=[11294, 28797, 82341, 177106],
+        slices_rates=[0.11, 0.30, 0.41, 0.45],
+        fees_10p_deduction_ceiling=14171,
+        fees_10p_deduction_floor=495
+    ),
 }
 
 
 def tax_round(v: float, places: int = 0) -> float:
     # python rounds half to even (bankers rounding), we need to tax_round half up
     q = Decimal(10) ** (-places)
     return float(Decimal(v).quantize(q, rounding=ROUND_HALF_UP))
```

### Comparing `easyfrenchtax-0.0.8/src/easyfrenchtax.egg-info/PKG-INFO` & `easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
@@ -13,17 +13,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: currencyconverter
 
 # easyfrenchtax
-This project helps me understanding and projecting French taxes, especially wrt. stock, stock options, RSUs and other systems. It doesn't replace a tax advisor, I am not a lawyer, you should not rely blindly on this software for filling your tax return.
+This project helps me to understand and project French taxes, especially wrt. stock, stock options, RSUs and other systems. It doesn't replace a tax advisor, I am not a lawyer, you should not rely blindly on this software for filling your tax return.
 
 # Tax simulator
 The following are supported:
 - Progressive income tax
 - Rental income (unfurnished)
 - Family quotient (incl. capping, but excl. shared custody situations)
 - Some deductions/reductions (PER, child care, home services, charity donations)
@@ -32,15 +33,15 @@
 - Fixed interest income, incl. when tax has been partially withheld by a bank
 - Social taxes
 
 These elements of taxation have been tested against the tax simulator of the French government. I invite you to read and understand these tests, this will give you a feeling of whether you want to trust this project or not.
 
 # Stock helper
 
-This module helps filling the tax statement regarding stock acquisition or capital gain. It takes as input the stocks received (RSU, Stock Options) or bought (ESPP, direct buying) and what has been exercised/sold; it outputs the fields to fill a form 2074 and parts of 2042C. More precisely, it supports the following:
+This module helps to fill the tax statement regarding stock acquisition or capital gain. It takes as input the stocks received (RSU, Stock Options) or bought (ESPP, direct buying) and what has been exercised/sold; it outputs the fields to fill a form 2074 and parts of 2042C. More precisely, it supports the following:
 - Typical retention plans like RSU or Stock Options, direct stocks
 - Currency conversion at acquisition/exercise/buying/selling dates
 - Weighted average price ("Prix moyen pondéré" or PMP in French tax lingo)
 - Outputs fields 3VG/3VH for form 2042C, and frame 5 (512-524) + fields 903/913 for form 2074
 
 # Contact and contributions
 If you want to chat about this project, don't hesitate to shoot an email at hadrien.hamel@gmail.com. Contributions and bug reports are welcome!
```

### Comparing `easyfrenchtax-0.0.8/tests/test_capital_tax.py` & `easyfrenchtax-0.0.9/tests/test_capital_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.8/tests/test_fiscal_advantages.py` & `easyfrenchtax-0.0.9/tests/test_fiscal_advantages.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.8/tests/test_income_tax.py` & `easyfrenchtax-0.0.9/tests/test_income_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.8/tests/test_rental_tax.py` & `easyfrenchtax-0.0.9/tests/test_rental_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.8/tests/test_stock_helper.py` & `easyfrenchtax-0.0.9/tests/test_stock_helper.py`

 * *Files identical despite different names*


# Comparing `tmp/kktools-3.6.tar.gz` & `tmp/kktools-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kktools-3.6.tar", last modified: Sat Jan 27 06:40:29 2024, max compression
+gzip compressed data, was "kktools-3.7.tar", last modified: Fri May  3 18:47:48 2024, max compression
```

## Comparing `kktools-3.6.tar` & `kktools-3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-01-27 06:40:29.038818 kktools-3.6/
--rw-rw-rw-   0        0        0     1095 2022-03-13 08:04:57.000000 kktools-3.6/LICENSE
--rw-rw-rw-   0        0        0     2116 2024-01-27 06:40:29.037853 kktools-3.6/PKG-INFO
--rw-rw-rw-   0        0        0     1794 2023-10-11 08:12:37.000000 kktools-3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-01-27 06:40:29.015903 kktools-3.6/kktools/
--rw-rw-rw-   0        0        0    12827 2024-01-27 06:36:53.000000 kktools-3.6/kktools/ISO20022.py
--rw-rw-rw-   0        0        0      201 2023-10-11 07:53:06.000000 kktools-3.6/kktools/__init__.py
--rw-rw-rw-   0        0        0    10626 2023-07-30 17:16:56.000000 kktools-3.6/kktools/core.py
-drwxrwxrwx   0        0        0        0 2024-01-27 06:40:29.036859 kktools-3.6/kktools.egg-info/
--rw-rw-rw-   0        0        0     2116 2024-01-27 06:40:28.000000 kktools-3.6/kktools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-01-27 06:40:28.000000 kktools-3.6/kktools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-27 06:40:28.000000 kktools-3.6/kktools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-01-27 06:40:28.000000 kktools-3.6/kktools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-27 06:40:28.000000 kktools-3.6/kktools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-27 06:40:29.038818 kktools-3.6/setup.cfg
--rw-rw-rw-   0        0        0      570 2024-01-27 06:30:50.000000 kktools-3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:47:48.240033 kktools-3.7/
+-rw-rw-rw-   0        0        0     1095 2022-03-13 08:04:57.000000 kktools-3.7/LICENSE
+-rw-rw-rw-   0        0        0     2116 2024-05-03 18:47:48.240033 kktools-3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1794 2023-10-11 08:12:37.000000 kktools-3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 18:47:48.217867 kktools-3.7/kktools/
+-rw-rw-rw-   0        0        0    13049 2024-05-03 18:41:15.000000 kktools-3.7/kktools/ISO20022.py
+-rw-rw-rw-   0        0        0      201 2023-10-11 07:53:06.000000 kktools-3.7/kktools/__init__.py
+-rw-rw-rw-   0        0        0    10626 2023-07-30 17:16:56.000000 kktools-3.7/kktools/core.py
+drwxrwxrwx   0        0        0        0 2024-05-03 18:47:48.240033 kktools-3.7/kktools.egg-info/
+-rw-rw-rw-   0        0        0     2116 2024-05-03 18:47:47.000000 kktools-3.7/kktools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-03 18:47:48.000000 kktools-3.7/kktools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 18:47:47.000000 kktools-3.7/kktools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-05-03 18:47:47.000000 kktools-3.7/kktools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-03 18:47:47.000000 kktools-3.7/kktools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 18:47:48.240033 kktools-3.7/setup.cfg
+-rw-rw-rw-   0        0        0      570 2024-05-03 18:41:15.000000 kktools-3.7/setup.py
```

### Comparing `kktools-3.6/LICENSE` & `kktools-3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kktools-3.6/PKG-INFO` & `kktools-3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kktools
-Version: 3.6
+Version: 3.7
 Summary: Tools for finance and treasury specialists
 Home-page: https://github.com/khorevkp/KK_Tools
 Author: Konstantin Khorev
 Author-email: khorevkp@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `kktools-3.6/README.md` & `kktools-3.7/README.md`

 * *Files identical despite different names*

### Comparing `kktools-3.6/kktools/ISO20022.py` & `kktools-3.7/kktools/ISO20022.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,14 @@
         return str(file_info)
 
 
 class InvalidCamt53Exception(Exception):
     """Raised when file provided is not a valid CAMT 053 file"""
     pass
 
-
 class Camt053:
     def __init__(self, file_name):
 
         self.DEFINITIONS = {'OPBD': 'Opening Booked balance',
                             'OPAV': 'Opening available balance',
                             'CLBD': 'Closing Booked balance',
                             'CLAV': 'Closing Available balance',
@@ -278,14 +277,21 @@
             Reference = ''
 
             refs = entry.xpath('.//Ustrd')
             if len(refs) > 0:
                 for ref in refs:
                     Reference += ref.text
 
+            AddInfo = ''
+
+            refs = entry.xpath('.//AddtlNtryInf')
+            if len(refs) > 0:
+                for ref in refs:
+                    AddInfo += ref.text
+
             Amount = entry.xpath('./Amt')[0].text
             Amount = float(Amount)
             Currency = entry.xpath('./Amt/@Ccy')[0]
             CdtDbtInd = entry.xpath('./CdtDbtInd')[0].text
 
             if CdtDbtInd == 'DBIT':
                 Amount = -Amount
@@ -304,14 +310,15 @@
                 'Currency': Currency,
                 'Dr_Cr': CdtDbtInd,
                 'Debtor': Debtor,
                 'DebtorAccount': DebtorAccount,
                 'Creditor': Creditor,
                 'CreditorAccount': CreditorAccount,
                 'Reference': Reference,
+                'AddInfo': AddInfo,
                 'ValDt': ValDt,
                 'BookgDt': BookgDt
             }
             entry_dict.update(stmt_header_main)
 
             entries_list.append(entry_dict)
```

### Comparing `kktools-3.6/kktools/core.py` & `kktools-3.7/kktools/core.py`

 * *Files identical despite different names*

### Comparing `kktools-3.6/kktools.egg-info/PKG-INFO` & `kktools-3.7/kktools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kktools
-Version: 3.6
+Version: 3.7
 Summary: Tools for finance and treasury specialists
 Home-page: https://github.com/khorevkp/KK_Tools
 Author: Konstantin Khorev
 Author-email: khorevkp@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `kktools-3.6/setup.py` & `kktools-3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='kktools',
-    version='3.6',
+    version='3.7',
     author='Konstantin Khorev',
     author_email='khorevkp@gmail.com',
     description='Tools for finance and treasury specialists',
     url='https://github.com/khorevkp/KK_Tools',
     install_requires=['pandas', 'requests', 'lxml'],
     packages=['kktools'],
     long_description=long_description,
```


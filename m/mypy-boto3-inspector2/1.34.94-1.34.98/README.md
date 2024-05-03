# Comparing `tmp/mypy_boto3_inspector2-1.34.94.tar.gz` & `tmp/mypy_boto3_inspector2-1.34.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_inspector2-1.34.94.tar", last modified: Mon Apr 29 19:32:09 2024, max compression
+gzip compressed data, was "mypy_boto3_inspector2-1.34.98.tar", last modified: Fri May  3 19:32:42 2024, max compression
```

## Comparing `mypy_boto3_inspector2-1.34.94.tar` & `mypy_boto3_inspector2-1.34.98.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.006773 mypy_boto3_inspector2-1.34.94/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-04-29 19:32:09.006773 mypy_boto3_inspector2-1.34.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.006773 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48612 2024-04-29 19:31:50.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    48609 2024-04-29 19:31:50.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22435 2024-04-29 19:31:51.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    22435 2024-04-29 19:31:51.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20380 2024-04-29 19:31:51.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20364 2024-04-29 19:31:50.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    98703 2024-04-29 19:31:52.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    98703 2024-04-29 19:31:52.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.006773 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:32:09.006773 mypy_boto3_inspector2-1.34.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:42.721294 mypy_boto3_inspector2-1.34.98/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 19:32:03.000000 mypy_boto3_inspector2-1.34.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-05-03 19:32:42.721294 mypy_boto3_inspector2-1.34.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-05-03 19:32:03.000000 mypy_boto3_inspector2-1.34.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:42.721294 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-03 19:32:03.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-03 19:32:03.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-03 19:32:03.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48711 2024-05-03 19:32:04.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48708 2024-05-03 19:32:03.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-05-03 19:32:04.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-05-03 19:32:04.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20380 2024-05-03 19:32:04.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20364 2024-05-03 19:32:04.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:03.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    98786 2024-05-03 19:32:06.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98786 2024-05-03 19:32:05.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 19:32:03.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:42.721294 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-05-03 19:32:42.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-03 19:32:42.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:42.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:42.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 19:32:42.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 19:32:42.000000 mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:32:42.721294 mypy_boto3_inspector2-1.34.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-03 19:32:03.000000 mypy_boto3_inspector2-1.34.98/setup.py
```

### Comparing `mypy_boto3_inspector2-1.34.94/LICENSE` & `mypy_boto3_inspector2-1.34.98/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_inspector2-1.34.94/PKG-INFO` & `mypy_boto3_inspector2-1.34.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.34.94
-Summary: Type annotations for boto3.Inspector2 1.34.94 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.98
+Summary: Type annotations for boto3.Inspector2 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_inspector2-1.34.94/README.md` & `mypy_boto3_inspector2-1.34.98/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__init__.py` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__init__.pyi` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__main__.py` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector2 1.34.94\n"
-        "Version:         1.34.94\n"
+        "Type annotations for boto3.Inspector2 1.34.98\n"
+        "Version:         1.34.98\n"
         "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.94")
+    print("1.34.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/client.py` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AggregationTypeType,
+    CisReportFormatType,
     CisScanConfigurationsSortByType,
     CisScanResultDetailsSortByType,
     CisScanResultsAggregatedByChecksSortByType,
     CisScanResultsAggregatedByTargetResourceSortByType,
     CisSecurityLevelType,
     CisSortOrderType,
     FilterActionType,
@@ -441,15 +442,19 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#generate_presigned_url)
         """
 
     def get_cis_scan_report(
-        self, *, scanArn: str, targetAccounts: Sequence[str] = ...
+        self,
+        *,
+        scanArn: str,
+        reportFormat: CisReportFormatType = ...,
+        targetAccounts: Sequence[str] = ...,
     ) -> GetCisScanReportResponseTypeDef:
         """
         Retrieves a CIS scan report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_cis_scan_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_cis_scan_report)
         """
```

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/client.pyi` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AggregationTypeType,
+    CisReportFormatType,
     CisScanConfigurationsSortByType,
     CisScanResultDetailsSortByType,
     CisScanResultsAggregatedByChecksSortByType,
     CisScanResultsAggregatedByTargetResourceSortByType,
     CisSecurityLevelType,
     CisSortOrderType,
     FilterActionType,
@@ -438,15 +439,19 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#generate_presigned_url)
         """
 
     def get_cis_scan_report(
-        self, *, scanArn: str, targetAccounts: Sequence[str] = ...
+        self,
+        *,
+        scanArn: str,
+        reportFormat: CisReportFormatType = ...,
+        targetAccounts: Sequence[str] = ...,
     ) -> GetCisScanReportResponseTypeDef:
         """
         Retrieves a CIS scan report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_cis_scan_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_cis_scan_report)
         """
```

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/literals.py` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "AggregationResourceTypeType",
     "AggregationTypeType",
     "AmiSortByType",
     "ArchitectureType",
     "AwsEcrContainerSortByType",
     "CisFindingStatusComparisonType",
     "CisFindingStatusType",
+    "CisReportFormatType",
     "CisReportStatusType",
     "CisResultStatusComparisonType",
     "CisResultStatusType",
     "CisRuleStatusType",
     "CisScanConfigurationsSortByType",
     "CisScanResultDetailsSortByType",
     "CisScanResultsAggregatedByChecksSortByType",
@@ -154,14 +155,15 @@
     "TITLE",
 ]
 AmiSortByType = Literal["AFFECTED_INSTANCES", "ALL", "CRITICAL", "HIGH"]
 ArchitectureType = Literal["ARM64", "X86_64"]
 AwsEcrContainerSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 CisFindingStatusComparisonType = Literal["EQUALS"]
 CisFindingStatusType = Literal["FAILED", "PASSED", "SKIPPED"]
+CisReportFormatType = Literal["CSV", "PDF"]
 CisReportStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 CisResultStatusComparisonType = Literal["EQUALS"]
 CisResultStatusType = Literal["FAILED", "PASSED", "SKIPPED"]
 CisRuleStatusType = Literal[
     "ERROR", "FAILED", "INFORMATIONAL", "NOT_APPLICABLE", "NOT_EVALUATED", "PASSED", "UNKNOWN"
 ]
 CisScanConfigurationsSortByType = Literal["SCAN_CONFIGURATION_ARN", "SCAN_NAME"]
```

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/literals.pyi` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "AggregationResourceTypeType",
     "AggregationTypeType",
     "AmiSortByType",
     "ArchitectureType",
     "AwsEcrContainerSortByType",
     "CisFindingStatusComparisonType",
     "CisFindingStatusType",
+    "CisReportFormatType",
     "CisReportStatusType",
     "CisResultStatusComparisonType",
     "CisResultStatusType",
     "CisRuleStatusType",
     "CisScanConfigurationsSortByType",
     "CisScanResultDetailsSortByType",
     "CisScanResultsAggregatedByChecksSortByType",
@@ -154,14 +155,15 @@
     "TITLE",
 ]
 AmiSortByType = Literal["AFFECTED_INSTANCES", "ALL", "CRITICAL", "HIGH"]
 ArchitectureType = Literal["ARM64", "X86_64"]
 AwsEcrContainerSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 CisFindingStatusComparisonType = Literal["EQUALS"]
 CisFindingStatusType = Literal["FAILED", "PASSED", "SKIPPED"]
+CisReportFormatType = Literal["CSV", "PDF"]
 CisReportStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 CisResultStatusComparisonType = Literal["EQUALS"]
 CisResultStatusType = Literal["FAILED", "PASSED", "SKIPPED"]
 CisRuleStatusType = Literal[
     "ERROR", "FAILED", "INFORMATIONAL", "NOT_APPLICABLE", "NOT_EVALUATED", "PASSED", "UNKNOWN"
 ]
 CisScanConfigurationsSortByType = Literal["SCAN_CONFIGURATION_ARN", "SCAN_NAME"]
```

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/paginator.py` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/paginator.pyi` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/type_defs.py` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     AggregationFindingTypeType,
     AggregationResourceTypeType,
     AggregationTypeType,
     AmiSortByType,
     ArchitectureType,
     AwsEcrContainerSortByType,
     CisFindingStatusType,
+    CisReportFormatType,
     CisReportStatusType,
     CisResultStatusType,
     CisRuleStatusType,
     CisScanConfigurationsSortByType,
     CisScanResultDetailsSortByType,
     CisScanResultsAggregatedByChecksSortByType,
     CisScanResultsAggregatedByTargetResourceSortByType,
@@ -1016,14 +1017,15 @@
         "type": FreeTrialTypeType,
     },
 )
 GetCisScanReportRequestRequestTypeDef = TypedDict(
     "GetCisScanReportRequestRequestTypeDef",
     {
         "scanArn": str,
+        "reportFormat": NotRequired[CisReportFormatType],
         "targetAccounts": NotRequired[Sequence[str]],
     },
 )
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
```

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/type_defs.pyi` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     AggregationFindingTypeType,
     AggregationResourceTypeType,
     AggregationTypeType,
     AmiSortByType,
     ArchitectureType,
     AwsEcrContainerSortByType,
     CisFindingStatusType,
+    CisReportFormatType,
     CisReportStatusType,
     CisResultStatusType,
     CisRuleStatusType,
     CisScanConfigurationsSortByType,
     CisScanResultDetailsSortByType,
     CisScanResultsAggregatedByChecksSortByType,
     CisScanResultsAggregatedByTargetResourceSortByType,
@@ -1016,14 +1017,15 @@
         "type": FreeTrialTypeType,
     },
 )
 GetCisScanReportRequestRequestTypeDef = TypedDict(
     "GetCisScanReportRequestRequestTypeDef",
     {
         "scanArn": str,
+        "reportFormat": NotRequired[CisReportFormatType],
         "targetAccounts": NotRequired[Sequence[str]],
     },
 )
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
```

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/PKG-INFO` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.34.94
-Summary: Type annotations for boto3.Inspector2 1.34.94 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.98
+Summary: Type annotations for boto3.Inspector2 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/SOURCES.txt` & `mypy_boto3_inspector2-1.34.98/mypy_boto3_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_inspector2-1.34.94/setup.py` & `mypy_boto3_inspector2-1.34.98/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector2",
-    version="1.34.94",
+    version="1.34.98",
     packages=["mypy_boto3_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Inspector2 1.34.94 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.Inspector2 1.34.98 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```


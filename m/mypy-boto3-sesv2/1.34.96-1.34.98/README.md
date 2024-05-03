# Comparing `tmp/mypy_boto3_sesv2-1.34.96.tar.gz` & `tmp/mypy_boto3_sesv2-1.34.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_sesv2-1.34.96.tar", last modified: Wed May  1 19:21:17 2024, max compression
+gzip compressed data, was "mypy_boto3_sesv2-1.34.98.tar", last modified: Fri May  3 19:32:43 2024, max compression
```

## Comparing `mypy_boto3_sesv2-1.34.96.tar` & `mypy_boto3_sesv2-1.34.98.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:17.132335 mypy_boto3_sesv2-1.34.96/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-05-01 19:21:17.132335 mypy_boto3_sesv2-1.34.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:17.132335 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59825 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    59822 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    70365 2024-05-01 19:21:04.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    70365 2024-05-01 19:21:04.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:17.132335 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:21:17.132335 mypy_boto3_sesv2-1.34.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:43.545305 mypy_boto3_sesv2-1.34.98/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 19:32:28.000000 mypy_boto3_sesv2-1.34.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-05-03 19:32:43.545305 mypy_boto3_sesv2-1.34.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-05-03 19:32:28.000000 mypy_boto3_sesv2-1.34.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:43.545305 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-03 19:32:28.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-03 19:32:28.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-03 19:32:28.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59825 2024-05-03 19:32:29.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59822 2024-05-03 19:32:28.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-03 19:32:30.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-03 19:32:30.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:28.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    70440 2024-05-03 19:32:31.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70440 2024-05-03 19:32:30.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 19:32:28.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:43.545305 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-05-03 19:32:43.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-03 19:32:43.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:43.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:43.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 19:32:43.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 19:32:43.000000 mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:32:43.545305 mypy_boto3_sesv2-1.34.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-03 19:32:28.000000 mypy_boto3_sesv2-1.34.98/setup.py
```

### Comparing `mypy_boto3_sesv2-1.34.96/LICENSE` & `mypy_boto3_sesv2-1.34.98/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sesv2-1.34.96/PKG-INFO` & `mypy_boto3_sesv2-1.34.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.34.96
-Summary: Type annotations for boto3.SESV2 1.34.96 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.98
+Summary: Type annotations for boto3.SESV2 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_sesv2-1.34.96/README.md` & `mypy_boto3_sesv2-1.34.98/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/__main__.py` & `mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SESV2 1.34.96\n"
-        "Version:         1.34.96\n"
+        "Type annotations for boto3.SESV2 1.34.98\n"
+        "Version:         1.34.98\n"
         "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.96")
+    print("1.34.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/client.py` & `mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/client.pyi` & `mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/literals.py` & `mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/literals.pyi` & `mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/type_defs.py` & `mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
     "BlobTypeDef",
     "ContentTypeDef",
     "BounceTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
+    "MessageHeaderTypeDef",
     "MessageTagTypeDef",
     "CancelExportJobRequestRequestTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "ComplaintTypeDef",
     "ContactListDestinationTypeDef",
     "ContactListTypeDef",
     "TopicPreferenceTypeDef",
@@ -173,15 +174,14 @@
     "ListExportJobsRequestRequestTypeDef",
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
     "SuppressedDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "MessageHeaderTypeDef",
     "MessageInsightsFiltersOutputTypeDef",
     "MessageInsightsFiltersTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountDetailsRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
@@ -223,14 +223,15 @@
     "SendCustomVerificationEmailResponseTypeDef",
     "SendEmailResponseTypeDef",
     "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "RawMessageTypeDef",
     "BodyTypeDef",
     "SendBulkEmailResponseTypeDef",
+    "TemplateTypeDef",
     "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "EventDetailsTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
     "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
@@ -267,23 +268,23 @@
     "VdmAttributesTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
-    "TemplateTypeDef",
     "MessageInsightsDataSourceOutputTypeDef",
     "MessageInsightsDataSourceTypeDef",
     "ReplacementEmailContentTypeDef",
     "VerificationInfoTypeDef",
     "SuppressedDestinationTypeDef",
     "BatchGetMetricDataRequestRequestTypeDef",
     "ReputationOptionsUnionTypeDef",
     "MessageTypeDef",
+    "BulkEmailContentTypeDef",
     "EventDestinationTypeDef",
     "EventDestinationDefinitionTypeDef",
     "InsightsEventTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionUnionTypeDef",
@@ -293,15 +294,14 @@
     "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
     "ListContactsRequestRequestTypeDef",
-    "BulkEmailContentTypeDef",
     "ExportDataSourceOutputTypeDef",
     "ExportDataSourceTypeDef",
     "BulkEmailEntryTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
@@ -389,14 +389,21 @@
     "DestinationTypeDef",
     {
         "ToAddresses": NotRequired[Sequence[str]],
         "CcAddresses": NotRequired[Sequence[str]],
         "BccAddresses": NotRequired[Sequence[str]],
     },
 )
+MessageHeaderTypeDef = TypedDict(
+    "MessageHeaderTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
 MessageTagTypeDef = TypedDict(
     "MessageTagTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -1058,21 +1065,14 @@
 )
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
-MessageHeaderTypeDef = TypedDict(
-    "MessageHeaderTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
 MessageInsightsFiltersOutputTypeDef = TypedDict(
     "MessageInsightsFiltersOutputTypeDef",
     {
         "FromEmailAddress": NotRequired[List[str]],
         "Destination": NotRequired[List[str]],
         "Subject": NotRequired[List[str]],
         "Isp": NotRequired[List[str]],
@@ -1449,14 +1449,23 @@
 SendBulkEmailResponseTypeDef = TypedDict(
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+TemplateTypeDef = TypedDict(
+    "TemplateTypeDef",
+    {
+        "TemplateName": NotRequired[str],
+        "TemplateArn": NotRequired[str],
+        "TemplateData": NotRequired[str],
+        "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
+    },
+)
 CloudWatchDestinationOutputTypeDef = TypedDict(
     "CloudWatchDestinationOutputTypeDef",
     {
         "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 CloudWatchDestinationTypeDef = TypedDict(
@@ -1801,23 +1810,14 @@
     "ListSuppressedDestinationsResponseTypeDef",
     {
         "SuppressedDestinationSummaries": List[SuppressedDestinationSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
         "NextToken": NotRequired[str],
     },
 )
-TemplateTypeDef = TypedDict(
-    "TemplateTypeDef",
-    {
-        "TemplateName": NotRequired[str],
-        "TemplateArn": NotRequired[str],
-        "TemplateData": NotRequired[str],
-        "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
-    },
-)
 MessageInsightsDataSourceOutputTypeDef = TypedDict(
     "MessageInsightsDataSourceOutputTypeDef",
     {
         "StartDate": datetime,
         "EndDate": datetime,
         "Include": NotRequired[MessageInsightsFiltersOutputTypeDef],
         "Exclude": NotRequired[MessageInsightsFiltersOutputTypeDef],
@@ -1869,14 +1869,20 @@
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
         "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
     },
 )
+BulkEmailContentTypeDef = TypedDict(
+    "BulkEmailContentTypeDef",
+    {
+        "Template": NotRequired[TemplateTypeDef],
+    },
+)
 EventDestinationTypeDef = TypedDict(
     "EventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": List[EventTypeType],
         "Enabled": NotRequired[bool],
         "KinesisFirehoseDestination": NotRequired[KinesisFirehoseDestinationTypeDef],
@@ -2037,20 +2043,14 @@
     {
         "ContactListName": str,
         "Filter": NotRequired[ListContactsFilterTypeDef],
         "PageSize": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
-BulkEmailContentTypeDef = TypedDict(
-    "BulkEmailContentTypeDef",
-    {
-        "Template": NotRequired[TemplateTypeDef],
-    },
-)
 ExportDataSourceOutputTypeDef = TypedDict(
     "ExportDataSourceOutputTypeDef",
     {
         "MetricsDataSource": NotRequired[MetricsDataSourceOutputTypeDef],
         "MessageInsightsDataSource": NotRequired[MessageInsightsDataSourceOutputTypeDef],
     },
 )
@@ -2063,14 +2063,15 @@
 )
 BulkEmailEntryTypeDef = TypedDict(
     "BulkEmailEntryTypeDef",
     {
         "Destination": DestinationTypeDef,
         "ReplacementTags": NotRequired[Sequence[MessageTagTypeDef]],
         "ReplacementEmailContent": NotRequired[ReplacementEmailContentTypeDef],
+        "ReplacementHeaders": NotRequired[Sequence[MessageHeaderTypeDef]],
     },
 )
 GetEmailIdentityResponseTypeDef = TypedDict(
     "GetEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
```

### Comparing `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/type_defs.pyi` & `mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
     "BlobTypeDef",
     "ContentTypeDef",
     "BounceTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
+    "MessageHeaderTypeDef",
     "MessageTagTypeDef",
     "CancelExportJobRequestRequestTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "ComplaintTypeDef",
     "ContactListDestinationTypeDef",
     "ContactListTypeDef",
     "TopicPreferenceTypeDef",
@@ -173,15 +174,14 @@
     "ListExportJobsRequestRequestTypeDef",
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
     "SuppressedDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "MessageHeaderTypeDef",
     "MessageInsightsFiltersOutputTypeDef",
     "MessageInsightsFiltersTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountDetailsRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
@@ -223,14 +223,15 @@
     "SendCustomVerificationEmailResponseTypeDef",
     "SendEmailResponseTypeDef",
     "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "RawMessageTypeDef",
     "BodyTypeDef",
     "SendBulkEmailResponseTypeDef",
+    "TemplateTypeDef",
     "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "EventDetailsTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
     "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
@@ -267,23 +268,23 @@
     "VdmAttributesTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
-    "TemplateTypeDef",
     "MessageInsightsDataSourceOutputTypeDef",
     "MessageInsightsDataSourceTypeDef",
     "ReplacementEmailContentTypeDef",
     "VerificationInfoTypeDef",
     "SuppressedDestinationTypeDef",
     "BatchGetMetricDataRequestRequestTypeDef",
     "ReputationOptionsUnionTypeDef",
     "MessageTypeDef",
+    "BulkEmailContentTypeDef",
     "EventDestinationTypeDef",
     "EventDestinationDefinitionTypeDef",
     "InsightsEventTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionUnionTypeDef",
@@ -293,15 +294,14 @@
     "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
     "ListContactsRequestRequestTypeDef",
-    "BulkEmailContentTypeDef",
     "ExportDataSourceOutputTypeDef",
     "ExportDataSourceTypeDef",
     "BulkEmailEntryTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
@@ -389,14 +389,21 @@
     "DestinationTypeDef",
     {
         "ToAddresses": NotRequired[Sequence[str]],
         "CcAddresses": NotRequired[Sequence[str]],
         "BccAddresses": NotRequired[Sequence[str]],
     },
 )
+MessageHeaderTypeDef = TypedDict(
+    "MessageHeaderTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
 MessageTagTypeDef = TypedDict(
     "MessageTagTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -1058,21 +1065,14 @@
 )
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
-MessageHeaderTypeDef = TypedDict(
-    "MessageHeaderTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
 MessageInsightsFiltersOutputTypeDef = TypedDict(
     "MessageInsightsFiltersOutputTypeDef",
     {
         "FromEmailAddress": NotRequired[List[str]],
         "Destination": NotRequired[List[str]],
         "Subject": NotRequired[List[str]],
         "Isp": NotRequired[List[str]],
@@ -1449,14 +1449,23 @@
 SendBulkEmailResponseTypeDef = TypedDict(
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+TemplateTypeDef = TypedDict(
+    "TemplateTypeDef",
+    {
+        "TemplateName": NotRequired[str],
+        "TemplateArn": NotRequired[str],
+        "TemplateData": NotRequired[str],
+        "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
+    },
+)
 CloudWatchDestinationOutputTypeDef = TypedDict(
     "CloudWatchDestinationOutputTypeDef",
     {
         "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 CloudWatchDestinationTypeDef = TypedDict(
@@ -1801,23 +1810,14 @@
     "ListSuppressedDestinationsResponseTypeDef",
     {
         "SuppressedDestinationSummaries": List[SuppressedDestinationSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
         "NextToken": NotRequired[str],
     },
 )
-TemplateTypeDef = TypedDict(
-    "TemplateTypeDef",
-    {
-        "TemplateName": NotRequired[str],
-        "TemplateArn": NotRequired[str],
-        "TemplateData": NotRequired[str],
-        "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
-    },
-)
 MessageInsightsDataSourceOutputTypeDef = TypedDict(
     "MessageInsightsDataSourceOutputTypeDef",
     {
         "StartDate": datetime,
         "EndDate": datetime,
         "Include": NotRequired[MessageInsightsFiltersOutputTypeDef],
         "Exclude": NotRequired[MessageInsightsFiltersOutputTypeDef],
@@ -1869,14 +1869,20 @@
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
         "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
     },
 )
+BulkEmailContentTypeDef = TypedDict(
+    "BulkEmailContentTypeDef",
+    {
+        "Template": NotRequired[TemplateTypeDef],
+    },
+)
 EventDestinationTypeDef = TypedDict(
     "EventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": List[EventTypeType],
         "Enabled": NotRequired[bool],
         "KinesisFirehoseDestination": NotRequired[KinesisFirehoseDestinationTypeDef],
@@ -2037,20 +2043,14 @@
     {
         "ContactListName": str,
         "Filter": NotRequired[ListContactsFilterTypeDef],
         "PageSize": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
-BulkEmailContentTypeDef = TypedDict(
-    "BulkEmailContentTypeDef",
-    {
-        "Template": NotRequired[TemplateTypeDef],
-    },
-)
 ExportDataSourceOutputTypeDef = TypedDict(
     "ExportDataSourceOutputTypeDef",
     {
         "MetricsDataSource": NotRequired[MetricsDataSourceOutputTypeDef],
         "MessageInsightsDataSource": NotRequired[MessageInsightsDataSourceOutputTypeDef],
     },
 )
@@ -2063,14 +2063,15 @@
 )
 BulkEmailEntryTypeDef = TypedDict(
     "BulkEmailEntryTypeDef",
     {
         "Destination": DestinationTypeDef,
         "ReplacementTags": NotRequired[Sequence[MessageTagTypeDef]],
         "ReplacementEmailContent": NotRequired[ReplacementEmailContentTypeDef],
+        "ReplacementHeaders": NotRequired[Sequence[MessageHeaderTypeDef]],
     },
 )
 GetEmailIdentityResponseTypeDef = TypedDict(
     "GetEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
```

### Comparing `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/PKG-INFO` & `mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.34.96
-Summary: Type annotations for boto3.SESV2 1.34.96 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.98
+Summary: Type annotations for boto3.SESV2 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/SOURCES.txt` & `mypy_boto3_sesv2-1.34.98/mypy_boto3_sesv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sesv2-1.34.96/setup.py` & `mypy_boto3_sesv2-1.34.98/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sesv2",
-    version="1.34.96",
+    version="1.34.98",
     packages=["mypy_boto3_sesv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.SESV2 1.34.96 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.SESV2 1.34.98 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```


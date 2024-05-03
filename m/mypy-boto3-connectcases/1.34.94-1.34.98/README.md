# Comparing `tmp/mypy_boto3_connectcases-1.34.94.tar.gz` & `tmp/mypy_boto3_connectcases-1.34.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_connectcases-1.34.94.tar", last modified: Mon Apr 29 19:32:08 2024, max compression
+gzip compressed data, was "mypy_boto3_connectcases-1.34.98.tar", last modified: Fri May  3 19:32:42 2024, max compression
```

## Comparing `mypy_boto3_connectcases-1.34.94.tar` & `mypy_boto3_connectcases-1.34.98.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:08.658774 mypy_boto3_connectcases-1.34.94/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-04-29 19:32:08.658774 mypy_boto3_connectcases-1.34.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11547 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:08.658774 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24124 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24121 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-29 19:31:48.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-29 19:31:48.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30101 2024-04-29 19:31:49.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30101 2024-04-29 19:31:48.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:08.658774 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:32:08.658774 mypy_boto3_connectcases-1.34.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:42.041286 mypy_boto3_connectcases-1.34.98/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 19:31:58.000000 mypy_boto3_connectcases-1.34.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-05-03 19:32:42.041286 mypy_boto3_connectcases-1.34.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11547 2024-05-03 19:31:58.000000 mypy_boto3_connectcases-1.34.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:42.041286 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-03 19:31:58.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-03 19:31:58.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-03 19:31:58.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24124 2024-05-03 19:31:59.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24121 2024-05-03 19:31:58.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-05-03 19:31:59.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-05-03 19:31:59.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-03 19:31:59.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-03 19:31:59.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:31:58.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30503 2024-05-03 19:31:59.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30503 2024-05-03 19:31:59.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 19:31:58.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:32:42.041286 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-05-03 19:32:42.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-03 19:32:42.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:42.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:32:42.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 19:32:42.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 19:32:42.000000 mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:32:42.041286 mypy_boto3_connectcases-1.34.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-03 19:31:58.000000 mypy_boto3_connectcases-1.34.98/setup.py
```

### Comparing `mypy_boto3_connectcases-1.34.94/LICENSE` & `mypy_boto3_connectcases-1.34.98/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_connectcases-1.34.94/PKG-INFO` & `mypy_boto3_connectcases-1.34.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.34.94
-Summary: Type annotations for boto3.ConnectCases 1.34.94 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.98
+Summary: Type annotations for boto3.ConnectCases 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_connectcases-1.34.94/README.md` & `mypy_boto3_connectcases-1.34.98/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__init__.py` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__init__.pyi` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__main__.py` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCases 1.34.94\n"
-        "Version:         1.34.94\n"
+        "Type annotations for boto3.ConnectCases 1.34.98\n"
+        "Version:         1.34.98\n"
         "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\n"
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

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/client.py` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/client.pyi` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/literals.py` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 AuditEventTypeType = Literal["Case.Created", "Case.Updated", "RelatedItem.Created"]
 CommentBodyTextTypeType = Literal["Text/Plain"]
 DomainStatusType = Literal["Active", "CreationFailed", "CreationInProgress"]
 FieldNamespaceType = Literal["Custom", "System"]
 FieldTypeType = Literal["Boolean", "DateTime", "Number", "SingleSelect", "Text", "Url", "User"]
 OrderType = Literal["Asc", "Desc"]
-RelatedItemTypeType = Literal["Comment", "Contact"]
+RelatedItemTypeType = Literal["Comment", "Contact", "File"]
 SearchCasesPaginatorName = Literal["search_cases"]
 SearchRelatedItemsPaginatorName = Literal["search_related_items"]
 TemplateStatusType = Literal["Active", "Inactive"]
 ConnectCasesServiceName = Literal["connectcases"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
```

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/literals.pyi` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 AuditEventTypeType = Literal["Case.Created", "Case.Updated", "RelatedItem.Created"]
 CommentBodyTextTypeType = Literal["Text/Plain"]
 DomainStatusType = Literal["Active", "CreationFailed", "CreationInProgress"]
 FieldNamespaceType = Literal["Custom", "System"]
 FieldTypeType = Literal["Boolean", "DateTime", "Number", "SingleSelect", "Text", "Url", "User"]
 OrderType = Literal["Asc", "Desc"]
-RelatedItemTypeType = Literal["Comment", "Contact"]
+RelatedItemTypeType = Literal["Comment", "Contact", "File"]
 SearchCasesPaginatorName = Literal["search_cases"]
 SearchRelatedItemsPaginatorName = Literal["search_related_items"]
 TemplateStatusType = Literal["Active", "Inactive"]
 ConnectCasesServiceName = Literal["connectcases"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
```

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/paginator.py` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/paginator.pyi` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/type_defs.py` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     "DomainSummaryTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionExtraOutputTypeDef",
     "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
+    "FileContentTypeDef",
+    "FileFilterTypeDef",
     "GetCaseAuditEventsRequestRequestTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
@@ -103,53 +105,53 @@
     "EmptyResponseMetadataTypeDef",
     "GetDomainResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
     "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
     "ListCasesForContactResponseTypeDef",
-    "RelatedItemContentTypeDef",
-    "RelatedItemTypeFilterTypeDef",
-    "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
     "ListFieldsResponseTypeDef",
     "FieldValueExtraOutputTypeDef",
     "FieldValueOutputTypeDef",
     "FieldValueTypeDef",
+    "RelatedItemContentTypeDef",
+    "RelatedItemInputContentTypeDef",
+    "RelatedItemTypeFilterTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "AuditEventTypeDef",
     "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
-    "SearchRelatedItemsResponseItemTypeDef",
-    "SearchRelatedItemsRequestRequestTypeDef",
-    "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
-    "CreateRelatedItemRequestRequestTypeDef",
     "SectionOutputTypeDef",
     "SectionTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
     "FieldFilterTypeDef",
     "FieldValueExtraUnionTypeDef",
+    "SearchRelatedItemsResponseItemTypeDef",
+    "CreateRelatedItemRequestRequestTypeDef",
+    "SearchRelatedItemsRequestRequestTypeDef",
+    "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "GetCaseAuditEventsResponseTypeDef",
     "EventBridgeConfigurationOutputTypeDef",
     "EventBridgeConfigurationTypeDef",
-    "SearchRelatedItemsResponseTypeDef",
     "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
     "SearchCasesResponseTypeDef",
     "CaseFilterTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "UpdateCaseRequestRequestTypeDef",
+    "SearchRelatedItemsResponseTypeDef",
     "GetCaseEventConfigurationResponseTypeDef",
     "EventBridgeConfigurationUnionTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
     "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
     "LayoutContentOutputTypeDef",
@@ -376,14 +378,26 @@
         "booleanValue": NotRequired[bool],
         "doubleValue": NotRequired[float],
         "emptyValue": NotRequired[Mapping[str, Any]],
         "stringValue": NotRequired[str],
         "userArnValue": NotRequired[str],
     },
 )
+FileContentTypeDef = TypedDict(
+    "FileContentTypeDef",
+    {
+        "fileArn": str,
+    },
+)
+FileFilterTypeDef = TypedDict(
+    "FileFilterTypeDef",
+    {
+        "fileArn": NotRequired[str],
+    },
+)
 GetCaseAuditEventsRequestRequestTypeDef = TypedDict(
     "GetCaseAuditEventsRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
@@ -679,35 +693,14 @@
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-RelatedItemContentTypeDef = TypedDict(
-    "RelatedItemContentTypeDef",
-    {
-        "comment": NotRequired[CommentContentTypeDef],
-        "contact": NotRequired[ContactContentTypeDef],
-    },
-)
-RelatedItemTypeFilterTypeDef = TypedDict(
-    "RelatedItemTypeFilterTypeDef",
-    {
-        "comment": NotRequired[Mapping[str, Any]],
-        "contact": NotRequired[ContactFilterTypeDef],
-    },
-)
-RelatedItemInputContentTypeDef = TypedDict(
-    "RelatedItemInputContentTypeDef",
-    {
-        "comment": NotRequired[CommentContentTypeDef],
-        "contact": NotRequired[ContactTypeDef],
-    },
-)
 CreateTemplateRequestRequestTypeDef = TypedDict(
     "CreateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "name": str,
         "description": NotRequired[str],
         "layoutConfiguration": NotRequired[LayoutConfigurationTypeDef],
@@ -791,14 +784,38 @@
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "id": str,
         "value": FieldValueUnionTypeDef,
     },
 )
+RelatedItemContentTypeDef = TypedDict(
+    "RelatedItemContentTypeDef",
+    {
+        "comment": NotRequired[CommentContentTypeDef],
+        "contact": NotRequired[ContactContentTypeDef],
+        "file": NotRequired[FileContentTypeDef],
+    },
+)
+RelatedItemInputContentTypeDef = TypedDict(
+    "RelatedItemInputContentTypeDef",
+    {
+        "comment": NotRequired[CommentContentTypeDef],
+        "contact": NotRequired[ContactTypeDef],
+        "file": NotRequired[FileContentTypeDef],
+    },
+)
+RelatedItemTypeFilterTypeDef = TypedDict(
+    "RelatedItemTypeFilterTypeDef",
+    {
+        "comment": NotRequired[Mapping[str, Any]],
+        "contact": NotRequired[ContactFilterTypeDef],
+        "file": NotRequired[FileFilterTypeDef],
+    },
+)
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -844,54 +861,14 @@
 EventIncludedDataTypeDef = TypedDict(
     "EventIncludedDataTypeDef",
     {
         "caseData": NotRequired[CaseEventIncludedDataTypeDef],
         "relatedItemData": NotRequired[RelatedItemEventIncludedDataTypeDef],
     },
 )
-SearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "SearchRelatedItemsResponseItemTypeDef",
-    {
-        "associationTime": datetime,
-        "content": RelatedItemContentTypeDef,
-        "relatedItemId": str,
-        "type": RelatedItemTypeType,
-        "performedBy": NotRequired[UserUnionTypeDef],
-        "tags": NotRequired[Dict[str, str]],
-    },
-)
-SearchRelatedItemsRequestRequestTypeDef = TypedDict(
-    "SearchRelatedItemsRequestRequestTypeDef",
-    {
-        "caseId": str,
-        "domainId": str,
-        "filters": NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-    },
-)
-SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
-    "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
-    {
-        "caseId": str,
-        "domainId": str,
-        "filters": NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],
-        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
-    },
-)
-CreateRelatedItemRequestRequestTypeDef = TypedDict(
-    "CreateRelatedItemRequestRequestTypeDef",
-    {
-        "caseId": str,
-        "content": RelatedItemInputContentTypeDef,
-        "domainId": str,
-        "type": RelatedItemTypeType,
-        "performedBy": NotRequired[UserUnionTypeDef],
-    },
-)
 SectionOutputTypeDef = TypedDict(
     "SectionOutputTypeDef",
     {
         "fieldGroup": NotRequired[FieldGroupOutputTypeDef],
     },
 )
 SectionTypeDef = TypedDict(
@@ -927,14 +904,54 @@
         "greaterThan": NotRequired[FieldValueTypeDef],
         "greaterThanOrEqualTo": NotRequired[FieldValueTypeDef],
         "lessThan": NotRequired[FieldValueTypeDef],
         "lessThanOrEqualTo": NotRequired[FieldValueTypeDef],
     },
 )
 FieldValueExtraUnionTypeDef = Union[FieldValueTypeDef, FieldValueExtraOutputTypeDef]
+SearchRelatedItemsResponseItemTypeDef = TypedDict(
+    "SearchRelatedItemsResponseItemTypeDef",
+    {
+        "associationTime": datetime,
+        "content": RelatedItemContentTypeDef,
+        "relatedItemId": str,
+        "type": RelatedItemTypeType,
+        "performedBy": NotRequired[UserUnionTypeDef],
+        "tags": NotRequired[Dict[str, str]],
+    },
+)
+CreateRelatedItemRequestRequestTypeDef = TypedDict(
+    "CreateRelatedItemRequestRequestTypeDef",
+    {
+        "caseId": str,
+        "content": RelatedItemInputContentTypeDef,
+        "domainId": str,
+        "type": RelatedItemTypeType,
+        "performedBy": NotRequired[UserUnionTypeDef],
+    },
+)
+SearchRelatedItemsRequestRequestTypeDef = TypedDict(
+    "SearchRelatedItemsRequestRequestTypeDef",
+    {
+        "caseId": str,
+        "domainId": str,
+        "filters": NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
+SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
+    "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
+    {
+        "caseId": str,
+        "domainId": str,
+        "filters": NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 GetCaseAuditEventsResponseTypeDef = TypedDict(
     "GetCaseAuditEventsResponseTypeDef",
     {
         "auditEvents": List[AuditEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -949,22 +966,14 @@
 EventBridgeConfigurationTypeDef = TypedDict(
     "EventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
         "includedData": NotRequired[EventIncludedDataTypeDef],
     },
 )
-SearchRelatedItemsResponseTypeDef = TypedDict(
-    "SearchRelatedItemsResponseTypeDef",
-    {
-        "nextToken": str,
-        "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 LayoutSectionsOutputTypeDef = TypedDict(
     "LayoutSectionsOutputTypeDef",
     {
         "sections": NotRequired[List[SectionOutputTypeDef]],
     },
 )
 LayoutSectionsTypeDef = TypedDict(
@@ -1005,14 +1014,22 @@
     {
         "caseId": str,
         "domainId": str,
         "fields": Sequence[FieldValueExtraUnionTypeDef],
         "performedBy": NotRequired[UserUnionTypeDef],
     },
 )
+SearchRelatedItemsResponseTypeDef = TypedDict(
+    "SearchRelatedItemsResponseTypeDef",
+    {
+        "nextToken": str,
+        "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
         "eventBridge": EventBridgeConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/type_defs.pyi` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     "DomainSummaryTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionExtraOutputTypeDef",
     "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
+    "FileContentTypeDef",
+    "FileFilterTypeDef",
     "GetCaseAuditEventsRequestRequestTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
@@ -103,53 +105,53 @@
     "EmptyResponseMetadataTypeDef",
     "GetDomainResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
     "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
     "ListCasesForContactResponseTypeDef",
-    "RelatedItemContentTypeDef",
-    "RelatedItemTypeFilterTypeDef",
-    "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
     "ListFieldsResponseTypeDef",
     "FieldValueExtraOutputTypeDef",
     "FieldValueOutputTypeDef",
     "FieldValueTypeDef",
+    "RelatedItemContentTypeDef",
+    "RelatedItemInputContentTypeDef",
+    "RelatedItemTypeFilterTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "AuditEventTypeDef",
     "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
-    "SearchRelatedItemsResponseItemTypeDef",
-    "SearchRelatedItemsRequestRequestTypeDef",
-    "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
-    "CreateRelatedItemRequestRequestTypeDef",
     "SectionOutputTypeDef",
     "SectionTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
     "FieldFilterTypeDef",
     "FieldValueExtraUnionTypeDef",
+    "SearchRelatedItemsResponseItemTypeDef",
+    "CreateRelatedItemRequestRequestTypeDef",
+    "SearchRelatedItemsRequestRequestTypeDef",
+    "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "GetCaseAuditEventsResponseTypeDef",
     "EventBridgeConfigurationOutputTypeDef",
     "EventBridgeConfigurationTypeDef",
-    "SearchRelatedItemsResponseTypeDef",
     "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
     "SearchCasesResponseTypeDef",
     "CaseFilterTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "UpdateCaseRequestRequestTypeDef",
+    "SearchRelatedItemsResponseTypeDef",
     "GetCaseEventConfigurationResponseTypeDef",
     "EventBridgeConfigurationUnionTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
     "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
     "LayoutContentOutputTypeDef",
@@ -376,14 +378,26 @@
         "booleanValue": NotRequired[bool],
         "doubleValue": NotRequired[float],
         "emptyValue": NotRequired[Mapping[str, Any]],
         "stringValue": NotRequired[str],
         "userArnValue": NotRequired[str],
     },
 )
+FileContentTypeDef = TypedDict(
+    "FileContentTypeDef",
+    {
+        "fileArn": str,
+    },
+)
+FileFilterTypeDef = TypedDict(
+    "FileFilterTypeDef",
+    {
+        "fileArn": NotRequired[str],
+    },
+)
 GetCaseAuditEventsRequestRequestTypeDef = TypedDict(
     "GetCaseAuditEventsRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
@@ -679,35 +693,14 @@
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-RelatedItemContentTypeDef = TypedDict(
-    "RelatedItemContentTypeDef",
-    {
-        "comment": NotRequired[CommentContentTypeDef],
-        "contact": NotRequired[ContactContentTypeDef],
-    },
-)
-RelatedItemTypeFilterTypeDef = TypedDict(
-    "RelatedItemTypeFilterTypeDef",
-    {
-        "comment": NotRequired[Mapping[str, Any]],
-        "contact": NotRequired[ContactFilterTypeDef],
-    },
-)
-RelatedItemInputContentTypeDef = TypedDict(
-    "RelatedItemInputContentTypeDef",
-    {
-        "comment": NotRequired[CommentContentTypeDef],
-        "contact": NotRequired[ContactTypeDef],
-    },
-)
 CreateTemplateRequestRequestTypeDef = TypedDict(
     "CreateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "name": str,
         "description": NotRequired[str],
         "layoutConfiguration": NotRequired[LayoutConfigurationTypeDef],
@@ -791,14 +784,38 @@
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "id": str,
         "value": FieldValueUnionTypeDef,
     },
 )
+RelatedItemContentTypeDef = TypedDict(
+    "RelatedItemContentTypeDef",
+    {
+        "comment": NotRequired[CommentContentTypeDef],
+        "contact": NotRequired[ContactContentTypeDef],
+        "file": NotRequired[FileContentTypeDef],
+    },
+)
+RelatedItemInputContentTypeDef = TypedDict(
+    "RelatedItemInputContentTypeDef",
+    {
+        "comment": NotRequired[CommentContentTypeDef],
+        "contact": NotRequired[ContactTypeDef],
+        "file": NotRequired[FileContentTypeDef],
+    },
+)
+RelatedItemTypeFilterTypeDef = TypedDict(
+    "RelatedItemTypeFilterTypeDef",
+    {
+        "comment": NotRequired[Mapping[str, Any]],
+        "contact": NotRequired[ContactFilterTypeDef],
+        "file": NotRequired[FileFilterTypeDef],
+    },
+)
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -844,54 +861,14 @@
 EventIncludedDataTypeDef = TypedDict(
     "EventIncludedDataTypeDef",
     {
         "caseData": NotRequired[CaseEventIncludedDataTypeDef],
         "relatedItemData": NotRequired[RelatedItemEventIncludedDataTypeDef],
     },
 )
-SearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "SearchRelatedItemsResponseItemTypeDef",
-    {
-        "associationTime": datetime,
-        "content": RelatedItemContentTypeDef,
-        "relatedItemId": str,
-        "type": RelatedItemTypeType,
-        "performedBy": NotRequired[UserUnionTypeDef],
-        "tags": NotRequired[Dict[str, str]],
-    },
-)
-SearchRelatedItemsRequestRequestTypeDef = TypedDict(
-    "SearchRelatedItemsRequestRequestTypeDef",
-    {
-        "caseId": str,
-        "domainId": str,
-        "filters": NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-    },
-)
-SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
-    "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
-    {
-        "caseId": str,
-        "domainId": str,
-        "filters": NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],
-        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
-    },
-)
-CreateRelatedItemRequestRequestTypeDef = TypedDict(
-    "CreateRelatedItemRequestRequestTypeDef",
-    {
-        "caseId": str,
-        "content": RelatedItemInputContentTypeDef,
-        "domainId": str,
-        "type": RelatedItemTypeType,
-        "performedBy": NotRequired[UserUnionTypeDef],
-    },
-)
 SectionOutputTypeDef = TypedDict(
     "SectionOutputTypeDef",
     {
         "fieldGroup": NotRequired[FieldGroupOutputTypeDef],
     },
 )
 SectionTypeDef = TypedDict(
@@ -927,14 +904,54 @@
         "greaterThan": NotRequired[FieldValueTypeDef],
         "greaterThanOrEqualTo": NotRequired[FieldValueTypeDef],
         "lessThan": NotRequired[FieldValueTypeDef],
         "lessThanOrEqualTo": NotRequired[FieldValueTypeDef],
     },
 )
 FieldValueExtraUnionTypeDef = Union[FieldValueTypeDef, FieldValueExtraOutputTypeDef]
+SearchRelatedItemsResponseItemTypeDef = TypedDict(
+    "SearchRelatedItemsResponseItemTypeDef",
+    {
+        "associationTime": datetime,
+        "content": RelatedItemContentTypeDef,
+        "relatedItemId": str,
+        "type": RelatedItemTypeType,
+        "performedBy": NotRequired[UserUnionTypeDef],
+        "tags": NotRequired[Dict[str, str]],
+    },
+)
+CreateRelatedItemRequestRequestTypeDef = TypedDict(
+    "CreateRelatedItemRequestRequestTypeDef",
+    {
+        "caseId": str,
+        "content": RelatedItemInputContentTypeDef,
+        "domainId": str,
+        "type": RelatedItemTypeType,
+        "performedBy": NotRequired[UserUnionTypeDef],
+    },
+)
+SearchRelatedItemsRequestRequestTypeDef = TypedDict(
+    "SearchRelatedItemsRequestRequestTypeDef",
+    {
+        "caseId": str,
+        "domainId": str,
+        "filters": NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
+SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
+    "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
+    {
+        "caseId": str,
+        "domainId": str,
+        "filters": NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 GetCaseAuditEventsResponseTypeDef = TypedDict(
     "GetCaseAuditEventsResponseTypeDef",
     {
         "auditEvents": List[AuditEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -949,22 +966,14 @@
 EventBridgeConfigurationTypeDef = TypedDict(
     "EventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
         "includedData": NotRequired[EventIncludedDataTypeDef],
     },
 )
-SearchRelatedItemsResponseTypeDef = TypedDict(
-    "SearchRelatedItemsResponseTypeDef",
-    {
-        "nextToken": str,
-        "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 LayoutSectionsOutputTypeDef = TypedDict(
     "LayoutSectionsOutputTypeDef",
     {
         "sections": NotRequired[List[SectionOutputTypeDef]],
     },
 )
 LayoutSectionsTypeDef = TypedDict(
@@ -1005,14 +1014,22 @@
     {
         "caseId": str,
         "domainId": str,
         "fields": Sequence[FieldValueExtraUnionTypeDef],
         "performedBy": NotRequired[UserUnionTypeDef],
     },
 )
+SearchRelatedItemsResponseTypeDef = TypedDict(
+    "SearchRelatedItemsResponseTypeDef",
+    {
+        "nextToken": str,
+        "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
         "eventBridge": EventBridgeConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/PKG-INFO` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.34.94
-Summary: Type annotations for boto3.ConnectCases 1.34.94 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.98
+Summary: Type annotations for boto3.ConnectCases 1.34.98 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.34.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/SOURCES.txt` & `mypy_boto3_connectcases-1.34.98/mypy_boto3_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_connectcases-1.34.94/setup.py` & `mypy_boto3_connectcases-1.34.98/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcases",
-    version="1.34.94",
+    version="1.34.98",
     packages=["mypy_boto3_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.ConnectCases 1.34.94 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.ConnectCases 1.34.98 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

